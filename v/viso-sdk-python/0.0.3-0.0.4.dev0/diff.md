# Comparing `tmp/viso_sdk_python-0.0.3-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/viso_sdk_python-0.0.4.dev0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,36 @@
-Zip file size: 1349534 bytes, number of entries: 21
-drwxr-xr-x  2.0 unx        0 b- stor 22-Jun-27 06:59 viso_sdk_python-0.0.3.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Jun-27 06:59 viso_sdk_python.libs/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Jun-27 06:59 viso/
--rw-rw-rw-  2.0 unx      200 b- defN 22-Jun-27 06:59 viso_sdk_python-0.0.3.dist-info/AUTHORS
--rw-rw-r--  2.0 unx     1665 b- defN 22-Jun-27 06:59 viso_sdk_python-0.0.3.dist-info/RECORD
--rw-r--r--  2.0 unx     1931 b- defN 22-Jun-27 06:59 viso_sdk_python-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       32 b- defN 22-Jun-27 06:59 viso_sdk_python-0.0.3.dist-info/dependency_links.txt
--rw-r--r--  2.0 unx      148 b- defN 22-Jun-27 06:59 viso_sdk_python-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 22-Jun-27 06:59 viso_sdk_python-0.0.3.dist-info/top_level.txt
--rw-rw-rw-  2.0 unx     7651 b- defN 22-Jun-27 06:59 viso_sdk_python-0.0.3.dist-info/COPYING
--rw-r--r--  2.0 unx        6 b- defN 22-Jun-27 06:59 viso/VERSION
--rwxr-xr-x  2.0 unx   132192 b- defN 22-Jun-27 06:59 viso/_version.cpython-39-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx   721160 b- defN 22-Jun-27 06:59 viso/redis_util.cpython-39-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx     1017 b- defN 22-Jun-27 06:59 viso/__init__.py
--rw-rw-rw-  2.0 unx        0 b- defN 22-Jun-27 06:59 viso/py.typed
--rwxr-xr-x  2.0 unx   499136 b- defN 22-Jun-27 06:59 viso/logging.cpython-39-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx   760040 b- defN 22-Jun-27 06:59 viso/status.cpython-39-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx   753568 b- defN 22-Jun-27 06:59 viso/common.cpython-39-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx   835736 b- defN 22-Jun-27 06:59 viso/flow.cpython-39-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx   645840 b- defN 22-Jun-27 06:59 viso/mqtt.cpython-39-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx   107520 b- defN 22-Jun-27 06:59 viso/constant.cpython-39-x86_64-linux-gnu.so
-21 files, 4467847 bytes uncompressed, 1346456 bytes compressed:  69.9%
+Zip file size: 26540 bytes, number of entries: 34
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-12 08:54 docs/ext/__init__.py
+-rw-r--r--  2.0 unx     1407 b- defN 23-Apr-12 08:54 docs/ext/docstrings.py
+-rw-rw-rw-  2.0 unx      816 b- defN 23-Apr-12 08:54 docs/ext/manager_tmpl.j2
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-12 08:54 tests/meta/__init__.py
+-rw-r--r--  2.0 unx     3434 b- defN 23-Apr-12 08:54 tests/meta/test_ensure_type_hints.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-12 08:54 tests/smoke/__init__.py
+-rw-r--r--  2.0 unx     1040 b- defN 23-Apr-12 08:54 tests/smoke/test_dists.py
+-rw-r--r--  2.0 unx     1131 b- defN 23-Apr-12 08:54 viso_sdk/__init__.py
+-rw-r--r--  2.0 unx      373 b- defN 23-Apr-12 08:54 viso_sdk/_version.py
+-rw-r--r--  2.0 unx      278 b- defN 23-Apr-12 08:54 viso_sdk/constants/__init__.py
+-rw-r--r--  2.0 unx     2697 b- defN 23-Apr-12 08:54 viso_sdk/constants/constants.py
+-rw-r--r--  2.0 unx      244 b- defN 23-Apr-12 08:54 viso_sdk/constants/modules.py
+-rw-r--r--  2.0 unx     1502 b- defN 23-Apr-12 08:54 viso_sdk/constants/variables.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-12 08:54 viso_sdk/edge/__init__.py
+-rw-r--r--  2.0 unx     2435 b- defN 23-Apr-12 08:54 viso_sdk/edge/common.py
+-rw-r--r--  2.0 unx       77 b- defN 23-Apr-12 08:54 viso_sdk/logging/__init__.py
+-rw-r--r--  2.0 unx     3455 b- defN 23-Apr-12 08:54 viso_sdk/logging/logger.py
+-rw-r--r--  2.0 unx     4603 b- defN 23-Apr-12 08:54 viso_sdk/logging/status_logger.py
+-rw-r--r--  2.0 unx       51 b- defN 23-Apr-12 08:54 viso_sdk/mqtt/__init__.py
+-rw-r--r--  2.0 unx     3424 b- defN 23-Apr-12 08:54 viso_sdk/mqtt/mqtt_wrapper.py
+-rw-r--r--  2.0 unx       45 b- defN 23-Apr-12 08:54 viso_sdk/nodered/__init__.py
+-rw-r--r--  2.0 unx     5658 b- defN 23-Apr-12 08:54 viso_sdk/nodered/flow.py
+-rw-r--r--  2.0 unx       54 b- defN 23-Apr-12 08:54 viso_sdk/redis/__init__.py
+-rw-r--r--  2.0 unx     4406 b- defN 23-Apr-12 08:54 viso_sdk/redis/redis_wrapper.py
+-rw-r--r--  2.0 unx       46 b- defN 23-Apr-12 08:54 viso_sdk/visualize/__init__.py
+-rw-r--r--  2.0 unx     2873 b- defN 23-Apr-12 08:54 viso_sdk/visualize/custom_font.py
+-rw-r--r--  2.0 unx     2400 b- defN 23-Apr-12 08:54 viso_sdk/visualize/palette.py
+-rw-r--r--  2.0 unx     7695 b- defN 23-Apr-12 08:54 viso_sdk/visualize/visualization.py
+-rw-rw-rw-  2.0 unx      166 b- defN 23-Apr-12 08:54 viso_sdk_python-0.0.4.dev0.dist-info/AUTHORS
+-rw-rw-rw-  2.0 unx     7651 b- defN 23-Apr-12 08:54 viso_sdk_python-0.0.4.dev0.dist-info/COPYING
+-rw-r--r--  2.0 unx     1500 b- defN 23-Apr-12 08:54 viso_sdk_python-0.0.4.dev0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 08:54 viso_sdk_python-0.0.4.dev0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-Apr-12 08:54 viso_sdk_python-0.0.4.dev0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2879 b- defN 23-Apr-12 08:54 viso_sdk_python-0.0.4.dev0.dist-info/RECORD
+34 files, 62452 bytes uncompressed, 21882 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -1,64 +1,103 @@
-Filename: viso_sdk_python-0.0.3.dist-info/
+Filename: docs/ext/__init__.py
 Comment: 
 
-Filename: viso_sdk_python.libs/
+Filename: docs/ext/docstrings.py
 Comment: 
 
-Filename: viso/
+Filename: docs/ext/manager_tmpl.j2
 Comment: 
 
-Filename: viso_sdk_python-0.0.3.dist-info/AUTHORS
+Filename: tests/meta/__init__.py
 Comment: 
 
-Filename: viso_sdk_python-0.0.3.dist-info/RECORD
+Filename: tests/meta/test_ensure_type_hints.py
 Comment: 
 
-Filename: viso_sdk_python-0.0.3.dist-info/METADATA
+Filename: tests/smoke/__init__.py
 Comment: 
 
-Filename: viso_sdk_python-0.0.3.dist-info/dependency_links.txt
+Filename: tests/smoke/test_dists.py
 Comment: 
 
-Filename: viso_sdk_python-0.0.3.dist-info/WHEEL
+Filename: viso_sdk/__init__.py
 Comment: 
 
-Filename: viso_sdk_python-0.0.3.dist-info/top_level.txt
+Filename: viso_sdk/_version.py
 Comment: 
 
-Filename: viso_sdk_python-0.0.3.dist-info/COPYING
+Filename: viso_sdk/constants/__init__.py
 Comment: 
 
-Filename: viso/VERSION
+Filename: viso_sdk/constants/constants.py
 Comment: 
 
-Filename: viso/_version.cpython-39-x86_64-linux-gnu.so
+Filename: viso_sdk/constants/modules.py
 Comment: 
 
-Filename: viso/redis_util.cpython-39-x86_64-linux-gnu.so
+Filename: viso_sdk/constants/variables.py
 Comment: 
 
-Filename: viso/__init__.py
+Filename: viso_sdk/edge/__init__.py
 Comment: 
 
-Filename: viso/py.typed
+Filename: viso_sdk/edge/common.py
 Comment: 
 
-Filename: viso/logging.cpython-39-x86_64-linux-gnu.so
+Filename: viso_sdk/logging/__init__.py
 Comment: 
 
-Filename: viso/status.cpython-39-x86_64-linux-gnu.so
+Filename: viso_sdk/logging/logger.py
 Comment: 
 
-Filename: viso/common.cpython-39-x86_64-linux-gnu.so
+Filename: viso_sdk/logging/status_logger.py
 Comment: 
 
-Filename: viso/flow.cpython-39-x86_64-linux-gnu.so
+Filename: viso_sdk/mqtt/__init__.py
 Comment: 
 
-Filename: viso/mqtt.cpython-39-x86_64-linux-gnu.so
+Filename: viso_sdk/mqtt/mqtt_wrapper.py
 Comment: 
 
-Filename: viso/constant.cpython-39-x86_64-linux-gnu.so
+Filename: viso_sdk/nodered/__init__.py
+Comment: 
+
+Filename: viso_sdk/nodered/flow.py
+Comment: 
+
+Filename: viso_sdk/redis/__init__.py
+Comment: 
+
+Filename: viso_sdk/redis/redis_wrapper.py
+Comment: 
+
+Filename: viso_sdk/visualize/__init__.py
+Comment: 
+
+Filename: viso_sdk/visualize/custom_font.py
+Comment: 
+
+Filename: viso_sdk/visualize/palette.py
+Comment: 
+
+Filename: viso_sdk/visualize/visualization.py
+Comment: 
+
+Filename: viso_sdk_python-0.0.4.dev0.dist-info/AUTHORS
+Comment: 
+
+Filename: viso_sdk_python-0.0.4.dev0.dist-info/COPYING
+Comment: 
+
+Filename: viso_sdk_python-0.0.4.dev0.dist-info/METADATA
+Comment: 
+
+Filename: viso_sdk_python-0.0.4.dev0.dist-info/WHEEL
+Comment: 
+
+Filename: viso_sdk_python-0.0.4.dev0.dist-info/top_level.txt
+Comment: 
+
+Filename: viso_sdk_python-0.0.4.dev0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## Comparing `viso_sdk_python-0.0.3.dist-info/METADATA` & `viso_sdk_python-0.0.4.dev0.dist-info/METADATA`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: viso-sdk-python
-Version: 0.0.3
-Summary: Viso SDK for Python
+Version: 0.0.4.dev0
+Summary: VisoSDK: A SDK in Python for viso containers
 Home-page: https://gitlab.com/TopKamera/03_edge/Base/viso-sdk-python-public.git
-Author: Shane Carlyon
-Author-email: s.carlyon@viso.ai
+Author: support@viso.ai
+Author-email: support@viso.ai
 License: LGPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Natural Language :: English
@@ -23,28 +23,30 @@
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: AUTHORS
 Requires-Dist: requests (==2.27.1)
 Requires-Dist: requests-toolbelt (==0.9.1)
 Requires-Dist: paho-mqtt
 Requires-Dist: redis
-Requires-Dist: opencv-python (==4.5.1.48) ; platform_machine != "aarch64" and platform_machine != "armv6l" and platform_machine != "armv7l" and python_version != "3.10"
-Requires-Dist: opencv-python (==4.5.4.58) ; platform_machine != "aarch64" and platform_machine != "armv6l" and platform_machine != "armv7l" and python_version == "3.10"
-Requires-Dist: opencv-python (==4.4.0.46) ; platform_machine == "armv6l" or platform_machine == "armv7l"
-Provides-Extra: autocompletion
-Requires-Dist: argcomplete (<3,>=1.10.0) ; extra == 'autocompletion'
-Provides-Extra: yaml
-Requires-Dist: PyYaml (>=5.2) ; extra == 'yaml'
+Requires-Dist: opencv-python (==4.5.4.58)
+Requires-Dist: Pillow
 
 # viso-sdk-python
 
 **viso-sdk-python** is a utility for [viso.ai](https://viso.ai) containers.
 
 ## Installation
 
 Use `pip` to install the latest stable version of **viso-sdk-python**:
 
 ```shell
 pip install viso-sdk-python
 ```
 
 
+## Build
+```shell
+python3 -m pip install -e .
+python3 setup.py sdist bdist_wheel
+```
+
+
```

## Comparing `viso_sdk_python-0.0.3.dist-info/COPYING` & `viso_sdk_python-0.0.4.dev0.dist-info/COPYING`

 * *Files identical despite different names*

## Comparing `viso/__init__.py` & `viso_sdk/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2018-2022 Shane Carlyon <s.carlyon@viso.ai>
+# Copyright (C) 2020-2023 viso.ai AG <info@viso.ai>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -14,17 +14,29 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """Wrapper for the Viso SDK."""
 
 import warnings
 
-from viso._version import (  # noqa: F401
+
+from viso_sdk import (
+    constants,
+    edge,
+    logging,
+    mqtt,
+    nodered,
+    redis,
+    visualize
+)
+
+from viso_sdk._version import (  # noqa: F401
     __author__,
     __copyright__,
     __email__,
     __license__,
     __title__,
     __version__,
 )
 
-warnings.filterwarnings("default", category=DeprecationWarning, module="^viso")
+
+warnings.filterwarnings("default", category=DeprecationWarning, module="^viso_sdk")
```

