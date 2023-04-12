# Comparing `tmp/twb_project-0.7.1.tar.gz` & `tmp/twb_project-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twb_project-0.7.1.tar", max compression
+gzip compressed data, was "twb_project-0.7.2.tar", max compression
```

## Comparing `twb_project-0.7.1.tar` & `twb_project-0.7.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    18092 2023-02-26 13:10:42.136159 twb_project-0.7.1/LICENSE
--rw-r--r--   0        0        0     1547 2023-02-27 01:45:34.838817 twb_project-0.7.1/README.md
--rw-r--r--   0        0        0      760 2023-03-27 02:05:29.889681 twb_project-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      201 2023-03-26 05:00:17.199386 twb_project-0.7.1/twb/__init__.py
--rw-r--r--   0        0        0      788 2023-02-26 15:18:15.849792 twb_project-0.7.1/twb/bip.py
--rw-r--r--   0        0        0    16138 2023-03-26 23:28:51.163801 twb_project-0.7.1/twb/builder.py
--rw-r--r--   0        0        0     4614 2023-03-26 18:02:08.247223 twb_project-0.7.1/twb/decompressor.py
--rw-r--r--   0        0        0     9493 2023-03-26 18:01:42.380403 twb_project-0.7.1/twb/downloader.py
--rw-r--r--   0        0        0     3607 2023-03-26 19:24:30.197127 twb_project-0.7.1/twb/logger.py
--rw-r--r--   0        0        0      546 2023-03-26 05:47:24.185465 twb_project-0.7.1/twb/modifier.py
--rw-r--r--   0        0        0    11632 2023-03-26 21:37:48.900993 twb_project-0.7.1/twb/parallelization.py
--rw-r--r--   0        0        0    10966 2023-03-27 02:23:52.390871 twb_project-0.7.1/twb/reader.py
--rw-r--r--   0        0        0     5713 2023-03-26 23:28:38.347621 twb_project-0.7.1/twb/utils.py
--rw-r--r--   0        0        0     2435 1970-01-01 00:00:00.000000 twb_project-0.7.1/setup.py
--rw-r--r--   0        0        0     2590 1970-01-01 00:00:00.000000 twb_project-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-02-26 13:10:42.136159 twb_project-0.7.2/LICENSE
+-rw-r--r--   0        0        0     1547 2023-02-27 01:45:34.838817 twb_project-0.7.2/README.md
+-rw-r--r--   0        0        0      760 2023-04-12 00:39:34.393087 twb_project-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0      201 2023-03-26 05:00:17.199386 twb_project-0.7.2/twb/__init__.py
+-rw-r--r--   0        0        0      788 2023-02-26 15:18:15.849792 twb_project-0.7.2/twb/bip.py
+-rw-r--r--   0        0        0    16138 2023-03-26 23:28:51.163801 twb_project-0.7.2/twb/builder.py
+-rw-r--r--   0        0        0     4614 2023-03-26 18:02:08.247223 twb_project-0.7.2/twb/decompressor.py
+-rw-r--r--   0        0        0     9493 2023-03-26 18:01:42.380403 twb_project-0.7.2/twb/downloader.py
+-rw-r--r--   0        0        0     3607 2023-03-26 19:24:30.197127 twb_project-0.7.2/twb/logger.py
+-rw-r--r--   0        0        0      546 2023-03-26 05:47:24.185465 twb_project-0.7.2/twb/modifier.py
+-rw-r--r--   0        0        0    11632 2023-03-26 21:37:48.900993 twb_project-0.7.2/twb/parallelization.py
+-rw-r--r--   0        0        0    11317 2023-04-12 00:22:13.542074 twb_project-0.7.2/twb/reader.py
+-rw-r--r--   0        0        0     6161 2023-04-12 00:33:50.301793 twb_project-0.7.2/twb/utils.py
+-rw-r--r--   0        0        0     2435 1970-01-01 00:00:00.000000 twb_project-0.7.2/setup.py
+-rw-r--r--   0        0        0     2590 1970-01-01 00:00:00.000000 twb_project-0.7.2/PKG-INFO
```

### Comparing `twb_project-0.7.1/LICENSE` & `twb_project-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.1/README.md` & `twb_project-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.1/pyproject.toml` & `twb_project-0.7.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twb-project"
-version = "0.7.1"
+version = "0.7.2"
 description = "An unified tool for the research in extracting information from Wikipedia Edit History chunk."
 authors = ["Lingxi Li <hi@lingxi.li>"]
 license = "GNU GPL"
 readme = "README.md"
 packages = [
     { include = "twb" },
 ]
```

### Comparing `twb_project-0.7.1/twb/bip.py` & `twb_project-0.7.2/twb/bip.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.1/twb/builder.py` & `twb_project-0.7.2/twb/builder.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.1/twb/decompressor.py` & `twb_project-0.7.2/twb/decompressor.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.1/twb/downloader.py` & `twb_project-0.7.2/twb/downloader.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.1/twb/logger.py` & `twb_project-0.7.2/twb/logger.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.1/twb/modifier.py` & `twb_project-0.7.2/twb/modifier.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.1/twb/parallelization.py` & `twb_project-0.7.2/twb/parallelization.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.1/twb/reader.py` & `twb_project-0.7.2/twb/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import json
 import logging
 import os
 import uuid
-from typing import Union, List
+from typing import Union, List, Tuple
 import time
 
 from .modifier import Modifier
 from .logger import cleanup_logger, universal_logger_init, twb_logger
 from .parallelization import RDSProcessManager, RDSProcessController
 from .utils import get_file_list, decompress_zstd, prepare_output_dir, get_curr_version, get_line_positions, \
-    cleanup_dir, read_line_in_file, compress_zstd, COMPRESSION_EXTENSION
+    cleanup_dir, read_line_in_file, compress_zstd, COMPRESSION_EXTENSION, parse_schema
 
 _DEFAULT_NUM_PROC = 1
 _DEFAULT_LOG_LEVEL = logging.DEBUG
 
 
 class Reader:
     """
@@ -68,15 +68,15 @@
         """
         if not path:
             raise ValueError('The path cannot be empty.')
         if not os.path.exists(path):
             raise FileNotFoundError('The path does not exist.')
         self.files.extend(get_file_list(path))
 
-    def glimpse(self) -> Union[dict, None]:
+    def glimpse(self) -> Union[Tuple[dict, dict], Tuple[None, None]]:
         """
         Take a glimpse of the data.
         It could still be large if one object contains a lot of information (e.g. many revisions, long article).
         """
         if len(self.files) == 0:
             twb_logger.warning('No file is loaded.')
             return None
@@ -95,23 +95,23 @@
 
         # Decompress the file.
         decompressed_path = _decompress_executor(glimpse_path, glimpse_temp_dir)
         first_block_text = read_line_in_file(decompressed_path, 0).rstrip('\n')
 
         if first_block_text[0] != '{' or first_block_text[-1] != '}':
             twb_logger.error(f'Invalid starting of block or end of block.')
-            return None
+            return None, None
 
         # Read the first block into memory and then delete the decompressed file.
         first_block = json.loads(first_block_text)
         cleanup_dir(glimpse_temp_dir)
 
         twb_logger.info(f'Glimpse finished.')
 
-        return first_block
+        return first_block, parse_schema(first_block)
 
     def decompress(self, output_dir: str):
         """
         Decompress the selected files.
         :param output_dir: the directory to store the decompressed files
         """
         # Log the version.
@@ -291,20 +291,27 @@
         return
 
     # Parse the block from text to JSON.
     block = json.loads(block_text)
 
     # Apply the modifiers.
     for modifier in modifiers:
+        if block is None:
+            break
         block = modifier.modify(block)
 
-    with controller.parallel_lock:
-        try:
-            with open(target_path, 'a') as f:
-                f.write(json.dumps(block) + '\n')
-        except Exception as e:
-            controller.logerr(f'Error occurred when writing block to file: {e}')
+    # We write the output only if the block is not None. Otherwise, we remove this block.
+    if block is not None:
+        with controller.parallel_lock:
+            try:
+                with open(target_path, 'a') as f:
+                    f.write(json.dumps(block) + '\n')
+            except Exception as e:
+                controller.logerr(f'Error occurred when writing block to file: {e}')
+
+    else:
+        controller.logdebug(f'Removed block because of "None": {position}')
 
     end_time = time.time()
     execution_duration = end_time - start_time
 
     controller.logdebug(f'Finished block: {position} -- (took {execution_duration:.2f}s)')
```

### Comparing `twb_project-0.7.1/twb/utils.py` & `twb_project-0.7.2/twb/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     for root, directories, files in os.walk(input_path):
         for file in files:
             if file.startswith('.'):
                 continue
             file_path = os.path.join(root, file)
             all_files.append(file_path)
 
-    # Remove duplicate files.
+    # Remove duplicate files. Sort them for determinism.
     all_files = sorted(list(set(all_files)))
     return all_files
 
 
 def get_decompress_output_path(input_path: str, output_dir: str):
     """
     Get the output path of the decompressed file.
@@ -180,7 +180,23 @@
             twb_logger.error(e)
 
 
 def prepare_output_dir(output_dir: str):
     if os.path.exists(output_dir):
         cleanup_dir(output_dir)
     os.makedirs(output_dir)
+
+
+def parse_schema(obj):
+    """
+    Parse the schema of the given object. Used for glimpse.
+    """
+    if isinstance(obj, dict):
+        if not obj:
+            return "empty"
+        return {key: parse_schema(value) for key, value in obj.items()}
+    elif isinstance(obj, list):
+        if not obj:
+            return "empty"
+        return [parse_schema(obj[0]), len(obj)]
+    else:
+        return type(obj).__name__
```

### Comparing `twb_project-0.7.1/setup.py` & `twb_project-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'py7zr>=0.20.4,<0.21.0',
  'requests>=2.28.2,<3.0.0',
  'xmltodict>=0.13.0,<0.14.0',
  'zstandard>=0.20.0,<0.21.0']
 
 setup_kwargs = {
     'name': 'twb-project',
-    'version': '0.7.1',
+    'version': '0.7.2',
     'description': 'An unified tool for the research in extracting information from Wikipedia Edit History chunk.',
     'long_description': '<img src="https://imagedelivery.net/Dr98IMl5gQ9tPkFM5JRcng/49178640-2f6d-4c23-e56f-a48eca531200/HD" alt="TWB" />\n\n# Temporal Wikipedia Blocks (TWB)\n\nTemporal Wikipedia Blocks (TWB) is a powerful Python package designed to process the extensive edit history of Wikipedia pages into easily manageable and memory-friendly blocks. The package is specifically developed to enable efficient parallelization and composition of these blocks to facilitate faster processing and analysis of large Wikipedia datasets. The original design of this package is to build other Wikipedia-oriented datasets on top of it.\n\nThe package works by dividing the Wikipedia edit history into temporal blocks, which are essentially subsets of the complete dataset that are based on time intervals. These blocks can then be easily processed and analyzed without the need to load the entire dataset into memory.\n\n## Installation\n\nThe package is available on PyPI and can be installed using pip:\n\n```bash\npip install twb-project\n```\n\n## Benefits\n\n- **Efficient**: The package is designed to be memory-friendly and can be easily parallelized to process large datasets.\n- **Fast**: The package is designed to be fast and can be easily optimized to process large datasets.\n- **Flexible**: The package is designed to be flexible and can be easily extended to support other types of blocks.\n- **Composable**: The package is designed to be composable and can be easily combined with other packages to build other datasets.\n\n## Specification\n\n- Default compression method: ZStandard.\n',
     'author': 'Lingxi Li',
     'author_email': 'hi@lingxi.li',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://twb.lingxi.li/',
```

### Comparing `twb_project-0.7.1/PKG-INFO` & `twb_project-0.7.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twb-project
-Version: 0.7.1
+Version: 0.7.2
 Summary: An unified tool for the research in extracting information from Wikipedia Edit History chunk.
 Home-page: https://twb.lingxi.li/
 License: GNU GPL
 Author: Lingxi Li
 Author-email: hi@lingxi.li
 Requires-Python: >=3.8,<4
 Classifier: License :: Other/Proprietary License
```

