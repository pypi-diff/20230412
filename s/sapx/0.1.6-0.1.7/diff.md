# Comparing `tmp/sapx-0.1.6.tar.gz` & `tmp/sapx-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sapx-0.1.6.tar", last modified: Mon Mar 27 14:25:38 2023, max compression
+gzip compressed data, was "sapx-0.1.7.tar", last modified: Wed Apr 12 07:48:55 2023, max compression
```

## Comparing `sapx-0.1.6.tar` & `sapx-0.1.7.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:25:38.814922 sapx-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-03-27 14:25:38.814922 sapx-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-27 14:25:17.000000 sapx-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-03-27 14:25:17.000000 sapx-0.1.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:25:38.810922 sapx-0.1.6/sap/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-27 14:25:17.000000 sapx-0.1.6/sap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:25:38.810922 sapx-0.1.6/sap/beanie/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-03-27 14:25:17.000000 sapx-0.1.6/sap/beanie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-03-27 14:25:17.000000 sapx-0.1.6/sap/beanie/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-03-27 14:25:17.000000 sapx-0.1.6/sap/beanie/document.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-03-27 14:25:17.000000 sapx-0.1.6/sap/beanie/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-03-27 14:25:17.000000 sapx-0.1.6/sap/beanie/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-03-27 14:25:17.000000 sapx-0.1.6/sap/beanie/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:25:38.810922 sapx-0.1.6/sap/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-03-27 14:25:17.000000 sapx-0.1.6/sap/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-03-27 14:25:17.000000 sapx-0.1.6/sap/fastapi/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-03-27 14:25:17.000000 sapx-0.1.6/sap/fastapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-03-27 14:25:17.000000 sapx-0.1.6/sap/fastapi/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-03-27 14:25:17.000000 sapx-0.1.6/sap/fastapi/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-03-27 14:25:17.000000 sapx-0.1.6/sap/fastapi/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-27 14:25:17.000000 sapx-0.1.6/sap/loggers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 14:25:17.000000 sapx-0.1.6/sap/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:25:38.810922 sapx-0.1.6/sap/rest/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-27 14:25:17.000000 sapx-0.1.6/sap/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-03-27 14:25:17.000000 sapx-0.1.6/sap/rest/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-03-27 14:25:17.000000 sapx-0.1.6/sap/rest/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-03-27 14:25:17.000000 sapx-0.1.6/sap/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:25:38.814922 sapx-0.1.6/sap/worker/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-03-27 14:25:17.000000 sapx-0.1.6/sap/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-03-27 14:25:17.000000 sapx-0.1.6/sap/worker/amqp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-03-27 14:25:17.000000 sapx-0.1.6/sap/worker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-03-27 14:25:17.000000 sapx-0.1.6/sap/worker/crons.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-27 14:25:17.000000 sapx-0.1.6/sap/worker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-03-27 14:25:17.000000 sapx-0.1.6/sap/worker/lambdas.py
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-03-27 14:25:17.000000 sapx-0.1.6/sap/worker/packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-03-27 14:25:17.000000 sapx-0.1.6/sap/worker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:25:38.814922 sapx-0.1.6/sapx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-03-27 14:25:38.000000 sapx-0.1.6/sapx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-03-27 14:25:38.000000 sapx-0.1.6/sapx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 14:25:38.000000 sapx-0.1.6/sapx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-27 14:25:38.000000 sapx-0.1.6/sapx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-27 14:25:38.000000 sapx-0.1.6/sapx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 14:25:38.814922 sapx-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-03-27 14:25:17.000000 sapx-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:25:38.814922 sapx-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-03-27 14:25:17.000000 sapx-0.1.6/tests/test_fastapi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-03-27 14:25:17.000000 sapx-0.1.6/tests/test_rest_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-03-27 14:25:17.000000 sapx-0.1.6/tests/test_worker_lambdas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-03-27 14:25:17.000000 sapx-0.1.6/tests/test_worker_packet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:48:55.029750 sapx-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-12 07:48:55.029750 sapx-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-12 07:48:45.000000 sapx-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-04-12 07:48:45.000000 sapx-0.1.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:48:55.017749 sapx-0.1.7/sap/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:48:55.021750 sapx-0.1.7/sap/beanie/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/beanie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/beanie/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/beanie/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/beanie/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/beanie/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/beanie/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:48:55.021750 sapx-0.1.7/sap/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/fastapi/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/fastapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/fastapi/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/fastapi/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9285 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/fastapi/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/fastapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:48:55.021750 sapx-0.1.7/sap/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/rest/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/rest/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:48:55.025750 sapx-0.1.7/sap/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/worker/amqp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/worker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/worker/crons.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/worker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/worker/lambdas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/worker/packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-04-12 07:48:45.000000 sapx-0.1.7/sap/worker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:48:55.025750 sapx-0.1.7/sapx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-12 07:48:55.000000 sapx-0.1.7/sapx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-12 07:48:55.000000 sapx-0.1.7/sapx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 07:48:55.000000 sapx-0.1.7/sapx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 07:48:55.000000 sapx-0.1.7/sapx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 07:48:55.000000 sapx-0.1.7/sapx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 07:48:55.029750 sapx-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-12 07:48:45.000000 sapx-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:48:55.029750 sapx-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-04-12 07:48:45.000000 sapx-0.1.7/tests/test_fastapi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-12 07:48:45.000000 sapx-0.1.7/tests/test_rest_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-12 07:48:45.000000 sapx-0.1.7/tests/test_worker_lambdas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-04-12 07:48:45.000000 sapx-0.1.7/tests/test_worker_packet.py
```

### Comparing `sapx-0.1.6/PKG-INFO` & `sapx-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapx
-Version: 0.1.6
+Version: 0.1.7
 Summary: Library of re-usable utilities for python web apps.
 Home-page: https://github.com/trellixio/sap
 Author: Trellix Dev
 Author-email: contact@trellix.io
 License: COPYRIGHT @ Trellix
 Classifier: Environment :: Web Environment
 Classifier: Framework :: FastAPI
```

### Comparing `sapx-0.1.6/pyproject.toml` & `sapx-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sapx-0.1.6/sap/beanie/client.py` & `sapx-0.1.7/sap/beanie/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+Beanie Client.
+
+Initialize connection to the Mongo Database.
+"""
 import typing
 
 from motor.motor_asyncio import AsyncIOMotorClient
 
 import beanie
 
 from sap.settings import DatabaseParams
@@ -9,26 +14,31 @@
 
 class BeanieClient:
     """Set up a connection to the MongoDB server."""
 
     connections: typing.ClassVar[dict[str, AsyncIOMotorClient]] = {}
 
     @classmethod
+    async def get_db_default(cls) -> AsyncIOMotorClient:
+        """Return the default db connection."""
+        return cls.connections["default"]
+
+    @classmethod
     async def init(
         cls,
         mongo_params: DatabaseParams,
         document_models: list[typing.Union[typing.Type[beanie.Document], typing.Type[beanie.View], str]],
     ) -> None:
         """Open and maintain a connection to the database.
 
         :force bool: Use it for force a connection initialization
         """
         # TODO: Check if connection exist, return existing connection
-        if "connection" in cls.connections:
-            # connection = cls.connections["connection"]
+        if "default" in cls.connections:
+            # connection = cls.connections["default"]
             return
 
         client = AsyncIOMotorClient(mongo_params.get_dns())
         connection = client[mongo_params.db]
         cls.connections["default"] = connection
         await beanie.init_beanie(connection, document_models=document_models)
         print("--> Initialized beanie")
```

### Comparing `sapx-0.1.6/sap/beanie/document.py` & `sapx-0.1.7/sap/beanie/document.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,16 @@
+"""
+Documents.
+
+Override beanie Documents to useful methods.
+Most of the methods are inspired from Django behavior on querying data.
+"""
+
 import datetime
-from typing import TYPE_CHECKING, Any, Mapping, Optional, Type, Union
+from typing import TYPE_CHECKING, Any, Mapping, Optional, Type, TypeVar, Union
 
 from pymongo.client_session import ClientSession
 
 import beanie
 import pydantic
 from beanie import PydanticObjectId
 
@@ -73,7 +80,10 @@
             fetch_links=fetch_links,
             with_children=with_children,
             **pymongo_kwargs,
         )
         if not result:
             raise Object404Error
         return result
+
+
+TDoc = TypeVar("TDoc", bound=Document)
```

### Comparing `sapx-0.1.6/sap/beanie/models.py` & `sapx-0.1.7/sap/beanie/models.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.6/sap/beanie/query.py` & `sapx-0.1.7/sap/beanie/query.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 """
-Query. 
+Query.
 
 Utils that can be used to optimize db queries and avoid redundant requests.
 """
 import typing
 
 from beanie import Document, Link, PydanticObjectId, operators
 from beanie.odm.fields import ExpressionField, LinkInfo
 
-ModelType = typing.TypeVar("ModelType", bound=Document)
+from .document import TDoc
 
-RelModelType = typing.TypeVar("RelModelType", bound=Document)  # Related Model Type
+RDoc = typing.TypeVar("RDoc", bound=Document)  # Related Model Type
 
 
-async def prefetch_related(item_list: list[ModelType], to_attribute: str) -> None:
+async def prefetch_related(item_list: list[TDoc], to_attribute: str) -> None:
     """
     Optimize fetching of a related attribute of one-to-one relation.
 
     Fetch related attribute efficiently in order to avoid multiple queries that could kill the db.
 
     Example:
-
     ```python
     class ProductCategory(Document):
         name: str
 
     class Product(Document):
         category: ProductCategory
         price: float
@@ -48,47 +47,46 @@
 
     # Find the model of the related attributed
     related_field: LinkInfo[Document] = type(item_list[0]).get_link_fields()[to_attribute]
     related_model: Document = related_field.model_class
 
     def get_related_id(item_: Document) -> typing.Optional[PydanticObjectId]:
         """Return the id of the related object."""
-        link: typing.Optional[Link] = getattr(item_, to_attribute)
+        link: typing.Optional[Link[Document]] = getattr(item_, to_attribute)
         if link:
             return link.ref.id
         return None
 
     # Fetch the related attribute and map it to the each item in the item_list
     related_item_ids = list(set(get_related_id(item) for item in item_list))
     related_item_list = await related_model.find(operators.In(related_model.id, related_item_ids)).to_list()
     for item in item_list:
         related_id = get_related_id(item)
         related_item = next((rel for rel in related_item_list if rel.id == related_id), None) if related_id else None
         setattr(item, to_attribute, related_item)
 
 
 async def prefetch_related_children(
-    item_list: list[ModelType],
+    item_list: list[TDoc],
     to_attribute: str,
-    related_model: type[RelModelType],
+    related_model: type[RDoc],
     related_attribute: str,
     filter_func: typing.Optional[
         typing.Callable[
-            [list[RelModelType], ModelType],
-            typing.Union[None, RelModelType, list[RelModelType]],
+            [list[RDoc], TDoc],
+            typing.Union[None, RDoc, list[RDoc]],
         ]
     ] = None,
 ) -> None:
     """
     Optimize fetching of a related attributes of one-to-many relation.
 
     Fetch related attribute efficiently in order to avoid multiple queries that could kill the db.
 
     Example:
-
     ```python
     class ProductCategory(Document):
         name: str
 
     class Product(Document):
         category: ProductCategory
         price: float
@@ -116,19 +114,19 @@
     related_item_list = await related_model.find(
         operators.In(related_expression, item_ids), sort="-doc_meta.created"
     ).to_list()
 
     for item in item_list:
         related_items = []
         for rel in related_item_list:
-            rel_link: Link[RelModelType] = getattr(rel, related_attribute)
+            rel_link: Link[RDoc] = getattr(rel, related_attribute)
             if item.id == rel_link.ref.id:
                 related_items.append(rel)
         setattr(item, to_attribute, filter_func(related_items=related_items, item=item))
 
 
 def prepare_search_string(search_text: str) -> str:
-    """Clean and reformat the search string"""
+    """Clean and reformat the search string."""
     res = search_text.strip()
     if "@" in res and not '"' in res:
         res = f'"{res}"'
     return res
```

### Comparing `sapx-0.1.6/sap/fastapi/middleware.py` & `sapx-0.1.7/sap/fastapi/middleware.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.6/sap/fastapi/serializers.py` & `sapx-0.1.7/sap/fastapi/serializers.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,29 +6,28 @@
 from __future__ import annotations
 
 import datetime
 from typing import TYPE_CHECKING, Any, Generic, Optional, TypeVar, Union
 
 from fastapi import Request
 from pydantic import BaseModel
-from pydantic.fields import SHAPE_LIST
+from pydantic.fields import SHAPE_LIST, ModelField
 
-from sap.beanie.document import Document
+from sap.beanie.document import Document, TDoc
 
 from . import utils
 
-ModelType = TypeVar("ModelType", bound=Document)
 # SerializerType = TypeVar("SerializerType", bound=BaseModel)
 
 if TYPE_CHECKING:
     from pydantic.typing import AbstractSetIntStr, DictStrAny, MappingIntStrAny
 
 
 class CursorInfo:
-    """Contains information on how the list should paginated"""
+    """Contains information on how the list should paginated."""
 
     offset: int = 0
     limit: int = 10
     sort: str = "-doc_meta.created"
 
     def __init__(self, request: Request) -> None:
         """Initialize the cursor info."""
@@ -36,15 +35,15 @@
         try:
             limit, offset = utils.base64_url_decode(cursor_str).split(",")
         except ValueError:
             return
         self.limit, self.offset = int(limit), int(offset)
 
     def get_beanie_query_params(self) -> dict[str, Any[int, str]]:
-        """Return params to apply to the database query when using beanie"""
+        """Return params to apply to the database query when using beanie."""
         return {
             "limit": self.limit,
             "skip": self.offset,
             "sort": self.sort,
         }
 
     def get_next(self) -> Optional[str]:
@@ -56,45 +55,48 @@
         """Get the cursor to paginate backward."""
         offset = self.offset - self.limit
         if offset <= 0:
             return None
         return utils.base64_url_encode(f"{self.limit},{offset}")
 
 
-class ObjectSerializer(Generic[ModelType], BaseModel):
+class ObjectSerializer(Generic[TDoc], BaseModel):
     """Serialize an object for retrieve or list."""
 
     @classmethod
-    def get_id(cls, instance: ModelType) -> str:
+    def get_id(cls, instance: TDoc) -> str:
+        """Return the Mongo ID of the object."""
         return str(instance.id)
 
     @classmethod
-    def get_created(cls, instance: ModelType) -> datetime.datetime:
+    def get_created(cls, instance: TDoc) -> datetime.datetime:
         """Return the user creation date."""
         assert instance.doc_meta.created  # let mypy know that this cannot be null
         return instance.doc_meta.created
 
     @classmethod
-    def get_updated(cls, instance: ModelType) -> datetime.datetime:
+    def get_updated(cls, instance: TDoc) -> datetime.datetime:
         """Return the user creation date."""
         assert instance.doc_meta.updated  # let mypy know that this cannot be null
         return instance.doc_meta.updated
 
     @classmethod
-    def _get_instance_data(cls, instance: ModelType, exclude: Union["AbstractSetIntStr"] = None) -> dict[str, Any]:
+    def _get_instance_data(
+        cls, instance: TDoc, exclude: Union["AbstractSetIntStr", "MappingIntStrAny"] = None
+    ) -> dict[str, Any]:
         """Retrieve the serializer value from the instance and getters."""
         data = {}
         exclude = exclude or set()
         for field_name, field in cls.__fields__.items():
             if field_name in exclude:
                 continue
             elif hasattr(cls, f"get_{field_name}"):
                 data[field_name] = getattr(cls, f"get_{field_name}")(instance=instance)
             elif issubclass(field.type_, ObjectSerializer):
-                related_object = getattr(instance, field_name)
+                related_object = getattr(instance, field_name, None)
                 if field.shape == SHAPE_LIST:
                     data[field_name] = (
                         field.type_.read_list(related_object, exclude=field.field_info.exclude)
                         if related_object
                         else []
                     )
                 else:
@@ -102,29 +104,29 @@
                         field.type_.read(related_object, exclude=field.field_info.exclude) if related_object else None
                     )
             else:
                 data[field_name] = getattr(instance, field_name)
         return data
 
     @classmethod
-    def read(cls, instance: ModelType, exclude: Union["AbstractSetIntStr"] = None) -> "SerializerType":
+    def read(cls, instance: TDoc, exclude: Union["AbstractSetIntStr", "MappingIntStrAny"] = None) -> "SerializerType":
         """Serialize a single object instance."""
         return cls(**cls._get_instance_data(instance, exclude=exclude))
 
     @classmethod
     def read_list(
-        cls, instance_list: list[ModelType], exclude: Union["AbstractSetIntStr"] = None
+        cls, instance_list: list[TDoc], exclude: Union["AbstractSetIntStr", "MappingIntStrAny"] = None
     ) -> list["SerializerType"]:
         """Serialize a list of objects."""
         return [cls.read(instance, exclude=exclude) for instance in instance_list]
 
     @classmethod
     def read_page(
         cls,
-        instance_list: list[ModelType],
+        instance_list: list[TDoc],
         cursor_info: CursorInfo,
         request: Request,
     ) -> PaginatedData["SerializerType"]:
         """Serialize a list of objects."""
 
         # TODO: implemented proper cursor pagination, for now fake it till you make it.
 
@@ -147,74 +149,106 @@
     object: str = "list"
     count: int
     next: Optional[str]
     previous: Optional[str]
     data: list[Any]
 
 
-class WriteObjectSerializer(Generic[ModelType], BaseModel):
+class WriteObjectSerializer(Generic[TDoc], BaseModel):
     """Serialize an object for create or update."""
 
-    instance: Optional[ModelType] = None
+    instance: Optional[TDoc] = None
+
+    async def run_async_validators(self) -> None:
+        """Check that data pass DB validation."""
+
+        field: ModelField
+        embedded_serializers = {}
+        for field_name, field in self.__fields__.items():
+            if issubclass(field.type_, WriteObjectSerializer):
+                embedded_serializers[field_name] = field
+
+        field_serializer: WriteObjectSerializer[TDoc]
+        for field_name in embedded_serializers:
+            if field_serializer := getattr(self, field_name):
+                if self.instance:
+                    field_serializer.instance = getattr(self.instance, field_name)
+                await field_serializer.run_async_validators()
 
     def dict(
         self,
         *,
         include: Optional[Union["AbstractSetIntStr", "MappingIntStrAny"]] = None,
         exclude: Optional[Union["AbstractSetIntStr", "MappingIntStrAny"]] = None,
         by_alias: bool = False,
         skip_defaults: Optional[bool] = None,
         exclude_unset: bool = False,
         exclude_defaults: bool = False,
         exclude_none: bool = False,
     ) -> "DictStrAny":
-        """Dumps the serializer data with exclusion of unwanted fields."""
+        """Dump the serializer data with exclusion of unwanted fields."""
         # Exclude from dumping
-        exclude = exclude or {}
-        exclude = exclude | {"instance": True}
+        exclude = (exclude or {}) | {"instance": True}
 
         # Some fields are only excluded from being cascade dumps to dict,
         # but their original value is still needed
-        exclude_dumps = {}
+        exclude_doc_dumps = {}
+
+        # Embedded documents need to be converted to object after dumps
+        embedded_serializers = {}
 
         for field_name, field in self.__fields__.items():
-            field.field_info
+            if field_name in exclude:
+                continue
 
             if issubclass(field.type_, Document):
-                exclude_dumps[field_name] = True
+                exclude_doc_dumps[field_name] = True
+
+            if issubclass(field.type_, WriteObjectSerializer):
+                embedded_serializers[field_name] = field.type_.__fields__["instance"].type_
 
             # Some fields are excluded as they are only needed for create
             if field.field_info.extra.get("exclude_update") and self.instance:
                 exclude[field_name] = True
 
             # Some fields are excluded as they are only needed for update
             if field.field_info.extra.get("exclude_create") and not self.instance:
                 exclude[field_name] = True
 
-        exclude = exclude | exclude_dumps
+        exclude = exclude | exclude_doc_dumps
 
         result = super().dict(
             include=include,
             exclude=exclude,
             by_alias=by_alias,
             skip_defaults=skip_defaults,
             exclude_unset=exclude_unset,
             exclude_defaults=exclude_defaults,
             exclude_none=exclude_none,
         )
 
-        for field_name in exclude_dumps:
+        for field_name in exclude_doc_dumps:
             result[field_name] = getattr(self, field_name)
 
+        instance_embedded: BaseModel
+        for field_name, field_model in embedded_serializers.items():
+            if not result[field_name]:
+                continue
+            if instance_embedded := getattr(self.instance, field_name, None):
+                result[field_name] = instance_embedded.copy(update=result[field_name])
+            else:
+                result[field_name] = field_model(**result[field_name])
+
         return result
 
-    async def create(self, **kwargs: Any) -> ModelType:
-        """Create the object in the database using the data extracted by the serializer"""
-        instance_class: type[ModelType] = self.__fields__["instance"].type_
+    async def create(self, **kwargs: Any) -> TDoc:
+        """Create the object in the database using the data extracted by the serializer."""
+        instance_class: type[TDoc] = self.__fields__["instance"].type_
         self.instance = await instance_class(**self.dict()).create()
         return self.instance
 
-    async def update(self, **kwargs: Any):
-        """Update the object in the database using the data extracted by the serializer"""
+    async def update(self, **kwargs: Any) -> TDoc:
+        """Update the object in the database using the data extracted by the serializer."""
+        assert self.instance
         self.instance = self.instance.copy(update=self.dict())
         await self.instance.save()
         return self.instance
```

### Comparing `sapx-0.1.6/sap/rest/client.py` & `sapx-0.1.7/sap/rest/client.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.6/sap/rest/exceptions.py` & `sapx-0.1.7/sap/rest/exceptions.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.6/sap/settings.py` & `sapx-0.1.7/sap/settings.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.6/sap/worker/__init__.py` & `sapx-0.1.7/sap/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.6/sap/worker/amqp.py` & `sapx-0.1.7/sap/worker/amqp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+AMQP.
+
+Establish connection to an AMQP server such as RabbitMQ.
+"""
 import asyncio
 
 import aioamqp
 import aioamqp.channel
 
 from sap.settings import DatabaseParams
 
@@ -13,14 +18,15 @@
     protocol: aioamqp.AmqpProtocol
     channel: aioamqp.channel.Channel
     db_params: DatabaseParams
 
     async def connect(self) -> None:
         """
         Establish connect to the AMQP server.
+
         An `__init__` method can't be a coroutine.
         """
         self.transport, self.protocol = await aioamqp.connect(
             host=self.db_params.host,
             port=self.db_params.port,
             login=self.db_params.username,
             password=self.db_params.password,
```

### Comparing `sapx-0.1.6/sap/worker/config.py` & `sapx-0.1.7/sap/worker/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+"""
+CeleryConfig.
+
+Celery config utility make it easier for app to load celery params
+depending of use case. The different use cases are:
+- LambdaCeleryConfig: Tasks that run on a remote server asynchronously, no need of waiting for result.
+- RPCCeleryConfig: Tasks that run on a remote server synchronously, need to wait for a result.
+- CronCeleryConfig: Periodic tasks that are scheduled.
+"""
 import typing
 
 # do not remove, forcing update of format for better amqp exchanges structures
 from kombu.pidbox import Mailbox
 
 Mailbox.reply_exchange_fmt = "%s.reply.pidbox"
```

### Comparing `sapx-0.1.6/sap/worker/crons.py` & `sapx-0.1.7/sap/worker/crons.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.6/sap/worker/lambdas.py` & `sapx-0.1.7/sap/worker/lambdas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
 Lambdas refers to async background tasks.
+
 They run code in response to events which are typically messages sent to a queue.
 """
 import asyncio
 import typing
 
 import celery
 import celery.bootsteps
@@ -15,16 +16,16 @@
 
 from .packet import SignalPacket
 from .utils import match_amqp_topics
 
 
 class LambdaTask(celery.Task):
     """
-    A lambda task is a task that run on a specific event,
-    usually after receiving a packet (message).
+    A lambda task is a task that run on a specific event, usually after receiving a packet (message).
+
     The Lambda will be connected to an AMQP Queue and will listen
     to packets sent to that queue that matches the packet's topic pattern.
     """
 
     time_limit: int = 60 * 1  # 1 minutes
     packet: SignalPacket
 
@@ -47,17 +48,15 @@
 
 def register_lambda(lambda_task_class: typing.Type[LambdaTask]) -> LambdaTask:
     """Register the Lambda Task to make it discoverable by task runner (celery)."""
     return lambda_task_class()
 
 
 class LambdaWorker(celery.bootsteps.ConsumerStep):
-    """
-    Celery worker that consumes packets (messages) sent to lambda queues.
-    """
+    """Celery worker that consumes packets (messages) sent to lambda queues."""
 
     packets: list[SignalPacket]
     name: str
 
     def _get_queues(self, channel: StdChannel) -> list[kombu.Queue]:
         """Retrieve the list of AMQP queues associated to each packet signal."""
         queue_list: list[kombu.Queue] = []
@@ -77,29 +76,33 @@
             # only listen to primary queue
             queue_list.append(queue_primary)
 
         return queue_list
 
     def get_consumers(self, channel: StdChannel) -> list[kombu.Consumer]:
         """
-        Create packet consumers. The consumers are the entrypoint of
+        Create packet consumers.
+
+        The consumers are the entrypoint of
         the application once celery starts receiving messages.
         """
         return [
             kombu.Consumer(
                 channel,
                 queues=self._get_queues(channel),
                 callbacks=[self.consume],
                 accept=["json"],
                 prefetch_count=10,
             )
         ]
 
     def consume(self, body: dict[str, typing.Any], message: kombu.Message) -> None:
         """
+        Run the celery worker and consume messages.
+
         This is the entrypoint of the application once celery starts receiving messages.
         All packets received are sent to this function that will acknowledge reception and dispatch
         to registered Lambda tasks.
         """
         # topic = message.delivery_info["routing_key"]
         # headers = message.headers
         # is_retry = headers and headers.get("x-death")
@@ -112,19 +115,20 @@
             message.reject()
         else:
             message.ack()
 
     def _propagate_signal(self, body: dict[str, typing.Any], message: kombu.Message) -> None:
         """
         Execute each lambda task that registered to that packet signal.
+
         Lambda tasks are all executed asynchronously and simultaneously through other background celery workers.
         Sometimes this can leads to duplicate key errors or integrity errors.
         """
         topic = message.delivery_info["routing_key"]
         for task in self.get_task_list():
             if match_amqp_topics(task.packet.topic, topic):
                 identifier = body.get("identifier") or body.get("card_pid") or body.get("clover_id")
                 task.apply_async(args=(identifier,), kwargs=body["kwargs"], time_limit=60)
 
     def get_task_list(self) -> list[LambdaTask]:
-        """Retrieves the list of lambda tasks to execute."""
+        """Retrieve the list of lambda tasks to execute."""
         raise NotImplementedError
```

### Comparing `sapx-0.1.6/sap/worker/packet.py` & `sapx-0.1.7/sap/worker/packet.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 # from . import exceptions
 
 DOMAIN_REGEX["queue-name"] = re.compile(r"^[a-zA-Z0-9-_.:@#,/><]*$")
 
 
 class _Packet:
     """
-    Defines common attributes of packets.
+    Define common attributes of packets.
+
     A Packet represents a message that has been sent to a queue
     in order to execute a task on a remote server.
     """
 
     namespace: str
     topic: str
     exchange: aioamqp.channel
@@ -36,14 +37,15 @@
     _event_type: str
     connections: dict[str, AMQPClient] = {}
     providing_args: list[str]
 
     def __init__(self, topic: str, providing_args: list[str]):
         """
         Initialize the packet. The topic contains the namespace.
+
         :providing_args: A list of arguments used for documentation purposes.
         """
         self.topic = topic
         self.namespace = topic.split(".")[0]
         self.providing_args = providing_args
 
     @classmethod
@@ -60,32 +62,34 @@
         channel = await cls.get_default_channel()
         if channel.is_open:
             await channel.close()
         cls.connections.pop("default")
 
     @classmethod
     async def get_default_channel(cls) -> aioamqp.channel.Channel:
-        """Return the default channel for the opened connection"""
+        """Return the default channel for the opened connection."""
         connection: AMQPClient = await cls.connection_retrieve()
         # if not connection.channel.is_open:
         #     cls.connections.pop('default')
         #     connection = await cls.connection_retrieve()
         return connection.channel
 
     def exchange_get_name(self, is_fallback: bool = False) -> str:
         """
         Get exchange name.
+
         :is_fallback: if True, get exchange where dead packets are transferred to.
         """
         suffix: str = ".retry" if is_fallback else ""
         return f"packet.{self._event_type}{suffix}"
 
     async def exchange_declare(self, is_fallback: bool = False) -> None:
         """
         Declare the exchange on the AMQP server.
+
         :is_fallback: if True, create a fallback exchange where dead packets are transferred to.
         """
         channel = await self.get_default_channel()
         await channel.exchange_declare(
             exchange_name=self.exchange_get_name(),
             type_name=self._exchange_type,
             durable=self._is_durable,
@@ -96,15 +100,16 @@
                 type_name=self._exchange_type,
                 durable=self._is_durable,
             )
 
 
 class SignalPacket(_Packet):
     """
-    A SignalPacket is a message sent to the messaging queue broker
+    A SignalPacket is a message sent to the messaging queue broker.
+
     to run a task asynchronously on remote server.
     Multiple applications can subscribe to the queue to receive the packets.
     """
 
     _is_durable: bool = True
     _exchange_type: str = "topic"
     _event_type: str = "signal"
@@ -131,20 +136,22 @@
             routing_key=self.topic,
             properties={"content_type": "application/json"},
         )
 
     def queue_get_name(self, task_name: str, is_fallback: bool = False) -> str:
         """
         Get queue name.
+
         :is_fallback: if True, get queue where dead packets are transferred to.
         """
         suffix: str = "@retry" if is_fallback else ""
         return f"{self._event_type}:{self.topic}->{task_name}{suffix}"
 
     def queue_get_params(self, task_name: str, is_fallback: bool = False) -> dict[str, typing.Any]:
+        """Retrieve params used to declare the queue."""
         name = self.queue_get_name(task_name=task_name, is_fallback=is_fallback)
         exchange_primary = self.exchange_get_name(is_fallback=False)
         exchange_fallback = self.exchange_get_name(is_fallback=True)
         arguments = {
             "x-delivery-limit": 5,
             "x-dead-letter-exchange": exchange_primary if is_fallback else exchange_fallback,
         }
```

### Comparing `sapx-0.1.6/sap/worker/utils.py` & `sapx-0.1.7/sap/worker/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+Utils.
+
+Utilities methods to manage worker tasks.
+"""
 import typing
 
 import celery
 import celery.schedules
 from celery.events.state import State
 from celery.utils.serialization import strtobool
 from celery.worker.control import Panel
@@ -33,14 +38,15 @@
 #         # if the timeout is not reached.
 #         signal.signal(signal.SIGALRM, signal.SIG_IGN)
 
 
 def match_amqp_topics(topic_alpha: str, topic_beta: str) -> bool:
     """
     Allow comparison on topics pattern.
+
     This method makes it easy to know if topic_a is contained in topic_b.
     """
     parts_alpha = topic_alpha.split(".")
     parts_beta = topic_beta.split(".")
     if any(a != b and a != "*" and b != "*" for (a, b) in zip(parts_alpha, parts_beta)):
         return False
     return True
@@ -55,17 +61,15 @@
     kwargs: dict[str, typing.Any]
     options: dict[str, str]
 
 
 def register_tasks_with_celery_beat(
     celery_app: celery.Celery, tasks: list[CronTask], options: dict[str, str]
 ) -> dict[str, CeleryBeatTaskParams]:
-    """
-    Retrieve all task params to set up celery beat.
-    """
+    """Retrieve all task params to set up celery beat."""
     beat_schedule: dict[str, CeleryBeatTaskParams] = {}
 
     for task in tasks:
         uid_args = "-".join([str(x) for x in task.args])
         uid_kwargs = "-".join([str(x) for x in task.kwargs.values()])
         uid = f"{task.get_name()}:{uid_args}:{uid_kwargs}"
         celery_app.register_task(task)
@@ -84,13 +88,14 @@
     type="inspect",
     alias="dump_conf",
     signature="[include_defaults=False]",
     args=[("with_defaults", strtobool)],
 )
 def conf(state: State, with_defaults: bool = False, **kwargs: typing.Any) -> dict[str, str]:
     """
-    This overrides the default `conf` inspect command to effectively disable it.
+    Override the default `conf` inspect command to effectively disable it.
+
     This is to stop sensitive configuration information appearing in e.g. Flower.
     (Celery makes an attempt to remove sensitive information, but it is not foolproof.)
     """
     assert state is not None and with_defaults is not None and kwargs is not None  # silent pylint
     return {"error": "Config inspection has been disabled."}
```

### Comparing `sapx-0.1.6/sapx.egg-info/PKG-INFO` & `sapx-0.1.7/sapx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapx
-Version: 0.1.6
+Version: 0.1.7
 Summary: Library of re-usable utilities for python web apps.
 Home-page: https://github.com/trellixio/sap
 Author: Trellix Dev
 Author-email: contact@trellix.io
 License: COPYRIGHT @ Trellix
 Classifier: Environment :: Web Environment
 Classifier: Framework :: FastAPI
```

### Comparing `sapx-0.1.6/sapx.egg-info/SOURCES.txt` & `sapx-0.1.7/sapx.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 sap/beanie/document.py
 sap/beanie/exceptions.py
 sap/beanie/models.py
 sap/beanie/query.py
 sap/fastapi/__init__.py
 sap/fastapi/auth.py
 sap/fastapi/exceptions.py
+sap/fastapi/forms.py
 sap/fastapi/middleware.py
 sap/fastapi/serializers.py
 sap/fastapi/utils.py
 sap/rest/__init__.py
 sap/rest/client.py
 sap/rest/exceptions.py
 sap/worker/__init__.py
```

### Comparing `sapx-0.1.6/setup.py` & `sapx-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
-VERSION = "0.1.6"
+VERSION = "0.1.7"
 
 setup(
     name="sapx",
     version=VERSION,
     packages=find_packages(include=("sap.*", "sap")),
     package_data={"sap": ["py.typed"]},
     include_package_data=True,
```

### Comparing `sapx-0.1.6/tests/test_fastapi_utils.py` & `sapx-0.1.7/tests/test_fastapi_utils.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.6/tests/test_rest_client.py` & `sapx-0.1.7/tests/test_rest_client.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.6/tests/test_worker_lambdas.py` & `sapx-0.1.7/tests/test_worker_lambdas.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.6/tests/test_worker_packet.py` & `sapx-0.1.7/tests/test_worker_packet.py`

 * *Files identical despite different names*

