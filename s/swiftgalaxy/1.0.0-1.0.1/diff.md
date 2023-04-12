# Comparing `tmp/swiftgalaxy-1.0.0.tar.gz` & `tmp/swiftgalaxy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftgalaxy-1.0.0.tar", last modified: Tue Jul 12 13:38:33 2022, max compression
+gzip compressed data, was "swiftgalaxy-1.0.1.tar", last modified: Wed Apr 12 16:39:01 2023, max compression
```

## Comparing `swiftgalaxy-1.0.0.tar` & `swiftgalaxy-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 13:38:33.379013 swiftgalaxy-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)    35148 2022-07-12 13:37:58.000000 swiftgalaxy-1.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-07-12 13:37:58.000000 swiftgalaxy-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-07-12 13:38:33.379013 swiftgalaxy-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2284 2022-07-12 13:37:58.000000 swiftgalaxy-1.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-12 13:38:33.379013 swiftgalaxy-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      551 2022-07-12 13:37:58.000000 swiftgalaxy-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 13:38:33.379013 swiftgalaxy-1.0.0/swiftgalaxy/
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-07-12 13:37:58.000000 swiftgalaxy-1.0.0/swiftgalaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-07-12 13:37:58.000000 swiftgalaxy-1.0.0/swiftgalaxy/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13008 2022-07-12 13:37:58.000000 swiftgalaxy-1.0.0/swiftgalaxy/halo_finders.py
--rw-r--r--   0 runner    (1001) docker     (121)     1607 2022-07-12 13:37:58.000000 swiftgalaxy-1.0.0/swiftgalaxy/masks.py
--rw-r--r--   0 runner    (1001) docker     (121)    68135 2022-07-12 13:37:58.000000 swiftgalaxy-1.0.0/swiftgalaxy/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 13:38:33.379013 swiftgalaxy-1.0.0/swiftgalaxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-07-12 13:38:33.000000 swiftgalaxy-1.0.0/swiftgalaxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      372 2022-07-12 13:38:33.000000 swiftgalaxy-1.0.0/swiftgalaxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-12 13:38:33.000000 swiftgalaxy-1.0.0/swiftgalaxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-12 13:38:30.000000 swiftgalaxy-1.0.0/swiftgalaxy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-07-12 13:38:33.000000 swiftgalaxy-1.0.0/swiftgalaxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-07-12 13:38:33.000000 swiftgalaxy-1.0.0/swiftgalaxy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:39:01.051945 swiftgalaxy-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-12 16:38:25.000000 swiftgalaxy-1.0.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-12 16:38:25.000000 swiftgalaxy-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-12 16:39:01.051945 swiftgalaxy-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-12 16:38:25.000000 swiftgalaxy-1.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 16:39:01.051945 swiftgalaxy-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-12 16:38:25.000000 swiftgalaxy-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:39:01.051945 swiftgalaxy-1.0.1/swiftgalaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-12 16:38:25.000000 swiftgalaxy-1.0.1/swiftgalaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 16:38:25.000000 swiftgalaxy-1.0.1/swiftgalaxy/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-04-12 16:38:25.000000 swiftgalaxy-1.0.1/swiftgalaxy/halo_finders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-12 16:38:25.000000 swiftgalaxy-1.0.1/swiftgalaxy/masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67805 2023-04-12 16:38:25.000000 swiftgalaxy-1.0.1/swiftgalaxy/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:39:01.051945 swiftgalaxy-1.0.1/swiftgalaxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-12 16:39:00.000000 swiftgalaxy-1.0.1/swiftgalaxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-12 16:39:00.000000 swiftgalaxy-1.0.1/swiftgalaxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:39:00.000000 swiftgalaxy-1.0.1/swiftgalaxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:38:58.000000 swiftgalaxy-1.0.1/swiftgalaxy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-12 16:39:00.000000 swiftgalaxy-1.0.1/swiftgalaxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 16:39:00.000000 swiftgalaxy-1.0.1/swiftgalaxy.egg-info/top_level.txt
```

### Comparing `swiftgalaxy-1.0.0/LICENSE.md` & `swiftgalaxy-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `swiftgalaxy-1.0.0/README.rst` & `swiftgalaxy-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `swiftgalaxy-1.0.0/setup.py` & `swiftgalaxy-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `swiftgalaxy-1.0.0/swiftgalaxy/halo_finders.py` & `swiftgalaxy-1.0.1/swiftgalaxy/halo_finders.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,15 +172,15 @@
         velociraptor_filebase: str = None,
         velociraptor_files: dict = None,
         halo_index: int = None,
         extra_mask: Union[str, MaskCollection] = "bound_only",
         centre_type: str = "minpot",  # _gas _star mbp minpot
         velociraptor_suffix: str = "",
     ) -> None:
-        from velociraptor.catalogue.catalogue import VelociraptorCatalogue
+        from velociraptor.catalogue.catalogue import Catalogue
 
         if velociraptor_filebase is not None and velociraptor_files is not None:
             raise ValueError(
                 "Provide either velociraptor_filebase or velociraptor_files, not both."
             )
         elif velociraptor_files is not None:
             self.velociraptor_files = velociraptor_files
@@ -194,15 +194,15 @@
                 "Provide one of velociraptor_filebase or velociraptor_files."
             )
         if halo_index is None:
             raise ValueError("Provide a halo_index.")
         else:
             self.halo_index: int = halo_index
         self.centre_type: str = centre_type
-        self._catalogue: Optional[VelociraptorCatalogue] = None
+        self._catalogue: Optional[Catalogue] = None
         self._particles: Optional[None] = None
         super().__init__(extra_mask=extra_mask)
         # currently velociraptor_python works with a halo index, not halo_id
         # self.catalogue_mask = (catalogue.ids.id == halo_id).nonzero()
         return
 
     def _load(self) -> None:
@@ -214,16 +214,15 @@
             self.scale_factor = (
                 float(propfile["SimulationInfo"].attrs["ScaleFactor"])
                 if propfile["SimulationInfo"].attrs["Cosmological_Sim"]
                 else 1.0
             )
 
         self._catalogue = load_catalogue(
-            self.velociraptor_files["properties"],
-            mask=self.halo_index,
+            self.velociraptor_files["properties"], mask=self.halo_index
         )
         groups = load_groups(
             self.velociraptor_files["catalog_groups"],
             catalogue=load_catalogue(self.velociraptor_files["properties"]),
         )
         self._particles, unbound_particles = groups.extract_halo(
             halo_index=self.halo_index
```

### Comparing `swiftgalaxy-1.0.0/swiftgalaxy/masks.py` & `swiftgalaxy-1.0.1/swiftgalaxy/masks.py`

 * *Files identical despite different names*

### Comparing `swiftgalaxy-1.0.0/swiftgalaxy/reader.py` & `swiftgalaxy-1.0.1/swiftgalaxy/reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,33 +32,26 @@
 from swiftgalaxy.halo_finders import _HaloFinder
 from swiftgalaxy.masks import MaskCollection
 
 from typing import Union, Any, Optional, Set
 
 
 def _apply_box_wrap(coords: cosmo_array, boxsize: Optional[cosmo_array]) -> cosmo_array:
-    retval = coords
     if boxsize is None:
-        return retval
+        return coords
     # Would like to ensure comoving coordinates here, but metadata gives boxsize as a
     # unyt_array instead of a cosmo_array. Pending swiftsimio issue #128. When
     # implementing, remove cast(s) to cosmo_array in test_coordinate_transformations.
     with catch_warnings():
         filterwarnings(
             "ignore", category=RuntimeWarning, message="Mixing ufunc arguments"
         )
-        for axis in range(3):
-            too_high = retval[:, axis] > boxsize[axis] / 2.0
-            while too_high.any():
-                retval[too_high, axis] -= boxsize[axis]
-                too_high = retval[:, axis] > boxsize[axis] / 2.0
-            too_low = retval[:, axis] <= -boxsize[axis] / 2.0
-            while too_low.any():
-                retval[too_low, axis] += boxsize[axis]
-                too_low = retval[:, axis] <= -boxsize[axis] / 2.0
+        retval = (coords + boxsize / 2.0) % boxsize - boxsize / 2.0
+    retval.comoving = coords.comoving
+    retval.cosmo_factor = coords.cosmo_factor
     return retval
 
 
 def _apply_translation(coords: cosmo_array, offset: cosmo_array) -> cosmo_array:
     if hasattr(offset, "comoving") and coords.comoving:
         offset = offset.to_comoving()
     elif hasattr(offset, "comoving") and not coords.comoving:
```

