# Comparing `tmp/ovos_PHAL-0.0.5a3-py3-none-any.whl.zip` & `tmp/ovos_PHAL-0.0.5a4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 9326 bytes, number of entries: 12
--rw-r--r--  2.0 unx      148 b- defN 23-Apr-08 03:52 ovos_PHAL/__init__.py
--rw-r--r--  2.0 unx      572 b- defN 23-Apr-08 03:52 ovos_PHAL/__main__.py
--rw-r--r--  2.0 unx     2594 b- defN 23-Apr-08 03:52 ovos_PHAL/admin.py
--rw-r--r--  2.0 unx     1436 b- defN 23-Apr-08 03:52 ovos_PHAL/detection.py
--rw-r--r--  2.0 unx     3073 b- defN 23-Apr-08 03:52 ovos_PHAL/service.py
--rw-r--r--  2.0 unx      177 b- defN 23-Apr-08 03:52 ovos_PHAL/version.py
--rw-r--r--  2.0 unx    11349 b- defN 23-Apr-08 03:52 ovos_PHAL-0.0.5a3.dist-info/LICENSE
--rw-r--r--  2.0 unx      899 b- defN 23-Apr-08 03:52 ovos_PHAL-0.0.5a3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-08 03:52 ovos_PHAL-0.0.5a3.dist-info/WHEEL
--rw-r--r--  2.0 unx       94 b- defN 23-Apr-08 03:52 ovos_PHAL-0.0.5a3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-Apr-08 03:52 ovos_PHAL-0.0.5a3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      966 b- defN 23-Apr-08 03:52 ovos_PHAL-0.0.5a3.dist-info/RECORD
-12 files, 21410 bytes uncompressed, 7702 bytes compressed:  64.0%
+Zip file size: 9313 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      148 b- defN 23-Apr-11 22:53 ovos_PHAL/__init__.py
+-rw-r--r--  2.0 unx      572 b- defN 23-Apr-11 22:53 ovos_PHAL/__main__.py
+-rw-r--r--  2.0 unx     2569 b- defN 23-Apr-11 22:53 ovos_PHAL/admin.py
+-rw-r--r--  2.0 unx     1436 b- defN 23-Apr-11 22:53 ovos_PHAL/detection.py
+-rw-r--r--  2.0 unx     3047 b- defN 23-Apr-11 22:53 ovos_PHAL/service.py
+-rw-r--r--  2.0 unx      177 b- defN 23-Apr-11 22:54 ovos_PHAL/version.py
+-rw-r--r--  2.0 unx    11349 b- defN 23-Apr-11 22:54 ovos_PHAL-0.0.5a4.dist-info/LICENSE
+-rw-r--r--  2.0 unx      899 b- defN 23-Apr-11 22:54 ovos_PHAL-0.0.5a4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 22:54 ovos_PHAL-0.0.5a4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       94 b- defN 23-Apr-11 22:54 ovos_PHAL-0.0.5a4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-Apr-11 22:54 ovos_PHAL-0.0.5a4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      966 b- defN 23-Apr-11 22:54 ovos_PHAL-0.0.5a4.dist-info/RECORD
+12 files, 21359 bytes uncompressed, 7689 bytes compressed:  64.0%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: ovos_PHAL/service.py
 Comment: 
 
 Filename: ovos_PHAL/version.py
 Comment: 
 
-Filename: ovos_PHAL-0.0.5a3.dist-info/LICENSE
+Filename: ovos_PHAL-0.0.5a4.dist-info/LICENSE
 Comment: 
 
-Filename: ovos_PHAL-0.0.5a3.dist-info/METADATA
+Filename: ovos_PHAL-0.0.5a4.dist-info/METADATA
 Comment: 
 
-Filename: ovos_PHAL-0.0.5a3.dist-info/WHEEL
+Filename: ovos_PHAL-0.0.5a4.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_PHAL-0.0.5a3.dist-info/entry_points.txt
+Filename: ovos_PHAL-0.0.5a4.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_PHAL-0.0.5a3.dist-info/top_level.txt
+Filename: ovos_PHAL-0.0.5a4.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_PHAL-0.0.5a3.dist-info/RECORD
+Filename: ovos_PHAL-0.0.5a4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_PHAL/admin.py

```diff
@@ -1,10 +1,10 @@
 from ovos_plugin_manager.phal import find_admin_plugins
 from ovos_utils import wait_for_exit_signal
-from ovos_utils.configuration import read_mycroft_config
+from ovos_config import Configuration
 from ovos_utils.log import LOG
 
 from ovos_PHAL import PHAL
 
 
 def on_admin_ready():
     LOG.info('PHAL Admin is ready.')
@@ -36,15 +36,15 @@
     """
 
     def __init__(self, config=None, bus=None, on_ready=on_admin_ready, on_error=on_admin_error,
                  on_stopping=on_admin_stopping, on_started=on_admin_started, on_alive=on_admin_alive,
                  watchdog=lambda: None, name="PHAL.admin", **kwargs):
         if not config:
             try:
-                config = read_mycroft_config()
+                config = Configuration()
                 config = config.get("PHAL", {}).get("admin", {})
             except:
                 config = {}
         super().__init__(config, bus, on_ready, on_error, on_stopping, on_started, on_alive, watchdog, name, **kwargs)
 
     def load_plugins(self):
         for name, plug in find_admin_plugins().items():
```

## ovos_PHAL/service.py

```diff
@@ -1,11 +1,11 @@
 from ovos_plugin_manager.phal import find_phal_plugins
-from ovos_utils.configuration import read_mycroft_config
+from ovos_config import Configuration
 from ovos_utils.log import LOG
-from ovos_utils.messagebus import get_mycroft_bus
+from ovos_bus_client.client import MessageBusClient
 from ovos_utils.process_utils import ProcessStatus, StatusCallbackMap
 from ovos_workshop import OVOSAbstractApplication
 
 
 def on_ready():
     LOG.info('PHAL is ready.')
 
@@ -48,21 +48,19 @@
         callbacks = StatusCallbackMap(on_ready=ready_hook,
                                       on_error=error_hook,
                                       on_stopping=stopping_hook,
                                       on_alive=alive_hook,
                                       on_started=started_hook)
         self.status = ProcessStatus(name, callback_map=callbacks)
         self._watchdog = watchdog  # TODO implement
-        if not config:
-            try:
-                config = read_mycroft_config()["PHAL"]
-            except:
-                config = {}
-        self.config = config
-        self.bus = bus or get_mycroft_bus()
+        self.config = config or Configuration().get("PHAL") or {}
+        if not bus:
+            bus = MessageBusClient()
+            bus.run_in_thread()
+        self.bus = bus
         self.drivers = {}
         self.status.bind(self.bus)
 
     def load_plugins(self):
         for name, plug in find_phal_plugins().items():
             config = self.config.get(name) or {}
             if hasattr(plug, "validator"):
@@ -79,11 +77,12 @@
 
     def start(self):
         self.status.set_started()
         try:
             self.load_plugins()
             self.status.set_ready()
         except Exception as e:
+            LOG.exception(e)
             self.status.set_error(e)
 
     def shutdown(self):
         self.status.set_stopping()
```

## ovos_PHAL/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
 VERSION_BUILD = 5
-VERSION_ALPHA = 3
+VERSION_ALPHA = 4
 # END_VERSION_BLOCK
```

## Comparing `ovos_PHAL-0.0.5a3.dist-info/LICENSE` & `ovos_PHAL-0.0.5a4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ovos_PHAL-0.0.5a3.dist-info/METADATA` & `ovos_PHAL-0.0.5a4.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ovos-PHAL
-Version: 0.0.5a3
+Version: 0.0.5a4
 Summary: UNKNOWN
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL
 Author: jarbasAi
 Author-email: jarbasai@mailfence.com
 License: apache-2.0
 Platform: UNKNOWN
 Requires-Dist: ovos-utils (>=0.0.31a6,~=0.0)
-Requires-Dist: ovos-bus-client (>=0.0.3a10,~=0.0)
+Requires-Dist: ovos-bus-client (>=0.0.3a16,~=0.0)
 Requires-Dist: ovos-workshop (>=0.0.12a3,~=0.0)
 Requires-Dist: ovos-config (>=0.0.8a3,~=0.0)
 Requires-Dist: ovos-plugin-manager (>=0.0.23a5,~=0.0)
 Requires-Dist: ovos-phal-plugin-connectivity-events (>=0.0.1,~=0.0)
 Requires-Dist: ovos-PHAL-plugin-wallpaper-manager (>=0.0.0,~=0.0)
 Requires-Dist: ovos-PHAL-plugin-network-manager (>=1.0.0,~=1.0)
 Requires-Dist: ovos-phal-plugin-ipgeo (>=0.0.1,~=0.0)
```

## Comparing `ovos_PHAL-0.0.5a3.dist-info/RECORD` & `ovos_PHAL-0.0.5a4.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ovos_PHAL/__init__.py,sha256=01I5hydahUGIIOXvvE2nM3Nul5Vr5YabvYM2aEh0TkQ,148
 ovos_PHAL/__main__.py,sha256=CsDEsncExx6vYTSJYkLDD6uL1hZXxwZA2KbKezr0Swo,572
-ovos_PHAL/admin.py,sha256=mUAy_iEnu_JI7YeE52JMsIDLtbhEYW-6bihI_auwIY0,2594
+ovos_PHAL/admin.py,sha256=DJbRTi0orOnBRIZXpqf7ya_fZI3za8gJRze2VTRYYOQ,2569
 ovos_PHAL/detection.py,sha256=GujqinjXF467EdMk80StP1he1bYUHUWvSQ1j7mYJbe8,1436
-ovos_PHAL/service.py,sha256=zmvSXLb8u_8YS2sRYEPQswOVGoafHcDtYGRTlO2xJlE,3073
-ovos_PHAL/version.py,sha256=O46IsF1GPQiLUxkULlCWU1ENwzuiE79ITXgmchnCrkw,177
-ovos_PHAL-0.0.5a3.dist-info/LICENSE,sha256=ujdvnin8cAYCsJhQhQxfUSvS5yCf7RAk24ltOrau7rA,11349
-ovos_PHAL-0.0.5a3.dist-info/METADATA,sha256=b5zTH8XzXa_9EHeIbOtEQFv0pbDxmNSWRRfk940Uxnw,899
-ovos_PHAL-0.0.5a3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ovos_PHAL-0.0.5a3.dist-info/entry_points.txt,sha256=iLNb-d0BX90d0YvhjUz0tr6l9-keqtJvUbj_djyE1vA,94
-ovos_PHAL-0.0.5a3.dist-info/top_level.txt,sha256=Pt4y92j6yi3cwUiC_jA7_7ztrK5zhkW3zQj0szVT8h0,10
-ovos_PHAL-0.0.5a3.dist-info/RECORD,,
+ovos_PHAL/service.py,sha256=fEzfP5RAASL_qui90CL3gjGDwVnluIfMLHTtnYty2Jw,3047
+ovos_PHAL/version.py,sha256=cKXdvCe6mkZOCYR1os_noY-8Ug8zh6pEIlyy1GuTY-k,177
+ovos_PHAL-0.0.5a4.dist-info/LICENSE,sha256=ujdvnin8cAYCsJhQhQxfUSvS5yCf7RAk24ltOrau7rA,11349
+ovos_PHAL-0.0.5a4.dist-info/METADATA,sha256=s576RLEHpDq8cmq22FSloT1WI1i6Emjv0Rt8YQ3dP-0,899
+ovos_PHAL-0.0.5a4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ovos_PHAL-0.0.5a4.dist-info/entry_points.txt,sha256=iLNb-d0BX90d0YvhjUz0tr6l9-keqtJvUbj_djyE1vA,94
+ovos_PHAL-0.0.5a4.dist-info/top_level.txt,sha256=Pt4y92j6yi3cwUiC_jA7_7ztrK5zhkW3zQj0szVT8h0,10
+ovos_PHAL-0.0.5a4.dist-info/RECORD,,
```

