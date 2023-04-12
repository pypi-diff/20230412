# Comparing `tmp/aars-0.5.6.tar.gz` & `tmp/aars-0.5.7.tar.gz`

## Comparing `aars-0.5.6.tar` & `aars-0.5.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 aars-0.5.6/docs-requirements.txt
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 aars-0.5.6/mkdocs.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.5.6/py.typed
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 aars-0.5.6/requirements.txt
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 aars-0.5.6/.github/workflows/mkdocs-gh-pages.yml
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aars-0.5.6/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 aars-0.5.6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 aars-0.5.6/docs/FastAPI_Cookbook.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.5.6/docs/index.md -> ../README.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aars-0.5.6/docs/Code_Reference/Exceptions.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 aars-0.5.6/docs/Code_Reference/utils.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 aars-0.5.6/docs/Code_Reference/core/AARS.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aars-0.5.6/docs/Code_Reference/core/Index.md
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 aars-0.5.6/docs/Code_Reference/core/Record.md
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 aars-0.5.6/src/aars/__init__.py
--rw-r--r--   0        0        0    37114 2020-02-02 00:00:00.000000 aars-0.5.6/src/aars/core.py
--rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 aars-0.5.6/src/aars/exceptions.py
--rw-r--r--   0        0        0    10191 2020-02-02 00:00:00.000000 aars-0.5.6/src/aars/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.5.6/tests/__init__.py
--rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 aars-0.5.6/tests/aars.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 aars-0.5.6/tests/fetch_all.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 aars-0.5.6/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 aars-0.5.6/LICENSE
--rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 aars-0.5.6/README.md
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 aars-0.5.6/pyproject.toml
--rw-r--r--   0        0        0     3804 2020-02-02 00:00:00.000000 aars-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 aars-0.5.7/docs-requirements.txt
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 aars-0.5.7/mkdocs.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.5.7/py.typed
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 aars-0.5.7/requirements.txt
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 aars-0.5.7/.github/workflows/mkdocs-gh-pages.yml
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aars-0.5.7/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 aars-0.5.7/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 aars-0.5.7/docs/FastAPI_Cookbook.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.5.7/docs/index.md -> ../README.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aars-0.5.7/docs/Code_Reference/Exceptions.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 aars-0.5.7/docs/Code_Reference/utils.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 aars-0.5.7/docs/Code_Reference/core/AARS.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aars-0.5.7/docs/Code_Reference/core/Index.md
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 aars-0.5.7/docs/Code_Reference/core/Record.md
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 aars-0.5.7/src/aars/__init__.py
+-rw-r--r--   0        0        0    38261 2020-02-02 00:00:00.000000 aars-0.5.7/src/aars/core.py
+-rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 aars-0.5.7/src/aars/exceptions.py
+-rw-r--r--   0        0        0    10191 2020-02-02 00:00:00.000000 aars-0.5.7/src/aars/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.5.7/tests/__init__.py
+-rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 aars-0.5.7/tests/aars.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 aars-0.5.7/tests/fetch_all.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 aars-0.5.7/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 aars-0.5.7/LICENSE
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 aars-0.5.7/README.md
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 aars-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0     3804 2020-02-02 00:00:00.000000 aars-0.5.7/PKG-INFO
```

### Comparing `aars-0.5.6/mkdocs.yml` & `aars-0.5.7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `aars-0.5.6/.github/workflows/mkdocs-gh-pages.yml` & `aars-0.5.7/.github/workflows/mkdocs-gh-pages.yml`

 * *Files identical despite different names*

### Comparing `aars-0.5.6/.github/workflows/publish.yml` & `aars-0.5.7/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `aars-0.5.6/.github/workflows/python-publish.yml` & `aars-0.5.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `aars-0.5.6/docs/FastAPI_Cookbook.md` & `aars-0.5.7/docs/FastAPI_Cookbook.md`

 * *Files identical despite different names*

### Comparing `aars-0.5.6/src/aars/core.py` & `aars-0.5.7/src/aars/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -797,37 +797,56 @@
         if not issubclass(record_type, Record):
             raise ValueError("record_type must be a subclass of Record.")
         channels = None if channel is None else [channel]
         owners = None if owner is None else [owner]
         if item_hashes is None and channels is None and owners is None:
             channels = [cls.channel]
 
+        returned_records = 0
+
         if cls.cache and item_hashes is not None:
             # TODO: Add some kind of caching for channels and owners or add recent item_hashes endpoint to the Aleph API
             records = await cls._fetch_records_from_cache(record_type, item_hashes)
             cached_ids = []
             for record in records:
                 cached_ids.append(record.id_hash)
                 record.changed = False
                 yield record
+                if page:
+                    # If we are fetching a specific page, we need to track the number of records returned
+                    # as the cache does not know about the pagination
+                    returned_records += 1
+                    if returned_records >= page_size:
+                        return
             # Remove the cached ids from the list of item_hashes to fetch from the API
             item_hashes = [h for h in item_hashes if h not in cached_ids]
             if len(item_hashes) == 0:
                 return
 
+        if returned_records:
+            # If we got some records from the cache, we fetch a reduced number of item_hashes from the API
+            # This messes with the pagination, so we need to drop all assumptions about the page number to be fetched
+            # and track the number of records returned instead
+            page = None
+
         async for record in cls._fetch_records_from_api(
             record_type=record_type,
             item_hashes=item_hashes,
             channels=channels,
             owners=owners,
             page_size=page_size,
             page=page,
         ):
             record.changed = False
             yield record
+            if returned_records:
+                # Only triggers if we are fetching a specific page
+                returned_records += 1
+                if returned_records >= page_size:
+                    return
 
     @classmethod
     async def _fetch_records_from_cache(
         cls, record_type: Type[R], item_hashes: List[str]
     ) -> List[R]:
         assert cls.cache, "Cache is not set"
         raw_records = await asyncio.gather(*[cls.cache.get(h) for h in item_hashes])
@@ -863,33 +882,36 @@
         """
         aleph_resp = None
         retries = cls.retry_count
         if item_hashes is not None:
             item_hashes = [str(h) for h in item_hashes]
         while aleph_resp is None:
             try:
+                # If we want to fetch all pages, we need to fetch the first page to get the total number of items
                 actual_page = page if page else 1
                 aleph_resp = await cls.session.get_posts(
                     hashes=item_hashes,
                     channels=channels,
                     types=[record_type.__name__],
                     addresses=owners,
                     refs=refs,
                     pagination=page_size,
                     page=actual_page,
                 )
             except ServerDisconnectedError:
+                # Retry if the connection was interrupted
                 retries -= 1
                 if retries == 0:
                     raise
+
         for post in aleph_resp["posts"]:
             yield await record_type.from_dict(post)
 
         if page is None:
-            # Get all pages
+            # Get all pages iteratively if page is not specified
             total_items = aleph_resp["pagination_total"]
             per_page = aleph_resp["pagination_per_page"]
             if total_items > per_page:
                 for next_page in range(2, math.ceil(total_items / per_page) + 1):
                     async for record in cls._fetch_records_from_api(
                         record_type=record_type,
                         item_hashes=item_hashes,
```

### Comparing `aars-0.5.6/src/aars/exceptions.py` & `aars-0.5.7/src/aars/exceptions.py`

 * *Files identical despite different names*

### Comparing `aars-0.5.6/src/aars/utils.py` & `aars-0.5.7/src/aars/utils.py`

 * *Files identical despite different names*

### Comparing `aars-0.5.6/tests/aars.py` & `aars-0.5.7/tests/aars.py`

 * *Files identical despite different names*

### Comparing `aars-0.5.6/tests/fetch_all.py` & `aars-0.5.7/tests/fetch_all.py`

 * *Files identical despite different names*

### Comparing `aars-0.5.6/.gitignore` & `aars-0.5.7/.gitignore`

 * *Files identical despite different names*

### Comparing `aars-0.5.6/LICENSE` & `aars-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aars-0.5.6/README.md` & `aars-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `aars-0.5.6/pyproject.toml` & `aars-0.5.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aars"
-version = "0.5.6"
+version = "0.5.7"
 authors = [
   { name="Mike Hukiewitz", email="mike.hukiewitz@robotter.ai" },
 ]
 description = "Experimental Object-Document-Mapper using pydantic to store objects on Aleph.im"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `aars-0.5.6/PKG-INFO` & `aars-0.5.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aars
-Version: 0.5.6
+Version: 0.5.7
 Summary: Experimental Object-Document-Mapper using pydantic to store objects on Aleph.im
 Project-URL: Homepage, https://github.com/aleph-im/active-record-sdk
 Project-URL: Bug Tracker, https://github.com/aleph-im/active-record-sdk/issues
 Author-email: Mike Hukiewitz <mike.hukiewitz@robotter.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

