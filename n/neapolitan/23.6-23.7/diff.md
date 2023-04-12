# Comparing `tmp/neapolitan-23.6.tar.gz` & `tmp/neapolitan-23.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neapolitan-23.6.tar", last modified: Wed Apr 12 07:39:29 2023, max compression
+gzip compressed data, was "neapolitan-23.7.tar", last modified: Wed Apr 12 10:09:11 2023, max compression
```

## Comparing `neapolitan-23.6.tar` & `neapolitan-23.7.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0       59 2023-04-08 15:53:57.994299 neapolitan-23.6/.gitignore
--rw-r--r--   0        0        0     1081 2023-04-08 09:37:37.437304 neapolitan-23.6/LICENSE
--rw-r--r--   0        0        0     1128 2023-04-11 13:44:05.034404 neapolitan-23.6/Notes.txt
--rw-r--r--   0        0        0     1621 2023-04-10 13:12:58.659109 neapolitan-23.6/README.rst
--rw-r--r--   0        0        0      638 2023-04-08 10:32:21.337055 neapolitan-23.6/docs/Makefile
--rw-r--r--   0        0        0      804 2023-04-08 10:32:21.337901 neapolitan-23.6/docs/make.bat
--rw-r--r--   0        0        0      943 2023-04-08 13:11:08.113103 neapolitan-23.6/docs/source/conf.py
--rw-r--r--   0        0        0      160 2023-04-11 14:07:29.272376 neapolitan-23.6/docs/source/crud-view.rst
--rw-r--r--   0        0        0     1218 2023-04-11 14:39:45.777398 neapolitan-23.6/docs/source/index.rst
--rw-r--r--   0        0        0      213 2023-04-08 15:52:45.220880 neapolitan-23.6/justfile
--rw-r--r--   0        0        0      653 2023-04-10 09:35:41.106347 neapolitan-23.6/pyproject.toml
--rw-r--r--   0        0        0      978 2023-04-12 07:38:47.923200 neapolitan-23.6/src/neapolitan/__init__.py
--rw-r--r--   0        0        0      273 2023-01-30 10:02:57.766415 neapolitan-23.6/src/neapolitan/templates/neapolitan/object_confirm_delete.html
--rw-r--r--   0        0        0      149 2023-02-03 20:19:46.419308 neapolitan-23.6/src/neapolitan/templates/neapolitan/object_detail.html
--rw-r--r--   0        0        0      349 2023-01-30 14:23:01.301967 neapolitan-23.6/src/neapolitan/templates/neapolitan/object_form.html
--rw-r--r--   0        0        0      381 2023-04-12 07:36:22.945023 neapolitan-23.6/src/neapolitan/templates/neapolitan/object_list.html
--rw-r--r--   0        0        0      131 2023-01-30 15:27:46.386717 neapolitan-23.6/src/neapolitan/templates/neapolitan/partial/detail.html
--rw-r--r--   0        0        0      313 2023-01-30 19:42:10.115831 neapolitan-23.6/src/neapolitan/templates/neapolitan/partial/list.html
--rw-r--r--   0        0        0        0 2023-01-30 15:19:09.531163 neapolitan-23.6/src/neapolitan/templatetags/__init__.py
--rw-r--r--   0        0        0     1263 2023-04-08 14:11:26.730590 neapolitan-23.6/src/neapolitan/templatetags/neapolitan.py
--rw-r--r--   0        0        0    17002 2023-04-11 14:10:32.822513 neapolitan-23.6/src/neapolitan/views.py
--rw-r--r--   0        0        0        0 2023-04-08 09:49:24.396767 neapolitan-23.6/tests/__init__.py
--rw-r--r--   0        0        0      840 2023-04-10 09:00:23.657242 neapolitan-23.6/tests/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-04-08 09:49:24.398351 neapolitan-23.6/tests/migrations/__init__.py
--rw-r--r--   0        0        0      236 2023-04-10 08:59:09.860534 neapolitan-23.6/tests/models.py
--rw-r--r--   0        0        0     1411 2023-04-08 16:03:51.880684 neapolitan-23.6/tests/settings.py
--rw-r--r--   0        0        0      181 2023-04-08 16:13:55.492481 neapolitan-23.6/tests/templates/base.html
--rw-r--r--   0        0        0     4348 2023-04-12 07:36:08.080636 neapolitan-23.6/tests/tests.py
--rw-r--r--   0        0        0     2226 1970-01-01 00:00:00.000000 neapolitan-23.6/PKG-INFO
+-rw-r--r--   0        0        0       59 2023-04-08 15:53:57.994299 neapolitan-23.7/.gitignore
+-rw-r--r--   0        0        0     1081 2023-04-08 09:37:37.437304 neapolitan-23.7/LICENSE
+-rw-r--r--   0        0        0     1128 2023-04-11 13:44:05.034404 neapolitan-23.7/Notes.txt
+-rw-r--r--   0        0        0     1621 2023-04-10 13:12:58.659109 neapolitan-23.7/README.rst
+-rw-r--r--   0        0        0      638 2023-04-08 10:32:21.337055 neapolitan-23.7/docs/Makefile
+-rw-r--r--   0        0        0      804 2023-04-08 10:32:21.337901 neapolitan-23.7/docs/make.bat
+-rw-r--r--   0        0        0      943 2023-04-08 13:11:08.113103 neapolitan-23.7/docs/source/conf.py
+-rw-r--r--   0        0        0      160 2023-04-11 14:07:29.272376 neapolitan-23.7/docs/source/crud-view.rst
+-rw-r--r--   0        0        0     1232 2023-04-12 10:05:03.102830 neapolitan-23.7/docs/source/index.rst
+-rw-r--r--   0        0        0      562 2023-04-12 10:04:35.742277 neapolitan-23.7/docs/source/templates.rst
+-rw-r--r--   0        0        0      213 2023-04-08 15:52:45.220880 neapolitan-23.7/justfile
+-rw-r--r--   0        0        0      653 2023-04-10 09:35:41.106347 neapolitan-23.7/pyproject.toml
+-rw-r--r--   0        0        0      978 2023-04-12 10:08:36.880467 neapolitan-23.7/src/neapolitan/__init__.py
+-rw-r--r--   0        0        0      273 2023-01-30 10:02:57.766415 neapolitan-23.7/src/neapolitan/templates/neapolitan/object_confirm_delete.html
+-rw-r--r--   0        0        0      149 2023-02-03 20:19:46.419308 neapolitan-23.7/src/neapolitan/templates/neapolitan/object_detail.html
+-rw-r--r--   0        0        0      427 2023-04-12 09:54:30.457200 neapolitan-23.7/src/neapolitan/templates/neapolitan/object_form.html
+-rw-r--r--   0        0        0      381 2023-04-12 07:36:22.945023 neapolitan-23.7/src/neapolitan/templates/neapolitan/object_list.html
+-rw-r--r--   0        0        0      131 2023-01-30 15:27:46.386717 neapolitan-23.7/src/neapolitan/templates/neapolitan/partial/detail.html
+-rw-r--r--   0        0        0      313 2023-01-30 19:42:10.115831 neapolitan-23.7/src/neapolitan/templates/neapolitan/partial/list.html
+-rw-r--r--   0        0        0        0 2023-01-30 15:19:09.531163 neapolitan-23.7/src/neapolitan/templatetags/__init__.py
+-rw-r--r--   0        0        0     1263 2023-04-08 14:11:26.730590 neapolitan-23.7/src/neapolitan/templatetags/neapolitan.py
+-rw-r--r--   0        0        0    17002 2023-04-11 14:10:32.822513 neapolitan-23.7/src/neapolitan/views.py
+-rw-r--r--   0        0        0        0 2023-04-08 09:49:24.396767 neapolitan-23.7/tests/__init__.py
+-rw-r--r--   0        0        0      840 2023-04-10 09:00:23.657242 neapolitan-23.7/tests/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-04-08 09:49:24.398351 neapolitan-23.7/tests/migrations/__init__.py
+-rw-r--r--   0        0        0      236 2023-04-10 08:59:09.860534 neapolitan-23.7/tests/models.py
+-rw-r--r--   0        0        0     1411 2023-04-08 16:03:51.880684 neapolitan-23.7/tests/settings.py
+-rw-r--r--   0        0        0      181 2023-04-08 16:13:55.492481 neapolitan-23.7/tests/templates/base.html
+-rw-r--r--   0        0        0     4434 2023-04-12 09:58:49.359041 neapolitan-23.7/tests/tests.py
+-rw-r--r--   0        0        0     2226 1970-01-01 00:00:00.000000 neapolitan-23.7/PKG-INFO
```

### Comparing `neapolitan-23.6/LICENSE` & `neapolitan-23.7/LICENSE`

 * *Files identical despite different names*

### Comparing `neapolitan-23.6/Notes.txt` & `neapolitan-23.7/Notes.txt`

 * *Files identical despite different names*

### Comparing `neapolitan-23.6/README.rst` & `neapolitan-23.7/README.rst`

 * *Files identical despite different names*

### Comparing `neapolitan-23.6/docs/Makefile` & `neapolitan-23.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `neapolitan-23.6/docs/make.bat` & `neapolitan-23.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `neapolitan-23.6/docs/source/conf.py` & `neapolitan-23.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `neapolitan-23.6/docs/source/index.rst` & `neapolitan-23.7/docs/source/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 
 
 .. toctree::
     :maxdepth: 1
     :caption: Contents:
 
     crud-view
+    templates
 
 ..
    Indices and tables
    ==================
 
    * :ref:`genindex`
    * :ref:`modindex`
```

### Comparing `neapolitan-23.6/pyproject.toml` & `neapolitan-23.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `neapolitan-23.6/src/neapolitan/__init__.py` & `neapolitan-23.7/src/neapolitan/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,8 +31,8 @@
 
 Where you take your app after that is up to you. But Neapolitan will get you
 started.
 
 Let's go! 🚀
 """
 
-__version__ = "23.6"
+__version__ = "23.7"
```

### Comparing `neapolitan-23.6/src/neapolitan/templatetags/neapolitan.py` & `neapolitan-23.7/src/neapolitan/templatetags/neapolitan.py`

 * *Files identical despite different names*

### Comparing `neapolitan-23.6/src/neapolitan/views.py` & `neapolitan-23.7/src/neapolitan/views.py`

 * *Files identical despite different names*

### Comparing `neapolitan-23.6/tests/migrations/0001_initial.py` & `neapolitan-23.7/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `neapolitan-23.6/tests/settings.py` & `neapolitan-23.7/tests/settings.py`

 * *Files identical despite different names*

### Comparing `neapolitan-23.6/tests/tests.py` & `neapolitan-23.7/tests/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 
     def test_create(self):
         create_url = reverse("bookmark-create")
 
         # Load the form.
         response = self.client.get(create_url)
         self.assertEqual(response.status_code, 200)
+        self.assertContains(response, '<form method="POST" action="/bookmark/new/">')
 
         # Submit the form.
         response = self.client.post(
             create_url,
             {
                 "url": "https://example.com/",
                 "title": "Example",
```

### Comparing `neapolitan-23.6/PKG-INFO` & `neapolitan-23.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neapolitan
-Version: 23.6
+Version: 23.7
 Summary: Neapolitan: quick CRUD views for Django.
 Author-email: Carlton Gibson <carlton.gibson@noumenal.es>
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: Django
 Requires-Dist: django-filter
 Requires-Dist: Sphinx ; extra == "docs"
```

