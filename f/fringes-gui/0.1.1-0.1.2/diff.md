# Comparing `tmp/fringes_gui-0.1.1.tar.gz` & `tmp/fringes_gui-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fringes_gui-0.1.1.tar", max compression
+gzip compressed data, was "fringes_gui-0.1.2.tar", max compression
```

## Comparing `fringes_gui-0.1.1.tar` & `fringes_gui-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       90 2023-04-12 19:12:29.413201 fringes_gui-0.1.1/fringes_gui/__init__.py
--rw-r--r--   0        0        0    16274 2023-04-12 16:24:37.024183 fringes_gui-0.1.1/fringes_gui/gui.py
--rw-r--r--   0        0        0    18031 2023-04-12 16:37:04.376908 fringes_gui-0.1.1/fringes_gui/logic.py
--rw-r--r--   0        0        0      231 2023-04-12 07:45:19.000000 fringes_gui-0.1.1/fringes_gui/main.py
--rw-r--r--   0        0        0    26876 2023-04-12 13:19:40.997785 fringes_gui-0.1.1/fringes_gui/params.py
--rw-r--r--   0        0        0    27386 2023-04-12 13:20:41.909708 fringes_gui-0.1.1/fringes_gui/setters.py
--rw-r--r--   0        0        0   250284 2023-04-01 09:49:27.000000 fringes_gui-0.1.1/fringes_gui/spirals.png
--rw-r--r--   0        0        0      715 2023-04-12 19:12:29.420182 fringes_gui-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3831 2023-04-12 19:08:07.044758 fringes_gui-0.1.1/README.md
--rw-r--r--   0        0        0     4676 1970-01-01 00:00:00.000000 fringes_gui-0.1.1/setup.py
--rw-r--r--   0        0        0     4637 1970-01-01 00:00:00.000000 fringes_gui-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       90 2023-04-12 20:02:53.369380 fringes_gui-0.1.2/fringes_gui/__init__.py
+-rw-r--r--   0        0        0    16385 2023-04-12 20:02:20.615647 fringes_gui-0.1.2/fringes_gui/gui.py
+-rw-r--r--   0        0        0    18072 2023-04-12 19:56:33.023246 fringes_gui-0.1.2/fringes_gui/logic.py
+-rw-r--r--   0        0        0      231 2023-04-12 07:45:19.000000 fringes_gui-0.1.2/fringes_gui/main.py
+-rw-r--r--   0        0        0    26876 2023-04-12 13:19:40.997785 fringes_gui-0.1.2/fringes_gui/params.py
+-rw-r--r--   0        0        0    27386 2023-04-12 13:20:41.909708 fringes_gui-0.1.2/fringes_gui/setters.py
+-rw-r--r--   0        0        0   250284 2023-04-01 09:49:27.000000 fringes_gui-0.1.2/fringes_gui/spirals.png
+-rw-r--r--   0        0        0      715 2023-04-12 20:02:53.377359 fringes_gui-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3858 2023-04-12 19:21:58.331433 fringes_gui-0.1.2/README.md
+-rw-r--r--   0        0        0     4707 1970-01-01 00:00:00.000000 fringes_gui-0.1.2/setup.py
+-rw-r--r--   0        0        0     4660 1970-01-01 00:00:00.000000 fringes_gui-0.1.2/PKG-INFO
```

### Comparing `fringes_gui-0.1.1/fringes_gui/gui.py` & `fringes_gui-0.1.2/fringes_gui/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,16 @@
     """Simple graphical user interface for the 'fringes' package."""
 
     def __init__(self):
         super(FringesGUI, self).__init__([])
 
         myappid = "Fringes-GUI"  # arbitrary string
         try:
-            version = toml.load("..\\pyproject.toml")["tool"]["poetry"]["version"]
+            fname = os.path.join(os.path.dirname(__file__), "..", "pyproject.toml")
+            version = toml.load(fname)["tool"]["poetry"]["version"]
             myappid += "_" + version
         except Exception:
             pass
         ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(myappid)
 
         pg.setConfigOptions(imageAxisOrder="row-major", useNumba=True)  # useCupy
 
@@ -55,15 +56,15 @@
         #     # self.win.move(0, 0)  # move to the left
         #     self.win.move(self.desktop.availableGeometry().width() // 2, 0)  # move to the right
         # else:
         #     self.win.showMaximized()  # self.win.showFullScreen()
 
         self.win.showMaximized()  # self.win.showFullScreen()
 
-        self.win.setWindowIcon(QtGui.QIcon("spirals.png"))
+        self.win.setWindowIcon(QtGui.QIcon(os.path.join(os.path.dirname(__file__), "spirals.png")))
 
         self.win.setWindowTitle(myappid)
 
         # set style
         # self.setStyleSheet(open("QTDark.stylesheet").read())
 
         # import qdarkstyle
```

### Comparing `fringes_gui-0.1.1/fringes_gui/logic.py` & `fringes_gui-0.1.2/fringes_gui/logic.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,16 @@
 
                         if ext_i == ext and root_i == root and data.shape == data_i.shape and data.dtype == data_i.dtype:
                             sequence[i+1] = data_i
                         else:
                             gui.fringes.logger.error("Files in list dint't match; terminated loading data.")
                             return
 
-                    setattr(gui.con, root, frng.vshape(sequence))
+                    sequence = frng.vshape(sequence)
+                    setattr(gui.con, root, sequence)
                     gui.fringes.logger.info(f"Loaded data from '{path}'.")
 
                     view(getattr(gui.con, root))
                     gui.data_table.setData(gui.con.info)
                     QtWidgets.QApplication.processEvents()  # refresh event queue
 
             gui.decode_button.setEnabled(gui.decodeOK)
```

### Comparing `fringes_gui-0.1.1/fringes_gui/params.py` & `fringes_gui-0.1.2/fringes_gui/params.py`

 * *Files identical despite different names*

### Comparing `fringes_gui-0.1.1/fringes_gui/setters.py` & `fringes_gui-0.1.2/fringes_gui/setters.py`

 * *Files identical despite different names*

### Comparing `fringes_gui-0.1.1/fringes_gui/spirals.png` & `fringes_gui-0.1.2/fringes_gui/spirals.png`

 * *Files identical despite different names*

### Comparing `fringes_gui-0.1.1/pyproject.toml` & `fringes_gui-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Fringes-GUI"
-version = "0.1.1"
+version = "0.1.2"
 description = "Graphical user interface for the 'fringes' package."
 license = "CC-BY-NC-SA-4.0"
 authors = ["Christian Kludt"]
 readme = "README.md"
 repository = "https://github.com/comimag/fringes-gui"
 keywords = ["phase shifting", "fringe analysis", "fringe projection", "deflectometry", "computational imaging"]
```

### Comparing `fringes_gui-0.1.1/README.md` & `fringes_gui-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -34,32 +34,36 @@
 
 The Visibility defines the type of user that should get access to the feature.
 It does not affect the functionality of the features but is used by the GUI to
 decide which features to display based on the current user level. The purpose
 is mainly to ensure that the GUI is not cluttered with information that is not
 intended at the current visibility level. The following criteria have been used
 for the assignment of the recommended visibility:
-- Beginner: Features that should be visible for all users via the GUI. This
-is the default visibility. The number of features with 'Beginner' visibility
-should be limited to all basic features so the GUI display is well-organized
-and easy to use.
-- Expert: Features that require a more in-depth knowledge of the system
-functionality. This is the preferred visibility level for all advanced features.
-- Guru: Advanced features that usually only people with a sound background in phase shifting can make good use of.
-- Experimental: New features that have not been tested yet
-and the system might probably crash at some point.
+- Beginner:\
+  Features that should be visible for all users via the GUI. This
+  is the default visibility. The number of features with 'Beginner' visibility
+  should be limited to all basic features so the GUI display is well-organized
+  and easy to use.
+- Expert:\
+  Features that require a more in-depth knowledge of the system
+  functionality. This is the preferred visibility level for all advanced features.
+- Guru:\
+  Advanced features that usually only people with a sound background in phase shifting can make good use of.
+- Experimental:\
+  New features that have not been tested yet
+  and are likely to crash the system at some point.
 
 ### Function Buttons
 In the bottem left corner you will find buttons for the associated methods of the `Fringes` class.
 Alternatively, you can use the keyboard shortcuts which are displayed when you hover over the buttons.
 The buttons are only active if the necessary data has been enoded, decoded or loaded.
 
 ### Viewer
 In the center resides the viewer.
-If float data is to be displayed, nan is replaced by zeros.
+If float data is to be displayed, `nan` is replaced by zeros.
 
 ### Data
 In the top right corner the data widget is located.
 It lists the data which has been encoded, decoded or was loaded.
 
 In order to keep the [Parameter Tree](#parameter-tree) consistent with the data,
 once a parameter has changed, certain data will be removed
@@ -74,12 +78,12 @@
 Use the `Clear all` button to delete all data.
 
 Please note: By default, the datum `fringes` is decoded.
 If you want to decode a datum with a different name (e.g. one that you just loaded),
 select its name in the table and klick `Set data (to be decoded)`.
 
 ### Log
-Here the logging of the `Fringes` class is displayed.
+The logging of the `Fringes` class is displayed here.
 The logging level can be set in the [Parameter Tree](#parameter-tree).
 
 ## License
 Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International Public License
```

### Comparing `fringes_gui-0.1.1/setup.py` & `fringes_gui-0.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,17 +14,17 @@
  'pyqtgraph>=0.13.2,<0.14.0',
  'pyyaml>=6.0,<7.0',
  'scikit-image>=0.19.3,<0.20.0',
  'toml>=0.10.2,<0.11.0']
 
 setup_kwargs = {
     'name': 'fringes-gui',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': "Graphical user interface for the 'fringes' package.",
-    'long_description': "# Fringes-GUI\nAuthor: Christian Kludt\n\n## Description\nGraphical user interface for the [fringes](https://pypi.org/project/fringes/) package.\n\n## Installation\nYou can install `fringes-gui` directly from [PyPi](https://pypi.org/project/fringes-gui) via `pip`:\n\n```\npip install fringes-gui\n```\n\n## Usage\nYou import the `fringes-gui` package and call the function `run()`.\n\n```python\nimport fringes_gui as fgui\nfgui.run()\n```\n\nNow the graphical user interface should appear:\n\n![Screenshot](docs/GUI.png)\\\nScreenshot of the GUI.\n\n### Parameter Tree\nIn the top left corner the attribute widget is located.\nIt contains the parameter tree with which all the properties of the `Fringes` class\nfrom the [fringes](https://pypi.org/project/fringes/) package can be controlled.\nCheck out its website for more details.\nHowever, if you select a parameter and hover over it, a tool tip will appear\ncontaining the docstring of the respective property of the `Fringes` class.\n\nThe Visibility defines the type of user that should get access to the feature.\nIt does not affect the functionality of the features but is used by the GUI to\ndecide which features to display based on the current user level. The purpose\nis mainly to ensure that the GUI is not cluttered with information that is not\nintended at the current visibility level. The following criteria have been used\nfor the assignment of the recommended visibility:\n- Beginner: Features that should be visible for all users via the GUI. This\nis the default visibility. The number of features with 'Beginner' visibility\nshould be limited to all basic features so the GUI display is well-organized\nand easy to use.\n- Expert: Features that require a more in-depth knowledge of the system\nfunctionality. This is the preferred visibility level for all advanced features.\n- Guru: Advanced features that usually only people with a sound background in phase shifting can make good use of.\n- Experimental: New features that have not been tested yet\nand the system might probably crash at some point.\n\n### Function Buttons\nIn the bottem left corner you will find buttons for the associated methods of the `Fringes` class.\nAlternatively, you can use the keyboard shortcuts which are displayed when you hover over the buttons.\nThe buttons are only active if the necessary data has been enoded, decoded or loaded.\n\n### Viewer\nIn the center resides the viewer.\nIf float data is to be displayed, nan is replaced by zeros.\n\n### Data\nIn the top right corner the data widget is located.\nIt lists the data which has been encoded, decoded or was loaded.\n\nIn order to keep the [Parameter Tree](#parameter-tree) consistent with the data,\nonce a parameter has changed, certain data will be removed\nand also certain [buttons](#function-buttons) will be deactivated.\nAs a consequence, if you load data - e.g. the acquired (deflected) fringe pattern sequence - \nthe first element of its videoshape has to match the parameter `Frames` in order to be able to decode it.\n\nTo display any datum listed in the table in the [Viewer](#viewer), simly select the name of it in the table.\n\nKlick the `Load` button to choose a data or parameter set to load.\nWith the `Save` button, all data including the parameter set are saved to the selected directory.\nUse the `Clear all` button to delete all data.\n\nPlease note: By default, the datum `fringes` is decoded.\nIf you want to decode a datum with a different name (e.g. one that you just loaded),\nselect its name in the table and klick `Set data (to be decoded)`.\n\n### Log\nHere the logging of the `Fringes` class is displayed.\nThe logging level can be set in the [Parameter Tree](#parameter-tree).\n\n## License\nCreative Commons Attribution-NonCommercial-ShareAlike 4.0 International Public License\n",
+    'long_description': "# Fringes-GUI\nAuthor: Christian Kludt\n\n## Description\nGraphical user interface for the [fringes](https://pypi.org/project/fringes/) package.\n\n## Installation\nYou can install `fringes-gui` directly from [PyPi](https://pypi.org/project/fringes-gui) via `pip`:\n\n```\npip install fringes-gui\n```\n\n## Usage\nYou import the `fringes-gui` package and call the function `run()`.\n\n```python\nimport fringes_gui as fgui\nfgui.run()\n```\n\nNow the graphical user interface should appear:\n\n![Screenshot](docs/GUI.png)\\\nScreenshot of the GUI.\n\n### Parameter Tree\nIn the top left corner the attribute widget is located.\nIt contains the parameter tree with which all the properties of the `Fringes` class\nfrom the [fringes](https://pypi.org/project/fringes/) package can be controlled.\nCheck out its website for more details.\nHowever, if you select a parameter and hover over it, a tool tip will appear\ncontaining the docstring of the respective property of the `Fringes` class.\n\nThe Visibility defines the type of user that should get access to the feature.\nIt does not affect the functionality of the features but is used by the GUI to\ndecide which features to display based on the current user level. The purpose\nis mainly to ensure that the GUI is not cluttered with information that is not\nintended at the current visibility level. The following criteria have been used\nfor the assignment of the recommended visibility:\n- Beginner:\\\n  Features that should be visible for all users via the GUI. This\n  is the default visibility. The number of features with 'Beginner' visibility\n  should be limited to all basic features so the GUI display is well-organized\n  and easy to use.\n- Expert:\\\n  Features that require a more in-depth knowledge of the system\n  functionality. This is the preferred visibility level for all advanced features.\n- Guru:\\\n  Advanced features that usually only people with a sound background in phase shifting can make good use of.\n- Experimental:\\\n  New features that have not been tested yet\n  and are likely to crash the system at some point.\n\n### Function Buttons\nIn the bottem left corner you will find buttons for the associated methods of the `Fringes` class.\nAlternatively, you can use the keyboard shortcuts which are displayed when you hover over the buttons.\nThe buttons are only active if the necessary data has been enoded, decoded or loaded.\n\n### Viewer\nIn the center resides the viewer.\nIf float data is to be displayed, `nan` is replaced by zeros.\n\n### Data\nIn the top right corner the data widget is located.\nIt lists the data which has been encoded, decoded or was loaded.\n\nIn order to keep the [Parameter Tree](#parameter-tree) consistent with the data,\nonce a parameter has changed, certain data will be removed\nand also certain [buttons](#function-buttons) will be deactivated.\nAs a consequence, if you load data - e.g. the acquired (deflected) fringe pattern sequence - \nthe first element of its videoshape has to match the parameter `Frames` in order to be able to decode it.\n\nTo display any datum listed in the table in the [Viewer](#viewer), simly select the name of it in the table.\n\nKlick the `Load` button to choose a data or parameter set to load.\nWith the `Save` button, all data including the parameter set are saved to the selected directory.\nUse the `Clear all` button to delete all data.\n\nPlease note: By default, the datum `fringes` is decoded.\nIf you want to decode a datum with a different name (e.g. one that you just loaded),\nselect its name in the table and klick `Set data (to be decoded)`.\n\n### Log\nThe logging of the `Fringes` class is displayed here.\nThe logging level can be set in the [Parameter Tree](#parameter-tree).\n\n## License\nCreative Commons Attribution-NonCommercial-ShareAlike 4.0 International Public License\n",
     'author': 'Christian Kludt',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/comimag/fringes-gui',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `fringes_gui-0.1.1/PKG-INFO` & `fringes_gui-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fringes-gui
-Version: 0.1.1
+Version: 0.1.2
 Summary: Graphical user interface for the 'fringes' package.
 Home-page: https://github.com/comimag/fringes-gui
 License: CC-BY-NC-SA-4.0
 Keywords: phase shifting,fringe analysis,fringe projection,deflectometry,computational imaging
 Author: Christian Kludt
 Requires-Python: >=3.10,<3.11
 Classifier: License :: Other/Proprietary License
@@ -56,32 +56,36 @@
 
 The Visibility defines the type of user that should get access to the feature.
 It does not affect the functionality of the features but is used by the GUI to
 decide which features to display based on the current user level. The purpose
 is mainly to ensure that the GUI is not cluttered with information that is not
 intended at the current visibility level. The following criteria have been used
 for the assignment of the recommended visibility:
-- Beginner: Features that should be visible for all users via the GUI. This
-is the default visibility. The number of features with 'Beginner' visibility
-should be limited to all basic features so the GUI display is well-organized
-and easy to use.
-- Expert: Features that require a more in-depth knowledge of the system
-functionality. This is the preferred visibility level for all advanced features.
-- Guru: Advanced features that usually only people with a sound background in phase shifting can make good use of.
-- Experimental: New features that have not been tested yet
-and the system might probably crash at some point.
+- Beginner:\
+  Features that should be visible for all users via the GUI. This
+  is the default visibility. The number of features with 'Beginner' visibility
+  should be limited to all basic features so the GUI display is well-organized
+  and easy to use.
+- Expert:\
+  Features that require a more in-depth knowledge of the system
+  functionality. This is the preferred visibility level for all advanced features.
+- Guru:\
+  Advanced features that usually only people with a sound background in phase shifting can make good use of.
+- Experimental:\
+  New features that have not been tested yet
+  and are likely to crash the system at some point.
 
 ### Function Buttons
 In the bottem left corner you will find buttons for the associated methods of the `Fringes` class.
 Alternatively, you can use the keyboard shortcuts which are displayed when you hover over the buttons.
 The buttons are only active if the necessary data has been enoded, decoded or loaded.
 
 ### Viewer
 In the center resides the viewer.
-If float data is to be displayed, nan is replaced by zeros.
+If float data is to be displayed, `nan` is replaced by zeros.
 
 ### Data
 In the top right corner the data widget is located.
 It lists the data which has been encoded, decoded or was loaded.
 
 In order to keep the [Parameter Tree](#parameter-tree) consistent with the data,
 once a parameter has changed, certain data will be removed
@@ -96,13 +100,13 @@
 Use the `Clear all` button to delete all data.
 
 Please note: By default, the datum `fringes` is decoded.
 If you want to decode a datum with a different name (e.g. one that you just loaded),
 select its name in the table and klick `Set data (to be decoded)`.
 
 ### Log
-Here the logging of the `Fringes` class is displayed.
+The logging of the `Fringes` class is displayed here.
 The logging level can be set in the [Parameter Tree](#parameter-tree).
 
 ## License
 Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International Public License
```

