# Comparing `tmp/edge_orm-0.5.2.tar.gz` & `tmp/edge_orm-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edge_orm-0.5.2.tar", max compression
+gzip compressed data, was "edge_orm-0.5.3.tar", max compression
```

## Comparing `edge_orm-0.5.2.tar` & `edge_orm-0.5.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       10 2023-02-08 20:21:01.345400 edge_orm-0.5.2/README.md
--rw-r--r--   0        0        0      774 2023-02-27 21:50:15.475075 edge_orm-0.5.2/edge_orm/__init__.py
--rw-r--r--   0        0        0     1729 2023-02-08 20:21:01.355224 edge_orm-0.5.2/edge_orm/cache.py
--rw-r--r--   0        0        0      108 2023-02-08 20:21:01.355283 edge_orm-0.5.2/edge_orm/errors.py
--rw-r--r--   0        0        0     2191 2023-02-08 20:21:01.355352 edge_orm-0.5.2/edge_orm/execute.py
--rw-r--r--   0        0        0     5446 2023-02-08 20:21:01.355464 edge_orm-0.5.2/edge_orm/external/encoders.py
--rw-r--r--   0        0        0     1036 2023-02-08 20:21:01.355536 edge_orm-0.5.2/edge_orm/helpers.py
--rw-r--r--   0        0        0     2194 2023-02-08 20:21:01.355611 edge_orm-0.5.2/edge_orm/logs.py
--rw-r--r--   0        0        0      302 2023-02-08 20:21:01.355706 edge_orm-0.5.2/edge_orm/node/__init__.py
--rw-r--r--   0        0        0       41 2023-02-08 20:21:01.355784 edge_orm-0.5.2/edge_orm/node/errors.py
--rw-r--r--   0        0        0     4533 2023-03-03 19:12:38.252561 edge_orm-0.5.2/edge_orm/node/models.py
--rw-r--r--   0        0        0      259 2023-02-27 21:41:14.553137 edge_orm-0.5.2/edge_orm/resolver/__init__.py
--rw-r--r--   0        0        0      180 2023-02-08 20:21:01.356047 edge_orm-0.5.2/edge_orm/resolver/enums.py
--rw-r--r--   0        0        0      135 2023-02-27 21:40:59.506123 edge_orm-0.5.2/edge_orm/resolver/errors.py
--rw-r--r--   0        0        0     5270 2023-02-08 20:21:01.356166 edge_orm-0.5.2/edge_orm/resolver/merging.py
--rw-r--r--   0        0        0    40536 2023-03-03 19:12:27.322122 edge_orm-0.5.2/edge_orm/resolver/model.py
--rw-r--r--   0        0        0     5294 2023-02-08 20:21:01.356439 edge_orm-0.5.2/edge_orm/resolver/nested_resolvers.py
--rw-r--r--   0        0        0     3706 2023-02-08 20:21:01.356510 edge_orm-0.5.2/edge_orm/resolver/utils.py
--rw-r--r--   0        0        0      957 2023-02-08 20:21:01.356588 edge_orm-0.5.2/edge_orm/span.py
--rw-r--r--   0        0        0      251 2023-02-08 20:21:01.356691 edge_orm-0.5.2/edge_orm/types_generator/__init__.py
--rw-r--r--   0        0        0     8120 2023-04-04 16:56:52.369943 edge_orm-0.5.2/edge_orm/types_generator/introspection.py
--rw-r--r--   0        0        0    39673 2023-03-28 16:19:37.524744 edge_orm-0.5.2/edge_orm/types_generator/main.py
--rw-r--r--   0        0        0      791 2023-02-08 20:21:01.357019 edge_orm-0.5.2/edge_orm/unset.py
--rw-r--r--   0        0        0     1381 2023-04-05 02:25:36.630393 edge_orm-0.5.2/edge_orm/validators.py
--rw-r--r--   0        0        0      725 2023-04-05 02:26:23.631208 edge_orm-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      874 1970-01-01 00:00:00.000000 edge_orm-0.5.2/setup.py
--rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 edge_orm-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0       10 2023-02-08 20:21:01.345400 edge_orm-0.5.3/README.md
+-rw-r--r--   0        0        0      774 2023-02-27 21:50:15.475075 edge_orm-0.5.3/edge_orm/__init__.py
+-rw-r--r--   0        0        0     1729 2023-02-08 20:21:01.355224 edge_orm-0.5.3/edge_orm/cache.py
+-rw-r--r--   0        0        0      108 2023-02-08 20:21:01.355283 edge_orm-0.5.3/edge_orm/errors.py
+-rw-r--r--   0        0        0     2191 2023-02-08 20:21:01.355352 edge_orm-0.5.3/edge_orm/execute.py
+-rw-r--r--   0        0        0     5446 2023-02-08 20:21:01.355464 edge_orm-0.5.3/edge_orm/external/encoders.py
+-rw-r--r--   0        0        0     1036 2023-02-08 20:21:01.355536 edge_orm-0.5.3/edge_orm/helpers.py
+-rw-r--r--   0        0        0     2194 2023-02-08 20:21:01.355611 edge_orm-0.5.3/edge_orm/logs.py
+-rw-r--r--   0        0        0      302 2023-02-08 20:21:01.355706 edge_orm-0.5.3/edge_orm/node/__init__.py
+-rw-r--r--   0        0        0       41 2023-02-08 20:21:01.355784 edge_orm-0.5.3/edge_orm/node/errors.py
+-rw-r--r--   0        0        0     4533 2023-03-03 19:12:38.252561 edge_orm-0.5.3/edge_orm/node/models.py
+-rw-r--r--   0        0        0      259 2023-02-27 21:41:14.553137 edge_orm-0.5.3/edge_orm/resolver/__init__.py
+-rw-r--r--   0        0        0      180 2023-02-08 20:21:01.356047 edge_orm-0.5.3/edge_orm/resolver/enums.py
+-rw-r--r--   0        0        0      135 2023-02-27 21:40:59.506123 edge_orm-0.5.3/edge_orm/resolver/errors.py
+-rw-r--r--   0        0        0     5270 2023-02-08 20:21:01.356166 edge_orm-0.5.3/edge_orm/resolver/merging.py
+-rw-r--r--   0        0        0    40592 2023-04-11 22:22:13.354696 edge_orm-0.5.3/edge_orm/resolver/model.py
+-rw-r--r--   0        0        0     5294 2023-02-08 20:21:01.356439 edge_orm-0.5.3/edge_orm/resolver/nested_resolvers.py
+-rw-r--r--   0        0        0     3706 2023-02-08 20:21:01.356510 edge_orm-0.5.3/edge_orm/resolver/utils.py
+-rw-r--r--   0        0        0      957 2023-02-08 20:21:01.356588 edge_orm-0.5.3/edge_orm/span.py
+-rw-r--r--   0        0        0      251 2023-02-08 20:21:01.356691 edge_orm-0.5.3/edge_orm/types_generator/__init__.py
+-rw-r--r--   0        0        0     8120 2023-04-04 16:56:52.369943 edge_orm-0.5.3/edge_orm/types_generator/introspection.py
+-rw-r--r--   0        0        0    39673 2023-03-28 16:19:37.524744 edge_orm-0.5.3/edge_orm/types_generator/main.py
+-rw-r--r--   0        0        0      791 2023-02-08 20:21:01.357019 edge_orm-0.5.3/edge_orm/unset.py
+-rw-r--r--   0        0        0     1381 2023-04-05 02:25:36.630393 edge_orm-0.5.3/edge_orm/validators.py
+-rw-r--r--   0        0        0      785 2023-04-11 22:19:36.080338 edge_orm-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0      874 1970-01-01 00:00:00.000000 edge_orm-0.5.3/setup.py
+-rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 edge_orm-0.5.3/PKG-INFO
```

### Comparing `edge_orm-0.5.2/edge_orm/__init__.py` & `edge_orm-0.5.3/edge_orm/__init__.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.5.2/edge_orm/cache.py` & `edge_orm-0.5.3/edge_orm/cache.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.5.2/edge_orm/execute.py` & `edge_orm-0.5.3/edge_orm/execute.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.5.2/edge_orm/external/encoders.py` & `edge_orm-0.5.3/edge_orm/external/encoders.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.5.2/edge_orm/helpers.py` & `edge_orm-0.5.3/edge_orm/helpers.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.5.2/edge_orm/logs.py` & `edge_orm-0.5.3/edge_orm/logs.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.5.2/edge_orm/node/models.py` & `edge_orm-0.5.3/edge_orm/node/models.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.5.2/edge_orm/resolver/merging.py` & `edge_orm-0.5.3/edge_orm/resolver/merging.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.5.2/edge_orm/resolver/model.py` & `edge_orm-0.5.3/edge_orm/resolver/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -750,15 +750,15 @@
             include_select=True,
             include_filters=False,
         )
 
         if include_changes or include_permissions:
             changes_keys = patch.set_fields_
             if include_changes:
-                changes_str = f"_changes := {{ {', '.join([f'{k} := (before.{k}, after.{k})' for k in changes_keys])} }}"
+                changes_str = f"_changes := {{ {', '.join([f'{k} := {{ _old := before.{k}, _new := after.{k} }}' for k in changes_keys])} }}"
             else:
                 changes_str = ""
             final_update_s = f"""
             with
                 before := (select {self.model_name} {filters_s}),
                 after := (update before set {update_s}),
             select {{ 
@@ -854,15 +854,17 @@
         raw_response = T.cast(RAW_RESP_ONE, raw_response)
         if raw_response["_exists"] and not raw_response["_updated"]:
             raise errors.PermissionsError("You do not have permissions to update.")
         if not raw_response["_updated"]:
             raise errors.ObjectNotFound("Object not found.")
         n = self.parse_obj_with_cache(raw_response["after"])
         # now make changes d
-        changes = {k: tuple(v) for k, v in raw_response["_changes"].items()}
+        changes = {
+            k: (v["_old"], v["_new"]) for k, v in raw_response["_changes"].items()
+        }
         return n, changes
 
     async def update_many(
         self,
         patch: PatchType,
         *,
         update_all: bool = False,
```

### Comparing `edge_orm-0.5.2/edge_orm/resolver/nested_resolvers.py` & `edge_orm-0.5.3/edge_orm/resolver/nested_resolvers.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.5.2/edge_orm/resolver/utils.py` & `edge_orm-0.5.3/edge_orm/resolver/utils.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.5.2/edge_orm/span.py` & `edge_orm-0.5.3/edge_orm/span.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.5.2/edge_orm/types_generator/introspection.py` & `edge_orm-0.5.3/edge_orm/types_generator/introspection.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.5.2/edge_orm/types_generator/main.py` & `edge_orm-0.5.3/edge_orm/types_generator/main.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.5.2/edge_orm/unset.py` & `edge_orm-0.5.3/edge_orm/unset.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.5.2/edge_orm/validators.py` & `edge_orm-0.5.3/edge_orm/validators.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.5.2/pyproject.toml` & `edge_orm-0.5.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tool.poetry]
 name = "edge-orm"
-version = "0.5.2"
+version = "0.5.3"
 description = ""
 authors = ["Jeremy Berman <jerber@sas.upenn.edu>"]
 readme = "README.md"
 packages = [{ include = "edge_orm" }]
 exclude = ["tests/**/*"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 edgedb = "^1.2.0"
+#pydantic = {version = ">=2.0a1", allow-prereleases = true}
 pydantic = { extras = ["email"], version = "^1.10" }
 orjson = "^3.8.0"
 devtools = "*"
 black = "*"
 
 
 mkdocs-material = { version = "^8.5.7", optional = true }
```

### Comparing `edge_orm-0.5.2/setup.py` & `edge_orm-0.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'pydantic[email]>=1.10,<2.0']
 
 extras_require = \
 {'docs': ['mkdocs-material>=8.5.7,<9.0.0']}
 
 setup_kwargs = {
     'name': 'edge-orm',
-    'version': '0.5.2',
+    'version': '0.5.3',
     'description': '',
     'long_description': '# edge orm',
     'author': 'Jeremy Berman',
     'author_email': 'jerber@sas.upenn.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `edge_orm-0.5.2/PKG-INFO` & `edge_orm-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edge-orm
-Version: 0.5.2
+Version: 0.5.3
 Summary: 
 Author: Jeremy Berman
 Author-email: jerber@sas.upenn.edu
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
```

