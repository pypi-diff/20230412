# Comparing `tmp/cavcalc-1.0.0.tar.gz` & `tmp/cavcalc-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cavcalc-1.0.0.tar", max compression
+gzip compressed data, was "cavcalc-1.1.0.tar", max compression
```

## Comparing `cavcalc-1.0.0.tar` & `cavcalc-1.1.0.tar`

### file list

```diff
@@ -1,34 +1,33 @@
--rw-r--r--   0        0        0    35129 2023-01-13 18:27:13.156578 cavcalc-1.0.0/LICENSE
--rw-r--r--   0        0        0    12302 2023-01-13 18:27:13.156578 cavcalc-1.0.0/README.md
--rw-r--r--   0        0        0     1711 2023-01-13 18:27:13.163579 cavcalc-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3921 2023-01-13 18:27:13.164579 cavcalc-1.0.0/src/cavcalc/__init__.py
--rw-r--r--   0        0        0      409 2023-01-13 18:27:13.164579 cavcalc-1.0.0/src/cavcalc/__main__.py
--rw-r--r--   0        0        0      168 2023-01-13 18:27:13.164579 cavcalc-1.0.0/src/cavcalc/__version__.py
--rw-r--r--   0        0        0        0 2023-01-13 18:27:13.164579 cavcalc-1.0.0/src/cavcalc/_arguments/__init__.py
--rw-r--r--   0        0        0     9420 2023-01-13 18:27:13.165579 cavcalc-1.0.0/src/cavcalc/_arguments/_container.py
--rw-r--r--   0        0        0     5348 2023-01-13 18:27:13.165579 cavcalc-1.0.0/src/cavcalc/_arguments/_groups.py
--rw-r--r--   0        0        0     3960 2023-01-13 18:27:13.165579 cavcalc-1.0.0/src/cavcalc/_arguments/_types.py
--rw-r--r--   0        0        0      748 2023-01-13 18:27:13.165579 cavcalc-1.0.0/src/cavcalc/_default.mplstyle
--rw-r--r--   0        0        0      403 2023-01-13 18:27:13.165579 cavcalc-1.0.0/src/cavcalc/_exiters.py
--rw-r--r--   0        0        0    10537 2023-01-13 18:27:13.165579 cavcalc-1.0.0/src/cavcalc/_handler.py
--rw-r--r--   0        0        0     3230 2023-01-13 18:27:13.165579 cavcalc-1.0.0/src/cavcalc/_main.py
--rw-r--r--   0        0        0     1462 2023-01-13 18:27:13.165579 cavcalc-1.0.0/src/cavcalc/_session.py
--rw-r--r--   0        0        0     8138 2023-01-13 18:27:13.165579 cavcalc-1.0.0/src/cavcalc/calculate.py
--rw-r--r--   0        0        0     1536 2023-01-13 18:27:13.165579 cavcalc-1.0.0/src/cavcalc/cavcalc.ini
--rw-r--r--   0        0        0     3844 2023-01-13 18:27:13.165579 cavcalc-1.0.0/src/cavcalc/env.py
--rw-r--r--   0        0        0      256 2023-01-13 18:27:13.165579 cavcalc-1.0.0/src/cavcalc/errors.py
--rw-r--r--   0        0        0      709 2023-01-13 18:27:13.165579 cavcalc-1.0.0/src/cavcalc/functions/__init__.py
--rw-r--r--   0        0        0     4957 2023-01-13 18:27:13.165579 cavcalc-1.0.0/src/cavcalc/functions/_maps.py
--rw-r--r--   0        0        0     1105 2023-01-13 18:27:13.165579 cavcalc-1.0.0/src/cavcalc/functions/_utils.py
--rw-r--r--   0        0        0     6560 2023-01-13 18:27:13.165579 cavcalc-1.0.0/src/cavcalc/functions/asymmetric.py
--rw-r--r--   0        0        0     3549 2023-01-13 18:27:13.165579 cavcalc-1.0.0/src/cavcalc/functions/resonance.py
--rw-r--r--   0        0        0     5961 2023-01-13 18:27:13.166579 cavcalc-1.0.0/src/cavcalc/functions/symmetric.py
--rw-r--r--   0        0        0    22848 2023-01-13 18:27:13.166579 cavcalc-1.0.0/src/cavcalc/output.py
--rw-r--r--   0        0        0      443 2023-01-13 18:27:13.166579 cavcalc-1.0.0/src/cavcalc/parameters/__init__.py
--rw-r--r--   0        0        0     5330 2023-01-13 18:27:13.166579 cavcalc-1.0.0/src/cavcalc/parameters/_maps.py
--rw-r--r--   0        0        0     1126 2023-01-13 18:27:13.166579 cavcalc-1.0.0/src/cavcalc/parameters/enums.py
--rw-r--r--   0        0        0     6339 2023-01-13 18:27:13.166579 cavcalc-1.0.0/src/cavcalc/parameters/parameter.py
--rw-r--r--   0        0        0     2072 2023-01-13 18:27:13.166579 cavcalc-1.0.0/src/cavcalc/parameters/tools.py
--rw-r--r--   0        0        0       78 2023-01-13 18:27:13.166579 cavcalc-1.0.0/src/cavcalc/testing.py
--rw-r--r--   0        0        0    13790 1970-01-01 00:00:00.000000 cavcalc-1.0.0/setup.py
--rw-r--r--   0        0        0    13591 1970-01-01 00:00:00.000000 cavcalc-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35129 2023-04-12 16:38:17.667410 cavcalc-1.1.0/LICENSE
+-rw-r--r--   0        0        0    12397 2023-04-12 16:38:17.667410 cavcalc-1.1.0/README.md
+-rw-r--r--   0        0        0     1782 2023-04-12 16:38:17.676410 cavcalc-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3921 2023-04-12 16:38:17.677410 cavcalc-1.1.0/src/cavcalc/__init__.py
+-rw-r--r--   0        0        0      409 2023-04-12 16:38:17.677410 cavcalc-1.1.0/src/cavcalc/__main__.py
+-rw-r--r--   0        0        0      168 2023-04-12 16:38:17.677410 cavcalc-1.1.0/src/cavcalc/__version__.py
+-rw-r--r--   0        0        0        0 2023-04-12 16:38:17.677410 cavcalc-1.1.0/src/cavcalc/_arguments/__init__.py
+-rw-r--r--   0        0        0     9474 2023-04-12 16:38:17.677410 cavcalc-1.1.0/src/cavcalc/_arguments/_container.py
+-rw-r--r--   0        0        0     5348 2023-04-12 16:38:17.677410 cavcalc-1.1.0/src/cavcalc/_arguments/_groups.py
+-rw-r--r--   0        0        0     3960 2023-04-12 16:38:17.677410 cavcalc-1.1.0/src/cavcalc/_arguments/_types.py
+-rw-r--r--   0        0        0      748 2023-04-12 16:38:17.677410 cavcalc-1.1.0/src/cavcalc/_default.mplstyle
+-rw-r--r--   0        0        0      403 2023-04-12 16:38:17.678410 cavcalc-1.1.0/src/cavcalc/_exiters.py
+-rw-r--r--   0        0        0    10537 2023-04-12 16:38:17.678410 cavcalc-1.1.0/src/cavcalc/_handler.py
+-rw-r--r--   0        0        0     3230 2023-04-12 16:38:17.678410 cavcalc-1.1.0/src/cavcalc/_main.py
+-rw-r--r--   0        0        0     1462 2023-04-12 16:38:17.678410 cavcalc-1.1.0/src/cavcalc/_session.py
+-rw-r--r--   0        0        0     9254 2023-04-12 16:38:17.678410 cavcalc-1.1.0/src/cavcalc/calculate.py
+-rw-r--r--   0        0        0     1536 2023-04-12 16:38:17.678410 cavcalc-1.1.0/src/cavcalc/cavcalc.ini
+-rw-r--r--   0        0        0     3856 2023-04-12 16:38:17.678410 cavcalc-1.1.0/src/cavcalc/env.py
+-rw-r--r--   0        0        0      256 2023-04-12 16:38:17.678410 cavcalc-1.1.0/src/cavcalc/errors.py
+-rw-r--r--   0        0        0      709 2023-04-12 16:38:17.678410 cavcalc-1.1.0/src/cavcalc/functions/__init__.py
+-rw-r--r--   0        0        0     5193 2023-04-12 16:38:17.678410 cavcalc-1.1.0/src/cavcalc/functions/_maps.py
+-rw-r--r--   0        0        0     1105 2023-04-12 16:38:17.678410 cavcalc-1.1.0/src/cavcalc/functions/_utils.py
+-rw-r--r--   0        0        0     7331 2023-04-12 16:38:17.678410 cavcalc-1.1.0/src/cavcalc/functions/asymmetric.py
+-rw-r--r--   0        0        0     3541 2023-04-12 16:38:17.678410 cavcalc-1.1.0/src/cavcalc/functions/resonance.py
+-rw-r--r--   0        0        0     6007 2023-04-12 16:38:17.678410 cavcalc-1.1.0/src/cavcalc/functions/symmetric.py
+-rw-r--r--   0        0        0    22169 2023-04-12 16:38:17.678410 cavcalc-1.1.0/src/cavcalc/output.py
+-rw-r--r--   0        0        0      443 2023-04-12 16:38:17.679411 cavcalc-1.1.0/src/cavcalc/parameters/__init__.py
+-rw-r--r--   0        0        0     5330 2023-04-12 16:38:17.679411 cavcalc-1.1.0/src/cavcalc/parameters/_maps.py
+-rw-r--r--   0        0        0     1126 2023-04-12 16:38:17.679411 cavcalc-1.1.0/src/cavcalc/parameters/enums.py
+-rw-r--r--   0        0        0     6339 2023-04-12 16:38:17.679411 cavcalc-1.1.0/src/cavcalc/parameters/parameter.py
+-rw-r--r--   0        0        0     3839 2023-04-12 16:38:17.679411 cavcalc-1.1.0/src/cavcalc/parameters/tools.py
+-rw-r--r--   0        0        0       78 2023-04-12 16:38:17.679411 cavcalc-1.1.0/src/cavcalc/testing.py
+-rw-r--r--   0        0        0    13686 1970-01-01 00:00:00.000000 cavcalc-1.1.0/PKG-INFO
```

### Comparing `cavcalc-1.0.0/LICENSE` & `cavcalc-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cavcalc-1.0.0/README.md` & `cavcalc-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![](https://gitlab.com/sjrowlinson/cavcalc/raw/master/images/logo_cavcalc.png)
+![](https://gitlab.com/sjrowlinson/cavcalc/raw/master/docs/source/_static/logo.svg)
 
 A command line program and Python module for computing parameters associated with linear, Fabry-Perot optical cavities.
 
 - Find the documentation at: https://cavcalc.readthedocs.io/en/latest/
 - Follow the latest changes: https://gitlab.com/sjrowlinson/cavcalc
 - See the entry on PyPI: https://pypi.org/project/cavcalc/
 
@@ -18,15 +18,15 @@
 ```bash
 cavcalc --version
 ```
 
 if you see something along the lines of
 
 ```
-cavcalc v1.0.0
+cavcalc v1.1.0
 ```
 
 then you should be ready to start using `cavcalc`!
 
 **Note**: As is often recommended with the installation of Python packages (especially those with dependencies
 on packages such as `numpy` and `matplotlib`, as is the case here), you should prefer to install `cavcalc` in
 a suitable virtual environment. See [the official documentation on Python virtual environments](https://docs.python.org/3/tutorial/venv.html)
@@ -127,14 +127,16 @@
 	Radius of beam at waist = 11.950538458990879 mm
 
 	Stability g-factor of cavity = 0.8350925761717987
 	Stability g-factor of first mirror = -1.0682523267838677
 	Stability g-factor of second mirror = -0.7817371937639199
 
 	Round-trip Gouy phase = 312.0813565565169 deg
+
+	Divergence angle = 0.0016237789746943276 deg
 ```
 
 ### Units of output
 
 The default behaviour for the output parameter units is to grab the relevant parameter type option under the `[units]` header
 of the `cavcalc.ini` configuration file. When installing `cavcalc`, this file is written to a new `cavcalc/` directory within
 your config directory (i.e. typically `~/.config/cavcalc/cavcalc.ini` under Unix systems). See the comments in this file for
@@ -254,15 +256,15 @@
 out = cc.calculate(L="4km", Rc1=1934, Rc2=2245)
 
 # Printing the output object results in the same output as
 # you would see when running via the CLI
 print(out)
 ```
 
-results in:
+producing:
 
 ```
 Given:
 	Cavity length = 4 km
 
 	Radius of curvature of first mirror = 1934 m
 	Radius of curvature of second mirror = 2245 m
@@ -280,26 +282,28 @@
 	Radius of beam at waist = 11.950538458990879 mm
 
 	Stability g-factor of cavity = 0.8350925761717987
 	Stability g-factor of first mirror = -1.0682523267838677
 	Stability g-factor of second mirror = -0.7817371937639199
 
 	Round-trip Gouy phase = 312.0813565565169 deg
+
+	Divergence angle = 0.0016237789746943276 deg
 ```
 
 An extra feature of the API is the ability to use the `cavcalc.configure` function for overriding
 default behaviour. For example, in the script below we use this in a context-managed scope to
 temporarily use microns for any beam radius parameters, mm for distances, and GHz for any frequencies:
 
 ```python
 import cavcalc as cc
 
 # Temporarily override units...
 with cc.configure(beamsizes="um", distances="mm", frequencies="GHz"):
-    out = cc.calculate(L="8mm", gouy=121)
+    out = cc.calculate(L=8, gouy=121)
     print(out)
 
 # ... previous state (using loaded config options) will
 # be restored on exit from the with block above
 ```
 
 resulting in:
@@ -322,9 +326,9 @@
 
     Radius of beam at mirrors = 55.79464044247193 µm
     Radius of beam at waist = 48.19739141432035 µm
 
     Stability g-factor of cavity = 0.2424809625449729
     Stability g-factor of both mirrors = 0.4924235601034671
 
-    Divergence angle = 0.4026158371180008 deg
+    Divergence angle = 0.40260921048107506 deg
 ```
```

### Comparing `cavcalc-1.0.0/pyproject.toml` & `cavcalc-1.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cavcalc"
-version = "1.0.0"
+version = "1.1.0"
 description = "A program for computing Fabry-Perot optical cavity parameters."
 authors = ["Samuel Rowlinson <samueljrowlinson@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://cavcalc.readthedocs.io/en/latest/"
 repository = "https://gitlab.com/sjrowlinson/cavcalc"
 documentation = "https://cavcalc.readthedocs.io/en/latest/"
@@ -36,20 +36,23 @@
 pytest = "^7.1.3"
 pytest-cov = "^4.0.0"
 coverage = "^6.5.0"
 pycobertura = "^3.0.0"
 
 [tool.poetry.group.doc.dependencies]
 Sphinx = "^5.2.3"
-sphinx-rtd-theme = "^1.0.0"
-sphinxcontrib-katex = "^0.9.0"
 numpydoc = "^1.5.0"
 reslate = "^0.56.0"
 jupyter-sphinx = "^0.4.0"
 tabulate = "^0.9.0"
+pydata-sphinx-theme = "^0.13.2"
+sphinx_design = "^0.3.0"
+sphinx-copybutton = "^0.5.1"
+pandas = "^2.0.0"
+sphinx-favicon = "^1.0.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.10.0"
 pre-commit = "^2.20.0"
 
 [tool.black]
 line-length = 100
```

### Comparing `cavcalc-1.0.0/src/cavcalc/__init__.py` & `cavcalc-1.1.0/src/cavcalc/__init__.py`

 * *Files identical despite different names*

### Comparing `cavcalc-1.0.0/src/cavcalc/_arguments/_container.py` & `cavcalc-1.1.0/src/cavcalc/_arguments/_container.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+from typing import Any, Union
 import warnings
 
 from .. import Q_
 from .._exiters import quit_print
 from ..parameters import ArgParameter, ParameterType
 
 
@@ -21,15 +22,15 @@
     def is_all_target(self) -> bool:
         return self["compute"] == "all"
 
     @property
     def is_single_target(self) -> bool:
         return not self.is_all_target
 
-    def __getitem__(self, argname: str):
+    def __getitem__(self, argname: str) -> Union[ArgParameter, Any]:
         return getattr(self, argname)
 
     def has(self, argname: str) -> bool:
         """Checks that `argname` was specified as one of the arguments, and so
         is held by this namespace-like object."""
         return getattr(self, argname, None) is not None
 
@@ -178,38 +179,38 @@
                 "value for 'g'. Or, to specify a symmetric cavity please use either 'g' or 'gs'; "
                 "g is then gs * gs where gs = g1 = g2."
             )
 
             if has_g1 or has_g2:
                 msg = (
                     "Incorrect usage! Cavity g-factor and individual mirror g-factors "
-                    "cannot be specified simulataneously."
+                    "cannot be specified simultaneously."
                 )
             elif has_gs:
                 msg = (
                     "Incorrect usage! Cavity g-factor and symmetric mirror g-factors "
-                    "cannot be specified simulataneously."
+                    "cannot be specified simultaneously."
                 )
 
             quit_print(msg + "\n\n" + instruct)
 
         # ... and same goes for combinations of RoCs...
         if self.has("Rc") and (self.has("Rc1") or self.has("Rc2")):
             quit_print(
                 "Incorrect usage! Symmetric curvature, 'Rc', and individual (non-symmetric), 'Rc1' and 'Rc2', "
-                "curvatures cannot be specified simulataneously.\n\nTo specify a non-symmetric cavity "
+                "curvatures cannot be specified simultaneously.\n\nTo specify a non-symmetric cavity "
                 "please use both 'Rc1' and 'Rc2', do not give a value for 'Rc'. To specify a symmetric "
                 "cavity please use just 'Rc'."
             )
 
         # ... and beam-sizes
         if self.has("w") and (self.has("w1") or self.has("w2")):
             quit_print(
                 "Incorrect usage! Symmetric beam-size, 'w', and individual (non-symmetric), 'w1' and 'w2', "
-                "beam-sizes cannot be specified simulataneously.\n\nTo specify a non-symmetric cavity "
+                "beam-sizes cannot be specified simultaneously.\n\nTo specify a non-symmetric cavity "
                 "please use both 'w1' and 'w2', do not give a value for 'w'. To specify a symmetric "
                 "cavity please use just 'w'."
             )
         for p in "w", "w1", "w2", "w0":
             if P := self[p]:
                 if np.any(P.value.m < 0):
                     quit_print(f"{p} is invalid. Beam sizes must be non-negative.")
```

### Comparing `cavcalc-1.0.0/src/cavcalc/_arguments/_groups.py` & `cavcalc-1.1.0/src/cavcalc/_arguments/_groups.py`

 * *Files identical despite different names*

### Comparing `cavcalc-1.0.0/src/cavcalc/_arguments/_types.py` & `cavcalc-1.1.0/src/cavcalc/_arguments/_types.py`

 * *Files identical despite different names*

### Comparing `cavcalc-1.0.0/src/cavcalc/_default.mplstyle` & `cavcalc-1.1.0/src/cavcalc/_default.mplstyle`

 * *Files identical despite different names*

### Comparing `cavcalc-1.0.0/src/cavcalc/_handler.py` & `cavcalc-1.1.0/src/cavcalc/_handler.py`

 * *Files identical despite different names*

### Comparing `cavcalc-1.0.0/src/cavcalc/_main.py` & `cavcalc-1.1.0/src/cavcalc/_main.py`

 * *Files identical despite different names*

### Comparing `cavcalc-1.0.0/src/cavcalc/_session.py` & `cavcalc-1.1.0/src/cavcalc/_session.py`

 * *Files identical despite different names*

### Comparing `cavcalc-1.0.0/src/cavcalc/calculate.py` & `cavcalc-1.1.0/src/cavcalc/calculate.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,74 +14,98 @@
 
 def calculate(target=None, meshes=None, **kwargs):
     """Calculates a target parameter from an arbitrary number of physical arguments.
 
     If no `target` is specified then the default behaviour is to calculate all computable
     parameters from the given arguments.
 
-    .. note::
+    .. dropdown:: Valid targets and keyword arguments
+        :icon: info
+        :color: primary
+        :animate: fade-in-slide-down
+
+        You can also refer to the :ref:`param_ref` for a convenient overview of
+        the information below.
 
         .. rubric:: Targets
 
         .. jupyter-execute::
             :hide-code:
 
-            import tabulate
-            import cavcalc.parameters
+            import cavcalc.parameters as ccp
+            import pandas as pd
 
-            headers = ["Target", "Description"]
-            table = [
-                (pname, cavcalc.parameters.TargetParameter(pname).description)
-                for pname in cavcalc.parameters.valid_targets
+            table_styles = [
+                {'selector': "th.col_heading", "props": 'text-align: center'},
+                {"selector": "td", "props": "padding: 10px; text-align: center"},
+                {
+                    "selector": "th",
+                    "props": "padding-left: 60px; padding-right: 60px; background-color: grey; text-align: center"
+                },
+                {"selector": "tr", "props": "border: solid; border-width: 0.5px 0"},
             ]
-            print(tabulate.tabulate(table, headers, tablefmt="fancy_grid"))
+
+            pd.DataFrame(
+                [
+                    (p.name, p.description) for p in sorted(
+                        (ccp.TargetParameter(name) for name in ccp.valid_targets),
+                        key=lambda p: (p.category.value, p.ptype.value)
+                    )
+                ],
+                columns=["Target", "Description"]
+            ).style.hide().set_table_styles(table_styles)
 
         .. rubric:: Keyword arguments
 
         .. jupyter-execute::
             :hide-code:
 
-            headers = ["Argument", "Description"]
-            table = [
-                (pname, cavcalc.parameters.ArgParameter(pname).description)
-                for pname in cavcalc.parameters.valid_arguments
-            ]
-            print(tabulate.tabulate(table, headers, tablefmt="fancy_grid"))
+            pd.DataFrame(
+                [
+                    (p.name, p.description) for p in sorted(
+                        (ccp.ArgParameter(name) for name in ccp.valid_arguments),
+                        key=lambda p: (p.category.value, p.ptype.value)
+                    )
+                ],
+                columns=["Argument", "Description"]
+            ).style.hide().set_table_styles(table_styles)
 
         Each kwarg value can be specified as:
 
         * A single value, or an array of values. The units of this value will correspond to
           those of the associated parameter, or parameter category, in the config file being used.
         * A ``cavcalc.ureg.Quantity`` instance. See the Pint documentation for details on
           instantiating ``Quantity`` objects.
         * Or any value which can be converted into a ``Quantity`` instance; e.g. a string
           (such as ``"10cm"``) or a tuple (such as ``(310, "deg")``).
 
     Parameters
     ----------
-    target : (str | :class:`.ParameterType`), optional
-        The target parameter to compute, can be specified as a string (see note above) or
-        a constant of the enum :class:`.ParameterType`. Defaults to `None` so that the function
+    target : str | :class:`.ParameterType`, optional
+        The target parameter to compute, can be specified as a string (see drop-down box above) or
+        a constant of the enum :class:`.ParameterType`. Defaults to ``None`` so that the function
         computes all the parameters it can from the given inputs.
 
-    meshes : (str | bool | Sequence[str | Sequence[str]]), optional
+    meshes : str | bool | Sequence[str | Sequence[str]], optional
         Parameter combinations from which to construct mesh-grids. This argument can given in
         a number of different ways, e.g:
 
+        * `meshes=True`: constructs mesh-grids from the array-like arguments in the order in which
+          they are given to this function.
         * `meshes="g1,g2"`: makes mesh-grids from arguments `g1` and `g2`, respectively.
         * `meshes=["g1,g2", "R1,R2"]`: makes mesh-grids from `g1` and `g2`, respectively, and also
           makes mesh-grids from `R1` and `R2`, respectively.
         * `meshes=("L, R1, R2")`: makes mesh-grids from `L1`, `R1` and `R2`, respectively.
 
-    **kwargs
-        See the note above for details.
+    **kwargs : Keyword Arguments
+        See the drop-down box above for details.
 
     Returns
     -------
-    out : (:class:`.SingleOutput` | :class:`.MultiOutput`)
+    out : :class:`.SingleOutput` | :class:`.MultiOutput`
         An output object containing the results; with methods for accessing, displaying, and plotting them. If
         a ``target`` was given, and was not ``None``, then this object will be a :class:`.SingleOutput` instance,
         otherwise it will be a :class:`.MultiOutput` object.
 
     Examples
     --------
     The following imports are used for the below examples:
```

### Comparing `cavcalc-1.0.0/src/cavcalc/cavcalc.ini` & `cavcalc-1.1.0/src/cavcalc/cavcalc.ini`

 * *Files identical despite different names*

### Comparing `cavcalc-1.0.0/src/cavcalc/env.py` & `cavcalc-1.1.0/src/cavcalc/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,32 +28,32 @@
 
     This function can be used both regularly, and via context-managed scopes using
     the ``with`` statement. In the latter case, any changes made via these configuration
     options will be reset on exit from the context-managed block.
 
     Parameters
     ----------
-    plt_style : (str | dict | Path | list)
+    plt_style : str | dict | Path | list
         The style-sheet to use, see :func:`matplotlib.pyplot.style.use` for details. Note
         that, in addition to the options specified in the linked matplotlib documentation,
         one can set this to ``"cavcalc"`` to use the default style-sheet that this package
         provides. This argument defaults to ``None``, such that no style modification
         is performed (and matplotlib not imported); this way, the default behaviour of
         this function is to have as minimal impact on the users' development workflow
         as possible.
 
-    **param_units : dict
+    **param_units : Keyword Arguments
         Keyword arguments specifying overrides for the units of any cavcalc parameter or
         parameter category. The names of these correspond exactly to those in the units
         section of a ``cavcalc.ini`` config file.
 
     Examples
     --------
     If you simply want to set-up the plotting style to be the same as the default
-    behaviour when running cavcalc from the command line, then do::
+    style used when running cavcalc from the command line, then do::
 
         import cavcalc as cc
         cc.configure(plt_style="cavcalc")
 
     or, if you only want to use this style-sheet temporarily::
 
         import numpy as np
```

### Comparing `cavcalc-1.0.0/src/cavcalc/functions/__init__.py` & `cavcalc-1.1.0/src/cavcalc/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `cavcalc-1.0.0/src/cavcalc/functions/_maps.py` & `cavcalc-1.1.0/src/cavcalc/functions/_maps.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,14 +117,23 @@
         (ParameterType.CAV_LENGTH, ParameterType.GFACTOR_M1, ParameterType.GFACTOR_M2),
         ParameterType.WAISTPOS,
     ),
     rtgouy_of_g1g2: (
         (ParameterType.GFACTOR_M1, ParameterType.GFACTOR_M2),
         ParameterType.GOUY,
     ),
+    divang_of_g1g2: (
+        (
+            ParameterType.CAV_LENGTH,
+            ParameterType.WAVELENGTH,
+            ParameterType.GFACTOR_M1,
+            ParameterType.GFACTOR_M2,
+        ),
+        ParameterType.DIVERGENCE,
+    ),
     g1_of_Rc1: (
         (ParameterType.CAV_LENGTH, ParameterType.ROC_M1),
         ParameterType.GFACTOR_M1,
     ),
     g2_of_Rc2: (
         (ParameterType.CAV_LENGTH, ParameterType.ROC_M2),
         ParameterType.GFACTOR_M2,
```

### Comparing `cavcalc-1.0.0/src/cavcalc/functions/_utils.py` & `cavcalc-1.1.0/src/cavcalc/functions/_utils.py`

 * *Files identical despite different names*

### Comparing `cavcalc-1.0.0/src/cavcalc/functions/asymmetric.py` & `cavcalc-1.1.0/src/cavcalc/functions/asymmetric.py`

 * *Files 12% similar despite different names*

```diff
@@ -69,30 +69,53 @@
     .. math::
         z_0(L, g_1, g_2) = \frac{L g_2 (1 - g_1)}{g_1 + g_2 - 2 g_1 g_2}
     """
     return L * g2 * (1 - g1) / (g1 + g2 - 2 * g1 * g2)
 
 
 def _rtgouy_of_g1g2_base(g1, g2):
-    return 2 * np.arccos(np.sign(g1 + g2) * np.sqrt(g1 * g2))
+    return 2 * np.arccos(0.5 * (np.sign(g1) + np.sign(g2)) * np.sqrt(g1 * g2))
 
 
 @check_physical()
 @ureg.wraps(ureg.radians, ("", ""))
 def rtgouy_of_g1g2(g1, g2):
     r"""Round-trip gouy phase of a cavity with mirror g-factors of :math:`g_1` and
     :math:`g_2`, respectively.
 
     .. math::
-        \psi(g_1, g_2) = 2\arccos{ \mathrm{sgn}\left(g_1 + g_2\right) \sqrt{g_1 g_2} }
+        \psi(g_1, g_2) = 2\arccos{
+            \left(
+                \frac{\mathrm{sgn}\left(g_1\right) + \mathrm{sgn}\left(g_2\right)}{2}
+                \sqrt{g_1 g_2}
+            \right)
+        }
     """
     return _rtgouy_of_g1g2_base(g1, g2)
 
 
 @check_physical()
+@ureg.wraps(ureg.radians, (ureg.meter, ureg.meter, "", ""))
+def divang_of_g1g2(L, wl, g1, g2):
+    r"""Divergence angle of the beam, of wavelength :math:`\lambda`, in a cavity of length
+    :math:`L`, with mirror g-factors of :math:`g_1` and :math:`g_2`, respectively.
+
+    .. math::
+        \theta(L, \lambda, g_1, g_2) = \arctan{\left(\sqrt{
+            \frac{\lambda}{L\pi} \sqrt{\frac{(g_1 + g_2 - 2 g_1 g_2)^2}{g_1 g_2 (1 - g_1 g_2)}}
+        }\right)}
+    """
+    return np.arctan(
+        np.sqrt(
+            (wl / (L * np.pi)) * np.sqrt((g1 + g2 - 2 * g1 * g2) ** 2 / (g1 * g2 * (1 - g1 * g2)))
+        )
+    )
+
+
+@check_physical()
 @ureg.wraps("", (ureg.meter, ureg.meter))
 def g1_of_Rc1(L, Rc1):
     r"""Stability factor of the *first* mirror of a cavity of length :math:`L`, where
     this mirror has radius of curvature :math:`R_{C,1}`.
 
     .. math::
         g_1(L, R_{C,1}) = 1 - \frac{L}{R_{C,1}}
```

### Comparing `cavcalc-1.0.0/src/cavcalc/functions/resonance.py` & `cavcalc-1.1.0/src/cavcalc/functions/resonance.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,10 +125,10 @@
     r"""The pole frequency of a cavity of length :math:`L`, where the first mirror has (power)
     reflectivity :math:`R_1` and the second mirror has reflectivity :math:`R_2`.
 
     In the equation below, :math:`\nu(L)` is the FSR, and :math:`\mathcal{F}(R_1,R_2)` is
     the finesse.
 
     .. math::
-        \mathrm{FWHM}(L, R_1, R_2) = \frac{\nu(L)}{2\mathcal{F}(R_1, R_2)}
+        \nu_p(L, R_1, R_2) = \frac{\nu(L)}{2\mathcal{F}(R_1, R_2)}
     """
     return 0.5 * _fsr_base(L) / _finesse_base(R1, R2)
```

### Comparing `cavcalc-1.0.0/src/cavcalc/functions/symmetric.py` & `cavcalc-1.1.0/src/cavcalc/functions/symmetric.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,32 +152,32 @@
 
 @check_physical()
 @ureg.wraps(ureg.radians, "")
 def rtgouy_of_gsingle(gsingle):
     r"""Round-trip gouy phase of a symmetric cavity with mirror g-factors of :math:`g_s`.
 
     .. math::
-        \psi(g_s) = 2 \arccos{g_s}
+        \psi(g_s) = 2 \arccos{\left(g_s\right)}
     """
     return _rtgouy_of_gsingle_base(gsingle)
 
 
 @check_physical()
 @ureg.wraps(ureg.radians, (ureg.meter, ureg.meter, ""))
 def divang_of_gsingle(L, wl, gsingle):
     r"""Divergence angle of the beam in a symmetric cavity of length :math:`L`, with
     mirror g-factors of :math:`g_s`; where the beam has wavelength :math:`\lambda`.
 
     .. math::
-        \theta(L, \lambda, g_s) = \sqrt{
+        \theta(L, \lambda, g_s) = \arctan{\left(\sqrt{
             \frac{2\lambda}{L\pi}
             \sqrt{\frac{1 - g_s}{1 + g_s}}
-        }
+        }\right)}
     """
-    return np.sqrt(2 * wl / (L * np.pi) * np.sqrt((1 - gsingle) / (1 + gsingle)))
+    return np.arctan(np.sqrt(2 * wl / (L * np.pi) * np.sqrt((1 - gsingle) / (1 + gsingle))))
 
 
 @check_physical()
 @ureg.wraps(ureg.hertz, (ureg.meter, ""))
 def modesep_of_gsingle(L, gsingle):
     r"""Mode separation frequency for a symmetric cavity of length :math:`L`, with
     mirror g-factors of :math:`g_s`.
```

### Comparing `cavcalc-1.0.0/src/cavcalc/output.py` & `cavcalc-1.1.0/src/cavcalc/output.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """
 The output objects which store the results from any call to :func:`.calculate`.
 """
 
+import abc
 import pickle
+from typing import Sequence, Union
 
 from . import Q_
 from .errors import CavCalcError
 from ._exiters import (
     bug as _bug,
     quit_print as _quit_print,
 )
@@ -26,75 +28,116 @@
     ----------
     file : str
         The name (and path if it isn't in the current working directory)
         of the file to open.
 
     Returns
     -------
-    output : (:class:`.SingleOutput` | :class:`.MultiOutput`)
+    output : :class:`.SingleOutput` | :class:`.MultiOutput`
         The cavcalc output instance.
+
+    Raises
+    ------
+    cce : :class:`.CavCalcError`
+        If the type of the loaded object is not :class:`.SingleOutput`
+        or :class:`.MultiOutput`.
     """
     with open(file, "rb") as f:
         output = pickle.load(f)
         if not isinstance(output, (SingleOutput, MultiOutput)):
             raise CavCalcError(f"Unrecognised serialized object in {file}")
 
     return output
 
 
-class SingleOutput:
-    """Storage and manipulation of a single target parameter computed via :func:`.calculate`."""
+def _param_str_gen(params: Sequence[Union[ArgParameter, TargetParameter]]):
+    return (f"{p.description} = {p.value:~}" for p in params)
 
-    def __init__(self, target: TargetParameter, phys_args: tuple[ArgParameter]):
-        self.__target = target
-        self.__given = phys_args
 
-    def __str__(self):
-        param_str_gen = lambda params: (f"{p.description} = {p.value:~}" for p in params)
-        order = (
-            ParameterCategory.Frequency,
-            ParameterCategory.Power,
-            ParameterCategory.Distance,
-            ParameterCategory.Curvature,
-            ParameterCategory.BeamRadius,
-            ParameterCategory.Stability,
-            ParameterCategory.Phase,
-            ParameterCategory.Angle,
-            ParameterCategory.Wave,
-        )
+class BaseOutput(abc.ABC):
+    """Abstract base class for output objects. Both :class:`.SingleOutput` and
+    :class:`.MultiOutput` derive from this type."""
+
+    category_order = (
+        ParameterCategory.Frequency,
+        ParameterCategory.Power,
+        ParameterCategory.Distance,
+        ParameterCategory.Curvature,
+        ParameterCategory.BeamRadius,
+        ParameterCategory.Stability,
+        ParameterCategory.Phase,
+        ParameterCategory.Angle,
+        ParameterCategory.Wave,
+    )
+
+    def __init__(self, phys_args: tuple[ArgParameter]):
+        self.__given = phys_args
 
-        given_str = "Given:\n\t"
-        for category in order:
+    def __str__(self) -> str:
+        s = "Given:\n\t"
+        for category in self.category_order:
             if args := tuple(filter(lambda p: p.category == category, self.__given)):
-                args = sorted(args, key=lambda a: a.ptype.value)
-                given_str += "\n\t".join(param_str_gen(args))
-                given_str += "\n\n\t"
+                s += "\n\t".join(_param_str_gen(sorted(args, key=lambda a: a.ptype.value)))
+                s += "\n\n\t"
 
-        computed_str = "Computed:\n\t" + "".join(param_str_gen((self.__target,)))
-        return given_str.strip() + "\n\n" + computed_str.strip()
+        return s.strip() + "\n\n"
 
     @property
-    def given(self):
+    def given(self) -> dict[str, ArgParameter]:
         """A dictionary of the given parameter names with their corresponding
         :class:`.ArgParameter` values."""
         return {arg_p.name: arg_p for arg_p in self.__given}
 
+    def print(self, **kwargs):
+        """Prints a string representation of the output, in an identical style to the CLI.
+
+        Parameters
+        ----------
+        kwargs : Keyword Arguments
+            Optional arguments to pass to Python ``print`` function.
+        """
+        print(str(self), **kwargs)
+
+    def save(self, file: str):
+        """Saves the output object to the specified ``file``, in a binary
+        serialised Python object format (via ``pickle``).
+
+        Parameters
+        ----------
+        file : str
+            The file name (and path if saving to a location outside of the current
+            working directory) to save this output instance to.
+        """
+        with open(file, "wb") as f:
+            pickle.dump(self, f, pickle.HIGHEST_PROTOCOL)
+
+
+class SingleOutput(BaseOutput):
+    """Storage and manipulation of a single target parameter computed via :func:`.calculate`."""
+
+    def __init__(self, target: TargetParameter, phys_args: tuple[ArgParameter]):
+        super().__init__(phys_args)
+        self.__target = target
+
+    def __str__(self) -> str:
+        return super().__str__() + "Computed:\n\t" + "".join(_param_str_gen((self.result,)))
+
     @property
     def name(self):
         """A short-hand for ``out.result.name``."""
         return self.__target.name
 
     @property
     def result(self):
         """The result itself as a :class:`.TargetParameter` instance.
 
         .. hint::
 
             Use ``result.value`` to get the ``pint.Quantity`` object, ``result.value.m``
-            to obtain the numerical value, and ``results.value.u`` to retrieve the units
+            to obtain the numerical value, and ``result.value.u`` to retrieve the units
             of this result.
         """
         return self.__target
 
     def convert(self, units):
         """Attempts to convert the result quantity, in-place, to the
         specified units.
@@ -111,18 +154,14 @@
         Parameters
         ----------
         units : str
             The units to convert to, as a string or ``cavcalc.ureg.<units>`` object.
         """
         self.__target = TargetParameter(self.result.name, self.result.value.to(units))
 
-    def print(self):
-        """Prints a string representation of the output, in an identical style to the CLI."""
-        print(str(self))
-
     def plot(
         self,
         xlim="auto",
         ylim="auto",
         zlim="auto",
         filename: str = None,
         logx: bool = False,
@@ -136,29 +175,29 @@
 
         If only one of the given arguments to the :func:`.calculate` call was array-like,
         then this will plot a standard line plot. Otherwise an image plot, via
         :func:`matplotlib.pyplot.imshow`, will be produced.
 
         Parameters
         ----------
-        xlim : (str | Iterable[float]), optional; default = "auto"
+        xlim : str | Iterable[float], optional; default = "auto"
             The limits of the x-axis. Defaults to ``"auto"`` such that matplotlib
             determines these automatically. This can be set to ``"data"`` so that
             the exact limits of the x-axis data are used. An iterable of length
             two can be used to manually override the x-axis limits; these will
             simply be forwarded to :func:`matplotlib.pyplot.xlim`.
 
-        ylim : (str | Iterable[float]), optional; default = "auto"
+        ylim : str | Iterable[float], optional; default = "auto"
             The limits of the y-axis. Defaults to ``"auto"`` such that matplotlib
             determines these automatically. This can be set to ``"data"`` so that
             the exact limits of the y-axis data are used. An iterable of length
             two can be used to manually override the y-axis limits; these will
             simply be forwarded to :func:`matplotlib.pyplot.ylim`.
 
-        zlim : (str | Iterable[float]), optional; default = "auto"
+        zlim : str | Iterable[float], optional; default = "auto"
             The limits of the color-bar scale for image plots. Ignored if
             this is a line plot.
 
         filename : str, optional; default = None
             A filename to save the figure to.
 
         logx : bool, optional; default = False
@@ -167,17 +206,18 @@
         logy : bool, optional; default = False
             Whether to use a log-scale on the y-axis. Ignored if this is an image plot.
 
         logz : bool, optional; default = False
             Whether to use a log normalisation of the image plot Z data. Ignored if
             this is a line plot.
 
-        cmap : (str | Colormap), optional; default = None
-            Name, or instance, of the colormap to use for image plots. Defaults to
-            the current default map as per matplotlib. Ignored if this is a line plot.
+        cmap : str | :class:`matplotlib.colors.ListedColormap`, optional; default = None
+            Name, or instance, of the colormap to use for image plots. If not given,
+            the colormap will default to the relevant ``matplotlib.rcParams`` value.
+            Ignored if this is a line plot.
 
         show : bool, optional; default = False
             Shows the resulting figure, via :func:`matplotlib.pyplot.show`, if true.
 
         fig : :class:`matplotlib.figure.Figure`, optional; default = None
             An optional pre-existing figure object to draw on. If not given, then a new
             figure is created and used.
@@ -196,21 +236,20 @@
         """
         if not self.__target.is_array:
             _quit_print(
                 f"Value of target '{self.__target.name}' is not array-like! Did "
                 "you forget to set one of the dependent arguments to an array?"
             )
 
-        xs = tuple(
-            sorted(filter(lambda p: p.is_array, self.__given), key=lambda p: (p.axis, p.index))
-        )
+        given = self.given.values()
+        xs = tuple(sorted(filter(lambda p: p.is_array, given), key=lambda p: (p.axis, p.index)))
         num_x_arrays = len(xs)
         if not num_x_arrays:
             _bug(
-                f"Somehow none of the given args, ({', '.join(arg_p.name for arg_p in self.__given)}), "
+                f"Somehow none of the given args, ({', '.join(self.given.keys())}), "
                 f"are array-like, but the target value, {self.__target.name}, is!"
             )
 
         plotting_dims = max(len(x.value.m.shape) for x in xs)
         if plotting_dims > 2:
             _quit_print(f"Cannot plot results over {plotting_dims} dimensions!")
 
@@ -224,15 +263,15 @@
             else:
                 plt.sca(fig.subplots())
 
         def _make_label(p: ArgParameter):
             return p.description + (f" [{p.value.units:~}]" if not p.is_unitless else "")
 
         # The non-array arguments specified
-        if fixed := tuple(filter(lambda p: p.is_scalar, self.__given)):
+        if fixed := tuple(filter(lambda p: p.is_scalar, given)):
             fixed_params_str = "with: " + ", ".join(f"{p.symbol_str} = {p.value:~}" for p in fixed)
         else:
             fixed_params_str = ""
 
         if plotting_dims == 1 or num_x_arrays == 1:
             if num_x_arrays > 2:
                 _quit_print("Plots with more than two x-axes are not supported.")
@@ -301,19 +340,21 @@
                 # Reset current state to first axes
                 plt.sca(ax1)
 
         else:
             if num_x_arrays > 2:
                 _quit_print("Image plots with multiple x-axes are not supported.")
 
+            import matplotlib
+
             x, y = xs
             z = self.__target
 
             try:
-                cmap = plt.cm.get_cmap(cmap)
+                cmap = matplotlib.colormaps.get_cmap(cmap)
             except ValueError as ex:
                 _quit_print(str(ex))
 
             extent = [x.value.m.min(), x.value.m.max(), y.value.m.min(), y.value.m.max()]
 
             if logz:
                 if not zlim or isinstance(zlim, str):
@@ -383,41 +424,27 @@
             fig.savefig(filename)
 
         if show:
             plt.show()
 
         return fig
 
-    def save(self, file: str):
-        """Saves this single-output object to the specified ``file``, in a binary
-        serialised Python object format (via ``pickle``).
-
-        Parameters
-        ----------
-        file : str
-
-            The file name (and path if saving to a location outside of the current
-            working directory) to save this single-output instance to.
-        """
-        with open(file, "wb") as f:
-            pickle.dump(self, f, pickle.HIGHEST_PROTOCOL)
-
 
-class MultiOutput:
+class MultiOutput(BaseOutput):
     """Storage and manipulation of multiple target parameters computed via :func:`.calculate`.
 
     Use :meth:`.MultiOutput.as_singles` to easily construct :class:`.SingleOutput` instances
     from a multi-output object.
     """
 
     def __init__(
         self, targets: dict[TargetParameter, tuple[ParameterType]], phys_args: tuple[ArgParameter]
     ):
+        super().__init__(phys_args)
         self.__targets = targets
-        self.__given = phys_args
 
     def __getitem__(self, key):
         if isinstance(key, str):
             try:
                 return next((tgt_p for tgt_p in self.__targets if tgt_p.name == key))
             except StopIteration:
                 raise CavCalcError(f"No target of name '{key}' exists in the output.")
@@ -431,61 +458,38 @@
         if isinstance(key, ParameterCategory):
             targets = tuple(filter(lambda t: t.category == key, self.__targets))
             if not targets:
                 raise CavCalcError(f"No targets of parameter category '{key}' exist in the output.")
 
             return targets
 
-    def __str__(self):
-        param_str_gen = lambda params: (f"{p.description} = {p.value:~}" for p in params)
-        order = (
-            ParameterCategory.Frequency,
-            ParameterCategory.Power,
-            ParameterCategory.Distance,
-            ParameterCategory.Curvature,
-            ParameterCategory.BeamRadius,
-            ParameterCategory.Stability,
-            ParameterCategory.Phase,
-            ParameterCategory.Angle,
-            ParameterCategory.Wave,
-        )
-        given_str = "Given:\n\t"
-        computed_str = "Computed:\n\t"
-        for category in order:
-            if args := tuple(filter(lambda p: p.category == category, self.__given)):
-                args = sorted(args, key=lambda a: a.ptype.value)
-                given_str += "\n\t".join(param_str_gen(args))
-                given_str += "\n\n\t"
+        raise TypeError("Expected key-type of str, ParameterType or ParameterCategory.")
 
+    def __str__(self) -> str:
+        s = "Computed:\n\t"
+        for category in self.category_order:
             if targets := self.get(category):
-                targets = sorted(targets, key=lambda t: t.ptype.value)
-                computed_str += "\n\t".join(param_str_gen(targets))
-                computed_str += "\n\n\t"
+                s += "\n\t".join(_param_str_gen(sorted(targets, key=lambda t: t.ptype.value)))
+                s += "\n\n\t"
 
-        return given_str.strip() + "\n\n" + computed_str.strip()
-
-    @property
-    def given(self):
-        """A dictionary of the given parameter names with their corresponding
-        :class:`.ArgParameter` values."""
-        return {arg_p.name: arg_p for arg_p in self.__given}
+        return super().__str__() + s.strip()
 
     @property
     def results(self):
         """A dictionary of results, mapping the names of the target parameters to their values (as
         ``pint.Quantity`` instances)."""
         return {tgt_p.name: tgt_p for tgt_p in self.__targets}
 
     def as_single(self, ptype) -> SingleOutput:
         """A :class:`.SingleOutput` instance constructed, from this multi-output,
         for a single desired parameter type.
 
         Parameters
         ----------
-        ptype : (str | :class:`.ParameterType`)
+        ptype : str | :class:`.ParameterType`
             The parameter type.
 
         Returns
         -------
         single : :class:`.SingleOutput`
             The single output object for the desired parameter type.
         """
@@ -528,15 +532,15 @@
             if target is None:
                 raise CavCalcError(f"No target of type '{arg}' in the output.")
 
             func_params = self.__targets.get(target)
             if not func_params:
                 _bug(f"No function parameters for target parameter of type '{arg}'")
 
-            phys_args = tuple(arg_p for arg_p in self.__given if arg_p.ptype in func_params)
+            phys_args = tuple(arg_p for arg_p in self.given.values() if arg_p.ptype in func_params)
             singles[arg] = SingleOutput(target, phys_args)
 
         return singles
 
     def get(self, key, default=None):
         """Retrieve a target result, or a collection of these, using a suitable key.
 
@@ -545,23 +549,23 @@
 
         Alternatively, ``key`` can be a :class:`.ParameterCategory`. In this case all the target
         parameters belonging to this category will be returned, or ``default`` if no targets of
         this category are present in the output.
 
         Parameters
         ----------
-        key : (str | :class:`.ParameterType` | :class:`.ParameterCategory`)
+        key : str | :class:`.ParameterType` | :class:`.ParameterCategory`
             The key of the target(s) to retrieve. See above for options.
 
-        default : (Any | NoneType), optional
+        default : Any | NoneType, optional
             The default value to return if no target(s) corresponding to ``key`` could be found.
 
         Returns
         -------
-        target : (:class:`.TargetParameter` | tuple[:class:`.TargetParameter`] | Any)
+        target : :class:`.TargetParameter` | tuple[:class:`.TargetParameter`] | Any
             The target, or tuple of targets if ``key`` was a :class:`.ParameterCategory`, or ``default``
             if no target(s) could be obtained from the given ``key``.
         """
         try:
             return self[key]
         except CavCalcError:
             return default
@@ -601,21 +605,7 @@
             fig = out.plot(filename=filename_single, show=False, **kwargs)
             figures[ptype] = fig
 
         if show and figures:
             plt.show()
 
         return figures
-
-    def save(self, file: str):
-        """Saves this multi-output object to the specified ``file``, in a binary
-        serialised Python object format (via ``pickle``).
-
-        Parameters
-        ----------
-        file : str
-
-            The file name (and path if saving to a location outside of the current
-            working directory) to save this multi-output instance to.
-        """
-        with open(file, "wb") as f:
-            pickle.dump(self, f, pickle.HIGHEST_PROTOCOL)
```

### Comparing `cavcalc-1.0.0/src/cavcalc/parameters/_maps.py` & `cavcalc-1.1.0/src/cavcalc/parameters/_maps.py`

 * *Files identical despite different names*

### Comparing `cavcalc-1.0.0/src/cavcalc/parameters/enums.py` & `cavcalc-1.1.0/src/cavcalc/parameters/enums.py`

 * *Files identical despite different names*

### Comparing `cavcalc-1.0.0/src/cavcalc/parameters/parameter.py` & `cavcalc-1.1.0/src/cavcalc/parameters/parameter.py`

 * *Files identical despite different names*

### Comparing `cavcalc-1.0.0/setup.py` & `cavcalc-1.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,364 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: cavcalc
+Version: 1.1.0
+Summary: A program for computing Fabry-Perot optical cavity parameters.
+Home-page: https://cavcalc.readthedocs.io/en/latest/
+License: GPL-3.0-or-later
+Keywords: physics,optics,interferometry
+Author: Samuel Rowlinson
+Author-email: samueljrowlinson@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Scientific/Engineering :: Physics
+Requires-Dist: Pint (>=0.19.2,<0.20.0)
+Requires-Dist: importlib-metadata (>=4.0,<5.0) ; python_version < "3.9"
+Requires-Dist: matplotlib (>=3.6.1,<4.0.0)
+Requires-Dist: numpy (>=1.23.3,<2.0.0)
+Project-URL: Documentation, https://cavcalc.readthedocs.io/en/latest/
+Project-URL: Repository, https://gitlab.com/sjrowlinson/cavcalc
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+![](https://gitlab.com/sjrowlinson/cavcalc/raw/master/docs/source/_static/logo.svg)
 
-packages = \
-['cavcalc', 'cavcalc._arguments', 'cavcalc.functions', 'cavcalc.parameters']
+A command line program and Python module for computing parameters associated with linear, Fabry-Perot optical cavities.
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['Pint>=0.19.2,<0.20.0', 'matplotlib>=3.6.1,<4.0.0', 'numpy>=1.23.3,<2.0.0']
-
-extras_require = \
-{':python_version < "3.9"': ['importlib-metadata>=4.0,<5.0']}
-
-entry_points = \
-{'console_scripts': ['cavcalc = cavcalc.__main__:cli_entry']}
-
-setup_kwargs = {
-    'name': 'cavcalc',
-    'version': '1.0.0',
-    'description': 'A program for computing Fabry-Perot optical cavity parameters.',
-    'long_description': '![](https://gitlab.com/sjrowlinson/cavcalc/raw/master/images/logo_cavcalc.png)\n\nA command line program and Python module for computing parameters associated with linear, Fabry-Perot optical cavities.\n\n- Find the documentation at: https://cavcalc.readthedocs.io/en/latest/\n- Follow the latest changes: https://gitlab.com/sjrowlinson/cavcalc\n- See the entry on PyPI: https://pypi.org/project/cavcalc/\n\n## Installation\nTo install `cavcalc`, simply run:\n\n```\npip install cavcalc\n```\n\nCheck that the installation was successful with:\n\n```bash\ncavcalc --version\n```\n\nif you see something along the lines of\n\n```\ncavcalc v1.0.0\n```\n\nthen you should be ready to start using `cavcalc`!\n\n**Note**: As is often recommended with the installation of Python packages (especially those with dependencies\non packages such as `numpy` and `matplotlib`, as is the case here), you should prefer to install `cavcalc` in\na suitable virtual environment. See [the official documentation on Python virtual environments](https://docs.python.org/3/tutorial/venv.html)\nfor details on how to set up these if you are unfamiliar with the topic.\n\n## Example usage via the CLI\n\nFor details on available arguments run `cavcalc -h` on the command line.\n\nSome examples follow on how to use `cavcalc`. See [the documentation on using cavcalc](https://cavcalc.readthedocs.io/en/latest/using/index.html)\nfor more in-depth examples and guides.\n\n### Computing single parameters\n\nYou can ask for, e.g., the beam size on the mirrors of a symmetric cavity given its length and stability factor of the mirrors (gs) with:\n\n```bash\ncavcalc w -L 4000 -gs 0.91\n```\n\nThis would result in an output of:\n\n```\nGiven:\n\tCavity length = 4000 m\n\n\tStability g-factor of both mirrors = 0.91\n\n\tWavelength of beam = 1064 nm\n\nComputed:\n\tRadius of beam at mirrors = 57.16193267930482 mm\n```\n\nUnits for both inputs and outputs can also be specified:\n\n```bash\ncavcalc w -u mm -L 10km -gouy 145deg\n```\n\nThis requests the beam radius (in mm) on the mirrors of a symmetric cavity of length 10km given that the\nround-trip Gouy phase is 145 degrees; resulting in the following output:\n\n```\nGiven:\n\tCavity length = 10 km\n\n\tRound-trip Gouy phase = 145 deg\n\n\tWavelength of beam = 1064 nm\n\nComputed:\n\tRadius of beam at mirrors = 59.59174828941794 mm\n```\n\nSupport for units is provided via the package [Pint](https://pint.readthedocs.io/en/stable/index.html), so any units\ndefined in the Pint unit-registry can be used in cavcalc.\n\n### Computing all available parameters\n\nA compute target of `all` is the default choice which is used to calculate all parameters which can be determined\nfrom the arguments specified. For example, using approximate values of the Advanced LIGO arm cavity parameters,\n\n```bash\ncavcalc -L 4km -Rc1 1934 -Rc2 2245 -T1 0.014 -L1 37.5e-6 -T2 5e-6 -L2 37.5e-6\n```\n\ngives the following output:\n\n```\nGiven:\n\tLoss of first mirror = 3.75e-05\n\tLoss of second mirror = 3.75e-05\n\tTransmission of first mirror = 0.014\n\tTransmission of second mirror = 5e-06\n\n\tCavity length = 4 km\n\n\tRadius of curvature of first mirror = 1934 m\n\tRadius of curvature of second mirror = 2245 m\n\n\tWavelength of beam = 1064 nm\n\nComputed:\n\tFSR = 37474.05725 Hz\n\tFWHM = 84.56921734107604 Hz\n\tMode separation frequency = 4988.072188176178 Hz\n\tPole frequency = 42.28460867053802 Hz\n\n\tFinesse = 443.11699254426594\n\tReflectivity of first mirror = 0.9859625\n\tReflectivity of second mirror = 0.9999574999999999\n\n\tPosition of beam waist (from first mirror) = 1837.2153886417168 m\n\n\tRadius of beam at first mirror = 53.421066433049255 mm\n\tRadius of beam at second mirror = 62.448079883230896 mm\n\tRadius of beam at waist = 11.950538458990879 mm\n\n\tStability g-factor of cavity = 0.8350925761717987\n\tStability g-factor of first mirror = -1.0682523267838677\n\tStability g-factor of second mirror = -0.7817371937639199\n\n\tRound-trip Gouy phase = 312.0813565565169 deg\n```\n\n### Units of output\n\nThe default behaviour for the output parameter units is to grab the relevant parameter type option under the `[units]` header\nof the `cavcalc.ini` configuration file. When installing `cavcalc`, this file is written to a new `cavcalc/` directory within\nyour config directory (i.e. typically `~/.config/cavcalc/cavcalc.ini` under Unix systems). See the comments in this file for\ndetails on the options available for the output units of each parameter type.\n\n`cavcalc` attempts to read a `cavcalc.ini` config file from several locations in this fixed order:\n\n- Firstly from the current working directory, then\n- from `$XDG_CONFIG_HOME/cavcalc/` (or `%APPDATA%/cavcalc/` on Windows), then\n- the final read attempt is from the within the source of the package directory itself.\n\nThe config options from these read attempts are loaded in a standard way; that is, any options appearing\nfirst in the sequence defined above will take priority. If any of the above read attempts fails, then this\nwill be a silent failure; the only situation where an error could occur would be when *all* of the above\nread attempts fail (which is very unlikely to happen).\n\nNote that if you specify a `-u` argument when running `cavcalc` from the CLI, then this takes priority over\nthe options in the config file (as we saw in an example above).\n\n### Evaluating, and plotting, parameters over data ranges\n\nParameters can be computed over ranges of data using:\n\n* the data range syntax: `-<param_name> "start stop num [<units>]"`,\n* or data from an input file with `-<param_name> <file>`.\n\nWe can use data-ranges to compute, and plot, arrays of target values, e.g:\n\n```bash\ncavcalc w -L "1 10 100 km" -Rc 5.1km --plot\n```\n\nThis results in a plot (see below) showing how the beam radius at the mirrors of a symmetric cavity varies from\na cavity length of 1 km to 10 km with 100 data points, with the radii of curvature of both mirrors fixed at 5.1 km.\n\n![](https://gitlab.com/sjrowlinson/cavcalc/raw/master/images/symmcav_ws_vs_lengths.png)\n\n\nAlternatively one could use a file of data, e.g:\n\n```bash\ncavcalc gouy -L 5cm -w beam_radii.txt --plot --saveplot symmcav_gouy_vs_ws.png\n```\n\nThis then computes the round-trip Gouy phase (in degrees) of a symmetric cavity of length 5cm\nusing beam radii data stored in a file `beam_radii.txt`, and plots the results (see below). Note also that\nyou can save the resulting figure using the `--saveplot <filename>` syntax as seen in the above command.\n\n![](https://gitlab.com/sjrowlinson/cavcalc/raw/master/images/symmcav_gouy_vs_ws.png)\n\nFrom the plot above you can also see that cavcalc supports automatically plotting of quantities which can be\ndual-valued. In this case, the Gouy phase can be one of two values for each beam radius; this is due to the\nnature of the equations which govern the Fabry-Perot cavity dynamics.\n\n### Image / density plots via `--mesh`\n\nWhen multiple arguments are given as data-ranges, one can use the `--mesh` option to construct mesh-grids\nof these parameters. This allows cavcalc to automatically produce image plots. For example:\n\n```bash\ncavcalc w -L "1 10 100 km" -gouy "20 120 100 deg" --mesh true --plot\n```\n\ncomputes the radius of the beam on the mirrors of a symmetric cavity, against both the cavity length and\nround-trip Gouy phase on a grid. This results in the plot shown below. Note that we simply used `--mesh true`\nhere, which automatically determines the ordering of the mesh-grid parameters based on the order in which\nthese parameters were given. One could replace the above with, e.g., `--mesh "gouy,L"` to reverse the order\nof the mesh-grid; and thereby flip the parameter axes on any automated plots.\n\n![](https://gitlab.com/sjrowlinson/cavcalc/raw/master/images/symmcav_w_vs_L_gouy.png)\n\nA matplotlib compliant colour-map can be specified when making an image plot using the `--cmap <name>` option. For example,\nthe following command gives the plot shown below.\n\n```bash\ncavcalc gouy -L 12um -g1 "-2 2 499" -g2 "-2 2 499" --mesh true --plot --cmap Spectral_r\n```\n\n![](https://gitlab.com/sjrowlinson/cavcalc/raw/master/images/asymmcav_w0_vs_g1g2.png)\n\n## A note on g-factors\n\nStability (g) factors are split into four different parameters for implementation purposes and to\nhopefully make it clearer as to which argument is being used and whether the resulting cavity\ncomputations are for a symmetric or asymmetric cavity. These arguments are detailed here:\n\n- `-gs` : The symmetric, singular stability factor. This represents the individual g-factors of **both**\n          cavity mirrors. Use this to define a *symmetric* cavity where the overall cavity g-factor is\n\t\t  then simply `g = gs * gs`.\n- `-g` : The overall cavity stability factor. This is the product of the individual g-factors of the\n         cavity mirrors. Use this to define a *symmetric* cavity where the individual g-factors of **both**\n\t\t mirrors are then `gs = +/- sqrt(g)`.\n- `-g1` : The stability factor of the first cavity mirror. Use this to define an *asymmetric* cavity\n          along with the argument `-g2` such that the overall cavity g-factor is then `g = g1 * g2`.\n- `-g2` : The stability factor of the second cavity mirror. Use this to define an *asymmetric* cavity\n          along with the argument `-g1` such that the overall cavity g-factor is then `g = g1 * g2`.\n\n---\n\n## Using `cavcalc` programmatically\n\nAs well as providing a CLI, cavcalc has a full API which allows users to interact with this tool\nvia Python. The recommended method for doing this is to use the single-function interface via\n[`cavcalc.calculate`](https://cavcalc.readthedocs.io/en/latest/api/generated/cavcalc.calculate.calculate.html#cavcalc.calculate.calculate). This\nfunction works similarly to the CLI, where a target can be specified along with a variable number of keyword\narguments corresponding to the physical parameters. This function then returns one of two output objects (`SingleOutput`\nif a target was given, `MultiOutput` otherwise); see [`cavcalc.output`](https://cavcalc.readthedocs.io/en/latest/api/cavcalc.output.html#module-cavcalc.output)\nfor details.\n\nFor example, the following script will compute all available targets from the cavity length and mirror radii\nof curvature provided:\n\n```python\nimport cavcalc as cc\n\n# Specifying no target means all possible targets are computed\nout = cc.calculate(L="4km", Rc1=1934, Rc2=2245)\n\n# Printing the output object results in the same output as\n# you would see when running via the CLI\nprint(out)\n```\n\nresults in:\n\n```\nGiven:\n\tCavity length = 4 km\n\n\tRadius of curvature of first mirror = 1934 m\n\tRadius of curvature of second mirror = 2245 m\n\n\tWavelength of beam = 1064 nm\n\nComputed:\n\tFSR = 37474.05725 Hz\n\tMode separation frequency = 4988.072188176178 Hz\n\n\tPosition of beam waist (from first mirror) = 1837.2153886417168 m\n\n\tRadius of beam at first mirror = 53.421066433049255 mm\n\tRadius of beam at second mirror = 62.448079883230896 mm\n\tRadius of beam at waist = 11.950538458990879 mm\n\n\tStability g-factor of cavity = 0.8350925761717987\n\tStability g-factor of first mirror = -1.0682523267838677\n\tStability g-factor of second mirror = -0.7817371937639199\n\n\tRound-trip Gouy phase = 312.0813565565169 deg\n```\n\nAn extra feature of the API is the ability to use the `cavcalc.configure` function for overriding\ndefault behaviour. For example, in the script below we use this in a context-managed scope to\ntemporarily use microns for any beam radius parameters, mm for distances, and GHz for any frequencies:\n\n```python\nimport cavcalc as cc\n\n# Temporarily override units...\nwith cc.configure(beamsizes="um", distances="mm", frequencies="GHz"):\n    out = cc.calculate(L="8mm", gouy=121)\n    print(out)\n\n# ... previous state (using loaded config options) will\n# be restored on exit from the with block above\n```\n\nresulting in:\n\n```\nGiven:\n    Cavity length = 8 mm\n\n    Round-trip Gouy phase = 121 deg\n\n    Wavelength of beam = 1064 nm\n\nComputed:\n    FSR = 18.737028625 GHz\n    Mode separation frequency = 6.297723510069445 GHz\n\n    Position of beam waist (from first mirror) = 4.0 mm\n\n    Radius of curvature of both mirrors = 0.01576117284251957 m\n\n    Radius of beam at mirrors = 55.79464044247193 µm\n    Radius of beam at waist = 48.19739141432035 µm\n\n    Stability g-factor of cavity = 0.2424809625449729\n    Stability g-factor of both mirrors = 0.4924235601034671\n\n    Divergence angle = 0.4026158371180008 deg\n```\n',
-    'author': 'Samuel Rowlinson',
-    'author_email': 'samueljrowlinson@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://cavcalc.readthedocs.io/en/latest/',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
-}
+- Find the documentation at: https://cavcalc.readthedocs.io/en/latest/
+- Follow the latest changes: https://gitlab.com/sjrowlinson/cavcalc
+- See the entry on PyPI: https://pypi.org/project/cavcalc/
 
+## Installation
+To install `cavcalc`, simply run:
+
+```
+pip install cavcalc
+```
+
+Check that the installation was successful with:
+
+```bash
+cavcalc --version
+```
+
+if you see something along the lines of
+
+```
+cavcalc v1.1.0
+```
+
+then you should be ready to start using `cavcalc`!
+
+**Note**: As is often recommended with the installation of Python packages (especially those with dependencies
+on packages such as `numpy` and `matplotlib`, as is the case here), you should prefer to install `cavcalc` in
+a suitable virtual environment. See [the official documentation on Python virtual environments](https://docs.python.org/3/tutorial/venv.html)
+for details on how to set up these if you are unfamiliar with the topic.
+
+## Example usage via the CLI
+
+For details on available arguments run `cavcalc -h` on the command line.
+
+Some examples follow on how to use `cavcalc`. See [the documentation on using cavcalc](https://cavcalc.readthedocs.io/en/latest/using/index.html)
+for more in-depth examples and guides.
+
+### Computing single parameters
+
+You can ask for, e.g., the beam size on the mirrors of a symmetric cavity given its length and stability factor of the mirrors (gs) with:
+
+```bash
+cavcalc w -L 4000 -gs 0.91
+```
+
+This would result in an output of:
+
+```
+Given:
+	Cavity length = 4000 m
+
+	Stability g-factor of both mirrors = 0.91
+
+	Wavelength of beam = 1064 nm
+
+Computed:
+	Radius of beam at mirrors = 57.16193267930482 mm
+```
+
+Units for both inputs and outputs can also be specified:
+
+```bash
+cavcalc w -u mm -L 10km -gouy 145deg
+```
+
+This requests the beam radius (in mm) on the mirrors of a symmetric cavity of length 10km given that the
+round-trip Gouy phase is 145 degrees; resulting in the following output:
+
+```
+Given:
+	Cavity length = 10 km
+
+	Round-trip Gouy phase = 145 deg
+
+	Wavelength of beam = 1064 nm
+
+Computed:
+	Radius of beam at mirrors = 59.59174828941794 mm
+```
+
+Support for units is provided via the package [Pint](https://pint.readthedocs.io/en/stable/index.html), so any units
+defined in the Pint unit-registry can be used in cavcalc.
+
+### Computing all available parameters
+
+A compute target of `all` is the default choice which is used to calculate all parameters which can be determined
+from the arguments specified. For example, using approximate values of the Advanced LIGO arm cavity parameters,
+
+```bash
+cavcalc -L 4km -Rc1 1934 -Rc2 2245 -T1 0.014 -L1 37.5e-6 -T2 5e-6 -L2 37.5e-6
+```
+
+gives the following output:
+
+```
+Given:
+	Loss of first mirror = 3.75e-05
+	Loss of second mirror = 3.75e-05
+	Transmission of first mirror = 0.014
+	Transmission of second mirror = 5e-06
+
+	Cavity length = 4 km
+
+	Radius of curvature of first mirror = 1934 m
+	Radius of curvature of second mirror = 2245 m
+
+	Wavelength of beam = 1064 nm
+
+Computed:
+	FSR = 37474.05725 Hz
+	FWHM = 84.56921734107604 Hz
+	Mode separation frequency = 4988.072188176178 Hz
+	Pole frequency = 42.28460867053802 Hz
+
+	Finesse = 443.11699254426594
+	Reflectivity of first mirror = 0.9859625
+	Reflectivity of second mirror = 0.9999574999999999
+
+	Position of beam waist (from first mirror) = 1837.2153886417168 m
+
+	Radius of beam at first mirror = 53.421066433049255 mm
+	Radius of beam at second mirror = 62.448079883230896 mm
+	Radius of beam at waist = 11.950538458990879 mm
+
+	Stability g-factor of cavity = 0.8350925761717987
+	Stability g-factor of first mirror = -1.0682523267838677
+	Stability g-factor of second mirror = -0.7817371937639199
+
+	Round-trip Gouy phase = 312.0813565565169 deg
+
+	Divergence angle = 0.0016237789746943276 deg
+```
+
+### Units of output
+
+The default behaviour for the output parameter units is to grab the relevant parameter type option under the `[units]` header
+of the `cavcalc.ini` configuration file. When installing `cavcalc`, this file is written to a new `cavcalc/` directory within
+your config directory (i.e. typically `~/.config/cavcalc/cavcalc.ini` under Unix systems). See the comments in this file for
+details on the options available for the output units of each parameter type.
+
+`cavcalc` attempts to read a `cavcalc.ini` config file from several locations in this fixed order:
+
+- Firstly from the current working directory, then
+- from `$XDG_CONFIG_HOME/cavcalc/` (or `%APPDATA%/cavcalc/` on Windows), then
+- the final read attempt is from the within the source of the package directory itself.
+
+The config options from these read attempts are loaded in a standard way; that is, any options appearing
+first in the sequence defined above will take priority. If any of the above read attempts fails, then this
+will be a silent failure; the only situation where an error could occur would be when *all* of the above
+read attempts fail (which is very unlikely to happen).
+
+Note that if you specify a `-u` argument when running `cavcalc` from the CLI, then this takes priority over
+the options in the config file (as we saw in an example above).
+
+### Evaluating, and plotting, parameters over data ranges
+
+Parameters can be computed over ranges of data using:
+
+* the data range syntax: `-<param_name> "start stop num [<units>]"`,
+* or data from an input file with `-<param_name> <file>`.
+
+We can use data-ranges to compute, and plot, arrays of target values, e.g:
+
+```bash
+cavcalc w -L "1 10 100 km" -Rc 5.1km --plot
+```
+
+This results in a plot (see below) showing how the beam radius at the mirrors of a symmetric cavity varies from
+a cavity length of 1 km to 10 km with 100 data points, with the radii of curvature of both mirrors fixed at 5.1 km.
+
+![](https://gitlab.com/sjrowlinson/cavcalc/raw/master/images/symmcav_ws_vs_lengths.png)
+
+
+Alternatively one could use a file of data, e.g:
+
+```bash
+cavcalc gouy -L 5cm -w beam_radii.txt --plot --saveplot symmcav_gouy_vs_ws.png
+```
+
+This then computes the round-trip Gouy phase (in degrees) of a symmetric cavity of length 5cm
+using beam radii data stored in a file `beam_radii.txt`, and plots the results (see below). Note also that
+you can save the resulting figure using the `--saveplot <filename>` syntax as seen in the above command.
+
+![](https://gitlab.com/sjrowlinson/cavcalc/raw/master/images/symmcav_gouy_vs_ws.png)
+
+From the plot above you can also see that cavcalc supports automatically plotting of quantities which can be
+dual-valued. In this case, the Gouy phase can be one of two values for each beam radius; this is due to the
+nature of the equations which govern the Fabry-Perot cavity dynamics.
+
+### Image / density plots via `--mesh`
+
+When multiple arguments are given as data-ranges, one can use the `--mesh` option to construct mesh-grids
+of these parameters. This allows cavcalc to automatically produce image plots. For example:
+
+```bash
+cavcalc w -L "1 10 100 km" -gouy "20 120 100 deg" --mesh true --plot
+```
+
+computes the radius of the beam on the mirrors of a symmetric cavity, against both the cavity length and
+round-trip Gouy phase on a grid. This results in the plot shown below. Note that we simply used `--mesh true`
+here, which automatically determines the ordering of the mesh-grid parameters based on the order in which
+these parameters were given. One could replace the above with, e.g., `--mesh "gouy,L"` to reverse the order
+of the mesh-grid; and thereby flip the parameter axes on any automated plots.
+
+![](https://gitlab.com/sjrowlinson/cavcalc/raw/master/images/symmcav_w_vs_L_gouy.png)
+
+A matplotlib compliant colour-map can be specified when making an image plot using the `--cmap <name>` option. For example,
+the following command gives the plot shown below.
+
+```bash
+cavcalc gouy -L 12um -g1 "-2 2 499" -g2 "-2 2 499" --mesh true --plot --cmap Spectral_r
+```
+
+![](https://gitlab.com/sjrowlinson/cavcalc/raw/master/images/asymmcav_w0_vs_g1g2.png)
+
+## A note on g-factors
+
+Stability (g) factors are split into four different parameters for implementation purposes and to
+hopefully make it clearer as to which argument is being used and whether the resulting cavity
+computations are for a symmetric or asymmetric cavity. These arguments are detailed here:
+
+- `-gs` : The symmetric, singular stability factor. This represents the individual g-factors of **both**
+          cavity mirrors. Use this to define a *symmetric* cavity where the overall cavity g-factor is
+		  then simply `g = gs * gs`.
+- `-g` : The overall cavity stability factor. This is the product of the individual g-factors of the
+         cavity mirrors. Use this to define a *symmetric* cavity where the individual g-factors of **both**
+		 mirrors are then `gs = +/- sqrt(g)`.
+- `-g1` : The stability factor of the first cavity mirror. Use this to define an *asymmetric* cavity
+          along with the argument `-g2` such that the overall cavity g-factor is then `g = g1 * g2`.
+- `-g2` : The stability factor of the second cavity mirror. Use this to define an *asymmetric* cavity
+          along with the argument `-g1` such that the overall cavity g-factor is then `g = g1 * g2`.
+
+---
+
+## Using `cavcalc` programmatically
+
+As well as providing a CLI, cavcalc has a full API which allows users to interact with this tool
+via Python. The recommended method for doing this is to use the single-function interface via
+[`cavcalc.calculate`](https://cavcalc.readthedocs.io/en/latest/api/generated/cavcalc.calculate.calculate.html#cavcalc.calculate.calculate). This
+function works similarly to the CLI, where a target can be specified along with a variable number of keyword
+arguments corresponding to the physical parameters. This function then returns one of two output objects (`SingleOutput`
+if a target was given, `MultiOutput` otherwise); see [`cavcalc.output`](https://cavcalc.readthedocs.io/en/latest/api/cavcalc.output.html#module-cavcalc.output)
+for details.
+
+For example, the following script will compute all available targets from the cavity length and mirror radii
+of curvature provided:
+
+```python
+import cavcalc as cc
+
+# Specifying no target means all possible targets are computed
+out = cc.calculate(L="4km", Rc1=1934, Rc2=2245)
+
+# Printing the output object results in the same output as
+# you would see when running via the CLI
+print(out)
+```
+
+producing:
+
+```
+Given:
+	Cavity length = 4 km
+
+	Radius of curvature of first mirror = 1934 m
+	Radius of curvature of second mirror = 2245 m
+
+	Wavelength of beam = 1064 nm
+
+Computed:
+	FSR = 37474.05725 Hz
+	Mode separation frequency = 4988.072188176178 Hz
+
+	Position of beam waist (from first mirror) = 1837.2153886417168 m
+
+	Radius of beam at first mirror = 53.421066433049255 mm
+	Radius of beam at second mirror = 62.448079883230896 mm
+	Radius of beam at waist = 11.950538458990879 mm
+
+	Stability g-factor of cavity = 0.8350925761717987
+	Stability g-factor of first mirror = -1.0682523267838677
+	Stability g-factor of second mirror = -0.7817371937639199
+
+	Round-trip Gouy phase = 312.0813565565169 deg
+
+	Divergence angle = 0.0016237789746943276 deg
+```
+
+An extra feature of the API is the ability to use the `cavcalc.configure` function for overriding
+default behaviour. For example, in the script below we use this in a context-managed scope to
+temporarily use microns for any beam radius parameters, mm for distances, and GHz for any frequencies:
+
+```python
+import cavcalc as cc
+
+# Temporarily override units...
+with cc.configure(beamsizes="um", distances="mm", frequencies="GHz"):
+    out = cc.calculate(L=8, gouy=121)
+    print(out)
+
+# ... previous state (using loaded config options) will
+# be restored on exit from the with block above
+```
+
+resulting in:
+
+```
+Given:
+    Cavity length = 8 mm
+
+    Round-trip Gouy phase = 121 deg
+
+    Wavelength of beam = 1064 nm
+
+Computed:
+    FSR = 18.737028625 GHz
+    Mode separation frequency = 6.297723510069445 GHz
+
+    Position of beam waist (from first mirror) = 4.0 mm
+
+    Radius of curvature of both mirrors = 0.01576117284251957 m
+
+    Radius of beam at mirrors = 55.79464044247193 µm
+    Radius of beam at waist = 48.19739141432035 µm
+
+    Stability g-factor of cavity = 0.2424809625449729
+    Stability g-factor of both mirrors = 0.4924235601034671
+
+    Divergence angle = 0.40260921048107506 deg
+```
 
-setup(**setup_kwargs)
```

