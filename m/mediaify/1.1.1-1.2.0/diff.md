# Comparing `tmp/mediaify-1.1.1.tar.gz` & `tmp/mediaify-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mediaify-1.1.1.tar", last modified: Tue Apr 11 13:06:53 2023, max compression
+gzip compressed data, was "mediaify-1.2.0.tar", last modified: Wed Apr 12 19:27:43 2023, max compression
```

## Comparing `mediaify-1.1.1.tar` & `mediaify-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,26 @@
--rw-r--r--   0        0        0     1147 2023-04-11 13:06:43.340757 mediaify-1.1.1/LICENSE
--rw-r--r--   0        0        0      935 2023-04-11 13:06:43.340757 mediaify-1.1.1/README.md
--rw-r--r--   0        0        0      359 2023-04-11 13:06:43.340757 mediaify-1.1.1/mediaify/__init__.py
--rw-r--r--   0        0        0      753 2023-04-11 13:06:43.340757 mediaify-1.1.1/mediaify/configs.py
--rw-r--r--   0        0        0      335 2023-04-11 13:06:43.340757 mediaify-1.1.1/mediaify/encoders/__init__.py
--rw-r--r--   0        0        0     4252 2023-04-11 13:06:43.340757 mediaify-1.1.1/mediaify/encoders/animation.py
--rw-r--r--   0        0        0     2615 2023-04-11 13:06:43.340757 mediaify-1.1.1/mediaify/encoders/image.py
--rw-r--r--   0        0        0     1954 2023-04-11 13:06:43.340757 mediaify-1.1.1/mediaify/encoders/probe.py
--rw-r--r--   0        0        0      727 2023-04-11 13:06:43.340757 mediaify-1.1.1/mediaify/encoders/utils.py
--rw-r--r--   0        0        0     2496 2023-04-11 13:06:43.340757 mediaify-1.1.1/mediaify/encoders/video.py
--rw-r--r--   0        0        0     2342 2023-04-11 13:06:43.340757 mediaify-1.1.1/mediaify/presets.py
--rw-r--r--   0        0        0     1014 2023-04-11 13:06:43.340757 mediaify-1.1.1/mediaify/types.py
--rw-r--r--   0        0        0     1903 2023-04-11 13:06:43.340757 mediaify-1.1.1/mediaify/utils.py
--rw-r--r--   0        0        0     1657 2023-04-11 13:06:43.340757 mediaify-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     2279 1970-01-01 00:00:00.000000 mediaify-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1147 2023-04-12 19:27:33.525744 mediaify-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2445 2023-04-12 19:27:33.525744 mediaify-1.2.0/README.md
+-rw-r--r--   0        0        0     1341 2023-04-12 19:27:33.541745 mediaify-1.2.0/mediaify/__init__.py
+-rw-r--r--   0        0        0      185 2023-04-12 19:27:33.541745 mediaify-1.2.0/mediaify/animation/__init__.py
+-rw-r--r--   0        0        0     2466 2023-04-12 19:27:33.541745 mediaify-1.2.0/mediaify/animation/encode.py
+-rw-r--r--   0        0        0     1321 2023-04-12 19:27:33.541745 mediaify-1.2.0/mediaify/animation/exports.py
+-rw-r--r--   0        0        0     1302 2023-04-12 19:27:33.541745 mediaify-1.2.0/mediaify/animation/gif.py
+-rw-r--r--   0        0        0      805 2023-04-12 19:27:33.541745 mediaify-1.2.0/mediaify/animation/utils.py
+-rw-r--r--   0        0        0     1446 2023-04-12 19:27:33.541745 mediaify-1.2.0/mediaify/animation/webp.py
+-rw-r--r--   0        0        0      940 2023-04-12 19:27:33.541745 mediaify-1.2.0/mediaify/configs.py
+-rw-r--r--   0        0        0     2434 2023-04-12 19:27:33.541745 mediaify-1.2.0/mediaify/files.py
+-rw-r--r--   0        0        0      145 2023-04-12 19:27:33.541745 mediaify-1.2.0/mediaify/image/__init__.py
+-rw-r--r--   0        0        0     1643 2023-04-12 19:27:33.541745 mediaify-1.2.0/mediaify/image/encode.py
+-rw-r--r--   0        0        0     1104 2023-04-12 19:27:33.541745 mediaify-1.2.0/mediaify/image/exports.py
+-rw-r--r--   0        0        0      789 2023-04-12 19:27:33.541745 mediaify-1.2.0/mediaify/image/webp.py
+-rw-r--r--   0        0        0     2457 2023-04-12 19:27:33.541745 mediaify-1.2.0/mediaify/media.py
+-rw-r--r--   0        0        0     2518 2023-04-12 19:27:33.541745 mediaify-1.2.0/mediaify/presets.py
+-rw-r--r--   0        0        0      711 2023-04-12 19:27:33.541745 mediaify-1.2.0/mediaify/utils.py
+-rw-r--r--   0        0        0      162 2023-04-12 19:27:33.541745 mediaify-1.2.0/mediaify/video/__init__.py
+-rw-r--r--   0        0        0     1144 2023-04-12 19:27:33.541745 mediaify-1.2.0/mediaify/video/encode.py
+-rw-r--r--   0        0        0     1154 2023-04-12 19:27:33.541745 mediaify-1.2.0/mediaify/video/exports.py
+-rw-r--r--   0        0        0     1804 2023-04-12 19:27:33.541745 mediaify-1.2.0/mediaify/video/info.py
+-rw-r--r--   0        0        0     1445 2023-04-12 19:27:33.541745 mediaify-1.2.0/mediaify/video/summary.py
+-rw-r--r--   0        0        0      900 2023-04-12 19:27:33.541745 mediaify-1.2.0/mediaify/video/thumbnail.py
+-rw-r--r--   0        0        0     1653 2023-04-12 19:27:33.541745 mediaify-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3800 1970-01-01 00:00:00.000000 mediaify-1.2.0/PKG-INFO
```

### Comparing `mediaify-1.1.1/LICENSE` & `mediaify-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mediaify-1.1.1/mediaify/configs.py` & `mediaify-1.2.0/mediaify/configs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,49 @@
 from dataclasses import dataclass
 from typing_extensions import TypeAlias
 
+ImageConfig: TypeAlias = \
+    "ThumbnailConfig | UnencodedConfig | WEBPImageEncodeConfig"
+AnimationConfig: TypeAlias = \
+    "ThumbnailConfig | UnencodedConfig | GIFEncodeConfig | WEBPAnimationEncodeConfig"
+VideoConfig: TypeAlias = \
+    "ThumbnailConfig | UnencodedConfig | AnimationSummaryConfig"
+
 
 @dataclass
-class OriginalFileConfig:
+class UnencodedConfig:
     pass
 
 
 @dataclass
-class ImageEncodeConfig:
+class WEBPImageEncodeConfig:
     width: int
     height: int
     quality: int = 100
     lossless: bool = False
 
 
 @dataclass
-class AnimationEncodeConfig:
+class GIFEncodeConfig:
     width: int
     height: int
-    quality: int = 100
-    lossless: bool = False
 
 
 @dataclass
-class ThumbnailConfig(ImageEncodeConfig):
-    offset: float = 0.5
+class WEBPAnimationEncodeConfig:
+    width: int
+    height: int
+    quality: int = 100
+    lossless: bool = False
 
 
 @dataclass
-class AnimationSummaryConfig(AnimationEncodeConfig):
-    frames: int = 0
+class ThumbnailConfig:
+    encoding: ImageConfig
+    offset: float = 0.2
 
 
-ImageConfig: TypeAlias = "ImageEncodeConfig | OriginalFileConfig"
-AnimationConfig: TypeAlias = "ThumbnailConfig | AnimationEncodeConfig | OriginalFileConfig"
-VideoConfig: TypeAlias = "ThumbnailConfig | OriginalFileConfig"
+@dataclass
+class AnimationSummaryConfig:
+    encoding: AnimationConfig
+    framerate: int = 5
+    frames: int = 20
```

### Comparing `mediaify-1.1.1/pyproject.toml` & `mediaify-1.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.8.0,<4"]
 
 [project]
 name = "mediaify"
-version = "1.1.1"
-description = "Encoding media into multiple qualities"
+version = "1.2.0"
+description = "Media encoding made simple"
 license = {file = "LICENSE"}
 readme = "README.md"
 authors = [
     {name = "Ben Brady", email = "benbradybusiness@gmail.com"},
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -32,14 +32,15 @@
 ]
 requires-python = ">=3.7"
 dependencies = [
     "ffmpeg-python~=0.2.0",
     "pillow~=9.5.0",
     "python_magic~=0.4.27",
     "python-magic-bin; sys_platform == 'win32'",
+    "numexpr",
 ]
 [project.urls]
 Source = "https://github.com/Ben-Brady/mediaify"
 
 
 [project.optional-dependencies]
 test = [
@@ -53,17 +54,12 @@
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "-ra -q"
 testpaths = [
     "tests",
 ]
 
-# [tool.mypy]
-# strict = true
-
-
-# [tool.coverage.run]
-# parallel = true
-# source = [
-#     "mediaify"
-# ]
-
+[tool.mypy]
+warn_return_any = true
+warn_unused_configs = true
+strict = true
+files = ["mediaify/**"]
```

