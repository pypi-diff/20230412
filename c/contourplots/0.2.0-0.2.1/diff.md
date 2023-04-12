# Comparing `tmp/contourplots-0.2.0.tar.gz` & `tmp/contourplots-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contourplots-0.2.0.tar", last modified: Wed Apr 12 02:12:36 2023, max compression
+gzip compressed data, was "contourplots-0.2.1.tar", last modified: Wed Apr 12 02:18:52 2023, max compression
```

## Comparing `contourplots-0.2.0.tar` & `contourplots-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 02:12:36.050519 contourplots-0.2.0/
--rw-rw-rw-   0        0        0     1986 2022-11-13 16:15:08.000000 contourplots-0.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0      608 2023-04-12 02:12:36.049558 contourplots-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      107 2022-11-13 16:29:55.000000 contourplots-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 02:12:36.038489 contourplots-0.2.0/contourplots/
--rw-rw-rw-   0        0        0      732 2023-04-12 02:10:36.000000 contourplots-0.2.0/contourplots/__init__.py
--rw-rw-rw-   0        0        0    25220 2023-03-20 13:57:23.000000 contourplots-0.2.0/contourplots/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 02:12:36.047527 contourplots-0.2.0/contourplots.egg-info/
--rw-rw-rw-   0        0        0      608 2023-04-12 02:12:35.000000 contourplots-0.2.0/contourplots.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2023-04-12 02:12:35.000000 contourplots-0.2.0/contourplots.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 02:12:35.000000 contourplots-0.2.0/contourplots.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-12 02:12:35.000000 contourplots-0.2.0/contourplots.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-12 02:12:35.000000 contourplots-0.2.0/contourplots.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 02:12:36.050519 contourplots-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1003 2023-04-12 02:10:29.000000 contourplots-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:18:52.910452 contourplots-0.2.1/
+-rw-rw-rw-   0        0        0     1986 2022-11-13 16:15:08.000000 contourplots-0.2.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      608 2023-04-12 02:18:52.909453 contourplots-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      107 2022-11-13 16:29:55.000000 contourplots-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 02:18:52.900478 contourplots-0.2.1/contourplots/
+-rw-rw-rw-   0        0        0      732 2023-04-12 02:18:07.000000 contourplots-0.2.1/contourplots/__init__.py
+-rw-rw-rw-   0        0        0    25746 2023-04-12 02:17:52.000000 contourplots-0.2.1/contourplots/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:18:52.908457 contourplots-0.2.1/contourplots.egg-info/
+-rw-rw-rw-   0        0        0      608 2023-04-12 02:18:52.000000 contourplots-0.2.1/contourplots.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2023-04-12 02:18:52.000000 contourplots-0.2.1/contourplots.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 02:18:52.000000 contourplots-0.2.1/contourplots.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-12 02:18:52.000000 contourplots-0.2.1/contourplots.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-12 02:18:52.000000 contourplots-0.2.1/contourplots.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 02:18:52.910452 contourplots-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2023-04-12 02:18:15.000000 contourplots-0.2.1/setup.py
```

### Comparing `contourplots-0.2.0/LICENSE.txt` & `contourplots-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `contourplots-0.2.0/PKG-INFO` & `contourplots-0.2.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contourplots
-Version: 0.2.0
+Version: 0.2.1
 Summary: A toolkit for generating multi-dimensional plots easily, usefully, and legibly.
 Home-page: https://github.com/sarangbhagwat/contourplots
 Author: Sarang S. Bhagwat
 Author-email: sarang.bhagwat.git@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `contourplots-0.2.0/contourplots/__init__.py` & `contourplots-0.2.1/contourplots/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # ContourPlots: A toolkit for generating multi-dimensional plots easily, usefully, and legibly.
 # Copyright (C) 2022-2023, Sarang Bhagwat <sarang.bhagwat.git@gmail.com>
 # 
 # This module is under the MIT open-source license. See 
 # https://github.com/sarangbhagwat/contourplots/blob/main/LICENSE
 # for license details.
 
-__version__ = '0.2.0'
+__version__ = '0.2.1'
 __author__ = 'Sarang S. Bhagwat'
 
 # %% Initialize ContourPlots 
 
 from . import utils
 
 animated_contourplot = utils.animated_contourplot
```

### Comparing `contourplots-0.2.0/contourplots/utils.py` & `contourplots-0.2.1/contourplots/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,14 @@
 # -*- coding: utf-8 -*-
+# ContourPlots: A toolkit for generating multi-dimensional plots easily, usefully, and legibly.
+# Copyright (C) 2022-2023, Sarang Bhagwat <sarang.bhagwat.git@gmail.com>
+# 
+# This module is under the MIT open-source license. See 
+# https://github.com/sarangbhagwat/contourplots/blob/main/LICENSE
+# for license details.
 """
 Created on Fri Nov 11 10:15:45 2022
 
 @author: sarangbhagwat
 """
 
 #%% Plot MPSP
@@ -15,14 +21,17 @@
 import matplotlib as mpl
 from matplotlib.ticker import AutoMinorLocator, LinearLocator, FixedLocator
 from matplotlib.ticker import FuncFormatter
 from matplotlib.container import BarContainer
 import textwrap
 import itertools
 
+defaults_dict ={'colors':
+                {'Guest_Group_TEA_Breakdown': ['#7BBD84', '#F7C652', '#63C6CE', '#94948C', '#734A8C', '#D1C0E1', '#648496', '#B97A57', '#D1C0E1', '#F8858A', '#F8858A', ]}}
+
 def wrap_labels(ax, width, break_long_words=False, fontsize=14):
     labels = []
     for label in ax.get_xticklabels():
         text = label.get_text()
         labels.append(textwrap.fill(text, width=width,
                       break_long_words=break_long_words))
     ax.set_xticklabels(labels, rotation=0, fontsize=fontsize, weight='bold')
```

### Comparing `contourplots-0.2.0/contourplots.egg-info/PKG-INFO` & `contourplots-0.2.1/contourplots.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contourplots
-Version: 0.2.0
+Version: 0.2.1
 Summary: A toolkit for generating multi-dimensional plots easily, usefully, and legibly.
 Home-page: https://github.com/sarangbhagwat/contourplots
 Author: Sarang S. Bhagwat
 Author-email: sarang.bhagwat.git@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `contourplots-0.2.0/setup.py` & `contourplots-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 
 from setuptools import setup
 
 setup(
     name='contourplots',
     packages=['contourplots'],
-    version='0.2.0',    
+    version='0.2.1',    
     description='A toolkit for generating multi-dimensional plots easily, usefully, and legibly.',
     url='https://github.com/sarangbhagwat/contourplots',
     author='Sarang S. Bhagwat',
     author_email='sarang.bhagwat.git@gmail.com',
     license='MIT',
     # packages=['contourplots'],
     install_requires=['matplotlib==3.5.2',
```

