# Comparing `tmp/smspdudecoder-2.0.3.tar.gz` & `tmp/smspdudecoder-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smspdudecoder-2.0.3.tar", last modified: Mon Feb  7 14:31:58 2022, max compression
+gzip compressed data, was "smspdudecoder-2.1.0.tar", last modified: Wed Apr 12 19:26:25 2023, max compression
```

## Comparing `smspdudecoder-2.0.3.tar` & `smspdudecoder-2.1.0.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 14:31:58.880077 smspdudecoder-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-02-07 14:31:48.000000 smspdudecoder-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2359 2022-02-07 14:31:58.880077 smspdudecoder-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1605 2022-02-07 14:31:48.000000 smspdudecoder-2.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-07 14:31:58.880077 smspdudecoder-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1226 2022-02-07 14:31:48.000000 smspdudecoder-2.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 14:31:58.880077 smspdudecoder-2.0.3/smspdudecoder/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-07 14:31:48.000000 smspdudecoder-2.0.3/smspdudecoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5968 2022-02-07 14:31:48.000000 smspdudecoder-2.0.3/smspdudecoder/codecs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-02-07 14:31:48.000000 smspdudecoder-2.0.3/smspdudecoder/easy.py
--rw-r--r--   0 runner    (1001) docker     (121)     6385 2022-02-07 14:31:48.000000 smspdudecoder-2.0.3/smspdudecoder/elements.py
--rw-r--r--   0 runner    (1001) docker     (121)     7485 2022-02-07 14:31:48.000000 smspdudecoder-2.0.3/smspdudecoder/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 14:31:58.880077 smspdudecoder-2.0.3/smspdudecoder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2359 2022-02-07 14:31:58.000000 smspdudecoder-2.0.3/smspdudecoder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      368 2022-02-07 14:31:58.000000 smspdudecoder-2.0.3/smspdudecoder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-07 14:31:58.000000 smspdudecoder-2.0.3/smspdudecoder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-07 14:31:58.000000 smspdudecoder-2.0.3/smspdudecoder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-02-07 14:31:58.000000 smspdudecoder-2.0.3/smspdudecoder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-02-07 14:31:58.000000 smspdudecoder-2.0.3/smspdudecoder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:26:25.523870 smspdudecoder-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-12 19:26:13.000000 smspdudecoder-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-12 19:26:25.523870 smspdudecoder-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-12 19:26:13.000000 smspdudecoder-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 19:26:25.523870 smspdudecoder-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-12 19:26:13.000000 smspdudecoder-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:26:25.523870 smspdudecoder-2.1.0/smspdudecoder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:26:13.000000 smspdudecoder-2.1.0/smspdudecoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-04-12 19:26:13.000000 smspdudecoder-2.1.0/smspdudecoder/codecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-12 19:26:13.000000 smspdudecoder-2.1.0/smspdudecoder/easy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-04-12 19:26:13.000000 smspdudecoder-2.1.0/smspdudecoder/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10140 2023-04-12 19:26:13.000000 smspdudecoder-2.1.0/smspdudecoder/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:26:25.523870 smspdudecoder-2.1.0/smspdudecoder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-12 19:26:25.000000 smspdudecoder-2.1.0/smspdudecoder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-12 19:26:25.000000 smspdudecoder-2.1.0/smspdudecoder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 19:26:25.000000 smspdudecoder-2.1.0/smspdudecoder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 19:26:25.000000 smspdudecoder-2.1.0/smspdudecoder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-12 19:26:25.000000 smspdudecoder-2.1.0/smspdudecoder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-12 19:26:25.000000 smspdudecoder-2.1.0/smspdudecoder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:26:25.523870 smspdudecoder-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-12 19:26:13.000000 smspdudecoder-2.1.0/tests/test_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-12 19:26:13.000000 smspdudecoder-2.1.0/tests/test_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-12 19:26:13.000000 smspdudecoder-2.1.0/tests/test_elements.py
```

### Comparing `smspdudecoder-2.0.3/LICENSE` & `smspdudecoder-2.1.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2018 Qotto
+Copyright (c) 2018-2023 Qotto
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `smspdudecoder-2.0.3/PKG-INFO` & `smspdudecoder-2.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: smspdudecoder
-Version: 2.0.3
+Version: 2.1.0
 Summary: Python SMS PDU Decoder
 Home-page: https://github.com/qotto/smspdudecoder
 Author: Alexandre Syenchuk
 Author-email: sacha@qotto.net
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Communications :: Telephony
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SMS-PDU Decoder
 
+[![PyPI version](https://badge.fury.io/py/smspdudecoder.svg)](https://badge.fury.io/py/smspdudecoder)
+
 This library will help you to decode raw SMS data you can get from a GSM modem (generally by using AT commands).
 
 It has some encoding functionality as well.
 
 It is recommended to read the [GSM 03.40](https://en.wikipedia.org/wiki/GSM_03.40) specification to better understand the components this library works wtih.
 
 ## How to install
@@ -79,9 +80,7 @@
 ```
 
 And use the following command:
 
 ```sh
 make test
 ```
-
-
```

### Comparing `smspdudecoder-2.0.3/README.md` & `smspdudecoder-2.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # SMS-PDU Decoder
 
+[![PyPI version](https://badge.fury.io/py/smspdudecoder.svg)](https://badge.fury.io/py/smspdudecoder)
+
 This library will help you to decode raw SMS data you can get from a GSM modem (generally by using AT commands).
 
 It has some encoding functionality as well.
 
 It is recommended to read the [GSM 03.40](https://en.wikipedia.org/wiki/GSM_03.40) specification to better understand the components this library works wtih.
 
 ## How to install
```

### Comparing `smspdudecoder-2.0.3/setup.py` & `smspdudecoder-2.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 if __name__ == '__main__':
     setup(
         name='smspdudecoder',
-        version='2.0.3',
+        version='2.1.0',
         url='https://github.com/qotto/smspdudecoder',
         license='MIT',
         author='Alexandre Syenchuk',
         author_email='sacha@qotto.net',
         description='Python SMS PDU Decoder',
         long_description=long_description,
         long_description_content_type="text/markdown",
```

### Comparing `smspdudecoder-2.0.3/smspdudecoder/codecs.py` & `smspdudecoder-2.1.0/smspdudecoder/codecs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# coding: utf-8
-# Copyright (c) Qotto, 2018-2019
+# Copyright (c) Qotto, 2018-2023
 # Open-source software, see LICENSE file for details
 
 """
 Implementation of different codecs used in SMS PDUs, according to the GSM 03.38 specification.
 """
 
 from binascii import hexlify
```

### Comparing `smspdudecoder-2.0.3/smspdudecoder/easy.py` & `smspdudecoder-2.1.0/smspdudecoder/easy.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-# coding: utf-8
-# Copyright (c) Qotto, 2018-2019
+# Copyright (c) Qotto, 2018-2023
 # Open-source software, see LICENSE file for details
 
-from .fields import SMSDeliver
 from io import StringIO
-
 from typing import Any, Dict
 
-__all__ = ['easy_sms']
+from .fields import SMSDeliver, SMSSubmit
+
+__all__ = [
+    'read_incoming_sms',
+    'read_outgoing_sms',
+]
+
 
-def easy_sms(data: str) -> Dict[str, Any]:
+def read_incoming_sms(data: str) -> Dict[str, Any]:
     sms = SMSDeliver.decode(StringIO(data))
     sender = sms['sender']['number']
     if sms['sender']['toa']['ton'] == 'international':
         sender = '+' + sender
     date = sms['scts']
     content = sms['user_data']['data']
     header = sms['user_data'].get('header')
@@ -29,7 +32,19 @@
                 }
     return {
         'sender': sender,
         'date': date,
         'content': content,
         'partial': partial,
     }
+
+
+def read_outgoing_sms(data: str) -> Dict[str, Any]:
+    sms = SMSSubmit.decode(StringIO(data))
+    recipient = sms['recipient']['number']
+    if sms['recipient']['toa']['ton'] == 'international':
+        recipient = '+' + recipient
+    content = sms['user_data']['data']
+    return {
+        'recipient': recipient,
+        'content': content,
+    }
```

### Comparing `smspdudecoder-2.0.3/smspdudecoder/elements.py` & `smspdudecoder-2.1.0/smspdudecoder/elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,32 @@
-# coding: utf-8
-# Copyright (c) Qotto, 2018-2019
+# Copyright (c) Qotto, 2018-2023
 # Open-source software, see LICENSE file for details
 
 """
 Various elements used in TP-DU, according to GSM 03.40.
 
 All these elements are encoded in strings and decoded in native Python objects.
 """
 
-import pytz
-
-from bitstring import BitStream
 from datetime import datetime
 from datetime import timedelta
 from datetime import timezone
 from io import StringIO
+from typing import Dict
+
+import pytz
+
+from bitstring import BitStream
 
-from typing import Any, Dict
+__all__ = [
+    'Date',
+    'Number',
+    'TypeOfAddress',
+]
 
-__all__ = ['Date', 'Number', 'TypeOfAddress']
 
 def swap_nibbles(data: str) -> str:
     """
     Swaps nibbles (semi-octets) in the PDU hex string and returns the result.
 
     Example:
```

### Comparing `smspdudecoder-2.0.3/smspdudecoder/fields.py` & `smspdudecoder-2.1.0/smspdudecoder/fields.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# coding: utf-8
-# Copyright (c) Qotto, 2018-2019
+# Copyright (c) Qotto, 2018-2023
 # Open-source software, see LICENSE file for details
 
 """
 TP-DU fields according to GSM 03.40.
 
 Unlike elements, fields represent independent datagram chunks, and are decoded from a file-like object.
 
@@ -71,14 +70,21 @@
 
         Example:
 
         >>> SMSC.decode(StringIO('07912299976758F2'))
         {'length': 7, 'toa': {'ton': 'international', 'npi': 'isdn'}, 'number': '22997976852'}
         """
         length = int(pdu_data.read(2), 16)
+        if not length:
+            return {
+                'length': 0,
+                'toa': None,
+                'number': None,
+            }
+
         toa = TypeOfAddress.decode(pdu_data.read(2))
         encoded_number = pdu_data.read(2*(length-1))
         if toa['ton'] == 'alphanumeric':
             number = GSM.decode(encoded_number)
         else:
             number = Number.decode(encoded_number)
         return {
@@ -122,14 +128,52 @@
         # Message Type Indicator
         result['mti'] = cls.MTI.get(io_data.read('bits:2').uint)
         if result['mti'] is None:
             raise ValueError("Invalid Message Type Indicator")
         return result
 
 
+class OutgoingPDUHeader:
+    """
+    Describes the outgoing TPDU header of SM-TP
+    """
+    MTI = {
+        0b00: 'deliver',
+        0b01: 'submit',
+        0b10: 'status',
+    }
+    MTI_INV = dict([(v[1], v[0]) for v in MTI.items()])
+
+    @classmethod
+    def decode(cls, pdu_data: StringIO) -> Dict[str, Any]:
+        """
+        Decodes an outgoing PDU header.
+
+        >>> OutgoingPDUHeader.decode(StringIO('11'))
+        {'rp': False, 'udhi': True, 'sri': False, 'lp': False, 'mms': True, 'mti': 'deliver'}
+        """
+        result = dict()
+        io_data = BitStream(hex=pdu_data.read(2))
+        # Reply Path
+        result['rp'] = io_data.read('bool')
+        # User Data Header Indicator
+        result['udhi'] = io_data.read('bool')
+        # Status Report Request
+        result['srr'] = io_data.read('bool')
+        # Validity Period Format
+        result['vpf'] = io_data.read('bits:2').uint
+        # Reject Duplicates
+        result['rd'] = io_data.read('bool')
+        # Message Type Indicator
+        result['mti'] = cls.MTI.get(io_data.read('bits:2').uint)
+        if result['mti'] is None:
+            raise ValueError("Invalid Message Type Indicator")
+        return result
+
+
 class DCS:
     """
     Data Coding Scheme (simplified, only the encoding is read)
     """
     @classmethod
     def decode(cls, pdu_data: StringIO) -> Dict[str, str]:
         dcs = int(pdu_data.read(2), 16)
@@ -230,7 +274,44 @@
         result['header'] = PDUHeader.decode(pdu_data)
         result['sender'] = Address.decode(pdu_data)
         result['pid'] = int(pdu_data.read(2), 16)
         result['dcs'] = DCS.decode(pdu_data)
         result['scts'] = Date.decode(pdu_data.read(2*7))
         result['user_data'] = UserData.decode(pdu_data, result)
         return result
+
+
+class SMSSubmit:
+    """
+    SMS-SUBMIT TP-DU.
+    """
+    @classmethod
+    def decode(cls, pdu_data: StringIO):
+        """
+        Decodes an SMS-SUBMIT TP-DU.
+        """
+        result = dict()
+        result['smsc'] = SMSC.decode(pdu_data)
+        result['header'] = OutgoingPDUHeader.decode(pdu_data)
+        result['message-ref'] = int(pdu_data.read(2), 16)
+        result['recipient'] = Address.decode(pdu_data)
+        result['pid'] = int(pdu_data.read(2), 16)
+        result['dcs'] = DCS.decode(pdu_data)
+        if result['header']['vpf'] == 0:
+            pass
+        elif result['header']['vpf'] == 2:
+            result['vp'] = int(pdu_data.read(2), 16)
+            if result['vp'] <= 143:
+                result['validity-minutes'] = result['vp'] * 5
+            elif result['vp'] <= 167:
+                result['validity-hours'] = 12 + (result['vp'] - 143) // 2
+            elif result['vp'] <= 196:
+                result['validity-days'] = result['vp'] - 166
+            else:
+                result['validity-weeks'] = result['vp'] - 192
+        elif result['header']['vpf'] == 3:
+            result['vp'] = Date.decode(pdu_data.read(2*7))
+        else:
+            pdu_data.read(2*7) # skips the enhanced format
+
+        result['user_data'] = UserData.decode(pdu_data, result)
+        return result
```

### Comparing `smspdudecoder-2.0.3/smspdudecoder.egg-info/PKG-INFO` & `smspdudecoder-2.1.0/smspdudecoder.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: smspdudecoder
-Version: 2.0.3
+Version: 2.1.0
 Summary: Python SMS PDU Decoder
 Home-page: https://github.com/qotto/smspdudecoder
 Author: Alexandre Syenchuk
 Author-email: sacha@qotto.net
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Communications :: Telephony
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SMS-PDU Decoder
 
+[![PyPI version](https://badge.fury.io/py/smspdudecoder.svg)](https://badge.fury.io/py/smspdudecoder)
+
 This library will help you to decode raw SMS data you can get from a GSM modem (generally by using AT commands).
 
 It has some encoding functionality as well.
 
 It is recommended to read the [GSM 03.40](https://en.wikipedia.org/wiki/GSM_03.40) specification to better understand the components this library works wtih.
 
 ## How to install
@@ -79,9 +80,7 @@
 ```
 
 And use the following command:
 
 ```sh
 make test
 ```
-
-
```

