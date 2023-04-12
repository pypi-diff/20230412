# Comparing `tmp/tencentcloud-sdk-python-vrs-3.0.870.tar.gz` & `tmp/tencentcloud-sdk-python-vrs-3.0.871.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vrs-3.0.870.tar", last modified: Tue Apr 11 04:04:03 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vrs-3.0.871.tar", last modified: Wed Apr 12 00:47:22 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vrs-3.0.870.tar` & `tencentcloud-sdk-python-vrs-3.0.871.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 04:04:03.000000 tencentcloud-sdk-python-vrs-3.0.870/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 04:04:03.000000 tencentcloud-sdk-python-vrs-3.0.870/tencentcloud_sdk_python_vrs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-11 04:04:03.000000 tencentcloud-sdk-python-vrs-3.0.870/tencentcloud_sdk_python_vrs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 04:04:03.000000 tencentcloud-sdk-python-vrs-3.0.870/tencentcloud_sdk_python_vrs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-11 04:04:03.000000 tencentcloud-sdk-python-vrs-3.0.870/tencentcloud_sdk_python_vrs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-11 04:04:03.000000 tencentcloud-sdk-python-vrs-3.0.870/tencentcloud_sdk_python_vrs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-11 04:04:03.000000 tencentcloud-sdk-python-vrs-3.0.870/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 04:04:03.000000 tencentcloud-sdk-python-vrs-3.0.870/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 04:04:03.000000 tencentcloud-sdk-python-vrs-3.0.870/tencentcloud/vrs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 04:04:03.000000 tencentcloud-sdk-python-vrs-3.0.870/tencentcloud/vrs/v20200824/
--rw-r--r--   0 root         (0) root         (0)    15014 2023-04-11 04:04:03.000000 tencentcloud-sdk-python-vrs-3.0.870/tencentcloud/vrs/v20200824/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 04:04:03.000000 tencentcloud-sdk-python-vrs-3.0.870/tencentcloud/vrs/v20200824/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6014 2023-04-11 04:04:03.000000 tencentcloud-sdk-python-vrs-3.0.870/tencentcloud/vrs/v20200824/vrs_client.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-04-11 04:04:03.000000 tencentcloud-sdk-python-vrs-3.0.870/tencentcloud/vrs/v20200824/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 04:04:03.000000 tencentcloud-sdk-python-vrs-3.0.870/tencentcloud/vrs/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-11 04:04:03.000000 tencentcloud-sdk-python-vrs-3.0.870/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-11 04:04:03.000000 tencentcloud-sdk-python-vrs-3.0.870/README.rst
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-11 04:04:03.000000 tencentcloud-sdk-python-vrs-3.0.870/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-11 04:04:03.000000 tencentcloud-sdk-python-vrs-3.0.870/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:47:22.000000 tencentcloud-sdk-python-vrs-3.0.871/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:47:22.000000 tencentcloud-sdk-python-vrs-3.0.871/tencentcloud_sdk_python_vrs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-12 00:47:22.000000 tencentcloud-sdk-python-vrs-3.0.871/tencentcloud_sdk_python_vrs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 00:47:22.000000 tencentcloud-sdk-python-vrs-3.0.871/tencentcloud_sdk_python_vrs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-12 00:47:22.000000 tencentcloud-sdk-python-vrs-3.0.871/tencentcloud_sdk_python_vrs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-12 00:47:22.000000 tencentcloud-sdk-python-vrs-3.0.871/tencentcloud_sdk_python_vrs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-12 00:47:22.000000 tencentcloud-sdk-python-vrs-3.0.871/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:47:22.000000 tencentcloud-sdk-python-vrs-3.0.871/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:47:22.000000 tencentcloud-sdk-python-vrs-3.0.871/tencentcloud/vrs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:47:22.000000 tencentcloud-sdk-python-vrs-3.0.871/tencentcloud/vrs/v20200824/
+-rw-r--r--   0 root         (0) root         (0)    15237 2023-04-12 00:47:22.000000 tencentcloud-sdk-python-vrs-3.0.871/tencentcloud/vrs/v20200824/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:47:22.000000 tencentcloud-sdk-python-vrs-3.0.871/tencentcloud/vrs/v20200824/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5710 2023-04-12 00:47:22.000000 tencentcloud-sdk-python-vrs-3.0.871/tencentcloud/vrs/v20200824/vrs_client.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-04-12 00:47:22.000000 tencentcloud-sdk-python-vrs-3.0.871/tencentcloud/vrs/v20200824/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:47:22.000000 tencentcloud-sdk-python-vrs-3.0.871/tencentcloud/vrs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-12 00:47:22.000000 tencentcloud-sdk-python-vrs-3.0.871/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-12 00:47:22.000000 tencentcloud-sdk-python-vrs-3.0.871/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-12 00:47:22.000000 tencentcloud-sdk-python-vrs-3.0.871/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-12 00:47:22.000000 tencentcloud-sdk-python-vrs-3.0.871/setup.cfg
```

### Comparing `tencentcloud-sdk-python-vrs-3.0.870/tencentcloud_sdk_python_vrs.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vrs-3.0.871/tencentcloud_sdk_python_vrs.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vrs
-Version: 3.0.870
+Version: 3.0.871
 Summary: Tencent Cloud Vrs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vrs-3.0.870/PKG-INFO` & `tencentcloud-sdk-python-vrs-3.0.871/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vrs
-Version: 3.0.870
+Version: 3.0.871
 Summary: Tencent Cloud Vrs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vrs-3.0.870/tencentcloud/vrs/v20200824/models.py` & `tencentcloud-sdk-python-vrs-3.0.871/tencentcloud/vrs/v20200824/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,16 @@
 
 1-中文（默认）
         :type VoiceLanguage: int
         :param Codec: 音频格式，音频类型(wav,mp3,aac,m4a)
         :type Codec: str
         :param AudioIdList: 音频ID集合
         :type AudioIdList: list of str
-        :param CallbackUrl: 回调 URL，用户自行搭建的用于接收识别结果的服务URL。如果用户使用轮询方式获取识别结果，则无需提交该参数。
+        :param CallbackUrl: 回调 URL，用户自行搭建的用于接收结果的服务URL。如果用户使用轮询方式获取识别结果，则无需提交该参数。
+回调采用POST请求方式，Content-Type为application/x-www-form-urlencoded，回调数据格式如下:callback_body=checksum=&data={"TaskId":"xxxxxxxxxxxxxx","Status":2,"StatusStr":"success","VoiceType":xxxxx,"ErrorMsg":""}
         :type CallbackUrl: str
         """
         self.SessionId = None
         self.VoiceName = None
         self.SampleRate = None
         self.VoiceGender = None
         self.VoiceLanguage = None
```

### Comparing `tencentcloud-sdk-python-vrs-3.0.870/tencentcloud/vrs/v20200824/vrs_client.py` & `tencentcloud-sdk-python-vrs-3.0.871/tencentcloud/vrs/v20200824/vrs_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     _service = 'vrs'
 
 
     def CreateVRSTask(self, request):
         """本接口服务对提交音频进行声音复刻任务创建接口，异步返回复刻结果。
         • 请求方法为 HTTP POST , Content-Type为"application/json; charset=utf-8"
         • 签名方法参考 公共参数 中签名方法v3。
-        • 默认接口请求频率限制：30次/秒，
 
         :param request: Request instance for CreateVRSTask.
         :type request: :class:`tencentcloud.vrs.v20200824.models.CreateVRSTaskRequest`
         :rtype: :class:`tencentcloud.vrs.v20200824.models.CreateVRSTaskResponse`
 
         """
         try:
@@ -54,15 +53,14 @@
 
     def DescribeVRSTaskStatus(self, request):
         """在调用声音复刻创建任务请求接口后，有回调和轮询两种方式获取识别结果。
         • 当采用回调方式时，识别完成后会将结果通过 POST 请求的形式通知到用户在请求时填写的回调 URL，具体请参见 声音复刻结果回调 。
         • 当采用轮询方式时，需要主动提交任务ID来轮询识别结果，共有任务成功、等待、执行中和失败四种结果，具体信息请参见下文说明。
         • 请求方法为 HTTP POST , Content-Type为"application/json; charset=utf-8"
         • 签名方法参考 公共参数 中签名方法v3。
-        • 默认接口请求频率限制：20次/秒，如您有提高请求频率限制的需求，请提工单进行咨询。
 
         :param request: Request instance for DescribeVRSTaskStatus.
         :type request: :class:`tencentcloud.vrs.v20200824.models.DescribeVRSTaskStatusRequest`
         :rtype: :class:`tencentcloud.vrs.v20200824.models.DescribeVRSTaskStatusResponse`
 
         """
         try:
@@ -80,15 +78,14 @@
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DetectEnvAndSoundQuality(self, request):
         """本接口用于检测音频的环境和音频质量。
         • 请求方法为 HTTP POST , Content-Type为"application/json; charset=utf-8"
         • 签名方法参考 公共参数 中签名方法v3。
-        • 默认接口请求频率限制：20次/秒。
 
         :param request: Request instance for DetectEnvAndSoundQuality.
         :type request: :class:`tencentcloud.vrs.v20200824.models.DetectEnvAndSoundQualityRequest`
         :rtype: :class:`tencentcloud.vrs.v20200824.models.DetectEnvAndSoundQualityResponse`
 
         """
         try:
@@ -106,15 +103,14 @@
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def GetTrainingText(self, request):
         """本接口用于获取声音复刻训练文本信息。
          请求方法为 HTTP POST , Content-Type为"application/json; charset=utf-8"
         • 签名方法参考 公共参数 中签名方法v3。
-        • 默认接口请求频率限制：20次/秒。
 
         :param request: Request instance for GetTrainingText.
         :type request: :class:`tencentcloud.vrs.v20200824.models.GetTrainingTextRequest`
         :rtype: :class:`tencentcloud.vrs.v20200824.models.GetTrainingTextResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-vrs-3.0.870/tencentcloud/vrs/v20200824/errorcodes.py` & `tencentcloud-sdk-python-vrs-3.0.871/tencentcloud/vrs/v20200824/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vrs-3.0.870/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vrs-3.0.871/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vrs-3.0.870/README.rst` & `tencentcloud-sdk-python-vrs-3.0.871/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vrs-3.0.870/setup.py` & `tencentcloud-sdk-python-vrs-3.0.871/setup.py`

 * *Files identical despite different names*

