# Comparing `tmp/hypergraphanalysistoolbox-1.0.10.tar.gz` & `tmp/hypergraphanalysistoolbox-1.0.20.tar.gz`

## Comparing `hypergraphanalysistoolbox-1.0.10.tar` & `hypergraphanalysistoolbox-1.0.20.tar`

### file list

```diff
@@ -1,144 +1,46 @@
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/README.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/requirements.txt
--rw-r--r--   0        0        0     7704 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/HAT/HAT.py
--rw-r--r--   0        0        0    23927 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/HAT/Hypergraph.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/HAT/__init__.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/HAT/conf.rst
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/HAT/draw.py
--rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/HAT/graph.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/HAT/modules.rst
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/HAT/multilinalg.py
--rw-r--r--   0        0        0     4563 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/dist_legacy/hypergraphanalysistoolbox-0.0.1-py3-none-any.whl
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/dist_legacy/hypergraphanalysistoolbox-0.0.1.tar.gz
--rw-r--r--   0        0        0    15624 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/dist_legacy/hypergraphanalysistoolbox-1.0-py3-none-any.whl
--rw-r--r--   0        0        0  3704614 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/dist_legacy/hypergraphanalysistoolbox-1.0.tar.gz
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/HAT.rst
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/Makefile
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/conf.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/control.rst
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/decompositions.rst
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/dev.rst
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/hypergraph.txt
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/index.rst
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/install.rst
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/intro.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/make.bat
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/modules.rst
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/properties.rst
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/ref.rst
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/similarity.rst
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/tutorials.rst
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/visualization.rst
--rw-r--r--   0        0        0   206640 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/doctrees/HAT.doctree
--rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/doctrees/control.doctree
--rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/doctrees/decompositions.doctree
--rw-r--r--   0        0        0     6994 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/doctrees/dev.doctree
--rw-r--r--   0        0        0    81001 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/doctrees/environment.pickle
--rw-r--r--   0        0        0    10543 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/doctrees/index.doctree
--rw-r--r--   0        0        0    12455 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/doctrees/install.doctree
--rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/doctrees/intro.doctree
--rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/doctrees/modules.doctree
--rw-r--r--   0        0        0     6978 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/doctrees/properties.doctree
--rw-r--r--   0        0        0    13930 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/doctrees/ref.doctree
--rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/doctrees/similarity.doctree
--rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/doctrees/tutorials.doctree
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/doctrees/visualization.doctree
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/.buildinfo
--rw-r--r--   0        0        0    68843 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/HAT.html
--rw-r--r--   0        0        0     4181 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/control.html
--rw-r--r--   0        0        0     4845 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/decompositions.html
--rw-r--r--   0        0        0     6147 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/dev.html
--rw-r--r--   0        0        0    11726 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/genindex.html
--rw-r--r--   0        0        0     8803 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/index.html
--rw-r--r--   0        0        0     8167 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/install.html
--rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/intro.html
--rw-r--r--   0        0        0     4784 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/modules.html
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/objects.inv
--rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/properties.html
--rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/py-modindex.html
--rw-r--r--   0        0        0     8747 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/ref.html
--rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/search.html
--rw-r--r--   0        0        0    12996 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/searchindex.js
--rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/similarity.html
--rw-r--r--   0        0        0     6719 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/tutorials.html
--rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/visualization.html
--rw-r--r--   0        0        0    13397 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_images/GC.png
--rw-r--r--   0        0        0    22840 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_images/GH.png
--rw-r--r--   0        0        0    37353 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_images/GL.png
--rw-r--r--   0        0        0    19051 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_images/GS.png
--rw-r--r--   0        0        0     9325 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_images/IncidenceMatrix.png
--rw-r--r--   0        0        0    46892 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_images/index_dyadic_decomp.png
--rw-r--r--   0        0        0     4025 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_modules/index.html
--rw-r--r--   0        0        0    34484 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_modules/HAT/HAT.html
--rw-r--r--   0        0        0    76265 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_modules/HAT/Hypergraph.html
--rw-r--r--   0        0        0    13681 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_modules/HAT/draw.html
--rw-r--r--   0        0        0    16093 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_modules/HAT/multilinalg.html
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_sources/HAT.rst.txt
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_sources/control.rst.txt
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_sources/decompositions.rst.txt
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_sources/dev.rst.txt
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_sources/install.rst.txt
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_sources/intro.rst.txt
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_sources/modules.rst.txt
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_sources/properties.rst.txt
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_sources/ref.rst.txt
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_sources/similarity.rst.txt
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_sources/tutorials.rst.txt
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_sources/visualization.rst.txt
--rw-r--r--   0        0        0    13397 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/GC.png
--rw-r--r--   0        0        0    22840 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/GH.png
--rw-r--r--   0        0        0    37353 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/GL.png
--rw-r--r--   0        0        0    19051 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/GS.png
--rw-r--r--   0        0        0     9325 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/IncidenceMatrix.png
--rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0        0        0    14621 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/basic.css
--rw-r--r--   0        0        0     8171 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/doctools.js
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/file.png
--rw-r--r--   0        0        0    46892 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/index_dyadic_decomp.png
--rw-r--r--   0        0        0   288580 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/jquery-3.6.0.js
--rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/jquery.js
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/plus.png
--rw-r--r--   0        0        0     4819 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/pygments.css
--rw-r--r--   0        0        0    17120 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/searchtools.js
--rw-r--r--   0        0        0    68420 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/underscore-1.13.1.js
--rw-r--r--   0        0        0    19530 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/underscore.js
--rw-r--r--   0        0        0    61976 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/vis.png
--rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/css/badge_only.css
--rw-r--r--   0        0        0   129674 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/css/theme.css
--rw-r--r--   0        0        0    87624 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0        0        0    67312 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0        0        0    86288 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0        0        0    66444 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0   323344 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0        0        0   193308 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0        0        0   309728 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0        0        0   184912 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0        0        0   328412 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0        0        0   195704 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0        0        0   309192 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0        0        0   182708 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/js/badge_only.js
--rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/js/html5shiv.min.js
--rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_build/html/_static/js/theme.js
--rw-r--r--   0        0        0    13397 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_static/GC.png
--rw-r--r--   0        0        0    22840 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_static/GH.png
--rw-r--r--   0        0        0    37353 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_static/GL.png
--rw-r--r--   0        0        0    19051 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_static/GS.png
--rw-r--r--   0        0        0     9325 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_static/IncidenceMatrix.png
--rw-r--r--   0        0        0    46892 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_static/index_dyadic_decomp.png
--rw-r--r--   0        0        0    61976 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/docs/_static/vis.png
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/LICENSE
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/PYPIREADME.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/pyproject.toml
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.10/PKG-INFO
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/README.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/requirements.txt
+-rw-r--r--   0        0        0    15744 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/HAT/HAT.py
+-rw-r--r--   0        0        0    23930 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/HAT/Hypergraph.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/HAT/__init__.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/HAT/conf.rst
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/HAT/draw.py
+-rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/HAT/graph.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/HAT/modules.rst
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/HAT/multilinalg.py
+-rw-r--r--   0        0        0   926960 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/HAT/data/aminer_cocitation.mat
+-rw-r--r--   0        0        0  1557832 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/HAT/data/aminer_coreference.mat
+-rw-r--r--   0        0        0   108408 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/HAT/data/citeseer_cocitation.mat
+-rw-r--r--   0        0        0   119824 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/HAT/data/citeseer_coreference.mat
+-rw-r--r--   0        0        0    61488 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/HAT/data/cora_cocitation.mat
+-rw-r--r--   0        0        0    59008 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/HAT/data/cora_coreference.mat
+-rw-r--r--   0        0        0   183176 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/HAT/data/dblp.mat
+-rw-r--r--   0        0        0     4563 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/dist_legacy/hypergraphanalysistoolbox-0.0.1-py3-none-any.whl
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/dist_legacy/hypergraphanalysistoolbox-0.0.1.tar.gz
+-rw-r--r--   0        0        0    15624 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/dist_legacy/hypergraphanalysistoolbox-1.0-py3-none-any.whl
+-rw-r--r--   0        0        0    15643 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/dist_legacy/hypergraphanalysistoolbox-1.0.1-py3-none-any.whl
+-rw-r--r--   0        0        0  3704706 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/dist_legacy/hypergraphanalysistoolbox-1.0.1.tar.gz
+-rw-r--r--   0        0        0  3704614 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/dist_legacy/hypergraphanalysistoolbox-1.0.tar.gz
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/docs/HAT.rst
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/docs/Makefile
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/docs/conf.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/docs/control.rst
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/docs/data.rst
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/docs/decompositions.rst
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/docs/dev.rst
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/docs/hypergraph.txt
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/docs/index.rst
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/docs/install.rst
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/docs/intro.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/docs/make.bat
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/docs/modules.rst
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/docs/properties.rst
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/docs/ref.rst
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/docs/similarity.rst
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/docs/tutorials.rst
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/docs/visualization.rst
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/LICENSE
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/PYPIREADME.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/pyproject.toml
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 hypergraphanalysistoolbox-1.0.20/PKG-INFO
```

### Comparing `hypergraphanalysistoolbox-1.0.10/HAT/Hypergraph.py` & `hypergraphanalysistoolbox-1.0.20/HAT/Hypergraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         ``HAT.draw.incidencePlot``, but is provided to generate the plot directly from the object.
 
         :param shadeRows: shade rows (bool)
         :param connectNodes: connect nodes in each hyperedge (bool)
         :param dpi: the resolution of the image (int)
         :param edgeColors: The colors of edges represented in the incidence matrix. This is random by default
         
-        :return: ``matplotlib`` axes with figure drawn on to it
+        :return: *matplotlib* axes with figure drawn on to it
         """
         # Auth: Joshua Pickard
         #       jpic@umich.edu
         # Date: Nov 30, 2022
         return HAT.draw.incidencePlot(self, shadeRows=shadeRows, connectNodes=connectNodes, dpi=dpi, edgeColors=edgeColors)
         
     def dual(self):
@@ -104,15 +104,15 @@
         #       jpic@umich.edu
         # Date: Nov 30, 2022
         edgeOrder = np.sum(self.IM, axis=0)
         M = np.zeros((len(edgeOrder),len(edgeOrder)))
         np.fill_diagonal(M, self.edgeWeights)
         A = self.IM @ M @ self.IM.T
         np.fill_diagonal(A,0) # Omit self loops
-        return nx.from_numpy_matrix(A)
+        return nx.from_numpy_array(A)
 
     def lineGraph(self):
         """The line graph, which is the clique expansion of the dual graph, is constructed.
         
         :return: Line graph
         :rtype: *networkx.graph*
 
@@ -146,15 +146,15 @@
         # Auth: Joshua Pickard
         #       jpic@umich.edu
         # Date: Nov 30, 2022
         n = len(self.IM) + len(self.IM[0])
         A = np.zeros((n,n))
         A[len(A) - len(self.IM):len(A),0:len(self.IM[0])] = self.IM
         A[0:len(self.IM[0]),len(A) - len(self.IM):len(A)] = self.IM.T
-        return nx.from_numpy_matrix(A)
+        return nx.from_numpy_array(A)
     
     def laplacianMatrix(self, type='Bolla'):
         """This function returns a version of the higher order Laplacian matrix of the hypergraph.
 
         :param type: Indicates which version of the Laplacin matrix to return. It defaults to ``Bolla`` [1], but ``Rodriguez`` [2,3] and ``Zhou`` [4] are valid arguments as well.
         :type type: str, optional
         :return: Laplacian matrix
@@ -287,15 +287,15 @@
     def degreeTensor(self):
         """This constructs the degree tensor for uniform hypergraphs.
         
         :return: Degree Tensor
         :rtype: *ndarray*
 
         The degree tensor :math:`D` is the hypergraph analog of the degree matrix. For a :math:`k-` order hypergraph
-         :math:`H=(V,E)` the degree tensor :math:`D` is a diagonal supersymmetric tensor defined
+        :math:`H=(V,E)` the degree tensor :math:`D` is a diagonal supersymmetric tensor defined
 
         .. math::
             D \in \mathbf{R}^{ \overbrace{n \\times \dots \\times n}^{k \\text{ times}}} \\text{ where }{D}_{i\dots i} = degree(v_i) \\text{ for all } v_i\in V
 
         References
         ----------
         .. [1] C. Chen and I. Rajapakse, Tensor Entropy for Uniform Hypergraphs, IEEE TRANSACTIONS ON NETWORK SCIENCE AND ENGINEERING (2020)
@@ -359,16 +359,16 @@
         _, S, _ = mla.hosvd(L, M=False, uniform=True)
         return sp.stats.entropy(S)
     
     def matrixEntropy(self, type='Rodriguez'):
         """Computes hypergraph entropy based on the eigenvalues values of the Laplacian matrix.
 
         :param type: Type of hypergraph Laplacian matrix. This defaults to 'Rodriguez' and other
-            choices inclue 'Bolla' and 'Zhou' (See: ``laplacianMatrix()``).
-        :type type: str, optional
+            choices inclue ``Bolla`` and ``Zhou`` (See: ``laplacianMatrix()``).
+        :type type: *str, optional*
         :return: Matrix based hypergraph entropy
         :rtype: *float*
 
         Matrix entropy of a hypergraph is defined as the entropy of the eigenvalues of the
         hypergraph Laplacian matrix [1]. This may be applied to any version of the Laplacian matrix.
 
         References
@@ -383,15 +383,15 @@
         U, V = np.linalg.eig(L)
         return sp.stats.entropy(U)
     
     def avgDistance(self):
         """Computes the average pairwise distance between any 2 vertices in the hypergraph.
 
         :return: avgDist
-        :rtype: float
+        :rtype: *float*
 
         The hypergraph is clique expanded to a graph object, and the average shortest path on
         the clique expanded graph is returned.
         """
         # Auth: Joshua Pickard
         #       jpic@umich.edu
         # Date: Nov 30, 2022
```

### Comparing `hypergraphanalysistoolbox-1.0.10/HAT/draw.py` & `hypergraphanalysistoolbox-1.0.20/HAT/draw.py`

 * *Files identical despite different names*

### Comparing `hypergraphanalysistoolbox-1.0.10/HAT/graph.py` & `hypergraphanalysistoolbox-1.0.20/HAT/graph.py`

 * *Files identical despite different names*

### Comparing `hypergraphanalysistoolbox-1.0.10/HAT/multilinalg.py` & `hypergraphanalysistoolbox-1.0.20/HAT/multilinalg.py`

 * *Files identical despite different names*

### Comparing `hypergraphanalysistoolbox-1.0.10/dist_legacy/hypergraphanalysistoolbox-0.0.1-py3-none-any.whl` & `hypergraphanalysistoolbox-1.0.20/dist_legacy/hypergraphanalysistoolbox-0.0.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `hypergraphanalysistoolbox-1.0.10/dist_legacy/hypergraphanalysistoolbox-0.0.1.tar.gz` & `hypergraphanalysistoolbox-1.0.20/dist_legacy/hypergraphanalysistoolbox-0.0.1.tar.gz`

 * *Files identical despite different names*

### Comparing `hypergraphanalysistoolbox-1.0.10/dist_legacy/hypergraphanalysistoolbox-1.0-py3-none-any.whl` & `hypergraphanalysistoolbox-1.0.20/dist_legacy/hypergraphanalysistoolbox-1.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `hypergraphanalysistoolbox-1.0.10/dist_legacy/hypergraphanalysistoolbox-1.0.tar.gz` & `hypergraphanalysistoolbox-1.0.20/dist_legacy/hypergraphanalysistoolbox-1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `hypergraphanalysistoolbox-1.0.10/docs/HAT.rst` & `hypergraphanalysistoolbox-1.0.20/docs/HAT.rst`

 * *Files identical despite different names*

### Comparing `hypergraphanalysistoolbox-1.0.10/docs/Makefile` & `hypergraphanalysistoolbox-1.0.20/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hypergraphanalysistoolbox-1.0.10/docs/conf.py` & `hypergraphanalysistoolbox-1.0.20/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hypergraphanalysistoolbox-1.0.10/docs/dev.rst` & `hypergraphanalysistoolbox-1.0.20/docs/dev.rst`

 * *Files identical despite different names*

### Comparing `hypergraphanalysistoolbox-1.0.10/docs/index.rst` & `hypergraphanalysistoolbox-1.0.20/docs/index.rst`

 * *Files 7% similar despite different names*

```diff
@@ -19,32 +19,33 @@
 1. Construction
 2. Visualization
 3. Expansion and numeric representation
 4. Structral Properties
 5. Controllability
 6. Similarity Measures
 
-The capabilities and use cases of HAT are outlined in `this short notice <https://drive.google.com/file/d/1Mx8ifUtjR05ufhTXc5QgYKlwmfQjfItv/view?usp=share_link>`_. 
+The capabilities and use cases of HAT are outlined in `this notice <https://arxiv.org/pdf/2211.11166.pdf>`_. 
 
 Contributors
 ************
-Joshua Pickard, Can Chen, Rahmy Salman, Cooper Stansbury, Sion Kim, Amit Surana, and Indika Rajapakse
+Joshua Pickard, Can Chen, Rahmy Salman, Cooper Stansbury, Sion Kim, Amit Surana, Anthony Bloch, and Indika Rajapakse
 
 Bug Reporting
 -------------
 Please report all bugs or defects in HAT to `this page <https://github.com/Jpickard1/Hypergraph-Analysis-Toolbox/issues>`_.
 
 
 .. toctree::
    :maxdepth: 2
    :caption: Contents:
 
    install.rst
    tutorials.rst
    HAT.rst
+   data.rst
    ref.rst
    dev.rst
 
 Indices and tables
 ==================
 
 * :ref:`genindex`
```

### Comparing `hypergraphanalysistoolbox-1.0.10/docs/install.rst` & `hypergraphanalysistoolbox-1.0.20/docs/install.rst`

 * *Files identical despite different names*

### Comparing `hypergraphanalysistoolbox-1.0.10/docs/make.bat` & `hypergraphanalysistoolbox-1.0.20/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hypergraphanalysistoolbox-1.0.10/docs/properties.rst` & `hypergraphanalysistoolbox-1.0.20/docs/properties.rst`

 * *Files identical despite different names*

### Comparing `hypergraphanalysistoolbox-1.0.10/docs/ref.rst` & `hypergraphanalysistoolbox-1.0.20/docs/ref.rst`

 * *Files identical despite different names*

### Comparing `hypergraphanalysistoolbox-1.0.10/docs/tutorials.rst` & `hypergraphanalysistoolbox-1.0.20/docs/tutorials.rst`

 * *Files identical despite different names*

### Comparing `hypergraphanalysistoolbox-1.0.10/LICENSE` & `hypergraphanalysistoolbox-1.0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `hypergraphanalysistoolbox-1.0.10/PYPIREADME.md` & `hypergraphanalysistoolbox-1.0.20/PYPIREADME.md`

 * *Files identical despite different names*

### Comparing `hypergraphanalysistoolbox-1.0.10/pyproject.toml` & `hypergraphanalysistoolbox-1.0.20/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "HypergraphAnalysisToolbox"
-version = "1.0.10"
+version = "1.0.20"
 authors = [
   { name="Joshua Pickard", email="jpic@umich.edu" },
 ]
 description = "This package performes hypergraph analysis."
 readme = "PYPIREADME.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `hypergraphanalysistoolbox-1.0.10/PKG-INFO` & `hypergraphanalysistoolbox-1.0.20/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HypergraphAnalysisToolbox
-Version: 1.0.10
+Version: 1.0.20
 Summary: This package performes hypergraph analysis.
 Project-URL: Homepage, https://hypergraph-analysis-toolbox.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/Jpickard1/Hypergraph-Analysis-Toolbox/issues
 Author-email: Joshua Pickard <jpic@umich.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

