# Comparing `tmp/simpleimageio-1.3.0.tar.gz` & `tmp/simpleimageio-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleimageio-1.3.0.tar", last modified: Tue Apr 11 18:26:31 2023, max compression
+gzip compressed data, was "simpleimageio-1.3.1.tar", last modified: Wed Apr 12 18:32:52 2023, max compression
```

## Comparing `simpleimageio-1.3.0.tar` & `simpleimageio-1.3.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:26:31.339984 simpleimageio-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:26:31.331983 simpleimageio-1.3.0/Core/
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/Core/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:26:31.335984 simpleimageio-1.3.0/Core/External/
--rw-r--r--   0 runner    (1001) docker     (123)   114725 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/Core/External/fpng.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/Core/External/fpng.h
--rw-r--r--   0 runner    (1001) docker     (123)   319839 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/Core/External/miniz.c
--rw-r--r--   0 runner    (1001) docker     (123)    69441 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/Core/External/miniz.h
--rw-r--r--   0 runner    (1001) docker     (123)   273149 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/Core/External/stb_image.h
--rw-r--r--   0 runner    (1001) docker     (123)    69564 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/Core/External/stb_image_write.h
--rw-r--r--   0 runner    (1001) docker     (123)   163059 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/Core/External/tiny_dng_loader.h
--rw-r--r--   0 runner    (1001) docker     (123)    38477 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/Core/External/tiny_dng_writer.h
--rw-r--r--   0 runner    (1001) docker     (123)   269883 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/Core/External/tinyexr.h
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/Core/error_metrics.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11082 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/Core/filter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/Core/image.h
--rw-r--r--   0 runner    (1001) docker     (123)    33227 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/Core/imageio.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/Core/manipulation.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/Core/tonemapping.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/Core/vec3.h
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-04-11 18:26:31.335984 simpleimageio-1.3.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:26:31.331983 simpleimageio-1.3.0/PyWrapper/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:26:31.335984 simpleimageio-1.3.0/PyWrapper/simpleimageio/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-11 18:26:28.000000 simpleimageio-1.3.0/PyWrapper/simpleimageio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-11 18:26:28.000000 simpleimageio-1.3.0/PyWrapper/simpleimageio/corelib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-11 18:26:28.000000 simpleimageio-1.3.0/PyWrapper/simpleimageio/error_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-04-11 18:26:28.000000 simpleimageio-1.3.0/PyWrapper/simpleimageio/flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-04-11 18:26:28.000000 simpleimageio-1.3.0/PyWrapper/simpleimageio/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    36113 2023-04-11 18:26:28.000000 simpleimageio-1.3.0/PyWrapper/simpleimageio/imageViewer.js
--rw-r--r--   0 runner    (1001) docker     (123)    89794 2023-04-11 18:26:28.000000 simpleimageio-1.3.0/PyWrapper/simpleimageio/jquery-3.6.4.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-11 18:26:28.000000 simpleimageio-1.3.0/PyWrapper/simpleimageio/manip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-11 18:26:28.000000 simpleimageio-1.3.0/PyWrapper/simpleimageio/style.css
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-04-11 18:26:28.000000 simpleimageio-1.3.0/PyWrapper/simpleimageio/tev.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-11 18:26:28.000000 simpleimageio-1.3.0/PyWrapper/simpleimageio/tonemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-04-11 18:26:28.000000 simpleimageio-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-11 18:26:28.000000 simpleimageio-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 18:26:31.339984 simpleimageio-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-11 18:26:28.000000 simpleimageio-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:26:31.335984 simpleimageio-1.3.0/simpleimageio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-04-11 18:26:31.000000 simpleimageio-1.3.0/simpleimageio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-11 18:26:31.000000 simpleimageio-1.3.0/simpleimageio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:26:31.000000 simpleimageio-1.3.0/simpleimageio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-11 18:26:31.000000 simpleimageio-1.3.0/simpleimageio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-11 18:26:31.000000 simpleimageio-1.3.0/simpleimageio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:32:52.480255 simpleimageio-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:32:52.476256 simpleimageio-1.3.1/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/Core/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:32:52.476256 simpleimageio-1.3.1/Core/External/
+-rw-r--r--   0 runner    (1001) docker     (123)   114725 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/Core/External/fpng.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/Core/External/fpng.h
+-rw-r--r--   0 runner    (1001) docker     (123)   319839 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/Core/External/miniz.c
+-rw-r--r--   0 runner    (1001) docker     (123)    69441 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/Core/External/miniz.h
+-rw-r--r--   0 runner    (1001) docker     (123)   273149 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/Core/External/stb_image.h
+-rw-r--r--   0 runner    (1001) docker     (123)    69564 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/Core/External/stb_image_write.h
+-rw-r--r--   0 runner    (1001) docker     (123)   163059 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/Core/External/tiny_dng_loader.h
+-rw-r--r--   0 runner    (1001) docker     (123)    38477 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/Core/External/tiny_dng_writer.h
+-rw-r--r--   0 runner    (1001) docker     (123)   269883 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/Core/External/tinyexr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/Core/error_metrics.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11082 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/Core/filter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/Core/image.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34881 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/Core/imageio.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/Core/manipulation.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/Core/tonemapping.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/Core/vec3.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-04-12 18:32:52.480255 simpleimageio-1.3.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:32:52.476256 simpleimageio-1.3.1/PyWrapper/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:32:52.480255 simpleimageio-1.3.1/PyWrapper/simpleimageio/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-12 18:32:50.000000 simpleimageio-1.3.1/PyWrapper/simpleimageio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-12 18:32:50.000000 simpleimageio-1.3.1/PyWrapper/simpleimageio/corelib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-12 18:32:50.000000 simpleimageio-1.3.1/PyWrapper/simpleimageio/error_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-04-12 18:32:50.000000 simpleimageio-1.3.1/PyWrapper/simpleimageio/flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-04-12 18:32:50.000000 simpleimageio-1.3.1/PyWrapper/simpleimageio/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35670 2023-04-12 18:32:50.000000 simpleimageio-1.3.1/PyWrapper/simpleimageio/imageViewer.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89794 2023-04-12 18:32:50.000000 simpleimageio-1.3.1/PyWrapper/simpleimageio/jquery-3.6.4.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-12 18:32:50.000000 simpleimageio-1.3.1/PyWrapper/simpleimageio/manip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-12 18:32:50.000000 simpleimageio-1.3.1/PyWrapper/simpleimageio/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-04-12 18:32:50.000000 simpleimageio-1.3.1/PyWrapper/simpleimageio/tev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-12 18:32:50.000000 simpleimageio-1.3.1/PyWrapper/simpleimageio/tonemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-04-12 18:32:50.000000 simpleimageio-1.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-12 18:32:50.000000 simpleimageio-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 18:32:52.480255 simpleimageio-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-12 18:32:50.000000 simpleimageio-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:32:52.480255 simpleimageio-1.3.1/simpleimageio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-04-12 18:32:52.000000 simpleimageio-1.3.1/simpleimageio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-12 18:32:52.000000 simpleimageio-1.3.1/simpleimageio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 18:32:52.000000 simpleimageio-1.3.1/simpleimageio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 18:32:52.000000 simpleimageio-1.3.1/simpleimageio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-12 18:32:52.000000 simpleimageio-1.3.1/simpleimageio.egg-info/top_level.txt
```

### Comparing `simpleimageio-1.3.0/Core/CMakeLists.txt` & `simpleimageio-1.3.1/Core/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.0/Core/External/fpng.cpp` & `simpleimageio-1.3.1/Core/External/fpng.cpp`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.0/Core/External/fpng.h` & `simpleimageio-1.3.1/Core/External/fpng.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.0/Core/External/miniz.c` & `simpleimageio-1.3.1/Core/External/miniz.c`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.0/Core/External/miniz.h` & `simpleimageio-1.3.1/Core/External/miniz.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.0/Core/External/stb_image.h` & `simpleimageio-1.3.1/Core/External/stb_image.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.0/Core/External/stb_image_write.h` & `simpleimageio-1.3.1/Core/External/stb_image_write.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.0/Core/External/tiny_dng_loader.h` & `simpleimageio-1.3.1/Core/External/tiny_dng_loader.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.0/Core/External/tiny_dng_writer.h` & `simpleimageio-1.3.1/Core/External/tiny_dng_writer.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.0/Core/External/tinyexr.h` & `simpleimageio-1.3.1/Core/External/tinyexr.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.0/Core/error_metrics.cpp` & `simpleimageio-1.3.1/Core/error_metrics.cpp`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.0/Core/filter.cpp` & `simpleimageio-1.3.1/Core/filter.cpp`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.0/Core/image.h` & `simpleimageio-1.3.1/Core/image.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.0/Core/imageio.cpp` & `simpleimageio-1.3.1/Core/imageio.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -896,8 +896,60 @@
         cacheMutex.unlock();
     } else {
         cacheMutex.unlock();
         std::cerr << "ERROR: attempted to copy non-existing image id " << id << std::endl;
     }
 }
 
+
+SIIO_API int GetExrLayerNames(const char* filename, char*** names) {
+    EXRVersion exrVersion;
+    int ret = ParseEXRVersionFromFile(&exrVersion, filename);
+    if (ret != 0) {
+        std::cerr << "Error loading '" << filename << "': Invalid .exr file. " << std::endl;
+        return -1;
+    }
+
+    const char* err;
+    EXRHeader header;
+    InitEXRHeader(&header);
+    ret = ParseEXRHeaderFromFile(&header, &exrVersion, filename, &err);
+    if (ret) {
+        std::cerr << "Error loading '" << filename << "': " << err << std::endl;
+        FreeEXRErrorMessage(err);
+        return -1;
+    }
+
+    // Read the number of channels in each layer
+    int freeChannels = 0;
+    std::unordered_set<std::string> layerNames;
+    for (int chan = 0; chan < header.num_channels; ++chan) {
+        // Extract the layer name by assuming a channel name of the form "layername.R", "layername.B" and so on
+        size_t len = strlen(header.channels[chan].name);
+        std::string layerName;
+        if (len <= 2) layerName = "";
+        else layerName = std::string(header.channels[chan].name, len - 2);
+        layerNames.insert(layerName);
+    }
+
+    FreeEXRHeader(&header);
+
+    int num = (int)layerNames.size();
+    *names = new char*[num];
+    auto iter = layerNames.begin();
+    for (int i = 0; i < num; ++i) {
+        (*names)[i] = new char[iter->size() + 1];
+        std::copy(iter->begin(), iter->end(), (*names)[i]);
+        (*names)[i][iter->size()] = 0;
+        iter++;
+    }
+    return num;
+}
+
+SIIO_API void DeleteExrLayerNames(int num, const char** names) {
+    for (int i = 0; i < num; ++i) {
+        delete[] names[i];
+    }
+    delete[] names;
+}
+
 } // extern "C"
```

### Comparing `simpleimageio-1.3.0/Core/manipulation.cpp` & `simpleimageio-1.3.1/Core/manipulation.cpp`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.0/Core/tonemapping.cpp` & `simpleimageio-1.3.1/Core/tonemapping.cpp`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.0/Core/vec3.h` & `simpleimageio-1.3.1/Core/vec3.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.0/LICENSE` & `simpleimageio-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.0/PKG-INFO` & `simpleimageio-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpleimageio
-Version: 1.3.0
+Version: 1.3.1
 Summary: A very simple Python wrapper to read and write various HDR and LDR image file formats.
 Home-page: https://github.com/pgrit/SimpleImageIO
 Author: Pascal Grittmann
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: simpleimageio Version: 1.3.0 Summary: A very simple
+Metadata-Version: 2.1 Name: simpleimageio Version: 1.3.1 Summary: A very simple
 Python wrapper to read and write various HDR and LDR image file formats. Home-
 page: https://github.com/pgrit/SimpleImageIO Author: Pascal Grittmann
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE ![Build](https://github.com/pgrit/SimpleImageIO/workflows/Build/
 badge.svg) [https://buildstats.info/nuget/SimpleImageIO] # Simple Image IO A
```

### Comparing `simpleimageio-1.3.0/PyWrapper/simpleimageio/corelib.py` & `simpleimageio-1.3.1/PyWrapper/simpleimageio/corelib.py`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.0/PyWrapper/simpleimageio/error_metrics.py` & `simpleimageio-1.3.1/PyWrapper/simpleimageio/error_metrics.py`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.0/PyWrapper/simpleimageio/flip.py` & `simpleimageio-1.3.1/PyWrapper/simpleimageio/flip.py`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.0/PyWrapper/simpleimageio/image.py` & `simpleimageio-1.3.1/PyWrapper/simpleimageio/image.py`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.0/PyWrapper/simpleimageio/imageViewer.js` & `simpleimageio-1.3.1/PyWrapper/simpleimageio/imageViewer.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -247,42 +247,25 @@
     let state = magnifierStates.get(container);
     if (!state.visible) return;
 
     let table = magnifier.find("table");
     table.children().remove();
 
     let activeImage = flipBookImages.get(container)[curImageIdx.get(container) - 1];
-
-    var canvas, pixels, buffer, glOrder;
     let size = 2 * MagnifierResolution + 1;
-    if (activeImage instanceof HDRImage) {
-        canvas = activeImage.canvas;
-        pixels = activeImage.pixels instanceof Float32Array ? activeImage.pixels : null;
-
-        let gl = canvas.getContext('webgl2');
-        buffer = new Uint8Array(size * size * 4);
-        gl.readPixels(state.col - MagnifierResolution, canvas.height - state.row - MagnifierResolution - 1,
-            size, size, gl.RGBA, gl.UNSIGNED_BYTE, buffer);
-
-        glOrder = true;
-    } else {
-        canvas = activeImage;
-        pixels = null;
 
-        let ctx = canvas.getContext('2d');
-        buffer = ctx.getImageData(state.col - MagnifierResolution, state.row - MagnifierResolution,
-            size, size).data;
-
-        glOrder = false;
-    }
+    let canvas = activeImage.canvas;
+    let pixels = activeImage.pixels instanceof Float32Array ? activeImage.pixels : null;
+    let ctx = canvas.getContext('2d');
+    let buffer = ctx.getImageData(state.col - MagnifierResolution, state.row - MagnifierResolution,
+        size, size).data;
 
-    let bufRow = glOrder ? size : -1;
+    let bufRow = -1;
     for (let row = state.row - MagnifierResolution; row <= state.row + MagnifierResolution; ++row) {
-        if (glOrder) bufRow--;
-        else bufRow++;
+        bufRow++;
         if (row < 0 || row >= canvas.height) continue;
 
         table.append("<tr></tr>");
         let tr = table.find("tr").last();
 
         let bufCol = -1;
         for (let col = state.col - MagnifierResolution; col <= state.col + MagnifierResolution; ++col) {
@@ -516,17 +499,17 @@
         $(flipbook).find(".tmo-script").removeClass("visible");
         $(flipbook).find(".tmo-falsecolor").removeClass("visible");
         $(flipbook).find(`.tmo-${initialTMO.name}`).addClass("visible");
     }
 }
 
 function renderImage(canvas, pixels, toneMapCode) {
-    const gl = canvas.getContext("webgl2", {
-        preserveDrawingBuffer: true
-    });
+    const offscreen = new OffscreenCanvas(canvas.width, canvas.height);
+    const gl = offscreen.getContext("webgl2");
+
     if (gl === null) {
         alert("Unable to initialize WebGL. Your browser or machine may not support it.");
         return;
     }
 
     const vsSource = `#version 300 es
 
@@ -693,14 +676,19 @@
     gl.enableVertexAttribArray(attribLocations.vertexPosition);
 
     gl.bindBuffer(gl.ARRAY_BUFFER, uvBuffer);
     gl.vertexAttribPointer(attribLocations.textureCoord, 2, gl.FLOAT, false, 0, 0);
     gl.enableVertexAttribArray(attribLocations.textureCoord);
 
     gl.drawArrays(gl.TRIANGLE_STRIP, 0, 4);
+
+    const ctx = canvas.getContext("2d", {
+        willReadFrequently: true
+    });
+    ctx.drawImage(offscreen.transferToImageBitmap(), 0, 0);
 }
 
 var lastFlipIdx = 0;
 /**
  *
  * @param {*} parentElement the DOM node to add this flipbook to
  * @param {*} names list of names, one for each image
@@ -844,16 +832,14 @@
         if (exponent == 0) {
             buffer[i] = 0.0; // TODO: proper mapping for subnormal numbers
         } else if (exponent == 31) {
             if (mantissa == 0)
                 buffer[i] = (255 << 23 | (sign << 31)) >>> 0;
             else
                 buffer[i] = ((1 << 13) | 255 << 23 | (1 << 31)) >>> 0;
-            console.log("got a nan / inf: ");
-            console.log(mantissa)
         } else {
             buffer[i] = ((mantissa << 13) | (exponent - 15 + 127) << 23 | (sign << 31)) >>> 0;
         }
     }
 
     // Now we create a new float32 view on the same underlying binary data
     return new Float32Array(buffer.buffer);
```

### Comparing `simpleimageio-1.3.0/PyWrapper/simpleimageio/jquery-3.6.4.min.js` & `simpleimageio-1.3.1/PyWrapper/simpleimageio/jquery-3.6.4.min.js`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.0/PyWrapper/simpleimageio/manip.py` & `simpleimageio-1.3.1/PyWrapper/simpleimageio/manip.py`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.0/PyWrapper/simpleimageio/style.css` & `simpleimageio-1.3.1/PyWrapper/simpleimageio/style.css`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.0/PyWrapper/simpleimageio/tev.py` & `simpleimageio-1.3.1/PyWrapper/simpleimageio/tev.py`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.0/PyWrapper/simpleimageio/tonemap.py` & `simpleimageio-1.3.1/PyWrapper/simpleimageio/tonemap.py`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.0/README.md` & `simpleimageio-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.0/setup.py` & `simpleimageio-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         os.chdir(str(cwd))
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='simpleimageio',
-    version='1.3.0',
+    version='1.3.1',
     author='Pascal Grittmann',
     url='https://github.com/pgrit/SimpleImageIO',
 
     description='A very simple Python wrapper to read and write various HDR and LDR image file formats.',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `simpleimageio-1.3.0/simpleimageio.egg-info/PKG-INFO` & `simpleimageio-1.3.1/simpleimageio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpleimageio
-Version: 1.3.0
+Version: 1.3.1
 Summary: A very simple Python wrapper to read and write various HDR and LDR image file formats.
 Home-page: https://github.com/pgrit/SimpleImageIO
 Author: Pascal Grittmann
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: simpleimageio Version: 1.3.0 Summary: A very simple
+Metadata-Version: 2.1 Name: simpleimageio Version: 1.3.1 Summary: A very simple
 Python wrapper to read and write various HDR and LDR image file formats. Home-
 page: https://github.com/pgrit/SimpleImageIO Author: Pascal Grittmann
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE ![Build](https://github.com/pgrit/SimpleImageIO/workflows/Build/
 badge.svg) [https://buildstats.info/nuget/SimpleImageIO] # Simple Image IO A
```

### Comparing `simpleimageio-1.3.0/simpleimageio.egg-info/SOURCES.txt` & `simpleimageio-1.3.1/simpleimageio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

