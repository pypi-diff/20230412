# Comparing `tmp/datarobot_predict-1.0.2-py3-none-any.whl.zip` & `tmp/datarobot_predict-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 11012 bytes, number of entries: 6
+Zip file size: 11833 bytes, number of entries: 6
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 datarobot_predict/__init__.py
--rw-r--r--  2.0 unx    23664 b- defN 80-Jan-01 00:00 datarobot_predict/scoring_code.py
--rw-r--r--  2.0 unx     7556 b- defN 80-Jan-01 00:00 datarobot_predict-1.0.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     3839 b- defN 80-Jan-01 00:00 datarobot_predict-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 datarobot_predict-1.0.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx      512 b- defN 16-Jan-01 00:00 datarobot_predict-1.0.2.dist-info/RECORD
-6 files, 35659 bytes uncompressed, 10078 bytes compressed:  71.7%
+-rw-r--r--  2.0 unx    24018 b- defN 80-Jan-01 00:00 datarobot_predict/scoring_code.py
+-rw-r--r--  2.0 unx    10141 b- defN 80-Jan-01 00:00 datarobot_predict-1.0.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     4000 b- defN 80-Jan-01 00:00 datarobot_predict-1.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 datarobot_predict-1.0.3.dist-info/WHEEL
+?rw-r--r--  2.0 unx      513 b- defN 16-Jan-01 00:00 datarobot_predict-1.0.3.dist-info/RECORD
+6 files, 38760 bytes uncompressed, 10899 bytes compressed:  71.9%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: datarobot_predict/__init__.py
 Comment: 
 
 Filename: datarobot_predict/scoring_code.py
 Comment: 
 
-Filename: datarobot_predict-1.0.2.dist-info/LICENSE.txt
+Filename: datarobot_predict-1.0.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: datarobot_predict-1.0.2.dist-info/METADATA
+Filename: datarobot_predict-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: datarobot_predict-1.0.2.dist-info/WHEEL
+Filename: datarobot_predict-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: datarobot_predict-1.0.2.dist-info/RECORD
+Filename: datarobot_predict-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datarobot_predict/scoring_code.py

```diff
@@ -1,18 +1,21 @@
 #
-# Copyright 2022 DataRobot, Inc. and its affiliates.
+# Copyright 2023 DataRobot, Inc. and its affiliates.
 #
-# All rights reserved.
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-# DataRobot, Inc.
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
-# This is proprietary source code of DataRobot, Inc. and its
-# affiliates.
-#
-# Released under the terms of DataRobot Tool and Utility Agreement.
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 # pylint: disable=import-error,import-outside-toplevel
 import datetime
 import enum
 import math
 import os.path
 import re
 from collections import OrderedDict
```

## Comparing `datarobot_predict-1.0.2.dist-info/METADATA` & `datarobot_predict-1.0.3.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: datarobot-predict
-Version: 1.0.2
+Version: 1.0.3
 Summary: DataRobot Prediction Library
+License: Apache-2.0
 Author: DataRobot
 Author-email: support@datarobot.com
 Requires-Python: >=3.7,<3.12
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=7,<9)
@@ -18,14 +20,17 @@
 
 # About
 DataRobot Prediction Library is a Python library for making predictions using various prediction methods supported by DataRobot.
 The intention is to provide a common interface for making predictions, making it easy to swap out the underlying implementation.
 
 For more info, see the [DataRobot Documentation](https://docs.datarobot.com/).
 
+## License
+[Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0)
+
 # Setup
 ## Prerequisites
 * Python 3.7 or greater
 * Scoring Code requires Java Runtime Environment 8 or higher
 * Scoring Code models generated on DataRobot 7.3 and later are supported
 
 ## Installation
```

