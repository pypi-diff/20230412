# Comparing `tmp/neetbox-0.1.502.tar.gz` & `tmp/neetbox-0.1.503.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neetbox-0.1.502.tar", max compression
+gzip compressed data, was "neetbox-0.1.503.tar", max compression
```

## Comparing `neetbox-0.1.502.tar` & `neetbox-0.1.503.tar`

### file list

```diff
@@ -1,37 +1,42 @@
--rw-r--r--   0        0        0     1067 2023-04-12 10:11:53.226734 neetbox-0.1.502/LICENSE
--rw-r--r--   0        0        0      397 2023-04-12 10:11:53.226734 neetbox-0.1.502/README.md
--rw-r--r--   0        0        0     2092 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/cli/__init__.py
--rw-r--r--   0        0        0     2594 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/cli/parse.py
--rw-r--r--   0        0        0      601 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/config/__init__.py
--rw-r--r--   0        0        0      184 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/config/_config.py
--rw-r--r--   0        0        0       96 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/config/_default.py
--rw-r--r--   0        0        0       19 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/core/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/core/core.py
--rw-r--r--   0        0        0      418 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/integrations/__init__.py
--rw-r--r--   0        0        0     1073 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/integrations/engine.py
--rw-r--r--   0        0        0     6754 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/integrations/environment.py
--rw-r--r--   0        0        0     8229 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/integrations/resource.py
--rw-r--r--   0        0        0       36 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/integrations/tensorboard.py
--rw-r--r--   0        0        0      301 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/logging/__init__.py
--rw-r--r--   0        0        0     2106 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/logging/_colorama.py
--rw-r--r--   0        0        0        0 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/logging/_default.py
--rw-r--r--   0        0        0     3921 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/logging/formatting.py
--rw-r--r--   0        0        0    18340 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/logging/logger.py
--rw-r--r--   0        0        0       54 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/pipeline/__init__.py
--rw-r--r--   0        0        0      171 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/pipeline/pipe.py
--rw-r--r--   0        0        0     5485 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/pipeline/registry.py
--rw-r--r--   0        0        0        0 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/plotting/__init__.py
--rw-r--r--   0        0        0     4922 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/plotting/plot.py
--rw-r--r--   0        0        0      115 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/torch/__init__.py
--rw-r--r--   0        0        0     5227 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/torch/arch/canny.py
--rw-r--r--   0        0        0     6437 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/torch/arch/cnn.py
--rw-r--r--   0        0        0     2319 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/torch/arch/kernels.py
--rw-r--r--   0        0        0     2440 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/torch/arch/mask_boundary_finder.py
--rw-r--r--   0        0        0     3678 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/torch/nlp.py
--rw-r--r--   0        0        0     4481 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/torch/profile.py
--rw-r--r--   0        0        0        0 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/utils/__init__.py
--rw-r--r--   0        0        0     2303 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/utils/framing.py
--rw-r--r--   0        0        0     2018 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/utils/utils.py
--rw-r--r--   0        0        0     1245 2023-04-12 10:11:53.234734 neetbox-0.1.502/pyproject.toml
--rw-r--r--   0        0        0     1788 1970-01-01 00:00:00.000000 neetbox-0.1.502/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-12 10:44:53.249547 neetbox-0.1.503/LICENSE
+-rw-r--r--   0        0        0      397 2023-04-12 10:44:53.249547 neetbox-0.1.503/README.md
+-rw-r--r--   0        0        0     2092 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/cli/__init__.py
+-rw-r--r--   0        0        0     2594 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/cli/parse.py
+-rw-r--r--   0        0        0      601 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/config/__init__.py
+-rw-r--r--   0        0        0      184 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/config/_config.py
+-rw-r--r--   0        0        0       93 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/config/_default.py
+-rw-r--r--   0        0        0       19 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/core/core.py
+-rw-r--r--   0        0        0      418 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/integrations/__init__.py
+-rw-r--r--   0        0        0     1073 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/integrations/engine.py
+-rw-r--r--   0        0        0     6754 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/integrations/environment.py
+-rw-r--r--   0        0        0     8229 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/integrations/resource.py
+-rw-r--r--   0        0        0       36 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/integrations/tensorboard.py
+-rw-r--r--   0        0        0      301 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/logging/__init__.py
+-rw-r--r--   0        0        0     2106 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/logging/_colorama.py
+-rw-r--r--   0        0        0        0 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/logging/_default.py
+-rw-r--r--   0        0        0    12181 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/logging/flfs/ansiregular.flf
+-rw-r--r--   0        0        0    12181 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/logging/flfs/ansishadow.flf
+-rw-r--r--   0        0        0    11585 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/logging/flfs/isometrixc2.flf
+-rw-r--r--   0        0        0    23112 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/logging/flfs/nscripts.flf
+-rw-r--r--   0        0        0    21669 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/logging/flfs/nvscript.flf
+-rw-r--r--   0        0        0     3921 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/logging/formatting.py
+-rw-r--r--   0        0        0    18566 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/logging/logger.py
+-rw-r--r--   0        0        0       54 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/pipeline/__init__.py
+-rw-r--r--   0        0        0      171 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/pipeline/pipe.py
+-rw-r--r--   0        0        0     5485 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/pipeline/registry.py
+-rw-r--r--   0        0        0        0 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/plotting/__init__.py
+-rw-r--r--   0        0        0     4922 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/plotting/plot.py
+-rw-r--r--   0        0        0      115 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/torch/__init__.py
+-rw-r--r--   0        0        0     5227 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/torch/arch/canny.py
+-rw-r--r--   0        0        0     6437 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/torch/arch/cnn.py
+-rw-r--r--   0        0        0     2319 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/torch/arch/kernels.py
+-rw-r--r--   0        0        0     2440 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/torch/arch/mask_boundary_finder.py
+-rw-r--r--   0        0        0     3678 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/torch/nlp.py
+-rw-r--r--   0        0        0     4481 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/torch/profile.py
+-rw-r--r--   0        0        0        0 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/utils/__init__.py
+-rw-r--r--   0        0        0     2303 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/utils/framing.py
+-rw-r--r--   0        0        0     2018 2023-04-12 10:44:53.257548 neetbox-0.1.503/neetbox/utils/utils.py
+-rw-r--r--   0        0        0     1245 2023-04-12 10:44:53.257548 neetbox-0.1.503/pyproject.toml
+-rw-r--r--   0        0        0     1788 1970-01-01 00:00:00.000000 neetbox-0.1.503/PKG-INFO
```

### Comparing `neetbox-0.1.502/LICENSE` & `neetbox-0.1.503/LICENSE`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.502/neetbox/__init__.py` & `neetbox-0.1.503/neetbox/__init__.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.502/neetbox/cli/parse.py` & `neetbox-0.1.503/neetbox/cli/parse.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.502/neetbox/config/__init__.py` & `neetbox-0.1.503/neetbox/config/__init__.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.502/neetbox/integrations/engine.py` & `neetbox-0.1.503/neetbox/integrations/engine.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.502/neetbox/integrations/environment.py` & `neetbox-0.1.503/neetbox/integrations/environment.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.502/neetbox/integrations/resource.py` & `neetbox-0.1.503/neetbox/integrations/resource.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.502/neetbox/logging/_colorama.py` & `neetbox-0.1.503/neetbox/logging/_colorama.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.502/neetbox/logging/formatting.py` & `neetbox-0.1.503/neetbox/logging/formatting.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.502/neetbox/logging/logger.py` & `neetbox-0.1.503/neetbox/logging/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -464,15 +464,16 @@
                 "nvscript",
             ]
         if not font:
             font = builtin_font_list[randint(0, len(builtin_font_list)) - 1]
             
         if font not in FigletFont.getFonts():
             if font in builtin_font_list: # builtin but not installed
-                FigletFont.installFonts(f"res/flfs/{font}.flf")
+                module_path = os.path.dirname(__file__)
+                FigletFont.installFonts(f"{module_path}/flfs/{font}.flf")
             else: # path?
                 assert os.path.isfile(
                 font
                 ), "The provided font is not a fontname or a font file path."
                 file_name = os.path.basename(font)
                 file = os.path.splitext(file_name)
                 if (
@@ -510,14 +511,17 @@
         context = ""
         for line in file.readlines():
             context += line
         self.log(context, with_datetime=False, with_identifier=False)
         return self
 
     def set_log_dir(self, path, independent=False):
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
@@ -527,14 +531,17 @@
         if independent:
             log_file_name += self.whom
         log_file_name += str(date.today()) + ".log"
         self._bind_file(os.path.join(path, log_file_name))
         return self
 
     def _bind_file(self, path):
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
```

### Comparing `neetbox-0.1.502/neetbox/pipeline/registry.py` & `neetbox-0.1.503/neetbox/pipeline/registry.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.502/neetbox/plotting/plot.py` & `neetbox-0.1.503/neetbox/plotting/plot.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.502/neetbox/torch/arch/canny.py` & `neetbox-0.1.503/neetbox/torch/arch/canny.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.502/neetbox/torch/arch/cnn.py` & `neetbox-0.1.503/neetbox/torch/arch/cnn.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.502/neetbox/torch/arch/kernels.py` & `neetbox-0.1.503/neetbox/torch/arch/kernels.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.502/neetbox/torch/arch/mask_boundary_finder.py` & `neetbox-0.1.503/neetbox/torch/arch/mask_boundary_finder.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.502/neetbox/torch/nlp.py` & `neetbox-0.1.503/neetbox/torch/nlp.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.502/neetbox/torch/profile.py` & `neetbox-0.1.503/neetbox/torch/profile.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.502/neetbox/utils/framing.py` & `neetbox-0.1.503/neetbox/utils/framing.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.502/neetbox/utils/utils.py` & `neetbox-0.1.503/neetbox/utils/utils.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.502/pyproject.toml` & `neetbox-0.1.503/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neetbox"
-version = "0.1.502"
+version = "0.1.503"
 description = "NEETBox contains useless CV code snippets."
 license = "MIT"
 authors = ["VisualDust <gavin@gong.host>"]
 maintainers = [
     "VisualDust <gavin@gong.host>",
     "PommesPeter <me@pommespeter.space>",
     "PaperCube <imzhy@hotmail.com>"
```

### Comparing `neetbox-0.1.502/PKG-INFO` & `neetbox-0.1.503/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neetbox
-Version: 0.1.502
+Version: 0.1.503
 Summary: NEETBox contains useless CV code snippets.
 Home-page: https://neetbox.550w.host
 License: MIT
 Keywords: computer vision,tools,logging
 Author: VisualDust
 Author-email: gavin@gong.host
 Maintainer: VisualDust
```

