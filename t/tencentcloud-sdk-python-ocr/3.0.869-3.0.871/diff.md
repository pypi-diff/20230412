# Comparing `tmp/tencentcloud-sdk-python-ocr-3.0.869.tar.gz` & `tmp/tencentcloud-sdk-python-ocr-3.0.871.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.869.tar", last modified: Mon Apr 10 03:10:43 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.871.tar", last modified: Wed Apr 12 00:37:30 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ocr-3.0.869.tar` & `tencentcloud-sdk-python-ocr-3.0.871.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/tencentcloud/ocr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/tencentcloud/ocr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/tencentcloud/ocr/v20181119/
--rw-r--r--   0 root         (0) root         (0)   406294 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/tencentcloud/ocr/v20181119/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/tencentcloud/ocr/v20181119/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5764 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/tencentcloud/ocr/v20181119/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   104266 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/tencentcloud/ocr/v20181119/ocr_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/tencentcloud_sdk_python_ocr.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/README.rst
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-10 03:10:43.000000 tencentcloud-sdk-python-ocr-3.0.869/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:37:30.000000 tencentcloud-sdk-python-ocr-3.0.871/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-12 00:37:30.000000 tencentcloud-sdk-python-ocr-3.0.871/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:37:30.000000 tencentcloud-sdk-python-ocr-3.0.871/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:37:30.000000 tencentcloud-sdk-python-ocr-3.0.871/tencentcloud/ocr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:37:30.000000 tencentcloud-sdk-python-ocr-3.0.871/tencentcloud/ocr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:37:30.000000 tencentcloud-sdk-python-ocr-3.0.871/tencentcloud/ocr/v20181119/
+-rw-r--r--   0 root         (0) root         (0)   406294 2023-04-12 00:37:30.000000 tencentcloud-sdk-python-ocr-3.0.871/tencentcloud/ocr/v20181119/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:37:30.000000 tencentcloud-sdk-python-ocr-3.0.871/tencentcloud/ocr/v20181119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5764 2023-04-12 00:37:30.000000 tencentcloud-sdk-python-ocr-3.0.871/tencentcloud/ocr/v20181119/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   104266 2023-04-12 00:37:30.000000 tencentcloud-sdk-python-ocr-3.0.871/tencentcloud/ocr/v20181119/ocr_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-12 00:37:30.000000 tencentcloud-sdk-python-ocr-3.0.871/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:37:30.000000 tencentcloud-sdk-python-ocr-3.0.871/tencentcloud_sdk_python_ocr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-12 00:37:30.000000 tencentcloud-sdk-python-ocr-3.0.871/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 00:37:30.000000 tencentcloud-sdk-python-ocr-3.0.871/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-12 00:37:30.000000 tencentcloud-sdk-python-ocr-3.0.871/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-12 00:37:30.000000 tencentcloud-sdk-python-ocr-3.0.871/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-12 00:37:30.000000 tencentcloud-sdk-python-ocr-3.0.871/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-12 00:37:30.000000 tencentcloud-sdk-python-ocr-3.0.871/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-12 00:37:30.000000 tencentcloud-sdk-python-ocr-3.0.871/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.869/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.871/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.869
+Version: 3.0.871
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.869/tencentcloud/ocr/v20181119/models.py` & `tencentcloud-sdk-python-ocr-3.0.871/tencentcloud/ocr/v20181119/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.869/tencentcloud/ocr/v20181119/errorcodes.py` & `tencentcloud-sdk-python-ocr-3.0.871/tencentcloud/ocr/v20181119/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.869/tencentcloud/ocr/v20181119/ocr_client.py` & `tencentcloud-sdk-python-ocr-3.0.871/tencentcloud/ocr/v20181119/ocr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.869/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ocr-3.0.871/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.869'
+__version__ = '3.0.871'
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.869/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.871/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.869
+Version: 3.0.871
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.869/README.rst` & `tencentcloud-sdk-python-ocr-3.0.871/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.869/setup.py` & `tencentcloud-sdk-python-ocr-3.0.871/setup.py`

 * *Files identical despite different names*

