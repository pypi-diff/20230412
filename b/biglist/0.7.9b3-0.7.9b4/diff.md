# Comparing `tmp/biglist-0.7.9b3.tar.gz` & `tmp/biglist-0.7.9b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biglist-0.7.9b3.tar", last modified: Tue Apr 11 16:10:10 2023, max compression
+gzip compressed data, was "biglist-0.7.9b4.tar", last modified: Wed Apr 12 20:07:25 2023, max compression
```

## Comparing `biglist-0.7.9b3.tar` & `biglist-0.7.9b4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1067 2023-01-09 08:46:44.766242 biglist-0.7.9b3/LICENSE
--rw-r--r--   0        0        0      931 2023-04-10 09:40:14.837561 biglist-0.7.9b3/README.rst
--rw-r--r--   0        0        0     1628 2023-04-11 16:08:19.638866 biglist-0.7.9b3/pyproject.toml
--rw-r--r--   0        0        0     2217 2023-04-11 15:56:45.207292 biglist-0.7.9b3/src/biglist/__init__.py
--rw-r--r--   0        0        0    18415 2023-04-10 09:40:14.847560 biglist-0.7.9b3/src/biglist/_base.py
--rw-r--r--   0        0        0    43822 2023-04-11 15:54:40.146432 biglist-0.7.9b3/src/biglist/_biglist.py
--rw-r--r--   0        0        0    33751 2023-04-10 09:40:14.847560 biglist-0.7.9b3/src/biglist/_parquet.py
--rw-r--r--   0        0        0    12025 2023-04-10 09:40:14.847560 biglist-0.7.9b3/src/biglist/_util.py
--rw-r--r--   0        0        0        0 2023-01-09 08:46:44.766242 biglist-0.7.9b3/src/biglist/py.typed
--rw-r--r--   0        0        0     2209 1970-01-01 00:00:00.000000 biglist-0.7.9b3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-01-09 08:46:44.766242 biglist-0.7.9b4/LICENSE
+-rw-r--r--   0        0        0      931 2023-04-10 09:40:14.837561 biglist-0.7.9b4/README.rst
+-rw-r--r--   0        0        0     1628 2023-04-11 16:08:19.638866 biglist-0.7.9b4/pyproject.toml
+-rw-r--r--   0        0        0     2217 2023-04-12 19:30:05.357161 biglist-0.7.9b4/src/biglist/__init__.py
+-rw-r--r--   0        0        0    18415 2023-04-10 09:40:14.847560 biglist-0.7.9b4/src/biglist/_base.py
+-rw-r--r--   0        0        0    43817 2023-04-12 20:05:04.951149 biglist-0.7.9b4/src/biglist/_biglist.py
+-rw-r--r--   0        0        0    33845 2023-04-12 19:44:51.303943 biglist-0.7.9b4/src/biglist/_parquet.py
+-rw-r--r--   0        0        0    12025 2023-04-10 09:40:14.847560 biglist-0.7.9b4/src/biglist/_util.py
+-rw-r--r--   0        0        0        0 2023-01-09 08:46:44.766242 biglist-0.7.9b4/src/biglist/py.typed
+-rw-r--r--   0        0        0     2209 1970-01-01 00:00:00.000000 biglist-0.7.9b4/PKG-INFO
```

### Comparing `biglist-0.7.9b3/LICENSE` & `biglist-0.7.9b4/LICENSE`

 * *Files identical despite different names*

### Comparing `biglist-0.7.9b3/README.rst` & `biglist-0.7.9b4/README.rst`

 * *Files identical despite different names*

### Comparing `biglist-0.7.9b3/pyproject.toml` & `biglist-0.7.9b4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `biglist-0.7.9b3/src/biglist/__init__.py` & `biglist-0.7.9b4/src/biglist/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,8 +48,8 @@
 )
 from ._util import (
     Chain,
     Seq,
     Slicer,
 )
 
-__version__ = "0.7.9b3"
+__version__ = "0.7.9b4"
```

### Comparing `biglist-0.7.9b3/src/biglist/_base.py` & `biglist-0.7.9b4/src/biglist/_base.py`

 * *Files identical despite different names*

### Comparing `biglist-0.7.9b3/src/biglist/_biglist.py` & `biglist-0.7.9b4/src/biglist/_biglist.py`

 * *Files 1% similar despite different names*

```diff
@@ -902,15 +902,15 @@
     @classmethod
     def new(
         cls,
         data: Iterable[Any],
         path: Optional[PathType],
         *,
         batch_size: int = 10_000,
-        storage_format: Optional[str] = None,
+        storage_format: str = 'pickle',
     ):
         """
         Parameters
         ----------
         data
             The data elements that need to be distributed. The elements should be pickle-able.
         path
@@ -923,15 +923,15 @@
             However, there are no strong reasons to use this facility on a local machine.
 
             Usually this class is used to distribute data to a cluster of machines, hence
             this path points to a location in a cloud storage that is supported by ``upathlib``.
         """
         path = resolve_path(path)
         bl = Biglist.new(
-            path / "data", batch_size=batch_size, storage_format=storage_format
+            path / "data", batch_size=batch_size, storage_format=storage_format,
         )
         bl.extend(data)
         bl.flush()
         assert len(bl) > 0
         return cls(path)
 
     def __init__(
```

### Comparing `biglist-0.7.9b3/src/biglist/_parquet.py` & `biglist-0.7.9b4/src/biglist/_parquet.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,20 +59,22 @@
 
         This is provided under the (un-verified) assumption that the
         default credential inference process is a high overhead.
         """
         # Import here b/c user may not be on GCP
         from upathlib.gcs import get_google_auth
 
-        _, cred, _ = get_google_auth(
+        cls._GCP_PROJECT_ID, cls._GCP_CREDENTIALS, _ = get_google_auth(
+            project_id=getattr(cls, '_GCP_PROJECT_ID', None),
             credentials=getattr(cls, "_GCP_CREDENTIALS", None),
             valid_for_seconds=good_for_seconds,
         )
         return GcsFileSystem(
-            access_token=cred.token, credential_token_expiration=cred.expiry
+            access_token=cls._GCP_CREDENTIALS.token,
+            credential_token_expiration=cls._GCP_CREDENTIALS.expiry
         )
 
     @classmethod
     def load_data_file(cls, path: Upath) -> ParquetFile:
         """
         Load the data file given by ``path``.
 
@@ -881,16 +883,14 @@
         Passed on to `pyarrow.parquet.write_table() <https://arrow.apache.org/docs/python/generated/pyarrow.parquet.write_table.html>`_.
     """
     path = resolve_path(path)
     if isinstance(path, LocalUpath):
         path.parent.path.mkdir(exist_ok=True, parents=True)
     ff, pp = FileSystem.from_uri(str(path))
     if isinstance(ff, GcsFileSystem):
-        from ._parquet import ParquetBiglist
-
         ff = ParquetBiglist.get_gcsfs()
     pyarrow.parquet.write_table(table, ff.open_output_stream(pp), **kwargs)
 
 
 def write_arrays_to_parquet(
     data: Sequence[pyarrow.Array | pyarrow.ChunkedArray | Iterable],
     path: PathType,
```

### Comparing `biglist-0.7.9b3/src/biglist/_util.py` & `biglist-0.7.9b4/src/biglist/_util.py`

 * *Files identical despite different names*

### Comparing `biglist-0.7.9b3/PKG-INFO` & `biglist-0.7.9b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biglist
-Version: 0.7.9b3
+Version: 0.7.9b4
 Summary: The package `biglist <https://github.com/zpz/biglist>`_ provides persisted, out-of-memory Python data structures
 Author-email: Zepu Zhang <zepu.zhang@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

