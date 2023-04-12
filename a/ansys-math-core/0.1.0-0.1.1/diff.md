# Comparing `tmp/ansys-math-core-0.1.0.tar.gz` & `tmp/ansys-math-core-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-math-core-0.1.0.tar", last modified: Wed Mar 22 09:05:10 2023, max compression
+gzip compressed data, was "ansys-math-core-0.1.1.tar", last modified: Wed Apr 12 13:16:23 2023, max compression
```

## Comparing `ansys-math-core-0.1.0.tar` & `ansys-math-core-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1089 2023-03-22 09:04:53.154039 ansys-math-core-0.1.0/LICENSE
--rw-r--r--   0        0        0     3341 2023-03-22 09:04:53.154039 ansys-math-core-0.1.0/README.rst
--rw-r--r--   0        0        0     2809 2023-03-22 09:04:53.154039 ansys-math-core-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      868 2023-03-22 09:04:53.154039 ansys-math-core-0.1.0/src/ansys/math/core/__init__.py
--rw-r--r--   0        0        0    61769 2023-03-22 09:04:53.158039 ansys-math-core-0.1.0/src/ansys/math/core/math.py
--rw-r--r--   0        0        0     5820 1970-01-01 00:00:00.000000 ansys-math-core-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-04-12 13:16:03.397489 ansys-math-core-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3266 2023-04-12 13:16:03.397489 ansys-math-core-0.1.1/README.rst
+-rw-r--r--   0        0        0     2809 2023-04-12 13:16:03.397489 ansys-math-core-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      868 2023-04-12 13:16:03.397489 ansys-math-core-0.1.1/src/ansys/math/core/__init__.py
+-rw-r--r--   0        0        0    62314 2023-04-12 13:16:03.397489 ansys-math-core-0.1.1/src/ansys/math/core/math.py
+-rw-r--r--   0        0        0     5745 1970-01-01 00:00:00.000000 ansys-math-core-0.1.1/PKG-INFO
```

### Comparing `ansys-math-core-0.1.0/LICENSE` & `ansys-math-core-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-math-core-0.1.0/README.rst` & `ansys-math-core-0.1.1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 PyAnsys Math
 ============
 
-|pyansys| |pypi| |PyPIact| |GH-CI| |codecov| |MIT| |black|
+|pyansys| |pypi| |GH-CI| |codecov| |MIT| |black|
 
 .. |pyansys| image:: https://img.shields.io/badge/Py-Ansys-ffc107.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC
    :target: https://docs.pyansys.com/
    :alt: PyAnsys
 
-.. |pypi| image:: https://img.shields.io/pypi/v/pyansys-math-core.svg?logo=python&logoColor=white
-   :target: https://pypi.org/project/ansys-math-core/
-
-.. |PyPIact| image:: https://img.shields.io/pypi/dm/pyansys-math-core.svg?label=PyPI%20downloads
+.. |pypi| image:: https://img.shields.io/pypi/v/ansys-math-core.svg?logo=python&logoColor=white
    :target: https://pypi.org/project/ansys-math-core/
 
 .. |codecov| image:: https://codecov.io/gh/pyansys/pyansys-math/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/pyansys/pyansys-math
 
 .. |GH-CI| image:: https://github.com/pyansys/pyansys-math/actions/workflows/ci_cd.yml/badge.svg
    :target: https://github.com/pyansys/pyansys-math/actions/workflows/ci_cd.yml
@@ -39,14 +36,19 @@
 ------------
 
 For users
 ~~~~~~~~~
 The ``ansys.math.core`` package currently supports Python 3.7 through
 Python 3.10 on Windows, Mac OS, and Linux.
 
+.. warning:: 
+
+   ``ansys.math.core`` will no longer support Python 3.7 by June 2023.
+
+
 Install the latest package for use with this command:
 
 .. code::
 
    pip install ansys-math-core
 
 Alternatively, install the latest
@@ -76,15 +78,15 @@
 
 
 Verify your installation
 ------------------------
 
 Check that you can start PyAnsys Math from Python by running this code:
 
-.. code:: python
+.. code:: python3
 
     import ansys.math.core.math as pymath
 
     # Start PyAnsys Math.
     mm = pymath.AnsMath()
     print(mm)
```

### Comparing `ansys-math-core-0.1.0/pyproject.toml` & `ansys-math-core-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "ansys-math-core"
-version = "0.1.0"
+version = "0.1.1"
 description = "A Python wrapper for PyAnsys Math libraries."
 readme = "README.rst"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
@@ -44,19 +44,19 @@
     "pyvista==0.38.5",
     "vtk==9.2.6",
 ]
 doc = [
     "Sphinx==5.3.0",
     "ansys-mapdl-core==0.64.0",
     "ansys-mapdl-reader==0.52.11",
-    "ansys-sphinx-theme==0.9.5",
+    "ansys-sphinx-theme==0.9.7",
     "jupyter_sphinx==0.4.0",
-    "jupyterlab==3.6.2",
+    "jupyterlab==3.6.3",
     "numpydoc==1.5.0",
-    "pandas==1.5.3",
+    "pandas==2.0.0",
     "pypandoc==1.11",
     "pytest-sphinx==0.5.0",
     "pyvista==0.38.5",
     "sphinx-autobuild==2021.3.14",
     "sphinx-autodoc-typehints==1.22",
     "sphinx-copybutton==0.5.1",
     "sphinx-notfound-page==0.8.3",
```

### Comparing `ansys-math-core-0.1.0/src/ansys/math/core/__init__.py` & `ansys-math-core-0.1.1/src/ansys/math/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys-math-core-0.1.0/src/ansys/math/core/math.py` & `ansys-math-core-0.1.1/src/ansys/math/core/math.py`

 * *Files 2% similar despite different names*

```diff
@@ -1490,26 +1490,42 @@
         """
         if not isinstance(vec, AnsVec):
             raise TypeError("The object to be multiplied must be an AnsMath vector.")
 
         self._mapdl.run(f"*DOT,{self.id},{vec.id},py_val")
         return self._mapdl.scalar_param("py_val")
 
-    def asarray(self) -> np.ndarray:
-        """Return this vector as a NumPy array.
+    def asarray(self, dtype=None) -> np.ndarray:
+        """Return the vector as a NumPy array.
+
+        Parameters
+        ----------
+        dtype : numpy.dtype, optional
+            NumPy data type to upload the array as. The options are `np.double <numpy.double>`_,
+            `np.int32 <numpy.int32>`_, and `np.int64 <numpy.int64>`_. The default is the current array
+            type.
+
+        Returns
+        -------
+        np.ndarray
+            NumPy array with the defined data type.
 
         Examples
         --------
         >>> import ansys.math.core.math as pymath
         >>> mm = pymath.AnsMath()
         >>> v = mm.ones(10)
         >>> v.asarray()
         [1. 1. 1. 1. 1. 1. 1. 1. 1. 1.]
+        >>> v.asarray(dtype=np.int32)
+        [1 1 1 1 1 1 1 1 1 1]
+
         """
-        return self._mapdl._vec_data(self.id)
+        vec_data = self._mapdl._vec_data(self.id)
+        return vec_data.astype(dtype) if dtype else vec_data
 
     def __array__(self):
         """Allow NumPy to access this object as if it was an array."""
         return self.asarray()
 
 
 class AnsMat(AnsMathObj):
@@ -1563,15 +1579,15 @@
         warn(
             "Call to ``sym`` method cannot evaluate if this matrix is symmetric "
             "with this version of MAPDL."
         )
         return True
 
     def asarray(self, dtype=None) -> np.ndarray:
-        """Return the vector as a NumPy array.
+        """Return the matrix as a NumPy array.
 
         Parameters
         ----------
         dtype : numpy.dtype, optional
             NumPy data type to upload the array as. The options are ``np.double``,
             ``np.int32``, and ``np.int64``. The default is the current array
             type.
@@ -1581,19 +1597,19 @@
         np.ndarray
             NumPy array with the defined data type.
 
         Examples
         --------
         >>> import ansys.math.core.math as pymath
         >>> mm = pymath.AnsMath()
-        >>> v = mm.ones(10)
+        >>> v = mm.ones(2,2)
         >>> v.asarray()
-        [1. 1. 1. 1. 1. 1. 1. 1. 1. 1.]
-        >>> v.asarray(dtype=np.int)
-        [1 1 1 1 1 1 1 1 1 1]
+        array([[1., 1.], [1., 1.]])
+        >>> v.asarray(dtype=np.int32)
+        array([[1, 1], [1, 1]])
 
         """
         if dtype:
             return self._mapdl._mat_data(self.id).astype(dtype)
         else:
             return self._mapdl._mat_data(self.id)
```

### Comparing `ansys-math-core-0.1.0/PKG-INFO` & `ansys-math-core-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-math-core
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python wrapper for PyAnsys Math libraries.
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
@@ -17,19 +17,19 @@
 Requires-Dist: ansys-mapdl-core>=0.64.0
 Requires-Dist: pyansys-tools-versioning>=0.3.3
 Requires-Dist: numpy>=1.14.0
 Requires-Dist: importlib-metadata>=4.0,<5; python_version<='3.8'
 Requires-Dist: Sphinx==5.3.0 ; extra == "doc"
 Requires-Dist: ansys-mapdl-core==0.64.0 ; extra == "doc"
 Requires-Dist: ansys-mapdl-reader==0.52.11 ; extra == "doc"
-Requires-Dist: ansys-sphinx-theme==0.9.5 ; extra == "doc"
+Requires-Dist: ansys-sphinx-theme==0.9.7 ; extra == "doc"
 Requires-Dist: jupyter_sphinx==0.4.0 ; extra == "doc"
-Requires-Dist: jupyterlab==3.6.2 ; extra == "doc"
+Requires-Dist: jupyterlab==3.6.3 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
-Requires-Dist: pandas==1.5.3 ; extra == "doc"
+Requires-Dist: pandas==2.0.0 ; extra == "doc"
 Requires-Dist: pypandoc==1.11 ; extra == "doc"
 Requires-Dist: pytest-sphinx==0.5.0 ; extra == "doc"
 Requires-Dist: pyvista==0.38.5 ; extra == "doc"
 Requires-Dist: sphinx-autobuild==2021.3.14 ; extra == "doc"
 Requires-Dist: sphinx-autodoc-typehints==1.22 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.1 ; extra == "doc"
 Requires-Dist: sphinx-notfound-page==0.8.3 ; extra == "doc"
@@ -49,24 +49,21 @@
 Project-URL: Tracker, https://github.com/pyansys/ansys-math/issues
 Provides-Extra: doc
 Provides-Extra: tests
 
 PyAnsys Math
 ============
 
-|pyansys| |pypi| |PyPIact| |GH-CI| |codecov| |MIT| |black|
+|pyansys| |pypi| |GH-CI| |codecov| |MIT| |black|
 
 .. |pyansys| image:: https://img.shields.io/badge/Py-Ansys-ffc107.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC
    :target: https://docs.pyansys.com/
    :alt: PyAnsys
 
-.. |pypi| image:: https://img.shields.io/pypi/v/pyansys-math-core.svg?logo=python&logoColor=white
-   :target: https://pypi.org/project/ansys-math-core/
-
-.. |PyPIact| image:: https://img.shields.io/pypi/dm/pyansys-math-core.svg?label=PyPI%20downloads
+.. |pypi| image:: https://img.shields.io/pypi/v/ansys-math-core.svg?logo=python&logoColor=white
    :target: https://pypi.org/project/ansys-math-core/
 
 .. |codecov| image:: https://codecov.io/gh/pyansys/pyansys-math/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/pyansys/pyansys-math
 
 .. |GH-CI| image:: https://github.com/pyansys/pyansys-math/actions/workflows/ci_cd.yml/badge.svg
    :target: https://github.com/pyansys/pyansys-math/actions/workflows/ci_cd.yml
@@ -91,14 +88,19 @@
 ------------
 
 For users
 ~~~~~~~~~
 The ``ansys.math.core`` package currently supports Python 3.7 through
 Python 3.10 on Windows, Mac OS, and Linux.
 
+.. warning:: 
+
+   ``ansys.math.core`` will no longer support Python 3.7 by June 2023.
+
+
 Install the latest package for use with this command:
 
 .. code::
 
    pip install ansys-math-core
 
 Alternatively, install the latest
@@ -128,15 +130,15 @@
 
 
 Verify your installation
 ------------------------
 
 Check that you can start PyAnsys Math from Python by running this code:
 
-.. code:: python
+.. code:: python3
 
     import ansys.math.core.math as pymath
 
     # Start PyAnsys Math.
     mm = pymath.AnsMath()
     print(mm)
```

