# Comparing `tmp/omnikinverter-0.9.0.tar.gz` & `tmp/omnikinverter-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnikinverter-0.9.0.tar", max compression
+gzip compressed data, was "omnikinverter-0.9.1.tar", max compression
```

## Comparing `omnikinverter-0.9.0.tar` & `omnikinverter-0.9.1.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1077 2023-02-13 19:22:29.491327 omnikinverter-0.9.0/LICENSE
--rw-r--r--   0        0        0     8190 2023-02-13 19:22:29.491327 omnikinverter-0.9.0/README.md
--rw-r--r--   0        0        0      494 2023-02-13 19:22:29.491327 omnikinverter-0.9.0/omnikinverter/__init__.py
--rw-r--r--   0        0        0       96 2023-02-13 19:22:29.491327 omnikinverter-0.9.0/omnikinverter/const.py
--rw-r--r--   0        0        0      867 2023-02-13 19:22:29.491327 omnikinverter-0.9.0/omnikinverter/exceptions.py
--rw-r--r--   0        0        0     9276 2023-02-13 19:22:29.491327 omnikinverter-0.9.0/omnikinverter/models.py
--rw-r--r--   0        0        0     8227 2023-02-13 19:22:29.491327 omnikinverter-0.9.0/omnikinverter/omnikinverter.py
--rw-r--r--   0        0        0        0 2023-02-13 19:22:29.491327 omnikinverter-0.9.0/omnikinverter/py.typed
--rw-r--r--   0        0        0    10133 2023-02-13 19:22:29.491327 omnikinverter-0.9.0/omnikinverter/tcp.py
--rw-r--r--   0        0        0     3953 2023-02-13 19:22:44.003663 omnikinverter-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     9195 1970-01-01 00:00:00.000000 omnikinverter-0.9.0/setup.py
--rw-r--r--   0        0        0     9727 1970-01-01 00:00:00.000000 omnikinverter-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-12 20:40:43.985755 omnikinverter-0.9.1/LICENSE
+-rw-r--r--   0        0        0     8235 2023-04-12 20:40:43.985755 omnikinverter-0.9.1/README.md
+-rw-r--r--   0        0        0      494 2023-04-12 20:40:43.989755 omnikinverter-0.9.1/omnikinverter/__init__.py
+-rw-r--r--   0        0        0       96 2023-04-12 20:40:43.989755 omnikinverter-0.9.1/omnikinverter/const.py
+-rw-r--r--   0        0        0      867 2023-04-12 20:40:43.989755 omnikinverter-0.9.1/omnikinverter/exceptions.py
+-rw-r--r--   0        0        0     9479 2023-04-12 20:40:43.989755 omnikinverter-0.9.1/omnikinverter/models.py
+-rw-r--r--   0        0        0     8022 2023-04-12 20:40:43.989755 omnikinverter-0.9.1/omnikinverter/omnikinverter.py
+-rw-r--r--   0        0        0        0 2023-04-12 20:40:43.989755 omnikinverter-0.9.1/omnikinverter/py.typed
+-rw-r--r--   0        0        0    10459 2023-04-12 20:40:43.989755 omnikinverter-0.9.1/omnikinverter/tcp.py
+-rw-r--r--   0        0        0     3918 2023-04-12 20:40:59.205972 omnikinverter-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     9779 1970-01-01 00:00:00.000000 omnikinverter-0.9.1/PKG-INFO
```

### Comparing `omnikinverter-0.9.0/LICENSE` & `omnikinverter-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `omnikinverter-0.9.0/README.md` & `omnikinverter-0.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 | Omnik    | Omniksol 2000TL  | JS         |
 | Omnik    | Omniksol 2000TL2 | JSON       |
 | Omnik    | Omniksol 2500TL  | HTML       |
 | Omnik    | Omniksol 3000TL  | TCP        |
 | Omnik    | Omniksol 4000TL2 | JS         |
 | Ginlong  | Solis-DLS-WiFi   | JSON/HTML  |
 | Hosola   | 1500TL           | JS         |
+| Hosala   | Bright 2500MTL-S | JS         |
 | Bosswerk | BW-MI300         | HTML       |
 | Bosswerk | BW-MI600         | HTML       |
 | Sofar    | 3600TLM          | HTML       |
 | Sofar    | 2200TL           | JS         |
 | Huayu    | HY-600-Pro       | HTML       |
 
 ## Installation
```

### Comparing `omnikinverter-0.9.0/omnikinverter/exceptions.py` & `omnikinverter-0.9.1/omnikinverter/exceptions.py`

 * *Files identical despite different names*

### Comparing `omnikinverter-0.9.0/omnikinverter/models.py` & `omnikinverter-0.9.1/omnikinverter/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,45 +37,48 @@
     ac_output_power: list[float] | None = None
 
     @staticmethod
     def from_json(data: dict[str, Any]) -> Inverter:
         """Return Inverter object from the Omnik Inverter response.
 
         Args:
+        ----
             data: The JSON data from the Omnik Inverter.
 
         Returns:
+        -------
             An Inverter object.
 
         Raises:
+        ------
             OmnikInverterWrongValuesError: Inverter pass on
                 incorrect data (day and total are equal).
         """
 
         def get_value(search: str) -> Any:
-            if data[search] != "":
+            if data[search]:
                 return data[search]
             return None
 
         def validation(data_list: list[Any]) -> bool:
             """Check if the values are not equal to each other.
 
             Args:
+            ----
                 data_list: List of values to check.
 
             Returns:
+            -------
                 Boolean value.
             """
-            res = all(ele == data_list[0] for ele in data_list)
-            return res
+            return all(ele == data_list[0] for ele in data_list)
 
         if validation([data["i_eday"], data["i_eall"]]):
-            raise OmnikInverterWrongValuesError(
-                "Inverter pass on incorrect data (day and total are equal)"
-            )
+            msg = "Inverter pass on incorrect data (day and total are equal)"
+            raise OmnikInverterWrongValuesError(msg)
 
         return Inverter(
             serial_number=get_value("i_sn"),
             model=get_value("i_modle"),
             firmware=get_value("i_ver_m"),
             firmware_slave=get_value("i_ver_s"),
             alarm_code=get_value("i_alarm"),
@@ -86,37 +89,38 @@
         )
 
     @staticmethod
     def from_html(data: str) -> Inverter:
         """Return Inverter object from the Omnik Inverter response.
 
         Args:
+        ----
             data: The HTML (webscraping) data from the Omnik Inverter.
 
         Returns:
+        -------
             An Inverter object.
         """
 
         def get_value(search_key: str) -> Any:
             try:
                 match = cast(
                     re.Match[str],
                     re.search(f'(?<={search_key}=").*?(?=";)', data.replace(" ", "")),
                 ).group(0)
-                if match != "":
+                if match:
                     if search_key in ["webdata_now_p", "webdata_rate_p"]:
                         return int(match)
                     if search_key in ["webdata_today_e", "webdata_total_e"]:
                         return float(match)
                     return match
                 return None
             except AttributeError as exception:
-                raise OmnikInverterWrongSourceError(
-                    "Your inverter has no data source from a html file."
-                ) from exception
+                msg = "Your inverter has no data source from a html file."
+                raise OmnikInverterWrongSourceError(msg) from exception
 
         return Inverter(
             serial_number=get_value("webdata_sn"),
             model=get_value("webdata_pv_type"),
             firmware=get_value("webdata_msvn"),
             firmware_slave=get_value("webdata_ssvn"),
             alarm_code=get_value("webdata_alarm"),
@@ -127,17 +131,19 @@
         )
 
     @staticmethod
     def from_js(data: str) -> Inverter:
         """Return Inverter object from the Omnik Inverter response.
 
         Args:
+        ----
             data: The JS (webscraping) data from the Omnik Inverter.
 
         Returns:
+        -------
             An Inverter object.
         """
 
         def get_value(position: int) -> Any:
             try:
                 if data.find("webData") != -1:
                     matches = (
@@ -151,30 +157,29 @@
                             re.Match[str],
                             re.search(r'(?<=myDeviceArray\[0\]=").*?(?=";)', data),
                         )
                         .group(0)
                         .split(",")
                     )
 
-                if matches[position] != "":
+                if matches[position]:
                     if position in [4, 5, 6, 7]:
                         if position in [4, 5]:
                             return int(matches[position].replace(" ", ""))
 
                         if position == 6:
                             energy_value = float(matches[position]) / 100
                         if position == 7:
                             energy_value = float(matches[position]) / 10
                         return energy_value
                     return matches[position].replace(" ", "")
                 return None
             except AttributeError as exception:
-                raise OmnikInverterWrongSourceError(
-                    "Your inverter has no data source from a javascript file."
-                ) from exception
+                msg = "Your inverter has no data source from a javascript file."
+                raise OmnikInverterWrongSourceError(msg) from exception
 
         return Inverter(
             serial_number=get_value(0),
             model=get_value(3),
             firmware=get_value(1),
             firmware_slave=get_value(2),
             alarm_code=get_value(8),
@@ -185,20 +190,21 @@
         )
 
     @staticmethod
     def from_tcp(data: dict[str, Any]) -> Inverter:
         """Return Inverter object from the Omnik Inverter response.
 
         Args:
+        ----
             data: The binary data from the Omnik Inverter.
 
         Returns:
+        -------
             An Inverter object.
         """
-
         return Inverter(
             **data,
             model=None,  # Not able to deduce this from raw message yet
             solar_rated_power=None,
             solar_current_power=sum(
                 p for p in data["ac_output_power"] if p is not None
             ),
@@ -214,45 +220,49 @@
     ip_address: str | None = None
 
     @staticmethod
     def from_json(data: dict[str, Any]) -> Device:
         """Return Device object from the Omnik Inverter response.
 
         Args:
+        ----
             data: The JSON data from the Omnik Inverter.
 
         Returns:
+        -------
             An Device object.
         """
         return Device(
             signal_quality=None,
             firmware=data["g_ver"].replace("VER:", ""),
             ip_address=data["ip"],
         )
 
     @staticmethod
     def from_html(data: str) -> Device:
         """Return Device object from the Omnik Inverter response.
 
         Args:
+        ----
             data: The HTML (webscraping) data from the Omnik Inverter.
 
         Returns:
+        -------
             An Device object.
         """
-
         for correction in [" ", "%"]:
             data = data.replace(correction, "")
 
         def get_value(search_key: str) -> Any:
             match = cast(
-                re.Match[str], re.search(f'(?<={search_key}=").*?(?=";)', data)
+                re.Match[str],
+                re.search(f'(?<={search_key}=").*?(?=";)', data),
             ).group(0)
 
-            if match != "":
+            if match:
                 if search_key in ["cover_sta_rssi"]:
                     return int(match)
                 return match
             return None
 
         return Device(
             signal_quality=get_value("cover_sta_rssi"),
@@ -261,28 +271,31 @@
         )
 
     @staticmethod
     def from_js(data: str) -> Device:
         """Return Device object from the Omnik Inverter response.
 
         Args:
+        ----
             data: The JS (webscraping) data from the Omnik Inverter.
 
         Returns:
+        -------
             An Device object.
         """
         for correction in [" ", "%"]:
             data = data.replace(correction, "")
 
         def get_value(search_key: str) -> Any:
             match = cast(
-                re.Match[str], re.search(f'(?<={search_key}=").*?(?=";)', data)
+                re.Match[str],
+                re.search(f'(?<={search_key}=").*?(?=";)', data),
             ).group(0)
 
-            if match != "":
+            if match:
                 if search_key == "m2mRssi":
                     return int(match)
                 return match
             return None
 
         return Device(
             signal_quality=get_value("m2mRssi"),
```

### Comparing `omnikinverter-0.9.0/omnikinverter/omnikinverter.py` & `omnikinverter-0.9.1/omnikinverter/omnikinverter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 """Asynchronous Python client for the Omnik Inverter."""
 from __future__ import annotations
 
 import asyncio
 import json
-from collections.abc import Mapping
 from dataclasses import dataclass
 from typing import Any
 
-import aiohttp
 import async_timeout
-from aiohttp.client import ClientError, ClientResponseError, ClientSession
+from aiohttp import BasicAuth, ClientError, ClientResponseError, ClientSession
 from aiohttp.hdrs import METH_GET
 from yarl import URL
 
 from . import tcp
 from .exceptions import (
     OmnikInverterAuthError,
     OmnikInverterConnectionError,
@@ -33,148 +31,145 @@
     request_timeout: float = 10.0
     session: ClientSession | None = None
     serial_number: int | None = None  # Optional, only for TCP backend
     tcp_port: int = 8899
 
     _close_session: bool = False
 
-    _socket_mock: None = None
-
     async def request(
         self,
         uri: str,
         *,
         method: str = METH_GET,
-        params: Mapping[str, Any] | None = None,
+        params: dict[str, Any] | None = None,
     ) -> str:
         """Handle a request to a Omnik Inverter device.
 
         Args:
+        ----
             uri: Request URI, without '/', for example, 'status'
             method: HTTP Method to use.
             params: Extra options to improve or limit the response.
 
         Returns:
+        -------
             A Python dictionary (text) with the response from
             the Omnik Inverter.
 
         Raises:
+        ------
             OmnikInverterConnectionError: An error occurred while communicating
                 with the Omnik Inverter.
             OmnikInverterAuthError: Authentication failed with the Omnik Inverter.
             OmnikInverterError: Received an unexpected response from the Omnik Inverter.
         """
         url = URL.build(scheme="http", host=self.host, path="/").join(URL(uri))
 
         headers = {
             "Accept": "text/html,application/xhtml+xml,application/xml",
         }
 
+        if self.source_type == "html" and (
+            self.username is None or self.password is None
+        ):
+            msg = "A username and/or password is missing from the request"
+            raise OmnikInverterAuthError(msg)
+
         if self.session is None:
             self.session = ClientSession()
             self._close_session = True
 
         # Use big try to make sure manual session is always cleaned up
         try:
-            if self.source_type == "html" and (
-                self.username is None or self.password is None
-            ):
-                raise OmnikInverterAuthError(
-                    "A username and/or password is missing from the request"
-                )
             auth = None
             if self.username and self.password:
-                auth = aiohttp.BasicAuth(self.username, self.password)
+                auth = BasicAuth(self.username, self.password)
 
             try:
                 async with async_timeout.timeout(self.request_timeout):
                     response = await self.session.request(
                         method,
                         url,
                         auth=auth,
                         params=params,
                         headers=headers,
                     )
                     response.raise_for_status()
             except asyncio.TimeoutError as exception:
-                raise OmnikInverterConnectionError(
-                    "Timeout occurred while connecting to Omnik Inverter device"
-                ) from exception
+                msg = "Timeout occurred while connecting to Omnik Inverter device"
+                raise OmnikInverterConnectionError(msg) from exception
             except (ClientError, ClientResponseError) as exception:
-                raise OmnikInverterConnectionError(
-                    "Error occurred while communicating with Omnik Inverter device"
-                ) from exception
-
-            types = ["application/json", "application/x-javascript", "text/html"]
-            content_type = response.headers.get("Content-Type", "")
-            if not any(item in content_type for item in types):
-                text = await response.text()
-                raise OmnikInverterError(
-                    "Unexpected response from the Omnik Inverter device",
-                    {"Content-Type": content_type, "response": text},
-                )
+                msg = "Error occurred while communicating with Omnik Inverter device"
+                raise OmnikInverterConnectionError(msg) from exception
 
             raw_response = await response.read()
         finally:
-            if self.session and self._close_session:
-                await self.session.close()
-                self.session = None
-                self._close_session = False
+            await self.close()
+
+        types = ["application/json", "application/x-javascript", "text/html"]
+        content_type = response.headers.get("Content-Type", "")
+        if not any(item in content_type for item in types):
+            text = await response.text()
+            msg = "Unexpected response from the Omnik Inverter device"
+            raise OmnikInverterError(
+                msg,
+                {"Content-Type": content_type, "response": text},
+            )
 
         return raw_response.decode("ascii", "ignore")
 
     async def tcp_request(self) -> dict[str, Any]:
         """Perform a raw TCP request to the Omnik device.
 
-        Returns:
+        Returns
+        -------
             A Python dictionary (text) with the response from
             the Omnik Inverter.
 
-        Raises:
+        Raises
+        ------
             OmnikInverterAuthError: Serial number is required to communicate
                 with the Omnik Inverter.
             OmnikInverterConnectionError: An error occurred while communicating
                 with the Omnik Inverter.
         """
         if self.serial_number is None:
-            raise OmnikInverterAuthError("serial_number is missing from the request")
+            msg = "serial_number is missing from the request"
+            raise OmnikInverterAuthError(msg)
 
         try:
-            if self._socket_mock is not None:
-                reader, writer = await asyncio.open_connection(sock=self._socket_mock)
-            else:  # pragma: no cover
-                reader, writer = await asyncio.open_connection(self.host, self.tcp_port)
+            reader, writer = await asyncio.open_connection(self.host, self.tcp_port)
         except OSError as exception:
-            raise OmnikInverterConnectionError(
-                "Failed to open a TCP connection to the Omnik Inverter device"
-            ) from exception
+            msg = "Failed to open a TCP connection to the Omnik Inverter device"
+            raise OmnikInverterConnectionError(msg) from exception
 
         try:
             writer.write(tcp.create_information_request(self.serial_number))
             await writer.drain()
 
             raw_msg = await reader.read(1024)
         finally:
             writer.close()
             try:
                 await writer.wait_closed()
             except OSError as exception:
-                raise OmnikInverterConnectionError(
-                    "Failed to communicate with the Omnik Inverter device over TCP"
-                ) from exception
+                msg = "Failed to communicate with the Omnik Inverter device over TCP"
+                raise OmnikInverterConnectionError(msg) from exception
 
         return tcp.parse_messages(self.serial_number, raw_msg)
 
     async def inverter(self) -> Inverter:
         """Get values from your Omnik Inverter.
 
-        Returns:
+        Returns
+        -------
             A Inverter data object from the Omnik Inverter.
 
-        Raises:
+        Raises
+        ------
             OmnikInverterError: Unknown source type.
         """
         if self.source_type == "json":
             data = await self.request("status.json", params={"CMD": "inv_query"})
             return Inverter.from_json(json.loads(data))
         if self.source_type == "html":
             data = await self.request("status.html")
@@ -182,23 +177,26 @@
         if self.source_type == "javascript":
             data = await self.request("js/status.js")
             return Inverter.from_js(data)
         if self.source_type == "tcp":
             fields = await self.tcp_request()
             return Inverter.from_tcp(fields)
 
-        raise OmnikInverterError(f"Unknown source type `{self.source_type}`")
+        msg = f"Unknown source type `{self.source_type}`"
+        raise OmnikInverterError(msg)
 
     async def device(self) -> Device:
         """Get values from the device.
 
-        Returns:
+        Returns
+        -------
             A Device data object from the Omnik Inverter. None on the "tcp" source_type.
 
-        Raises:
+        Raises
+        ------
             OmnikInverterError: Unknown source type.
         """
         if self.source_type == "json":
             data = await self.request("status.json", params={"CMD": "inv_query"})
             return Device.from_json(json.loads(data))
         if self.source_type == "html":
             data = await self.request("status.html")
@@ -206,29 +204,34 @@
         if self.source_type == "javascript":
             data = await self.request("js/status.js")
             return Device.from_js(data)
         if self.source_type == "tcp":
             # None of the fields are available through a TCP data dump.
             return Device()
 
-        raise OmnikInverterError(f"Unknown source type `{self.source_type}`")
+        msg = f"Unknown source type `{self.source_type}`"
+        raise OmnikInverterError(msg)
 
     async def close(self) -> None:
         """Close open client session."""
         if self.session and self._close_session:
             await self.session.close()
+            self.session = None
+            self._close_session = False
 
     async def __aenter__(self) -> OmnikInverter:
         """Async enter.
 
-        Returns:
+        Returns
+        -------
             The Omnik Inverter object.
         """
         return self
 
     async def __aexit__(self, *_exc_info: str) -> None:
         """Async exit.
 
         Args:
+        ----
             _exc_info: Exec type.
         """
         await self.close()
```

### Comparing `omnikinverter-0.9.0/omnikinverter/tcp.py` & `omnikinverter-0.9.1/omnikinverter/tcp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 """Data model and conversions for tcp-based communication with the Omnik Inverter."""
-from collections.abc import Generator
+from __future__ import annotations
+
 from ctypes import BigEndianStructure, c_char, c_ubyte, c_uint, c_ushort
-from typing import Any, Optional
+from typing import TYPE_CHECKING, Any
 
 from .const import LOGGER
 from .exceptions import OmnikInverterPacketInvalidError
 
+if TYPE_CHECKING:
+    from collections.abc import Generator
+
 MESSAGE_START = 0x68
 MESSAGE_END = 0x16
 MESSAGE_SEND_SEP = 0x40
 MESSAGE_RECV_SEP = 0x41
 MESSAGE_TYPE_INFORMATION_REQUEST = 0x30
 MESSAGE_TYPE_INFORMATION_REPLY = 0xB0
 MESSAGE_TYPE_STRING = 0xF0  # Message seems to consist of pure text
@@ -25,26 +29,28 @@
 
 class _AcOutput(BigEndianStructure):
     _fields_ = [
         ("frequency", c_ushort),
         ("power", c_ushort),
     ]
 
-    def get_power(self) -> Optional[int]:
+    def get_power(self) -> int | None:
         """Retrieve AC power.
 
-        Returns:
+        Returns
+        -------
             The power field, or None if it is unset.
         """
         return None if self.power == UINT16_MAX else self.power
 
-    def get_frequency(self) -> Optional[float]:
+    def get_frequency(self) -> float | None:
         """Retrieve AC frequency.
 
-        Returns:
+        Returns
+        -------
             The frequency field in Hertz, or None if it is unset.
         """
         return None if self.frequency == UINT16_MAX else self.frequency * 0.01
 
 
 class _TcpData(BigEndianStructure):
     _pack_ = 1
@@ -68,15 +74,17 @@
         ("padding3", c_ubyte * 4),
         ("firmware_slave", c_char * 16),
         ("padding4", c_ubyte * 4),
     ]
 
 
 def _pack_message(
-    message_type: int, serial_number: int, message: bytearray
+    message_type: int,
+    serial_number: int,
+    message: bytearray,
 ) -> bytearray:
     # Prepend message "header"
     request_data = bytearray([len(message), MESSAGE_SEND_SEP, message_type])
     serial_bytes = serial_number.to_bytes(4, "little")
     request_data.extend(serial_bytes)
     request_data.extend(serial_bytes)
 
@@ -95,111 +103,121 @@
 
 def _unpack_message(message: bytearray) -> tuple[int, int, bytearray]:
     LOGGER.debug("Handling message `%s`", message)
 
     message_checksum = message.pop()
     checksum = sum(message) & 0xFF
     if message_checksum != checksum:
-        raise OmnikInverterPacketInvalidError(
-            f"Checksum mismatch (calculated `{checksum}` got `{message_checksum}`)"
-        )
+        msg = f"Checksum mismatch (calculated `{checksum}` got `{message_checksum}`)"
+        raise OmnikInverterPacketInvalidError(msg)
 
     # Now that the checksum has been computed remove the length,
     # separator, message type and repeated serial number
 
     length = message.pop(0)  # Length
     if message.pop(0) != MESSAGE_RECV_SEP:
-        raise OmnikInverterPacketInvalidError("Invalid receiver separator")
+        msg = "Invalid receiver separator"
+        raise OmnikInverterPacketInvalidError(msg)
 
     message_type = message.pop(0)
     LOGGER.debug(
-        "Message type %02x, length %s, checksum %02x", message_type, length, checksum
+        "Message type %02x, length %s, checksum %02x",
+        message_type,
+        length,
+        checksum,
     )
 
     serial0 = int.from_bytes(message[:4], "little")
     serial1 = int.from_bytes(message[4:8], "little")
     if serial0 != serial1:
-        raise OmnikInverterPacketInvalidError(
-            f"Serial number mismatch in reply {serial0} != {serial1}"
-        )
+        msg = f"Serial number mismatch in reply {serial0} != {serial1}"
+        raise OmnikInverterPacketInvalidError(msg)
 
     return (message_type, serial0, message[8:])
 
 
 def _unpack_messages(
     data: bytearray,
 ) -> Generator[tuple[int, int, bytearray], None, None]:
     while len(data):
         message_start = data.pop(0)
         # Whenever my Omnik sends an INFORMATION_REPLY followed by a STRING
         # text message, there's a bunch of trailing 0xFF garbage
         if message_start == 0xFF:  # pragma: no cover
             if not all(d == 0xFF for d in data):
-                raise OmnikInverterPacketInvalidError(
+                msg = (
                     "(Next) message starts with `0xFF` but the remainder "
                     f"is not strictly 0xFF: {data}"
                 )
+                raise OmnikInverterPacketInvalidError(msg)
             # We're done
             return
 
         if message_start != MESSAGE_START:
-            raise OmnikInverterPacketInvalidError("Invalid start byte")
+            msg = f"Invalid start byte: {message_start}"
+            raise OmnikInverterPacketInvalidError(msg)
 
         length = data[0] + MESSAGE_HEADER_SIZE
 
         message = data[:length]
         if len(message) != length:
-            raise OmnikInverterPacketInvalidError(
+            msg = (
                 f"Could only read {len(message)} out of {length} "
-                "expected bytes from TCP stream",
+                "expected bytes from TCP stream"
             )
+            raise OmnikInverterPacketInvalidError(msg)
 
         yield _unpack_message(message)
 
         # Prepare for the next message by stripping off the end byte
         data = data[length:]
         if data.pop(0) != MESSAGE_END:
-            raise OmnikInverterPacketInvalidError("Invalid end byte")
+            msg = "Invalid end byte"
+            raise OmnikInverterPacketInvalidError(msg)
 
 
 def create_information_request(serial_number: int) -> bytearray:
     """Compute a magic message to which the Omnik will reply with raw statistics.
 
     Args:
+    ----
         serial_number: Integer with the serial number of your Omnik device.
 
     Returns:
+    -------
         A bytearray with the raw message data, to be sent over a TCP socket.
     """
     return _pack_message(
-        MESSAGE_TYPE_INFORMATION_REQUEST, serial_number, bytearray([0x01, 0x00])
+        MESSAGE_TYPE_INFORMATION_REQUEST,
+        serial_number,
+        bytearray([0x01, 0x00]),
     )
 
 
 def parse_messages(serial_number: int, data: bytes) -> dict[str, Any]:
     """Perform a raw TCP request to the Omnik device.
 
     Args:
+    ----
         serial_number: Serial number passed to
             `clk.create_information_request()`, used to validate the reply.
         data: Raw data reply from the Omnik Inverter.
 
     Returns:
+    -------
         A Python dictionary (text) with the response from
         the Omnik Inverter.
 
     Raises:
+    ------
         OmnikInverterPacketInvalidError: Received data fails basic validity checks.
     """
-
     info = None
 
-    for (message_type, reply_serial_number, message) in _unpack_messages(
-        bytearray(data)
-    ):
+    for message_type, reply_serial_number, message in _unpack_messages(bytearray(data)):
         if reply_serial_number != serial_number:  # pragma: no cover
             # This is allowed as it does not seem to be required to pass the serial
             # number in the request - though empirical testing has to point out whether
             # the request takes longer this way.
             LOGGER.debug(
                 "Replied serial number %s not equal to request %s",
                 reply_serial_number,
@@ -208,26 +226,27 @@
 
         if message_type == MESSAGE_TYPE_INFORMATION_REPLY:
             if info is not None:  # pragma: no cover
                 LOGGER.warning("Omnik sent multiple INFORMATION_REPLY messages")
             info = _parse_information_reply(message)
         elif message_type == MESSAGE_TYPE_STRING:  # pragma: no cover
             LOGGER.warning(
-                "Omnik sent text message `%s`", message.decode("utf8").strip()
+                "Omnik sent text message `%s`",
+                message.decode("utf8").strip(),
             )
         else:
-            raise OmnikInverterPacketInvalidError(
+            msg = (
                 f"Unknown Omnik message type {message_type:02x} "
-                f"with contents `{message}`",
+                f"with contents `{message}`"
             )
+            raise OmnikInverterPacketInvalidError(msg)
 
     if info is None:
-        raise OmnikInverterPacketInvalidError(
-            "None of the messages contained an information reply!"
-        )
+        msg = "None of the messages contained an information reply!"
+        raise OmnikInverterPacketInvalidError(msg)
 
     return info
 
 
 def _parse_information_reply(data: bytes) -> dict[str, Any]:
     tcp_data = _TcpData.from_buffer_copy(data)
 
@@ -242,26 +261,26 @@
     # uncovered.
     for idx in range(1, 5):  # pragma: no cover
         name = f"padding{idx}"
         padding = getattr(tcp_data, name)
         if sum(padding):
             LOGGER.warning("Unexpected `%s`: `%s`", name, padding)
 
-    def list_divide_10(integers: list[int]) -> list[Optional[float]]:
+    def list_divide_10(integers: list[int]) -> list[float | None]:
         return [None if v == UINT16_MAX else v * 0.1 for v in integers]
 
     def int_to_bool(num: int) -> bool:
         return {
             0: False,
             1: True,
         }[num]
 
     # Set temperature to None if it matches 65326, this is returned
     # when the inverter is "offline".
-    def temperature_to_float(temp: int) -> Optional[float]:
+    def temperature_to_float(temp: int) -> float | None:
         return None if temp == 65326 else temp * 0.1
 
     # Only these fields will be extracted from the structure
     field_extractors = {
         "serial_number": None,
         "temperature": temperature_to_float,
         "dc_input_voltage": list_divide_10,
@@ -275,15 +294,15 @@
         "inverter_active": int_to_bool,
         "firmware": None,
         "firmware_slave": None,
     }
 
     result: dict[str, Any] = {}
 
-    for (name, extractor) in field_extractors.items():
+    for name, extractor in field_extractors.items():
         value = getattr(tcp_data, name)
 
         if name == "ac_output":
             # Flatten the list of frequency+power AC objects
 
             result["ac_output_frequency"] = [o.get_frequency() for o in value]
             result["ac_output_power"] = [o.get_power() for o in value]
```

### Comparing `omnikinverter-0.9.0/pyproject.toml` & `omnikinverter-0.9.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omnikinverter"
-version = "0.9.0"
+version = "0.9.1"
 description = "Asynchronous Python client for the Omnik Inverter"
 authors = ["Klaas Schoute <hello@student-techlife.com>"]
 maintainers = ["Klaas Schoute <hello@student-techlife.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/klaasnicolaas/python-omnikinverter"
 repository = "https://github.com/klaasnicolaas/python-omnikinverter"
@@ -14,116 +14,96 @@
     "Development Status :: 5 - Production/Stable",
     "Framework :: AsyncIO",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 packages = [
     { include = "omnikinverter" },
 ]
 
 [tool.poetry.dependencies]
-python = "^3.9"
 aiohttp = ">=3.0.0"
+python = "^3.9"
 yarl = ">=1.6.0"
-asynctest = "^0.13.0"
-
-[tool.poetry.group.dev.dependencies]
-aresponses = "^2.1.6"
-bandit = "^1.7.4"
-black = "^22.10"
-blacken-docs = "^1.12.1"
-codespell = "^2.2.2"
-coverage = {version = "^6.5", extras = ["toml"]}
-darglint = "^1.8.1"
-flake8 = "^4.0.1"
-flake8-bandit = "^3.0.0"
-flake8-bugbear = "^22.10.27"
-flake8-builtins = "^2.0.1"
-flake8-comprehensions = "^3.10.1"
-flake8-docstrings = "^1.5.0"
-flake8-eradicate = "^1.4.0"
-flake8-markdown = "^0.3.0"
-flake8-simplify = "^0.19.3"
-isort = "^5.10.1"
-mypy = "^0.991"
-pre-commit = "^2.20.0"
-pre-commit-hooks = "^4.3.0"
-pylint = "^2.15.6"
-pytest = "^7.2.0"
-pytest-asyncio = "^0.20.2"
-pytest-cov = "^4.0.0"
-pyupgrade = "^3.2.2"
-safety = "^2.3.2"
-vulture = "^2.6"
-yamllint = "^1.28.0"
-types-cachetools = "^5.2.1"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/klaasnicolaas/python-omnikinverter/issues"
 Changelog = "https://github.com/klaasnicolaas/python-omnikinverter/releases"
 
+[tool.poetry.group.dev.dependencies]
+ruff = ">=0.0.243,<0.0.262"
+aresponses = "^2.1.6"
+black = ">=22.10,<24.0"
+blacken-docs = "^1.13.0"
+codespell = "^2.2.4"
+coverage = {version = ">=7.2,<8.0", extras = ["toml"]}
+mypy = ">=1.0,<1.3"
+pre-commit = ">=3.2,<4.0"
+pre-commit-hooks = "^4.4.0"
+pylint = "^2.17.1"
+pytest = "^7.2.2"
+pytest-asyncio = "^0.21.0"
+pytest-cov = "^4.0.0"
+yamllint = "^1.30.0"
+covdefaults = "^2.3.0"
+
 [tool.black]
 target-version = ['py39']
 
 [tool.coverage.paths]
 source = ["omnikinverter"]
 
-[tool.coverage.report]
-show_missing = true
-exclude_lines = ["pragma: no cover", "if TYPE_CHECKING:"]
-
 [tool.coverage.run]
-branch = true
+plugins = ["covdefaults"]
 source = ["omnikinverter"]
 
-[tool.isort]
-profile = "black"
-multi_line_output = 3
-
 [tool.mypy]
 # Specify the target platform details in config, so your developers are
 # free to run mypy on Windows, Linux, or macOS and get consistent
 # results.
 platform = "linux"
-python_version = 3.9
-
-# flake8-mypy expects the two following for sensible formatting
-show_column_numbers = true
+python_version = "3.9"
 
 # show error messages from unrelated files
 follow_imports = "normal"
 
 # suppress errors about unsatisfied imports
 ignore_missing_imports = true
 
 # be strict
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_subclassing_any = true
 disallow_untyped_calls = true
 disallow_untyped_defs = true
-disallow_untyped_decorators = false # thanks backoff :(
+disallow_untyped_decorators = true
 no_implicit_optional = true
 no_implicit_reexport = true
 strict_optional = true
 warn_incomplete_stub = true
 warn_no_return = true
 warn_redundant_casts = true
 warn_return_any = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
-# No incremental mode
-cache_dir = "/dev/null"
+[tool.pylint.MASTER]
+extension-pkg-whitelist = [
+  "pydantic"
+]
+ignore= [
+  "tests"
+]
 
 [tool.pylint.BASIC]
 good-names = [
     "_",
     "ex",
     "fp",
     "i",
@@ -131,36 +111,53 @@
     "j",
     "k",
     "on",
     "Run",
     "T",
 ]
 
+[tool.pylint.DESIGN]
+max-attributes=20
+
 [tool.pylint."MESSAGES CONTROL"]
 disable= [
     "too-few-public-methods",
     "duplicate-code",
     "format",
     "unsubscriptable-object",
 ]
 
 [tool.pylint.SIMILARITIES]
 ignore-imports = true
 
 [tool.pylint.FORMAT]
 max-line-length=88
 
-[tool.pylint.DESIGN]
-max-attributes=20
-
 [tool.pytest.ini_options]
 addopts = "--cov"
 asyncio_mode = "auto"
 
-[tool.vulture]
-min_confidence = 80
-paths = ["omnikinverter"]
-verbose = true
+[tool.ruff]
+select = ["ALL"]
+ignore = [
+  "ANN101", # Self... explanatory
+  "ANN401", # Opinionated warning on disallowing dynamically typed expressions
+  "D203", # Conflicts with other rules
+  "D213", # Conflicts with other rules
+  "D417", # False positives in some occasions
+  "PLR2004", # Just annoying, not really useful
+  "TRY300", # Conflicts with RET505
+]
+
+[tool.ruff.flake8-pytest-style]
+mark-parentheses = false
+fixture-parentheses = false
+
+[tool.ruff.isort]
+known-first-party = ["omnikinverter"]
+
+[tool.ruff.mccabe]
+max-complexity = 25
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `omnikinverter-0.9.0/setup.py` & `omnikinverter-0.9.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,265 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: omnikinverter
+Version: 0.9.1
+Summary: Asynchronous Python client for the Omnik Inverter
+Home-page: https://github.com/klaasnicolaas/python-omnikinverter
+License: MIT
+Keywords: omnik,inverter,power,energy,async,client
+Author: Klaas Schoute
+Author-email: hello@student-techlife.com
+Maintainer: Klaas Schoute
+Maintainer-email: hello@student-techlife.com
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: AsyncIO
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: aiohttp (>=3.0.0)
+Requires-Dist: yarl (>=1.6.0)
+Project-URL: Bug Tracker, https://github.com/klaasnicolaas/python-omnikinverter/issues
+Project-URL: Changelog, https://github.com/klaasnicolaas/python-omnikinverter/releases
+Project-URL: Documentation, https://github.com/klaasnicolaas/python-omnikinverter
+Project-URL: Repository, https://github.com/klaasnicolaas/python-omnikinverter
+Description-Content-Type: text/markdown
 
-packages = \
-['omnikinverter']
+<!-- Banner -->
+![alt Banner of the Omnik Inverter package](https://raw.githubusercontent.com/klaasnicolaas/python-omnikinverter/main/assets/header_omnik_inverter-min.png)
 
-package_data = \
-{'': ['*']}
+<!-- PROJECT SHIELDS -->
+[![GitHub Release][releases-shield]][releases]
+[![Python Versions][python-versions-shield]][pypi]
+![Project Stage][project-stage-shield]
+![Project Maintenance][maintenance-shield]
+[![License][license-shield]](LICENSE)
 
-install_requires = \
-['aiohttp>=3.0.0', 'asynctest>=0.13.0,<0.14.0', 'yarl>=1.6.0']
-
-setup_kwargs = {
-    'name': 'omnikinverter',
-    'version': '0.9.0',
-    'description': 'Asynchronous Python client for the Omnik Inverter',
-    'long_description': '<!-- Banner -->\n![alt Banner of the Omnik Inverter package](https://raw.githubusercontent.com/klaasnicolaas/python-omnikinverter/main/assets/header_omnik_inverter-min.png)\n\n<!-- PROJECT SHIELDS -->\n[![GitHub Release][releases-shield]][releases]\n[![Python Versions][python-versions-shield]][pypi]\n![Project Stage][project-stage-shield]\n![Project Maintenance][maintenance-shield]\n[![License][license-shield]](LICENSE)\n\n[![GitHub Activity][commits-shield]][commits-url]\n[![PyPi Downloads][downloads-shield]][downloads-url]\n[![GitHub Last Commit][last-commit-shield]][commits-url]\n[![Stargazers][stars-shield]][stars-url]\n[![Issues][issues-shield]][issues-url]\n\n[![Maintainability][maintainability-shield]][maintainability-url]\n[![Code Coverage][codecov-shield]][codecov-url]\n\n[![Code Quality][code-quality-shield]][code-quality]\n[![Build Status][build-shield]][build-url]\n\nAsynchronous Python client for the Omnik Inverter.\n\n## About\n\nA python package with which you can read the data from your Omnik Inverter. Keep in mind that this repository uses webscraping, this is **not** a neat way of data processing but due to the lack of a local API this is the only option.\n\n**NOTE**: In mid-2021, manufacturer Omnik was declared bankrupt. You can find more information about what your alternatives are [here][energiewacht].\n\n## Supported models\n\n| Brand    | Model            | Datasource |\n|----------|------------------|------------|\n| Omnik    | Omniksol 1000TL  | JS         |\n| Omnik    | Omniksol 1500TL  | JS         |\n| Omnik    | Omniksol 2000TL  | JS         |\n| Omnik    | Omniksol 2000TL2 | JSON       |\n| Omnik    | Omniksol 2500TL  | HTML       |\n| Omnik    | Omniksol 3000TL  | TCP        |\n| Omnik    | Omniksol 4000TL2 | JS         |\n| Ginlong  | Solis-DLS-WiFi   | JSON/HTML  |\n| Hosola   | 1500TL           | JS         |\n| Bosswerk | BW-MI300         | HTML       |\n| Bosswerk | BW-MI600         | HTML       |\n| Sofar    | 3600TLM          | HTML       |\n| Sofar    | 2200TL           | JS         |\n| Huayu    | HY-600-Pro       | HTML       |\n\n## Installation\n\n```bash\npip install omnikinverter\n```\n\n## Usage\n\n```python\nimport asyncio\n\nfrom omnikinverter import OmnikInverter\n\n\nasync def main():\n    """Show example on getting Omnik Inverter data."""\n    async with OmnikInverter(\n        host="example_host",\n        source_type="javascript",\n        username="omnik",\n        password="inverter",\n    ) as client:\n        inverter = await client.inverter()\n        device = await client.device()\n        print(inverter)\n        print(device)\n\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\nFor the **source type** you can choose between: `javascript` (default), `json`, `html` and `tcp`.\n\n## Data\n\nYou can read the following data with this package:\n\n### Inverter\n\n- Serial Number\n- Inverter Model\n- Firmware Version - Main\n- Firmware Version - Slave\n- Alarm Code\n- Rated Power (W)\n- Current Power Production (W)\n- Day Energy Production (kWh)\n- Total Energy Production (kWh)\n\nOn the `tcp` source type you can also find:\n\n- Inverter temperature;\n- Voltage and current for the DC input strings (up to 3)\n- Voltage, current, frequency and power for all AC outputs (also up to 3)\n- Total number of runtime hours.\n\n### Device\n\n- Signal Quality (only with JS)\n- Firmware Version\n- IP Address\n\n## Use cases\n\nThis python package is used in the following projects, among others:\n\n- [home-assistant-omnik-inverter][omnik-inverter] by Robbin Janssen\n\n## Contributing\n\nThis is an active open-source project. We are always open to people who want to\nuse the code or contribute to it.\n\nWe\'ve set up a separate document for our\n[contribution guidelines](CONTRIBUTING.md).\n\nThank you for being involved! :heart_eyes:\n\n## Setting up development environment\n\nThis Python project is fully managed using the [Poetry][poetry] dependency\nmanager.\n\nYou need at least:\n\n- Python 3.9+\n- [Poetry][poetry-install]\n\nInstall all packages, including all development requirements:\n\n```bash\npoetry install\n```\n\nPoetry creates by default an virtual environment where it installs all\nnecessary pip packages, to enter or exit the venv run the following commands:\n\n```bash\npoetry shell\nexit\n```\n\nSetup the pre-commit check, you must run this inside the virtual environment:\n\n```bash\npre-commit install\n```\n\n*Now you\'re all set to get started!*\n\nAs this repository uses the [pre-commit][pre-commit] framework, all changes\nare linted and tested with each commit. You can run all checks and tests\nmanually, using the following command:\n\n```bash\npoetry run pre-commit run --all-files\n```\n\nTo run just the Python tests:\n\n```bash\npoetry run pytest\n```\n\n## License\n\nMIT License\n\nCopyright (c) 2021-2023 Klaas Schoute\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the "Software"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n\n<!-- MARKDOWN LINKS & IMAGES -->\n[build-shield]: https://github.com/klaasnicolaas/python-omnikinverter/actions/workflows/tests.yaml/badge.svg\n[build-url]: https://github.com/klaasnicolaas/python-omnikinverter/actions/workflows/tests.yaml\n[code-quality-shield]: https://github.com/klaasnicolaas/python-omnikinverter/actions/workflows/codeql.yaml/badge.svg\n[code-quality]: https://github.com/klaasnicolaas/python-omnikinverter/actions/workflows/codeql.yaml\n[commits-shield]: https://img.shields.io/github/commit-activity/y/klaasnicolaas/python-omnikinverter.svg\n[commits-url]: https://github.com/klaasnicolaas/python-omnikinverter/commits/main\n[codecov-shield]: https://codecov.io/gh/klaasnicolaas/python-omnikinverter/branch/main/graph/badge.svg?token=VQTR24YFQ9\n[codecov-url]: https://codecov.io/gh/klaasnicolaas/python-omnikinverter\n[downloads-shield]: https://img.shields.io/pypi/dm/omnikinverter\n[downloads-url]: https://pypistats.org/packages/omnikinverter\n[issues-shield]: https://img.shields.io/github/issues/klaasnicolaas/python-omnikinverter.svg\n[issues-url]: https://github.com/klaasnicolaas/python-omnikinverter/issues\n[license-shield]: https://img.shields.io/github/license/klaasnicolaas/python-omnikinverter.svg\n[last-commit-shield]: https://img.shields.io/github/last-commit/klaasnicolaas/python-omnikinverter.svg\n[maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg\n[maintainability-shield]: https://api.codeclimate.com/v1/badges/ec5166b74a63f375d1a1/maintainability\n[maintainability-url]: https://codeclimate.com/github/klaasnicolaas/python-omnikinverter/maintainability\n[project-stage-shield]: https://img.shields.io/badge/project%20stage-experimental-yellow.svg\n[pypi]: https://pypi.org/project/omnikinverter/\n[python-versions-shield]: https://img.shields.io/pypi/pyversions/omnikinverter\n[releases-shield]: https://img.shields.io/github/release/klaasnicolaas/python-omnikinverter.svg\n[releases]: https://github.com/klaasnicolaas/python-omnikinverter/releases\n[stars-shield]: https://img.shields.io/github/stars/klaasnicolaas/python-omnikinverter.svg\n[stars-url]: https://github.com/klaasnicolaas/python-omnikinverter/stargazers\n\n[energiewacht]: https://www.energiewacht.com/hoofdsite/home/nieuws/omnik-failliet/\n[omnik-inverter]: https://github.com/robbinjanssen/home-assistant-omnik-inverter\n[poetry-install]: https://python-poetry.org/docs/#installation\n[poetry]: https://python-poetry.org\n[pre-commit]: https://pre-commit.com\n',
-    'author': 'Klaas Schoute',
-    'author_email': 'hello@student-techlife.com',
-    'maintainer': 'Klaas Schoute',
-    'maintainer_email': 'hello@student-techlife.com',
-    'url': 'https://github.com/klaasnicolaas/python-omnikinverter',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
+[![GitHub Activity][commits-shield]][commits-url]
+[![PyPi Downloads][downloads-shield]][downloads-url]
+[![GitHub Last Commit][last-commit-shield]][commits-url]
+[![Stargazers][stars-shield]][stars-url]
+[![Issues][issues-shield]][issues-url]
 
+[![Maintainability][maintainability-shield]][maintainability-url]
+[![Code Coverage][codecov-shield]][codecov-url]
+
+[![Code Quality][code-quality-shield]][code-quality]
+[![Build Status][build-shield]][build-url]
+
+Asynchronous Python client for the Omnik Inverter.
+
+## About
+
+A python package with which you can read the data from your Omnik Inverter. Keep in mind that this repository uses webscraping, this is **not** a neat way of data processing but due to the lack of a local API this is the only option.
+
+**NOTE**: In mid-2021, manufacturer Omnik was declared bankrupt. You can find more information about what your alternatives are [here][energiewacht].
+
+## Supported models
+
+| Brand    | Model            | Datasource |
+|----------|------------------|------------|
+| Omnik    | Omniksol 1000TL  | JS         |
+| Omnik    | Omniksol 1500TL  | JS         |
+| Omnik    | Omniksol 2000TL  | JS         |
+| Omnik    | Omniksol 2000TL2 | JSON       |
+| Omnik    | Omniksol 2500TL  | HTML       |
+| Omnik    | Omniksol 3000TL  | TCP        |
+| Omnik    | Omniksol 4000TL2 | JS         |
+| Ginlong  | Solis-DLS-WiFi   | JSON/HTML  |
+| Hosola   | 1500TL           | JS         |
+| Hosala   | Bright 2500MTL-S | JS         |
+| Bosswerk | BW-MI300         | HTML       |
+| Bosswerk | BW-MI600         | HTML       |
+| Sofar    | 3600TLM          | HTML       |
+| Sofar    | 2200TL           | JS         |
+| Huayu    | HY-600-Pro       | HTML       |
+
+## Installation
+
+```bash
+pip install omnikinverter
+```
+
+## Usage
+
+```python
+import asyncio
+
+from omnikinverter import OmnikInverter
+
+
+async def main():
+    """Show example on getting Omnik Inverter data."""
+    async with OmnikInverter(
+        host="example_host",
+        source_type="javascript",
+        username="omnik",
+        password="inverter",
+    ) as client:
+        inverter = await client.inverter()
+        device = await client.device()
+        print(inverter)
+        print(device)
+
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
+
+For the **source type** you can choose between: `javascript` (default), `json`, `html` and `tcp`.
+
+## Data
+
+You can read the following data with this package:
+
+### Inverter
+
+- Serial Number
+- Inverter Model
+- Firmware Version - Main
+- Firmware Version - Slave
+- Alarm Code
+- Rated Power (W)
+- Current Power Production (W)
+- Day Energy Production (kWh)
+- Total Energy Production (kWh)
+
+On the `tcp` source type you can also find:
+
+- Inverter temperature;
+- Voltage and current for the DC input strings (up to 3)
+- Voltage, current, frequency and power for all AC outputs (also up to 3)
+- Total number of runtime hours.
+
+### Device
+
+- Signal Quality (only with JS)
+- Firmware Version
+- IP Address
+
+## Use cases
+
+This python package is used in the following projects, among others:
+
+- [home-assistant-omnik-inverter][omnik-inverter] by Robbin Janssen
+
+## Contributing
+
+This is an active open-source project. We are always open to people who want to
+use the code or contribute to it.
+
+We've set up a separate document for our
+[contribution guidelines](CONTRIBUTING.md).
+
+Thank you for being involved! :heart_eyes:
+
+## Setting up development environment
+
+This Python project is fully managed using the [Poetry][poetry] dependency
+manager.
+
+You need at least:
+
+- Python 3.9+
+- [Poetry][poetry-install]
+
+Install all packages, including all development requirements:
+
+```bash
+poetry install
+```
+
+Poetry creates by default an virtual environment where it installs all
+necessary pip packages, to enter or exit the venv run the following commands:
+
+```bash
+poetry shell
+exit
+```
+
+Setup the pre-commit check, you must run this inside the virtual environment:
+
+```bash
+pre-commit install
+```
+
+*Now you're all set to get started!*
+
+As this repository uses the [pre-commit][pre-commit] framework, all changes
+are linted and tested with each commit. You can run all checks and tests
+manually, using the following command:
+
+```bash
+poetry run pre-commit run --all-files
+```
+
+To run just the Python tests:
+
+```bash
+poetry run pytest
+```
+
+## License
+
+MIT License
+
+Copyright (c) 2021-2023 Klaas Schoute
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+<!-- MARKDOWN LINKS & IMAGES -->
+[build-shield]: https://github.com/klaasnicolaas/python-omnikinverter/actions/workflows/tests.yaml/badge.svg
+[build-url]: https://github.com/klaasnicolaas/python-omnikinverter/actions/workflows/tests.yaml
+[code-quality-shield]: https://github.com/klaasnicolaas/python-omnikinverter/actions/workflows/codeql.yaml/badge.svg
+[code-quality]: https://github.com/klaasnicolaas/python-omnikinverter/actions/workflows/codeql.yaml
+[commits-shield]: https://img.shields.io/github/commit-activity/y/klaasnicolaas/python-omnikinverter.svg
+[commits-url]: https://github.com/klaasnicolaas/python-omnikinverter/commits/main
+[codecov-shield]: https://codecov.io/gh/klaasnicolaas/python-omnikinverter/branch/main/graph/badge.svg?token=VQTR24YFQ9
+[codecov-url]: https://codecov.io/gh/klaasnicolaas/python-omnikinverter
+[downloads-shield]: https://img.shields.io/pypi/dm/omnikinverter
+[downloads-url]: https://pypistats.org/packages/omnikinverter
+[issues-shield]: https://img.shields.io/github/issues/klaasnicolaas/python-omnikinverter.svg
+[issues-url]: https://github.com/klaasnicolaas/python-omnikinverter/issues
+[license-shield]: https://img.shields.io/github/license/klaasnicolaas/python-omnikinverter.svg
+[last-commit-shield]: https://img.shields.io/github/last-commit/klaasnicolaas/python-omnikinverter.svg
+[maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg
+[maintainability-shield]: https://api.codeclimate.com/v1/badges/ec5166b74a63f375d1a1/maintainability
+[maintainability-url]: https://codeclimate.com/github/klaasnicolaas/python-omnikinverter/maintainability
+[project-stage-shield]: https://img.shields.io/badge/project%20stage-experimental-yellow.svg
+[pypi]: https://pypi.org/project/omnikinverter/
+[python-versions-shield]: https://img.shields.io/pypi/pyversions/omnikinverter
+[releases-shield]: https://img.shields.io/github/release/klaasnicolaas/python-omnikinverter.svg
+[releases]: https://github.com/klaasnicolaas/python-omnikinverter/releases
+[stars-shield]: https://img.shields.io/github/stars/klaasnicolaas/python-omnikinverter.svg
+[stars-url]: https://github.com/klaasnicolaas/python-omnikinverter/stargazers
+
+[energiewacht]: https://www.energiewacht.com/hoofdsite/home/nieuws/omnik-failliet/
+[omnik-inverter]: https://github.com/robbinjanssen/home-assistant-omnik-inverter
+[poetry-install]: https://python-poetry.org/docs/#installation
+[poetry]: https://python-poetry.org
+[pre-commit]: https://pre-commit.com
 
-setup(**setup_kwargs)
```

