# Comparing `tmp/pygeoops-0.1.0a1.tar.gz` & `tmp/pygeoops-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygeoops-0.1.0a1.tar", last modified: Tue Feb 28 09:56:08 2023, max compression
+gzip compressed data, was "pygeoops-0.1.1.tar", last modified: Tue Apr 11 23:35:07 2023, max compression
```

## Comparing `pygeoops-0.1.0a1.tar` & `pygeoops-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 09:56:08.195897 pygeoops-0.1.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-02-28 09:55:58.000000 pygeoops-0.1.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-28 09:55:58.000000 pygeoops-0.1.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-02-28 09:56:08.195897 pygeoops-0.1.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-02-28 09:55:58.000000 pygeoops-0.1.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 09:56:08.195897 pygeoops-0.1.0a1/pygeoops/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-02-28 09:55:58.000000 pygeoops-0.1.0a1/pygeoops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-02-28 09:55:58.000000 pygeoops-0.1.0a1/pygeoops/centerline.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-28 09:55:58.000000 pygeoops-0.1.0a1/pygeoops/version.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-02-28 09:55:58.000000 pygeoops-0.1.0a1/pygeoops/view_angles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 09:56:08.195897 pygeoops-0.1.0a1/pygeoops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-02-28 09:56:08.000000 pygeoops-0.1.0a1/pygeoops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-02-28 09:56:08.000000 pygeoops-0.1.0a1/pygeoops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 09:56:08.000000 pygeoops-0.1.0a1/pygeoops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-28 09:56:08.000000 pygeoops-0.1.0a1/pygeoops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-28 09:56:08.000000 pygeoops-0.1.0a1/pygeoops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-02-28 09:55:58.000000 pygeoops-0.1.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-28 09:56:08.195897 pygeoops-0.1.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-02-28 09:55:58.000000 pygeoops-0.1.0a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 09:56:08.195897 pygeoops-0.1.0a1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-02-28 09:55:58.000000 pygeoops-0.1.0a1/tests/test_centerline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-02-28 09:55:58.000000 pygeoops-0.1.0a1/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-02-28 09:55:58.000000 pygeoops-0.1.0a1/tests/test_view_angles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:35:07.326212 pygeoops-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-11 23:34:56.000000 pygeoops-0.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-11 23:34:56.000000 pygeoops-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-11 23:35:07.326212 pygeoops-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-11 23:34:56.000000 pygeoops-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:35:07.322212 pygeoops-0.1.1/pygeoops/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-11 23:34:56.000000 pygeoops-0.1.1/pygeoops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11510 2023-04-11 23:34:56.000000 pygeoops-0.1.1/pygeoops/centerline.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-11 23:34:56.000000 pygeoops-0.1.1/pygeoops/version.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-04-11 23:34:56.000000 pygeoops-0.1.1/pygeoops/view_angles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:35:07.326212 pygeoops-0.1.1/pygeoops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-11 23:35:07.000000 pygeoops-0.1.1/pygeoops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-11 23:35:07.000000 pygeoops-0.1.1/pygeoops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 23:35:07.000000 pygeoops-0.1.1/pygeoops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 23:35:07.000000 pygeoops-0.1.1/pygeoops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 23:35:07.000000 pygeoops-0.1.1/pygeoops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-11 23:34:56.000000 pygeoops-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-11 23:35:07.326212 pygeoops-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-11 23:34:56.000000 pygeoops-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:35:07.326212 pygeoops-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-11 23:34:56.000000 pygeoops-0.1.1/tests/test_centerline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-11 23:34:56.000000 pygeoops-0.1.1/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-04-11 23:34:56.000000 pygeoops-0.1.1/tests/test_view_angles.py
```

### Comparing `pygeoops-0.1.0a1/LICENSE` & `pygeoops-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygeoops-0.1.0a1/PKG-INFO` & `pygeoops-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,19 @@
-Metadata-Version: 2.1
-Name: pygeoops
-Version: 0.1.0a1
-Summary: PyGeoOps provides some less common or extended spatial algorithms and utility functions.
-Home-page: https://github.com/pygeoops/pygeoops
-Author: Pieter Roggemans
-Author-email: pieter.roggemans@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PyGeoOps
 
 [![Actions Status](https://github.com/pygeoops/pygeoops/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/pygeoops/pygeoops/actions/workflows/tests.yml?query=workflow%3ATests) 
 [![codecov](https://codecov.io/gh/pygeoops/pygeoops/branch/main/graph/badge.svg?token=4241CY86O2)](https://codecov.io/gh/pygeoops/pygeoops)
 [![PyPI version](https://img.shields.io/pypi/v/pygeoops.svg)](https://pypi.org/project/pygeoops)
 [![Conda version](https://anaconda.org/conda-forge/pygeoops/badges/version.svg)](https://anaconda.org/conda-forge/pygeoops)
 
 PyGeoOps provides some less common or extended spatial algorithms and utility functions.
 
 ## Usage
 
-Calculate a centerline for a polygon:
+Calculate a [centerline](https://pygeoops.readthedocs.io/en/latest/api/pygeoops.centerline.html#pygeoops.centerline) for a polygon:
 
 ```
 import pygeoops
 import shapely
 
 polygon = shapely.from_wkt("POLYGON ((0 0, 0 8, -2 10, 4 10, 2 8, 2 2, 10 2, 10 0, 0 0))")
 centerline = pygeoops.centerline(polygon)
```

### Comparing `pygeoops-0.1.0a1/pygeoops/centerline.py` & `pygeoops-0.1.1/pygeoops/centerline.py`

 * *Files 17% similar despite different names*

```diff
@@ -124,15 +124,15 @@
     min_branch_length_cur = min_branch_length
     if min_branch_length_cur < 0:
         # If < 0, calculate
         if average_width is None:
             average_width = _average_width(geom)
         min_branch_length_cur = abs(min_branch_length_cur) * average_width
     if min_branch_length_cur > 0:
-        lines = _remove_short_branches(lines, min_branch_length_cur)
+        lines = _remove_short_branches_notempty(lines, min_branch_length_cur)
 
     # Simplify if needed
     if simplifytolerance is not None:
         tol = simplifytolerance
         if simplifytolerance < 0:
             # Automatically determine tol
             if average_width is None:
@@ -154,38 +154,79 @@
 
     Returns:
         float: the average width
     """
     return geom.length / 4 - math.sqrt(max((geom.length / 4) ** 2 - geom.area, 0))
 
 
+def _remove_short_branches_notempty(
+    line: Union[shapely.MultiLineString, shapely.LineString, None],
+    min_branch_length: float,
+) -> Union[shapely.MultiLineString, shapely.LineString, None]:
+    """
+    Remove all branches of the input lines shorter than min_branch_length. If this
+    leads to a None or empty result, return a valid line anyway.
+
+    Args:
+        line (shapely line): input line
+        min_branch_length (float): the minimum length of branches to keep.
+
+    Returns:
+        Union[shapely.MultiLineString, shapely.LineString, None]: the cleaned line
+    """
+    # If line already OK or minimum branch length invalid, just return input
+    if line is None or isinstance(line, shapely.LineString) or min_branch_length <= 0:
+        return line
+
+    # Remove short branches
+    line_cleaned = _remove_short_branches(
+        line, min_branch_length, remove_one_by_one=False
+    )
+
+    # If _remove_short_branches returned an empty result, try again but less agressive
+    if line_cleaned is None or line_cleaned.is_empty:
+        line_cleaned = _remove_short_branches(
+            line, min_branch_length, remove_one_by_one=True
+        )
+
+    # If still an empty result, return original version
+    if line_cleaned is None or line_cleaned.is_empty:
+        line_cleaned = line
+
+    return line_cleaned
+
+
 def _remove_short_branches(
     line: Union[shapely.MultiLineString, shapely.LineString, None],
     min_branch_length: float,
+    remove_one_by_one: bool,
 ) -> Union[shapely.MultiLineString, shapely.LineString, None]:
     """
     Remove all branches of the input lines shorter than min_branch_length.
 
     Args:
         line (shapely line): input line
         min_branch_length (float): the minimum length of branches to keep.
+        remove_one_by_one (bool): True to remove short branches one by one, with line
+            merges in between. This will give a less clean result, but will less often
+            result in an empty result.
 
     Returns:
         Union[shapely.MultiLineString, shapely.LineString, None]: the cleaned line
     """
     # If line already OK or minimum branch length invalid, just return input
     if line is None or isinstance(line, shapely.LineString) or min_branch_length <= 0:
         return line
 
     # Remove short branches till there are no more short branches
     line_cleaned = shapely.normalize(line)
     while isinstance(line_cleaned, shapely.MultiLineString):
         # Loop over each line to check if we keep it, ordered by length
         lines_rtree = None
-        line_removed = False
+        line_parts_to_remove = []
         line_cleaned_parts = shapely.get_parts(line_cleaned)
         linetuples_sorted = sorted(
             enumerate(line_cleaned_parts),
             key=lambda x: shapely.length(x[1]),
         )
         for line_cur_idx, line_cur in linetuples_sorted:
             # If the line is long enough, always keep it
@@ -237,24 +278,24 @@
                 continue
             elif startpoint_adjacency and endpoint_adjacency:
                 # Line between two others, so keep it
                 continue
             else:
                 # Only either start or end point has an adjacency: short branch,
                 # so don't keep.
-                line_cleaned = shapely.multilinestrings(
-                    np.delete(line_cleaned_parts, line_cur_idx, axis=0)
-                )
-                line_removed = True
-                break
-
-        # If no lines were removed anymore in the last pass, we are ready
-        if not line_removed:
+                line_parts_to_remove.append(line_cur_idx)
+                if remove_one_by_one:
+                    break
+
+        # Remove the line parts found
+        if len(line_parts_to_remove) > 0:
+            line_cleaned = shapely.multilinestrings(
+                np.delete(line_cleaned_parts, line_parts_to_remove, axis=0)
+            )
+        else:
+            # If no lines were removed anymore in the last pass, we are ready
             break
 
         # Merge the lines to keep again...
         line_cleaned = shapely.line_merge(line_cleaned)
 
-    if line_cleaned is None or line_cleaned.is_empty:
-        return line
-
     return line_cleaned
```

### Comparing `pygeoops-0.1.0a1/tests/test_centerline.py` & `pygeoops-0.1.1/tests/test_centerline.py`

 * *Files 23% similar despite different names*

```diff
@@ -49,37 +49,58 @@
     for test_idx, box_test in enumerate(box_tests):
         output_path = tmp_path / f"test_centerline_box_arr_{box_test[0]}.png"
         test_helper.plot([centerlines[test_idx], centerlines[test_idx]], output_path)
         assert centerlines[test_idx].wkt == box_test[2]
 
 
 @pytest.mark.parametrize(
-    "test, poly_wkt, expected_centerline_wkt",
+    "test, min_branch_length, poly_wkt, expected_centerline_wkt",
     [
         (
             "input: elleptical shape, resulted in small branch not being removed",
+            0.0,
+            "MULTIPOLYGON (((0 1, 1 3.25, 2 4.5, 3 5.75, 3.5 6.25, 5 3.25, 3.75 1.75, 2.5 0.5, 1 0, 0 1)))",  # noqa: E501
+            "MULTILINESTRING ((3.2641509433962264 3.3726415094339623, 3.7916666666666665 5.458333333333333), (3.2641509433962264 3.3726415094339623, 3.34375 3.359375), (1.375 1.375, 3.2641509433962264 3.3726415094339623))",  # noqa: E501
+        ),
+        (
+            "input: elleptical shape, resulted in small branch not being removed",
+            -1.0,
             "MULTIPOLYGON (((0 1, 1 3.25, 2 4.5, 3 5.75, 3.5 6.25, 5 3.25, 3.75 1.75, 2.5 0.5, 1 0, 0 1)))",  # noqa: E501
             "LINESTRING (1.375 1.375, 3.7916666666666665 5.458333333333333)",
         ),
         (
             "input: fancy L shape, output: L-ish line",
+            0.0,
+            "POLYGON ((0 0, 0 8, -2 10, 4 10, 2 8, 2 2, 10 2, 10 0, 0 0))",
+            "MULTILINESTRING ((8.87687074829932 0.9829931972789112, 9.2 1.5), (8.87687074829932 0.9829931972789112, 9.166666666666666 0.5), (1.1367816091954022 1.1160919540229888, 8.87687074829932 0.9829931972789112), (1 8.75, 3.25 9.75), (1 8.75, 1.1367816091954022 1.1160919540229888), (0.833333333333333 0.8, 1.1367816091954022 1.1160919540229888), (-1.25 9.75, 1 8.75))",  # noqa: E501
+        ),
+        (
+            "input: fancy L shape, output: L-ish line",
+            -1.0,
             "POLYGON ((0 0, 0 8, -2 10, 4 10, 2 8, 2 2, 10 2, 10 0, 0 0))",
-            "MULTILINESTRING ((1 8.75, 1.1367816091954022 1.1160919540229888, 8.87687074829932 0.9829931972789112, 9.2 1.5), (1 8.75, 3.25 9.75), (-1.25 9.75, 1 8.75))",  # noqa: E501
+            "MULTILINESTRING ((1 8.75, 1.1367816091954022 1.1160919540229888, 8.87687074829932 0.9829931972789112), (1 8.75, 3.25 9.75), (-1.25 9.75, 1 8.75))",  # noqa: E501
         ),
         (
             "input: L shape, output: L line",
+            -1.0,
             "POLYGON ((0 0, 0 10, 2 10, 2 2, 10 2, 10 0, 0 0))",
             "LINESTRING (1 9, 1 1, 9 1)",
         ),
     ],
 )
 def test_centerline_poly(
-    tmp_path: Path, test: str, poly_wkt: str, expected_centerline_wkt: str
+    tmp_path: Path,
+    test: str,
+    min_branch_length: float,
+    poly_wkt: str,
+    expected_centerline_wkt: str,
 ):
     """More complicated polygon tests."""
     poly = shapely.from_wkt(poly_wkt)
-    centerline = pygeoops.centerline(poly)
+    centerline = pygeoops.centerline(poly, min_branch_length=min_branch_length)
     assert centerline is not None
     assert isinstance(centerline, BaseGeometry)
-    output_path = tmp_path / f"test_centerline_poly_{test}.png"
+    output_path = tmp_path / f"test_centerline_poly_{test}_{min_branch_length}.png"
     test_helper.plot([poly, centerline], output_path)
-    assert centerline.wkt == expected_centerline_wkt, f"test descr: {test}"
+    assert (
+        centerline.wkt == expected_centerline_wkt
+    ), f"test descr: {test}, {min_branch_length}"
```

### Comparing `pygeoops-0.1.0a1/tests/test_helper.py` & `pygeoops-0.1.1/tests/test_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,31 +2,38 @@
 """
 Helper functions for all tests.
 """
 
 import os
 from pathlib import Path
 import re
-from typing import List
+from typing import List, Optional
 
 from matplotlib import figure as mpl_figure
 import matplotlib.colors as mcolors
 import shapely
 import shapely.affinity
 import shapely.plotting
 from shapely.geometry.base import BaseGeometry
 
 
-def plot(geoms: List[BaseGeometry], output_path: Path, clean_name: bool = True):
+def plot(
+    geoms: List[BaseGeometry],
+    output_path: Path,
+    title: Optional[str] = None,
+    clean_name: bool = True,
+):
     # If we are running on CI server, don't plot
     if "GITHUB_ACTIONS" in os.environ:
         return
 
     figure = mpl_figure.Figure()
     figure.subplots(1, 1)
+    if title is not None:
+        figure.suptitle(title)
 
     colors = mcolors.TABLEAU_COLORS  # type: ignore
     for geom_idx, geom in enumerate(geoms):
         if geom.is_empty:
             continue
 
         color = colors[list(colors.keys())[geom_idx % len(colors)]]
```

