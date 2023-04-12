# Comparing `tmp/shiny_mdc-1.1.0.tar.gz` & `tmp/shiny_mdc-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shiny_mdc-1.1.0.tar", max compression
+gzip compressed data, was "shiny_mdc-1.2.0.tar", max compression
```

## Comparing `shiny_mdc-1.1.0.tar` & `shiny_mdc-1.2.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     1678 2023-04-12 05:28:44.092441 shiny_mdc-1.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1082 2023-04-12 05:28:44.092441 shiny_mdc-1.1.0/LICENSE
--rw-r--r--   0        0        0       78 2023-04-12 05:28:44.092441 shiny_mdc-1.1.0/README.md
--rw-r--r--   0        0        0     2295 2023-04-12 05:29:06.732437 shiny_mdc-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       34 2023-04-12 05:28:44.092441 shiny_mdc-1.1.0/shinymdc/__init__.py
--rw-r--r--   0        0        0     1061 2023-04-12 05:28:44.092441 shiny_mdc-1.1.0/shinymdc/_latexmk.py
--rw-r--r--   0        0        0     1867 2023-04-12 05:28:44.092441 shiny_mdc-1.1.0/shinymdc/_liquid.py
--rw-r--r--   0        0        0     4643 2023-04-12 05:28:44.092441 shiny_mdc-1.1.0/shinymdc/_pandoc.py
--rw-r--r--   0        0        0     4713 2023-04-12 05:28:44.092441 shiny_mdc-1.1.0/shinymdc/_templates.py
--rw-r--r--   0        0        0       64 2023-04-12 05:29:06.732437 shiny_mdc-1.1.0/shinymdc/_version.py
--rw-r--r--   0        0        0      312 2023-04-12 05:28:44.092441 shiny_mdc-1.1.0/shinymdc/resources/dynamic/addappendices.tex
--rw-r--r--   0        0        0      853 2023-04-12 05:28:44.092441 shiny_mdc-1.1.0/shinymdc/resources/dynamic/authsetup.tex
--rw-r--r--   0        0        0      290 2023-04-12 05:28:44.092441 shiny_mdc-1.1.0/shinymdc/resources/dynamic/authsetupshort.tex
--rw-r--r--   0        0        0      572 2023-04-12 05:28:44.092441 shiny_mdc-1.1.0/shinymdc/resources/dynamic/dblfloatsetup.tex
--rw-r--r--   0        0        0     3288 2023-04-12 05:28:44.092441 shiny_mdc-1.1.0/shinymdc/resources/static/floatsetup.tex
--rw-r--r--   0        0        0    19901 2023-04-12 05:28:44.092441 shiny_mdc-1.1.0/shinymdc/resources/static/iccv/bibstyle.bst
--rw-r--r--   0        0        0     9433 2023-04-12 05:28:44.092441 shiny_mdc-1.1.0/shinymdc/resources/static/iccv/esopic.sty
--rw-r--r--   0        0        0     3869 2023-04-12 05:28:44.092441 shiny_mdc-1.1.0/shinymdc/resources/static/iccv/everyshi.sty
--rw-r--r--   0        0        0     8276 2023-04-12 05:28:44.092441 shiny_mdc-1.1.0/shinymdc/resources/static/iccv/iccv.sty
--rw-r--r--   0        0        0    26973 2023-04-12 05:28:44.092441 shiny_mdc-1.1.0/shinymdc/resources/static/iclr/bibstyle.bst
--rw-r--r--   0        0        0     9153 2023-04-12 05:28:44.092441 shiny_mdc-1.1.0/shinymdc/resources/static/iclr/iclr.sty
--rw-r--r--   0        0        0    12284 2023-04-12 05:28:44.092441 shiny_mdc-1.1.0/shinymdc/resources/static/iclr/mathcommands.tex
--rw-r--r--   0        0        0    27146 2023-04-12 05:28:44.096441 shiny_mdc-1.1.0/shinymdc/resources/static/icml/bibstyle.bst
--rw-r--r--   0        0        0    27887 2023-04-12 05:28:44.096441 shiny_mdc-1.1.0/shinymdc/resources/static/icml/icml.sty
--rw-r--r--   0        0        0      735 2023-04-12 05:28:44.096441 shiny_mdc-1.1.0/shinymdc/resources/static/mathsetup.tex
--rw-r--r--   0        0        0     1041 2023-04-12 05:28:44.096441 shiny_mdc-1.1.0/shinymdc/resources/static/miscsetup.tex
--rw-r--r--   0        0        0    11306 2023-04-12 05:28:44.096441 shiny_mdc-1.1.0/shinymdc/resources/static/neurips/neurips.sty
--rw-r--r--   0        0        0      426 2023-04-12 05:28:44.096441 shiny_mdc-1.1.0/shinymdc/resources/static/reqsetup.tex
--rw-r--r--   0        0        0    16548 2023-04-12 05:28:44.096441 shiny_mdc-1.1.0/shinymdc/shinymdc.py
--rw-r--r--   0        0        0      977 2023-04-12 05:28:44.096441 shiny_mdc-1.1.0/shinymdc/templates/basic.tex
--rw-r--r--   0        0        0     1443 2023-04-12 05:28:44.096441 shiny_mdc-1.1.0/shinymdc/templates/iccv.tex
--rw-r--r--   0        0        0     1440 2023-04-12 05:28:44.096441 shiny_mdc-1.1.0/shinymdc/templates/iclr.tex
--rw-r--r--   0        0        0     2187 2023-04-12 05:28:44.096441 shiny_mdc-1.1.0/shinymdc/templates/icml.tex
--rw-r--r--   0        0        0      897 2023-04-12 05:28:44.096441 shiny_mdc-1.1.0/shinymdc/templates/neurips.tex
--rw-r--r--   0        0        0     2099 2023-04-12 05:28:44.096441 shiny_mdc-1.1.0/shinymdc/templates/spacious.tex
--rw-r--r--   0        0        0      511 2023-04-12 05:28:44.096441 shiny_mdc-1.1.0/shinymdc/templates/standalone.tex
--rw-r--r--   0        0        0     2343 2023-04-12 05:28:44.096441 shiny_mdc-1.1.0/shinymdc/templates/stylish.tex
--rw-r--r--   0        0        0    15953 2023-04-12 05:28:44.096441 shiny_mdc-1.1.0/test/figures/anscombe.pdf
--rw-r--r--   0        0        0    40892 2023-04-12 05:28:44.096441 shiny_mdc-1.1.0/test/figures/densities.pdf
--rw-r--r--   0        0        0    10736 2023-04-12 05:28:44.096441 shiny_mdc-1.1.0/test/figures/diamonds.pdf
--rw-r--r--   0        0        0   197017 2023-04-12 05:28:44.096441 shiny_mdc-1.1.0/test/figures/gaussian2d.pdf
--rw-r--r--   0        0        0    28282 2023-04-12 05:28:44.096441 shiny_mdc-1.1.0/test/figures/lines.png
--rw-r--r--   0        0        0     2971 2023-04-12 05:28:44.096441 shiny_mdc-1.1.0/test/main.md
--rwxr-xr-x   0        0        0      315 2023-04-12 05:28:44.096441 shiny_mdc-1.1.0/test/make.sh
--rw-r--r--   0        0        0     1166 2023-04-12 05:28:44.096441 shiny_mdc-1.1.0/test/references.bib
--rw-r--r--   0        0        0   678739 2023-04-12 05:28:44.100441 shiny_mdc-1.1.0/test/samples/basic.pdf
--rw-r--r--   0        0        0   411248 2023-04-12 05:28:44.104441 shiny_mdc-1.1.0/test/samples/iccv.pdf
--rw-r--r--   0        0        0   404522 2023-04-12 05:28:44.104441 shiny_mdc-1.1.0/test/samples/iclr.pdf
--rw-r--r--   0        0        0   442985 2023-04-12 05:28:44.108441 shiny_mdc-1.1.0/test/samples/icml.pdf
--rw-r--r--   0        0        0   449267 2023-04-12 05:28:44.108441 shiny_mdc-1.1.0/test/samples/neurips.pdf
--rw-r--r--   0        0        0   596993 2023-04-12 05:28:44.112441 shiny_mdc-1.1.0/test/samples/spacious.pdf
--rw-r--r--   0        0        0   548586 2023-04-12 05:28:44.112441 shiny_mdc-1.1.0/test/samples/standalone.pdf
--rw-r--r--   0        0        0   420424 2023-04-12 05:28:44.116441 shiny_mdc-1.1.0/test/samples/stylish.pdf
--rw-r--r--   0        0        0     1535 2023-04-12 05:28:44.116441 shiny_mdc-1.1.0/test/sections/appendix1.md
--rw-r--r--   0        0        0     1619 2023-04-12 05:28:44.116441 shiny_mdc-1.1.0/test/sections/appendix2.md
--rw-r--r--   0        0        0        0 2023-04-12 05:28:44.116441 shiny_mdc-1.1.0/test/sections/empty.md
--rw-r--r--   0        0        0     1356 2023-04-12 05:28:44.116441 shiny_mdc-1.1.0/test/sections/main1.md
--rw-r--r--   0        0        0     1351 2023-04-12 05:28:44.116441 shiny_mdc-1.1.0/test/sections/main2.md
--rw-r--r--   0        0        0      992 2023-04-12 05:28:44.116441 shiny_mdc-1.1.0/test/utils/commands.md
--rw-r--r--   0        0        0       41 2023-04-12 05:28:44.116441 shiny_mdc-1.1.0/test/utils/ext.md
--rw-r--r--   0        0        0     1004 1970-01-01 00:00:00.000000 shiny_mdc-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2246 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1082 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/LICENSE
+-rw-r--r--   0        0        0       78 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/README.md
+-rw-r--r--   0        0        0     2295 2023-04-12 21:01:55.260967 shiny_mdc-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/__init__.py
+-rw-r--r--   0        0        0     1061 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/_latexmk.py
+-rw-r--r--   0        0        0     1867 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/_liquid.py
+-rw-r--r--   0        0        0     4643 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/_pandoc.py
+-rw-r--r--   0        0        0     4713 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/_templates.py
+-rw-r--r--   0        0        0       64 2023-04-12 21:01:55.260967 shiny_mdc-1.2.0/shinymdc/_version.py
+-rw-r--r--   0        0        0      337 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/resources/dynamic/addappendices.tex
+-rw-r--r--   0        0        0      853 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/resources/dynamic/authsetup.tex
+-rw-r--r--   0        0        0      290 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/resources/dynamic/authsetupshort.tex
+-rw-r--r--   0        0        0      572 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/resources/dynamic/dblfloatsetup.tex
+-rw-r--r--   0        0        0     3359 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/resources/static/floatsetup.tex
+-rw-r--r--   0        0        0    19901 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/resources/static/iccv/bibstyle.bst
+-rw-r--r--   0        0        0     9433 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/resources/static/iccv/esopic.sty
+-rw-r--r--   0        0        0     3869 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/resources/static/iccv/everyshi.sty
+-rw-r--r--   0        0        0     8276 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/resources/static/iccv/iccv.sty
+-rw-r--r--   0        0        0    26973 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/resources/static/iclr/bibstyle.bst
+-rw-r--r--   0        0        0     9153 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/resources/static/iclr/iclr.sty
+-rw-r--r--   0        0        0    12284 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/resources/static/iclr/mathcommands.tex
+-rw-r--r--   0        0        0    27146 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/resources/static/icml/bibstyle.bst
+-rw-r--r--   0        0        0    27887 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/resources/static/icml/icml.sty
+-rw-r--r--   0        0        0      735 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/resources/static/mathsetup.tex
+-rw-r--r--   0        0        0     1041 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/resources/static/miscsetup.tex
+-rw-r--r--   0        0        0    11306 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/resources/static/neurips/neurips.sty
+-rw-r--r--   0        0        0      426 2023-04-12 21:01:30.036997 shiny_mdc-1.2.0/shinymdc/resources/static/reqsetup.tex
+-rw-r--r--   0        0        0    16580 2023-04-12 21:01:30.040997 shiny_mdc-1.2.0/shinymdc/shinymdc.py
+-rw-r--r--   0        0        0      977 2023-04-12 21:01:30.040997 shiny_mdc-1.2.0/shinymdc/templates/basic.tex
+-rw-r--r--   0        0        0     1443 2023-04-12 21:01:30.040997 shiny_mdc-1.2.0/shinymdc/templates/iccv.tex
+-rw-r--r--   0        0        0     1440 2023-04-12 21:01:30.040997 shiny_mdc-1.2.0/shinymdc/templates/iclr.tex
+-rw-r--r--   0        0        0     2187 2023-04-12 21:01:30.040997 shiny_mdc-1.2.0/shinymdc/templates/icml.tex
+-rw-r--r--   0        0        0      897 2023-04-12 21:01:30.040997 shiny_mdc-1.2.0/shinymdc/templates/neurips.tex
+-rw-r--r--   0        0        0     2099 2023-04-12 21:01:30.040997 shiny_mdc-1.2.0/shinymdc/templates/spacious.tex
+-rw-r--r--   0        0        0      511 2023-04-12 21:01:30.040997 shiny_mdc-1.2.0/shinymdc/templates/standalone.tex
+-rw-r--r--   0        0        0     2343 2023-04-12 21:01:30.040997 shiny_mdc-1.2.0/shinymdc/templates/stylish.tex
+-rw-r--r--   0        0        0    15953 2023-04-12 21:01:30.040997 shiny_mdc-1.2.0/test/figures/anscombe.pdf
+-rw-r--r--   0        0        0    40892 2023-04-12 21:01:30.040997 shiny_mdc-1.2.0/test/figures/densities.pdf
+-rw-r--r--   0        0        0    10736 2023-04-12 21:01:30.040997 shiny_mdc-1.2.0/test/figures/diamonds.pdf
+-rw-r--r--   0        0        0   197017 2023-04-12 21:01:30.040997 shiny_mdc-1.2.0/test/figures/gaussian2d.pdf
+-rw-r--r--   0        0        0    28282 2023-04-12 21:01:30.040997 shiny_mdc-1.2.0/test/figures/lines.png
+-rw-r--r--   0        0        0     2971 2023-04-12 21:01:30.040997 shiny_mdc-1.2.0/test/main.md
+-rwxr-xr-x   0        0        0      315 2023-04-12 21:01:30.040997 shiny_mdc-1.2.0/test/make.sh
+-rw-r--r--   0        0        0     1166 2023-04-12 21:01:30.040997 shiny_mdc-1.2.0/test/references.bib
+-rw-r--r--   0        0        0   678733 2023-04-12 21:01:30.044997 shiny_mdc-1.2.0/test/samples/basic.pdf
+-rw-r--r--   0        0        0   411241 2023-04-12 21:01:30.044997 shiny_mdc-1.2.0/test/samples/iccv.pdf
+-rw-r--r--   0        0        0   404508 2023-04-12 21:01:30.048997 shiny_mdc-1.2.0/test/samples/iclr.pdf
+-rw-r--r--   0        0        0   443714 2023-04-12 21:01:30.048997 shiny_mdc-1.2.0/test/samples/icml.pdf
+-rw-r--r--   0        0        0   449285 2023-04-12 21:01:30.052997 shiny_mdc-1.2.0/test/samples/neurips.pdf
+-rw-r--r--   0        0        0   599001 2023-04-12 21:01:30.056997 shiny_mdc-1.2.0/test/samples/spacious.pdf
+-rw-r--r--   0        0        0   548590 2023-04-12 21:01:30.060997 shiny_mdc-1.2.0/test/samples/standalone.pdf
+-rw-r--r--   0        0        0   421381 2023-04-12 21:01:30.060997 shiny_mdc-1.2.0/test/samples/stylish.pdf
+-rw-r--r--   0        0        0     1535 2023-04-12 21:01:30.060997 shiny_mdc-1.2.0/test/sections/appendix1.md
+-rw-r--r--   0        0        0     1619 2023-04-12 21:01:30.060997 shiny_mdc-1.2.0/test/sections/appendix2.md
+-rw-r--r--   0        0        0        0 2023-04-12 21:01:30.060997 shiny_mdc-1.2.0/test/sections/empty.md
+-rw-r--r--   0        0        0     1356 2023-04-12 21:01:30.060997 shiny_mdc-1.2.0/test/sections/main1.md
+-rw-r--r--   0        0        0     1351 2023-04-12 21:01:30.060997 shiny_mdc-1.2.0/test/sections/main2.md
+-rw-r--r--   0        0        0      992 2023-04-12 21:01:30.060997 shiny_mdc-1.2.0/test/utils/commands.md
+-rw-r--r--   0        0        0       41 2023-04-12 21:01:30.060997 shiny_mdc-1.2.0/test/utils/ext.md
+-rw-r--r--   0        0        0     1004 1970-01-01 00:00:00.000000 shiny_mdc-1.2.0/PKG-INFO
```

### Comparing `shiny_mdc-1.1.0/CHANGELOG.md` & `shiny_mdc-1.2.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
+## [1.2.0](https://github.com/jayanthkoushik/shiny-mdc/compare/v1.1.0...v1.2.0) (2023-04-12)
+
+
+### Features
+
+* use more organized tex folder structure ([4296148](https://github.com/jayanthkoushik/shiny-mdc/commit/4296148d049c41634f80e8aa9535a5710d7d7874))
+
+
+### Bug Fixes
+
+* fix handling of labels in figures and tables ([0a6fb66](https://github.com/jayanthkoushik/shiny-mdc/commit/0a6fb6669cbc763f22af11dca108a489df60a8d4))
+* reset figure counter in appendices ([de0514b](https://github.com/jayanthkoushik/shiny-mdc/commit/de0514be47f1c50be1eb9a551ab82767a0b87fe1))
+
 ## [1.1.0](https://github.com/jayanthkoushik/shiny-mdc/compare/v1.0.1...v1.1.0) (2023-04-12)
 
 
 ### Features
 
 * align author list in `authsetup` using fixed size boxes ([ebfa391](https://github.com/jayanthkoushik/shiny-mdc/commit/ebfa3914b635f8609f6c3651ea7455b5649f02e9))
 * increase max figure/table width for spacious and basic templates ([773ec2c](https://github.com/jayanthkoushik/shiny-mdc/commit/773ec2c9ddb6843e8eaa3b38c8f1f2c4844db46c))
```

### Comparing `shiny_mdc-1.1.0/LICENSE` & `shiny_mdc-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/pyproject.toml` & `shiny_mdc-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shiny-mdc"
-version = "1.1.0"  # managed by `poetry-dynamic-versioning`
+version = "1.2.0"  # managed by `poetry-dynamic-versioning`
 description = "Tool to compile markdown files to tex/pdf using pandoc, latexmk"
 readme = "README.md"
 authors = ["Jayanth Koushik <mail@jkoushik.me>"]
 license = "MIT"
 repository = "https://github.com/jayanthkoushik/shinymdc"
 packages = [
   { include = "shinymdc" }
```

### Comparing `shiny_mdc-1.1.0/shinymdc/_latexmk.py` & `shiny_mdc-1.2.0/shinymdc/_latexmk.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/shinymdc/_liquid.py` & `shiny_mdc-1.2.0/shinymdc/_liquid.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/shinymdc/_pandoc.py` & `shiny_mdc-1.2.0/shinymdc/_pandoc.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/shinymdc/_templates.py` & `shiny_mdc-1.2.0/shinymdc/_templates.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/shinymdc/resources/dynamic/authsetup.tex` & `shiny_mdc-1.2.0/shinymdc/resources/dynamic/authsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/shinymdc/resources/dynamic/dblfloatsetup.tex` & `shiny_mdc-1.2.0/shinymdc/resources/dynamic/dblfloatsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/shinymdc/resources/static/floatsetup.tex` & `shiny_mdc-1.2.0/shinymdc/resources/static/floatsetup.tex`

 * *Files 8% similar despite different names*

```diff
@@ -45,30 +45,37 @@
 
 % Automatically adjust figure layout based on width.
 \let\oldfigure\figure
 \let\endoldfigure\endfigure
 \RenewEnviron{figure}{
   % Save old caption/label commands.
   \let\oldcaption\caption
-  \let\oldlabel\label
   \let\oldsetcaptionsubtype\setcaptionsubtype
+  \let\oldlabel\label
 
+  \renewcommand{\setcaptionsubtype}{}
   % Update caption/label commands to save the values to a global variable.
   \renewcommand{\caption}[2][]{\global\def\mdccap{##2}}
-  \renewcommand{\label}[1]{\global\def\mdclab{##1}}
-  \renewcommand{\setcaptionsubtype}{}
+  % Label command is updated conditionally based on if 'insubfloat' is defined.
+  \renewcommand{\label}[1]{%
+    \ifdefined\insubfloat
+      \oldlabel{##1}
+    \else
+      \global\def\mdclab{##1}
+    \fi
+  }
+
+  % Update \subfloat to define 'insubfloat' so that labels within sub-floats still work.
+  \let\oldsubfloat\subfloat
+  \renewcommand{\subfloat}[2][]{\def\insubfloat{}\oldsubfloat[##1]{##2}\let\insubfloat\undefined}
 
   % Render the body inside a box.
   \sbox{0}{\BODY}
 
   \let\setcaptionsubtype\oldsetcaptionsubtype
-  % Restore the label command so that sub-figures will have their labels
-  % set properly. TODO: this leads to multiply defined top level labels,
-  % which doesn't seem to cause any issues, but try to avoid.
-  \let\label\oldlabel
 
   % Save the linewidth to a constant (the macro will change depending on environment).
   \xdef\thelinew{\the\linewidth}
 
   \ifdim\wd0>\thelinew
     \begin{figure*}[tbp]
   \else
@@ -94,27 +101,25 @@
 
   \ifdim\wd0>\thelinew
     \end{figure*}
   \else
     \end{oldfigure}
   \fi
 
-  % Restore caption command.
+  % Restore caption/label commands.
   \let\caption\oldcaption
+  \let\label\oldlabel
 }
 
 % Automatically adjust table layout based on width.
 \let\oldtable\table
 \let\endoldtable\endtable
 \RenewEnviron{table}{
   \let\oldcaption\caption
-  \let\oldlabel\label
-
   \renewcommand{\caption}[2][]{\global\def\mdccap{##2}}
-  \renewcommand{\label}[1]{\global\def\mdclab{##1}}
 
   \sbox{0}{\BODY}
 
   \xdef\thelinew{\the\linewidth}
 
   \ifdim\wd0>\thelinew
     \begin{table*}[tbp]
@@ -123,15 +128,14 @@
   \fi
 
       \begin{adjustbox}{center}
         \maxsizebox{\maxtabwidth}{\maxtabheight}{\BODY}
       \end{adjustbox}
 
       \oldcaption{\mdccap}
-      \oldlabel{\mdclab}
 
   \ifdim\wd0>\thelinew
     \end{table*}
   \else
     \end{oldtable}
   \fi
 }
```

### Comparing `shiny_mdc-1.1.0/shinymdc/resources/static/iccv/bibstyle.bst` & `shiny_mdc-1.2.0/shinymdc/resources/static/iccv/bibstyle.bst`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/shinymdc/resources/static/iccv/esopic.sty` & `shiny_mdc-1.2.0/shinymdc/resources/static/iccv/esopic.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/shinymdc/resources/static/iccv/everyshi.sty` & `shiny_mdc-1.2.0/shinymdc/resources/static/iccv/everyshi.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/shinymdc/resources/static/iccv/iccv.sty` & `shiny_mdc-1.2.0/shinymdc/resources/static/iccv/iccv.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/shinymdc/resources/static/iclr/bibstyle.bst` & `shiny_mdc-1.2.0/shinymdc/resources/static/iclr/bibstyle.bst`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/shinymdc/resources/static/iclr/iclr.sty` & `shiny_mdc-1.2.0/shinymdc/resources/static/iclr/iclr.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/shinymdc/resources/static/iclr/mathcommands.tex` & `shiny_mdc-1.2.0/shinymdc/resources/static/iclr/mathcommands.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/shinymdc/resources/static/icml/bibstyle.bst` & `shiny_mdc-1.2.0/shinymdc/resources/static/icml/bibstyle.bst`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/shinymdc/resources/static/icml/icml.sty` & `shiny_mdc-1.2.0/shinymdc/resources/static/icml/icml.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/shinymdc/resources/static/mathsetup.tex` & `shiny_mdc-1.2.0/shinymdc/resources/static/mathsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/shinymdc/resources/static/miscsetup.tex` & `shiny_mdc-1.2.0/shinymdc/resources/static/miscsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/shinymdc/resources/static/neurips/neurips.sty` & `shiny_mdc-1.2.0/shinymdc/resources/static/neurips/neurips.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/shinymdc/shinymdc.py` & `shiny_mdc-1.2.0/shinymdc/shinymdc.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,34 +289,34 @@
         _input_template = r"\input{%s}"
 
         # Save body.
         if body_tex:
             body_tex_path = self.tex_files_dir / "body.tex"
             print(f"+ write '{body_tex_path}'", file=sys.stderr)
             body_tex_path.write_text(body_tex)
-            metadata["body"] = _input_template % body_tex_path
+            metadata["body"] = _input_template % body_tex_path.with_suffix("")
 
         # Save abstract.
         if abstract_tex:
             abstract_tex_path = self.tex_files_dir / "abstract.tex"
             print(f"+ write '{abstract_tex_path}'", file=sys.stderr)
             abstract_tex_path.write_text(abstract_tex)
-            metadata["abstract"] = _input_template % abstract_tex_path
+            metadata["abstract"] = _input_template % abstract_tex_path.with_suffix("")
 
         def _write_tex_and_get_pstrs(texs, metadata_key, otype):
             new_pstrs = []
             for _tex, _old_pstr in zip(texs, metadata.get(metadata_key, [])):
                 _tex = _tex.strip()
                 if not _tex:
                     continue
                 old_fname = Path(_old_pstr).stem
                 new_tex_path = self.tex_files_dir / f"{otype}_{old_fname}.tex"
                 print(f"+ write '{new_tex_path}'", file=sys.stderr)
                 new_tex_path.write_text(_tex)
-                new_pstrs.append(str(new_tex_path))
+                new_pstrs.append(str(new_tex_path.with_suffix("")))
             return new_pstrs
 
         section_tex_pstrs = _write_tex_and_get_pstrs(
             sections_tex, "sections", "section"
         )
         include_tex_pstrs = _write_tex_and_get_pstrs(
             includes_tex, "includes", "include"
@@ -338,26 +338,26 @@
 
         ############################################################
 
         ## 5. Combine raw latex parts with user template.
 
         # Now, all the necessary parts are linked through the metadata.
         # So we can pass a dummy empty file to pandoc with the user template.
+        rescs_dir = self.tex_files_dir / "resources"
+        rescs_dir.mkdir(exist_ok=True)
         with self.template.load() as (
             template_path,
             static_resc_paths,
             dynamic_resc_paths,
         ):
             # Add static resources to metadata.
             for resc_name, resc_path in static_resc_paths.items():
                 if self.copy_statics:
                     # Copy the resource to the tex files dir if it is not already there.
-                    copy_resc_path = (
-                        self.tex_files_dir / f"_{resc_name}{resc_path.suffix}"
-                    )
+                    copy_resc_path = rescs_dir / f"{resc_name}{resc_path.suffix}"
                     if not copy_resc_path.exists():
                         print(f"+ cp '{resc_path}' '{copy_resc_path}'", file=sys.stderr)
                         shutil.copy(resc_path, copy_resc_path)
                     resc_path = copy_resc_path
                 metadata[resc_name] = str(resc_path.with_suffix(""))
 
             # Process dynamic resources with pandoc.
@@ -368,17 +368,15 @@
                     bib_path,
                     metadata_path,
                     self.default_img_ext,
                     self.natbib,
                     self.verbose,
                     **self.meta,
                 )
-                processed_resc_path = (
-                    self.tex_files_dir / f"_{resc_name}{resc_path.suffix}"
-                )
+                processed_resc_path = rescs_dir / f"{resc_name}{resc_path.suffix}"
                 print(f"+ write '{processed_resc_path}'", file=sys.stderr)
                 processed_resc_path.write_text(processed_resc_tex)
                 metadata[resc_name] = str(processed_resc_path.with_suffix(""))
 
             # Write updated metadata to file.
             print(f"+ write '{metadata_path}'", file=sys.stderr)
             metadata_path.write_text(yaml.dump(metadata))
```

### Comparing `shiny_mdc-1.1.0/shinymdc/templates/basic.tex` & `shiny_mdc-1.2.0/shinymdc/templates/basic.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/shinymdc/templates/iccv.tex` & `shiny_mdc-1.2.0/shinymdc/templates/iccv.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/shinymdc/templates/iclr.tex` & `shiny_mdc-1.2.0/shinymdc/templates/iclr.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/shinymdc/templates/icml.tex` & `shiny_mdc-1.2.0/shinymdc/templates/icml.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/shinymdc/templates/neurips.tex` & `shiny_mdc-1.2.0/shinymdc/templates/neurips.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/shinymdc/templates/spacious.tex` & `shiny_mdc-1.2.0/shinymdc/templates/spacious.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/shinymdc/templates/stylish.tex` & `shiny_mdc-1.2.0/shinymdc/templates/stylish.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/test/figures/anscombe.pdf` & `shiny_mdc-1.2.0/test/figures/anscombe.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/test/figures/densities.pdf` & `shiny_mdc-1.2.0/test/figures/densities.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/test/figures/diamonds.pdf` & `shiny_mdc-1.2.0/test/figures/diamonds.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/test/figures/gaussian2d.pdf` & `shiny_mdc-1.2.0/test/figures/gaussian2d.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/test/figures/lines.png` & `shiny_mdc-1.2.0/test/figures/lines.png`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/test/main.md` & `shiny_mdc-1.2.0/test/main.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/test/references.bib` & `shiny_mdc-1.2.0/test/references.bib`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/test/samples/basic.pdf` & `shiny_mdc-1.2.0/test/samples/basic.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 2% similar despite different names*

#### pdftotext {} -

```diff
@@ -169,15 +169,15 @@
 x + y + z = 100
 
 6
 
 Links
 • Section: Section 1, Section 1.2
 • Appendix section: Section B, Section A.1.1
-• Appendix figure: Figure A5
+• Appendix figure: Figure A1
 • Appendix table: Table B1
 • Appendix math: Equation 4
 • Short citation [2]
 • Long citation: Mittelbach et al. (2004) [2] , Lesk and Kernighan (1977) [3]
 • Multi citation [2–4]
 • Pointer to footnote1
 
@@ -428,16 +428,16 @@
 consequat maximus lorem faucibus in. Nam purus eros, rutrum in sapien et, condimentum
 lacinia nibh.
 
 A.2
 
 Appendix figures
 
-• Figure A5
-• Figure A6
+• Figure A1
+• Figure A2
 
 A.3
 
 Appendix includes
 
 • Commands from metadata include (argmin R):
 • Include command in body (there should be text after this):
@@ -475,15 +475,15 @@
 
 68
 
 x
 
 70
 
-Figure A5: Extra wide figure
+Figure A1: Extra wide figure
 
 9
 
 72
 
 74
 
@@ -532,15 +532,15 @@
 
 x
 
 15
 
 (c) Sub-figure
 
-Figure A6: Sub-figures with large combined size.
+Figure A2: Sub-figures with large combined size.
 
 10
 
 Col1
 
 Col2
```

### Comparing `shiny_mdc-1.1.0/test/samples/iccv.pdf` & `shiny_mdc-1.2.0/test/samples/iccv.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 3% similar despite different names*

#### pdftotext {} -

```diff
@@ -206,15 +206,15 @@
 x=1
 x + y = 10
 
 6. Links
 
 • Section: Section 1, Section 1.2
 • Appendix section: Section B, Section A.1.1
-• Appendix figure: Figure A5
+• Appendix figure: Figure A1
 • Appendix table: Table B1
 • Appendix math: Equation 4
 • Short citation[4]
 • Long citation: [4], [3]
 • Multi citation[1, 3, 4]
 • Pointer to footnote¹
 
@@ -410,15 +410,15 @@
 
 72
 
 74
 
 76
 
-Figure A5: Extra wide figure
+Figure A1: Extra wide figure
 
 Appendix A. Appendix 1
 Lorem ipsum dolor sit amet, consectetur adipiscing elit.
 Aliquam nisi purus, bibendum non neque sed, lacinia tristique
 tortor. Vestibulum eu lectus sed velit luctus varius. Sed
 sollicitudin ligula ante. Integer porta a erat commodo
 dignissim. Duis et lectus diam. Nulla id erat vestibulum nisi
@@ -434,17 +434,17 @@
 
 Proin eleifend lorem semper, commodo tellus nec, porta
 purus. Nullam commodo lectus nibh, consequat maximus
 lorem faucibus in. Nam purus eros, rutrum in sapien et,
 condimentum lacinia nibh.
 
 A.2. Appendix figures
-• Figure A5
+• Figure A1
 
-• Figure A6
+• Figure A2
 
 A.3. Appendix includes
 • Commands from metadata include (argmin R):
 • Include command in body (there should be text after
 this):
 Content added through include statement.
 
@@ -497,15 +497,15 @@
 
 10
 
 x
 
 (c) Sub-figure
 
-Figure A6: Sub-figures with large combined size.
+Figure A2: Sub-figures with large combined size.
 
 15
 
 Col1
 
 Col2
```

### Comparing `shiny_mdc-1.1.0/test/samples/iclr.pdf` & `shiny_mdc-1.2.0/test/samples/iclr.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 3% similar despite different names*

#### pdftotext {} -

```diff
@@ -95,18 +95,18 @@
 8
 6
 4
 5
 
 10
 
-x
-
 15
 
+x
+
 5
 
 10
 
 x
 
 15
@@ -164,15 +164,15 @@
 x + y + z = 100
 
 6
 
 Links
 • Section: Section 1, Section 1.2
 • Appendix section: Section B, Section A.1.1
-• Appendix figure: Figure A5
+• Appendix figure: Figure A1
 • Appendix table: Table B1
 • Appendix math: Equation 4
 • Short citation(Mittelbach et al., 2004)
 • Long citation: Mittelbach et al. (2004), Lesk & Kernighan (1977)
 • Multi citation(Lesk & Kernighan, 1977; Knuth, 1984; Mittelbach et al., 2004)
 • Pointer to footnote¹
 
@@ -423,15 +423,15 @@
 
 72
 
 74
 
 76
 
-Figure A5: Extra wide figure
+Figure A1: Extra wide figure
 
 Appendix A
 
 Appendix 1
 
 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam nisi purus, bibendum non neque
 sed, lacinia tristique tortor. Vestibulum eu lectus sed velit luctus varius. Sed sollicitudin ligula ante.
@@ -446,16 +446,16 @@
 
 Proin eleifend lorem semper, commodo tellus nec, porta purus. Nullam commodo lectus nibh,
 consequat maximus lorem faucibus in. Nam purus eros, rutrum in sapien et, condimentum lacinia
 nibh.
 A.2
 
 Appendix figures
-• Figure A5
-• Figure A6
+• Figure A1
+• Figure A2
 
 A.3
 
 Appendix includes
 • Commands from metadata include (argmin R):
 • Include command in body (there should be text after this):
 
@@ -503,15 +503,15 @@
 
 10
 
 x
 
 (c) Sub-figure
 
-Figure A6: Sub-figures with large combined size.
+Figure A2: Sub-figures with large combined size.
 
 8
 
 15
 
 A.4
```

### Comparing `shiny_mdc-1.1.0/test/samples/icml.pdf` & `shiny_mdc-1.2.0/test/samples/icml.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 6% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,10 +1,10 @@
 shinymdc-test
 
-Author1 * 1 Author2 * 1 2 Author3 * Author4
+Author One * 1 Author MiddleName Two * 1 2 Author * Author Four Author Number Five 2
 
 Abstract
 Markdown in abstract.
 Reference(Knuth, 1986).
 
 x + 2.
 
@@ -42,20 +42,17 @@
 placerat, fringilla augue at, pretium nisl.
 
 1.2. Subsection 2
 
 1.2.2. SUBSUBSECTION 2
 
 *
-Equal contribution 1 Institute1 2 Institute2. Correspondence
-to:
-Author1
-<author1@institute1.edu>,
-Author2
-<author2@institute1.edu>.
+Equal contribution 1 Institute One 2 Institute Two at City,
+State. Correspondence to: Author One <author1@institute1.edu>,
+Author MiddleName Two <authortwo@institute1.edu>.
 
 Proceedings of the 40 th International Conference on Machine
 Learning, Honolulu, Hawaii, USA. PMLR 202, 2023. Copyright
 2023 by the author(s).
 
 In ut nunc libero. Duis eu elementum purus. Etiam dictum,
 ipsum nec aliquam lobortis, magna magna pellentesque
@@ -199,15 +196,15 @@
 3. Numbers
 • Normal: 0123456789
 • Math: 0123456789
 
 6. Links
 • Section: Section 1, Section 1.2
 • Appendix section: Section B, Section A.1.1
-• Appendix figure: Figure A5
+• Appendix figure: Figure A1
 • Appendix table: Table B1
 • Appendix math: Equation 4
 • Short citation(Mittelbach et al., 2004)
 • Long citation: Mittelbach et al. (2004), Lesk &
 Kernighan (1977)
 • Multi citation(Lesk & Kernighan, 1977; Knuth, 1984;
 Mittelbach et al., 2004)
@@ -405,15 +402,15 @@
 
 72
 
 74
 
 76
 
-Figure A5. Extra wide figure
+Figure A1. Extra wide figure
 
 A. Appendix 1
 Lorem ipsum dolor sit amet, consectetur adipiscing elit.
 Aliquam nisi purus, bibendum non neque sed, lacinia
 tristique tortor. Vestibulum eu lectus sed velit luctus varius.
 Sed sollicitudin ligula ante. Integer porta a erat commodo
 dignissim. Duis et lectus diam. Nulla id erat vestibulum nisi
@@ -424,17 +421,17 @@
 A.1. Appendix subsection
 A.1.1. APPENDIX SUBSUBSECTION
 Proin eleifend lorem semper, commodo tellus nec, porta
 purus. Nullam commodo lectus nibh, consequat maximus
 lorem faucibus in. Nam purus eros, rutrum in sapien et,
 condimentum lacinia nibh.
 A.2. Appendix figures
-• Figure A5
+• Figure A1
 
-• Figure A6
+• Figure A2
 A.3. Appendix includes
 • Commands from metadata include (argmin R):
 • Include command in body (there should be text after
 this):
 Content added through include statement.
 A.4. Appendix links
 • Appendix section: Section A.1.1, Section B
@@ -485,15 +482,15 @@
 
 10
 
 x
 
 (c) Sub-figure
 
-Figure A6. Sub-figures with large combined size.
+Figure A2. Sub-figures with large combined size.
 
 15
 
 Col1
 
 Col2
```

### Comparing `shiny_mdc-1.1.0/test/samples/neurips.pdf` & `shiny_mdc-1.2.0/test/samples/neurips.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 5% similar despite different names*

#### pdftotext {} -

```diff
@@ -164,15 +164,15 @@
 x + y + z = 100
 
 6
 
 Links
 • Section: Section 1, Section 1.2
 • Appendix section: Section B, Section A.1.1
-• Appendix figure: Figure A5
+• Appendix figure: Figure A1
 • Appendix table: Table B1
 • Appendix math: Equation 4
 • Short citation[2]
 • Long citation: Mittelbach et al. (2004) [2], Lesk and Kernighan (1977) [3]
 • Multi citation[2–4]
 • Pointer to footnote1
 
@@ -421,15 +421,15 @@
 
 72
 
 74
 
 76
 
-Figure A5: Extra wide figure
+Figure A1: Extra wide figure
 
 Appendix A
 
 Appendix 1
 
 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam nisi purus, bibendum non neque
 sed, lacinia tristique tortor. Vestibulum eu lectus sed velit luctus varius. Sed sollicitudin ligula ante.
@@ -444,16 +444,16 @@
 
 Proin eleifend lorem semper, commodo tellus nec, porta purus. Nullam commodo lectus nibh,
 consequat maximus lorem faucibus in. Nam purus eros, rutrum in sapien et, condimentum lacinia
 nibh.
 A.2
 
 Appendix figures
-• Figure A5
-• Figure A6
+• Figure A1
+• Figure A2
 
 A.3
 
 Appendix includes
 • Commands from metadata include (argmin R):
 • Include command in body (there should be text after this):
 
@@ -505,15 +505,15 @@
 
 10
 
 x
 
 (c) Sub-figure
 
-Figure A6: Sub-figures with large combined size.
+Figure A2: Sub-figures with large combined size.
 
 9
 
 15
 
 • Main body section: Section 1
 • Main body figure: Figure 2
```

### Comparing `shiny_mdc-1.1.0/test/samples/spacious.pdf` & `shiny_mdc-1.2.0/test/samples/spacious.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 12% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,33 +1,36 @@
 shinymdc-test
-Author11,*
+Author One1,*
 author1@institute1.edu
 
-Author21,2,*
-author2@institute1.edu
+Author MiddleName Two1,2,*
+authortwo@institute1.edu
 
-Author3*
-Author4
+Author*
+Author Four
 author4@author4.com
 
+Author Number Five2
+authornumberfive@institutetwo.edu
+
 Abstract
 Markdown in abstract. x + 2. Section 1. Reference [1] .
 
 1. Section
 Integer at enim eu tellus malesuada scelerisque. Ut sed rhoncus ipsum,
 at tempor nisl. Vivamus vitae pulvinar leo, at pharetra massa. Ut
 lobortis odio non nulla tincidunt pulvinar. Nunc faucibus pellentesque
 elit, non ornare risus suscipit sed. Maecenas vel blandit ex.
 Phasellus ultrices mi non nulla hendrerit, at rhoncus augue
 suscipit. Pellentesque a lectus eget felis maximus feugiat nec ut ante.
 Sed eget laoreet lectus. Vestibulum iaculis enim nec libero sollicitudin,
 id rhoncus libero consectetur. Integer eget sem quis urna vulputate
 aliquet.
 
-* Equal contribution. 1 Institute1. 2 Institute2.
+* Equal contribution. 1 Institute One. 2 Institute Two at City, State.
 
 2
 dataset = I
 
 dataset = II
 
 dataset = III
@@ -144,15 +147,15 @@
 x=1
 x + y = 10
 x + y + z = 100
 
 6. Links
 • Section: Section 1, Section 1.2
 • Appendix section: Section B, Section A.1.1
-• Appendix figure: Figure A5
+• Appendix figure: Figure A1
 • Appendix table: Table B1
 • Appendix math: Equation 4
 • Short citation [2]
 • Long citation: Mittelbach et al. (2004) [2] , Lesk and Kernighan
 (1977) [3]
 • Multi citation [2–4]
 • Pointer to footnote1
@@ -379,16 +382,16 @@
 A.1 Appendix subsection
 A.1.1 Appendix subsubsection
 Proin eleifend lorem semper, commodo tellus nec, porta purus. Nullam
 commodo lectus nibh, consequat maximus lorem faucibus in. Nam
 purus eros, rutrum in sapien et, condimentum lacinia nibh.
 
 A.2 Appendix figures
-• Figure A5
-• Figure A6
+• Figure A1
+• Figure A2
 
 A.3 Appendix includes
 • Commands from metadata include (argmin R):
 • Include command in body (there should be text after this):
 Content added through include statement.
 
 A.4 Appendix links
@@ -422,15 +425,15 @@
 
 x
 
 70
 
 72
 
-Figure A5: Extra wide figure
+Figure A1: Extra wide figure
 
 74
 
 76
 
 11
 
@@ -478,15 +481,15 @@
 
 x
 
 15
 
 (c) Sub-figure
 
-Figure A6: Sub-figures with large combined size.
+Figure A2: Sub-figures with large combined size.
 
 12
 
 Col1 Col2
 
 Col3
```

### Comparing `shiny_mdc-1.1.0/test/samples/standalone.pdf` & `shiny_mdc-1.2.0/test/samples/standalone.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 5% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'547573'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'547573'*

 * *DEBUG:pdfminer.psparser:seek: 547573*

 * *DEBUG:pdfminer.psparser:nexttoken: (547573, 293)*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=547573, token=293*

 * *DEBUG:pdfminer.psparser:seek: 547573*

 * *DEBUG:pdfminer.psparser:nexttoken: (547573, 293)*

 * *DEBUG:pdfminer.psparser:nexttoken: (547577, 0)*

 * *DEBUG:pdfminer.psparser:nexttoken: (547579, /b'obj')*

 * *DEBUG:pdfminer.psparser:nexttoken: (547583, /b'<<')*

 * *DEBUG:pdfminer.psparser:start_type: pos=547583, type='d'*

 * *DEBUG:pdfminer.psparser:nexttoken: (547586, /'Type')*

 * *DEBUG:pdfminer.psparser:nexttoken: (547592, /'XRef')*

 * *DEBUG:pdfminer.psparser:nexttoken: (547598, /'Index')*

 * *DEBUG:pdfminer.psparser:nexttoken: (547605, /b'[')*

 * *DEBUG:pdfminer.psparser:start_type: pos=547605, type='a'*

 * *DEBUG:pdfminer.psparser:nexttoken: (547607, 0)*

 * *DEBUG:pdfminer.psparser:nexttoken: (547609, 294)*

 * *DEBUG:pdfminer.psparser:nexttoken: (547613, /b']')*

 * *DEBUG:pdfminer.psparser:end_type: pos=547605, type='a', objs=[0, 294]*

 * *DEBUG:pdfminer.psparser:nexttoken: (547615, /'Size')*

 * *[ truncated after 25 lines; 11923 ignored ]*

```diff
@@ -36,18 +36,18 @@
 <key>N</key>
 <value><number>100</number></value>
 <key>First</key>
 <value><number>825</number></value>
 <key>Filter</key>
 <value><literal>FlateDecode</literal></value>
 <key>Length</key>
-<value><number>2823</number></value>
+<value><number>2824</number></value>
 </dict>
 </props>
-<data size="11618">4 0 8 30 9 77 12 112 13 187 16 222 17 297 20 337 21 427 24 467&#10;25 557 28 587 29 649 32 679 33 726 36 756 37 808 40 838 41 870 44 900&#10;45 937 48 967 49 1009 52 1039 53 1086 56 1116 57 1168 58 1202 152 1322 153 1459&#10;154 1465 155 1483 156 1567 157 1573 160 1579 161 1597 162 1651 163 1735 164 1741 165 1747&#10;170 2171 171 2369 172 2600 191 3632 192 3638 193 3644 194 3770 195 3776 196 3782 197 3812&#10;198 3818 199 3902 200 3908 201 3914 202 4248 203 4610 204 4805 205 4921 206 5956 207 6154&#10;208 6255 62 7287 63 7427 64 7569 65 7707 66 7851 67 7999 68 8148 69 8291 70 8439&#10;71 8583 72 8720 73 8855 76 8990 77 9124 78 9258 79 9392 80 9535 82 9679 84 9818&#10;87 9954 88 9997 89 10038 6 10079 92 10120 93 10165 94 10211 95 10257 96 10303 10 10344&#10;97 10385 14 10426 98 10467 18 10508 100 10549 22 10590 101 10631 102 10672 103 10713 26 10754&#10;&#60;&#60; /S /GoTo /D &#40;section.1&#41; &#62;&#62;&#10;&#40;&#92;376&#92;377&#92;000S&#92;000e&#92;000c&#92;000t&#92;000i&#92;000o&#92;000n&#41;&#10;&#10;&#60;&#60; /S /GoTo /D &#40;subsection.1.1&#41; &#62;&#62;&#10;&#40;&#92;376&#92;377&#92;000S&#92;000u&#92;000b&#92;000s&#92;000e&#92;000c&#92;000t&#92;000i&#92;000o&#92;000n&#92;000&#92;040&#92;0001&#41;&#10;&#10;&#60;&#60; /S /GoTo /D &#40;subsection.1.2&#41; &#62;&#62;&#10;&#40;&#92;376&#92;377&#92;000S&#92;000u&#92;000b&#92;000s&#92;000e&#92;000c&#92;000t&#92;000i&#92;000o&#92;000n&#92;000&#92;040&#92;0002&#41;&#10;&#10;&#60;&#60; /S /GoTo /D &#40;subsubsection.1.2.1&#41; &#62;&#62;&#10;&#40;&#92;376&#92;377&#92;000S&#92;000u&#92;000b&#92;000s&#92;000u&#92;000b&#92;000s&#92;000e&#92;000c&#92;000t&#92;000i&#92;000o&#92;000n&#92;000&#92;040&#92;0001&#41;&#10;&#10;&#60;&#60; /S /GoTo /D &#40;subsubsection.1.2.2&#41; &#62;&#62;&#10;&#40;&#92;376&#92;377&#92;000S&#92;000u&#92;000b&#92;000s&#92;000u&#92;000b&#92;000s&#92;000e&#92;000c&#92;000t&#92;000i&#92;000o&#92;000n&#92;000&#92;040&#92;0002&#41;&#10;&#10;&#60;&#60; /S /GoTo /D &#40;section.2&#41; &#62;&#62;&#10;&#40;&#92;376&#92;377&#92;000T&#92;000y&#92;000p&#92;000o&#92;000g&#92;000r&#92;000a&#92;000p&#92;000h&#92;000y&#41;&#10;&#10;&#60;&#60; /S /GoTo /D &#40;section.3&#41; &#62;&#62;&#10;&#40;&#92;376&#92;377&#92;000N&#92;000u&#92;000m&#92;000b&#92;000e&#92;000r&#92;000s&#41;&#10;&#10;&#60;&#60; /S /GoTo /D &#40;section.4&#41; &#62;&#62;&#10;&#40;&#92;376&#92;377&#92;000A&#92;000c&#92;000r&#92;000o&#92;000n&#92;000y&#92;000m&#92;000s&#41;&#10;&#10;&#60;&#60; /S /GoTo /D &#40;section.5&#41; &#62;&#62;&#10;&#40;&#92;376&#92;377&#92;000M&#92;000a&#92;000t&#92;000h&#41;&#10;&#10;&#60;&#60; /S /GoTo /D &#40;section.6&#41; &#62;&#62;&#10;&#40;&#92;376&#92;377&#92;000L&#92;000i&#92;000n&#92;000k&#92;000s&#41;&#10;&#10;&#60;&#60; /S /GoTo /D &#40;section.7&#41; &#62;&#62;&#10;&#40;&#92;376&#92;377&#92;000T&#92;000a&#92;000b&#92;000l&#92;000e&#92;000s&#41;&#10;&#10;&#60;&#60; /S /GoTo /D &#40;section.8&#41; &#62;&#62;&#10;&#40;&#92;376&#92;377&#92;000F&#92;000i&#92;000g&#92;000u&#92;000r&#92;000e&#92;000s&#41;&#10;&#10;&#60;&#60; /S /GoTo /D &#40;section.9&#41; &#62;&#62;&#10;&#40;&#92;376&#92;377&#92;000I&#92;000n&#92;000c&#92;000l&#92;000u&#92;000d&#92;000e&#92;000s&#41;&#10;&#10;&#60;&#60; /S /GoTo /D [ 58 0 R /Fit ] &#62;&#62;&#10;&#60;&#60; /Type /Page /Contents 86 0 R /Resources 85 0 R /MediaBox [ 0 0 343.711 3178.815 ] /Parent 151 0 R /Annots 152 0 R &#62;&#62;&#10;[ 62 0 R 63 0 R 64 0 R 65 0 R 66 0 R 67 0 R 68 0 R 69 0 R 70 0 R 71 0 R 72 0 R 73 0 R 76 0 R 77 0 R 78 0 R 79 0 R 80 0 R 82 0 R 84 0 R ]&#10;&#60;&#60; &#62;&#62;&#10;&#60;&#60; /M0 158 0 R &#62;&#62;&#10;&#60;&#60; /A1 &#60;&#60; /Type /ExtGState /CA 0 /ca 1 &#62;&#62; /A2 &#60;&#60; /Type /ExtGState /CA 1 /ca 1 &#62;&#62; &#62;&#62;&#10;&#60;&#60; &#62;&#62;&#10;&#60;&#60; &#62;&#62;&#10;&#60;&#60; /F1 165 0 R &#62;&#62;&#10;&#60;&#60; /M0 166 0 R /M1 167 0 R /M2 168 0 R /M3 169 0 R &#62;&#62;&#10;&#60;&#60; /A1 &#60;&#60; /Type /ExtGState /CA 0 /ca 1 &#62;&#62; /A2 &#60;&#60; /Type /ExtGState /CA 1 /ca 1 &#62;&#62; &#62;&#62;&#10;&#60;&#60; &#62;&#62;&#10;&#60;&#60; &#62;&#62;&#10;&#60;&#60; /Type /Font /BaseFont /CLATDO+LMRoman10-Regular /FirstChar 0 /LastChar 255 /FontDescriptor 170 0 R /Subtype /Type3 /Name /CLATDO+LMRoman10-Regular /FontBBox [ -430 -290 1417 1127 ] /FontMatrix [ 0.001 0 0 0.001 0 0 ] /CharProcs 171 0 R /Encoding &#60;&#60; /Type /Encoding /Differences [ 32 /space 48 /zero /one /two 52 /four /five /six 56 /eight 61 /equal 73 /I 86 /V 97 /a 100 /d /e 115 /s /t 120 /x /y ] &#62;&#62; /Widths 172 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /CLATDO+LMRoman10-Regular /Flags 32 /FontBBox [ -430 -290 1417 1127 ] /Ascent 1127 /Descent -290 /CapHeight 0 /XHeight 0 /ItalicAngle 0 /StemV 0 /MaxWidth 1140 &#62;&#62;&#10;&#60;&#60; /I 173 0 R /V 174 0 R /a 175 0 R /d 176 0 R /e 177 0 R /eight 178 0 R /equal 179 0 R /five 180 0 R /four 181 0 R /one 182 0 R /s 183 0 R /six 184 0 R /space 185 0 R /t 186 0 R /two 187 0 R /x 188 0 R /y 189 0 R /zero 190 0 R &#62;&#62;&#10;[ 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 333 278 374 833 500 833 778 278 389 389 500 778 278 333 278 500 500 500 500 500 500 500 500 500 500 500 278 278 778 778 778 472 778 750 708 722 764 681 653 785 750 361 514 778 625 917 750 778 681 778 736 556 722 750 750 1028 750 750 611 278 500 278 556 750 500 500 556 444 556 444 306 500 556 278 306 528 278 833 556 500 556 528 392 394 389 556 528 722 528 528 444 500 278 500 556 280 627 280 278 306 472 670 444 444 500 1140 556 389 1014 280 611 280 280 278 278 472 472 778 500 1000 500 983 394 389 778 280 444 750 500 278 444 750 778 750 278 484 500 683 449 556 778 333 683 500 375 778 359 359 500 556 611 778 444 366 419 556 825 825 825 472 750 750 750 750 750 750 903 722 681 681 681 681 361 361 361 361 764 750 778 778 778 778 778 778 778 750 750 750 750 750 625 500 500 500 500 500 500 500 722 444 444 444 444 444 278 278 278 278 500 556 500 500 500 500 500 778 500 556 556 556 556 528 556 528 ]&#10;&#60;&#60; &#62;&#62;&#10;&#60;&#60; &#62;&#62;&#10;&#60;&#60; /A1 &#60;&#60; /Type /ExtGState /CA 0 /ca 1 &#62;&#62; /A2 &#60;&#60; /Type /ExtGState /CA 1 /ca 0.75 &#62;&#62; /A3 &#60;&#60; /Type /ExtGState /CA 1 /ca 1 &#62;&#62; &#62;&#62;&#10;&#60;&#60; &#62;&#62;&#10;&#60;&#60; &#62;&#62;&#10;&#60;&#60; /F1 201 0 R /F2 202 0 R &#62;&#62;&#10;&#60;&#60; &#62;&#62;&#10;&#60;&#60; /A1 &#60;&#60; /Type /ExtGState /CA 0 /ca 1 &#62;&#62; /A2 &#60;&#60; /Type /ExtGState /CA 1 /ca 1 &#62;&#62; &#62;&#62;&#10;&#60;&#60; &#62;&#62;&#10;&#60;&#60; &#62;&#62;&#10;&#60;&#60; /Type /Font /BaseFont /CLATDO+LMRoman10-Bold /FirstChar 0 /LastChar 255 /FontDescriptor 203 0 R /Subtype /Type3 /Name /CLATDO+LMRoman10-Bold /FontBBox [ -486 -295 1607 1133 ] /FontMatrix [ 0.001 0 0 0.001 0 0 ] /CharProcs 204 0 R /Encoding &#60;&#60; /Type /Encoding /Differences [ 65 /A /B /C /D /E /F /G /H /I /J ] &#62;&#62; /Widths 205 0 R &#62;&#62;&#10;&#60;&#60; /Type /Font /BaseFont /CLATDO+LMRoman10-Regular /FirstChar 0 /LastChar 255 /FontDescriptor 206 0 R /Subtype /Type3 /Name /CLATDO+LMRoman10-Regular /FontBBox [ -430 -290 1417 1127 ] /FontMatrix [ 0.001 0 0 0.001 0 0 ] /CharProcs 207 0 R /Encoding &#60;&#60; /Type /Encoding /Differences [ 48 /zero 50 /two 52 /four 54 /six /seven /eight 120 /x ] &#62;&#62; /Widths 208 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /CLATDO+LMRoman10-Bold /Flags 32 /FontBBox [ -486 -295 1607 1133 ] /Ascent 1133 /Descent -295 /CapHeight 0 /XHeight 0 /ItalicAngle 0 /StemV 0 /MaxWidth 1288 &#62;&#62;&#10;&#60;&#60; /A 209 0 R /B 210 0 R /C 211 0 R /D 212 0 R /E 213 0 R /F 214 0 R /G 215 0 R /H 216 0 R /I 217 0 R /J 218 0 R &#62;&#62;&#10;[ 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 383 350 481 958 575 958 894 319 447 447 575 894 319 383 319 575 575 575 575 575 575 575 575 575 575 575 319 319 894 894 894 543 894 869 818 831 882 756 724 904 900 436 594 901 692 1092 900 864 786 864 863 639 800 885 869 1189 869 869 703 319 575 319 556 869 575 559 639 511 639 527 351 575 639 319 351 607 319 958 639 575 639 607 474 454 447 639 607 831 607 607 511 575 319 575 556 280 720 280 319 351 571 838 511 511 575 1288 639 445 1169 280 703 280 280 319 319 571 571 894 575 1150 575 1135 454 445 894 280 511 869 575 350 511 869 894 869 319 695 575 686 496 639 894 383 686 575 431 894 413 413 575 639 703 894 511 417 482 639 983 983 983 543 869 869 869 869 869 869 1042 831 756 756 756 756 436 436 436 436 882 900 864 864 864 864 864 894 894 885 885 885 885 869 724 597 559 559 559 559 559 559 831 511 527 527 527 527 319 319 319 319 575 639 575 575 575 575 575 894 575 639 639 639 639 607 639 607 ]&#10;&#60;&#60; /Type /FontDescriptor /FontName /CLATDO+LMRoman10-Regular /Flags 32 /FontBBox [ -430 -290 1417 1127 ] /Ascent 1127 /Descent -290 /CapHeight 0 /XHeight 0 /ItalicAngle 0 /StemV 0 /MaxWidth 1140 &#62;&#62;&#10;&#60;&#60; /eight 219 0 R /four 220 0 R /seven 221 0 R /six 222 0 R /two 223 0 R /x 224 0 R /zero 225 0 R &#62;&#62;&#10;[ 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 333 278 374 833 500 833 778 278 389 389 500 778 278 333 278 500 500 500 500 500 500 500 500 500 500 500 278 278 778 778 778 472 778 750 708 722 764 681 653 785 750 361 514 778 625 917 750 778 681 778 736 556 722 750 750 1028 750 750 611 278 500 278 556 750 500 500 556 444 556 444 306 500 556 278 306 528 278 833 556 500 556 528 392 394 389 556 528 722 528 528 444 500 278 500 556 280 627 280 278 306 472 670 444 444 500 1140 556 389 1014 280 611 280 280 278 278 472 472 778 500 1000 500 983 394 389 778 280 444 750 500 278 444 750 778 750 278 484 500 683 449 556 778 333 683 500 375 778 359 359 500 556 611 778 444 366 419 556 825 825 825 472 750 750 750 750 750 750 903 722 681 681 681 681 361 361 361 361 764 750 778 778 778 778 778 778 778 750 750 750 750 750 625 500 500 500 500 500 500 500 722 444 444 444 444 444 278 278 278 278 500 556 500 500 500 500 500 778 500 556 556 556 556 528 556 528 ]&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[1 0 0] /Rect [ 98.63 1955.011 105.604 1965.803 ]/A  &#60;&#60; /S /GoTo /D &#40;equation.5.1&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[1 0 0] /Rect [ 152.733 1955.011 159.707 1965.803 ]/A  &#60;&#60; /S /GoTo /D &#40;equation.5.2&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[1 0 0] /Rect [ 97.523 1818.705 104.497 1829.497 ]/A  &#60;&#60; /S /GoTo /D &#40;section.1&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[1 0 0] /Rect [ 143.462 1818.705 158.185 1829.497 ]/A  &#60;&#60; /S /GoTo /D &#40;subsection.1.2&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[0 1 0] /Rect [ 87.519 1764.481 93.483 1770.865 ]/A  &#60;&#60; /S /GoTo /D &#40;cite.latex:companion&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[0 1 0] /Rect [ 197.109 1752.526 203.073 1758.91 ]/A  &#60;&#60; /S /GoTo /D &#40;cite.latex:companion&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[0 1 0] /Rect [ 333.114 1752.526 339.077 1758.91 ]/A  &#60;&#60; /S /GoTo /D &#40;cite.lesk:1977&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[0 1 0] /Rect [ 87.769 1740.571 93.732 1746.955 ]/A  &#60;&#60; /S /GoTo /D &#40;cite.latex:companion&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[0 1 0] /Rect [ 95.711 1740.571 101.675 1746.955 ]/A  &#60;&#60; /S /GoTo /D &#40;cite.knuth:1984&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[1 0 0] /Rect [ 107.099 1725 113.796 1733.856 ]/A  &#60;&#60; /S /GoTo /D &#40;Hfootnote.1&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[1 0 0] /Rect [ 50.949 1670.234 57.923 1679.089 ]/A  &#60;&#60; /S /GoTo /D &#40;table.1&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[1 0 0] /Rect [ 50.949 1658.279 57.923 1667.134 ]/A  &#60;&#60; /S /GoTo /D &#40;table.2&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[1 0 0] /Rect [ 55.348 846.212 62.322 857.004 ]/A  &#60;&#60; /S /GoTo /D &#40;figure.2&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[1 0 0] /Rect [ 55.348 834.256 62.322 845.049 ]/A  &#60;&#60; /S /GoTo /D &#40;figure.3&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[1 0 0] /Rect [ 55.348 822.301 62.322 833.094 ]/A  &#60;&#60; /S /GoTo /D &#40;figure.4&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[1 0 0] /Rect [ 97.856 822.301 109.811 833.094 ]/A  &#60;&#60; /S /GoTo /D &#40;figure.caption.8&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[1 0 0] /Rect [ 145.344 822.301 157.853 833.094 ]/A  &#60;&#60; /S /GoTo /D &#40;figure.caption.9&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[1 0 0] /Rect [ 169.282 331.459 175.979 345.406 ]/A  &#60;&#60; /S /GoTo /D &#40;Hfootnote.3&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[1 0 0] /Rect [ 90.854 301.52 97.141 315.518 ]/A  &#60;&#60; /S /GoTo /D &#40;Hfootnote.5&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ -73 3251.815 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 3178.815 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 3177.818 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 3177.818 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 22.867 3052.54 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 176.837 3052.54 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 98.195 2885.619 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 43.614 2699.378 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 2673.873 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 2669.895 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 2591.387 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 2577.446 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 2559.002 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 2559.002 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 2490.855 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 2476.914 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 2400.686 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 2386.746 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 2348.943 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 2333.93 null ] &#62;&#62;</data>
+<data size="11618">4 0 8 30 9 77 12 112 13 187 16 222 17 297 20 337 21 427 24 467&#10;25 557 28 587 29 649 32 679 33 726 36 756 37 808 40 838 41 870 44 900&#10;45 937 48 967 49 1009 52 1039 53 1086 56 1116 57 1168 58 1202 152 1322 153 1459&#10;154 1465 155 1483 156 1567 157 1573 160 1579 161 1597 162 1651 163 1735 164 1741 165 1747&#10;170 2171 171 2369 172 2600 191 3632 192 3638 193 3644 194 3770 195 3776 196 3782 197 3812&#10;198 3818 199 3902 200 3908 201 3914 202 4248 203 4610 204 4805 205 4921 206 5956 207 6154&#10;208 6255 62 7287 63 7427 64 7569 65 7707 66 7851 67 7999 68 8148 69 8291 70 8439&#10;71 8583 72 8720 73 8855 76 8990 77 9124 78 9258 79 9392 80 9535 82 9679 84 9818&#10;87 9954 88 9997 89 10038 6 10079 92 10120 93 10165 94 10211 95 10257 96 10303 10 10344&#10;97 10385 14 10426 98 10467 18 10508 100 10549 22 10590 101 10631 102 10672 103 10713 26 10754&#10;&#60;&#60; /S /GoTo /D &#40;section.1&#41; &#62;&#62;&#10;&#40;&#92;376&#92;377&#92;000S&#92;000e&#92;000c&#92;000t&#92;000i&#92;000o&#92;000n&#41;&#10;&#10;&#60;&#60; /S /GoTo /D &#40;subsection.1.1&#41; &#62;&#62;&#10;&#40;&#92;376&#92;377&#92;000S&#92;000u&#92;000b&#92;000s&#92;000e&#92;000c&#92;000t&#92;000i&#92;000o&#92;000n&#92;000&#92;040&#92;0001&#41;&#10;&#10;&#60;&#60; /S /GoTo /D &#40;subsection.1.2&#41; &#62;&#62;&#10;&#40;&#92;376&#92;377&#92;000S&#92;000u&#92;000b&#92;000s&#92;000e&#92;000c&#92;000t&#92;000i&#92;000o&#92;000n&#92;000&#92;040&#92;0002&#41;&#10;&#10;&#60;&#60; /S /GoTo /D &#40;subsubsection.1.2.1&#41; &#62;&#62;&#10;&#40;&#92;376&#92;377&#92;000S&#92;000u&#92;000b&#92;000s&#92;000u&#92;000b&#92;000s&#92;000e&#92;000c&#92;000t&#92;000i&#92;000o&#92;000n&#92;000&#92;040&#92;0001&#41;&#10;&#10;&#60;&#60; /S /GoTo /D &#40;subsubsection.1.2.2&#41; &#62;&#62;&#10;&#40;&#92;376&#92;377&#92;000S&#92;000u&#92;000b&#92;000s&#92;000u&#92;000b&#92;000s&#92;000e&#92;000c&#92;000t&#92;000i&#92;000o&#92;000n&#92;000&#92;040&#92;0002&#41;&#10;&#10;&#60;&#60; /S /GoTo /D &#40;section.2&#41; &#62;&#62;&#10;&#40;&#92;376&#92;377&#92;000T&#92;000y&#92;000p&#92;000o&#92;000g&#92;000r&#92;000a&#92;000p&#92;000h&#92;000y&#41;&#10;&#10;&#60;&#60; /S /GoTo /D &#40;section.3&#41; &#62;&#62;&#10;&#40;&#92;376&#92;377&#92;000N&#92;000u&#92;000m&#92;000b&#92;000e&#92;000r&#92;000s&#41;&#10;&#10;&#60;&#60; /S /GoTo /D &#40;section.4&#41; &#62;&#62;&#10;&#40;&#92;376&#92;377&#92;000A&#92;000c&#92;000r&#92;000o&#92;000n&#92;000y&#92;000m&#92;000s&#41;&#10;&#10;&#60;&#60; /S /GoTo /D &#40;section.5&#41; &#62;&#62;&#10;&#40;&#92;376&#92;377&#92;000M&#92;000a&#92;000t&#92;000h&#41;&#10;&#10;&#60;&#60; /S /GoTo /D &#40;section.6&#41; &#62;&#62;&#10;&#40;&#92;376&#92;377&#92;000L&#92;000i&#92;000n&#92;000k&#92;000s&#41;&#10;&#10;&#60;&#60; /S /GoTo /D &#40;section.7&#41; &#62;&#62;&#10;&#40;&#92;376&#92;377&#92;000T&#92;000a&#92;000b&#92;000l&#92;000e&#92;000s&#41;&#10;&#10;&#60;&#60; /S /GoTo /D &#40;section.8&#41; &#62;&#62;&#10;&#40;&#92;376&#92;377&#92;000F&#92;000i&#92;000g&#92;000u&#92;000r&#92;000e&#92;000s&#41;&#10;&#10;&#60;&#60; /S /GoTo /D &#40;section.9&#41; &#62;&#62;&#10;&#40;&#92;376&#92;377&#92;000I&#92;000n&#92;000c&#92;000l&#92;000u&#92;000d&#92;000e&#92;000s&#41;&#10;&#10;&#60;&#60; /S /GoTo /D [ 58 0 R /Fit ] &#62;&#62;&#10;&#60;&#60; /Type /Page /Contents 86 0 R /Resources 85 0 R /MediaBox [ 0 0 343.711 3178.815 ] /Parent 151 0 R /Annots 152 0 R &#62;&#62;&#10;[ 62 0 R 63 0 R 64 0 R 65 0 R 66 0 R 67 0 R 68 0 R 69 0 R 70 0 R 71 0 R 72 0 R 73 0 R 76 0 R 77 0 R 78 0 R 79 0 R 80 0 R 82 0 R 84 0 R ]&#10;&#60;&#60; &#62;&#62;&#10;&#60;&#60; /M0 158 0 R &#62;&#62;&#10;&#60;&#60; /A1 &#60;&#60; /Type /ExtGState /CA 0 /ca 1 &#62;&#62; /A2 &#60;&#60; /Type /ExtGState /CA 1 /ca 1 &#62;&#62; &#62;&#62;&#10;&#60;&#60; &#62;&#62;&#10;&#60;&#60; &#62;&#62;&#10;&#60;&#60; /F1 165 0 R &#62;&#62;&#10;&#60;&#60; /M0 166 0 R /M1 167 0 R /M2 168 0 R /M3 169 0 R &#62;&#62;&#10;&#60;&#60; /A1 &#60;&#60; /Type /ExtGState /CA 0 /ca 1 &#62;&#62; /A2 &#60;&#60; /Type /ExtGState /CA 1 /ca 1 &#62;&#62; &#62;&#62;&#10;&#60;&#60; &#62;&#62;&#10;&#60;&#60; &#62;&#62;&#10;&#60;&#60; /Type /Font /BaseFont /CLATDO+LMRoman10-Regular /FirstChar 0 /LastChar 255 /FontDescriptor 170 0 R /Subtype /Type3 /Name /CLATDO+LMRoman10-Regular /FontBBox [ -430 -290 1417 1127 ] /FontMatrix [ 0.001 0 0 0.001 0 0 ] /CharProcs 171 0 R /Encoding &#60;&#60; /Type /Encoding /Differences [ 32 /space 48 /zero /one /two 52 /four /five /six 56 /eight 61 /equal 73 /I 86 /V 97 /a 100 /d /e 115 /s /t 120 /x /y ] &#62;&#62; /Widths 172 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /CLATDO+LMRoman10-Regular /Flags 32 /FontBBox [ -430 -290 1417 1127 ] /Ascent 1127 /Descent -290 /CapHeight 0 /XHeight 0 /ItalicAngle 0 /StemV 0 /MaxWidth 1140 &#62;&#62;&#10;&#60;&#60; /I 173 0 R /V 174 0 R /a 175 0 R /d 176 0 R /e 177 0 R /eight 178 0 R /equal 179 0 R /five 180 0 R /four 181 0 R /one 182 0 R /s 183 0 R /six 184 0 R /space 185 0 R /t 186 0 R /two 187 0 R /x 188 0 R /y 189 0 R /zero 190 0 R &#62;&#62;&#10;[ 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 333 278 374 833 500 833 778 278 389 389 500 778 278 333 278 500 500 500 500 500 500 500 500 500 500 500 278 278 778 778 778 472 778 750 708 722 764 681 653 785 750 361 514 778 625 917 750 778 681 778 736 556 722 750 750 1028 750 750 611 278 500 278 556 750 500 500 556 444 556 444 306 500 556 278 306 528 278 833 556 500 556 528 392 394 389 556 528 722 528 528 444 500 278 500 556 280 627 280 278 306 472 670 444 444 500 1140 556 389 1014 280 611 280 280 278 278 472 472 778 500 1000 500 983 394 389 778 280 444 750 500 278 444 750 778 750 278 484 500 683 449 556 778 333 683 500 375 778 359 359 500 556 611 778 444 366 419 556 825 825 825 472 750 750 750 750 750 750 903 722 681 681 681 681 361 361 361 361 764 750 778 778 778 778 778 778 778 750 750 750 750 750 625 500 500 500 500 500 500 500 722 444 444 444 444 444 278 278 278 278 500 556 500 500 500 500 500 778 500 556 556 556 556 528 556 528 ]&#10;&#60;&#60; &#62;&#62;&#10;&#60;&#60; &#62;&#62;&#10;&#60;&#60; /A1 &#60;&#60; /Type /ExtGState /CA 0 /ca 1 &#62;&#62; /A2 &#60;&#60; /Type /ExtGState /CA 1 /ca 0.75 &#62;&#62; /A3 &#60;&#60; /Type /ExtGState /CA 1 /ca 1 &#62;&#62; &#62;&#62;&#10;&#60;&#60; &#62;&#62;&#10;&#60;&#60; &#62;&#62;&#10;&#60;&#60; /F1 201 0 R /F2 202 0 R &#62;&#62;&#10;&#60;&#60; &#62;&#62;&#10;&#60;&#60; /A1 &#60;&#60; /Type /ExtGState /CA 0 /ca 1 &#62;&#62; /A2 &#60;&#60; /Type /ExtGState /CA 1 /ca 1 &#62;&#62; &#62;&#62;&#10;&#60;&#60; &#62;&#62;&#10;&#60;&#60; &#62;&#62;&#10;&#60;&#60; /Type /Font /BaseFont /CLATDO+LMRoman10-Bold /FirstChar 0 /LastChar 255 /FontDescriptor 203 0 R /Subtype /Type3 /Name /CLATDO+LMRoman10-Bold /FontBBox [ -486 -295 1607 1133 ] /FontMatrix [ 0.001 0 0 0.001 0 0 ] /CharProcs 204 0 R /Encoding &#60;&#60; /Type /Encoding /Differences [ 65 /A /B /C /D /E /F /G /H /I /J ] &#62;&#62; /Widths 205 0 R &#62;&#62;&#10;&#60;&#60; /Type /Font /BaseFont /CLATDO+LMRoman10-Regular /FirstChar 0 /LastChar 255 /FontDescriptor 206 0 R /Subtype /Type3 /Name /CLATDO+LMRoman10-Regular /FontBBox [ -430 -290 1417 1127 ] /FontMatrix [ 0.001 0 0 0.001 0 0 ] /CharProcs 207 0 R /Encoding &#60;&#60; /Type /Encoding /Differences [ 48 /zero 50 /two 52 /four 54 /six /seven /eight 120 /x ] &#62;&#62; /Widths 208 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /CLATDO+LMRoman10-Bold /Flags 32 /FontBBox [ -486 -295 1607 1133 ] /Ascent 1133 /Descent -295 /CapHeight 0 /XHeight 0 /ItalicAngle 0 /StemV 0 /MaxWidth 1288 &#62;&#62;&#10;&#60;&#60; /A 209 0 R /B 210 0 R /C 211 0 R /D 212 0 R /E 213 0 R /F 214 0 R /G 215 0 R /H 216 0 R /I 217 0 R /J 218 0 R &#62;&#62;&#10;[ 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 383 350 481 958 575 958 894 319 447 447 575 894 319 383 319 575 575 575 575 575 575 575 575 575 575 575 319 319 894 894 894 543 894 869 818 831 882 756 724 904 900 436 594 901 692 1092 900 864 786 864 863 639 800 885 869 1189 869 869 703 319 575 319 556 869 575 559 639 511 639 527 351 575 639 319 351 607 319 958 639 575 639 607 474 454 447 639 607 831 607 607 511 575 319 575 556 280 720 280 319 351 571 838 511 511 575 1288 639 445 1169 280 703 280 280 319 319 571 571 894 575 1150 575 1135 454 445 894 280 511 869 575 350 511 869 894 869 319 695 575 686 496 639 894 383 686 575 431 894 413 413 575 639 703 894 511 417 482 639 983 983 983 543 869 869 869 869 869 869 1042 831 756 756 756 756 436 436 436 436 882 900 864 864 864 864 864 894 894 885 885 885 885 869 724 597 559 559 559 559 559 559 831 511 527 527 527 527 319 319 319 319 575 639 575 575 575 575 575 894 575 639 639 639 639 607 639 607 ]&#10;&#60;&#60; /Type /FontDescriptor /FontName /CLATDO+LMRoman10-Regular /Flags 32 /FontBBox [ -430 -290 1417 1127 ] /Ascent 1127 /Descent -290 /CapHeight 0 /XHeight 0 /ItalicAngle 0 /StemV 0 /MaxWidth 1140 &#62;&#62;&#10;&#60;&#60; /eight 219 0 R /four 220 0 R /seven 221 0 R /six 222 0 R /two 223 0 R /x 224 0 R /zero 225 0 R &#62;&#62;&#10;[ 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 280 333 278 374 833 500 833 778 278 389 389 500 778 278 333 278 500 500 500 500 500 500 500 500 500 500 500 278 278 778 778 778 472 778 750 708 722 764 681 653 785 750 361 514 778 625 917 750 778 681 778 736 556 722 750 750 1028 750 750 611 278 500 278 556 750 500 500 556 444 556 444 306 500 556 278 306 528 278 833 556 500 556 528 392 394 389 556 528 722 528 528 444 500 278 500 556 280 627 280 278 306 472 670 444 444 500 1140 556 389 1014 280 611 280 280 278 278 472 472 778 500 1000 500 983 394 389 778 280 444 750 500 278 444 750 778 750 278 484 500 683 449 556 778 333 683 500 375 778 359 359 500 556 611 778 444 366 419 556 825 825 825 472 750 750 750 750 750 750 903 722 681 681 681 681 361 361 361 361 764 750 778 778 778 778 778 778 778 750 750 750 750 750 625 500 500 500 500 500 500 500 722 444 444 444 444 444 278 278 278 278 500 556 500 500 500 500 500 778 500 556 556 556 556 528 556 528 ]&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[1 0 0] /Rect [ 98.63 1955.011 105.604 1965.803 ]/A  &#60;&#60; /S /GoTo /D &#40;equation.5.1&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[1 0 0] /Rect [ 152.733 1955.011 159.707 1965.803 ]/A  &#60;&#60; /S /GoTo /D &#40;equation.5.2&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[1 0 0] /Rect [ 97.523 1818.705 104.497 1829.497 ]/A  &#60;&#60; /S /GoTo /D &#40;section.1&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[1 0 0] /Rect [ 143.462 1818.705 158.185 1829.497 ]/A  &#60;&#60; /S /GoTo /D &#40;subsection.1.2&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[0 1 0] /Rect [ 87.519 1764.481 93.483 1770.865 ]/A  &#60;&#60; /S /GoTo /D &#40;cite.latex:companion&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[0 1 0] /Rect [ 197.109 1752.526 203.073 1758.91 ]/A  &#60;&#60; /S /GoTo /D &#40;cite.latex:companion&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[0 1 0] /Rect [ 333.114 1752.526 339.077 1758.91 ]/A  &#60;&#60; /S /GoTo /D &#40;cite.lesk:1977&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[0 1 0] /Rect [ 87.769 1740.571 93.732 1746.955 ]/A  &#60;&#60; /S /GoTo /D &#40;cite.latex:companion&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[0 1 0] /Rect [ 95.711 1740.571 101.675 1746.955 ]/A  &#60;&#60; /S /GoTo /D &#40;cite.knuth:1984&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[1 0 0] /Rect [ 107.099 1725 113.796 1733.856 ]/A  &#60;&#60; /S /GoTo /D &#40;Hfootnote.1&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[1 0 0] /Rect [ 50.949 1670.234 57.923 1679.089 ]/A  &#60;&#60; /S /GoTo /D &#40;table.1&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[1 0 0] /Rect [ 50.949 1658.279 57.923 1667.134 ]/A  &#60;&#60; /S /GoTo /D &#40;table.2&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[1 0 0] /Rect [ 55.348 846.212 62.322 857.004 ]/A  &#60;&#60; /S /GoTo /D &#40;figure.2&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[1 0 0] /Rect [ 55.348 834.256 62.322 845.049 ]/A  &#60;&#60; /S /GoTo /D &#40;figure.3&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[1 0 0] /Rect [ 55.348 822.301 62.322 833.094 ]/A  &#60;&#60; /S /GoTo /D &#40;figure.4&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[1 0 0] /Rect [ 97.856 822.301 109.811 833.094 ]/A  &#60;&#60; /S /GoTo /D &#40;figure.caption.8&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[1 0 0] /Rect [ 145.344 822.301 157.853 833.094 ]/A  &#60;&#60; /S /GoTo /D &#40;figure.caption.9&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[1 0 0] /Rect [ 167.621 331.459 174.318 345.406 ]/A  &#60;&#60; /S /GoTo /D &#40;Hfootnote.3&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /Type /Annot /Subtype /Link /Border[0 0 0]/H/I/C[1 0 0] /Rect [ 90.854 301.52 97.141 315.518 ]/A  &#60;&#60; /S /GoTo /D &#40;Hfootnote.5&#41; &#62;&#62; &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ -73 3251.815 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 3178.815 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 3177.818 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 3177.818 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 21.206 3052.54 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 178.497 3052.54 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 96.535 2885.619 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 43.614 2699.378 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 2673.873 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 2669.895 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 2591.387 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 2577.446 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 2559.002 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 2559.002 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 2490.855 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 2476.914 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 2400.686 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 2386.746 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 2348.943 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 2333.93 null ] &#62;&#62;</data>
 </stream>
 </object>
 
 <object id="6">
 <dict size="1">
 <key>D</key>
 <value><list size="5">
@@ -1516,17 +1516,17 @@
 <value><list size="3">
 <number>1</number>
 <number>0</number>
 <number>0</number>
 </list></value>
 <key>Rect</key>
 <value><list size="4">
-<number>169.282</number>
+<number>167.621</number>
 <number>331.459</number>
-<number>175.979</number>
+<number>174.318</number>
 <number>345.406</number>
 </list></value>
 <key>A</key>
 <value><dict size="2">
 <key>S</key>
 <value><literal>GoTo</literal></value>
 <key>D</key>
@@ -1646,18 +1646,18 @@
 <object id="86">
 <stream>
 <props>
 <dict size="2">
 <key>Filter</key>
 <value><literal>FlateDecode</literal></value>
 <key>Length</key>
-<value><number>5684</number></value>
+<value><number>5686</number></value>
 </dict>
 </props>
-<data size="21306">0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;BT&#10;/F18 14.3462 Tf&#10;1 0 0 1 -0.807 3168.01 Tm [&#40;1&#41;-1125&#40;Section&#41;]TJ&#10;/F16 9.96264 Tf&#10;0.98 0 0 1 0 3146.189 Tm [&#40;In&#41;28&#40;tege&#41;1&#40;r&#41;-280&#40;at&#41;-281&#40;enim&#41;-281&#40;eu&#41;-281&#40;tellus&#41;-281&#40;malesuada&#41;-281&#40;scelerisque.&#41;-434&#40;Ut&#41;-281&#40;sed&#41;-281&#40;rhoncus&#41;-281&#40;ipsum,&#41;-292&#40;at&#41;-281&#40;temp&#41;-29&#40;or&#41;]TJ&#10;0.996 0 0 1 0 3134.234 Tm [&#40;nisl.&#41;-446&#40;Viv&#41;56&#40;am&#41;29&#40;us&#41;-334&#40;vitae&#41;-335&#40;pulvinar&#41;-335&#40;leo,&#41;-334&#40;at&#41;-335&#40;pharetra&#41;-335&#40;massa.&#41;-446&#40;Ut&#41;-335&#40;lob&#41;-28&#40;ortis&#41;-335&#40;o&#41;-29&#40;dio&#41;-334&#40;non&#41;-335&#40;n&#41;27&#40;ulla&#41;]TJ&#10;0.98 0 0 1 0 3122.279 Tm [&#40;tincidun&#41;28&#40;t&#41;-312&#40;pulvinar.&#41;-445&#40;Nunc&#41;-313&#40;faucibus&#41;-314&#40;p&#41;-28&#40;ellen&#41;28&#40;tesque&#41;-313&#40;elit,&#41;-318&#40;non&#41;-314&#40;ornare&#41;-313&#40;risus&#41;-313&#40;su&#41;-1&#40;scipit&#41;-313&#40;sed.&#41;]TJ&#10;1 0 0 1 0 3110.323 Tm [&#40;Maecenas&#41;-333&#40;v&#41;27&#40;el&#41;-332&#40;blandit&#41;-334&#40;ex.&#41;]TJ&#10;0.98 0 0 1 0 3098.368 Tm [&#40;Phasellus&#41;-286&#40;ultrices&#41;-285&#40;mi&#41;-286&#40;non&#41;-286&#40;n&#41;28&#40;ulla&#41;-285&#40;hendrerit,&#41;-297&#40;at&#41;-285&#40;rhoncus&#41;-286&#40;augue&#41;-286&#40;suscipit.&#41;-436&#40;P&#41;28&#40;elle&#41;1&#40;n&#41;28&#40;tesque&#41;]TJ&#10;1.02 0 0 1 0 3086.413 Tm [&#40;a&#41;-544&#40;lectus&#41;-544&#40;eget&#41;-544&#40;felis&#41;-544&#40;maxim&#41;27&#40;us&#41;-543&#40;feugiat&#41;-544&#40;nec&#41;-544&#40;ut&#41;-544&#40;an&#41;27&#40;te.&#41;-1087&#40;Sed&#41;-544&#40;eget&#41;-544&#40;laoreet&#41;-544&#40;lectus.&#41;]TJ&#10;1.02 0 0 1 -0.379 3074.458 Tm [&#40;V&#41;83&#40;estibulum&#41;-370&#40;iaculis&#41;-370&#40;enim&#41;-371&#40;nec&#41;-370&#40;lib&#41;-28&#40;ero&#41;-370&#40;s&#41;-1&#40;ollicitudin,&#41;-381&#40;id&#41;-370&#40;rhon&#41;-1&#40;cus&#41;-370&#40;lib&#41;-28&#40;ero&#41;-370&#40;consectetur.&#41;]TJ&#10;1 0 0 1 0 3062.503 Tm [&#40;In&#41;27&#40;teger&#41;-332&#40;eget&#41;-333&#40;sem&#41;-334&#40;quis&#41;-333&#40;urna&#41;-333&#40;vulpu&#41;-1&#40;tate&#41;-333&#40;aliquet.&#41;]TJ&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;ET&#10;1 0 0 1 22.867 2902.555 cm&#10;q&#10;.6667 0 0 .6667 0 0 cm&#10;0 g 0 G&#10;q&#10;1 0 0 1 0 0 cm&#10;/Im1 Do&#10;Q&#10;0 g 0 G&#10;Q&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;1 0 0 1 -22.867 -2902.555 cm&#10;BT&#10;/F16 9.96264 Tf&#10;1 0 0 1 22.867 2884.224 Tm [&#40;a:&#41;-444&#40;Sub-&#92;034gure&#41;-333&#40;with&#41;-334&#40;`width=2in&#39;&#41;]TJ&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;ET&#10;1 0 0 1 176.837 2902.555 cm&#10;q&#10;.6667 0 0 .6667 0 0 cm&#10;0 g 0 G&#10;q&#10;216 0 0 216 0 0 cm&#10;/Im2 Do&#10;Q&#10;0 g 0 G&#10;Q&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;1 0 0 1 -176.837 -2902.555 cm&#10;BT&#10;/F16 9.96264 Tf&#10;1 0 0 1 176.837 2884.224 Tm [&#40;b:&#41;-444&#40;Sub-&#92;034gure&#41;-334&#40;with&#41;-333&#40;`width=2in&#39;&#41;]TJ&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;ET&#10;1 0 0 1 98.195 2735.642 cm&#10;q&#10;.5 0 0 .5 0 0 cm&#10;0 g 0 G&#10;q&#10;1 0 0 1 0 0 cm&#10;/Im3 Do&#10;Q&#10;0 g 0 G&#10;Q&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;1 0 0 1 -98.195 -2735.642 cm&#10;BT&#10;/F16 9.96264 Tf&#10;1 0 0 1 98.195 2717.31 Tm [&#40;c:&#41;-444&#40;Sub-&#92;034gure&#41;-333&#40;with&#41;-334&#40;`width=2in&#39;&#41;]TJ&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;1 0 0 1 0 2687.422 Tm [&#40;Figure&#41;-333&#40;1:&#41;-444&#40;Sub-&#92;034gu&#41;-1&#40;res&#41;]TJ&#10;0 g 0 G&#10;/F18 11.95517 Tf&#10;1 0 0 1 -0.672 2659.534 Tm [&#40;1.1&#41;-1125&#40;Subsection&#41;-375&#40;1&#41;]TJ&#10;/F16 9.96264 Tf&#10;0.987 0 0 1 0 2641.145 Tm [&#40;In&#41;-338&#40;mollis&#41;-338&#40;tortor&#41;-338&#40;v&#41;28&#40;el&#41;-337&#40;an&#41;28&#40;te&#41;-337&#40;cursus,&#41;-338&#40;ac&#41;-338&#40;consectetur&#41;-338&#40;nibh&#41;-338&#40;commo&#41;-29&#40;do.&#41;-451&#40;A&#41;28&#40;enean&#41;-337&#40;ultricies&#41;]TJ&#10;0.98 0 0 1 0 2629.19 Tm [&#40;ornare&#41;-237&#40;an&#41;28&#40;te&#41;-236&#40;ac&#41;-237&#40;fermen&#41;28&#40;tum.&#41;-418&#40;V&#41;86&#40;estibulum&#41;-237&#40;malesuada&#41;-237&#40;lectus&#41;-237&#40;at&#41;-237&#40;p&#41;-29&#40;ellen&#41;28&#40;tesque&#41;-236&#40;hendrerit.&#41;]TJ&#10;0.98 0 0 1 0 2617.234 Tm [&#40;Praesen&#41;28&#40;t&#41;-319&#40;a&#41;-320&#40;temp&#41;-28&#40;or&#41;-320&#40;ex,&#41;-324&#40;eget&#41;-320&#40;iaculis&#41;-320&#40;mauris.&#41;-447&#40;In&#41;28&#40;teger&#41;-319&#40;turpis&#41;-320&#40;n&#41;28&#40;unc,&#41;-323&#40;v&#41;57&#40;arius&#41;-319&#40;ac&#41;-320&#40;p&#41;-29&#40;osuere&#41;]TJ&#10;1 0 0 1 0 2605.279 Tm [&#40;consequat,&#41;-332&#40;molestie&#41;-332&#40;sed&#41;-332&#40;felis.&#41;-444&#40;F&#41;84&#40;usce&#41;-331&#40;cursus&#41;-332&#40;v&#41;28&#40;elit&#41;-331&#40;eu&#41;-332&#40;magna&#41;-332&#40;p&#41;-29&#40;ellen&#41;28&#40;tesque&#41;-331&#40;p&#41;-29&#40;osuere&#41;]TJ&#10;1 0 0 1 0 2593.324 Tm [&#40;sed&#41;-333&#40;eget&#41;-333&#40;ex.&#41;-445&#40;Viv&#41;55&#40;am&#41;28&#40;us&#41;-333&#40;in&#41;-333&#40;gra&#41;27&#40;vida&#41;-333&#40;quam,&#41;-333&#40;in&#41;-333&#40;v&#41;27&#40;olutpat&#41;-333&#40;erat.&#41;]TJ&#10;/F18 11.95517 Tf&#10;1 0 0 1 -0.672 2565.436 Tm [&#40;1.2&#41;-1125&#40;Subsection&#41;-375&#40;2&#41;]TJ&#10;/F48 9.96264 Tf&#10;1 0 0 1 -0.573 2547.047 Tm [&#40;1.2.1&#41;-1149&#40;Subsubsection&#41;-384&#40;1&#41;]TJ&#10;/F16 9.96264 Tf&#10;0.98 0 0 1 0 2528.657 Tm [&#40;Susp&#41;-29&#40;endisse&#41;-290&#40;erat&#41;-290&#40;est,&#41;-300&#40;imp&#41;-29&#40;erdiet&#41;-291&#40;sed&#41;-290&#40;dolor&#41;-290&#40;at,&#41;-300&#40;sagittis&#41;-291&#40;lob&#41;-29&#40;ortis&#41;-290&#40;tortor.&#41;-437&#40;Nulla&#41;-290&#40;facilisi.&#41;]TJ&#10;1.02 0 0 1 -0.379 2516.702 Tm [&#40;Aliquam&#41;-356&#40;ph&#41;-1&#40;aretra&#41;-356&#40;scelerisque&#41;-357&#40;auctor.&#41;-526&#40;Duis&#41;-357&#40;v&#41;27&#40;el&#41;-356&#40;auctor&#41;-357&#40;ipsum.&#41;-525&#40;Nu&#41;-1&#40;llam&#41;-356&#40;sagittis&#41;]TJ&#10;1.003 0 0 1 0 2504.747 Tm [&#40;feugiat&#41;-331&#40;mollis.&#41;-443&#40;Aliquam&#41;-331&#40;at&#41;-332&#40;ultrices&#41;-331&#40;lib&#41;-29&#40;ero.&#41;-442&#40;Nulla&#41;-332&#40;facilisi.&#41;-443&#40;F&#41;84&#40;usce&#41;-330&#40;s&#41;-1&#40;ed&#41;-331&#40;est&#41;-332&#40;placerat,&#41;]TJ&#10;1 0 0 1 0 2492.792 Tm [&#40;fringilla&#41;-333&#40;augue&#41;-333&#40;at,&#41;-334&#40;pretium&#41;-333&#40;nisl.&#41;]TJ&#10;/F48 9.96264 Tf&#10;1 0 0 1 -0.573 2466.896 Tm [&#40;1.2.2&#41;-1149&#40;Subsubsection&#41;-384&#40;2&#41;]TJ&#10;/F16 9.96264 Tf&#10;0.986 0 0 1 0 2448.507 Tm [&#40;In&#41;-337&#40;ut&#41;-337&#40;n&#41;27&#40;unc&#41;-336&#40;lib&#41;-29&#40;ero.&#41;-450&#40;Duis&#41;-338&#40;eu&#41;-337&#40;elemen&#41;28&#40;tum&#41;-336&#40;purus&#41;-1&#40;.&#41;-450&#40;Etiam&#41;-337&#40;dictum,&#41;-338&#40;ipsum&#41;-337&#40;nec&#41;-338&#40;aliquam&#41;]TJ&#10;1.02 0 0 1 0 2436.552 Tm [&#40;lob&#41;-27&#40;ortis,&#41;-359&#40;magna&#41;-353&#40;magna&#41;-353&#40;p&#41;-27&#40;ellen&#41;27&#40;tesque&#41;-352&#40;ligula,&#41;-359&#40;sed&#41;-353&#40;ultricies&#41;-352&#40;o&#41;-28&#40;dio&#41;-353&#40;ligula&#41;-352&#40;vitae&#41;-353&#40;orci.&#41;]TJ&#10;0.98 0 0 1 0 2424.596 Tm [&#40;F&#41;86&#40;usce&#41;-329&#40;bib&#41;-29&#40;endum&#41;-331&#40;maxim&#41;28&#40;us&#41;-329&#40;ligula,&#41;-333&#40;id&#41;-330&#40;gra&#41;28&#40;vida&#41;-330&#40;felis&#41;-330&#40;dictum&#41;-331&#40;a.&#41;-450&#40;In&#41;-331&#40;dapibus&#41;-330&#40;n&#41;28&#40;ulla&#41;-330&#40;eget&#41;]TJ&#10;1.02 0 0 1 -0.259 2412.641 Tm [&#40;v&#41;27&#40;olutpat&#41;-361&#40;vulputate.&#41;-543&#40;Quisque&#41;-362&#40;congue&#41;-363&#40;erat&#41;-362&#40;quis&#41;-362&#40;nibh&#41;-363&#40;molestie,&#41;-371&#40;eget&#41;-362&#40;v&#41;54&#40;arius&#41;-361&#40;eros&#41;]TJ&#10;1 0 0 1 0 2400.686 Tm [&#40;ultrices.&#41;]TJ&#10;/F48 9.96264 Tf&#10;1.005 0 0 1 0 2374.79 Tm [&#40;Subsubsubsection&#41;]TJ&#10;/F16 9.96264 Tf&#10;1.005 0 0 1 98.591 2374.79 Tm [&#40;Proin&#41;-333&#40;eleifend&#41;-333&#40;lorem&#41;-333&#40;semp&#41;-28&#40;er,&#41;-334&#40;commo&#41;-28&#40;do&#41;-333&#40;tellus&#41;-333&#40;nec,&#41;-334&#40;p&#41;-28&#40;orta&#41;]TJ&#10;1.02 0 0 1 0 2362.835 Tm [&#40;purus.&#41;-639&#40;Nullam&#41;-395&#40;commo&#41;-28&#40;do&#41;-394&#40;lectus&#41;-395&#40;nibh,&#41;-412&#40;consequat&#41;-394&#40;maxim&#41;26&#40;us&#41;-393&#40;lorem&#41;-395&#40;faucibus&#41;-395&#40;in.&#41;]TJ&#10;1 0 0 1 0 2350.88 Tm [&#40;Nam&#41;-333&#40;purus&#41;-333&#40;eros,&#41;-334&#40;rutrum&#41;-333&#40;in&#41;-333&#40;sapien&#41;-334&#40;et,&#41;-333&#40;condimen&#41;27&#40;tum&#41;-333&#40;lacinia&#41;-333&#40;nibh.&#41;]TJ&#10;/F18 14.3462 Tf&#10;1 0 0 1 -0.404 2317.934 Tm [&#40;2&#41;-1125&#40;T&#41;31&#40;yp&#41;-31&#40;ograph&#41;31&#40;y&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 2296.114 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F48 9.96264 Tf&#10;1 0 0 1 24.907 2296.114 Tm [&#40;Bold&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 2284.158 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F50 9.96264 Tf&#10;1 0 0 1 24.907 2284.158 Tm [&#40;Italic&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 2272.203 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F51 9.96264 Tf&#10;1 0 0 1 24.907 2272.203 Tm [&#40;Bold&#41;-414&#40;italic&#41;]TJ&#10;/F16 9.96264 Tf&#10;1 0 0 1 77.292 2272.203 Tm [&#40;.&#41;]TJ&#10;/F18 14.3462 Tf&#10;1 0 0 1 -0.404 2239.257 Tm [&#40;3&#41;-1125&#40;Num&#41;31&#40;b&#41;-31&#40;ers&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 2217.437 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 2217.437 Tm [&#40;Normal:&#41;-444&#40;0123456789&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 2205.482 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 2205.482 Tm [&#40;Math:&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 55.625 2205.482 Tm [&#40;0123456789&#41;]TJ&#10;/F18 14.3462 Tf&#10;1 0 0 1 -0.565 2172.536 Tm [&#40;4&#41;-1125&#40;A&#41;31&#40;cron&#41;31&#40;yms&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 2150.715 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 2150.715 Tm [&#40;Default&#41;-333&#40;&#92;050short+long&#92;051:&#41;-444&#40;Carnegie&#41;-334&#40;Mellon&#41;-333&#40;Univ&#41;27&#40;ersit&#41;28&#40;y&#41;-333&#40;&#92;050&#41;]TJ&#10;/F54 7.97011 Tf&#10;1 0 0 1 250.173 2150.715 Tm [&#40;C&#41;-110&#40;M&#41;-111&#40;U&#41;]TJ&#10;/F16 9.96264 Tf&#10;1 0 0 1 273.23 2150.715 Tm [&#40;&#92;051&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 2138.76 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 2138.76 Tm [&#40;Rep&#41;-27&#40;eated&#41;-334&#40;&#92;050short&#92;051:&#41;]TJ&#10;/F54 7.97011 Tf&#10;1 0 0 1 105.318 2138.76 Tm [&#40;C&#41;-110&#40;M&#41;-111&#40;U&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 2126.805 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 2126.805 Tm [&#40;F&#41;83&#40;orced&#41;-332&#40;sh&#41;-1&#40;ort:&#41;]TJ&#10;/F54 7.97011 Tf&#10;1 0 0 1 85.697 2126.805 Tm [&#40;U&#41;-110&#40;S&#41;-111&#40;A&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 2114.849 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;0.98 0 0 1 24.907 2114.849 Tm [&#40;Rep&#41;-28&#40;eated&#41;-309&#40;after&#41;-308&#40;forced&#41;-309&#40;short&#41;-309&#40;&#92;050short+long&#92;051:&#41;-437&#40;United&#41;-309&#40;States&#41;-309&#40;of&#41;-308&#40;America&#41;-309&#40;&#92;050&#41;]TJ&#10;/F54 7.97011 Tf&#10;1 0 0 1 320.812 2114.849 Tm [&#40;U&#41;-110&#40;S&#41;-111&#40;A&#41;]TJ&#10;/F16 9.96264 Tf&#10;0.98 0 0 1 341.08 2114.849 Tm [&#40;&#92;051&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 2102.894 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 2102.894 Tm [&#40;Plural:&#41;-444&#40;so&#41;-28&#40;cial&#41;-333&#40;securit&#41;27&#40;y&#41;-333&#40;n&#41;27&#40;um&#41;28&#40;b&#41;-27&#40;ers&#41;-333&#40;&#92;050&#41;]TJ&#10;/F54 7.97011 Tf&#10;1 0 0 1 167.759 2102.894 Tm [&#40;S&#41;-110&#40;S&#41;-111&#40;N&#41;-110&#40;s&#41;]TJ&#10;/F16 9.96264 Tf&#10;1 0 0 1 190.94 2102.894 Tm [&#40;&#92;051&#41;]TJ&#10;/F18 14.3462 Tf&#10;1 0 0 1 0 2069.949 Tm [&#40;5&#41;-1125&#40;Math&#41;]TJ&#10;/F28 9.96264 Tf&#10;1 0 0 1 139.373 2058.547 Tm [&#40;Z&#41;]TJ&#10;/F26 6.97385 Tf&#10;1 0 0 1 149.336 2056.084 Tm [&#40;1&#41;]TJ&#10;/F20 6.97385 Tf&#10;1 0 0 1 144.908 2035.91 Tm [&#40;0&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 159.437 2044.987 Tm [&#40;exp&#41;]TJ&#10;/F26 6.97385 Tf&#10;1 0 0 1 174.658 2049.1 Tm [&#40;&#92;000&#41;]TJ&#10;/F23 6.97385 Tf&#10;1 0 0 1 180.884 2049.1 Tm [&#40;x&#41;]TJ&#10;/F21 4.98132 Tf&#10;1 0 0 1 185.402 2052.107 Tm [&#40;2&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 193.109 2044.987 Tm [&#40;d&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 198.644 2044.987 Tm [&#40;x&#41;]TJ&#10;/F16 9.96264 Tf&#10;1 0 0 1 332.146 2044.987 Tm [&#40;&#92;0501&#92;051&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 3.312 2005.136 Tm [&#40;a;&#41;-166&#40;b;&#41;-167&#40;c;&#41;-166&#40;d;&#41;-167&#40;e;&#41;-167&#40;f&#41;-52&#40;;&#41;-166&#40;g&#41;-36&#40;;&#41;-167&#40;h;&#41;-166&#40;i;&#41;-167&#40;j&#41;-2&#40;;&#41;-166&#40;k&#41;-32&#40;;&#41;-167&#40;l&#41;-19&#40;;&#41;-167&#40;m;&#41;-167&#40;n;&#41;-166&#40;o;&#41;-167&#40;p;&#41;-167&#40;q&#41;-35&#40;;&#41;-167&#40;r&#41;27&#40;;&#41;-166&#40;s;&#41;-166&#40;t;&#41;-167&#40;u;&#41;-167&#40;v&#41;-36&#40;;&#41;-166&#40;w&#41;-27&#40;;&#41;-167&#40;x;&#41;-167&#40;y&#41;-35&#40;;&#41;-167&#40;z&#41;-44&#40;;&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 250.736 2005.136 Tm [&#40;0&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 255.717 2005.136 Tm [&#40;;&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 260.145 2005.136 Tm [&#40;1&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 265.126 2005.136 Tm [&#40;;&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 269.554 2005.136 Tm [&#40;2&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 274.535 2005.136 Tm [&#40;;&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 278.963 2005.136 Tm [&#40;3&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 283.944 2005.136 Tm [&#40;;&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 288.372 2005.136 Tm [&#40;4&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 293.353 2005.136 Tm [&#40;;&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 297.781 2005.136 Tm [&#40;5&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 302.763 2005.136 Tm [&#40;;&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 307.19 2005.136 Tm [&#40;6&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 312.172 2005.136 Tm [&#40;;&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 316.6 2005.136 Tm [&#40;7&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 321.581 2005.136 Tm [&#40;;&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 326.009 2005.136 Tm [&#40;8&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 330.99 2005.136 Tm [&#40;;&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 335.418 2005.136 Tm [&#40;9&#41;]TJ&#10;/F16 9.96264 Tf&#10;1 0 0 1 332.146 1993.181 Tm [&#40;&#92;0502&#92;051&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 1969.899 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 1969.899 Tm [&#40;Inline:&#41;]TJ&#10;/F28 9.96264 Tf&#10;1 0 0 1 56.731 1977.925 Tm [&#40;R&#41;]TJ&#10;/F26 6.97385 Tf&#10;1 0 0 1 63.373 1975.462 Tm [&#40;1&#41;]TJ&#10;/F20 6.97385 Tf&#10;1 0 0 1 61.436 1966.357 Tm [&#40;0&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 73.474 1969.899 Tm [&#40;exp&#41;]TJ&#10;/F26 6.97385 Tf&#10;1 0 0 1 88.695 1973.515 Tm [&#40;&#92;000&#41;]TJ&#10;/F23 6.97385 Tf&#10;1 0 0 1 94.922 1973.515 Tm [&#40;x&#41;]TJ&#10;/F21 4.98132 Tf&#10;1 0 0 1 99.439 1976.521 Tm [&#40;2&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 107.147 1969.899 Tm [&#40;d&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 112.681 1969.899 Tm [&#40;x&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 1957.944 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 1957.944 Tm [&#40;Blo&#41;-27&#40;c&#41;27&#40;k:&#41;-444&#40;Equation&#41;-333&#40;1,&#41;-334&#40;Equation&#41;-333&#40;2&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 1945.989 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 1945.989 Tm [&#40;Commands&#41;-333&#40;de&#92;034ned&#41;-333&#40;in&#41;-334&#40;b&#41;-28&#40;o&#41;-27&#40;dy&#41;-334&#40;&#92;050P[x&#41;-333&#40;in&#41;-333&#40;X]&#92;051:&#41;]TJ&#10;/F34 9.96264 Tf&#10;1 0 0 1 201.936 1945.989 Tm [&#40;P&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 208.523 1945.989 Tm [&#40;[&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 211.29 1945.989 Tm [&#40;x&#41;]TJ&#10;/F25 9.96264 Tf&#10;1 0 0 1 219.751 1945.989 Tm [&#40;2&#41;-277&#40;X&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 237.726 1945.989 Tm [&#40;]&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 1934.034 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.528 1934.034 Tm [&#40;Aligned:&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 172.228 1902.751 Tm [&#40;x&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 180.689 1902.751 Tm [&#40;=&#41;-277&#40;1&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 154.81 1887.807 Tm [&#40;x&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 162.717 1887.807 Tm [&#40;+&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 172.68 1887.807 Tm [&#40;y&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 180.689 1887.807 Tm [&#40;=&#41;-277&#40;10&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 137.562 1872.863 Tm [&#40;x&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 145.47 1872.863 Tm [&#40;+&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 155.432 1872.863 Tm [&#40;y&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 162.888 1872.863 Tm [&#40;+&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 172.851 1872.863 Tm [&#40;z&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 180.689 1872.863 Tm [&#40;=&#41;-277&#40;100&#41;]TJ&#10;/F18 14.3462 Tf&#10;1 0 0 1 0 1843.459 Tm [&#40;6&#41;-1125&#40;Links&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 1821.638 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 1821.638 Tm [&#40;Section:&#41;-444&#40;Section&#41;-333&#40;1,&#41;-334&#40;Section&#41;-333&#40;1.2&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 1809.683 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.528 1809.683 Tm [&#40;App&#41;-27&#40;endix&#41;-334&#40;section:&#41;-444&#40;Section&#41;]TJ&#10;/F48 9.96264 Tf&#10;1 0 0 1 142.198 1809.683 Tm [&#40;??&#41;]TJ&#10;/F16 9.96264 Tf&#10;1 0 0 1 153.019 1809.683 Tm [&#40;,&#41;-333&#40;Section&#41;]TJ&#10;/F48 9.96264 Tf&#10;1 0 0 1 193.976 1809.683 Tm [&#40;??&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 1797.728 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.528 1797.728 Tm [&#40;App&#41;-27&#40;endix&#41;-334&#40;&#92;034gure:&#41;-444&#40;Figure&#41;]TJ&#10;/F48 9.96264 Tf&#10;1 0 0 1 133.204 1797.728 Tm [&#40;??&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 1785.773 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.528 1785.773 Tm [&#40;App&#41;-27&#40;endix&#41;-334&#40;table:&#41;-444&#40;T&#41;82&#40;able&#41;]TJ&#10;/F48 9.96264 Tf&#10;1 0 0 1 126.368 1785.773 Tm [&#40;??&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 1773.817 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.528 1773.817 Tm [&#40;App&#41;-27&#40;endix&#41;-334&#40;math:&#41;-444&#40;Equation&#41;]TJ&#10;/F48 9.96264 Tf&#10;1 0 0 1 143.111 1773.817 Tm [&#40;??&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 1761.862 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 1761.862 Tm [&#40;Short&#41;-333&#40;citation&#41;]TJ&#10;/F56 6.97385 Tf&#10;1 0 0 1 86.26 1765.478 Tm [&#40;[1]&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 1749.907 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 1749.907 Tm [&#40;Long&#41;-333&#40;citation:&#41;-444&#40;Mittelbac&#41;27&#40;h&#41;-333&#40;et&#41;-333&#40;al.&#41;-383&#40;&#92;0502004&#41;-50&#40;&#92;051&#41;]TJ&#10;/F56 6.97385 Tf&#10;1 0 0 1 195.85 1753.522 Tm [&#40;[1]&#41;]TJ&#10;/F16 9.96264 Tf&#10;1 0 0 1 204.83 1749.907 Tm [&#40;,&#41;-333&#40;Lesk&#41;-333&#40;and&#41;-334&#40;Kernighan&#41;-383&#40;&#92;0501977&#41;-50&#40;&#92;051&#41;]TJ&#10;/F56 6.97385 Tf&#10;1 0 0 1 331.854 1753.522 Tm [&#40;[2]&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 1737.952 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 1737.952 Tm [&#40;Multi&#41;-333&#40;citation&#41;]TJ&#10;/F56 6.97385 Tf&#10;1 0 0 1 86.509 1741.567 Tm [&#40;[1&#92;0253]&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 1725.997 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 1725.997 Tm [&#40;P&#41;27&#40;oin&#41;28&#40;ter&#41;-332&#40;to&#41;-334&#40;fo&#41;-27&#40;otnote&#41;]TJ&#10;/F57 6.97385 Tf&#10;1 0 0 1 108.095 1729.612 Tm [&#40;a&#41;]TJ&#10;/F18 14.3462 Tf&#10;1 0 0 1 -0.404 1693.051 Tm [&#40;7&#41;-1125&#40;T&#41;93&#40;ables&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 1671.23 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.548 1671.23 Tm [&#40;T&#41;83&#40;able&#41;-333&#40;1&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 1659.275 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.548 1659.275 Tm [&#40;T&#41;83&#40;able&#41;-333&#40;2&#41;]TJ&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;ET&#10;q&#10;1 0 0 1 112.412 1647.918 cm&#10;[] 0 d 0 J 0.797 w 0 0 m 115.566 0 l S&#10;Q&#10;BT&#10;/F16 9.96264 Tf&#10;1 0 0 1 112.412 1636.36 Tm [&#40;Col1&#41;-1200&#40;Col2&#41;-1200&#40;Col3&#41;-1200&#40;Col4&#41;]TJ&#10;ET&#10;q&#10;1 0 0 1 112.412 1630.806 cm&#10;[] 0 d 0 J 0.498 w 0 0 m 115.566 0 l S&#10;Q&#10;BT&#10;/F16 9.96264 Tf&#10;1 0 0 1 112.412 1619.398 Tm [&#40;1&#41;-4200&#40;2&#41;-1950&#40;3&#41;-1950&#40;4&#41;]TJ&#10;1 0 0 1 112.412 1607.443 Tm [&#40;11&#41;-3200&#40;22&#41;-1700&#40;33&#41;-1700&#40;44&#41;]TJ&#10;1 0 0 1 112.412 1595.487 Tm [&#40;111&#41;-2200&#40;222&#41;-1450&#40;333&#41;-1450&#40;444&#41;]TJ&#10;ET&#10;q&#10;1 0 0 1 112.412 1589.785 cm&#10;[] 0 d 0 J 0.797 w 0 0 m 115.566 0 l S&#10;Q&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;BT&#10;/F16 9.96264 Tf&#10;1 0 0 1 -0.359 1571.055 Tm [&#40;T&#41;83&#40;able&#41;-333&#40;1:&#41;-444&#40;Short&#41;-333&#40;table&#41;]TJ&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;ET&#10;q&#10;1 0 0 1 13.616 1556.111 cm&#10;[] 0 d 0 J 0.797 w 0 0 m 313.158 0 l S&#10;Q&#10;BT&#10;/F16 9.96264 Tf&#10;1 0 0 1 14.115 1544.553 Tm [&#40;Col1&#41;-1200&#40;Col2&#41;-1200&#40;Col3&#41;-1199&#40;Col4&#41;-1200&#40;Col5&#41;-1284&#40;Col6&#41;-1200&#40;Col7&#41;-1200&#40;Col8&#41;-1200&#40;Col9&#41;-1200&#40;Col10&#41;]TJ&#10;ET&#10;q&#10;1 0 0 1 13.616 1539 cm&#10;[] 0 d 0 J 0.498 w 0 0 m 313.158 0 l S&#10;Q&#10;BT&#10;/F16 9.96264 Tf&#10;1 0 0 1 29.059 1527.591 Tm [&#40;a&#41;-2700&#40;1&#41;-2699&#40;2&#41;-2700&#40;3&#41;-1700&#40;123&#41;-1200&#40;ab&#41;-28&#40;cd&#41;-1200&#40;1234&#41;-1700&#40;444&#41;-1700&#40;555&#41;-2200&#40;666&#41;]TJ&#10;1 0 0 1 28.505 1515.636 Tm [&#40;b&#41;-2200&#40;11&#41;-2200&#40;22&#41;-2200&#40;33&#41;-1700&#40;456&#41;-1477&#40;efgh&#41;-1700&#40;567&#41;-2200&#40;44&#41;-2200&#40;55&#41;-2700&#40;66&#41;]TJ&#10;/F48 9.96264 Tf&#10;1 0 0 1 13.616 1491.726 Tm [&#40;Mid&#41;]TJ&#10;/F16 9.96264 Tf&#10;1 0 0 1 29.612 1479.77 Tm [&#40;c&#41;-1699&#40;111&#41;-1700&#40;222&#41;-1700&#40;333&#41;-1700&#40;789&#41;-1895&#40;ijkl&#41;-2200&#40;89&#41;-2700&#40;4&#41;-2700&#40;5&#41;-3200&#40;6&#41;]TJ&#10;ET&#10;q&#10;1 0 0 1 13.616 1474.068 cm&#10;[] 0 d 0 J 0.797 w 0 0 m 313.158 0 l S&#10;Q&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;BT&#10;/F16 9.96264 Tf&#10;1 0 0 1 -0.359 1455.338 Tm [&#40;T&#41;83&#40;able&#41;-333&#40;2:&#41;-444&#40;Wide&#41;-333&#40;table&#41;]TJ&#10;0 g 0 G&#10;/F18 14.3462 Tf&#10;1 0 0 1 0 1422.392 Tm [&#40;8&#41;-1125&#40;Figures&#41;]TJ&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;ET&#10;q&#10;1 0 0 1 70.475 1199.139 cm&#10;/Im4 Do&#10;Q&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;q&#10;1 0 0 1 0 1192.963 cm&#10;[] 0 d 0 J 0.398 w 0 0 m 137.482 0 l S&#10;Q&#10;BT&#10;/F57 5.97758 Tf&#10;1 0 0 1 13.829 1186.361 Tm [&#40;a&#41;]TJ&#10;/F58 7.97011 Tf&#10;1 0 0 1 17.933 1183.548 Tm [&#40;Example&#41;-354&#40;fo&#41;-29&#40;otnote&#41;-354&#40;text.&#41;]TJ&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 0 1154.407 Tm [&#40;Figure&#41;-333&#40;2:&#41;-444&#40;Narro&#41;27&#40;w&#41;-333&#40;&#92;034gure&#41;]TJ&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;ET&#10;1 0 0 1 0 909.319 cm&#10;q&#10;.95476 0 0 .95476 0 0 cm&#10;0 g 0 G&#10;q&#10;.95241 0 0 .95241 0 0 cm&#10;0 g 0 G&#10;q&#10;1 0 0 1 0 0 cm&#10;/Im5 Do&#10;Q&#10;0 g 0 G&#10;Q&#10;0 g 0 G&#10;Q&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;1 0 0 1 0 -909.319 cm&#10;BT&#10;/F16 9.96264 Tf&#10;1 0 0 1 0 871.063 Tm [&#40;Figure&#41;-333&#40;3:&#41;-444&#40;Wide&#41;-334&#40;&#92;034gure&#41;]TJ&#10;0 g 0 G&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 849.145 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 849.145 Tm [&#40;Figure&#41;-333&#40;2&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 837.19 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 837.19 Tm [&#40;Figure&#41;-333&#40;3&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 825.235 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 825.235 Tm [&#40;Figure&#41;-333&#40;4,&#41;-333&#40;Figure&#41;-333&#40;3a,&#41;-334&#40;Figure&#41;-333&#40;3b&#41;]TJ&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;ET&#10;1 0 0 1 81.851 629.286 cm&#10;q&#10;.83337 0 0 .83337 0 0 cm&#10;0 g 0 G&#10;q&#10;1 0 0 1 0 0 cm&#10;/Im1 Do&#10;Q&#10;0 g 0 G&#10;Q&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;1 0 0 1 -81.851 -629.286 cm&#10;BT&#10;/F16 9.96264 Tf&#10;1 0 0 1 81.851 610.955 Tm [&#40;a:&#41;-444&#40;Figure&#41;-333&#40;with&#41;-334&#40;`width=2.5in&#39;&#41;]TJ&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;ET&#10;1 0 0 1 44.195 354.373 cm&#10;q&#10;.875 0 0 .875 0 0 cm&#10;0 g 0 G&#10;q&#10;1 0 0 1 0 0 cm&#10;/Im3 Do&#10;Q&#10;0 g 0 G&#10;Q&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;1 0 0 1 -44.195 -354.373 cm&#10;BT&#10;/F16 9.96264 Tf&#10;1 0 0 1 44.195 336.041 Tm [&#40;b:&#41;-444&#40;Figure&#41;-333&#40;with&#41;-334&#40;`width=3.5in&#39;&#41;]TJ&#10;/F57 6.97385 Tf&#10;1 0 0 1 170.278 339.657 Tm [&#40;a&#41;]TJ&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 0 306.103 Tm [&#40;Figure&#41;-333&#40;4:&#41;-444&#40;Sub-&#92;034gu&#41;-1&#40;res&#41;]TJ&#10;/F57 6.97385 Tf&#10;1 0 0 1 91.85 309.718 Tm [&#40;b&#41;]TJ&#10;0 g 0 G&#10;/F18 14.3462 Tf&#10;1 0 0 1 0 273.157 Tm [&#40;9&#41;-1125&#40;Includes&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 251.336 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 251.336 Tm [&#40;Commands&#41;-333&#40;from&#41;-333&#40;metadata&#41;-334&#40;include:&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 183.007 251.336 Tm [&#40;arg&#41;-180&#40;min&#41;]TJ&#10;/F34 9.96264 Tf&#10;1 0 0 1 218.595 251.336 Tm [&#40;R&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 239.381 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 239.381 Tm [&#40;Include&#41;-333&#40;command&#41;-333&#40;in&#41;-334&#40;b&#41;-27&#40;o&#41;-28&#40;dy&#41;-334&#40;&#92;050there&#41;-333&#40;should&#41;-333&#40;b&#41;-28&#40;e&#41;-333&#40;text&#41;-334&#40;after&#41;-333&#40;this&#92;051:&#41;]TJ&#10;1 0 0 1 0 217.463 Tm [&#40;Con&#41;27&#40;ten&#41;28&#40;t&#41;-332&#40;added&#41;-334&#40;through&#41;-333&#40;include&#41;-334&#40;statemen&#41;27&#40;t.&#41;]TJ&#10;/F18 14.3462 Tf&#10;1 0 0 1 0 174.499 Tm [&#40;References&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 0 152.679 Tm [&#40;[1]&#41;]TJ&#10;0 g 0 G&#10;1.02 0 0 1 15.497 152.679 Tm [&#40;F&#41;83&#40;rank&#41;-338&#40;Mittelbac&#41;27&#40;h,&#41;-341&#40;Mic&#41;27&#40;hel&#41;-338&#40;Gossens,&#41;-342&#40;Johannes&#41;-339&#40;Braams,&#41;-341&#40;Da&#41;27&#40;vid&#41;-338&#40;Carlisle,&#41;-342&#40;and&#41;]TJ&#10;0.98 0 0 1 15.497 140.723 Tm [&#40;Chris&#41;-269&#40;Ro&#41;28&#40;wley&#41;87&#40;.&#41;]TJ&#10;/F50 9.96264 Tf&#10;0.98 0 0 1 77.185 140.723 Tm [&#40;The&#41;-299&#40;L&#41;]TJ&#10;/F57 6.97385 Tf&#10;1 0 0 1 99.038 142.782 Tm [&#40;A&#41;]TJ&#10;/F50 9.96264 Tf&#10;0.98 0 0 1 103.549 140.723 Tm [&#40;T&#41;]TJ&#10;1 0 0 1 108.837 138.579 Tm [&#40;E&#41;]TJ&#10;0.98 0 0 1 114.323 140.723 Tm [&#40;X&#41;-299&#40;Comp&#41;52&#40;anion&#41;]TJ&#10;/F16 9.96264 Tf&#10;0.98 0 0 1 172.892 140.723 Tm [&#40;.&#41;-336&#40;A&#41;28&#40;ddison-W&#41;86&#40;esley&#41;-268&#40;Professional,&#41;-284&#40;2&#41;-269&#40;edition,&#41;]TJ&#10;1 0 0 1 15.248 128.768 Tm [&#40;2004.&#41;]TJ&#10;0 g 0 G&#10;1 0 0 1 0 108.843 Tm [&#40;[2]&#41;]TJ&#10;0 g 0 G&#10;1.02 0 0 1 15.497 108.843 Tm [&#40;Mic&#41;27&#40;hael&#41;-465&#40;Lesk&#41;-466&#40;and&#41;-466&#40;Brian&#41;-466&#40;Kernighan.&#41;-850&#40;Computer&#41;-466&#40;t&#41;27&#40;yp&#41;-27&#40;esetting&#41;-466&#40;of&#41;-466&#40;tec&#41;27&#40;hnical&#41;]TJ&#10;1.02 0 0 1 15.497 96.888 Tm [&#40;journals&#41;-346&#40;on&#41;-347&#40;UNIX.&#41;-494&#40;In&#41;]TJ&#10;/F50 9.96264 Tf&#10;1.02 0 0 1 115.846 96.888 Tm [&#40;Pr&#41;51&#40;o&#41;51&#40;c&#41;51&#40;e&#41;51&#40;e&#41;51&#40;dings&#41;-368&#40;of&#41;-369&#40;A&#41;50&#40;meric&#41;52&#40;an&#41;-369&#40;F&#41;76&#40;e&#41;51&#40;der&#41;51&#40;a&#41;1&#40;tion&#41;-369&#40;of&#41;-368&#40;I&#41;-1&#40;nformation&#41;]TJ&#10;1.02 0 0 1 14.947 84.933 Tm [&#40;Pr&#41;51&#40;o&#41;51&#40;c&#41;51&#40;essing&#41;-355&#40;So&#41;50&#40;cieties:&#41;-460&#40;1977&#41;-356&#40;National&#41;-356&#40;Computer&#41;-355&#40;Confer&#41;50&#40;enc&#41;51&#40;e&#41;]TJ&#10;/F16 9.96264 Tf&#10;1.02 0 0 1 272.785 84.933 Tm [&#40;,&#41;-333&#40;pages&#41;-332&#40;879&#92;025888,&#41;]TJ&#10;1 0 0 1 15.497 72.977 Tm [&#40;Dallas,&#41;-333&#40;T&#41;83&#40;exas,&#41;-333&#40;1977.&#41;]TJ&#10;0 g 0 G&#10;1 0 0 1 0 53.052 Tm [&#40;[3]&#41;]TJ&#10;0 g 0 G&#10;1.02 0 0 1 15.497 53.052 Tm [&#40;Donald&#41;-379&#40;E.&#41;-380&#40;Kn&#41;27&#40;uth.&#41;-591&#40;Literate&#41;-379&#40;programming.&#41;]TJ&#10;/F50 9.96264 Tf&#10;1.02 0 0 1 209.53 53.052 Tm [&#40;The&#41;-399&#40;Computer&#41;-399&#40;Journal&#41;]TJ&#10;/F16 9.96264 Tf&#10;1.02 0 0 1 312.313 53.052 Tm [&#40;,&#41;-392&#40;27&#92;0502&#92;051:&#41;]TJ&#10;1 0 0 1 15.497 41.097 Tm [&#40;97&#92;025111,&#41;-333&#40;1984.&#41;]TJ&#10;0 g 0 G&#10;ET&#10;q&#10;1 0 0 1 0 23.02 cm&#10;[] 0 d 0 J 0.398 w 0 0 m 137.482 0 l S&#10;Q&#10;BT&#10;/F57 5.97758 Tf&#10;1 0 0 1 13.829 16.418 Tm [&#40;a&#41;]TJ&#10;/F58 7.97011 Tf&#10;1 0 0 1 17.933 13.606 Tm [&#40;F&#41;88&#40;o&#41;-28&#40;otnote&#41;-355&#40;in&#41;-354&#40;sub-&#92;034gure&#41;-354&#40;caption.&#41;]TJ&#10;/F57 5.97758 Tf&#10;1 0 0 1 14.18 6.648 Tm [&#40;b&#41;]TJ&#10;/F58 7.97011 Tf&#10;1 0 0 1 17.933 3.836 Tm [&#40;F&#41;88&#40;o&#41;-28&#40;otnote&#41;-355&#40;in&#41;-354&#40;&#92;034gure&#41;-354&#40;caption.&#41;]TJ&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;ET&#10;</data>
+<data size="21306">0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;BT&#10;/F18 14.3462 Tf&#10;1 0 0 1 -0.807 3168.01 Tm [&#40;1&#41;-1125&#40;Section&#41;]TJ&#10;/F16 9.96264 Tf&#10;0.98 0 0 1 0 3146.189 Tm [&#40;In&#41;28&#40;tege&#41;1&#40;r&#41;-280&#40;at&#41;-281&#40;enim&#41;-281&#40;eu&#41;-281&#40;tellus&#41;-281&#40;malesuada&#41;-281&#40;scelerisque.&#41;-434&#40;Ut&#41;-281&#40;sed&#41;-281&#40;rhoncus&#41;-281&#40;ipsum,&#41;-292&#40;at&#41;-281&#40;temp&#41;-29&#40;or&#41;]TJ&#10;0.996 0 0 1 0 3134.234 Tm [&#40;nisl.&#41;-446&#40;Viv&#41;56&#40;am&#41;29&#40;us&#41;-334&#40;vitae&#41;-335&#40;pulvinar&#41;-335&#40;leo,&#41;-334&#40;at&#41;-335&#40;pharetra&#41;-335&#40;massa.&#41;-446&#40;Ut&#41;-335&#40;lob&#41;-28&#40;ortis&#41;-335&#40;o&#41;-29&#40;dio&#41;-334&#40;non&#41;-335&#40;n&#41;27&#40;ulla&#41;]TJ&#10;0.98 0 0 1 0 3122.279 Tm [&#40;tincidun&#41;28&#40;t&#41;-312&#40;pulvinar.&#41;-445&#40;Nunc&#41;-313&#40;faucibus&#41;-314&#40;p&#41;-28&#40;ellen&#41;28&#40;tesque&#41;-313&#40;elit,&#41;-318&#40;non&#41;-314&#40;ornare&#41;-313&#40;risus&#41;-313&#40;su&#41;-1&#40;scipit&#41;-313&#40;sed.&#41;]TJ&#10;1 0 0 1 0 3110.323 Tm [&#40;Maecenas&#41;-333&#40;v&#41;27&#40;el&#41;-332&#40;blandit&#41;-334&#40;ex.&#41;]TJ&#10;0.98 0 0 1 0 3098.368 Tm [&#40;Phasellus&#41;-286&#40;ultrices&#41;-285&#40;mi&#41;-286&#40;non&#41;-286&#40;n&#41;28&#40;ulla&#41;-285&#40;hendrerit,&#41;-297&#40;at&#41;-285&#40;rhoncus&#41;-286&#40;augue&#41;-286&#40;suscipit.&#41;-436&#40;P&#41;28&#40;elle&#41;1&#40;n&#41;28&#40;tesque&#41;]TJ&#10;1.02 0 0 1 0 3086.413 Tm [&#40;a&#41;-544&#40;lectus&#41;-544&#40;eget&#41;-544&#40;felis&#41;-544&#40;maxim&#41;27&#40;us&#41;-543&#40;feugiat&#41;-544&#40;nec&#41;-544&#40;ut&#41;-544&#40;an&#41;27&#40;te.&#41;-1087&#40;Sed&#41;-544&#40;eget&#41;-544&#40;laoreet&#41;-544&#40;lectus.&#41;]TJ&#10;1.02 0 0 1 -0.379 3074.458 Tm [&#40;V&#41;83&#40;estibulum&#41;-370&#40;iaculis&#41;-370&#40;enim&#41;-371&#40;nec&#41;-370&#40;lib&#41;-28&#40;ero&#41;-370&#40;s&#41;-1&#40;ollicitudin,&#41;-381&#40;id&#41;-370&#40;rhon&#41;-1&#40;cus&#41;-370&#40;lib&#41;-28&#40;ero&#41;-370&#40;consectetur.&#41;]TJ&#10;1 0 0 1 0 3062.503 Tm [&#40;In&#41;27&#40;teger&#41;-332&#40;eget&#41;-333&#40;sem&#41;-334&#40;quis&#41;-333&#40;urna&#41;-333&#40;vulpu&#41;-1&#40;tate&#41;-333&#40;aliquet.&#41;]TJ&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;ET&#10;1 0 0 1 21.206 2902.555 cm&#10;q&#10;.6667 0 0 .6667 0 0 cm&#10;0 g 0 G&#10;q&#10;1 0 0 1 0 0 cm&#10;/Im1 Do&#10;Q&#10;0 g 0 G&#10;Q&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;1 0 0 1 -21.206 -2902.555 cm&#10;BT&#10;/F16 9.96264 Tf&#10;1 0 0 1 21.206 2884.224 Tm [&#40;a:&#41;-444&#40;Sub-&#92;034gure&#41;-334&#40;with&#41;-333&#40;`width=2in&#39;&#41;]TJ&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;ET&#10;1 0 0 1 178.497 2902.555 cm&#10;q&#10;.6667 0 0 .6667 0 0 cm&#10;0 g 0 G&#10;q&#10;216 0 0 216 0 0 cm&#10;/Im2 Do&#10;Q&#10;0 g 0 G&#10;Q&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;1 0 0 1 -178.497 -2902.555 cm&#10;BT&#10;/F16 9.96264 Tf&#10;1 0 0 1 178.497 2884.224 Tm [&#40;b:&#41;-444&#40;Sub-&#92;034gure&#41;-334&#40;with&#41;-333&#40;`width=2in&#39;&#41;]TJ&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;ET&#10;1 0 0 1 96.535 2735.642 cm&#10;q&#10;.5 0 0 .5 0 0 cm&#10;0 g 0 G&#10;q&#10;1 0 0 1 0 0 cm&#10;/Im3 Do&#10;Q&#10;0 g 0 G&#10;Q&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;1 0 0 1 -96.535 -2735.642 cm&#10;BT&#10;/F16 9.96264 Tf&#10;1 0 0 1 96.535 2717.31 Tm [&#40;c:&#41;-444&#40;Sub-&#92;034gure&#41;-333&#40;with&#41;-334&#40;`width=2in&#39;&#41;]TJ&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;1 0 0 1 0 2687.422 Tm [&#40;Figure&#41;-333&#40;1:&#41;-444&#40;Sub-&#92;034gu&#41;-1&#40;res&#41;]TJ&#10;0 g 0 G&#10;/F18 11.95517 Tf&#10;1 0 0 1 -0.672 2659.534 Tm [&#40;1.1&#41;-1125&#40;Subsection&#41;-375&#40;1&#41;]TJ&#10;/F16 9.96264 Tf&#10;0.987 0 0 1 0 2641.145 Tm [&#40;In&#41;-338&#40;mollis&#41;-338&#40;tortor&#41;-338&#40;v&#41;28&#40;el&#41;-337&#40;an&#41;28&#40;te&#41;-337&#40;cursus,&#41;-338&#40;ac&#41;-338&#40;consectetur&#41;-338&#40;nibh&#41;-338&#40;commo&#41;-29&#40;do.&#41;-451&#40;A&#41;28&#40;enean&#41;-337&#40;ultricies&#41;]TJ&#10;0.98 0 0 1 0 2629.19 Tm [&#40;ornare&#41;-237&#40;an&#41;28&#40;te&#41;-236&#40;ac&#41;-237&#40;fermen&#41;28&#40;tum.&#41;-418&#40;V&#41;86&#40;estibulum&#41;-237&#40;malesuada&#41;-237&#40;lectus&#41;-237&#40;at&#41;-237&#40;p&#41;-29&#40;ellen&#41;28&#40;tesque&#41;-236&#40;hendrerit.&#41;]TJ&#10;0.98 0 0 1 0 2617.234 Tm [&#40;Praesen&#41;28&#40;t&#41;-319&#40;a&#41;-320&#40;temp&#41;-28&#40;or&#41;-320&#40;ex,&#41;-324&#40;eget&#41;-320&#40;iaculis&#41;-320&#40;mauris.&#41;-447&#40;In&#41;28&#40;teger&#41;-319&#40;turpis&#41;-320&#40;n&#41;28&#40;unc,&#41;-323&#40;v&#41;57&#40;arius&#41;-319&#40;ac&#41;-320&#40;p&#41;-29&#40;osuere&#41;]TJ&#10;1 0 0 1 0 2605.279 Tm [&#40;consequat,&#41;-332&#40;molestie&#41;-332&#40;sed&#41;-332&#40;felis.&#41;-444&#40;F&#41;84&#40;usce&#41;-331&#40;cursus&#41;-332&#40;v&#41;28&#40;elit&#41;-331&#40;eu&#41;-332&#40;magna&#41;-332&#40;p&#41;-29&#40;ellen&#41;28&#40;tesque&#41;-331&#40;p&#41;-29&#40;osuere&#41;]TJ&#10;1 0 0 1 0 2593.324 Tm [&#40;sed&#41;-333&#40;eget&#41;-333&#40;ex.&#41;-445&#40;Viv&#41;55&#40;am&#41;28&#40;us&#41;-333&#40;in&#41;-333&#40;gra&#41;27&#40;vida&#41;-333&#40;quam,&#41;-333&#40;in&#41;-333&#40;v&#41;27&#40;olutpat&#41;-333&#40;erat.&#41;]TJ&#10;/F18 11.95517 Tf&#10;1 0 0 1 -0.672 2565.436 Tm [&#40;1.2&#41;-1125&#40;Subsection&#41;-375&#40;2&#41;]TJ&#10;/F48 9.96264 Tf&#10;1 0 0 1 -0.573 2547.047 Tm [&#40;1.2.1&#41;-1149&#40;Subsubsection&#41;-384&#40;1&#41;]TJ&#10;/F16 9.96264 Tf&#10;0.98 0 0 1 0 2528.657 Tm [&#40;Susp&#41;-29&#40;endisse&#41;-290&#40;erat&#41;-290&#40;est,&#41;-300&#40;imp&#41;-29&#40;erdiet&#41;-291&#40;sed&#41;-290&#40;dolor&#41;-290&#40;at,&#41;-300&#40;sagittis&#41;-291&#40;lob&#41;-29&#40;ortis&#41;-290&#40;tortor.&#41;-437&#40;Nulla&#41;-290&#40;facilisi.&#41;]TJ&#10;1.02 0 0 1 -0.379 2516.702 Tm [&#40;Aliquam&#41;-356&#40;ph&#41;-1&#40;aretra&#41;-356&#40;scelerisque&#41;-357&#40;auctor.&#41;-526&#40;Duis&#41;-357&#40;v&#41;27&#40;el&#41;-356&#40;auctor&#41;-357&#40;ipsum.&#41;-525&#40;Nu&#41;-1&#40;llam&#41;-356&#40;sagittis&#41;]TJ&#10;1.003 0 0 1 0 2504.747 Tm [&#40;feugiat&#41;-331&#40;mollis.&#41;-443&#40;Aliquam&#41;-331&#40;at&#41;-332&#40;ultrices&#41;-331&#40;lib&#41;-29&#40;ero.&#41;-442&#40;Nulla&#41;-332&#40;facilisi.&#41;-443&#40;F&#41;84&#40;usce&#41;-330&#40;s&#41;-1&#40;ed&#41;-331&#40;est&#41;-332&#40;placerat,&#41;]TJ&#10;1 0 0 1 0 2492.792 Tm [&#40;fringilla&#41;-333&#40;augue&#41;-333&#40;at,&#41;-334&#40;pretium&#41;-333&#40;nisl.&#41;]TJ&#10;/F48 9.96264 Tf&#10;1 0 0 1 -0.573 2466.896 Tm [&#40;1.2.2&#41;-1149&#40;Subsubsection&#41;-384&#40;2&#41;]TJ&#10;/F16 9.96264 Tf&#10;0.986 0 0 1 0 2448.507 Tm [&#40;In&#41;-337&#40;ut&#41;-337&#40;n&#41;27&#40;unc&#41;-336&#40;lib&#41;-29&#40;ero.&#41;-450&#40;Duis&#41;-338&#40;eu&#41;-337&#40;elemen&#41;28&#40;tum&#41;-336&#40;purus&#41;-1&#40;.&#41;-450&#40;Etiam&#41;-337&#40;dictum,&#41;-338&#40;ipsum&#41;-337&#40;nec&#41;-338&#40;aliquam&#41;]TJ&#10;1.02 0 0 1 0 2436.552 Tm [&#40;lob&#41;-27&#40;ortis,&#41;-359&#40;magna&#41;-353&#40;magna&#41;-353&#40;p&#41;-27&#40;ellen&#41;27&#40;tesque&#41;-352&#40;ligula,&#41;-359&#40;sed&#41;-353&#40;ultricies&#41;-352&#40;o&#41;-28&#40;dio&#41;-353&#40;ligula&#41;-352&#40;vitae&#41;-353&#40;orci.&#41;]TJ&#10;0.98 0 0 1 0 2424.596 Tm [&#40;F&#41;86&#40;usce&#41;-329&#40;bib&#41;-29&#40;endum&#41;-331&#40;maxim&#41;28&#40;us&#41;-329&#40;ligula,&#41;-333&#40;id&#41;-330&#40;gra&#41;28&#40;vida&#41;-330&#40;felis&#41;-330&#40;dictum&#41;-331&#40;a.&#41;-450&#40;In&#41;-331&#40;dapibus&#41;-330&#40;n&#41;28&#40;ulla&#41;-330&#40;eget&#41;]TJ&#10;1.02 0 0 1 -0.259 2412.641 Tm [&#40;v&#41;27&#40;olutpat&#41;-361&#40;vulputate.&#41;-543&#40;Quisque&#41;-362&#40;congue&#41;-363&#40;erat&#41;-362&#40;quis&#41;-362&#40;nibh&#41;-363&#40;molestie,&#41;-371&#40;eget&#41;-362&#40;v&#41;54&#40;arius&#41;-361&#40;eros&#41;]TJ&#10;1 0 0 1 0 2400.686 Tm [&#40;ultrices.&#41;]TJ&#10;/F48 9.96264 Tf&#10;1.005 0 0 1 0 2374.79 Tm [&#40;Subsubsubsection&#41;]TJ&#10;/F16 9.96264 Tf&#10;1.005 0 0 1 98.591 2374.79 Tm [&#40;Proin&#41;-333&#40;eleifend&#41;-333&#40;lorem&#41;-333&#40;semp&#41;-28&#40;er,&#41;-334&#40;commo&#41;-28&#40;do&#41;-333&#40;tellus&#41;-333&#40;nec,&#41;-334&#40;p&#41;-28&#40;orta&#41;]TJ&#10;1.02 0 0 1 0 2362.835 Tm [&#40;purus.&#41;-639&#40;Nullam&#41;-395&#40;commo&#41;-28&#40;do&#41;-394&#40;lectus&#41;-395&#40;nibh,&#41;-412&#40;consequat&#41;-394&#40;maxim&#41;26&#40;us&#41;-393&#40;lorem&#41;-395&#40;faucibus&#41;-395&#40;in.&#41;]TJ&#10;1 0 0 1 0 2350.88 Tm [&#40;Nam&#41;-333&#40;purus&#41;-333&#40;eros,&#41;-334&#40;rutrum&#41;-333&#40;in&#41;-333&#40;sapien&#41;-334&#40;et,&#41;-333&#40;condimen&#41;27&#40;tum&#41;-333&#40;lacinia&#41;-333&#40;nibh.&#41;]TJ&#10;/F18 14.3462 Tf&#10;1 0 0 1 -0.404 2317.934 Tm [&#40;2&#41;-1125&#40;T&#41;31&#40;yp&#41;-31&#40;ograph&#41;31&#40;y&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 2296.114 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F48 9.96264 Tf&#10;1 0 0 1 24.907 2296.114 Tm [&#40;Bold&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 2284.158 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F50 9.96264 Tf&#10;1 0 0 1 24.907 2284.158 Tm [&#40;Italic&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 2272.203 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F51 9.96264 Tf&#10;1 0 0 1 24.907 2272.203 Tm [&#40;Bold&#41;-414&#40;italic&#41;]TJ&#10;/F16 9.96264 Tf&#10;1 0 0 1 77.292 2272.203 Tm [&#40;.&#41;]TJ&#10;/F18 14.3462 Tf&#10;1 0 0 1 -0.404 2239.257 Tm [&#40;3&#41;-1125&#40;Num&#41;31&#40;b&#41;-31&#40;ers&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 2217.437 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 2217.437 Tm [&#40;Normal:&#41;-444&#40;0123456789&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 2205.482 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 2205.482 Tm [&#40;Math:&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 55.625 2205.482 Tm [&#40;0123456789&#41;]TJ&#10;/F18 14.3462 Tf&#10;1 0 0 1 -0.565 2172.536 Tm [&#40;4&#41;-1125&#40;A&#41;31&#40;cron&#41;31&#40;yms&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 2150.715 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 2150.715 Tm [&#40;Default&#41;-333&#40;&#92;050short+long&#92;051:&#41;-444&#40;Carnegie&#41;-334&#40;Mellon&#41;-333&#40;Univ&#41;27&#40;ersit&#41;28&#40;y&#41;-333&#40;&#92;050&#41;]TJ&#10;/F54 7.97011 Tf&#10;1 0 0 1 250.173 2150.715 Tm [&#40;C&#41;-110&#40;M&#41;-111&#40;U&#41;]TJ&#10;/F16 9.96264 Tf&#10;1 0 0 1 273.23 2150.715 Tm [&#40;&#92;051&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 2138.76 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 2138.76 Tm [&#40;Rep&#41;-27&#40;eated&#41;-334&#40;&#92;050short&#92;051:&#41;]TJ&#10;/F54 7.97011 Tf&#10;1 0 0 1 105.318 2138.76 Tm [&#40;C&#41;-110&#40;M&#41;-111&#40;U&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 2126.805 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 2126.805 Tm [&#40;F&#41;83&#40;orced&#41;-332&#40;sh&#41;-1&#40;ort:&#41;]TJ&#10;/F54 7.97011 Tf&#10;1 0 0 1 85.697 2126.805 Tm [&#40;U&#41;-110&#40;S&#41;-111&#40;A&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 2114.849 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;0.98 0 0 1 24.907 2114.849 Tm [&#40;Rep&#41;-28&#40;eated&#41;-309&#40;after&#41;-308&#40;forced&#41;-309&#40;short&#41;-309&#40;&#92;050short+long&#92;051:&#41;-437&#40;United&#41;-309&#40;States&#41;-309&#40;of&#41;-308&#40;America&#41;-309&#40;&#92;050&#41;]TJ&#10;/F54 7.97011 Tf&#10;1 0 0 1 320.812 2114.849 Tm [&#40;U&#41;-110&#40;S&#41;-111&#40;A&#41;]TJ&#10;/F16 9.96264 Tf&#10;0.98 0 0 1 341.08 2114.849 Tm [&#40;&#92;051&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 2102.894 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 2102.894 Tm [&#40;Plural:&#41;-444&#40;so&#41;-28&#40;cial&#41;-333&#40;securit&#41;27&#40;y&#41;-333&#40;n&#41;27&#40;um&#41;28&#40;b&#41;-27&#40;ers&#41;-333&#40;&#92;050&#41;]TJ&#10;/F54 7.97011 Tf&#10;1 0 0 1 167.759 2102.894 Tm [&#40;S&#41;-110&#40;S&#41;-111&#40;N&#41;-110&#40;s&#41;]TJ&#10;/F16 9.96264 Tf&#10;1 0 0 1 190.94 2102.894 Tm [&#40;&#92;051&#41;]TJ&#10;/F18 14.3462 Tf&#10;1 0 0 1 0 2069.949 Tm [&#40;5&#41;-1125&#40;Math&#41;]TJ&#10;/F28 9.96264 Tf&#10;1 0 0 1 139.373 2058.547 Tm [&#40;Z&#41;]TJ&#10;/F26 6.97385 Tf&#10;1 0 0 1 149.336 2056.084 Tm [&#40;1&#41;]TJ&#10;/F20 6.97385 Tf&#10;1 0 0 1 144.908 2035.91 Tm [&#40;0&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 159.437 2044.987 Tm [&#40;exp&#41;]TJ&#10;/F26 6.97385 Tf&#10;1 0 0 1 174.658 2049.1 Tm [&#40;&#92;000&#41;]TJ&#10;/F23 6.97385 Tf&#10;1 0 0 1 180.884 2049.1 Tm [&#40;x&#41;]TJ&#10;/F21 4.98132 Tf&#10;1 0 0 1 185.402 2052.107 Tm [&#40;2&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 193.109 2044.987 Tm [&#40;d&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 198.644 2044.987 Tm [&#40;x&#41;]TJ&#10;/F16 9.96264 Tf&#10;1 0 0 1 332.146 2044.987 Tm [&#40;&#92;0501&#92;051&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 3.312 2005.136 Tm [&#40;a;&#41;-166&#40;b;&#41;-167&#40;c;&#41;-166&#40;d;&#41;-167&#40;e;&#41;-167&#40;f&#41;-52&#40;;&#41;-166&#40;g&#41;-36&#40;;&#41;-167&#40;h;&#41;-166&#40;i;&#41;-167&#40;j&#41;-2&#40;;&#41;-166&#40;k&#41;-32&#40;;&#41;-167&#40;l&#41;-19&#40;;&#41;-167&#40;m;&#41;-167&#40;n;&#41;-166&#40;o;&#41;-167&#40;p;&#41;-167&#40;q&#41;-35&#40;;&#41;-167&#40;r&#41;27&#40;;&#41;-166&#40;s;&#41;-166&#40;t;&#41;-167&#40;u;&#41;-167&#40;v&#41;-36&#40;;&#41;-166&#40;w&#41;-27&#40;;&#41;-167&#40;x;&#41;-167&#40;y&#41;-35&#40;;&#41;-167&#40;z&#41;-44&#40;;&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 250.736 2005.136 Tm [&#40;0&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 255.717 2005.136 Tm [&#40;;&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 260.145 2005.136 Tm [&#40;1&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 265.126 2005.136 Tm [&#40;;&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 269.554 2005.136 Tm [&#40;2&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 274.535 2005.136 Tm [&#40;;&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 278.963 2005.136 Tm [&#40;3&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 283.944 2005.136 Tm [&#40;;&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 288.372 2005.136 Tm [&#40;4&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 293.353 2005.136 Tm [&#40;;&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 297.781 2005.136 Tm [&#40;5&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 302.763 2005.136 Tm [&#40;;&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 307.19 2005.136 Tm [&#40;6&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 312.172 2005.136 Tm [&#40;;&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 316.6 2005.136 Tm [&#40;7&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 321.581 2005.136 Tm [&#40;;&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 326.009 2005.136 Tm [&#40;8&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 330.99 2005.136 Tm [&#40;;&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 335.418 2005.136 Tm [&#40;9&#41;]TJ&#10;/F16 9.96264 Tf&#10;1 0 0 1 332.146 1993.181 Tm [&#40;&#92;0502&#92;051&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 1969.899 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 1969.899 Tm [&#40;Inline:&#41;]TJ&#10;/F28 9.96264 Tf&#10;1 0 0 1 56.731 1977.925 Tm [&#40;R&#41;]TJ&#10;/F26 6.97385 Tf&#10;1 0 0 1 63.373 1975.462 Tm [&#40;1&#41;]TJ&#10;/F20 6.97385 Tf&#10;1 0 0 1 61.436 1966.357 Tm [&#40;0&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 73.474 1969.899 Tm [&#40;exp&#41;]TJ&#10;/F26 6.97385 Tf&#10;1 0 0 1 88.695 1973.515 Tm [&#40;&#92;000&#41;]TJ&#10;/F23 6.97385 Tf&#10;1 0 0 1 94.922 1973.515 Tm [&#40;x&#41;]TJ&#10;/F21 4.98132 Tf&#10;1 0 0 1 99.439 1976.521 Tm [&#40;2&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 107.147 1969.899 Tm [&#40;d&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 112.681 1969.899 Tm [&#40;x&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 1957.944 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 1957.944 Tm [&#40;Blo&#41;-27&#40;c&#41;27&#40;k:&#41;-444&#40;Equation&#41;-333&#40;1,&#41;-334&#40;Equation&#41;-333&#40;2&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 1945.989 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 1945.989 Tm [&#40;Commands&#41;-333&#40;de&#92;034ned&#41;-333&#40;in&#41;-334&#40;b&#41;-28&#40;o&#41;-27&#40;dy&#41;-334&#40;&#92;050P[x&#41;-333&#40;in&#41;-333&#40;X]&#92;051:&#41;]TJ&#10;/F34 9.96264 Tf&#10;1 0 0 1 201.936 1945.989 Tm [&#40;P&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 208.523 1945.989 Tm [&#40;[&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 211.29 1945.989 Tm [&#40;x&#41;]TJ&#10;/F25 9.96264 Tf&#10;1 0 0 1 219.751 1945.989 Tm [&#40;2&#41;-277&#40;X&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 237.726 1945.989 Tm [&#40;]&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 1934.034 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.528 1934.034 Tm [&#40;Aligned:&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 172.228 1902.751 Tm [&#40;x&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 180.689 1902.751 Tm [&#40;=&#41;-277&#40;1&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 154.81 1887.807 Tm [&#40;x&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 162.717 1887.807 Tm [&#40;+&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 172.68 1887.807 Tm [&#40;y&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 180.689 1887.807 Tm [&#40;=&#41;-277&#40;10&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 137.562 1872.863 Tm [&#40;x&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 145.47 1872.863 Tm [&#40;+&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 155.432 1872.863 Tm [&#40;y&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 162.888 1872.863 Tm [&#40;+&#41;]TJ&#10;/F22 9.96264 Tf&#10;1 0 0 1 172.851 1872.863 Tm [&#40;z&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 180.689 1872.863 Tm [&#40;=&#41;-277&#40;100&#41;]TJ&#10;/F18 14.3462 Tf&#10;1 0 0 1 0 1843.459 Tm [&#40;6&#41;-1125&#40;Links&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 1821.638 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 1821.638 Tm [&#40;Section:&#41;-444&#40;Section&#41;-333&#40;1,&#41;-334&#40;Section&#41;-333&#40;1.2&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 1809.683 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.528 1809.683 Tm [&#40;App&#41;-27&#40;endix&#41;-334&#40;section:&#41;-444&#40;Section&#41;]TJ&#10;/F48 9.96264 Tf&#10;1 0 0 1 142.198 1809.683 Tm [&#40;??&#41;]TJ&#10;/F16 9.96264 Tf&#10;1 0 0 1 153.019 1809.683 Tm [&#40;,&#41;-333&#40;Section&#41;]TJ&#10;/F48 9.96264 Tf&#10;1 0 0 1 193.976 1809.683 Tm [&#40;??&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 1797.728 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.528 1797.728 Tm [&#40;App&#41;-27&#40;endix&#41;-334&#40;&#92;034gure:&#41;-444&#40;Figure&#41;]TJ&#10;/F48 9.96264 Tf&#10;1 0 0 1 133.204 1797.728 Tm [&#40;??&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 1785.773 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.528 1785.773 Tm [&#40;App&#41;-27&#40;endix&#41;-334&#40;table:&#41;-444&#40;T&#41;82&#40;able&#41;]TJ&#10;/F48 9.96264 Tf&#10;1 0 0 1 126.368 1785.773 Tm [&#40;??&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 1773.817 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.528 1773.817 Tm [&#40;App&#41;-27&#40;endix&#41;-334&#40;math:&#41;-444&#40;Equation&#41;]TJ&#10;/F48 9.96264 Tf&#10;1 0 0 1 143.111 1773.817 Tm [&#40;??&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 1761.862 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 1761.862 Tm [&#40;Short&#41;-333&#40;citation&#41;]TJ&#10;/F56 6.97385 Tf&#10;1 0 0 1 86.26 1765.478 Tm [&#40;[1]&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 1749.907 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 1749.907 Tm [&#40;Long&#41;-333&#40;citation:&#41;-444&#40;Mittelbac&#41;27&#40;h&#41;-333&#40;et&#41;-333&#40;al.&#41;-383&#40;&#92;0502004&#41;-50&#40;&#92;051&#41;]TJ&#10;/F56 6.97385 Tf&#10;1 0 0 1 195.85 1753.522 Tm [&#40;[1]&#41;]TJ&#10;/F16 9.96264 Tf&#10;1 0 0 1 204.83 1749.907 Tm [&#40;,&#41;-333&#40;Lesk&#41;-333&#40;and&#41;-334&#40;Kernighan&#41;-383&#40;&#92;0501977&#41;-50&#40;&#92;051&#41;]TJ&#10;/F56 6.97385 Tf&#10;1 0 0 1 331.854 1753.522 Tm [&#40;[2]&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 1737.952 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 1737.952 Tm [&#40;Multi&#41;-333&#40;citation&#41;]TJ&#10;/F56 6.97385 Tf&#10;1 0 0 1 86.509 1741.567 Tm [&#40;[1&#92;0253]&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 1725.997 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 1725.997 Tm [&#40;P&#41;27&#40;oin&#41;28&#40;ter&#41;-332&#40;to&#41;-334&#40;fo&#41;-27&#40;otnote&#41;]TJ&#10;/F57 6.97385 Tf&#10;1 0 0 1 108.095 1729.612 Tm [&#40;a&#41;]TJ&#10;/F18 14.3462 Tf&#10;1 0 0 1 -0.404 1693.051 Tm [&#40;7&#41;-1125&#40;T&#41;93&#40;ables&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 1671.23 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.548 1671.23 Tm [&#40;T&#41;83&#40;able&#41;-333&#40;1&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 1659.275 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.548 1659.275 Tm [&#40;T&#41;83&#40;able&#41;-333&#40;2&#41;]TJ&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;ET&#10;q&#10;1 0 0 1 112.412 1647.918 cm&#10;[] 0 d 0 J 0.797 w 0 0 m 115.566 0 l S&#10;Q&#10;BT&#10;/F16 9.96264 Tf&#10;1 0 0 1 112.412 1636.36 Tm [&#40;Col1&#41;-1200&#40;Col2&#41;-1200&#40;Col3&#41;-1200&#40;Col4&#41;]TJ&#10;ET&#10;q&#10;1 0 0 1 112.412 1630.806 cm&#10;[] 0 d 0 J 0.498 w 0 0 m 115.566 0 l S&#10;Q&#10;BT&#10;/F16 9.96264 Tf&#10;1 0 0 1 112.412 1619.398 Tm [&#40;1&#41;-4200&#40;2&#41;-1950&#40;3&#41;-1950&#40;4&#41;]TJ&#10;1 0 0 1 112.412 1607.443 Tm [&#40;11&#41;-3200&#40;22&#41;-1700&#40;33&#41;-1700&#40;44&#41;]TJ&#10;1 0 0 1 112.412 1595.487 Tm [&#40;111&#41;-2200&#40;222&#41;-1450&#40;333&#41;-1450&#40;444&#41;]TJ&#10;ET&#10;q&#10;1 0 0 1 112.412 1589.785 cm&#10;[] 0 d 0 J 0.797 w 0 0 m 115.566 0 l S&#10;Q&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;BT&#10;/F16 9.96264 Tf&#10;1 0 0 1 -0.359 1571.055 Tm [&#40;T&#41;83&#40;able&#41;-333&#40;1:&#41;-444&#40;Short&#41;-333&#40;table&#41;]TJ&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;ET&#10;q&#10;1 0 0 1 13.616 1556.111 cm&#10;[] 0 d 0 J 0.797 w 0 0 m 313.158 0 l S&#10;Q&#10;BT&#10;/F16 9.96264 Tf&#10;1 0 0 1 14.115 1544.553 Tm [&#40;Col1&#41;-1200&#40;Col2&#41;-1200&#40;Col3&#41;-1199&#40;Col4&#41;-1200&#40;Col5&#41;-1284&#40;Col6&#41;-1200&#40;Col7&#41;-1200&#40;Col8&#41;-1200&#40;Col9&#41;-1200&#40;Col10&#41;]TJ&#10;ET&#10;q&#10;1 0 0 1 13.616 1539 cm&#10;[] 0 d 0 J 0.498 w 0 0 m 313.158 0 l S&#10;Q&#10;BT&#10;/F16 9.96264 Tf&#10;1 0 0 1 29.059 1527.591 Tm [&#40;a&#41;-2700&#40;1&#41;-2699&#40;2&#41;-2700&#40;3&#41;-1700&#40;123&#41;-1200&#40;ab&#41;-28&#40;cd&#41;-1200&#40;1234&#41;-1700&#40;444&#41;-1700&#40;555&#41;-2200&#40;666&#41;]TJ&#10;1 0 0 1 28.505 1515.636 Tm [&#40;b&#41;-2200&#40;11&#41;-2200&#40;22&#41;-2200&#40;33&#41;-1700&#40;456&#41;-1477&#40;efgh&#41;-1700&#40;567&#41;-2200&#40;44&#41;-2200&#40;55&#41;-2700&#40;66&#41;]TJ&#10;/F48 9.96264 Tf&#10;1 0 0 1 13.616 1491.726 Tm [&#40;Mid&#41;]TJ&#10;/F16 9.96264 Tf&#10;1 0 0 1 29.612 1479.77 Tm [&#40;c&#41;-1699&#40;111&#41;-1700&#40;222&#41;-1700&#40;333&#41;-1700&#40;789&#41;-1895&#40;ijkl&#41;-2200&#40;89&#41;-2700&#40;4&#41;-2700&#40;5&#41;-3200&#40;6&#41;]TJ&#10;ET&#10;q&#10;1 0 0 1 13.616 1474.068 cm&#10;[] 0 d 0 J 0.797 w 0 0 m 313.158 0 l S&#10;Q&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;BT&#10;/F16 9.96264 Tf&#10;1 0 0 1 -0.359 1455.338 Tm [&#40;T&#41;83&#40;able&#41;-333&#40;2:&#41;-444&#40;Wide&#41;-333&#40;table&#41;]TJ&#10;0 g 0 G&#10;/F18 14.3462 Tf&#10;1 0 0 1 0 1422.392 Tm [&#40;8&#41;-1125&#40;Figures&#41;]TJ&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;ET&#10;q&#10;1 0 0 1 68.815 1199.139 cm&#10;/Im4 Do&#10;Q&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;q&#10;1 0 0 1 0 1192.963 cm&#10;[] 0 d 0 J 0.398 w 0 0 m 137.482 0 l S&#10;Q&#10;BT&#10;/F57 5.97758 Tf&#10;1 0 0 1 13.829 1186.361 Tm [&#40;a&#41;]TJ&#10;/F58 7.97011 Tf&#10;1 0 0 1 17.933 1183.548 Tm [&#40;Example&#41;-354&#40;fo&#41;-29&#40;otnote&#41;-354&#40;text.&#41;]TJ&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 0 1154.407 Tm [&#40;Figure&#41;-333&#40;2:&#41;-444&#40;Narro&#41;27&#40;w&#41;-333&#40;&#92;034gure&#41;]TJ&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;ET&#10;1 0 0 1 0 909.319 cm&#10;q&#10;.95476 0 0 .95476 0 0 cm&#10;0 g 0 G&#10;q&#10;.95241 0 0 .95241 0 0 cm&#10;0 g 0 G&#10;q&#10;1 0 0 1 0 0 cm&#10;/Im5 Do&#10;Q&#10;0 g 0 G&#10;Q&#10;0 g 0 G&#10;Q&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;1 0 0 1 0 -909.319 cm&#10;BT&#10;/F16 9.96264 Tf&#10;1 0 0 1 0 871.063 Tm [&#40;Figure&#41;-333&#40;3:&#41;-444&#40;Wide&#41;-334&#40;&#92;034gure&#41;]TJ&#10;0 g 0 G&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 849.145 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 849.145 Tm [&#40;Figure&#41;-333&#40;2&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 837.19 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 837.19 Tm [&#40;Figure&#41;-333&#40;3&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 825.235 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 825.235 Tm [&#40;Figure&#41;-333&#40;4,&#41;-333&#40;Figure&#41;-333&#40;3a,&#41;-334&#40;Figure&#41;-333&#40;3b&#41;]TJ&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;ET&#10;1 0 0 1 81.851 629.286 cm&#10;q&#10;.83337 0 0 .83337 0 0 cm&#10;0 g 0 G&#10;q&#10;1 0 0 1 0 0 cm&#10;/Im1 Do&#10;Q&#10;0 g 0 G&#10;Q&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;1 0 0 1 -81.851 -629.286 cm&#10;BT&#10;/F16 9.96264 Tf&#10;1 0 0 1 81.851 610.955 Tm [&#40;a:&#41;-444&#40;Figure&#41;-333&#40;with&#41;-334&#40;`width=2.5in&#39;&#41;]TJ&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;ET&#10;1 0 0 1 42.535 354.373 cm&#10;q&#10;.875 0 0 .875 0 0 cm&#10;0 g 0 G&#10;q&#10;1 0 0 1 0 0 cm&#10;/Im3 Do&#10;Q&#10;0 g 0 G&#10;Q&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;1 0 0 1 -42.535 -354.373 cm&#10;BT&#10;/F16 9.96264 Tf&#10;1 0 0 1 42.535 336.041 Tm [&#40;b:&#41;-444&#40;Figure&#41;-333&#40;with&#41;-334&#40;`width=3.5in&#39;&#41;]TJ&#10;/F57 6.97385 Tf&#10;1 0 0 1 168.617 339.657 Tm [&#40;a&#41;]TJ&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 0 306.103 Tm [&#40;Figure&#41;-333&#40;4:&#41;-444&#40;Sub-&#92;034gu&#41;-1&#40;res&#41;]TJ&#10;/F57 6.97385 Tf&#10;1 0 0 1 91.85 309.718 Tm [&#40;b&#41;]TJ&#10;0 g 0 G&#10;/F18 14.3462 Tf&#10;1 0 0 1 0 273.157 Tm [&#40;9&#41;-1125&#40;Includes&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 251.336 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 251.336 Tm [&#40;Commands&#41;-333&#40;from&#41;-333&#40;metadata&#41;-334&#40;include:&#41;]TJ&#10;/F19 9.96264 Tf&#10;1 0 0 1 183.007 251.336 Tm [&#40;arg&#41;-180&#40;min&#41;]TJ&#10;/F34 9.96264 Tf&#10;1 0 0 1 218.595 251.336 Tm [&#40;R&#41;]TJ&#10;0 g 0 G&#10;/F49 9.96264 Tf&#10;1 0 0 1 12.176 239.381 Tm [&#40;&#92;210&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 24.907 239.381 Tm [&#40;Include&#41;-333&#40;command&#41;-333&#40;in&#41;-334&#40;b&#41;-27&#40;o&#41;-28&#40;dy&#41;-334&#40;&#92;050there&#41;-333&#40;should&#41;-333&#40;b&#41;-28&#40;e&#41;-333&#40;text&#41;-334&#40;after&#41;-333&#40;this&#92;051:&#41;]TJ&#10;1 0 0 1 0 217.463 Tm [&#40;Con&#41;27&#40;ten&#41;28&#40;t&#41;-332&#40;added&#41;-334&#40;through&#41;-333&#40;include&#41;-334&#40;statemen&#41;27&#40;t.&#41;]TJ&#10;/F18 14.3462 Tf&#10;1 0 0 1 0 174.499 Tm [&#40;References&#41;]TJ&#10;0 g 0 G&#10;/F16 9.96264 Tf&#10;1 0 0 1 0 152.679 Tm [&#40;[1]&#41;]TJ&#10;0 g 0 G&#10;1.02 0 0 1 15.497 152.679 Tm [&#40;F&#41;83&#40;rank&#41;-338&#40;Mittelbac&#41;27&#40;h,&#41;-341&#40;Mic&#41;27&#40;hel&#41;-338&#40;Gossens,&#41;-342&#40;Johannes&#41;-339&#40;Braams,&#41;-341&#40;Da&#41;27&#40;vid&#41;-338&#40;Carlisle,&#41;-342&#40;and&#41;]TJ&#10;0.98 0 0 1 15.497 140.723 Tm [&#40;Chris&#41;-269&#40;Ro&#41;28&#40;wley&#41;87&#40;.&#41;]TJ&#10;/F50 9.96264 Tf&#10;0.98 0 0 1 77.185 140.723 Tm [&#40;The&#41;-299&#40;L&#41;]TJ&#10;/F57 6.97385 Tf&#10;1 0 0 1 99.038 142.782 Tm [&#40;A&#41;]TJ&#10;/F50 9.96264 Tf&#10;0.98 0 0 1 103.549 140.723 Tm [&#40;T&#41;]TJ&#10;1 0 0 1 108.837 138.579 Tm [&#40;E&#41;]TJ&#10;0.98 0 0 1 114.323 140.723 Tm [&#40;X&#41;-299&#40;Comp&#41;52&#40;anion&#41;]TJ&#10;/F16 9.96264 Tf&#10;0.98 0 0 1 172.892 140.723 Tm [&#40;.&#41;-336&#40;A&#41;28&#40;ddison-W&#41;86&#40;esley&#41;-268&#40;Professional,&#41;-284&#40;2&#41;-269&#40;edition,&#41;]TJ&#10;1 0 0 1 15.248 128.768 Tm [&#40;2004.&#41;]TJ&#10;0 g 0 G&#10;1 0 0 1 0 108.843 Tm [&#40;[2]&#41;]TJ&#10;0 g 0 G&#10;1.02 0 0 1 15.497 108.843 Tm [&#40;Mic&#41;27&#40;hael&#41;-465&#40;Lesk&#41;-466&#40;and&#41;-466&#40;Brian&#41;-466&#40;Kernighan.&#41;-850&#40;Computer&#41;-466&#40;t&#41;27&#40;yp&#41;-27&#40;esetting&#41;-466&#40;of&#41;-466&#40;tec&#41;27&#40;hnical&#41;]TJ&#10;1.02 0 0 1 15.497 96.888 Tm [&#40;journals&#41;-346&#40;on&#41;-347&#40;UNIX.&#41;-494&#40;In&#41;]TJ&#10;/F50 9.96264 Tf&#10;1.02 0 0 1 115.846 96.888 Tm [&#40;Pr&#41;51&#40;o&#41;51&#40;c&#41;51&#40;e&#41;51&#40;e&#41;51&#40;dings&#41;-368&#40;of&#41;-369&#40;A&#41;50&#40;meric&#41;52&#40;an&#41;-369&#40;F&#41;76&#40;e&#41;51&#40;der&#41;51&#40;a&#41;1&#40;tion&#41;-369&#40;of&#41;-368&#40;I&#41;-1&#40;nformation&#41;]TJ&#10;1.02 0 0 1 14.947 84.933 Tm [&#40;Pr&#41;51&#40;o&#41;51&#40;c&#41;51&#40;essing&#41;-355&#40;So&#41;50&#40;cieties:&#41;-460&#40;1977&#41;-356&#40;National&#41;-356&#40;Computer&#41;-355&#40;Confer&#41;50&#40;enc&#41;51&#40;e&#41;]TJ&#10;/F16 9.96264 Tf&#10;1.02 0 0 1 272.785 84.933 Tm [&#40;,&#41;-333&#40;pages&#41;-332&#40;879&#92;025888,&#41;]TJ&#10;1 0 0 1 15.497 72.977 Tm [&#40;Dallas,&#41;-333&#40;T&#41;83&#40;exas,&#41;-333&#40;1977.&#41;]TJ&#10;0 g 0 G&#10;1 0 0 1 0 53.052 Tm [&#40;[3]&#41;]TJ&#10;0 g 0 G&#10;1.02 0 0 1 15.497 53.052 Tm [&#40;Donald&#41;-379&#40;E.&#41;-380&#40;Kn&#41;27&#40;uth.&#41;-591&#40;Literate&#41;-379&#40;programming.&#41;]TJ&#10;/F50 9.96264 Tf&#10;1.02 0 0 1 209.53 53.052 Tm [&#40;The&#41;-399&#40;Computer&#41;-399&#40;Journal&#41;]TJ&#10;/F16 9.96264 Tf&#10;1.02 0 0 1 312.313 53.052 Tm [&#40;,&#41;-392&#40;27&#92;0502&#92;051:&#41;]TJ&#10;1 0 0 1 15.497 41.097 Tm [&#40;97&#92;025111,&#41;-333&#40;1984.&#41;]TJ&#10;0 g 0 G&#10;ET&#10;q&#10;1 0 0 1 0 23.02 cm&#10;[] 0 d 0 J 0.398 w 0 0 m 137.482 0 l S&#10;Q&#10;BT&#10;/F57 5.97758 Tf&#10;1 0 0 1 13.829 16.418 Tm [&#40;a&#41;]TJ&#10;/F58 7.97011 Tf&#10;1 0 0 1 17.933 13.606 Tm [&#40;F&#41;88&#40;o&#41;-28&#40;otnote&#41;-355&#40;in&#41;-354&#40;sub-&#92;034gure&#41;-354&#40;caption.&#41;]TJ&#10;/F57 5.97758 Tf&#10;1 0 0 1 14.18 6.648 Tm [&#40;b&#41;]TJ&#10;/F58 7.97011 Tf&#10;1 0 0 1 17.933 3.836 Tm [&#40;F&#41;88&#40;o&#41;-28&#40;otnote&#41;-355&#40;in&#41;-354&#40;&#92;034gure&#41;-354&#40;caption.&#41;]TJ&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;0 g 0 G&#10;ET&#10;</data>
 </stream>
 </object>
 
 <object id="87">
 <dict size="1">
 <key>D</key>
 <value><list size="5">
@@ -1740,41 +1740,41 @@
 
 <object id="92">
 <dict size="1">
 <key>D</key>
 <value><list size="5">
 <ref id="58" />
 <literal>XYZ</literal>
-<number>22.867</number>
+<number>21.206</number>
 <number>3052.54</number>
 <keyword>b'null'</keyword>
 </list></value>
 </dict>
 </object>
 
 <object id="93">
 <dict size="1">
 <key>D</key>
 <value><list size="5">
 <ref id="58" />
 <literal>XYZ</literal>
-<number>176.837</number>
+<number>178.497</number>
 <number>3052.54</number>
 <keyword>b'null'</keyword>
 </list></value>
 </dict>
 </object>
 
 <object id="94">
 <dict size="1">
 <key>D</key>
 <value><list size="5">
 <ref id="58" />
 <literal>XYZ</literal>
-<number>98.195</number>
+<number>96.535</number>
 <number>2885.619</number>
 <keyword>b'null'</keyword>
 </list></value>
 </dict>
 </object>
 
 <object id="95">
@@ -2521,15 +2521,15 @@
 
 <object id="143">
 <dict size="1">
 <key>D</key>
 <value><list size="5">
 <ref id="58" />
 <literal>XYZ</literal>
-<number>44.195</number>
+<number>42.535</number>
 <number>612.35</number>
 <keyword>b'null'</keyword>
 </list></value>
 </dict>
 </object>
 
 <object id="144">
@@ -4671,18 +4671,18 @@
 <key>N</key>
 <value><number>100</number></value>
 <key>First</key>
 <value><number>874</number></value>
 <key>Filter</key>
 <value><literal>FlateDecode</literal></value>
 <key>Length</key>
-<value><number>3426</number></value>
+<value><number>3425</number></value>
 </dict>
 </props>
-<data size="13627">107 0 30 41 109 81 34 122 110 163 112 209 113 256 114 302 38 343 115 384&#10;116 431 123 478 124 523 127 568 42 609 130 650 46 691 131 732 132 773 133 818&#10;134 859 135 905 50 946 136 987 137 1028 139 1074 140 1120 141 1161 142 1206 143 1251&#10;144 1295 145 1340 54 1380 146 1420 147 1460 148 1500 149 1540 150 1579 85 1618 1 2039&#10;2 2044 3 2049 226 2087 229 2103 230 2380 231 2463 232 2636 233 2725 234 2742 235 2975&#10;236 2984 237 2993 238 3002 239 3114 240 3143 241 3276 242 3507 243 3642 245 3907 246 3916&#10;247 4126 248 4576 249 4870 251 5101 253 5390 255 5595 257 5926 259 6131 261 6337 263 6553&#10;265 6773 267 7056 269 7418 271 7662 273 7899 275 8444 277 8710 279 9001 281 9329 283 9553&#10;228 9758 244 10175 117 10226 122 10352 120 10479 108 10606 121 10732 119 10856 126 10980 118 11106&#10;99 11230 90 11383 106 11536 111 11695 91 11855 128 12011 138 12165 105 12320 129 12475 125 12628&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 2262.241 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 2257.19 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 2195.519 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 2190.469 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 123.648 2162.67 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 206.216 2126.805 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 58.835 2114.849 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 2090.441 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 2085.391 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 139.373 2056.942 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 139.373 2044.987 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 3.312 2017.091 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 3.312 2005.136 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 1863.299 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 1854.264 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 1716.034 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 1710.984 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 1649.312 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 39.215 1583.01 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 1557.506 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 39.215 1467.293 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 1441.789 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 1436.738 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 1398.579 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 17.933 1193.012 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 43.614 1166.362 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 1138.467 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 43.614 883.018 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 81.851 815.272 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 44.195 612.35 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 43.614 318.058 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 292.553 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 287.503 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 192.432 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 164.634 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 120.798 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 65.007 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 20.231 null ] &#62;&#62;&#10;&#60;&#60;  /ColorSpace 3 0 R /Pattern 2 0 R /ExtGState 1 0 R  /Font &#60;&#60; /F18 90 0 R /F16 91 0 R /F48 99 0 R /F49 104 0 R /F50 105 0 R /F51 106 0 R /F19 108 0 R /F54 111 0 R /F28 117 0 R /F26 118 0 R /F20 119 0 R /F23 120 0 R /F21 121 0 R /F22 122 0 R /F34 125 0 R /F25 126 0 R /F56 128 0 R /F57 129 0 R /F58 138 0 R &#62;&#62; /XObject &#60;&#60; /Im1 59 0 R /Im2 60 0 R /Im3 61 0 R /Im4 74 0 R /Im5 75 0 R &#62;&#62; /ProcSet [ /PDF /Text /ImageC ] &#62;&#62;&#10;&#60;&#60;&#62;&#62;&#10;&#60;&#60;&#62;&#62;&#10;&#60;&#60;  /pgfprgb [/Pattern /DeviceRGB] &#62;&#62;&#10;[ 58 0 R /Fit ]&#10;[590.3 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 354.2 295.1 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 722.6 693.1 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 531.3 590.3 472.2 0 472.2 324.7 531.3 0 295.1 0 0 295.1 885.4 590.3 531.3 590.3 0 414.1 419.1 413.2 590.3 0 0 560.7 ]&#10;[865.9 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 603.2 544.4 ]&#10;[569.4 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 569.4 569.4 569.4 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 323.4 0 323.4 ]&#10;[666.7 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 713.3 ]&#10;[611.1 0 722.2 ]&#10;[277.8 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 528.6 429.2 432.8 520.5 465.6 489.6 477 576.2 344.5 411.8 520.6 298.4 878 600.2 484.7 503.1 446.4 451.2 468.8 361.1 572.5 484.7 715.9 571.5 490.3 465 ]&#10;[680.6 ]&#10;[647.8 ]&#10;[569.4 ]&#10;[892.9 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 1138.9 ]&#10;[472.2 0 0 0 0 0 0 0 555.6 ]&#10;[813.9 0 786.1 0 0 0 0 0 0 0 0 0 988.9 813.9 0 0 0 0 611.1 0 813.9 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 457.8 ]&#10;[777.8 0 0 0 0 500 500 500 500 500 500 500 500 500 500 0 0 0 777.8 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 277.8 0 277.8 0 0 0 500 0 0 555.6 444.4 0 500 0 277.8 0 0 0 833.3 555.6 0 555.6 0 391.7 0 0 0 0 0 527.8 ]&#10;[816.7 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 591.1 0 532.2 591.1 0 0 0 0 355.5 0 0 296.7 0 0 591.1 0 0 0 0 385 ]&#10;[511.1 0 0 0 0 0 511.1 0 511.1 306.7 0 0 0 0 0 0 743.3 0 715.6 0 678.3 652.8 0 0 385.5 525 0 627.2 0 743.3 0 678.3 0 0 562.2 715.6 0 0 0 743.3 0 0 0 0 0 0 0 0 511.1 0 460 511.1 460 306.7 460 511.1 306.7 0 0 255.5 817.8 562.2 511.1 511.1 0 421.7 408.9 332.2 536.7 ]&#10;[777.8 ]&#10;[319.5 0 0 575 575 0 0 0 0 0 0 0 0 0 0 0 0 543 0 0 818 0 0 0 0 0 0 0 0 0 0 1091.7 0 0 0 0 0 638.9 0 0 0 0 0 0 0 0 0 0 0 0 0 0 638.9 511.1 638.9 527.1 0 0 0 319.5 0 0 319.5 0 638.9 575 0 0 0 453.6 447.2 638.9 ]&#10;[500 0 0 0 0 0 0 555.5 0 0 0 0 0 0 0 0 0 0 277.8 388.9 388.9 0 777.8 277.8 333.3 277.8 0 500 500 500 500 500 500 500 500 500 500 277.8 0 0 777.8 0 0 0 750 708.3 722.2 763.9 680.5 652.8 784.7 0 361.1 513.9 777.8 625 916.7 750 0 680.5 777.8 736.1 555.5 722.2 750 750 1027.8 750 0 0 277.8 0 277.8 0 0 277.8 500 555.5 444.5 555.5 444.5 305.5 500 555.5 277.8 305.5 527.8 277.8 833.3 555.5 500 555.5 527.8 391.7 394.4 388.9 555.5 527.8 722.2 527.8 527.8 ]&#10;[312.5 0 0 562.5 562.5 562.5 562.5 562.5 562.5 562.5 562.5 562.5 0 0 0 0 0 0 0 849.5 0 0 0 0 707.2 0 0 419 0 0 675.9 1067.2 879.6 0 0 0 839.2 625 782.4 0 0 0 0 0 0 0 0 0 0 0 0 546.9 625 500 625 513.3 343.7 562.5 625 312.5 0 593.7 312.5 937.5 625 562.5 625 0 459.5 443.7 437.5 625 0 0 0 593.7 ]&#10;&#60;&#60; /Type /FontDescriptor /FontName /JCFPGD+CMEX10 /Flags 4 /FontBBox [ -24 -2960 1454 772 ] /Ascent 40 /CapHeight 0 /Descent -600 /ItalicAngle 0 /StemV 47 /XHeight 431 /CharSet&#40; /integraldisplay /integraltext&#41; /FontFile 250 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /XSTMCN+CMMI10 /Flags 4 /FontBBox [ -32 -250 1048 750 ] /Ascent 694 /CapHeight 683 /Descent -194 /ItalicAngle -14 /StemV 72 /XHeight 431 /CharSet&#40; /a /b /c /comma /d /e /f /g /h /i /j /k /l /m /n /o /p /q /r /s /t /u /v /w /x /y /z&#41; /FontFile 252 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /QXILPS+CMMI7 /Flags 4 /FontBBox [ -1 -250 1171 750 ] /Ascent 694 /CapHeight 683 /Descent -194 /ItalicAngle -14 /StemV 81 /XHeight 431 /CharSet&#40; /x&#41; /FontFile 254 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /IKPMKY+CMR10 /Flags 4 /FontBBox [ -40 -250 1009 750 ] /Ascent 694 /CapHeight 683 /Descent -194 /ItalicAngle 0 /StemV 69 /XHeight 431 /CharSet&#40; /a /bracketleft /bracketright /d /e /eight /equal /five /four /g /i /m /n /nine /one /p /plus /r /seven /six /three /two /x /zero&#41; /FontFile 256 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /THGOAZ+CMR5 /Flags 4 /FontBBox [ -10 -250 1304 750 ] /Ascent 694 /CapHeight 680 /Descent -194 /ItalicAngle 0 /StemV 89 /XHeight 431 /CharSet&#40; /two&#41; /FontFile 258 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /REOFEC+CMR7 /Flags 4 /FontBBox [ -27 -250 1122 750 ] /Ascent 694 /CapHeight 683 /Descent -194 /ItalicAngle 0 /StemV 79 /XHeight 431 /CharSet&#40; /zero&#41; /FontFile 260 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /KZGXGZ+CMSY10 /Flags 4 /FontBBox [ -29 -960 1116 775 ] /Ascent 750 /CapHeight 683 /Descent -194 /ItalicAngle -14 /StemV 40 /XHeight 431 /CharSet&#40; /X /element&#41; /FontFile 262 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /XNLILI+CMSY7 /Flags 4 /FontBBox [ -15 -951 1251 782 ] /Ascent 750 /CapHeight 683 /Descent -194 /ItalicAngle -14 /StemV 49 /XHeight 431 /CharSet&#40; /infinity /minus&#41; /FontFile 264 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /JNKRSO+LMRoman10-Bold /Flags 4 /FontBBox [ -486 -295 1607 1133 ] /Ascent 699 /CapHeight 699 /Descent -194 /ItalicAngle 0 /StemV 114 /XHeight 444 /CharSet&#40; /B /M /S /b /c /d /e /i /l /n /o /one /period /question /s /t /two /u&#41; /FontFile 266 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /ESECFF+LMRoman12-Bold /Flags 4 /FontBBox [ -476 -289 1577 1137 ] /Ascent 684 /CapHeight 684 /Descent -194 /ItalicAngle 0 /StemV 109 /XHeight 444 /CharSet&#40; /A /F /I /L /M /N /R /S /T /a /b /c /d /e /eight /f /five /four /g /h /i /k /l /m /n /nine /o /one /p /period /r /s /seven /six /t /three /two /u /y&#41; /FontFile 268 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /DMGJGY+LMRoman10-BoldItalic /Flags 4 /FontBBox [ -518 -307 1565 1147 ] /Ascent 700 /CapHeight 700 /Descent -194 /ItalicAngle -14 /StemV 96 /XHeight 444 /CharSet&#40; /B /a /c /d /i /l /o /t&#41; /FontFile 270 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /MRRRNS+LMRomanCaps10-Regular /Flags 4 /FontBBox [ -496 -290 1501 1100 ] /Ascent 527 /CapHeight 689 /Descent 0 /ItalicAngle 0 /StemV 89 /XHeight 431 /CharSet&#40; /A /C /M /N /S /U /s&#41; /FontFile 272 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /KIPIOQ+LMRoman10-Regular /Flags 4 /FontBBox [ -430 -290 1417 1127 ] /Ascent 0 /CapHeight 0 /Descent 0 /ItalicAngle 0 /StemV 69 /XHeight 431 /CharSet&#40; /A /B /C /D /E /F /G /I /J /K /L /M /N /P /Q /R /S /T /U /V /W /X /a /b /bracketleft /bracketright /bullet /c /colon /comma /d /e /eight /endash /equal /f /fi /five /four /g /h /hyphen /i /j /k /l /m /n /nine /o /one /p /parenleft /parenright /period /plus /q /quoteleft /quoteright /r /s /seven /six /t /three /two /u /v /w /x /y /zero&#41; /FontFile 274 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /RRPEYH+LMRoman7-Regular /Flags 4 /FontBBox [ -483 -292 1562 1124 ] /Ascent 689 /CapHeight 689 /Descent -194 /ItalicAngle 0 /StemV 79 /XHeight 431 /CharSet&#40; /bracketleft /bracketright /endash /one /three /two&#41; /FontFile 276 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /DBJOTS+LMRoman8-Regular /Flags 4 /FontBBox [ -456 -292 1497 1125 ] /Ascent 689 /CapHeight 689 /Descent -194 /ItalicAngle 0 /StemV 76 /XHeight 431 /CharSet&#40; /E /F /a /b /c /e /f /fi /g /hyphen /i /l /m /n /o /p /period /r /s /t /u /x&#41; /FontFile 278 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /QQNAVM+LMRoman10-Italic /Flags 4 /FontBBox [ -458 -290 1386 1125 ] /Ascent 689 /CapHeight 689 /Descent -194 /ItalicAngle -14 /StemV 56 /XHeight 431 /CharSet&#40; /A /C /E /F /I /J /L /N /P /S /T /X /a /c /colon /d /e /f /g /h /i /l /m /n /nine /o /one /p /r /s /seven /t /u&#41; /FontFile 280 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /RBBYWX+LMRoman7-Italic /Flags 4 /FontBBox [ -528 -292 1571 1123 ] /Ascent 689 /CapHeight 689 /Descent -194 /ItalicAngle -14 /StemV 70 /XHeight 431 /CharSet&#40; /A /a /b&#41; /FontFile 282 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /NANTFZ+MSBM10 /Flags 4 /FontBBox [ -55 -420 2343 920 ] /Ascent 464 /CapHeight 689 /Descent 0 /ItalicAngle 0 /StemV 40 /XHeight 463 /CharSet&#40; /P /R&#41; /FontFile 284 0 R &#62;&#62;&#10;&#60;&#60; /Type /Encoding /Differences [ 21 /endash 28 /fi 39 /quoteright /parenleft /parenright 43 /plus /comma /hyphen /period 48 /zero /one /two /three /four /five /six /seven /eight /nine /colon 61 /equal 63 /question 65 /A /B /C /D /E /F /G 73 /I /J /K /L /M /N 80 /P /Q /R /S /T /U /V /W /X 91 /bracketleft 93 /bracketright 96 /quoteleft /a /b /c /d /e /f /g /h /i /j /k /l /m /n /o /p /q /r /s /t /u /v /w /x /y ] &#62;&#62;&#10;&#60;&#60; /Type /Encoding /Differences [ 136 /bullet ] &#62;&#62;&#10;&#60;&#60; /Type /Font /Subtype /Type1 /BaseFont /JCFPGD+CMEX10 /FontDescriptor 249 0 R /FirstChar 82 /LastChar 90 /Widths 239 0 R &#62;&#62;&#10;&#60;&#60; /Type /Font /Subtype /Type1 /BaseFont /XSTMCN+CMMI10 /FontDescriptor 251 0 R /FirstChar 59 /LastChar 122 /Widths 234 0 R &#62;&#62;&#10;&#60;&#60; /Type /Font /Subtype /Type1 /BaseFont /QXILPS+CMMI7 /FontDescriptor 253 0 R /FirstChar 120 /LastChar 120 /Widths 236 0 R &#62;&#62;&#10;&#60;&#60; /Type /Font /Subtype /Type1 /BaseFont /IKPMKY+CMR10 /FontDescriptor 255 0 R /FirstChar 43 /LastChar 120 /Widths 241 0 R &#62;&#62;&#10;&#60;&#60; /Type /Font /Subtype /Type1 /BaseFont /THGOAZ+CMR5 /FontDescriptor 257 0 R /FirstChar 50 /LastChar 50 /Widths 235 0 R &#62;&#62;&#10;&#60;&#60; /Type /Font /Subtype /Type1 /BaseFont /REOFEC+CMR7 /FontDescriptor 259 0 R /FirstChar 48 /LastChar 48 /Widths 237 0 R &#62;&#62;&#10;&#60;&#60; /Type /Font /Subtype /Type1 /BaseFont /KZGXGZ+CMSY10 /FontDescriptor 261 0 R /FirstChar 50 /LastChar 88 /Widths 232 0 R &#62;&#62;&#10;&#60;&#60; /Type /Font /Subtype /Type1 /BaseFont /XNLILI+CMSY7 /FontDescriptor 263 0 R /FirstChar 0 /LastChar 49 /Widths 238 0 R &#62;&#62;&#10;&#60;&#60; /Type /Font /Subtype /Type1 /BaseFont /JNKRSO+LMRoman10-Bold /FontDescriptor 265 0 R /FirstChar 46 /LastChar 117 /Widths 246 0 R /Encoding 228 0 R &#62;&#62;&#10;&#60;&#60; /Type /Font /Subtype /Type1 /BaseFont /ESECFF+LMRoman12-Bold /FontDescriptor 267 0 R /FirstChar 46 /LastChar 121 /Widths 248 0 R /Encoding 228 0 R &#62;&#62;&#10;&#60;&#60; /Type /Font /Subtype /Type1 /BaseFont /DMGJGY+LMRoman10-BoldItalic /FontDescriptor 269 0 R /FirstChar 66 /LastChar 116 /Widths 242 0 R /Encoding 228 0 R &#62;&#62;&#10;&#60;&#60; /Type /Font /Subtype /Type1 /BaseFont /MRRRNS+LMRomanCaps10-Regular /FontDescriptor 271 0 R /FirstChar 65 /LastChar 115 /Widths 240 0 R /Encoding 228 0 R &#62;&#62;&#10;&#60;&#60; /Type /Font /Subtype /Type1 /BaseFont /KIPIOQ+LMRoman10-Regular /FontDescriptor 273 0 R /FirstChar 21 /LastChar 121 /Widths 247 0 R /Encoding 228 0 R &#62;&#62;&#10;&#60;&#60; /Type /Font /Subtype /Type1 /BaseFont /RRPEYH+LMRoman7-Regular /FontDescriptor 275 0 R /FirstChar 21 /LastChar 93 /Widths 231 0 R /Encoding 228 0 R &#62;&#62;&#10;&#60;&#60; /Type /Font /Subtype /Type1 /BaseFont /DBJOTS+LMRoman8-Regular /FontDescriptor 277 0 R /FirstChar 28 /LastChar 120 /Widths 229 0 R /Encoding 228 0 R &#62;&#62;&#10;&#60;&#60; /Type /Font /Subtype /Type1 /BaseFont /QQNAVM+LMRoman10-Italic /FontDescriptor 279 0 R /FirstChar 49 /LastChar 117 /Widths 243 0 R /Encoding 228 0 R &#62;&#62;&#10;&#60;&#60; /Type /Font /Subtype /Type1 /BaseFont /RBBYWX+LMRoman7-Italic /FontDescriptor 281 0 R /FirstChar 65 /LastChar 98 /Widths 230 0 R /Encoding 228 0 R &#62;&#62;&#10;&#60;&#60; /Type /Font /Subtype /Type1 /BaseFont /NANTFZ+MSBM10 /FontDescriptor 283 0 R /FirstChar 80 /LastChar 82 /Widths 233 0 R &#62;&#62;</data>
+<data size="13627">107 0 30 41 109 81 34 122 110 163 112 209 113 256 114 302 38 343 115 384&#10;116 431 123 478 124 523 127 568 42 609 130 650 46 691 131 732 132 773 133 818&#10;134 859 135 905 50 946 136 987 137 1028 139 1074 140 1120 141 1161 142 1206 143 1251&#10;144 1295 145 1340 54 1380 146 1420 147 1460 148 1500 149 1540 150 1579 85 1618 1 2039&#10;2 2044 3 2049 226 2087 229 2103 230 2380 231 2463 232 2636 233 2725 234 2742 235 2975&#10;236 2984 237 2993 238 3002 239 3114 240 3143 241 3276 242 3507 243 3642 245 3907 246 3916&#10;247 4126 248 4576 249 4870 251 5101 253 5390 255 5595 257 5926 259 6131 261 6337 263 6553&#10;265 6773 267 7056 269 7418 271 7662 273 7899 275 8444 277 8710 279 9001 281 9329 283 9553&#10;228 9758 244 10175 117 10226 122 10352 120 10479 108 10606 121 10732 119 10856 126 10980 118 11106&#10;99 11230 90 11383 106 11536 111 11695 91 11855 128 12011 138 12165 105 12320 129 12475 125 12628&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 2262.241 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 2257.19 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 2195.519 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 2190.469 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 123.648 2162.67 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 206.216 2126.805 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 58.835 2114.849 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 2090.441 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 2085.391 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 139.373 2056.942 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 139.373 2044.987 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 3.312 2017.091 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 3.312 2005.136 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 1863.299 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 1854.264 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 1716.034 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 1710.984 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 1649.312 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 39.215 1583.01 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 1557.506 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 39.215 1467.293 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 1441.789 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 1436.738 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 1398.579 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 17.933 1193.012 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 43.614 1166.362 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 1138.467 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 43.614 883.018 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 81.851 815.272 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 42.535 612.35 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 43.614 318.058 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 292.553 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 287.503 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 192.432 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 164.634 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 120.798 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 65.007 null ] &#62;&#62;&#10;&#60;&#60; /D [ 58 0 R /XYZ 0 20.231 null ] &#62;&#62;&#10;&#60;&#60;  /ColorSpace 3 0 R /Pattern 2 0 R /ExtGState 1 0 R  /Font &#60;&#60; /F18 90 0 R /F16 91 0 R /F48 99 0 R /F49 104 0 R /F50 105 0 R /F51 106 0 R /F19 108 0 R /F54 111 0 R /F28 117 0 R /F26 118 0 R /F20 119 0 R /F23 120 0 R /F21 121 0 R /F22 122 0 R /F34 125 0 R /F25 126 0 R /F56 128 0 R /F57 129 0 R /F58 138 0 R &#62;&#62; /XObject &#60;&#60; /Im1 59 0 R /Im2 60 0 R /Im3 61 0 R /Im4 74 0 R /Im5 75 0 R &#62;&#62; /ProcSet [ /PDF /Text /ImageC ] &#62;&#62;&#10;&#60;&#60;&#62;&#62;&#10;&#60;&#60;&#62;&#62;&#10;&#60;&#60;  /pgfprgb [/Pattern /DeviceRGB] &#62;&#62;&#10;[ 58 0 R /Fit ]&#10;[590.3 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 354.2 295.1 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 722.6 693.1 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 531.3 590.3 472.2 0 472.2 324.7 531.3 0 295.1 0 0 295.1 885.4 590.3 531.3 590.3 0 414.1 419.1 413.2 590.3 0 0 560.7 ]&#10;[865.9 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 603.2 544.4 ]&#10;[569.4 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 569.4 569.4 569.4 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 323.4 0 323.4 ]&#10;[666.7 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 713.3 ]&#10;[611.1 0 722.2 ]&#10;[277.8 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 528.6 429.2 432.8 520.5 465.6 489.6 477 576.2 344.5 411.8 520.6 298.4 878 600.2 484.7 503.1 446.4 451.2 468.8 361.1 572.5 484.7 715.9 571.5 490.3 465 ]&#10;[680.6 ]&#10;[647.8 ]&#10;[569.4 ]&#10;[892.9 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 1138.9 ]&#10;[472.2 0 0 0 0 0 0 0 555.6 ]&#10;[813.9 0 786.1 0 0 0 0 0 0 0 0 0 988.9 813.9 0 0 0 0 611.1 0 813.9 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 457.8 ]&#10;[777.8 0 0 0 0 500 500 500 500 500 500 500 500 500 500 0 0 0 777.8 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 277.8 0 277.8 0 0 0 500 0 0 555.6 444.4 0 500 0 277.8 0 0 0 833.3 555.6 0 555.6 0 391.7 0 0 0 0 0 527.8 ]&#10;[816.7 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 591.1 0 532.2 591.1 0 0 0 0 355.5 0 0 296.7 0 0 591.1 0 0 0 0 385 ]&#10;[511.1 0 0 0 0 0 511.1 0 511.1 306.7 0 0 0 0 0 0 743.3 0 715.6 0 678.3 652.8 0 0 385.5 525 0 627.2 0 743.3 0 678.3 0 0 562.2 715.6 0 0 0 743.3 0 0 0 0 0 0 0 0 511.1 0 460 511.1 460 306.7 460 511.1 306.7 0 0 255.5 817.8 562.2 511.1 511.1 0 421.7 408.9 332.2 536.7 ]&#10;[777.8 ]&#10;[319.5 0 0 575 575 0 0 0 0 0 0 0 0 0 0 0 0 543 0 0 818 0 0 0 0 0 0 0 0 0 0 1091.7 0 0 0 0 0 638.9 0 0 0 0 0 0 0 0 0 0 0 0 0 0 638.9 511.1 638.9 527.1 0 0 0 319.5 0 0 319.5 0 638.9 575 0 0 0 453.6 447.2 638.9 ]&#10;[500 0 0 0 0 0 0 555.5 0 0 0 0 0 0 0 0 0 0 277.8 388.9 388.9 0 777.8 277.8 333.3 277.8 0 500 500 500 500 500 500 500 500 500 500 277.8 0 0 777.8 0 0 0 750 708.3 722.2 763.9 680.5 652.8 784.7 0 361.1 513.9 777.8 625 916.7 750 0 680.5 777.8 736.1 555.5 722.2 750 750 1027.8 750 0 0 277.8 0 277.8 0 0 277.8 500 555.5 444.5 555.5 444.5 305.5 500 555.5 277.8 305.5 527.8 277.8 833.3 555.5 500 555.5 527.8 391.7 394.4 388.9 555.5 527.8 722.2 527.8 527.8 ]&#10;[312.5 0 0 562.5 562.5 562.5 562.5 562.5 562.5 562.5 562.5 562.5 0 0 0 0 0 0 0 849.5 0 0 0 0 707.2 0 0 419 0 0 675.9 1067.2 879.6 0 0 0 839.2 625 782.4 0 0 0 0 0 0 0 0 0 0 0 0 546.9 625 500 625 513.3 343.7 562.5 625 312.5 0 593.7 312.5 937.5 625 562.5 625 0 459.5 443.7 437.5 625 0 0 0 593.7 ]&#10;&#60;&#60; /Type /FontDescriptor /FontName /JCFPGD+CMEX10 /Flags 4 /FontBBox [ -24 -2960 1454 772 ] /Ascent 40 /CapHeight 0 /Descent -600 /ItalicAngle 0 /StemV 47 /XHeight 431 /CharSet&#40; /integraldisplay /integraltext&#41; /FontFile 250 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /XSTMCN+CMMI10 /Flags 4 /FontBBox [ -32 -250 1048 750 ] /Ascent 694 /CapHeight 683 /Descent -194 /ItalicAngle -14 /StemV 72 /XHeight 431 /CharSet&#40; /a /b /c /comma /d /e /f /g /h /i /j /k /l /m /n /o /p /q /r /s /t /u /v /w /x /y /z&#41; /FontFile 252 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /QXILPS+CMMI7 /Flags 4 /FontBBox [ -1 -250 1171 750 ] /Ascent 694 /CapHeight 683 /Descent -194 /ItalicAngle -14 /StemV 81 /XHeight 431 /CharSet&#40; /x&#41; /FontFile 254 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /IKPMKY+CMR10 /Flags 4 /FontBBox [ -40 -250 1009 750 ] /Ascent 694 /CapHeight 683 /Descent -194 /ItalicAngle 0 /StemV 69 /XHeight 431 /CharSet&#40; /a /bracketleft /bracketright /d /e /eight /equal /five /four /g /i /m /n /nine /one /p /plus /r /seven /six /three /two /x /zero&#41; /FontFile 256 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /THGOAZ+CMR5 /Flags 4 /FontBBox [ -10 -250 1304 750 ] /Ascent 694 /CapHeight 680 /Descent -194 /ItalicAngle 0 /StemV 89 /XHeight 431 /CharSet&#40; /two&#41; /FontFile 258 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /REOFEC+CMR7 /Flags 4 /FontBBox [ -27 -250 1122 750 ] /Ascent 694 /CapHeight 683 /Descent -194 /ItalicAngle 0 /StemV 79 /XHeight 431 /CharSet&#40; /zero&#41; /FontFile 260 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /KZGXGZ+CMSY10 /Flags 4 /FontBBox [ -29 -960 1116 775 ] /Ascent 750 /CapHeight 683 /Descent -194 /ItalicAngle -14 /StemV 40 /XHeight 431 /CharSet&#40; /X /element&#41; /FontFile 262 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /XNLILI+CMSY7 /Flags 4 /FontBBox [ -15 -951 1251 782 ] /Ascent 750 /CapHeight 683 /Descent -194 /ItalicAngle -14 /StemV 49 /XHeight 431 /CharSet&#40; /infinity /minus&#41; /FontFile 264 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /JNKRSO+LMRoman10-Bold /Flags 4 /FontBBox [ -486 -295 1607 1133 ] /Ascent 699 /CapHeight 699 /Descent -194 /ItalicAngle 0 /StemV 114 /XHeight 444 /CharSet&#40; /B /M /S /b /c /d /e /i /l /n /o /one /period /question /s /t /two /u&#41; /FontFile 266 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /ESECFF+LMRoman12-Bold /Flags 4 /FontBBox [ -476 -289 1577 1137 ] /Ascent 684 /CapHeight 684 /Descent -194 /ItalicAngle 0 /StemV 109 /XHeight 444 /CharSet&#40; /A /F /I /L /M /N /R /S /T /a /b /c /d /e /eight /f /five /four /g /h /i /k /l /m /n /nine /o /one /p /period /r /s /seven /six /t /three /two /u /y&#41; /FontFile 268 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /DMGJGY+LMRoman10-BoldItalic /Flags 4 /FontBBox [ -518 -307 1565 1147 ] /Ascent 700 /CapHeight 700 /Descent -194 /ItalicAngle -14 /StemV 96 /XHeight 444 /CharSet&#40; /B /a /c /d /i /l /o /t&#41; /FontFile 270 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /MRRRNS+LMRomanCaps10-Regular /Flags 4 /FontBBox [ -496 -290 1501 1100 ] /Ascent 527 /CapHeight 689 /Descent 0 /ItalicAngle 0 /StemV 89 /XHeight 431 /CharSet&#40; /A /C /M /N /S /U /s&#41; /FontFile 272 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /KIPIOQ+LMRoman10-Regular /Flags 4 /FontBBox [ -430 -290 1417 1127 ] /Ascent 0 /CapHeight 0 /Descent 0 /ItalicAngle 0 /StemV 69 /XHeight 431 /CharSet&#40; /A /B /C /D /E /F /G /I /J /K /L /M /N /P /Q /R /S /T /U /V /W /X /a /b /bracketleft /bracketright /bullet /c /colon /comma /d /e /eight /endash /equal /f /fi /five /four /g /h /hyphen /i /j /k /l /m /n /nine /o /one /p /parenleft /parenright /period /plus /q /quoteleft /quoteright /r /s /seven /six /t /three /two /u /v /w /x /y /zero&#41; /FontFile 274 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /RRPEYH+LMRoman7-Regular /Flags 4 /FontBBox [ -483 -292 1562 1124 ] /Ascent 689 /CapHeight 689 /Descent -194 /ItalicAngle 0 /StemV 79 /XHeight 431 /CharSet&#40; /bracketleft /bracketright /endash /one /three /two&#41; /FontFile 276 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /DBJOTS+LMRoman8-Regular /Flags 4 /FontBBox [ -456 -292 1497 1125 ] /Ascent 689 /CapHeight 689 /Descent -194 /ItalicAngle 0 /StemV 76 /XHeight 431 /CharSet&#40; /E /F /a /b /c /e /f /fi /g /hyphen /i /l /m /n /o /p /period /r /s /t /u /x&#41; /FontFile 278 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /QQNAVM+LMRoman10-Italic /Flags 4 /FontBBox [ -458 -290 1386 1125 ] /Ascent 689 /CapHeight 689 /Descent -194 /ItalicAngle -14 /StemV 56 /XHeight 431 /CharSet&#40; /A /C /E /F /I /J /L /N /P /S /T /X /a /c /colon /d /e /f /g /h /i /l /m /n /nine /o /one /p /r /s /seven /t /u&#41; /FontFile 280 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /RBBYWX+LMRoman7-Italic /Flags 4 /FontBBox [ -528 -292 1571 1123 ] /Ascent 689 /CapHeight 689 /Descent -194 /ItalicAngle -14 /StemV 70 /XHeight 431 /CharSet&#40; /A /a /b&#41; /FontFile 282 0 R &#62;&#62;&#10;&#60;&#60; /Type /FontDescriptor /FontName /NANTFZ+MSBM10 /Flags 4 /FontBBox [ -55 -420 2343 920 ] /Ascent 464 /CapHeight 689 /Descent 0 /ItalicAngle 0 /StemV 40 /XHeight 463 /CharSet&#40; /P /R&#41; /FontFile 284 0 R &#62;&#62;&#10;&#60;&#60; /Type /Encoding /Differences [ 21 /endash 28 /fi 39 /quoteright /parenleft /parenright 43 /plus /comma /hyphen /period 48 /zero /one /two /three /four /five /six /seven /eight /nine /colon 61 /equal 63 /question 65 /A /B /C /D /E /F /G 73 /I /J /K /L /M /N 80 /P /Q /R /S /T /U /V /W /X 91 /bracketleft 93 /bracketright 96 /quoteleft /a /b /c /d /e /f /g /h /i /j /k /l /m /n /o /p /q /r /s /t /u /v /w /x /y ] &#62;&#62;&#10;&#60;&#60; /Type /Encoding /Differences [ 136 /bullet ] &#62;&#62;&#10;&#60;&#60; /Type /Font /Subtype /Type1 /BaseFont /JCFPGD+CMEX10 /FontDescriptor 249 0 R /FirstChar 82 /LastChar 90 /Widths 239 0 R &#62;&#62;&#10;&#60;&#60; /Type /Font /Subtype /Type1 /BaseFont /XSTMCN+CMMI10 /FontDescriptor 251 0 R /FirstChar 59 /LastChar 122 /Widths 234 0 R &#62;&#62;&#10;&#60;&#60; /Type /Font /Subtype /Type1 /BaseFont /QXILPS+CMMI7 /FontDescriptor 253 0 R /FirstChar 120 /LastChar 120 /Widths 236 0 R &#62;&#62;&#10;&#60;&#60; /Type /Font /Subtype /Type1 /BaseFont /IKPMKY+CMR10 /FontDescriptor 255 0 R /FirstChar 43 /LastChar 120 /Widths 241 0 R &#62;&#62;&#10;&#60;&#60; /Type /Font /Subtype /Type1 /BaseFont /THGOAZ+CMR5 /FontDescriptor 257 0 R /FirstChar 50 /LastChar 50 /Widths 235 0 R &#62;&#62;&#10;&#60;&#60; /Type /Font /Subtype /Type1 /BaseFont /REOFEC+CMR7 /FontDescriptor 259 0 R /FirstChar 48 /LastChar 48 /Widths 237 0 R &#62;&#62;&#10;&#60;&#60; /Type /Font /Subtype /Type1 /BaseFont /KZGXGZ+CMSY10 /FontDescriptor 261 0 R /FirstChar 50 /LastChar 88 /Widths 232 0 R &#62;&#62;&#10;&#60;&#60; /Type /Font /Subtype /Type1 /BaseFont /XNLILI+CMSY7 /FontDescriptor 263 0 R /FirstChar 0 /LastChar 49 /Widths 238 0 R &#62;&#62;&#10;&#60;&#60; /Type /Font /Subtype /Type1 /BaseFont /JNKRSO+LMRoman10-Bold /FontDescriptor 265 0 R /FirstChar 46 /LastChar 117 /Widths 246 0 R /Encoding 228 0 R &#62;&#62;&#10;&#60;&#60; /Type /Font /Subtype /Type1 /BaseFont /ESECFF+LMRoman12-Bold /FontDescriptor 267 0 R /FirstChar 46 /LastChar 121 /Widths 248 0 R /Encoding 228 0 R &#62;&#62;&#10;&#60;&#60; /Type /Font /Subtype /Type1 /BaseFont /DMGJGY+LMRoman10-BoldItalic /FontDescriptor 269 0 R /FirstChar 66 /LastChar 116 /Widths 242 0 R /Encoding 228 0 R &#62;&#62;&#10;&#60;&#60; /Type /Font /Subtype /Type1 /BaseFont /MRRRNS+LMRomanCaps10-Regular /FontDescriptor 271 0 R /FirstChar 65 /LastChar 115 /Widths 240 0 R /Encoding 228 0 R &#62;&#62;&#10;&#60;&#60; /Type /Font /Subtype /Type1 /BaseFont /KIPIOQ+LMRoman10-Regular /FontDescriptor 273 0 R /FirstChar 21 /LastChar 121 /Widths 247 0 R /Encoding 228 0 R &#62;&#62;&#10;&#60;&#60; /Type /Font /Subtype /Type1 /BaseFont /RRPEYH+LMRoman7-Regular /FontDescriptor 275 0 R /FirstChar 21 /LastChar 93 /Widths 231 0 R /Encoding 228 0 R &#62;&#62;&#10;&#60;&#60; /Type /Font /Subtype /Type1 /BaseFont /DBJOTS+LMRoman8-Regular /FontDescriptor 277 0 R /FirstChar 28 /LastChar 120 /Widths 229 0 R /Encoding 228 0 R &#62;&#62;&#10;&#60;&#60; /Type /Font /Subtype /Type1 /BaseFont /QQNAVM+LMRoman10-Italic /FontDescriptor 279 0 R /FirstChar 49 /LastChar 117 /Widths 243 0 R /Encoding 228 0 R &#62;&#62;&#10;&#60;&#60; /Type /Font /Subtype /Type1 /BaseFont /RBBYWX+LMRoman7-Italic /FontDescriptor 281 0 R /FirstChar 65 /LastChar 98 /Widths 230 0 R /Encoding 228 0 R &#62;&#62;&#10;&#60;&#60; /Type /Font /Subtype /Type1 /BaseFont /NANTFZ+MSBM10 /FontDescriptor 283 0 R /FirstChar 80 /LastChar 82 /Widths 233 0 R &#62;&#62;</data>
 </stream>
 </object>
 
 <object id="228">
 <dict size="2">
 <key>Type</key>
 <value><literal>Encoding</literal></value>
@@ -6950,17 +6950,17 @@
 <key>Creator</key>
 <value><string size="19">LaTeX with hyperref</string></value>
 <key>Keywords</key>
 <value><string size="0"></string></value>
 <key>Producer</key>
 <value><string size="13">LuaTeX-1.15.0</string></value>
 <key>CreationDate</key>
-<value><string size="23">D:20230412012359-04&#39;00&#39;</string></value>
+<value><string size="23">D:20230412162148-04&#39;00&#39;</string></value>
 <key>ModDate</key>
-<value><string size="23">D:20230412012359-04&#39;00&#39;</string></value>
+<value><string size="23">D:20230412162148-04&#39;00&#39;</string></value>
 <key>Trapped</key>
 <value><literal>False</literal></value>
 <key>PTEX.FullBanner</key>
 <value><string size="48">This is LuaHBTeX, Version 1.15.0 &#40;TeX Live 2022&#41;</string></value>
 </dict>
 </object>
 
@@ -6985,24 +6985,24 @@
 </list></value>
 <key>Root</key>
 <value><ref id="291" /></value>
 <key>Info</key>
 <value><ref id="292" /></value>
 <key>ID</key>
 <value><list size="2">
-<string size="16">&#151;&#28;aEgUk&#13;=Mm&#218;.wku</string>
-<string size="16">&#151;&#28;aEgUk&#13;=Mm&#218;.wku</string>
+<string size="16">&#132;&#194;&#20;&#202;ne&#245;&#26;&#162;&#237;&#164;&#130;&#16;&#221;c&#225;</string>
+<string size="16">&#132;&#194;&#20;&#202;ne&#245;&#26;&#162;&#237;&#164;&#130;&#16;&#221;c&#225;</string>
 </list></value>
 <key>Filter</key>
 <value><literal>FlateDecode</literal></value>
 <key>Length</key>
-<value><number>750</number></value>
+<value><number>752</number></value>
 </dict>
 </props>
-<data size="1470">&#0;&#0;&#0;Q&#255;&#2;&#0;&#0;&#227;&#39;&#2;&#0;&#0;&#227;&#40;&#2;&#0;&#0;&#227;&#41;&#2;&#0;&#0;&#5;&#0;&#1;&#4;BN&#0;&#2;&#0;&#0;&#5;S&#2;&#0;&#1;&#29;&#15;&#2;&#0;&#0;&#5;&#1;&#2;&#0;&#0;&#5;&#2;&#2;&#0;&#0;&#5;Y&#2;&#0;&#1;&#29;&#14;&#2;&#0;&#0;&#5;&#3;&#2;&#0;&#0;&#5;&#4;&#2;&#0;&#0;&#5;[&#2;&#0;&#1;&#29;&#13;&#2;&#0;&#0;&#5;&#5;&#2;&#0;&#0;&#5;&#6;&#2;&#0;&#0;&#5;]&#2;&#0;&#1;&#29;&#12;&#2;&#0;&#0;&#5;&#7;&#2;&#0;&#0;&#5;&#8;&#2;&#0;&#0;&#5;_&#2;&#0;&#1;&#29;&#11;&#2;&#0;&#0;&#5;&#9;&#2;&#0;&#0;&#5;&#10;&#2;&#0;&#0;&#5;c&#2;&#0;&#1;&#29;&#10;&#2;&#0;&#0;&#5;&#11;&#2;&#0;&#0;&#5;&#12;&#2;&#0;&#0;&#227;&#1;&#2;&#0;&#1;&#29;&#9;&#2;&#0;&#0;&#5;&#13;&#2;&#0;&#0;&#5;&#14;&#2;&#0;&#0;&#227;&#3;&#2;&#0;&#1;&#29;&#8;&#2;&#0;&#0;&#5;&#15;&#2;&#0;&#0;&#5;&#16;&#2;&#0;&#0;&#227;&#8;&#2;&#0;&#1;&#29;&#7;&#2;&#0;&#0;&#5;&#17;&#2;&#0;&#0;&#5;&#18;&#2;&#0;&#0;&#227;&#14;&#2;&#0;&#1;&#29;&#6;&#2;&#0;&#0;&#5;&#19;&#2;&#0;&#0;&#5;&#20;&#2;&#0;&#0;&#227;&#16;&#2;&#0;&#1;&#29;&#5;&#2;&#0;&#0;&#5;&#21;&#2;&#0;&#0;&#5;&#22;&#2;&#0;&#0;&#227;&#22;&#2;&#0;&#1;&#29;&#4;&#2;&#0;&#0;&#5;&#23;&#2;&#0;&#0;&#5;&#24;&#2;&#0;&#0;&#227; &#2;&#0;&#1;&#29;&#3;&#2;&#0;&#0;&#5;&#25;&#2;&#0;&#0;&#5;&#26;&#2;&#0;&#0;&#5;&#27;&#1;&#0;&#22;&#153;&#0;&#1;&#3;&#21;&#39;&#0;&#1;&#3;&#92;&#131;&#0;&#2;&#0;&#0;&#5;=&#2;&#0;&#0;&#5;&#62;&#2;&#0;&#0;&#5;?&#2;&#0;&#0;&#5;@&#2;&#0;&#0;&#5;A&#2;&#0;&#0;&#5;B&#2;&#0;&#0;&#5;C&#2;&#0;&#0;&#5;D&#2;&#0;&#0;&#5;E&#2;&#0;&#0;&#5;F&#2;&#0;&#0;&#5;G&#2;&#0;&#0;&#5;H&#1;&#3;&#142;+&#0;&#1;&#3;&#181;&#9;&#0;&#2;&#0;&#0;&#5;I&#2;&#0;&#0;&#5;J&#2;&#0;&#0;&#5;K&#2;&#0;&#0;&#5;L&#2;&#0;&#0;&#5;M&#0;&#0;&#0;S&#255;&#2;&#0;&#0;&#5;N&#0;&#0;&#0;&#0;&#255;&#2;&#0;&#0;&#5;O&#2;&#0;&#0;&#227;&#38;&#1;&#0;&#0;&#20;&#0;&#2;&#0;&#0;&#5;P&#2;&#0;&#0;&#5;Q&#2;&#0;&#0;&#5;R&#2;&#0;&#0;&#227;[&#2;&#0;&#0;&#227;^&#2;&#0;&#0;&#5;T&#2;&#0;&#0;&#5;U&#2;&#0;&#0;&#5;V&#2;&#0;&#0;&#5;W&#2;&#0;&#0;&#5;X&#2;&#0;&#0;&#5;Z&#2;&#0;&#0;&#5;&#92;&#2;&#0;&#0;&#227;Z&#2;&#0;&#0;&#5;^&#2;&#0;&#0;&#5;`&#2;&#0;&#0;&#5;a&#2;&#0;&#0;&#5;b&#2;&#0;&#1;&#29;&#0;&#2;&#0;&#0;&#227;a&#2;&#0;&#0;&#227;&#92;&#2;&#0;&#0;&#227;&#0;&#2;&#0;&#0;&#227;U&#2;&#0;&#0;&#227;&#2;&#2;&#0;&#0;&#227;&#4;&#2;&#0;&#0;&#227;]&#2;&#0;&#0;&#227;&#5;&#2;&#0;&#0;&#227;&#6;&#2;&#0;&#0;&#227;&#7;&#2;&#0;&#0;&#227;&#9;&#2;&#0;&#0;&#227;&#10;&#2;&#0;&#0;&#227;R&#2;&#0;&#0;&#227;Y&#2;&#0;&#0;&#227;W&#2;&#0;&#0;&#227;T&#2;&#0;&#0;&#227;V&#2;&#0;&#0;&#227;S&#2;&#0;&#0;&#227;&#11;&#2;&#0;&#0;&#227;&#12;&#2;&#0;&#0;&#227;c&#2;&#0;&#0;&#227;X&#2;&#0;&#0;&#227;&#13;&#2;&#0;&#0;&#227;_&#2;&#0;&#0;&#227;b&#2;&#0;&#0;&#227;&#15;&#2;&#0;&#0;&#227;&#17;&#2;&#0;&#0;&#227;&#18;&#2;&#0;&#0;&#227;&#19;&#2;&#0;&#0;&#227;&#20;&#2;&#0;&#0;&#227;&#21;&#2;&#0;&#0;&#227;&#23;&#2;&#0;&#0;&#227;&#24;&#2;&#0;&#0;&#227;`&#2;&#0;&#0;&#227;&#25;&#2;&#0;&#0;&#227;&#26;&#2;&#0;&#0;&#227;&#27;&#2;&#0;&#0;&#227;&#28;&#2;&#0;&#0;&#227;&#29;&#2;&#0;&#0;&#227;&#30;&#2;&#0;&#0;&#227;&#31;&#2;&#0;&#0;&#227;!&#2;&#0;&#0;&#227;&#34;&#2;&#0;&#0;&#227;#&#2;&#0;&#0;&#227;$&#2;&#0;&#0;&#227;%&#2;&#0;&#1;&#29;&#1;&#2;&#0;&#0;&#5;&#28;&#2;&#0;&#0;&#5;&#29;&#2;&#0;&#0;&#5;&#30;&#2;&#0;&#0;&#5;&#31;&#2;&#0;&#0;&#5; &#2;&#0;&#0;&#5;!&#1;&#3;&#19;&#249;&#0;&#1;&#3;.*&#0;&#2;&#0;&#0;&#5;&#34;&#2;&#0;&#0;&#5;#&#2;&#0;&#0;&#5;$&#2;&#0;&#0;&#5;%&#2;&#0;&#0;&#5;&#38;&#2;&#0;&#0;&#5;&#39;&#1;&#3;u&#216;&#0;&#1;&#3;w&#3;&#0;&#1;&#3;x.&#0;&#1;&#3;yY&#0;&#2;&#0;&#0;&#5;&#40;&#2;&#0;&#0;&#5;&#41;&#2;&#0;&#0;&#5;*&#1;&#3;z&#132;&#0;&#1;&#3;{j&#0;&#1;&#3;|q&#0;&#1;&#3;}&#204;&#0;&#1;&#3;~&#253;&#0;&#1;&#3;&#127;&#255;&#0;&#1;&#3;&#129;L&#0;&#1;&#3;&#130;&#25;&#0;&#1;&#3;&#131;&#143;&#0;&#1;&#3;&#132;{&#0;&#1;&#3;&#133;L&#0;&#1;&#3;&#134;&#193;&#0;&#1;&#3;&#135;&#251;&#0;&#1;&#3;&#136;V&#0;&#1;&#3;&#137;&#38;&#0;&#1;&#3;&#138;?&#0;&#1;&#3;&#139;&#182;&#0;&#1;&#3;&#140;&#254;&#0;&#2;&#0;&#0;&#5;+&#2;&#0;&#0;&#5;,&#2;&#0;&#0;&#5;-&#2;&#0;&#0;&#5;.&#2;&#0;&#0;&#5;/&#2;&#0;&#0;&#5;0&#2;&#0;&#0;&#5;1&#2;&#0;&#0;&#5;2&#2;&#0;&#0;&#5;3&#2;&#0;&#0;&#5;4&#2;&#0;&#0;&#5;5&#2;&#0;&#0;&#5;6&#2;&#0;&#0;&#5;7&#2;&#0;&#0;&#5;8&#2;&#0;&#0;&#5;9&#2;&#0;&#0;&#5;:&#2;&#0;&#0;&#5;;&#2;&#0;&#0;&#5;&#60;&#1;&#4;0?&#0;&#1;&#4;18&#0;&#1;&#4;2=&#0;&#1;&#4;3n&#0;&#1;&#4;4L&#0;&#1;&#4;54&#0;&#1;&#4;6&#22;&#0;&#1;&#4;7}&#0;&#1;&#4;8&#130;&#0;&#1;&#4;99&#0;&#1;&#4;:&#34;&#0;&#1;&#4;;o&#0;&#1;&#4;&#60;[&#0;&#1;&#4;=W&#0;&#1;&#4;&#62;&#145;&#0;&#1;&#4;?&#170;&#0;&#1;&#4;A!&#0;&#2;&#0;&#0;&#227;*&#1;&#8;G&#217;&#0;&#2;&#0;&#0;&#227;P&#2;&#0;&#0;&#227;+&#2;&#0;&#0;&#227;,&#2;&#0;&#0;&#227;-&#2;&#0;&#0;&#227;.&#2;&#0;&#0;&#227;/&#2;&#0;&#0;&#227;0&#2;&#0;&#0;&#227;1&#2;&#0;&#0;&#227;2&#2;&#0;&#0;&#227;3&#2;&#0;&#0;&#227;4&#2;&#0;&#0;&#227;5&#2;&#0;&#0;&#227;6&#2;&#0;&#0;&#227;7&#2;&#0;&#0;&#227;8&#2;&#0;&#0;&#227;9&#2;&#0;&#0;&#227;Q&#2;&#0;&#0;&#227;:&#2;&#0;&#0;&#227;;&#2;&#0;&#0;&#227;&#60;&#2;&#0;&#0;&#227;=&#2;&#0;&#0;&#227;&#62;&#1;&#4;M&#197;&#0;&#2;&#0;&#0;&#227;?&#1;&#4;j &#0;&#2;&#0;&#0;&#227;@&#1;&#4;&#154;&#147;&#0;&#2;&#0;&#0;&#227;A&#1;&#4;&#182;t&#0;&#2;&#0;&#0;&#227;B&#1;&#4;&#235;&#243;&#0;&#2;&#0;&#0;&#227;C&#1;&#5;&#7;e&#0;&#2;&#0;&#0;&#227;D&#1;&#5;&#34;&#205;&#0;&#2;&#0;&#0;&#227;E&#1;&#5;?F&#0;&#2;&#0;&#0;&#227;F&#1;&#5;[P&#0;&#2;&#0;&#0;&#227;G&#1;&#5;&#182;]&#0;&#2;&#0;&#0;&#227;H&#1;&#6;&#30;&#14;&#0;&#2;&#0;&#0;&#227;I&#1;&#6;O&#168;&#0;&#2;&#0;&#0;&#227;J&#1;&#6;&#155;&#142;&#0;&#2;&#0;&#0;&#227;K&#1;&#7; &#194;&#0;&#2;&#0;&#0;&#227;L&#1;&#7;n&#62;&#0;&#2;&#0;&#0;&#227;M&#1;&#7;&#208;c&#0;&#2;&#0;&#0;&#227;N&#1;&#8;&#23;&#176;&#0;&#2;&#0;&#0;&#227;O&#1;&#8;=&#212;&#0;&#1;&#8;V&#193;&#0;&#2;&#0;&#1;&#29;&#2;&#2;&#0;&#1;&#29;&#16;&#2;&#0;&#1;&#29;&#17;&#2;&#0;&#1;&#29;&#18;&#2;&#0;&#1;&#29;&#19;&#2;&#0;&#1;&#29;&#20;&#1;&#8;U&#173;&#0;&#1;&#8;Z&#245;&#0;</data>
+<data size="1470">&#0;&#0;&#0;Q&#255;&#2;&#0;&#0;&#227;&#39;&#2;&#0;&#0;&#227;&#40;&#2;&#0;&#0;&#227;&#41;&#2;&#0;&#0;&#5;&#0;&#1;&#4;BP&#0;&#2;&#0;&#0;&#5;S&#2;&#0;&#1;&#29;&#15;&#2;&#0;&#0;&#5;&#1;&#2;&#0;&#0;&#5;&#2;&#2;&#0;&#0;&#5;Y&#2;&#0;&#1;&#29;&#14;&#2;&#0;&#0;&#5;&#3;&#2;&#0;&#0;&#5;&#4;&#2;&#0;&#0;&#5;[&#2;&#0;&#1;&#29;&#13;&#2;&#0;&#0;&#5;&#5;&#2;&#0;&#0;&#5;&#6;&#2;&#0;&#0;&#5;]&#2;&#0;&#1;&#29;&#12;&#2;&#0;&#0;&#5;&#7;&#2;&#0;&#0;&#5;&#8;&#2;&#0;&#0;&#5;_&#2;&#0;&#1;&#29;&#11;&#2;&#0;&#0;&#5;&#9;&#2;&#0;&#0;&#5;&#10;&#2;&#0;&#0;&#5;c&#2;&#0;&#1;&#29;&#10;&#2;&#0;&#0;&#5;&#11;&#2;&#0;&#0;&#5;&#12;&#2;&#0;&#0;&#227;&#1;&#2;&#0;&#1;&#29;&#9;&#2;&#0;&#0;&#5;&#13;&#2;&#0;&#0;&#5;&#14;&#2;&#0;&#0;&#227;&#3;&#2;&#0;&#1;&#29;&#8;&#2;&#0;&#0;&#5;&#15;&#2;&#0;&#0;&#5;&#16;&#2;&#0;&#0;&#227;&#8;&#2;&#0;&#1;&#29;&#7;&#2;&#0;&#0;&#5;&#17;&#2;&#0;&#0;&#5;&#18;&#2;&#0;&#0;&#227;&#14;&#2;&#0;&#1;&#29;&#6;&#2;&#0;&#0;&#5;&#19;&#2;&#0;&#0;&#5;&#20;&#2;&#0;&#0;&#227;&#16;&#2;&#0;&#1;&#29;&#5;&#2;&#0;&#0;&#5;&#21;&#2;&#0;&#0;&#5;&#22;&#2;&#0;&#0;&#227;&#22;&#2;&#0;&#1;&#29;&#4;&#2;&#0;&#0;&#5;&#23;&#2;&#0;&#0;&#5;&#24;&#2;&#0;&#0;&#227; &#2;&#0;&#1;&#29;&#3;&#2;&#0;&#0;&#5;&#25;&#2;&#0;&#0;&#5;&#26;&#2;&#0;&#0;&#5;&#27;&#1;&#0;&#22;&#155;&#0;&#1;&#3;&#21;&#41;&#0;&#1;&#3;&#92;&#133;&#0;&#2;&#0;&#0;&#5;=&#2;&#0;&#0;&#5;&#62;&#2;&#0;&#0;&#5;?&#2;&#0;&#0;&#5;@&#2;&#0;&#0;&#5;A&#2;&#0;&#0;&#5;B&#2;&#0;&#0;&#5;C&#2;&#0;&#0;&#5;D&#2;&#0;&#0;&#5;E&#2;&#0;&#0;&#5;F&#2;&#0;&#0;&#5;G&#2;&#0;&#0;&#5;H&#1;&#3;&#142;-&#0;&#1;&#3;&#181;&#11;&#0;&#2;&#0;&#0;&#5;I&#2;&#0;&#0;&#5;J&#2;&#0;&#0;&#5;K&#2;&#0;&#0;&#5;L&#2;&#0;&#0;&#5;M&#0;&#0;&#0;S&#255;&#2;&#0;&#0;&#5;N&#0;&#0;&#0;&#0;&#255;&#2;&#0;&#0;&#5;O&#2;&#0;&#0;&#227;&#38;&#1;&#0;&#0;&#20;&#0;&#2;&#0;&#0;&#5;P&#2;&#0;&#0;&#5;Q&#2;&#0;&#0;&#5;R&#2;&#0;&#0;&#227;[&#2;&#0;&#0;&#227;^&#2;&#0;&#0;&#5;T&#2;&#0;&#0;&#5;U&#2;&#0;&#0;&#5;V&#2;&#0;&#0;&#5;W&#2;&#0;&#0;&#5;X&#2;&#0;&#0;&#5;Z&#2;&#0;&#0;&#5;&#92;&#2;&#0;&#0;&#227;Z&#2;&#0;&#0;&#5;^&#2;&#0;&#0;&#5;`&#2;&#0;&#0;&#5;a&#2;&#0;&#0;&#5;b&#2;&#0;&#1;&#29;&#0;&#2;&#0;&#0;&#227;a&#2;&#0;&#0;&#227;&#92;&#2;&#0;&#0;&#227;&#0;&#2;&#0;&#0;&#227;U&#2;&#0;&#0;&#227;&#2;&#2;&#0;&#0;&#227;&#4;&#2;&#0;&#0;&#227;]&#2;&#0;&#0;&#227;&#5;&#2;&#0;&#0;&#227;&#6;&#2;&#0;&#0;&#227;&#7;&#2;&#0;&#0;&#227;&#9;&#2;&#0;&#0;&#227;&#10;&#2;&#0;&#0;&#227;R&#2;&#0;&#0;&#227;Y&#2;&#0;&#0;&#227;W&#2;&#0;&#0;&#227;T&#2;&#0;&#0;&#227;V&#2;&#0;&#0;&#227;S&#2;&#0;&#0;&#227;&#11;&#2;&#0;&#0;&#227;&#12;&#2;&#0;&#0;&#227;c&#2;&#0;&#0;&#227;X&#2;&#0;&#0;&#227;&#13;&#2;&#0;&#0;&#227;_&#2;&#0;&#0;&#227;b&#2;&#0;&#0;&#227;&#15;&#2;&#0;&#0;&#227;&#17;&#2;&#0;&#0;&#227;&#18;&#2;&#0;&#0;&#227;&#19;&#2;&#0;&#0;&#227;&#20;&#2;&#0;&#0;&#227;&#21;&#2;&#0;&#0;&#227;&#23;&#2;&#0;&#0;&#227;&#24;&#2;&#0;&#0;&#227;`&#2;&#0;&#0;&#227;&#25;&#2;&#0;&#0;&#227;&#26;&#2;&#0;&#0;&#227;&#27;&#2;&#0;&#0;&#227;&#28;&#2;&#0;&#0;&#227;&#29;&#2;&#0;&#0;&#227;&#30;&#2;&#0;&#0;&#227;&#31;&#2;&#0;&#0;&#227;!&#2;&#0;&#0;&#227;&#34;&#2;&#0;&#0;&#227;#&#2;&#0;&#0;&#227;$&#2;&#0;&#0;&#227;%&#2;&#0;&#1;&#29;&#1;&#2;&#0;&#0;&#5;&#28;&#2;&#0;&#0;&#5;&#29;&#2;&#0;&#0;&#5;&#30;&#2;&#0;&#0;&#5;&#31;&#2;&#0;&#0;&#5; &#2;&#0;&#0;&#5;!&#1;&#3;&#19;&#251;&#0;&#1;&#3;.,&#0;&#2;&#0;&#0;&#5;&#34;&#2;&#0;&#0;&#5;#&#2;&#0;&#0;&#5;$&#2;&#0;&#0;&#5;%&#2;&#0;&#0;&#5;&#38;&#2;&#0;&#0;&#5;&#39;&#1;&#3;u&#218;&#0;&#1;&#3;w&#5;&#0;&#1;&#3;x0&#0;&#1;&#3;y[&#0;&#2;&#0;&#0;&#5;&#40;&#2;&#0;&#0;&#5;&#41;&#2;&#0;&#0;&#5;*&#1;&#3;z&#134;&#0;&#1;&#3;{l&#0;&#1;&#3;|s&#0;&#1;&#3;}&#206;&#0;&#1;&#3;~&#255;&#0;&#1;&#3;&#128;&#1;&#0;&#1;&#3;&#129;N&#0;&#1;&#3;&#130;&#27;&#0;&#1;&#3;&#131;&#145;&#0;&#1;&#3;&#132;}&#0;&#1;&#3;&#133;N&#0;&#1;&#3;&#134;&#195;&#0;&#1;&#3;&#135;&#253;&#0;&#1;&#3;&#136;X&#0;&#1;&#3;&#137;&#40;&#0;&#1;&#3;&#138;A&#0;&#1;&#3;&#139;&#184;&#0;&#1;&#3;&#141;&#0;&#0;&#2;&#0;&#0;&#5;+&#2;&#0;&#0;&#5;,&#2;&#0;&#0;&#5;-&#2;&#0;&#0;&#5;.&#2;&#0;&#0;&#5;/&#2;&#0;&#0;&#5;0&#2;&#0;&#0;&#5;1&#2;&#0;&#0;&#5;2&#2;&#0;&#0;&#5;3&#2;&#0;&#0;&#5;4&#2;&#0;&#0;&#5;5&#2;&#0;&#0;&#5;6&#2;&#0;&#0;&#5;7&#2;&#0;&#0;&#5;8&#2;&#0;&#0;&#5;9&#2;&#0;&#0;&#5;:&#2;&#0;&#0;&#5;;&#2;&#0;&#0;&#5;&#60;&#1;&#4;0A&#0;&#1;&#4;1:&#0;&#1;&#4;2?&#0;&#1;&#4;3p&#0;&#1;&#4;4N&#0;&#1;&#4;56&#0;&#1;&#4;6&#24;&#0;&#1;&#4;7&#127;&#0;&#1;&#4;8&#132;&#0;&#1;&#4;9;&#0;&#1;&#4;:$&#0;&#1;&#4;;q&#0;&#1;&#4;&#60;]&#0;&#1;&#4;=Y&#0;&#1;&#4;&#62;&#147;&#0;&#1;&#4;?&#172;&#0;&#1;&#4;A#&#0;&#2;&#0;&#0;&#227;*&#1;&#8;G&#220;&#0;&#2;&#0;&#0;&#227;P&#2;&#0;&#0;&#227;+&#2;&#0;&#0;&#227;,&#2;&#0;&#0;&#227;-&#2;&#0;&#0;&#227;.&#2;&#0;&#0;&#227;/&#2;&#0;&#0;&#227;0&#2;&#0;&#0;&#227;1&#2;&#0;&#0;&#227;2&#2;&#0;&#0;&#227;3&#2;&#0;&#0;&#227;4&#2;&#0;&#0;&#227;5&#2;&#0;&#0;&#227;6&#2;&#0;&#0;&#227;7&#2;&#0;&#0;&#227;8&#2;&#0;&#0;&#227;9&#2;&#0;&#0;&#227;Q&#2;&#0;&#0;&#227;:&#2;&#0;&#0;&#227;;&#2;&#0;&#0;&#227;&#60;&#2;&#0;&#0;&#227;=&#2;&#0;&#0;&#227;&#62;&#1;&#4;M&#200;&#0;&#2;&#0;&#0;&#227;?&#1;&#4;j#&#0;&#2;&#0;&#0;&#227;@&#1;&#4;&#154;&#150;&#0;&#2;&#0;&#0;&#227;A&#1;&#4;&#182;w&#0;&#2;&#0;&#0;&#227;B&#1;&#4;&#235;&#246;&#0;&#2;&#0;&#0;&#227;C&#1;&#5;&#7;h&#0;&#2;&#0;&#0;&#227;D&#1;&#5;&#34;&#208;&#0;&#2;&#0;&#0;&#227;E&#1;&#5;?I&#0;&#2;&#0;&#0;&#227;F&#1;&#5;[S&#0;&#2;&#0;&#0;&#227;G&#1;&#5;&#182;`&#0;&#2;&#0;&#0;&#227;H&#1;&#6;&#30;&#17;&#0;&#2;&#0;&#0;&#227;I&#1;&#6;O&#171;&#0;&#2;&#0;&#0;&#227;J&#1;&#6;&#155;&#145;&#0;&#2;&#0;&#0;&#227;K&#1;&#7; &#197;&#0;&#2;&#0;&#0;&#227;L&#1;&#7;nA&#0;&#2;&#0;&#0;&#227;M&#1;&#7;&#208;f&#0;&#2;&#0;&#0;&#227;N&#1;&#8;&#23;&#179;&#0;&#2;&#0;&#0;&#227;O&#1;&#8;=&#215;&#0;&#1;&#8;V&#195;&#0;&#2;&#0;&#1;&#29;&#2;&#2;&#0;&#1;&#29;&#16;&#2;&#0;&#1;&#29;&#17;&#2;&#0;&#1;&#29;&#18;&#2;&#0;&#1;&#29;&#19;&#2;&#0;&#1;&#29;&#20;&#1;&#8;U&#175;&#0;&#1;&#8;Z&#247;&#0;</data>
 </stream>
 </object>
 
 <trailer>
 <dict size="9">
 <key>Type</key>
 <value><literal>XRef</literal></value>
@@ -7021,18 +7021,18 @@
 </list></value>
 <key>Root</key>
 <value><ref id="291" /></value>
 <key>Info</key>
 <value><ref id="292" /></value>
 <key>ID</key>
 <value><list size="2">
-<string size="16">&#151;&#28;aEgUk&#13;=Mm&#218;.wku</string>
-<string size="16">&#151;&#28;aEgUk&#13;=Mm&#218;.wku</string>
+<string size="16">&#132;&#194;&#20;&#202;ne&#245;&#26;&#162;&#237;&#164;&#130;&#16;&#221;c&#225;</string>
+<string size="16">&#132;&#194;&#20;&#202;ne&#245;&#26;&#162;&#237;&#164;&#130;&#16;&#221;c&#225;</string>
 </list></value>
 <key>Filter</key>
 <value><literal>FlateDecode</literal></value>
 <key>Length</key>
-<value><number>750</number></value>
+<value><number>752</number></value>
 </dict>
 </trailer>
 
 </pdf>
```

### Comparing `shiny_mdc-1.1.0/test/samples/stylish.pdf` & `shiny_mdc-1.2.0/test/samples/stylish.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 5% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,41 +1,43 @@
 shinymdc-test
-Author11,*
+Author One1,*
 
-Author21,2,*
-
-Author3*
+Author MiddleName Two1,2,*
 
 author1@institute1.edu
 
-author2@institute1.edu
+authortwo@institute1.edu
+
+Author*
+
+Author Four
+author4@author4.com
+
+Author Number Five2
+authornumberfive@institutetwo.edu
 
-Markdown in abstract. x + 2. Section 1. Reference [1] .
+[1]
+
+Markdown in abstract. x + 2. Section 1. Reference .
 
 1. Section
 Integer at enim eu tellus malesuada scelerisque. Ut sed rhoncus ipsum, at tempor nisl. Vivamus vitae pulvinar leo, at
 pharetra massa. Ut lobortis odio non nulla tincidunt pulvinar.
 Nunc faucibus pellentesque elit, non ornare risus suscipit sed.
 Maecenas vel blandit ex.
 Phasellus ultrices mi non nulla hendrerit, at rhoncus augue suscipit. Pellentesque a lectus eget felis maximus feugiat
 nec ut ante. Sed eget laoreet lectus. Vestibulum iaculis enim
 nec libero sollicitudin, id rhoncus libero consectetur. Integer
 eget sem quis urna vulputate aliquet.
 
 1.1. Subsection 1
 In mollis tortor vel ante cursus, ac consectetur nibh commodo.
 Aenean ultricies ornare ante ac fermentum. Vestibulum malesuada lectus at pellentesque hendrerit. Praesent a tempor ex,
-eget iaculis mauris. Integer turpis nunc, varius ac posuere
-consequat, molestie sed felis. Fusce cursus velit eu magna
-
-Author4
-author4@author4.com
 
-pellentesque posuere sed eget ex. Vivamus in gravida quam,
-in volutpat erat.
+Equal contribution. 1 Institute One. 2 Institute Two at City, State.
 
 1.2. Subsection 2
 1.2.1. Subsubsection 1
 Suspendisse erat est, imperdiet sed dolor at, sagittis lobortis
 tortor. Nulla facilisi. Aliquam pharetra scelerisque auctor.
 Duis vel auctor ipsum. Nullam sagittis feugiat mollis. Aliquam at ultrices libero. Nulla facilisi. Fusce sed est placerat,
 fringilla augue at, pretium nisl.
@@ -45,20 +47,14 @@
 sed ultricies odio ligula vitae orci. Fusce bibendum maximus
 ligula, id gravida felis dictum a. In dapibus nulla eget volutpat
 vulputate. Quisque congue erat quis nibh molestie, eget varius
 eros ultrices.
 Subsubsubsection Proin eleifend lorem semper, commodo
 tellus nec, porta purus. Nullam commodo lectus nibh, consequat maximus lorem faucibus in. Nam purus eros, rutrum in
 sapien et, condimentum lacinia nibh.
-
-2. Typography
-Equal contribution. 1 Institute1. 2 Institute2.
-
-• Bold
-• Italic
 dataset = I
 
 dataset = II
 
 dataset = III
 
 dataset = IV
@@ -75,14 +71,19 @@
 12
 10
 
 y
 
 *
 
+eget iaculis mauris. Integer turpis nunc, varius ac posuere
+consequat, molestie sed felis. Fusce cursus velit eu magna
+pellentesque posuere sed eget ex. Vivamus in gravida quam,
+in volutpat erat.
+
 8
 6
 4
 5
 
 (a) Sub-figure with ‘width=2in’
 
@@ -177,71 +178,45 @@
 
 5
 
 6
 
 Table 2: Wide table
 
-• Bold italic.
+2. Typography
 
+• Appendix table: Table B1
+• Appendix math: Equation 4
+• Short citation [²]
 • Long citation: Mittelbach et al. (2004) [²], Lesk and
 Kernighan (1977)[³]
 • Multi citation [²𝄒³𝄒⁴]
 • Pointer to footnote¹
 
+• Bold
+• Italic
+• Bold italic.
+
 3. Numbers
 • Normal: 0123456789
 • Math: 0123456789
 
+7. Tables
+• Table 1
+• Table 2
+
 4. Acronyms
 • Default (short+long): Carnegie Mellon University
 (CMU)
 • Repeated (short): CMU
 • Forced short: USA
 • Repeated after forced short (short+long): United States
 of America (USA)
 • Plural: social security numbers (SSNs)
 
-5. Math
-Z ∞
-
-2
-
-exp−x dx
-
-(1)
-
-0
-
-a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t, u, v, w, x, y, z, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9
-(2)
-R∞
-2
-• Inline: 0 exp−x dx
-• Block: Equation 1, Equation 2
-• Commands defined in body (P[x in X]): P[x ∈ X ]
-• Aligned:
-x=1
-x + y = 10
-x + y + z = 100
-
-6. Links
-• Section: Section 1, Section 1.2
-• Appendix section: Section B, Section A.1.1
-• Appendix figure: Figure A5
-• Appendix table: Table B1
-• Appendix math: Equation 4
-• Short citation [²]
-
-¹ Example footnote text.
-
-7. Tables
-• Table 1
-• Table 2
-
 Col1
 
 Col2
 
 Col3
 
 Col4
@@ -260,14 +235,44 @@
 
 4
 44
 444
 
 Table 1: Short table
 
+5. Math
+Z ∞
+
+2
+
+exp−x dx
+
+0
+
+(1)
+
+8. Figures
+
+a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t, u, v, w, x, y, z, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9
+(2)
+R∞
+2
+• Inline: 0 exp−x dx
+• Block: Equation 1, Equation 2
+• Commands defined in body (P[x in X]): P[x ∈ X ]
+• Aligned:
+x=1
+x + y = 10
+x + y + z = 100
+
+6. Links
+• Section: Section 1, Section 1.2
+• Appendix section: Section B, Section A.1.1
+• Appendix figure: Figure A1
+Figure 2: Narrow figure
 2
 
 A
 B
 C
 D
 E
@@ -293,15 +298,41 @@
 
 74
 
 76
 
 Figure 3: Wide figure
 
-dataset = I
+• Figure 2
+• Figure 3
+• Figure 4, Figure 4a, Figure 4b
+
+9. Includes
+• Commands from metadata include: arg min R
+• Include command in body (there should be text after
+this):
+Content added through include statement.
+
+References
+[1] Donald E. Knuth. The TEX Book. Addison-Wesley Professional, 1986.
+[2] Frank Mittelbach, Michel Gossens, Johannes Braams, David Carlisle,
+and Chris Rowley. The LATEX Companion. Addison-Wesley Professional,
+2 edition, 2004.
+[3] Michael Lesk and Brian Kernighan. Computer typesetting of technical
+journals on UNIX. In Proceedings of American Federation of Information Processing Societies: 1977 National Computer Conference, pages
+879–888, Dallas, Texas, 1977.
+[4] Donald E. Knuth. Literate programming. The Computer Journal, 27(2):
+97–111, 1984.
+
+² Footnote in sub-figure caption.
+³ Footnote in figure caption.
+
+3
+
+dataset = I
 
 dataset = II
 
 dataset = III
 
 dataset = IV
 
@@ -339,44 +370,14 @@
 
 15
 
 (b) Figure with ‘width=3.5in’²
 
 Figure 4: Sub-figures³
 
-3
-
-8. Figures
-
-Figure 2: Narrow figure
-
-• Figure 2
-• Figure 3
-• Figure 4, Figure 4a, Figure 4b
-
-9. Includes
-• Commands from metadata include: arg min R
-• Include command in body (there should be text after
-this):
-Content added through include statement.
-
-References
-[1] Donald E. Knuth. The TEX Book. Addison-Wesley Professional, 1986.
-[2] Frank Mittelbach, Michel Gossens, Johannes Braams, David Carlisle,
-and Chris Rowley. The LATEX Companion. Addison-Wesley Professional,
-2 edition, 2004.
-[3] Michael Lesk and Brian Kernighan. Computer typesetting of technical
-journals on UNIX. In Proceedings of American Federation of Information Processing Societies: 1977 National Computer Conference, pages
-879–888, Dallas, Texas, 1977.
-[4] Donald E. Knuth. Literate programming. The Computer Journal, 27(2):
-97–111, 1984.
-
-² Footnote in sub-figure caption.
-³ Footnote in figure caption.
-
 4
 
 A
 B
 C
 D
 E
@@ -400,15 +401,15 @@
 
 72
 
 74
 
 76
 
-Figure A5: Extra wide figure
+Figure A1: Extra wide figure
 
 Appendix A
 
 Appendix 1
 
 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam nisi purus, bibendum non neque sed, lacinia tristique
 tortor. Vestibulum eu lectus sed velit luctus varius. Sed sollicitudin ligula ante. Integer porta a erat commodo dignissim.
@@ -423,16 +424,16 @@
 Appendix subsubsection
 
 Proin eleifend lorem semper, commodo tellus nec, porta purus.
 Nullam commodo lectus nibh, consequat maximus lorem faucibus in. Nam purus eros, rutrum in sapien et, condimentum
 lacinia nibh.
 
 A.2 Appendix figures
-• Figure A5
-• Figure A6
+• Figure A1
+• Figure A2
 
 A.3 Appendix includes
 • Commands from metadata include (argmin R):
 • Include command in body (there should be text after
 this):
 Content added through include statement.
 
@@ -489,15 +490,15 @@
 
 x
 
 15
 
 (c) Sub-figure
 
-Figure A6: Sub-figures with large combined size.
+Figure A2: Sub-figures with large combined size.
 
 6
 
 Col1
 
 Col2
```

### Comparing `shiny_mdc-1.1.0/test/sections/appendix1.md` & `shiny_mdc-1.2.0/test/sections/appendix1.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/test/sections/appendix2.md` & `shiny_mdc-1.2.0/test/sections/appendix2.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/test/sections/main1.md` & `shiny_mdc-1.2.0/test/sections/main1.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/test/sections/main2.md` & `shiny_mdc-1.2.0/test/sections/main2.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/test/utils/commands.md` & `shiny_mdc-1.2.0/test/utils/commands.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.1.0/PKG-INFO` & `shiny_mdc-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shiny-mdc
-Version: 1.1.0
+Version: 1.2.0
 Summary: Tool to compile markdown files to tex/pdf using pandoc, latexmk
 Home-page: https://github.com/jayanthkoushik/shinymdc
 License: MIT
 Author: Jayanth Koushik
 Author-email: mail@jkoushik.me
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

