# Comparing `tmp/pyfeyn2-2.2.5.tar.gz` & `tmp/pyfeyn2-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfeyn2-2.2.5.tar", max compression
+gzip compressed data, was "pyfeyn2-2.2.6.tar", max compression
```

## Comparing `pyfeyn2-2.2.5.tar` & `pyfeyn2-2.2.6.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    35149 2023-04-12 13:07:48.890074 pyfeyn2-2.2.5/LICENSE
--rw-r--r--   0        0        0     3226 2023-04-12 13:07:48.890074 pyfeyn2-2.2.5/README.md
--rw-r--r--   0        0        0      154 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/auto/__init__.py
--rw-r--r--   0        0        0     2841 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/auto/bend.py
--rw-r--r--   0        0        0      774 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/auto/label.py
--rw-r--r--   0        0        0     2073 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/auto/position.py
--rw-r--r--   0        0        0        0 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/auto/reshuffle.py
--rw-r--r--   0        0        0      680 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/feynmandiagram.py
--rw-r--r--   0        0        0     2305 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/interface/dot.py
--rw-r--r--   0        0        0       85 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/interface/hepmc.py
--rw-r--r--   0        0        0       85 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/interface/qgraf.py
--rw-r--r--   0        0        0      169 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/mkfeyndiag.py
--rw-r--r--   0        0        0        0 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/__init__.py
--rw-r--r--   0        0        0     3651 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/all.py
--rw-r--r--   0        0        0        0 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/latex/__init__.py
--rw-r--r--   0        0        0     3492 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/latex/dot.py
--rw-r--r--   0        0        0     5921 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/latex/feynmp.py
--rw-r--r--   0        0        0     1616 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/latex/latex.py
--rw-r--r--   0        0        0     2407 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/latex/metapost.py
--rw-r--r--   0        0        0     6302 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/latex/tikzfeynman.py
--rw-r--r--   0        0        0     6026 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/mpl/feynmanrender.py
--rw-r--r--   0        0        0        0 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/pyx/__init__.py
--rw-r--r--   0        0        0     7132 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/pyx/blobs.py
--rw-r--r--   0        0        0     1319 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/pyx/config.py
--rw-r--r--   0        0        0    13169 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/pyx/deco.py
--rw-r--r--   0        0        0     2561 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/pyx/diagrams.py
--rw-r--r--   0        0        0    41301 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/pyx/lines.py
--rw-r--r--   0        0        0     3549 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/pyx/paint.py
--rw-r--r--   0        0        0    12623 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/pyx/points.py
--rw-r--r--   0        0        0     8043 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/pyx/pyxrender.py
--rw-r--r--   0        0        0     1501 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/pyx/utils.py
--rw-r--r--   0        0        0     2914 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/render.py
--rw-r--r--   0        0        0     7120 2023-04-12 13:07:48.978074 pyfeyn2-2.2.5/pyfeyn2/render/text/ascii.py
--rw-r--r--   0        0        0      745 2023-04-12 13:07:48.978074 pyfeyn2-2.2.5/pyfeyn2/render/text/asciipdf.py
--rw-r--r--   0        0        0     2228 2023-04-12 13:07:48.978074 pyfeyn2-2.2.5/pyfeyn2/render/text/label.py
--rw-r--r--   0        0        0     1547 2023-04-12 13:07:48.978074 pyfeyn2-2.2.5/pyfeyn2/render/text/line.py
--rw-r--r--   0        0        0     1502 2023-04-12 13:07:48.978074 pyfeyn2-2.2.5/pyfeyn2/render/text/plainpdf.py
--rw-r--r--   0        0        0      483 2023-04-12 13:07:48.978074 pyfeyn2-2.2.5/pyfeyn2/render/text/point.py
--rw-r--r--   0        0        0     3846 2023-04-12 13:07:48.978074 pyfeyn2-2.2.5/pyfeyn2/render/text/style.py
--rw-r--r--   0        0        0     1401 2023-04-12 13:07:48.978074 pyfeyn2-2.2.5/pyfeyn2/render/text/unicode.py
--rw-r--r--   0        0        0     1858 2023-04-12 13:07:48.978074 pyfeyn2-2.2.5/pyfeyn2/render/text/unicodepdf.py
--rw-r--r--   0        0        0     2480 2023-04-12 13:07:51.842085 pyfeyn2-2.2.5/pyproject.toml
--rw-r--r--   0        0        0     5016 1970-01-01 00:00:00.000000 pyfeyn2-2.2.5/setup.py
--rw-r--r--   0        0        0     4886 1970-01-01 00:00:00.000000 pyfeyn2-2.2.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-12 17:41:17.301008 pyfeyn2-2.2.6/LICENSE
+-rw-r--r--   0        0        0     3115 2023-04-12 17:41:17.301008 pyfeyn2-2.2.6/README.md
+-rw-r--r--   0        0        0      154 2023-04-12 17:41:17.377009 pyfeyn2-2.2.6/pyfeyn2/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 17:41:17.377009 pyfeyn2-2.2.6/pyfeyn2/auto/__init__.py
+-rw-r--r--   0        0        0     2841 2023-04-12 17:41:17.377009 pyfeyn2-2.2.6/pyfeyn2/auto/bend.py
+-rw-r--r--   0        0        0      774 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/auto/label.py
+-rw-r--r--   0        0        0     2073 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/auto/position.py
+-rw-r--r--   0        0        0        0 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/auto/reshuffle.py
+-rw-r--r--   0        0        0     3332 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/feynmandiagram.py
+-rw-r--r--   0        0        0     2742 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/interface/dot.py
+-rw-r--r--   0        0        0      273 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/interface/hepmc.py
+-rw-r--r--   0        0        0      238 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/interface/qgraf.py
+-rw-r--r--   0        0        0      169 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/mkfeyndiag.py
+-rw-r--r--   0        0        0        0 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/__init__.py
+-rw-r--r--   0        0        0     3651 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/all.py
+-rw-r--r--   0        0        0        0 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/latex/__init__.py
+-rw-r--r--   0        0        0     3494 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/latex/dot.py
+-rw-r--r--   0        0        0     5920 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/latex/feynmp.py
+-rw-r--r--   0        0        0     1616 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/latex/latex.py
+-rw-r--r--   0        0        0     2407 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/latex/metapost.py
+-rw-r--r--   0        0        0     6302 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/latex/tikzfeynman.py
+-rw-r--r--   0        0        0     6026 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/mpl/feynmanrender.py
+-rw-r--r--   0        0        0        0 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/pyx/__init__.py
+-rw-r--r--   0        0        0     7132 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/pyx/blobs.py
+-rw-r--r--   0        0        0     1319 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/pyx/config.py
+-rw-r--r--   0        0        0    13169 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/pyx/deco.py
+-rw-r--r--   0        0        0     2561 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/pyx/diagrams.py
+-rw-r--r--   0        0        0    41341 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/pyx/lines.py
+-rw-r--r--   0        0        0     3549 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/pyx/paint.py
+-rw-r--r--   0        0        0    12623 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/pyx/points.py
+-rw-r--r--   0        0        0     8043 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/pyx/pyxrender.py
+-rw-r--r--   0        0        0     1501 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/pyx/utils.py
+-rw-r--r--   0        0        0     2914 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/render.py
+-rw-r--r--   0        0        0     7120 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/text/ascii.py
+-rw-r--r--   0        0        0      745 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/text/asciipdf.py
+-rw-r--r--   0        0        0     2228 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/text/label.py
+-rw-r--r--   0        0        0     1547 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/text/line.py
+-rw-r--r--   0        0        0     1502 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/text/plainpdf.py
+-rw-r--r--   0        0        0      483 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/text/point.py
+-rw-r--r--   0        0        0     3846 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/text/style.py
+-rw-r--r--   0        0        0     1401 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/text/unicode.py
+-rw-r--r--   0        0        0     1858 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/text/unicodepdf.py
+-rw-r--r--   0        0        0     2480 2023-04-12 17:41:19.381020 pyfeyn2-2.2.6/pyproject.toml
+-rw-r--r--   0        0        0     4903 1970-01-01 00:00:00.000000 pyfeyn2-2.2.6/setup.py
+-rw-r--r--   0        0        0     4775 1970-01-01 00:00:00.000000 pyfeyn2-2.2.6/PKG-INFO
```

### Comparing `pyfeyn2-2.2.5/LICENSE` & `pyfeyn2-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.5/README.md` & `pyfeyn2-2.2.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 [![test][a t image]][a t link]      [![Coverage Status][c t i]][c t l]  [![Codacy Badge][cc c i]][cc c l]   [![Codacy Badge][cc q i]][cc q l]  [![Documentation][rtd t i]][rtd t l]
 
 ## Dependencies
 
 *   libmagickwand-dev (to display pdfs in a jupyter-notebook, might require a policy change of the imagemagick config for PDFs, see Troubleshooting)
 *   ghostscript
 *   latexmk
+*   (graphviz)
 *   (feynmp-auto/feynmf)
 
 ## Installation
 
 ```sh
 poerty install --with docs --with dev
 poetry shell
@@ -46,17 +47,14 @@
 
 
 ### package/python structure:
 
 *   <https://mathspp.com/blog/how-to-create-a-python-package-in-2022>
 *   <https://www.brainsorting.com/posts/publish-a-package-on-pypi-using-poetry/>
 
-[doc stable]: https://apn-pucky.github.io/pyfeyn2/index.html
-[doc test]: https://apn-pucky.github.io/pyfeyn2/test/index.html
-
 [pypi image]: https://badge.fury.io/py/pyfeyn2.svg
 [pypi link]: https://pypi.org/project/pyfeyn2/
 [pypi versions]: https://img.shields.io/pypi/pyversions/pyfeyn2.svg
 
 [a t link]: https://github.com/APN-Pucky/pyfeyn2/actions/workflows/test.yml
 [a t image]: https://github.com/APN-Pucky/pyfeyn2/actions/workflows/test.yml/badge.svg
```

### Comparing `pyfeyn2-2.2.5/pyfeyn2/auto/bend.py` & `pyfeyn2-2.2.6/pyfeyn2/auto/bend.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.5/pyfeyn2/auto/label.py` & `pyfeyn2-2.2.6/pyfeyn2/auto/label.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.5/pyfeyn2/auto/position.py` & `pyfeyn2-2.2.6/pyfeyn2/auto/position.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.5/pyfeyn2/interface/dot.py` & `pyfeyn2-2.2.6/pyfeyn2/interface/dot.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,62 +1,83 @@
+from warnings import warn
+
 import dot2tex
 
 REPLACE_THIS_WITH_A_BACKSLASH = "¬"
 
 
 def _fake_styler(fd, p):
     return 'style="draw=none"'
 
 
-def feynman_to_dot(fd, resubstituteslash=True, styler=_fake_styler):
-    # TODO better use pydot? still alive? or grpahviz?
-    fdstyle = fd.get_style(fd)
+def get_rankdir(fdstyle):
     rankdir = None
-    rdir = fdstyle.getProperty("direction").value
-    if rdir == "right":
+    if fdstyle.getProperty("direction") is not None:
+        warn("direction is unknwon, using default of 'right'")
         rankdir = "LR"
-    elif rdir == "left":
-        rankdir = "RL"
-    elif rdir == "down":
-        rankdir = "TB"
-    elif rdir == "up":
-        rankdir = "BT"
     else:
-        raise Exception(f"Unknown direction: {rdir}")
-    layout = fdstyle.getProperty("layout").value
+        rdir = fdstyle.getProperty("direction").value
+        if rdir == "right":
+            rankdir = "LR"
+        elif rdir == "left":
+            rankdir = "RL"
+        elif rdir == "down":
+            rankdir = "TB"
+        elif rdir == "up":
+            rankdir = "BT"
+        else:
+            raise Exception(f"Unknown direction: {rdir}")
+    return rankdir
+
+
+def get_layout(fdstyle):
+    layout = None
+    if fdstyle.getProperty("layout") is not None:
+        warn("layout is unknwon, using default of 'dot'")
+        layout = "dot"
+    else:
+        layout = fdstyle.getProperty("layout").value
+    return layout
+
+
+def feynman_to_dot(fd, resubstituteslash=True, styler=_fake_styler):
+    # TODO better use pydot? still alive? or grpahviz?
+    fdstyle = fd.get_style(fd)
+    rankdir = get_rankdir(fdstyle)
+    layout = get_layout(fdstyle)
 
     thestyle = ""
     src = "graph G {\n"
     src += f"rankdir={rankdir};\n"
     src += f"layout={layout};\n"
     # src += "mode=hier;\n"
     src += 'node [style="invis"];\n'
-    for l in fd.legs:
-        if l.x is not None and l.y is not None:
-            src += f'\t\t{l.id} [ pos="{l.x},{l.y}!"];\n'
-    for l in fd.vertices:
+    # nodes
+    for l in fd.legs + fd.vertices:
         if l.x is not None and l.y is not None:
             src += f'\t\t{l.id} [ pos="{l.x},{l.y}!"];\n'
+    # edges
     for p in fd.propagators:
         if styler is not None:
             thestyle = styler(fd, p)
-        src += "edge [{}];\n".format(thestyle)
+        src += f"edge [{thestyle}];\n"
         src += f"\t\t{p.source} -- {p.target};\n"
     rank_in = "{rank=min; "
     rank_out = "{rank=max; "
 
+    # edges
     for l in fd.legs:
         if styler is not None:
             thestyle = styler(fd, l)
         if l.sense == "incoming":
-            src += "edge [{}];\n".format(thestyle)
+            src += f"edge [{thestyle}];\n"
             src += f"\t\t{l.id} -- {l.target};\n"
             rank_in += f"{l.id} "
         elif l.sense == "outgoing":
-            src += "edge [{}];\n".format(thestyle)
+            src += f"edge [{thestyle}];\n"
             src += f"\t\t{l.target} -- {l.id};\n"
             rank_out += f"{l.id} ;"
         else:
             # TODO maybe not error but just use the default
             raise Exception("Unknown sense")
     src += rank_in + "}\n"
     src += rank_out + "}\n"
```

### Comparing `pyfeyn2-2.2.5/pyfeyn2/render/all.py` & `pyfeyn2-2.2.6/pyfeyn2/render/all.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.5/pyfeyn2/render/latex/dot.py` & `pyfeyn2-2.2.6/pyfeyn2/render/latex/dot.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,16 +37,16 @@
         lname = c.type  # fallback to type if no style
     style = 'style="{}",texmode="raw"'.format(map_feyn_to_tikz[lname])
     if c.label is None:
         label = ""
     else:
         label = c.label.replace("\\", REPLACE_THIS_WITH_A_BACKSLASH)
     if fstyle.getProperty("length") is not None:
-        len = fstyle.getProperty("length").value
-        style += f",len={len}"
+        leng = fstyle.getProperty("length").value
+        style += f",len={leng}"
     style += f',label="{label}"'
     return style
 
 
 class DotRender(LatexRender):
     def __init__(
         self,
```

### Comparing `pyfeyn2-2.2.5/pyfeyn2/render/latex/feynmp.py` & `pyfeyn2-2.2.6/pyfeyn2/render/latex/feynmp.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 def stylize_line(fd: feynmandiagram, c: Connector) -> str:
     cstyle = fd.get_style(c)
     style = ""
     if c.label is not None:
         style += f",label={c.label}"
     if cstyle.getProperty("tension") is not None:
-        style += f",tension=" + str(cstyle.getProperty("tension").value)
+        style += ",tension=" + str(cstyle.getProperty("tension").value)
     return style
 
 
 def feynman_to_feynmp(fd):
     dire = fd.get_style(fd).getProperty("direction").value
     dirin = ""
     dirout = ""
```

### Comparing `pyfeyn2-2.2.5/pyfeyn2/render/latex/latex.py` & `pyfeyn2-2.2.6/pyfeyn2/render/latex/latex.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.5/pyfeyn2/render/latex/metapost.py` & `pyfeyn2-2.2.6/pyfeyn2/render/latex/metapost.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.5/pyfeyn2/render/latex/tikzfeynman.py` & `pyfeyn2-2.2.6/pyfeyn2/render/latex/tikzfeynman.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.5/pyfeyn2/render/mpl/feynmanrender.py` & `pyfeyn2-2.2.6/pyfeyn2/render/mpl/feynmanrender.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.5/pyfeyn2/render/pyx/blobs.py` & `pyfeyn2-2.2.6/pyfeyn2/render/pyx/blobs.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.5/pyfeyn2/render/pyx/config.py` & `pyfeyn2-2.2.6/pyfeyn2/render/pyx/config.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.5/pyfeyn2/render/pyx/deco.py` & `pyfeyn2-2.2.6/pyfeyn2/render/pyx/deco.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.5/pyfeyn2/render/pyx/diagrams.py` & `pyfeyn2-2.2.6/pyfeyn2/render/pyx/diagrams.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.5/pyfeyn2/render/pyx/lines.py` & `pyfeyn2-2.2.6/pyfeyn2/render/pyx/lines.py`

 * *Files 1% similar despite different names*

```diff
@@ -559,15 +559,15 @@
         return self
 
     def setExtraCycles(self, extras):
         """Add some extra (possibly negative) cycles to the oscillation."""
         self.extras = extras
         return self
 
-    def getDeformedPath(self):
+    def getDeformedPath(self, sign=1):
         """Get the deformed path."""
         return self.getVisiblePath()
 
 
 class Gluon(DecoratedLine):
     """A line with a cycloid deformation"""
 
@@ -599,15 +599,15 @@
             styles,
             arcthrupoint,
             is3D,
             arrows,
             labels,
         )
 
-    def getDeformedPath(self):
+    def getDeformedPath(self, sign=1):
         """Get the path modified by the coil warping."""
         needwindings = (
             self.frequency
             * pyx.unit.tocm(self.getVisiblePath().arclen())
             / pyx.unit.tocm(self.arcradius)
         )
         ## Get the whole number of windings and make sure that it's odd so we
@@ -688,15 +688,15 @@
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
@@ -896,15 +896,15 @@
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
@@ -1031,15 +1031,15 @@
             styles,
             arcthrupoint,
             is3D,
             arrows,
             labels,
         )
 
-    def getDeformedPath(self):
+    def getDeformedPath(self, sign=1):
         """Get the path with the decorative deformation."""
         needwindings = (
             self.frequency
             * pyx.unit.tocm(self.getVisiblePath().arclen())
             / pyx.unit.tocm(self.arcradius)
         )
         ## Get the whole number of windings and make sure that it's odd so we
```

### Comparing `pyfeyn2-2.2.5/pyfeyn2/render/pyx/paint.py` & `pyfeyn2-2.2.6/pyfeyn2/render/pyx/paint.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.5/pyfeyn2/render/pyx/points.py` & `pyfeyn2-2.2.6/pyfeyn2/render/pyx/points.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.5/pyfeyn2/render/pyx/pyxrender.py` & `pyfeyn2-2.2.6/pyfeyn2/render/pyx/pyxrender.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.5/pyfeyn2/render/pyx/utils.py` & `pyfeyn2-2.2.6/pyfeyn2/render/pyx/utils.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.5/pyfeyn2/render/render.py` & `pyfeyn2-2.2.6/pyfeyn2/render/render.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.5/pyfeyn2/render/text/ascii.py` & `pyfeyn2-2.2.6/pyfeyn2/render/text/ascii.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.5/pyfeyn2/render/text/asciipdf.py` & `pyfeyn2-2.2.6/pyfeyn2/render/text/asciipdf.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.5/pyfeyn2/render/text/label.py` & `pyfeyn2-2.2.6/pyfeyn2/render/text/label.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.5/pyfeyn2/render/text/line.py` & `pyfeyn2-2.2.6/pyfeyn2/render/text/line.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.5/pyfeyn2/render/text/plainpdf.py` & `pyfeyn2-2.2.6/pyfeyn2/render/text/plainpdf.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.5/pyfeyn2/render/text/style.py` & `pyfeyn2-2.2.6/pyfeyn2/render/text/style.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.5/pyfeyn2/render/text/unicode.py` & `pyfeyn2-2.2.6/pyfeyn2/render/text/unicode.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.5/pyfeyn2/render/text/unicodepdf.py` & `pyfeyn2-2.2.6/pyfeyn2/render/text/unicodepdf.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.5/pyproject.toml` & `pyfeyn2-2.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyfeyn2"
-version = "2.2.5"
+version = "2.2.6"
 description = "PyFeyn is a package which makes drawing Feynman diagrams simple and programmatic.  Feynman diagrams are important constructs in perturbative field theory, so being able to draw them in a programmatic fashion is important if attempting to enumerate a large number of diagram configurations is important. The output quality of PyFeyn diagrams (into PDF or EPS formats) is very high, and special effects can be obtained by using constructs from PyX, which PyFeyn is based around"
 authors = ["Alexander Puck Neuwirth <alexander@neuwirth-informatik.de>"]
 readme = "README.md"
 repository = "https://github.com/APN-Pucky/pyfeyn2"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `pyfeyn2-2.2.5/setup.py` & `pyfeyn2-2.2.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,17 +39,17 @@
  'xsdata[cli,lxml,soap]']
 
 entry_points = \
 {'console_scripts': ['mkfeyndiag = pyfeyn2.mkfeyndiag:main']}
 
 setup_kwargs = {
     'name': 'pyfeyn2',
-    'version': '2.2.5',
+    'version': '2.2.6',
     'description': 'PyFeyn is a package which makes drawing Feynman diagrams simple and programmatic.  Feynman diagrams are important constructs in perturbative field theory, so being able to draw them in a programmatic fashion is important if attempting to enumerate a large number of diagram configurations is important. The output quality of PyFeyn diagrams (into PDF or EPS formats) is very high, and special effects can be obtained by using constructs from PyX, which PyFeyn is based around',
-    'long_description': "# PyFeyn2\n\nForked from <https://pyfeyn.hepforge.org/> \n\nPyFeyn is a Python-language based system for drawing Feynman diagrams. It was inspired by the C++ FeynDiagram system, and aims to provide the same functionality and quality of output as that, with the added benefits of a modern interpreted language, an improved interface and output direct to both EPS and PDF. Behind the scenes, PyFeyn uses the excellent PyX system - you can use PyX constructs in PyFeyn diagrams if you want, too.\n\n[![PyPI version][pypi image]][pypi link] [![PyPI version][pypi versions]][pypi link]  ![downloads](https://img.shields.io/pypi/dm/pyfeyn2.svg)\n\n[![test][a t image]][a t link]      [![Coverage Status][c t i]][c t l]  [![Codacy Badge][cc c i]][cc c l]   [![Codacy Badge][cc q i]][cc q l]  [![Documentation][rtd t i]][rtd t l]\n\n## Dependencies\n\n*   libmagickwand-dev (to display pdfs in a jupyter-notebook, might require a policy change of the imagemagick config for PDFs, see Troubleshooting)\n*   ghostscript\n*   latexmk\n*   (feynmp-auto/feynmf)\n\n## Installation\n\n```sh\npoerty install --with docs --with dev\npoetry shell\n```\n\n## Documentation\n\n*   <https://pyfeyn2.readthedocs.io/en/stable/>\n*   <https://apn-pucky.github.io/pyfeyn2/index.html>\n\n## Similar Feynman diagram rendering project:\n\n*   <https://github.com/ndeutschmann/qgraf-xml-drawer>\n*   <https://github.com/GkAntonius/feynman>\n*   <https://github.com/JP-Ellis/tikz-feynman>\n*   <https://pyfeyn.hepforge.org/> \n*   <https://feynml.hepforge.org/>\n*   <http://www.feyndiagram.com/>\n\nSeveral of these are integrated into pyfeyn2.\n\n## Troubleshooting\n\n*   [ImageMagick security policy 'PDF' blocking conversion]( https://stackoverflow.com/questions/52998331/imagemagick-security-policy-pdf-blocking-conversion )\n\n## Development\n\n\n### package/python structure:\n\n*   <https://mathspp.com/blog/how-to-create-a-python-package-in-2022>\n*   <https://www.brainsorting.com/posts/publish-a-package-on-pypi-using-poetry/>\n\n[doc stable]: https://apn-pucky.github.io/pyfeyn2/index.html\n[doc test]: https://apn-pucky.github.io/pyfeyn2/test/index.html\n\n[pypi image]: https://badge.fury.io/py/pyfeyn2.svg\n[pypi link]: https://pypi.org/project/pyfeyn2/\n[pypi versions]: https://img.shields.io/pypi/pyversions/pyfeyn2.svg\n\n[a t link]: https://github.com/APN-Pucky/pyfeyn2/actions/workflows/test.yml\n[a t image]: https://github.com/APN-Pucky/pyfeyn2/actions/workflows/test.yml/badge.svg\n\n[cc q i]: https://app.codacy.com/project/badge/Grade/135bae47c6344ab0bfb180135ea1db44\n[cc q l]: https://www.codacy.com/gh/APN-Pucky/pyfeyn2/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/pyfeyn2&amp;utm_campaign=Badge_Grade\n[cc c i]: https://app.codacy.com/project/badge/Coverage/135bae47c6344ab0bfb180135ea1db44\n[cc c l]: https://www.codacy.com/gh/APN-Pucky/pyfeyn2/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/pyfeyn2&utm_campaign=Badge_Coverage\n\n[c t l]: https://coveralls.io/github/APN-Pucky/pyfeyn2?branch=master\n[c t i]: https://coveralls.io/repos/github/APN-Pucky/pyfeyn2/badge.svg?branch=master\n\n[rtd t i]: https://readthedocs.org/projects/pyfeyn2/badge/?version=latest\n[rtd t l]: https://pyfeyn2.readthedocs.io/en/latest/?badge=latest\n",
+    'long_description': "# PyFeyn2\n\nForked from <https://pyfeyn.hepforge.org/> \n\nPyFeyn is a Python-language based system for drawing Feynman diagrams. It was inspired by the C++ FeynDiagram system, and aims to provide the same functionality and quality of output as that, with the added benefits of a modern interpreted language, an improved interface and output direct to both EPS and PDF. Behind the scenes, PyFeyn uses the excellent PyX system - you can use PyX constructs in PyFeyn diagrams if you want, too.\n\n[![PyPI version][pypi image]][pypi link] [![PyPI version][pypi versions]][pypi link]  ![downloads](https://img.shields.io/pypi/dm/pyfeyn2.svg)\n\n[![test][a t image]][a t link]      [![Coverage Status][c t i]][c t l]  [![Codacy Badge][cc c i]][cc c l]   [![Codacy Badge][cc q i]][cc q l]  [![Documentation][rtd t i]][rtd t l]\n\n## Dependencies\n\n*   libmagickwand-dev (to display pdfs in a jupyter-notebook, might require a policy change of the imagemagick config for PDFs, see Troubleshooting)\n*   ghostscript\n*   latexmk\n*   (graphviz)\n*   (feynmp-auto/feynmf)\n\n## Installation\n\n```sh\npoerty install --with docs --with dev\npoetry shell\n```\n\n## Documentation\n\n*   <https://pyfeyn2.readthedocs.io/en/stable/>\n*   <https://apn-pucky.github.io/pyfeyn2/index.html>\n\n## Similar Feynman diagram rendering project:\n\n*   <https://github.com/ndeutschmann/qgraf-xml-drawer>\n*   <https://github.com/GkAntonius/feynman>\n*   <https://github.com/JP-Ellis/tikz-feynman>\n*   <https://pyfeyn.hepforge.org/> \n*   <https://feynml.hepforge.org/>\n*   <http://www.feyndiagram.com/>\n\nSeveral of these are integrated into pyfeyn2.\n\n## Troubleshooting\n\n*   [ImageMagick security policy 'PDF' blocking conversion]( https://stackoverflow.com/questions/52998331/imagemagick-security-policy-pdf-blocking-conversion )\n\n## Development\n\n\n### package/python structure:\n\n*   <https://mathspp.com/blog/how-to-create-a-python-package-in-2022>\n*   <https://www.brainsorting.com/posts/publish-a-package-on-pypi-using-poetry/>\n\n[pypi image]: https://badge.fury.io/py/pyfeyn2.svg\n[pypi link]: https://pypi.org/project/pyfeyn2/\n[pypi versions]: https://img.shields.io/pypi/pyversions/pyfeyn2.svg\n\n[a t link]: https://github.com/APN-Pucky/pyfeyn2/actions/workflows/test.yml\n[a t image]: https://github.com/APN-Pucky/pyfeyn2/actions/workflows/test.yml/badge.svg\n\n[cc q i]: https://app.codacy.com/project/badge/Grade/135bae47c6344ab0bfb180135ea1db44\n[cc q l]: https://www.codacy.com/gh/APN-Pucky/pyfeyn2/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/pyfeyn2&amp;utm_campaign=Badge_Grade\n[cc c i]: https://app.codacy.com/project/badge/Coverage/135bae47c6344ab0bfb180135ea1db44\n[cc c l]: https://www.codacy.com/gh/APN-Pucky/pyfeyn2/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/pyfeyn2&utm_campaign=Badge_Coverage\n\n[c t l]: https://coveralls.io/github/APN-Pucky/pyfeyn2?branch=master\n[c t i]: https://coveralls.io/repos/github/APN-Pucky/pyfeyn2/badge.svg?branch=master\n\n[rtd t i]: https://readthedocs.org/projects/pyfeyn2/badge/?version=latest\n[rtd t l]: https://pyfeyn2.readthedocs.io/en/latest/?badge=latest\n",
     'author': 'Alexander Puck Neuwirth',
     'author_email': 'alexander@neuwirth-informatik.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/APN-Pucky/pyfeyn2',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pyfeyn2-2.2.5/PKG-INFO` & `pyfeyn2-2.2.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfeyn2
-Version: 2.2.5
+Version: 2.2.6
 Summary: PyFeyn is a package which makes drawing Feynman diagrams simple and programmatic.  Feynman diagrams are important constructs in perturbative field theory, so being able to draw them in a programmatic fashion is important if attempting to enumerate a large number of diagram configurations is important. The output quality of PyFeyn diagrams (into PDF or EPS formats) is very high, and special effects can be obtained by using constructs from PyX, which PyFeyn is based around
 Home-page: https://github.com/APN-Pucky/pyfeyn2
 Author: Alexander Puck Neuwirth
 Author-email: alexander@neuwirth-informatik.de
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -47,14 +47,15 @@
 [![test][a t image]][a t link]      [![Coverage Status][c t i]][c t l]  [![Codacy Badge][cc c i]][cc c l]   [![Codacy Badge][cc q i]][cc q l]  [![Documentation][rtd t i]][rtd t l]
 
 ## Dependencies
 
 *   libmagickwand-dev (to display pdfs in a jupyter-notebook, might require a policy change of the imagemagick config for PDFs, see Troubleshooting)
 *   ghostscript
 *   latexmk
+*   (graphviz)
 *   (feynmp-auto/feynmf)
 
 ## Installation
 
 ```sh
 poerty install --with docs --with dev
 poetry shell
@@ -84,17 +85,14 @@
 
 
 ### package/python structure:
 
 *   <https://mathspp.com/blog/how-to-create-a-python-package-in-2022>
 *   <https://www.brainsorting.com/posts/publish-a-package-on-pypi-using-poetry/>
 
-[doc stable]: https://apn-pucky.github.io/pyfeyn2/index.html
-[doc test]: https://apn-pucky.github.io/pyfeyn2/test/index.html
-
 [pypi image]: https://badge.fury.io/py/pyfeyn2.svg
 [pypi link]: https://pypi.org/project/pyfeyn2/
 [pypi versions]: https://img.shields.io/pypi/pyversions/pyfeyn2.svg
 
 [a t link]: https://github.com/APN-Pucky/pyfeyn2/actions/workflows/test.yml
 [a t image]: https://github.com/APN-Pucky/pyfeyn2/actions/workflows/test.yml/badge.svg
```

