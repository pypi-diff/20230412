# Comparing `tmp/pyb_utils-0.2.2.tar.gz` & `tmp/pyb_utils-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyb_utils-0.2.2.tar", max compression
+gzip compressed data, was "pyb_utils-0.2.3.tar", max compression
```

## Comparing `pyb_utils-0.2.2.tar` & `pyb_utils-0.2.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1077 2023-03-01 18:44:35.352445 pyb_utils-0.2.2/LICENSE
--rw-r--r--   0        0        0     2011 2023-03-01 18:44:35.352445 pyb_utils-0.2.2/README.md
--rw-r--r--   0        0        0        0 2023-03-01 18:44:35.352445 pyb_utils-0.2.2/pyb_utils/__init__.py
--rw-r--r--   0        0        0     8332 2023-03-01 18:44:35.352445 pyb_utils-0.2.2/pyb_utils/camera.py
--rw-r--r--   0        0        0     4587 2023-03-01 18:44:35.356445 pyb_utils-0.2.2/pyb_utils/collision.py
--rw-r--r--   0        0        0     1425 2023-03-01 18:44:35.356445 pyb_utils-0.2.2/pyb_utils/frame.py
--rw-r--r--   0        0        0     4588 2023-03-01 18:44:35.356445 pyb_utils-0.2.2/pyb_utils/ghost.py
--rw-r--r--   0        0        0      729 2023-03-01 18:44:35.356445 pyb_utils-0.2.2/pyb_utils/math.py
--rw-r--r--   0        0        0      881 2023-03-01 18:44:35.356445 pyb_utils-0.2.2/pyb_utils/robots.py
--rw-r--r--   0        0        0      598 2023-04-11 22:44:18.290567 pyb_utils-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2909 1970-01-01 00:00:00.000000 pyb_utils-0.2.2/setup.py
--rw-r--r--   0        0        0     2870 1970-01-01 00:00:00.000000 pyb_utils-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-03-01 18:44:35.352445 pyb_utils-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1956 2023-04-11 22:45:04.986417 pyb_utils-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2023-03-01 18:44:35.352445 pyb_utils-0.2.3/pyb_utils/__init__.py
+-rw-r--r--   0        0        0     8332 2023-03-01 18:44:35.352445 pyb_utils-0.2.3/pyb_utils/camera.py
+-rw-r--r--   0        0        0     4587 2023-03-01 18:44:35.356445 pyb_utils-0.2.3/pyb_utils/collision.py
+-rw-r--r--   0        0        0     1425 2023-03-01 18:44:35.356445 pyb_utils-0.2.3/pyb_utils/frame.py
+-rw-r--r--   0        0        0     4588 2023-03-01 18:44:35.356445 pyb_utils-0.2.3/pyb_utils/ghost.py
+-rw-r--r--   0        0        0      729 2023-03-01 18:44:35.356445 pyb_utils-0.2.3/pyb_utils/math.py
+-rw-r--r--   0        0        0      881 2023-03-01 18:44:35.356445 pyb_utils-0.2.3/pyb_utils/robots.py
+-rw-r--r--   0        0        0      598 2023-04-11 22:46:45.778095 pyb_utils-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2854 1970-01-01 00:00:00.000000 pyb_utils-0.2.3/setup.py
+-rw-r--r--   0        0        0     2815 1970-01-01 00:00:00.000000 pyb_utils-0.2.3/PKG-INFO
```

### Comparing `pyb_utils-0.2.2/LICENSE` & `pyb_utils-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyb_utils-0.2.2/README.md` & `pyb_utils-0.2.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,19 @@
 * Camera: virtual camera from which to get RGBA, depth, segmentation, and point
   cloud data. Also provides video recording using OpenCV.
 
 ## Install and run
 This package requires **Python 3.7+**. It has been tested on Ubuntu 16.04,
 18.04, and 20.04.
 
+### From pip
+```
+pip install pyb_utils
+```
+
 ### From source
 Clone the repo:
 ```bash
 git clone https://github.com/adamheins/pyb_utils
 cd pyb_utils
 ```
 
@@ -28,19 +33,14 @@
 ```
 
 Or using pip:
 ```bash
 python -m pip install .
 ```
 
-### Directly from GitHub
-```
-python -m pip install git+https://github.com/adamheins/pyb_utils
-```
-
 ## Usage and examples
 You can find example scripts demonstrating all of this package's utilities in
 the `scripts/` directory:
 
 * [collision detection](https://github.com/adamheins/pyb_utils/blob/main/scripts/collision_detection_example.py)
 * [ghost objects](https://github.com/adamheins/pyb_utils/blob/main/scripts/ghost_object_example.py)
 * [camera](https://github.com/adamheins/pyb_utils/blob/main/scripts/camera_example.py)
```

### Comparing `pyb_utils-0.2.2/pyb_utils/camera.py` & `pyb_utils-0.2.3/pyb_utils/camera.py`

 * *Files identical despite different names*

### Comparing `pyb_utils-0.2.2/pyb_utils/collision.py` & `pyb_utils-0.2.3/pyb_utils/collision.py`

 * *Files identical despite different names*

### Comparing `pyb_utils-0.2.2/pyb_utils/frame.py` & `pyb_utils-0.2.3/pyb_utils/frame.py`

 * *Files identical despite different names*

### Comparing `pyb_utils-0.2.2/pyb_utils/ghost.py` & `pyb_utils-0.2.3/pyb_utils/ghost.py`

 * *Files identical despite different names*

### Comparing `pyb_utils-0.2.2/pyb_utils/math.py` & `pyb_utils-0.2.3/pyb_utils/math.py`

 * *Files identical despite different names*

### Comparing `pyb_utils-0.2.2/pyb_utils/robots.py` & `pyb_utils-0.2.3/pyb_utils/robots.py`

 * *Files identical despite different names*

### Comparing `pyb_utils-0.2.2/pyproject.toml` & `pyb_utils-0.2.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.black]
 line-length = 80
 
 [tool.poetry]
 name = "pyb_utils"
-version = "0.2.2"
+version = "0.2.3"
 description = "Basic utilities for PyBullet, including collision detection, ghost (i.e. visual-only) objects, and cameras."
 authors = ["Adam Heins <mail@adamheins.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.11"
```

### Comparing `pyb_utils-0.2.2/setup.py` & `pyb_utils-0.2.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,17 +13,17 @@
  'numpy>=1.21.5,<2.0.0',
  'opencv-python>=4.5.5,<5.0.0',
  'pybullet>=3.2.1,<4.0.0',
  'spatialmath-python>=1.0.0']
 
 setup_kwargs = {
     'name': 'pyb-utils',
-    'version': '0.2.2',
+    'version': '0.2.3',
     'description': 'Basic utilities for PyBullet, including collision detection, ghost (i.e. visual-only) objects, and cameras.',
-    'long_description': "# pyb_utils: utilities for PyBullet\n\nThis is a collection of utilities I've found useful for working with PyBullet,\nincluding:\n* Collision detection: conveniently set up shortest distance computations and\n  collision checking between arbitrary objects in arbitrary configurations with\n  PyBullet. See the accompanying [blog post](https://adamheins.com/blog/collision-detection-pybullet).\n* Ghost objects: add purely visual objects to the simulation, optionally\n  attached to another body.\n* Camera: virtual camera from which to get RGBA, depth, segmentation, and point\n  cloud data. Also provides video recording using OpenCV.\n\n## Install and run\nThis package requires **Python 3.7+**. It has been tested on Ubuntu 16.04,\n18.04, and 20.04.\n\n### From source\nClone the repo:\n```bash\ngit clone https://github.com/adamheins/pyb_utils\ncd pyb_utils\n```\n\nInstall using [poetry](https://python-poetry.org/):\n```bash\npoetry install\npoetry run python scripts/collision_detection_example.py  # for example\n```\n\nOr using pip:\n```bash\npython -m pip install .\n```\n\n### Directly from GitHub\n```\npython -m pip install git+https://github.com/adamheins/pyb_utils\n```\n\n## Usage and examples\nYou can find example scripts demonstrating all of this package's utilities in\nthe `scripts/` directory:\n\n* [collision detection](https://github.com/adamheins/pyb_utils/blob/main/scripts/collision_detection_example.py)\n* [ghost objects](https://github.com/adamheins/pyb_utils/blob/main/scripts/ghost_object_example.py)\n* [camera](https://github.com/adamheins/pyb_utils/blob/main/scripts/camera_example.py)\n* [video](https://github.com/adamheins/pyb_utils/blob/main/scripts/video_example.py)\n\n## Known issues\nFeel free to open issues (or better yet, a pull request!) if you find a\nproblem. Currently known issues:\n\n* Video recording does not output MP4 videos correctly. The AVI format works,\n  however.\n* Ghost objects sometimes flicker (spooky, but undesirable).\n\n## License\n[MIT](https://github.com/adamheins/pyb_utils/blob/main/LICENSE)\n",
+    'long_description': "# pyb_utils: utilities for PyBullet\n\nThis is a collection of utilities I've found useful for working with PyBullet,\nincluding:\n* Collision detection: conveniently set up shortest distance computations and\n  collision checking between arbitrary objects in arbitrary configurations with\n  PyBullet. See the accompanying [blog post](https://adamheins.com/blog/collision-detection-pybullet).\n* Ghost objects: add purely visual objects to the simulation, optionally\n  attached to another body.\n* Camera: virtual camera from which to get RGBA, depth, segmentation, and point\n  cloud data. Also provides video recording using OpenCV.\n\n## Install and run\nThis package requires **Python 3.7+**. It has been tested on Ubuntu 16.04,\n18.04, and 20.04.\n\n### From pip\n```\npip install pyb_utils\n```\n\n### From source\nClone the repo:\n```bash\ngit clone https://github.com/adamheins/pyb_utils\ncd pyb_utils\n```\n\nInstall using [poetry](https://python-poetry.org/):\n```bash\npoetry install\npoetry run python scripts/collision_detection_example.py  # for example\n```\n\nOr using pip:\n```bash\npython -m pip install .\n```\n\n## Usage and examples\nYou can find example scripts demonstrating all of this package's utilities in\nthe `scripts/` directory:\n\n* [collision detection](https://github.com/adamheins/pyb_utils/blob/main/scripts/collision_detection_example.py)\n* [ghost objects](https://github.com/adamheins/pyb_utils/blob/main/scripts/ghost_object_example.py)\n* [camera](https://github.com/adamheins/pyb_utils/blob/main/scripts/camera_example.py)\n* [video](https://github.com/adamheins/pyb_utils/blob/main/scripts/video_example.py)\n\n## Known issues\nFeel free to open issues (or better yet, a pull request!) if you find a\nproblem. Currently known issues:\n\n* Video recording does not output MP4 videos correctly. The AVI format works,\n  however.\n* Ghost objects sometimes flicker (spooky, but undesirable).\n\n## License\n[MIT](https://github.com/adamheins/pyb_utils/blob/main/LICENSE)\n",
     'author': 'Adam Heins',
     'author_email': 'mail@adamheins.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pyb_utils-0.2.2/PKG-INFO` & `pyb_utils-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyb-utils
-Version: 0.2.2
+Version: 0.2.3
 Summary: Basic utilities for PyBullet, including collision detection, ghost (i.e. visual-only) objects, and cameras.
 License: MIT
 Author: Adam Heins
 Author-email: mail@adamheins.com
 Requires-Python: >=3.7,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -32,14 +32,19 @@
 * Camera: virtual camera from which to get RGBA, depth, segmentation, and point
   cloud data. Also provides video recording using OpenCV.
 
 ## Install and run
 This package requires **Python 3.7+**. It has been tested on Ubuntu 16.04,
 18.04, and 20.04.
 
+### From pip
+```
+pip install pyb_utils
+```
+
 ### From source
 Clone the repo:
 ```bash
 git clone https://github.com/adamheins/pyb_utils
 cd pyb_utils
 ```
 
@@ -50,19 +55,14 @@
 ```
 
 Or using pip:
 ```bash
 python -m pip install .
 ```
 
-### Directly from GitHub
-```
-python -m pip install git+https://github.com/adamheins/pyb_utils
-```
-
 ## Usage and examples
 You can find example scripts demonstrating all of this package's utilities in
 the `scripts/` directory:
 
 * [collision detection](https://github.com/adamheins/pyb_utils/blob/main/scripts/collision_detection_example.py)
 * [ghost objects](https://github.com/adamheins/pyb_utils/blob/main/scripts/ghost_object_example.py)
 * [camera](https://github.com/adamheins/pyb_utils/blob/main/scripts/camera_example.py)
```

