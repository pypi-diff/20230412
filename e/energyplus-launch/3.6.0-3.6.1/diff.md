# Comparing `tmp/energyplus_launch-3.6.0.tar.gz` & `tmp/energyplus_launch-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energyplus_launch-3.6.0.tar", last modified: Wed Apr 12 19:34:58 2023, max compression
+gzip compressed data, was "energyplus_launch-3.6.1.tar", last modified: Wed Apr 12 20:31:45 2023, max compression
```

## Comparing `energyplus_launch-3.6.0.tar` & `energyplus_launch-3.6.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 19:34:58.345736 energyplus_launch-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3197 2023-04-12 19:34:58.345736 energyplus_launch-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 19:34:58.345736 energyplus_launch-3.6.0/energyplus_launch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3197 2023-04-12 19:34:58.000000 energyplus_launch-3.6.0/energyplus_launch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1260 2023-04-12 19:34:58.000000 energyplus_launch-3.6.0/energyplus_launch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 19:34:58.000000 energyplus_launch-3.6.0/energyplus_launch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-04-12 19:34:58.000000 energyplus_launch-3.6.0/energyplus_launch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-12 19:34:58.000000 energyplus_launch-3.6.0/energyplus_launch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-12 19:34:58.000000 energyplus_launch-3.6.0/energyplus_launch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 19:34:58.345736 energyplus_launch-3.6.0/eplaunch/
--rw-r--r--   0 runner    (1001) docker     (122)      389 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      289 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/configure.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 19:34:58.345736 energyplus_launch-3.6.0/eplaunch/interface/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9400 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/interface/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     5989 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/interface/dialog_external_viewers.py
--rw-r--r--   0 runner    (1001) docker     (122)      772 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/interface/dialog_generic.py
--rw-r--r--   0 runner    (1001) docker     (122)     2489 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/interface/dialog_output.py
--rw-r--r--   0 runner    (1001) docker     (122)     4914 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/interface/dialog_weather.py
--rw-r--r--   0 runner    (1001) docker     (122)     4588 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/interface/dialog_workflow_dirs.py
--rw-r--r--   0 runner    (1001) docker     (122)    68682 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/interface/frame_main.py
--rw-r--r--   0 runner    (1001) docker     (122)     5813 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/interface/widget_dir_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     5490 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/interface/widget_file_list.py
--rw-r--r--   0 runner    (1001) docker     (122)      146 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/tk_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 19:34:58.345736 energyplus_launch-3.6.0/eplaunch/utilities/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10941 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/utilities/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)      641 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/utilities/crossplatform.py
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/utilities/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 19:34:58.345736 energyplus_launch-3.6.0/eplaunch/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4817 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/workflows/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 19:34:58.345736 energyplus_launch-3.6.0/eplaunch/workflows/default/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/workflows/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/workflows/default/file_details.py
--rw-r--r--   0 runner    (1001) docker     (122)     3266 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/workflows/default/idf_details.py
--rw-r--r--   0 runner    (1001) docker     (122)     2163 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/workflows/default/site_location.py
--rw-r--r--   0 runner    (1001) docker     (122)     9936 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/workflows/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/workflows/workflow.py
--rw-r--r--   0 runner    (1001) docker     (122)     5368 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/workflows/workflow_tester.py
--rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/eplaunch/workflows/workflow_thread.py
--rw-r--r--   0 runner    (1001) docker     (122)      216 2023-04-12 19:34:58.345736 energyplus_launch-3.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-04-12 19:34:54.000000 energyplus_launch-3.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:31:45.971402 energyplus_launch-3.6.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-04-12 20:31:39.000000 energyplus_launch-3.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3197 2023-04-12 20:31:45.971402 energyplus_launch-3.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-04-12 20:31:39.000000 energyplus_launch-3.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:31:45.967402 energyplus_launch-3.6.1/energyplus_launch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3197 2023-04-12 20:31:45.000000 energyplus_launch-3.6.1/energyplus_launch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1260 2023-04-12 20:31:45.000000 energyplus_launch-3.6.1/energyplus_launch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 20:31:45.000000 energyplus_launch-3.6.1/energyplus_launch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-04-12 20:31:45.000000 energyplus_launch-3.6.1/energyplus_launch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-12 20:31:45.000000 energyplus_launch-3.6.1/energyplus_launch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-12 20:31:45.000000 energyplus_launch-3.6.1/energyplus_launch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:31:45.967402 energyplus_launch-3.6.1/eplaunch/
+-rw-r--r--   0 runner    (1001) docker     (122)      389 2023-04-12 20:31:39.000000 energyplus_launch-3.6.1/eplaunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-12 20:31:39.000000 energyplus_launch-3.6.1/eplaunch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-04-12 20:31:39.000000 energyplus_launch-3.6.1/eplaunch/configure.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:31:45.971402 energyplus_launch-3.6.1/eplaunch/interface/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 20:31:39.000000 energyplus_launch-3.6.1/eplaunch/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9400 2023-04-12 20:31:39.000000 energyplus_launch-3.6.1/eplaunch/interface/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5989 2023-04-12 20:31:39.000000 energyplus_launch-3.6.1/eplaunch/interface/dialog_external_viewers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      772 2023-04-12 20:31:39.000000 energyplus_launch-3.6.1/eplaunch/interface/dialog_generic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2489 2023-04-12 20:31:39.000000 energyplus_launch-3.6.1/eplaunch/interface/dialog_output.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4914 2023-04-12 20:31:39.000000 energyplus_launch-3.6.1/eplaunch/interface/dialog_weather.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4588 2023-04-12 20:31:39.000000 energyplus_launch-3.6.1/eplaunch/interface/dialog_workflow_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    68748 2023-04-12 20:31:39.000000 energyplus_launch-3.6.1/eplaunch/interface/frame_main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5813 2023-04-12 20:31:39.000000 energyplus_launch-3.6.1/eplaunch/interface/widget_dir_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5490 2023-04-12 20:31:39.000000 energyplus_launch-3.6.1/eplaunch/interface/widget_file_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)      146 2023-04-12 20:31:39.000000 energyplus_launch-3.6.1/eplaunch/tk_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:31:45.971402 energyplus_launch-3.6.1/eplaunch/utilities/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 20:31:39.000000 energyplus_launch-3.6.1/eplaunch/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10941 2023-04-12 20:31:39.000000 energyplus_launch-3.6.1/eplaunch/utilities/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)      641 2023-04-12 20:31:39.000000 energyplus_launch-3.6.1/eplaunch/utilities/crossplatform.py
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-04-12 20:31:39.000000 energyplus_launch-3.6.1/eplaunch/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-04-12 20:31:39.000000 energyplus_launch-3.6.1/eplaunch/utilities/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:31:45.971402 energyplus_launch-3.6.1/eplaunch/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 20:31:39.000000 energyplus_launch-3.6.1/eplaunch/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4817 2023-04-12 20:31:39.000000 energyplus_launch-3.6.1/eplaunch/workflows/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:31:45.971402 energyplus_launch-3.6.1/eplaunch/workflows/default/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 20:31:39.000000 energyplus_launch-3.6.1/eplaunch/workflows/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-04-12 20:31:39.000000 energyplus_launch-3.6.1/eplaunch/workflows/default/file_details.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3266 2023-04-12 20:31:39.000000 energyplus_launch-3.6.1/eplaunch/workflows/default/idf_details.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2163 2023-04-12 20:31:39.000000 energyplus_launch-3.6.1/eplaunch/workflows/default/site_location.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10103 2023-04-12 20:31:39.000000 energyplus_launch-3.6.1/eplaunch/workflows/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-04-12 20:31:39.000000 energyplus_launch-3.6.1/eplaunch/workflows/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5368 2023-04-12 20:31:39.000000 energyplus_launch-3.6.1/eplaunch/workflows/workflow_tester.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-04-12 20:31:39.000000 energyplus_launch-3.6.1/eplaunch/workflows/workflow_thread.py
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-04-12 20:31:45.971402 energyplus_launch-3.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-04-12 20:31:39.000000 energyplus_launch-3.6.1/setup.py
```

### Comparing `energyplus_launch-3.6.0/LICENSE` & `energyplus_launch-3.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.0/PKG-INFO` & `energyplus_launch-3.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energyplus_launch
-Version: 3.6.0
+Version: 3.6.1
 Summary: Graphical Interface and Workflow Manager for EnergyPlus
 Home-page: https://github.com/NREL/EP-Launch
 Author: Jason Glazer and Edwin Lee for the United States Department of Energy
 License: ModifiedBSD
 Description: # EP-Launch3
         
         [![GitHub release](https://img.shields.io/github/release/nrel/ep-launch.svg?style=for-the-badge)](https://github.com/nrel/ep-launch/releases/latest)
```

### Comparing `energyplus_launch-3.6.0/README.md` & `energyplus_launch-3.6.1/README.md`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.0/energyplus_launch.egg-info/PKG-INFO` & `energyplus_launch-3.6.1/energyplus_launch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energyplus-launch
-Version: 3.6.0
+Version: 3.6.1
 Summary: Graphical Interface and Workflow Manager for EnergyPlus
 Home-page: https://github.com/NREL/EP-Launch
 Author: Jason Glazer and Edwin Lee for the United States Department of Energy
 License: ModifiedBSD
 Description: # EP-Launch3
         
         [![GitHub release](https://img.shields.io/github/release/nrel/ep-launch.svg?style=for-the-badge)](https://github.com/nrel/ep-launch/releases/latest)
```

### Comparing `energyplus_launch-3.6.0/energyplus_launch.egg-info/SOURCES.txt` & `energyplus_launch-3.6.1/energyplus_launch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.0/eplaunch/interface/config.py` & `energyplus_launch-3.6.1/eplaunch/interface/config.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.0/eplaunch/interface/dialog_external_viewers.py` & `energyplus_launch-3.6.1/eplaunch/interface/dialog_external_viewers.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.0/eplaunch/interface/dialog_generic.py` & `energyplus_launch-3.6.1/eplaunch/interface/dialog_generic.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.0/eplaunch/interface/dialog_output.py` & `energyplus_launch-3.6.1/eplaunch/interface/dialog_output.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.0/eplaunch/interface/dialog_weather.py` & `energyplus_launch-3.6.1/eplaunch/interface/dialog_weather.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.0/eplaunch/interface/dialog_workflow_dirs.py` & `energyplus_launch-3.6.1/eplaunch/interface/dialog_workflow_dirs.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.0/eplaunch/interface/frame_main.py` & `energyplus_launch-3.6.1/eplaunch/interface/frame_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -311,15 +311,15 @@
             self.dir_files_pw, on_select=self._new_dir_selected, on_root_changed=self._new_root_dir
         )
         self.dir_files_pw.add(self.dir_tree, weight=1)
         self.file_list = FileListScrollableFrame(
             self.dir_files_pw, on_selection_changed=self._callback_file_selection_changed
         )
         self.dir_files_pw.add(self.file_list, weight=1)
-        self.list_group_pw.add(self.dir_files_pw, weight=10)
+        self.list_group_pw.add(self.dir_files_pw, weight=5)
         # the bottom part of the primary pane will be a label frame containing a group listbox, add it with lower weight
         group_label_frame = LabelFrame(self.list_group_pw, text="Current Group")
         self.group_list_box = Listbox(group_label_frame, height=5, selectmode=SINGLE)
         self.group_list_box.bind('<Double-1>', self._handle_group_selection_from_widget)
         from string import ascii_uppercase
         for i, e in enumerate(ascii_uppercase):
             self.group_list_box.insert(i + 1, e)
@@ -747,15 +747,15 @@
             weather_path = x
             self.option_weather_recent['menu'].add_command(
                 label=weather_path.name,
                 command=lambda w=weather_path: self._handler_weather_recent_option_changed(w)
             )
         if try_to_select in self.conf.weathers_recent:
             self._handler_weather_recent_option_changed(try_to_select)
-        else:
+        elif len(self.conf.weathers_recent) > 0:
             self._handler_weather_recent_option_changed(self.conf.weathers_recent[0])  # could persist in self.conf
 
     def _handler_weather_recent_option_changed(self, new_weather_path: Path):
         """This is called when the recent weather option menu changes value"""
         self._tk_var_weather_recent.set(str(new_weather_path.name))
         selected_recent_weather_string = self._tk_var_weather_recent.get()
         for selected_file_name in self.conf.file_selection:
@@ -804,15 +804,15 @@
         for opt in all_available_contexts:
             self.option_workflow_context['menu'].add_command(
                 label=opt, command=lambda c=opt: self._handler_workflow_context_option_changed(c)
             )
         # call the handler method with either the saved context name, or the top one in the list
         if desired_selected_workflow_context in all_available_contexts:
             self._handler_workflow_context_option_changed(desired_selected_workflow_context)
-        else:
+        elif len(all_available_contexts) > 0:
             self._handler_workflow_context_option_changed(all_available_contexts[0])
 
     def _handler_workflow_context_option_changed(self, new_value: str):
         """This is called when the workflow context option menu changes value"""
         # set the tk var and the config var to the new value
         self._tk_var_workflow_context.set(new_value)
         self.conf.cur_workflow_context = self._tk_var_workflow_context.get()
```

### Comparing `energyplus_launch-3.6.0/eplaunch/interface/widget_dir_list.py` & `energyplus_launch-3.6.1/eplaunch/interface/widget_dir_list.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.0/eplaunch/interface/widget_file_list.py` & `energyplus_launch-3.6.1/eplaunch/interface/widget_file_list.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.0/eplaunch/utilities/cache.py` & `energyplus_launch-3.6.1/eplaunch/utilities/cache.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.0/eplaunch/utilities/crossplatform.py` & `energyplus_launch-3.6.1/eplaunch/utilities/crossplatform.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.0/eplaunch/utilities/version.py` & `energyplus_launch-3.6.1/eplaunch/utilities/version.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.0/eplaunch/workflows/base.py` & `energyplus_launch-3.6.1/eplaunch/workflows/base.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.0/eplaunch/workflows/default/file_details.py` & `energyplus_launch-3.6.1/eplaunch/workflows/default/file_details.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.0/eplaunch/workflows/default/idf_details.py` & `energyplus_launch-3.6.1/eplaunch/workflows/default/idf_details.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.0/eplaunch/workflows/default/site_location.py` & `energyplus_launch-3.6.1/eplaunch/workflows/default/site_location.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.0/eplaunch/workflows/manager.py` & `energyplus_launch-3.6.1/eplaunch/workflows/manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,22 +25,24 @@
     def workflow_instances(self, workflow_context: str) -> List[Workflow]:
         return [x for x in self.workflows if x.context == workflow_context]
 
     def auto_find_workflow_directories(self) -> None:
         """Locate the (EnergyPlus) workflow directories that are in predestined locations"""
         self.auto_found_workflow_dirs = []
         # then search for e+ workflows
-        search_roots: Dict[str, List[Path]] = {
+        search_roots: Dict[int, List[Path]] = {
             Platform.WINDOWS: [Path(f"{c}:\\") for c in ascii_uppercase],
             Platform.LINUX: [Path('/usr/local/bin/'), Path('/tmp/')],
             Platform.MAC: [Path('/Applications/'), Path('/tmp/')],
             Platform.UNKNOWN: [],
         }
         current_search_roots = search_roots[Platform.get_current_platform()]
-        search_names = ["EnergyPlus*", "energyplus*", "EP*", "ep*", "E+*", "e+*"]
+        search_names = ["EnergyPlus*", "EP*", "ep*", "E+*", "e+*"]
+        if Platform.get_current_platform() == Platform.LINUX:
+            search_names.append("energyplus*")  # add lower case check on case-sensitive file systems (typically Linux)
         for search_root in current_search_roots:
             for search_name in search_names:
                 eplus_folder_matches = search_root.glob(search_name)
                 for ep_folder in eplus_folder_matches:  # pragma: no cover, would have to install into system folders
                     ep_workflow_dir = ep_folder / 'workflows'
                     if ep_workflow_dir.exists():
                         self.auto_found_workflow_dirs.append(ep_workflow_dir)
```

### Comparing `energyplus_launch-3.6.0/eplaunch/workflows/workflow.py` & `energyplus_launch-3.6.1/eplaunch/workflows/workflow.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.0/eplaunch/workflows/workflow_tester.py` & `energyplus_launch-3.6.1/eplaunch/workflows/workflow_tester.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.0/eplaunch/workflows/workflow_thread.py` & `energyplus_launch-3.6.1/eplaunch/workflows/workflow_thread.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.0/setup.py` & `energyplus_launch-3.6.1/setup.py`

 * *Files identical despite different names*

