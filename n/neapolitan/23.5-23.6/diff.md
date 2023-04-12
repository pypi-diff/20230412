# Comparing `tmp/neapolitan-23.5.tar.gz` & `tmp/neapolitan-23.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neapolitan-23.5.tar", last modified: Tue Apr 11 14:14:04 2023, max compression
+gzip compressed data, was "neapolitan-23.6.tar", last modified: Wed Apr 12 07:39:29 2023, max compression
```

## Comparing `neapolitan-23.5.tar` & `neapolitan-23.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       59 2023-04-08 15:53:57.994299 neapolitan-23.5/.gitignore
--rw-r--r--   0        0        0     1081 2023-04-08 09:37:37.437304 neapolitan-23.5/LICENSE
--rw-r--r--   0        0        0     1128 2023-04-11 13:44:05.034404 neapolitan-23.5/Notes.txt
--rw-r--r--   0        0        0     1621 2023-04-10 13:12:58.659109 neapolitan-23.5/README.rst
--rw-r--r--   0        0        0      638 2023-04-08 10:32:21.337055 neapolitan-23.5/docs/Makefile
--rw-r--r--   0        0        0      804 2023-04-08 10:32:21.337901 neapolitan-23.5/docs/make.bat
--rw-r--r--   0        0        0      943 2023-04-08 13:11:08.113103 neapolitan-23.5/docs/source/conf.py
--rw-r--r--   0        0        0      160 2023-04-11 14:07:29.272376 neapolitan-23.5/docs/source/crud-view.rst
--rw-r--r--   0        0        0     1169 2023-04-11 14:06:03.118807 neapolitan-23.5/docs/source/index.rst
--rw-r--r--   0        0        0      213 2023-04-08 15:52:45.220880 neapolitan-23.5/justfile
--rw-r--r--   0        0        0      653 2023-04-10 09:35:41.106347 neapolitan-23.5/pyproject.toml
--rw-r--r--   0        0        0      948 2023-04-11 14:13:17.268344 neapolitan-23.5/src/neapolitan/__init__.py
--rw-r--r--   0        0        0      273 2023-01-30 10:02:57.766415 neapolitan-23.5/src/neapolitan/templates/neapolitan/object_confirm_delete.html
--rw-r--r--   0        0        0      149 2023-02-03 20:19:46.419308 neapolitan-23.5/src/neapolitan/templates/neapolitan/object_detail.html
--rw-r--r--   0        0        0      349 2023-01-30 14:23:01.301967 neapolitan-23.5/src/neapolitan/templates/neapolitan/object_form.html
--rw-r--r--   0        0        0      259 2023-04-11 13:59:14.152085 neapolitan-23.5/src/neapolitan/templates/neapolitan/object_list.html
--rw-r--r--   0        0        0      131 2023-01-30 15:27:46.386717 neapolitan-23.5/src/neapolitan/templates/neapolitan/partial/detail.html
--rw-r--r--   0        0        0      313 2023-01-30 19:42:10.115831 neapolitan-23.5/src/neapolitan/templates/neapolitan/partial/list.html
--rw-r--r--   0        0        0        0 2023-01-30 15:19:09.531163 neapolitan-23.5/src/neapolitan/templatetags/__init__.py
--rw-r--r--   0        0        0     1263 2023-04-08 14:11:26.730590 neapolitan-23.5/src/neapolitan/templatetags/neapolitan.py
--rw-r--r--   0        0        0    17002 2023-04-11 14:10:32.822513 neapolitan-23.5/src/neapolitan/views.py
--rw-r--r--   0        0        0        0 2023-04-08 09:49:24.396767 neapolitan-23.5/tests/__init__.py
--rw-r--r--   0        0        0      840 2023-04-10 09:00:23.657242 neapolitan-23.5/tests/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-04-08 09:49:24.398351 neapolitan-23.5/tests/migrations/__init__.py
--rw-r--r--   0        0        0      236 2023-04-10 08:59:09.860534 neapolitan-23.5/tests/models.py
--rw-r--r--   0        0        0     1411 2023-04-08 16:03:51.880684 neapolitan-23.5/tests/settings.py
--rw-r--r--   0        0        0      181 2023-04-08 16:13:55.492481 neapolitan-23.5/tests/templates/base.html
--rw-r--r--   0        0        0     3972 2023-04-11 13:56:54.581398 neapolitan-23.5/tests/tests.py
--rw-r--r--   0        0        0     2196 1970-01-01 00:00:00.000000 neapolitan-23.5/PKG-INFO
+-rw-r--r--   0        0        0       59 2023-04-08 15:53:57.994299 neapolitan-23.6/.gitignore
+-rw-r--r--   0        0        0     1081 2023-04-08 09:37:37.437304 neapolitan-23.6/LICENSE
+-rw-r--r--   0        0        0     1128 2023-04-11 13:44:05.034404 neapolitan-23.6/Notes.txt
+-rw-r--r--   0        0        0     1621 2023-04-10 13:12:58.659109 neapolitan-23.6/README.rst
+-rw-r--r--   0        0        0      638 2023-04-08 10:32:21.337055 neapolitan-23.6/docs/Makefile
+-rw-r--r--   0        0        0      804 2023-04-08 10:32:21.337901 neapolitan-23.6/docs/make.bat
+-rw-r--r--   0        0        0      943 2023-04-08 13:11:08.113103 neapolitan-23.6/docs/source/conf.py
+-rw-r--r--   0        0        0      160 2023-04-11 14:07:29.272376 neapolitan-23.6/docs/source/crud-view.rst
+-rw-r--r--   0        0        0     1218 2023-04-11 14:39:45.777398 neapolitan-23.6/docs/source/index.rst
+-rw-r--r--   0        0        0      213 2023-04-08 15:52:45.220880 neapolitan-23.6/justfile
+-rw-r--r--   0        0        0      653 2023-04-10 09:35:41.106347 neapolitan-23.6/pyproject.toml
+-rw-r--r--   0        0        0      978 2023-04-12 07:38:47.923200 neapolitan-23.6/src/neapolitan/__init__.py
+-rw-r--r--   0        0        0      273 2023-01-30 10:02:57.766415 neapolitan-23.6/src/neapolitan/templates/neapolitan/object_confirm_delete.html
+-rw-r--r--   0        0        0      149 2023-02-03 20:19:46.419308 neapolitan-23.6/src/neapolitan/templates/neapolitan/object_detail.html
+-rw-r--r--   0        0        0      349 2023-01-30 14:23:01.301967 neapolitan-23.6/src/neapolitan/templates/neapolitan/object_form.html
+-rw-r--r--   0        0        0      381 2023-04-12 07:36:22.945023 neapolitan-23.6/src/neapolitan/templates/neapolitan/object_list.html
+-rw-r--r--   0        0        0      131 2023-01-30 15:27:46.386717 neapolitan-23.6/src/neapolitan/templates/neapolitan/partial/detail.html
+-rw-r--r--   0        0        0      313 2023-01-30 19:42:10.115831 neapolitan-23.6/src/neapolitan/templates/neapolitan/partial/list.html
+-rw-r--r--   0        0        0        0 2023-01-30 15:19:09.531163 neapolitan-23.6/src/neapolitan/templatetags/__init__.py
+-rw-r--r--   0        0        0     1263 2023-04-08 14:11:26.730590 neapolitan-23.6/src/neapolitan/templatetags/neapolitan.py
+-rw-r--r--   0        0        0    17002 2023-04-11 14:10:32.822513 neapolitan-23.6/src/neapolitan/views.py
+-rw-r--r--   0        0        0        0 2023-04-08 09:49:24.396767 neapolitan-23.6/tests/__init__.py
+-rw-r--r--   0        0        0      840 2023-04-10 09:00:23.657242 neapolitan-23.6/tests/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-04-08 09:49:24.398351 neapolitan-23.6/tests/migrations/__init__.py
+-rw-r--r--   0        0        0      236 2023-04-10 08:59:09.860534 neapolitan-23.6/tests/models.py
+-rw-r--r--   0        0        0     1411 2023-04-08 16:03:51.880684 neapolitan-23.6/tests/settings.py
+-rw-r--r--   0        0        0      181 2023-04-08 16:13:55.492481 neapolitan-23.6/tests/templates/base.html
+-rw-r--r--   0        0        0     4348 2023-04-12 07:36:08.080636 neapolitan-23.6/tests/tests.py
+-rw-r--r--   0        0        0     2226 1970-01-01 00:00:00.000000 neapolitan-23.6/PKG-INFO
```

### Comparing `neapolitan-23.5/LICENSE` & `neapolitan-23.6/LICENSE`

 * *Files identical despite different names*

### Comparing `neapolitan-23.5/Notes.txt` & `neapolitan-23.6/Notes.txt`

 * *Files identical despite different names*

### Comparing `neapolitan-23.5/README.rst` & `neapolitan-23.6/README.rst`

 * *Files identical despite different names*

### Comparing `neapolitan-23.5/docs/Makefile` & `neapolitan-23.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `neapolitan-23.5/docs/make.bat` & `neapolitan-23.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `neapolitan-23.5/docs/source/conf.py` & `neapolitan-23.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `neapolitan-23.5/docs/source/index.rst` & `neapolitan-23.6/docs/source/index.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Welcome to Neapolitan's documentation!
 ======================================
 
+Neapolitan provides quick CRUD views for Django.
 
 I have a Django model::
 
     from django.db import models
 
     class Bookmark(models.Model):
         url = models.URLField(unique=True)
```

### Comparing `neapolitan-23.5/pyproject.toml` & `neapolitan-23.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `neapolitan-23.5/src/neapolitan/__init__.py` & `neapolitan-23.6/src/neapolitan/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Neapolitan
+Neapolitan: quick CRUD views for Django.
 
 I have a Django model::
 
     from django.db import models
 
     class Bookmark(models.Model):
         url = models.URLField(unique=True)
@@ -31,8 +31,8 @@
 
 Where you take your app after that is up to you. But Neapolitan will get you
 started.
 
 Let's go! 🚀
 """
 
-__version__ = "23.5"
+__version__ = "23.6"
```

### Comparing `neapolitan-23.5/src/neapolitan/templatetags/neapolitan.py` & `neapolitan-23.6/src/neapolitan/templatetags/neapolitan.py`

 * *Files identical despite different names*

### Comparing `neapolitan-23.5/src/neapolitan/views.py` & `neapolitan-23.6/src/neapolitan/views.py`

 * *Files identical despite different names*

### Comparing `neapolitan-23.5/tests/migrations/0001_initial.py` & `neapolitan-23.6/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `neapolitan-23.5/tests/settings.py` & `neapolitan-23.6/tests/settings.py`

 * *Files identical despite different names*

### Comparing `neapolitan-23.5/tests/tests.py` & `neapolitan-23.6/tests/tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,14 +44,23 @@
         self.assertContains(response, self.homepage.title)
         self.assertContains(response, self.github.title)
         self.assertContains(response, self.fosstodon.title)
         self.assertContains(
             response, '<a href="/bookmark/new/">Add a new bookmark</a>', html=True
         )
 
+    def test_list_empty(self):
+        Bookmark.objects.all().delete()
+        response = self.client.get("/bookmark/")
+        self.assertEqual(response.status_code, 200)
+        self.assertContains(response, "There are no bookmarks. Create one now?")
+        self.assertContains(
+            response, '<a href="/bookmark/new/">Add a new bookmark</a>', html=True
+        )
+
     def test_detail(self):
         response = self.client.get(f"/bookmark/{self.homepage.pk}/")
         self.assertEqual(response.status_code, 200)
         self.assertContains(response, self.homepage.title)
         self.assertContains(response, escape(self.homepage.note))
 
     def test_create(self):
```

### Comparing `neapolitan-23.5/PKG-INFO` & `neapolitan-23.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: neapolitan
-Version: 23.5
-Summary: Neapolitan
+Version: 23.6
+Summary: Neapolitan: quick CRUD views for Django.
 Author-email: Carlton Gibson <carlton.gibson@noumenal.es>
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: Django
 Requires-Dist: django-filter
 Requires-Dist: Sphinx ; extra == "docs"
 Requires-Dist: coverage ; extra == "tests"
```

