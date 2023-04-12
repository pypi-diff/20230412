# Comparing `tmp/bigraph-schema-0.0.1.tar.gz` & `tmp/bigraph-schema-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigraph-schema-0.0.1.tar", last modified: Tue Apr 11 21:41:27 2023, max compression
+gzip compressed data, was "bigraph-schema-0.0.2.tar", last modified: Wed Apr 12 21:55:38 2023, max compression
```

## Comparing `bigraph-schema-0.0.1.tar` & `bigraph-schema-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-04-11 21:41:27.188581 bigraph-schema-0.0.1/
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1081 2023-04-11 21:41:27.188581 bigraph-schema-0.0.1/PKG-INFO
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      151 2023-04-11 21:38:33.000000 bigraph-schema-0.0.1/README.md
-drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-04-11 21:41:27.188581 bigraph-schema-0.0.1/bigraph_schema/
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      109 2023-04-11 21:34:23.000000 bigraph-schema-0.0.1/bigraph_schema/__init__.py
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     2140 2023-04-11 21:34:23.000000 bigraph-schema-0.0.1/bigraph_schema/parse.py
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)    20676 2023-04-11 21:34:23.000000 bigraph-schema-0.0.1/bigraph_schema/registry.py
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)    17453 2023-04-11 21:34:23.000000 bigraph-schema-0.0.1/bigraph_schema/schema.py
-drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-04-11 21:41:27.188581 bigraph-schema-0.0.1/bigraph_schema.egg-info/
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1081 2023-04-11 21:41:27.000000 bigraph-schema-0.0.1/bigraph_schema.egg-info/PKG-INFO
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      310 2023-04-11 21:41:27.000000 bigraph-schema-0.0.1/bigraph_schema.egg-info/SOURCES.txt
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)        1 2023-04-11 21:41:27.000000 bigraph-schema-0.0.1/bigraph_schema.egg-info/dependency_links.txt
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       18 2023-04-11 21:41:27.000000 bigraph-schema-0.0.1/bigraph_schema.egg-info/requires.txt
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       15 2023-04-11 21:41:27.000000 bigraph-schema-0.0.1/bigraph_schema.egg-info/top_level.txt
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       38 2023-04-11 21:41:27.188581 bigraph-schema-0.0.1/setup.cfg
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1309 2023-04-11 21:34:23.000000 bigraph-schema-0.0.1/setup.py
+drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-04-12 21:55:38.493119 bigraph-schema-0.0.2/
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1081 2023-04-12 21:55:38.493119 bigraph-schema-0.0.2/PKG-INFO
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      151 2023-04-11 21:38:33.000000 bigraph-schema-0.0.2/README.md
+drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-04-12 21:55:38.493119 bigraph-schema-0.0.2/bigraph_schema/
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      109 2023-04-11 21:34:23.000000 bigraph-schema-0.0.2/bigraph_schema/__init__.py
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     2140 2023-04-11 21:34:23.000000 bigraph-schema-0.0.2/bigraph_schema/parse.py
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)    17514 2023-04-12 21:52:57.000000 bigraph-schema-0.0.2/bigraph_schema/registry.py
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)    15754 2023-04-12 21:54:50.000000 bigraph-schema-0.0.2/bigraph_schema/schema.py
+drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-04-12 21:55:38.493119 bigraph-schema-0.0.2/bigraph_schema.egg-info/
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1081 2023-04-12 21:55:38.000000 bigraph-schema-0.0.2/bigraph_schema.egg-info/PKG-INFO
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      310 2023-04-12 21:55:38.000000 bigraph-schema-0.0.2/bigraph_schema.egg-info/SOURCES.txt
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)        1 2023-04-12 21:55:38.000000 bigraph-schema-0.0.2/bigraph_schema.egg-info/dependency_links.txt
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       18 2023-04-12 21:55:38.000000 bigraph-schema-0.0.2/bigraph_schema.egg-info/requires.txt
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       15 2023-04-12 21:55:38.000000 bigraph-schema-0.0.2/bigraph_schema.egg-info/top_level.txt
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       38 2023-04-12 21:55:38.493119 bigraph-schema-0.0.2/setup.cfg
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1309 2023-04-12 21:55:21.000000 bigraph-schema-0.0.2/setup.py
```

### Comparing `bigraph-schema-0.0.1/PKG-INFO` & `bigraph-schema-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigraph-schema
-Version: 0.0.1
+Version: 0.0.2
 Summary: A serializable type schema for compositional systems biology
 Home-page: https://github.com/vivarium-collective/bigraph-schema
 Author: Eran Agmon, Ryan Spangler
 Author-email: agmon.eran@gmail.com, ryan.spangler@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bigraph-schema-0.0.1/bigraph_schema/parse.py` & `bigraph-schema-0.0.2/bigraph_schema/parse.py`

 * *Files identical despite different names*

### Comparing `bigraph-schema-0.0.1/bigraph_schema/registry.py` & `bigraph-schema-0.0.2/bigraph_schema/registry.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,28 +19,14 @@
     '_ports',
     '_type_parameters',
     '_super',
 )
 
 type_schema_keys = required_schema_keys + optional_schema_keys
 
-
-# (
-#     '_default',
-#     '_apply',
-#     '_serialize',
-#     '_deserialize',
-#     '_value',
-#     '_divide',
-#     '_description',
-#     '_ports',
-#     '_type_parameters',
-#     '_super',
-# )
-
 overridable_schema_keys = (
     '_default',
     '_apply',
     '_serialize',
     '_deserialize',
     '_value',
     '_divide',
@@ -110,29 +96,14 @@
                 and isinstance(merge_dct[k], collections.abc.Mapping)):
             deep_merge(dct[k], merge_dct[k])
         else:
             dct[k] = merge_dct[k]
     return dct
 
 
-
-# class Function(object):
-#     def __init__(self, domain, codomain, fn):
-#         self.domain = domain
-#         self.codomain = codomain
-#         self.fn = fn
-
-#     def __apply__(self, arguments):
-#         return None
-
-# divide_longest = Function(Dimension, )
-
-
-
-
 class Registry(object):
     def __init__(self):
         """A Registry holds a collection of functions or objects."""
         self.registry = {}
         self.main_keys = []
 
     def register(self, key, item, alternate_keys=tuple()):
@@ -233,14 +204,27 @@
             schema = schema.copy()
             schema.pop('_type')
             schema.update(type_schema)
 
         return schema
 
 
+    def expand_schema(self, schema):
+        step = self.substitute_type(schema)
+        for key, subschema in step.items():
+            if key not in type_schema_keys:
+                step[key] = self.expand_schema(subschema)
+        return step
+        
+
+    def expand(self, schema):
+        duplicate = copy.deepcopy(schema)
+        return self.expand_schema(duplicate)
+
+
     def generate_default(self, schema):
         default = None
 
         if isinstance(schema, str):
             schema = self.access(schema)
         elif '_type' in schema:
             schema = self.access(schema['_type'])
@@ -256,57 +240,29 @@
         else:
             default = {}
             for key, subschema in schema.items():
                 if key not in type_schema_keys:
                     default[key] = self.generate_default(subschema)
 
         return default
-
-        # for key, subschema in schema.items():
-        #     if key == '_default':
-        #         if not '_deserialize' in typ:
-        #             raise Exception(
-        #                 f'asking for default for {type_key} but no deserialize in {typ}')
-        #         deserialize = deserialize_registry.access(typ['_deserialize'])
-        #         default['_value'] = deserialize(subtyp)
-        #     elif key not in type_schema_keys:
         
 
     def generate_default_type(self, type_key):
         schema = self.access(type_key)
         return self.generate_default(schema)
 
-        for key, subtyp in typ.items():
-            if key == '_default':
-                if not '_deserialize' in typ:
-                    raise Exception(
-                        f'asking for default for {type_key} but no deserialize in {typ}')
-                deserialize = deserialize_registry.access(typ['_deserialize'])
-                default['_value'] = deserialize(subtyp)
-            elif key not in type_schema_keys:
-                if '_type' in subtyp:
-                    subtyp_key = subtyp['_type']
-                    default[key] = self.generate_default(
-                        subtyp_key)
-                else:
-                    pass
-
-        default = self.generate_type_default(typ)
-                
-        return default
 
     def access(self, key):
         """Get an item by key from the registry."""
         typ = self.registry.get(key)
 
         if typ is None:
             parse = parse_type_parameters(key)
             if parse[0] in self.registry:
                 typ = self.resolve_parameters(parse)
-                print(f'parsed {key} to get {typ}')
 
         return typ
 
 
     def lookup(type_key, attribute):
         return self.access(type_key).get(attribute)
 
@@ -543,81 +499,19 @@
         '_serialize': 'str',
         '_deserialize': 'float',
         '_divide': 'divide_float',
         '_description': 'meters per second'
     }
 }
 
+
 for key, units in supported_units.items():
     type_registry.register(key, units)
 
 
-# class DimensionProcess(Process):
-#     def ports_schema(self):
-#         return {'_type': 'dimension'}
-
-#         return {
-#             '_description': 'a two-dimensional value',
-#             '_divide': custom_divide,
-#             'width': {'_type': 'float'},
-#             'height': {'_type': 'float'},
-#         }
-
-#         return {
-#             '_description': 'a two-dimensional value',
-#             '_divide': custom_divide,
-#             'width': {'_type': 'int'},
-#             'height': {
-#                 '_default': 0,
-#                 '_apply': accumulate,
-#                 '_serialize': str,
-#                 '_deserialize': int,
-#                 '_divide': divide_int,
-#                 '_description': '64-bit integer'
-#             }
-#         }
-
-    #### 
-    # def process_types(self):
-    #     return {
-    #         'base_rectangle': {
-    #             'width': {'_type': 'int'},
-    #             'height': {'_type': 'int'},
-    #             '_description': 'a two-dimensional value',
-    #             '_super': 'rectangle',
-    #         },
-    #         'rectangle_width': {
-    #             '_divide': 'divide_width',
-    #             '_super': 'base_rectangle',
-    #         },
-    #         'rectangle_longest': {
-    #             '_divide': 'divide_width',
-    #             '_super': 'base_rectangle',
-    #         }            
-    #     }
-
-
-    # def ports_schema(self):
-    #     return {'rectangle': {'_type': 'base_rectangle'}}
-
-
-    # def next_update(self, timestep, state):
-    #     rect = generate('rectangle_width', {
-    #         'width': 5,
-    #         'height': 11,
-    #     })
-
-    #     rect = generate('rectangle_base': {
-    #         'width': 5,
-    #         'height': 11,
-    #         '_divider': lambda a, parameters: a * 5
-    #     })
-    
-
-
 def schema_zoo():
     mitochondria_schema = {
         'mitochondria': {
             'volume': {'_type': 'float'},
             'membrane': {
                 'surface_proteins': {'_type': 'branch[protein]'},
                 'potential': {'_type': 'microvolts'}},
```

### Comparing `bigraph-schema-0.0.1/bigraph_schema/schema.py` & `bigraph-schema-0.0.2/bigraph_schema/schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 import pprint
 from bigraph_schema.registry import registry_registry, type_schema_keys, optional_schema_keys, type_library, deep_merge
 
 
 type_registry = registry_registry.access('_type')
 serialize_registry = registry_registry.access('_serialize')
 deserialize_registry = registry_registry.access('_deserialize')
@@ -9,21 +10,18 @@
 
 def validate_schema(schema, enforce_connections=False):
     # add ports and wires
     # validate ports are wired to a matching type,
     #   either the same type or a subtype (more specific type)
     # declared ports are equivalent to the presence of a process
     #   where the ports need to be looked up
-    # if _wires key, must have _ports key (later we will look up
-    #   processes by key and find their ports)
 
     if not isinstance(schema, dict):
         return f'schema is not a dict: {schema}'
 
-    # must be a dict
     report = {}
 
     schema_keys = set([])
     branches = set([])
 
     for key, value in schema.items():
         if key == '_type':
@@ -162,20 +160,18 @@
 
                 peer = get_path(
                     top,
                     path[:-1]
                 )
 
                 destination = establish_path(
-                    # instance,
                     peer,
                     subwires[:-1],
                     top=top,
                     cursor=path[:-1])
-                    # cursor=path)
 
                 destination_key = subwires[-1]
 
                 if destination_key in destination:
                     pass
                     # validate_instance(
                     #     port_schema,
@@ -186,16 +182,15 @@
         else:
             # handle unconnected ports
             pass
 
     return instance
 
 
-def fill(schema, instance=None, top=None, path=(), type_key=None, context=None):
-
+def fill_instance(schema, instance=None, top=None, path=(), type_key=None, context=None):
     # if a port is disconnected, build a store
     # for it under the '_open' key in the current
     # node
 
     # inform the user that they have disconnected
     # ports somehow
 
@@ -224,57 +219,27 @@
                 instance=instance,
                 top=top,
                 path=path)
 
         elif key not in type_schema_keys:
             subpath = path + (key,)
             if isinstance(instance, dict):
-                instance[key] = fill(
+                instance[key] = fill_instance(
                     subschema,
                     instance=instance.get(key),
                     top=top,
                     path=subpath)
         
     return instance
 
-    # if instance is None:
-    #     instance = type_registry.generate_default()
-
-    # if type_key is None:
-    #     if '_type' in schema:
-    #         type_key = schema['_type']
-    #     else:
-    #         raise Exception(
-    #             f'no _type known or inferred at path {path} for {schema}'
-    #         )
-
-    # if context is None:
-    #     context = type_registry.access(type_key)
-
-    # result = {
-    #     '_type': type_key
-    # }
-
-    # if top is None:
-    #     top = result
-
-    # for key, subcontext in context.items():
-    #     if key not in schema:
-    #         raise Exception(
-    #             f'branch of type {type_key} not present in schema {schema}'
-    #         )
-    #     if key not in type_schema_keys:
-    #         result[key] = fill_schema(schema[key])
 
-    # return result
-
-
-# def validate_edges(state, schema, enforce_connections=False):
-#     for key, subschema in schema.items():
-        
+def fill(schema, instance=None):
+    if instance is not None:
+        instance = copy.deepcopy(instance)
+    return fill_instance(schema, instance=instance)
 
 
 def merge(a, b):
     pass
 
 
 def compose(a, b):
@@ -332,35 +297,18 @@
         },
         'ports match': {
             'a': {
                 '_type': 'int',
                 '_value': 2
             },
             'edge1': {
-                # this could become a process_edge type
                 '_type': 'edge',
                 '_ports': {
                     '1': {'_type': 'int'},
-                    # '2': {'_type': 'float'}
                 },
-                # 'process': {
-                #     '_type': 'process instance',
-                #     '_value': 'process:location/somewhere',
-                # },
-                # 'config': {
-                #     '_type': 'hash[any]',
-                #     '_value': {},
-                # },
-                # 'wires': {
-                #     '_type': 'hash[list[string]]',
-                #     '_value': {
-                #         '1': ['..', 'a'],
-                #         # '2': ['..', 'b']
-                #     }
-                # }
             }
         }
     }        
 
     # bad schemas
     bad = {
         'empty': None,
@@ -416,18 +364,15 @@
                 'port A': {'_type': 'float'},
             },
         }
     }
 
     test_instance = {
         'edge 1': {
-            # 'process': some_process,
             'wires': {
-                ## support this syntax
-                # 'port A': 'a',
                 'port A': 'a',
             }
         }
     }
 
     filled = fill(
         test_schema,
@@ -441,20 +386,18 @@
                 'port A': 'a'
             }
         }
     }
 
 def test_fill_in_disconnected_port():
     test_schema = {
-        # 'a': {'_type': 'int', '_value': 2},
         'edge1': {
             '_type': 'edge',
             '_ports': {
                 '1': {'_type': 'float'},
-                # '2': {'_type': 'float'}
             },
         }
     }
 
     test_instance = {}
 
     import ipdb; ipdb.set_trace()
@@ -463,15 +406,15 @@
 def test_fill_type_mismatch():
     test_schema = {
         'a': {'_type': 'int', '_value': 2},
         'edge1': {
             '_type': 'edge',
             '_ports': {
                 '1': {'_type': 'float'},
-                # '2': {'_type': 'float'}
+                '2': {'_type': 'float'}
             },
             'wires': {
                 '1': ['..', 'a'],
                 '2': ['a'],
             },
             'a': 5
         },
@@ -498,21 +441,19 @@
                 '1': ['..', 'a']
             },
         },
     }
 
 
 def test_fill_nested_store():
-        # 'a': {'_type': 'int', '_value': 2},
     test_schema = {
         'edge1': {
             '_type': 'edge',
             '_ports': {
                 '1': {'_type': 'float'},
-                # '2': {'_type': 'float'}
             },
             'wires': {
                 '1': ['somewhere', 'down', 'this', 'path']
             },
         },
     }    
 
@@ -532,14 +473,22 @@
          'made',
          'of',
          'light'))
 
     assert tree['some']['where']['deep']['inside']['lives']['a']['tiny']['creature']['made']['of']['light'] == destination
 
 
+def test_expand_schema():
+    schema = {'_type': 'cube'}
+    expanded = type_registry.expand(schema)
+
+    assert len(schema) == 1
+    assert 'height' in expanded
+
+
 def test_expected_schema():
     # equivalent to previous schema:
 
     # expected = {
     #     'store1': {
     #         'store1.1': {
     #             '_value': 1.1,
@@ -660,15 +609,15 @@
 if __name__ == '__main__':
     test_validate_schema()
     test_fill_int()
     test_fill_cube()
     test_establish_path()
     test_fill_in_missing_nodes()
     test_expected_schema()
-
+    test_expand_schema()
```

### Comparing `bigraph-schema-0.0.1/bigraph_schema.egg-info/PKG-INFO` & `bigraph-schema-0.0.2/bigraph_schema.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigraph-schema
-Version: 0.0.1
+Version: 0.0.2
 Summary: A serializable type schema for compositional systems biology
 Home-page: https://github.com/vivarium-collective/bigraph-schema
 Author: Eran Agmon, Ryan Spangler
 Author-email: agmon.eran@gmail.com, ryan.spangler@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bigraph-schema-0.0.1/setup.py` & `bigraph-schema-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 from setuptools import setup, find_packages
 
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 
 
 with open("README.md", "r") as readme:
     description = readme.read()
 
 
 setup(
```

