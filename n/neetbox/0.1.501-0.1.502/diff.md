# Comparing `tmp/neetbox-0.1.501.tar.gz` & `tmp/neetbox-0.1.502.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neetbox-0.1.501.tar", max compression
+gzip compressed data, was "neetbox-0.1.502.tar", max compression
```

## Comparing `neetbox-0.1.501.tar` & `neetbox-0.1.502.tar`

### file list

```diff
@@ -1,31 +1,37 @@
--rw-r--r--   0        0        0      397 2023-04-08 10:22:09.657826 neetbox-0.1.501/README.md
--rw-r--r--   0        0        0        0 2023-04-08 10:22:09.665826 neetbox-0.1.501/neetbox/__init__.py
--rw-r--r--   0        0        0       19 2023-04-08 10:22:09.665826 neetbox-0.1.501/neetbox/core/__init__.py
--rw-r--r--   0        0        0        0 2023-04-08 10:22:09.665826 neetbox-0.1.501/neetbox/core/core.py
--rw-r--r--   0        0        0      418 2023-04-08 10:22:09.665826 neetbox-0.1.501/neetbox/integrations/__init__.py
--rw-r--r--   0        0        0     1073 2023-04-08 10:22:09.665826 neetbox-0.1.501/neetbox/integrations/engine.py
--rw-r--r--   0        0        0     6752 2023-04-08 10:22:09.665826 neetbox-0.1.501/neetbox/integrations/environment.py
--rw-r--r--   0        0        0     8046 2023-04-08 10:22:09.665826 neetbox-0.1.501/neetbox/integrations/resource.py
--rw-r--r--   0        0        0      255 2023-04-08 10:22:09.665826 neetbox-0.1.501/neetbox/logging/__init__.py
--rw-r--r--   0        0        0     2106 2023-04-08 10:22:09.665826 neetbox-0.1.501/neetbox/logging/_colorama.py
--rw-r--r--   0        0        0        0 2023-04-08 10:22:09.665826 neetbox-0.1.501/neetbox/logging/_default.py
--rw-r--r--   0        0        0     3921 2023-04-08 10:22:09.665826 neetbox-0.1.501/neetbox/logging/formatting.py
--rw-r--r--   0        0        0    17105 2023-04-08 10:22:09.665826 neetbox-0.1.501/neetbox/logging/logger.py
--rw-r--r--   0        0        0       54 2023-04-08 10:22:09.665826 neetbox-0.1.501/neetbox/pipeline/__init__.py
--rw-r--r--   0        0        0      171 2023-04-08 10:22:09.665826 neetbox-0.1.501/neetbox/pipeline/pipe.py
--rw-r--r--   0        0        0     4754 2023-04-08 10:22:09.665826 neetbox-0.1.501/neetbox/pipeline/registry.py
--rw-r--r--   0        0        0       72 2023-04-08 10:22:09.665826 neetbox-0.1.501/neetbox/pipeline/runner.py
--rw-r--r--   0        0        0        0 2023-04-08 10:22:09.665826 neetbox-0.1.501/neetbox/plotting/__init__.py
--rw-r--r--   0        0        0     4922 2023-04-08 10:22:09.665826 neetbox-0.1.501/neetbox/plotting/plot.py
--rw-r--r--   0        0        0      115 2023-04-08 10:22:09.665826 neetbox-0.1.501/neetbox/torch/__init__.py
--rw-r--r--   0        0        0     5227 2023-04-08 10:22:09.665826 neetbox-0.1.501/neetbox/torch/arch/canny.py
--rw-r--r--   0        0        0     6437 2023-04-08 10:22:09.665826 neetbox-0.1.501/neetbox/torch/arch/cnn.py
--rw-r--r--   0        0        0     2319 2023-04-08 10:22:09.665826 neetbox-0.1.501/neetbox/torch/arch/kernels.py
--rw-r--r--   0        0        0     2440 2023-04-08 10:22:09.665826 neetbox-0.1.501/neetbox/torch/arch/mask_boundary_finder.py
--rw-r--r--   0        0        0     3122 2023-04-08 10:22:09.665826 neetbox-0.1.501/neetbox/torch/nlp.py
--rw-r--r--   0        0        0     4517 2023-04-08 10:22:09.665826 neetbox-0.1.501/neetbox/torch/profile.py
--rw-r--r--   0        0        0        0 2023-04-08 10:22:09.665826 neetbox-0.1.501/neetbox/utils/__init__.py
--rw-r--r--   0        0        0     2303 2023-04-08 10:22:09.665826 neetbox-0.1.501/neetbox/utils/framing.py
--rw-r--r--   0        0        0     1420 2023-04-08 10:22:09.665826 neetbox-0.1.501/neetbox/utils/utils.py
--rw-r--r--   0        0        0     1140 2023-04-08 10:22:09.665826 neetbox-0.1.501/pyproject.toml
--rw-r--r--   0        0        0     1784 1970-01-01 00:00:00.000000 neetbox-0.1.501/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-12 10:11:53.226734 neetbox-0.1.502/LICENSE
+-rw-r--r--   0        0        0      397 2023-04-12 10:11:53.226734 neetbox-0.1.502/README.md
+-rw-r--r--   0        0        0     2092 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/cli/__init__.py
+-rw-r--r--   0        0        0     2594 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/cli/parse.py
+-rw-r--r--   0        0        0      601 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/config/__init__.py
+-rw-r--r--   0        0        0      184 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/config/_config.py
+-rw-r--r--   0        0        0       96 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/config/_default.py
+-rw-r--r--   0        0        0       19 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/core/core.py
+-rw-r--r--   0        0        0      418 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/integrations/__init__.py
+-rw-r--r--   0        0        0     1073 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/integrations/engine.py
+-rw-r--r--   0        0        0     6754 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/integrations/environment.py
+-rw-r--r--   0        0        0     8229 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/integrations/resource.py
+-rw-r--r--   0        0        0       36 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/integrations/tensorboard.py
+-rw-r--r--   0        0        0      301 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/logging/__init__.py
+-rw-r--r--   0        0        0     2106 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/logging/_colorama.py
+-rw-r--r--   0        0        0        0 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/logging/_default.py
+-rw-r--r--   0        0        0     3921 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/logging/formatting.py
+-rw-r--r--   0        0        0    18340 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/logging/logger.py
+-rw-r--r--   0        0        0       54 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/pipeline/__init__.py
+-rw-r--r--   0        0        0      171 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/pipeline/pipe.py
+-rw-r--r--   0        0        0     5485 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/pipeline/registry.py
+-rw-r--r--   0        0        0        0 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/plotting/__init__.py
+-rw-r--r--   0        0        0     4922 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/plotting/plot.py
+-rw-r--r--   0        0        0      115 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/torch/__init__.py
+-rw-r--r--   0        0        0     5227 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/torch/arch/canny.py
+-rw-r--r--   0        0        0     6437 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/torch/arch/cnn.py
+-rw-r--r--   0        0        0     2319 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/torch/arch/kernels.py
+-rw-r--r--   0        0        0     2440 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/torch/arch/mask_boundary_finder.py
+-rw-r--r--   0        0        0     3678 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/torch/nlp.py
+-rw-r--r--   0        0        0     4481 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/torch/profile.py
+-rw-r--r--   0        0        0        0 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/utils/__init__.py
+-rw-r--r--   0        0        0     2303 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/utils/framing.py
+-rw-r--r--   0        0        0     2018 2023-04-12 10:11:53.234734 neetbox-0.1.502/neetbox/utils/utils.py
+-rw-r--r--   0        0        0     1245 2023-04-12 10:11:53.234734 neetbox-0.1.502/pyproject.toml
+-rw-r--r--   0        0        0     1788 1970-01-01 00:00:00.000000 neetbox-0.1.502/PKG-INFO
```

### Comparing `neetbox-0.1.501/neetbox/integrations/engine.py` & `neetbox-0.1.502/neetbox/integrations/engine.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.501/neetbox/integrations/environment.py` & `neetbox-0.1.502/neetbox/integrations/environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
                 else:
                     logger.warn(f"{package} is not going to be installed")
                     break
             else:  # illegal input
                 retry -= 1
                 if retry:
                     logger.err(
-                        f"illegal input: required 'y'/'n' but recieved {choice}. {retry} retries remaining."
+                        f"illegal input: required 'y'/'n' but recieved '{choice}'. {retry} retries remaining."
                     )
         return _installed
 
     def is_installed(self, package: str, try_install_if_not: Union[str, bool] = True):
         caller = get_caller_identity_traceback(2)
         caller_name = caller.module_name if caller.module else caller.filename
         if not self.installed_packages:
```

### Comparing `neetbox-0.1.501/neetbox/integrations/resource.py` & `neetbox-0.1.502/neetbox/integrations/resource.py`

 * *Files 5% similar despite different names*

```diff
@@ -203,17 +203,18 @@
     logger.log(f"Downloading {len(urls)} file(s)...")
 
     if verbose:
         outer_pbar = tqdm(total=len(urls), desc=f"Overall process")
 
     _reporthook = None
     _results = []
-    for fname, furl in urls.items():
+    for fname, furl in tqdm(urls.items()):
         if fname and os.path.isfile(fname):
             if not overwrite:
+                _results.append((fname,None))
                 logger.log(
                     f"File {fname} already exists. If you want to redownload it, try to pass 'overwrite=True'"
                 )
                 continue
         if verbose:
             inner_pbar = tqdm(total=100, leave=False, desc=f"Currently downloading")
 
@@ -233,8 +234,13 @@
                 _results.append(res)
                 break
             except:
                 retry -= 1
                 logger.err(f"Download interrupt. {retry} retry(s) remaining.")
                 if not retry:
                     raise RuntimeError(f"Download failed after retries")
-    return [fname for fname, reqmsg in _results]
+    results = [fname for fname, reqmsg in _results]
+    if not len(results):
+        results = None
+    if len(results) == 1:
+        results = results[0]
+    return results
```

### Comparing `neetbox-0.1.501/neetbox/logging/_colorama.py` & `neetbox-0.1.502/neetbox/logging/_colorama.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.501/neetbox/logging/formatting.py` & `neetbox-0.1.502/neetbox/logging/formatting.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.501/neetbox/logging/logger.py` & `neetbox-0.1.502/neetbox/logging/logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,23 +5,25 @@
 # Date:   20230315
 
 import os
 import io
 import re
 from datetime import date, datetime
 from enum import Enum
+from pyfiglet import Figlet, FigletFont
 from neetbox.utils.framing import *
+from neetbox.config import get_module_config
 from neetbox.utils import utils
 from neetbox.logging.formatting import *
 from inspect import isclass, iscoroutinefunction, isgeneratorfunction
 import functools
 import pathlib
+from random import randint
 from typing import *
 
-
 class LogLevel(Enum):
     ALL = 4
     INFO = 3
     DEBUG = 2
     WARNING = 1
     ERROR = 0
 
@@ -51,14 +53,15 @@
 _global_log_level = LogLevel.ALL
 
 
 def set_log_level(level: LogLevel):
     if type(level) is int:
         assert level >= 0 and level <= 3
         level = LogLevel(level)
+    global _global_log_level
     _global_log_level = level
 
 
 class LogMetadata:
     def __init__(self, writer: "_AutoSplitLogWriter"):
         self.written_bytes = 0
         self.log_writer = writer
@@ -413,15 +416,15 @@
                 from_decorator = self._from_decorator
                 catch_options = [(type_, value, traceback_)]
                 if handler:
                     handler(traceback_)
                 # logger.log(
                 #     from_decorator, catch_options, traceback=4 if from_decorator else 3
                 # )
-                #todo add reraise functions
+                # todo add reraise functions
                 return not reraise
 
             def __call__(self, function):
                 if isclass(function):
                     raise TypeError(
                         "Invalid object decorated with 'catch()', it must be a function, "
                         "not a class (tried to wrap '%s')" % function.__name__
@@ -448,14 +451,51 @@
                             return function(*args, **kwargs)
 
                 functools.update_wrapper(catch_wrapper, function)
                 return catch_wrapper
 
         return Catcher(False)
 
+    def banner(self, text, font: Optional[str] = None):
+        builtin_font_list = [
+                "ansiregular",
+                "ansishadow",
+                "isometrixc2",
+                "nscripts",
+                "nvscript",
+            ]
+        if not font:
+            font = builtin_font_list[randint(0, len(builtin_font_list)) - 1]
+            
+        if font not in FigletFont.getFonts():
+            if font in builtin_font_list: # builtin but not installed
+                FigletFont.installFonts(f"res/flfs/{font}.flf")
+            else: # path?
+                assert os.path.isfile(
+                font
+                ), "The provided font is not a fontname or a font file path."
+                file_name = os.path.basename(font)
+                file = os.path.splitext(file_name)
+                if (
+                    file[0] not in FigletFont.getFonts()
+                ):  # no installed file match the file name
+                    try:
+                        self.info(
+                            f"{file[0]} is not installed. Trying to install as a fontfile."
+                        )
+                        FigletFont.installFonts(f"res/flfs/{font}.flf")
+                    except:
+                        self.err("Could not install font {font}. Fallback to default.")
+                        font = None
+                else:
+                    font = file[0]
+        f = Figlet(font)
+        self.log(f.renderText(text), with_datetime=False, with_identifier=False)
+        return self
+
     def skip_lines(self, line_cnt=1):
         """Let the logger log some empty lines
 
         Args:
             line_cnt (int, optional): how many empty line. Defaults to 1.
 
         Returns:
@@ -507,21 +547,8 @@
         self.file_writer = writers_dict[log_file_identity]
         return self
 
     def file_bend(self) -> bool:
         return self.file_writer != None
 
 
-DEFAULT_LOGGER = Logger(None)
-
-
-# todo remove dedicated
-def get_logger(whom: any = None, style: LogStyle = None) -> Logger:
-    DEFAULT_LOGGER.warn(
-        "'get_logger(whom)' is outdated and will be removed in the near future. Use 'logger(whom)' instead."
-    )
-    if whom is None:
-        return DEFAULT_LOGGER
-    if whom in loggers_dict:
-        return loggers_dict[whom]
-    loggers_dict[whom] = Logger(whom=whom, style=style)
-    return loggers_dict[whom]
+DEFAULT_LOGGER = Logger(None)
```

### Comparing `neetbox-0.1.501/neetbox/pipeline/registry.py` & `neetbox-0.1.502/neetbox/pipeline/registry.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,142 +1,171 @@
 from neetbox.logging import logger
-from neetbox.utils import utils
+from neetbox.utils.utils import *
 from typing import Optional, Union, Sequence
 import inspect
 import json
 import functools
 from typing import Any, Callable, Dict, List, Optional, Sequence, Union
 
-_registry_pool: Dict[str, "Registry"] = dict()  # all registeres are stored here
 
 class Registry(dict):
     """Register Helper Class
     A Register is a 'dict[str:any]'
     Registers are stored in a pool of type dict[str:Register]
     """
 
-    def __new__(cls, name: str, filter_strs: any = None) -> "Registry":
-        assert utils.is_pure_ansi(
-            name
-        ), "Registry name should not contain non-ansi char."
-        if name in _registry_pool:
-            return _registry_pool[name]
+    # class level
+    _registry_pool: Dict[str, "Registry"] = dict()  # all registeres are stored here
+
+    # instance level
+    initialized: bool = False
+
+    def __new__(cls, name: str) -> "Registry":
+        assert is_pure_ansi(name), "Registry name should not contain non-ansi char."
+        if name in cls._registry_pool:
+            return cls._registry_pool[name]
+        logger.log(f"Creating Registry for {cls}")
         instance = dict.__new__(cls)
-        _registry_pool[name] = instance
+        cls._registry_pool[name] = instance
         return instance
 
     # not compatible with python below 3.8
-    def __init__(
-        self, name: str, *, filter_strs: Optional[Union[str, Sequence[str]]] = None
-    ) -> None:
-        super().__init__()
-        self.name = name
-        if filter_strs:
-            self.filter_strs = (
-                [filter_strs] if isinstance(filter_strs, str) else filter_strs
-            )
-            self.filter_strs = dict()
+    def __init__(self, name: str) -> None:
+        if not self.initialized:
+            # do initializations
+            self.name = name
+            self.initialized = True
 
     def _register(
         self,
-        what: any,
-        force: bool = False,
+        what: Any,
         name: Optional[str] = None,
-        **filter_strs,
+        force: bool = False,
+        tags: Optional[Union[str, Sequence[str]]] = None,
     ):
         if not (inspect.isfunction(what) or inspect.isclass(what)):
             logger.warn("Registering {type(what)}, which is not a class or a callable.")
         name = name or what.__name__
-        if not force and name in self.keys():
-            raise ValueError(f"{name} already exists in Registry:{self.name}")
-
-        if filter_strs:
-            if not hasattr(self, "filter_strs"):
-                raise ValueError(
-                    "Registry `{}` does not have `filter_strs`.".format(self.name)
+        if type(tags) is str:
+            tags = [tags]
+        if name in self.keys():
+            if not force:
+                logger.warn(
+                    f"{name} already exists in Registry:{self.name}. If you want to overwrite, try to register with 'force=True'"
                 )
-            for k in filter_strs.keys():
-                if k not in self.filter_strs:
-                    raise ValueError(
-                        "Registry `{}`: 'filter_strs' does not has expected key {}.".format(
-                            self.name, k
-                        )
-                    )
-            self.filter_strs[name] = [
-                filter_strs.get(k, None) for k in self.filter_strs
-            ]
-        elif hasattr(self, "filter_strs"):
-            self.filter_strs[name] = [None] * len(self.filter_strs)
-
-        self[name] = what
+            else:
+                logger.warn(f"Overwritting: {name} existed in Registry:{self.name}.")
+                self[name] = (what, tags)
+        else:
+            self[name] = (what, tags)
         return what
 
     def register(
-        self, force: bool = False, name: Optional[str] = None, **filter_strs
+        self,
+        *,
+        name: Optional[str] = None,
+        force: bool = False,
+        tags: Optional[Union[str, Sequence[str]]] = None,
     ) -> Callable:
-        return functools.partial(self._register, force=force, name=name, **filter_strs)
+        return functools.partial(
+            self._register, name=name, force=force, tags=tags
+        )
 
     def register_all(
         self,
-        modules: Sequence[Callable],
+        what: Union[Dict, Sequence[Callable]],
         names: Optional[Sequence[str]] = None,
-        filter_strs: Optional[Sequence[Dict[str, Any]]] = None,
+        tags: Optional[Union[str, Sequence[str]]] = None,
         force: bool = False,
     ) -> None:
-        _names = names if names else [None] * len(modules)
-        _info = filter_strs if filter_strs else [{}] * len(modules)
-        for module, name, info in zip(modules, _names, _info):
-            self._register(module, force=force, name=name, **info)
+        if type(what) is dict:
+            _names = what.keys()
+            what = what.values()
+        if type(what) is list:
+            _names = names if names else [None] * len(what)
+            for module, name, info in zip(what, _names, tags):
+                self._register(module, force=force, name=name, tags=tags)
+        else:
+            logger.err(
+                ValueError(
+                    f"Unsupported format of 'what'. Please use list or dict(tuple)."
+                ),
+                reraise=True,
+            )
 
     def merge(
         self,
         others: Union["Registry", List["Registry"]],
         force: bool = False,
     ) -> None:
         if not isinstance(others, list):
             others = [others]
         if not isinstance(others[0], Registry):
-            raise TypeError(
-                "Expect `Registry` type, but got {}".format(type(others[0]))
+            logger.err(
+                TypeError("Expect `Registry` type, but got {}".format(type(others[0]))),
+                reraise=True,
             )
         for other in others:
-            modules = list(other.values())
-            names = list(other.keys())
-            self.register_all(modules, force=force, names=names)
-            
-            
-    @classmethod
-    def get_all_registries():
-        return _registry_pool
-    
+            self.register_all(other, force=force)
+
     @classmethod
-    def _find_global_with_name(name:str, default = None):
-        for reg_name, reg in _registry_pool.values():
-            private_sign = '__'
+    def find(
+        cls,
+        name: Optional[str] = None,
+        tags: Optional[Union[str, List[str]]] = None,
+        default=None,
+    ):
+        if not name and not tags:
+            logger.err(
+                ValueError(
+                    "Please provide at least the name or the tags you want to find."
+                ),
+                reraise=True,
+            )
+        results = []
+        # filter name
+        for reg_name, reg in cls._registry_pool.items():
+            private_sign = "__"
             if not reg_name.startswith(private_sign):
-                if name in reg:
-                    return reg[name]
-        return default
-    
-    @classmethod
-    def _find_global_with_filter_strs(fileters:List[str]):
-        pass
+                if not name:
+                    results += [(_n, _o) for _n, _o in reg.items()]
+                elif name in reg:
+                    results.append((name, reg[name]))
+
+        # filter tags
+        if type(tags) is str:
+            tags = [tags]
+
+        def _tags_match(f_tags, s_tags) -> bool:
+            # check if all tags in f_tags are listed in s_tags
+            for _t in f_tags:
+                if _t not in s_tags:
+                    return False
+            return True
+
+        results = {
+            _name: obj_tag_pair[0]
+            for _name, obj_tag_pair in results
+            if _tags_match(tags, obj_tag_pair[1])
+        }
+        return results
 
     def __getitem__(self, __key: str) -> Any:
-        return super().__getitem__(__key)
+        return super().__getitem__(__key)[0]
 
     def __setitem__(self, k, v) -> None:
-        assert utils.is_pure_ansi(
-            k
-        ), "Only ANSI chars are allowed for registering things."
+        assert is_pure_ansi(k), "Only ANSI chars are allowed for registering things."
+        if type(v) is not tuple:
+            v = (v, None)
+        if len(v) != 2:
+            raise ValueError("Only support value of format (object, list(str))")
         super().__setitem__(k, v)
 
     def __str__(self) -> str:
-        s = json.dumps(
+        return json.dumps(
             self,
             indent=4,
             ensure_ascii=False,
             sort_keys=False,
             separators=(",", ":"),
             default=str,
         )
-        return s
```

### Comparing `neetbox-0.1.501/neetbox/plotting/plot.py` & `neetbox-0.1.502/neetbox/plotting/plot.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.501/neetbox/torch/arch/canny.py` & `neetbox-0.1.502/neetbox/torch/arch/canny.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.501/neetbox/torch/arch/cnn.py` & `neetbox-0.1.502/neetbox/torch/arch/cnn.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.501/neetbox/torch/arch/kernels.py` & `neetbox-0.1.502/neetbox/torch/arch/kernels.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.501/neetbox/torch/arch/mask_boundary_finder.py` & `neetbox-0.1.502/neetbox/torch/arch/mask_boundary_finder.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.501/neetbox/torch/profile.py` & `neetbox-0.1.502/neetbox/torch/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 # Date:   20230315
 
 from neetbox.integrations import pkg
 import time
 from tqdm import tqdm
 import torch
 
-from neetbox.logging import get_logger
-
-logger = get_logger("NEETBOX")
+from neetbox.logging import logger
 
 
 def profile(
     model,
     input_shape=(1, 3, 1280, 720),
     specific_input=None,
     profiling=True,
```

### Comparing `neetbox-0.1.501/neetbox/utils/framing.py` & `neetbox-0.1.502/neetbox/utils/framing.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.501/pyproject.toml` & `neetbox-0.1.502/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 [tool.poetry]
 name = "neetbox"
-version = "0.1.501"
+version = "0.1.502"
 description = "NEETBox contains useless CV code snippets."
 license = "MIT"
-authors = [
-    "VisualDust <gavin@gong.host>",
-]
+authors = ["VisualDust <gavin@gong.host>"]
 maintainers = [
     "VisualDust <gavin@gong.host>",
     "PommesPeter <me@pommespeter.space>",
+    "PaperCube <imzhy@hotmail.com>"
 ]
 
 
 readme = "README.md"
 homepage = "https://neetbox.550w.host"
 repository = "https://github.com/visualDust/neetbox"
 keywords = ["computer vision", "tools", "logging"]
@@ -20,15 +19,15 @@
     "Development Status :: 1 - Planning",
     "Environment :: Console",
     "Framework :: Matplotlib",
     "Programming Language :: Python",
     "Topic :: Scientific/Engineering :: Visualization",
     "Topic :: Software Development :: Testing",
     "Topic :: System :: Logging",
-    "Topic :: Utilities"
+    "Topic :: Utilities",
 ]
 
 # [[tool.poetry.source]]
 # name = "pypi"
 # url = "https://pypi.org/simple"
 # default = true
 
@@ -37,14 +36,18 @@
 numpy = ">=1"
 pillow = ">=8"
 pandas = ">=1"
 tqdm = ">=4"
 colorama = ">=0.3"
 toml = ">0.10"
 pytest = "*"
-gputil = "^1.4.0"
-psutil = "^5.9.4"
-injector = "^0.20.1"
+gputil = ">=1.4"
+psutil = ">=5.0"
+injector = ">=0.20"
+pyfiglet = ">=0.8"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
+
+[tool.poetry.scripts]
+neetbox = 'neetbox.cli.parse:parse'
```

### Comparing `neetbox-0.1.501/PKG-INFO` & `neetbox-0.1.502/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neetbox
-Version: 0.1.501
+Version: 0.1.502
 Summary: NEETBox contains useless CV code snippets.
 Home-page: https://neetbox.550w.host
 License: MIT
 Keywords: computer vision,tools,logging
 Author: VisualDust
 Author-email: gavin@gong.host
 Maintainer: VisualDust
@@ -21,20 +21,21 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: System :: Logging
 Classifier: Topic :: Utilities
 Requires-Dist: colorama (>=0.3)
-Requires-Dist: gputil (>=1.4.0,<2.0.0)
-Requires-Dist: injector (>=0.20.1,<0.21.0)
+Requires-Dist: gputil (>=1.4)
+Requires-Dist: injector (>=0.20)
 Requires-Dist: numpy (>=1)
 Requires-Dist: pandas (>=1)
 Requires-Dist: pillow (>=8)
-Requires-Dist: psutil (>=5.9.4,<6.0.0)
+Requires-Dist: psutil (>=5.0)
+Requires-Dist: pyfiglet (>=0.8)
 Requires-Dist: pytest
 Requires-Dist: toml (>0.10)
 Requires-Dist: tqdm (>=4)
 Project-URL: Repository, https://github.com/visualDust/neetbox
 Description-Content-Type: text/markdown
 
 # NEETBox contains use~~ful~~less tiny deeplearning code snippets
```

