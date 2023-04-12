# Comparing `tmp/pyfeyn2-2.2.4.tar.gz` & `tmp/pyfeyn2-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfeyn2-2.2.4.tar", max compression
+gzip compressed data, was "pyfeyn2-2.2.5.tar", max compression
```

## Comparing `pyfeyn2-2.2.4.tar` & `pyfeyn2-2.2.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    35149 2023-04-12 08:31:25.170839 pyfeyn2-2.2.4/LICENSE
--rw-r--r--   0        0        0     3226 2023-04-12 08:31:25.170839 pyfeyn2-2.2.4/README.md
--rw-r--r--   0        0        0      154 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/auto/__init__.py
--rw-r--r--   0        0        0     2841 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/auto/bend.py
--rw-r--r--   0        0        0      774 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/auto/label.py
--rw-r--r--   0        0        0     2073 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/auto/position.py
--rw-r--r--   0        0        0        0 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/auto/reshuffle.py
--rw-r--r--   0        0        0      680 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/feynmandiagram.py
--rw-r--r--   0        0        0     2305 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/interface/dot.py
--rw-r--r--   0        0        0       85 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/interface/hepmc.py
--rw-r--r--   0        0        0       85 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/interface/qgraf.py
--rw-r--r--   0        0        0      169 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/mkfeyndiag.py
--rw-r--r--   0        0        0        0 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/__init__.py
--rw-r--r--   0        0        0     3651 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/all.py
--rw-r--r--   0        0        0        0 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/latex/__init__.py
--rw-r--r--   0        0        0     3492 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/latex/dot.py
--rw-r--r--   0        0        0     6203 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/latex/feynmp.py
--rw-r--r--   0        0        0     1616 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/latex/latex.py
--rw-r--r--   0        0        0     2407 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/latex/metapost.py
--rw-r--r--   0        0        0     6302 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/latex/tikzfeynman.py
--rw-r--r--   0        0        0     6026 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/mpl/feynmanrender.py
--rw-r--r--   0        0        0        0 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/pyx/__init__.py
--rw-r--r--   0        0        0     7132 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/pyx/blobs.py
--rw-r--r--   0        0        0     1319 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/pyx/config.py
--rw-r--r--   0        0        0    13169 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/pyx/deco.py
--rw-r--r--   0        0        0     2561 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/pyx/diagrams.py
--rw-r--r--   0        0        0    41291 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/pyx/lines.py
--rw-r--r--   0        0        0     3549 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/pyx/paint.py
--rw-r--r--   0        0        0    12623 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/pyx/points.py
--rw-r--r--   0        0        0     7976 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/pyx/pyxrender.py
--rw-r--r--   0        0        0     1501 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/pyx/utils.py
--rw-r--r--   0        0        0     2914 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/render.py
--rw-r--r--   0        0        0     7120 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/text/ascii.py
--rw-r--r--   0        0        0      745 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/text/asciipdf.py
--rw-r--r--   0        0        0     2228 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/text/label.py
--rw-r--r--   0        0        0     1547 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/text/line.py
--rw-r--r--   0        0        0     1502 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/text/plainpdf.py
--rw-r--r--   0        0        0      483 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/text/point.py
--rw-r--r--   0        0        0     3846 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/text/style.py
--rw-r--r--   0        0        0     1401 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/text/unicode.py
--rw-r--r--   0        0        0     1858 2023-04-12 08:31:25.226843 pyfeyn2-2.2.4/pyfeyn2/render/text/unicodepdf.py
--rw-r--r--   0        0        0     2480 2023-04-12 08:31:27.499010 pyfeyn2-2.2.4/pyproject.toml
--rw-r--r--   0        0        0     5016 1970-01-01 00:00:00.000000 pyfeyn2-2.2.4/setup.py
--rw-r--r--   0        0        0     4886 1970-01-01 00:00:00.000000 pyfeyn2-2.2.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-12 13:07:48.890074 pyfeyn2-2.2.5/LICENSE
+-rw-r--r--   0        0        0     3226 2023-04-12 13:07:48.890074 pyfeyn2-2.2.5/README.md
+-rw-r--r--   0        0        0      154 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/auto/__init__.py
+-rw-r--r--   0        0        0     2841 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/auto/bend.py
+-rw-r--r--   0        0        0      774 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/auto/label.py
+-rw-r--r--   0        0        0     2073 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/auto/position.py
+-rw-r--r--   0        0        0        0 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/auto/reshuffle.py
+-rw-r--r--   0        0        0      680 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/feynmandiagram.py
+-rw-r--r--   0        0        0     2305 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/interface/dot.py
+-rw-r--r--   0        0        0       85 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/interface/hepmc.py
+-rw-r--r--   0        0        0       85 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/interface/qgraf.py
+-rw-r--r--   0        0        0      169 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/mkfeyndiag.py
+-rw-r--r--   0        0        0        0 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/__init__.py
+-rw-r--r--   0        0        0     3651 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/all.py
+-rw-r--r--   0        0        0        0 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/latex/__init__.py
+-rw-r--r--   0        0        0     3492 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/latex/dot.py
+-rw-r--r--   0        0        0     5921 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/latex/feynmp.py
+-rw-r--r--   0        0        0     1616 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/latex/latex.py
+-rw-r--r--   0        0        0     2407 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/latex/metapost.py
+-rw-r--r--   0        0        0     6302 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/latex/tikzfeynman.py
+-rw-r--r--   0        0        0     6026 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/mpl/feynmanrender.py
+-rw-r--r--   0        0        0        0 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/pyx/__init__.py
+-rw-r--r--   0        0        0     7132 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/pyx/blobs.py
+-rw-r--r--   0        0        0     1319 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/pyx/config.py
+-rw-r--r--   0        0        0    13169 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/pyx/deco.py
+-rw-r--r--   0        0        0     2561 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/pyx/diagrams.py
+-rw-r--r--   0        0        0    41301 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/pyx/lines.py
+-rw-r--r--   0        0        0     3549 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/pyx/paint.py
+-rw-r--r--   0        0        0    12623 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/pyx/points.py
+-rw-r--r--   0        0        0     8043 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/pyx/pyxrender.py
+-rw-r--r--   0        0        0     1501 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/pyx/utils.py
+-rw-r--r--   0        0        0     2914 2023-04-12 13:07:48.974074 pyfeyn2-2.2.5/pyfeyn2/render/render.py
+-rw-r--r--   0        0        0     7120 2023-04-12 13:07:48.978074 pyfeyn2-2.2.5/pyfeyn2/render/text/ascii.py
+-rw-r--r--   0        0        0      745 2023-04-12 13:07:48.978074 pyfeyn2-2.2.5/pyfeyn2/render/text/asciipdf.py
+-rw-r--r--   0        0        0     2228 2023-04-12 13:07:48.978074 pyfeyn2-2.2.5/pyfeyn2/render/text/label.py
+-rw-r--r--   0        0        0     1547 2023-04-12 13:07:48.978074 pyfeyn2-2.2.5/pyfeyn2/render/text/line.py
+-rw-r--r--   0        0        0     1502 2023-04-12 13:07:48.978074 pyfeyn2-2.2.5/pyfeyn2/render/text/plainpdf.py
+-rw-r--r--   0        0        0      483 2023-04-12 13:07:48.978074 pyfeyn2-2.2.5/pyfeyn2/render/text/point.py
+-rw-r--r--   0        0        0     3846 2023-04-12 13:07:48.978074 pyfeyn2-2.2.5/pyfeyn2/render/text/style.py
+-rw-r--r--   0        0        0     1401 2023-04-12 13:07:48.978074 pyfeyn2-2.2.5/pyfeyn2/render/text/unicode.py
+-rw-r--r--   0        0        0     1858 2023-04-12 13:07:48.978074 pyfeyn2-2.2.5/pyfeyn2/render/text/unicodepdf.py
+-rw-r--r--   0        0        0     2480 2023-04-12 13:07:51.842085 pyfeyn2-2.2.5/pyproject.toml
+-rw-r--r--   0        0        0     5016 1970-01-01 00:00:00.000000 pyfeyn2-2.2.5/setup.py
+-rw-r--r--   0        0        0     4886 1970-01-01 00:00:00.000000 pyfeyn2-2.2.5/PKG-INFO
```

### Comparing `pyfeyn2-2.2.4/LICENSE` & `pyfeyn2-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.4/README.md` & `pyfeyn2-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.4/pyfeyn2/auto/bend.py` & `pyfeyn2-2.2.5/pyfeyn2/auto/bend.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.4/pyfeyn2/auto/label.py` & `pyfeyn2-2.2.5/pyfeyn2/auto/label.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.4/pyfeyn2/auto/position.py` & `pyfeyn2-2.2.5/pyfeyn2/auto/position.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.4/pyfeyn2/feynmandiagram.py` & `pyfeyn2-2.2.5/pyfeyn2/feynmandiagram.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.4/pyfeyn2/interface/dot.py` & `pyfeyn2-2.2.5/pyfeyn2/interface/dot.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.4/pyfeyn2/render/all.py` & `pyfeyn2-2.2.5/pyfeyn2/render/all.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.4/pyfeyn2/render/latex/dot.py` & `pyfeyn2-2.2.5/pyfeyn2/render/latex/dot.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.4/pyfeyn2/render/latex/feynmp.py` & `pyfeyn2-2.2.5/pyfeyn2/render/latex/feynmp.py`

 * *Files 8% similar despite different names*

```diff
@@ -104,44 +104,36 @@
     if len(outgoing) > 0:
         src += f"\t\t\\fmf{dirout}" + "{"
         for l in outgoing:
             src += f"{l.id},"
         src = src[:-1]
         src += "}\n"
 
-    for l in incoming:
-        lstyle = fd.get_style(l)
-        if lstyle.getProperty("line") is not None:
-            tttype = type_map[lstyle.getProperty("line").value]
-        else:
-            tttype = l.type  # fallback to type if no line style is set
-        style = stylize_line(fd, l)
-        for ttype in tttype:
-            lid = l.id
-            ltarget = l.target
-            if l.type.startswith("anti"):
-                lid = l.target
-                ltarget = l.id
-            src += f"\t\t\\fmf{{{ttype}{style}}}{{{lid},{ltarget}}}\n"
-            style = ""
-    for l in outgoing:
-        lstyle = fd.get_style(l)
-        if lstyle.getProperty("line") is not None:
-            tttype = type_map[lstyle.getProperty("line").value]
-        else:
-            tttype = l.type  # fallback to type if no line style is set
-        style = stylize_line(fd, l)
-        for ttype in tttype:
-            lid = l.id
-            ltarget = l.target
-            if l.type.startswith("anti"):
-                lid = l.target
-                ltarget = l.id
-            src += f"\t\t\\fmf{{{ttype}{style}}}{{{ltarget},{lid}}}\n"
-            style = ""
+    def do_legs(src, legs, inward):
+        for l in legs:
+            lstyle = fd.get_style(l)
+            if lstyle.getProperty("line") is not None:
+                tttype = type_map[lstyle.getProperty("line").value]
+            else:
+                tttype = l.type  # fallback to type if no line style is set
+            style = stylize_line(fd, l)
+            for ttype in tttype:
+                lid = l.id
+                ltarget = l.target
+                if l.type.startswith("anti"):
+                    lid = l.target
+                    ltarget = l.id
+                if inward:
+                    src += f"\t\t\\fmf{{{ttype}{style}}}{{{lid},{ltarget}}}\n"
+                else:
+                    src += f"\t\t\\fmf{{{ttype}{style}}}{{{ltarget},{lid}}}\n"
+                style = ""
+
+    do_legs(src, incoming, True)
+    do_legs(src, outgoing, False)
 
     for p in fd.propagators:
         pstyle = fd.get_style(p)
         if pstyle.getProperty("line") is not None:
             tttype = type_map[pstyle.getProperty("line").value]
         else:
             tttype = p.type  # fallback to type if no line style is set
```

### Comparing `pyfeyn2-2.2.4/pyfeyn2/render/latex/latex.py` & `pyfeyn2-2.2.5/pyfeyn2/render/latex/latex.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.4/pyfeyn2/render/latex/metapost.py` & `pyfeyn2-2.2.5/pyfeyn2/render/latex/metapost.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.4/pyfeyn2/render/latex/tikzfeynman.py` & `pyfeyn2-2.2.5/pyfeyn2/render/latex/tikzfeynman.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.4/pyfeyn2/render/mpl/feynmanrender.py` & `pyfeyn2-2.2.5/pyfeyn2/render/mpl/feynmanrender.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.4/pyfeyn2/render/pyx/blobs.py` & `pyfeyn2-2.2.5/pyfeyn2/render/pyx/blobs.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.4/pyfeyn2/render/pyx/config.py` & `pyfeyn2-2.2.5/pyfeyn2/render/pyx/config.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.4/pyfeyn2/render/pyx/deco.py` & `pyfeyn2-2.2.5/pyfeyn2/render/pyx/deco.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.4/pyfeyn2/render/pyx/diagrams.py` & `pyfeyn2-2.2.5/pyfeyn2/render/pyx/diagrams.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.4/pyfeyn2/render/pyx/lines.py` & `pyfeyn2-2.2.5/pyfeyn2/render/pyx/lines.py`

 * *Files 0% similar despite different names*

```diff
@@ -920,15 +920,15 @@
         for curveradius in curveradii:
             try:
                 curveradius = abs(mincurveradius / pyx.unit.m)
                 # if config.getOptions().DEBUG:
                 #    print self.__class__, "- curvature radius = ", curveradius
                 if mincurveradius is None or curveradius < mincurveradius:
                     mincurveradius = curveradius
-            except:
+            except Exception:
                 pass
 
         ## Use curvature info to increase number of curve sections
         numhloopcurves = 5
         if mincurveradius is not None:
             numhloopcurves += int(0.1 / mincurveradius)
         if config.getOptions().DEBUG:
```

### Comparing `pyfeyn2-2.2.4/pyfeyn2/render/pyx/paint.py` & `pyfeyn2-2.2.5/pyfeyn2/render/pyx/paint.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.4/pyfeyn2/render/pyx/points.py` & `pyfeyn2-2.2.5/pyfeyn2/render/pyx/points.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.4/pyfeyn2/render/pyx/pyxrender.py` & `pyfeyn2-2.2.5/pyfeyn2/render/pyx/pyxrender.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,16 @@
                 break
             s = styling.split(":")
             styledict[s[0].lstrip().rstrip()] = s[1]
         if "fill-style" in styledict:
             filltype = styledict["fill-style"].split()
             if filltype[0] == "solid":
                 R, G, B = [
-                    eval("0x%s" % x) / 255.0
+                    int("0x" + x, base=16) / 255.0
+                    # eval("0x%s" % x) / 255.0 # <- old code
                     for x in [filltype[1][n : n + 2] for n in (1, 3, 5)]
                 ]
                 obj.fillstyles = [pyx.color.rgb(R, G, B)]
             elif filltype[0] == "hatched":
                 D, A = float(filltype[1]), int(filltype[2])
                 obj.fillstyles = [pyx.pattern.hatched(D, A)]
             elif filltype[0] == "crosshatched":
```

### Comparing `pyfeyn2-2.2.4/pyfeyn2/render/pyx/utils.py` & `pyfeyn2-2.2.5/pyfeyn2/render/pyx/utils.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.4/pyfeyn2/render/render.py` & `pyfeyn2-2.2.5/pyfeyn2/render/render.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.4/pyfeyn2/render/text/ascii.py` & `pyfeyn2-2.2.5/pyfeyn2/render/text/ascii.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.4/pyfeyn2/render/text/asciipdf.py` & `pyfeyn2-2.2.5/pyfeyn2/render/text/asciipdf.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.4/pyfeyn2/render/text/label.py` & `pyfeyn2-2.2.5/pyfeyn2/render/text/label.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.4/pyfeyn2/render/text/line.py` & `pyfeyn2-2.2.5/pyfeyn2/render/text/line.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.4/pyfeyn2/render/text/plainpdf.py` & `pyfeyn2-2.2.5/pyfeyn2/render/text/plainpdf.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.4/pyfeyn2/render/text/style.py` & `pyfeyn2-2.2.5/pyfeyn2/render/text/style.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.4/pyfeyn2/render/text/unicode.py` & `pyfeyn2-2.2.5/pyfeyn2/render/text/unicode.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.4/pyfeyn2/render/text/unicodepdf.py` & `pyfeyn2-2.2.5/pyfeyn2/render/text/unicodepdf.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.4/pyproject.toml` & `pyfeyn2-2.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyfeyn2"
-version = "2.2.4"
+version = "2.2.5"
 description = "PyFeyn is a package which makes drawing Feynman diagrams simple and programmatic.  Feynman diagrams are important constructs in perturbative field theory, so being able to draw them in a programmatic fashion is important if attempting to enumerate a large number of diagram configurations is important. The output quality of PyFeyn diagrams (into PDF or EPS formats) is very high, and special effects can be obtained by using constructs from PyX, which PyFeyn is based around"
 authors = ["Alexander Puck Neuwirth <alexander@neuwirth-informatik.de>"]
 readme = "README.md"
 repository = "https://github.com/APN-Pucky/pyfeyn2"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `pyfeyn2-2.2.4/setup.py` & `pyfeyn2-2.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
  'xsdata[cli,lxml,soap]']
 
 entry_points = \
 {'console_scripts': ['mkfeyndiag = pyfeyn2.mkfeyndiag:main']}
 
 setup_kwargs = {
     'name': 'pyfeyn2',
-    'version': '2.2.4',
+    'version': '2.2.5',
     'description': 'PyFeyn is a package which makes drawing Feynman diagrams simple and programmatic.  Feynman diagrams are important constructs in perturbative field theory, so being able to draw them in a programmatic fashion is important if attempting to enumerate a large number of diagram configurations is important. The output quality of PyFeyn diagrams (into PDF or EPS formats) is very high, and special effects can be obtained by using constructs from PyX, which PyFeyn is based around',
     'long_description': "# PyFeyn2\n\nForked from <https://pyfeyn.hepforge.org/> \n\nPyFeyn is a Python-language based system for drawing Feynman diagrams. It was inspired by the C++ FeynDiagram system, and aims to provide the same functionality and quality of output as that, with the added benefits of a modern interpreted language, an improved interface and output direct to both EPS and PDF. Behind the scenes, PyFeyn uses the excellent PyX system - you can use PyX constructs in PyFeyn diagrams if you want, too.\n\n[![PyPI version][pypi image]][pypi link] [![PyPI version][pypi versions]][pypi link]  ![downloads](https://img.shields.io/pypi/dm/pyfeyn2.svg)\n\n[![test][a t image]][a t link]      [![Coverage Status][c t i]][c t l]  [![Codacy Badge][cc c i]][cc c l]   [![Codacy Badge][cc q i]][cc q l]  [![Documentation][rtd t i]][rtd t l]\n\n## Dependencies\n\n*   libmagickwand-dev (to display pdfs in a jupyter-notebook, might require a policy change of the imagemagick config for PDFs, see Troubleshooting)\n*   ghostscript\n*   latexmk\n*   (feynmp-auto/feynmf)\n\n## Installation\n\n```sh\npoerty install --with docs --with dev\npoetry shell\n```\n\n## Documentation\n\n*   <https://pyfeyn2.readthedocs.io/en/stable/>\n*   <https://apn-pucky.github.io/pyfeyn2/index.html>\n\n## Similar Feynman diagram rendering project:\n\n*   <https://github.com/ndeutschmann/qgraf-xml-drawer>\n*   <https://github.com/GkAntonius/feynman>\n*   <https://github.com/JP-Ellis/tikz-feynman>\n*   <https://pyfeyn.hepforge.org/> \n*   <https://feynml.hepforge.org/>\n*   <http://www.feyndiagram.com/>\n\nSeveral of these are integrated into pyfeyn2.\n\n## Troubleshooting\n\n*   [ImageMagick security policy 'PDF' blocking conversion]( https://stackoverflow.com/questions/52998331/imagemagick-security-policy-pdf-blocking-conversion )\n\n## Development\n\n\n### package/python structure:\n\n*   <https://mathspp.com/blog/how-to-create-a-python-package-in-2022>\n*   <https://www.brainsorting.com/posts/publish-a-package-on-pypi-using-poetry/>\n\n[doc stable]: https://apn-pucky.github.io/pyfeyn2/index.html\n[doc test]: https://apn-pucky.github.io/pyfeyn2/test/index.html\n\n[pypi image]: https://badge.fury.io/py/pyfeyn2.svg\n[pypi link]: https://pypi.org/project/pyfeyn2/\n[pypi versions]: https://img.shields.io/pypi/pyversions/pyfeyn2.svg\n\n[a t link]: https://github.com/APN-Pucky/pyfeyn2/actions/workflows/test.yml\n[a t image]: https://github.com/APN-Pucky/pyfeyn2/actions/workflows/test.yml/badge.svg\n\n[cc q i]: https://app.codacy.com/project/badge/Grade/135bae47c6344ab0bfb180135ea1db44\n[cc q l]: https://www.codacy.com/gh/APN-Pucky/pyfeyn2/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/pyfeyn2&amp;utm_campaign=Badge_Grade\n[cc c i]: https://app.codacy.com/project/badge/Coverage/135bae47c6344ab0bfb180135ea1db44\n[cc c l]: https://www.codacy.com/gh/APN-Pucky/pyfeyn2/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/pyfeyn2&utm_campaign=Badge_Coverage\n\n[c t l]: https://coveralls.io/github/APN-Pucky/pyfeyn2?branch=master\n[c t i]: https://coveralls.io/repos/github/APN-Pucky/pyfeyn2/badge.svg?branch=master\n\n[rtd t i]: https://readthedocs.org/projects/pyfeyn2/badge/?version=latest\n[rtd t l]: https://pyfeyn2.readthedocs.io/en/latest/?badge=latest\n",
     'author': 'Alexander Puck Neuwirth',
     'author_email': 'alexander@neuwirth-informatik.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/APN-Pucky/pyfeyn2',
```

### Comparing `pyfeyn2-2.2.4/PKG-INFO` & `pyfeyn2-2.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfeyn2
-Version: 2.2.4
+Version: 2.2.5
 Summary: PyFeyn is a package which makes drawing Feynman diagrams simple and programmatic.  Feynman diagrams are important constructs in perturbative field theory, so being able to draw them in a programmatic fashion is important if attempting to enumerate a large number of diagram configurations is important. The output quality of PyFeyn diagrams (into PDF or EPS formats) is very high, and special effects can be obtained by using constructs from PyX, which PyFeyn is based around
 Home-page: https://github.com/APN-Pucky/pyfeyn2
 Author: Alexander Puck Neuwirth
 Author-email: alexander@neuwirth-informatik.de
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

