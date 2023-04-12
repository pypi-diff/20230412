# Comparing `tmp/neetbox-0.1.503.tar.gz` & `tmp/neetbox-0.1.504.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neetbox-0.1.503.tar", max compression
+gzip compressed data, was "neetbox-0.1.504.tar", max compression
```

## Comparing `neetbox-0.1.503.tar` & `neetbox-0.1.504.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1067 2023-04-12 10:44:53.249547 neetbox-0.1.503/LICENSE
--rw-r--r--   0        0        0      397 2023-04-12 10:44:53.249547 neetbox-0.1.503/README.md
--rw-r--r--   0        0        0     2092 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/cli/__init__.py
--rw-r--r--   0        0        0     2594 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/cli/parse.py
--rw-r--r--   0        0        0      601 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/config/__init__.py
--rw-r--r--   0        0        0      184 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/config/_config.py
--rw-r--r--   0        0        0       93 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/config/_default.py
--rw-r--r--   0        0        0       19 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/core/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/core/core.py
--rw-r--r--   0        0        0      418 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/integrations/__init__.py
--rw-r--r--   0        0        0     1073 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/integrations/engine.py
--rw-r--r--   0        0        0     6754 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/integrations/environment.py
--rw-r--r--   0        0        0     8229 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/integrations/resource.py
--rw-r--r--   0        0        0       36 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/integrations/tensorboard.py
--rw-r--r--   0        0        0      301 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/logging/__init__.py
--rw-r--r--   0        0        0     2106 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/logging/_colorama.py
--rw-r--r--   0        0        0        0 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/logging/_default.py
--rw-r--r--   0        0        0    12181 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/logging/flfs/ansiregular.flf
--rw-r--r--   0        0        0    12181 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/logging/flfs/ansishadow.flf
--rw-r--r--   0        0        0    11585 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/logging/flfs/isometrixc2.flf
--rw-r--r--   0        0        0    23112 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/logging/flfs/nscripts.flf
--rw-r--r--   0        0        0    21669 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/logging/flfs/nvscript.flf
--rw-r--r--   0        0        0     3921 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/logging/formatting.py
--rw-r--r--   0        0        0    18566 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/logging/logger.py
--rw-r--r--   0        0        0       54 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/pipeline/__init__.py
--rw-r--r--   0        0        0      171 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/pipeline/pipe.py
--rw-r--r--   0        0        0     5485 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/pipeline/registry.py
--rw-r--r--   0        0        0        0 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/plotting/__init__.py
--rw-r--r--   0        0        0     4922 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/plotting/plot.py
--rw-r--r--   0        0        0      115 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/torch/__init__.py
--rw-r--r--   0        0        0     5227 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/torch/arch/canny.py
--rw-r--r--   0        0        0     6437 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/torch/arch/cnn.py
--rw-r--r--   0        0        0     2319 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/torch/arch/kernels.py
--rw-r--r--   0        0        0     2440 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/torch/arch/mask_boundary_finder.py
--rw-r--r--   0        0        0     3678 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/torch/nlp.py
--rw-r--r--   0        0        0     4481 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/torch/profile.py
--rw-r--r--   0        0        0        0 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/utils/__init__.py
--rw-r--r--   0        0        0     2303 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/utils/framing.py
--rw-r--r--   0        0        0     2018 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/utils/utils.py
--rw-r--r--   0        0        0     1245 2023-04-12 10:44:53.257548 neetbox-0.1.503/pyproject.toml
--rw-r--r--   0        0        0     1788 1970-01-01 00:00:00.000000 neetbox-0.1.503/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-12 11:13:03.328087 neetbox-0.1.504/LICENSE
+-rw-r--r--   0        0        0      397 2023-04-12 11:13:03.328087 neetbox-0.1.504/README.md
+-rw-r--r--   0        0        0     2138 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/cli/__init__.py
+-rw-r--r--   0        0        0     2594 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/cli/parse.py
+-rw-r--r--   0        0        0      601 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/config/__init__.py
+-rw-r--r--   0        0        0      184 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/config/_config.py
+-rw-r--r--   0        0        0       93 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/config/_default.py
+-rw-r--r--   0        0        0       19 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/core/core.py
+-rw-r--r--   0        0        0      418 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/integrations/__init__.py
+-rw-r--r--   0        0        0     1073 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/integrations/engine.py
+-rw-r--r--   0        0        0     6754 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/integrations/environment.py
+-rw-r--r--   0        0        0     8229 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/integrations/resource.py
+-rw-r--r--   0        0        0       36 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/integrations/tensorboard.py
+-rw-r--r--   0        0        0      301 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/logging/__init__.py
+-rw-r--r--   0        0        0     2106 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/logging/_colorama.py
+-rw-r--r--   0        0        0        0 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/logging/_default.py
+-rw-r--r--   0        0        0    12181 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/logging/flfs/ansiregular.flf
+-rw-r--r--   0        0        0    12181 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/logging/flfs/ansishadow.flf
+-rw-r--r--   0        0        0    11585 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/logging/flfs/isometrixc2.flf
+-rw-r--r--   0        0        0    23112 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/logging/flfs/nscripts.flf
+-rw-r--r--   0        0        0    21669 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/logging/flfs/nvscript.flf
+-rw-r--r--   0        0        0     3921 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/logging/formatting.py
+-rw-r--r--   0        0        0    18566 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/logging/logger.py
+-rw-r--r--   0        0        0       54 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/pipeline/__init__.py
+-rw-r--r--   0        0        0      171 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/pipeline/pipe.py
+-rw-r--r--   0        0        0     5485 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/pipeline/registry.py
+-rw-r--r--   0        0        0        0 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/plotting/__init__.py
+-rw-r--r--   0        0        0     4922 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/plotting/plot.py
+-rw-r--r--   0        0        0      115 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/torch/__init__.py
+-rw-r--r--   0        0        0     5227 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/torch/arch/canny.py
+-rw-r--r--   0        0        0     6437 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/torch/arch/cnn.py
+-rw-r--r--   0        0        0     2319 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/torch/arch/kernels.py
+-rw-r--r--   0        0        0     2440 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/torch/arch/mask_boundary_finder.py
+-rw-r--r--   0        0        0     3678 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/torch/nlp.py
+-rw-r--r--   0        0        0     4481 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/torch/profile.py
+-rw-r--r--   0        0        0        0 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/utils/__init__.py
+-rw-r--r--   0        0        0     2303 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/utils/framing.py
+-rw-r--r--   0        0        0     2018 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/utils/utils.py
+-rw-r--r--   0        0        0     1245 2023-04-12 11:13:03.336088 neetbox-0.1.504/pyproject.toml
+-rw-r--r--   0        0        0     1788 1970-01-01 00:00:00.000000 neetbox-0.1.504/PKG-INFO
```

### Comparing `neetbox-0.1.503/LICENSE` & `neetbox-0.1.504/LICENSE`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.503/neetbox/__init__.py` & `neetbox-0.1.504/neetbox/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,58 @@
 import os
 import toml
 from neetbox.config import default
-from neetbox.logging.logger import Logger
 from neetbox.config._config import _update
 from neetbox.utils.framing import get_frame_module_traceback
 
 module_name = get_frame_module_traceback(1).__name__
 config_file_name = f"{module_name}.toml"
-logger = Logger("NEETBOX")  # builtin standalone logger
 
-def init(path=None, load_only=False):
+
+def init(path=None, load=False) -> bool:
     if path:
         os.chdir(path=path)
     current_path = os.getcwd()
     config_file_path = os.path.join(current_path, config_file_name)
-    _fallback_flag = False
-    
-    if not load_only:
+
+    if not load:
+        from neetbox.logging.logger import Logger
+
+        logger = Logger("NEETBOX")  # builtin standalone logger
         if not os.path.isfile(config_file_path):  # config file not exist
             try:  # creating config file using default config
                 with open(config_file_path, "w+") as cfgf:
                     toml.dump(default, cfgf)
                 logger.ok(f"Workspace config created as {config_file_path}.")
+                return True
             except Exception as e:
                 logger.err(f"Failed to create {config_file_path}: {e}")
-                _fallback_flag = True
-        else: # config file exist:
-            logger.err(f"Config file already exists.")
-            raise RuntimeError(f"Config file already exists.")
-    else: # load only. trying to load from not existing file
+                return False
+        else:  # config file exist:
+            logger.err((f"Config file already exists."))
+            return False
+    else:  # load only. trying to load from not existing file
         if not os.path.isfile(config_file_path):  # config file not exist
+            from neetbox.logging.logger import Logger
+
+            logger = Logger("NEETBOX")  # builtin standalone logger
             logger.err(f"Config file {config_file_path} not exists.")
-            _fallback_flag = True
+            return False
+
+    try:
+        load_config = toml.load(config_file_path)
+        _update(load_config)
+        from neetbox.logging.logger import Logger
+
+        logger = Logger("NEETBOX")  # builtin standalone logger
+        logger.ok(f"Loaded workspace config from {config_file_path}.")
+        return True
+    except Exception as e:
+        from neetbox.logging.logger import Logger
+
+        logger = Logger("NEETBOX")  # builtin standalone logger
+        logger.err(f"Failed to load config from {config_file_path}: {e}")
+        return False
 
-    if not _fallback_flag:  # if file exist
-        try:
-            load_config = toml.load(config_file_path)
-            _update(load_config)
-            logger.ok(f"Loaded workspace config from {config_file_path}.")
-        except Exception as e:
-            logger.err(f"Failed to load config from {config_file_path}: {e}")
-            _fallback_flag = True
-
-    if _fallback_flag:  # something wrong, using default config
-        raise RuntimeError(
-            f"Failed to parse config file '{config_file_path}'. Check permissions and file format."
-        )
 
 if os.path.isfile(config_file_name):  # if in a workspace
-    init(load_only=True)
+    init(load=True)
```

### Comparing `neetbox-0.1.503/neetbox/cli/parse.py` & `neetbox-0.1.504/neetbox/cli/parse.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.503/neetbox/config/__init__.py` & `neetbox-0.1.504/neetbox/config/__init__.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.503/neetbox/integrations/engine.py` & `neetbox-0.1.504/neetbox/integrations/engine.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.503/neetbox/integrations/environment.py` & `neetbox-0.1.504/neetbox/integrations/environment.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.503/neetbox/integrations/resource.py` & `neetbox-0.1.504/neetbox/integrations/resource.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.503/neetbox/logging/_colorama.py` & `neetbox-0.1.504/neetbox/logging/_colorama.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.503/neetbox/logging/flfs/ansiregular.flf` & `neetbox-0.1.504/neetbox/logging/flfs/ansiregular.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.503/neetbox/logging/flfs/ansishadow.flf` & `neetbox-0.1.504/neetbox/logging/flfs/ansishadow.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.503/neetbox/logging/flfs/isometrixc2.flf` & `neetbox-0.1.504/neetbox/logging/flfs/isometrixc2.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.503/neetbox/logging/flfs/nscripts.flf` & `neetbox-0.1.504/neetbox/logging/flfs/nscripts.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.503/neetbox/logging/flfs/nvscript.flf` & `neetbox-0.1.504/neetbox/logging/flfs/nvscript.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.503/neetbox/logging/formatting.py` & `neetbox-0.1.504/neetbox/logging/formatting.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.503/neetbox/logging/logger.py` & `neetbox-0.1.504/neetbox/logging/logger.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.503/neetbox/pipeline/registry.py` & `neetbox-0.1.504/neetbox/pipeline/registry.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.503/neetbox/plotting/plot.py` & `neetbox-0.1.504/neetbox/plotting/plot.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.503/neetbox/torch/arch/canny.py` & `neetbox-0.1.504/neetbox/torch/arch/canny.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.503/neetbox/torch/arch/cnn.py` & `neetbox-0.1.504/neetbox/torch/arch/cnn.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.503/neetbox/torch/arch/kernels.py` & `neetbox-0.1.504/neetbox/torch/arch/kernels.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.503/neetbox/torch/arch/mask_boundary_finder.py` & `neetbox-0.1.504/neetbox/torch/arch/mask_boundary_finder.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.503/neetbox/torch/nlp.py` & `neetbox-0.1.504/neetbox/torch/nlp.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.503/neetbox/torch/profile.py` & `neetbox-0.1.504/neetbox/torch/profile.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.503/neetbox/utils/framing.py` & `neetbox-0.1.504/neetbox/utils/framing.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.503/neetbox/utils/utils.py` & `neetbox-0.1.504/neetbox/utils/utils.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.503/pyproject.toml` & `neetbox-0.1.504/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neetbox"
-version = "0.1.503"
+version = "0.1.504"
 description = "NEETBox contains useless CV code snippets."
 license = "MIT"
 authors = ["VisualDust <gavin@gong.host>"]
 maintainers = [
     "VisualDust <gavin@gong.host>",
     "PommesPeter <me@pommespeter.space>",
     "PaperCube <imzhy@hotmail.com>"
```

### Comparing `neetbox-0.1.503/PKG-INFO` & `neetbox-0.1.504/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neetbox
-Version: 0.1.503
+Version: 0.1.504
 Summary: NEETBox contains useless CV code snippets.
 Home-page: https://neetbox.550w.host
 License: MIT
 Keywords: computer vision,tools,logging
 Author: VisualDust
 Author-email: gavin@gong.host
 Maintainer: VisualDust
```

