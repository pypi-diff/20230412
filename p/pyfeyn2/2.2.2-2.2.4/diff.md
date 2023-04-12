# Comparing `tmp/pyfeyn2-2.2.2.tar.gz` & `tmp/pyfeyn2-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfeyn2-2.2.2.tar", max compression
+gzip compressed data, was "pyfeyn2-2.2.4.tar", max compression
```

## Comparing `pyfeyn2-2.2.2.tar` & `pyfeyn2-2.2.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    35149 2022-12-05 14:40:29.583013 pyfeyn2-2.2.2/LICENSE
--rw-r--r--   0        0        0     4258 2023-01-02 20:30:26.485525 pyfeyn2-2.2.2/README.md
--rw-r--r--   0        0        0      154 2022-12-20 14:55:57.993414 pyfeyn2-2.2.2/pyfeyn2/__init__.py
--rw-r--r--   0        0        0        0 2022-12-18 10:12:48.176221 pyfeyn2-2.2.2/pyfeyn2/auto/__init__.py
--rw-r--r--   0        0        0     2841 2022-12-20 20:00:59.986327 pyfeyn2-2.2.2/pyfeyn2/auto/bend.py
--rw-r--r--   0        0        0      774 2022-12-26 00:16:46.384489 pyfeyn2-2.2.2/pyfeyn2/auto/label.py
--rw-r--r--   0        0        0     2073 2022-12-20 15:20:32.847535 pyfeyn2-2.2.2/pyfeyn2/auto/position.py
--rw-r--r--   0        0        0        0 2022-12-18 10:12:48.176221 pyfeyn2-2.2.2/pyfeyn2/auto/reshuffle.py
--rw-r--r--   0        0        0      647 2023-01-02 20:30:11.604327 pyfeyn2-2.2.2/pyfeyn2/feynmandiagram.py
--rw-r--r--   0        0        0     2305 2022-12-27 00:30:58.970725 pyfeyn2-2.2.2/pyfeyn2/interface/dot.py
--rw-r--r--   0        0        0     1488 2023-01-02 20:52:49.233790 pyfeyn2-2.2.2/pyfeyn2/interface/hepmc.py
--rw-r--r--   0        0        0     1569 2023-01-02 20:52:49.233790 pyfeyn2-2.2.2/pyfeyn2/interface/qgraf.py
--rw-r--r--   0        0        0      169 2022-12-09 20:44:01.292940 pyfeyn2-2.2.2/pyfeyn2/mkfeyndiag.py
--rw-r--r--   0        0        0        0 2022-12-05 14:40:29.591013 pyfeyn2-2.2.2/pyfeyn2/render/__init__.py
--rw-r--r--   0        0        0     3651 2023-01-02 20:30:11.595326 pyfeyn2-2.2.2/pyfeyn2/render/all.py
--rw-r--r--   0        0        0        0 2022-12-18 10:12:48.177221 pyfeyn2-2.2.2/pyfeyn2/render/latex/__init__.py
--rw-r--r--   0        0        0     3372 2023-01-02 20:11:55.464689 pyfeyn2-2.2.2/pyfeyn2/render/latex/dot.py
--rw-r--r--   0        0        0     5609 2022-12-27 00:28:15.158277 pyfeyn2-2.2.2/pyfeyn2/render/latex/feynmp.py
--rw-r--r--   0        0        0     1616 2022-12-11 20:29:57.890504 pyfeyn2-2.2.2/pyfeyn2/render/latex/latex.py
--rw-r--r--   0        0        0     2407 2022-12-11 20:29:57.890504 pyfeyn2-2.2.2/pyfeyn2/render/latex/metapost.py
--rw-r--r--   0        0        0     6178 2023-01-02 20:33:53.469287 pyfeyn2-2.2.2/pyfeyn2/render/latex/tikzfeynman.py
--rw-r--r--   0        0        0     5592 2022-12-27 00:25:55.499219 pyfeyn2-2.2.2/pyfeyn2/render/mpl/feynmanrender.py
--rw-r--r--   0        0        0        0 2022-12-09 18:35:43.493131 pyfeyn2-2.2.2/pyfeyn2/render/pyx/__init__.py
--rw-r--r--   0        0        0     7132 2022-12-09 20:44:01.292940 pyfeyn2-2.2.2/pyfeyn2/render/pyx/blobs.py
--rw-r--r--   0        0        0     1319 2022-12-09 18:35:41.233098 pyfeyn2-2.2.2/pyfeyn2/render/pyx/config.py
--rw-r--r--   0        0        0    13169 2022-12-09 20:44:01.292940 pyfeyn2-2.2.2/pyfeyn2/render/pyx/deco.py
--rw-r--r--   0        0        0     2561 2022-12-10 22:09:51.360630 pyfeyn2-2.2.2/pyfeyn2/render/pyx/diagrams.py
--rw-r--r--   0        0        0    41001 2022-12-11 20:30:04.144574 pyfeyn2-2.2.2/pyfeyn2/render/pyx/lines.py
--rw-r--r--   0        0        0     3549 2022-12-09 20:44:01.293940 pyfeyn2-2.2.2/pyfeyn2/render/pyx/paint.py
--rw-r--r--   0        0        0    12623 2022-12-11 20:30:04.144574 pyfeyn2-2.2.2/pyfeyn2/render/pyx/points.py
--rw-r--r--   0        0        0     7816 2023-01-02 20:36:12.878182 pyfeyn2-2.2.2/pyfeyn2/render/pyx/pyxrender.py
--rw-r--r--   0        0        0     1501 2022-12-09 18:46:15.468331 pyfeyn2-2.2.2/pyfeyn2/render/pyx/utils.py
--rw-r--r--   0        0        0     2642 2023-01-02 20:27:47.379402 pyfeyn2-2.2.2/pyfeyn2/render/render.py
--rw-r--r--   0        0        0     6943 2022-12-27 00:52:38.751536 pyfeyn2-2.2.2/pyfeyn2/render/text/ascii.py
--rw-r--r--   0        0        0      745 2022-12-11 20:29:57.890504 pyfeyn2-2.2.2/pyfeyn2/render/text/asciipdf.py
--rw-r--r--   0        0        0     2228 2022-12-11 20:29:57.890504 pyfeyn2-2.2.2/pyfeyn2/render/text/label.py
--rw-r--r--   0        0        0     1547 2022-12-11 20:29:57.890504 pyfeyn2-2.2.2/pyfeyn2/render/text/line.py
--rw-r--r--   0        0        0     1502 2022-12-11 20:29:57.890504 pyfeyn2-2.2.2/pyfeyn2/render/text/plainpdf.py
--rw-r--r--   0        0        0      483 2022-12-27 00:07:12.242606 pyfeyn2-2.2.2/pyfeyn2/render/text/point.py
--rw-r--r--   0        0        0     3846 2022-12-11 20:29:57.890504 pyfeyn2-2.2.2/pyfeyn2/render/text/style.py
--rw-r--r--   0        0        0     1401 2022-12-27 00:00:29.004965 pyfeyn2-2.2.2/pyfeyn2/render/text/unicode.py
--rw-r--r--   0        0        0     1858 2022-12-11 20:29:57.890504 pyfeyn2-2.2.2/pyfeyn2/render/text/unicodepdf.py
--rw-r--r--   0        0        0     2470 2023-01-02 20:53:02.924978 pyfeyn2-2.2.2/pyproject.toml
--rw-r--r--   0        0        0     6062 1970-01-01 00:00:00.000000 pyfeyn2-2.2.2/setup.py
--rw-r--r--   0        0        0     5946 1970-01-01 00:00:00.000000 pyfeyn2-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-12 08:31:25.170839 pyfeyn2-2.2.4/LICENSE
+-rw-r--r--   0        0        0     3226 2023-04-12 08:31:25.170839 pyfeyn2-2.2.4/README.md
+-rw-r--r--   0        0        0      154 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/auto/__init__.py
+-rw-r--r--   0        0        0     2841 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/auto/bend.py
+-rw-r--r--   0        0        0      774 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/auto/label.py
+-rw-r--r--   0        0        0     2073 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/auto/position.py
+-rw-r--r--   0        0        0        0 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/auto/reshuffle.py
+-rw-r--r--   0        0        0      680 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/feynmandiagram.py
+-rw-r--r--   0        0        0     2305 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/interface/dot.py
+-rw-r--r--   0        0        0       85 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/interface/hepmc.py
+-rw-r--r--   0        0        0       85 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/interface/qgraf.py
+-rw-r--r--   0        0        0      169 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/mkfeyndiag.py
+-rw-r--r--   0        0        0        0 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/__init__.py
+-rw-r--r--   0        0        0     3651 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/all.py
+-rw-r--r--   0        0        0        0 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/latex/__init__.py
+-rw-r--r--   0        0        0     3492 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/latex/dot.py
+-rw-r--r--   0        0        0     6203 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/latex/feynmp.py
+-rw-r--r--   0        0        0     1616 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/latex/latex.py
+-rw-r--r--   0        0        0     2407 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/latex/metapost.py
+-rw-r--r--   0        0        0     6302 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/latex/tikzfeynman.py
+-rw-r--r--   0        0        0     6026 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/mpl/feynmanrender.py
+-rw-r--r--   0        0        0        0 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/pyx/__init__.py
+-rw-r--r--   0        0        0     7132 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/pyx/blobs.py
+-rw-r--r--   0        0        0     1319 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/pyx/config.py
+-rw-r--r--   0        0        0    13169 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/pyx/deco.py
+-rw-r--r--   0        0        0     2561 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/pyx/diagrams.py
+-rw-r--r--   0        0        0    41291 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/pyx/lines.py
+-rw-r--r--   0        0        0     3549 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/pyx/paint.py
+-rw-r--r--   0        0        0    12623 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/pyx/points.py
+-rw-r--r--   0        0        0     7976 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/pyx/pyxrender.py
+-rw-r--r--   0        0        0     1501 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/pyx/utils.py
+-rw-r--r--   0        0        0     2914 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/render.py
+-rw-r--r--   0        0        0     7120 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/text/ascii.py
+-rw-r--r--   0        0        0      745 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/text/asciipdf.py
+-rw-r--r--   0        0        0     2228 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/text/label.py
+-rw-r--r--   0        0        0     1547 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/text/line.py
+-rw-r--r--   0        0        0     1502 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/text/plainpdf.py
+-rw-r--r--   0        0        0      483 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/text/point.py
+-rw-r--r--   0        0        0     3846 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/text/style.py
+-rw-r--r--   0        0        0     1401 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/text/unicode.py
+-rw-r--r--   0        0        0     1858 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/text/unicodepdf.py
+-rw-r--r--   0        0        0     2480 2023-04-12 08:31:27.499010 pyfeyn2-2.2.4/pyproject.toml
+-rw-r--r--   0        0        0     5016 1970-01-01 00:00:00.000000 pyfeyn2-2.2.4/setup.py
+-rw-r--r--   0        0        0     4886 1970-01-01 00:00:00.000000 pyfeyn2-2.2.4/PKG-INFO
```

### Comparing `pyfeyn2-2.2.2/LICENSE` & `pyfeyn2-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.2/README.md` & `pyfeyn2-2.2.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # PyFeyn2
 
 Forked from <https://pyfeyn.hepforge.org/> 
 
 PyFeyn is a Python-language based system for drawing Feynman diagrams. It was inspired by the C++ FeynDiagram system, and aims to provide the same functionality and quality of output as that, with the added benefits of a modern interpreted language, an improved interface and output direct to both EPS and PDF. Behind the scenes, PyFeyn uses the excellent PyX system - you can use PyX constructs in PyFeyn diagrams if you want, too.
 
-[![PyPI version][pypi image]][pypi link] [![PyPI version][pypi versions]][pypi link]  ![downloads](https://img.shields.io/pypi/dm/smpl.svg)
+[![PyPI version][pypi image]][pypi link] [![PyPI version][pypi versions]][pypi link]  ![downloads](https://img.shields.io/pypi/dm/pyfeyn2.svg)
 
 [![test][a t image]][a t link]      [![Coverage Status][c t i]][c t l]  [![Codacy Badge][cc c i]][cc c l]   [![Codacy Badge][cc q i]][cc q l]  [![Documentation][rtd t i]][rtd t l]
 
 ## Dependencies
 
 *   libmagickwand-dev (to display pdfs in a jupyter-notebook, might require a policy change of the imagemagick config for PDFs, see Troubleshooting)
 *   ghostscript
@@ -53,31 +53,20 @@
 [doc stable]: https://apn-pucky.github.io/pyfeyn2/index.html
 [doc test]: https://apn-pucky.github.io/pyfeyn2/test/index.html
 
 [pypi image]: https://badge.fury.io/py/pyfeyn2.svg
 [pypi link]: https://pypi.org/project/pyfeyn2/
 [pypi versions]: https://img.shields.io/pypi/pyversions/pyfeyn2.svg
 
-[a s image]: https://github.com/APN-Pucky/pyfeyn2/actions/workflows/stable.yml/badge.svg
-[a s link]: https://github.com/APN-Pucky/pyfeyn2/actions/workflows/stable.yml
 [a t link]: https://github.com/APN-Pucky/pyfeyn2/actions/workflows/test.yml
 [a t image]: https://github.com/APN-Pucky/pyfeyn2/actions/workflows/test.yml/badge.svg
 
-[cc s q i]: https://app.codacy.com/project/badge/Grade/135bae47c6344ab0bfb180135ea1db44?branch=stable
-[cc s q l]: https://www.codacy.com/gh/APN-Pucky/pyfeyn2/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/pyfeyn2&amp;utm_campaign=Badge_Grade?branch=stable
-[cc s c i]: https://app.codacy.com/project/badge/Coverage/135bae47c6344ab0bfb180135ea1db44?branch=stable
-[cc s c l]: https://www.codacy.com/gh/APN-Pucky/smpl/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/pyfeyn2&utm_campaign=Badge_Coverage?branch=stable
-
 [cc q i]: https://app.codacy.com/project/badge/Grade/135bae47c6344ab0bfb180135ea1db44
 [cc q l]: https://www.codacy.com/gh/APN-Pucky/pyfeyn2/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/pyfeyn2&amp;utm_campaign=Badge_Grade
 [cc c i]: https://app.codacy.com/project/badge/Coverage/135bae47c6344ab0bfb180135ea1db44
 [cc c l]: https://www.codacy.com/gh/APN-Pucky/pyfeyn2/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/pyfeyn2&utm_campaign=Badge_Coverage
 
-[c s i]: https://coveralls.io/repos/github/APN-Pucky/pyfeyn2/badge.svg?branch=stable
-[c s l]: https://coveralls.io/github/APN-Pucky/pyfeyn2?branch=stable
 [c t l]: https://coveralls.io/github/APN-Pucky/pyfeyn2?branch=master
 [c t i]: https://coveralls.io/repos/github/APN-Pucky/pyfeyn2/badge.svg?branch=master
 
-[rtd s i]: https://readthedocs.org/projects/pyfeyn2/badge/?version=stable
-[rtd s l]: https://pyfeyn2.readthedocs.io/en/stable/?badge=stable
 [rtd t i]: https://readthedocs.org/projects/pyfeyn2/badge/?version=latest
 [rtd t l]: https://pyfeyn2.readthedocs.io/en/latest/?badge=latest
```

### Comparing `pyfeyn2-2.2.2/pyfeyn2/auto/bend.py` & `pyfeyn2-2.2.4/pyfeyn2/auto/bend.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.2/pyfeyn2/auto/label.py` & `pyfeyn2-2.2.4/pyfeyn2/auto/label.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.2/pyfeyn2/auto/position.py` & `pyfeyn2-2.2.4/pyfeyn2/auto/position.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.2/pyfeyn2/feynmandiagram.py` & `pyfeyn2-2.2.4/pyfeyn2/feynmandiagram.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+"""Moved to :py:mod:`feynml`"""
 from importlib.metadata import version
 
 from feynml.connector import Connector
 from feynml.feynmandiagram import FeynmanDiagram
 from feynml.feynml import FeynML as FeynML_
 from feynml.feynml import Head, Meta, Tool
 from feynml.leg import Leg
 from feynml.momentum import Momentum
 from feynml.pdgid import PDG
 from feynml.point import Point
 from feynml.propagator import Propagator
-from feynml.style import Styled
+from feynml.styled import Styled
 from feynml.vertex import Vertex
 
 
 class FeynML(FeynML_):
     """FeynML with pyfeyn2 meta tag."""
 
     def __post_init__(self):
```

### Comparing `pyfeyn2-2.2.2/pyfeyn2/interface/dot.py` & `pyfeyn2-2.2.4/pyfeyn2/interface/dot.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.2/pyfeyn2/render/all.py` & `pyfeyn2-2.2.4/pyfeyn2/render/all.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.2/pyfeyn2/render/latex/dot.py` & `pyfeyn2-2.2.4/pyfeyn2/render/latex/dot.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,17 +27,19 @@
     "zigzag": "decorate,decoration=zigzag",
     "phantom": "draw=none",
 }
 
 
 def stylize_connect(fd: FeynmanDiagram, c: Connector) -> str:
     fstyle = fd.get_style(c)
-    style = 'style="{}",texmode="raw"'.format(
-        map_feyn_to_tikz[fstyle.getProperty("line").value]
-    )
+    if fstyle.getProperty("line") is not None:
+        lname = fstyle.getProperty("line").value
+    else:
+        lname = c.type  # fallback to type if no style
+    style = 'style="{}",texmode="raw"'.format(map_feyn_to_tikz[lname])
     if c.label is None:
         label = ""
     else:
         label = c.label.replace("\\", REPLACE_THIS_WITH_A_BACKSLASH)
     if fstyle.getProperty("length") is not None:
         len = fstyle.getProperty("length").value
         style += f",len={len}"
```

### Comparing `pyfeyn2-2.2.2/pyfeyn2/render/latex/feynmp.py` & `pyfeyn2-2.2.4/pyfeyn2/render/latex/feynmp.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import uuid
 from typing import List
 
 from pylatex import Command
 from pylatex.utils import NoEscape
 
+from pyfeyn2 import feynmandiagram
 from pyfeyn2.feynmandiagram import Connector
 from pyfeyn2.render.latex.metapost import MetaPostRender
 
 # converte FeynmanDiagram to tikz-feynman
 
 type_map = {
     "gluon": ["gluon"],
@@ -47,20 +48,21 @@
     "slepton": ["scalar"],
     "squark": ["scalar"],
     "gluino": ["gluon", "plain"],
     "gaugino": ["photon", "plain"],
 }
 
 
-def stylize_line(c: Connector) -> str:
+def stylize_line(fd: feynmandiagram, c: Connector) -> str:
+    cstyle = fd.get_style(c)
     style = ""
     if c.label is not None:
         style += f",label={c.label}"
-    if c.tension is not None:
-        style += f",tension={c.tension}"
+    if cstyle.getProperty("tension") is not None:
+        style += f",tension=" + str(cstyle.getProperty("tension").value)
     return style
 
 
 def feynman_to_feynmp(fd):
     dire = fd.get_style(fd).getProperty("direction").value
     dirin = ""
     dirout = ""
@@ -104,41 +106,50 @@
         for l in outgoing:
             src += f"{l.id},"
         src = src[:-1]
         src += "}\n"
 
     for l in incoming:
         lstyle = fd.get_style(l)
-        tttype = type_map[lstyle.getProperty("line").value]
-        style = stylize_line(l)
+        if lstyle.getProperty("line") is not None:
+            tttype = type_map[lstyle.getProperty("line").value]
+        else:
+            tttype = l.type  # fallback to type if no line style is set
+        style = stylize_line(fd, l)
         for ttype in tttype:
             lid = l.id
             ltarget = l.target
             if l.type.startswith("anti"):
                 lid = l.target
                 ltarget = l.id
             src += f"\t\t\\fmf{{{ttype}{style}}}{{{lid},{ltarget}}}\n"
             style = ""
     for l in outgoing:
         lstyle = fd.get_style(l)
-        tttype = type_map[lstyle.getProperty("line").value]
-        style = stylize_line(l)
+        if lstyle.getProperty("line") is not None:
+            tttype = type_map[lstyle.getProperty("line").value]
+        else:
+            tttype = l.type  # fallback to type if no line style is set
+        style = stylize_line(fd, l)
         for ttype in tttype:
             lid = l.id
             ltarget = l.target
             if l.type.startswith("anti"):
                 lid = l.target
                 ltarget = l.id
             src += f"\t\t\\fmf{{{ttype}{style}}}{{{ltarget},{lid}}}\n"
             style = ""
 
     for p in fd.propagators:
         pstyle = fd.get_style(p)
-        tttype = type_map[pstyle.getProperty("line").value]
-        style = stylize_line(p)
+        if pstyle.getProperty("line") is not None:
+            tttype = type_map[pstyle.getProperty("line").value]
+        else:
+            tttype = p.type  # fallback to type if no line style is set
+        style = stylize_line(fd, p)
         for ttype in tttype:
             psource = p.source
             ptarget = p.target
             if p.type.startswith("anti"):
                 psource = p.target
                 ptarget = p.source
             src += f"\t\t\\fmf{{{ttype}{style}}}{{{psource},{ptarget}}}\n"
@@ -188,8 +199,9 @@
         return super(FeynmpRender, cls).valid_types() + list(type_map.keys())
 
     @classmethod
     def valid_styles(cls) -> bool:
         return super(FeynmpRender, cls).valid_styles() + [
             "line",
             "direction",
+            "tension",
         ]
```

### Comparing `pyfeyn2-2.2.2/pyfeyn2/render/latex/latex.py` & `pyfeyn2-2.2.4/pyfeyn2/render/latex/latex.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.2/pyfeyn2/render/latex/metapost.py` & `pyfeyn2-2.2.4/pyfeyn2/render/latex/metapost.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.2/pyfeyn2/render/latex/tikzfeynman.py` & `pyfeyn2-2.2.4/pyfeyn2/render/latex/tikzfeynman.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,18 @@
     "blob": "blob",
 }
 
 
 def stylize_connect(fd: FeynmanDiagram, c: Connector):
     style = fd.get_style(c)
     ret = ""
-    ret += type_map[style.getProperty("line").value]
+    if style.getProperty("line") is not None:
+        ret += type_map[style.getProperty("line").value]
+    else:
+        ret += type_map[c.type]  # fallback to type if no style
 
     if c.label is not None:
         ret += ",edge label=" + c.label
     # if c.edge_label_ is not None: style += ",edge label'=" + c.edge_label_
     if (
         style.getProperty("momentum-arrow") is not None
         and style.getProperty("momentum-arrow").value == "true"
```

### Comparing `pyfeyn2-2.2.2/pyfeyn2/render/mpl/feynmanrender.py` & `pyfeyn2-2.2.4/pyfeyn2/render/mpl/feynmanrender.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,22 +21,26 @@
     "fermion": [{"style": "simple"}],
     "anti fermion": [{"style": "simple"}],
     "higgs": [{"style": "dashed"}],
     "gaugino": [
         {"style": "wiggly"},
         {"style": "simple"},
     ],
-    "phantom": [],
+    "phantom": [{"style": "simple", "alpha": 0.0}],
 }
 
 
 def get_styled_lines(fd: FeynmanDiagram, p: Union[Propagator, Leg]) -> List[dict]:
     ret = []
     style = fd.get_style(p)
-    for i in namedlines[style.getProperty("line").value]:
+    if style.getProperty("line") is not None:
+        lname = style.getProperty("line").value
+    else:
+        lname = p.type
+    for i in namedlines[lname]:
         d = {**i}
         if style.getProperty("arrow-sense") is not None:
             val = style.getProperty("arrow-sense").value
             if val != 0 and val != "none" and val != "None" and val != "0":
                 d["arrow"] = True
                 d["arrow_param"] = {"direction": float(val)}
                 if style.getProperty("arrow-length") is not None:
@@ -45,14 +49,16 @@
                     )
                 if style.getProperty("arrow-width") is not None:
                     d["arrow_param"]["width"] = float(
                         style.getProperty("arrow-width").value
                     )
                 if style.getProperty("color") is not None:
                     d["arrow_param"]["color"] = style.getProperty("color").value
+            else:
+                d["arrow"] = False
         else:
             d["arrow"] = False
         # copy css style to feynman kwargs dict
         for k in [
             "xamp",
             "yamp",
         ]:
@@ -113,41 +119,48 @@
         ax = fig.add_axes([0, 0, 1, 1], frameon=False)
         diagram = Diagram(ax)
         byid = {}
         for v in self.fd.vertices:
             byid[v.id] = diagram.vertex(
                 xy=((v.x + kickx) * scalex, (v.y + kicky) * scaley)
             )
+            if v.label is not None:
+                byid[v.id].text(v.label)
         for v in self.fd.legs:
             byid[v.id] = diagram.vertex(
                 xy=((v.x + kickx) * scalex, (v.y + kicky) * scaley), marker=""
             )
+            if v.label is not None:
+                byid[v.id].text(v.label)
 
         for p in self.fd.propagators:
+            cur = None
             for style in get_styled_lines(self.fd, p):
                 cur = diagram.line(byid[p.source], byid[p.target], **style)
             if p.label is not None:
                 cur.text(p.label)
         for l in self.fd.legs:
+            cur = None
             for style in get_styled_lines(self.fd, l):
                 if l.sense[:2] == "in":
                     cur = diagram.line(byid[l.id], byid[l.target], **style)
                 elif l.sense[:3] == "out":
                     cur = diagram.line(byid[l.target], byid[l.id], **style)
                 else:
                     raise Exception("Unknown sense")
             if l.label is not None:
                 cur.text(l.label)
 
-        for l in self.fd.labels:
-            diagram.text(
-                l.x,
-                l.y,
-                l.text,
-            )
+        # TODO maybe reintroduce labels
+        # for l in self.fd.labels:
+        #    diagram.text(
+        #        l.x,
+        #        l.y,
+        #        l.text,
+        #    )
         diagram.plot()
         if show:
             plt.show()
         if file is not None:
             plt.savefig(file)
         if clean_up:
             plt.close()
```

### Comparing `pyfeyn2-2.2.2/pyfeyn2/render/pyx/blobs.py` & `pyfeyn2-2.2.4/pyfeyn2/render/pyx/blobs.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.2/pyfeyn2/render/pyx/config.py` & `pyfeyn2-2.2.4/pyfeyn2/render/pyx/config.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.2/pyfeyn2/render/pyx/deco.py` & `pyfeyn2-2.2.4/pyfeyn2/render/pyx/deco.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.2/pyfeyn2/render/pyx/diagrams.py` & `pyfeyn2-2.2.4/pyfeyn2/render/pyx/diagrams.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.2/pyfeyn2/render/pyx/lines.py` & `pyfeyn2-2.2.4/pyfeyn2/render/pyx/lines.py`

 * *Files 2% similar despite different names*

```diff
@@ -376,15 +376,15 @@
                         )
         if config.getOptions().VDEBUG:
             FeynDiagram.currentDiagram.currentCanvas.stroke(vispath, [color.rgb.red])
         # return pyx.path.circle(-2,-1,0.2)
         return vispath
 
     def draw(self, canvas):
-        """Drwa this line on the given canvas."""
+        """Draw this line on the given canvas."""
         path = self.getVisiblePath()
         styles = self.styles + self.arrows
         if config.getOptions().DEBUG:
             print("Drawing " + str(self.__class__) + " with styles = " + str(styles))
             print(path)
         canvas.stroke(path, styles)
         for l in self.labels:
@@ -484,15 +484,23 @@
         arcthrupoint=None,
         is3D=False,
         arrows=None,
         labels=None,
         **kwargs
     ):
         Scalar.__init__(
-            self, point1, point2, styles, arcthrupoint, is3D, arrows, labels, linestyle
+            self,
+            point1=point1,
+            point2=point2,
+            styles=styles,
+            arcthrupoint=arcthrupoint,
+            is3D=is3D,
+            arrows=arrows,
+            labels=labels,
+            linestyle=linestyle,
         )
 
 
 ## DecoratedLine base class
 class DecoratedLine(Line):
     """Base class for spring and sine-like lines"""
 
@@ -751,25 +759,25 @@
             styles,
             arcthrupoint,
             is3D,
             arrows,
             labels,
         )
 
-    def getDeformedPath(self):
+    def getDeformedPath(self, sign=1):
         """Get the path with the decorative deformation."""
         intwindings = int(
             self.frequency
             * pyx.unit.tocm(self.getVisiblePath().arclen())
             / pyx.unit.tocm(self.arcradius)
         )
         intwindings += self.extras
-        sign = 1
+        sign *= 1
         if self.inverted:
-            sign = -1
+            sign *= -1
 
         vispath = self.getVisiblePath()
         # TODO curveradius is not implemented in pyx 0.12
         # curveradii = vispath.curveradius([i / 10.0 for i in range(0, 11)])
         curveradii = []
         mincurveradius = None
         for curveradius in curveradii:
@@ -1177,25 +1185,25 @@
             styles,
             arcthrupoint,
             is3D,
             arrows,
             labels,
         )
 
-    def getDeformedPath(self):
+    def getDeformedPath(self, sign=1):
         """Get the path with the decorative deformation."""
         intwindings = int(
             self.frequency
             * pyx.unit.tocm(self.getVisiblePath().arclen())
             / pyx.unit.tocm(self.arcradius)
         )
         intwindings += self.extras
-        sign = 1
+        sign *= 1
         if self.inverted:
-            sign = -1
+            sign *= -1
         vispath = self.getVisiblePath()
         # TODO curveradius is deprecated in pyx 0.14
         # curveradii = vispath.curveradius([i / 10.0 for i in range(0, 11)])
         curveradii = []
         mincurveradius = None
         for curveradius in curveradii:
             try:
@@ -1283,14 +1291,15 @@
         is3D=False,
         arrows=None,
         labels=None,
         **kwargs
     ):
         """Constructor."""
         DecoratedLine.__init__(
+            self,
             point1,
             point2,
             amplitude,
             frequency,
             extras,
             invert,
             "phantom",
@@ -1298,27 +1307,30 @@
             arcthrupoint,
             is3D,
             arrows,
             labels,
         )
 
     def draw(self, canvas):
-        """Draw the line on the supplied canvas (does nothing for a phantom)."""
+        """Draw the line on the supplied canvas (does nothing for a phantom apart from labels)."""
+        for l in self.labels:
+            l.draw(canvas)
         return
 
 
 # A dictionary for mapping FeynML line types to line classes
 NamedLine = {
-    "higgs": Higgs,
-    "photon": Photon,
-    "vector": Photon,
+    "line": Line,
+    "higgs": Scalar,
+    "photon": Vector,
+    "vector": Vector,
     "gluon": Gluon,
-    "fermion": Fermion,
+    "fermion": Line,
     "graviton": Graviton,
     "gaugino": Gaugino,
     "gluino": Gluino,
     "gravitino": Gravitino,
-    "scalar": Higgs,
+    "scalar": Scalar,
     "ghost": Ghost,
     "phantom": Phantom,
-    "boson": Photon,
+    "boson": Vector,
 }
```

### Comparing `pyfeyn2-2.2.2/pyfeyn2/render/pyx/paint.py` & `pyfeyn2-2.2.4/pyfeyn2/render/pyx/paint.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.2/pyfeyn2/render/pyx/points.py` & `pyfeyn2-2.2.4/pyfeyn2/render/pyx/points.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.2/pyfeyn2/render/pyx/pyxrender.py` & `pyfeyn2-2.2.4/pyfeyn2/render/pyx/pyxrender.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,39 +36,43 @@
             dp = self.apply_layout(v.raw_style(), dp)
             if v.label is not None:
                 dp.setFillstyles(PointLabel(dp, v.label, displace=3, angle=90))
             pyxfd.add(dp)
         for l in self.fd.legs:
             lstyle = self.fd.get_style(l)
             tar = self.fd.get_vertex(l.target)
-            if l.sense[:2] == "in" or l.sense[:8] == "anti-out":
-                nl = NamedLine[lstyle.getProperty("line").value](
-                    Point(l.x, l.y), Point(tar.x, tar.y)
-                )
-            elif l.sense[:3] == "out" or l.sense[:9] == "anti-in":
-                nl = NamedLine[lstyle.getProperty("line").value](
-                    Point(tar.x, tar.y), Point(l.x, l.y)
-                )
+            if lstyle.getProperty("line") is not None:
+                lname = lstyle.getProperty("line").value
+            else:
+                lname = l.type  # fallback to type
+            if l.is_incoming():
+                nl = NamedLine[lname](Point(l.x, l.y), Point(tar.x, tar.y))
+            elif l.is_outgoing():
+                nl = NamedLine[lname](Point(tar.x, tar.y), Point(l.x, l.y))
             if lstyle.getProperty("bend") is not None:
                 nl = nl.bend(lstyle.getProperty("bend").value)
             nl = self.apply_layout(v.raw_style(), nl)
             nl = nl.addLabel(l.label)
 
         for p in self.fd.propagators:
             pstyle = self.fd.get_style(p)
             src = self.fd.get_vertex(p.source)
             tar = self.fd.get_vertex(p.target)
-            nl = NamedLine[pstyle.getProperty("line").value](
-                Point(src.x, src.y), Point(tar.x, tar.y)
-            )
+            if pstyle.getProperty("line") is not None:
+                lname = pstyle.getProperty("line").value
+            else:
+                lname = p.type
+            nl = NamedLine[lname](Point(src.x, src.y), Point(tar.x, tar.y))
+            print(nl, lname)
             if pstyle.getProperty("bend") is not None:
                 nl = nl.bend(pstyle.getProperty("bend").value)
             nl = self.apply_layout(v.raw_style(), nl)
             nl = nl.addLabel(p.label)
         pyxfd.draw(file)
+        print("Drawing to %s" % file)
         wi = WImage(filename=file, resolution=resolution, width=width, height=height)
         if delete:
             os.remove(file)
         if show:
             display(wi)
         if clean_up:
             # TODO: clean up
@@ -202,10 +206,10 @@
 
     @classmethod
     def valid_styles(cls):
         return super(PyxRender, cls).valid_styles() + [
             "line",
             "bend",
             "arrow-pos",
-            "arrow-sense",  #           "parallel-arrow-sense",
-            "arrow-displace",  #           "parallel-arrow-displace",
+            # "arrow-sense",  #           "parallel-arrow-sense",
+            # "arrow-displace",  #           "parallel-arrow-displace",
         ]
```

### Comparing `pyfeyn2-2.2.2/pyfeyn2/render/pyx/utils.py` & `pyfeyn2-2.2.4/pyfeyn2/render/pyx/utils.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.2/pyfeyn2/render/render.py` & `pyfeyn2-2.2.4/pyfeyn2/render/render.py`

 * *Files 12% similar despite different names*

```diff
@@ -61,25 +61,28 @@
     def valid_style(cls, style: str) -> bool:
         return style in cls.valid_styles()
 
     @classmethod
     def valid_attribute(cls, attr: str) -> bool:
         return attr in cls.valid_attributes()
 
-    def demo_propagator(self, d, show=True, label=None):
+    def demo_propagator(self, propagator, show=True, label=None, shape=None, **kwargs):
         v1 = Vertex().with_xy(-2, -2)
         v2 = Vertex().with_xy(2, -2)
+        if shape is not None:
+            v1 = v1.with_shape(shape)
+            v1 = v2.with_shape(shape)
 
         fd = FeynmanDiagram().add(
             v1,
             v2,
             Propagator()
             .connect(v1, v2)
-            .with_type(d)
-            .with_label(label)
+            .with_type(propagator)
+            .with_label(label if label else propagator)
             .with_tension(0.0),
             Leg()
             .with_target(v1)
             .with_point(v1)
             .with_type("phantom")
             .with_incoming()
             .with_length(0.0),
@@ -88,18 +91,23 @@
             .with_point(v2)
             .with_type("phantom")
             .with_outgoing()
             .with_length(0.0),
         )
 
         self.set_feynman_diagram(fd)
-        self.render(show=show)
+        self.render(show=show, **kwargs)
 
-    def demo_vertex(self, d, show=True, label=None):
-        v1 = Vertex().with_xy(0, 0).with_shape(d)  # .set_label(label)
+    def demo_vertex(self, vertex, show=True, label=None):
+        v1 = (
+            Vertex()
+            .with_xy(0, 0)
+            .with_shape(vertex)
+            .with_label(label if label else vertex)
+        )
 
         fd = FeynmanDiagram().add(
             v1,
             Leg().with_target(v1).with_xy(-1, 0).with_type("line").with_incoming(),
             Leg().with_target(v1).with_xy(1, -1).with_type("line").with_incoming(),
             Leg().with_target(v1).with_xy(1, 1).with_type("line").with_outgoing(),
         )
```

### Comparing `pyfeyn2-2.2.2/pyfeyn2/render/text/ascii.py` & `pyfeyn2-2.2.4/pyfeyn2/render/text/ascii.py`

 * *Files 8% similar despite different names*

```diff
@@ -185,34 +185,36 @@
         kicky = -maxy
         fmt = {"scalex": scalex, "kickx": kickx, "scaley": scaley, "kicky": kicky}
 
         for p in self.fd.propagators:
             pstyle = self.fd.get_style(p)
             src = self.fd.get_vertex(p.source)
             tar = self.fd.get_vertex(p.target)
-            self.namedlines[pstyle.getProperty("line").value]().draw(
-                pane, src, tar, **fmt
-            )
+            if pstyle.getProperty("line") is not None:
+                lname = pstyle.getProperty("line").value
+            else:
+                lname = p.type  # fallback no style
+            self.namedlines[lname]().draw(pane, src, tar, **fmt)
             if p.label is not None:
                 self.namedlines["label"](p.label).draw(pane, src, tar, **fmt)
         for l in self.fd.legs:
             lstyle = self.fd.get_style(l)
             tar = self.fd.get_vertex(l.target)
+            if lstyle.getProperty("line") is not None:
+                lname = lstyle.getProperty("line").value
+            else:
+                lname = l.type  # fallback no style
             if l.is_incoming():
-                self.namedlines[lstyle.getProperty("line").value]().draw(
-                    pane, Point(l.x, l.y), tar, **fmt
-                )
+                self.namedlines[lname]().draw(pane, Point(l.x, l.y), tar, **fmt)
                 if l.label is not None:
                     self.namedlines["label"](l.label).draw(
                         pane, Point(l.x, l.y), tar, **fmt
                     )
             elif l.is_outgoing():
-                self.namedlines[lstyle.getProperty("line").value]().draw(
-                    pane, tar, Point(l.x, l.y), **fmt
-                )
+                self.namedlines[lname]().draw(pane, tar, Point(l.x, l.y), **fmt)
                 if l.label is not None:
                     self.namedlines["label"](l.label).draw(
                         pane, tar, Point(l.x, l.y), **fmt
                     )
         for v in self.fd.vertices:
             ssss = self.fd.get_style(v)
             if ssss.getProperty("symbol") is not None:
```

### Comparing `pyfeyn2-2.2.2/pyfeyn2/render/text/asciipdf.py` & `pyfeyn2-2.2.4/pyfeyn2/render/text/asciipdf.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.2/pyfeyn2/render/text/label.py` & `pyfeyn2-2.2.4/pyfeyn2/render/text/label.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.2/pyfeyn2/render/text/line.py` & `pyfeyn2-2.2.4/pyfeyn2/render/text/line.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.2/pyfeyn2/render/text/plainpdf.py` & `pyfeyn2-2.2.4/pyfeyn2/render/text/plainpdf.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.2/pyfeyn2/render/text/style.py` & `pyfeyn2-2.2.4/pyfeyn2/render/text/style.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.2/pyfeyn2/render/text/unicode.py` & `pyfeyn2-2.2.4/pyfeyn2/render/text/unicode.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.2/pyfeyn2/render/text/unicodepdf.py` & `pyfeyn2-2.2.4/pyfeyn2/render/text/unicodepdf.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.2/pyproject.toml` & `pyfeyn2-2.2.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 [tool.poetry]
 name = "pyfeyn2"
-version = "2.2.2"
+version = "2.2.4"
 description = "PyFeyn is a package which makes drawing Feynman diagrams simple and programmatic.  Feynman diagrams are important constructs in perturbative field theory, so being able to draw them in a programmatic fashion is important if attempting to enumerate a large number of diagram configurations is important. The output quality of PyFeyn diagrams (into PDF or EPS formats) is very high, and special effects can be obtained by using constructs from PyX, which PyFeyn is based around"
 authors = ["Alexander Puck Neuwirth <alexander@neuwirth-informatik.de>"]
 readme = "README.md"
 repository = "https://github.com/APN-Pucky/pyfeyn2"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 particle = "*"
 xsdata = {version = "*", extras = ["cli","lxml","soap"]}
 pylatex = "*"
 dot2tex = "*"
-matplotlib = ">=1.4.0"
+matplotlib = ">=1.4.0,<4.0.0"
 Wand = "*"
 numpy = ">=1.6,<1.24" # Upper limit due to feynman using np.complex
-pyx = ">=0.12"
+pyx = ">=0.12,<1.0.0"
 pydot = "*"
-feynman=">=2.0.0"
+feynman="^2.0"
 cssutils= "*"
 pylatexenc = "*"
 pygments = "*"
-pyhepmc = "*"
-pyqgraf = ">=0.0.3"
-#pyqgraf = {path= "../pyqgraf", develop = true }
 graphviz = "*"
 ipyparallel = "*"
 deprecated = "*"
 deprecation = "*"
 cssselect ="*"
 smpl_io = "*"
 smpl_doc = "*"
 smpl_util= "*"
-feynml = ">=0.0.3"
+feynml = {version = ">=0.1.3", extras = ["interface"]}
+#feynml= {path= "../feynml", develop = true }
 
 [tool.poetry.scripts]
 mkfeyndiag = "pyfeyn2.mkfeyndiag:main"
 
 [tool.poetry.group.docs]
 optional = true
```

### Comparing `pyfeyn2-2.2.2/setup.py` & `pyfeyn2-2.2.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,41 +17,39 @@
 install_requires = \
 ['Wand',
  'cssselect',
  'cssutils',
  'deprecated',
  'deprecation',
  'dot2tex',
- 'feynman>=2.0.0',
- 'feynml>=0.0.3',
+ 'feynman>=2.0,<3.0',
+ 'feynml[interface]>=0.1.3',
  'graphviz',
  'ipyparallel',
- 'matplotlib>=1.4.0',
+ 'matplotlib>=1.4.0,<4.0.0',
  'numpy>=1.6,<1.24',
  'particle',
  'pydot',
  'pygments',
- 'pyhepmc',
  'pylatex',
  'pylatexenc',
- 'pyqgraf>=0.0.3',
- 'pyx>=0.12',
+ 'pyx>=0.12,<1.0.0',
  'smpl_doc',
  'smpl_io',
  'smpl_util',
  'xsdata[cli,lxml,soap]']
 
 entry_points = \
 {'console_scripts': ['mkfeyndiag = pyfeyn2.mkfeyndiag:main']}
 
 setup_kwargs = {
     'name': 'pyfeyn2',
-    'version': '2.2.2',
+    'version': '2.2.4',
     'description': 'PyFeyn is a package which makes drawing Feynman diagrams simple and programmatic.  Feynman diagrams are important constructs in perturbative field theory, so being able to draw them in a programmatic fashion is important if attempting to enumerate a large number of diagram configurations is important. The output quality of PyFeyn diagrams (into PDF or EPS formats) is very high, and special effects can be obtained by using constructs from PyX, which PyFeyn is based around',
-    'long_description': "# PyFeyn2\n\nForked from <https://pyfeyn.hepforge.org/> \n\nPyFeyn is a Python-language based system for drawing Feynman diagrams. It was inspired by the C++ FeynDiagram system, and aims to provide the same functionality and quality of output as that, with the added benefits of a modern interpreted language, an improved interface and output direct to both EPS and PDF. Behind the scenes, PyFeyn uses the excellent PyX system - you can use PyX constructs in PyFeyn diagrams if you want, too.\n\n[![PyPI version][pypi image]][pypi link] [![PyPI version][pypi versions]][pypi link]  ![downloads](https://img.shields.io/pypi/dm/smpl.svg)\n\n[![test][a t image]][a t link]      [![Coverage Status][c t i]][c t l]  [![Codacy Badge][cc c i]][cc c l]   [![Codacy Badge][cc q i]][cc q l]  [![Documentation][rtd t i]][rtd t l]\n\n## Dependencies\n\n*   libmagickwand-dev (to display pdfs in a jupyter-notebook, might require a policy change of the imagemagick config for PDFs, see Troubleshooting)\n*   ghostscript\n*   latexmk\n*   (feynmp-auto/feynmf)\n\n## Installation\n\n```sh\npoerty install --with docs --with dev\npoetry shell\n```\n\n## Documentation\n\n*   <https://pyfeyn2.readthedocs.io/en/stable/>\n*   <https://apn-pucky.github.io/pyfeyn2/index.html>\n\n## Similar Feynman diagram rendering project:\n\n*   <https://github.com/ndeutschmann/qgraf-xml-drawer>\n*   <https://github.com/GkAntonius/feynman>\n*   <https://github.com/JP-Ellis/tikz-feynman>\n*   <https://pyfeyn.hepforge.org/> \n*   <https://feynml.hepforge.org/>\n*   <http://www.feyndiagram.com/>\n\nSeveral of these are integrated into pyfeyn2.\n\n## Troubleshooting\n\n*   [ImageMagick security policy 'PDF' blocking conversion]( https://stackoverflow.com/questions/52998331/imagemagick-security-policy-pdf-blocking-conversion )\n\n## Development\n\n\n### package/python structure:\n\n*   <https://mathspp.com/blog/how-to-create-a-python-package-in-2022>\n*   <https://www.brainsorting.com/posts/publish-a-package-on-pypi-using-poetry/>\n\n[doc stable]: https://apn-pucky.github.io/pyfeyn2/index.html\n[doc test]: https://apn-pucky.github.io/pyfeyn2/test/index.html\n\n[pypi image]: https://badge.fury.io/py/pyfeyn2.svg\n[pypi link]: https://pypi.org/project/pyfeyn2/\n[pypi versions]: https://img.shields.io/pypi/pyversions/pyfeyn2.svg\n\n[a s image]: https://github.com/APN-Pucky/pyfeyn2/actions/workflows/stable.yml/badge.svg\n[a s link]: https://github.com/APN-Pucky/pyfeyn2/actions/workflows/stable.yml\n[a t link]: https://github.com/APN-Pucky/pyfeyn2/actions/workflows/test.yml\n[a t image]: https://github.com/APN-Pucky/pyfeyn2/actions/workflows/test.yml/badge.svg\n\n[cc s q i]: https://app.codacy.com/project/badge/Grade/135bae47c6344ab0bfb180135ea1db44?branch=stable\n[cc s q l]: https://www.codacy.com/gh/APN-Pucky/pyfeyn2/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/pyfeyn2&amp;utm_campaign=Badge_Grade?branch=stable\n[cc s c i]: https://app.codacy.com/project/badge/Coverage/135bae47c6344ab0bfb180135ea1db44?branch=stable\n[cc s c l]: https://www.codacy.com/gh/APN-Pucky/smpl/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/pyfeyn2&utm_campaign=Badge_Coverage?branch=stable\n\n[cc q i]: https://app.codacy.com/project/badge/Grade/135bae47c6344ab0bfb180135ea1db44\n[cc q l]: https://www.codacy.com/gh/APN-Pucky/pyfeyn2/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/pyfeyn2&amp;utm_campaign=Badge_Grade\n[cc c i]: https://app.codacy.com/project/badge/Coverage/135bae47c6344ab0bfb180135ea1db44\n[cc c l]: https://www.codacy.com/gh/APN-Pucky/pyfeyn2/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/pyfeyn2&utm_campaign=Badge_Coverage\n\n[c s i]: https://coveralls.io/repos/github/APN-Pucky/pyfeyn2/badge.svg?branch=stable\n[c s l]: https://coveralls.io/github/APN-Pucky/pyfeyn2?branch=stable\n[c t l]: https://coveralls.io/github/APN-Pucky/pyfeyn2?branch=master\n[c t i]: https://coveralls.io/repos/github/APN-Pucky/pyfeyn2/badge.svg?branch=master\n\n[rtd s i]: https://readthedocs.org/projects/pyfeyn2/badge/?version=stable\n[rtd s l]: https://pyfeyn2.readthedocs.io/en/stable/?badge=stable\n[rtd t i]: https://readthedocs.org/projects/pyfeyn2/badge/?version=latest\n[rtd t l]: https://pyfeyn2.readthedocs.io/en/latest/?badge=latest\n",
+    'long_description': "# PyFeyn2\n\nForked from <https://pyfeyn.hepforge.org/> \n\nPyFeyn is a Python-language based system for drawing Feynman diagrams. It was inspired by the C++ FeynDiagram system, and aims to provide the same functionality and quality of output as that, with the added benefits of a modern interpreted language, an improved interface and output direct to both EPS and PDF. Behind the scenes, PyFeyn uses the excellent PyX system - you can use PyX constructs in PyFeyn diagrams if you want, too.\n\n[![PyPI version][pypi image]][pypi link] [![PyPI version][pypi versions]][pypi link]  ![downloads](https://img.shields.io/pypi/dm/pyfeyn2.svg)\n\n[![test][a t image]][a t link]      [![Coverage Status][c t i]][c t l]  [![Codacy Badge][cc c i]][cc c l]   [![Codacy Badge][cc q i]][cc q l]  [![Documentation][rtd t i]][rtd t l]\n\n## Dependencies\n\n*   libmagickwand-dev (to display pdfs in a jupyter-notebook, might require a policy change of the imagemagick config for PDFs, see Troubleshooting)\n*   ghostscript\n*   latexmk\n*   (feynmp-auto/feynmf)\n\n## Installation\n\n```sh\npoerty install --with docs --with dev\npoetry shell\n```\n\n## Documentation\n\n*   <https://pyfeyn2.readthedocs.io/en/stable/>\n*   <https://apn-pucky.github.io/pyfeyn2/index.html>\n\n## Similar Feynman diagram rendering project:\n\n*   <https://github.com/ndeutschmann/qgraf-xml-drawer>\n*   <https://github.com/GkAntonius/feynman>\n*   <https://github.com/JP-Ellis/tikz-feynman>\n*   <https://pyfeyn.hepforge.org/> \n*   <https://feynml.hepforge.org/>\n*   <http://www.feyndiagram.com/>\n\nSeveral of these are integrated into pyfeyn2.\n\n## Troubleshooting\n\n*   [ImageMagick security policy 'PDF' blocking conversion]( https://stackoverflow.com/questions/52998331/imagemagick-security-policy-pdf-blocking-conversion )\n\n## Development\n\n\n### package/python structure:\n\n*   <https://mathspp.com/blog/how-to-create-a-python-package-in-2022>\n*   <https://www.brainsorting.com/posts/publish-a-package-on-pypi-using-poetry/>\n\n[doc stable]: https://apn-pucky.github.io/pyfeyn2/index.html\n[doc test]: https://apn-pucky.github.io/pyfeyn2/test/index.html\n\n[pypi image]: https://badge.fury.io/py/pyfeyn2.svg\n[pypi link]: https://pypi.org/project/pyfeyn2/\n[pypi versions]: https://img.shields.io/pypi/pyversions/pyfeyn2.svg\n\n[a t link]: https://github.com/APN-Pucky/pyfeyn2/actions/workflows/test.yml\n[a t image]: https://github.com/APN-Pucky/pyfeyn2/actions/workflows/test.yml/badge.svg\n\n[cc q i]: https://app.codacy.com/project/badge/Grade/135bae47c6344ab0bfb180135ea1db44\n[cc q l]: https://www.codacy.com/gh/APN-Pucky/pyfeyn2/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/pyfeyn2&amp;utm_campaign=Badge_Grade\n[cc c i]: https://app.codacy.com/project/badge/Coverage/135bae47c6344ab0bfb180135ea1db44\n[cc c l]: https://www.codacy.com/gh/APN-Pucky/pyfeyn2/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/pyfeyn2&utm_campaign=Badge_Coverage\n\n[c t l]: https://coveralls.io/github/APN-Pucky/pyfeyn2?branch=master\n[c t i]: https://coveralls.io/repos/github/APN-Pucky/pyfeyn2/badge.svg?branch=master\n\n[rtd t i]: https://readthedocs.org/projects/pyfeyn2/badge/?version=latest\n[rtd t l]: https://pyfeyn2.readthedocs.io/en/latest/?badge=latest\n",
     'author': 'Alexander Puck Neuwirth',
     'author_email': 'alexander@neuwirth-informatik.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/APN-Pucky/pyfeyn2',
     'packages': packages,
     'package_data': package_data,
```

