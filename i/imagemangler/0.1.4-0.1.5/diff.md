# Comparing `tmp/imagemangler-0.1.4.tar.gz` & `tmp/imagemangler-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imagemangler-0.1.4.tar", max compression
+gzip compressed data, was "imagemangler-0.1.5.tar", max compression
```

## Comparing `imagemangler-0.1.4.tar` & `imagemangler-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      790 2023-04-12 14:34:50.972577 imagemangler-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-04-12 10:06:57.002508 imagemangler-0.1.4/imagemangler/__init__.py
--rw-r--r--   0        0        0     1937 2023-04-12 14:36:39.339244 imagemangler-0.1.4/imagemangler/cli.py
--rw-r--r--   0        0        0        0 2023-04-12 10:09:01.962509 imagemangler-0.1.4/imagemangler/core/__init__.py
--rw-r--r--   0        0        0      531 2023-04-12 12:54:57.179218 imagemangler-0.1.4/imagemangler/core/mangler.py
--rw-r--r--   0        0        0      502 2023-04-12 14:18:20.919239 imagemangler-0.1.4/imagemangler/core/utils.py
--rw-r--r--   0        0        0      548 2023-04-12 14:37:26.022578 imagemangler-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1655 1970-01-01 00:00:00.000000 imagemangler-0.1.4/setup.py
--rw-r--r--   0        0        0     1315 1970-01-01 00:00:00.000000 imagemangler-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      856 2023-04-12 18:32:44.389305 imagemangler-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-04-12 10:06:57.002508 imagemangler-0.1.5/imagemangler/__init__.py
+-rw-r--r--   0        0        0     1889 2023-04-12 18:50:06.765976 imagemangler-0.1.5/imagemangler/cli.py
+-rw-r--r--   0        0        0        0 2023-04-12 10:09:01.962509 imagemangler-0.1.5/imagemangler/core/__init__.py
+-rw-r--r--   0        0        0      564 2023-04-12 18:29:29.685971 imagemangler-0.1.5/imagemangler/core/mangler.py
+-rw-r--r--   0        0        0      567 2023-04-12 18:29:29.689304 imagemangler-0.1.5/imagemangler/core/utils.py
+-rw-r--r--   0        0        0      548 2023-04-12 18:50:13.935976 imagemangler-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1723 1970-01-01 00:00:00.000000 imagemangler-0.1.5/setup.py
+-rw-r--r--   0        0        0     1381 1970-01-01 00:00:00.000000 imagemangler-0.1.5/PKG-INFO
```

### Comparing `imagemangler-0.1.4/README.md` & `imagemangler-0.1.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# Image Mangler
+![logo](https://github.com/miguelvalente/imagemangler/blob/master/logo.png?raw=true)
 
-Image Mangler is a command-line tool to deteriorate an image iteratively with using lossy algorithms.
+
+Image Mangler is a command-line tool to deteriorate an image iteratively using lossy algorithms.
 
 # Installation
 
 You can install Image Mangler via pip:
 
 ```bash
 pip install imagemangler
@@ -25,8 +26,8 @@
 imagemangler path/to/image.jpg --quality 60 --quality-step 5 --no-auto-mangle
 ```
 
 For a more details you can use `--help`:
 
 ```bash
 imagemangler --help
-```
+```
```

### Comparing `imagemangler-0.1.4/imagemangler/cli.py` & `imagemangler-0.1.5/imagemangler/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-import concurrent.futures
 import io
 import zipfile
 
 import cv2
 import typer
 from PIL import Image
 
 from imagemangler.core.mangler import deteriorate
-from imagemangler.core.utils import show_image, zip_image
+from imagemangler.core.utils import show_image, zip_images
 
 app = typer.Typer()
 
 
 @app.command()
 def main(
     image_path: str,
-    quality: int = typer.Argument(70, help="Base quality to start with"),
+    quality: int = typer.Option(70, help="Base quality to start with"),
     quality_step: int = typer.Option(2, help="Quality step to reduce by"),
     auto_mangle: bool = typer.Option(
         True, help="Automatically mangle the image across all quality steps"
     ),
 ):
     """
     Mangle an image by deteriorating it iteratively with
     quality reduction of lossy algorithms
     """
+    extension = image_path.split(".")[-1]
     img = Image.open(io.BytesIO(open(image_path, "rb").read()))
 
     mangled_images = []
     while True:
-        img = deteriorate(img, quality=quality)
+        img = deteriorate(img, extension=extension, quality=quality)
         mangled_images.append(img)
 
         show_image(img)
 
         if not auto_mangle:
             if not typer.confirm("Mangle again?", default=True):
                 break
@@ -41,26 +41,25 @@
         quality = max(0, quality - quality_step)
         if quality == 0:
             break
 
     cv2.waitKey(0)
     cv2.destroyAllWindows()
 
-    extension = image_path.split(".")[-1]
-    if typer.confirm("Do you want to save all mangled images?"):
-        with zipfile.ZipFile("mangled_images.zip", "w") as zip_file:
-            # for faster zipping, use concurrent.futures
-            with concurrent.futures.ThreadPoolExecutor() as executor:
-                futures = []
-                for i, img in enumerate(mangled_images):
-                    futures.append(
-                        executor.submit(
-                            zip_image, zip_file, img, f"mangled_img_{i}", extension
-                        )
-                    )
-                concurrent.futures.wait(futures)
+    image_name = image_path.split("/")[-1]
+    image_no_ext = image_name.split(".")[0]
 
+    print("🖨")
+    print(f"Your image `{image_name}` was mangled {len(mangled_images)} times!")
+    print("🖨")
+
+    if typer.confirm("Do you want to save all mangled images?"):
+        with zipfile.ZipFile(f"mangled_{image_no_ext}.zip", "w") as zip_file:
+            zip_images(zip_file, mangled_images, extension)
+        print(f"Your mangled images were saved to mangled_{image_no_ext}.zip")
     elif typer.confirm("Do you want to save the last mangled image?"):
         img.save(f"mangled_img.{extension}")
+        print(f"Your mangled image was saved to mangled_img.{extension}")
+
 
 if __name__ == "__main__":
-    app()
+    app()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `imagemangler-0.1.4/imagemangler/core/mangler.py` & `imagemangler-0.1.5/imagemangler/core/mangler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 import io
 
 from PIL import Image
 
 
-def deteriorate(img: Image, optimize: bool = True, quality: int = 20) -> Image:
+def deteriorate(
+    img: Image,
+    extension,
+    optimize: bool = True,
+    quality: int = 20,
+) -> Image:
     """Deteriorate the image quality for `iterations` number of times"""
 
     compressed_buffer = io.BytesIO()
-    img.save(compressed_buffer, format="JPEG", optimize=optimize, quality=quality)
+    img.save(compressed_buffer, format=extension, optimize=optimize, quality=quality)
 
     # Get the compressed image data as bytes
     compressed_bytes = compressed_buffer.getvalue()
 
     # Load the compressed image into a PIL.Image object
     img = Image.open(io.BytesIO(compressed_bytes))
```

### Comparing `imagemangler-0.1.4/pyproject.toml` & `imagemangler-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "imagemangler"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["miguelvalente <miguelvalente@protonmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pillow = "^9.5.0"
```

### Comparing `imagemangler-0.1.4/setup.py` & `imagemangler-0.1.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,17 +14,17 @@
  'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['imagemangler = imagemangler.cli:app']}
 
 setup_kwargs = {
     'name': 'imagemangler',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': '',
-    'long_description': '# Image Mangler\n\nImage Mangler is a command-line tool to deteriorate an image iteratively with using lossy algorithms.\n\n# Installation\n\nYou can install Image Mangler via pip:\n\n```bash\npip install imagemangler\n```\n\n# Usage\n\nYou can run Image Mangler by invoking the imagemangler command in the terminal, followed by the path of the image file you want to mangle:\n\n```bash\nimagemangler path/to/image.jpg\n```\n\nBy default, Image Mangler will automatically mangle the image across all quality steps with a base quality of 70 and a quality step of 2. You can specify your own values for these parameters using the optional flags:\n\n\n```bash\nimagemangler path/to/image.jpg --quality 60 --quality-step 5 --no-auto-mangle\n```\n\nFor a more details you can use `--help`:\n\n```bash\nimagemangler --help\n```',
+    'long_description': '![logo](https://github.com/miguelvalente/imagemangler/blob/master/logo.png?raw=true)\n\n\nImage Mangler is a command-line tool to deteriorate an image iteratively using lossy algorithms.\n\n# Installation\n\nYou can install Image Mangler via pip:\n\n```bash\npip install imagemangler\n```\n\n# Usage\n\nYou can run Image Mangler by invoking the imagemangler command in the terminal, followed by the path of the image file you want to mangle:\n\n```bash\nimagemangler path/to/image.jpg\n```\n\nBy default, Image Mangler will automatically mangle the image across all quality steps with a base quality of 70 and a quality step of 2. You can specify your own values for these parameters using the optional flags:\n\n\n```bash\nimagemangler path/to/image.jpg --quality 60 --quality-step 5 --no-auto-mangle\n```\n\nFor a more details you can use `--help`:\n\n```bash\nimagemangler --help\n```\n',
     'author': 'miguelvalente',
     'author_email': 'miguelvalente@protonmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `imagemangler-0.1.4/PKG-INFO` & `imagemangler-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: imagemangler
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: miguelvalente
 Author-email: miguelvalente@protonmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
-# Image Mangler
+![logo](https://github.com/miguelvalente/imagemangler/blob/master/logo.png?raw=true)
 
-Image Mangler is a command-line tool to deteriorate an image iteratively with using lossy algorithms.
+
+Image Mangler is a command-line tool to deteriorate an image iteratively using lossy algorithms.
 
 # Installation
 
 You can install Image Mangler via pip:
 
 ```bash
 pip install imagemangler
@@ -42,7 +43,8 @@
 ```
 
 For a more details you can use `--help`:
 
 ```bash
 imagemangler --help
 ```
+
```

