# Comparing `tmp/ssb_sgis-0.1.4.tar.gz` & `tmp/ssb_sgis-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_sgis-0.1.4.tar", max compression
+gzip compressed data, was "ssb_sgis-0.1.5.tar", max compression
```

## Comparing `ssb_sgis-0.1.4.tar` & `ssb_sgis-0.1.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1074 2023-04-11 16:36:33.486727 ssb_sgis-0.1.4/LICENSE
--rw-r--r--   0        0        0     7070 2023-04-11 16:36:48.967527 ssb_sgis-0.1.4/README.md
--rw-r--r--   0        0        0     2484 2023-04-11 16:36:48.991528 ssb_sgis-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1651 2023-04-11 16:36:48.991528 ssb_sgis-0.1.4/src/sgis/__init__.py
--rw-r--r--   0        0        0     2634 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/dapla.py
--rw-r--r--   0        0        0      666 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/geopandas_tools/__init__.py
--rw-r--r--   0        0        0     8776 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/geopandas_tools/buffer_dissolve_explode.py
--rw-r--r--   0        0        0    27301 2023-04-11 16:36:48.991528 ssb_sgis-0.1.4/src/sgis/geopandas_tools/general.py
--rw-r--r--   0        0        0     5456 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/geopandas_tools/geometry_types.py
--rw-r--r--   0        0        0    34762 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/geopandas_tools/line_operations.py
--rw-r--r--   0        0        0    16647 2023-04-11 16:36:48.991528 ssb_sgis-0.1.4/src/sgis/geopandas_tools/neighbors.py
--rw-r--r--   0        0        0    14044 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/geopandas_tools/overlay.py
--rw-r--r--   0        0        0     6316 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/geopandas_tools/point_operations.py
--rw-r--r--   0        0        0     5046 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/geopandas_tools/polygon_operations.py
--rw-r--r--   0        0        0     2468 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/helpers.py
--rw-r--r--   0        0        0        0 2023-04-11 16:36:48.991528 ssb_sgis-0.1.4/src/sgis/maps/__init__.py
--rw-r--r--   0        0        0    21371 2023-04-11 16:36:48.991528 ssb_sgis-0.1.4/src/sgis/maps/explore.py
--rw-r--r--   0        0        0    17271 2023-04-11 16:36:48.991528 ssb_sgis-0.1.4/src/sgis/maps/legend.py
--rw-r--r--   0        0        0    16587 2023-04-11 16:36:48.991528 ssb_sgis-0.1.4/src/sgis/maps/map.py
--rw-r--r--   0        0        0    12535 2023-04-11 16:36:48.991528 ssb_sgis-0.1.4/src/sgis/maps/maps.py
--rw-r--r--   0        0        0    11182 2023-04-11 16:36:48.991528 ssb_sgis-0.1.4/src/sgis/maps/thematicmap.py
--rw-r--r--   0        0        0        0 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/networkanalysis/__init__.py
--rw-r--r--   0        0        0     5171 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/networkanalysis/_get_route.py
--rw-r--r--   0        0        0     2521 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/networkanalysis/_od_cost_matrix.py
--rw-r--r--   0        0        0     4819 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/networkanalysis/_points.py
--rw-r--r--   0        0        0     4426 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/networkanalysis/_service_area.py
--rw-r--r--   0        0        0    11360 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/networkanalysis/directednetwork.py
--rw-r--r--   0        0        0    23953 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/networkanalysis/network.py
--rw-r--r--   0        0        0     6124 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/networkanalysis/network_norway.py
--rw-r--r--   0        0        0    58054 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/networkanalysis/networkanalysis.py
--rw-r--r--   0        0        0    12655 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/networkanalysis/networkanalysisrules.py
--rw-r--r--   0        0        0        0 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/py.typed
--rw-r--r--   0        0        0     3765 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/read_parquet.py
--rw-r--r--   0        0        0     8441 1970-01-01 00:00:00.000000 ssb_sgis-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-12 19:35:11.603711 ssb_sgis-0.1.5/LICENSE
+-rw-r--r--   0        0        0     7070 2023-04-12 19:35:11.603711 ssb_sgis-0.1.5/README.md
+-rw-r--r--   0        0        0     2477 2023-04-12 19:35:28.572292 ssb_sgis-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1651 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/__init__.py
+-rw-r--r--   0        0        0     2634 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/dapla.py
+-rw-r--r--   0        0        0      666 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/geopandas_tools/__init__.py
+-rw-r--r--   0        0        0     8776 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/geopandas_tools/buffer_dissolve_explode.py
+-rw-r--r--   0        0        0    27649 2023-04-12 19:35:28.576292 ssb_sgis-0.1.5/src/sgis/geopandas_tools/general.py
+-rw-r--r--   0        0        0     5456 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/geopandas_tools/geometry_types.py
+-rw-r--r--   0        0        0    34762 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/geopandas_tools/line_operations.py
+-rw-r--r--   0        0        0    16647 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/geopandas_tools/neighbors.py
+-rw-r--r--   0        0        0    14435 2023-04-12 19:35:28.576292 ssb_sgis-0.1.5/src/sgis/geopandas_tools/overlay.py
+-rw-r--r--   0        0        0     6316 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/geopandas_tools/point_operations.py
+-rw-r--r--   0        0        0     5046 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/geopandas_tools/polygon_operations.py
+-rw-r--r--   0        0        0     2468 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/helpers.py
+-rw-r--r--   0        0        0        0 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/maps/__init__.py
+-rw-r--r--   0        0        0    23159 2023-04-12 19:35:28.576292 ssb_sgis-0.1.5/src/sgis/maps/explore.py
+-rw-r--r--   0        0        0    20458 2023-04-12 19:35:28.576292 ssb_sgis-0.1.5/src/sgis/maps/legend.py
+-rw-r--r--   0        0        0    16402 2023-04-12 19:35:28.576292 ssb_sgis-0.1.5/src/sgis/maps/map.py
+-rw-r--r--   0        0        0    12564 2023-04-12 19:35:28.576292 ssb_sgis-0.1.5/src/sgis/maps/maps.py
+-rw-r--r--   0        0        0    13220 2023-04-12 19:35:28.576292 ssb_sgis-0.1.5/src/sgis/maps/thematicmap.py
+-rw-r--r--   0        0        0        0 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/networkanalysis/__init__.py
+-rw-r--r--   0        0        0     5171 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/networkanalysis/_get_route.py
+-rw-r--r--   0        0        0     2521 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/networkanalysis/_od_cost_matrix.py
+-rw-r--r--   0        0        0     4819 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/networkanalysis/_points.py
+-rw-r--r--   0        0        0     4426 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/networkanalysis/_service_area.py
+-rw-r--r--   0        0        0    11360 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/networkanalysis/directednetwork.py
+-rw-r--r--   0        0        0    23953 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/networkanalysis/network.py
+-rw-r--r--   0        0        0     6124 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/networkanalysis/network_norway.py
+-rw-r--r--   0        0        0    58054 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/networkanalysis/networkanalysis.py
+-rw-r--r--   0        0        0    12655 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/networkanalysis/networkanalysisrules.py
+-rw-r--r--   0        0        0        0 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/py.typed
+-rw-r--r--   0        0        0     3765 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/read_parquet.py
+-rw-r--r--   0        0        0     8434 1970-01-01 00:00:00.000000 ssb_sgis-0.1.5/PKG-INFO
```

### Comparing `ssb_sgis-0.1.4/LICENSE` & `ssb_sgis-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.4/README.md` & `ssb_sgis-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.4/pyproject.toml` & `ssb_sgis-0.1.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "ssb-sgis"
-version = "0.1.4"
-description = "GIS utility functions used at Statistics Norway."
+version = "0.1.5"
+description = "GIS functions used at Statistics Norway."
 authors = ["Statistics Norway <ort@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "sgis", from = "src"}]
 homepage = "https://github.com/statisticsnorway/ssb-sgis"
 repository = "https://github.com/statisticsnorway/ssb-sgis"
 classifiers = [
@@ -13,15 +13,15 @@
     "Topic :: Scientific/Engineering :: GIS",
 ]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/statisticsnorway/ssb-sgis/releases"
 
 [tool.poetry.dependencies]
-python = ">=3.10,<4.0"
+python = ">=3.10,<3.12"
 branca = "^0.6.0"
 folium = "^0.14.0"
 geopandas = "^0.12.2"
 igraph = "^0.10.4"
 mapclassify = "^2.5.0"
 matplotlib = "^3.7.0"
 networkx = "^3.0"
```

### Comparing `ssb_sgis-0.1.4/src/sgis/__init__.py` & `ssb_sgis-0.1.5/src/sgis/__init__.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.4/src/sgis/dapla.py` & `ssb_sgis-0.1.5/src/sgis/dapla.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.4/src/sgis/exceptions.py` & `ssb_sgis-0.1.5/src/sgis/exceptions.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.4/src/sgis/geopandas_tools/buffer_dissolve_explode.py` & `ssb_sgis-0.1.5/src/sgis/geopandas_tools/buffer_dissolve_explode.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.4/src/sgis/geopandas_tools/general.py` & `ssb_sgis-0.1.5/src/sgis/geopandas_tools/general.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,15 +230,15 @@
 
     Returns:
         A GeoDataFrame of points with 'n' rows per row in 'gdf'. It uses the index
         values of 'gdf'.
 
     Examples
     --------
-    Buffer 100 random points.
+    First create and buffer 100 random points.
 
     >>> import sgis as sg
     >>> gdf = sg.random_points(100)
     >>> polygons = sg.buff(gdf, 1)
     >>> polygons
                                                  geometry
     0   POLYGON ((1.49436 0.36088, 1.49387 0.32947, 1....
@@ -307,17 +307,30 @@
 
             overlapping_indices = overlapping_indices + tuple(overlapping.index.values)
 
             gdf__ = gdf.loc[~gdf["temp_idx____"].isin(overlapping_indices)]
             bounds = gdf__.bounds
             temp_idx____ = gdf__["temp_idx____"].values
 
+    all_points = all_points.sort_index().drop(["temp_idx____", "index_right"], axis=1)
+
+    if gdf.index.is_unique:
+        gdf = gdf.drop("temp_idx____", axis=1)
+        return all_points
+
+    original_index = {
+        temp_idx: idx for temp_idx, idx in zip(gdf.temp_idx____, gdf.index)
+    }
+
+    all_points.index = all_points.index.map(original_index)
+    all_points.index.name = None
+
     gdf = gdf.drop("temp_idx____", axis=1)
 
-    return all_points.sort_index().drop(["temp_idx____", "index_right"], axis=1)
+    return all_points
 
 
 def points_in_bounds(gdf: GeoDataFrame, n2: int):
     minx, miny, maxx, maxy = gdf.total_bounds
     xs = np.linspace(minx, maxx, num=n2)
     ys = np.linspace(miny, maxy, num=n2)
     x_coords, y_coords = np.meshgrid(xs, ys, indexing="ij")
```

### Comparing `ssb_sgis-0.1.4/src/sgis/geopandas_tools/geometry_types.py` & `ssb_sgis-0.1.5/src/sgis/geopandas_tools/geometry_types.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.4/src/sgis/geopandas_tools/line_operations.py` & `ssb_sgis-0.1.5/src/sgis/geopandas_tools/line_operations.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.4/src/sgis/geopandas_tools/neighbors.py` & `ssb_sgis-0.1.5/src/sgis/geopandas_tools/neighbors.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.4/src/sgis/geopandas_tools/overlay.py` & `ssb_sgis-0.1.5/src/sgis/geopandas_tools/overlay.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,17 @@
     ]
     # Error Messages
     if how not in allowed_hows:
         raise ValueError(
             f"'how' was {how!r} but is expected to be in {', '.join(allowed_hows)}"
         )
 
+    if df1.crs != df2.crs:
+        raise ValueError(f"crs mismatch. Got {df1.crs} and {df2.crs}")
+
     df1 = clean_geoms(df1)
     df2 = clean_geoms(df2)
 
     geom_type_left, geom_type_right = _get_geom_type_left_right(geom_type)
 
     if geom_type_left:
         df1 = to_single_geom_type(df1, geom_type=geom_type_left)
@@ -291,46 +294,54 @@
 def _union(pairs, df1, df2, left, right):
     merged = []
     if len(left):
         intersections = _intersection(pairs)
         merged.append(intersections)
     symmdiff = _symmetric_difference(pairs, df1, df2, left, right)
     merged.append(symmdiff)
+    crs = merged[0].crs
+    merged = [gdf.to_crs(crs) for gdf in merged]
     return pd.concat(merged, ignore_index=True).pipe(_push_geom_col)
 
 
 def _identity(pairs, df1, left):
     merged = []
     if len(left):
         intersections = _intersection(pairs)
         merged.append(intersections)
     diff = _difference(pairs, df1, left)
     merged.append(diff)
+    crs = merged[0].crs
+    merged = [gdf.to_crs(crs) for gdf in merged]
     return pd.concat(merged, ignore_index=True).pipe(_push_geom_col)
 
 
 def _symmetric_difference(pairs, df1, df2, left, right):
     merged = []
     difference_left = _difference(pairs, df1, left)
     merged.append(difference_left)
     if len(left):
         clip_right = _shapely_diffclip_right(pairs, df1, df2)
         merged.append(clip_right)
     diff_right = _add_from_right(df1, df2, right)
     merged.append(diff_right)
+    crs = merged[0].crs
+    merged = [gdf.to_crs(crs) for gdf in merged]
     return pd.concat(merged, ignore_index=True).pipe(_push_geom_col)
 
 
 def _difference(pairs, df1, left):
     merged = []
     if len(left):
         clip_left = _shapely_diffclip_left(pairs, df1)
         merged.append(clip_left)
     diff_left = _add_from_left(df1, left)
     merged.append(diff_left)
+    crs = merged[0].crs
+    merged = [gdf.to_crs(crs) for gdf in merged]
     return pd.concat(merged, ignore_index=True).pipe(_push_geom_col)
 
 
 def _get_intersects_pairs(
     df1: GeoDataFrame, df2: GeoDataFrame, left: np.ndarray, right: np.ndarray
 ) -> GeoDataFrame:
     return pd.concat(
```

### Comparing `ssb_sgis-0.1.4/src/sgis/geopandas_tools/point_operations.py` & `ssb_sgis-0.1.5/src/sgis/geopandas_tools/point_operations.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.4/src/sgis/geopandas_tools/polygon_operations.py` & `ssb_sgis-0.1.5/src/sgis/geopandas_tools/polygon_operations.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.4/src/sgis/helpers.py` & `ssb_sgis-0.1.5/src/sgis/helpers.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.4/src/sgis/maps/explore.py` & `ssb_sgis-0.1.5/src/sgis/maps/explore.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 """
 import warnings
 from statistics import mean
 
 import branca as bc
 import folium
 import matplotlib
+import numpy as np
 import pandas as pd
 from geopandas import GeoDataFrame
 from shapely.geometry import LineString
 
 from ..geopandas_tools.general import clean_geoms, random_points_in_polygons
 from ..geopandas_tools.geometry_types import get_geom_type
 from .map import Map
@@ -26,15 +27,15 @@
 
 
 # gray for NaNs
 NAN_COLOR = "#969696"
 
 
 # cols to not show when hovering over geometries (tooltip)
-COLS_TO_DROP = ["color", "geometry"]
+COLS_TO_DROP = ["color", "col_as_int", "geometry"]
 
 
 # from geopandas
 _MAP_KWARGS = [
     "location",
     "prefer_canvas",
     "no_touch",
@@ -67,15 +68,21 @@
         **kwargs,
     ):
         super().__init__(*gdfs, column=column, **kwargs)
         self.popup = popup
         self.max_zoom = max_zoom
         self.show_in_browser = show_in_browser
 
-        if not self._is_categorical:
+        if any(get_geom_type(gdf) == "mixed" for gdf in self.gdfs):
+            self._make_all_polygon()
+
+        if self._is_categorical:
+            if len(self.gdfs) == 1:
+                self._split_categories()
+        else:
             if not self._cmap:
                 self._cmap = "viridis"
             self.cmap_start = kwargs.pop("cmap_start", 0)
             self.cmap_stop = kwargs.pop("cmap_stop", 256)
 
     def explore(self, column: str | None = None, **kwargs) -> None:
         """Interactive map of the GeoDataFrames with layers that can be toggles on/off.
@@ -218,41 +225,76 @@
             self._column = column
             self._update_column()
             kwargs.pop("column", None)
 
         gdfs: tuple[GeoDataFrame] = ()
         for gdf in self._gdfs:
             gdf = gdf.clip(mask)
+            collections = gdf.loc[gdf.geom_type == "GeometryCollection"]
+            if len(collections):
+                collections = collections.explode(index_parts=False)
+                gdf = pd.concat([gdf, collections], ignore_index=False)
             gdfs = gdfs + (gdf,)
         self._gdfs = gdfs
         self._gdf = pd.concat(gdfs, ignore_index=True)
         self._explore(**kwargs)
 
-    def _update_column(self):
-        self._is_categorical = self._check_if_categorical()
-        self._fill_missings()
-        self._gdf = pd.concat(self._gdfs, ignore_index=True)
-
     def _explore(self, **kwargs):
         self.kwargs = self.kwargs | kwargs
 
         if self._is_categorical:
             self._create_categorical_map()
         else:
             self._create_continous_map()
 
         if self.show_in_browser:
             self.map.show_in_browser()
         else:
             display(self.map)
 
+    def _split_categories(self):
+        new_gdfs, new_labels = [], []
+        for cat in self._unique_values:
+            gdf = self.gdf.loc[self.gdf[self.column] == cat]
+            new_gdfs.append(gdf)
+            new_labels.append(cat)
+        self._gdfs = new_gdfs
+        self._gdf = pd.concat(new_gdfs, ignore_index=True)
+        self.labels = new_labels
+
+    def _make_all_polygon(self):
+        """Buffer gdf if mixed geometry types
+
+        Because Folium does not handle GeometryCollection well
+        """
+
+        new_gdfs = []
+        for gdf in self.gdfs:
+            if get_geom_type(gdf) == "mixed":
+                gdf[gdf._geometry_column_name] = gdf.buffer(0.1)
+            new_gdfs.append(gdf)
+        self._gdfs = new_gdfs
+        self._gdf = pd.concat(new_gdfs, ignore_index=True)
+        self._nan_idx = self._gdf[self._column].isna()
+
+    def _update_column(self):
+        self._is_categorical = self._check_if_categorical()
+        self._fill_missings()
+        self._gdf = pd.concat(self._gdfs, ignore_index=True)
+
     def _create_categorical_map(self):
         self._get_categorical_colors()
 
-        self.map = self._explore_return(self._gdf, return_="empty_map", **self.kwargs)
+        self.map = self._explore_return(
+            self._gdf,
+            return_="empty_map",
+            max_zoom=self.max_zoom,
+            popup=self.popup,
+            **self.kwargs,
+        )
 
         for gdf, label in zip(self._gdfs, self.labels, strict=True):
             if not len(gdf):
                 continue
             f = folium.FeatureGroup(name=label)
 
             gjs = self._explore_return(
@@ -276,43 +318,49 @@
         )
         folium.TileLayer("stamentoner").add_to(self.map)
         folium.TileLayer("cartodbdark_matter").add_to(self.map)
         self.map.add_child(folium.LayerControl())
 
     def _create_continous_map(self):
         self._prepare_continous_map()
-        self.colorlist = self._get_continous_colors()
-        self.colors = self._classify_from_bins(self._gdf)
+        if self.scheme:
+            classified = self._classify_from_bins(self._gdf, bins=self.bins)
+            classified_sequential = self._push_classification(classified)
+            n_colors = len(np.unique(classified_sequential)) - any(self._nan_idx)
+            unique_colors = self._get_continous_colors(n=n_colors)
 
         self.map = self._explore_return(
             self._gdf,
             return_="empty_map",
+            max_zoom=self.max_zoom,
+            popup=self.popup,
             **self.kwargs,
         )
 
         colorbar = bc.colormap.StepColormap(
-            self.colorlist,
+            unique_colors,
             vmin=self._gdf[self._column].min(),
             vmax=self._gdf[self._column].max(),
             caption=self._column,
             index=self.bins,
             #  **colormap_kwds,
         )
 
         for gdf, label in zip(self._gdfs, self.labels, strict=True):
             if not len(gdf):
                 continue
             f = folium.FeatureGroup(name=label)
 
-            self.colors = self._classify_from_bins(gdf)
+            classified = self._classify_from_bins(gdf, bins=self.bins)
+            colorarray = unique_colors[classified]
 
             gjs = self._explore_return(
                 gdf,
                 tooltip=self._tooltip_cols(gdf),
-                color=self.colors,
+                color=colorarray,
                 return_="geojson",
                 **{key: value for key, value in self.kwargs.items() if key != "title"},
             )
             f.add_child(gjs)
             self.map.add_child(f)
 
         self.map.add_child(colorbar)
@@ -411,15 +459,15 @@
                     tiles = xyzservices.providers.query_name(tiles)
                 except ValueError:
                     pass
 
             if isinstance(tiles, xyzservices.TileProvider):
                 attr = attr if attr else tiles.html_attribution
                 map_kwds["min_zoom"] = tiles.get("min_zoom", 0)
-                map_kwds["max_zoom"] = tiles.get("max_zoom", 18)
+                map_kwds["max_zoom"] = tiles.get("max_zoom", 30)
                 tiles = tiles.build_url(scale_factor="{r}")
 
             m = folium.Map(
                 location=location,
                 control_scale=control_scale,
                 tiles=tiles,
                 attr=attr,
```

### Comparing `ssb_sgis-0.1.4/src/sgis/maps/legend.py` & `ssb_sgis-0.1.5/src/sgis/maps/legend.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,56 @@
 """Attributes of the legend of the ThematicMap class.
 
 The Legend class is best accessed through the 'legend' attribute of the ThematicMap
 class.
 
 """
 import warnings
-from statistics import mean
 
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-from geopandas import GeoDataFrame
 from matplotlib.lines import Line2D
 from pandas import Series
 
-from ..geopandas_tools.general import points_in_bounds, to_gdf
-from ..geopandas_tools.point_operations import snap_all
+from ..geopandas_tools.general import points_in_bounds
 
 
 # the geopandas._explore raises a deprication warning. Ignoring for now.
 warnings.filterwarnings(
     action="ignore", category=matplotlib.MatplotlibDeprecationWarning
 )
 pd.options.mode.chained_assignment = None
 
 
 class Legend:
-    """Holds the attributes of the legend in the ThematicMap class.
+    """Holds the general attributes of the legend in the ThematicMap class.
 
-    This class is stored in the 'legend' attribute of the ThematicMap class.
+    This class holds attributes of the 'legend' attribute of the ThematicMap class.
     The fontsize, title_fontsize and markersize attributes are adjusted
     according to the size attribute of the ThematicMap.
 
-    The attributes 'label_suffix', 'label_sep' and 'rounding' only apply to plots
-    of numeric columns.
-
-    The 'labels' attribute can be used to set labels manually. By default, the
-    maximum and minimum values of each color group is used as label for numeric
-    columns. For categorical columns, the column values are used.
+    If a numeric column is used, additional attributes can be found in the
+    ContinousLegend class.
 
     Attributes:
         title: Legend title. Defaults to the column name if used in the
             ThematicMap class.
-        labels: To manually set labels for the color groups. Must be a list/tuple of
-            same length as the number of color groups (k).
         position: The legend's x and y position in the plot, specified as a tuple of
             x and y position between 0 and 1. E.g. position=(0.8, 0.2) for a position
             in the bottom right corner, (0.2, 0.8) for the upper left corner.
         fontsize: Text size of the legend labels. Defaults to the size of
             the ThematicMap class.
         title_fontsize: Text size of the legend title. Defaults to the
             size * 1.2 of the ThematicMap class.
         markersize: Size of the color circles in the legend. Defaults to the size of
             the ThematicMap class.
         framealpha: Transparency of the legend background.
         edgecolor: Color of the legend border. Defaults to #0f0f0f (almost black).
-        label_suffix: For numeric columns. The text to put after each number in the
-            legend labels.
-        label_sep: For numeric columns. Text to put in between the two numbers in each
-            color group in the legend.
-        rounding: For numeric columns. Number of decimals in the legend labels. By
-            default the rounding depends on the column's maximum value and standard
-            deviation.
         kwargs: Stores additional keyword arguments taken by the matplotlib legend
             method. Specify this as e.g. m.legend.kwargs["labelcolor"] = "red", where
             'm' is the name of the ThematicMap instance. See here:
             https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.legend.html
 
     Examples
     --------
@@ -84,53 +68,48 @@
     4  POINT (0.47373 0.20040)       4
     5  POINT (0.98661 0.15614)       5
     6  POINT (0.30951 0.77057)       6
     7  POINT (0.47802 0.52824)       7
     8  POINT (0.12215 0.96588)       8
     9  POINT (0.02938 0.93467)       9
 
-    Creating the ThematicMap instance.
+    Creating the ThematicMap instance will also create the legend. Since we
+    specify a numeric column, a ContinousLegend instance is created.
 
     >>> m = sg.ThematicMap(points, column="number")
+    >>> m.legend
+    <sgis.maps.legend.ContinousLegend object at 0x00000222206738D0>
 
     Changing the attributes that apply to both numeric and categorical columns.
 
     >>> m.legend.title = "Meters"
     >>> m.legend.title_fontsize = 11
     >>> m.legend.fontsize = 9
     >>> m.legend.markersize = 7.5
     >>> m.legend.position = (0.35, 0.28)
-    >>> m.legend.kwargs["labelcolor"] = "red"
     >>> m.plot()
 
-    Changing the additional attributes that only apply only to numeric columns.
+    Additional matplotlib keyword arguments can be specified as kwargs.
+
+    >>> m.legend.kwargs["labelcolor"] = "red"
+
+    Since we are using a numeric column, the legend is of type ContinousLegend.
+    We can therefore also access the attributes that only apply to numeric columns.
 
-    >>> m = sg.ThematicMap(points, column="number")
     >>> m.label_sep = "to"
     >>> m.label_suffix = "num"
     >>> m.rounding = 2
     >>> m.plot()
 
-    The final attribute, labels, should be changed along with the bins attribute
-    of the ThematicMap class. The following bins will create a plot with the color
-    groups 0-2, 3-5, 6-7 and 8-9. The legend labels can then be set accordingly.
-
-    >>> m.bins = [2, 5, 7]
-    >>> m.legend.labels = ["0 to 2 num", "3 to 5 num", "6 to 7 num", "8 to 9 num"]
-    >>> m.plot()
-
     """
 
     def __init__(
         self,
         title: str | None = None,
         labels: list[str] | None = None,
-        label_suffix: str = "",
-        label_sep: str = "-",
-        rounding: int | None = None,
         position: tuple[float] | None = None,
         markersize: int | None = None,
         fontsize: int | None = None,
         title_fontsize: int | None = None,
         framealpha: float = 1.0,
         edgecolor: str = "#0f0f0f",
         **kwargs,
@@ -148,22 +127,18 @@
         self.framealpha = framealpha
         self.edgecolor = edgecolor
         self.width = kwargs.pop("width", 0.1)
         self.height = kwargs.pop("height", 0.1)
         self.title_color = kwargs.pop("title_color", None)
         self.labelspacing = kwargs.pop("labelspacing", 0.8)
 
-        self.label_suffix = label_suffix
-        self.label_sep = label_sep
         self.labels = labels
-        self._rounding = rounding
         self._position = position
         self.kwargs = kwargs
         self._position_has_been_set = True if position else False
-        self._rounding_has_been_set = True if rounding else False
 
     def _get_legend_sizes(self, size, kwargs):
         """Adjust fontsize and markersize to size kwarg."""
 
         if "title_fontsize" in kwargs:
             self._title_fontsize = kwargs["title_fontsize"]
             self._title_fontsize_has_been_set = True
@@ -178,136 +153,27 @@
 
         if "markersize" in kwargs:
             self._markersize = kwargs["markersize"]
             self._markersize_has_been_set = True
         else:
             self._markersize = size
 
-    def _get_rounding(self, array: Series | np.ndarray) -> int:
-        def isinteger(x):
-            return np.equal(np.mod(x, 1), 0)
-
-        if np.all(isinteger(array)):
-            return 0
-        if np.max(array) > 30 and np.std(array) > 5:
-            return 0
-        if np.max(array) > 5 and np.std(array) > 1:
-            return 1
-        if np.max(array) > 1 and np.std(array) > 0.1:
-            return 2
-        return int(abs(np.log10(np.std(array)))) + 1
-
-    @staticmethod
-    def _set_rounding(bins, rounding: int | float):
-        if rounding == 0:
-            return [int(round(bin, 0)) for bin in bins]
-        else:
-            return [round(bin, rounding) for bin in bins]
-
-    def _remove_max_legend_value(self):
-        if not self._legend:
-            raise ValueError("Cannot modify legend before it is created.")
-
-    def _actually_add_continous_legend(
-        self,
-        ax,
-        bins: list[float],
-        colors: list[str],
-        nan_label: str,
-        bin_values: dict,
-    ):
-        for attr in self.__dict__.keys():
-            if attr in self.kwargs:
-                self[attr] = self.kwargs.pop(attr)
-
-        self._patches, self._categories = [], []
-
-        for color in colors:
-            self._patches.append(
-                Line2D(
-                    [0],
-                    [0],
-                    linestyle="none",
-                    marker="o",
-                    alpha=self.kwargs.get("alpha", 1),
-                    markersize=self._markersize,
-                    markerfacecolor=color,
-                    markeredgewidth=0,
-                )
-            )
-
-        if self.labels:
-            if len(self.labels) != len(colors):
-                raise ValueError(
-                    f"Label list must be same length as 'k'. Got k={len(colors)} and "
-                    f"labels={len(self.labels)}"
-                )
-            self._categories = self.labels
-
-        elif len(bins) == len(colors):
-            for i, _ in enumerate(bins):
-                min_ = np.min(bin_values[i])
-                max_ = np.max(bin_values[i])
-                min_rounded = self._set_rounding([min_], self._rounding)[0]
-                max_rounded = self._set_rounding([max_], self._rounding)[0]
-                if min_ == max_:
-                    self._categories.append(f"{min_rounded} {self.label_suffix}")
-                else:
-                    self._categories.append(
-                        f"{min_rounded} {self.label_suffix} {self.label_sep} "
-                        f"{max_rounded} {self.label_suffix}"
-                    )
-
-        else:
-            for i, (cat1, cat2) in enumerate(zip(bins[:-1], bins[1:], strict=True)):
-                if nan_label in str(cat1) or nan_label in str(cat2):
-                    self._categories.append(nan_label)
-                else:
-                    min_ = np.min(bin_values[i])
-                    max_ = np.max(bin_values[i])
-                    min_rounded = self._set_rounding([min_], self._rounding)[0]
-                    max_rounded = self._set_rounding([max_], self._rounding)[0]
-                    if min_ == max_:
-                        self._categories.append(f"{min_rounded} {self.label_suffix}")
-                    else:
-                        self._categories.append(
-                            f"{min_rounded} {self.label_suffix} {self.label_sep} "
-                            f"{max_rounded} {self.label_suffix}"
-                        )
-
-        legend = ax.legend(
-            self._patches,
-            self._categories,
-            fontsize=self._fontsize,
-            title=self.title,
-            title_fontsize=self._title_fontsize,
-            bbox_to_anchor=self._position + (self.width, self.height),
-            fancybox=False,
-            framealpha=self.framealpha,
-            edgecolor=self.edgecolor,
-            labelspacing=self.labelspacing,
-            **self.kwargs,
-        )
-
-        if self.title_color:
-            plt.setp(legend.get_title(), color=self.title_color)
-
-        return ax
-
     def _actually_add_categorical_legend(
         self, ax, categories_colors: dict, nan_label: str
     ):
         for attr in self.__dict__.keys():
             if attr in self.kwargs:
                 self[attr] = self.kwargs.pop(attr)
 
+        # swap column values with label values if labels is dict
         if self.labels and isinstance(self.labels, dict):
             categories_colors = {
                 self.labels[cat]: color for cat, color in categories_colors.items()
             }
+        # swap column values with label list and hope it's in the correct order
         elif self.labels:
             categories_colors = {
                 label: color
                 for label, color in zip(
                     self.labels, categories_colors.values(), strict=True
                 )
             }
@@ -376,14 +242,17 @@
         besty_01 = 0.0375 * k if besty_01 < 0.5 else 1
 
         return bestx_01, besty_01
 
     def __getitem__(self, item):
         return getattr(self, item)
 
+    def __setitem__(self, key, value):
+        setattr(self, key, value)
+
     def get(self, key, default=None):
         try:
             return self[key]
         except (KeyError, ValueError, IndexError, AttributeError):
             return default
 
     @property
@@ -392,23 +261,14 @@
 
     @position.setter
     def position(self, new_value: bool):
         self._position = new_value
         self._position_has_been_set = True
 
     @property
-    def rounding(self):
-        return self._rounding
-
-    @rounding.setter
-    def rounding(self, new_value: bool):
-        self._rounding = new_value
-        self._rounding_has_been_set = True
-
-    @property
     def title_fontsize(self):
         return self._title_fontsize
 
     @title_fontsize.setter
     def title_fontsize(self, new_value: bool):
         self._title_fontsize = new_value
         self._title_fontsize_has_been_set = True
@@ -428,62 +288,299 @@
 
     @markersize.setter
     def markersize(self, new_value: bool):
         self._markersize = new_value
         self._markersize_has_been_set = True
 
 
-class _ContinousLegend(Legend):
+class ContinousLegend(Legend):
     """Holds the legend attributes specific to numeric columns.
 
-    This class is stored in the 'legend' attribute of the ThematicMap class.
-    The fontsize, title_fontsize and markersize attributes are adjusted
-    according to the size attribute of the ThematicMap.
-
-    The 'labels' attribute can be used to set labels manually. By default, the
-    maximum and minimum values of each color group is used as label.
+    The attributes consern the labeling of the groups in the legend.
+    Labels can be set manually with the 'labels' attribute, or the format
+    of the labels can be changed with the remaining attributes.
 
     Attributes:
-        labels: To manually set labels for the color groups. Must be a list/tuple of
-            same length as the number of color groups (k).
-        label_suffix: For numeric columns. The text to put after each number in the
-            legend labels.
-        label_sep: For numeric columns. Text to put in between the two numbers in each
-            color group in the legend.
-        rounding: Number of decimals for numeric columns. By default the rounding
-            depends on the column's
+        labels: To manually set labels. If set, all other labeling attributes are
+            ignored. Should be given as a list of strings with the same length as
+            the number of color groups.
+        pretty_labels: If False (default), the minimum and maximum values of each
+            color group will be used as legend labels. If True, the labels will end
+            with the maximum value, but start at 1 + the maximum value of the previous
+            group. The labels will be correct but inaccurate.
+        label_suffix: The text to put after each number in the legend labels.
+            Defaults to None.
+        label_sep: Text to put in between the two numbers in each color group in
+            the legend. Defaults to '-'.
+        rounding: Number of decimals in the labels. By default, the rounding
+            depends on the column's maximum value and standard deviation.
+            OBS: The bins will not be rounded, meaning the labels might be wrong
+            if not bins are set manually.
+        thousand_sep: Separator between each thousand for large numbers. Defaults to
+            None, meaning no separator.
+        decimal_mark: Text to use as decimal point. Defaults to None, meaning '.' (dot)
+            unless 'thousand_sep' is '.'. In this case, ',' (comma) will be used as
+            decimal mark.
 
     Examples
     --------
-    """
+    Create ten random points with a numeric column from 0 to 9.
 
-    pass
+    >>> import sgis as sg
+    >>> points = sg.random_points(10)
+    >>> points["number"] = range(10)
+    >>> points
+                    geometry  number
+    0  POINT (0.59780 0.50425)       0
+    1  POINT (0.07019 0.26167)       1
+    2  POINT (0.56475 0.15422)       2
+    3  POINT (0.87293 0.60316)       3
+    4  POINT (0.47373 0.20040)       4
+    5  POINT (0.98661 0.15614)       5
+    6  POINT (0.30951 0.77057)       6
+    7  POINT (0.47802 0.52824)       7
+    8  POINT (0.12215 0.96588)       8
+    9  POINT (0.02938 0.93467)       9
 
+    Creating the ThematicMap instance with a numeric column.
 
-class _CategoricalLegend(Legend):
-    """Holds the attributes of the legend in the ThematicMap class.
+    >>> m = sg.ThematicMap(points, column="number")
 
-    This class is stored in the 'legend' attribute of the ThematicMap class.
-    The fontsize, title_fontsize and markersize attributes are adjusted
-    according to the size attribute of the ThematicMap.
+    Changing the attributes that apply to both numeric and categorical columns.
 
-    Attributes:
-        title: Legend title. Defaults to the column name if used in the
-            ThematicMap class.
-        position: The legend's x and y position in the plot, specified as a tuple of
-            x and y position between 0 and 1. E.g. position=(0.8, 0.2) for a position
-            in the bottom right corner, (0.2, 0.8) for the upper left corner.
-        fontsize: Text size of the legend labels. Defaults to the size of
-            the ThematicMap class.
-        title_fontsize: Text size of the legend title. Defaults to the
-            size * 1.2 of the ThematicMap class.
-        markersize: Size of the color circles in the legend. Defaults to the size of
-            the ThematicMap class.
-        kwargs: Stores additional keyword arguments taken by the matplotlib legend
-            method. Specify this as e.g. m.legend.kwargs["labelcolor"] = "red", where
-            'm' is the name of the ThematicMap instance.
+    >>> m.legend.title = "Meters"
+    >>> m.legend.position = (0.35, 0.28)
+
+    Change the attributes that only apply to numeric columns.
+
+    >>> m.label_sep = "to"
+    >>> m.label_suffix = "num"
+    >>> m.rounding = 2
+    >>> m.plot()
+
+    Setting labels manually. For better control, it might be wise to also set the bins
+    manually. The following bins will create a plot with the color groups
+    0-2, 3-5, 6-7 and 8-9. The legend labels can then be set accordingly.
+
+    >>> m = sg.ThematicMap(points, column="number")
+    >>> m.bins = [0, 2, 5, 7, 9]
+    >>> m.legend.labels = ["0 to 2 num", "3 to 5 num", "6 to 7 num", "8 to 9 num"]
+    >>> m.plot()
+
+    We will get the same groups if we exclude the first and last bin values. The
+    minimum and maximum values will be filled anyway.
+
+    >>> m = sg.ThematicMap(points, column="number")
+    >>> m.bins = [2, 5, 7]
+    >>> m.legend.labels = ["0 to 2 num", "3 to 5 num", "6 to 7 num", "8 to 9 num"]
+    >>> m.plot()
 
-    Examples
-    --------
     """
 
-    pass
+    def __init__(
+        self,
+        labels: list[str] | None = None,
+        pretty_labels: bool = False,
+        label_suffix: str | None = None,
+        label_sep: str = "-",
+        rounding: int | None = None,
+        thousand_sep: str | None = None,
+        decimal_mark: str | None = None,
+        **kwargs,
+    ):
+        super().__init__(**kwargs)
+
+        self.pretty_labels = pretty_labels
+        self.thousand_sep = thousand_sep
+        self.decimal_mark = decimal_mark
+
+        self.label_sep = label_sep
+        self.label_suffix = "" if not label_suffix else label_suffix
+        self._rounding = rounding
+        self._rounding_has_been_set = True if rounding else False
+
+    def _get_rounding(self, array: Series | np.ndarray) -> int:
+        def isinteger(x):
+            return np.equal(np.mod(x, 1), 0)
+
+        if np.all(isinteger(array)):
+            return 0
+
+        closest_to_zero_idx = np.argmin(np.abs(array))
+        closest_to_zero = np.abs(array[closest_to_zero_idx])
+
+        between_1_and_0 = 1 > closest_to_zero > 0
+        if between_1_and_0:
+            return int(abs(np.log10(abs(closest_to_zero)))) + 1
+
+        std_ = np.std(array)
+        max_ = np.max(array)
+        if max_ > 30 and std_ > 5:
+            return 0
+        if max_ > 5 and std_ > 1:
+            return 1
+        if max_ > 1 and std_ > 0.1:
+            return 2
+        return int(abs(np.log10(std_))) + 1
+
+    @staticmethod
+    def _set_rounding(bins, rounding: int | float):
+        if rounding == 0:
+            return [int(round(bin, 0)) for bin in bins]
+        else:
+            return [round(bin, rounding) for bin in bins]
+
+    def _remove_max_legend_value(self):
+        if not self._legend:
+            raise ValueError("Cannot modify legend before it is created.")
+
+    def _actually_add_continous_legend(
+        self,
+        ax,
+        bins: list[float],
+        colors: list[str],
+        nan_label: str,
+        bin_values: dict,
+    ):
+        # TODO: clean up this messy method
+
+        for attr in self.__dict__.keys():
+            if attr in self.kwargs:
+                self[attr] = self.kwargs.pop(attr)
+
+        self._patches, self._categories = [], []
+
+        for color in colors:
+            self._patches.append(
+                Line2D(
+                    [0],
+                    [0],
+                    linestyle="none",
+                    marker="o",
+                    alpha=self.kwargs.get("alpha", 1),
+                    markersize=self._markersize,
+                    markerfacecolor=color,
+                    markeredgewidth=0,
+                )
+            )
+
+        if self.labels:
+            if len(self.labels) != len(colors):
+                raise ValueError(
+                    "Label list must be same length as the number of groups. "
+                    f"Got k={len(colors)} and labels={len(colors)}."
+                    f"labels: {', '.join(self.labels)}"
+                    f"colors: {', '.join(colors)}"
+                )
+            self._categories = self.labels
+
+        elif len(bins) == len(colors):
+            for i, _ in enumerate(bins):
+                min_ = np.min(bin_values[i])
+                max_ = np.max(bin_values[i])
+                min_rounded = self._set_rounding([min_], self._rounding)[0]
+                max_rounded = self._set_rounding([max_], self._rounding)[0]
+                if min_ == max_:
+                    self._categories.append(f"{min_rounded} {self.label_suffix}")
+                else:
+                    self._categories.append(
+                        f"{min_rounded} {self.label_suffix} {self.label_sep} "
+                        f"{max_rounded} {self.label_suffix}"
+                    )
+
+        else:
+            for i, (cat1, cat2) in enumerate(zip(bins[:-1], bins[1:], strict=True)):
+                if nan_label in str(cat1) or nan_label in str(cat2):
+                    self._categories.append(nan_label)
+                    continue
+
+                min_ = np.min(bin_values[i])
+                max_ = np.max(bin_values[i])
+                min_rounded = self._set_rounding([min_], self._rounding)[0]
+                max_rounded = self._set_rounding([max_], self._rounding)[0]
+                if self.pretty_labels:
+                    if i != 0 and self._rounding == 0:
+                        cat1 = int(cat1 + 1)
+                    elif i != 0:
+                        cat1 = cat1 + float(f"1e-{self._rounding}")
+
+                    cat1 = self._format_number(cat1)
+                    cat2 = self._format_number(cat2)
+
+                    if min_ == max_:
+                        label = self._two_value_label(cat1, cat2)
+                        self._categories.append(label)
+                        continue
+
+                    label = self._two_value_label(cat1, cat2)
+                    self._categories.append(label)
+
+                elif min_ == max_:
+                    min_rounded = self._format_number(min_rounded)
+                    label = self._one_value_label(min_rounded)
+                    self._categories.append(label)
+                else:
+                    min_rounded = self._format_number(min_rounded)
+                    max_rounded = self._format_number(max_rounded)
+                    label = self._two_value_label(min_rounded, max_rounded)
+                    self._categories.append(label)
+
+        legend = ax.legend(
+            self._patches,
+            self._categories,
+            fontsize=self._fontsize,
+            title=self.title,
+            title_fontsize=self._title_fontsize,
+            bbox_to_anchor=self._position + (self.width, self.height),
+            fancybox=False,
+            framealpha=self.framealpha,
+            edgecolor=self.edgecolor,
+            labelspacing=self.labelspacing,
+            **self.kwargs,
+        )
+
+        if self.title_color:
+            plt.setp(legend.get_title(), color=self.title_color)
+
+        return ax
+
+    def _two_value_label(self, value1, value2):
+        return (
+            f"{value1} {self.label_suffix} {self.label_sep} "
+            f"{value2} {self.label_suffix}"
+        )
+
+    def _one_value_label(self, value1):
+        return f"{value1} {self.label_suffix}"
+
+    def _format_number(self, number):
+        if not self.thousand_sep and not self.decimal_mark:
+            return number
+
+        if self.thousand_sep:
+            number = f"{number:,}".replace(",", "*temp_thousand*")
+
+        if self.decimal_mark:
+            number = str(number).replace(".", "*temp_decimal*")
+
+        if self.thousand_sep == "." and not self.decimal_mark:
+            number = number.replace(".", ",").replace(
+                "*temp_thousand*", self.thousand_sep
+            )
+        elif not self.thousand_sep:
+            number = number.replace("*temp_decimal*", self.decimal_mark)
+        elif not self.decimal_mark:
+            number = number.replace("*temp_thousand*", self.thousand_sep)
+        else:
+            number = number.replace("*temp_thousand*", self.thousand_sep).replace(
+                "*temp_decimal*", self.decimal_mark
+            )
+        return number
+
+    @property
+    def rounding(self):
+        return self._rounding
+
+    @rounding.setter
+    def rounding(self, new_value: bool):
+        self._rounding = new_value
+        self._rounding_has_been_set = True
```

### Comparing `ssb_sgis-0.1.4/src/sgis/maps/map.py` & `ssb_sgis-0.1.5/src/sgis/maps/map.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,61 +115,76 @@
             if self._k > len(self._unique_values):
                 self._k = len(self._unique_values)
         else:
             self._unique_values = sorted(
                 list(self._gdf.loc[~self._nan_idx, self._column].unique())
             )
 
-    def _get_unique_floats(self) -> list[int | float]:
-        """Converting floats to large integers, then getting unique values.
+    def _get_unique_floats(self) -> np.array:
+        """Get unique floats by multiplying, then converting to integer.
 
-        Also making a column of the large integers to use in the bin classifying later.
+        Find a multiplier that makes the max value greater than +- 1_000_000.
+        Because floats don't always equal each other. This will make very
+        similar values count as the same value in the color classification.
         """
         array = self._gdf.loc[~self._nan_idx, self._column]
 
-        self._gdf["col_as_int"] = self._array_to_large_int(array)
+        self._min = np.min(array)
+        self._max = np.max(array)
+        self._get_multiplier(array)
 
         unique = array.reset_index(drop=True).drop_duplicates()
-
         as_int = self._array_to_large_int(unique)
         no_duplicates = as_int.drop_duplicates()
-        return list(sorted(unique.loc[no_duplicates.index]))
 
-    @staticmethod
-    def _array_to_large_int(array: np.ndarray):
+        return np.sort(np.array(unique.loc[no_duplicates.index]))
+
+    def _array_to_large_int(self, array: np.ndarray):
         """Multiply values in float array, then convert to integer."""
-        max_ = np.max(array)
-        min_ = np.min(array)
 
-        if max_ > 1 or min_ < -1:
-            unique_multiplied = array * np.emath.logn(1.25, np.abs(np.mean(array)) + 1)
-        else:
-            unique_multiplied = array
-            while max_ < 1_000_000:
-                unique_multiplied = unique_multiplied * 10
-                max_ = np.max(unique_multiplied)
+        unique_multiplied = array * self._multiplier
 
         return unique_multiplied.astype(np.int64)
 
+    def _get_multiplier(self, array: np.ndarray):
+        """Find the number of zeros needed to push the max value of the array above
+        +-1_000_000.
+
+        Adding this as an attribute to use later in _classify_from_bins.
+        """
+        multiplier = 10
+        max_ = np.max(array * multiplier)
+
+        if self._max > 0:
+            while max_ < 1_000_000:
+                multiplier *= 10
+                max_ = np.max(array * multiplier)
+        else:
+            while max_ > -1_000_000:
+                multiplier *= 10
+                max_ = np.max(array * multiplier)
+
+        self._multiplier: int = multiplier
+
     def _add_minmax_to_bins(self, bins: list[float | int]) -> list[float | int]:
         """If values are outside the bin range, add max and/or min values of array."""
         # make sure they are lists
         bins = [bin for bin in bins]
 
-        if min(bins) > 0 and min(self._gdf[self._column]) < min(bins) * 0.999:
-            bins = [min(self._gdf[self._column]) * 0.9999] + bins
+        if min(bins) > 0 and min(self._gdf[self._column]) < min(bins):
+            bins = [min(self._gdf[self._column])] + bins
 
-        if min(bins) < 0 and min(self._gdf[self._column]) < min(bins) * 1.0001:
-            bins = [min(self._gdf[self._column]) * 1.0001] + bins
+        if min(bins) < 0 and min(self._gdf[self._column]) < min(bins):
+            bins = [min(self._gdf[self._column])] + bins
 
-        if max(bins) > 0 and max(self._gdf[self._column]) > max(bins) * 1.0001:
-            bins = bins + [max(self._gdf[self._column]) * 1.0001]
+        if max(bins) > 0 and max(self._gdf[self._column]) > max(bins):
+            bins = bins + [max(self._gdf[self._column])]
 
-        if max(bins) < 0 and max(self._gdf[self._column]) < max(bins) * 1.0001:
-            bins = bins + [max(self._gdf[self._column]) * 1.0001]
+        if max(bins) < 0 and max(self._gdf[self._column]) < max(bins):
+            bins = bins + [max(self._gdf[self._column])]
 
         return bins
 
     @staticmethod
     def _separate_args(
         args: tuple,
         column: str | None,
@@ -190,25 +205,24 @@
 
         return gdfs, column
 
     def _prepare_continous_map(self):
         """Create bins if not already done and adjust k if needed."""
 
         if not hasattr(self, "scheme"):
-            self.scheme = self.kwargs.get("scheme", "fisherjenks")
+            self.scheme = self.kwargs.pop("scheme", "fisherjenks")
 
         if self.scheme is None:
             return
 
         if not self.bins:
             self.bins = self._create_bins(self._gdf, self._column)
             if len(self.bins) <= self._k and len(self.bins) != len(self._unique_values):
                 warnings.warn(f"Could not create {self._k} classes.")
                 self._k = len(self.bins)
-            self.bins = self._add_minmax_to_bins(self.bins)
         else:
             self.bins = self._add_minmax_to_bins(self.bins)
             if len(self._unique_values) > len(self.bins):
                 self._k = len(self.bins) - 1
 
     def _get_labels(self, gdfs: tuple[GeoDataFrame]) -> None:
         """Putting the labels/names in a list before copying the gdfs."""
@@ -281,18 +295,18 @@
             self._column = "area"
             return False
         if maybe_length > 1:
             self._column = "length"
             return False
 
         if all_nan == len(self._gdfs):
-            raise ValueError(f"All values are NaN in column {self.kwargs['column']!r}.")
+            raise ValueError(f"All values are NaN in column {self.column!r}.")
 
         if col_not_present == len(self._gdfs):
-            raise ValueError(f"{self.kwargs['column']} not found.")
+            raise ValueError(f"{self.column} not found.")
 
         return False
 
     def _get_categorical_colors(self) -> None:
         # custom categorical cmap
         if not self._cmap and len(self._unique_values) <= len(_CATEGORICAL_CMAP):
             self._categories_colors_dict = {
@@ -319,65 +333,51 @@
             self._categories_colors_dict[self.nan_label] = self.nan_color
 
         for gdf in self._gdfs:
             gdf["color"] = gdf[self._column].map(self._categories_colors_dict)
 
         self._gdf["color"] = self._gdf[self._column].map(self._categories_colors_dict)
 
-    def _create_bins(self, gdf, column) -> np.ndarray:
+    def _create_bins(self, gdf: GeoDataFrame, column: str) -> np.ndarray:
         """Make bin list of length k + 1, or length of unique values.
 
         The returned bins sometimes have two almost identical
 
         If 'scheme' is not specified, the jenks_breaks function is used, which is
         much faster than the one from Mapclassifier.
         """
 
-        if hasattr(self, "scheme"):
-            scheme = self.scheme
-        else:
-            scheme = self.kwargs.get("scheme", "fisherjenks")
-
-        if scheme is None:
-            return
-
         n_classes = (
             self._k if len(self._unique_values) > self._k else len(self._unique_values)
         )
 
         if self._k == len(self._unique_values) - 1:
             n_classes = self._k - 1
 
-        if scheme == "fisherjenks":
+        if self.scheme == "fisherjenks":
             bins = jenks_breaks(gdf.loc[~self._nan_idx, column], n_classes=n_classes)
         else:
             binning = classify(
                 np.asarray(gdf.loc[~self._nan_idx, column]),
-                scheme=scheme,
+                scheme=self.scheme,
                 k=self._k,
             )
             bins = binning.bins
             bins = self._add_minmax_to_bins(bins)
 
         unique_bins = list({round(bin, 5) for bin in bins})
         unique_bins.sort()
 
         if self._k == len(self._unique_values) - 1:
             return np.array(unique_bins)
 
         if len(unique_bins) == len(self._unique_values):
             return np.array(unique_bins)
 
-        binarray = np.array(bins)
-        binarray = np.where(
-            binarray > 0,
-            binarray + binarray / 100_000,
-            binarray - binarray / 100_000,
-        )
-        return binarray
+        return np.array(bins)
 
     def change_cmap(self, cmap: str, start: int = 0, stop: int = 256):
         """Change the color palette of the plot.
 
         Args:
             cmap: The colormap.
                 https://matplotlib.org/stable/tutorials/colors/colormaps.html
@@ -387,55 +387,50 @@
         """
         self.cmap_start = start
         self.cmap_stop = stop
         self._cmap = cmap
         self._cmap_has_been_set = True
         return self
 
-    def _get_continous_colors(self) -> list[str]:
+    def _get_continous_colors(self, n: int) -> np.ndarray:
         cmap = matplotlib.colormaps.get_cmap(self._cmap)
         colors_ = [
             colors.to_hex(cmap(int(i)))
-            for i in np.linspace(self.cmap_start, self.cmap_stop, num=self._k)
+            #            for i in np.linspace(self.cmap_start, self.cmap_stop, num=self._k)
+            for i in np.linspace(self.cmap_start, self.cmap_stop, num=n)
         ]
         if any(self._nan_idx):
             colors_ = colors_ + [self.nan_color]
-        return colors_
+        return np.array(colors_)
 
-    def _classify_from_bins(self, gdf: GeoDataFrame) -> np.ndarray:
-        """Place the values of the column into groups."""
-        # if equal lenght, use integer column to check for equality
-        # since long floats are unpredictable
-        if len(self.bins) == len(self._unique_values):
-            if "col_as_int" not in gdf.columns:
-                gdf["col_as_int"] = self._array_to_large_int(gdf[self._column])
-            bins = np.array(sorted(gdf["col_as_int"].unique()))
+    def _classify_from_bins(self, gdf: GeoDataFrame, bins: np.ndarray) -> np.ndarray:
+        """Place the column values into groups."""
+        if len(bins) == len(self._unique_values):
+            # if equal lenght, convert to integer and check for equality
+            gdf["col_as_int"] = self._array_to_large_int(gdf[self._column])
+            bins = self._array_to_large_int(self._unique_values)
             classified = np.searchsorted(bins, gdf["col_as_int"])
         else:
-            if any(self._nan_idx) and len(self.bins) == len(self.colorlist):
-                bins = self.bins[1:]
-            elif not any(self._nan_idx) and len(self.bins) == len(self.colorlist) + 1:
-                bins = self.bins[1:]
-            else:
-                bins = self.bins
+            if len(bins) == self._k + 1:
+                bins = bins[1:]
 
             classified = np.searchsorted(bins, gdf[self._column])
 
-        # storing unique values to use in legend labels
-        self._bins_unique_values = {
-            i: list(set(gdf.loc[classified == i, self._column]))
-            for i, _ in enumerate(bins)
-        }
+        return classified
 
-        colors_ = np.array(self.colorlist)
+    def _push_classification(self, classified: np.ndarray) -> np.ndarray:
+        """Push classes downwards if gaps in classification sequence.
 
-        # nans are sorted to the end, so nans will get NAN_COLOR
-        colors_classified = colors_[classified]
+        So from e.g. [0,2,4] to [0,1,2].
+
+        Otherwise, will get index error when classifying colors.
+        """
+        rank_dict = {val: rank for rank, val in enumerate(np.unique(classified))}
 
-        return colors_classified
+        return np.array([rank_dict[val] for val in classified])
 
     @property
     def k(self):
         return self._k
 
     @k.setter
     def k(self, new_value: bool):
```

### Comparing `ssb_sgis-0.1.4/src/sgis/maps/maps.py` & `ssb_sgis-0.1.5/src/sgis/maps/maps.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 The main function is 'explore', which displays one of more GeoDataFrames together in an
 interactive map with layers that can be toggled on and off. The 'samplemap' and
 'clipmap' functions do the same, but displays a random and chosen area respectfully.
 
 The 'qtm' function shows a static map of one or more GeoDataFrames.
 """
 from geopandas import GeoDataFrame, GeoSeries
-from matplotlib.axes._axes import Axes
-from matplotlib.figure import Figure
 from shapely import Geometry
 
 from ..exceptions import NotInJupyterError
 from ..geopandas_tools.general import random_points_in_polygons
 from ..geopandas_tools.geometry_types import get_geom_type
 from ..helpers import make_namedict
 from .explore import Explore
@@ -295,14 +293,15 @@
     column: str | None = None,
     title: str | None = None,
     black: bool = True,
     size: int = 10,
     legend: bool = True,
     cmap: str | None = None,
     k: int = 5,
+    **kwargs,
 ) -> None:
     """Quick, thematic map of one or more GeoDataFrames.
 
     Shows one or more GeoDataFrames in the same plot, with a common color scheme if
     column is specified, otherwise with unique colors for each GeoDataFrame.
 
     The 'qtm' name is taken from the tmap package in R.
@@ -316,26 +315,27 @@
             white. If False, it will be the opposite. The colormap will also be
             'viridis' when black, and 'RdPu' when white.
         size: Size of the plot. Defaults to 10.
         title_fontsize: Size of the title.
         cmap: Color palette of the map. See:
             https://matplotlib.org/stable/tutorials/colors/colormaps.html
         k: Number of color groups.
+        **kwargs: Additional keyword arguments taken by the geopandas plot method.
 
     See also:
         ThematicMap: Class with more options for customising the plot.
     """
 
     m = ThematicMap(*gdfs, column=column, size=size, black=black)
 
     m.title = title
 
-    if k and len(m._unique_values) >= 6:
+    if k and len(m._unique_values) >= k:
         m.k = k
 
     if cmap:
         m.cmap = cmap
 
     if not legend:
         m.legend = None
 
-    m.plot()
+    m.plot(**kwargs)
```

### Comparing `ssb_sgis-0.1.4/src/sgis/maps/thematicmap.py` & `ssb_sgis-0.1.5/src/sgis/maps/thematicmap.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Creating static maps with geopandas and matplotlib."""
 import warnings
 
 import matplotlib
 import matplotlib.pyplot as plt
+import numpy as np
 import pandas as pd
 from geopandas import GeoDataFrame
 
-from .legend import Legend
+from .legend import ContinousLegend, Legend
 from .map import Map
 
 
 # the geopandas._explore raises a deprication warning. Ignoring for now.
 warnings.filterwarnings(
     action="ignore", category=matplotlib.MatplotlibDeprecationWarning
 )
@@ -99,15 +100,15 @@
         self._title_fontsize = self._size * 2
 
         self.black = black
 
         if not self._is_categorical:
             self._choose_cmap()
 
-        self._add_legend()
+        self._create_legend()
 
     def change_cmap(self, cmap: str, start: int = 0, stop: int = 256):
         """Change the color palette of the plot.
 
         Args:
             cmap: The colormap.
                 https://matplotlib.org/stable/tutorials/colors/colormaps.html
@@ -135,125 +136,183 @@
                 [self._background_gdfs, gdf], ignore_index=True
             )
         self.minx, self.miny, self.maxx, self.maxy = self._gdf.total_bounds
         self.diffx = self.maxx - self.minx
         self.diffy = self.maxy - self.miny
         return self
 
-    def plot(self) -> None:
+    def plot(self, **kwargs) -> None:
         """Creates the final plot.
 
         This method should be run after customising the map, but before saving.
         """
 
+        include_legend = bool(kwargs.pop("legend", self.legend))
+
+        self._prepare_plot(**kwargs)
+
+        if "color" in kwargs:
+            kwargs["column"] = self.column
+            self.legend = None
+            include_legend = False
+        elif hasattr(self, "color"):
+            kwargs["column"] = self.column
+            kwargs["color"] = self.color
+            self.legend = None
+            include_legend = False
+        elif self._is_categorical:
+            kwargs = self._prepare_categorical_plot(kwargs)
+        else:
+            kwargs = self._prepare_continous_plot(kwargs)
+
+        if self.legend:
+            self._actually_add_legend()
+
+        self._gdf.plot(legend=include_legend, ax=self.ax, **kwargs)
+
+    def save(self, path: str) -> None:
+        """Save figure as image file.
+
+        To be run after the plot method.
+
+        Args:
+            path: File path.
+        """
+        try:
+            plt.savefig(path)
+        except FileNotFoundError:
+            from dapla import FileClient
+
+            fs = FileClient.get_gcs_file_system()
+            with fs.open(path, "wb") as file:
+                plt.savefig(file)
+
+    def _prepare_plot(self, **kwargs):
+        """Add figure and axis, title and background gdf."""
+        for attr in self.__dict__.keys():
+            if attr in self.kwargs:
+                self[attr] = self.kwargs.pop(attr)
+            if attr in kwargs:
+                self[attr] = kwargs.pop(attr)
+
         self.fig, self.ax = self._get_matplotlib_figure_and_axix(
             figsize=(self._size, self._size)
         )
         self.fig.patch.set_facecolor(self.facecolor)
         self.ax.set_axis_off()
 
         if hasattr(self, "_background_gdfs"):
             self._actually_add_background()
 
         if hasattr(self, "title") and self.title:
             self.ax.set_title(
                 self.title, fontsize=self.title_fontsize, color=self.title_color
             )
 
-        if not self._is_categorical:
-            self._prepare_continous_map()
-            if self.scheme:
-                self.colorlist = self._get_continous_colors()
-                self.colors = self._classify_from_bins(self._gdf)
+    def _prepare_continous_plot(self, kwargs) -> dict:
+        """Create bins and colors."""
+        self._prepare_continous_map()
+
+        if self.scheme is None:
+            self.legend = None
+            kwargs["column"] = self.column
+            return kwargs
+
+        elif self.bins is None:
+            kwargs["column"] = self.column
+            return kwargs
+
         else:
-            self._get_categorical_colors()
-            self.colors = self._gdf["color"]
+            classified = self._classify_from_bins(self._gdf, bins=self.bins)
+            classified_sequential = self._push_classification(classified)
+            n_colors = len(np.unique(classified_sequential)) - any(self._nan_idx)
+            self._unique_colors = self._get_continous_colors(n=n_colors)
+            self._bins_unique_values = self._make_bin_value_dict(
+                self._gdf, classified_sequential
+            )
+            colorarray = self._unique_colors[classified_sequential]
+            kwargs["color"] = colorarray
 
-        if self.legend:
-            if not self.legend._position_has_been_set:
-                self.legend._position = self.legend._get_best_legend_position(
-                    self._gdf, k=self._k + bool(len(self._nan_idx))
-                )
-
-            if not self._is_categorical and not self.legend._rounding_has_been_set:
-                self.legend._rounding = self.legend._get_rounding(
-                    array=self._gdf.loc[~self._nan_idx, self._column]
-                )
+        if self.legend and not self.legend._rounding_has_been_set:
+            self.bins = self.legend._set_rounding(
+                bins=self.bins, rounding=self.legend._rounding
+            )
 
-        if not self.legend:
-            self._include_legend = False
-        elif self._is_categorical:
+            if any(self._nan_idx):
+                self.bins = self.bins + [self.nan_label]
+
+        return kwargs
+
+    def _prepare_categorical_plot(self, kwargs) -> dict:
+        """Map values to colors."""
+        self._get_categorical_colors()
+        colorarray = self._gdf["color"]
+
+        kwargs["color"] = colorarray
+        return kwargs
+
+    def _actually_add_legend(self) -> None:
+        """Add legend to the axis and fill it with colors and labels."""
+        if not self.legend._position_has_been_set:
+            self.legend._position = self.legend._get_best_legend_position(
+                self._gdf, k=self._k + bool(len(self._nan_idx))
+            )
+
+        if not self._is_categorical and not self.legend._rounding_has_been_set:
+            self.legend._rounding = self.legend._get_rounding(
+                array=self._gdf.loc[~self._nan_idx, self._column]
+            )
+
+        if self._is_categorical:
             self.ax = self.legend._actually_add_categorical_legend(
                 ax=self.ax,
                 categories_colors=self._categories_colors_dict,
                 nan_label=self.nan_label,
             )
-            self._include_legend = True
-        elif self.scheme is None:
-            self._include_legend = True
         else:
-            self._include_legend = True
-            if not self.legend._rounding_has_been_set:
-                self.bins = self.legend._set_rounding(
-                    bins=self.bins, rounding=self.legend._rounding
-                )
-
-            if any(self._nan_idx):
-                self.bins = self.bins + [self.nan_label]
-
             self.ax = self.legend._actually_add_continous_legend(
                 ax=self.ax,
                 bins=self.bins,
-                colors=self.colorlist,
+                colors=self._unique_colors,
                 nan_label=self.nan_label,
                 bin_values=self._bins_unique_values,
             )
 
-        if self.bins or self._is_categorical:
-            self._gdf.plot(color=self.colors, legend=self._include_legend, ax=self.ax)
-        else:
-            self._gdf.plot(column=self.column, legend=self._include_legend, ax=self.ax)
-
-    def save(self, path: str) -> None:
-        """Save figure as image file.
-
-        To be run after the plot method.
-
-        Args:
-            path: File path.
-        """
-        try:
-            plt.savefig(path)
-        except FileNotFoundError:
-            from dapla import FileClient
-
-            fs = FileClient.get_gcs_file_system()
-            with fs.open(path, "wb") as file:
-                plt.savefig(file)
-
-    def _add_legend(self):
+    def _create_legend(self):
+        """Instantiate the Legend class."""
         kwargs = {}
         if self._black:
             kwargs["facecolor"] = "#0f0f0f"
             kwargs["labelcolor"] = "#fefefe"
             kwargs["title_color"] = "#fefefe"
 
-        self.legend = Legend(title=self._column, size=self._size, **kwargs)
+        if self._is_categorical:
+            self.legend = Legend(title=self._column, size=self._size, **kwargs)
+        else:
+            self.legend = ContinousLegend(title=self._column, size=self._size, **kwargs)
 
     def _choose_cmap(self):
         """kwargs is to catch start and stop points for the cmap in __init__."""
         if self._black:
             self._cmap = "viridis"
             self.cmap_start = 0
             self.cmap_stop = 256
         else:
             self._cmap = "RdPu"
             self.cmap_start = 23
             self.cmap_stop = 256
 
+    def _make_bin_value_dict(self, gdf, classified) -> dict:
+        """Dict with unique values of all bins. Used in labels in ContinousLegend."""
+        bins_unique_values = {
+            i: list(set(gdf.loc[classified == i, self._column]))
+            for i, _ in enumerate(np.unique(classified))
+        }
+        return bins_unique_values
+
     def _actually_add_background(self):
         self.ax.set_xlim([self.minx - self.diffx * 0.03, self.maxx + self.diffx * 0.03])
         self.ax.set_ylim([self.miny - self.diffy * 0.03, self.maxy + self.diffy * 0.03])
         self._background_gdfs.plot(ax=self.ax, color=self.bg_gdf_color)
 
     @staticmethod
     def _get_matplotlib_figure_and_axix(figsize: tuple[int, int]):
@@ -267,26 +326,26 @@
                 "#0f0f0f",
                 "#fefefe",
                 "#383836",
             )
             self.nan_color = "#666666"
             if not self._is_categorical:
                 self.change_cmap("viridis")
-            self._add_legend()
 
         else:
             self.facecolor, self.title_color, self.bg_gdf_color = (
                 "#fefefe",
                 "#0f0f0f",
                 "#ebebeb",
             )
             self.nan_color = "#c2c2c2"
             if not self._is_categorical:
                 self.change_cmap("RdPu", start=23)
-            self._add_legend()
+
+        self._create_legend()
 
     def __getitem__(self, item):
         return getattr(self, item)
 
     def get(self, key, default=None):
         try:
             return self[key]
```

### Comparing `ssb_sgis-0.1.4/src/sgis/networkanalysis/_get_route.py` & `ssb_sgis-0.1.5/src/sgis/networkanalysis/_get_route.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.4/src/sgis/networkanalysis/_od_cost_matrix.py` & `ssb_sgis-0.1.5/src/sgis/networkanalysis/_od_cost_matrix.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.4/src/sgis/networkanalysis/_points.py` & `ssb_sgis-0.1.5/src/sgis/networkanalysis/_points.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.4/src/sgis/networkanalysis/_service_area.py` & `ssb_sgis-0.1.5/src/sgis/networkanalysis/_service_area.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.4/src/sgis/networkanalysis/directednetwork.py` & `ssb_sgis-0.1.5/src/sgis/networkanalysis/directednetwork.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.4/src/sgis/networkanalysis/network.py` & `ssb_sgis-0.1.5/src/sgis/networkanalysis/network.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.4/src/sgis/networkanalysis/network_norway.py` & `ssb_sgis-0.1.5/src/sgis/networkanalysis/network_norway.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.4/src/sgis/networkanalysis/networkanalysis.py` & `ssb_sgis-0.1.5/src/sgis/networkanalysis/networkanalysis.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.4/src/sgis/networkanalysis/networkanalysisrules.py` & `ssb_sgis-0.1.5/src/sgis/networkanalysis/networkanalysisrules.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.4/src/sgis/read_parquet.py` & `ssb_sgis-0.1.5/src/sgis/read_parquet.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.4/PKG-INFO` & `ssb_sgis-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ssb-sgis
-Version: 0.1.4
-Summary: GIS utility functions used at Statistics Norway.
+Version: 0.1.5
+Summary: GIS functions used at Statistics Norway.
 Home-page: https://github.com/statisticsnorway/ssb-sgis
 License: MIT
 Author: Statistics Norway
 Author-email: ort@ssb.no
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Dist: branca (>=0.6.0,<0.7.0)
```

