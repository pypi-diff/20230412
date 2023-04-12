# Comparing `tmp/quantifiles-0.1.1.tar.gz` & `tmp/quantifiles-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantifiles-0.1.1.tar", last modified: Tue Mar 28 19:11:38 2023, max compression
+gzip compressed data, was "quantifiles-0.2.0.tar", last modified: Wed Apr 12 18:53:48 2023, max compression
```

## Comparing `quantifiles-0.1.1.tar` & `quantifiles-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-03-28 19:11:38.054787 quantifiles-0.1.1/
--rw-rw-rw-   0        0        0     1351 2023-03-12 18:13:35.000000 quantifiles-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     4459 2023-03-28 19:11:38.054787 quantifiles-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2531 2023-03-26 21:36:14.000000 quantifiles-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-28 19:11:37.991877 quantifiles-0.1.1/quantifiles/
--rw-rw-rw-   0        0        0     1499 2023-03-28 19:08:40.000000 quantifiles-0.1.1/quantifiles/__init__.py
--rw-rw-rw-   0        0        0     8044 2023-03-26 21:36:14.000000 quantifiles-0.1.1/quantifiles/data.py
--rw-rw-rw-   0        0        0    17956 2023-03-28 18:55:26.000000 quantifiles-0.1.1/quantifiles/main.py
--rw-rw-rw-   0        0        0      486 2023-03-24 06:46:53.000000 quantifiles-0.1.1/quantifiles/path.py
-drwxrwxrwx   0        0        0        0 2023-03-28 19:11:38.050276 quantifiles-0.1.1/quantifiles/plot/
--rw-rw-rw-   0        0        0        0 2023-03-14 21:03:29.000000 quantifiles-0.1.1/quantifiles/plot/__init__.py
--rw-rw-rw-   0        0        0     1749 2023-03-28 18:55:26.000000 quantifiles-0.1.1/quantifiles/plot/autoplot.py
--rw-rw-rw-   0        0        0     3489 2023-03-28 18:55:26.000000 quantifiles-0.1.1/quantifiles/plot/baseplot.py
--rw-rw-rw-   0        0        0     5307 2023-03-28 18:55:26.000000 quantifiles-0.1.1/quantifiles/plot/colorplot.py
--rw-rw-rw-   0        0        0     2676 2023-03-24 06:46:53.000000 quantifiles-0.1.1/quantifiles/plot/header.py
--rw-rw-rw-   0        0        0     4695 2023-03-28 18:55:26.000000 quantifiles-0.1.1/quantifiles/plot/lineplot.py
--rw-rw-rw-   0        0        0     2118 2023-03-26 21:36:14.000000 quantifiles-0.1.1/quantifiles/plot/utils.py
--rw-rw-rw-   0        0        0    14913 2023-03-28 18:55:26.000000 quantifiles-0.1.1/quantifiles/plot/window.py
--rw-rw-rw-   0        0        0     2187 2023-03-26 21:36:14.000000 quantifiles-0.1.1/quantifiles/units.py
--rw-rw-rw-   0        0        0    10207 2023-03-26 21:36:14.000000 quantifiles-0.1.1/quantifiles/watcher.py
-drwxrwxrwx   0        0        0        0 2023-03-28 19:11:38.023137 quantifiles-0.1.1/quantifiles.egg-info/
--rw-rw-rw-   0        0        0     4459 2023-03-28 19:11:37.000000 quantifiles-0.1.1/quantifiles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      649 2023-03-28 19:11:37.000000 quantifiles-0.1.1/quantifiles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-28 19:11:37.000000 quantifiles-0.1.1/quantifiles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-03-28 19:11:37.000000 quantifiles-0.1.1/quantifiles.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      104 2023-03-28 19:11:37.000000 quantifiles-0.1.1/quantifiles.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-03-28 19:11:37.000000 quantifiles-0.1.1/quantifiles.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-28 19:11:38.054787 quantifiles-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      967 2023-03-28 19:08:40.000000 quantifiles-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-28 19:11:38.054787 quantifiles-0.1.1/tests/
--rw-rw-rw-   0        0        0        0 2023-03-19 19:21:13.000000 quantifiles-0.1.1/tests/__init__.py
--rw-rw-rw-   0        0        0     1095 2023-03-26 21:36:14.000000 quantifiles-0.1.1/tests/test_data.py
--rw-rw-rw-   0        0        0      539 2023-03-19 19:21:13.000000 quantifiles-0.1.1/tests/test_units.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:53:48.976854 quantifiles-0.2.0/
+-rw-rw-rw-   0        0        0     1351 2023-03-12 18:13:35.000000 quantifiles-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     4459 2023-04-12 18:53:48.976854 quantifiles-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2531 2023-03-26 21:36:14.000000 quantifiles-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 18:53:48.778313 quantifiles-0.2.0/quantifiles/
+-rw-rw-rw-   0        0        0     1499 2023-04-12 18:52:19.000000 quantifiles-0.2.0/quantifiles/__init__.py
+-rw-rw-rw-   0        0        0     8044 2023-03-26 21:36:14.000000 quantifiles-0.2.0/quantifiles/data.py
+-rw-rw-rw-   0        0        0    18739 2023-04-12 18:52:19.000000 quantifiles-0.2.0/quantifiles/main.py
+-rw-rw-rw-   0        0        0      486 2023-03-24 06:46:53.000000 quantifiles-0.2.0/quantifiles/path.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:53:48.935103 quantifiles-0.2.0/quantifiles/plot/
+-rw-rw-rw-   0        0        0        0 2023-03-14 21:03:29.000000 quantifiles-0.2.0/quantifiles/plot/__init__.py
+-rw-rw-rw-   0        0        0     1749 2023-03-28 19:15:19.000000 quantifiles-0.2.0/quantifiles/plot/autoplot.py
+-rw-rw-rw-   0        0        0     3489 2023-03-28 19:15:19.000000 quantifiles-0.2.0/quantifiles/plot/baseplot.py
+-rw-rw-rw-   0        0        0     5408 2023-04-12 18:52:19.000000 quantifiles-0.2.0/quantifiles/plot/colorplot.py
+-rw-rw-rw-   0        0        0     2676 2023-03-24 06:46:53.000000 quantifiles-0.2.0/quantifiles/plot/header.py
+-rw-rw-rw-   0        0        0     4695 2023-03-28 19:15:19.000000 quantifiles-0.2.0/quantifiles/plot/lineplot.py
+-rw-rw-rw-   0        0        0     2118 2023-03-26 21:36:14.000000 quantifiles-0.2.0/quantifiles/plot/utils.py
+-rw-rw-rw-   0        0        0    15748 2023-04-12 18:52:19.000000 quantifiles-0.2.0/quantifiles/plot/window.py
+-rw-rw-rw-   0        0        0     2187 2023-03-26 21:36:14.000000 quantifiles-0.2.0/quantifiles/units.py
+-rw-rw-rw-   0        0        0    10207 2023-03-26 21:36:14.000000 quantifiles-0.2.0/quantifiles/watcher.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:53:48.856501 quantifiles-0.2.0/quantifiles.egg-info/
+-rw-rw-rw-   0        0        0     4459 2023-04-12 18:53:48.000000 quantifiles-0.2.0/quantifiles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      649 2023-04-12 18:53:48.000000 quantifiles-0.2.0/quantifiles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 18:53:48.000000 quantifiles-0.2.0/quantifiles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-04-12 18:53:48.000000 quantifiles-0.2.0/quantifiles.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      104 2023-04-12 18:53:48.000000 quantifiles-0.2.0/quantifiles.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-12 18:53:48.000000 quantifiles-0.2.0/quantifiles.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 18:53:48.976854 quantifiles-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      967 2023-04-12 18:52:19.000000 quantifiles-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:53:48.966338 quantifiles-0.2.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-19 19:21:13.000000 quantifiles-0.2.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     1095 2023-03-26 21:36:14.000000 quantifiles-0.2.0/tests/test_data.py
+-rw-rw-rw-   0        0        0      539 2023-03-19 19:21:13.000000 quantifiles-0.2.0/tests/test_units.py
```

### Comparing `quantifiles-0.1.1/LICENSE` & `quantifiles-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quantifiles-0.1.1/PKG-INFO` & `quantifiles-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantifiles
-Version: 0.1.1
+Version: 0.2.0
 Summary: Simple databrowser for quantify datasets.
 Home-page: https://gitlab.com/dcrielaard/quantifiles
 Author: Damien Crielaard
 Author-email: damiencrielaard@gmail.com
 License: BSD 2-Clause License
         
         Copyright (c) 2023, Damien Crielaard
```

### Comparing `quantifiles-0.1.1/README.md` & `quantifiles-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `quantifiles-0.1.1/quantifiles/__init__.py` & `quantifiles-0.2.0/quantifiles/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from quantifiles.main import main
 
 from pathlib import Path
 
 __all__ = ["quantifiles", "__version__"]
 
-__version__ = "0.1.1"
+__version__ = "0.2.0"
 
 
 def quantifiles(
     data_dir: str | Path | None = None,
     liveplotting: bool = False,
     log_level: int | str = logging.WARNING,
 ) -> None:
```

### Comparing `quantifiles-0.1.1/quantifiles/data.py` & `quantifiles-0.2.0/quantifiles/data.py`

 * *Files identical despite different names*

### Comparing `quantifiles-0.1.1/quantifiles/main.py` & `quantifiles-0.2.0/quantifiles/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 import sys
 from datetime import datetime
 from pathlib import Path
 from typing import Sequence, Mapping
 
 from PyQt5 import QtCore, QtWidgets, QtGui
-from PyQt5.QtWidgets import QDesktopWidget
+from PyQt5.QtWidgets import QDesktopWidget, QMessageBox
 from quantify_core.data.handling import set_datadir
 from quantify_core.data.types import TUID
 
 from quantifiles.path import load_icon
 from quantifiles.data import (
     get_results_for_date,
     safe_load_dataset,
@@ -357,14 +357,20 @@
         file_menu.addAction(open_action)
 
         reload_action = QtWidgets.QAction("&Reload", self)
         reload_action.setShortcut("R")
         reload_action.triggered.connect(self.reload_datadir)
         file_menu.addAction(reload_action)
 
+        # create Close all plots action
+        close_plots_action = QtWidgets.QAction("&Close all plots", self)
+        close_plots_action.setShortcut("X")
+        close_plots_action.triggered.connect(self.close_all_plots)
+        file_menu.addAction(close_plots_action)
+
         # create Exit action
         exit_action = QtWidgets.QAction("&Exit", self)
         exit_action.setShortcut("Ctrl+Q")
         exit_action.triggered.connect(self.close)
         file_menu.addAction(exit_action)
 
         self._today_folder_monitor = TodayFolderMonitor(self.datadir)
@@ -422,14 +428,19 @@
         self._update_date_list()
         self._today_folder_monitor.set_datadir(self.datadir)
 
         # Reselect the dates to update
         self.set_date_selection(self._selected_dates)
 
     @QtCore.pyqtSlot()
+    def close_all_plots(self) -> None:
+        for plot in self.plots:
+            plot.close()
+
+    @QtCore.pyqtSlot()
     def _update_date_list(self) -> None:
         dates = get_all_dates_with_measurements()
         date_strings = [date.strftime("%Y-%m-%d") for date in dates]
         self.date_list.update_date_list(date_strings)
 
     @QtCore.pyqtSlot()
     def configure_datadir(self) -> None:
@@ -446,14 +457,21 @@
         if path:
             self.datadir = path
             self.new_datadir_selected.emit(path)
 
     def update_datadir(self) -> None:
         self.reload_datadir()
         self.date_list.setCurrentRow(0)
+        if self.date_list.count() == 0:
+            QMessageBox.warning(
+                self,
+                "No measurements found",
+                "No measurements were found in the selected data directory.\n\nEither no measurements have been taken "
+                "yet or the selected directory is not a valid quantify data directory.",
+            )
 
     @QtCore.pyqtSlot(str)
     def _on_new_measurement(self, tuid: str):
         self.set_date_selection(self._selected_dates)
         if self._auto_open_plots:
             self.open_plots(tuid)
```

### Comparing `quantifiles-0.1.1/quantifiles/plot/autoplot.py` & `quantifiles-0.2.0/quantifiles/plot/autoplot.py`

 * *Files identical despite different names*

### Comparing `quantifiles-0.1.1/quantifiles/plot/baseplot.py` & `quantifiles-0.2.0/quantifiles/plot/baseplot.py`

 * *Files identical despite different names*

### Comparing `quantifiles-0.1.1/quantifiles/plot/colorplot.py` & `quantifiles-0.2.0/quantifiles/plot/colorplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,16 @@
 
         self.x = x
         self.y = y
         self.z = z
 
         self.img = pyqtgraph.ImageItem()
         self.img.setColorMap(pyqtgraph.colormap.get(colormap))
-        self.colorbar = pyqtgraph.ColorBarItem()
+
+        self.colorbar = pyqtgraph.ColorBarItem(width=16, cmap=colormap)
 
         self.plot.addItem(self.img)
 
         # Check that necessary attributes are present in the dataset
         assert "long_name" in dataset[x].attrs, f"{x} attribute 'long_name' not found"
         assert "units" in dataset[x].attrs, f"{x} attribute 'units' not found"
         assert "long_name" in dataset[y].attrs, f"{y} attribute 'long_name' not found"
@@ -128,14 +129,15 @@
             QtCore.QRectF(
                 np.min(x_data),
                 np.min(y_data),
                 np.max(x_data) - np.min(x_data),
                 np.max(y_data) - np.min(y_data),
             )
         )
+        self.colorbar.setImageItem(self.img, insert_in=self.plot.plotItem)
 
     def get_mouse_position_text(self, x: float, y: float) -> str:
         """
         Get the text to display when the mouse is moved over the plot.
 
         Parameters
         ----------
```

### Comparing `quantifiles-0.1.1/quantifiles/plot/header.py` & `quantifiles-0.2.0/quantifiles/plot/header.py`

 * *Files identical despite different names*

### Comparing `quantifiles-0.1.1/quantifiles/plot/lineplot.py` & `quantifiles-0.2.0/quantifiles/plot/lineplot.py`

 * *Files identical despite different names*

### Comparing `quantifiles-0.1.1/quantifiles/plot/utils.py` & `quantifiles-0.2.0/quantifiles/plot/utils.py`

 * *Files identical despite different names*

### Comparing `quantifiles-0.1.1/quantifiles/plot/window.py` & `quantifiles-0.2.0/quantifiles/plot/window.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,15 +167,15 @@
         self.mouse_pos_label.setWordWrap(True)
         self.mouse_pos_label.setSizePolicy(
             QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed
         )
         layout.addWidget(self.mouse_pos_label)
 
     def on_new_mouse_pos_text(self, text: str):
-        self.mouse_pos_label.setText(f"Mouse at: {text}")
+        self.mouse_pos_label.setText(str(text))
 
     def gettable_state_changed(self, name: str):
         """
         Emit the gettable_toggled signal with the name of the toggled checkbox and its state.
 
         Parameters
         ----------
@@ -245,37 +245,51 @@
 class PlotTab(QtWidgets.QWidget):
     def __init__(self, dataset: xr.Dataset | None):
         super().__init__()
         self.dataset = dataset
         self.gettable_select_box = GettableSelectBox(dataset=dataset)
         self.name_and_tuid_box = NameAndTuidBox(name=dataset.name, tuid=dataset.tuid)
 
-        layout = QtWidgets.QHBoxLayout(self)
-
         left_column_layout = QtWidgets.QVBoxLayout(self)
         left_column_layout.addWidget(self.name_and_tuid_box)
         left_column_layout.addWidget(self.gettable_select_box)
 
-        layout.addLayout(left_column_layout)
+        column_container = QtWidgets.QWidget()
+        column_container.setLayout(left_column_layout)
+
+        self.plot_layout = QtWidgets.QHBoxLayout(self)
+        plot_container = QtWidgets.QWidget()
+        plot_container.setLayout(self.plot_layout)
+
+        splitter = QtWidgets.QSplitter(QtCore.Qt.Horizontal)
+        splitter.addWidget(column_container)
+        splitter.addWidget(plot_container)
+        splitter.setSizes([80, 640])
+
+        layout = QtWidgets.QHBoxLayout(self)
+        layout.addWidget(splitter)
         self.setLayout(layout)
 
     def add_plot(self, plot: QtWidgets.QWidget):
-        self.layout().addWidget(plot)
+        self.plot_layout.addWidget(plot)
+        plot.setSizePolicy(
+            QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Preferred
+        )
 
 
 class SnapshotTab(QtWidgets.QWidget):
     def __init__(self, snapshot: dict[str, any]):
         super().__init__()
         self.snapshot = snapshot
 
         layout = QtWidgets.QVBoxLayout(self)
 
         self.snapshot_tree = QtWidgets.QTreeWidget()
         self.snapshot_tree.setHeaderLabels(["Name", "Value"])
-        self.snapshot_tree.setColumnWidth(0, 200)
+        self.snapshot_tree.setColumnWidth(0, 256)
         self.snapshot_tree.setSortingEnabled(True)
         self.snapshot_tree.setContextMenuPolicy(QtCore.Qt.CustomContextMenu)
         self.snapshot_tree.customContextMenuRequested.connect(
             self.show_copy_context_menu
         )
 
         self.add_snapshot_to_tree(self.snapshot_tree, self.snapshot)
@@ -351,15 +365,16 @@
 
     def add_plot(self, plot: QtWidgets.QWidget):
         self.plot_tab.add_plot(plot)
 
 
 class PlotWindow(QtWidgets.QMainWindow):
     _WINDOW_TITLE: str = "Quantifiles plot window"
-    _WINDOW_SIZE: int = 200
+    _WINDOW_HEIGHT: int = 600
+    _WINDOW_WIDTH: int = 300
 
     def __init__(self, dataset: xr.Dataset, parent: QtWidgets.QWidget | None = None):
         super().__init__(parent)
         self.dataset = dataset
         self.plots = {}
 
         tuid = self.dataset.tuid if hasattr(self.dataset, "tuid") else "no tuid"
@@ -371,28 +386,36 @@
             f"Initialized {self.__class__.__name__} with title: {self.windowTitle()}"
         )
 
         canvas = PlotWindowContent(self, dataset=dataset, snapshot=self.snapshot)
         self.canvas = canvas
         self.setCentralWidget(canvas)
 
-        self.setSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.setMinimumSize(self._WINDOW_SIZE, self._WINDOW_SIZE)
-
         canvas.plot_tab.gettable_select_box.gettable_toggled.connect(
             self.toggle_gettable
         )
 
+        # make sure the window is on top, and that it is activated. Does not always work on Windows due to Windows not
+        # allowing this if the application is not the active window.
+        self.show()
+        self.raise_()
+        self.activateWindow()
+
     def add_plot(self, name: str, plot: BasePlot):
         self.canvas.add_plot(plot)
         self.plots[name] = plot
         plot.mouse_text_changed.connect(
             self.canvas.plot_tab.gettable_select_box.on_new_mouse_pos_text
         )
 
+        self.resize(
+            self._WINDOW_WIDTH + self._WINDOW_HEIGHT * len(self.plots),
+            self._WINDOW_HEIGHT,
+        )
+
         logger.debug(f"Added plot with name {name} to {self.__class__.__name__}")
 
     @QtCore.pyqtSlot(str, bool)
     def toggle_gettable(self, name: str, enabled: bool):
         self.plots[name].setVisible(enabled)
 
         logger.debug(f"Toggled visibility of plot with name {name} to {enabled}")
```

### Comparing `quantifiles-0.1.1/quantifiles/units.py` & `quantifiles-0.2.0/quantifiles/units.py`

 * *Files identical despite different names*

### Comparing `quantifiles-0.1.1/quantifiles/watcher.py` & `quantifiles-0.2.0/quantifiles/watcher.py`

 * *Files identical despite different names*

### Comparing `quantifiles-0.1.1/quantifiles.egg-info/PKG-INFO` & `quantifiles-0.2.0/quantifiles.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantifiles
-Version: 0.1.1
+Version: 0.2.0
 Summary: Simple databrowser for quantify datasets.
 Home-page: https://gitlab.com/dcrielaard/quantifiles
 Author: Damien Crielaard
 Author-email: damiencrielaard@gmail.com
 License: BSD 2-Clause License
         
         Copyright (c) 2023, Damien Crielaard
```

### Comparing `quantifiles-0.1.1/quantifiles.egg-info/SOURCES.txt` & `quantifiles-0.2.0/quantifiles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quantifiles-0.1.1/setup.py` & `quantifiles-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     readme = f.read()
 
 with open("LICENSE") as f:
     license = f.read()
 
 setup(
     name="quantifiles",
-    version="0.1.1",
+    version="0.2.0",
     description="Simple databrowser for quantify datasets.",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Damien Crielaard",
     author_email="damiencrielaard@gmail.com",
     url="https://gitlab.com/dcrielaard/quantifiles",
     license=license,
```

### Comparing `quantifiles-0.1.1/tests/test_data.py` & `quantifiles-0.2.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `quantifiles-0.1.1/tests/test_units.py` & `quantifiles-0.2.0/tests/test_units.py`

 * *Files identical despite different names*

