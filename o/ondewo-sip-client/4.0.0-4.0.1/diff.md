# Comparing `tmp/ondewo-sip-client-4.0.0.tar.gz` & `tmp/ondewo-sip-client-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ondewo-sip-client-4.0.0.tar", last modified: Thu Sep 15 08:47:32 2022, max compression
+gzip compressed data, was "ondewo-sip-client-4.0.1.tar", last modified: Wed Apr 12 16:36:38 2023, max compression
```

## Comparing `ondewo-sip-client-4.0.0.tar` & `ondewo-sip-client-4.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 08:47:32.157089 ondewo-sip-client-4.0.0/
--rw-rw-r--   0 root         (0) root         (0)    10257 2022-07-20 06:52:01.000000 ondewo-sip-client-4.0.0/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       71 2022-08-03 07:29:53.000000 ondewo-sip-client-4.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2845 2022-09-15 08:47:32.157089 ondewo-sip-client-4.0.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     2255 2022-09-12 09:23:06.000000 ondewo-sip-client-4.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 08:47:32.153089 ondewo-sip-client-4.0.0/ondewo/
--rw-rw-r--   0 root         (0) root         (0)       81 2022-07-20 06:52:01.000000 ondewo-sip-client-4.0.0/ondewo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 08:47:32.157089 ondewo-sip-client-4.0.0/ondewo/sip/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-07-20 06:52:01.000000 ondewo-sip-client-4.0.0/ondewo/sip/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 08:47:32.157089 ondewo-sip-client-4.0.0/ondewo/sip/client/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-07-20 06:52:01.000000 ondewo-sip-client-4.0.0/ondewo/sip/client/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1294 2022-07-20 06:52:01.000000 ondewo-sip-client-4.0.0/ondewo/sip/client/client.py
--rw-rw-r--   0 root         (0) root         (0)      838 2022-07-20 06:52:01.000000 ondewo-sip-client-4.0.0/ondewo/sip/client/client_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 08:47:32.157089 ondewo-sip-client-4.0.0/ondewo/sip/client/services/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-07-20 06:52:01.000000 ondewo-sip-client-4.0.0/ondewo/sip/client/services/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2767 2022-07-20 06:52:01.000000 ondewo-sip-client-4.0.0/ondewo/sip/client/services/sip.py
--rw-rw-r--   0 root         (0) root         (0)      803 2022-07-20 06:52:01.000000 ondewo-sip-client-4.0.0/ondewo/sip/client/services_container.py
--rw-rw-r--   0 root         (0) root         (0)    10572 2022-09-15 08:47:19.000000 ondewo-sip-client-4.0.0/ondewo/sip/sip_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    19098 2022-09-15 08:47:19.000000 ondewo-sip-client-4.0.0/ondewo/sip/sip_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 08:47:32.157089 ondewo-sip-client-4.0.0/ondewo_sip_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2845 2022-09-15 08:47:32.000000 ondewo-sip-client-4.0.0/ondewo_sip_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      549 2022-09-15 08:47:32.000000 ondewo-sip-client-4.0.0/ondewo_sip_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-15 08:47:32.000000 ondewo-sip-client-4.0.0/ondewo_sip_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      193 2022-09-15 08:47:32.000000 ondewo-sip-client-4.0.0/ondewo_sip_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-09-15 08:47:32.000000 ondewo-sip-client-4.0.0/ondewo_sip_client.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       67 2022-09-15 08:47:32.157089 ondewo-sip-client-4.0.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1002 2022-09-15 08:47:20.000000 ondewo-sip-client-4.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:36:38.699214 ondewo-sip-client-4.0.1/
+-rw-rw-r--   0 root         (0) root         (0)    10257 2023-01-24 18:48:33.000000 ondewo-sip-client-4.0.1/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       71 2023-01-24 18:48:33.000000 ondewo-sip-client-4.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6340 2023-04-12 16:36:38.699214 ondewo-sip-client-4.0.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     5497 2023-01-24 18:48:33.000000 ondewo-sip-client-4.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:36:38.698214 ondewo-sip-client-4.0.1/ondewo/
+-rw-rw-r--   0 root         (0) root         (0)       81 2023-01-24 18:48:33.000000 ondewo-sip-client-4.0.1/ondewo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:36:38.698214 ondewo-sip-client-4.0.1/ondewo/sip/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-01-24 18:48:33.000000 ondewo-sip-client-4.0.1/ondewo/sip/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:36:38.698214 ondewo-sip-client-4.0.1/ondewo/sip/client/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-01-24 18:48:33.000000 ondewo-sip-client-4.0.1/ondewo/sip/client/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1294 2023-01-24 18:48:33.000000 ondewo-sip-client-4.0.1/ondewo/sip/client/client.py
+-rw-rw-r--   0 root         (0) root         (0)      838 2023-04-12 15:48:56.000000 ondewo-sip-client-4.0.1/ondewo/sip/client/client_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:36:38.698214 ondewo-sip-client-4.0.1/ondewo/sip/client/services/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-01-24 18:48:33.000000 ondewo-sip-client-4.0.1/ondewo/sip/client/services/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2825 2023-04-12 15:51:37.000000 ondewo-sip-client-4.0.1/ondewo/sip/client/services/sip.py
+-rw-rw-r--   0 root         (0) root         (0)      803 2023-01-24 18:48:33.000000 ondewo-sip-client-4.0.1/ondewo/sip/client/services_container.py
+-rw-rw-r--   0 root         (0) root         (0)    10572 2023-04-12 16:08:55.000000 ondewo-sip-client-4.0.1/ondewo/sip/sip_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    19098 2023-04-12 16:08:55.000000 ondewo-sip-client-4.0.1/ondewo/sip/sip_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:36:38.698214 ondewo-sip-client-4.0.1/ondewo_sip_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6340 2023-04-12 16:36:38.000000 ondewo-sip-client-4.0.1/ondewo_sip_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      549 2023-04-12 16:36:38.000000 ondewo-sip-client-4.0.1/ondewo_sip_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 16:36:38.000000 ondewo-sip-client-4.0.1/ondewo_sip_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      193 2023-04-12 16:36:38.000000 ondewo-sip-client-4.0.1/ondewo_sip_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-12 16:36:38.000000 ondewo-sip-client-4.0.1/ondewo_sip_client.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)       67 2023-04-12 16:36:38.699214 ondewo-sip-client-4.0.1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1906 2023-04-12 16:08:59.000000 ondewo-sip-client-4.0.1/setup.py
```

### Comparing `ondewo-sip-client-4.0.0/LICENSE` & `ondewo-sip-client-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ondewo-sip-client-4.0.0/ondewo/sip/client/client.py` & `ondewo-sip-client-4.0.1/ondewo/sip/client/client.py`

 * *Files identical despite different names*

### Comparing `ondewo-sip-client-4.0.0/ondewo/sip/client/client_config.py` & `ondewo-sip-client-4.0.1/ondewo/sip/client/client_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 from dataclasses_json import dataclass_json
 from ondewo.utils.base_client_config import BaseClientConfig
 
 
 @dataclass_json
 @dataclass(frozen=True)
 class ClientConfig(BaseClientConfig):
-    """ Config for ONDEWO T2S client. """
+    """ Config for ONDEWO SIP Client. """
```

### Comparing `ondewo-sip-client-4.0.0/ondewo/sip/client/services/sip.py` & `ondewo-sip-client-4.0.1/ondewo/sip/client/services/sip.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from google.protobuf.empty_pb2 import Empty
 from ondewo.utils.base_services_interface import BaseServicesInterface
 
 from ondewo.sip.sip_pb2 import (
-    StartSessionRequest,
-    StartCallRequest,
     EndCallRequest,
-    TransferCallRequest,
-    SipStatus,
-    SipStatusHistoryResponse,
     PlayWavFilesRequest,
     RegisterAccountRequest,
+    SipStatus,
+    SipStatusHistoryResponse,
+    StartCallRequest,
+    StartSessionRequest,
+    TransferCallRequest,
 )
 from ondewo.sip.sip_pb2_grpc import SipStub
 
 
 class Sip(BaseServicesInterface):
     """
     Exposes the sip endpoints of ONDEWO sip in a user-friendly way.
@@ -36,50 +36,50 @@
     """
 
     @property
     def stub(self) -> SipStub:
         stub: SipStub = SipStub(channel=self.grpc_channel)
         return stub
 
-    def start_session(self, request: StartSessionRequest) -> Empty:
-        response: Empty = self.stub.StartSession(request)
+    def start_session(self, request: StartSessionRequest) -> SipStatus:
+        response: SipStatus = self.stub.StartSession(request)
         return response
 
-    def end_session(self) -> Empty:
-        response: Empty = self.stub.EndSession(Empty())
+    def end_session(self) -> SipStatus:
+        response: SipStatus = self.stub.EndSession(Empty())
         return response
 
-    def register_account(self, request: RegisterAccountRequest) -> Empty:
-        response: Empty = self.stub.RegisterAccount(request)
+    def register_account(self, request: RegisterAccountRequest) -> SipStatus:
+        response: SipStatus = self.stub.RegisterAccount(request)
         return response
 
-    def start_call(self, request: StartCallRequest) -> Empty:
-        response: Empty = self.stub.StartCall(request)
+    def start_call(self, request: StartCallRequest) -> SipStatus:
+        response: SipStatus = self.stub.StartCall(request)
         return response
 
-    def end_call(self, request: EndCallRequest) -> Empty:
-        response: Empty = self.stub.EndCall(request)
+    def end_call(self, request: EndCallRequest) -> SipStatus:
+        response: SipStatus = self.stub.EndCall(request)
         return response
 
-    def transfer_call(self, request: TransferCallRequest) -> Empty:
-        response: Empty = self.stub.TransferCall(request)
+    def transfer_call(self, request: TransferCallRequest) -> SipStatus:
+        response: SipStatus = self.stub.TransferCall(request)
         return response
 
     def get_sip_status(self) -> SipStatus:
         response: SipStatus = self.stub.GetSipStatus(Empty())
         return response
 
     def get_sip_status_history(self) -> SipStatusHistoryResponse:
         response: SipStatusHistoryResponse = self.stub.GetSipStatusHistory(Empty())
         return response
 
-    def play_wav_files(self, request: PlayWavFilesRequest) -> Empty:
-        response: PlayWavFilesRequest = self.stub.PlayWavFiles(request)
+    def play_wav_files(self, request: PlayWavFilesRequest) -> SipStatus:
+        response: SipStatus = self.stub.PlayWavFiles(request)
         return response
 
-    def mute(self) -> Empty:
-        response: Empty = self.stub.Mute(Empty())
+    def mute(self) -> SipStatus:
+        response: SipStatus = self.stub.Mute(Empty())
         return response
 
-    def un_mute(self) -> Empty:
-        response: Empty = self.stub.UnMute(Empty())
+    def un_mute(self) -> SipStatus:
+        response: SipStatus = self.stub.UnMute(Empty())
         return response
```

### Comparing `ondewo-sip-client-4.0.0/ondewo/sip/client/services_container.py` & `ondewo-sip-client-4.0.1/ondewo/sip/client/services_container.py`

 * *Files identical despite different names*

### Comparing `ondewo-sip-client-4.0.0/ondewo/sip/sip_pb2.py` & `ondewo-sip-client-4.0.1/ondewo/sip/sip_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-sip-client-4.0.0/ondewo/sip/sip_pb2_grpc.py` & `ondewo-sip-client-4.0.1/ondewo/sip/sip_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-sip-client-4.0.0/ondewo_sip_client.egg-info/SOURCES.txt` & `ondewo-sip-client-4.0.1/ondewo_sip_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

