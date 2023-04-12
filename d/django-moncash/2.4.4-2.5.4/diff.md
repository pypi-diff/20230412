# Comparing `tmp/django_moncash-2.4.4.tar.gz` & `tmp/django_moncash-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_moncash-2.4.4.tar", last modified: Sun Apr  9 15:06:57 2023, max compression
+gzip compressed data, was "django_moncash-2.5.4.tar", last modified: Wed Apr 12 13:25:04 2023, max compression
```

## Comparing `django_moncash-2.4.4.tar` & `django_moncash-2.5.4.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-09 15:06:57.426357 django_moncash-2.4.4/
--rw-r--r--   0 macbook    (501) staff       (20)    35149 2023-04-06 01:43:10.000000 django_moncash-2.4.4/LICENSE
--rw-r--r--   0 macbook    (501) staff       (20)    49325 2023-04-09 15:06:57.426581 django_moncash-2.4.4/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)     8192 2023-04-09 15:05:54.000000 django_moncash-2.4.4/README.md
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-09 15:06:57.424220 django_moncash-2.4.4/django_moncash/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-06 01:44:10.000000 django_moncash-2.4.4/django_moncash/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      298 2023-04-07 14:53:44.000000 django_moncash-2.4.4/django_moncash/_utils.py
--rw-r--r--   0 macbook    (501) staff       (20)      722 2023-04-07 15:50:36.000000 django_moncash-2.4.4/django_moncash/admin.py
--rw-r--r--   0 macbook    (501) staff       (20)      159 2023-04-06 01:44:10.000000 django_moncash-2.4.4/django_moncash/apps.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-09 15:06:57.426215 django_moncash-2.4.4/django_moncash/migrations/
--rw-r--r--   0 macbook    (501) staff       (20)     1466 2023-04-07 15:39:31.000000 django_moncash-2.4.4/django_moncash/migrations/0001_initial.py
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-06 01:44:10.000000 django_moncash-2.4.4/django_moncash/migrations/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1088 2023-04-07 15:37:08.000000 django_moncash-2.4.4/django_moncash/models.py
--rw-r--r--   0 macbook    (501) staff       (20)       60 2023-04-06 01:44:10.000000 django_moncash-2.4.4/django_moncash/tests.py
--rw-r--r--   0 macbook    (501) staff       (20)      148 2023-04-06 18:01:13.000000 django_moncash-2.4.4/django_moncash/urls.py
--rw-r--r--   0 macbook    (501) staff       (20)     2526 2023-04-08 04:00:18.000000 django_moncash-2.4.4/django_moncash/utils.py
--rw-r--r--   0 macbook    (501) staff       (20)      564 2023-04-08 03:20:24.000000 django_moncash-2.4.4/django_moncash/views.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-09 15:06:57.425658 django_moncash-2.4.4/django_moncash.egg-info/
--rw-r--r--   0 macbook    (501) staff       (20)    49325 2023-04-09 15:06:57.000000 django_moncash-2.4.4/django_moncash.egg-info/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)      539 2023-04-09 15:06:57.000000 django_moncash-2.4.4/django_moncash.egg-info/SOURCES.txt
--rw-r--r--   0 macbook    (501) staff       (20)        1 2023-04-09 15:06:57.000000 django_moncash-2.4.4/django_moncash.egg-info/dependency_links.txt
--rw-r--r--   0 macbook    (501) staff       (20)       51 2023-04-09 15:06:57.000000 django_moncash-2.4.4/django_moncash.egg-info/requires.txt
--rw-r--r--   0 macbook    (501) staff       (20)       15 2023-04-09 15:06:57.000000 django_moncash-2.4.4/django_moncash.egg-info/top_level.txt
--rw-r--r--   0 macbook    (501) staff       (20)      809 2023-04-09 15:06:41.000000 django_moncash-2.4.4/pyproject.toml
--rw-r--r--   0 macbook    (501) staff       (20)      904 2023-04-09 15:06:57.427018 django_moncash-2.4.4/setup.cfg
--rw-r--r--   0 macbook    (501) staff       (20)       96 2023-04-08 01:26:12.000000 django_moncash-2.4.4/setup.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-12 13:25:04.958658 django_moncash-2.5.4/
+-rw-r--r--   0 macbook    (501) staff       (20)    35149 2023-04-06 01:43:10.000000 django_moncash-2.5.4/LICENSE
+-rw-r--r--   0 macbook    (501) staff       (20)    49325 2023-04-12 13:25:04.958886 django_moncash-2.5.4/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)     8192 2023-04-09 15:05:54.000000 django_moncash-2.5.4/README.md
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-12 13:25:04.956313 django_moncash-2.5.4/django_moncash/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-06 01:44:10.000000 django_moncash-2.5.4/django_moncash/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      298 2023-04-07 14:53:44.000000 django_moncash-2.5.4/django_moncash/_utils.py
+-rw-r--r--   0 macbook    (501) staff       (20)      722 2023-04-07 15:50:36.000000 django_moncash-2.5.4/django_moncash/admin.py
+-rw-r--r--   0 macbook    (501) staff       (20)      159 2023-04-06 01:44:10.000000 django_moncash-2.5.4/django_moncash/apps.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-12 13:25:04.958496 django_moncash-2.5.4/django_moncash/migrations/
+-rw-r--r--   0 macbook    (501) staff       (20)     1466 2023-04-07 15:39:31.000000 django_moncash-2.5.4/django_moncash/migrations/0001_initial.py
+-rw-r--r--   0 macbook    (501) staff       (20)      636 2023-04-12 13:09:41.000000 django_moncash-2.5.4/django_moncash/migrations/0002_alter_transaction_user.py
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-06 01:44:10.000000 django_moncash-2.5.4/django_moncash/migrations/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1132 2023-04-12 13:03:32.000000 django_moncash-2.5.4/django_moncash/models.py
+-rw-r--r--   0 macbook    (501) staff       (20)       60 2023-04-06 01:44:10.000000 django_moncash-2.5.4/django_moncash/tests.py
+-rw-r--r--   0 macbook    (501) staff       (20)      148 2023-04-06 18:01:13.000000 django_moncash-2.5.4/django_moncash/urls.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2526 2023-04-08 04:00:18.000000 django_moncash-2.5.4/django_moncash/utils.py
+-rw-r--r--   0 macbook    (501) staff       (20)      564 2023-04-08 03:20:24.000000 django_moncash-2.5.4/django_moncash/views.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-12 13:25:04.957612 django_moncash-2.5.4/django_moncash.egg-info/
+-rw-r--r--   0 macbook    (501) staff       (20)    49325 2023-04-12 13:25:04.000000 django_moncash-2.5.4/django_moncash.egg-info/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)      596 2023-04-12 13:25:04.000000 django_moncash-2.5.4/django_moncash.egg-info/SOURCES.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        1 2023-04-12 13:25:04.000000 django_moncash-2.5.4/django_moncash.egg-info/dependency_links.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       51 2023-04-12 13:25:04.000000 django_moncash-2.5.4/django_moncash.egg-info/requires.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       15 2023-04-12 13:25:04.000000 django_moncash-2.5.4/django_moncash.egg-info/top_level.txt
+-rw-r--r--   0 macbook    (501) staff       (20)      809 2023-04-12 13:19:59.000000 django_moncash-2.5.4/pyproject.toml
+-rw-r--r--   0 macbook    (501) staff       (20)      904 2023-04-12 13:25:04.959308 django_moncash-2.5.4/setup.cfg
+-rw-r--r--   0 macbook    (501) staff       (20)       96 2023-04-08 01:26:12.000000 django_moncash-2.5.4/setup.py
```

### Comparing `django_moncash-2.4.4/LICENSE` & `django_moncash-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_moncash-2.4.4/PKG-INFO` & `django_moncash-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_moncash
-Version: 2.4.4
+Version: 2.5.4
 Summary: Installable django moncash
 Home-page: https://github.com/undisplay/django_moncash
 Author-email: Freedy Meritus <meritusfreedy@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `django_moncash-2.4.4/README.md` & `django_moncash-2.5.4/README.md`

 * *Files identical despite different names*

### Comparing `django_moncash-2.4.4/django_moncash/admin.py` & `django_moncash-2.5.4/django_moncash/admin.py`

 * *Files identical despite different names*

### Comparing `django_moncash-2.4.4/django_moncash/migrations/0001_initial.py` & `django_moncash-2.5.4/django_moncash/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_moncash-2.4.4/django_moncash/models.py` & `django_moncash-2.5.4/django_moncash/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,15 +16,16 @@
         CONSUME = 'CONSUME', _("Consume")
 
 
     user = models.ForeignKey(
         User,
         on_delete=models.SET_NULL,
         null=True,
-        blank=True
+        blank=True,
+        related_name='moncash_transaction'
     )
 
     order_id = models.CharField(_("Order id"), max_length=50,default=uuid.uuid4,unique=True, editable=False)
     amount   = models.DecimalField(_("Amount"), max_digits=11, decimal_places=2,blank=False,null=False)
     status = models.CharField(_('Status'),max_length=25,choices=Status.choices,default=Status.PENDING,blank=False)
 
     return_url = models.TextField(_("Return URL"),blank=False,null=False)
```

### Comparing `django_moncash-2.4.4/django_moncash/utils.py` & `django_moncash-2.5.4/django_moncash/utils.py`

 * *Files identical despite different names*

### Comparing `django_moncash-2.4.4/django_moncash/views.py` & `django_moncash-2.5.4/django_moncash/views.py`

 * *Files identical despite different names*

### Comparing `django_moncash-2.4.4/django_moncash.egg-info/PKG-INFO` & `django_moncash-2.5.4/django_moncash.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-moncash
-Version: 2.4.4
+Version: 2.5.4
 Summary: Installable django moncash
 Home-page: https://github.com/undisplay/django_moncash
 Author-email: Freedy Meritus <meritusfreedy@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `django_moncash-2.4.4/pyproject.toml` & `django_moncash-2.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django_moncash"
-version = "2.4.4"
+version = "2.5.4"
 description = "Installable django moncash"
 readme = "README.md"
 authors = [{ name = "Freedy Meritus", email = "meritusfreedy@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
```

### Comparing `django_moncash-2.4.4/setup.cfg` & `django_moncash-2.5.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django_moncash
-version = 2.4.4
+version = 2.5.4
 description = Installable django moncash
 long_description = file:README.md
 url = https://github.com/undisplay/django_moncash
 license = GNU
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Web Environment
```

