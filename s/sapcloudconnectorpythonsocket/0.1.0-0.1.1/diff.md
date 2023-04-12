# Comparing `tmp/sapcloudconnectorpythonsocket-0.1.0-py2.py3-none-any.whl.zip` & `tmp/sapcloudconnectorpythonsocket-0.1.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6998 bytes, number of entries: 9
+Zip file size: 6999 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-12 14:00 sap-cloud-connector-python-socket/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-12 14:01 sap-cloud-connector-python-socket/sap-cloud-connector-python-socket.py
--rw-rw-rw-  2.0 fat      338 b- defN 23-Apr-12 16:23 sapcloudconnectorpythonsocket/__init__.py
+-rw-rw-rw-  2.0 fat      338 b- defN 23-Apr-12 16:35 sapcloudconnectorpythonsocket/__init__.py
 -rw-rw-rw-  2.0 fat     9318 b- defN 23-Apr-12 15:20 sapcloudconnectorpythonsocket/sapcloudconnectorpythonsocket.py
--rw-rw-rw-  2.0 fat     1062 b- defN 23-Apr-12 16:32 sapcloudconnectorpythonsocket-0.1.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2395 b- defN 23-Apr-12 16:32 sapcloudconnectorpythonsocket-0.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-12 16:32 sapcloudconnectorpythonsocket-0.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       30 b- defN 23-Apr-12 16:32 sapcloudconnectorpythonsocket-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      936 b- defN 23-Apr-12 16:32 sapcloudconnectorpythonsocket-0.1.0.dist-info/RECORD
-9 files, 14189 bytes uncompressed, 5318 bytes compressed:  62.5%
+-rw-rw-rw-  2.0 fat     1062 b- defN 23-Apr-12 16:35 sapcloudconnectorpythonsocket-0.1.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2402 b- defN 23-Apr-12 16:35 sapcloudconnectorpythonsocket-0.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-12 16:35 sapcloudconnectorpythonsocket-0.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       30 b- defN 23-Apr-12 16:35 sapcloudconnectorpythonsocket-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      936 b- defN 23-Apr-12 16:35 sapcloudconnectorpythonsocket-0.1.1.dist-info/RECORD
+9 files, 14196 bytes uncompressed, 5319 bytes compressed:  62.5%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: sapcloudconnectorpythonsocket/__init__.py
 Comment: 
 
 Filename: sapcloudconnectorpythonsocket/sapcloudconnectorpythonsocket.py
 Comment: 
 
-Filename: sapcloudconnectorpythonsocket-0.1.0.dist-info/LICENSE
+Filename: sapcloudconnectorpythonsocket-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: sapcloudconnectorpythonsocket-0.1.0.dist-info/METADATA
+Filename: sapcloudconnectorpythonsocket-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: sapcloudconnectorpythonsocket-0.1.0.dist-info/WHEEL
+Filename: sapcloudconnectorpythonsocket-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: sapcloudconnectorpythonsocket-0.1.0.dist-info/top_level.txt
+Filename: sapcloudconnectorpythonsocket-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: sapcloudconnectorpythonsocket-0.1.0.dist-info/RECORD
+Filename: sapcloudconnectorpythonsocket-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sapcloudconnectorpythonsocket/__init__.py

```diff
@@ -1,14 +1,14 @@
 """
 sap-cloud-connector-python-socket
 
 Python Socket to connect to the SAP Cloud Connector via Connectivity Service
 """
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __author__ = 'fyx99'
 __credits__ = 'No credits'
 
 from sapcloudconnectorpythonsocket.sapcloudconnectorpythonsocket import CloudConnectorSocket
 
 __all__ = [
     CloudConnectorSocket
```

## Comparing `sapcloudconnectorpythonsocket-0.1.0.dist-info/LICENSE` & `sapcloudconnectorpythonsocket-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sapcloudconnectorpythonsocket-0.1.0.dist-info/METADATA` & `sapcloudconnectorpythonsocket-0.1.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapcloudconnectorpythonsocket
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python Package to open socket to SAP Cloud Connector via Connectivity Proxy
 Home-page: https://github.com/fyx99/sap-cloud-connector-python-socket
 Author: fxy99
 Author-email: 
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -20,15 +20,15 @@
 # sap-cloud-connector-python-socket
 Python Socket to connect to the SAP Cloud Connector via Connectivity Service
 
 The SAP BTP Connectivity Proxy allows to connect to on-prem systems. It can act as a SOCKS5 Proxy to establish TCP connections. 
 Due to its custom authentication scheme one can not use standard SOCKS5 client libaries. For details on how to authenticate against the Connectivity Proxy see the official Documentation. https://help.sap.com/docs/connectivity/sap-btp-connectivity-cf/using-tcp-protocol-for-cloud-applications
 
 Sample Usage:
-```
+```python 
 from sapcloudconnectorpythonsocket import CloudConnectorSocket
 
 cc_socket = CloudConnectorSocket()
 cc_socket.connect(
     dest_host="virtualhost", 
     dest_port=3333, 
     proxy_host="connectivity-proxy",
```

## Comparing `sapcloudconnectorpythonsocket-0.1.0.dist-info/RECORD` & `sapcloudconnectorpythonsocket-0.1.1.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 sap-cloud-connector-python-socket/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sap-cloud-connector-python-socket/sap-cloud-connector-python-socket.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sapcloudconnectorpythonsocket/__init__.py,sha256=nQ6IuLOqaYQfoS0KnagRaFPQfCb2fDW-cqqEuV9va2A,338
+sapcloudconnectorpythonsocket/__init__.py,sha256=T-my2U6Wz4Q3q_LJJH0huWloSRC47YuzU5I3Sf5MaeI,338
 sapcloudconnectorpythonsocket/sapcloudconnectorpythonsocket.py,sha256=lvBURHfMAmfS4azROIbfXYG05J7mhnvrkPEe_7YLWso,9318
-sapcloudconnectorpythonsocket-0.1.0.dist-info/LICENSE,sha256=oXTItccfzyUudck6ObY-GItzzZwngLzQ403XSpITg0U,1062
-sapcloudconnectorpythonsocket-0.1.0.dist-info/METADATA,sha256=qKuR9SjPXbrKye_oxaodsPA6rDrFxi4OfBq88UcoIJw,2395
-sapcloudconnectorpythonsocket-0.1.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-sapcloudconnectorpythonsocket-0.1.0.dist-info/top_level.txt,sha256=Sr63qbSm-90o-CQ-qwd4EKcLFznczAzm416CC87q0pA,30
-sapcloudconnectorpythonsocket-0.1.0.dist-info/RECORD,,
+sapcloudconnectorpythonsocket-0.1.1.dist-info/LICENSE,sha256=oXTItccfzyUudck6ObY-GItzzZwngLzQ403XSpITg0U,1062
+sapcloudconnectorpythonsocket-0.1.1.dist-info/METADATA,sha256=PTHI7kDxpPjWaIzEl9MWb5wKbNPaHUzjvB8h0jKJRA0,2402
+sapcloudconnectorpythonsocket-0.1.1.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+sapcloudconnectorpythonsocket-0.1.1.dist-info/top_level.txt,sha256=Sr63qbSm-90o-CQ-qwd4EKcLFznczAzm416CC87q0pA,30
+sapcloudconnectorpythonsocket-0.1.1.dist-info/RECORD,,
```

