# Comparing `tmp/imagemangler-0.1.1.tar.gz` & `tmp/imagemangler-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imagemangler-0.1.1.tar", max compression
+gzip compressed data, was "imagemangler-0.1.2.tar", max compression
```

## Comparing `imagemangler-0.1.1.tar` & `imagemangler-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1575 2023-04-12 12:56:47.112552 imagemangler-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-04-12 10:06:57.002508 imagemangler-0.1.1/imagemangler/__init__.py
--rw-r--r--   0        0        0     2573 2023-04-12 12:54:57.179218 imagemangler-0.1.1/imagemangler/cli.py
--rw-r--r--   0        0        0        0 2023-04-12 10:09:01.962509 imagemangler-0.1.1/imagemangler/core/__init__.py
--rw-r--r--   0        0        0      531 2023-04-12 12:54:57.179218 imagemangler-0.1.1/imagemangler/core/mangler.py
--rw-r--r--   0        0        0      549 2023-04-12 13:08:01.879221 imagemangler-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2456 1970-01-01 00:00:00.000000 imagemangler-0.1.1/setup.py
--rw-r--r--   0        0        0     2100 1970-01-01 00:00:00.000000 imagemangler-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      167 2023-04-12 13:11:29.472555 imagemangler-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-12 10:06:57.002508 imagemangler-0.1.2/imagemangler/__init__.py
+-rw-r--r--   0        0        0     2600 2023-04-12 13:26:37.415892 imagemangler-0.1.2/imagemangler/cli.py
+-rw-r--r--   0        0        0        0 2023-04-12 10:09:01.962509 imagemangler-0.1.2/imagemangler/core/__init__.py
+-rw-r--r--   0        0        0      531 2023-04-12 12:54:57.179218 imagemangler-0.1.2/imagemangler/core/mangler.py
+-rw-r--r--   0        0        0      548 2023-04-12 13:26:49.909226 imagemangler-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1004 1970-01-01 00:00:00.000000 imagemangler-0.1.2/setup.py
+-rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 imagemangler-0.1.2/PKG-INFO
```

### Comparing `imagemangler-0.1.1/imagemangler/cli.py` & `imagemangler-0.1.2/imagemangler/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,23 +5,27 @@
 import cv2
 import numpy as np
 import typer
 from PIL import Image
 
 from imagemangler.core.mangler import deteriorate
 
+app = typer.Typer()
+
+
 WINDOW_SIZE = (800, 600)
 
 
 def zip_image(zip_file, img, name, extension):
     img_bytes = io.BytesIO()
     img.save(img_bytes, format=extension)
     zip_file.writestr(f"{name}.{extension}", img_bytes.getvalue())
 
 
+@app.command()
 def main(
     image_path: str,
     quality: int = typer.Argument(70, help="Base quality to start with"),
     quality_step: int = typer.Option(2, help="Quality step to reduce by"),
     auto_mangle: bool = typer.Option(
         False, help="Automatically mangle the image across all qualitie steps"
     ),
@@ -77,8 +81,8 @@
                 concurrent.futures.wait(futures)
 
     elif typer.confirm("Do you want to save the last mangled image?"):
         img.save(f"mangled_img.{extension}")
 
 
 if __name__ == "__main__":
-    typer.run(main)
+    app()
```

### Comparing `imagemangler-0.1.1/imagemangler/core/mangler.py` & `imagemangler-0.1.2/imagemangler/core/mangler.py`

 * *Files identical despite different names*

### Comparing `imagemangler-0.1.1/pyproject.toml` & `imagemangler-0.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "imagemangler"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["miguelvalente <miguelvalente@protonmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pillow = "^9.5.0"
@@ -19,8 +19,8 @@
 isort = "^5.12.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-imagemangler = "imagemangler.cli:main"
+imagemangler = "imagemangler.cli:app"
```

