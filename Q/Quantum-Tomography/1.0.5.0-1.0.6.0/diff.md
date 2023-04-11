# Comparing `tmp/Quantum-Tomography-1.0.5.0.tar.gz` & `tmp/Quantum-Tomography-1.0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Quantum-Tomography-1.0.5.0.tar", last modified: Mon Feb  6 18:33:45 2023, max compression
+gzip compressed data, was "Quantum-Tomography-1.0.6.0.tar", last modified: Tue Apr 11 23:54:10 2023, max compression
```

## Comparing `Quantum-Tomography-1.0.5.0.tar` & `Quantum-Tomography-1.0.6.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 18:33:45.325702 Quantum-Tomography-1.0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-02-06 18:27:41.000000 Quantum-Tomography-1.0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-06 18:27:41.000000 Quantum-Tomography-1.0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10491 2023-02-06 18:33:45.325702 Quantum-Tomography-1.0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-02-06 18:27:41.000000 Quantum-Tomography-1.0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-06 18:33:45.325702 Quantum-Tomography-1.0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-02-06 18:27:41.000000 Quantum-Tomography-1.0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 18:33:45.317702 Quantum-Tomography-1.0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 18:33:45.321702 Quantum-Tomography-1.0.5.0/src/QuantumTomography/
--rw-r--r--   0 runner    (1001) docker     (123)    75281 2023-02-06 18:27:41.000000 Quantum-Tomography-1.0.5.0/src/QuantumTomography/TomoClass.py
--rw-r--r--   0 runner    (1001) docker     (123)    19099 2023-02-06 18:27:41.000000 Quantum-Tomography-1.0.5.0/src/QuantumTomography/TomoClassHelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13268 2023-02-06 18:27:41.000000 Quantum-Tomography-1.0.5.0/src/QuantumTomography/TomoDisplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-02-06 18:27:41.000000 Quantum-Tomography-1.0.5.0/src/QuantumTomography/TomoDisplayHelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    19774 2023-02-06 18:27:41.000000 Quantum-Tomography-1.0.5.0/src/QuantumTomography/TomoFunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-02-06 18:27:41.000000 Quantum-Tomography-1.0.5.0/src/QuantumTomography/TomoFunctionsHelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-02-06 18:27:41.000000 Quantum-Tomography-1.0.5.0/src/QuantumTomography/Utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-02-06 18:27:41.000000 Quantum-Tomography-1.0.5.0/src/QuantumTomography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-02-06 18:27:41.000000 Quantum-Tomography-1.0.5.0/src/QuantumTomography/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 18:33:45.321702 Quantum-Tomography-1.0.5.0/src/Quantum_Tomography.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10491 2023-02-06 18:33:45.000000 Quantum-Tomography-1.0.5.0/src/Quantum_Tomography.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-02-06 18:33:45.000000 Quantum-Tomography-1.0.5.0/src/Quantum_Tomography.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 18:33:45.000000 Quantum-Tomography-1.0.5.0/src/Quantum_Tomography.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-06 18:33:45.000000 Quantum-Tomography-1.0.5.0/src/Quantum_Tomography.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-06 18:33:45.000000 Quantum-Tomography-1.0.5.0/src/Quantum_Tomography.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-06 18:33:45.000000 Quantum-Tomography-1.0.5.0/src/Quantum_Tomography.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:54:10.713207 Quantum-Tomography-1.0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-11 23:48:29.000000 Quantum-Tomography-1.0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 23:48:29.000000 Quantum-Tomography-1.0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10491 2023-04-11 23:54:10.713207 Quantum-Tomography-1.0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-04-11 23:48:29.000000 Quantum-Tomography-1.0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 23:54:10.713207 Quantum-Tomography-1.0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-11 23:48:29.000000 Quantum-Tomography-1.0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:54:10.709207 Quantum-Tomography-1.0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:54:10.713207 Quantum-Tomography-1.0.6.0/src/QuantumTomography/
+-rw-r--r--   0 runner    (1001) docker     (123)    75121 2023-04-11 23:48:29.000000 Quantum-Tomography-1.0.6.0/src/QuantumTomography/TomoClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19099 2023-04-11 23:48:29.000000 Quantum-Tomography-1.0.6.0/src/QuantumTomography/TomoClassHelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13268 2023-04-11 23:48:29.000000 Quantum-Tomography-1.0.6.0/src/QuantumTomography/TomoDisplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-11 23:48:29.000000 Quantum-Tomography-1.0.6.0/src/QuantumTomography/TomoDisplayHelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19774 2023-04-11 23:48:29.000000 Quantum-Tomography-1.0.6.0/src/QuantumTomography/TomoFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-11 23:48:29.000000 Quantum-Tomography-1.0.6.0/src/QuantumTomography/TomoFunctionsHelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-11 23:48:29.000000 Quantum-Tomography-1.0.6.0/src/QuantumTomography/Utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-11 23:48:29.000000 Quantum-Tomography-1.0.6.0/src/QuantumTomography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-04-11 23:48:29.000000 Quantum-Tomography-1.0.6.0/src/QuantumTomography/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:54:10.713207 Quantum-Tomography-1.0.6.0/src/Quantum_Tomography.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10491 2023-04-11 23:54:10.000000 Quantum-Tomography-1.0.6.0/src/Quantum_Tomography.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-11 23:54:10.000000 Quantum-Tomography-1.0.6.0/src/Quantum_Tomography.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 23:54:10.000000 Quantum-Tomography-1.0.6.0/src/Quantum_Tomography.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-11 23:54:10.000000 Quantum-Tomography-1.0.6.0/src/Quantum_Tomography.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 23:54:10.000000 Quantum-Tomography-1.0.6.0/src/Quantum_Tomography.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-11 23:54:10.000000 Quantum-Tomography-1.0.6.0/src/Quantum_Tomography.egg-info/top_level.txt
```

### Comparing `Quantum-Tomography-1.0.5.0/LICENSE` & `Quantum-Tomography-1.0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Quantum-Tomography-1.0.5.0/PKG-INFO` & `Quantum-Tomography-1.0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quantum-Tomography
-Version: 1.0.5.0
+Version: 1.0.6.0
 Summary: A python library to help perform tomography on a quantum state.
 Home-page: https://github.com/KwiatQIM/Quantum-Tomography
 Author: University of Illinois
 Author-email: turroscott@gmail.com
 License: MIT
 Project-URL: Documentation, https://quantumtomo.web.illinois.edu/Doc/
 Project-URL: Video Tutorial, https://www.youtube.com/watch?v=I-214P0LOfQ&list=PLJLHMKtk5Pqy9w9aCuyowUF1p7pl2JCI9&index=3
```

### Comparing `Quantum-Tomography-1.0.5.0/README.md` & `Quantum-Tomography-1.0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `Quantum-Tomography-1.0.5.0/setup.py` & `Quantum-Tomography-1.0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     with open('README.md') as f:
         README  = f.read()
     return README
 
 
 setup(
     name = "Quantum-Tomography",
-    version = "1.0.5.0",
+    version = "1.0.6.0",
     description = "A python library to help perform tomography on a quantum state.",
     long_description = readme(),
     long_description_content_type = "text/markdown",
     url = "https://github.com/KwiatQIM/Quantum-Tomography",
     author = "University of Illinois",
     author_email = "turroscott@gmail.com",
     license = "MIT",
```

### Comparing `Quantum-Tomography-1.0.5.0/src/QuantumTomography/TomoClass.py` & `Quantum-Tomography-1.0.6.0/src/QuantumTomography/TomoClass.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,15 @@
         Each row in the matrix is a set of independent measurements.
     crosstalk : ndarray shape = ( Number of measurements , 2**NQubits,2**NQubits ) (optional)
         The crosstalk matrix to compensate for inefficentcies in your beam splitter.
     efficiency : 1darray with length = NQubits*NDetectors (optional)
         The relative efficienies between your detector pairs.
     time :  1darray with length = Number of measurements (optional)
         The total duration of each measurment.
-    singles : ndarray shape = ( Number of measurements , 2*NQubits ) (optional)
+    singles : ndarray shape = ( Number of measurements , NDetectors*NQubits ) (optional)
         The singles counts on each detector.
     window : 1darray with length = NQubits*NDetectors (optional)
         The coincidence window duration for each detector pair.
     error : int (optional)
         The number of monte carlo states used to estimate the properties of the state.
     intensities : 1darray with length = Number of measurements (optional)
         The relative intensity of each measurement. Used for drift correction.
@@ -223,15 +223,15 @@
     """
     StateTomography_Matrix(tomo_input, intensities)
     Desc: Main function that runs tomography.
 
     Parameters
     ----------
     tomo_input : ndarray
-        The input data for the current tomography. Example can be seen at top of page.
+        The input data for the current tomography.
     intensities : 1darray with length = number of measurements (optional)
         Relative pump power (arb. units) during measurement; used for drift correction. Default will be an array of ones
     method : ['MLE','HMLE','BME','LINER'] (optional)
             Which method to use to run tomography. Default is MLE
 
     Returns
     -------
@@ -765,15 +765,15 @@
     """
     filter_data(tomo_input)
     Desc: Filters the data into separate arrays.
 
     Parameters
     ----------
     tomo_input : ndarray
-        The input data for the current tomography. Example can be seen at top of page.
+        The input data for the current tomography.
 
     Returns
     -------
     coincidences : ndarray shape = (Number of measurements, NDetectors**NQubits)
         The counts of the tomography.
     measurements_densities : ndarray with shape = (NDetectors*number of measurements,2^numQubits, 2^numQubits) 
         The measurements of the tomography in density matrix form.
@@ -976,15 +976,15 @@
                 self.conf['Window'] = window
             elif (len(window.shape) == 1 and window.shape[0] == self.getNumCoinc()):
                 self.conf['Window'] = window
             else:
                 raise ValueError("Invalid window array")
         else:
             time = np.ones(measurements.shape[0])
-            singles = np.zeros((measurements.shape[0],self.conf["NQubits"]))
+            singles = np.zeros((measurements.shape[0],self.getNumSingles()))
             self.conf['Window'] = window
 
 
         #############
         # crosstalk #
         #############
         if (isinstance(crosstalk, int)):
@@ -1021,15 +1021,14 @@
             # singles
             tomo_input[:, 1: 2 * n_qubit + 1] = singles
             # counts
             tomo_input[:, 2 * n_qubit + 1: 2 ** n_qubit + 2 * n_qubit + 1] = counts
             # measurements
             tomo_input[:, 2 ** n_qubit + 2 * n_qubit + 1: 2 ** n_qubit + 4 * n_qubit + 1] = measurements
 
-
         return tomo_input
 
     """
     checkForInvalidSettings()
     desc : Checks the current settings and throws errors if any are invalid.
     """
     def checkForInvalidSettings(self):
@@ -1047,15 +1046,15 @@
                 raise ValueError('Invalid Conf settings. Window should have length ' +str(self.getNumCoinc()) + " with the given settings.")
         # Efficicieny and Ndetectors
         if not self.conf['NDetectors'] in [1,2]:
             raise ValueError('Invalid Conf settings. NDetectors can be either 1 or 2, corresponding to the number of detectors per qubit.')
         elif self.conf['NDetectors'] == 2:
             try:
                 eff = np.array(self.conf['Efficiency'],dtype=float)
-                if isinstance(eff,int):
+                if isinstance(self.conf['Efficiency'],int):
                     eff = np.ones(self.getNumCoinc())
                 if len(eff.shape) != 1 or len(eff) != self.getNumCoinc():
                     raise
             except:
                 raise ValueError('Invalid Conf settings. Efficiency should have length ' +str(self.getNumCoinc()) + " with the given settings.")
         elif self.conf['NDetectors'] == 1:
             eff = np.ones(1)
@@ -1145,18 +1144,15 @@
             return 1
 
     """
     getNumSingles()
     Desc: Returns the number of singles per measurement for the current configurations.
     """
     def getNumSingles(self):
-        if (self.conf['NDetectors'] == 2):
-            return 2 * self.conf['NQubits']
-        else:
-            return self.conf['NQubits']
+        return self.conf['NDetectors']*self.conf['NQubits']
 
     """
     getNumDetPerQubit()
     Desc: returns the number of detectors per qubit for the current configurations.
     """
     def getNumDetPerQubit(self):
         return self.conf['NDetectors']
@@ -1219,15 +1215,15 @@
         number of qubits you want for each measurement. Default will use the number of qubits in the current configurations.
     numDet : 1 or 2
         Number of detectors for each measurement Default will use the number of qubits in the current configurations.   
 
     Returns
     -------
     Tomoinput : ndarray
-        The input data for the current tomography.Example can be seen at top of page.
+        The input data for the current tomography.
     """
     def getTomoInputTemplate(self, numBits = -1,numDet = -1):
         # check if numBits is an int
         if not (isinstance(numBits, int)):
             raise ValueError("numBits must be an integer")
         if (numBits < 1):
             numBits = self.getNumQubits()
```

### Comparing `Quantum-Tomography-1.0.5.0/src/QuantumTomography/TomoClassHelpers.py` & `Quantum-Tomography-1.0.6.0/src/QuantumTomography/TomoClassHelpers.py`

 * *Files identical despite different names*

### Comparing `Quantum-Tomography-1.0.5.0/src/QuantumTomography/TomoDisplay.py` & `Quantum-Tomography-1.0.6.0/src/QuantumTomography/TomoDisplay.py`

 * *Files identical despite different names*

### Comparing `Quantum-Tomography-1.0.5.0/src/QuantumTomography/TomoDisplayHelpers.py` & `Quantum-Tomography-1.0.6.0/src/QuantumTomography/TomoDisplayHelpers.py`

 * *Files identical despite different names*

### Comparing `Quantum-Tomography-1.0.5.0/src/QuantumTomography/TomoFunctions.py` & `Quantum-Tomography-1.0.6.0/src/QuantumTomography/TomoFunctions.py`

 * *Files identical despite different names*

### Comparing `Quantum-Tomography-1.0.5.0/src/QuantumTomography/TomoFunctionsHelpers.py` & `Quantum-Tomography-1.0.6.0/src/QuantumTomography/TomoFunctionsHelpers.py`

 * *Files identical despite different names*

### Comparing `Quantum-Tomography-1.0.5.0/src/QuantumTomography/Utilities.py` & `Quantum-Tomography-1.0.6.0/src/QuantumTomography/Utilities.py`

 * *Files identical despite different names*

### Comparing `Quantum-Tomography-1.0.5.0/src/QuantumTomography/__init__.py` & `Quantum-Tomography-1.0.6.0/src/QuantumTomography/__init__.py`

 * *Files identical despite different names*

### Comparing `Quantum-Tomography-1.0.5.0/src/QuantumTomography/cli.py` & `Quantum-Tomography-1.0.6.0/src/QuantumTomography/cli.py`

 * *Files identical despite different names*

### Comparing `Quantum-Tomography-1.0.5.0/src/Quantum_Tomography.egg-info/PKG-INFO` & `Quantum-Tomography-1.0.6.0/src/Quantum_Tomography.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quantum-Tomography
-Version: 1.0.5.0
+Version: 1.0.6.0
 Summary: A python library to help perform tomography on a quantum state.
 Home-page: https://github.com/KwiatQIM/Quantum-Tomography
 Author: University of Illinois
 Author-email: turroscott@gmail.com
 License: MIT
 Project-URL: Documentation, https://quantumtomo.web.illinois.edu/Doc/
 Project-URL: Video Tutorial, https://www.youtube.com/watch?v=I-214P0LOfQ&list=PLJLHMKtk5Pqy9w9aCuyowUF1p7pl2JCI9&index=3
```

### Comparing `Quantum-Tomography-1.0.5.0/src/Quantum_Tomography.egg-info/SOURCES.txt` & `Quantum-Tomography-1.0.6.0/src/Quantum_Tomography.egg-info/SOURCES.txt`

 * *Files identical despite different names*

