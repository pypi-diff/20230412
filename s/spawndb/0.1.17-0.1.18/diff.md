# Comparing `tmp/spawndb-0.1.17.tar.gz` & `tmp/spawndb-0.1.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spawndb-0.1.17.tar", max compression
+gzip compressed data, was "spawndb-0.1.18.tar", max compression
```

## Comparing `spawndb-0.1.17.tar` & `spawndb-0.1.18.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      900 2023-02-15 10:02:18.865698 spawndb-0.1.17/README.md
--rw-r--r--   0        0        0      488 2023-02-15 12:37:41.876708 spawndb-0.1.17/pyproject.toml
--rw-r--r--   0        0        0      108 2023-02-15 10:02:18.870064 spawndb-0.1.17/src/spawndb/__init__.py
--rw-r--r--   0        0        0     2347 2023-02-15 10:02:18.870211 spawndb-0.1.17/src/spawndb/aio.py
--rw-r--r--   0        0        0     2047 2023-02-15 10:02:18.870355 spawndb-0.1.17/src/spawndb/spawndb.py
--rw-r--r--   0        0        0     1595 1970-01-01 00:00:00.000000 spawndb-0.1.17/setup.py
--rw-r--r--   0        0        0     1339 1970-01-01 00:00:00.000000 spawndb-0.1.17/PKG-INFO
+-rw-r--r--   0        0        0      910 2023-04-12 13:09:43.001204 spawndb-0.1.18/README.md
+-rw-r--r--   0        0        0      537 2023-04-12 13:15:24.574894 spawndb-0.1.18/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-02-15 10:02:18.870064 spawndb-0.1.18/src/spawndb/__init__.py
+-rw-r--r--   0        0        0     3583 2023-04-12 13:07:24.236766 spawndb-0.1.18/src/spawndb/aio.py
+-rw-r--r--   0        0        0     2047 2023-02-15 10:02:18.870355 spawndb-0.1.18/src/spawndb/spawndb.py
+-rw-r--r--   0        0        0     1633 1970-01-01 00:00:00.000000 spawndb-0.1.18/setup.py
+-rw-r--r--   0        0        0     1451 1970-01-01 00:00:00.000000 spawndb-0.1.18/PKG-INFO
```

### Comparing `spawndb-0.1.17/README.md` & `spawndb-0.1.18/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-# TestDB
+# SpawnDB
 
 This is a simple library that helps in the creation of test databases for Python
 projects that use SQLAlchemy.
 
 It's aim it's to seamlessly handle creation of a separate test database, including
-the creation of all schema objects and finally, handling the destruction of the test
+the creation of all schemas, their objects and finally, handling the destruction of the test
 database when it's no longer needed.
 
 # Usage
 To create a test database, use the init_test_db function.
 
 This function expects two arguments:  
    - *database_url*: sqlalchemy.engine.URL  
    - *metadata*: sqlalchemy.schema.MetaData
 
 It will return an instantiated Engine for the test database which you can use for 
 your database logics.
 
 ```python
 # Sample usage for Pytest
-from testdb import init_test_db, destroy_test_db
+from spawndb import init_test_db, destroy_test_db
 
 def my_cool_test():
     db_engine = init_test_db(database_url, sqla_metadata)
     
     try:
         # your stuff goes here
```

### Comparing `spawndb-0.1.17/src/spawndb/aio.py` & `spawndb-0.1.18/src/spawndb/aio.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import *
+from typing import Union
 
-
+import sqlalchemy.exc
 from sqlalchemy.engine.url import URL
-from sqlalchemy import text, MetaData
-from sqlalchemy.ext.asyncio import create_async_engine, AsyncEngine
-
+from sqlalchemy import text, MetaData, inspect
+from sqlalchemy.schema import CreateSchema
+from sqlalchemy.ext.asyncio import create_async_engine, AsyncEngine, AsyncConnection
 
 _engine: Optional[AsyncEngine] = None
 _is_started = False
 
 
 async def create_db(engine_to_use, name: str):
     async with engine_to_use.connect() as conn:
@@ -26,20 +27,45 @@
     """
     Returns a modified URL where the database name is suffixed with _test
     :return:
     """
     return url_to_modify.set(database=url_to_modify.database + "_test")
 
 
-async def init_async_test_db(db_url: URL, metadata: MetaData, drop_existing=False) -> AsyncEngine:
+async def schema_exists(conn: AsyncConnection, schema_name: str) -> bool:
+    """
+    Evaluates if a schema is present in the given database.
+
+    Args:
+        conn: AsyncConnection to work with.
+        schema_name: Schema name to test
+
+    Returns:
+        bool
+    """
+    def inner(sync_conn):
+        inspector = inspect(sync_conn)
+        return inspector.dialect.has_schema(sync_conn, schema_name)
+
+    return await conn.run_sync(inner)
+
+
+async def init_async_test_db(db_url: URL, metadata: Union[list[MetaData], MetaData], drop_existing=False) -> AsyncEngine:
     """
     Connects to the configured database temporarily, issues CREATE commands to instantiate a test database,
-    disposes the engine and replaces the global engine with the test one.
+    creates schemas if needed, disposes the engine and replaces the global engine with the test one.
 
-    :return: Reference to the instantiated test engine.
+    Args:
+        db_url: Database URL
+        metadata: Either a single MetaData object or a list of MetaData instances. If a list
+            is passed, create commands will be issued for all objects in all MetaData instances.
+        drop_existing: If set to True, it will DROP the database first.
+
+    Returns:
+        Reference to the instantiated test engine.
     """
     global _engine
     global _is_started
 
     temp_engine = create_async_engine(db_url)
     test_db_url = create_test_database_url(db_url)
 
@@ -49,15 +75,23 @@
             await drop_db(temp_engine, test_db_url.database)
 
         await create_db(temp_engine, test_db_url.database)
 
         _engine = create_async_engine(test_db_url)
 
         async with _engine.begin() as conn:
-            await conn.run_sync(metadata.create_all)
+            if isinstance(metadata, MetaData):
+                metadata = [metadata]
+            for metadata_ in metadata:
+                if not await schema_exists(conn, metadata_.schema):
+                    await conn.execute(
+                        CreateSchema(metadata_.schema)
+                    )
+
+                await conn.run_sync(metadata_.create_all)
 
         _is_started = True
 
     return _engine
 
 
 async def destroy_async_test_db(db_url):
```

### Comparing `spawndb-0.1.17/src/spawndb/spawndb.py` & `spawndb-0.1.18/src/spawndb/spawndb.py`

 * *Files identical despite different names*

### Comparing `spawndb-0.1.17/setup.py` & `spawndb-0.1.18/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 {'': ['*']}
 
 install_requires = \
 ['SQLAlchemy[asyncio]>1.4.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'spawndb',
-    'version': '0.1.17',
+    'version': '0.1.18',
     'description': '',
-    'long_description': "# TestDB\n\nThis is a simple library that helps in the creation of test databases for Python\nprojects that use SQLAlchemy.\n\nIt's aim it's to seamlessly handle creation of a separate test database, including\nthe creation of all schema objects and finally, handling the destruction of the test\ndatabase when it's no longer needed.\n\n# Usage\nTo create a test database, use the init_test_db function.\n\nThis function expects two arguments:  \n   - *database_url*: sqlalchemy.engine.URL  \n   - *metadata*: sqlalchemy.schema.MetaData\n\nIt will return an instantiated Engine for the test database which you can use for \nyour database logics.\n\n```python\n# Sample usage for Pytest\nfrom testdb import init_test_db, destroy_test_db\n\ndef my_cool_test():\n    db_engine = init_test_db(database_url, sqla_metadata)\n    \n    try:\n        # your stuff goes here\n    \n    finally:\n        destroy_test_db(database_url)\n```\n\n",
+    'long_description': "# SpawnDB\n\nThis is a simple library that helps in the creation of test databases for Python\nprojects that use SQLAlchemy.\n\nIt's aim it's to seamlessly handle creation of a separate test database, including\nthe creation of all schemas, their objects and finally, handling the destruction of the test\ndatabase when it's no longer needed.\n\n# Usage\nTo create a test database, use the init_test_db function.\n\nThis function expects two arguments:  \n   - *database_url*: sqlalchemy.engine.URL  \n   - *metadata*: sqlalchemy.schema.MetaData\n\nIt will return an instantiated Engine for the test database which you can use for \nyour database logics.\n\n```python\n# Sample usage for Pytest\nfrom spawndb import init_test_db, destroy_test_db\n\ndef my_cool_test():\n    db_engine = init_test_db(database_url, sqla_metadata)\n    \n    try:\n        # your stuff goes here\n    \n    finally:\n        destroy_test_db(database_url)\n```\n\n",
     'author': 'Pablo Prieto',
     'author_email': 'pabloprieto@live.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://github.com/ppmdo/spawndb',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.9,<4.0',
 }
```

### Comparing `spawndb-0.1.17/PKG-INFO` & `spawndb-0.1.18/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 Metadata-Version: 2.1
 Name: spawndb
-Version: 0.1.17
+Version: 0.1.18
 Summary: 
+Home-page: https://github.com/ppmdo/spawndb
 Author: Pablo Prieto
 Author-email: pabloprieto@live.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: SQLAlchemy[asyncio] (>1.4.0,<3.0.0)
+Project-URL: Repository, https://github.com/ppmdo/spawndb
 Description-Content-Type: text/markdown
 
-# TestDB
+# SpawnDB
 
 This is a simple library that helps in the creation of test databases for Python
 projects that use SQLAlchemy.
 
 It's aim it's to seamlessly handle creation of a separate test database, including
-the creation of all schema objects and finally, handling the destruction of the test
+the creation of all schemas, their objects and finally, handling the destruction of the test
 database when it's no longer needed.
 
 # Usage
 To create a test database, use the init_test_db function.
 
 This function expects two arguments:  
    - *database_url*: sqlalchemy.engine.URL  
    - *metadata*: sqlalchemy.schema.MetaData
 
 It will return an instantiated Engine for the test database which you can use for 
 your database logics.
 
 ```python
 # Sample usage for Pytest
-from testdb import init_test_db, destroy_test_db
+from spawndb import init_test_db, destroy_test_db
 
 def my_cool_test():
     db_engine = init_test_db(database_url, sqla_metadata)
     
     try:
         # your stuff goes here
```

