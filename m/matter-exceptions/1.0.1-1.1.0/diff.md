# Comparing `tmp/matter_exceptions-1.0.1-py3-none-any.whl.zip` & `tmp/matter_exceptions-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 6665 bytes, number of entries: 12
+Zip file size: 6666 bytes, number of entries: 12
 -rw-r--r--  2.0 unx      134 b- defN 20-Feb-02 00:00 matter_exceptions/__about__.py
 -rw-r--r--  2.0 unx      152 b- defN 20-Feb-02 00:00 matter_exceptions/__init__.py
 -rw-r--r--  2.0 unx      850 b- defN 20-Feb-02 00:00 matter_exceptions/base_api_exception.py
 -rw-r--r--  2.0 unx      864 b- defN 20-Feb-02 00:00 matter_exceptions/base_fastapi_exception.py
 -rw-r--r--  2.0 unx      890 b- defN 20-Feb-02 00:00 matter_exceptions/detailed_exception.py
 -rw-r--r--  2.0 unx      520 b- defN 20-Feb-02 00:00 matter_exceptions/exceptions/api.py
 -rw-r--r--  2.0 unx      556 b- defN 20-Feb-02 00:00 matter_exceptions/exceptions/fastapi.py
 -rw-r--r--  2.0 unx      163 b- defN 20-Feb-02 00:00 matter_exceptions/exceptions/general.py
-?rw-r--r--  2.0 unx     4313 b- defN 20-Feb-02 00:00 matter_exceptions-1.0.1.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 matter_exceptions-1.0.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1104 b- defN 20-Feb-02 00:00 matter_exceptions-1.0.1.dist-info/licenses/LICENSE.txt
-?rw-r--r--  2.0 unx     1088 b- defN 20-Feb-02 00:00 matter_exceptions-1.0.1.dist-info/RECORD
-12 files, 10721 bytes uncompressed, 4795 bytes compressed:  55.3%
+?rw-r--r--  2.0 unx     4313 b- defN 20-Feb-02 00:00 matter_exceptions-1.1.0.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 matter_exceptions-1.1.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1104 b- defN 20-Feb-02 00:00 matter_exceptions-1.1.0.dist-info/licenses/LICENSE.txt
+?rw-r--r--  2.0 unx     1088 b- defN 20-Feb-02 00:00 matter_exceptions-1.1.0.dist-info/RECORD
+12 files, 10721 bytes uncompressed, 4796 bytes compressed:  55.3%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: matter_exceptions/exceptions/fastapi.py
 Comment: 
 
 Filename: matter_exceptions/exceptions/general.py
 Comment: 
 
-Filename: matter_exceptions-1.0.1.dist-info/METADATA
+Filename: matter_exceptions-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: matter_exceptions-1.0.1.dist-info/WHEEL
+Filename: matter_exceptions-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: matter_exceptions-1.0.1.dist-info/licenses/LICENSE.txt
+Filename: matter_exceptions-1.1.0.dist-info/licenses/LICENSE.txt
 Comment: 
 
-Filename: matter_exceptions-1.0.1.dist-info/RECORD
+Filename: matter_exceptions-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## matter_exceptions/__about__.py

```diff
@@ -1,4 +1,4 @@
 # SPDX-FileCopyrightText: 2023-present Rômulo Jales <romulo@thisismatter.com>
 #
 # SPDX-License-Identifier: MIT
-__version__ = "1.0.1"
+__version__ = "1.1.0"
```

## Comparing `matter_exceptions-1.0.1.dist-info/METADATA` & `matter_exceptions-1.1.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: matter-exceptions
-Version: 1.0.1
+Version: 1.1.0
 Project-URL: Documentation, https://github.com/Matter/matter-exceptions#readme
 Project-URL: Issues, https://github.com/Matter/matter-exceptions/issues
 Project-URL: Source, https://github.com/Matter/matter-exceptions
 Author-email: Rômulo Jales <romulo@thisismatter.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Provides-Extra: fastapi
-Requires-Dist: fastapi<=0.94.1,>=0.88.0; extra == 'fastapi'
+Requires-Dist: fastapi<=0.95.0,>=0.88.0; extra == 'fastapi'
 Description-Content-Type: text/markdown
 
 # matter-exceptions
 
 **Table of Contents**
 
 - [Installation](#installation)
```

## Comparing `matter_exceptions-1.0.1.dist-info/licenses/LICENSE.txt` & `matter_exceptions-1.1.0.dist-info/licenses/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `matter_exceptions-1.0.1.dist-info/RECORD` & `matter_exceptions-1.1.0.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-matter_exceptions/__about__.py,sha256=nvdF5_ifouXNU7C5_TVYAl3_bbZD_njzk7lhv6XSKFE,134
+matter_exceptions/__about__.py,sha256=bY_nM7erfu6ZowAj4rj9sUxHb6UwLAepqSYI0RRu0ck,134
 matter_exceptions/__init__.py,sha256=rECityBo2G83dKwnB-nRrmUoggNxNoCmOoj8gfggTUw,152
 matter_exceptions/base_api_exception.py,sha256=Z0YiFlVgPKnAADxgGQhQ55gH-GkhVpr-6mxzxJw4WBs,850
 matter_exceptions/base_fastapi_exception.py,sha256=1qkoXgufYNrX1i0ohmxFHjjVc8tEpQh1P-JfWLEUpkQ,864
 matter_exceptions/detailed_exception.py,sha256=PWrNYp7mDsXSyk-o2ac7_DQzghH-SP3aXw7AP8VeVvM,890
 matter_exceptions/exceptions/api.py,sha256=rSbtijiMJtBMKBMWfa3E-kchM0R5fUScFvxtBkfGcdA,520
 matter_exceptions/exceptions/fastapi.py,sha256=unLPcgD7DOv5uPgZX4WN3MK8rFaXIj3R14HTIVRUwso,556
 matter_exceptions/exceptions/general.py,sha256=F6kZhoctNzZo-4wbAb3SIUoLzlEAEPOxIJY7sH_xtLs,163
-matter_exceptions-1.0.1.dist-info/METADATA,sha256=RFIvLtj2-ho9xvmcX_EIO--1uQWQ84HRTqAJ7R4xYdU,4313
-matter_exceptions-1.0.1.dist-info/WHEEL,sha256=Fd6mP6ydyRguakwUJ05oBE7fh2IPxgtDN9IwHJ9OqJQ,87
-matter_exceptions-1.0.1.dist-info/licenses/LICENSE.txt,sha256=n41DRZaDViDKDB5AGAyKl4AJRRtsxMGDFCcABsdEioU,1104
-matter_exceptions-1.0.1.dist-info/RECORD,,
+matter_exceptions-1.1.0.dist-info/METADATA,sha256=Nh6GP2UPD8DjCeSHg-hg5wIPJoLnUfDch67TeKCaxOY,4313
+matter_exceptions-1.1.0.dist-info/WHEEL,sha256=EI2JsGydwUL5GP9t6kzZv7G3HDPi7FuZDDf9In6amRM,87
+matter_exceptions-1.1.0.dist-info/licenses/LICENSE.txt,sha256=n41DRZaDViDKDB5AGAyKl4AJRRtsxMGDFCcABsdEioU,1104
+matter_exceptions-1.1.0.dist-info/RECORD,,
```

