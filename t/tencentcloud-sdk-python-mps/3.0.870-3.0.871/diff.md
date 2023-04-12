# Comparing `tmp/tencentcloud-sdk-python-mps-3.0.870.tar.gz` & `tmp/tencentcloud-sdk-python-mps-3.0.871.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-mps-3.0.870.tar", last modified: Tue Apr 11 03:43:28 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-mps-3.0.871.tar", last modified: Wed Apr 12 00:36:20 2023, max compression
```

## Comparing `tencentcloud-sdk-python-mps-3.0.870.tar` & `tencentcloud-sdk-python-mps-3.0.871.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:43:28.000000 tencentcloud-sdk-python-mps-3.0.870/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-11 03:43:28.000000 tencentcloud-sdk-python-mps-3.0.870/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:43:28.000000 tencentcloud-sdk-python-mps-3.0.870/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-11 03:43:28.000000 tencentcloud-sdk-python-mps-3.0.870/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:43:28.000000 tencentcloud-sdk-python-mps-3.0.870/tencentcloud/mps/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:43:28.000000 tencentcloud-sdk-python-mps-3.0.870/tencentcloud/mps/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:43:28.000000 tencentcloud-sdk-python-mps-3.0.870/tencentcloud/mps/v20190612/
--rw-r--r--   0 root         (0) root         (0)    89755 2023-04-11 03:43:28.000000 tencentcloud-sdk-python-mps-3.0.870/tencentcloud/mps/v20190612/mps_client.py
--rw-r--r--   0 root         (0) root         (0)   797827 2023-04-11 03:43:28.000000 tencentcloud-sdk-python-mps-3.0.870/tencentcloud/mps/v20190612/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:43:28.000000 tencentcloud-sdk-python-mps-3.0.870/tencentcloud/mps/v20190612/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13373 2023-04-11 03:43:28.000000 tencentcloud-sdk-python-mps-3.0.870/tencentcloud/mps/v20190612/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:43:28.000000 tencentcloud-sdk-python-mps-3.0.870/tencentcloud_sdk_python_mps.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-11 03:43:28.000000 tencentcloud-sdk-python-mps-3.0.870/tencentcloud_sdk_python_mps.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 03:43:28.000000 tencentcloud-sdk-python-mps-3.0.870/tencentcloud_sdk_python_mps.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-11 03:43:28.000000 tencentcloud-sdk-python-mps-3.0.870/tencentcloud_sdk_python_mps.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-11 03:43:28.000000 tencentcloud-sdk-python-mps-3.0.870/tencentcloud_sdk_python_mps.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-11 03:43:28.000000 tencentcloud-sdk-python-mps-3.0.870/README.rst
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-11 03:43:28.000000 tencentcloud-sdk-python-mps-3.0.870/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-11 03:43:28.000000 tencentcloud-sdk-python-mps-3.0.870/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:36:20.000000 tencentcloud-sdk-python-mps-3.0.871/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-12 00:36:20.000000 tencentcloud-sdk-python-mps-3.0.871/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:36:20.000000 tencentcloud-sdk-python-mps-3.0.871/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-12 00:36:19.000000 tencentcloud-sdk-python-mps-3.0.871/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:36:20.000000 tencentcloud-sdk-python-mps-3.0.871/tencentcloud/mps/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:36:19.000000 tencentcloud-sdk-python-mps-3.0.871/tencentcloud/mps/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:36:20.000000 tencentcloud-sdk-python-mps-3.0.871/tencentcloud/mps/v20190612/
+-rw-r--r--   0 root         (0) root         (0)    89755 2023-04-12 00:36:19.000000 tencentcloud-sdk-python-mps-3.0.871/tencentcloud/mps/v20190612/mps_client.py
+-rw-r--r--   0 root         (0) root         (0)   797947 2023-04-12 00:36:19.000000 tencentcloud-sdk-python-mps-3.0.871/tencentcloud/mps/v20190612/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:36:19.000000 tencentcloud-sdk-python-mps-3.0.871/tencentcloud/mps/v20190612/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13373 2023-04-12 00:36:19.000000 tencentcloud-sdk-python-mps-3.0.871/tencentcloud/mps/v20190612/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:36:20.000000 tencentcloud-sdk-python-mps-3.0.871/tencentcloud_sdk_python_mps.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-12 00:36:20.000000 tencentcloud-sdk-python-mps-3.0.871/tencentcloud_sdk_python_mps.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 00:36:20.000000 tencentcloud-sdk-python-mps-3.0.871/tencentcloud_sdk_python_mps.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-12 00:36:20.000000 tencentcloud-sdk-python-mps-3.0.871/tencentcloud_sdk_python_mps.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-12 00:36:20.000000 tencentcloud-sdk-python-mps-3.0.871/tencentcloud_sdk_python_mps.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-12 00:36:19.000000 tencentcloud-sdk-python-mps-3.0.871/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-12 00:36:19.000000 tencentcloud-sdk-python-mps-3.0.871/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-12 00:36:20.000000 tencentcloud-sdk-python-mps-3.0.871/setup.cfg
```

### Comparing `tencentcloud-sdk-python-mps-3.0.870/PKG-INFO` & `tencentcloud-sdk-python-mps-3.0.871/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mps
-Version: 3.0.870
+Version: 3.0.871
 Summary: Tencent Cloud Mps SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mps-3.0.870/tencentcloud/__init__.py` & `tencentcloud-sdk-python-mps-3.0.871/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-mps-3.0.870/tencentcloud/mps/v20190612/mps_client.py` & `tencentcloud-sdk-python-mps-3.0.871/tencentcloud/mps/v20190612/mps_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mps-3.0.870/tencentcloud/mps/v20190612/models.py` & `tencentcloud-sdk-python-mps-3.0.871/tencentcloud/mps/v20190612/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5497,15 +5497,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param Mode: SRT模式，可选[LISTENER|CALLER]，默认为LISTENER。
         :type Mode: str
-        :param StreamId: 流Id，可选大小写字母、数字和特殊字符（.#!:&,=_-），长度为0~512。
+        :param StreamId: 流Id，可选大小写字母、数字和特殊字符（.#!:&,=_-），长度为0~512。具体格式可以参考：https://github.com/Haivision/srt/blob/master/docs/features/access-control.md#standard-keys。
         :type StreamId: str
         :param Latency: 延迟，默认0，单位ms，范围为[0, 3000]。
         :type Latency: int
         :param RecvLatency: 接收延迟，默认120，单位ms，范围为[0, 3000]。
         :type RecvLatency: int
         :param PeerLatency: 对端延迟，默认0，单位ms，范围为[0, 3000]。
         :type PeerLatency: int
```

### Comparing `tencentcloud-sdk-python-mps-3.0.870/tencentcloud/mps/v20190612/errorcodes.py` & `tencentcloud-sdk-python-mps-3.0.871/tencentcloud/mps/v20190612/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mps-3.0.870/tencentcloud_sdk_python_mps.egg-info/PKG-INFO` & `tencentcloud-sdk-python-mps-3.0.871/tencentcloud_sdk_python_mps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mps
-Version: 3.0.870
+Version: 3.0.871
 Summary: Tencent Cloud Mps SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mps-3.0.870/README.rst` & `tencentcloud-sdk-python-mps-3.0.871/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mps-3.0.870/setup.py` & `tencentcloud-sdk-python-mps-3.0.871/setup.py`

 * *Files identical despite different names*

