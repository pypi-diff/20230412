# Comparing `tmp/apache-airflow-providers-smtp-1.0.1.tar.gz` & `tmp/apache-airflow-providers-smtp-1.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-smtp-1.0.1.tar", last modified: Sun Apr  9 13:44:05 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-smtp-1.0.1rc1.tar", last modified: Sun Apr  9 13:49:56 2023, max compression
```

## Comparing `apache-airflow-providers-smtp-1.0.1.tar` & `apache-airflow-providers-smtp-1.0.1rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:44:05.000000 apache-airflow-providers-smtp-1.0.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-smtp-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-04-09 13:44:03.000000 apache-airflow-providers-smtp-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-smtp-1.0.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4882 2023-04-09 13:44:05.000000 apache-airflow-providers-smtp-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3364 2023-04-09 13:44:03.000000 apache-airflow-providers-smtp-1.0.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:44:04.000000 apache-airflow-providers-smtp-1.0.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:44:04.000000 apache-airflow-providers-smtp-1.0.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:44:05.000000 apache-airflow-providers-smtp-1.0.1/airflow/providers/smtp/
--rw-r--r--   0 root         (0) root         (0)      787 2023-03-15 08:58:48.000000 apache-airflow-providers-smtp-1.0.1/airflow/providers/smtp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2288 2023-04-09 13:44:03.000000 apache-airflow-providers-smtp-1.0.1/airflow/providers/smtp/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:44:05.000000 apache-airflow-providers-smtp-1.0.1/airflow/providers/smtp/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-03-15 08:58:48.000000 apache-airflow-providers-smtp-1.0.1/airflow/providers/smtp/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13824 2023-04-07 21:10:19.000000 apache-airflow-providers-smtp-1.0.1/airflow/providers/smtp/hooks/smtp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:44:05.000000 apache-airflow-providers-smtp-1.0.1/airflow/providers/smtp/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-03-15 08:58:48.000000 apache-airflow-providers-smtp-1.0.1/airflow/providers/smtp/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3434 2023-04-09 06:57:27.000000 apache-airflow-providers-smtp-1.0.1/airflow/providers/smtp/operators/smtp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:44:05.000000 apache-airflow-providers-smtp-1.0.1/apache_airflow_providers_smtp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4882 2023-04-09 13:44:04.000000 apache-airflow-providers-smtp-1.0.1/apache_airflow_providers_smtp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      686 2023-04-09 13:44:04.000000 apache-airflow-providers-smtp-1.0.1/apache_airflow_providers_smtp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 13:44:04.000000 apache-airflow-providers-smtp-1.0.1/apache_airflow_providers_smtp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-04-09 13:44:04.000000 apache-airflow-providers-smtp-1.0.1/apache_airflow_providers_smtp.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 13:44:04.000000 apache-airflow-providers-smtp-1.0.1/apache_airflow_providers_smtp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-09 13:44:04.000000 apache-airflow-providers-smtp-1.0.1/apache_airflow_providers_smtp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-09 13:44:04.000000 apache-airflow-providers-smtp-1.0.1/apache_airflow_providers_smtp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-smtp-1.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1808 2023-04-09 13:44:05.000000 apache-airflow-providers-smtp-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1626 2023-04-09 13:44:03.000000 apache-airflow-providers-smtp-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-smtp-1.0.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-04-09 13:49:54.000000 apache-airflow-providers-smtp-1.0.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-smtp-1.0.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4888 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3367 2023-04-09 13:49:54.000000 apache-airflow-providers-smtp-1.0.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-03-15 08:58:48.000000 apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2288 2023-04-09 13:49:54.000000 apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-03-15 08:58:48.000000 apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13824 2023-04-07 21:10:19.000000 apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/hooks/smtp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-03-15 08:58:48.000000 apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3434 2023-04-09 06:57:27.000000 apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/operators/smtp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/apache_airflow_providers_smtp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4888 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/apache_airflow_providers_smtp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      686 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/apache_airflow_providers_smtp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/apache_airflow_providers_smtp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/apache_airflow_providers_smtp.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/apache_airflow_providers_smtp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       27 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/apache_airflow_providers_smtp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/apache_airflow_providers_smtp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-smtp-1.0.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1816 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-04-09 13:49:54.000000 apache-airflow-providers-smtp-1.0.1rc1/setup.py
```

### Comparing `apache-airflow-providers-smtp-1.0.1/LICENSE` & `apache-airflow-providers-smtp-1.0.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.0.1/MANIFEST.in` & `apache-airflow-providers-smtp-1.0.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.0.1/PKG-INFO` & `apache-airflow-providers-smtp-1.0.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-smtp
-Version: 1.0.1
+Version: 1.0.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-smtp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.0.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-smtp``
 
-Release: ``1.0.1``
+Release: ``1.0.1rc1``
 
 
 `Simple Mail Transfer Protocol (SMTP) <https://tools.ietf.org/html/rfc5321>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-smtp-1.0.1/README.rst` & `apache-airflow-providers-smtp-1.0.1rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-smtp``
 
-Release: ``1.0.1``
+Release: ``1.0.1rc1``
 
 
 `Simple Mail Transfer Protocol (SMTP) <https://tools.ietf.org/html/rfc5321>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-smtp-1.0.1/airflow/providers/smtp/__init__.py` & `apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.0.1/airflow/providers/smtp/get_provider_info.py` & `apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.0.1/airflow/providers/smtp/hooks/__init__.py` & `apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.0.1/airflow/providers/smtp/hooks/smtp.py` & `apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/hooks/smtp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.0.1/airflow/providers/smtp/operators/__init__.py` & `apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.0.1/airflow/providers/smtp/operators/smtp.py` & `apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/operators/smtp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.0.1/apache_airflow_providers_smtp.egg-info/PKG-INFO` & `apache-airflow-providers-smtp-1.0.1rc1/apache_airflow_providers_smtp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-smtp
-Version: 1.0.1
+Version: 1.0.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-smtp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.0.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-smtp``
 
-Release: ``1.0.1``
+Release: ``1.0.1rc1``
 
 
 `Simple Mail Transfer Protocol (SMTP) <https://tools.ietf.org/html/rfc5321>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-smtp-1.0.1/apache_airflow_providers_smtp.egg-info/SOURCES.txt` & `apache-airflow-providers-smtp-1.0.1rc1/apache_airflow_providers_smtp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.0.1/pyproject.toml` & `apache-airflow-providers-smtp-1.0.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.0.1/setup.cfg` & `apache-airflow-providers-smtp-1.0.1rc1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -42,20 +42,20 @@
 include_package_data = True
 python_requires = ~=3.7
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow>=2.3.0
+	apache-airflow>=2.3.0.dev0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.smtp.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.smtp
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-smtp-1.0.1/setup.py` & `apache-airflow-providers-smtp-1.0.1rc1/setup.py`

 * *Files identical despite different names*

