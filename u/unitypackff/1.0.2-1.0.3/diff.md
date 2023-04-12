# Comparing `tmp/unitypackff-1.0.2.tar.gz` & `tmp/unitypackff-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitypackff-1.0.2.tar", last modified: Tue Feb 14 08:46:31 2023, max compression
+gzip compressed data, was "unitypackff-1.0.3.tar", last modified: Wed Apr 12 14:34:34 2023, max compression
```

## Comparing `unitypackff-1.0.2.tar` & `unitypackff-1.0.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-02-14 08:46:31.024651 unitypackff-1.0.2/
--rw-rw-rw-   0        0        0     1074 2023-02-14 07:28:01.000000 unitypackff-1.0.2/LICENSE
--rw-rw-rw-   0        0        0    20918 2023-02-14 08:46:31.024651 unitypackff-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    19941 2023-02-14 07:39:24.000000 unitypackff-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-02-14 08:46:31.015958 unitypackff-1.0.2/bin/
--rw-rw-rw-   0        0        0     4999 2023-02-14 07:28:01.000000 unitypackff-1.0.2/bin/additem.py
--rw-rw-rw-   0        0        0     1014 2023-02-14 07:28:01.000000 unitypackff-1.0.2/bin/dump_terrain.py
--rw-rw-rw-   0        0        0      648 2023-02-14 07:28:01.000000 unitypackff-1.0.2/bin/dumpxdt.py
--rw-rw-rw-   0        0        0     7781 2023-02-14 07:28:01.000000 unitypackff-1.0.2/bin/ffextract.py
--rw-rw-rw-   0        0        0      404 2023-02-14 07:28:01.000000 unitypackff-1.0.2/bin/list_ab_alt.py
--rw-rw-rw-   0        0        0      388 2023-02-14 07:28:01.000000 unitypackff-1.0.2/bin/list_assetbundle.py
--rw-rw-rw-   0        0        0      380 2023-02-14 07:28:01.000000 unitypackff-1.0.2/bin/list_contents.py
--rw-rw-rw-   0        0        0     1007 2023-02-14 07:28:01.000000 unitypackff-1.0.2/bin/replace_mesh.py
--rw-rw-rw-   0        0        0      926 2023-02-14 07:28:01.000000 unitypackff-1.0.2/bin/replace_terrain.py
--rw-rw-rw-   0        0        0     3899 2023-02-14 07:28:01.000000 unitypackff-1.0.2/bin/show_gameobject.py
--rw-rw-rw-   0        0        0     2587 2023-02-14 07:28:01.000000 unitypackff-1.0.2/bin/unity2yaml.py
--rw-rw-rw-   0        0        0     5102 2023-02-14 07:28:01.000000 unitypackff-1.0.2/bin/unityextract.py
--rw-rw-rw-   0        0        0     1110 2023-02-14 08:46:31.025651 unitypackff-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      453 2023-02-14 08:39:04.000000 unitypackff-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-14 08:46:30.997891 unitypackff-1.0.2/unitypackff/
--rw-rw-rw-   0        0        0      357 2023-02-14 07:28:01.000000 unitypackff-1.0.2/unitypackff/__init__.py
--rw-rw-rw-   0        0        0     7968 2023-02-14 07:28:01.000000 unitypackff-1.0.2/unitypackff/asset.py
--rw-rw-rw-   0        0        0     6996 2023-02-14 07:28:01.000000 unitypackff-1.0.2/unitypackff/assetbundle.py
--rw-rw-rw-   0        0        0     5949 2023-02-14 07:28:01.000000 unitypackff-1.0.2/unitypackff/classes.json
-drwxrwxrwx   0        0        0        0 2023-02-14 08:46:31.006819 unitypackff-1.0.2/unitypackff/engine/
--rw-rw-rw-   0        0        0      790 2023-02-14 07:28:01.000000 unitypackff-1.0.2/unitypackff/engine/__init__.py
--rw-rw-rw-   0        0        0     2310 2023-02-14 07:28:01.000000 unitypackff-1.0.2/unitypackff/engine/animation.py
--rw-rw-rw-   0        0        0     2369 2023-02-14 07:28:01.000000 unitypackff-1.0.2/unitypackff/engine/audio.py
--rw-rw-rw-   0        0        0      376 2023-02-14 07:28:01.000000 unitypackff-1.0.2/unitypackff/engine/component.py
--rw-rw-rw-   0        0        0      396 2023-02-14 07:28:01.000000 unitypackff-1.0.2/unitypackff/engine/font.py
--rw-rw-rw-   0        0        0     1499 2023-02-14 07:28:01.000000 unitypackff-1.0.2/unitypackff/engine/mesh.py
--rw-rw-rw-   0        0        0      258 2023-02-14 07:28:01.000000 unitypackff-1.0.2/unitypackff/engine/movie.py
--rw-rw-rw-   0        0        0      708 2023-02-14 07:28:01.000000 unitypackff-1.0.2/unitypackff/engine/object.py
--rw-rw-rw-   0        0        0     1230 2023-02-14 07:28:01.000000 unitypackff-1.0.2/unitypackff/engine/particle.py
--rw-rw-rw-   0        0        0     1047 2023-02-14 07:28:01.000000 unitypackff-1.0.2/unitypackff/engine/physics.py
--rw-rw-rw-   0        0        0     2330 2023-02-14 07:28:01.000000 unitypackff-1.0.2/unitypackff/engine/renderer.py
--rw-rw-rw-   0        0        0     1262 2023-02-14 07:28:01.000000 unitypackff-1.0.2/unitypackff/engine/text.py
--rw-rw-rw-   0        0        0     5119 2023-02-14 07:28:01.000000 unitypackff-1.0.2/unitypackff/engine/texture.py
--rw-rw-rw-   0        0        0      812 2023-02-14 07:28:01.000000 unitypackff-1.0.2/unitypackff/enums.py
--rw-rw-rw-   0        0        0     3079 2023-02-14 07:28:01.000000 unitypackff-1.0.2/unitypackff/environment.py
--rw-rw-rw-   0        0        0     9167 2023-02-14 07:28:01.000000 unitypackff-1.0.2/unitypackff/export.py
--rw-rw-rw-   0        0        0     3774 2023-02-14 07:28:01.000000 unitypackff-1.0.2/unitypackff/modding.py
--rw-rw-rw-   0        0        0    11601 2023-02-14 07:28:01.000000 unitypackff-1.0.2/unitypackff/object.py
--rw-rw-rw-   0        0        0      358 2023-02-14 07:28:01.000000 unitypackff-1.0.2/unitypackff/resources.py
--rw-rw-rw-   0        0        0     1051 2023-02-14 07:28:01.000000 unitypackff-1.0.2/unitypackff/strings.dat
--rw-rw-rw-   0        0        0   295489 2023-02-14 07:28:01.000000 unitypackff-1.0.2/unitypackff/structs.dat
--rw-rw-rw-   0        0        0     4727 2023-02-14 07:28:01.000000 unitypackff-1.0.2/unitypackff/type.py
--rw-rw-rw-   0        0        0     5818 2023-02-14 07:28:01.000000 unitypackff-1.0.2/unitypackff/utils.py
-drwxrwxrwx   0        0        0        0 2023-02-14 08:46:31.021587 unitypackff-1.0.2/unitypackff.egg-info/
--rw-rw-rw-   0        0        0    20918 2023-02-14 08:46:30.000000 unitypackff-1.0.2/unitypackff.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1917 2023-02-14 08:46:30.000000 unitypackff-1.0.2/unitypackff.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-14 08:46:30.000000 unitypackff-1.0.2/unitypackff.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-02-14 08:46:30.000000 unitypackff-1.0.2/unitypackff.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-02-14 08:46:30.000000 unitypackff-1.0.2/unitypackff.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 14:34:34.221823 unitypackff-1.0.3/
+-rw-rw-rw-   0        0        0     1074 2023-02-14 07:28:01.000000 unitypackff-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0    20918 2023-04-12 14:34:34.221823 unitypackff-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    19941 2023-02-14 07:39:24.000000 unitypackff-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 14:34:34.212990 unitypackff-1.0.3/bin/
+-rw-rw-rw-   0        0        0     4999 2023-02-14 07:28:01.000000 unitypackff-1.0.3/bin/additem.py
+-rw-rw-rw-   0        0        0     1014 2023-02-14 07:28:01.000000 unitypackff-1.0.3/bin/dump_terrain.py
+-rw-rw-rw-   0        0        0      648 2023-02-14 07:28:01.000000 unitypackff-1.0.3/bin/dumpxdt.py
+-rw-rw-rw-   0        0        0     7781 2023-02-14 07:28:01.000000 unitypackff-1.0.3/bin/ffextract.py
+-rw-rw-rw-   0        0        0      404 2023-02-14 07:28:01.000000 unitypackff-1.0.3/bin/list_ab_alt.py
+-rw-rw-rw-   0        0        0      388 2023-02-14 07:28:01.000000 unitypackff-1.0.3/bin/list_assetbundle.py
+-rw-rw-rw-   0        0        0      380 2023-02-14 07:28:01.000000 unitypackff-1.0.3/bin/list_contents.py
+-rw-rw-rw-   0        0        0     1007 2023-02-14 07:28:01.000000 unitypackff-1.0.3/bin/replace_mesh.py
+-rw-rw-rw-   0        0        0      926 2023-02-14 07:28:01.000000 unitypackff-1.0.3/bin/replace_terrain.py
+-rw-rw-rw-   0        0        0     3899 2023-02-14 07:28:01.000000 unitypackff-1.0.3/bin/show_gameobject.py
+-rw-rw-rw-   0        0        0     2587 2023-02-14 07:28:01.000000 unitypackff-1.0.3/bin/unity2yaml.py
+-rw-rw-rw-   0        0        0     5102 2023-02-14 07:28:01.000000 unitypackff-1.0.3/bin/unityextract.py
+-rw-rw-rw-   0        0        0     1110 2023-04-12 14:34:34.223327 unitypackff-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      453 2023-02-14 08:39:04.000000 unitypackff-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:34:34.193107 unitypackff-1.0.3/unitypackff/
+-rw-rw-rw-   0        0        0      357 2023-02-14 07:28:01.000000 unitypackff-1.0.3/unitypackff/__init__.py
+-rw-rw-rw-   0        0        0     7968 2023-02-14 07:28:01.000000 unitypackff-1.0.3/unitypackff/asset.py
+-rw-rw-rw-   0        0        0     6996 2023-02-14 07:28:01.000000 unitypackff-1.0.3/unitypackff/assetbundle.py
+-rw-rw-rw-   0        0        0     5949 2023-02-14 07:28:01.000000 unitypackff-1.0.3/unitypackff/classes.json
+drwxrwxrwx   0        0        0        0 2023-04-12 14:34:34.202849 unitypackff-1.0.3/unitypackff/engine/
+-rw-rw-rw-   0        0        0      790 2023-02-14 07:28:01.000000 unitypackff-1.0.3/unitypackff/engine/__init__.py
+-rw-rw-rw-   0        0        0     2310 2023-02-14 07:28:01.000000 unitypackff-1.0.3/unitypackff/engine/animation.py
+-rw-rw-rw-   0        0        0     2369 2023-02-14 07:28:01.000000 unitypackff-1.0.3/unitypackff/engine/audio.py
+-rw-rw-rw-   0        0        0      376 2023-02-14 07:28:01.000000 unitypackff-1.0.3/unitypackff/engine/component.py
+-rw-rw-rw-   0        0        0      396 2023-02-14 07:28:01.000000 unitypackff-1.0.3/unitypackff/engine/font.py
+-rw-rw-rw-   0        0        0     1499 2023-02-14 07:28:01.000000 unitypackff-1.0.3/unitypackff/engine/mesh.py
+-rw-rw-rw-   0        0        0      258 2023-02-14 07:28:01.000000 unitypackff-1.0.3/unitypackff/engine/movie.py
+-rw-rw-rw-   0        0        0      708 2023-02-14 07:28:01.000000 unitypackff-1.0.3/unitypackff/engine/object.py
+-rw-rw-rw-   0        0        0     1230 2023-02-14 07:28:01.000000 unitypackff-1.0.3/unitypackff/engine/particle.py
+-rw-rw-rw-   0        0        0     1047 2023-02-14 07:28:01.000000 unitypackff-1.0.3/unitypackff/engine/physics.py
+-rw-rw-rw-   0        0        0     2330 2023-02-14 07:28:01.000000 unitypackff-1.0.3/unitypackff/engine/renderer.py
+-rw-rw-rw-   0        0        0     1262 2023-02-14 07:28:01.000000 unitypackff-1.0.3/unitypackff/engine/text.py
+-rw-rw-rw-   0        0        0     5119 2023-02-14 07:28:01.000000 unitypackff-1.0.3/unitypackff/engine/texture.py
+-rw-rw-rw-   0        0        0      812 2023-02-14 07:28:01.000000 unitypackff-1.0.3/unitypackff/enums.py
+-rw-rw-rw-   0        0        0     3079 2023-02-14 07:28:01.000000 unitypackff-1.0.3/unitypackff/environment.py
+-rw-rw-rw-   0        0        0     9167 2023-02-14 07:28:01.000000 unitypackff-1.0.3/unitypackff/export.py
+-rw-rw-rw-   0        0        0     3799 2023-04-12 14:32:04.000000 unitypackff-1.0.3/unitypackff/modding.py
+-rw-rw-rw-   0        0        0    11601 2023-02-14 07:28:01.000000 unitypackff-1.0.3/unitypackff/object.py
+-rw-rw-rw-   0        0        0      358 2023-02-14 07:28:01.000000 unitypackff-1.0.3/unitypackff/resources.py
+-rw-rw-rw-   0        0        0     1051 2023-02-14 07:28:01.000000 unitypackff-1.0.3/unitypackff/strings.dat
+-rw-rw-rw-   0        0        0   295489 2023-02-14 07:28:01.000000 unitypackff-1.0.3/unitypackff/structs.dat
+-rw-rw-rw-   0        0        0     4727 2023-02-14 07:28:01.000000 unitypackff-1.0.3/unitypackff/type.py
+-rw-rw-rw-   0        0        0     5818 2023-02-14 07:28:01.000000 unitypackff-1.0.3/unitypackff/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:34:34.219619 unitypackff-1.0.3/unitypackff.egg-info/
+-rw-rw-rw-   0        0        0    20918 2023-04-12 14:34:34.000000 unitypackff-1.0.3/unitypackff.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1917 2023-04-12 14:34:34.000000 unitypackff-1.0.3/unitypackff.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 14:34:34.000000 unitypackff-1.0.3/unitypackff.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-04-12 14:34:34.000000 unitypackff-1.0.3/unitypackff.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-12 14:34:34.000000 unitypackff-1.0.3/unitypackff.egg-info/top_level.txt
```

### Comparing `unitypackff-1.0.2/LICENSE` & `unitypackff-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unitypackff-1.0.2/PKG-INFO` & `unitypackff-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitypackff
-Version: 1.0.2
+Version: 1.0.3
 Summary: UnityPackFF is a fork of UnityPack specialized for working with FusionFall assets
 Home-page: https://github.com/SirDank/UnityPackFF
 Download-URL: https://github.com/SirDank/UnityPackFF/tarball/master
 Author: dongresource
 License: MIT
 Project-URL: GitHub, https://github.com/SirDank/UnityPackFF
 Project-URL: Bug Tracker, https://github.com/SirDank/UnityPackFF/issues
```

### Comparing `unitypackff-1.0.2/README.md` & `unitypackff-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `unitypackff-1.0.2/bin/additem.py` & `unitypackff-1.0.3/bin/additem.py`

 * *Files identical despite different names*

### Comparing `unitypackff-1.0.2/bin/dump_terrain.py` & `unitypackff-1.0.3/bin/dump_terrain.py`

 * *Files identical despite different names*

### Comparing `unitypackff-1.0.2/bin/dumpxdt.py` & `unitypackff-1.0.3/bin/dumpxdt.py`

 * *Files identical despite different names*

### Comparing `unitypackff-1.0.2/bin/ffextract.py` & `unitypackff-1.0.3/bin/ffextract.py`

 * *Files identical despite different names*

### Comparing `unitypackff-1.0.2/bin/replace_mesh.py` & `unitypackff-1.0.3/bin/replace_mesh.py`

 * *Files identical despite different names*

### Comparing `unitypackff-1.0.2/bin/replace_terrain.py` & `unitypackff-1.0.3/bin/replace_terrain.py`

 * *Files identical despite different names*

### Comparing `unitypackff-1.0.2/bin/show_gameobject.py` & `unitypackff-1.0.3/bin/show_gameobject.py`

 * *Files identical despite different names*

### Comparing `unitypackff-1.0.2/bin/unity2yaml.py` & `unitypackff-1.0.3/bin/unity2yaml.py`

 * *Files identical despite different names*

### Comparing `unitypackff-1.0.2/bin/unityextract.py` & `unitypackff-1.0.3/bin/unityextract.py`

 * *Files identical despite different names*

### Comparing `unitypackff-1.0.2/setup.cfg` & `unitypackff-1.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2075 6e69 7479 7061 636b 6666 0d0a   = unitypackff..
-00000020: 7665 7273 696f 6e20 3d20 312e 302e 320d  version = 1.0.2.
+00000020: 7665 7273 696f 6e20 3d20 312e 302e 330d  version = 1.0.3.
 00000030: 0a64 6573 6372 6970 7469 6f6e 203d 2055  .description = U
 00000040: 6e69 7479 5061 636b 4646 2069 7320 6120  nityPackFF is a 
 00000050: 666f 726b 206f 6620 556e 6974 7950 6163  fork of UnityPac
 00000060: 6b20 7370 6563 6961 6c69 7a65 6420 666f  k specialized fo
 00000070: 7220 776f 726b 696e 6720 7769 7468 2046  r working with F
 00000080: 7573 696f 6e46 616c 6c20 6173 7365 7473  usionFall assets
 00000090: 0d0a 6175 7468 6f72 203d 2064 6f6e 6772  ..author = dongr
```

### Comparing `unitypackff-1.0.2/unitypackff/asset.py` & `unitypackff-1.0.3/unitypackff/asset.py`

 * *Files identical despite different names*

### Comparing `unitypackff-1.0.2/unitypackff/assetbundle.py` & `unitypackff-1.0.3/unitypackff/assetbundle.py`

 * *Files identical despite different names*

### Comparing `unitypackff-1.0.2/unitypackff/classes.json` & `unitypackff-1.0.3/unitypackff/classes.json`

 * *Files identical despite different names*

### Comparing `unitypackff-1.0.2/unitypackff/engine/__init__.py` & `unitypackff-1.0.3/unitypackff/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `unitypackff-1.0.2/unitypackff/engine/animation.py` & `unitypackff-1.0.3/unitypackff/engine/animation.py`

 * *Files identical despite different names*

### Comparing `unitypackff-1.0.2/unitypackff/engine/audio.py` & `unitypackff-1.0.3/unitypackff/engine/audio.py`

 * *Files identical despite different names*

### Comparing `unitypackff-1.0.2/unitypackff/engine/mesh.py` & `unitypackff-1.0.3/unitypackff/engine/mesh.py`

 * *Files identical despite different names*

### Comparing `unitypackff-1.0.2/unitypackff/engine/object.py` & `unitypackff-1.0.3/unitypackff/engine/object.py`

 * *Files identical despite different names*

### Comparing `unitypackff-1.0.2/unitypackff/engine/particle.py` & `unitypackff-1.0.3/unitypackff/engine/particle.py`

 * *Files identical despite different names*

### Comparing `unitypackff-1.0.2/unitypackff/engine/physics.py` & `unitypackff-1.0.3/unitypackff/engine/physics.py`

 * *Files identical despite different names*

### Comparing `unitypackff-1.0.2/unitypackff/engine/renderer.py` & `unitypackff-1.0.3/unitypackff/engine/renderer.py`

 * *Files identical despite different names*

### Comparing `unitypackff-1.0.2/unitypackff/engine/text.py` & `unitypackff-1.0.3/unitypackff/engine/text.py`

 * *Files identical despite different names*

### Comparing `unitypackff-1.0.2/unitypackff/engine/texture.py` & `unitypackff-1.0.3/unitypackff/engine/texture.py`

 * *Files identical despite different names*

### Comparing `unitypackff-1.0.2/unitypackff/enums.py` & `unitypackff-1.0.3/unitypackff/enums.py`

 * *Files identical despite different names*

### Comparing `unitypackff-1.0.2/unitypackff/environment.py` & `unitypackff-1.0.3/unitypackff/environment.py`

 * *Files identical despite different names*

### Comparing `unitypackff-1.0.2/unitypackff/export.py` & `unitypackff-1.0.3/unitypackff/export.py`

 * *Files identical despite different names*

### Comparing `unitypackff-1.0.2/unitypackff/modding.py` & `unitypackff-1.0.3/unitypackff/modding.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from io import BytesIO
-from wand.image import Image
+#from wand.image import Image
+import wand
 
 from .utils import BinaryWriter
 from .object import FFOrderedDict
 from .engine.object import Object
 from .engine.mesh import SubMesh
 
 
@@ -21,15 +22,15 @@
 		obj.name = name
 
 
 def import_texture(obj, imgpath, name=None, fmt='dxt1'):
 	if not isinstance(obj, Object):
 		raise ValueError('Invalid target object')
 
-	img = Image(filename=imgpath)
+	img = wand.image.Image(filename=imgpath)
 
 	if name is not None:
 		obj.name = name
 	obj.height = img.height
 	obj.width = img.width
 	# DXT1 or DXT5
 	obj.format = 12 if fmt == 'dxt5' else 10
```

### Comparing `unitypackff-1.0.2/unitypackff/object.py` & `unitypackff-1.0.3/unitypackff/object.py`

 * *Files identical despite different names*

### Comparing `unitypackff-1.0.2/unitypackff/strings.dat` & `unitypackff-1.0.3/unitypackff/strings.dat`

 * *Files identical despite different names*

### Comparing `unitypackff-1.0.2/unitypackff/structs.dat` & `unitypackff-1.0.3/unitypackff/structs.dat`

 * *Files identical despite different names*

### Comparing `unitypackff-1.0.2/unitypackff/type.py` & `unitypackff-1.0.3/unitypackff/type.py`

 * *Files identical despite different names*

### Comparing `unitypackff-1.0.2/unitypackff/utils.py` & `unitypackff-1.0.3/unitypackff/utils.py`

 * *Files identical despite different names*

### Comparing `unitypackff-1.0.2/unitypackff.egg-info/PKG-INFO` & `unitypackff-1.0.3/unitypackff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitypackff
-Version: 1.0.2
+Version: 1.0.3
 Summary: UnityPackFF is a fork of UnityPack specialized for working with FusionFall assets
 Home-page: https://github.com/SirDank/UnityPackFF
 Download-URL: https://github.com/SirDank/UnityPackFF/tarball/master
 Author: dongresource
 License: MIT
 Project-URL: GitHub, https://github.com/SirDank/UnityPackFF
 Project-URL: Bug Tracker, https://github.com/SirDank/UnityPackFF/issues
```

### Comparing `unitypackff-1.0.2/unitypackff.egg-info/SOURCES.txt` & `unitypackff-1.0.3/unitypackff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

