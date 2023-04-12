# Comparing `tmp/arduino_iot_cloud-0.0.5.tar.gz` & `tmp/arduino_iot_cloud-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arduino_iot_cloud-0.0.5.tar", last modified: Wed Mar  8 13:59:08 2023, max compression
+gzip compressed data, was "arduino_iot_cloud-0.0.6.tar", last modified: Wed Apr 12 09:58:21 2023, max compression
```

## Comparing `arduino_iot_cloud-0.0.5.tar` & `arduino_iot_cloud-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 13:59:08.900318 arduino_iot_cloud-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-03-08 13:58:57.000000 arduino_iot_cloud-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-03-08 13:59:08.900318 arduino_iot_cloud-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-03-08 13:58:57.000000 arduino_iot_cloud-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 13:59:08.896318 arduino_iot_cloud-0.0.5/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-03-08 13:58:57.000000 arduino_iot_cloud-0.0.5/examples/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-03-08 13:58:57.000000 arduino_iot_cloud-0.0.5/examples/micropython.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-03-08 13:58:57.000000 arduino_iot_cloud-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-08 13:59:08.900318 arduino_iot_cloud-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 13:59:08.896318 arduino_iot_cloud-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 13:59:08.896318 arduino_iot_cloud-0.0.5/src/arduino_iot_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-03-08 13:58:57.000000 arduino_iot_cloud-0.0.5/src/arduino_iot_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-08 13:59:08.000000 arduino_iot_cloud-0.0.5/src/arduino_iot_cloud/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15978 2023-03-08 13:58:57.000000 arduino_iot_cloud-0.0.5/src/arduino_iot_cloud/ucloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-03-08 13:58:57.000000 arduino_iot_cloud-0.0.5/src/arduino_iot_cloud/umqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-03-08 13:58:57.000000 arduino_iot_cloud-0.0.5/src/arduino_iot_cloud/ussl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 13:59:08.900318 arduino_iot_cloud-0.0.5/src/arduino_iot_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-03-08 13:59:08.000000 arduino_iot_cloud-0.0.5/src/arduino_iot_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-08 13:59:08.000000 arduino_iot_cloud-0.0.5/src/arduino_iot_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 13:59:08.000000 arduino_iot_cloud-0.0.5/src/arduino_iot_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-08 13:59:08.000000 arduino_iot_cloud-0.0.5/src/arduino_iot_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-08 13:59:08.000000 arduino_iot_cloud-0.0.5/src/arduino_iot_cloud.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 13:59:08.900318 arduino_iot_cloud-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 13:58:57.000000 arduino_iot_cloud-0.0.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:58:21.907830 arduino_iot_cloud-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-12 09:58:07.000000 arduino_iot_cloud-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-04-12 09:58:21.907830 arduino_iot_cloud-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-04-12 09:58:07.000000 arduino_iot_cloud-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:58:21.907830 arduino_iot_cloud-0.0.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-12 09:58:07.000000 arduino_iot_cloud-0.0.6/examples/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-04-12 09:58:07.000000 arduino_iot_cloud-0.0.6/examples/micropython.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-12 09:58:07.000000 arduino_iot_cloud-0.0.6/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-12 09:58:07.000000 arduino_iot_cloud-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 09:58:21.907830 arduino_iot_cloud-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:58:21.907830 arduino_iot_cloud-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:58:21.907830 arduino_iot_cloud-0.0.6/src/arduino_iot_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-04-12 09:58:07.000000 arduino_iot_cloud-0.0.6/src/arduino_iot_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 09:58:21.000000 arduino_iot_cloud-0.0.6/src/arduino_iot_cloud/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16018 2023-04-12 09:58:07.000000 arduino_iot_cloud-0.0.6/src/arduino_iot_cloud/ucloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-04-12 09:58:07.000000 arduino_iot_cloud-0.0.6/src/arduino_iot_cloud/umqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-12 09:58:07.000000 arduino_iot_cloud-0.0.6/src/arduino_iot_cloud/ussl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:58:21.907830 arduino_iot_cloud-0.0.6/src/arduino_iot_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-04-12 09:58:21.000000 arduino_iot_cloud-0.0.6/src/arduino_iot_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-12 09:58:21.000000 arduino_iot_cloud-0.0.6/src/arduino_iot_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 09:58:21.000000 arduino_iot_cloud-0.0.6/src/arduino_iot_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-12 09:58:21.000000 arduino_iot_cloud-0.0.6/src/arduino_iot_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 09:58:21.000000 arduino_iot_cloud-0.0.6/src/arduino_iot_cloud.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:58:21.907830 arduino_iot_cloud-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:58:07.000000 arduino_iot_cloud-0.0.6/tests/__init__.py
```

### Comparing `arduino_iot_cloud-0.0.5/LICENSE` & `arduino_iot_cloud-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `arduino_iot_cloud-0.0.5/PKG-INFO` & `arduino_iot_cloud-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: arduino_iot_cloud
-Version: 0.0.5
+Version: 0.0.6
 Summary: Arduino IoT Cloud Python client
 Author-email: Ibrahim Abdelkader <i.abdelkader@arduino.cc>
 Project-URL: Homepage, https://github.com/arduino/arduino-iot-cloud-py
 Project-URL: Bug Tracker, https://github.com/arduino/arduino-iot-cloud-py/issues
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Arduino IoT Cloud Python client ☁️🐍☁️
 This is a Python client for the Arduino IoT cloud, which runs on both CPython and MicroPython. The client supports basic and advanced authentication methods, and provides a user-friendly API that allows the user to connect to the cloud, and create and link local objects to cloud objects with a just a few lines of code.
 
@@ -25,15 +25,15 @@
     # and modify any registered cloud object. The following line updates
     # the LED value.
     client["led"] = value
 
 # 1. Create a client object, which is used to connect to the IoT cloud and link local
 # objects to cloud objects. Note a username and password can be used for basic authentication
 # on both CPython and MicroPython. For more advanced authentication methods, please see the examples.
-client = AIOTClient(device_id=b"DEVICE_ID", username=b"DEVICE_ID", password=b"SECRET_KEY")
+client = ArduinoCloudClient(device_id=b"DEVICE_ID", username=b"DEVICE_ID", password=b"SECRET_KEY")
 
 # 2. Register cloud objects.
 # Note: The following objects must be created first in the dashboard and linked to the device.
 # When the switch is toggled from the dashboard, the on_switch_changed function is called with
 # the client object and new value args.
 client.register("sw1", value=None, on_write=on_switch_changed)
```

### Comparing `arduino_iot_cloud-0.0.5/README.md` & `arduino_iot_cloud-0.0.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     # and modify any registered cloud object. The following line updates
     # the LED value.
     client["led"] = value
 
 # 1. Create a client object, which is used to connect to the IoT cloud and link local
 # objects to cloud objects. Note a username and password can be used for basic authentication
 # on both CPython and MicroPython. For more advanced authentication methods, please see the examples.
-client = AIOTClient(device_id=b"DEVICE_ID", username=b"DEVICE_ID", password=b"SECRET_KEY")
+client = ArduinoCloudClient(device_id=b"DEVICE_ID", username=b"DEVICE_ID", password=b"SECRET_KEY")
 
 # 2. Register cloud objects.
 # Note: The following objects must be created first in the dashboard and linked to the device.
 # When the switch is toggled from the dashboard, the on_switch_changed function is called with
 # the client object and new value args.
 client.register("sw1", value=None, on_write=on_switch_changed)
```

### Comparing `arduino_iot_cloud-0.0.5/examples/example.py` & `arduino_iot_cloud-0.0.6/examples/example.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file is part of the Python Arduino IoT Cloud.
 # Any copyright is dedicated to the Public Domain.
 # https://creativecommons.org/publicdomain/zero/1.0/
 import time
 import logging
 from time import strftime
-from arduino_iot_cloud import AIOTClient
+from arduino_iot_cloud import ArduinoCloudClient
 from arduino_iot_cloud import Location
 from arduino_iot_cloud import Schedule
 from arduino_iot_cloud import ColoredLight
 from arduino_iot_cloud import Task
 from random import uniform
 import argparse
 import arduino_iot_cloud.ussl as ssl
@@ -55,16 +55,16 @@
         level=logging.DEBUG if args.debug else logging.INFO,
     )
 
     # Create a client object to connect to the Arduino IoT cloud.
     # To use a secure element, set the token's "pin" and URI in "keyfile" and "certfile", and
     # the CA certificate (if any) in "ssl_params". Alternatively, a username and password can
     # be used to authenticate, for example:
-    #   client = AIOTClient(device_id=b"DEVICE_ID", username=b"DEVICE_ID", password=b"SECRET_KEY")
-    client = AIOTClient(
+    #   client = ArduinoCloudClient(device_id=b"DEVICE_ID", username=b"DEVICE_ID", password=b"SECRET_KEY")
+    client = ArduinoCloudClient(
         device_id=DEVICE_ID,
         ssl_params={
             "pin": "1234",
             "keyfile": KEY_PATH, "certfile": CERT_PATH, "ca_certs": CA_PATH, "cert_reqs": ssl.CERT_REQUIRED
         },
     )
```

### Comparing `arduino_iot_cloud-0.0.5/examples/micropython.py` & `arduino_iot_cloud-0.0.6/examples/micropython.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Any copyright is dedicated to the Public Domain.
 # https://creativecommons.org/publicdomain/zero/1.0/
 import time
 import ussl
 import network
 import logging
 from time import strftime
-from arduino_iot_cloud import AIOTClient
+from arduino_iot_cloud import ArduinoCloudClient
 from arduino_iot_cloud import Location
 from arduino_iot_cloud import Schedule
 from arduino_iot_cloud import ColoredLight
 from arduino_iot_cloud import Task
 from arduino_iot_cloud import CADATA
 from random import uniform
 from secrets import WIFI_SSID
@@ -64,16 +64,16 @@
 
     # NOTE: Add networking code here or in boot.py
     wifi_connect()
 
     # Create a client object to connect to the Arduino IoT cloud.
     # For MicroPython, the key and cert files must be stored in DER format on the filesystem.
     # Alternatively, a username and password can be used to authenticate:
-    #   client = AIOTClient(device_id=b"DEVICE_ID", username=b"DEVICE_ID", password=b"SECRET_KEY")
-    client = AIOTClient(
+    #   client = ArduinoCloudClient(device_id=b"DEVICE_ID", username=b"DEVICE_ID", password=b"SECRET_KEY")
+    client = ArduinoCloudClient(
         device_id=DEVICE_ID,
         ssl_params={
             "keyfile": KEY_PATH, "certfile": CERT_PATH, "cadata": CADATA, "cert_reqs": ussl.CERT_REQUIRED
         }
     )
 
     # Register cloud objects.
```

### Comparing `arduino_iot_cloud-0.0.5/pyproject.toml` & `arduino_iot_cloud-0.0.6/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -12,19 +12,20 @@
   { name="Ibrahim Abdelkader", email="i.abdelkader@arduino.cc" },
 ]
 description = "Arduino IoT Cloud Python client"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
     "Topic :: Software Development :: Embedded Systems",
     "Operating System :: OS Independent",
+    "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
 ]
 dependencies = [
   'cbor2 >= 5.4.6',
+  'M2Crypto >= 0.38.0',
   'micropython-senml >= 0.1.0',
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/arduino/arduino-iot-cloud-py"
 "Bug Tracker" = "https://github.com/arduino/arduino-iot-cloud-py/issues"
```

### Comparing `arduino_iot_cloud-0.0.5/src/arduino_iot_cloud/__init__.py` & `arduino_iot_cloud-0.0.6/src/arduino_iot_cloud/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This file is part of the Arduino IoT Cloud Python client.
 # Copyright (c) 2022 Arduino SA
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
-from .ucloud import AIOTClient # noqa
-from .ucloud import AIOTObject
+from .ucloud import ArduinoCloudClient # noqa
+from .ucloud import ArduinoCloudObject
 from .ucloud import timestamp
 
 try:
     import asyncio
     import binascii
 except ImportError:
     import uasyncio as asyncio
@@ -32,35 +32,35 @@
     b"5b3e2a6b8ec9b01aa854e6369b8c09f9fce1b980300a06082a8648ce3d04"
     b"03020349003046022100bfd3dc236668b50adc3f0d0ec373e20ac7f760aa"
     b"100dd320bfe102969b6b05d8022100ead9d9da5acd12529709a8ed660fe1"
     b"8d6444ffe82217304ff2b89aafca8ecf"
 )
 
 
-class Location(AIOTObject):
+class Location(ArduinoCloudObject):
     def __init__(self, name, **kwargs):
         super().__init__(name, keys={"lat", "lon"}, **kwargs)
 
 
-class Color(AIOTObject):
+class Color(ArduinoCloudObject):
     def __init__(self, name, **kwargs):
         super().__init__(name, keys={"hue", "sat", "bri"}, **kwargs)
 
 
-class ColoredLight(AIOTObject):
+class ColoredLight(ArduinoCloudObject):
     def __init__(self, name, **kwargs):
         super().__init__(name, keys={"swi", "hue", "sat", "bri"}, **kwargs)
 
 
-class DimmedLight(AIOTObject):
+class DimmedLight(ArduinoCloudObject):
     def __init__(self, name, **kwargs):
         super().__init__(name, keys={"swi", "bri"}, **kwargs)
 
 
-class Schedule(AIOTObject):
+class Schedule(ArduinoCloudObject):
     def __init__(self, name, **kwargs):
         kwargs.update({("runnable", True)})  # Force task creation.
         self.on_active = kwargs.pop("on_active", None)
         # Uncomment to allow the schedule to change in runtime.
         # kwargs["on_write"] = kwargs.get("on_write", lambda aiot, value: None)
         self.active = False
         super().__init__(name, keys={"frm", "to", "len", "msk"}, **kwargs)
@@ -74,15 +74,15 @@
                         self.on_active(aiot, self.value)
                     self.active = True
                 else:
                     self.active = False
             await asyncio.sleep(self.interval)
 
 
-class Task(AIOTObject):
+class Task(ArduinoCloudObject):
     def __init__(self, name, **kwargs):
         kwargs.update({("runnable", True)})  # Force task creation.
         self.on_run = kwargs.pop("on_run", None)
         if not callable(self.on_run):
             raise TypeError("Expected a callable object")
         super().__init__(name, **kwargs)
```

### Comparing `arduino_iot_cloud-0.0.5/src/arduino_iot_cloud/ucloud.py` & `arduino_iot_cloud-0.0.6/src/arduino_iot_cloud/ucloud.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,24 +33,24 @@
     pass
 
 
 def timestamp():
     return int(time.time())
 
 
-class AIOTObject(SenmlRecord):
+class ArduinoCloudObject(SenmlRecord):
     def __init__(self, name, **kwargs):
         self.on_read = kwargs.pop("on_read", None)
         self.on_write = kwargs.pop("on_write", None)
         self.interval = kwargs.pop("interval", 1.0)
         self._runnable = kwargs.pop("runnable", False)
         value = kwargs.pop("value", None)
         if keys := kwargs.pop("keys", {}):
             value = {   # Create a complex object (with sub-records).
-                k: AIOTObject(f"{name}:{k}", value=v, callback=self.senml_callback)
+                k: ArduinoCloudObject(f"{name}:{k}", value=v, callback=self.senml_callback)
                 for (k, v) in {k: kwargs.pop(k, None) for k in keys}.items()
             }
         self._updated = False
         self.on_write_scheduled = False
         self.timestamp = timestamp()
         callback = kwargs.pop("callback", self.senml_callback)
         for key in kwargs:  # kwargs should be empty by now, unless a wrong attr was used.
@@ -153,15 +153,15 @@
                 self.value = self.on_read(client)
             if self.on_write is not None and self.on_write_scheduled:
                 self.on_write_scheduled = False
                 self.on_write(client, self if isinstance(self.value, dict) else self.value)
             await asyncio.sleep(self.interval)
 
 
-class AIOTClient:
+class ArduinoCloudClient:
     def __init__(
             self,
             device_id,
             username=None,
             password=None,
             ssl_params={},
             server=None,
@@ -252,17 +252,17 @@
     def create_topic(self, topic, inout):
         return bytes(f"/a/t/{self.thing_id}/{topic}/{inout}", "utf-8")
 
     def register(self, aiotobj, coro=None, **kwargs):
         if isinstance(aiotobj, str):
             if kwargs.get("value", None) is None and kwargs.get("on_read", None) is not None:
                 kwargs["value"] = kwargs.get("on_read")(self)
-            aiotobj = AIOTObject(aiotobj, **kwargs)
+            aiotobj = ArduinoCloudObject(aiotobj, **kwargs)
 
-        # Register the AIOTObject
+        # Register the ArduinoCloudObject
         self.records[aiotobj.name] = aiotobj
 
         # Create a task for this object if it has any callbacks.
         if aiotobj.runnable:
             self.create_task(aiotobj.name, aiotobj.run, self)
 
         # Check if object needs to be initialized from the cloud.
```

### Comparing `arduino_iot_cloud-0.0.5/src/arduino_iot_cloud/umqtt.py` & `arduino_iot_cloud-0.0.6/src/arduino_iot_cloud/umqtt.py`

 * *Files identical despite different names*

### Comparing `arduino_iot_cloud-0.0.5/src/arduino_iot_cloud/ussl.py` & `arduino_iot_cloud-0.0.6/src/arduino_iot_cloud/ussl.py`

 * *Files identical despite different names*

### Comparing `arduino_iot_cloud-0.0.5/src/arduino_iot_cloud.egg-info/PKG-INFO` & `arduino_iot_cloud-0.0.6/src/arduino_iot_cloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: arduino-iot-cloud
-Version: 0.0.5
+Version: 0.0.6
 Summary: Arduino IoT Cloud Python client
 Author-email: Ibrahim Abdelkader <i.abdelkader@arduino.cc>
 Project-URL: Homepage, https://github.com/arduino/arduino-iot-cloud-py
 Project-URL: Bug Tracker, https://github.com/arduino/arduino-iot-cloud-py/issues
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Arduino IoT Cloud Python client ☁️🐍☁️
 This is a Python client for the Arduino IoT cloud, which runs on both CPython and MicroPython. The client supports basic and advanced authentication methods, and provides a user-friendly API that allows the user to connect to the cloud, and create and link local objects to cloud objects with a just a few lines of code.
 
@@ -25,15 +25,15 @@
     # and modify any registered cloud object. The following line updates
     # the LED value.
     client["led"] = value
 
 # 1. Create a client object, which is used to connect to the IoT cloud and link local
 # objects to cloud objects. Note a username and password can be used for basic authentication
 # on both CPython and MicroPython. For more advanced authentication methods, please see the examples.
-client = AIOTClient(device_id=b"DEVICE_ID", username=b"DEVICE_ID", password=b"SECRET_KEY")
+client = ArduinoCloudClient(device_id=b"DEVICE_ID", username=b"DEVICE_ID", password=b"SECRET_KEY")
 
 # 2. Register cloud objects.
 # Note: The following objects must be created first in the dashboard and linked to the device.
 # When the switch is toggled from the dashboard, the on_switch_changed function is called with
 # the client object and new value args.
 client.register("sw1", value=None, on_write=on_switch_changed)
```

