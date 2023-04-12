# Comparing `tmp/tencentcloud-sdk-python-dbbrain-3.0.870.tar.gz` & `tmp/tencentcloud-sdk-python-dbbrain-3.0.871.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dbbrain-3.0.870.tar", last modified: Tue Apr 11 03:31:56 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dbbrain-3.0.871.tar", last modified: Wed Apr 12 00:22:15 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dbbrain-3.0.870.tar` & `tencentcloud-sdk-python-dbbrain-3.0.871.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/dbbrain/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/dbbrain/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/dbbrain/v20191016/
--rw-r--r--   0 root         (0) root         (0)    27659 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/dbbrain/v20191016/dbbrain_client.py
--rw-r--r--   0 root         (0) root         (0)   111297 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/dbbrain/v20191016/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/dbbrain/v20191016/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1567 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/dbbrain/v20191016/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/dbbrain/v20210527/
--rw-r--r--   0 root         (0) root         (0)    45821 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/dbbrain/v20210527/dbbrain_client.py
--rw-r--r--   0 root         (0) root         (0)   171969 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/dbbrain/v20210527/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/dbbrain/v20210527/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1930 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/dbbrain/v20210527/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud_sdk_python_dbbrain.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud_sdk_python_dbbrain.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud_sdk_python_dbbrain.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      663 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      749 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/README.rst
--rw-r--r--   0 root         (0) root         (0)     1014 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:22:15.000000 tencentcloud-sdk-python-dbbrain-3.0.871/
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-04-12 00:22:15.000000 tencentcloud-sdk-python-dbbrain-3.0.871/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:22:15.000000 tencentcloud-sdk-python-dbbrain-3.0.871/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-12 00:22:15.000000 tencentcloud-sdk-python-dbbrain-3.0.871/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:22:15.000000 tencentcloud-sdk-python-dbbrain-3.0.871/tencentcloud/dbbrain/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:22:15.000000 tencentcloud-sdk-python-dbbrain-3.0.871/tencentcloud/dbbrain/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:22:15.000000 tencentcloud-sdk-python-dbbrain-3.0.871/tencentcloud/dbbrain/v20191016/
+-rw-r--r--   0 root         (0) root         (0)    27659 2023-04-12 00:22:15.000000 tencentcloud-sdk-python-dbbrain-3.0.871/tencentcloud/dbbrain/v20191016/dbbrain_client.py
+-rw-r--r--   0 root         (0) root         (0)   111297 2023-04-12 00:22:15.000000 tencentcloud-sdk-python-dbbrain-3.0.871/tencentcloud/dbbrain/v20191016/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:22:15.000000 tencentcloud-sdk-python-dbbrain-3.0.871/tencentcloud/dbbrain/v20191016/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-04-12 00:22:15.000000 tencentcloud-sdk-python-dbbrain-3.0.871/tencentcloud/dbbrain/v20191016/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:22:15.000000 tencentcloud-sdk-python-dbbrain-3.0.871/tencentcloud/dbbrain/v20210527/
+-rw-r--r--   0 root         (0) root         (0)    45821 2023-04-12 00:22:15.000000 tencentcloud-sdk-python-dbbrain-3.0.871/tencentcloud/dbbrain/v20210527/dbbrain_client.py
+-rw-r--r--   0 root         (0) root         (0)   172014 2023-04-12 00:22:15.000000 tencentcloud-sdk-python-dbbrain-3.0.871/tencentcloud/dbbrain/v20210527/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:22:15.000000 tencentcloud-sdk-python-dbbrain-3.0.871/tencentcloud/dbbrain/v20210527/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1930 2023-04-12 00:22:15.000000 tencentcloud-sdk-python-dbbrain-3.0.871/tencentcloud/dbbrain/v20210527/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:22:15.000000 tencentcloud-sdk-python-dbbrain-3.0.871/tencentcloud_sdk_python_dbbrain.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-04-12 00:22:15.000000 tencentcloud-sdk-python-dbbrain-3.0.871/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 00:22:15.000000 tencentcloud-sdk-python-dbbrain-3.0.871/tencentcloud_sdk_python_dbbrain.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-12 00:22:15.000000 tencentcloud-sdk-python-dbbrain-3.0.871/tencentcloud_sdk_python_dbbrain.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      663 2023-04-12 00:22:15.000000 tencentcloud-sdk-python-dbbrain-3.0.871/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      749 2023-04-12 00:22:15.000000 tencentcloud-sdk-python-dbbrain-3.0.871/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-04-12 00:22:15.000000 tencentcloud-sdk-python-dbbrain-3.0.871/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-12 00:22:15.000000 tencentcloud-sdk-python-dbbrain-3.0.871/setup.cfg
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.870/PKG-INFO` & `tencentcloud-sdk-python-dbbrain-3.0.871/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dbbrain
-Version: 3.0.870
+Version: 3.0.871
 Summary: Tencent Cloud Dbbrain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dbbrain-3.0.871/tencentcloud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.870'
+__version__ = '3.0.871'
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/dbbrain/v20191016/dbbrain_client.py` & `tencentcloud-sdk-python-dbbrain-3.0.871/tencentcloud/dbbrain/v20191016/dbbrain_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/dbbrain/v20191016/models.py` & `tencentcloud-sdk-python-dbbrain-3.0.871/tencentcloud/dbbrain/v20191016/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/dbbrain/v20191016/errorcodes.py` & `tencentcloud-sdk-python-dbbrain-3.0.871/tencentcloud/dbbrain/v20191016/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/dbbrain/v20210527/dbbrain_client.py` & `tencentcloud-sdk-python-dbbrain-3.0.871/tencentcloud/dbbrain/v20210527/dbbrain_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/dbbrain/v20210527/models.py` & `tencentcloud-sdk-python-dbbrain-3.0.871/tencentcloud/dbbrain/v20210527/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2331,17 +2331,17 @@
         :type InstanceId: str
         :param Md5: sql模版的md5值
         :type Md5: str
         :param StartTime: 开始时间，如“2019-09-10 12:13:14”。
         :type StartTime: str
         :param EndTime: 截止时间，如“2019-09-11 10:13:14”，截止时间与开始时间的间隔小于7天。
         :type EndTime: str
-        :param Offset: 分页参数
+        :param Offset: 偏移量，默认为0。
         :type Offset: int
-        :param Limit: 分页参数
+        :param Limit: 查询数目，默认为20，最大为100。
         :type Limit: int
         :param DB: 数据库列表
         :type DB: list of str
         :param Key: 关键字
         :type Key: list of str
         :param User: 用户
         :type User: list of str
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/dbbrain/v20210527/errorcodes.py` & `tencentcloud-sdk-python-dbbrain-3.0.871/tencentcloud/dbbrain/v20210527/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dbbrain-3.0.871/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dbbrain
-Version: 3.0.870
+Version: 3.0.871
 Summary: Tencent Cloud Dbbrain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-dbbrain-3.0.871/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.870/README.rst` & `tencentcloud-sdk-python-dbbrain-3.0.871/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.870/setup.py` & `tencentcloud-sdk-python-dbbrain-3.0.871/setup.py`

 * *Files identical despite different names*

