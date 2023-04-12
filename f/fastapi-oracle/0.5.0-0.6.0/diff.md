# Comparing `tmp/fastapi_oracle-0.5.0-py3-none-any.whl.zip` & `tmp/fastapi_oracle-0.6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 13016 bytes, number of entries: 11
+Zip file size: 13125 bytes, number of entries: 11
 -rw-r--r--  2.0 unx     1412 b- defN 80-Jan-01 00:00 fastapi_oracle/__init__.py
--rw-r--r--  2.0 unx      723 b- defN 80-Jan-01 00:00 fastapi_oracle/config.py
+-rw-r--r--  2.0 unx      767 b- defN 80-Jan-01 00:00 fastapi_oracle/config.py
 -rw-r--r--  2.0 unx      891 b- defN 80-Jan-01 00:00 fastapi_oracle/constants.py
--rw-r--r--  2.0 unx     7706 b- defN 80-Jan-01 00:00 fastapi_oracle/core.py
+-rw-r--r--  2.0 unx     7986 b- defN 80-Jan-01 00:00 fastapi_oracle/core.py
 -rw-r--r--  2.0 unx     2088 b- defN 80-Jan-01 00:00 fastapi_oracle/errors.py
 -rw-r--r--  2.0 unx      207 b- defN 80-Jan-01 00:00 fastapi_oracle/pools.py
 -rw-r--r--  2.0 unx     1793 b- defN 80-Jan-01 00:00 fastapi_oracle/utils.py
--rw-r--r--  2.0 unx    11357 b- defN 80-Jan-01 00:00 fastapi_oracle-0.5.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     4624 b- defN 80-Jan-01 00:00 fastapi_oracle-0.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fastapi_oracle-0.5.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx      888 b- defN 16-Jan-01 00:00 fastapi_oracle-0.5.0.dist-info/RECORD
-11 files, 31777 bytes uncompressed, 11520 bytes compressed:  63.7%
+-rw-r--r--  2.0 unx    11357 b- defN 80-Jan-01 00:00 fastapi_oracle-0.6.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4624 b- defN 80-Jan-01 00:00 fastapi_oracle-0.6.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fastapi_oracle-0.6.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx      888 b- defN 16-Jan-01 00:00 fastapi_oracle-0.6.0.dist-info/RECORD
+11 files, 32101 bytes uncompressed, 11629 bytes compressed:  63.8%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: fastapi_oracle/pools.py
 Comment: 
 
 Filename: fastapi_oracle/utils.py
 Comment: 
 
-Filename: fastapi_oracle-0.5.0.dist-info/LICENSE
+Filename: fastapi_oracle-0.6.0.dist-info/LICENSE
 Comment: 
 
-Filename: fastapi_oracle-0.5.0.dist-info/METADATA
+Filename: fastapi_oracle-0.6.0.dist-info/METADATA
 Comment: 
 
-Filename: fastapi_oracle-0.5.0.dist-info/WHEEL
+Filename: fastapi_oracle-0.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: fastapi_oracle-0.5.0.dist-info/RECORD
+Filename: fastapi_oracle-0.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fastapi_oracle/config.py

```diff
@@ -6,14 +6,15 @@
 class Settings(BaseSettings):
     db_host: str = "127.0.0.1"
     db_port: int = 1521
     db_user: str = "dbuser"
     db_password: str = "dbpassword"  # nosemgrep
     db_service_name: str = "dbservicename"
     db_conn_ttl: int | None = None
+    db_wait_timeout_secs: int | None = None
 
 
 @lru_cache()
 def get_settings() -> Settings:  # pragma: no cover
     """Get settings for fastapi-oracle.
 
     A settings object is only created once, per FastAPI recommended practice, so that
```

## fastapi_oracle/core.py

```diff
@@ -1,13 +1,13 @@
 import time
 from functools import wraps
 from re import Pattern
 from typing import AsyncGenerator, Awaitable, Callable, ParamSpec, TypeVar
 
-from cx_Oracle import DatabaseError, makedsn
+from cx_Oracle import SPOOL_ATTRVAL_TIMEDWAIT, DatabaseError, makedsn
 from cx_Oracle_async import create_pool
 from cx_Oracle_async.pools import AsyncPoolWrapper
 from fastapi import Depends
 from loguru import logger
 
 from fastapi_oracle import pools
 from fastapi_oracle.config import Settings, get_settings
@@ -83,18 +83,25 @@
             return pool
 
     dsn = makedsn(
         host=settings.db_host,
         port=settings.db_port,
         sid=settings.db_service_name,
     )
+    create_pool_kwargs = {}
+
+    if settings.db_wait_timeout_secs is not None:
+        create_pool_kwargs["getmode"] = SPOOL_ATTRVAL_TIMEDWAIT
+        create_pool_kwargs["waitTimeout"] = settings.db_wait_timeout_secs * 1000
+
     pool = await create_pool(
         user=settings.db_user,
         password=settings.db_password,
         dsn=dsn,
+        **create_pool_kwargs,
     )
     pools.DB_POOLS[pool_key] = DbPoolAndCreatedTime(
         pool=pool, created_time=time.monotonic()
     )
 
     return pools.DB_POOLS[pool_key].pool
```

## Comparing `fastapi_oracle-0.5.0.dist-info/LICENSE` & `fastapi_oracle-0.6.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fastapi_oracle-0.5.0.dist-info/METADATA` & `fastapi_oracle-0.6.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-oracle
-Version: 0.5.0
+Version: 0.6.0
 Summary: Helpers for using the cx_Oracle_async library with the FastAPI framework.
 Home-page: https://github.com/Jaza/fastapi-oracle
 License: Apache-2.0
 Author: Jeremy Epstein
 Author-email: jazepstein@gmail.com
 Requires-Python: >=3.10,<4
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `fastapi_oracle-0.5.0.dist-info/RECORD` & `fastapi_oracle-0.6.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 fastapi_oracle/__init__.py,sha256=zRvlU5zn4jQ1aoh-0hfM7ryDCDwUVkX-J7ykbNk4jBc,1412
-fastapi_oracle/config.py,sha256=BpcZF5h0UxJnF0sN34C-g88xnxxbBF_hhFDIumsfYcc,723
+fastapi_oracle/config.py,sha256=hDQbaVzjX2vOb8ujxYWDGM-n39_r5lXQeCJd__Qeo9M,767
 fastapi_oracle/constants.py,sha256=Rg-nkuQXVQQoAeE9AUdsa4RNv0nMKscVvYSa1pqpfeM,891
-fastapi_oracle/core.py,sha256=24mdF7LP9-d2I5tE2o9pTpxzPrbpsQWPLOXJDWE2E-g,7706
+fastapi_oracle/core.py,sha256=VrKeh1a2nLqMBIqEdV_FaTIZZcwjsTkGrmwK_WR1Zms,7986
 fastapi_oracle/errors.py,sha256=owpkOovw44qoHuqpVkrJuxFIJ5XuGWH2cv_wuFaEQGs,2088
 fastapi_oracle/pools.py,sha256=fVkOPrtwoQMhlI85szk6k7m6tvPUGLmGKCBHGOqyl2U,207
 fastapi_oracle/utils.py,sha256=HhOAibZLmGxEhbouXtFjjjn50NzoTLL7R6EHEyZJcVU,1793
-fastapi_oracle-0.5.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-fastapi_oracle-0.5.0.dist-info/METADATA,sha256=Q7y7eXdapufO9KOcRER3-awzrgJOt7NmqPcRlMpsMsE,4624
-fastapi_oracle-0.5.0.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-fastapi_oracle-0.5.0.dist-info/RECORD,,
+fastapi_oracle-0.6.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+fastapi_oracle-0.6.0.dist-info/METADATA,sha256=4baMYYtDJSPYhfnmXUkiwzN7qJWalKqkLG_TKxM7a9o,4624
+fastapi_oracle-0.6.0.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+fastapi_oracle-0.6.0.dist-info/RECORD,,
```

