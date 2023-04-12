# Comparing `tmp/matter_task_queue-1.1.2-py3-none-any.whl.zip` & `tmp/matter_task_queue-1.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8741 bytes, number of entries: 10
+Zip file size: 8740 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      134 b- defN 20-Feb-02 00:00 matter_task_queue/__about__.py
 -rw-r--r--  2.0 unx      353 b- defN 20-Feb-02 00:00 matter_task_queue/__init__.py
 -rw-r--r--  2.0 unx     1228 b- defN 20-Feb-02 00:00 matter_task_queue/base_task.py
 -rw-r--r--  2.0 unx     3862 b- defN 20-Feb-02 00:00 matter_task_queue/celery_config.py
 -rw-r--r--  2.0 unx      901 b- defN 20-Feb-02 00:00 matter_task_queue/config.py
 -rw-r--r--  2.0 unx     3232 b- defN 20-Feb-02 00:00 matter_task_queue/utils.py
-?rw-r--r--  2.0 unx     4757 b- defN 20-Feb-02 00:00 matter_task_queue-1.1.2.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 matter_task_queue-1.1.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1068 b- defN 20-Feb-02 00:00 matter_task_queue-1.1.2.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      858 b- defN 20-Feb-02 00:00 matter_task_queue-1.1.2.dist-info/RECORD
-10 files, 16480 bytes uncompressed, 7265 bytes compressed:  55.9%
+?rw-r--r--  2.0 unx     4757 b- defN 20-Feb-02 00:00 matter_task_queue-1.1.3.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 matter_task_queue-1.1.3.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1068 b- defN 20-Feb-02 00:00 matter_task_queue-1.1.3.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      858 b- defN 20-Feb-02 00:00 matter_task_queue-1.1.3.dist-info/RECORD
+10 files, 16480 bytes uncompressed, 7264 bytes compressed:  55.9%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: matter_task_queue/config.py
 Comment: 
 
 Filename: matter_task_queue/utils.py
 Comment: 
 
-Filename: matter_task_queue-1.1.2.dist-info/METADATA
+Filename: matter_task_queue-1.1.3.dist-info/METADATA
 Comment: 
 
-Filename: matter_task_queue-1.1.2.dist-info/WHEEL
+Filename: matter_task_queue-1.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: matter_task_queue-1.1.2.dist-info/licenses/LICENSE
+Filename: matter_task_queue-1.1.3.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: matter_task_queue-1.1.2.dist-info/RECORD
+Filename: matter_task_queue-1.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## matter_task_queue/__about__.py

```diff
@@ -1,4 +1,4 @@
 # SPDX-FileCopyrightText: 2023-present Rômulo Jales <romulo@thisismatter.com>
 #
 # SPDX-License-Identifier: MIT
-__version__ = "1.1.2"
+__version__ = "1.1.3"
```

## Comparing `matter_task_queue-1.1.2.dist-info/METADATA` & `matter_task_queue-1.1.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matter-task-queue
-Version: 1.1.2
+Version: 1.1.3
 Summary: A template for new Matter's library
 Project-URL: Documentation, https://github.com/Matter-Tech/matter-task-queue#readme
 Project-URL: Issues, https://github.com/Matter-Tech/matter-task-queue/issues
 Project-URL: Source, https://github.com/Matter-Tech/matter-task-queue
 Author-email: Tomer Sasson <tomer@thisismatter.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -13,17 +13,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: celery[sqs]==5.2.7
 Requires-Dist: kombu==5.2.4
-Requires-Dist: matter-exceptions==1.0.1
+Requires-Dist: matter-exceptions==1.1.0
 Provides-Extra: sentry
-Requires-Dist: sentry-sdk==1.18.0; extra == 'sentry'
+Requires-Dist: sentry-sdk==1.19.1; extra == 'sentry'
 Description-Content-Type: text/markdown
 
 # matter-task-queue
 
 The Task Queue Library is a Python library that provides functionality for managing queues and integrates Celery into FastAPI apps. It enables a seamless integration that unlocks all of Celery's capabilities and allows for easy queue management and task execution.
 
 Celery is an open-source, distributed task queue that is widely used in Python-based applications for processing and executing background tasks or long-running processes asynchronously. It was created in 2009 and has since grown into a mature and powerful library that provides a robust and scalable solution for managing task queues.
```

## Comparing `matter_task_queue-1.1.2.dist-info/licenses/LICENSE` & `matter_task_queue-1.1.3.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `matter_task_queue-1.1.2.dist-info/RECORD` & `matter_task_queue-1.1.3.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-matter_task_queue/__about__.py,sha256=Rv-A6ZB56Ed1hstuopjg4OLAD-HSY-31bNag8HF3c3I,134
+matter_task_queue/__about__.py,sha256=5jZ_bunLB35tAJtOWPCPdLieY39QQan3HeQVIaOJFNk,134
 matter_task_queue/__init__.py,sha256=VZQFnoZIVpJBsw_NI3KOJxuShkSuzedEMIm3x0ZSE4M,353
 matter_task_queue/base_task.py,sha256=6J-CkaNo3PoERYwfcq2N6WKvUkm7eE1ZtGqqv9ms7nk,1228
 matter_task_queue/celery_config.py,sha256=651NRkHE1CeVETvAG4TCmJFKygj_gLveCxUrAyZMVOQ,3862
 matter_task_queue/config.py,sha256=1SZH75s5HGu7CcQKqGVxLuVwRR8L61MSIycMpy9daBM,901
 matter_task_queue/utils.py,sha256=V5vlCW39lRJvorJka7kAAt2IRSebgmAGVXydOYHwdQ0,3232
-matter_task_queue-1.1.2.dist-info/METADATA,sha256=2hIS58H53MNvbS7bQwuzxGZl3pv6I9tS9xafKhFpxLc,4757
-matter_task_queue-1.1.2.dist-info/WHEEL,sha256=EI2JsGydwUL5GP9t6kzZv7G3HDPi7FuZDDf9In6amRM,87
-matter_task_queue-1.1.2.dist-info/licenses/LICENSE,sha256=bqRY4B_u4xSKzKFb3ML8l0nCWvMXyzEGwY2B2hteV8g,1068
-matter_task_queue-1.1.2.dist-info/RECORD,,
+matter_task_queue-1.1.3.dist-info/METADATA,sha256=uLCJbIuioKS2W_MSpn4GU9U1g-nlAkl_cUtg8-N023Q,4757
+matter_task_queue-1.1.3.dist-info/WHEEL,sha256=EI2JsGydwUL5GP9t6kzZv7G3HDPi7FuZDDf9In6amRM,87
+matter_task_queue-1.1.3.dist-info/licenses/LICENSE,sha256=bqRY4B_u4xSKzKFb3ML8l0nCWvMXyzEGwY2B2hteV8g,1068
+matter_task_queue-1.1.3.dist-info/RECORD,,
```

