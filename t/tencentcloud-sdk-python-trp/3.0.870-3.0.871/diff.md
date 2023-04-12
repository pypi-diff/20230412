# Comparing `tmp/tencentcloud-sdk-python-trp-3.0.870.tar.gz` & `tmp/tencentcloud-sdk-python-trp-3.0.871.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-trp-3.0.870.tar", last modified: Tue Apr 11 03:57:39 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-trp-3.0.871.tar", last modified: Wed Apr 12 00:45:16 2023, max compression
```

## Comparing `tencentcloud-sdk-python-trp-3.0.870.tar` & `tencentcloud-sdk-python-trp-3.0.871.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:57:39.000000 tencentcloud-sdk-python-trp-3.0.870/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-11 03:57:39.000000 tencentcloud-sdk-python-trp-3.0.870/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:57:39.000000 tencentcloud-sdk-python-trp-3.0.870/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-11 03:57:39.000000 tencentcloud-sdk-python-trp-3.0.870/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:57:39.000000 tencentcloud-sdk-python-trp-3.0.870/tencentcloud/trp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:57:39.000000 tencentcloud-sdk-python-trp-3.0.870/tencentcloud/trp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:57:39.000000 tencentcloud-sdk-python-trp-3.0.870/tencentcloud/trp/v20210515/
--rw-r--r--   0 root         (0) root         (0)   130844 2023-04-11 03:57:39.000000 tencentcloud-sdk-python-trp-3.0.870/tencentcloud/trp/v20210515/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:57:39.000000 tencentcloud-sdk-python-trp-3.0.870/tencentcloud/trp/v20210515/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39990 2023-04-11 03:57:39.000000 tencentcloud-sdk-python-trp-3.0.870/tencentcloud/trp/v20210515/trp_client.py
--rw-r--r--   0 root         (0) root         (0)      992 2023-04-11 03:57:39.000000 tencentcloud-sdk-python-trp-3.0.870/tencentcloud/trp/v20210515/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:57:39.000000 tencentcloud-sdk-python-trp-3.0.870/tencentcloud_sdk_python_trp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-11 03:57:39.000000 tencentcloud-sdk-python-trp-3.0.870/tencentcloud_sdk_python_trp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 03:57:39.000000 tencentcloud-sdk-python-trp-3.0.870/tencentcloud_sdk_python_trp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-11 03:57:39.000000 tencentcloud-sdk-python-trp-3.0.870/tencentcloud_sdk_python_trp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-11 03:57:39.000000 tencentcloud-sdk-python-trp-3.0.870/tencentcloud_sdk_python_trp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-11 03:57:39.000000 tencentcloud-sdk-python-trp-3.0.870/README.rst
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-11 03:57:39.000000 tencentcloud-sdk-python-trp-3.0.870/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-11 03:57:39.000000 tencentcloud-sdk-python-trp-3.0.870/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:45:16.000000 tencentcloud-sdk-python-trp-3.0.871/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-12 00:45:16.000000 tencentcloud-sdk-python-trp-3.0.871/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:45:16.000000 tencentcloud-sdk-python-trp-3.0.871/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-12 00:45:15.000000 tencentcloud-sdk-python-trp-3.0.871/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:45:16.000000 tencentcloud-sdk-python-trp-3.0.871/tencentcloud/trp/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:45:15.000000 tencentcloud-sdk-python-trp-3.0.871/tencentcloud/trp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:45:16.000000 tencentcloud-sdk-python-trp-3.0.871/tencentcloud/trp/v20210515/
+-rw-r--r--   0 root         (0) root         (0)   130963 2023-04-12 00:45:15.000000 tencentcloud-sdk-python-trp-3.0.871/tencentcloud/trp/v20210515/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:45:15.000000 tencentcloud-sdk-python-trp-3.0.871/tencentcloud/trp/v20210515/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39990 2023-04-12 00:45:15.000000 tencentcloud-sdk-python-trp-3.0.871/tencentcloud/trp/v20210515/trp_client.py
+-rw-r--r--   0 root         (0) root         (0)      992 2023-04-12 00:45:15.000000 tencentcloud-sdk-python-trp-3.0.871/tencentcloud/trp/v20210515/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:45:16.000000 tencentcloud-sdk-python-trp-3.0.871/tencentcloud_sdk_python_trp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-12 00:45:15.000000 tencentcloud-sdk-python-trp-3.0.871/tencentcloud_sdk_python_trp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 00:45:15.000000 tencentcloud-sdk-python-trp-3.0.871/tencentcloud_sdk_python_trp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-12 00:45:15.000000 tencentcloud-sdk-python-trp-3.0.871/tencentcloud_sdk_python_trp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-12 00:45:16.000000 tencentcloud-sdk-python-trp-3.0.871/tencentcloud_sdk_python_trp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-12 00:45:15.000000 tencentcloud-sdk-python-trp-3.0.871/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-12 00:45:15.000000 tencentcloud-sdk-python-trp-3.0.871/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-12 00:45:16.000000 tencentcloud-sdk-python-trp-3.0.871/setup.cfg
```

### Comparing `tencentcloud-sdk-python-trp-3.0.870/PKG-INFO` & `tencentcloud-sdk-python-trp-3.0.871/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trp
-Version: 3.0.870
+Version: 3.0.871
 Summary: Tencent Cloud Trp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trp-3.0.870/tencentcloud/__init__.py` & `tencentcloud-sdk-python-trp-3.0.871/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-trp-3.0.870/tencentcloud/trp/v20210515/models.py` & `tencentcloud-sdk-python-trp-3.0.871/tencentcloud/trp/v20210515/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2401,30 +2401,34 @@
         :type PageNumber: int
         :param MerchantId: 商户ID
         :type MerchantId: str
         :param ProductId: 产品ID
         :type ProductId: str
         :param BatchId: 批次ID
         :type BatchId: str
+        :param Code: 安心码
+        :type Code: str
         """
         self.CorpId = None
         self.PageSize = None
         self.PageNumber = None
         self.MerchantId = None
         self.ProductId = None
         self.BatchId = None
+        self.Code = None
 
 
     def _deserialize(self, params):
         self.CorpId = params.get("CorpId")
         self.PageSize = params.get("PageSize")
         self.PageNumber = params.get("PageNumber")
         self.MerchantId = params.get("MerchantId")
         self.ProductId = params.get("ProductId")
         self.BatchId = params.get("BatchId")
+        self.Code = params.get("Code")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-trp-3.0.870/tencentcloud/trp/v20210515/trp_client.py` & `tencentcloud-sdk-python-trp-3.0.871/tencentcloud/trp/v20210515/trp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trp-3.0.870/tencentcloud/trp/v20210515/errorcodes.py` & `tencentcloud-sdk-python-trp-3.0.871/tencentcloud/trp/v20210515/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trp-3.0.870/tencentcloud_sdk_python_trp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-trp-3.0.871/tencentcloud_sdk_python_trp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trp
-Version: 3.0.870
+Version: 3.0.871
 Summary: Tencent Cloud Trp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trp-3.0.870/README.rst` & `tencentcloud-sdk-python-trp-3.0.871/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trp-3.0.870/setup.py` & `tencentcloud-sdk-python-trp-3.0.871/setup.py`

 * *Files identical despite different names*

