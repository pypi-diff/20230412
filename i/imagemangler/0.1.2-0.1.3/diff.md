# Comparing `tmp/imagemangler-0.1.2.tar.gz` & `tmp/imagemangler-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imagemangler-0.1.2.tar", max compression
+gzip compressed data, was "imagemangler-0.1.3.tar", max compression
```

## Comparing `imagemangler-0.1.2.tar` & `imagemangler-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      167 2023-04-12 13:11:29.472555 imagemangler-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-04-12 10:06:57.002508 imagemangler-0.1.2/imagemangler/__init__.py
--rw-r--r--   0        0        0     2600 2023-04-12 13:26:37.415892 imagemangler-0.1.2/imagemangler/cli.py
--rw-r--r--   0        0        0        0 2023-04-12 10:09:01.962509 imagemangler-0.1.2/imagemangler/core/__init__.py
--rw-r--r--   0        0        0      531 2023-04-12 12:54:57.179218 imagemangler-0.1.2/imagemangler/core/mangler.py
--rw-r--r--   0        0        0      548 2023-04-12 13:26:49.909226 imagemangler-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1004 1970-01-01 00:00:00.000000 imagemangler-0.1.2/setup.py
--rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 imagemangler-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      167 2023-04-12 13:11:29.472555 imagemangler-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-12 10:06:57.002508 imagemangler-0.1.3/imagemangler/__init__.py
+-rw-r--r--   0        0        0     2629 2023-04-12 14:01:17.312568 imagemangler-0.1.3/imagemangler/cli.py
+-rw-r--r--   0        0        0        0 2023-04-12 10:09:01.962509 imagemangler-0.1.3/imagemangler/core/__init__.py
+-rw-r--r--   0        0        0      531 2023-04-12 12:54:57.179218 imagemangler-0.1.3/imagemangler/core/mangler.py
+-rw-r--r--   0        0        0      548 2023-04-12 14:03:22.395902 imagemangler-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1004 1970-01-01 00:00:00.000000 imagemangler-0.1.3/setup.py
+-rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 imagemangler-0.1.3/PKG-INFO
```

### Comparing `imagemangler-0.1.2/imagemangler/cli.py` & `imagemangler-0.1.3/imagemangler/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 import concurrent.futures
 import io
+import threading
 import zipfile
 
 import cv2
 import numpy as np
 import typer
 from PIL import Image
 
 from imagemangler.core.mangler import deteriorate
 
 app = typer.Typer()
 
-
 WINDOW_SIZE = (800, 600)
 
 
 def zip_image(zip_file, img, name, extension):
     img_bytes = io.BytesIO()
     img.save(img_bytes, format=extension)
     zip_file.writestr(f"{name}.{extension}", img_bytes.getvalue())
 
 
+def show_image(img, window_name):
+    cv2.imshow(window_name, cv2.cvtColor(np.asarray(img), cv2.COLOR_RGB2BGR))
+    cv2.waitKey(1)
+
+
 @app.command()
 def main(
     image_path: str,
     quality: int = typer.Argument(70, help="Base quality to start with"),
     quality_step: int = typer.Option(2, help="Quality step to reduce by"),
     auto_mangle: bool = typer.Option(
-        False, help="Automatically mangle the image across all qualitie steps"
+        False, help="Automatically mangle the image across all quality steps"
     ),
 ):
     """
     Mangle an image by deteriorating it iteratively with
     quality reduction of lossy algorithms
     """
 
@@ -47,28 +52,26 @@
     cv2.waitKey(1)
 
     mangled_images = []
     while True:
         img = deteriorate(img, quality=quality)
         mangled_images.append(img)
 
-        cv2.imshow("Deteriorated", cv2.cvtColor(np.asarray(img), cv2.COLOR_RGB2BGR))
-        cv2.waitKey(2)
+        show_image(img, "Deteriorated")
 
         if not auto_mangle:
-            if not typer.confirm("Do you want to continue?", default=True):
+            if not typer.confirm("Mangle again?", default=True):
                 break
 
         quality = max(0, quality - quality_step)
         if quality == 0:
             break
 
     if auto_mangle:
         cv2.waitKey(0)
-
     cv2.destroyAllWindows()
 
     extension = image_path.split(".")[-1]
     if typer.confirm("Do you want to save all mangled images?"):
         with zipfile.ZipFile("mangled_images.zip", "w") as zip_file:
             with concurrent.futures.ThreadPoolExecutor() as executor:
                 futures = []
@@ -78,11 +81,7 @@
                             zip_image, zip_file, img, f"mangled_img_{i}", extension
                         )
                     )
                 concurrent.futures.wait(futures)
 
     elif typer.confirm("Do you want to save the last mangled image?"):
         img.save(f"mangled_img.{extension}")
-
-
-if __name__ == "__main__":
-    app()
```

### Comparing `imagemangler-0.1.2/imagemangler/core/mangler.py` & `imagemangler-0.1.3/imagemangler/core/mangler.py`

 * *Files identical despite different names*

### Comparing `imagemangler-0.1.2/pyproject.toml` & `imagemangler-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "imagemangler"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["miguelvalente <miguelvalente@protonmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pillow = "^9.5.0"
```

### Comparing `imagemangler-0.1.2/setup.py` & `imagemangler-0.1.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['imagemangler = imagemangler.cli:app']}
 
 setup_kwargs = {
     'name': 'imagemangler',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': '',
     'long_description': '# Image Mangler\n\nImage Mangler is a Python command-line tool for deteriorating images iteratively with quality reduction of lossy algorithms such as JPEG compression.\n',
     'author': 'miguelvalente',
     'author_email': 'miguelvalente@protonmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `imagemangler-0.1.2/PKG-INFO` & `imagemangler-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imagemangler
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: miguelvalente
 Author-email: miguelvalente@protonmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

