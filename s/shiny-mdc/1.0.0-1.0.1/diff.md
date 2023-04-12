# Comparing `tmp/shiny_mdc-1.0.0.tar.gz` & `tmp/shiny_mdc-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shiny_mdc-1.0.0.tar", max compression
+gzip compressed data, was "shiny_mdc-1.0.1.tar", max compression
```

## Comparing `shiny_mdc-1.0.0.tar` & `shiny_mdc-1.0.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0      188 2023-04-11 21:12:37.200710 shiny_mdc-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     1082 2023-04-11 21:12:37.200710 shiny_mdc-1.0.0/LICENSE
--rw-r--r--   0        0        0       78 2023-04-11 21:12:37.200710 shiny_mdc-1.0.0/README.md
--rw-r--r--   0        0        0     2295 2023-04-11 21:13:00.440920 shiny_mdc-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       34 2023-04-11 21:12:37.200710 shiny_mdc-1.0.0/shinymdc/__init__.py
--rw-r--r--   0        0        0     1061 2023-04-11 21:12:37.200710 shiny_mdc-1.0.0/shinymdc/_latexmk.py
--rw-r--r--   0        0        0     1867 2023-04-11 21:12:37.200710 shiny_mdc-1.0.0/shinymdc/_liquid.py
--rw-r--r--   0        0        0     4643 2023-04-11 21:12:37.200710 shiny_mdc-1.0.0/shinymdc/_pandoc.py
--rw-r--r--   0        0        0     3970 2023-04-11 21:12:37.200710 shiny_mdc-1.0.0/shinymdc/_templates.py
--rw-r--r--   0        0        0       64 2023-04-11 21:13:00.440920 shiny_mdc-1.0.0/shinymdc/_version.py
--rw-r--r--   0        0        0      312 2023-04-11 21:12:37.200710 shiny_mdc-1.0.0/shinymdc/resources/dynamic/addappendices.tex
--rw-r--r--   0        0        0      319 2023-04-11 21:12:37.200710 shiny_mdc-1.0.0/shinymdc/resources/dynamic/authsetup.tex
--rw-r--r--   0        0        0      290 2023-04-11 21:12:37.200710 shiny_mdc-1.0.0/shinymdc/resources/dynamic/authsetupshort.tex
--rw-r--r--   0        0        0      572 2023-04-11 21:12:37.200710 shiny_mdc-1.0.0/shinymdc/resources/dynamic/dblfloatsetup.tex
--rw-r--r--   0        0        0     3160 2023-04-11 21:12:37.204710 shiny_mdc-1.0.0/shinymdc/resources/static/floatsetup.tex
--rw-r--r--   0        0        0    19901 2023-04-11 21:12:37.204710 shiny_mdc-1.0.0/shinymdc/resources/static/iccv/bibstyle.bst
--rw-r--r--   0        0        0     9433 2023-04-11 21:12:37.204710 shiny_mdc-1.0.0/shinymdc/resources/static/iccv/esopic.sty
--rw-r--r--   0        0        0     3869 2023-04-11 21:12:37.204710 shiny_mdc-1.0.0/shinymdc/resources/static/iccv/everyshi.sty
--rw-r--r--   0        0        0     8276 2023-04-11 21:12:37.204710 shiny_mdc-1.0.0/shinymdc/resources/static/iccv/iccv.sty
--rw-r--r--   0        0        0    26973 2023-04-11 21:12:37.204710 shiny_mdc-1.0.0/shinymdc/resources/static/iclr/bibstyle.bst
--rw-r--r--   0        0        0     9153 2023-04-11 21:12:37.204710 shiny_mdc-1.0.0/shinymdc/resources/static/iclr/iclr.sty
--rw-r--r--   0        0        0    12284 2023-04-11 21:12:37.204710 shiny_mdc-1.0.0/shinymdc/resources/static/iclr/mathcommands.tex
--rw-r--r--   0        0        0    27146 2023-04-11 21:12:37.204710 shiny_mdc-1.0.0/shinymdc/resources/static/icml/bibstyle.bst
--rw-r--r--   0        0        0    27887 2023-04-11 21:12:37.204710 shiny_mdc-1.0.0/shinymdc/resources/static/icml/icml.sty
--rw-r--r--   0        0        0      735 2023-04-11 21:12:37.204710 shiny_mdc-1.0.0/shinymdc/resources/static/mathsetup.tex
--rw-r--r--   0        0        0     1019 2023-04-11 21:12:37.204710 shiny_mdc-1.0.0/shinymdc/resources/static/miscsetup.tex
--rw-r--r--   0        0        0    11306 2023-04-11 21:12:37.204710 shiny_mdc-1.0.0/shinymdc/resources/static/neurips/neurips.sty
--rw-r--r--   0        0        0      426 2023-04-11 21:12:37.204710 shiny_mdc-1.0.0/shinymdc/resources/static/reqsetup.tex
--rw-r--r--   0        0        0    16068 2023-04-11 21:12:37.204710 shiny_mdc-1.0.0/shinymdc/shinymdc.py
--rw-r--r--   0        0        0      866 2023-04-11 21:12:37.204710 shiny_mdc-1.0.0/shinymdc/templates/basic.tex
--rw-r--r--   0        0        0     1443 2023-04-11 21:12:37.204710 shiny_mdc-1.0.0/shinymdc/templates/iccv.tex
--rw-r--r--   0        0        0      906 2023-04-11 21:12:37.204710 shiny_mdc-1.0.0/shinymdc/templates/iclr.tex
--rw-r--r--   0        0        0     2144 2023-04-11 21:12:37.204710 shiny_mdc-1.0.0/shinymdc/templates/icml.tex
--rw-r--r--   0        0        0      897 2023-04-11 21:12:37.204710 shiny_mdc-1.0.0/shinymdc/templates/neurips.tex
--rw-r--r--   0        0        0     2095 2023-04-11 21:12:37.204710 shiny_mdc-1.0.0/shinymdc/templates/spacious.tex
--rw-r--r--   0        0        0      511 2023-04-11 21:12:37.204710 shiny_mdc-1.0.0/shinymdc/templates/standalone.tex
--rw-r--r--   0        0        0     2343 2023-04-11 21:12:37.204710 shiny_mdc-1.0.0/shinymdc/templates/stylish.tex
--rw-r--r--   0        0        0    15953 2023-04-11 21:12:37.208710 shiny_mdc-1.0.0/test/figures/anscombe.pdf
--rw-r--r--   0        0        0    40892 2023-04-11 21:12:37.208710 shiny_mdc-1.0.0/test/figures/densities.pdf
--rw-r--r--   0        0        0    10736 2023-04-11 21:12:37.208710 shiny_mdc-1.0.0/test/figures/diamonds.pdf
--rw-r--r--   0        0        0   197017 2023-04-11 21:12:37.208710 shiny_mdc-1.0.0/test/figures/gaussian2d.pdf
--rw-r--r--   0        0        0    28282 2023-04-11 21:12:37.208710 shiny_mdc-1.0.0/test/figures/lines.png
--rw-r--r--   0        0        0     2579 2023-04-11 21:12:37.208710 shiny_mdc-1.0.0/test/main.md
--rwxr-xr-x   0        0        0      315 2023-04-11 21:12:37.208710 shiny_mdc-1.0.0/test/make.sh
--rw-r--r--   0        0        0     1166 2023-04-11 21:12:37.208710 shiny_mdc-1.0.0/test/references.bib
--rw-r--r--   0        0        0   675190 2023-04-11 21:12:37.208710 shiny_mdc-1.0.0/test/samples/basic.pdf
--rw-r--r--   0        0        0   409896 2023-04-11 21:12:37.212710 shiny_mdc-1.0.0/test/samples/iccv.pdf
--rw-r--r--   0        0        0   402766 2023-04-11 21:12:37.212710 shiny_mdc-1.0.0/test/samples/iclr.pdf
--rw-r--r--   0        0        0   442274 2023-04-11 21:12:37.212710 shiny_mdc-1.0.0/test/samples/icml.pdf
--rw-r--r--   0        0        0   447265 2023-04-11 21:12:37.212710 shiny_mdc-1.0.0/test/samples/neurips.pdf
--rw-r--r--   0        0        0   595883 2023-04-11 21:12:37.212710 shiny_mdc-1.0.0/test/samples/spacious.pdf
--rw-r--r--   0        0        0   530011 2023-04-11 21:12:37.216710 shiny_mdc-1.0.0/test/samples/standalone.pdf
--rw-r--r--   0        0        0   419540 2023-04-11 21:12:37.216710 shiny_mdc-1.0.0/test/samples/stylish.pdf
--rw-r--r--   0        0        0     1535 2023-04-11 21:12:37.216710 shiny_mdc-1.0.0/test/sections/appendix1.md
--rw-r--r--   0        0        0     1619 2023-04-11 21:12:37.216710 shiny_mdc-1.0.0/test/sections/appendix2.md
--rw-r--r--   0        0        0        0 2023-04-11 21:12:37.216710 shiny_mdc-1.0.0/test/sections/empty.md
--rw-r--r--   0        0        0     1356 2023-04-11 21:12:37.216710 shiny_mdc-1.0.0/test/sections/main1.md
--rw-r--r--   0        0        0     1351 2023-04-11 21:12:37.216710 shiny_mdc-1.0.0/test/sections/main2.md
--rw-r--r--   0        0        0      992 2023-04-11 21:12:37.216710 shiny_mdc-1.0.0/test/utils/commands.md
--rw-r--r--   0        0        0       41 2023-04-11 21:12:37.216710 shiny_mdc-1.0.0/test/utils/ext.md
--rw-r--r--   0        0        0     1004 1970-01-01 00:00:00.000000 shiny_mdc-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1244 2023-04-12 01:04:50.539643 shiny_mdc-1.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1082 2023-04-12 01:04:50.539643 shiny_mdc-1.0.1/LICENSE
+-rw-r--r--   0        0        0       78 2023-04-12 01:04:50.539643 shiny_mdc-1.0.1/README.md
+-rw-r--r--   0        0        0     2295 2023-04-12 01:05:13.976297 shiny_mdc-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-04-12 01:04:50.539643 shiny_mdc-1.0.1/shinymdc/__init__.py
+-rw-r--r--   0        0        0     1061 2023-04-12 01:04:50.539643 shiny_mdc-1.0.1/shinymdc/_latexmk.py
+-rw-r--r--   0        0        0     1867 2023-04-12 01:04:50.539643 shiny_mdc-1.0.1/shinymdc/_liquid.py
+-rw-r--r--   0        0        0     4643 2023-04-12 01:04:50.539643 shiny_mdc-1.0.1/shinymdc/_pandoc.py
+-rw-r--r--   0        0        0     4713 2023-04-12 01:04:50.539643 shiny_mdc-1.0.1/shinymdc/_templates.py
+-rw-r--r--   0        0        0       64 2023-04-12 01:05:13.976297 shiny_mdc-1.0.1/shinymdc/_version.py
+-rw-r--r--   0        0        0      312 2023-04-12 01:04:50.539643 shiny_mdc-1.0.1/shinymdc/resources/dynamic/addappendices.tex
+-rw-r--r--   0        0        0      319 2023-04-12 01:04:50.539643 shiny_mdc-1.0.1/shinymdc/resources/dynamic/authsetup.tex
+-rw-r--r--   0        0        0      290 2023-04-12 01:04:50.539643 shiny_mdc-1.0.1/shinymdc/resources/dynamic/authsetupshort.tex
+-rw-r--r--   0        0        0      572 2023-04-12 01:04:50.539643 shiny_mdc-1.0.1/shinymdc/resources/dynamic/dblfloatsetup.tex
+-rw-r--r--   0        0        0     3160 2023-04-12 01:04:50.539643 shiny_mdc-1.0.1/shinymdc/resources/static/floatsetup.tex
+-rw-r--r--   0        0        0    19901 2023-04-12 01:04:50.539643 shiny_mdc-1.0.1/shinymdc/resources/static/iccv/bibstyle.bst
+-rw-r--r--   0        0        0     9433 2023-04-12 01:04:50.539643 shiny_mdc-1.0.1/shinymdc/resources/static/iccv/esopic.sty
+-rw-r--r--   0        0        0     3869 2023-04-12 01:04:50.539643 shiny_mdc-1.0.1/shinymdc/resources/static/iccv/everyshi.sty
+-rw-r--r--   0        0        0     8276 2023-04-12 01:04:50.539643 shiny_mdc-1.0.1/shinymdc/resources/static/iccv/iccv.sty
+-rw-r--r--   0        0        0    26973 2023-04-12 01:04:50.539643 shiny_mdc-1.0.1/shinymdc/resources/static/iclr/bibstyle.bst
+-rw-r--r--   0        0        0     9153 2023-04-12 01:04:50.539643 shiny_mdc-1.0.1/shinymdc/resources/static/iclr/iclr.sty
+-rw-r--r--   0        0        0    12284 2023-04-12 01:04:50.539643 shiny_mdc-1.0.1/shinymdc/resources/static/iclr/mathcommands.tex
+-rw-r--r--   0        0        0    27146 2023-04-12 01:04:50.539643 shiny_mdc-1.0.1/shinymdc/resources/static/icml/bibstyle.bst
+-rw-r--r--   0        0        0    27887 2023-04-12 01:04:50.543643 shiny_mdc-1.0.1/shinymdc/resources/static/icml/icml.sty
+-rw-r--r--   0        0        0      735 2023-04-12 01:04:50.543643 shiny_mdc-1.0.1/shinymdc/resources/static/mathsetup.tex
+-rw-r--r--   0        0        0     1041 2023-04-12 01:04:50.543643 shiny_mdc-1.0.1/shinymdc/resources/static/miscsetup.tex
+-rw-r--r--   0        0        0    11306 2023-04-12 01:04:50.543643 shiny_mdc-1.0.1/shinymdc/resources/static/neurips/neurips.sty
+-rw-r--r--   0        0        0      426 2023-04-12 01:04:50.543643 shiny_mdc-1.0.1/shinymdc/resources/static/reqsetup.tex
+-rw-r--r--   0        0        0    16068 2023-04-12 01:04:50.543643 shiny_mdc-1.0.1/shinymdc/shinymdc.py
+-rw-r--r--   0        0        0      866 2023-04-12 01:04:50.543643 shiny_mdc-1.0.1/shinymdc/templates/basic.tex
+-rw-r--r--   0        0        0     1443 2023-04-12 01:04:50.543643 shiny_mdc-1.0.1/shinymdc/templates/iccv.tex
+-rw-r--r--   0        0        0     1440 2023-04-12 01:04:50.543643 shiny_mdc-1.0.1/shinymdc/templates/iclr.tex
+-rw-r--r--   0        0        0     2187 2023-04-12 01:04:50.543643 shiny_mdc-1.0.1/shinymdc/templates/icml.tex
+-rw-r--r--   0        0        0      897 2023-04-12 01:04:50.543643 shiny_mdc-1.0.1/shinymdc/templates/neurips.tex
+-rw-r--r--   0        0        0     2095 2023-04-12 01:04:50.543643 shiny_mdc-1.0.1/shinymdc/templates/spacious.tex
+-rw-r--r--   0        0        0      511 2023-04-12 01:04:50.543643 shiny_mdc-1.0.1/shinymdc/templates/standalone.tex
+-rw-r--r--   0        0        0     2343 2023-04-12 01:04:50.543643 shiny_mdc-1.0.1/shinymdc/templates/stylish.tex
+-rw-r--r--   0        0        0    15953 2023-04-12 01:04:50.543643 shiny_mdc-1.0.1/test/figures/anscombe.pdf
+-rw-r--r--   0        0        0    40892 2023-04-12 01:04:50.543643 shiny_mdc-1.0.1/test/figures/densities.pdf
+-rw-r--r--   0        0        0    10736 2023-04-12 01:04:50.543643 shiny_mdc-1.0.1/test/figures/diamonds.pdf
+-rw-r--r--   0        0        0   197017 2023-04-12 01:04:50.543643 shiny_mdc-1.0.1/test/figures/gaussian2d.pdf
+-rw-r--r--   0        0        0    28282 2023-04-12 01:04:50.543643 shiny_mdc-1.0.1/test/figures/lines.png
+-rw-r--r--   0        0        0     2579 2023-04-12 01:04:50.543643 shiny_mdc-1.0.1/test/main.md
+-rwxr-xr-x   0        0        0      315 2023-04-12 01:04:50.543643 shiny_mdc-1.0.1/test/make.sh
+-rw-r--r--   0        0        0     1166 2023-04-12 01:04:50.543643 shiny_mdc-1.0.1/test/references.bib
+-rw-r--r--   0        0        0   675190 2023-04-12 01:04:50.547644 shiny_mdc-1.0.1/test/samples/basic.pdf
+-rw-r--r--   0        0        0   409896 2023-04-12 01:04:50.547644 shiny_mdc-1.0.1/test/samples/iccv.pdf
+-rw-r--r--   0        0        0   402633 2023-04-12 01:04:50.551643 shiny_mdc-1.0.1/test/samples/iclr.pdf
+-rw-r--r--   0        0        0   442208 2023-04-12 01:04:50.551643 shiny_mdc-1.0.1/test/samples/icml.pdf
+-rw-r--r--   0        0        0   447276 2023-04-12 01:04:50.555644 shiny_mdc-1.0.1/test/samples/neurips.pdf
+-rw-r--r--   0        0        0   595883 2023-04-12 01:04:50.559644 shiny_mdc-1.0.1/test/samples/spacious.pdf
+-rw-r--r--   0        0        0   530011 2023-04-12 01:04:50.559644 shiny_mdc-1.0.1/test/samples/standalone.pdf
+-rw-r--r--   0        0        0   419540 2023-04-12 01:04:50.563644 shiny_mdc-1.0.1/test/samples/stylish.pdf
+-rw-r--r--   0        0        0     1535 2023-04-12 01:04:50.563644 shiny_mdc-1.0.1/test/sections/appendix1.md
+-rw-r--r--   0        0        0     1619 2023-04-12 01:04:50.563644 shiny_mdc-1.0.1/test/sections/appendix2.md
+-rw-r--r--   0        0        0        0 2023-04-12 01:04:50.563644 shiny_mdc-1.0.1/test/sections/empty.md
+-rw-r--r--   0        0        0     1356 2023-04-12 01:04:50.563644 shiny_mdc-1.0.1/test/sections/main1.md
+-rw-r--r--   0        0        0     1351 2023-04-12 01:04:50.563644 shiny_mdc-1.0.1/test/sections/main2.md
+-rw-r--r--   0        0        0      992 2023-04-12 01:04:50.563644 shiny_mdc-1.0.1/test/utils/commands.md
+-rw-r--r--   0        0        0       41 2023-04-12 01:04:50.563644 shiny_mdc-1.0.1/test/utils/ext.md
+-rw-r--r--   0        0        0     1004 1970-01-01 00:00:00.000000 shiny_mdc-1.0.1/PKG-INFO
```

### Comparing `shiny_mdc-1.0.0/LICENSE` & `shiny_mdc-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.0.0/pyproject.toml` & `shiny_mdc-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shiny-mdc"
-version = "1.0.0"  # managed by `poetry-dynamic-versioning`
+version = "1.0.1"  # managed by `poetry-dynamic-versioning`
 description = "Tool to compile markdown files to tex/pdf using pandoc, latexmk"
 readme = "README.md"
 authors = ["Jayanth Koushik <mail@jkoushik.me>"]
 license = "MIT"
 repository = "https://github.com/jayanthkoushik/shinymdc"
 packages = [
   { include = "shinymdc" }
```

### Comparing `shiny_mdc-1.0.0/shinymdc/_latexmk.py` & `shiny_mdc-1.0.1/shinymdc/_latexmk.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.0.0/shinymdc/_liquid.py` & `shiny_mdc-1.0.1/shinymdc/_liquid.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.0.0/shinymdc/_pandoc.py` & `shiny_mdc-1.0.1/shinymdc/_pandoc.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.0.0/shinymdc/resources/dynamic/dblfloatsetup.tex` & `shiny_mdc-1.0.1/shinymdc/resources/dynamic/dblfloatsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.0.0/shinymdc/resources/static/floatsetup.tex` & `shiny_mdc-1.0.1/shinymdc/resources/static/floatsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.0.0/shinymdc/resources/static/iccv/bibstyle.bst` & `shiny_mdc-1.0.1/shinymdc/resources/static/iccv/bibstyle.bst`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.0.0/shinymdc/resources/static/iccv/esopic.sty` & `shiny_mdc-1.0.1/shinymdc/resources/static/iccv/esopic.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.0.0/shinymdc/resources/static/iccv/everyshi.sty` & `shiny_mdc-1.0.1/shinymdc/resources/static/iccv/everyshi.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.0.0/shinymdc/resources/static/iccv/iccv.sty` & `shiny_mdc-1.0.1/shinymdc/resources/static/iccv/iccv.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.0.0/shinymdc/resources/static/iclr/bibstyle.bst` & `shiny_mdc-1.0.1/shinymdc/resources/static/iclr/bibstyle.bst`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.0.0/shinymdc/resources/static/iclr/iclr.sty` & `shiny_mdc-1.0.1/shinymdc/resources/static/iclr/iclr.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.0.0/shinymdc/resources/static/iclr/mathcommands.tex` & `shiny_mdc-1.0.1/shinymdc/resources/static/iclr/mathcommands.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.0.0/shinymdc/resources/static/icml/bibstyle.bst` & `shiny_mdc-1.0.1/shinymdc/resources/static/icml/bibstyle.bst`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.0.0/shinymdc/resources/static/icml/icml.sty` & `shiny_mdc-1.0.1/shinymdc/resources/static/icml/icml.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.0.0/shinymdc/resources/static/mathsetup.tex` & `shiny_mdc-1.0.1/shinymdc/resources/static/mathsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.0.0/shinymdc/resources/static/miscsetup.tex` & `shiny_mdc-1.0.1/shinymdc/resources/static/miscsetup.tex`

 * *Files 7% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 \usepackage{xcolor}
 \usepackage{tikz}
 \usepackage{fancyvrb}
 \usepackage{pgf}
 
 % Put year in citet.
 \newcommand*{\nolink}[1]{{\protect\NoHyper#1\protect\endNoHyper}}
+\let\origcitet\citet
 \renewcommand{\citet}[1]{%
-  \nolink{\citeauthor{#1} (\citeyear{#1})}\citep{#1}%
+  \nolink{\citeauthor{#1} (\citeyear{#1})}~\citep{#1}%
 }
 
 % Handle footnotes inside tables, figures.
 \makesavenoteenv{table}
 \makesavenoteenv{table*}
 \makesavenoteenv{figure}
 \makesavenoteenv{figure*}
```

### Comparing `shiny_mdc-1.0.0/shinymdc/resources/static/neurips/neurips.sty` & `shiny_mdc-1.0.1/shinymdc/resources/static/neurips/neurips.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.0.0/shinymdc/shinymdc.py` & `shiny_mdc-1.0.1/shinymdc/shinymdc.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.0.0/shinymdc/templates/basic.tex` & `shiny_mdc-1.0.1/shinymdc/templates/basic.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.0.0/shinymdc/templates/iccv.tex` & `shiny_mdc-1.0.1/shinymdc/templates/iccv.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.0.0/shinymdc/templates/iclr.tex` & `shiny_mdc-1.0.1/shinymdc/templates/neurips.tex`

 * *Files 27% similar despite different names*

```diff
@@ -1,63 +1,60 @@
+$if(submission)$
+\RequirePackage{scrlfile}
+\PreventPackageFromLoading{babel}
+\PreventPackageFromLoading{microtype}
+$endif$
+
 \documentclass{article}
 
-\usepackage{$iclr$,newtxtext}
-\usepackage{url}
+\PassOptionsToPackage{square,numbers,sort&compress}{natbib}
+\usepackage$if(submission)$$else$$if(preprint)$[preprint]$else$[final]$endif$$endif${$neurips$}
 
 \input{$reqsetup$}
 \input{$floatsetup$}
 \input{$mathsetup$}
 \input{$miscsetup$}
 
-% Optional math commands from https://github.com/goodfeli/dlbook_notation.
-% \input{$mathcommands$.tex}
-
 \title{$title$}
 
 \input{$authsetup$}
 
-\newcommand{\fix}{\marginpar{FIX}}
-\newcommand{\new}{\marginpar{NEW}}
-
-% Uncomment for camera-ready version, but NOT for submission.
-$if(submission)$
-$else$
-\iclrfinalcopy
-$endif$
-
 $for(includes)$
 $it$
 $endfor$
 
 \begin{document}
 
 \maketitle
 
+% Add equal-contrib footnote.
 $if(skipequal)$
+$else$
 $if(submission)$
 $else$
 \blfootnote{\textsuperscript{*}\,Equal contribution.}
 $endif$
 $endif$
 
 $if(abstract)$
 \begin{abstract}
-  $abstract$
+$abstract$
 \end{abstract}
 $endif$
 
 $if(body)$
 $body$
 $endif$
 
 $for(sections)$
 $it$
 $endfor$
 
 $if(bibliography)$
+\clearpage
+\bibliographystyle{unsrtnat}
 \bibliography{$bibliography$}
-\bibliographystyle{$bibstyle$}
 $endif$
 
 \input{$addappendices$}
 
 \end{document}
```

### Comparing `shiny_mdc-1.0.0/shinymdc/templates/icml.tex` & `shiny_mdc-1.0.1/shinymdc/templates/icml.tex`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 \usepackage$if(submission)$$else$[accepted]$endif${$icml$}
 
 \input{$floatsetup$}
 \input{$dblfloatsetup$}
 \input{$mathsetup$}
 \input{$miscsetup$}
 
+% Restore old citet.
+\let\citet\origcitet
+
 %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
 % THEOREMS
 %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
 \theoremstyle{plain}
 \newtheorem{theorem}{Theorem}[section]
 \newtheorem{proposition}[theorem]{Proposition}
 \newtheorem{lemma}[theorem]{Lemma}
```

### Comparing `shiny_mdc-1.0.0/shinymdc/templates/spacious.tex` & `shiny_mdc-1.0.1/shinymdc/templates/spacious.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.0.0/shinymdc/templates/stylish.tex` & `shiny_mdc-1.0.1/shinymdc/templates/stylish.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.0.0/test/figures/anscombe.pdf` & `shiny_mdc-1.0.1/test/figures/anscombe.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.0.0/test/figures/densities.pdf` & `shiny_mdc-1.0.1/test/figures/densities.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.0.0/test/figures/diamonds.pdf` & `shiny_mdc-1.0.1/test/figures/diamonds.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.0.0/test/figures/gaussian2d.pdf` & `shiny_mdc-1.0.1/test/figures/gaussian2d.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.0.0/test/figures/lines.png` & `shiny_mdc-1.0.1/test/figures/lines.png`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.0.0/test/main.md` & `shiny_mdc-1.0.1/test/main.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.0.0/test/references.bib` & `shiny_mdc-1.0.1/test/references.bib`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.0.0/test/samples/basic.pdf` & `shiny_mdc-1.0.1/test/samples/basic.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 0% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'673796'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'673796'*

 * *DEBUG:pdfminer.psparser:seek: 673796*

 * *DEBUG:pdfminer.psparser:nexttoken: (673796, 442)*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=673796, token=442*

 * *DEBUG:pdfminer.psparser:seek: 673796*

 * *DEBUG:pdfminer.psparser:nexttoken: (673796, 442)*

 * *DEBUG:pdfminer.psparser:nexttoken: (673800, 0)*

 * *DEBUG:pdfminer.psparser:nexttoken: (673802, /b'obj')*

 * *DEBUG:pdfminer.psparser:nexttoken: (673806, /b'<<')*

 * *DEBUG:pdfminer.psparser:start_type: pos=673806, type='d'*

 * *DEBUG:pdfminer.psparser:nexttoken: (673809, /'Type')*

 * *DEBUG:pdfminer.psparser:nexttoken: (673815, /'XRef')*

 * *DEBUG:pdfminer.psparser:nexttoken: (673821, /'Index')*

 * *DEBUG:pdfminer.psparser:nexttoken: (673828, /b'[')*

 * *DEBUG:pdfminer.psparser:start_type: pos=673828, type='a'*

 * *DEBUG:pdfminer.psparser:nexttoken: (673830, 0)*

 * *DEBUG:pdfminer.psparser:nexttoken: (673832, 443)*

 * *DEBUG:pdfminer.psparser:nexttoken: (673836, /b']')*

 * *DEBUG:pdfminer.psparser:end_type: pos=673828, type='a', objs=[0, 443]*

 * *DEBUG:pdfminer.psparser:nexttoken: (673838, /'Size')*

 * *[ truncated after 25 lines; 17928 ignored ]*

```diff
@@ -10167,17 +10167,17 @@
 <key>Creator</key>
 <value><string size="19">LaTeX with hyperref</string></value>
 <key>Keywords</key>
 <value><string size="0"></string></value>
 <key>Producer</key>
 <value><string size="13">LuaTeX-1.15.0</string></value>
 <key>CreationDate</key>
-<value><string size="23">D:20230411142440-04&#39;00&#39;</string></value>
+<value><string size="23">D:20230411204957-04&#39;00&#39;</string></value>
 <key>ModDate</key>
-<value><string size="23">D:20230411142440-04&#39;00&#39;</string></value>
+<value><string size="23">D:20230411204957-04&#39;00&#39;</string></value>
 <key>Trapped</key>
 <value><literal>False</literal></value>
 <key>PTEX.FullBanner</key>
 <value><string size="48">This is LuaHBTeX, Version 1.15.0 &#40;TeX Live 2022&#41;</string></value>
 </dict>
 </object>
 
@@ -10202,16 +10202,16 @@
 </list></value>
 <key>Root</key>
 <value><ref id="440" /></value>
 <key>Info</key>
 <value><ref id="441" /></value>
 <key>ID</key>
 <value><list size="2">
-<string size="16">v&#212;&#128;&#8;m&#168;&#148;I&#249;.&#214;T&#190;&#219;/&#146;</string>
-<string size="16">v&#212;&#128;&#8;m&#168;&#148;I&#249;.&#214;T&#190;&#219;/&#146;</string>
+<string size="16">w&#186;&#155;Q&#187;u?&#17;&#247;W,&#188;H&#40;Ic</string>
+<string size="16">w&#186;&#155;Q&#187;u?&#17;&#247;W,&#188;H&#40;Ic</string>
 </list></value>
 <key>Filter</key>
 <value><literal>FlateDecode</literal></value>
 <key>Length</key>
 <value><number>1131</number></value>
 </dict>
 </props>
@@ -10238,16 +10238,16 @@
 </list></value>
 <key>Root</key>
 <value><ref id="440" /></value>
 <key>Info</key>
 <value><ref id="441" /></value>
 <key>ID</key>
 <value><list size="2">
-<string size="16">v&#212;&#128;&#8;m&#168;&#148;I&#249;.&#214;T&#190;&#219;/&#146;</string>
-<string size="16">v&#212;&#128;&#8;m&#168;&#148;I&#249;.&#214;T&#190;&#219;/&#146;</string>
+<string size="16">w&#186;&#155;Q&#187;u?&#17;&#247;W,&#188;H&#40;Ic</string>
+<string size="16">w&#186;&#155;Q&#187;u?&#17;&#247;W,&#188;H&#40;Ic</string>
 </list></value>
 <key>Filter</key>
 <value><literal>FlateDecode</literal></value>
 <key>Length</key>
 <value><number>1131</number></value>
 </dict>
 </trailer>
```

### Comparing `shiny_mdc-1.0.0/test/samples/iccv.pdf` & `shiny_mdc-1.0.1/test/samples/iccv.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 0% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'408747'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'408747'*

 * *DEBUG:pdfminer.psparser:seek: 408747*

 * *DEBUG:pdfminer.psparser:nexttoken: (408747, 337)*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=408747, token=337*

 * *DEBUG:pdfminer.psparser:seek: 408747*

 * *DEBUG:pdfminer.psparser:nexttoken: (408747, 337)*

 * *DEBUG:pdfminer.psparser:nexttoken: (408751, 0)*

 * *DEBUG:pdfminer.psparser:nexttoken: (408753, /b'obj')*

 * *DEBUG:pdfminer.psparser:nexttoken: (408757, /b'<<')*

 * *DEBUG:pdfminer.psparser:start_type: pos=408757, type='d'*

 * *DEBUG:pdfminer.psparser:nexttoken: (408760, /'Type')*

 * *DEBUG:pdfminer.psparser:nexttoken: (408766, /'XRef')*

 * *DEBUG:pdfminer.psparser:nexttoken: (408772, /'Index')*

 * *DEBUG:pdfminer.psparser:nexttoken: (408779, /b'[')*

 * *DEBUG:pdfminer.psparser:start_type: pos=408779, type='a'*

 * *DEBUG:pdfminer.psparser:nexttoken: (408781, 0)*

 * *DEBUG:pdfminer.psparser:nexttoken: (408783, 338)*

 * *DEBUG:pdfminer.psparser:nexttoken: (408787, /b']')*

 * *DEBUG:pdfminer.psparser:end_type: pos=408779, type='a', objs=[0, 338]*

 * *DEBUG:pdfminer.psparser:nexttoken: (408789, /'Size')*

 * *[ truncated after 25 lines; 14452 ignored ]*

```diff
@@ -8227,17 +8227,17 @@
 <key>Creator</key>
 <value><string size="19">LaTeX with hyperref</string></value>
 <key>Keywords</key>
 <value><string size="0"></string></value>
 <key>Producer</key>
 <value><string size="13">LuaTeX-1.15.0</string></value>
 <key>CreationDate</key>
-<value><string size="23">D:20230411142445-04&#39;00&#39;</string></value>
+<value><string size="23">D:20230411205002-04&#39;00&#39;</string></value>
 <key>ModDate</key>
-<value><string size="23">D:20230411142445-04&#39;00&#39;</string></value>
+<value><string size="23">D:20230411205002-04&#39;00&#39;</string></value>
 <key>Trapped</key>
 <value><literal>False</literal></value>
 <key>PTEX.FullBanner</key>
 <value><string size="48">This is LuaHBTeX, Version 1.15.0 &#40;TeX Live 2022&#41;</string></value>
 </dict>
 </object>
 
@@ -8262,16 +8262,16 @@
 </list></value>
 <key>Root</key>
 <value><ref id="335" /></value>
 <key>Info</key>
 <value><ref id="336" /></value>
 <key>ID</key>
 <value><list size="2">
-<string size="16">&#251;&#8;izI&#141;WJ&#241;:&#182;&#248;&#196;&#170;&#233;L</string>
-<string size="16">&#251;&#8;izI&#141;WJ&#241;:&#182;&#248;&#196;&#170;&#233;L</string>
+<string size="16">&#143;l&#165;.&#225;&#252;O=R&#142;&#215;&#170;&#15;&#145;&#29;&#139;</string>
+<string size="16">&#143;l&#165;.&#225;&#252;O=R&#142;&#215;&#170;&#15;&#145;&#29;&#139;</string>
 </list></value>
 <key>Filter</key>
 <value><literal>FlateDecode</literal></value>
 <key>Length</key>
 <value><number>886</number></value>
 </dict>
 </props>
@@ -8298,16 +8298,16 @@
 </list></value>
 <key>Root</key>
 <value><ref id="335" /></value>
 <key>Info</key>
 <value><ref id="336" /></value>
 <key>ID</key>
 <value><list size="2">
-<string size="16">&#251;&#8;izI&#141;WJ&#241;:&#182;&#248;&#196;&#170;&#233;L</string>
-<string size="16">&#251;&#8;izI&#141;WJ&#241;:&#182;&#248;&#196;&#170;&#233;L</string>
+<string size="16">&#143;l&#165;.&#225;&#252;O=R&#142;&#215;&#170;&#15;&#145;&#29;&#139;</string>
+<string size="16">&#143;l&#165;.&#225;&#252;O=R&#142;&#215;&#170;&#15;&#145;&#29;&#139;</string>
 </list></value>
 <key>Filter</key>
 <value><literal>FlateDecode</literal></value>
 <key>Length</key>
 <value><number>886</number></value>
 </dict>
 </trailer>
```

### Comparing `shiny_mdc-1.0.0/test/samples/iclr.pdf` & `shiny_mdc-1.0.1/test/samples/iclr.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 4% similar despite different names*

#### pdftotext {} -

```diff
@@ -64,14 +64,17 @@
 
 2
 
 Typography
 • Bold
 • Italic
 • Bold italic.
+
+* Equal contribution.
+
 1
 
 3
 
 Numbers
 • Normal: 0123456789
 • Math: 0123456789
@@ -101,32 +104,28 @@
 a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t, u, v, w, x, y, z, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9
 R∞
 2
 • Inline: 0 exp−x dx
 • Block: Equation 1, Equation 2
 • Commands defined in body (P[x in X]): P[x ∈ X ]
 • Aligned:
-
-(2)
-
 x=1
 x + y = 10
 x + y + z = 100
 
 6
 
 Links
 • Section: Section 1, Section 1.2
 • Appendix section: Section B, Section A.1.1
 • Appendix figure: Figure A4
 • Appendix table: Table B1
 • Appendix math: Equation 4
 • Short citation(Mittelbach et al., 2004)
-• Long citation: Mittelbach et al. (2004)(Mittelbach et al., 2004), Lesk & Kernighan
-(1977)(Lesk & Kernighan, 1977)
+• Long citation: Mittelbach et al. (2004), Lesk & Kernighan (1977)
 • Multi citation(Lesk & Kernighan, 1977; Knuth, 1984; Mittelbach et al., 2004)
 • Pointer to footnote¹
 
 7
 
 Tables
 • Table 1
@@ -136,17 +135,20 @@
 
 Figures
 • Figure 1
 • Figure 2
 • Figure 3, Figure 3a, Figure 3b
 ¹ Example footnote text.
 ² Footnote in sub-figure caption.
+³ Footnote in figure caption.
 
 2
 
+(2)
+
 Col1
 
 Col2
 
 Col3
 
 Col4
@@ -251,18 +253,18 @@
 
 References
 Donald E. Knuth. Literate programming. The Computer Journal, 27(2):97–111, 1984.
 Donald E. Knuth. The TEX Book. Addison-Wesley Professional, 1986.
 Michael Lesk and Brian Kernighan. Computer typesetting of technical journals on UNIX. In
 Proceedings of American Federation of Information Processing Societies: 1977 National Computer
 Conference, pp. 879–888, Dallas, Texas, 1977.
+Frank Mittelbach, Michel Gossens, Johannes Braams, David Carlisle, and Chris Rowley. The LATEX
+Companion. Addison-Wesley Professional, 2 edition, 2004.
 
 Figure 1: Narrow figure
-³ Footnote in figure caption.
-
 3
 
 A
 B
 C
 D
 E
@@ -280,26 +282,24 @@
 
 68
 
 x
 
 70
 
+Figure 2: Wide figure
+
+4
+
 72
 
 74
 
 76
 
-Figure 2: Wide figure
-Frank Mittelbach, Michel Gossens, Johannes Braams, David Carlisle, and Chris Rowley. The LATEX
-Companion. Addison-Wesley Professional, 2 edition, 2004.
-
-4
-
 (a) Figure with ‘width=2.5in’
 
 dataset = I
 
 dataset = II
 
 dataset = III
@@ -464,15 +464,15 @@
 
 Appendix links
 • Appendix section: Section A.1.1, Section B
 • Main body section: Section 1
 • Main body figure: Figure 1
 • Main body table: Table 1
 • Main body equation: Equation 1
-• Citation: Knuth (1984)(Knuth, 1984)
+• Citation: Knuth (1984)
 
 8
 
 Col1
 
 Col2
```

### Comparing `shiny_mdc-1.0.0/test/samples/icml.pdf` & `shiny_mdc-1.0.1/test/samples/icml.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 4% similar despite different names*

#### pdftotext {} -

```diff
@@ -169,44 +169,42 @@
 R∞
 2
 • Inline: 0 exp−x dx
 • Block: Equation 1, Equation 2
 • Commands defined in body (P[x in X]): P[x ∈ X ]
 • Aligned:
 
-8. Figures
-
 x=1
 x + y = 10
 x + y + z = 100
 
 6. Links
 • Section: Section 1, Section 1.2
 • Appendix section: Section B, Section A.1.1
 • Appendix figure: Figure A4
 • Appendix table: Table B1
 • Appendix math: Equation 4
 • Short citation(Mittelbach et al., 2004)
-• Long citation: Mittelbach et al. (2004)(Mittelbach
-et al., 2004), Lesk & Kernighan (1977)(Lesk &
-Kernighan, 1977)
+• Long citation: Mittelbach et al. (2004), Lesk &
+Kernighan (1977)
 • Multi citation(Lesk & Kernighan, 1977; Knuth, 1984;
 Mittelbach et al., 2004)
 • Pointer to footnote1
 
-7. Tables
-• Table 1
-• Table 2
-
 Figure 1. Narrow figure
 
+8. Figures
 • Figure 1
 • Figure 2
 • Figure 3, Figure 3a, Figure 3b
 
+7. Tables
+• Table 1
+• Table 2
+
 9. Includes
 
 Col1
 
 Col2
 
 Col3
@@ -225,33 +223,32 @@
 33
 333
 
 4
 44
 444
 
-• Commands from metadata include: arg min R
-• Include command in body (there should be text after
-this):
-Content added through include statement.
-
 Table 1. Short table
 
-2
+• Commands from metadata include: arg min R
+•1 Include command in body (there should be text after
+Example footnote text.
+2 this):
 
 Footnote in sub-figure caption.
 Footnote in figure caption.
 4
-Footnote in figure caption.
+Content
+Footnote
+added
+in through
+figure caption.
+include statement.
 3
 
-1
-
-Example footnote text.
-
 A
 B
 C
 D
 E
 F
 G
@@ -397,15 +394,15 @@
 Content added through include statement.
 A.4. Appendix links
 • Appendix section: Section A.1.1, Section B
 • Main body section: Section 1
 • Main body figure: Figure 1
 • Main body table: Table 1
 • Main body equation: Equation 1
-• Citation: Knuth (1984)(Knuth, 1984)
+• Citation: Knuth (1984)
 
 (a) Figure with non-default extension
 
 (b) Sub-figure
 
 dataset = I
```

### Comparing `shiny_mdc-1.0.0/test/samples/neurips.pdf` & `shiny_mdc-1.0.1/test/samples/neurips.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 4% similar despite different names*

#### pdftotext {} -

```diff
@@ -114,15 +114,15 @@
 Links
 • Section: Section 1, Section 1.2
 • Appendix section: Section B, Section A.1.1
 • Appendix figure: Figure A4
 • Appendix table: Table B1
 • Appendix math: Equation 4
 • Short citation[2]
-• Long citation: Mittelbach et al. (2004)[2], Lesk and Kernighan (1977)[3]
+• Long citation: Mittelbach et al. (2004) [2], Lesk and Kernighan (1977) [3]
 • Multi citation[2–4]
 • Pointer to footnote1
 
 7
 
 Tables
 • Table 1
@@ -463,15 +463,15 @@
 
 15
 
 • Main body section: Section 1
 • Main body figure: Figure 1
 • Main body table: Table 1
 • Main body equation: Equation 1
-• Citation: Knuth (1984)[4]
+• Citation: Knuth (1984) [4]
 
 9
 
 Col1
 
 Col2
```

### Comparing `shiny_mdc-1.0.0/test/samples/spacious.pdf` & `shiny_mdc-1.0.1/test/samples/spacious.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 1% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'594482'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'594482'*

 * *DEBUG:pdfminer.psparser:seek: 594482*

 * *DEBUG:pdfminer.psparser:nexttoken: (594482, 448)*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=594482, token=448*

 * *DEBUG:pdfminer.psparser:seek: 594482*

 * *DEBUG:pdfminer.psparser:nexttoken: (594482, 448)*

 * *DEBUG:pdfminer.psparser:nexttoken: (594486, 0)*

 * *DEBUG:pdfminer.psparser:nexttoken: (594488, /b'obj')*

 * *DEBUG:pdfminer.psparser:nexttoken: (594492, /b'<<')*

 * *DEBUG:pdfminer.psparser:start_type: pos=594492, type='d'*

 * *DEBUG:pdfminer.psparser:nexttoken: (594495, /'Type')*

 * *DEBUG:pdfminer.psparser:nexttoken: (594501, /'XRef')*

 * *DEBUG:pdfminer.psparser:nexttoken: (594507, /'Index')*

 * *DEBUG:pdfminer.psparser:nexttoken: (594514, /b'[')*

 * *DEBUG:pdfminer.psparser:start_type: pos=594514, type='a'*

 * *DEBUG:pdfminer.psparser:nexttoken: (594516, 0)*

 * *DEBUG:pdfminer.psparser:nexttoken: (594518, 449)*

 * *DEBUG:pdfminer.psparser:nexttoken: (594522, /b']')*

 * *DEBUG:pdfminer.psparser:end_type: pos=594514, type='a', objs=[0, 449]*

 * *DEBUG:pdfminer.psparser:nexttoken: (594524, /'Size')*

 * *[ truncated after 25 lines; 18040 ignored ]*

```diff
@@ -10083,17 +10083,17 @@
 <key>Creator</key>
 <value><string size="19">LaTeX with hyperref</string></value>
 <key>Keywords</key>
 <value><string size="0"></string></value>
 <key>Producer</key>
 <value><string size="13">LuaTeX-1.15.0</string></value>
 <key>CreationDate</key>
-<value><string size="23">D:20230411142502-04&#39;00&#39;</string></value>
+<value><string size="23">D:20230411205019-04&#39;00&#39;</string></value>
 <key>ModDate</key>
-<value><string size="23">D:20230411142502-04&#39;00&#39;</string></value>
+<value><string size="23">D:20230411205019-04&#39;00&#39;</string></value>
 <key>Trapped</key>
 <value><literal>False</literal></value>
 <key>PTEX.FullBanner</key>
 <value><string size="48">This is LuaHBTeX, Version 1.15.0 &#40;TeX Live 2022&#41;</string></value>
 </dict>
 </object>
 
@@ -10118,16 +10118,16 @@
 </list></value>
 <key>Root</key>
 <value><ref id="446" /></value>
 <key>Info</key>
 <value><ref id="447" /></value>
 <key>ID</key>
 <value><list size="2">
-<string size="16">&#214;19&#232;&#198;&#147;&#178;;&#60;&#13;&#153;&#220;&#62;V=&#146;</string>
-<string size="16">&#214;19&#232;&#198;&#147;&#178;;&#60;&#13;&#153;&#220;&#62;V=&#146;</string>
+<string size="16">&#246;Ad&#202;&#192;&#15;&#1;&#166;&#152;&#149;&#127;&#0;&#135;&#129;{U</string>
+<string size="16">&#246;Ad&#202;&#192;&#15;&#1;&#166;&#152;&#149;&#127;&#0;&#135;&#129;{U</string>
 </list></value>
 <key>Filter</key>
 <value><literal>FlateDecode</literal></value>
 <key>Length</key>
 <value><number>1138</number></value>
 </dict>
 </props>
@@ -10154,16 +10154,16 @@
 </list></value>
 <key>Root</key>
 <value><ref id="446" /></value>
 <key>Info</key>
 <value><ref id="447" /></value>
 <key>ID</key>
 <value><list size="2">
-<string size="16">&#214;19&#232;&#198;&#147;&#178;;&#60;&#13;&#153;&#220;&#62;V=&#146;</string>
-<string size="16">&#214;19&#232;&#198;&#147;&#178;;&#60;&#13;&#153;&#220;&#62;V=&#146;</string>
+<string size="16">&#246;Ad&#202;&#192;&#15;&#1;&#166;&#152;&#149;&#127;&#0;&#135;&#129;{U</string>
+<string size="16">&#246;Ad&#202;&#192;&#15;&#1;&#166;&#152;&#149;&#127;&#0;&#135;&#129;{U</string>
 </list></value>
 <key>Filter</key>
 <value><literal>FlateDecode</literal></value>
 <key>Length</key>
 <value><number>1138</number></value>
 </dict>
 </trailer>
```

### Comparing `shiny_mdc-1.0.0/test/samples/standalone.pdf` & `shiny_mdc-1.0.1/test/samples/standalone.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 0% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'529012'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'529012'*

 * *DEBUG:pdfminer.psparser:seek: 529012*

 * *DEBUG:pdfminer.psparser:nexttoken: (529012, 287)*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=529012, token=287*

 * *DEBUG:pdfminer.psparser:seek: 529012*

 * *DEBUG:pdfminer.psparser:nexttoken: (529012, 287)*

 * *DEBUG:pdfminer.psparser:nexttoken: (529016, 0)*

 * *DEBUG:pdfminer.psparser:nexttoken: (529018, /b'obj')*

 * *DEBUG:pdfminer.psparser:nexttoken: (529022, /b'<<')*

 * *DEBUG:pdfminer.psparser:start_type: pos=529022, type='d'*

 * *DEBUG:pdfminer.psparser:nexttoken: (529025, /'Type')*

 * *DEBUG:pdfminer.psparser:nexttoken: (529031, /'XRef')*

 * *DEBUG:pdfminer.psparser:nexttoken: (529037, /'Index')*

 * *DEBUG:pdfminer.psparser:nexttoken: (529044, /b'[')*

 * *DEBUG:pdfminer.psparser:start_type: pos=529044, type='a'*

 * *DEBUG:pdfminer.psparser:nexttoken: (529046, 0)*

 * *DEBUG:pdfminer.psparser:nexttoken: (529048, 288)*

 * *DEBUG:pdfminer.psparser:nexttoken: (529052, /b']')*

 * *DEBUG:pdfminer.psparser:end_type: pos=529044, type='a', objs=[0, 288]*

 * *DEBUG:pdfminer.psparser:nexttoken: (529054, /'Size')*

 * *[ truncated after 25 lines; 11694 ignored ]*

```diff
@@ -6833,17 +6833,17 @@
 <key>Creator</key>
 <value><string size="19">LaTeX with hyperref</string></value>
 <key>Keywords</key>
 <value><string size="0"></string></value>
 <key>Producer</key>
 <value><string size="13">LuaTeX-1.15.0</string></value>
 <key>CreationDate</key>
-<value><string size="23">D:20230411142506-04&#39;00&#39;</string></value>
+<value><string size="23">D:20230411205023-04&#39;00&#39;</string></value>
 <key>ModDate</key>
-<value><string size="23">D:20230411142506-04&#39;00&#39;</string></value>
+<value><string size="23">D:20230411205023-04&#39;00&#39;</string></value>
 <key>Trapped</key>
 <value><literal>False</literal></value>
 <key>PTEX.FullBanner</key>
 <value><string size="48">This is LuaHBTeX, Version 1.15.0 &#40;TeX Live 2022&#41;</string></value>
 </dict>
 </object>
 
@@ -6868,16 +6868,16 @@
 </list></value>
 <key>Root</key>
 <value><ref id="285" /></value>
 <key>Info</key>
 <value><ref id="286" /></value>
 <key>ID</key>
 <value><list size="2">
-<string size="16">&#227;&#0;&#194;&#173;+t&#15;&#10;&#189;I&#128;&#150;H&#184;&#226;&#243;</string>
-<string size="16">&#227;&#0;&#194;&#173;+t&#15;&#10;&#189;I&#128;&#150;H&#184;&#226;&#243;</string>
+<string size="16">&#4;&#127;=&#133;&#204;},&#198;J&#159;&#155;VL&#146;&#223;X</string>
+<string size="16">&#4;&#127;=&#133;&#204;},&#198;J&#159;&#155;VL&#146;&#223;X</string>
 </list></value>
 <key>Filter</key>
 <value><literal>FlateDecode</literal></value>
 <key>Length</key>
 <value><number>736</number></value>
 </dict>
 </props>
@@ -6904,16 +6904,16 @@
 </list></value>
 <key>Root</key>
 <value><ref id="285" /></value>
 <key>Info</key>
 <value><ref id="286" /></value>
 <key>ID</key>
 <value><list size="2">
-<string size="16">&#227;&#0;&#194;&#173;+t&#15;&#10;&#189;I&#128;&#150;H&#184;&#226;&#243;</string>
-<string size="16">&#227;&#0;&#194;&#173;+t&#15;&#10;&#189;I&#128;&#150;H&#184;&#226;&#243;</string>
+<string size="16">&#4;&#127;=&#133;&#204;},&#198;J&#159;&#155;VL&#146;&#223;X</string>
+<string size="16">&#4;&#127;=&#133;&#204;},&#198;J&#159;&#155;VL&#146;&#223;X</string>
 </list></value>
 <key>Filter</key>
 <value><literal>FlateDecode</literal></value>
 <key>Length</key>
 <value><number>736</number></value>
 </dict>
 </trailer>
```

### Comparing `shiny_mdc-1.0.0/test/samples/stylish.pdf` & `shiny_mdc-1.0.1/test/samples/stylish.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 2% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'418087'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'418087'*

 * *DEBUG:pdfminer.psparser:seek: 418087*

 * *DEBUG:pdfminer.psparser:nexttoken: (418087, 455)*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=418087, token=455*

 * *DEBUG:pdfminer.psparser:seek: 418087*

 * *DEBUG:pdfminer.psparser:nexttoken: (418087, 455)*

 * *DEBUG:pdfminer.psparser:nexttoken: (418091, 0)*

 * *DEBUG:pdfminer.psparser:nexttoken: (418093, /b'obj')*

 * *DEBUG:pdfminer.psparser:nexttoken: (418097, /b'<<')*

 * *DEBUG:pdfminer.psparser:start_type: pos=418097, type='d'*

 * *DEBUG:pdfminer.psparser:nexttoken: (418100, /'Type')*

 * *DEBUG:pdfminer.psparser:nexttoken: (418106, /'XRef')*

 * *DEBUG:pdfminer.psparser:nexttoken: (418112, /'Index')*

 * *DEBUG:pdfminer.psparser:nexttoken: (418119, /b'[')*

 * *DEBUG:pdfminer.psparser:start_type: pos=418119, type='a'*

 * *DEBUG:pdfminer.psparser:nexttoken: (418121, 0)*

 * *DEBUG:pdfminer.psparser:nexttoken: (418123, 456)*

 * *DEBUG:pdfminer.psparser:nexttoken: (418127, /b']')*

 * *DEBUG:pdfminer.psparser:end_type: pos=418119, type='a', objs=[0, 456]*

 * *DEBUG:pdfminer.psparser:nexttoken: (418129, /'Size')*

 * *[ truncated after 25 lines; 18314 ignored ]*

```diff
@@ -10092,17 +10092,17 @@
 <key>Creator</key>
 <value><string size="19">LaTeX with hyperref</string></value>
 <key>Keywords</key>
 <value><string size="0"></string></value>
 <key>Producer</key>
 <value><string size="13">LuaTeX-1.15.0</string></value>
 <key>CreationDate</key>
-<value><string size="23">D:20230411142511-04&#39;00&#39;</string></value>
+<value><string size="23">D:20230411205028-04&#39;00&#39;</string></value>
 <key>ModDate</key>
-<value><string size="23">D:20230411142511-04&#39;00&#39;</string></value>
+<value><string size="23">D:20230411205028-04&#39;00&#39;</string></value>
 <key>Trapped</key>
 <value><literal>False</literal></value>
 <key>PTEX.FullBanner</key>
 <value><string size="48">This is LuaHBTeX, Version 1.15.0 &#40;TeX Live 2022&#41;</string></value>
 </dict>
 </object>
 
@@ -10127,16 +10127,16 @@
 </list></value>
 <key>Root</key>
 <value><ref id="453" /></value>
 <key>Info</key>
 <value><ref id="454" /></value>
 <key>ID</key>
 <value><list size="2">
-<string size="16">&#206;]&#26;&#11;$&#237;&#179;&#185;&#160;&#4;&#202;Q&#189;&#162;&#130;#</string>
-<string size="16">&#206;]&#26;&#11;$&#237;&#179;&#185;&#160;&#4;&#202;Q&#189;&#162;&#130;#</string>
+<string size="16">&#243;&#135;GY&#253;&#188;}Z&#220;&#167;&#236;&#157;&#222;?&#229;&#7;</string>
+<string size="16">&#243;&#135;GY&#253;&#188;}Z&#220;&#167;&#236;&#157;&#222;?&#229;&#7;</string>
 </list></value>
 <key>Filter</key>
 <value><literal>FlateDecode</literal></value>
 <key>Length</key>
 <value><number>1190</number></value>
 </dict>
 </props>
@@ -10163,16 +10163,16 @@
 </list></value>
 <key>Root</key>
 <value><ref id="453" /></value>
 <key>Info</key>
 <value><ref id="454" /></value>
 <key>ID</key>
 <value><list size="2">
-<string size="16">&#206;]&#26;&#11;$&#237;&#179;&#185;&#160;&#4;&#202;Q&#189;&#162;&#130;#</string>
-<string size="16">&#206;]&#26;&#11;$&#237;&#179;&#185;&#160;&#4;&#202;Q&#189;&#162;&#130;#</string>
+<string size="16">&#243;&#135;GY&#253;&#188;}Z&#220;&#167;&#236;&#157;&#222;?&#229;&#7;</string>
+<string size="16">&#243;&#135;GY&#253;&#188;}Z&#220;&#167;&#236;&#157;&#222;?&#229;&#7;</string>
 </list></value>
 <key>Filter</key>
 <value><literal>FlateDecode</literal></value>
 <key>Length</key>
 <value><number>1190</number></value>
 </dict>
 </trailer>
```

### Comparing `shiny_mdc-1.0.0/test/sections/appendix1.md` & `shiny_mdc-1.0.1/test/sections/appendix1.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.0.0/test/sections/appendix2.md` & `shiny_mdc-1.0.1/test/sections/appendix2.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.0.0/test/sections/main1.md` & `shiny_mdc-1.0.1/test/sections/main1.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.0.0/test/sections/main2.md` & `shiny_mdc-1.0.1/test/sections/main2.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.0.0/test/utils/commands.md` & `shiny_mdc-1.0.1/test/utils/commands.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.0.0/PKG-INFO` & `shiny_mdc-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shiny-mdc
-Version: 1.0.0
+Version: 1.0.1
 Summary: Tool to compile markdown files to tex/pdf using pandoc, latexmk
 Home-page: https://github.com/jayanthkoushik/shinymdc
 License: MIT
 Author: Jayanth Koushik
 Author-email: mail@jkoushik.me
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

