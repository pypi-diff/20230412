# Comparing `tmp/imagemangler-0.1.3.tar.gz` & `tmp/imagemangler-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imagemangler-0.1.3.tar", max compression
+gzip compressed data, was "imagemangler-0.1.4.tar", max compression
```

## Comparing `imagemangler-0.1.3.tar` & `imagemangler-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      167 2023-04-12 13:11:29.472555 imagemangler-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-04-12 10:06:57.002508 imagemangler-0.1.3/imagemangler/__init__.py
--rw-r--r--   0        0        0     2629 2023-04-12 14:01:17.312568 imagemangler-0.1.3/imagemangler/cli.py
--rw-r--r--   0        0        0        0 2023-04-12 10:09:01.962509 imagemangler-0.1.3/imagemangler/core/__init__.py
--rw-r--r--   0        0        0      531 2023-04-12 12:54:57.179218 imagemangler-0.1.3/imagemangler/core/mangler.py
--rw-r--r--   0        0        0      548 2023-04-12 14:03:22.395902 imagemangler-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1004 1970-01-01 00:00:00.000000 imagemangler-0.1.3/setup.py
--rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 imagemangler-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      790 2023-04-12 14:34:50.972577 imagemangler-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-04-12 10:06:57.002508 imagemangler-0.1.4/imagemangler/__init__.py
+-rw-r--r--   0        0        0     1937 2023-04-12 14:36:39.339244 imagemangler-0.1.4/imagemangler/cli.py
+-rw-r--r--   0        0        0        0 2023-04-12 10:09:01.962509 imagemangler-0.1.4/imagemangler/core/__init__.py
+-rw-r--r--   0        0        0      531 2023-04-12 12:54:57.179218 imagemangler-0.1.4/imagemangler/core/mangler.py
+-rw-r--r--   0        0        0      502 2023-04-12 14:18:20.919239 imagemangler-0.1.4/imagemangler/core/utils.py
+-rw-r--r--   0        0        0      548 2023-04-12 14:37:26.022578 imagemangler-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1655 1970-01-01 00:00:00.000000 imagemangler-0.1.4/setup.py
+-rw-r--r--   0        0        0     1315 1970-01-01 00:00:00.000000 imagemangler-0.1.4/PKG-INFO
```

### Comparing `imagemangler-0.1.3/imagemangler/cli.py` & `imagemangler-0.1.4/imagemangler/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,87 +1,66 @@
 import concurrent.futures
 import io
-import threading
 import zipfile
 
 import cv2
-import numpy as np
 import typer
 from PIL import Image
 
 from imagemangler.core.mangler import deteriorate
+from imagemangler.core.utils import show_image, zip_image
 
 app = typer.Typer()
 
-WINDOW_SIZE = (800, 600)
-
-
-def zip_image(zip_file, img, name, extension):
-    img_bytes = io.BytesIO()
-    img.save(img_bytes, format=extension)
-    zip_file.writestr(f"{name}.{extension}", img_bytes.getvalue())
-
-
-def show_image(img, window_name):
-    cv2.imshow(window_name, cv2.cvtColor(np.asarray(img), cv2.COLOR_RGB2BGR))
-    cv2.waitKey(1)
-
 
 @app.command()
 def main(
     image_path: str,
     quality: int = typer.Argument(70, help="Base quality to start with"),
     quality_step: int = typer.Option(2, help="Quality step to reduce by"),
     auto_mangle: bool = typer.Option(
-        False, help="Automatically mangle the image across all quality steps"
+        True, help="Automatically mangle the image across all quality steps"
     ),
 ):
     """
     Mangle an image by deteriorating it iteratively with
     quality reduction of lossy algorithms
     """
-
-    original_img = Image.open(io.BytesIO(open(image_path, "rb").read()))
     img = Image.open(io.BytesIO(open(image_path, "rb").read()))
 
-    cv2.namedWindow("Original", cv2.WINDOW_NORMAL)
-    cv2.namedWindow("Deteriorated", cv2.WINDOW_NORMAL)
-    cv2.resizeWindow("Original", WINDOW_SIZE[0], WINDOW_SIZE[1])
-    cv2.resizeWindow("Deteriorated", WINDOW_SIZE[0], WINDOW_SIZE[1])
-
-    cv2.imshow("Original", cv2.cvtColor(np.asarray(original_img), cv2.COLOR_RGB2BGR))
-    cv2.waitKey(1)
-
     mangled_images = []
     while True:
         img = deteriorate(img, quality=quality)
         mangled_images.append(img)
 
-        show_image(img, "Deteriorated")
+        show_image(img)
 
         if not auto_mangle:
             if not typer.confirm("Mangle again?", default=True):
                 break
 
         quality = max(0, quality - quality_step)
         if quality == 0:
             break
 
-    if auto_mangle:
-        cv2.waitKey(0)
+    cv2.waitKey(0)
     cv2.destroyAllWindows()
 
     extension = image_path.split(".")[-1]
     if typer.confirm("Do you want to save all mangled images?"):
         with zipfile.ZipFile("mangled_images.zip", "w") as zip_file:
+            # for faster zipping, use concurrent.futures
             with concurrent.futures.ThreadPoolExecutor() as executor:
                 futures = []
                 for i, img in enumerate(mangled_images):
                     futures.append(
                         executor.submit(
                             zip_image, zip_file, img, f"mangled_img_{i}", extension
                         )
                     )
                 concurrent.futures.wait(futures)
 
     elif typer.confirm("Do you want to save the last mangled image?"):
         img.save(f"mangled_img.{extension}")
+
+if __name__ == "__main__":
+    app()
```

### Comparing `imagemangler-0.1.3/imagemangler/core/mangler.py` & `imagemangler-0.1.4/imagemangler/core/mangler.py`

 * *Files identical despite different names*

### Comparing `imagemangler-0.1.3/pyproject.toml` & `imagemangler-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "imagemangler"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["miguelvalente <miguelvalente@protonmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pillow = "^9.5.0"
```

