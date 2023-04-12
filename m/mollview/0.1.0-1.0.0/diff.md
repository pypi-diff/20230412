# Comparing `tmp/mollview-0.1.0.tar.gz` & `tmp/mollview-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mollview-0.1.0.tar", max compression
+gzip compressed data, was "mollview-1.0.0.tar", max compression
```

## Comparing `mollview-0.1.0.tar` & `mollview-1.0.0.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0      578 2023-04-12 13:36:33.967771 mollview-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2184 2023-04-12 14:11:59.244423 mollview-0.1.0/src/mollview/__init__.py
--rw-r--r--   0        0        0       32 2023-04-12 13:13:00.617058 mollview-0.1.0/src/mollview/__main__.py
--rw-r--r--   0        0        0      835 2023-04-12 14:28:32.947205 mollview-0.1.0/setup.py
--rw-r--r--   0        0        0      563 2023-04-12 14:28:32.947449 mollview-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-12 14:49:20.509536 mollview-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2293 2023-04-12 14:54:37.667964 mollview-1.0.0/README.md
+-rw-r--r--   0        0        0      662 2023-04-12 14:57:44.772573 mollview-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2204 2023-04-12 14:54:19.524042 mollview-1.0.0/src/mollview/__init__.py
+-rw-r--r--   0        0        0       32 2023-04-12 13:13:00.617058 mollview-1.0.0/src/mollview/__main__.py
+-rw-r--r--   0        0        0     3211 2023-04-12 15:00:31.221718 mollview-1.0.0/setup.py
+-rw-r--r--   0        0        0     2961 2023-04-12 15:00:31.221967 mollview-1.0.0/PKG-INFO
```

### Comparing `mollview-0.1.0/pyproject.toml` & `mollview-1.0.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tool.poetry]
 name = "mollview"
-version = "0.1.0"
-description = "Plot HEALPix maps from the commandline."
+version = "1.0.0"
+description = "mollview is a command line tool for plotting HEALPix maps from fits files."
 authors = ["Metin San <metinisan@gmail.com>"]
-license = "GNU"
+license = "GNU General Public License v3.0"
+readme = "README.md"
 
 [tool.poetry.scripts]
 mollview = "mollview:app"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 healpy = "^1.16.2"
```

### Comparing `mollview-0.1.0/src/mollview/__init__.py` & `mollview-1.0.0/src/mollview/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from pathlib import Path
 from typing import Tuple
 
 import healpy as hp
 import matplotlib.pyplot as plt
 import typer
 
-app = typer.Typer()
+app = typer.Typer(add_completion=False)
 
 
 @app.command()
 def plot_map(
     filename: Path = typer.Argument(..., help="Name of HEALPIX fits file"),
     field: int = typer.Option(0, help="Column to read. 0 is I, 1 is Q, and 2 is U"),
-    norm: str = typer.Option(None, help="Normalization method"),
     min: float = typer.Option(None, help="Minimum value"),
     max: float = typer.Option(None, help="Maximum value"),
-    coord: Tuple[str, str] = typer.Option((None, None), help="Coordinate system"),
+    norm: str = typer.Option(None, help="Normalization method"),
+    cmap: str = typer.Option(None, help="Color map"),
     unit: str = typer.Option(None, help="Unit"),
-    nest: bool = typer.Option(False, help="Use NESTED pixel ordering"),
     title: str = typer.Option("", help="Title"),
-    xsize: int = typer.Option(800, help="Size of the figure"),
-    notext: bool = typer.Option(False, help="Do not show text"),
-    cmap: str = typer.Option(None, help="Color map"),
-    cbar: bool = typer.Option(True, help="Show color bar"),
     save: bool = typer.Option(False, help="Save the figure"),
+    coord: Tuple[str, str] = typer.Option((None, None), help="Coordinate system"),
+    cbar: bool = typer.Option(True, help="Show color bar"),
+    notext: bool = typer.Option(False, help="Do not show text"),
+    xsize: int = typer.Option(800, help="Size of the figure"),
+    nest: bool = typer.Option(False, help="Use NESTED pixel ordering"),
     remove_dip: bool = typer.Option(False, help="Remove the dipole"),
     gal_cut: float = typer.Option(
         None,
         help="Symmetric galactic cut for the dipole/monopole fit. Removes points in latitude range [-gal_cut, +gal_cut]",
     ),
     remove_mono: bool = typer.Option(False, help="Remove the monopole"),
     badcolor: str = typer.Option("gray", help="Color of bad pixels"),
```

