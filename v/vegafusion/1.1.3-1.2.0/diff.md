# Comparing `tmp/vegafusion-1.1.3.tar.gz` & `tmp/vegafusion-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vegafusion-1.1.3.tar", last modified: Thu Apr  6 18:12:40 2023, max compression
+gzip compressed data, was "vegafusion-1.2.0.tar", last modified: Tue Apr 11 20:22:09 2023, max compression
```

## Comparing `vegafusion-1.1.3.tar` & `vegafusion-1.2.0.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:12:40.993816 vegafusion-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-06 18:11:41.000000 vegafusion-1.1.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-06 18:12:40.993816 vegafusion-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-06 18:11:41.000000 vegafusion-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-06 18:11:41.000000 vegafusion-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-06 18:12:40.993816 vegafusion-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 18:11:41.000000 vegafusion-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:12:40.989815 vegafusion-1.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-06 18:11:41.000000 vegafusion-1.1.3/tests/test_conext_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    18632 2023-04-06 18:11:41.000000 vegafusion-1.1.3/tests/test_input_utc.py
--rw-r--r--   0 runner    (1001) docker     (123)    31525 2023-04-06 18:11:41.000000 vegafusion-1.1.3/tests/test_pretransform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-04-06 18:11:41.000000 vegafusion-1.1.3/tests/test_pretransform_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-06 18:11:41.000000 vegafusion-1.1.3/tests/test_row_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-04-06 18:11:41.000000 vegafusion-1.1.3/tests/test_transformed_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-06 18:11:41.000000 vegafusion-1.1.3/tests/test_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:12:40.993816 vegafusion-1.1.3/vegafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-04-06 18:11:41.000000 vegafusion-1.1.3/vegafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-06 18:11:41.000000 vegafusion-1.1.3/vegafusion/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-06 18:11:41.000000 vegafusion-1.1.3/vegafusion/compilers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:12:40.993816 vegafusion-1.1.3/vegafusion/connection/
--rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-04-06 18:11:41.000000 vegafusion-1.1.3/vegafusion/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-04-06 18:11:41.000000 vegafusion-1.1.3/vegafusion/connection/duckdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-06 18:11:41.000000 vegafusion-1.1.3/vegafusion/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-06 18:11:41.000000 vegafusion-1.1.3/vegafusion/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-06 18:11:41.000000 vegafusion-1.1.3/vegafusion/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-06 18:11:41.000000 vegafusion-1.1.3/vegafusion/local_tz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-06 18:11:41.000000 vegafusion-1.1.3/vegafusion/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20434 2023-04-06 18:11:41.000000 vegafusion-1.1.3/vegafusion/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-04-06 18:11:41.000000 vegafusion-1.1.3/vegafusion/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-06 18:11:41.000000 vegafusion-1.1.3/vegafusion/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:12:40.993816 vegafusion-1.1.3/vegafusion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-06 18:12:40.000000 vegafusion-1.1.3/vegafusion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-06 18:12:40.000000 vegafusion-1.1.3/vegafusion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 18:12:40.000000 vegafusion-1.1.3/vegafusion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-06 18:12:40.000000 vegafusion-1.1.3/vegafusion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-06 18:12:40.000000 vegafusion-1.1.3/vegafusion.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:22:09.095437 vegafusion-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-11 20:21:07.000000 vegafusion-1.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-11 20:22:09.095437 vegafusion-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-11 20:21:07.000000 vegafusion-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-11 20:21:07.000000 vegafusion-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-11 20:22:09.095437 vegafusion-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 20:21:07.000000 vegafusion-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:22:09.091437 vegafusion-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-11 20:21:07.000000 vegafusion-1.2.0/tests/test_conext_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18632 2023-04-11 20:21:07.000000 vegafusion-1.2.0/tests/test_input_utc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32055 2023-04-11 20:21:07.000000 vegafusion-1.2.0/tests/test_pretransform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-04-11 20:21:07.000000 vegafusion-1.2.0/tests/test_pretransform_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-11 20:21:07.000000 vegafusion-1.2.0/tests/test_row_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-11 20:21:07.000000 vegafusion-1.2.0/tests/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-04-11 20:21:07.000000 vegafusion-1.2.0/tests/test_transformed_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-11 20:21:07.000000 vegafusion-1.2.0/tests/test_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:22:09.095437 vegafusion-1.2.0/vegafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-11 20:21:07.000000 vegafusion-1.2.0/vegafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 20:21:07.000000 vegafusion-1.2.0/vegafusion/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-11 20:21:07.000000 vegafusion-1.2.0/vegafusion/compilers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:22:09.095437 vegafusion-1.2.0/vegafusion/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-04-11 20:21:07.000000 vegafusion-1.2.0/vegafusion/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12895 2023-04-11 20:21:07.000000 vegafusion-1.2.0/vegafusion/connection/duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-11 20:21:07.000000 vegafusion-1.2.0/vegafusion/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-11 20:21:07.000000 vegafusion-1.2.0/vegafusion/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-11 20:21:07.000000 vegafusion-1.2.0/vegafusion/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-11 20:21:07.000000 vegafusion-1.2.0/vegafusion/local_tz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-11 20:21:07.000000 vegafusion-1.2.0/vegafusion/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20434 2023-04-11 20:21:07.000000 vegafusion-1.2.0/vegafusion/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-04-11 20:21:07.000000 vegafusion-1.2.0/vegafusion/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-04-11 20:21:07.000000 vegafusion-1.2.0/vegafusion/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-11 20:21:07.000000 vegafusion-1.2.0/vegafusion/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:22:09.095437 vegafusion-1.2.0/vegafusion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-11 20:22:09.000000 vegafusion-1.2.0/vegafusion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-11 20:22:09.000000 vegafusion-1.2.0/vegafusion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 20:22:09.000000 vegafusion-1.2.0/vegafusion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-11 20:22:09.000000 vegafusion-1.2.0/vegafusion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-11 20:22:09.000000 vegafusion-1.2.0/vegafusion.egg-info/top_level.txt
```

### Comparing `vegafusion-1.1.3/LICENSE.txt` & `vegafusion-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vegafusion-1.1.3/PKG-INFO` & `vegafusion-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vegafusion
-Version: 1.1.3
+Version: 1.2.0
 Summary: Core tools for using VegaFusion from Python
 License: BSD-3-Clause
 Keywords: vega,altair,vegafusion,arrow
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `vegafusion-1.1.3/README.md` & `vegafusion-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `vegafusion-1.1.3/setup.cfg` & `vegafusion-1.2.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [bdist_wheel]
 universal = 0
 
 [metadata]
 name = vegafusion
 description = Core tools for using VegaFusion from Python
-version = 1.1.3
+version = 1.2.0
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = vega, altair, vegafusion, arrow
 license = BSD-3-Clause
 license_file = LICENSE.txt
 python = "^3.7"
 homepage = "https://vegafusion.io"
@@ -30,14 +30,14 @@
 	altair>=4.2.0
 	pyarrow>=5
 	pandas
 	psutil
 
 [options.extras_require]
 embed = 
-	vegafusion-python-embed==1.1.3
+	vegafusion-python-embed==1.2.0
 	vl-convert-python>=0.7.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `vegafusion-1.1.3/tests/test_conext_manager.py` & `vegafusion-1.2.0/tests/test_conext_manager.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.1.3/tests/test_input_utc.py` & `vegafusion-1.2.0/tests/test_input_utc.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.1.3/tests/test_pretransform.py` & `vegafusion-1.2.0/tests/test_pretransform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1104,21 +1104,41 @@
             pd.Timestamp('2022-01-01 00:00:00', tz='UTC'),
             pd.Timestamp('2022-01-02 00:00:00', tz='UTC'),
             pd.Timestamp('2022-01-03 00:00:00', tz='UTC')
         ]
     finally:
         vf.runtime.set_connection("datafusion")
 
+
 def test_gh_268_hang():
     """
     Tests for hang reported in https://github.com/hex-inc/vegafusion/issues/268
     """
+    vf.runtime.set_connection("datafusion")
+    movies = pd.read_json("https://raw.githubusercontent.com/vega/vega-datasets/main/data/movies.json")
+    spec = gh_268_hang_spec()
+    for i in range(20):
+        # Break cache by removing one row each iteration
+        movies_inner = movies.iloc[i:]
+        vf.runtime.pre_transform_datasets(spec, ["data_3"], "UTC", inline_datasets=dict(movies_clean=movies_inner))
 
+
+def test_repeat_duckdb():
+    """
+    Tests for hang reported in https://github.com/hex-inc/vegafusion/issues/268
+    """
+    vf.runtime.set_connection("duckdb")
     movies = pd.read_json("https://raw.githubusercontent.com/vega/vega-datasets/main/data/movies.json")
-    spec = json.loads(r""" 
+    spec = gh_268_hang_spec()
+    for i in range(2):
+        vf.runtime.pre_transform_datasets(spec, ["data_3"], "UTC", inline_datasets=dict(movies_clean=movies))
+
+
+def gh_268_hang_spec():
+    return json.loads(r""" 
     {
       "$schema": "https://vega.github.io/schema/vega/v5.json",
       "data": [
         {
           "name": "interval_intervalselection__store"
         },
         {
@@ -1175,12 +1195,8 @@
               "type": "filter",
               "expr": "!length(data(\"legend_pointselection__store\")) || vlSelectionTest(\"legend_pointselection__store\", datum)"
             }
           ]
         }
       ]
     }
-    """)
-    for i in range(20):
-        # Break cache by removing one row each iteration
-        movies_inner = movies.iloc[i:]
-        vf.runtime.pre_transform_datasets(spec, ["data_3"], "UTC", inline_datasets=dict(movies_clean=movies_inner))
+    """)
```

### Comparing `vegafusion-1.1.3/tests/test_pretransform_specs.py` & `vegafusion-1.2.0/tests/test_pretransform_specs.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.1.3/tests/test_row_limit.py` & `vegafusion-1.2.0/tests/test_row_limit.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.1.3/tests/test_transformed_data.py` & `vegafusion-1.2.0/tests/test_transformed_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -127,22 +127,41 @@
         if dtype.kind == "M":
             assert dtype.tz == pytz.timezone(vf.get_local_tz())
 
     # Check expected length
     assert len(df) == expected_len
 
 
-def test_gh_286():
+@pytest.mark.parametrize("connection", get_connections())
+def test_gh_286(connection):
     # https://github.com/hex-inc/vegafusion/issues/286
+    vf.runtime.set_connection(connection)
     source = pl.from_pandas(data.seattle_weather())
 
     chart = alt.Chart(source).mark_bar(
         cornerRadiusTopLeft=3,
         cornerRadiusTopRight=3
     ).encode(
         x='month(date):O',
         y='count():Q',
         color='weather:N'
     )
     transformed = vf.transformed_data(chart)
     assert isinstance(transformed, pl.DataFrame)
     assert len(transformed) == 53
+
+
+@pytest.mark.parametrize("connection", get_connections())
+def test_categorical_columns(connection):
+    vf.runtime.set_connection(connection)
+
+    df = pd.DataFrame({
+        "a": [0, 1, 2, 3, 4, 5],
+        "categorical": pd.Categorical.from_codes([0, 1, 0, 1, 1, 0], ["A", "BB"])
+    })
+
+    chart = alt.Chart(df).mark_bar().encode(
+        alt.X("categorical:N"), alt.Y("sum(a):Q")
+    )
+    transformed = vf.transformed_data(chart)
+    expected = pd.DataFrame({"categorical": ["A", "BB"], "sum_a": [7, 8]})
+    pd.testing.assert_frame_equal(transformed, expected)
```

### Comparing `vegafusion-1.1.3/tests/test_transformer.py` & `vegafusion-1.2.0/tests/test_transformer.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.1.3/vegafusion/__init__.py` & `vegafusion-1.2.0/vegafusion/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # Please consult the license documentation provided alongside
 # this program the details of the active license.
 from .runtime import runtime
 from .transformer import to_feather, get_inline_datasets_for_spec
 from .renderer import RowLimitError
 from .local_tz import set_local_tz, get_local_tz
 from .evaluation import transformed_data
+from .save import save_html, save_vega, save_png, save_svg
 from . import renderer
 from .compilers import vegalite_compilers
 import altair as alt
 
 from ._version import __version__
 from .utils import RendererTransformerEnabler
 
@@ -40,15 +41,15 @@
 
     if vl_convert:
         # Compute VlConvert's vl_version string (of the form 'v5_2')
         # from SCHEMA_VERSION (of the form 'v5.2.0')
         return "_".join(SCHEMA_VERSION.split(".")[:2])
     else:
         # Return full version without leading v
-        return SCHEMA_VERSION.rstrip("v")
+        return SCHEMA_VERSION.lstrip("v")
 
 
 def enable(mimetype="html", row_limit=10000, embed_options=None):
     """
     Enable the VegaFusion mime renderer so that all Altair charts
     are displayed using VegaFusion.
```

### Comparing `vegafusion-1.1.3/vegafusion/compilers.py` & `vegafusion-1.2.0/vegafusion/compilers.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.1.3/vegafusion/connection/__init__.py` & `vegafusion-1.2.0/vegafusion/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.1.3/vegafusion/evaluation.py` & `vegafusion-1.2.0/vegafusion/evaluation.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.1.3/vegafusion/local_tz.py` & `vegafusion-1.2.0/vegafusion/local_tz.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.1.3/vegafusion/renderer.py` & `vegafusion-1.2.0/vegafusion/renderer.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,31 @@
             f"Limit of {self.row_limit} rows was exceeded.\n"
             "Either introduce an aggregation to reduce the number of rows sent to the client or\n"
             "increase the row_limit argument to the vegafusion.enable() function"
         )
 
 
 def vegafusion_mime_renderer(spec, mimetype="html", row_limit=None, embed_options=None):
+    return spec_to_mime_bundle(
+        spec,
+        mimetype=mimetype,
+        row_limit=row_limit,
+        embed_options=embed_options
+    )
+
+
+def spec_to_mime_bundle(
+        spec,
+        mimetype="html",
+        row_limit=None,
+        embed_options=None,
+        html_template="universal",
+        full_html=False,
+        scale=1,
+):
     from . import transformer, runtime, local_tz, vegalite_compilers, altair_vl_version
     vega_spec = vegalite_compilers.get()(spec)
 
     inline_datasets = transformer.get_inline_datasets_for_spec(vega_spec)
     tx_vega_spec, warnings = runtime.pre_transform_spec(
         vega_spec,
         local_tz.get_local_tz(),
@@ -45,26 +62,26 @@
         output_div = f"altair-viz-{uuid4().hex}"
         html = spec_to_html(
             tx_vega_spec,
             mode="vega",
             vega_version="5",
             vegalite_version=altair_vl_version(),
             vegaembed_version="6",
-            fullhtml=False,
+            fullhtml=full_html,
             output_div=output_div,
-            template="universal",
+            template=html_template,
             embed_options=embed_options
         )
         return {"text/html": html}
     elif mimetype == "svg":
         import vl_convert as vlc
         svg = vlc.vega_to_svg(tx_vega_spec)
         return {"image/svg+xml": svg}
     elif mimetype == "png":
         import vl_convert as vlc
-        png = vlc.vega_to_png(tx_vega_spec)
+        png = vlc.vega_to_png(tx_vega_spec, scale=scale)
         return {"image/png": png}
     else:
         raise ValueError(f"Unsupported mimetype: {mimetype}")
 
 
 alt.renderers.register('vegafusion-mime', vegafusion_mime_renderer)
```

### Comparing `vegafusion-1.1.3/vegafusion/runtime.py` & `vegafusion-1.2.0/vegafusion/runtime.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.1.3/vegafusion/transformer.py` & `vegafusion-1.2.0/vegafusion/transformer.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.1.3/vegafusion/utils.py` & `vegafusion-1.2.0/vegafusion/utils.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.1.3/vegafusion.egg-info/PKG-INFO` & `vegafusion-1.2.0/vegafusion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vegafusion
-Version: 1.1.3
+Version: 1.2.0
 Summary: Core tools for using VegaFusion from Python
 License: BSD-3-Clause
 Keywords: vega,altair,vegafusion,arrow
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `vegafusion-1.1.3/vegafusion.egg-info/SOURCES.txt` & `vegafusion-1.2.0/vegafusion.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 setup.cfg
 setup.py
 tests/test_conext_manager.py
 tests/test_input_utc.py
 tests/test_pretransform.py
 tests/test_pretransform_specs.py
 tests/test_row_limit.py
+tests/test_save.py
 tests/test_transformed_data.py
 tests/test_transformer.py
 vegafusion/__init__.py
 vegafusion/_version.py
 vegafusion/compilers.py
 vegafusion/embed.py
 vegafusion/evaluation.py
 vegafusion/jupyter.py
 vegafusion/local_tz.py
 vegafusion/renderer.py
 vegafusion/runtime.py
+vegafusion/save.py
 vegafusion/transformer.py
 vegafusion/utils.py
 vegafusion.egg-info/PKG-INFO
 vegafusion.egg-info/SOURCES.txt
 vegafusion.egg-info/dependency_links.txt
 vegafusion.egg-info/requires.txt
 vegafusion.egg-info/top_level.txt
```

