# Comparing `tmp/fastapi_oracle-0.6.0-py3-none-any.whl.zip` & `tmp/fastapi_oracle-0.6.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 13125 bytes, number of entries: 11
+Zip file size: 13242 bytes, number of entries: 11
 -rw-r--r--  2.0 unx     1412 b- defN 80-Jan-01 00:00 fastapi_oracle/__init__.py
 -rw-r--r--  2.0 unx      767 b- defN 80-Jan-01 00:00 fastapi_oracle/config.py
 -rw-r--r--  2.0 unx      891 b- defN 80-Jan-01 00:00 fastapi_oracle/constants.py
--rw-r--r--  2.0 unx     7986 b- defN 80-Jan-01 00:00 fastapi_oracle/core.py
+-rw-r--r--  2.0 unx     8671 b- defN 80-Jan-01 00:00 fastapi_oracle/core.py
 -rw-r--r--  2.0 unx     2088 b- defN 80-Jan-01 00:00 fastapi_oracle/errors.py
 -rw-r--r--  2.0 unx      207 b- defN 80-Jan-01 00:00 fastapi_oracle/pools.py
 -rw-r--r--  2.0 unx     1793 b- defN 80-Jan-01 00:00 fastapi_oracle/utils.py
--rw-r--r--  2.0 unx    11357 b- defN 80-Jan-01 00:00 fastapi_oracle-0.6.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     4624 b- defN 80-Jan-01 00:00 fastapi_oracle-0.6.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fastapi_oracle-0.6.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx      888 b- defN 16-Jan-01 00:00 fastapi_oracle-0.6.0.dist-info/RECORD
-11 files, 32101 bytes uncompressed, 11629 bytes compressed:  63.8%
+-rw-r--r--  2.0 unx    11357 b- defN 80-Jan-01 00:00 fastapi_oracle-0.6.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4624 b- defN 80-Jan-01 00:00 fastapi_oracle-0.6.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fastapi_oracle-0.6.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx      888 b- defN 16-Jan-01 00:00 fastapi_oracle-0.6.1.dist-info/RECORD
+11 files, 32786 bytes uncompressed, 11746 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: fastapi_oracle/pools.py
 Comment: 
 
 Filename: fastapi_oracle/utils.py
 Comment: 
 
-Filename: fastapi_oracle-0.6.0.dist-info/LICENSE
+Filename: fastapi_oracle-0.6.1.dist-info/LICENSE
 Comment: 
 
-Filename: fastapi_oracle-0.6.0.dist-info/METADATA
+Filename: fastapi_oracle-0.6.1.dist-info/METADATA
 Comment: 
 
-Filename: fastapi_oracle-0.6.0.dist-info/WHEEL
+Filename: fastapi_oracle-0.6.1.dist-info/WHEEL
 Comment: 
 
-Filename: fastapi_oracle-0.6.0.dist-info/RECORD
+Filename: fastapi_oracle-0.6.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fastapi_oracle/core.py

```diff
@@ -134,14 +134,26 @@
             logger.warning(
                 '"not connected" was raised, either when acquiring or when releasing '
                 "the database connection pool - this can happen on release when the "
                 "pool has already been closed - assuming that that's what happened in "
                 "this case, therefore suppressing this error, so that consuming code "
                 "can continue gracefully"
             )
+        elif "timed out waiting for pool to create new connections" in f"{ex}":
+            logger.warning(
+                '"timed out waiting for pool to create new connections" was raised, '
+                "when attempting to acquire a connection, assuming that this is "
+                "because there is too high a load for the pool to be able to handle at "
+                "this time, therefore raising an intermittent database error, the call "
+                "will have to be retried later"
+            )
+            raise IntermittentDatabaseError(
+                "An intermittent database error occurred, please try this call again "
+                "soon"
+            )
         else:
             raise ex
 
 
 async def get_db_cursor(
     pool_and_conn: DbPoolAndConn = Depends(get_db_conn),
 ) -> AsyncGenerator[DbPoolConnAndCursor, None]:  # pragma: no cover
```

## Comparing `fastapi_oracle-0.6.0.dist-info/LICENSE` & `fastapi_oracle-0.6.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fastapi_oracle-0.6.0.dist-info/METADATA` & `fastapi_oracle-0.6.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-oracle
-Version: 0.6.0
+Version: 0.6.1
 Summary: Helpers for using the cx_Oracle_async library with the FastAPI framework.
 Home-page: https://github.com/Jaza/fastapi-oracle
 License: Apache-2.0
 Author: Jeremy Epstein
 Author-email: jazepstein@gmail.com
 Requires-Python: >=3.10,<4
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `fastapi_oracle-0.6.0.dist-info/RECORD` & `fastapi_oracle-0.6.1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 fastapi_oracle/__init__.py,sha256=zRvlU5zn4jQ1aoh-0hfM7ryDCDwUVkX-J7ykbNk4jBc,1412
 fastapi_oracle/config.py,sha256=hDQbaVzjX2vOb8ujxYWDGM-n39_r5lXQeCJd__Qeo9M,767
 fastapi_oracle/constants.py,sha256=Rg-nkuQXVQQoAeE9AUdsa4RNv0nMKscVvYSa1pqpfeM,891
-fastapi_oracle/core.py,sha256=VrKeh1a2nLqMBIqEdV_FaTIZZcwjsTkGrmwK_WR1Zms,7986
+fastapi_oracle/core.py,sha256=9LyLb-jhc11JBrId0pxigbHLzNGWAzoe0XHevWoxFqI,8671
 fastapi_oracle/errors.py,sha256=owpkOovw44qoHuqpVkrJuxFIJ5XuGWH2cv_wuFaEQGs,2088
 fastapi_oracle/pools.py,sha256=fVkOPrtwoQMhlI85szk6k7m6tvPUGLmGKCBHGOqyl2U,207
 fastapi_oracle/utils.py,sha256=HhOAibZLmGxEhbouXtFjjjn50NzoTLL7R6EHEyZJcVU,1793
-fastapi_oracle-0.6.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-fastapi_oracle-0.6.0.dist-info/METADATA,sha256=4baMYYtDJSPYhfnmXUkiwzN7qJWalKqkLG_TKxM7a9o,4624
-fastapi_oracle-0.6.0.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-fastapi_oracle-0.6.0.dist-info/RECORD,,
+fastapi_oracle-0.6.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+fastapi_oracle-0.6.1.dist-info/METADATA,sha256=zk_opuPhHw7oxSfCVu30lBjK37afPHU94dPFmn9l8dU,4624
+fastapi_oracle-0.6.1.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+fastapi_oracle-0.6.1.dist-info/RECORD,,
```

