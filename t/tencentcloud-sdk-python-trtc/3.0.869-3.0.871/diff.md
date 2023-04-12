# Comparing `tmp/tencentcloud-sdk-python-trtc-3.0.869.tar.gz` & `tmp/tencentcloud-sdk-python-trtc-3.0.871.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-trtc-3.0.869.tar", last modified: Mon Apr 10 03:17:27 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-trtc-3.0.871.tar", last modified: Wed Apr 12 00:45:29 2023, max compression
```

## Comparing `tencentcloud-sdk-python-trtc-3.0.869.tar` & `tencentcloud-sdk-python-trtc-3.0.871.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/tencentcloud/trtc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/tencentcloud/trtc/v20190722/
--rw-r--r--   0 root         (0) root         (0)   198735 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/tencentcloud/trtc/v20190722/models.py
--rw-r--r--   0 root         (0) root         (0)    58128 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/tencentcloud/trtc/v20190722/trtc_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/tencentcloud/trtc/v20190722/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9679 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/tencentcloud/trtc/v20190722/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/tencentcloud/trtc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/README.rst
--rw-r--r--   0 root         (0) root         (0)     1008 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/tencentcloud_sdk_python_trtc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/tencentcloud_sdk_python_trtc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/tencentcloud_sdk_python_trtc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/tencentcloud_sdk_python_trtc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-10 03:17:27.000000 tencentcloud-sdk-python-trtc-3.0.869/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:45:29.000000 tencentcloud-sdk-python-trtc-3.0.871/
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-12 00:45:29.000000 tencentcloud-sdk-python-trtc-3.0.871/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:45:29.000000 tencentcloud-sdk-python-trtc-3.0.871/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:45:29.000000 tencentcloud-sdk-python-trtc-3.0.871/tencentcloud/trtc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:45:29.000000 tencentcloud-sdk-python-trtc-3.0.871/tencentcloud/trtc/v20190722/
+-rw-r--r--   0 root         (0) root         (0)   198775 2023-04-12 00:45:29.000000 tencentcloud-sdk-python-trtc-3.0.871/tencentcloud/trtc/v20190722/models.py
+-rw-r--r--   0 root         (0) root         (0)    58128 2023-04-12 00:45:29.000000 tencentcloud-sdk-python-trtc-3.0.871/tencentcloud/trtc/v20190722/trtc_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:45:29.000000 tencentcloud-sdk-python-trtc-3.0.871/tencentcloud/trtc/v20190722/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9679 2023-04-12 00:45:29.000000 tencentcloud-sdk-python-trtc-3.0.871/tencentcloud/trtc/v20190722/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:45:29.000000 tencentcloud-sdk-python-trtc-3.0.871/tencentcloud/trtc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-12 00:45:29.000000 tencentcloud-sdk-python-trtc-3.0.871/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-12 00:45:29.000000 tencentcloud-sdk-python-trtc-3.0.871/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-04-12 00:45:29.000000 tencentcloud-sdk-python-trtc-3.0.871/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:45:29.000000 tencentcloud-sdk-python-trtc-3.0.871/tencentcloud_sdk_python_trtc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-12 00:45:29.000000 tencentcloud-sdk-python-trtc-3.0.871/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 00:45:29.000000 tencentcloud-sdk-python-trtc-3.0.871/tencentcloud_sdk_python_trtc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-12 00:45:29.000000 tencentcloud-sdk-python-trtc-3.0.871/tencentcloud_sdk_python_trtc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-04-12 00:45:29.000000 tencentcloud-sdk-python-trtc-3.0.871/tencentcloud_sdk_python_trtc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-12 00:45:29.000000 tencentcloud-sdk-python-trtc-3.0.871/setup.cfg
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.869/PKG-INFO` & `tencentcloud-sdk-python-trtc-3.0.871/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trtc
-Version: 3.0.869
+Version: 3.0.871
 Summary: Tencent Cloud Trtc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.869/tencentcloud/trtc/v20190722/models.py` & `tencentcloud-sdk-python-trtc-3.0.871/tencentcloud/trtc/v20190722/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1175,15 +1175,15 @@
         r"""
         :param SdkAppId: 用户SdkAppId（如：1400xxxxxx）
         :type SdkAppId: int
         :param StartTime: 查询开始时间，本地unix时间戳，单位为秒（如：1590065777）
 注意：支持查询14天内的数据。
         :type StartTime: int
         :param EndTime: 查询结束时间，本地unix时间戳，单位为秒（如：1590065877），建议与StartTime间隔时间超过24小时。
-注意：按天统计，结束时间小于前一天，否则查询数据为空（如：需查询20号数据，结束时间需小于20号0点）。
+注意：按天统计，结束时间小于前一天，否则查询数据为空（如：需查询20号数据，结束时间需晚于20号0点）。
         :type EndTime: int
         """
         self.SdkAppId = None
         self.StartTime = None
         self.EndTime = None
 
 
@@ -4320,17 +4320,17 @@
 class StorageParams(AbstractModel):
     """第三方存储参数。
 
     """
 
     def __init__(self):
         r"""
-        :param CloudStorage: 第三方云存储的账号信息（CloudStorage参数暂不可用，请使用CloudVod参数存储至云点播）。
+        :param CloudStorage: 第三方云存储的账号信息（特别说明：若您选择存储至对象存储COS将会收取录制文件投递至COS的费用，详见云端录制收费说明，存储至VOD将不收取此项费用。）。
         :type CloudStorage: :class:`tencentcloud.trtc.v20190722.models.CloudStorage`
-        :param CloudVod: 【必填】腾讯云云点播的账号信息，目前仅支持存储至腾讯云点播VOD。
+        :param CloudVod: 腾讯云云点播的账号信息。
         :type CloudVod: :class:`tencentcloud.trtc.v20190722.models.CloudVod`
         """
         self.CloudStorage = None
         self.CloudVod = None
 
 
     def _deserialize(self, params):
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.869/tencentcloud/trtc/v20190722/trtc_client.py` & `tencentcloud-sdk-python-trtc-3.0.871/tencentcloud/trtc/v20190722/trtc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.869/tencentcloud/trtc/v20190722/errorcodes.py` & `tencentcloud-sdk-python-trtc-3.0.871/tencentcloud/trtc/v20190722/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.869/tencentcloud/__init__.py` & `tencentcloud-sdk-python-trtc-3.0.871/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-trtc-3.0.869/README.rst` & `tencentcloud-sdk-python-trtc-3.0.871/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.869/setup.py` & `tencentcloud-sdk-python-trtc-3.0.871/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.869/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-trtc-3.0.871/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trtc
-Version: 3.0.869
+Version: 3.0.871
 Summary: Tencent Cloud Trtc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

