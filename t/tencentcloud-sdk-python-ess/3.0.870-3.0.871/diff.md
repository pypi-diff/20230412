# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.870.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.871.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.870.tar", last modified: Tue Apr 11 03:38:34 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.871.tar", last modified: Wed Apr 12 00:24:30 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.870.tar` & `tencentcloud-sdk-python-ess-3.0.871.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/tencentcloud/ess/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    47026 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)   212239 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/tencentcloud/ess/v20201111/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23577 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/README.rst
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:24:30.000000 tencentcloud-sdk-python-ess-3.0.871/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-12 00:24:30.000000 tencentcloud-sdk-python-ess-3.0.871/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:24:30.000000 tencentcloud-sdk-python-ess-3.0.871/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-12 00:24:29.000000 tencentcloud-sdk-python-ess-3.0.871/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:24:30.000000 tencentcloud-sdk-python-ess-3.0.871/tencentcloud/ess/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:24:30.000000 tencentcloud-sdk-python-ess-3.0.871/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    47026 2023-04-12 00:24:29.000000 tencentcloud-sdk-python-ess-3.0.871/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)   212473 2023-04-12 00:24:29.000000 tencentcloud-sdk-python-ess-3.0.871/tencentcloud/ess/v20201111/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:24:29.000000 tencentcloud-sdk-python-ess-3.0.871/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23577 2023-04-12 00:24:29.000000 tencentcloud-sdk-python-ess-3.0.871/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:24:29.000000 tencentcloud-sdk-python-ess-3.0.871/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:24:30.000000 tencentcloud-sdk-python-ess-3.0.871/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-12 00:24:30.000000 tencentcloud-sdk-python-ess-3.0.871/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 00:24:30.000000 tencentcloud-sdk-python-ess-3.0.871/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-12 00:24:30.000000 tencentcloud-sdk-python-ess-3.0.871/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-12 00:24:30.000000 tencentcloud-sdk-python-ess-3.0.871/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-12 00:24:29.000000 tencentcloud-sdk-python-ess-3.0.871/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-12 00:24:29.000000 tencentcloud-sdk-python-ess-3.0.871/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-12 00:24:30.000000 tencentcloud-sdk-python-ess-3.0.871/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ess-3.0.870/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.871/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.870
+Version: 3.0.871
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.870/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.871/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.870/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.871/tencentcloud/ess/v20201111/ess_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.870/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.871/tencentcloud/ess/v20201111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5397,14 +5397,16 @@
         :type Status: int
         :param Creator: 模板的创建人
         :type Creator: str
         :param CreatedOn: 模板创建的时间戳（精确到秒）
         :type CreatedOn: int
         :param Promoter: 发起人角色信息
         :type Promoter: :class:`tencentcloud.ess.v20201111.models.Recipient`
+        :param Available: 模板可用状态，取值：0未知，但默认会被转成启用；1启用（默认），2停用
+        :type Available: int
         :param OrganizationId: 模板创建组织id
         :type OrganizationId: str
         :param PreviewUrl: 模板预览链接
 注意：此字段可能返回 null，表示取不到有效值。
         :type PreviewUrl: str
         :param TemplateVersion: 模板版本。默认为空时，全数字字符，初始版本为yyyyMMdd001。
 注意：此字段可能返回 null，表示取不到有效值。
@@ -5423,14 +5425,15 @@
         self.Recipients = None
         self.Components = None
         self.SignComponents = None
         self.Status = None
         self.Creator = None
         self.CreatedOn = None
         self.Promoter = None
+        self.Available = None
         self.OrganizationId = None
         self.PreviewUrl = None
         self.TemplateVersion = None
         self.Published = None
 
 
     def _deserialize(self, params):
@@ -5466,14 +5469,15 @@
                 self.SignComponents.append(obj)
         self.Status = params.get("Status")
         self.Creator = params.get("Creator")
         self.CreatedOn = params.get("CreatedOn")
         if params.get("Promoter") is not None:
             self.Promoter = Recipient()
             self.Promoter._deserialize(params.get("Promoter"))
+        self.Available = params.get("Available")
         self.OrganizationId = params.get("OrganizationId")
         self.PreviewUrl = params.get("PreviewUrl")
         self.TemplateVersion = params.get("TemplateVersion")
         self.Published = params.get("Published")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
```

### Comparing `tencentcloud-sdk-python-ess-3.0.870/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.871/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.870/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.871/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.870
+Version: 3.0.871
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.870/README.rst` & `tencentcloud-sdk-python-ess-3.0.871/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.870/setup.py` & `tencentcloud-sdk-python-ess-3.0.871/setup.py`

 * *Files identical despite different names*

