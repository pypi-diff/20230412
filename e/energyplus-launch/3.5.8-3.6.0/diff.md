# Comparing `tmp/energyplus_launch-3.5.8.tar.gz` & `tmp/energyplus_launch-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energyplus_launch-3.5.8.tar", last modified: Tue Apr 11 17:59:25 2023, max compression
+gzip compressed data, was "energyplus_launch-3.6.0.tar", last modified: Wed Apr 12 19:34:58 2023, max compression
```

## Comparing `energyplus_launch-3.5.8.tar` & `energyplus_launch-3.6.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 17:59:25.845486 energyplus_launch-3.5.8/
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3197 2023-04-11 17:59:25.845486 energyplus_launch-3.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 17:59:25.841486 energyplus_launch-3.5.8/energyplus_launch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3197 2023-04-11 17:59:25.000000 energyplus_launch-3.5.8/energyplus_launch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1260 2023-04-11 17:59:25.000000 energyplus_launch-3.5.8/energyplus_launch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 17:59:25.000000 energyplus_launch-3.5.8/energyplus_launch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-04-11 17:59:25.000000 energyplus_launch-3.5.8/energyplus_launch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-11 17:59:25.000000 energyplus_launch-3.5.8/energyplus_launch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-11 17:59:25.000000 energyplus_launch-3.5.8/energyplus_launch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 17:59:25.841486 energyplus_launch-3.5.8/eplaunch/
--rw-r--r--   0 runner    (1001) docker     (122)      389 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      289 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/configure.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 17:59:25.845486 energyplus_launch-3.5.8/eplaunch/interface/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8727 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/interface/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     5989 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/interface/dialog_external_viewers.py
--rw-r--r--   0 runner    (1001) docker     (122)      772 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/interface/dialog_generic.py
--rw-r--r--   0 runner    (1001) docker     (122)     2489 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/interface/dialog_output.py
--rw-r--r--   0 runner    (1001) docker     (122)     6648 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/interface/dialog_weather.py
--rw-r--r--   0 runner    (1001) docker     (122)     4588 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/interface/dialog_workflow_dirs.py
--rw-r--r--   0 runner    (1001) docker     (122)    63951 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/interface/frame_main.py
--rw-r--r--   0 runner    (1001) docker     (122)     5813 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/interface/widget_dir_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     4808 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/interface/widget_file_list.py
--rw-r--r--   0 runner    (1001) docker     (122)      146 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/tk_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 17:59:25.845486 energyplus_launch-3.5.8/eplaunch/utilities/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10941 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/utilities/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)      641 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/utilities/crossplatform.py
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/utilities/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 17:59:25.845486 energyplus_launch-3.5.8/eplaunch/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4817 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/workflows/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 17:59:25.845486 energyplus_launch-3.5.8/eplaunch/workflows/default/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/workflows/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/workflows/default/file_details.py
--rw-r--r--   0 runner    (1001) docker     (122)     3266 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/workflows/default/idf_details.py
--rw-r--r--   0 runner    (1001) docker     (122)     2163 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/workflows/default/site_location.py
--rw-r--r--   0 runner    (1001) docker     (122)     9936 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/workflows/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/workflows/workflow.py
--rw-r--r--   0 runner    (1001) docker     (122)     5368 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/workflows/workflow_tester.py
--rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/workflows/workflow_thread.py
--rw-r--r--   0 runner    (1001) docker     (122)      216 2023-04-11 17:59:25.845486 energyplus_launch-3.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 19:34:58.345736 energyplus_launch-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3197 2023-04-12 19:34:58.345736 energyplus_launch-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 19:34:58.345736 energyplus_launch-3.6.0/energyplus_launch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3197 2023-04-12 19:34:58.000000 energyplus_launch-3.6.0/energyplus_launch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1260 2023-04-12 19:34:58.000000 energyplus_launch-3.6.0/energyplus_launch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 19:34:58.000000 energyplus_launch-3.6.0/energyplus_launch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-04-12 19:34:58.000000 energyplus_launch-3.6.0/energyplus_launch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-12 19:34:58.000000 energyplus_launch-3.6.0/energyplus_launch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-12 19:34:58.000000 energyplus_launch-3.6.0/energyplus_launch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 19:34:58.345736 energyplus_launch-3.6.0/eplaunch/
+-rw-r--r--   0 runner    (1001) docker     (122)      389 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/configure.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 19:34:58.345736 energyplus_launch-3.6.0/eplaunch/interface/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9400 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/interface/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5989 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/interface/dialog_external_viewers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      772 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/interface/dialog_generic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2489 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/interface/dialog_output.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4914 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/interface/dialog_weather.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4588 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/interface/dialog_workflow_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    68682 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/interface/frame_main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5813 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/interface/widget_dir_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5490 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/interface/widget_file_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)      146 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/tk_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 19:34:58.345736 energyplus_launch-3.6.0/eplaunch/utilities/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10941 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/utilities/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)      641 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/utilities/crossplatform.py
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/utilities/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 19:34:58.345736 energyplus_launch-3.6.0/eplaunch/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4817 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/workflows/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 19:34:58.345736 energyplus_launch-3.6.0/eplaunch/workflows/default/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/workflows/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/workflows/default/file_details.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3266 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/workflows/default/idf_details.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2163 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/workflows/default/site_location.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9936 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/workflows/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/workflows/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5368 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/workflows/workflow_tester.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/workflows/workflow_thread.py
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-04-12 19:34:58.345736 energyplus_launch-3.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/setup.py
```

### Comparing `energyplus_launch-3.5.8/LICENSE` & `energyplus_launch-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.5.8/PKG-INFO` & `energyplus_launch-3.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energyplus_launch
-Version: 3.5.8
+Version: 3.6.0
 Summary: Graphical Interface and Workflow Manager for EnergyPlus
 Home-page: https://github.com/NREL/EP-Launch
 Author: Jason Glazer and Edwin Lee for the United States Department of Energy
 License: ModifiedBSD
 Description: # EP-Launch3
         
         [![GitHub release](https://img.shields.io/github/release/nrel/ep-launch.svg?style=for-the-badge)](https://github.com/nrel/ep-launch/releases/latest)
```

### Comparing `energyplus_launch-3.5.8/README.md` & `energyplus_launch-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.5.8/energyplus_launch.egg-info/PKG-INFO` & `energyplus_launch-3.6.0/energyplus_launch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energyplus-launch
-Version: 3.5.8
+Version: 3.6.0
 Summary: Graphical Interface and Workflow Manager for EnergyPlus
 Home-page: https://github.com/NREL/EP-Launch
 Author: Jason Glazer and Edwin Lee for the United States Department of Energy
 License: ModifiedBSD
 Description: # EP-Launch3
         
         [![GitHub release](https://img.shields.io/github/release/nrel/ep-launch.svg?style=for-the-badge)](https://github.com/nrel/ep-launch/releases/latest)
```

### Comparing `energyplus_launch-3.5.8/energyplus_launch.egg-info/SOURCES.txt` & `energyplus_launch-3.6.0/energyplus_launch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.5.8/eplaunch/interface/config.py` & `energyplus_launch-3.6.0/eplaunch/interface/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,19 +21,21 @@
         self.width: int = -1
         self.x: int = -1
         self.y: int = -1
         self.workflow_directories: List[Path] = []
         self.folders_recent: deque[Optional[Path]] = deque(maxlen=5)
         self.folders_favorite: List[Path] = []
         self.weathers_recent: deque[Optional[Path]] = deque(maxlen=5)
-        self.weathers_favorite: List[Path] = []
+        # self.weathers_favorite: List[Path] = []
         self.group_locations: List[Path] = []
         # self.groups_recent: List[str] = []
         # self.groups_favorite: List[str] = []
         self.viewer_overrides: Dict[str, Path] = {}
+        self.dir_file_paned_window_sash_position: int = 400
+        self.list_group_paned_window_sash_position: int = 500
 
     def load(self):
         # load the config from the file on disk
         config_file_path = Path.home() / ConfigManager.config_file_name
         if not config_file_path.exists():
             pass  # just use the default values
         else:
@@ -100,23 +102,28 @@
                         for string_path in recent_folders:
                             self.folders_recent.appendleft(Path(string_path))
                     self.folders_favorite = [Path(p) for p in config.get('FavoriteFolders', self.folders_favorite)]
                     recent_weather = config.get('RecentWeather', self.weathers_recent)
                     if recent_weather is not None:
                         for string_path in recent_weather:
                             self.weathers_recent.appendleft(Path(string_path))
-                    self.weathers_favorite = [Path(p) for p in config.get('FavoriteWeather', self.weathers_favorite)]
+                    # self.weathers_favorite = [Path(p) for p in config.get('FavoriteWeather', self.weathers_favorite)]
                     # self.groups_recent = config.get('RecentGroup', self.groups_recent)
                     # self.groups_favorite = config.get('FavoriteGroup', self.groups_favorite)
                     temp_group_locations = config.get('GroupLocations', self.group_locations)
                     for t in temp_group_locations:
                         self.group_locations.append(Path(t))
                     for k, v in config.get('ViewerOverrides', self.viewer_overrides).items():
                         self.viewer_overrides[k] = Path(v) if v else None
-
+                    self.dir_file_paned_window_sash_position = config.get(
+                        'DirFilePanedWindowSash', self.dir_file_paned_window_sash_position
+                    )
+                    self.list_group_paned_window_sash_position = config.get(
+                        'ListGroupPanedWindowSash', self.list_group_paned_window_sash_position
+                    )
                 else:
                     pass  # Bad config saved file format?  Indicates a crash?
                 # fix up the current selected directory to initialize in case it doesn't exist (anymore)
                 if not self.directory:
                     self.directory = Path.home()
                 elif not self.directory.exists():
                     self.directory = Path.home()
@@ -135,15 +142,17 @@
             'width': self.width,
             'x': self.x,
             'y': self.y,
             'WorkflowDirectories': [str(p) for p in self.workflow_directories],
             'RecentFolders': [str(p) for p in self.folders_recent if p is not None],
             'FavoriteFolders': [str(p) for p in self.folders_favorite],
             'RecentWeather': [str(p) for p in self.weathers_recent if p is not None],
-            'FavoriteWeather': [str(p) for p in self.weathers_favorite],
+            # 'FavoriteWeather': [str(p) for p in self.weathers_favorite],
             # 'RecentGroup': self.groups_recent,
             # 'FavoriteGroup': self.groups_favorite,
             'GroupLocations': [str(t) for t in self.group_locations],
             'ViewerOverrides': {k: None if v is None else str(v) for k, v in self.viewer_overrides.items()},
+            'DirFilePanedWindowSash': self.dir_file_paned_window_sash_position,
+            'ListGroupPanedWindowSash': self.list_group_paned_window_sash_position,
         }
         config_file_path = Path.home() / ConfigManager.config_file_name
         config_file_path.write_text(dumps(output_dict, indent=2))
```

### Comparing `energyplus_launch-3.5.8/eplaunch/interface/dialog_external_viewers.py` & `energyplus_launch-3.6.0/eplaunch/interface/dialog_external_viewers.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.5.8/eplaunch/interface/dialog_generic.py` & `energyplus_launch-3.6.0/eplaunch/interface/dialog_generic.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.5.8/eplaunch/interface/dialog_output.py` & `energyplus_launch-3.6.0/eplaunch/interface/dialog_output.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.5.8/eplaunch/interface/dialog_workflow_dirs.py` & `energyplus_launch-3.6.0/eplaunch/interface/dialog_workflow_dirs.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.5.8/eplaunch/interface/frame_main.py` & `energyplus_launch-3.6.0/eplaunch/interface/frame_main.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 from json import dumps
 from mimetypes import guess_type
 from pathlib import Path
 from platform import system
 from queue import Queue
 
 from subprocess import Popen
-from tkinter import Tk, PhotoImage, StringVar, Menu, DISABLED, OptionMenu, Frame, Label, Button, NSEW, \
-    SUNKEN, S, LEFT, BOTH, messagebox, END, BooleanVar, ACTIVE, LabelFrame, RIGHT, EW, PanedWindow, NS, filedialog, ALL
-from tkinter.ttk import Combobox
+from tkinter import Tk, PhotoImage, StringVar, Menu, DISABLED, OptionMenu, Frame, Label, Button, NSEW, E, VERTICAL, \
+    SUNKEN, S, LEFT, BOTH, messagebox, END, BooleanVar, ACTIVE, LabelFrame, RIGHT, EW, NS, filedialog, \
+    ALL, Listbox, Scrollbar, SINGLE, Variable, HORIZONTAL
+from tkinter.ttk import Combobox, PanedWindow as ttkPanedWindow
 from typing import Dict, List, Optional, Tuple
 from uuid import uuid4
 from webbrowser import open as open_web
 from plan_tools.runtime import fixup_taskbar_icon_on_windows
 
 from eplaunch import VERSION, DOCS_URL, NAME
 from eplaunch.interface.dialog_generic import TkGenericDialog
@@ -113,14 +114,16 @@
 
         # finally set the initial directory and update the file listing
         self.dir_tree.dir_list.refresh_listing(self.conf.directory)
         self._update_file_list()
 
         # set the minimum size and redraw the app
         self.minsize(1050, 400)
+        self.dir_files_pw.sashpos(0, self.conf.dir_file_paned_window_sash_position)
+        self.list_group_pw.sashpos(0, self.conf.list_group_paned_window_sash_position)
         self.update()
 
         # one time update of the status bar
         self._update_status_bar("Program Initialized")
 
         # potentially show a welcome screen if we are on a new version
         self._open_welcome()
@@ -168,31 +171,29 @@
 
     def _build_top_menu(self):
         menubar = Menu(self)
 
         menu_file = Menu(menubar, tearoff=False)
         menu_file.add_command(label="Run Current Workflow on Selection", command=self._run_workflow_on_selection)
         menu_file.add_command(label="Run Current Workflow on Current Group", command=self._run_workflow_on_group)
-        menu_file.add_command(label="Quit", command=self.window_close)
+        menu_file.add_command(label="Quit", command=self._window_close)
         menubar.add_cascade(label="File", menu=menu_file)
 
         menu_nav = Menu(menubar, tearoff=False)
         self.menu_nav_recent = Menu(menu_nav, tearoff=False)
         menu_nav.add_cascade(label="Recent", menu=self.menu_nav_recent)
         menu_nav.add_command(label="Navigate to previous folder", command=self._navigate_to_previous_folder)
         menu_nav.add_separator()
         self.menu_nav_favorites = Menu(menu_nav, tearoff=False)
         menu_nav.add_cascade(label="Favorites", menu=self.menu_nav_favorites)
-        menu_nav.add_command(label="Add Current Folder to Favorites", command=self.add_folder_to_favorites)
-        menu_nav.add_command(label="Remove Current Folder from Favorites", command=self.remove_folder_from_favorites)
+        menu_nav.add_command(label="Add Current Folder to Favorites", command=self._add_folder_to_favorites)
+        menu_nav.add_command(label="Remove Current Folder from Favorites", command=self._remove_folder_from_favorites)
         menubar.add_cascade(label="Navigation", menu=menu_nav)
 
         menu_group = Menu(menubar, tearoff=False)
-        self.menu_group_current = Menu(menu_group, tearoff=False)
-        menu_group.add_cascade(label="Current Group", menu=self.menu_group_current)
         menu_group.add_command(label="Clear Current Group", command=self._clear_group)
         menu_group.add_command(label="Load new Group file...", command=self._load_new_group_file)
         menu_group.add_command(label="Save Current Group to file...", command=self._save_group_file)
         menu_group.add_command(
             label="Add selected files to current group", command=self._add_current_files_to_group
         )
         menu_group.add_command(
@@ -224,47 +225,44 @@
         menubar.add_cascade(label="Help", menu=menu_help)
 
         self.config(menu=menubar)
 
     # noinspection SqlNoDataSourceInspection
     def _build_top_icon_bar(self, container: Frame):
         lf = LabelFrame(container, text="Workflow Selection")
-        Label(lf, text="Context:", justify=RIGHT).grid(row=0, column=0, **self.pad)
+        Label(lf, text="Context:", justify=RIGHT).grid(row=0, column=0, sticky=E, **self.pad)
         self.option_workflow_context = OptionMenu(lf, self._tk_var_workflow_context, '<context>')
         self.option_workflow_context.grid(row=0, column=1, sticky=EW, **self.pad)
-        Label(lf, text="Workflow: ", justify=RIGHT).grid(row=1, column=0, **self.pad)
+        Label(lf, text="Workflow:", justify=RIGHT).grid(row=1, column=0, sticky=E, **self.pad)
         self.option_workflow_instance = OptionMenu(lf, self._tk_var_workflow_instance, '<instance>')
         self.option_workflow_instance.grid(row=1, column=1, sticky=EW, **self.pad)
         lf.grid(row=0, column=0, sticky=NS, **self.pad)
 
-        lf = LabelFrame(container, text="Workflow Execution")
+        lf = LabelFrame(container, text="Run Workflow on...")
         Button(
-            lf, text=u"\U000025B6 Run Workflow on Current File(s)", command=self._run_workflow_on_selection
+            lf, text=u"\U000025B6 Selected File(s)", command=self._run_workflow_on_selection
         ).grid(row=0, column=0, sticky=EW, **self.pad)
         Button(
-            lf, text=u"\U000025B6 Run Workflow on Current Group", command=self._run_workflow_on_group
+            lf, text=u"\U000025B6 Current Group", command=self._run_workflow_on_group
         ).grid(row=1, column=0, sticky=EW, **self.pad)
         lf.grid(row=0, column=1, sticky=NS, **self.pad)
 
         lf = LabelFrame(container, text="Weather Selection")
         Label(lf, text="Recent: ", justify=RIGHT).grid(row=0, column=0, **self.pad)
-        self.option_weather_recent = Combobox(lf, textvariable=self._tk_var_weather_recent)
-        self.option_weather_recent.grid(row=0, column=1, **self.pad)
-        self.option_weather_recent['state'] = 'readonly'
-        self.button_weather_set = Button(lf, text=u"\U00002713 Set", command=self._set_weather_from_recent)
-        self.button_weather_set.grid(row=0, column=2, **self.pad)
+        self.option_weather_recent = OptionMenu(lf, self._tk_var_weather_recent, '<weather>')
+        self.option_weather_recent.grid(row=0, column=1, sticky=EW, **self.pad)
         self.button_weather_select = Button(
-            lf, text=u"\U0001f325 Select Weather From Disk...", command=self._open_weather_dialog
+            lf, text=u"\U0001f325 Select Weather File...", command=self._open_weather_dialog
         )
-        self.button_weather_select.grid(row=1, column=0, columnspan=3, sticky=EW, **self.pad)
+        self.button_weather_select.grid(row=1, column=0, columnspan=2, sticky=EW, **self.pad)
         lf.grid(row=0, column=2, sticky=NS, **self.pad)
 
         lf = LabelFrame(container, text="Quicklinks")
         self.button_open_in_text = Button(
-            lf, text=u"\U0001F5B9 Open Selected File in Text Editor", command=self._open_text_editor, state=DISABLED
+            lf, text=u"\U0001F5B9 Open File in Text Editor", command=self._open_text_editor, state=DISABLED
         )
         self.button_open_in_text.grid(row=0, column=0, columnspan=3, sticky=EW, **self.pad)
         Button(
             lf, text=u"\U0001F5C0 Open Dir in File Browser", command=self._open_file_browser
         ).grid(row=1, column=0, columnspan=3, sticky=EW, **self.pad)
         lf.grid(row=0, column=3, sticky=NS, **self.pad)
 
@@ -300,20 +298,43 @@
         self.button_open_output_file = Button(lf, text=u"\U0001f325 Open", command=self._open_output_file)
         self.button_open_output_file.grid(row=1, column=2, **self.pad)
         lf.grid_columnconfigure(ALL, weight=1)
         lf.grid_rowconfigure(ALL, weight=1)
         lf.grid(row=0, column=4, sticky=NS, **self.pad)
 
     def _build_listings(self, container: Frame):
-        pw = PanedWindow(container)  # default horizontal
-        self.dir_tree = DirListScrollableFrame(pw, on_select=self._new_dir_selected, on_root_changed=self._new_root_dir)
-        pw.add(self.dir_tree)
-        self.file_list = FileListScrollableFrame(container, on_selection_changed=self._callback_file_selection_changed)
-        pw.add(self.file_list)
-        pw.pack(fill=BOTH, expand=True, **self.pad)
+        # use vertical for the primary paned window
+        self.list_group_pw = ttkPanedWindow(container, orient=VERTICAL)
+        # create a sub paned window that is vertical to split the directory from the group box
+        self.dir_files_pw = ttkPanedWindow(container, orient=HORIZONTAL)
+        # the top part of this pane is simply the directory tree, add it with a heavier weight
+        self.dir_tree = DirListScrollableFrame(
+            self.dir_files_pw, on_select=self._new_dir_selected, on_root_changed=self._new_root_dir
+        )
+        self.dir_files_pw.add(self.dir_tree, weight=1)
+        self.file_list = FileListScrollableFrame(
+            self.dir_files_pw, on_selection_changed=self._callback_file_selection_changed
+        )
+        self.dir_files_pw.add(self.file_list, weight=1)
+        self.list_group_pw.add(self.dir_files_pw, weight=10)
+        # the bottom part of the primary pane will be a label frame containing a group listbox, add it with lower weight
+        group_label_frame = LabelFrame(self.list_group_pw, text="Current Group")
+        self.group_list_box = Listbox(group_label_frame, height=5, selectmode=SINGLE)
+        self.group_list_box.bind('<Double-1>', self._handle_group_selection_from_widget)
+        from string import ascii_uppercase
+        for i, e in enumerate(ascii_uppercase):
+            self.group_list_box.insert(i + 1, e)
+        self.group_list_box.pack(side=LEFT, fill=BOTH, expand=True)
+        scroll = Scrollbar(group_label_frame)
+        scroll.pack(side=RIGHT, fill=BOTH)
+        self.group_list_box.config(yscrollcommand=scroll.set)
+        scroll.config(command=self.group_list_box.yview)
+        self.list_group_pw.add(group_label_frame, weight=1)
+        # add the left paned window to the primary panes
+        self.list_group_pw.pack(fill=BOTH, expand=True, **self.pad)
 
     def _build_status_bar(self, container: Frame):
         Label(container, relief=SUNKEN, anchor=S, textvariable=self._tk_var_status_dir).pack(
             side=LEFT, fill=BOTH, expand=True
         )
         Label(container, relief=SUNKEN, anchor=S, textvariable=self._tk_var_status_workflow).pack(
             side=LEFT, fill=BOTH, expand=True
@@ -335,18 +356,18 @@
 
     # endregion
 
     # region main window run/close/update functions
 
     def run(self):
         """Main entry point to register a close handler and execute the app main loop"""
-        self.protocol('WM_DELETE_WINDOW', self.window_close)
+        self.protocol('WM_DELETE_WINDOW', self._window_close)
         self.mainloop()
 
-    def window_close(self, *_):
+    def _window_close(self, *_):
         # block for running threads
         if len(self.workflow_manager.threads) > 0:
             msg = 'Program closing, but there are threads running; would you like to kill the threads and close?'
             if messagebox.askyesno(msg):
                 for thread_id in self.workflow_manager.threads:
                     try:
                         self.workflow_manager.threads[thread_id].abort()
@@ -360,14 +381,16 @@
         for dialog_id in keys:
             self.output_dialogs[dialog_id].close()
         # save the configuration and close
         self.conf.x = self.winfo_x()
         self.conf.y = self.winfo_y()
         self.conf.width = self.winfo_width()
         self.conf.height = self.winfo_height()
+        self.conf.dir_file_paned_window_sash_position = self.dir_files_pw.sashpos(0)
+        self.conf.list_group_paned_window_sash_position = self.list_group_pw.sashpos(0)
         self.conf.save()
         self.destroy()
 
     def _update_status_bar(self, message: str) -> None:
         """Updates all the status bar entries for current status and status by setting tk variables"""
         if self.conf.directory:
             self._tk_var_status_dir.set(str(self.conf.directory))
@@ -464,29 +487,40 @@
             messagebox.showwarning("Warning", "At least one file path was not in the current group and was skipped")
         self._rebuild_group_menu()
 
     def _cycle_through_group(self):
         if len(self.conf.group_locations) == 0:
             messagebox.showwarning("Invalid Group Cycle", "Could not cycle through empty group list")
             return
+        self.group_list_box.selection_clear(0, END)
+        self.group_list_box.selection_set(self.group_cycle_next_index)
         self._handle_group_selection(self.group_cycle_next_index)
         self.group_cycle_next_index += 1
         if self.group_cycle_next_index + 1 > len(self.conf.group_locations):
             self.group_cycle_next_index = 0
 
     def _rebuild_group_menu(self):
         self.group_cycle_next_index = 0
-        self.menu_group_current.delete(0, END)
+        self.group_list_box.delete(0, END)
         for index, entry in enumerate(self.conf.group_locations):
-            self.menu_group_current.add_command(
-                label=str(entry), command=lambda i=index: self._handle_group_selection(i)
-            )
+            self.group_list_box.insert(index, str(entry))
 
-    def _handle_group_selection(self, index: int):
-        entry = self.conf.group_locations[index]
+    def _handle_group_selection_from_widget(self, *_):
+        self._handle_group_selection()
+
+    def _handle_group_selection(self, specific_index: Optional[int] = None):
+        if isinstance(specific_index, int):
+            idx = specific_index
+        else:
+            idx = self.group_list_box.curselection()[0]
+        try:
+            entry = self.conf.group_locations[idx]
+        except IndexError:
+            messagebox.showerror("Error", f"Could not navigate to group entry at index {idx}")
+            return
         if not entry.exists():
             messagebox.showerror("Error", f"Could not navigate to group entry, it doesn't exist: {entry}")
             return
         self.conf.directory = entry.parent
         self.dir_tree.dir_list.refresh_listing(self.conf.directory)
         self._update_file_list()
         self.file_list.tree.try_to_reselect([entry.name])
@@ -505,22 +539,22 @@
         if self.workflow_manager.current_workflow:
             if self.workflow_manager.current_workflow.uses_weather:
                 column_list.append("Weather")
             column_list.extend(self.workflow_manager.current_workflow.columns)
         # ask the file listing widget to update columns
         self.file_list.tree.set_new_columns(column_list)
 
-    def add_folder_to_favorites(self):
+    def _add_folder_to_favorites(self):
         if self.conf.directory in self.conf.folders_favorite:
             messagebox.showwarning("Favorite Selection", "Folder already exists in favorites, skipping")
             return
         self.conf.folders_favorite.append(self.conf.directory)
         self._rebuild_favorite_folder_menu()
 
-    def remove_folder_from_favorites(self):
+    def _remove_folder_from_favorites(self):
         if self.conf.directory not in self.conf.folders_favorite:
             messagebox.showwarning("Favorite Selection", "Folder is not in favorites, skipping")
             return
         self.conf.folders_favorite.remove(self.conf.directory)
         self._rebuild_favorite_folder_menu()
 
     def _rebuild_favorite_folder_menu(self):
@@ -693,61 +727,52 @@
         return False
 
     def _callback_file_selection_changed(self, selected_file_names: List[str]) -> None:
         """This gets called back by the file listing widget when a selection changes"""
         self.conf.file_selection = selected_file_names
         status = ACTIVE if len(self.conf.file_selection) > 0 else DISABLED
         self.button_open_in_text['state'] = status
+        self._refresh_output_suffix_buttons_based_on_selection()
 
     # endregion
 
     # region weather operations
 
-    def set_weather_widget_state(self, weather_enabled) -> None:
+    def _set_weather_widget_state(self, weather_enabled) -> None:
         self.option_weather_recent.configure(state=weather_enabled)
         self.button_weather_select.configure(state=weather_enabled)
-        self.button_weather_set.configure(state=weather_enabled)
 
     def _repopulate_recent_weather_list(self, try_to_select: Optional[Path] = None):
-        recent_weather = self.conf.weathers_recent
-        combobox_weather_enabled = 'readonly' if len(recent_weather) > 0 else 'disabled'
-        button_weather_enabled = ACTIVE if len(recent_weather) > 0 else DISABLED
-        self.option_weather_recent.configure(state=combobox_weather_enabled)
-        self.button_weather_set.configure(state=button_weather_enabled)
-
-        if button_weather_enabled == ACTIVE:
-            if try_to_select:
-                desired_weather_path = str(try_to_select)
-            else:
-                desired_weather_path = str(self.conf.weathers_recent[self.option_weather_recent.current()])
-            self.option_weather_recent['values'] = [x.name for x in recent_weather]
-            self.option_weather_recent.current(0)
-            for i, r in enumerate(recent_weather):
-                if str(r) == desired_weather_path:
-                    self.option_weather_recent.current(i)
-                    break
+        self.option_weather_recent['menu'].delete(0, END)
+        for x in self.conf.weathers_recent:
+            weather_path = x
+            self.option_weather_recent['menu'].add_command(
+                label=weather_path.name,
+                command=lambda w=weather_path: self._handler_weather_recent_option_changed(w)
+            )
+        if try_to_select in self.conf.weathers_recent:
+            self._handler_weather_recent_option_changed(try_to_select)
         else:
-            self.option_weather_recent['values'] = []
+            self._handler_weather_recent_option_changed(self.conf.weathers_recent[0])  # could persist in self.conf
 
-    def _set_weather_from_recent(self) -> None:
-        current_index = self.option_weather_recent.current()
-        selected_recent_weather_string = str(self.conf.weathers_recent[current_index])
+    def _handler_weather_recent_option_changed(self, new_weather_path: Path):
+        """This is called when the recent weather option menu changes value"""
+        self._tk_var_weather_recent.set(str(new_weather_path.name))
+        selected_recent_weather_string = self._tk_var_weather_recent.get()
         for selected_file_name in self.conf.file_selection:
             cache = CacheFile(self.conf.directory)
             cache.add_config(
                 self.workflow_manager.current_workflow.name,
                 selected_file_name,
                 {'weather': selected_recent_weather_string}
             )
         self._update_file_list()
 
     def _open_weather_dialog(self) -> None:
-        dialog_weather = TkWeatherDialog(
-            self, list(self.conf.weathers_recent), self.conf.weathers_favorite
-        )
+        dialog_weather = TkWeatherDialog(self, list(self.conf.weathers_recent))
         self.wait_window(dialog_weather)
         if dialog_weather.exit_code == TkWeatherDialog.CLOSE_SIGNAL_CANCEL:
             return
         if not dialog_weather.selected_weather_file:
             weather_file_to_use = self.dd_only_string
         else:
             weather_file_to_use = dialog_weather.selected_weather_file
@@ -800,24 +825,30 @@
         desired_selected_workflow_name = self.conf.cur_workflow_name
         # get all known workflows for the current context
         self.available_workflows = self.workflow_manager.workflow_instances(self.conf.cur_workflow_context)
         # clear the option menu entirely
         self.option_workflow_instance['menu'].delete(0, END)
         # add in all the instances, registering a lambda that will set the tk var and refresh the file list as needed
         just_names = []
+        energyplus_ip_workflow_name = None
         for w in self.available_workflows:
             workflow_name = w.name
+            workflow_name_upper = workflow_name.upper()
+            if 'ENERGYPLUS' in workflow_name_upper and 'IP' in workflow_name_upper:
+                energyplus_ip_workflow_name = workflow_name
             just_names.append(workflow_name)
             self.option_workflow_instance['menu'].add_command(
                 label=workflow_name,
                 command=lambda n=workflow_name: self._handler_workflow_instance_option_changed(n)
             )
-        # call the handler method with either the saved instance name, or the top one in the list
+        # call the handler method with either the saved instance name, or an E+ one, or the top one in the list
         if desired_selected_workflow_name in just_names:
             self._handler_workflow_instance_option_changed(desired_selected_workflow_name)
+        elif energyplus_ip_workflow_name:
+            self._handler_workflow_instance_option_changed(energyplus_ip_workflow_name)
         else:
             self._handler_workflow_instance_option_changed(just_names[0])
 
     def _handler_workflow_instance_option_changed(self, new_value: str):
         """This is called when the workflow instance option menu changes value"""
         # store the new instance name in the tk var and in the config
         self._tk_var_workflow_instance.set(new_value)
@@ -829,24 +860,23 @@
                 new_workflow = w
                 break
         if new_workflow is None:
             messagebox.showerror("There was an unexpected error updating the workflow list, suggest restarting app.")
         # assign the current workflow instance in the workflow manager
         self.workflow_manager.current_workflow = new_workflow
         # update the weather buttons accordingly depending on if the workflow uses weather inputs
-        self.set_weather_widget_state(ACTIVE if new_workflow.uses_weather else DISABLED)
+        self._set_weather_widget_state(ACTIVE if new_workflow.uses_weather else DISABLED)
         # clear the output menu entirely, and set status conditionally
         self._repopulate_output_suffix_options()
         # now that the workflow has been set, repopulate the file list columns and the file list itself
         self._repopulate_control_list_columns()
         self._update_file_list()
 
     def _repopulate_output_suffix_options(self):
-        suffixes = self.workflow_manager.current_workflow.output_suffixes
-        sorted_suffixes = sorted(suffixes)
+        sorted_suffixes = sorted(self.workflow_manager.current_workflow.output_suffixes)
         combobox_output_enabled = 'readonly' if len(sorted_suffixes) > 0 else 'disabled'
         output_enabled = ACTIVE if len(sorted_suffixes) > 0 else DISABLED
         self.option_workflow_outputs.configure(state=combobox_output_enabled)
         self.button_open_output_file.configure(state=output_enabled)
 
         # rebuild the option menu if applicable
         current_selection = self._tk_var_output_suffix.get()
@@ -854,26 +884,58 @@
             self.option_workflow_outputs['values'] = sorted_suffixes
             if current_selection not in sorted_suffixes:
                 self._tk_var_output_suffix.set(sorted_suffixes[0])
         else:
             self.option_workflow_outputs['values'] = []
             self._tk_var_output_suffix.set('')
         self.option_workflow_outputs.selection_clear()
-
-        # update the output file buttons too
+        suffixes = self.workflow_manager.current_workflow.output_suffixes
         self.button_open_output_1.configure(state=ACTIVE if len(suffixes) > 0 else DISABLED)
         self._tk_var_output_1.set(suffixes[0] if len(suffixes) > 0 else '--')
         self.button_open_output_2.configure(state=ACTIVE if len(suffixes) > 1 else DISABLED)
         self._tk_var_output_2.set(suffixes[1] if len(suffixes) > 1 else '--')
         self.button_open_output_3.configure(state=ACTIVE if len(suffixes) > 2 else DISABLED)
         self._tk_var_output_3.set(suffixes[2] if len(suffixes) > 2 else '--')
         self.button_open_output_4.configure(state=ACTIVE if len(suffixes) > 3 else DISABLED)
         self._tk_var_output_4.set(suffixes[3] if len(suffixes) > 3 else '--')
         self.button_open_output_5.configure(state=ACTIVE if len(suffixes) > 4 else DISABLED)
         self._tk_var_output_5.set(suffixes[4] if len(suffixes) > 4 else '--')
+        self._refresh_output_suffix_buttons_based_on_selection()
+
+    def suffixed_paths_exist(self, original_path: Path, new_suffix: str) -> Tuple[Optional[Path], Optional[Path]]:
+        filename_no_ext = original_path.with_suffix('').name
+        new_path = self.conf.directory / (filename_no_ext + new_suffix)
+        eplus_sub_dir = f"EPLaunchRun_{filename_no_ext}"
+        eplus_specific_output_path = self.conf.directory / eplus_sub_dir / f"{filename_no_ext}{new_suffix}"
+        primary_path_to_return = new_path if new_path.exists() else None
+        eplus_path_to_return = eplus_specific_output_path if eplus_specific_output_path.exists() else None
+        return primary_path_to_return, eplus_path_to_return
+
+    def _refresh_single_output_suffix_button(self, tk_var: Variable, button: Button):
+        if tk_var.get() == '--':
+            return
+        else:
+            suffix_to_open = tk_var.get()
+            all_files_have_this_suffix = True
+            for f in self.conf.file_selection:
+                original_path = self.conf.directory / f
+                new_path, eplus_path = self.suffixed_paths_exist(original_path, suffix_to_open)
+                if (new_path and new_path.exists()) or (eplus_path and eplus_path.exists()):
+                    pass  # good
+                else:
+                    all_files_have_this_suffix = False
+                    break
+            button.configure(state=ACTIVE if all_files_have_this_suffix else DISABLED)
+
+    def _refresh_output_suffix_buttons_based_on_selection(self):
+        self._refresh_single_output_suffix_button(self._tk_var_output_1, self.button_open_output_1)
+        self._refresh_single_output_suffix_button(self._tk_var_output_2, self.button_open_output_2)
+        self._refresh_single_output_suffix_button(self._tk_var_output_3, self.button_open_output_3)
+        self._refresh_single_output_suffix_button(self._tk_var_output_4, self.button_open_output_4)
+        self._refresh_single_output_suffix_button(self._tk_var_output_5, self.button_open_output_5)
 
     def _open_workflow_dir_dialog(self):
         if len(self.workflow_manager.threads) > 0:
             messagebox.showerror("Workflow Selection Error", 'Cannot change workflows while threads are running')
             return  # will leave the window open
         # refresh the list of workflows auto-found on the machine
         self.workflow_manager.auto_find_workflow_directories()
@@ -890,20 +952,20 @@
             self.generic_dialogs.display(
                 self, 'Workflow Processing Errors', '\n'.join(self.workflow_manager.warnings)
             )
         self.conf.workflow_directories = self.workflow_manager.workflow_directories
         self._repopulate_workflow_context_menu()
         self._repopulate_workflow_instance_menu()
 
-    def get_or_set_weather_for_file(self,
-                                    cur_workflow: Optional[BaseEPLaunchWorkflow1],
-                                    directory: Path,
-                                    selected_file: str,
-                                    backup_weather_file_to_use: str,
-                                    ) -> Tuple[bool, str, str]:
+    def _get_or_set_weather_for_file(self,
+                                     cur_workflow: Optional[BaseEPLaunchWorkflow1],
+                                     directory: Path,
+                                     selected_file: str,
+                                     backup_weather_file_to_use: str,
+                                     ) -> Tuple[bool, str, str]:
         """
         cur_workflow is "None" at init time, so it is marked technically optional
         """
         weather_file_to_use: Optional[str] = None
         # if we find this file in the current folder cache
         cache = CacheFile(directory)
         files_in_current_workflow = cache.get_files_for_workflow(cur_workflow.name)
@@ -918,18 +980,16 @@
             # since we could be asking for many files, we don't want to ask for each
             # get a backup file to use only once, and apply that to any missing ones as needed
             if backup_weather_file_to_use:
                 weather_file_to_use = backup_weather_file_to_use
             else:
                 # if we need weather, didn't find one in the cache, and didn't have a backup, ask for one now
                 recent_files = list(self.conf.weathers_recent)
-                favorite_files = self.conf.weathers_favorite
-                w = TkWeatherDialog(
-                    self, recent_files, favorite_files, "*At least one file is missing a weather configuration*"
-                )
+                # favorite_files = self.conf.weathers_favorite
+                w = TkWeatherDialog(self, recent_files, "*At least one file is missing a weather configuration*")
                 self.wait_window(w)
                 if w.exit_code == TkWeatherDialog.CLOSE_SIGNAL_CANCEL:
                     return False, '', ''
                 else:  # a valid response was encountered
                     if not w.selected_weather_file:
                         weather_file_to_use = self.dd_only_string
                     else:
@@ -966,15 +1026,15 @@
         backup_weather_file_to_use: Optional[str] = None
 
         # loop over all the selected files and try to run the current workflow on each of them
         for path in file_paths:
             # if the current workflow uses weather, we need to determine what to pass into it
             weather_file_to_use: Optional[str] = None
             if cur_workflow.uses_weather:
-                success, weather_file_to_use, backup_weather_file_to_use = self.get_or_set_weather_for_file(
+                success, weather_file_to_use, backup_weather_file_to_use = self._get_or_set_weather_for_file(
                     cur_workflow, path.parent, path.name, backup_weather_file_to_use
                 )
                 if not success:
                     return  # TODO: probably shouldn't just return blindly here
             this_wea = '' if weather_file_to_use == self.dd_only_string else weather_file_to_use
 
             # now we actually need to run this current file
@@ -1159,17 +1219,17 @@
 OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE,
 EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         """ % VERSION
         self.generic_dialogs.display(self, "About EP-Launch", text)
 
     def _open_output_file_generic(self, suffix_to_open: str):
-        if len(self.conf.file_selection) > 2:
-            message = """More than 2 files were selected when choosing to open workflow outputs.
-        This could generate many output windows and is usually not intentional.  Select up to 2 input files."""
+        if len(self.conf.file_selection) > 5:
+            message = """More than 5 files were selected when choosing to open workflow outputs.
+        This could generate many output windows and is usually not intentional.  Select up to 5 input files."""
             messagebox.showerror("File Selection Issue", message)
             return
         for f in self.conf.file_selection:
             original_path = self.conf.directory / f
             filename_no_ext = original_path.with_suffix('').name
             new_path = self.conf.directory / (filename_no_ext + suffix_to_open)
             new_path_str = str(new_path)
@@ -1211,28 +1271,40 @@
     def _open_output_4(self):
         self._open_output_file_generic(self._tk_var_output_4.get())
 
     def _open_output_5(self):
         self._open_output_file_generic(self._tk_var_output_5.get())
 
     @staticmethod
-    def _open_file_or_dir_with_default(full_path_obj: Path) -> None:
+    def _open_file_or_dir_with_default(full_path_obj: Path, text_file_override: bool = False) -> None:
         full_path = str(full_path_obj)
         if system() == 'Windows':
             from os import startfile
             startfile(full_path)
         elif system() == 'Linux':
             Popen(['xdg-open', full_path])
+            # could try to find the default text/plain editor and open using gtk-launch
+            # if text_file_override:
+            #     desktop_file = check_output(['xdg-mime', 'query', 'default', 'text/plain'], shell=False)
+            #     if '.desktop' in desktop_file.decode('utf-8'):
+            #         Popen(['gtk-launch', desktop_file, full_path])
+            #     else:  # try falling back to the default application
+            #         Popen(['xdg-open', full_path])
+            # else:
+            #     Popen(['xdg-open', full_path])
         else:  # assuming Mac
-            Popen(['open', full_path])
+            if text_file_override:  # will open in the default text editor specifically
+                Popen(['open', '-t', full_path])
+            else:
+                Popen(['open', full_path])
 
     def _open_text_editor(self) -> None:
         for file_name in self.conf.file_selection:
             full_path_str = self.conf.directory / file_name
-            if 'txt' in self.conf.viewer_overrides:
+            if 'txt' in self.conf.viewer_overrides and self.conf.viewer_overrides['txt']:
                 text_editor_binary = str(self.conf.viewer_overrides['txt'])
                 Popen([text_editor_binary, full_path_str])
             else:
                 self._open_file_or_dir_with_default(full_path_str)
 
     def _open_file_browser(self) -> None:
         self._open_file_or_dir_with_default(self.conf.directory)
```

### Comparing `energyplus_launch-3.5.8/eplaunch/interface/widget_dir_list.py` & `energyplus_launch-3.6.0/eplaunch/interface/widget_dir_list.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.5.8/eplaunch/interface/widget_file_list.py` & `energyplus_launch-3.6.0/eplaunch/interface/widget_file_list.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,26 +3,29 @@
 from tkinter.ttk import Treeview, Scrollbar
 from tkinter.messagebox import showinfo
 from typing import Tuple, Optional, Callable, List
 
 
 class FileListWidget(Treeview):
 
-    def __init__(self, parent_frame: Frame, on_selection_changed: Optional[Callable[[List[str]], None]] = None):
+    def __init__(self, parent_frame: Frame, on_selection_changed: Optional[Callable[[List[str]], None]] = None,
+                 on_double_click: Optional[Callable[[str], None]] = None):
         super().__init__(parent_frame, columns=['File Name'], show='headings', selectmode=EXTENDED)
         # disable callbacks while widget is initializing
         self.callback_on_selection_changed = None
+        self.callback_on_double_click = None
         self.columns = ['File Name']
         # define headings
         for c in self.columns:
             self.heading(c, text=c)
         self.file_ids: List[str] = []
         self.bind('<<TreeviewSelect>>', self._selection_changed)
         self.bind('<Double-1>', self._item_double_clicked)
         self.callback_on_selection_changed = on_selection_changed
+        self.callback_on_double_click = on_double_click
 
     def set_files(self, file_list: List[Tuple]):
         for file_id in self.file_ids:
             self.delete(file_id)
         self.file_ids.clear()
         for file_data in file_list:
             self.file_ids.append(self.insert('', END, values=file_data))
@@ -34,18 +37,20 @@
         for selected_id in self.selection():
             item_contents = self.item(selected_id)
             file_name = item_contents['values'][0]
             response.append(file_name)
         self.callback_on_selection_changed(response)
 
     def _item_double_clicked(self, _):
-        for selected_item in self.selection():
-            item = self.item(selected_item)
-            record = [str(x) for x in item['values']]
-            showinfo(title='Information', message=','.join(record))
+        if not self.callback_on_selection_changed:
+            return
+        selected_item = self.selection()[0]
+        item = self.item(selected_item)
+        record = [str(x) for x in item['values']]
+        showinfo(title='Information', message=','.join(record))
 
     def try_to_reselect(self, files_to_reselect: List[str]):
         # don't call back during programmatic selection
         hold_callback = self.callback_on_selection_changed
         self.callback_on_selection_changed = None
         for item in self.selection():
             self.selection_remove(item)
@@ -63,17 +68,23 @@
     def set_new_columns(self, extended_column_names=None) -> None:
         # we always leave Filename, the list should include Stale, Weather, etc.
         if extended_column_names is None:
             extended_column_names = list()
         column_list = ['File Name']
         column_list.extend(extended_column_names)
         self["columns"] = column_list
+        num_cols = len(column_list)
+        widget_width = max(self.winfo_width(), 400)
+        desired_first_column_portion = 1.093 - 0.195 * num_cols + 0.0116667 * num_cols * num_cols
+        first_column_width = int(desired_first_column_portion * widget_width)
+        remaining_width = widget_width - first_column_width
+        remaining_column_widths = remaining_width // (len(column_list) - 1)
         for i, c in enumerate(column_list):
-            # self.column(i, anchor='c')
             self.heading(i, text=c)
+            self.column(i, width=first_column_width if i == 0 else remaining_column_widths)
 
 
 class FileListScrollableFrame(Frame):
     def __init__(self, parent, on_selection_changed: Optional[Callable[[List[str]], None]] = None):
         super().__init__(parent)
         self.tree = FileListWidget(self, on_selection_changed)
         self.tree.grid(row=0, column=0, sticky=NSEW)
@@ -104,14 +115,15 @@
         file_listing.tree.set_new_columns()
     elif counter == 5:
         file_listing.tree.set_new_columns(['edwin', 'lee'])
 
 
 if __name__ == "__main__":
     from tkinter import Button, Tk
+
     root = Tk()
     root.title('File Listing Widget Demo')
 
     file_listing = FileListScrollableFrame(root, printer)
     files = []
     for n in range(1, 100):
         rand = randint(1, 10)
```

### Comparing `energyplus_launch-3.5.8/eplaunch/utilities/cache.py` & `energyplus_launch-3.6.0/eplaunch/utilities/cache.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.5.8/eplaunch/utilities/crossplatform.py` & `energyplus_launch-3.6.0/eplaunch/utilities/crossplatform.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.5.8/eplaunch/utilities/version.py` & `energyplus_launch-3.6.0/eplaunch/utilities/version.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.5.8/eplaunch/workflows/base.py` & `energyplus_launch-3.6.0/eplaunch/workflows/base.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.5.8/eplaunch/workflows/default/file_details.py` & `energyplus_launch-3.6.0/eplaunch/workflows/default/file_details.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.5.8/eplaunch/workflows/default/idf_details.py` & `energyplus_launch-3.6.0/eplaunch/workflows/default/idf_details.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.5.8/eplaunch/workflows/default/site_location.py` & `energyplus_launch-3.6.0/eplaunch/workflows/default/site_location.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.5.8/eplaunch/workflows/manager.py` & `energyplus_launch-3.6.0/eplaunch/workflows/manager.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.5.8/eplaunch/workflows/workflow.py` & `energyplus_launch-3.6.0/eplaunch/workflows/workflow.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.5.8/eplaunch/workflows/workflow_tester.py` & `energyplus_launch-3.6.0/eplaunch/workflows/workflow_tester.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.5.8/eplaunch/workflows/workflow_thread.py` & `energyplus_launch-3.6.0/eplaunch/workflows/workflow_thread.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.5.8/setup.py` & `energyplus_launch-3.6.0/setup.py`

 * *Files identical despite different names*

