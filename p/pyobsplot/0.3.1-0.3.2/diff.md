# Comparing `tmp/pyobsplot-0.3.1.tar.gz` & `tmp/pyobsplot-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobsplot-0.3.1.tar", max compression
+gzip compressed data, was "pyobsplot-0.3.2.tar", max compression
```

## Comparing `pyobsplot-0.3.1.tar` & `pyobsplot-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1071 2023-03-29 08:42:01.834769 pyobsplot-0.3.1/LICENSE
--rw-r--r--   0        0        0     3816 2023-04-06 15:53:55.434769 pyobsplot-0.3.1/README.md
--rw-r--r--   0        0        0     1251 2023-04-06 16:14:11.004831 pyobsplot-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      535 2023-04-06 08:28:46.892341 pyobsplot-0.3.1/src/pyobsplot/__init__.py
--rw-r--r--   0        0        0     2553 2023-03-30 12:48:09.497135 pyobsplot-0.3.1/src/pyobsplot/data.py
--rw-r--r--   0        0        0     1810 2023-04-06 09:50:53.580377 pyobsplot-0.3.1/src/pyobsplot/jsdom.py
--rw-r--r--   0        0        0     1943 2023-04-06 14:50:12.511091 pyobsplot-0.3.1/src/pyobsplot/jsmodules.py
--rw-r--r--   0        0        0     3150 2023-04-06 10:10:11.360454 pyobsplot-0.3.1/src/pyobsplot/obsplot.py
--rw-r--r--   0        0        0     5511 2023-04-06 14:15:31.707100 pyobsplot-0.3.1/src/pyobsplot/parsing.py
--rw-r--r--   0        0        0       89 2023-04-06 16:25:33.736471 pyobsplot-0.3.1/src/pyobsplot/static/styles.css
--rw-r--r--   0        0        0  2268308 2023-04-06 16:25:33.736471 pyobsplot-0.3.1/src/pyobsplot/static/widget.js
--rw-r--r--   0        0        0      148 2023-04-05 14:06:25.509832 pyobsplot-0.3.1/src/pyobsplot/utils.py
--rw-r--r--   0        0        0     1067 2023-04-06 09:50:18.108129 pyobsplot-0.3.1/src/pyobsplot/widget.py
--rw-r--r--   0        0        0     5088 1970-01-01 00:00:00.000000 pyobsplot-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-03-29 08:42:01.834769 pyobsplot-0.3.2/LICENSE
+-rw-r--r--   0        0        0     3843 2023-04-08 15:49:45.532400 pyobsplot-0.3.2/README.md
+-rw-r--r--   0        0        0     1251 2023-04-12 09:10:42.356278 pyobsplot-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      535 2023-04-06 08:28:46.892341 pyobsplot-0.3.2/src/pyobsplot/__init__.py
+-rw-r--r--   0        0        0     3428 2023-04-11 14:13:06.230946 pyobsplot-0.3.2/src/pyobsplot/data.py
+-rw-r--r--   0        0        0     2045 2023-04-12 08:53:57.503120 pyobsplot-0.3.2/src/pyobsplot/jsdom.py
+-rw-r--r--   0        0        0     1963 2023-04-09 22:23:38.052708 pyobsplot-0.3.2/src/pyobsplot/jsmodules.py
+-rw-r--r--   0        0        0     3802 2023-04-09 22:23:38.052708 pyobsplot-0.3.2/src/pyobsplot/obsplot.py
+-rw-r--r--   0        0        0     6158 2023-04-11 14:11:53.254582 pyobsplot-0.3.2/src/pyobsplot/parsing.py
+-rw-r--r--   0        0        0       89 2023-04-12 09:12:28.362119 pyobsplot-0.3.2/src/pyobsplot/static/styles.css
+-rw-r--r--   0        0        0  2268272 2023-04-12 09:12:28.362119 pyobsplot-0.3.2/src/pyobsplot/static/widget.js
+-rw-r--r--   0        0        0      344 2023-04-09 22:23:38.084708 pyobsplot-0.3.2/src/pyobsplot/utils.py
+-rw-r--r--   0        0        0     1179 2023-04-09 22:23:38.084708 pyobsplot-0.3.2/src/pyobsplot/widget.py
+-rw-r--r--   0        0        0     5115 1970-01-01 00:00:00.000000 pyobsplot-0.3.2/PKG-INFO
```

### Comparing `pyobsplot-0.3.1/LICENSE` & `pyobsplot-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyobsplot-0.3.1/README.md` & `pyobsplot-0.3.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [![PyPI](https://img.shields.io/pypi/v/pyobsplot.svg?color=green)](https://pypi.org/project/pyobsplot)
 [![Tests](https://github.com/juba/pyobsplot/actions/workflows/tests.yml/badge.svg)](https://github.com/juba/pyobsplot/actions/workflows/tests.yml)
 [![Documentation](https://github.com/juba/pyobsplot/actions/workflows/publish.yml/badge.svg)](https://github.com/juba/pyobsplot/actions/workflows/publish.yml)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/juba/pyobsplot/blob/main/examples/introduction.ipynb)
 
 
-`pyobsplot` allows to use [Observable Plot](https://observablehq.com/@observablehq/plot?collection=@observablehq/plot) to create charts in Jupyter notebooks, VSCode notebooks, Google Colab and Quarto documents. Plots are created from Python code with a syntax as close as possible to the JavaScript one.
+`pyobsplot` allows to use [Observable Plot](https://observablehq.com/@observablehq/plot?collection=@observablehq/plot) to create charts in [Jupyter](https://jupyter.org) notebooks, [VSCode](https://code.visualstudio.com) notebooks, [Google Colab](https://colab.research.google.com) and [Quarto](https://quarto.org) documents. Plots are created from Python code with a syntax as close as possible to the JavaScript one.
 
 It allows to do things like :
 
 ```python
 import polars as pl
 from pyobsplot import Plot
 
@@ -72,8 +72,8 @@
 
 
 ## Credits
 
 - [Observable Plot](https://observablehq.com/@observablehq/plot?collection=@observablehq/plot), developed by [Mike Bostock](https://observablehq.com/@mbostock) and [Philippe Rivière](https://observablehq.com/@fil) among others.
 - The widget is developed thanks to the [anywidget](https://anywidget.dev) framework.
 - Some code from the `jsdom` renderer has been adapted from [altair_saver](https://github.com/altair-viz/altair_saver).
-- The documentation website is generated by [Quarto](https://quarto.org) and the [bookup](https://github.com/juba/bookup-html) custom format.
+- The documentation website is generated by [Quarto].
```

### Comparing `pyobsplot-0.3.1/pyproject.toml` & `pyobsplot-0.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyobsplot"
-version = "0.3.1"
+version = "0.3.2"
 description = "Observable Plot in Jupyter notebooks and Quarto documents"
 authors = ["Julien Barnier <julien@nozav.org>"]
 license = "MIT"
 readme = "README.md"
 include = ["src/pyobsplot/static/*"]
 homepage = "https://github.com/juba/pyobsplot"
 documentation = "https://juba.github.io/pyobsplot"
```

### Comparing `pyobsplot-0.3.1/src/pyobsplot/__init__.py` & `pyobsplot-0.3.2/src/pyobsplot/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobsplot-0.3.1/src/pyobsplot/jsdom.py` & `pyobsplot-0.3.2/src/pyobsplot/jsdom.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Obsplot jsdom handling.
 """
 
 import subprocess
+import os
 import json
 import shutil
 from IPython.display import HTML, SVG
 
 from typing import Any
 
 from .parsing import SpecParser
@@ -18,22 +19,23 @@
     The class takes a plot specification as input and generates a plot as SVG or HTML
     by calling a JSDom script with node.
 
     The specification can be given as a dict, a Plot function call or as
     Python kwargs.
     """
 
-    def __init__(self, spec: Any, debug: bool = False) -> None:
+    def __init__(self, spec: Any, default: dict = {}, debug: bool = False) -> None:
         """
         Constructor. Parse the spec given as argument.
         """
         # Create parser
-        parser = SpecParser("jsdom")
+        parser = SpecParser(renderer="jsdom", default=default)
         # Parse spec code
-        code = parser.parse(spec)
+        parser.spec = spec
+        code = parser.parse_spec()
         # Create spec object
         spec = {"data": parser.serialize_data(), "code": code, "debug": debug}
         self.spec = spec
 
     def plot(self):
         """Generates the plot by calling node script.
 
@@ -47,14 +49,17 @@
             raise RuntimeError("npx executable has not been found.")
         # Run node script with JSON spec as input
         p = subprocess.run(
             ["npx", "pyobsplot"],
             input=json.dumps(self.spec),
             capture_output=True,
             encoding="Utf8",
+            # Use shell=True if we are on Windows. Otherwise PATH
+            # is not parsed and npx is not found.
+            shell=os.name == "nt",
         )
         if p.returncode != 0:
             raise RuntimeError(
                 f"jsdom script error (${p.returncode}): ${p.stderr} - ${p.stdout}"
             )
         # Get script output
         out = p.stdout
```

### Comparing `pyobsplot-0.3.1/src/pyobsplot/jsmodules.py` & `pyobsplot-0.3.2/src/pyobsplot/jsmodules.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 class Plot(metaclass=JSModule):
     """JSModule class to allow Plot objects in specification."""
 
     @staticmethod
     def plot(*args, **kwargs) -> ObsplotWidget:
         """
         Plot.plot static method. If called directly, create an ObsplotWidget
-        with args and kwargs.
+        or an ObpsplotJsdom with args and kwargs.
         """
         if _plot_renderer == "widget":
             op = ObsplotWidgetCreator()
         if _plot_renderer == "jsdom":
             op = ObsplotJsdomCreator()
         return op(*args, **kwargs)
```

### Comparing `pyobsplot-0.3.1/src/pyobsplot/parsing.py` & `pyobsplot-0.3.2/src/pyobsplot/parsing.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,52 @@
 """
 Plot specification parsing.
 """
 
 import datetime
 import json
-import base64
 import pandas as pd
 import polars as pl
 
 from typing import Any, Optional
 
-from .data import pd_to_arrow, pl_to_arrow
+from .data import serialize
 
 
 class SpecParser:
     """
     Class implementing plot specification parsing.
     """
 
-    def __init__(self, renderer: str = "widget") -> None:
+    def __init__(self, renderer: str = "widget", default: dict = {}) -> None:
         """
         SpecParser constructor.
 
         Args:
             renderer(str): type of renderer ("widget" or "jsdom").
+            default(dict): dict of default spec values.
         """
         self.renderer = renderer
         self.data = []
+        self._spec = dict()
+        self._default = default
+
+    @property
+    def spec(self):
+        return self._spec
+
+    @spec.setter
+    def spec(self, value):
+        if (
+            "pyobsplot-type" in value
+            and value["pyobsplot-type"] == "function"
+            and value["module"] == "Plot"
+        ):
+            value = {"marks": [value]}
+        self._spec = value
 
     def cache_index(self, data: Any) -> Optional[int]:
         """Returns the index of a data object in the data cache.
 
         Args:
             data (Any): a data object (DataFeame, GeoJson...)
 
@@ -38,22 +54,53 @@
             Optional[int]: index of the data object in the cache, or None if absent.
         """
         index = [i for i, d in enumerate(self.data) if d is data]
         if len(index) == 1:
             return index[0]
         return None
 
+    def merge_default(self, spec: dict) -> dict:
+        """Merge SpecParser default spec values with an actual spec.
+
+        Args:
+            spec (dict): spec to update with default values.
+
+        Returns:
+            dict: merged spec.
+        """
+        default = self._default
+        for k in default:
+            if k not in spec:
+                spec[k] = default[k]
+        return spec
+
+    def parse_spec(self) -> dict:
+        """Start spec parsing from _spec attribute.
+
+        Args:
+            default (dict): default spec values defined during Creator creation.
+
+        Returns:
+            dict: parsed specification.
+        """
+        # Deep copy should not be needed and copy should be sufficient as
+        # merge_default only affects top-level elements.
+        spec = self.spec.copy()
+        spec = self.merge_default(spec)
+        return self.parse(spec)
+
     def parse(self, spec: Any) -> Any:
-        """Recursively parse a Plot specification to check and convert its elements.
+        """Recursively parse part of a Plot specification to check and convert
+        its elements.
 
         Args:
-            spec (Any): a complete specification or part of a specification.
+            spec (Any): part of a specification.
 
         Returns:
-            Any: parsed specification or part of a specification.
+            Any: parsed part of a specification.
         """
         if spec is None:
             return None
         # If list or tuple, recursively parse elements
         if isinstance(spec, (list, tuple)):
             return [self.parse(s) for s in spec]
         # If Geojson as string, parse as dict and continue parsing
@@ -67,14 +114,17 @@
         ):
             index = self.cache_index(spec)
             if index is None:
                 self.data.append(spec)
                 return {"pyobsplot-type": "GeoJson-ref", "value": (len(self.data) - 1)}
             else:
                 return {"pyobsplot-type": "GeoJson-ref", "value": index}
+        # If range, convert  to list
+        if isinstance(spec, range):
+            return self.parse(list(spec))
         # If dict, parse recursively
         if isinstance(spec, dict):
             return {k: self.parse(v) for k, v in spec.items()}
         # If pandas DataFrame, handle caching, add type and serialize to Arrow IPC
         if isinstance(spec, pd.DataFrame):
             index = self.cache_index(spec)
             if index is None:
@@ -119,32 +169,15 @@
 
     def serialize_data(self) -> list:
         """Serialize data in the data cache.
 
         Returns:
             list: list of serialized data objects.
         """
-        result = []
-        for d in self.data:
-            # If polars DataFrame, serialize to Arrow IPC
-            if isinstance(d, pl.DataFrame):
-                value = pl_to_arrow(d)
-                if self.renderer == "jsdom":
-                    value = base64.standard_b64encode(value).decode("ascii")
-                result.append({"pyobsplot-type": "DataFrame", "value": value})
-            # If pandas DataFrame, serialize to Arrow IPC
-            elif isinstance(d, pd.DataFrame):
-                value = pd_to_arrow(d)
-                if self.renderer == "jsdom":
-                    value = base64.standard_b64encode(value).decode("ascii")
-                result.append({"pyobsplot-type": "DataFrame", "value": value})
-            # Else, keep as is
-            else:
-                result.append(d)
-        return result
+        return [serialize(d, renderer=self.renderer) for d in self.data]
 
 
 def js(txt: str) -> dict:
     """Tag a string as JavaScript code.
 
     Args:
         txt (str): string containing JavaScript code.
```

### Comparing `pyobsplot-0.3.1/src/pyobsplot/static/widget.js` & `pyobsplot-0.3.2/src/pyobsplot/static/widget.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -82030,17 +82030,15 @@
 // js/pyobsplot-js/plot.js
 function generate_plot(spec, renderer) {
     let out;
     try {
         spec["data"] = unserialize_data(spec["data"], renderer);
         out = parse_spec(spec["code"], spec["data"]);
         if (spec["code"]["pyobsplot-type"] == "function") {
-            if (!(out instanceof Node)) {
-                out = out.plot();
-            }
+            out = out.plot();
         } else {
             if (spec["debug"]) {
                 console.log("--- start pyobsplot debugging output ---");
                 console.log(out);
                 console.log("--- end pyobsplot debugging output ---");
             }
             out = plot2(out);
@@ -82068,12 +82066,12 @@
     view.model.on("change:spec", () => _onValueChanged(view, view.el));
 }
 
 function _onValueChanged(view, el) {
     let plot3 = el.querySelector(".pyobsplot-plot");
     plot3.replaceChildren();
     let spec = () => view.model.get("spec");
-    plot3.appendChild(generate_plot(spec()));
+    plot3.appendChild(generate_plot(spec(), "widget"));
 }
 export {
     render
 };
```

### Comparing `pyobsplot-0.3.1/src/pyobsplot/widget.py` & `pyobsplot-0.3.2/src/pyobsplot/widget.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,20 +22,22 @@
     """
 
     _esm = bundler_output_dir / "widget.js"
     _css = bundler_output_dir / "styles.css"
     # spec traitlet : plot specification
     spec = traitlets.Dict().tag(sync=True)
 
-    def __init__(self, spec, debug: bool = False):
+    def __init__(self, spec, default: dict = {}, debug: bool = False):
         """Obsplot widget constructor."""
         self._debug = debug
+        self._default = default
         # Init widget
         super().__init__(spec=spec)
 
     @traitlets.validate("spec")
     def _validate_spec(self, proposal):
         spec = proposal["value"]
-        parser = SpecParser("widget")
-        code = parser.parse(spec)
+        parser = SpecParser(renderer="widget", default=self._default)
+        parser.spec = spec
+        code = parser.parse_spec()
         spec = {"data": parser.serialize_data(), "code": code, "debug": self._debug}
         return spec
```

### Comparing `pyobsplot-0.3.1/PKG-INFO` & `pyobsplot-0.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobsplot
-Version: 0.3.1
+Version: 0.3.2
 Summary: Observable Plot in Jupyter notebooks and Quarto documents
 Home-page: https://github.com/juba/pyobsplot
 License: MIT
 Author: Julien Barnier
 Author-email: julien@nozav.org
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -33,15 +33,15 @@
 
 [![PyPI](https://img.shields.io/pypi/v/pyobsplot.svg?color=green)](https://pypi.org/project/pyobsplot)
 [![Tests](https://github.com/juba/pyobsplot/actions/workflows/tests.yml/badge.svg)](https://github.com/juba/pyobsplot/actions/workflows/tests.yml)
 [![Documentation](https://github.com/juba/pyobsplot/actions/workflows/publish.yml/badge.svg)](https://github.com/juba/pyobsplot/actions/workflows/publish.yml)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/juba/pyobsplot/blob/main/examples/introduction.ipynb)
 
 
-`pyobsplot` allows to use [Observable Plot](https://observablehq.com/@observablehq/plot?collection=@observablehq/plot) to create charts in Jupyter notebooks, VSCode notebooks, Google Colab and Quarto documents. Plots are created from Python code with a syntax as close as possible to the JavaScript one.
+`pyobsplot` allows to use [Observable Plot](https://observablehq.com/@observablehq/plot?collection=@observablehq/plot) to create charts in [Jupyter](https://jupyter.org) notebooks, [VSCode](https://code.visualstudio.com) notebooks, [Google Colab](https://colab.research.google.com) and [Quarto](https://quarto.org) documents. Plots are created from Python code with a syntax as close as possible to the JavaScript one.
 
 It allows to do things like :
 
 ```python
 import polars as pl
 from pyobsplot import Plot
 
@@ -103,9 +103,9 @@
 
 
 ## Credits
 
 - [Observable Plot](https://observablehq.com/@observablehq/plot?collection=@observablehq/plot), developed by [Mike Bostock](https://observablehq.com/@mbostock) and [Philippe Rivière](https://observablehq.com/@fil) among others.
 - The widget is developed thanks to the [anywidget](https://anywidget.dev) framework.
 - Some code from the `jsdom` renderer has been adapted from [altair_saver](https://github.com/altair-viz/altair_saver).
-- The documentation website is generated by [Quarto](https://quarto.org) and the [bookup](https://github.com/juba/bookup-html) custom format.
+- The documentation website is generated by [Quarto].
```

