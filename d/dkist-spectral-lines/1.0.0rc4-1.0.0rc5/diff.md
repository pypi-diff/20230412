# Comparing `tmp/dkist-spectral-lines-1.0.0rc4.tar.gz` & `tmp/dkist-spectral-lines-1.0.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-spectral-lines-1.0.0rc4.tar", last modified: Mon Feb 27 18:43:50 2023, max compression
+gzip compressed data, was "dkist-spectral-lines-1.0.0rc5.tar", last modified: Wed Apr 12 18:55:05 2023, max compression
```

## Comparing `dkist-spectral-lines-1.0.0rc4.tar` & `dkist-spectral-lines-1.0.0rc5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-27 18:43:50.759597 dkist-spectral-lines-1.0.0rc4/
--rw-rw-rw-   0 root         (0) root         (0)     2448 2023-02-27 18:43:45.000000 dkist-spectral-lines-1.0.0rc4/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-02-27 18:43:45.000000 dkist-spectral-lines-1.0.0rc4/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      256 2023-02-27 18:43:45.000000 dkist-spectral-lines-1.0.0rc4/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-27 18:43:45.000000 dkist-spectral-lines-1.0.0rc4/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     4111 2023-02-27 18:43:50.759597 dkist-spectral-lines-1.0.0rc4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3553 2023-02-27 18:43:45.000000 dkist-spectral-lines-1.0.0rc4/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2066 2023-02-27 18:43:45.000000 dkist-spectral-lines-1.0.0rc4/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-27 18:43:50.755597 dkist-spectral-lines-1.0.0rc4/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-27 18:43:45.000000 dkist-spectral-lines-1.0.0rc4/changelog/.gitempty
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-02-27 18:43:45.000000 dkist-spectral-lines-1.0.0rc4/changelog/1.feature.rst
--rwxrwxrwx   0 root         (0) root         (0)      643 2023-02-27 18:43:45.000000 dkist-spectral-lines-1.0.0rc4/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-27 18:43:50.755597 dkist-spectral-lines-1.0.0rc4/dkist_spectral_lines/
--rw-rw-rw-   0 root         (0) root         (0)      387 2023-02-27 18:43:45.000000 dkist-spectral-lines-1.0.0rc4/dkist_spectral_lines/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2182 2023-02-27 18:43:45.000000 dkist-spectral-lines-1.0.0rc4/dkist_spectral_lines/find.py
--rw-rw-rw-   0 root         (0) root         (0)     7301 2023-02-27 18:43:45.000000 dkist-spectral-lines-1.0.0rc4/dkist_spectral_lines/lines.py
--rw-rw-rw-   0 root         (0) root         (0)     3393 2023-02-27 18:43:45.000000 dkist-spectral-lines-1.0.0rc4/dkist_spectral_lines/models.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-27 18:43:50.759597 dkist-spectral-lines-1.0.0rc4/dkist_spectral_lines/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-27 18:43:45.000000 dkist-spectral-lines-1.0.0rc4/dkist_spectral_lines/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5075 2023-02-27 18:43:45.000000 dkist-spectral-lines-1.0.0rc4/dkist_spectral_lines/tests/test_find.py
--rw-rw-rw-   0 root         (0) root         (0)     1043 2023-02-27 18:43:45.000000 dkist-spectral-lines-1.0.0rc4/dkist_spectral_lines/tests/test_lines.py
--rw-rw-rw-   0 root         (0) root         (0)     4739 2023-02-27 18:43:45.000000 dkist-spectral-lines-1.0.0rc4/dkist_spectral_lines/tests/test_models.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-27 18:43:50.759597 dkist-spectral-lines-1.0.0rc4/dkist_spectral_lines.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4111 2023-02-27 18:43:50.000000 dkist-spectral-lines-1.0.0rc4/dkist_spectral_lines.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      805 2023-02-27 18:43:50.000000 dkist-spectral-lines-1.0.0rc4/dkist_spectral_lines.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-02-27 18:43:50.000000 dkist-spectral-lines-1.0.0rc4/dkist_spectral_lines.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      155 2023-02-27 18:43:50.000000 dkist-spectral-lines-1.0.0rc4/dkist_spectral_lines.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-02-27 18:43:50.000000 dkist-spectral-lines-1.0.0rc4/dkist_spectral_lines.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-27 18:43:50.759597 dkist-spectral-lines-1.0.0rc4/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-02-27 18:43:45.000000 dkist-spectral-lines-1.0.0rc4/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-02-27 18:43:45.000000 dkist-spectral-lines-1.0.0rc4/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1852 2023-02-27 18:43:45.000000 dkist-spectral-lines-1.0.0rc4/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-02-27 18:43:45.000000 dkist-spectral-lines-1.0.0rc4/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-02-27 18:43:45.000000 dkist-spectral-lines-1.0.0rc4/docs/make.bat
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-27 18:43:50.759597 dkist-spectral-lines-1.0.0rc4/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-02-27 18:43:45.000000 dkist-spectral-lines-1.0.0rc4/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-02-27 18:43:45.000000 dkist-spectral-lines-1.0.0rc4/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1136 2023-02-27 18:43:50.759597 dkist-spectral-lines-1.0.0rc4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-02-27 18:43:45.000000 dkist-spectral-lines-1.0.0rc4/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 18:55:05.151088 dkist-spectral-lines-1.0.0rc5/
+-rw-rw-rw-   0 root         (0) root         (0)     2448 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      256 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4198 2023-04-12 18:55:05.151088 dkist-spectral-lines-1.0.0rc5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3640 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2066 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 18:55:05.147088 dkist-spectral-lines-1.0.0rc5/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/changelog/.gitempty
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/changelog/1.feature.rst
+-rwxrwxrwx   0 root         (0) root         (0)      643 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 18:55:05.147088 dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5156 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines/lines.py
+-rw-rw-rw-   0 root         (0) root         (0)     1476 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      716 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines/search.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 18:55:05.147088 dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1416 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines/tests/test_lines.py
+-rw-rw-rw-   0 root         (0) root         (0)     1545 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     3267 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines/tests/test_search.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 18:55:05.147088 dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4198 2023-04-12 18:55:05.000000 dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      809 2023-04-12 18:55:05.000000 dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-12 18:55:05.000000 dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      155 2023-04-12 18:55:05.000000 dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-12 18:55:05.000000 dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 18:55:05.151088 dkist-spectral-lines-1.0.0rc5/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1852 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/docs/make.bat
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 18:55:05.151088 dkist-spectral-lines-1.0.0rc5/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1136 2023-04-12 18:55:05.151088 dkist-spectral-lines-1.0.0rc5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-04-12 18:54:57.000000 dkist-spectral-lines-1.0.0rc5/setup.py
```

### Comparing `dkist-spectral-lines-1.0.0rc4/.gitignore` & `dkist-spectral-lines-1.0.0rc5/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-spectral-lines-1.0.0rc4/.pre-commit-config.yaml` & `dkist-spectral-lines-1.0.0rc5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-spectral-lines-1.0.0rc4/PKG-INFO` & `dkist-spectral-lines-1.0.0rc5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-spectral-lines
-Version: 1.0.0rc4
+Version: 1.0.0rc5
 Summary: Spectral line metadata for the DKIST suite of instruments
 Home-page: https://bitbucket.org/dkistdc/dkist-spectral-lines/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/spectral_lines
 Classifier: Programming Language :: Python
@@ -25,18 +25,19 @@
 Usage
 -----
 The spectral lines are all defined as classes with properties capturing their relevant metadata.  Spectral lines can be
 retrieved using one of the helper functions
 
 .. code-block:: python
 
-    from dkist_spectral_lines import find_spectral_lines
-    from dkist_spectral_lines import Instrument
+    from dkist_spectral_lines import get_spectral_lines
+    from dkist_spectral_lines import get_closest_spectral_line
 
-    all_visp_spectral_lines = find_spectral_lines(instrument=Instrument.VISP)
+    spectral_lines_in_a_range = get_spectral_lines(wavelength_min=1, wavelength_max=1000)
+    closest_line = get_closest_spectral_line(wavelength=100)
 
 Build
 -----
 dkist-spectral-lines is built using `bitbucket-pipelines <bitbucket-pipelines.yml>`_
 
 Deployment
 ----------
```

### Comparing `dkist-spectral-lines-1.0.0rc4/README.rst` & `dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: dkist-spectral-lines
+Version: 1.0.0rc5
+Summary: Spectral line metadata for the DKIST suite of instruments
+Home-page: https://bitbucket.org/dkistdc/dkist-spectral-lines/src/main/
+Author: NSO / AURA
+Author-email: "dkistdc@nso.edu"
+License: MIT
+Project-URL: Documentation, https://docs.dkist.nso.edu/projects/spectral_lines
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10
+Provides-Extra: test
+Provides-Extra: docs
+
 dkist-spectral-lines
 =====================
 
 Overview
 --------
 The dkist-spectral-lines package consolidates the definition of metadata associated with spectral lines observed by the
 DKIST instruments.
@@ -9,18 +25,19 @@
 Usage
 -----
 The spectral lines are all defined as classes with properties capturing their relevant metadata.  Spectral lines can be
 retrieved using one of the helper functions
 
 .. code-block:: python
 
-    from dkist_spectral_lines import find_spectral_lines
-    from dkist_spectral_lines import Instrument
+    from dkist_spectral_lines import get_spectral_lines
+    from dkist_spectral_lines import get_closest_spectral_line
 
-    all_visp_spectral_lines = find_spectral_lines(instrument=Instrument.VISP)
+    spectral_lines_in_a_range = get_spectral_lines(wavelength_min=1, wavelength_max=1000)
+    closest_line = get_closest_spectral_line(wavelength=100)
 
 Build
 -----
 dkist-spectral-lines is built using `bitbucket-pipelines <bitbucket-pipelines.yml>`_
 
 Deployment
 ----------
```

### Comparing `dkist-spectral-lines-1.0.0rc4/bitbucket-pipelines.yml` & `dkist-spectral-lines-1.0.0rc5/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-spectral-lines-1.0.0rc4/check_changelog_updated.sh` & `dkist-spectral-lines-1.0.0rc5/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist-spectral-lines-1.0.0rc4/dkist_spectral_lines/tests/test_lines.py` & `dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines/tests/test_lines.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Tests for the line definitions"""
 from collections import Counter
 
 import pytest
 
-from dkist_spectral_lines import SpectralLine
+from dkist_spectral_lines import get_spectral_lines
+from dkist_spectral_lines.models import SpectralLine
 
 
 @pytest.fixture()
 def spectral_lines() -> tuple[SpectralLine]:
     """Import of spectral lines to capture validation errors in test setup vs collection"""
     from dkist_spectral_lines.lines import SPECTRAL_LINES
 
@@ -20,17 +21,30 @@
     :When: Instantiating the data structures
     :Then: Validation doesn't raise s pydantic.ValidationError
     """
     # Then
     assert spectral_lines
 
 
+def test_lines_are_sortable(spectral_lines):
+    """
+    :Given: Spectral line data structures
+    :When: Sorting them
+    :Then: They get sorted by rest_wavelength_in_air
+    """
+    sorted_lines = list(sorted(spectral_lines))
+    # Then
+    for idx in range(1, len(sorted_lines)):
+        assert (
+            sorted_lines[idx - 1].rest_wavelength_in_air < sorted_lines[idx].rest_wavelength_in_air
+        )
+
+
 def test_lines_are_uniquely_named(spectral_lines):
     """
     :Given: Spectral line data structures
     :When: Inspecting name_id
     :Then: All name ids are unique
     """
-    name_ids = [l.name_id for l in spectral_lines]
-    name_id_counts = Counter(name_ids)
-    assert not ({k: v for k, v in name_id_counts.items() if v > 1})
-    # failing here probably means the SpectralLine needs include_wavelength_in_name=True
+    names = [line.name for line in spectral_lines]
+    name_counts = Counter(names)
+    assert not ({k: v for k, v in name_counts.items() if v > 1})
```

### Comparing `dkist-spectral-lines-1.0.0rc4/dkist_spectral_lines.egg-info/SOURCES.txt` & `dkist-spectral-lines-1.0.0rc5/dkist_spectral_lines.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 check_changelog_updated.sh
 pyproject.toml
 setup.cfg
 setup.py
 changelog/.gitempty
 changelog/1.feature.rst
 dkist_spectral_lines/__init__.py
-dkist_spectral_lines/find.py
 dkist_spectral_lines/lines.py
 dkist_spectral_lines/models.py
+dkist_spectral_lines/search.py
 dkist_spectral_lines.egg-info/PKG-INFO
 dkist_spectral_lines.egg-info/SOURCES.txt
 dkist_spectral_lines.egg-info/dependency_links.txt
 dkist_spectral_lines.egg-info/requires.txt
 dkist_spectral_lines.egg-info/top_level.txt
 dkist_spectral_lines/tests/__init__.py
-dkist_spectral_lines/tests/test_find.py
 dkist_spectral_lines/tests/test_lines.py
 dkist_spectral_lines/tests/test_models.py
+dkist_spectral_lines/tests/test_search.py
 docs/Makefile
 docs/changelog.rst
 docs/conf.py
 docs/index.rst
 docs/make.bat
 licenses/LICENSE.rst
```

### Comparing `dkist-spectral-lines-1.0.0rc4/docs/Makefile` & `dkist-spectral-lines-1.0.0rc5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-spectral-lines-1.0.0rc4/docs/conf.py` & `dkist-spectral-lines-1.0.0rc5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-spectral-lines-1.0.0rc4/docs/make.bat` & `dkist-spectral-lines-1.0.0rc5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-spectral-lines-1.0.0rc4/licenses/LICENSE.rst` & `dkist-spectral-lines-1.0.0rc5/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-spectral-lines-1.0.0rc4/pyproject.toml` & `dkist-spectral-lines-1.0.0rc5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist-spectral-lines-1.0.0rc4/setup.cfg` & `dkist-spectral-lines-1.0.0rc5/setup.cfg`

 * *Files identical despite different names*

