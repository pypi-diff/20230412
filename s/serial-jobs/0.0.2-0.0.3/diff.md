# Comparing `tmp/serial-jobs-0.0.2.tar.gz` & `tmp/serial-jobs-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serial-jobs-0.0.2.tar", last modified: Sun May 15 12:04:01 2022, max compression
+gzip compressed data, was "serial-jobs-0.0.3.tar", last modified: Wed Apr 12 14:45:26 2023, max compression
```

## Comparing `serial-jobs-0.0.2.tar` & `serial-jobs-0.0.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2022-05-15 12:04:01.921271 serial-jobs-0.0.2/
--rw-r--r--   0 peter     (1000) peter     (1000)     1071 2022-05-01 11:21:32.000000 serial-jobs-0.0.2/LICENSE
--rw-r--r--   0 peter     (1000) peter     (1000)     2218 2022-05-15 12:04:01.921271 serial-jobs-0.0.2/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)     1839 2022-05-15 11:54:41.000000 serial-jobs-0.0.2/README.md
--rw-r--r--   0 peter     (1000) peter     (1000)      373 2022-05-15 09:42:17.000000 serial-jobs-0.0.2/pyproject.toml
--rw-r--r--   0 peter     (1000) peter     (1000)      829 2022-05-15 12:04:01.921271 serial-jobs-0.0.2/setup.cfg
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2022-05-15 12:04:01.921271 serial-jobs-0.0.2/src/
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2022-05-15 12:04:01.921271 serial-jobs-0.0.2/src/serial_jobs/
--rw-r--r--   0 peter     (1000) peter     (1000)      333 2022-05-15 11:30:27.000000 serial-jobs-0.0.2/src/serial_jobs/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3479 2022-05-15 09:17:46.000000 serial-jobs-0.0.2/src/serial_jobs/config.py
--rw-r--r--   0 peter     (1000) peter     (1000)     7372 2022-05-14 20:06:05.000000 serial-jobs-0.0.2/src/serial_jobs/data.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2022-05-15 12:04:01.921271 serial-jobs-0.0.2/src/serial_jobs/device/
--rw-r--r--   0 peter     (1000) peter     (1000)      127 2022-05-14 20:06:35.000000 serial-jobs-0.0.2/src/serial_jobs/device/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)    11125 2022-05-14 20:40:07.000000 serial-jobs-0.0.2/src/serial_jobs/device/base.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3407 2022-05-14 17:53:31.000000 serial-jobs-0.0.2/src/serial_jobs/device/bms.py
--rw-r--r--   0 peter     (1000) peter     (1000)     8104 2022-05-14 16:04:42.000000 serial-jobs-0.0.2/src/serial_jobs/device/modbus.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2622 2022-05-15 09:00:47.000000 serial-jobs-0.0.2/src/serial_jobs/handler.py
--rw-r--r--   0 peter     (1000) peter     (1000)     5855 2022-05-14 02:57:27.000000 serial-jobs-0.0.2/src/serial_jobs/job.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2341 2022-05-14 18:17:41.000000 serial-jobs-0.0.2/src/serial_jobs/main.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3182 2022-05-14 17:33:59.000000 serial-jobs-0.0.2/src/serial_jobs/mqtt.py
--rw-r--r--   0 peter     (1000) peter     (1000)     4972 2022-05-15 09:00:47.000000 serial-jobs-0.0.2/src/serial_jobs/schema.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2022-05-15 12:04:01.921271 serial-jobs-0.0.2/src/serial_jobs/scripts/
--rw-r--r--   0 peter     (1000) peter     (1000)        0 2022-05-15 09:09:58.000000 serial-jobs-0.0.2/src/serial_jobs/scripts/__init__.py
--rwxr-xr-x   0 peter     (1000) peter     (1000)     1445 2022-05-15 09:00:47.000000 serial-jobs-0.0.2/src/serial_jobs/scripts/convert_config.py
--rwxr-xr-x   0 peter     (1000) peter     (1000)     1924 2022-05-15 09:00:47.000000 serial-jobs-0.0.2/src/serial_jobs/scripts/merge_config.py
--rwxr-xr-x   0 peter     (1000) peter     (1000)     1804 2022-05-14 18:30:21.000000 serial-jobs-0.0.2/src/serial_jobs/scripts/run.py
--rw-r--r--   0 peter     (1000) peter     (1000)     5291 2022-05-14 18:35:31.000000 serial-jobs-0.0.2/src/serial_jobs/service.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1362 2022-05-08 13:19:30.000000 serial-jobs-0.0.2/src/serial_jobs/specification.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2437 2022-05-14 02:57:04.000000 serial-jobs-0.0.2/src/serial_jobs/task.py
--rw-r--r--   0 peter     (1000) peter     (1000)     4463 2022-05-14 19:27:00.000000 serial-jobs-0.0.2/src/serial_jobs/value.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2022-05-15 12:04:01.921271 serial-jobs-0.0.2/src/serial_jobs.egg-info/
--rw-r--r--   0 peter     (1000) peter     (1000)     2218 2022-05-15 12:04:01.000000 serial-jobs-0.0.2/src/serial_jobs.egg-info/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)      867 2022-05-15 12:04:01.000000 serial-jobs-0.0.2/src/serial_jobs.egg-info/SOURCES.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        1 2022-05-15 12:04:01.000000 serial-jobs-0.0.2/src/serial_jobs.egg-info/dependency_links.txt
--rw-r--r--   0 peter     (1000) peter     (1000)      199 2022-05-15 12:04:01.000000 serial-jobs-0.0.2/src/serial_jobs.egg-info/entry_points.txt
--rw-r--r--   0 peter     (1000) peter     (1000)       65 2022-05-15 12:04:01.000000 serial-jobs-0.0.2/src/serial_jobs.egg-info/requires.txt
--rw-r--r--   0 peter     (1000) peter     (1000)       12 2022-05-15 12:04:01.000000 serial-jobs-0.0.2/src/serial_jobs.egg-info/top_level.txt
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2023-04-12 14:45:26.292306 serial-jobs-0.0.3/
+-rw-r--r--   0 peter      (501) staff       (20)     1071 2022-05-08 11:19:26.000000 serial-jobs-0.0.3/LICENSE
+-rw-r--r--   0 peter      (501) staff       (20)    30579 2023-04-12 14:45:26.292356 serial-jobs-0.0.3/PKG-INFO
+-rw-r--r--   0 peter      (501) staff       (20)    30203 2023-04-12 14:44:50.000000 serial-jobs-0.0.3/README.rst
+-rw-r--r--   0 peter      (501) staff       (20)      373 2022-05-18 00:29:13.000000 serial-jobs-0.0.3/pyproject.toml
+-rw-r--r--   0 peter      (501) staff       (20)      827 2023-04-12 14:45:26.292636 serial-jobs-0.0.3/setup.cfg
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2023-04-12 14:45:26.287250 serial-jobs-0.0.3/src/
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2023-04-12 14:45:26.290502 serial-jobs-0.0.3/src/serial_jobs/
+-rw-r--r--   0 peter      (501) staff       (20)      333 2023-04-12 14:44:50.000000 serial-jobs-0.0.3/src/serial_jobs/__init__.py
+-rw-r--r--   0 peter      (501) staff       (20)     3479 2023-04-07 09:18:03.000000 serial-jobs-0.0.3/src/serial_jobs/config.py
+-rw-r--r--   0 peter      (501) staff       (20)     7372 2022-07-24 13:43:17.000000 serial-jobs-0.0.3/src/serial_jobs/data.py
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2023-04-12 14:45:26.291694 serial-jobs-0.0.3/src/serial_jobs/device/
+-rw-r--r--   0 peter      (501) staff       (20)      127 2022-05-18 00:29:13.000000 serial-jobs-0.0.3/src/serial_jobs/device/__init__.py
+-rw-r--r--   0 peter      (501) staff       (20)    11125 2022-05-18 00:29:13.000000 serial-jobs-0.0.3/src/serial_jobs/device/base.py
+-rw-r--r--   0 peter      (501) staff       (20)     3407 2022-05-18 00:29:13.000000 serial-jobs-0.0.3/src/serial_jobs/device/bms.py
+-rw-r--r--   0 peter      (501) staff       (20)     8104 2022-05-18 00:29:13.000000 serial-jobs-0.0.3/src/serial_jobs/device/modbus.py
+-rw-r--r--   0 peter      (501) staff       (20)     2622 2022-05-18 00:29:13.000000 serial-jobs-0.0.3/src/serial_jobs/handler.py
+-rw-r--r--   0 peter      (501) staff       (20)     5855 2022-05-18 00:29:13.000000 serial-jobs-0.0.3/src/serial_jobs/job.py
+-rw-r--r--   0 peter      (501) staff       (20)     2341 2022-05-18 00:29:13.000000 serial-jobs-0.0.3/src/serial_jobs/main.py
+-rw-r--r--   0 peter      (501) staff       (20)     3182 2022-05-18 00:29:13.000000 serial-jobs-0.0.3/src/serial_jobs/mqtt.py
+-rw-r--r--   0 peter      (501) staff       (20)     4971 2023-04-07 09:18:03.000000 serial-jobs-0.0.3/src/serial_jobs/schema.py
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2023-04-12 14:45:26.292176 serial-jobs-0.0.3/src/serial_jobs/scripts/
+-rw-r--r--   0 peter      (501) staff       (20)        0 2022-05-18 00:29:13.000000 serial-jobs-0.0.3/src/serial_jobs/scripts/__init__.py
+-rwxr-xr-x   0 peter      (501) staff       (20)     1445 2022-05-18 00:29:13.000000 serial-jobs-0.0.3/src/serial_jobs/scripts/convert_config.py
+-rwxr-xr-x   0 peter      (501) staff       (20)     1924 2022-05-18 00:29:13.000000 serial-jobs-0.0.3/src/serial_jobs/scripts/merge_config.py
+-rwxr-xr-x   0 peter      (501) staff       (20)     1804 2022-05-18 00:29:13.000000 serial-jobs-0.0.3/src/serial_jobs/scripts/run.py
+-rw-r--r--   0 peter      (501) staff       (20)     5291 2022-05-18 00:29:13.000000 serial-jobs-0.0.3/src/serial_jobs/service.py
+-rw-r--r--   0 peter      (501) staff       (20)     1362 2022-05-08 13:39:42.000000 serial-jobs-0.0.3/src/serial_jobs/specification.py
+-rw-r--r--   0 peter      (501) staff       (20)     2437 2022-05-18 00:29:13.000000 serial-jobs-0.0.3/src/serial_jobs/task.py
+-rw-r--r--   0 peter      (501) staff       (20)     4463 2022-05-18 00:29:13.000000 serial-jobs-0.0.3/src/serial_jobs/value.py
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2023-04-12 14:45:26.291205 serial-jobs-0.0.3/src/serial_jobs.egg-info/
+-rw-r--r--   0 peter      (501) staff       (20)    30579 2023-04-12 14:45:26.000000 serial-jobs-0.0.3/src/serial_jobs.egg-info/PKG-INFO
+-rw-r--r--   0 peter      (501) staff       (20)      868 2023-04-12 14:45:26.000000 serial-jobs-0.0.3/src/serial_jobs.egg-info/SOURCES.txt
+-rw-r--r--   0 peter      (501) staff       (20)        1 2023-04-12 14:45:26.000000 serial-jobs-0.0.3/src/serial_jobs.egg-info/dependency_links.txt
+-rw-r--r--   0 peter      (501) staff       (20)      199 2023-04-12 14:45:26.000000 serial-jobs-0.0.3/src/serial_jobs.egg-info/entry_points.txt
+-rw-r--r--   0 peter      (501) staff       (20)       65 2023-04-12 14:45:26.000000 serial-jobs-0.0.3/src/serial_jobs.egg-info/requires.txt
+-rw-r--r--   0 peter      (501) staff       (20)       12 2023-04-12 14:45:26.000000 serial-jobs-0.0.3/src/serial_jobs.egg-info/top_level.txt
```

### Comparing `serial-jobs-0.0.2/LICENSE` & `serial-jobs-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `serial-jobs-0.0.2/setup.cfg` & `serial-jobs-0.0.3/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 url = https://github.com/pbasista/serial-jobs/
 author = Peter Bašista
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Topic :: Home Automation
 	Topic :: Utilities
-long_description = file: README.md
-long_description_content_type = text/markdown
+long_description = file: README.rst
+long_description_content_type = text/x-rst
 
 [options]
 package_dir = 
 	= src
 packages = find:
 install_requires = 
 	gmqtt
```

### Comparing `serial-jobs-0.0.2/src/serial_jobs/config.py` & `serial-jobs-0.0.3/src/serial_jobs/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os.path import isfile
 
 from strictyaml import YAML, as_document, load
 from strictyaml.ruamel.comments import CommentedMap
 
 from .schema import configuration_schema, configuration_stub_schema
 
-DEFAULT_CONFIG_PATH = "./configuration.yaml"
+DEFAULT_CONFIG_PATH = "./configuration.json"
 DEFAULT_JSON_CONFIG_PATH = DEFAULT_CONFIG_PATH.rsplit(".", maxsplit=1)[0] + ".json"
 LOGGER = getLogger(__name__)
 
 
 def merge_configurations(
     input_one: CommentedMap, input_two: CommentedMap
 ) -> CommentedMap:
```

### Comparing `serial-jobs-0.0.2/src/serial_jobs/data.py` & `serial-jobs-0.0.3/src/serial_jobs/data.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -34,16 +34,16 @@
     data_type: type[RegisterDataT]
     register_spec: RegisterSpec
     byte_order: Optional[list[int]]
     byte_offset: int
     byte_count: Optional[int]
     bitmask: Optional[int]
     bitshift: Optional[int]
-    scale_factor: Optional[int]
     increase_by: Optional[int]
+    scale_factor: Optional[int]
 
     @classmethod
     # pylint: disable-next=too-many-locals
     def from_spec(cls, spec: dict) -> Data:
         unpack_type, data_part_spec = next(iter(spec.items()))
         data_type: type[RegisterDataT] = str
         if unpack_type in (
@@ -75,28 +75,28 @@
         byte_offset = data_part_spec.get("byte_offset", 0)
         byte_count = data_part_spec.get("byte_count")
         if byte_index is not None:
             byte_offset = byte_index
             byte_count = 1
         bitmask = data_part_spec.get("bitmask")
         bitshift = data_part_spec.get("bitshift")
-        scale_factor = data_part_spec.get("scale_factor")
         increase_by = data_part_spec.get("increase_by")
+        scale_factor = data_part_spec.get("scale_factor")
 
         return cls(
             unpack_type=unpack_type,
             data_type=data_type,
             register_spec=register_spec,
             byte_order=byte_order,
             byte_offset=byte_offset,
             byte_count=byte_count,
             bitmask=bitmask,
             bitshift=bitshift,
-            scale_factor=scale_factor,
             increase_by=increase_by,
+            scale_factor=scale_factor,
         )
 
     def unpack(self, register_bytes: bytes) -> RegisterDataT:
         if self.unpack_type == "string":
             return register_bytes.decode("utf-8")
         return unpack(self.format_strings[self.unpack_type], register_bytes)[0]
```

### Comparing `serial-jobs-0.0.2/src/serial_jobs/device/base.py` & `serial-jobs-0.0.3/src/serial_jobs/device/base.py`

 * *Files identical despite different names*

### Comparing `serial-jobs-0.0.2/src/serial_jobs/device/bms.py` & `serial-jobs-0.0.3/src/serial_jobs/device/bms.py`

 * *Files identical despite different names*

### Comparing `serial-jobs-0.0.2/src/serial_jobs/device/modbus.py` & `serial-jobs-0.0.3/src/serial_jobs/device/modbus.py`

 * *Files identical despite different names*

### Comparing `serial-jobs-0.0.2/src/serial_jobs/handler.py` & `serial-jobs-0.0.3/src/serial_jobs/handler.py`

 * *Files identical despite different names*

### Comparing `serial-jobs-0.0.2/src/serial_jobs/job.py` & `serial-jobs-0.0.3/src/serial_jobs/job.py`

 * *Files identical despite different names*

### Comparing `serial-jobs-0.0.2/src/serial_jobs/main.py` & `serial-jobs-0.0.3/src/serial_jobs/main.py`

 * *Files identical despite different names*

### Comparing `serial-jobs-0.0.2/src/serial_jobs/mqtt.py` & `serial-jobs-0.0.3/src/serial_jobs/mqtt.py`

 * *Files identical despite different names*

### Comparing `serial-jobs-0.0.2/src/serial_jobs/schema.py` & `serial-jobs-0.0.3/src/serial_jobs/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 class YAMLSerializationError(ValueError):
     ...
 
 
 def is_binary(value: str) -> bool:
     """Return true if the provided value is a string of a binary integer."""
-    return re_compile(r"^0[bB]+[01]+$").match(value) is not None
+    return re_compile(r"^0[bB][01]+$").match(value) is not None
 
 
 class BinInt(ScalarValidator):
     def validate_scalar(self, chunk):
         val = chunk.contents
         if not is_binary(val):
             chunk.expecting_but_found("when expecting a binary integer")
@@ -104,16 +104,16 @@
         "address": HexInt(),
         Optional("byte_order"): Seq(Int()),
         Optional("byte_offset"): Int(),
         Optional("byte_count"): Int(),
         Optional("byte_index"): Int(),  # if defined, overrides offset and count
         Optional("bitmask"): BinInt(),
         Optional("bitshift"): Int(),  # if positive, shift to the right
-        Optional("scale_factor"): Int(),
         Optional("increase_by"): Int(),
+        Optional("scale_factor"): Int(),
     }
 )
 
 data_part_schema = MapPattern(
     Enum(list(Data.format_strings.keys()) + ["string"]),
     register_schema,
     minimum_keys=1,
```

### Comparing `serial-jobs-0.0.2/src/serial_jobs/scripts/convert_config.py` & `serial-jobs-0.0.3/src/serial_jobs/scripts/convert_config.py`

 * *Files identical despite different names*

### Comparing `serial-jobs-0.0.2/src/serial_jobs/scripts/merge_config.py` & `serial-jobs-0.0.3/src/serial_jobs/scripts/merge_config.py`

 * *Files identical despite different names*

### Comparing `serial-jobs-0.0.2/src/serial_jobs/scripts/run.py` & `serial-jobs-0.0.3/src/serial_jobs/scripts/run.py`

 * *Files identical despite different names*

### Comparing `serial-jobs-0.0.2/src/serial_jobs/service.py` & `serial-jobs-0.0.3/src/serial_jobs/service.py`

 * *Files identical despite different names*

### Comparing `serial-jobs-0.0.2/src/serial_jobs/specification.py` & `serial-jobs-0.0.3/src/serial_jobs/specification.py`

 * *Files identical despite different names*

### Comparing `serial-jobs-0.0.2/src/serial_jobs/task.py` & `serial-jobs-0.0.3/src/serial_jobs/task.py`

 * *Files identical despite different names*

### Comparing `serial-jobs-0.0.2/src/serial_jobs/value.py` & `serial-jobs-0.0.3/src/serial_jobs/value.py`

 * *Files identical despite different names*

### Comparing `serial-jobs-0.0.2/src/serial_jobs.egg-info/SOURCES.txt` & `serial-jobs-0.0.3/src/serial_jobs.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 LICENSE
-README.md
+README.rst
 pyproject.toml
 setup.cfg
 src/serial_jobs/__init__.py
 src/serial_jobs/config.py
 src/serial_jobs/data.py
 src/serial_jobs/handler.py
 src/serial_jobs/job.py
```

