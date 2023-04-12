# Comparing `tmp/qudi_hira_analysis-1.3.5.tar.gz` & `tmp/qudi_hira_analysis-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qudi_hira_analysis-1.3.5.tar", max compression
+gzip compressed data, was "qudi_hira_analysis-1.4.0.tar", max compression
```

## Comparing `qudi_hira_analysis-1.3.5.tar` & `qudi_hira_analysis-1.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1069 2023-02-26 15:52:31.954729 qudi_hira_analysis-1.3.5/LICENSE
--rw-r--r--   0        0        0     9531 2023-04-12 17:44:20.350633 qudi_hira_analysis-1.3.5/README.md
--rw-r--r--   0        0        0      868 2023-04-12 17:54:57.241605 qudi_hira_analysis-1.3.5/pyproject.toml
--rw-r--r--   0        0        0      171 2023-03-05 21:19:20.709702 qudi_hira_analysis-1.3.5/qudi_hira_analysis/__init__.py
--rw-r--r--   0        0        0    10745 2023-03-05 21:19:20.709832 qudi_hira_analysis-1.3.5/qudi_hira_analysis/analysis_logic.py
--rw-r--r--   0        0        0    13322 2023-03-09 12:03:13.046866 qudi_hira_analysis-1.3.5/qudi_hira_analysis/data_handler.py
--rw-r--r--   0        0        0        0 2023-03-05 21:19:20.710018 qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/__init__.py
--rw-r--r--   0        0        0     1936 2023-03-05 21:19:20.710848 qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/antibunchingmethods.py
--rw-r--r--   0        0        0    24480 2023-03-05 21:19:20.711380 qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/decaylikemethods.py
--rw-r--r--   0        0        0    40854 2023-03-05 21:19:20.711692 qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/gaussianlikemethods.py
--rw-r--r--   0        0        0    23150 2023-03-05 21:19:20.711989 qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/generalmethods.py
--rw-r--r--   0        0        0     5848 2023-03-05 21:19:20.712252 qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/hyperbolicsaturationmethods.py
--rw-r--r--   0        0        0    10577 2023-03-05 21:19:20.712412 qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/linearmethods.py
--rw-r--r--   0        0        0    41457 2023-03-05 21:19:20.712635 qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/lorentzianlikemethods.py
--rw-r--r--   0        0        0    16450 2023-03-05 21:19:20.712885 qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/poissonianlikemethods.py
--rw-r--r--   0        0        0   106110 2023-03-05 21:19:20.713199 qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/sinemethods.py
--rw-r--r--   0        0        0     1792 2023-04-12 17:43:42.063526 qudi_hira_analysis-1.3.5/qudi_hira_analysis/helper_functions.py
--rw-r--r--   0        0        0    12696 2023-04-12 17:43:42.063710 qudi_hira_analysis-1.3.5/qudi_hira_analysis/io_handler.py
--rw-r--r--   0        0        0     6758 2023-04-12 17:43:42.063880 qudi_hira_analysis-1.3.5/qudi_hira_analysis/measurement_dataclass.py
--rw-r--r--   0        0        0    18729 2023-03-05 21:19:20.714069 qudi_hira_analysis-1.3.5/qudi_hira_analysis/qudi_fit_logic.py
--rw-r--r--   0        0        0    10529 1970-01-01 00:00:00.000000 qudi_hira_analysis-1.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-02-26 15:52:31.954729 qudi_hira_analysis-1.4.0/LICENSE
+-rw-r--r--   0        0        0    10431 2023-04-12 19:37:13.223794 qudi_hira_analysis-1.4.0/README.md
+-rw-r--r--   0        0        0      868 2023-04-12 19:39:36.964668 qudi_hira_analysis-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      171 2023-03-05 21:19:20.709702 qudi_hira_analysis-1.4.0/qudi_hira_analysis/__init__.py
+-rw-r--r--   0        0        0    11044 2023-04-12 19:03:20.871413 qudi_hira_analysis-1.4.0/qudi_hira_analysis/analysis_logic.py
+-rw-r--r--   0        0        0    13112 2023-04-12 19:28:24.073699 qudi_hira_analysis-1.4.0/qudi_hira_analysis/data_handler.py
+-rw-r--r--   0        0        0        0 2023-03-05 21:19:20.710018 qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/__init__.py
+-rw-r--r--   0        0        0     1936 2023-03-05 21:19:20.710848 qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/antibunchingmethods.py
+-rw-r--r--   0        0        0    24480 2023-03-05 21:19:20.711380 qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/decaylikemethods.py
+-rw-r--r--   0        0        0    40854 2023-03-05 21:19:20.711692 qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/gaussianlikemethods.py
+-rw-r--r--   0        0        0    23150 2023-03-05 21:19:20.711989 qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/generalmethods.py
+-rw-r--r--   0        0        0     5848 2023-03-05 21:19:20.712252 qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/hyperbolicsaturationmethods.py
+-rw-r--r--   0        0        0    10577 2023-03-05 21:19:20.712412 qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/linearmethods.py
+-rw-r--r--   0        0        0    41457 2023-03-05 21:19:20.712635 qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/lorentzianlikemethods.py
+-rw-r--r--   0        0        0    16450 2023-03-05 21:19:20.712885 qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/poissonianlikemethods.py
+-rw-r--r--   0        0        0   106110 2023-03-05 21:19:20.713199 qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/sinemethods.py
+-rw-r--r--   0        0        0     1792 2023-04-12 17:43:42.063526 qudi_hira_analysis-1.4.0/qudi_hira_analysis/helper_functions.py
+-rw-r--r--   0        0        0    12696 2023-04-12 17:43:42.063710 qudi_hira_analysis-1.4.0/qudi_hira_analysis/io_handler.py
+-rw-r--r--   0        0        0     6758 2023-04-12 17:43:42.063880 qudi_hira_analysis-1.4.0/qudi_hira_analysis/measurement_dataclass.py
+-rw-r--r--   0        0        0    18729 2023-03-05 21:19:20.714069 qudi_hira_analysis-1.4.0/qudi_hira_analysis/qudi_fit_logic.py
+-rw-r--r--   0        0        0    11429 1970-01-01 00:00:00.000000 qudi_hira_analysis-1.4.0/PKG-INFO
```

### Comparing `qudi_hira_analysis-1.3.5/LICENSE` & `qudi_hira_analysis-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.3.5/README.md` & `qudi_hira_analysis-1.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -134,70 +134,91 @@
 ├── Sample_MW_Pin_comparision.png
 ├── Tip_MW_Pin_comparision.png
 └── Tip_Sample_MW_Pin_comparision.png
 ```
 
 ### Automated data extraction
 
-#### Example 1: Extract, fit and plot all Rabi measurements
+First set up the `DataHandler` object with the correct paths to the data and figure folders.
 
 ```python
 from pathlib import Path
 import matplotlib.pyplot as plt
 import seaborn as sns
 
 from qudi_hira_analysis import DataHandler
 
-nv1 = DataHandler(
-  data_folder=Path("C:\\", "Data"),
+data = DataHandler(
+  data_folder=Path("C:\\", "Data"), 
   figure_folder=Path("C:\\", "QudiHiraAnalysis"),
   measurement_folder=Path("20230101_NV1")
 )
+```
+
+#### Example 1: Extract autocorrelation measurements, fit and save
+
+```python
+autocorrelation_measurements = data.load_measurements(measurement_str="Autocorrelation")
+
+fig, ax = plt.subplots()
 
-rabi_measurements = nv1.load_measurements(measurement_str="rabi", qudi=True, pulsed=True)
+for autocorrelation in autocorrelation_measurements.values():
+  sns.lineplot(data=autocorrelation.data, x="Controlled variable(s)", y="g2(t)", ax=ax)
+  fit_x, fit_y, result = data.fit(
+    x="Controlled variable(s)", y="g2(t)", data=autocorrelation.data, fit_function=data.fit_function.antibunching
+  )
+  sns.lineplot(x=fit_x, y=fit_y, ax=ax)
+  
+data.save_figures(filepath="autocorrelation_variation", fig=fig)
+```
+
+#### Example 2: Extract ODMR measurements, fit and save
+
+```python
+odmr_measurements = data.load_measurements(measurement_str="ODMR", pulsed=True)
 
 fig, ax = plt.subplots()
 
-for rabi in rabi_measurements:
-  sns.lineplot(data=rabi.data, x="Controlled variable(s)", y="Signal", ax=ax)
-  fit_x, fit_y, result = rabi.analysis.fit(
-    x="Controlled variable(s)", y="Signal",
-    data=rabi.data,
-    fit_function=rabi_measurements.sineexponentialdecay
+for odmr in odmr_measurements.values():
+  sns.scatterplot(data=odmr.data, x="Controlled variable(Hz)", y="Signal", ax=ax)
+  fit_x, fit_y, result = data.fit(
+    x="Controlled variable(Hz)", y="Signal", data=odmr.data, fit_function=data.fit_function.lorentzian_double
   )
   sns.lineplot(x=fit_x, y=fit_y, ax=ax)
 
-nv1.save_figures(filepath="rabi_variation", fig=fig)
+data.save_figures(filepath="odmr_variation", fig=fig)
 ```
 
-#### Example 2: Combine all temperature data, plot and save
+#### Example 3: Extract Rabi measurements, fit and save
 
 ```python
-from pathlib import Path
+rabi_measurements = data.load_measurements(measurement_str="Rabi", pulsed=True)
 
-import matplotlib.pyplot as plt
-import pandas as pd
-import seaborn as sns
+fig, ax = plt.subplots()
 
-from qudi_hira_analysis import DataHandler
+for rabi in rabi_measurements.values():
+  sns.scatterplot(data=rabi.data, x="Controlled variable(s)", y="Signal", ax=ax)
+  fit_x, fit_y, result = data.fit(
+    x="Controlled variable(s)", y="Signal", data=rabi.data, fit_function=data.fit_function.sineexponentialdecay
+  )
+  sns.lineplot(x=fit_x, y=fit_y, ax=ax)
 
-nv1 = DataHandler(
-  data_folder=Path("C:\\", "Data"),
-  figure_folder=Path("C:\\", "QudiHiraAnalysis"),
-  measurement_folder=Path("20230101_NV1"),
-  copy_measurement_folder_structure=False
-)
+data.save_figures(filepath="rabi_variation", fig=fig)
+```
+
+#### Example 4: Extract all temperature data, plot and save
 
-temperature_measurements = nv1.load_measurements(measurement_str="temperature-monitoring")
+```python
+temperature_measurements = data.load_measurements(measurement_str="Temperature")
 
 dft = pd.concat([t.data for t in temperature_measurements.values()])
 
 fig, ax = plt.subplots()
 sns.lineplot(data=dft, x="Time", y="Temperature", ax=ax)
-nv1.save_figures(filepath="temperature-monitoring", fig=fig)
+data.save_figures(filepath="temperature_monitoring", fig=fig)
 ```
 
 ## Build
 
 ### Prerequisites
 
 Latest version of:
```

### Comparing `qudi_hira_analysis-1.3.5/pyproject.toml` & `qudi_hira_analysis-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qudi-hira-analysis"
-version = "1.3.5"
+version = "1.4.0"
 repository = "https://github.com/dineshpinto/qudi-hira-analysis"
 homepage = "https://github.com/dineshpinto/qudi-hira-analysis"
 keywords = ["python", "qubit", "analysis", "nv centers", "photon timetrace"]
 description = "A Python toolkit to analzye photon timetrace data from qubit sensors"
 authors = ["dineshpinto <annual.fallout_0z@icloud.com>"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `qudi_hira_analysis-1.3.5/qudi_hira_analysis/analysis_logic.py` & `qudi_hira_analysis-1.4.0/qudi_hira_analysis/analysis_logic.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,62 @@
 from __future__ import annotations
 
 import logging
-from enum import Enum
 from typing import Tuple, TYPE_CHECKING
 
 import numpy as np
 import pandas as pd
 
 from qudi_hira_analysis.qudi_fit_logic import FitLogic
 
 if TYPE_CHECKING:
     from lmfit.model import ModelResult
 
 logging.basicConfig(format='%(name)s :: %(levelname)s :: %(message)s', level=logging.INFO)
 
 
-class FitMethods(Enum):
-    decayexponential: str = "decayexponential"
-    biexponential: str = "biexponential"
-    decayexponentialstretched: str = "decayexponentialstretched"
-    gaussian: str = "gaussian"
-    gaussiandouble: str = "gaussiandouble"
-    gaussianlinearoffset: str = "gaussianlinearoffset"
-    hyperbolicsaturation: str = "hyperbolicsaturation"
-    linear: str = "linear"
-    lorentzian: str = "lorentzian"
-    lorentziandouble: str = "lorentziandouble"
-    lorentziantriple: str = "lorentziantriple"
-    sine: str = "sine"
-    sinedouble: str = "sinedouble"
-    sinedoublewithexpdecay: str = "sinedoublewithexpdecay"
-    sinedoublewithtwoexpdecay: str = "sinedoublewithtwoexpdecay"
-    sineexponentialdecay: str = "sineexponentialdecay"
-    sinestretchedexponentialdecay: str = "sinestretchedexponentialdecay"
-    sinetriple: str = "sinetriple"
-    sinetriplewithexpdecay: str = "sinetriplewithexpdecay"
-    sinetriplewiththreeexpdecay: str = "sinetriplewiththreeexpdecay"
-    twoDgaussian: str = "twoDgaussian"
-    antibunching: str = "antibunching"
+class FitMethodsAndEstimators:
+    # Fit methods with corresponding estimators
+    antibunching: tuple = ("antibunching", "dip")
+    hyperbolicsaturation: tuple = ("hyperbolicsaturation", "generic")
+    lorentzian: tuple = ("lorentzian", "dip")
+    lorentziandouble: tuple = ("lorentziandouble", "N15")
+    sineexponentialdecay: tuple = ("sineexponentialdecay", "generic")
+    decayexponential: tuple = ("decayexponential", "generic")
+    gaussian: tuple = ("gaussian", "dip")
+    gaussiandouble: tuple = ("gaussiandouble", "dip")
+    gaussianlinearoffset: tuple = ("gaussianlinearoffset", "dip")
+    lorentziantriple: tuple = ("lorentziantriple", "N14")
+    biexponential: tuple = ("biexponential", "generic")
+    decayexponentialstretched: tuple = ("decayexponentialstretched", "generic")
+    linear: tuple = ("linear", "generic")
+    sine: tuple = ("sine", "generic")
+    sinedouble: tuple = ("sinedouble", "generic")
+    sinedoublewithexpdecay: tuple = ("sinedoublewithexpdecay", "generic")
+    sinedoublewithtwoexpdecay: tuple = ("sinedoublewithtwoexpdecay", "generic")
+    sinestretchedexponentialdecay: tuple = ("sinestretchedexponentialdecay", "generic")
+    sinetriple: tuple = ("sinetriple", "generic")
+    sinetriplewithexpdecay: tuple = ("sinetriplewithexpdecay", "generic")
+    sinetriplewiththreeexpdecay: tuple = ("sinetriplewiththreeexpdecay", "generic")
+    twoDgaussian: tuple = ("twoDgaussian", "generic")
 
 
 class AnalysisLogic(FitLogic):
+    fit_function = FitMethodsAndEstimators
+
     def __init__(self):
         super().__init__()
         self.log = logging.getLogger(__name__)
-        self.fit_methods = FitMethods
 
     def perform_fit(
             self,
             x: pd.Series,
             y: pd.Series,
-            fit_function: str | FitMethods,
-            estimator: str = "generic",
+            fit_function: str,
+            estimator: str,
             dims: str = "1d") -> Tuple[np.ndarray, np.ndarray, ModelResult]:
         """
         Fits available:
             | Dimension | Fit                           |
             |-----------|-------------------------------|
             | 1d        | decayexponential              |
             |           | biexponential                 |
@@ -83,16 +84,14 @@
             - dip
         """
 
         if isinstance(x, pd.Series) or isinstance(x, pd.Index):
             x = x.to_numpy()
         if isinstance(y, pd.Series):
             y = y.to_numpy()
-        if isinstance(fit_function, FitMethods):
-            fit_function = fit_function.name
 
         fit = {dims: {'default': {'fit_function': fit_function, 'estimator': estimator}}}
         user_fit = self.validate_load_fits(fit)
 
         use_settings = {}
         for key in user_fit[dims]["default"]["parameters"].keys():
             use_settings[key] = False
@@ -106,23 +105,27 @@
         return fit_x, fit_y, result
 
     def fit(
             self,
             x: str,
             y: str,
             data: pd.DataFrame,
-            fit_function: str | FitMethods,
-            estimator: str = "generic",
+            fit_function: FitMethodsAndEstimators,
     ) -> Tuple[np.ndarray, np.ndarray, ModelResult]:
+        if "twoD" in fit_function[0]:
+            dims = "2d"
+        else:
+            dims = "1d"
+
         return self.perform_fit(
             x=data[x],
             y=data[y],
-            fit_function=fit_function,
-            estimator=estimator,
-            dims="1d"
+            fit_function=fit_function[0],
+            estimator=fit_function[1],
+            dims=dims
         )
 
     def get_all_fits(self) -> Tuple[list, list]:
         one_d_fits = list(self.fit_list['1d'].keys())
         two_d_fits = list(self.fit_list['2d'].keys())
         self.log.info(f"1d fits: {one_d_fits}\n2d fits: {two_d_fits}")
         return one_d_fits, two_d_fits
```

### Comparing `qudi_hira_analysis-1.3.5/qudi_hira_analysis/data_handler.py` & `qudi_hira_analysis-1.4.0/qudi_hira_analysis/data_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         )
         self.pressure_loader: (Callable[[Path], pd.DataFrame], None) = (
             self.read_pfeiffer_data,
             None
         )
 
 
-class DataHandler(DataLoader):
+class DataHandler(DataLoader, AnalysisLogic):
     """
     Handles automated data searching and extraction into dataclasses.
 
     Parameters
     ----------
         data_folder: pathlib.Path
             Path to the data folder.
@@ -75,32 +75,29 @@
 
     Examples
     --------
     Create an instance of the DataHandler class:
 
     Set up the source data folder, the figure folder and the measurement folder.
 
-    >>> from pathlib import Path
-    >>> from qudi_hira_analysis import DataHandler
-    >>> bakeout_handler = DataHandler(
+    >>> data = DataHandler(
     >>>     data_folder=Path('C:\\'', 'Data'),
     >>>     figure_folder=Path('C:\\'', 'QudiHiraAnalysis'),
     >>>     measurement_folder=Path('20230101_Bakeout'),
     >>> )
     """
 
     def __init__(
             self,
             data_folder: Path,
             figure_folder: Path,
             measurement_folder: Path,
             copy_measurement_folder_structure: bool = True
     ):
         self.log = logging.getLogger(__name__)
-        self.analysis = AnalysisLogic()
 
         self.data_folder_path = self.__get_data_folder_path(data_folder, measurement_folder)
         if copy_measurement_folder_structure:
             self.figure_folder_path = self.__get_figure_folder_path(figure_folder, measurement_folder)
         else:
             self.figure_folder_path = figure_folder
 
@@ -289,15 +286,15 @@
                 )
             )
         return measurement_list
 
     def load_measurements(
             self,
             measurement_str: str,
-            qudi: bool = False,
+            qudi: bool = True,
             pulsed: bool = False,
             extension: str = ".dat"
     ) -> dict[str: MeasurementDataclass]:
         """
         Lazy load all measurements of a given type into a dictionary of dataclasses.
 
         Parameters
@@ -319,29 +316,31 @@
         Returns
         -------
             measurement_list: dict[str: MeasurementDataclass]
                 A dictionary of dataclasses containing the measurement data.
 
         Examples
         --------
-        Load all T1 measurements measured using qudi:
+        `data` is an instance of the `DataHandler` class.
 
-        >>> handler.load_measurements(measurement_str="t1", qudi=True, pulsed=True)
+        Load all T1 measurements:
 
-        Load all confocal data measured using qudi:
+        >>> data.load_measurements(measurement_str="ODMR", qudi=True, pulsed=True)
 
-        >>> handler.load_measurements(measurement_str="confocal", qudi=True)
+        Load all confocal data:
 
-        Load all temperature monitoring data measured using a Lakeshore monitor:
+        >>> data.load_measurements(measurement_str="Confocal", qudi=True)
 
-        >>> handler.load_measurements(measurement_str="temperature-monitoring", extension=".xls")
+        Load all temperature monitoring data:
 
-        Load all pressure monitoring data measured using a Pfeiffer monitor:
+        >>> data.load_measurements(measurement_str="Temperature", extension=".xls")
 
-        >>> handler.load_measurements(measurement_str="pressure-monitoring", extension=".txt")
+        Load all pressure monitoring data:
+
+        >>> data.load_measurements(measurement_str="Pressure", qudi=True)
         """
 
         measurement_str = measurement_str.lower()
         if qudi:
             return self.__load_qudi_measurements_into_dataclass(measurement_str, pulsed=pulsed, extension=".dat")
         else:
             return self.__load_standard_measurements_into_dataclass(measurement_str, extension=extension)
```

### Comparing `qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/antibunchingmethods.py` & `qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/antibunchingmethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/decaylikemethods.py` & `qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/decaylikemethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/gaussianlikemethods.py` & `qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/gaussianlikemethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/generalmethods.py` & `qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/generalmethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/hyperbolicsaturationmethods.py` & `qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/hyperbolicsaturationmethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/linearmethods.py` & `qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/linearmethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/lorentzianlikemethods.py` & `qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/lorentzianlikemethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/poissonianlikemethods.py` & `qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/poissonianlikemethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.3.5/qudi_hira_analysis/fitmethods/sinemethods.py` & `qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/sinemethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.3.5/qudi_hira_analysis/helper_functions.py` & `qudi_hira_analysis-1.4.0/qudi_hira_analysis/helper_functions.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.3.5/qudi_hira_analysis/io_handler.py` & `qudi_hira_analysis-1.4.0/qudi_hira_analysis/io_handler.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.3.5/qudi_hira_analysis/measurement_dataclass.py` & `qudi_hira_analysis-1.4.0/qudi_hira_analysis/measurement_dataclass.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.3.5/qudi_hira_analysis/qudi_fit_logic.py` & `qudi_hira_analysis-1.4.0/qudi_hira_analysis/qudi_fit_logic.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.3.5/PKG-INFO` & `qudi_hira_analysis-1.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qudi-hira-analysis
-Version: 1.3.5
+Version: 1.4.0
 Summary: A Python toolkit to analzye photon timetrace data from qubit sensors
 Home-page: https://github.com/dineshpinto/qudi-hira-analysis
 License: MIT
 Keywords: python,qubit,analysis,nv centers,photon timetrace
 Author: dineshpinto
 Author-email: annual.fallout_0z@icloud.com
 Requires-Python: >=3.10,<4.0
@@ -159,70 +159,91 @@
 ├── Sample_MW_Pin_comparision.png
 ├── Tip_MW_Pin_comparision.png
 └── Tip_Sample_MW_Pin_comparision.png
 ```
 
 ### Automated data extraction
 
-#### Example 1: Extract, fit and plot all Rabi measurements
+First set up the `DataHandler` object with the correct paths to the data and figure folders.
 
 ```python
 from pathlib import Path
 import matplotlib.pyplot as plt
 import seaborn as sns
 
 from qudi_hira_analysis import DataHandler
 
-nv1 = DataHandler(
-  data_folder=Path("C:\\", "Data"),
+data = DataHandler(
+  data_folder=Path("C:\\", "Data"), 
   figure_folder=Path("C:\\", "QudiHiraAnalysis"),
   measurement_folder=Path("20230101_NV1")
 )
+```
+
+#### Example 1: Extract autocorrelation measurements, fit and save
+
+```python
+autocorrelation_measurements = data.load_measurements(measurement_str="Autocorrelation")
+
+fig, ax = plt.subplots()
 
-rabi_measurements = nv1.load_measurements(measurement_str="rabi", qudi=True, pulsed=True)
+for autocorrelation in autocorrelation_measurements.values():
+  sns.lineplot(data=autocorrelation.data, x="Controlled variable(s)", y="g2(t)", ax=ax)
+  fit_x, fit_y, result = data.fit(
+    x="Controlled variable(s)", y="g2(t)", data=autocorrelation.data, fit_function=data.fit_function.antibunching
+  )
+  sns.lineplot(x=fit_x, y=fit_y, ax=ax)
+  
+data.save_figures(filepath="autocorrelation_variation", fig=fig)
+```
+
+#### Example 2: Extract ODMR measurements, fit and save
+
+```python
+odmr_measurements = data.load_measurements(measurement_str="ODMR", pulsed=True)
 
 fig, ax = plt.subplots()
 
-for rabi in rabi_measurements:
-  sns.lineplot(data=rabi.data, x="Controlled variable(s)", y="Signal", ax=ax)
-  fit_x, fit_y, result = rabi.analysis.fit(
-    x="Controlled variable(s)", y="Signal",
-    data=rabi.data,
-    fit_function=rabi_measurements.sineexponentialdecay
+for odmr in odmr_measurements.values():
+  sns.scatterplot(data=odmr.data, x="Controlled variable(Hz)", y="Signal", ax=ax)
+  fit_x, fit_y, result = data.fit(
+    x="Controlled variable(Hz)", y="Signal", data=odmr.data, fit_function=data.fit_function.lorentzian_double
   )
   sns.lineplot(x=fit_x, y=fit_y, ax=ax)
 
-nv1.save_figures(filepath="rabi_variation", fig=fig)
+data.save_figures(filepath="odmr_variation", fig=fig)
 ```
 
-#### Example 2: Combine all temperature data, plot and save
+#### Example 3: Extract Rabi measurements, fit and save
 
 ```python
-from pathlib import Path
+rabi_measurements = data.load_measurements(measurement_str="Rabi", pulsed=True)
 
-import matplotlib.pyplot as plt
-import pandas as pd
-import seaborn as sns
+fig, ax = plt.subplots()
 
-from qudi_hira_analysis import DataHandler
+for rabi in rabi_measurements.values():
+  sns.scatterplot(data=rabi.data, x="Controlled variable(s)", y="Signal", ax=ax)
+  fit_x, fit_y, result = data.fit(
+    x="Controlled variable(s)", y="Signal", data=rabi.data, fit_function=data.fit_function.sineexponentialdecay
+  )
+  sns.lineplot(x=fit_x, y=fit_y, ax=ax)
 
-nv1 = DataHandler(
-  data_folder=Path("C:\\", "Data"),
-  figure_folder=Path("C:\\", "QudiHiraAnalysis"),
-  measurement_folder=Path("20230101_NV1"),
-  copy_measurement_folder_structure=False
-)
+data.save_figures(filepath="rabi_variation", fig=fig)
+```
+
+#### Example 4: Extract all temperature data, plot and save
 
-temperature_measurements = nv1.load_measurements(measurement_str="temperature-monitoring")
+```python
+temperature_measurements = data.load_measurements(measurement_str="Temperature")
 
 dft = pd.concat([t.data for t in temperature_measurements.values()])
 
 fig, ax = plt.subplots()
 sns.lineplot(data=dft, x="Time", y="Temperature", ax=ax)
-nv1.save_figures(filepath="temperature-monitoring", fig=fig)
+data.save_figures(filepath="temperature_monitoring", fig=fig)
 ```
 
 ## Build
 
 ### Prerequisites
 
 Latest version of:
```

