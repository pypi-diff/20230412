# Comparing `tmp/imagemangler-0.1.0.tar.gz` & `tmp/imagemangler-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imagemangler-0.1.0.tar", max compression
+gzip compressed data, was "imagemangler-0.1.1.tar", max compression
```

## Comparing `imagemangler-0.1.0.tar` & `imagemangler-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1575 2023-04-12 12:56:47.112552 imagemangler-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-12 10:06:57.002508 imagemangler-0.1.0/imagemangler/__init__.py
--rw-r--r--   0        0        0     2573 2023-04-12 12:54:57.179218 imagemangler-0.1.0/imagemangler/cli.py
--rw-r--r--   0        0        0        0 2023-04-12 10:09:01.962509 imagemangler-0.1.0/imagemangler/core/__init__.py
--rw-r--r--   0        0        0      531 2023-04-12 12:54:57.179218 imagemangler-0.1.0/imagemangler/core/mangler.py
--rw-r--r--   0        0        0      487 2023-04-12 12:54:39.305884 imagemangler-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2342 1970-01-01 00:00:00.000000 imagemangler-0.1.0/setup.py
--rw-r--r--   0        0        0     2100 1970-01-01 00:00:00.000000 imagemangler-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1575 2023-04-12 12:56:47.112552 imagemangler-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-12 10:06:57.002508 imagemangler-0.1.1/imagemangler/__init__.py
+-rw-r--r--   0        0        0     2573 2023-04-12 12:54:57.179218 imagemangler-0.1.1/imagemangler/cli.py
+-rw-r--r--   0        0        0        0 2023-04-12 10:09:01.962509 imagemangler-0.1.1/imagemangler/core/__init__.py
+-rw-r--r--   0        0        0      531 2023-04-12 12:54:57.179218 imagemangler-0.1.1/imagemangler/core/mangler.py
+-rw-r--r--   0        0        0      549 2023-04-12 13:08:01.879221 imagemangler-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2456 1970-01-01 00:00:00.000000 imagemangler-0.1.1/setup.py
+-rw-r--r--   0        0        0     2100 1970-01-01 00:00:00.000000 imagemangler-0.1.1/PKG-INFO
```

### Comparing `imagemangler-0.1.0/README.md` & `imagemangler-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `imagemangler-0.1.0/imagemangler/cli.py` & `imagemangler-0.1.1/imagemangler/cli.py`

 * *Files identical despite different names*

### Comparing `imagemangler-0.1.0/imagemangler/core/mangler.py` & `imagemangler-0.1.1/imagemangler/core/mangler.py`

 * *Files identical despite different names*

### Comparing `imagemangler-0.1.0/setup.py` & `imagemangler-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,25 +9,29 @@
 
 install_requires = \
 ['numpy>=1.24.2,<2.0.0',
  'opencv-python>=4.7.0.72,<5.0.0.0',
  'pillow>=9.5.0,<10.0.0',
  'typer[all]>=0.7.0,<0.8.0']
 
+entry_points = \
+{'console_scripts': ['imagemangler = imagemangler.cli:main']}
+
 setup_kwargs = {
     'name': 'imagemangler',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
     'long_description': 'Image Mangler\n\nImage Mangler is a command-line tool for deteriorating images iteratively with quality reduction of lossy algorithms.\nFeatures\n\n    Reduce image quality iteratively to produce a mangled image\n    Option to automatically mangle the image across all quality steps\n    Option to save all mangled images to a zip file or just the last one\n    Supports JPEG compression only\n    Uses Poetry for dependency management\n\nInstallation\n\n    Clone this repository: git clone https://github.com/your_username/image-mangler.git\n    Navigate to the project directory: cd image-mangler\n    Install the dependencies: poetry install\n\nUsage\n\nvbnet\n\nUsage: image-mangler [OPTIONS] IMAGE_PATH\n\n  Mangle an image by deteriorating it iteratively with quality reduction of\n  lossy algorithms\n\nArguments:\n  IMAGE_PATH  Path to the image to be mangled  [required]\n\nOptions:\n  --quality INTEGER  Base quality to start with (default: 70)\n  --quality-step INTEGER  Quality step to reduce by (default: 2)\n  --auto-mangle / --no-auto-mangle  Automatically mangle the image across all quality steps (default: False)\n  --help  Show this message and exit.\n\nExample usage:\n\narduino\n\n$ image-mangler image.jpg --quality 50 --quality-step 5 --auto-mangle\n\nSaving Mangled Images\n\nAfter mangling an image, you will be prompted to save the mangled images. You can choose to save all mangled images to a zip file or just the last one. The zip file will be saved as mangled_images.zip in the current directory.\nLicense\n\nThis project is licensed under the MIT License. See the LICENSE file for details.',
     'author': 'miguelvalente',
     'author_email': 'miguelvalente@protonmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
+    'entry_points': entry_points,
     'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `imagemangler-0.1.0/PKG-INFO` & `imagemangler-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imagemangler
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: miguelvalente
 Author-email: miguelvalente@protonmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

