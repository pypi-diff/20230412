# Comparing `tmp/otc_sphinx_directives-0.0.2.tar.gz` & `tmp/otc_sphinx_directives-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otc_sphinx_directives-0.0.2.tar", last modified: Wed Apr  5 13:45:28 2023, max compression
+gzip compressed data, was "otc_sphinx_directives-0.1.0.tar", last modified: Wed Apr 12 14:11:01 2023, max compression
```

## Comparing `otc_sphinx_directives-0.0.2.tar` & `otc_sphinx_directives-0.1.0.tar`

### file list

```diff
@@ -1,43 +1,50 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 13:45:28.054751 otc_sphinx_directives-0.0.2/
--rw-r--r--   0 root         (0) root         (0)       50 2023-04-05 13:43:34.000000 otc_sphinx_directives-0.0.2/.stestr.conf
--rw-r--r--   0 root         (0) root         (0)      188 2023-04-05 13:45:28.000000 otc_sphinx_directives-0.0.2/AUTHORS
--rw-r--r--   0 root         (0) root         (0)     1449 2023-04-05 13:45:28.000000 otc_sphinx_directives-0.0.2/ChangeLog
--rw-r--r--   0 root         (0) root         (0)    11357 2023-04-05 13:43:34.000000 otc_sphinx_directives-0.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      744 2023-04-05 13:45:28.054751 otc_sphinx_directives-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      110 2023-04-05 13:43:34.000000 otc_sphinx_directives-0.0.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 13:45:28.052752 otc_sphinx_directives-0.0.2/doc/
--rw-r--r--   0 root         (0) root         (0)      301 2023-04-05 13:43:34.000000 otc_sphinx_directives-0.0.2/doc/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 13:45:28.052752 otc_sphinx_directives-0.0.2/doc/source/
--rw-r--r--   0 root         (0) root         (0)      311 2023-04-05 13:43:34.000000 otc_sphinx_directives-0.0.2/doc/source/conf.py
--rw-r--r--   0 root         (0) root         (0)      310 2023-04-05 13:43:34.000000 otc_sphinx_directives-0.0.2/doc/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 13:45:28.052752 otc_sphinx_directives-0.0.2/otc_sphinx_directives/
--rw-r--r--   0 root         (0) root         (0)      108 2023-04-05 13:43:34.000000 otc_sphinx_directives-0.0.2/otc_sphinx_directives/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2383 2023-04-05 13:43:34.000000 otc_sphinx_directives-0.0.2/otc_sphinx_directives/directive_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     1308 2023-04-05 13:43:34.000000 otc_sphinx_directives-0.0.2/otc_sphinx_directives/otc_sphinx_directives_setup.py
--rw-r--r--   0 root         (0) root         (0)     2665 2023-04-05 13:43:34.000000 otc_sphinx_directives-0.0.2/otc_sphinx_directives/service_card.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 13:45:28.053752 otc_sphinx_directives-0.0.2/otc_sphinx_directives/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 13:43:34.000000 otc_sphinx_directives-0.0.2/otc_sphinx_directives/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1767 2023-04-05 13:43:34.000000 otc_sphinx_directives-0.0.2/otc_sphinx_directives/tests/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 13:45:28.050752 otc_sphinx_directives-0.0.2/otc_sphinx_directives/tests/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 13:45:28.054751 otc_sphinx_directives-0.0.2/otc_sphinx_directives/tests/templates/directive_wrapper/
--rw-r--r--   0 root         (0) root         (0)      868 2023-04-05 13:43:34.000000 otc_sphinx_directives-0.0.2/otc_sphinx_directives/tests/templates/directive_wrapper/conf.py
--rw-r--r--   0 root         (0) root         (0)      250 2023-04-05 13:43:34.000000 otc_sphinx_directives-0.0.2/otc_sphinx_directives/tests/templates/directive_wrapper/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 13:45:28.054751 otc_sphinx_directives-0.0.2/otc_sphinx_directives/tests/templates/service_card/
--rw-r--r--   0 root         (0) root         (0)      868 2023-04-05 13:43:34.000000 otc_sphinx_directives-0.0.2/otc_sphinx_directives/tests/templates/service_card/conf.py
--rw-r--r--   0 root         (0) root         (0)       95 2023-04-05 13:43:34.000000 otc_sphinx_directives-0.0.2/otc_sphinx_directives/tests/templates/service_card/index.rst
--rw-r--r--   0 root         (0) root         (0)     2330 2023-04-05 13:43:34.000000 otc_sphinx_directives-0.0.2/otc_sphinx_directives/tests/test_directive_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     2337 2023-04-05 13:43:34.000000 otc_sphinx_directives-0.0.2/otc_sphinx_directives/tests/test_service_card.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 13:45:28.053752 otc_sphinx_directives-0.0.2/otc_sphinx_directives.egg-info/
--rw-r--r--   0 root         (0) root         (0)      744 2023-04-05 13:45:28.000000 otc_sphinx_directives-0.0.2/otc_sphinx_directives.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1091 2023-04-05 13:45:28.000000 otc_sphinx_directives-0.0.2/otc_sphinx_directives.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       86 2023-04-05 13:45:28.000000 otc_sphinx_directives-0.0.2/otc_sphinx_directives.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-05 13:45:28.000000 otc_sphinx_directives-0.0.2/otc_sphinx_directives.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       46 2023-04-05 13:45:28.000000 otc_sphinx_directives-0.0.2/otc_sphinx_directives.egg-info/pbr.json
--rw-r--r--   0 root         (0) root         (0)       27 2023-04-05 13:45:28.000000 otc_sphinx_directives-0.0.2/otc_sphinx_directives.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-05 13:45:28.000000 otc_sphinx_directives-0.0.2/otc_sphinx_directives.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      309 2023-04-05 13:43:34.000000 otc_sphinx_directives-0.0.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      586 2023-04-05 13:45:28.054751 otc_sphinx_directives-0.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      651 2023-04-05 13:43:34.000000 otc_sphinx_directives-0.0.2/setup.py
--rw-r--r--   0 root         (0) root         (0)      344 2023-04-05 13:43:34.000000 otc_sphinx_directives-0.0.2/test-requirements.txt
--rw-r--r--   0 root         (0) root         (0)     1352 2023-04-05 13:43:34.000000 otc_sphinx_directives-0.0.2/tox.ini
--rw-r--r--   0 root         (0) root         (0)      199 2023-04-05 13:43:34.000000 otc_sphinx_directives-0.0.2/zuul.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 14:11:01.892186 otc_sphinx_directives-0.1.0/
+-rw-r--r--   0 root         (0) root         (0)       50 2023-04-12 14:08:08.000000 otc_sphinx_directives-0.1.0/.stestr.conf
+-rw-r--r--   0 root         (0) root         (0)      188 2023-04-12 14:11:01.000000 otc_sphinx_directives-0.1.0/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)     1576 2023-04-12 14:11:01.000000 otc_sphinx_directives-0.1.0/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-04-12 14:08:08.000000 otc_sphinx_directives-0.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      744 2023-04-12 14:11:01.893185 otc_sphinx_directives-0.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      110 2023-04-12 14:08:08.000000 otc_sphinx_directives-0.1.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 14:11:01.890185 otc_sphinx_directives-0.1.0/doc/
+-rw-r--r--   0 root         (0) root         (0)      301 2023-04-12 14:08:08.000000 otc_sphinx_directives-0.1.0/doc/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 14:11:01.890185 otc_sphinx_directives-0.1.0/doc/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 14:11:01.890185 otc_sphinx_directives-0.1.0/doc/source/_static/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 14:08:08.000000 otc_sphinx_directives-0.1.0/doc/source/_static/.placeholder
+-rw-r--r--   0 root         (0) root         (0)      311 2023-04-12 14:08:08.000000 otc_sphinx_directives-0.1.0/doc/source/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 14:11:01.890185 otc_sphinx_directives-0.1.0/doc/source/examples/
+-rw-r--r--   0 root         (0) root         (0)      966 2023-04-12 14:08:08.000000 otc_sphinx_directives-0.1.0/doc/source/examples/directives_ecs.rst
+-rw-r--r--   0 root         (0) root         (0)     1386 2023-04-12 14:08:08.000000 otc_sphinx_directives-0.1.0/doc/source/examples/directives_obs.rst
+-rw-r--r--   0 root         (0) root         (0)      423 2023-04-12 14:08:08.000000 otc_sphinx_directives-0.1.0/doc/source/examples/directives_obs_clean.rst
+-rw-r--r--   0 root         (0) root         (0)      121 2023-04-12 14:08:08.000000 otc_sphinx_directives-0.1.0/doc/source/examples/index.rst
+-rw-r--r--   0 root         (0) root         (0)      118 2023-04-12 14:08:08.000000 otc_sphinx_directives-0.1.0/doc/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 14:11:01.891186 otc_sphinx_directives-0.1.0/otc_sphinx_directives/
+-rw-r--r--   0 root         (0) root         (0)      108 2023-04-12 14:08:08.000000 otc_sphinx_directives-0.1.0/otc_sphinx_directives/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2383 2023-04-12 14:08:08.000000 otc_sphinx_directives-0.1.0/otc_sphinx_directives/directive_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     1308 2023-04-12 14:08:08.000000 otc_sphinx_directives-0.1.0/otc_sphinx_directives/otc_sphinx_directives_setup.py
+-rw-r--r--   0 root         (0) root         (0)     3321 2023-04-12 14:08:08.000000 otc_sphinx_directives-0.1.0/otc_sphinx_directives/service_card.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 14:11:01.892186 otc_sphinx_directives-0.1.0/otc_sphinx_directives/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 14:08:08.000000 otc_sphinx_directives-0.1.0/otc_sphinx_directives/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1767 2023-04-12 14:08:08.000000 otc_sphinx_directives-0.1.0/otc_sphinx_directives/tests/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 14:11:01.888186 otc_sphinx_directives-0.1.0/otc_sphinx_directives/tests/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 14:11:01.892186 otc_sphinx_directives-0.1.0/otc_sphinx_directives/tests/templates/directive_wrapper/
+-rw-r--r--   0 root         (0) root         (0)      791 2023-04-12 14:08:08.000000 otc_sphinx_directives-0.1.0/otc_sphinx_directives/tests/templates/directive_wrapper/conf.py
+-rw-r--r--   0 root         (0) root         (0)      250 2023-04-12 14:08:08.000000 otc_sphinx_directives-0.1.0/otc_sphinx_directives/tests/templates/directive_wrapper/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 14:11:01.892186 otc_sphinx_directives-0.1.0/otc_sphinx_directives/tests/templates/service_card/
+-rw-r--r--   0 root         (0) root         (0)      791 2023-04-12 14:08:08.000000 otc_sphinx_directives-0.1.0/otc_sphinx_directives/tests/templates/service_card/conf.py
+-rw-r--r--   0 root         (0) root         (0)      140 2023-04-12 14:08:08.000000 otc_sphinx_directives-0.1.0/otc_sphinx_directives/tests/templates/service_card/index.rst
+-rw-r--r--   0 root         (0) root         (0)     2330 2023-04-12 14:08:08.000000 otc_sphinx_directives-0.1.0/otc_sphinx_directives/tests/test_directive_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     1978 2023-04-12 14:08:08.000000 otc_sphinx_directives-0.1.0/otc_sphinx_directives/tests/test_service_card.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 14:11:01.892186 otc_sphinx_directives-0.1.0/otc_sphinx_directives.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      744 2023-04-12 14:11:01.000000 otc_sphinx_directives-0.1.0/otc_sphinx_directives.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1276 2023-04-12 14:11:01.000000 otc_sphinx_directives-0.1.0/otc_sphinx_directives.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2023-04-12 14:11:01.000000 otc_sphinx_directives-0.1.0/otc_sphinx_directives.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 14:11:01.000000 otc_sphinx_directives-0.1.0/otc_sphinx_directives.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       46 2023-04-12 14:11:01.000000 otc_sphinx_directives-0.1.0/otc_sphinx_directives.egg-info/pbr.json
+-rw-r--r--   0 root         (0) root         (0)       27 2023-04-12 14:11:01.000000 otc_sphinx_directives-0.1.0/otc_sphinx_directives.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-12 14:11:01.000000 otc_sphinx_directives-0.1.0/otc_sphinx_directives.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      311 2023-04-12 14:08:08.000000 otc_sphinx_directives-0.1.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      586 2023-04-12 14:11:01.893185 otc_sphinx_directives-0.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      651 2023-04-12 14:08:08.000000 otc_sphinx_directives-0.1.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)      312 2023-04-12 14:08:08.000000 otc_sphinx_directives-0.1.0/test-requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     1366 2023-04-12 14:08:08.000000 otc_sphinx_directives-0.1.0/tox.ini
+-rw-r--r--   0 root         (0) root         (0)      245 2023-04-12 14:08:08.000000 otc_sphinx_directives-0.1.0/zuul.yaml
```

### Comparing `otc_sphinx_directives-0.0.2/ChangeLog` & `otc_sphinx_directives-0.1.0/ChangeLog`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 CHANGES
 =======
 
+0.1.0
+-----
+
+* Service based view (#14)
+* change zuul.yaml and add py39 (#12)
+* remove otcdocstheme from test templates (#10)
+
 0.0.2
 -----
 
 * Add unit tests for directives (#4)
 * Add Example Documentation (#6)
 
 0.0.1
```

### Comparing `otc_sphinx_directives-0.0.2/LICENSE` & `otc_sphinx_directives-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.0.2/PKG-INFO` & `otc_sphinx_directives-0.1.0/otc_sphinx_directives.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: otc_sphinx_directives
-Version: 0.0.2
+Name: otc-sphinx-directives
+Version: 0.1.0
 Summary: Open Telekom Cloud Sphinx Directives
 Home-page: UNKNOWN
 Author: Open Telekom Cloud Ecosystem Squad
 License: UNKNOWN
 Keywords: Sphinx, Sphinx Directives, Open Telekom Cloud
 Platform: UNKNOWN
 Classifier: Framework :: Sphinx
```

### Comparing `otc_sphinx_directives-0.0.2/otc_sphinx_directives/directive_wrapper.py` & `otc_sphinx_directives-0.1.0/otc_sphinx_directives/directive_wrapper.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.0.2/otc_sphinx_directives/otc_sphinx_directives_setup.py` & `otc_sphinx_directives-0.1.0/otc_sphinx_directives/otc_sphinx_directives_setup.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.0.2/otc_sphinx_directives/tests/base.py` & `otc_sphinx_directives-0.1.0/otc_sphinx_directives/tests/base.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.0.2/otc_sphinx_directives/tests/templates/directive_wrapper/conf.py` & `otc_sphinx_directives-0.1.0/otc_sphinx_directives/tests/templates/directive_wrapper/conf.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,26 +7,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 extensions = [
-    'otcdocstheme',
     'otc_sphinx_directives'
 ]
 
 
-html_theme = 'otcdocs'
+html_theme = 'classic'
 html_theme_options = {
 }
 html_title = "Test Case"
 html_static_path = ['_static']
 html_copy_source = False
 
 source_suffix = '.rst'
 source_encoding = 'utf-8'
 master_doc = 'index'
-
-
-otcdocs_auto_name = False
-otcdocs_auto_version = False
```

### Comparing `otc_sphinx_directives-0.0.2/otc_sphinx_directives/tests/templates/service_card/conf.py` & `otc_sphinx_directives-0.1.0/otc_sphinx_directives/tests/templates/service_card/conf.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,26 +7,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 extensions = [
-    'otcdocstheme',
     'otc_sphinx_directives'
 ]
 
 
-html_theme = 'otcdocs'
+html_theme = 'classic'
 html_theme_options = {
 }
 html_title = "Test Case"
 html_static_path = ['_static']
 html_copy_source = False
 
 source_suffix = '.rst'
 source_encoding = 'utf-8'
 master_doc = 'index'
-
-
-otcdocs_auto_name = False
-otcdocs_auto_version = False
```

### Comparing `otc_sphinx_directives-0.0.2/otc_sphinx_directives/tests/test_directive_wrapper.py` & `otc_sphinx_directives-0.1.0/otc_sphinx_directives/tests/test_directive_wrapper.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.0.2/otc_sphinx_directives.egg-info/PKG-INFO` & `otc_sphinx_directives-0.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: otc-sphinx-directives
-Version: 0.0.2
+Name: otc_sphinx_directives
+Version: 0.1.0
 Summary: Open Telekom Cloud Sphinx Directives
 Home-page: UNKNOWN
 Author: Open Telekom Cloud Ecosystem Squad
 License: UNKNOWN
 Keywords: Sphinx, Sphinx Directives, Open Telekom Cloud
 Platform: UNKNOWN
 Classifier: Framework :: Sphinx
```

### Comparing `otc_sphinx_directives-0.0.2/otc_sphinx_directives.egg-info/SOURCES.txt` & `otc_sphinx_directives-0.1.0/otc_sphinx_directives.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,19 @@
 setup.py
 test-requirements.txt
 tox.ini
 zuul.yaml
 doc/requirements.txt
 doc/source/conf.py
 doc/source/index.rst
+doc/source/_static/.placeholder
+doc/source/examples/directives_ecs.rst
+doc/source/examples/directives_obs.rst
+doc/source/examples/directives_obs_clean.rst
+doc/source/examples/index.rst
 otc_sphinx_directives/__init__.py
 otc_sphinx_directives/directive_wrapper.py
 otc_sphinx_directives/otc_sphinx_directives_setup.py
 otc_sphinx_directives/service_card.py
 otc_sphinx_directives.egg-info/PKG-INFO
 otc_sphinx_directives.egg-info/SOURCES.txt
 otc_sphinx_directives.egg-info/dependency_links.txt
```

### Comparing `otc_sphinx_directives-0.0.2/setup.cfg` & `otc_sphinx_directives-0.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.0.2/setup.py` & `otc_sphinx_directives-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.0.2/tox.ini` & `otc_sphinx_directives-0.1.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -40,8 +40,9 @@
 #      Also, both openstacksdk and Donald Knuth disagree with the rule. Line
 #      breaks should occur before the binary operator for readability.
 ignore = H306,H4,W503, E501
 show-source = True
 exclude=.venv,.git,.tox,dist,doc,*lib/python*,*egg,build
 
 [doc8]
+ignore = D001
 extensions = .rst, .yaml
```

