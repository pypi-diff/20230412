# Comparing `tmp/tencentcloud-sdk-python-cwp-3.0.870.tar.gz` & `tmp/tencentcloud-sdk-python-cwp-3.0.871.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cwp-3.0.870.tar", last modified: Tue Apr 11 03:28:19 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cwp-3.0.871.tar", last modified: Wed Apr 12 00:21:30 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cwp-3.0.870.tar` & `tencentcloud-sdk-python-cwp-3.0.871.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/tencentcloud/cwp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/tencentcloud/cwp/v20180228/
--rw-r--r--   0 root         (0) root         (0)   900743 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/tencentcloud/cwp/v20180228/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/tencentcloud/cwp/v20180228/__init__.py
--rw-r--r--   0 root         (0) root         (0)   250501 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/tencentcloud/cwp/v20180228/cwp_client.py
--rw-r--r--   0 root         (0) root         (0)     3900 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/tencentcloud/cwp/v20180228/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/tencentcloud/cwp/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/tencentcloud_sdk_python_cwp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/tencentcloud_sdk_python_cwp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/tencentcloud_sdk_python_cwp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/tencentcloud_sdk_python_cwp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:21:30.000000 tencentcloud-sdk-python-cwp-3.0.871/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-12 00:21:30.000000 tencentcloud-sdk-python-cwp-3.0.871/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:21:30.000000 tencentcloud-sdk-python-cwp-3.0.871/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:21:30.000000 tencentcloud-sdk-python-cwp-3.0.871/tencentcloud/cwp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:21:30.000000 tencentcloud-sdk-python-cwp-3.0.871/tencentcloud/cwp/v20180228/
+-rw-r--r--   0 root         (0) root         (0)   901450 2023-04-12 00:21:30.000000 tencentcloud-sdk-python-cwp-3.0.871/tencentcloud/cwp/v20180228/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:21:30.000000 tencentcloud-sdk-python-cwp-3.0.871/tencentcloud/cwp/v20180228/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   250501 2023-04-12 00:21:30.000000 tencentcloud-sdk-python-cwp-3.0.871/tencentcloud/cwp/v20180228/cwp_client.py
+-rw-r--r--   0 root         (0) root         (0)     3900 2023-04-12 00:21:30.000000 tencentcloud-sdk-python-cwp-3.0.871/tencentcloud/cwp/v20180228/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:21:30.000000 tencentcloud-sdk-python-cwp-3.0.871/tencentcloud/cwp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-12 00:21:30.000000 tencentcloud-sdk-python-cwp-3.0.871/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-12 00:21:30.000000 tencentcloud-sdk-python-cwp-3.0.871/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:21:30.000000 tencentcloud-sdk-python-cwp-3.0.871/tencentcloud_sdk_python_cwp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-12 00:21:30.000000 tencentcloud-sdk-python-cwp-3.0.871/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 00:21:30.000000 tencentcloud-sdk-python-cwp-3.0.871/tencentcloud_sdk_python_cwp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-12 00:21:30.000000 tencentcloud-sdk-python-cwp-3.0.871/tencentcloud_sdk_python_cwp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-12 00:21:30.000000 tencentcloud-sdk-python-cwp-3.0.871/tencentcloud_sdk_python_cwp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-12 00:21:30.000000 tencentcloud-sdk-python-cwp-3.0.871/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-12 00:21:30.000000 tencentcloud-sdk-python-cwp-3.0.871/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.870/PKG-INFO` & `tencentcloud-sdk-python-cwp-3.0.871/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cwp
-Version: 3.0.870
+Version: 3.0.871
 Summary: Tencent Cloud Cwp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.870/tencentcloud/cwp/v20180228/models.py` & `tencentcloud-sdk-python-cwp-3.0.871/tencentcloud/cwp/v20180228/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -11600,40 +11600,48 @@
 
     """
 
     def __init__(self):
         r"""
         :param Limit: 返回数量，默认为10，最大值为100。
         :type Limit: int
-        :param Offset: 偏移量，默认为0。
-        :type Offset: int
         :param Filters: 过滤条件。
-<li>Keywords - String - 是否必填：否 - 关键词(主机内网IP)</li>
+<li>HostName - String - 是否必填：否 - 主机名</li>
+<li>Hostip - String - 是否必填：否 - 主机内网IP</li>
+<li>RuleCategory - Int - 是否必填：否 - 策略类型,全部或者单选(0:系统 1:用户)</li>
+<li>RuleName - String - 是否必填：否 - 策略名称</li>
+<li>RuleLevel - Int - 是否必填：否 - 威胁等级,可以多选</li>
+<li>Status - Int - 是否必填：否 - 处理状态,可多选(0:待处理 1:已处理 2:已加白  3:已忽略 4:已删除 5:已拦截)</li>
+<li>DetectBy - Int - 是否必填：否 - 数据来源,可多选(0:bash日志 1:实时监控)</li>
+<li>StartTime - String - 是否必填：否 - 开始时间</li>
+<li>EndTime - String - 是否必填：否 - 结束时间</li>
         :type Filters: list of Filter
+        :param Offset: 偏移量，默认为0。
+        :type Offset: int
         :param Order: 排序方式：根据请求次数排序：asc-升序/desc-降序
         :type Order: str
         :param By: 排序字段：CreateTime-发生时间。ModifyTime-处理时间
         :type By: str
         """
         self.Limit = None
-        self.Offset = None
         self.Filters = None
+        self.Offset = None
         self.Order = None
         self.By = None
 
 
     def _deserialize(self, params):
         self.Limit = params.get("Limit")
-        self.Offset = params.get("Offset")
         if params.get("Filters") is not None:
             self.Filters = []
             for item in params.get("Filters"):
                 obj = Filter()
                 obj._deserialize(item)
                 self.Filters.append(obj)
+        self.Offset = params.get("Offset")
         self.Order = params.get("Order")
         self.By = params.get("By")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
@@ -11752,15 +11760,15 @@
         r"""
         :param Limit: 需要返回的数量，最大值为100
         :type Limit: int
         :param Offset: 偏移量，默认为0。
         :type Offset: int
         :param Filters: 过滤条件。
 <li>IpOrAlias - String - 是否必填：否 - 主机ip或别名筛选</li>
-<li>Uuid - String - 是否必填：否 - 云镜唯一Uuid</li>
+<li>Uuid - String - 是否必填：否 - 主机安全唯一Uuid</li>
 <li>Quuid - String - 是否必填：否 - 云服务器uuid</li>
 <li>Status - String - 是否必填：否 - 状态筛选：失败：FAILED 成功：SUCCESS</li>
 <li>UserName - String - 是否必填：否 - UserName筛选</li>
 <li>SrcIp - String - 是否必填：否 - 来源ip筛选</li>
 <li>CreateBeginTime - String - 是否必填：否 - 首次攻击时间筛选，开始时间</li>
 <li>CreateEndTime - String - 是否必填：否 - 首次攻击时间筛选，结束时间</li>
 <li>ModifyBeginTime - String - 是否必填：否 - 最近攻击时间筛选，开始时间</li>
@@ -12804,15 +12812,15 @@
         r"""
         :param Limit: 需要返回的数量，最大值为100
         :type Limit: int
         :param Offset: 偏移量，默认为0。
         :type Offset: int
         :param Filters: 过滤条件。
 <li>IpOrAlias - String - 是否必填：否 - 主机ip或别名筛选</li>
-<li>Uuid - String - 是否必填：否 - 云镜唯一Uuid</li>
+<li>Uuid - String - 是否必填：否 - 主机安全唯一Uuid</li>
 <li>Quuid - String - 是否必填：否 - 云服务器uuid</li>
 <li>UserName - String - 是否必填：否 - 用户名筛选</li>
 <li>LoginTimeBegin - String - 是否必填：否 - 按照修改时间段筛选，开始时间</li>
 <li>LoginTimeEnd - String - 是否必填：否 - 按照修改时间段筛选，结束时间</li>
 <li>SrcIp - String - 是否必填：否 - 来源ip筛选</li>
 <li>Status - int - 是否必填：否 - 状态筛选1:正常登录；5：已加白,14:已处理，15：已忽略</li>
 <li>RiskLevel - int - 是否必填：否 - 状态筛选0:高危；1：可疑</li>
@@ -14976,15 +14984,15 @@
 class DescribeProVersionStatusRequest(AbstractModel):
     """DescribeProVersionStatus请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Uuid: 云镜客户端UUID、填写"all"表示所有主机。
+        :param Uuid: 主机安全客户端UUID、填写"all"表示所有主机。
         :type Uuid: str
         """
         self.Uuid = None
 
 
     def _deserialize(self, params):
         self.Uuid = params.get("Uuid")
@@ -21183,19 +21191,19 @@
         :type MachineName: str
         :param MachineWanIp: 机器公网IP
         :type MachineWanIp: str
         :param MachineIp: 机器内网IP
         :type MachineIp: str
         :param Quuid: 云服务器UUID
         :type Quuid: str
-        :param Uuid: 云镜客户端UUID
+        :param Uuid: 主机安全客户端UUID
         :type Uuid: str
         :param Tags: 标签信息
         :type Tags: list of str
-        :param AgentStatus: 云镜客户端状态,OFFLINE 离线,ONLINE 在线,UNINSTALL 未安装
+        :param AgentStatus: 主机安全客户端状态,OFFLINE 离线,ONLINE 在线,UNINSTALL 未安装
         :type AgentStatus: str
         :param IsUnBind: 是否允许解绑,false 不允许解绑
         :type IsUnBind: bool
         :param IsSwitchBind: 是否允许换绑,false 不允许换绑
         :type IsSwitchBind: bool
         :param MachineExtraInfo: 主机额外信息
 注意：此字段可能返回 null，表示取不到有效值。
@@ -23304,15 +23312,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param Id: 数据ID
         :type Id: int
-        :param Uuid: 云镜ID
+        :param Uuid: 主机安全ID
         :type Uuid: str
         :param Quuid: 主机ID
         :type Quuid: str
         :param Hostip: 主机内网IP
         :type Hostip: str
         :param ProcessName: 进程名
         :type ProcessName: str
@@ -24156,15 +24164,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param Id: ID 主键
         :type Id: int
-        :param Uuid: 云镜UUID
+        :param Uuid: 主机安全UUID
         :type Uuid: str
         :param Quuid: 主机ID
         :type Quuid: str
         :param Hostip: 主机内网IP
         :type Hostip: str
         :param DstIp: 目标IP
         :type DstIp: str
@@ -25121,15 +25129,15 @@
 class SecurityDynamic(AbstractModel):
     """安全事件消息数据。
 
     """
 
     def __init__(self):
         r"""
-        :param Uuid: 云镜客户端UUID。
+        :param Uuid: 主机安全客户端UUID。
         :type Uuid: str
         :param EventTime: 安全事件发生时间。
         :type EventTime: str
         :param EventType: 安全事件类型。
 <li>MALWARE：木马事件</li>
 <li>NON_LOCAL_LOGIN：异地登录</li>
 <li>BRUTEATTACK_SUCCESS：密码破解成功</li>
@@ -26048,15 +26056,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param Id: ID。
         :type Id: int
-        :param Uuid: 云镜客户端唯一标识UUID。
+        :param Uuid: 主机安全客户端唯一标识UUID。
         :type Uuid: str
         :param CountryId: 国家 ID。
         :type CountryId: int
         :param ProvinceId: 省份 ID。
         :type ProvinceId: int
         :param CityId: 城市 ID。
         :type CityId: int
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.870/tencentcloud/cwp/v20180228/cwp_client.py` & `tencentcloud-sdk-python-cwp-3.0.871/tencentcloud/cwp/v20180228/cwp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cwp-3.0.870/tencentcloud/cwp/v20180228/errorcodes.py` & `tencentcloud-sdk-python-cwp-3.0.871/tencentcloud/cwp/v20180228/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cwp-3.0.870/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cwp-3.0.871/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cwp-3.0.870/README.rst` & `tencentcloud-sdk-python-cwp-3.0.871/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cwp-3.0.870/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cwp-3.0.871/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cwp
-Version: 3.0.870
+Version: 3.0.871
 Summary: Tencent Cloud Cwp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.870/setup.py` & `tencentcloud-sdk-python-cwp-3.0.871/setup.py`

 * *Files identical despite different names*

