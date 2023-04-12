# Comparing `tmp/neetbox-0.1.504.tar.gz` & `tmp/neetbox-0.1.505.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neetbox-0.1.504.tar", max compression
+gzip compressed data, was "neetbox-0.1.505.tar", max compression
```

## Comparing `neetbox-0.1.504.tar` & `neetbox-0.1.505.tar`

### file list

```diff
@@ -1,42 +1,40 @@
--rw-r--r--   0        0        0     1067 2023-04-12 11:13:03.328087 neetbox-0.1.504/LICENSE
--rw-r--r--   0        0        0      397 2023-04-12 11:13:03.328087 neetbox-0.1.504/README.md
--rw-r--r--   0        0        0     2138 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/cli/__init__.py
--rw-r--r--   0        0        0     2594 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/cli/parse.py
--rw-r--r--   0        0        0      601 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/config/__init__.py
--rw-r--r--   0        0        0      184 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/config/_config.py
--rw-r--r--   0        0        0       93 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/config/_default.py
--rw-r--r--   0        0        0       19 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/core/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/core/core.py
--rw-r--r--   0        0        0      418 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/integrations/__init__.py
--rw-r--r--   0        0        0     1073 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/integrations/engine.py
--rw-r--r--   0        0        0     6754 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/integrations/environment.py
--rw-r--r--   0        0        0     8229 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/integrations/resource.py
--rw-r--r--   0        0        0       36 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/integrations/tensorboard.py
--rw-r--r--   0        0        0      301 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/logging/__init__.py
--rw-r--r--   0        0        0     2106 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/logging/_colorama.py
--rw-r--r--   0        0        0        0 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/logging/_default.py
--rw-r--r--   0        0        0    12181 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/logging/flfs/ansiregular.flf
--rw-r--r--   0        0        0    12181 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/logging/flfs/ansishadow.flf
--rw-r--r--   0        0        0    11585 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/logging/flfs/isometrixc2.flf
--rw-r--r--   0        0        0    23112 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/logging/flfs/nscripts.flf
--rw-r--r--   0        0        0    21669 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/logging/flfs/nvscript.flf
--rw-r--r--   0        0        0     3921 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/logging/formatting.py
--rw-r--r--   0        0        0    18566 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/logging/logger.py
--rw-r--r--   0        0        0       54 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/pipeline/__init__.py
--rw-r--r--   0        0        0      171 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/pipeline/pipe.py
--rw-r--r--   0        0        0     5485 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/pipeline/registry.py
--rw-r--r--   0        0        0        0 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/plotting/__init__.py
--rw-r--r--   0        0        0     4922 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/plotting/plot.py
--rw-r--r--   0        0        0      115 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/torch/__init__.py
--rw-r--r--   0        0        0     5227 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/torch/arch/canny.py
--rw-r--r--   0        0        0     6437 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/torch/arch/cnn.py
--rw-r--r--   0        0        0     2319 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/torch/arch/kernels.py
--rw-r--r--   0        0        0     2440 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/torch/arch/mask_boundary_finder.py
--rw-r--r--   0        0        0     3678 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/torch/nlp.py
--rw-r--r--   0        0        0     4481 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/torch/profile.py
--rw-r--r--   0        0        0        0 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/utils/__init__.py
--rw-r--r--   0        0        0     2303 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/utils/framing.py
--rw-r--r--   0        0        0     2018 2023-04-12 11:13:03.336088 neetbox-0.1.504/neetbox/utils/utils.py
--rw-r--r--   0        0        0     1245 2023-04-12 11:13:03.336088 neetbox-0.1.504/pyproject.toml
--rw-r--r--   0        0        0     1788 1970-01-01 00:00:00.000000 neetbox-0.1.504/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-12 12:16:59.917266 neetbox-0.1.505/LICENSE
+-rw-r--r--   0        0        0      397 2023-04-12 12:16:59.917266 neetbox-0.1.505/README.md
+-rw-r--r--   0        0        0     2138 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/cli/__init__.py
+-rw-r--r--   0        0        0     2594 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/cli/parse.py
+-rw-r--r--   0        0        0      549 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/config/__init__.py
+-rw-r--r--   0        0        0      907 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/config/_config.py
+-rw-r--r--   0        0        0       19 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/core/core.py
+-rw-r--r--   0        0        0      418 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/integrations/__init__.py
+-rw-r--r--   0        0        0     1073 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/integrations/engine.py
+-rw-r--r--   0        0        0     6754 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/integrations/environment.py
+-rw-r--r--   0        0        0     8229 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/integrations/resource.py
+-rw-r--r--   0        0        0      301 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/logging/__init__.py
+-rw-r--r--   0        0        0     2106 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/logging/_colorama.py
+-rw-r--r--   0        0        0        0 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/logging/_default.py
+-rw-r--r--   0        0        0    12181 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/logging/flfs/ansiregular.flf
+-rw-r--r--   0        0        0    12181 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/logging/flfs/ansishadow.flf
+-rw-r--r--   0        0        0    11585 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/logging/flfs/isometrixc2.flf
+-rw-r--r--   0        0        0    23112 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/logging/flfs/nscripts.flf
+-rw-r--r--   0        0        0    21669 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/logging/flfs/nvscript.flf
+-rw-r--r--   0        0        0     3921 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/logging/formatting.py
+-rw-r--r--   0        0        0    18657 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/logging/logger.py
+-rw-r--r--   0        0        0       54 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/pipeline/__init__.py
+-rw-r--r--   0        0        0      171 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/pipeline/pipe.py
+-rw-r--r--   0        0        0     5485 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/pipeline/registry.py
+-rw-r--r--   0        0        0        0 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/plotting/__init__.py
+-rw-r--r--   0        0        0     4922 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/plotting/plot.py
+-rw-r--r--   0        0        0      115 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/torch/__init__.py
+-rw-r--r--   0        0        0     5227 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/torch/arch/canny.py
+-rw-r--r--   0        0        0     6437 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/torch/arch/cnn.py
+-rw-r--r--   0        0        0     2319 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/torch/arch/kernels.py
+-rw-r--r--   0        0        0     2440 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/torch/arch/mask_boundary_finder.py
+-rw-r--r--   0        0        0     3678 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/torch/nlp.py
+-rw-r--r--   0        0        0     4481 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/torch/profile.py
+-rw-r--r--   0        0        0        0 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/utils/__init__.py
+-rw-r--r--   0        0        0     2303 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/utils/framing.py
+-rw-r--r--   0        0        0     2018 2023-04-12 12:16:59.925266 neetbox-0.1.505/neetbox/utils/utils.py
+-rw-r--r--   0        0        0     1245 2023-04-12 12:16:59.925266 neetbox-0.1.505/pyproject.toml
+-rw-r--r--   0        0        0     1788 1970-01-01 00:00:00.000000 neetbox-0.1.505/PKG-INFO
```

### Comparing `neetbox-0.1.504/LICENSE` & `neetbox-0.1.505/LICENSE`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.504/neetbox/__init__.py` & `neetbox-0.1.505/neetbox/__init__.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.504/neetbox/cli/parse.py` & `neetbox-0.1.505/neetbox/cli/parse.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.504/neetbox/config/__init__.py` & `neetbox-0.1.505/neetbox/config/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-from neetbox.config._default import DEFAULT_CONFIG as default
-from neetbox.config._config import _update as update
-
-update(default)
+from neetbox.config._config import _update as update, DEFAULT_CONFIG as default
 from neetbox.config._config import _get
 from neetbox.utils.framing import *
 
 
 def get_module_config():
     module_name = get_frame_module_traceback(traceback=2).__name__
     the_config = _get()
```

### Comparing `neetbox-0.1.504/neetbox/integrations/engine.py` & `neetbox-0.1.505/neetbox/integrations/engine.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.504/neetbox/integrations/environment.py` & `neetbox-0.1.505/neetbox/integrations/environment.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.504/neetbox/integrations/resource.py` & `neetbox-0.1.505/neetbox/integrations/resource.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.504/neetbox/logging/_colorama.py` & `neetbox-0.1.505/neetbox/logging/_colorama.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.504/neetbox/logging/flfs/ansiregular.flf` & `neetbox-0.1.505/neetbox/logging/flfs/ansiregular.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.504/neetbox/logging/flfs/ansishadow.flf` & `neetbox-0.1.505/neetbox/logging/flfs/ansishadow.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.504/neetbox/logging/flfs/isometrixc2.flf` & `neetbox-0.1.505/neetbox/logging/flfs/isometrixc2.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.504/neetbox/logging/flfs/nscripts.flf` & `neetbox-0.1.505/neetbox/logging/flfs/nscripts.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.504/neetbox/logging/flfs/nvscript.flf` & `neetbox-0.1.505/neetbox/logging/flfs/nvscript.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.504/neetbox/logging/formatting.py` & `neetbox-0.1.505/neetbox/logging/formatting.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.504/neetbox/logging/logger.py` & `neetbox-0.1.505/neetbox/logging/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 # Date:   20230315
 
 import os
 import io
 import re
 from datetime import date, datetime
 from enum import Enum
-from pyfiglet import Figlet, FigletFont
 from neetbox.utils.framing import *
-from neetbox.config import get_module_config
+from pyfiglet import Figlet, FigletFont
 from neetbox.utils import utils
 from neetbox.logging.formatting import *
 from inspect import isclass, iscoroutinefunction, isgeneratorfunction
 import functools
 import pathlib
 from random import randint
 from typing import *
 
+
 class LogLevel(Enum):
     ALL = 4
     INFO = 3
     DEBUG = 2
     WARNING = 1
     ERROR = 0
 
@@ -451,30 +451,30 @@
                             return function(*args, **kwargs)
 
                 functools.update_wrapper(catch_wrapper, function)
                 return catch_wrapper
 
         return Catcher(False)
 
-    def banner(self, text, font: Optional[str] = None):
+    def banner(self, text, font: Optional[str] = None):        
         builtin_font_list = [
-                "ansiregular",
-                "ansishadow",
-                "isometrixc2",
-                "nscripts",
-                "nvscript",
-            ]
+            "ansiregular",
+            "ansishadow",
+            "isometrixc2",
+            "nscripts",
+            "nvscript",
+        ]
         if not font:
             font = builtin_font_list[randint(0, len(builtin_font_list)) - 1]
-            
+
         if font not in FigletFont.getFonts():
-            if font in builtin_font_list: # builtin but not installed
+            if font in builtin_font_list:  # builtin but not installed
                 module_path = os.path.dirname(__file__)
                 FigletFont.installFonts(f"{module_path}/flfs/{font}.flf")
-            else: # path?
+            else:  # path?
                 assert os.path.isfile(
                 font
                 ), "The provided font is not a fontname or a font file path."
                 file_name = os.path.basename(font)
                 file = os.path.splitext(file_name)
                 if (
                     file[0] not in FigletFont.getFonts()
@@ -514,14 +514,17 @@
         self.log(context, with_datetime=False, with_identifier=False)
         return self
 
     def set_log_dir(self, path, independent=False):
         if not path:
             self._bind_file(None)
             return self
+        if not path:
+            self._bind_file(None)
+            return self
         if os.path.isfile(path):
             raise "Target path is not a directory."
         if not os.path.exists(path):
             DEFAULT_LOGGER.info(f"Directory {path} not found, trying to create.")
             try:
                 os.makedirs(path)
             except:
@@ -534,14 +537,17 @@
         self._bind_file(os.path.join(path, log_file_name))
         return self
 
     def _bind_file(self, path):
         if not path:
             self.file_writer = None
             return self
+        if not path:
+            self.file_writer = None
+            return self
         log_file_identity = os.path.abspath(path)
         if os.path.isdir(log_file_identity):
             raise Exception("Target path is not a file.")
         filename = utils.legal_file_name_of(os.path.basename(path))
         dirname = os.path.dirname(path) if len(os.path.dirname(path)) != 0 else "."
         if not os.path.exists(dirname):
             raise Exception(f"Could not find dictionary {dirname}")
@@ -554,8 +560,8 @@
         self.file_writer = writers_dict[log_file_identity]
         return self
 
     def file_bend(self) -> bool:
         return self.file_writer != None
 
 
-DEFAULT_LOGGER = Logger(None)
+DEFAULT_LOGGER = Logger(None)
```

### Comparing `neetbox-0.1.504/neetbox/pipeline/registry.py` & `neetbox-0.1.505/neetbox/pipeline/registry.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.504/neetbox/plotting/plot.py` & `neetbox-0.1.505/neetbox/plotting/plot.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.504/neetbox/torch/arch/canny.py` & `neetbox-0.1.505/neetbox/torch/arch/canny.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.504/neetbox/torch/arch/cnn.py` & `neetbox-0.1.505/neetbox/torch/arch/cnn.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.504/neetbox/torch/arch/kernels.py` & `neetbox-0.1.505/neetbox/torch/arch/kernels.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.504/neetbox/torch/arch/mask_boundary_finder.py` & `neetbox-0.1.505/neetbox/torch/arch/mask_boundary_finder.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.504/neetbox/torch/nlp.py` & `neetbox-0.1.505/neetbox/torch/nlp.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.504/neetbox/torch/profile.py` & `neetbox-0.1.505/neetbox/torch/profile.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.504/neetbox/utils/framing.py` & `neetbox-0.1.505/neetbox/utils/framing.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.504/neetbox/utils/utils.py` & `neetbox-0.1.505/neetbox/utils/utils.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.504/pyproject.toml` & `neetbox-0.1.505/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neetbox"
-version = "0.1.504"
+version = "0.1.505"
 description = "NEETBox contains useless CV code snippets."
 license = "MIT"
 authors = ["VisualDust <gavin@gong.host>"]
 maintainers = [
     "VisualDust <gavin@gong.host>",
     "PommesPeter <me@pommespeter.space>",
     "PaperCube <imzhy@hotmail.com>"
```

### Comparing `neetbox-0.1.504/PKG-INFO` & `neetbox-0.1.505/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neetbox
-Version: 0.1.504
+Version: 0.1.505
 Summary: NEETBox contains useless CV code snippets.
 Home-page: https://neetbox.550w.host
 License: MIT
 Keywords: computer vision,tools,logging
 Author: VisualDust
 Author-email: gavin@gong.host
 Maintainer: VisualDust
```

