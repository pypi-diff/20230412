# Comparing `tmp/ddcci_plasmoid_backend-0.1.3.tar.gz` & `tmp/ddcci_plasmoid_backend-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddcci_plasmoid_backend-0.1.3.tar", max compression
+gzip compressed data, was "ddcci_plasmoid_backend-0.1.4.tar", max compression
```

## Comparing `ddcci_plasmoid_backend-0.1.3.tar` & `ddcci_plasmoid_backend-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     3126 2023-04-11 20:59:26.584966 ddcci_plasmoid_backend-0.1.3/ddcci_plasmoid_backend/Node.py
--rw-r--r--   0        0        0     3393 2023-04-11 20:59:26.588299 ddcci_plasmoid_backend-0.1.3/ddcci_plasmoid_backend/Node_test.py
--rw-r--r--   0        0        0      889 2023-04-11 20:59:26.588299 ddcci_plasmoid_backend-0.1.3/ddcci_plasmoid_backend/__init__.py
--rw-r--r--   0        0        0     3253 2023-04-11 20:59:26.588299 ddcci_plasmoid_backend-0.1.3/ddcci_plasmoid_backend/__main__.py
--rw-r--r--   0        0        0     5512 2023-04-11 20:59:26.588299 ddcci_plasmoid_backend-0.1.3/ddcci_plasmoid_backend/ddcci.py
--rw-r--r--   0        0        0     1941 2023-04-11 20:59:26.588299 ddcci_plasmoid_backend-0.1.3/ddcci_plasmoid_backend/ddcci_test.py
--rw-r--r--   0        0        0      631 2023-04-11 20:59:42.701439 ddcci_plasmoid_backend-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      468 1970-01-01 00:00:00.000000 ddcci_plasmoid_backend-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     3126 2023-04-11 20:59:26.584966 ddcci_plasmoid_backend-0.1.4/ddcci_plasmoid_backend/Node.py
+-rw-r--r--   0        0        0     3393 2023-04-11 20:59:26.588299 ddcci_plasmoid_backend-0.1.4/ddcci_plasmoid_backend/Node_test.py
+-rw-r--r--   0        0        0      889 2023-04-11 20:59:26.588299 ddcci_plasmoid_backend-0.1.4/ddcci_plasmoid_backend/__init__.py
+-rw-r--r--   0        0        0     3484 2023-04-12 12:46:00.782718 ddcci_plasmoid_backend-0.1.4/ddcci_plasmoid_backend/__main__.py
+-rw-r--r--   0        0        0     6132 2023-04-12 12:46:00.782718 ddcci_plasmoid_backend-0.1.4/ddcci_plasmoid_backend/ddcci.py
+-rw-r--r--   0        0        0     1967 2023-04-12 12:46:00.786051 ddcci_plasmoid_backend-0.1.4/ddcci_plasmoid_backend/ddcci_test.py
+-rw-r--r--   0        0        0      631 2023-04-12 12:47:17.500355 ddcci_plasmoid_backend-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      468 1970-01-01 00:00:00.000000 ddcci_plasmoid_backend-0.1.4/PKG-INFO
```

### Comparing `ddcci_plasmoid_backend-0.1.3/ddcci_plasmoid_backend/Node.py` & `ddcci_plasmoid_backend-0.1.4/ddcci_plasmoid_backend/Node.py`

 * *Files identical despite different names*

### Comparing `ddcci_plasmoid_backend-0.1.3/ddcci_plasmoid_backend/Node_test.py` & `ddcci_plasmoid_backend-0.1.4/ddcci_plasmoid_backend/Node_test.py`

 * *Files identical despite different names*

### Comparing `ddcci_plasmoid_backend-0.1.3/ddcci_plasmoid_backend/__init__.py` & `ddcci_plasmoid_backend-0.1.4/ddcci_plasmoid_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `ddcci_plasmoid_backend-0.1.3/ddcci_plasmoid_backend/__main__.py` & `ddcci_plasmoid_backend-0.1.4/ddcci_plasmoid_backend/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 arguments = vars(get_parser().parse_args())
 
 logging.basicConfig(format='%(levelname)s %(name)s: %(message)s',
                     level=logging.DEBUG if arguments['debug'] else logging.INFO)
 # supress log message `DEBUG asyncio: Using selector: EpollSelector`
 logging.getLogger('asyncio').setLevel(logging.WARNING)
 logger = logging.getLogger(__name__)
-logger.debug('Run in debug mode')
+logger.debug(f'Running version {version("ddcci-plasmoid-backend")} in debug mode')
 
 
 def handle_error(error: str | subprocess.CalledProcessError) -> NoReturn:
     if isinstance(error, subprocess.CalledProcessError):
-        error = err.stderr.decode() if err.stderr else err.stdout.decode()
+        error = err.stderr if err.stderr else err.stdout
     print(json.dumps({
         'command': arguments['command'],
         'error': error.replace('\n', ' ')
     }))
     sys.exit(1)
 
 
@@ -44,15 +44,19 @@
     # include the username in the lock file. Otherwise, if user A creates a lock, user B may not have the permissions
     # to access the lock file and this program will fail until the lock file is deleted.
     with fasteners.InterProcessLock(Path(tempfile.gettempdir()) / f'ddcci_plasmoid_backend-{os.getlogin()}.lock'):
         if arguments['command'] == 'detect':
             try:
                 result = asyncio.run(ddcci.detect())
             except subprocess.CalledProcessError as err:
+                logger.debug(err)
                 handle_error(err)
+            except Exception as err:
+                logger.debug(err)
+                handle_error('Failed to fetch monitor data')
 
             count = len(result)
             # Remove objects that are errors
             for report in result:
                 if isinstance(report, Exception):
                     logger.debug(report)
                     result.remove(report)
@@ -80,10 +84,11 @@
                     'command': 'set-brightness',
                     'value': {
                         'bus_id': bus_id,
                         'brightness': brightness
                     }
                 }))
             except subprocess.CalledProcessError as err:
+                logger.debug(err)
                 handle_error(err)
 
     sys.exit(0)
```

### Comparing `ddcci_plasmoid_backend-0.1.3/ddcci_plasmoid_backend/ddcci.py` & `ddcci_plasmoid_backend-0.1.4/ddcci_plasmoid_backend/ddcci.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 import logging
 import re
 import subprocess
-from typing import TypedDict
+from typing import TypedDict, Optional
 
 from ddcci_plasmoid_backend.Node import Node
 
 logger = logging.getLogger(__name__)
 brightness_feature_code = 0x10
 
 
@@ -40,15 +40,21 @@
             return False
         return True
 
 
 async def detect():
     async def fetch_monitor_data(node: Node) -> MonitorData:
         display_id = get_monitor_id(node)
-        display_name = get_EDID_value(node, 'Model')
+        display_name = ''
+        if 'EDID synopsis' in node.child_by_key:
+            display_name = get_EDID_value(node, 'Model')
+        # Use generic name if the EDID model is either empty or not present
+        if not display_name:
+            display_name = 'Unknown display'
+
         bus_id = int(re.search(r'\d+$', node.child_by_key['I2C bus'].value).group())
 
         result = await async_subprocess_wrapper(
             f'ddcutil getvcp --bus {bus_id} --brief {brightness_feature_code:x}')
 
         _, _, _, display_brightness_raw, _ = result['stdout'].split(' ')
 
@@ -66,39 +72,47 @@
     found_monitors: list[MonitorID] = []
     awaitables = []
     for child in content.children:
         if not re.fullmatch(r'Display \d+', child.key.strip()):
             logger.debug(
                 f'Key {child.key.strip()} does not match pattern for valid display, so skip it')
             continue
-
-        # monitors connected to DisplayPort may appear twice. This is apparently related to DisplayPort MST.
-        # Since the EDID data of both entries is identical, we simply remove duplicate monitors based on their serial
-        # number
-        monitorId = MonitorID(
-            serial_number=get_EDID_value(child, 'Serial number'),
-            binary_serial_number=get_EDID_value(child, 'Binary serial number')
-        )
-        if monitorId in found_monitors:
-            logger.debug(
-                f'{get_EDID_value(child, "Model")} id={get_monitor_id(child)}: Duplicate monitor found and removed'
+        monitor_id = get_monitor_id(child)
+        if 'EDID synopsis' in child.child_by_key:
+            # monitors connected to DisplayPort may appear twice. This is apparently related to DisplayPort MST.
+            # Since the EDID data of both entries is identical, we simply remove duplicate monitors based on their
+            # serial number
+            monitorId = MonitorID(
+                serial_number=get_EDID_value(child, 'Serial number'),
+                binary_serial_number=get_EDID_value(child, 'Binary serial number')
             )
-            continue
-        found_monitors.append(monitorId)
+            if monitorId in found_monitors:
+                logger.debug(
+                    f'{get_EDID_value(child, "Model")} id={monitor_id}: Duplicate monitor found and removed'
+                )
+                continue
+            found_monitors.append(monitorId)
+        else:
+            # For the unlikely case that no EDID synopsis is included, skip all duplication tests
+            logger.debug(f'id={monitor_id} No EDID synopsis returned')
+
         awaitables.append(fetch_monitor_data(child))
 
     return await asyncio.gather(*awaitables, return_exceptions=True)
 
 
 def set_brightness(bus_id: int, brightness: int) -> None:
     subprocess_wrapper(f'ddcutil setvcp --bus {bus_id} {brightness_feature_code:x} {brightness}')
 
 
-def get_EDID_value(node: Node, value: str) -> str:
-    return node.child_by_key['EDID synopsis'].child_by_key[value].value
+def get_EDID_value(node: Node, value: str) -> Optional[str]:
+    node = node.child_by_key['EDID synopsis'].child_by_key.get(value)
+    if node:
+        return node.value
+    return None
 
 
 def get_monitor_id(node: Node):
     return int(re.search(r'\d+', node.key).group())
 
 
 # Wrap sync and async subprocess calls for mocking
```

### Comparing `ddcci_plasmoid_backend-0.1.3/ddcci_plasmoid_backend/ddcci_test.py` & `ddcci_plasmoid_backend-0.1.4/ddcci_plasmoid_backend/ddcci_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         }
 
     return inner
 
 
 @pytest.mark.parametrize('dir', [
     'simple', 'duplicate', '#1-wrong-duplicates', 'duplicate-binary-serial-numbers', 'duplicate-serial-numbers',
-    'invalid-display-error'
+    'invalid-display-error', 'missing-serial-numbers'
 ])
 async def test_detect(monkeypatch, dir, return_coroutine, return_CommandOutput):
     path = Path('fixtures/detect/') / dir
     with open(path / 'input.txt') as file:
         input_data = file.read()
     with open(path / 'output.json') as file:
         output_data = json.load(file)
```

### Comparing `ddcci_plasmoid_backend-0.1.3/pyproject.toml` & `ddcci_plasmoid_backend-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ddcci-plasmoid-backend"
-version = "0.1.3"
+version = "0.1.4"
 description = "Backend for ddcci-plasmoid"
 authors = ["David Himmelstoß <77309510+davidhi7@users.noreply.github.com>"]
 license = "MIT"
 packages = [{include = "ddcci_plasmoid_backend"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

