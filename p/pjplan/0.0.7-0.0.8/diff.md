# Comparing `tmp/pjplan-0.0.7.tar.gz` & `tmp/pjplan-0.0.8.tar.gz`

## Comparing `pjplan-0.0.7.tar` & `pjplan-0.0.8.tar`

### file list

```diff
@@ -1,107 +1,109 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pjplan-0.0.7/.env
--rwxr-xr-x   0        0        0       79 2020-02-02 00:00:00.000000 pjplan-0.0.7/install.bat
--rwxr-xr-x   0        0        0       56 2020-02-02 00:00:00.000000 pjplan-0.0.7/publish.bat
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 pjplan-0.0.7/.vscode/settings.json
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/Makefile
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/conf.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/index.rst
--rwxr-xr-x   0        0        0      800 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/make.bat
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/modules.rst
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/pjplan.io.rst
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/pjplan.rst
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/pjplan.viz.dhtmlx.rst
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/pjplan.viz.mermaid.rst
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/pjplan.viz.rst
--rw-r--r--   0        0        0   446858 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/doctrees/environment.pickle
--rw-r--r--   0        0        0     5580 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/doctrees/index.doctree
--rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/doctrees/modules.doctree
--rw-r--r--   0        0        0   196365 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/doctrees/pjplan.doctree
--rw-r--r--   0        0        0    33626 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/doctrees/pjplan.io.doctree
--rw-r--r--   0        0        0    22463 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/doctrees/pjplan.viz.dhtmlx.doctree
--rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/doctrees/pjplan.viz.doctree
--rw-r--r--   0        0        0    18945 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/doctrees/pjplan.viz.mermaid.doctree
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/.buildinfo
--rw-r--r--   0        0        0    20224 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/genindex.html
--rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/index.html
--rw-r--r--   0        0        0    19015 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/modules.html
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/objects.inv
--rw-r--r--   0        0        0    75565 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/pjplan.html
--rw-r--r--   0        0        0    14983 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/pjplan.io.html
--rw-r--r--   0        0        0    10720 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/pjplan.viz.dhtmlx.html
--rw-r--r--   0        0        0     7865 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/pjplan.viz.html
--rw-r--r--   0        0        0     9195 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/pjplan.viz.mermaid.html
--rw-r--r--   0        0        0     6010 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/py-modindex.html
--rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/search.html
--rw-r--r--   0        0        0    21596 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/searchindex.js
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_sources/modules.rst.txt
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_sources/pjplan.io.rst.txt
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_sources/pjplan.rst.txt
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_sources/pjplan.viz.dhtmlx.rst.txt
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_sources/pjplan.viz.mermaid.rst.txt
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_sources/pjplan.viz.rst.txt
--rw-r--r--   0        0        0    11932 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_static/alabaster.css
--rw-r--r--   0        0        0    15715 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_static/basic.css
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_static/custom.css
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_static/doctools.js
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_static/file.png
--rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_static/plus.png
--rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_static/pygments.css
--rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_static/searchtools.js
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/README.md
--rw-r--r--   0        0        0    15655 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/jupyter/calendar/calendar.ipynb
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/jupyter/calendar/.ipynb_checkpoints/calendar-checkpoint.ipynb
--rw-r--r--   0        0        0    14430 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/jupyter/critical-path/critical-path.ipynb
--rw-r--r--   0        0        0    93575 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/jupyter/dhtmlx-gantt/dhtmlx-gantt.ipynb
--rw-r--r--   0        0        0    80191 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/jupyter/dhtmlx-gantt/.ipynb_checkpoints/dhtmlx-gantt-checkpoint.ipynb
--rw-r--r--   0        0        0     8977 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/jupyter/forward-scheduler/forward-scheduler.ipynb
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/jupyter/getting-started/getting-started.ipynb
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/jupyter/getting-started/gs.html
--rw-r--r--   0        0        0    10375 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/jupyter/mermaid-gantt/mermaid-gantt.ipynb
--rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/jupyter/mermaid-gantt/.ipynb_checkpoints/mermaid-checkpoint.ipynb
--rw-r--r--   0        0        0     5396 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/jupyter/mermaid-network/mermaid-network.ipynb
--rw-r--r--   0        0        0    12084 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/jupyter/pandas/pandas.ipynb
--rw-r--r--   0        0        0    23893 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/jupyter/print/print.ipynb
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/streamlit/dhtmlx-gantt/main.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/streamlit/dhtmlx-gantt/.streamlit/config.toml
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/streamlit/mermaid-gantt/main.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/streamlit/mermaid-gantt/.streamlit/config.toml
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/streamlit/mermaid-network/main.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/streamlit/mermaid-network/.streamlit/config.toml
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/__init__.py
--rw-r--r--   0        0        0    12226 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/calendar.py
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/resource.py
--rw-r--r--   0        0        0    16734 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/schedule.py
--rw-r--r--   0        0        0    31938 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/task.py
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/utils.py
--rw-r--r--   0        0        0     6372 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/wbs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/alg/__init__.py
--rw-r--r--   0        0        0     4983 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/alg/critical_path.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/io/__init__.py
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/io/csv_io.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/io/raw.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/viz/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/viz/dhtmlx/__init__.py
--rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/viz/dhtmlx/gantt.py
--rw-r--r--   0        0        0     3744 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/viz/dhtmlx/templates/gantt.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/viz/mermaid/__init__.py
--rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/viz/mermaid/gantt.py
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/viz/mermaid/network.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/viz/mermaid/templates/gantt.html
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/viz/mermaid/templates/network.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pjplan-0.0.7/tests/test_pjplan/__init__.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 pjplan-0.0.7/tests/test_pjplan/test_calendar.py
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 pjplan-0.0.7/tests/test_pjplan/test_schedule.py
--rw-r--r--   0        0        0    12361 2020-02-02 00:00:00.000000 pjplan-0.0.7/tests/test_pjplan/test_task.py
--rw-r--r--   0        0        0     9655 2020-02-02 00:00:00.000000 pjplan-0.0.7/tests/test_pjplan/test_wbs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pjplan-0.0.7/tests/test_pjplan/test_io/__init__.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 pjplan-0.0.7/tests/test_pjplan/test_io/test_csv_io.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pjplan-0.0.7/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pjplan-0.0.7/LICENSE
--rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 pjplan-0.0.7/README.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 pjplan-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 pjplan-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pjplan-0.0.8/.env
+-rwxr-xr-x   0        0        0       79 2020-02-02 00:00:00.000000 pjplan-0.0.8/install.bat
+-rwxr-xr-x   0        0        0       56 2020-02-02 00:00:00.000000 pjplan-0.0.8/publish.bat
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 pjplan-0.0.8/.vscode/settings.json
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/Makefile
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/conf.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/index.rst
+-rwxr-xr-x   0        0        0      800 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/make.bat
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/modules.rst
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/pjplan.io.rst
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/pjplan.rst
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/pjplan.viz.dhtmlx.rst
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/pjplan.viz.mermaid.rst
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/pjplan.viz.rst
+-rw-r--r--   0        0        0   446858 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/doctrees/environment.pickle
+-rw-r--r--   0        0        0     5580 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/doctrees/index.doctree
+-rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/doctrees/modules.doctree
+-rw-r--r--   0        0        0   196365 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/doctrees/pjplan.doctree
+-rw-r--r--   0        0        0    33626 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/doctrees/pjplan.io.doctree
+-rw-r--r--   0        0        0    22463 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/doctrees/pjplan.viz.dhtmlx.doctree
+-rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/doctrees/pjplan.viz.doctree
+-rw-r--r--   0        0        0    18945 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/doctrees/pjplan.viz.mermaid.doctree
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/.buildinfo
+-rw-r--r--   0        0        0    20224 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/genindex.html
+-rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/index.html
+-rw-r--r--   0        0        0    19015 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/modules.html
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/objects.inv
+-rw-r--r--   0        0        0    75565 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/pjplan.html
+-rw-r--r--   0        0        0    14983 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/pjplan.io.html
+-rw-r--r--   0        0        0    10720 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/pjplan.viz.dhtmlx.html
+-rw-r--r--   0        0        0     7865 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/pjplan.viz.html
+-rw-r--r--   0        0        0     9195 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/pjplan.viz.mermaid.html
+-rw-r--r--   0        0        0     6010 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/py-modindex.html
+-rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/search.html
+-rw-r--r--   0        0        0    21596 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/searchindex.js
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_sources/modules.rst.txt
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_sources/pjplan.io.rst.txt
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_sources/pjplan.rst.txt
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_sources/pjplan.viz.dhtmlx.rst.txt
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_sources/pjplan.viz.mermaid.rst.txt
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_sources/pjplan.viz.rst.txt
+-rw-r--r--   0        0        0    11932 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_static/alabaster.css
+-rw-r--r--   0        0        0    15715 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_static/basic.css
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_static/custom.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_static/doctools.js
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_static/file.png
+-rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_static/plus.png
+-rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_static/pygments.css
+-rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_static/img/readme/mermaid_gantt.png
+-rw-r--r--   0        0        0    10485 2020-02-02 00:00:00.000000 pjplan-0.0.8/docs/_static/img/readme/mermaid_network.png
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/README.md
+-rw-r--r--   0        0        0    15655 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/jupyter/calendar/calendar.ipynb
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/jupyter/calendar/.ipynb_checkpoints/calendar-checkpoint.ipynb
+-rw-r--r--   0        0        0    14430 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/jupyter/critical-path/critical-path.ipynb
+-rw-r--r--   0        0        0    93575 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/jupyter/dhtmlx-gantt/dhtmlx-gantt.ipynb
+-rw-r--r--   0        0        0    80191 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/jupyter/dhtmlx-gantt/.ipynb_checkpoints/dhtmlx-gantt-checkpoint.ipynb
+-rw-r--r--   0        0        0     8977 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/jupyter/forward-scheduler/forward-scheduler.ipynb
+-rw-r--r--   0        0        0     6005 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/jupyter/getting-started/getting-started.ipynb
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/jupyter/getting-started/gs.html
+-rw-r--r--   0        0        0    10375 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/jupyter/mermaid-gantt/mermaid-gantt.ipynb
+-rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/jupyter/mermaid-gantt/.ipynb_checkpoints/mermaid-checkpoint.ipynb
+-rw-r--r--   0        0        0     5396 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/jupyter/mermaid-network/mermaid-network.ipynb
+-rw-r--r--   0        0        0    12084 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/jupyter/pandas/pandas.ipynb
+-rw-r--r--   0        0        0    23893 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/jupyter/print/print.ipynb
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/streamlit/dhtmlx-gantt/main.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/streamlit/dhtmlx-gantt/.streamlit/config.toml
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/streamlit/mermaid-gantt/main.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/streamlit/mermaid-gantt/.streamlit/config.toml
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/streamlit/mermaid-network/main.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pjplan-0.0.8/examples/streamlit/mermaid-network/.streamlit/config.toml
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/__init__.py
+-rw-r--r--   0        0        0    12226 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/calendar.py
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/resource.py
+-rw-r--r--   0        0        0    16734 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/schedule.py
+-rw-r--r--   0        0        0    31938 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/task.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/utils.py
+-rw-r--r--   0        0        0     6372 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/wbs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/alg/__init__.py
+-rw-r--r--   0        0        0     4983 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/alg/critical_path.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/io/__init__.py
+-rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/io/csv_io.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/io/raw.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/viz/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/viz/dhtmlx/__init__.py
+-rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/viz/dhtmlx/gantt.py
+-rw-r--r--   0        0        0     3744 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/viz/dhtmlx/templates/gantt.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/viz/mermaid/__init__.py
+-rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/viz/mermaid/gantt.py
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/viz/mermaid/network.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/viz/mermaid/templates/gantt.html
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 pjplan-0.0.8/src/pjplan/viz/mermaid/templates/network.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pjplan-0.0.8/tests/test_pjplan/__init__.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 pjplan-0.0.8/tests/test_pjplan/test_calendar.py
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 pjplan-0.0.8/tests/test_pjplan/test_schedule.py
+-rw-r--r--   0        0        0    12361 2020-02-02 00:00:00.000000 pjplan-0.0.8/tests/test_pjplan/test_task.py
+-rw-r--r--   0        0        0     9655 2020-02-02 00:00:00.000000 pjplan-0.0.8/tests/test_pjplan/test_wbs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pjplan-0.0.8/tests/test_pjplan/test_io/__init__.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 pjplan-0.0.8/tests/test_pjplan/test_io/test_csv_io.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pjplan-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pjplan-0.0.8/LICENSE
+-rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 pjplan-0.0.8/README.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 pjplan-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 pjplan-0.0.8/PKG-INFO
```

### Comparing `pjplan-0.0.7/docs/Makefile` & `pjplan-0.0.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/docs/conf.py` & `pjplan-0.0.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/docs/make.bat` & `pjplan-0.0.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/docs/pjplan.io.rst` & `pjplan-0.0.8/docs/pjplan.io.rst`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/docs/pjplan.rst` & `pjplan-0.0.8/docs/pjplan.rst`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/docs/pjplan.viz.mermaid.rst` & `pjplan-0.0.8/docs/pjplan.viz.mermaid.rst`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/docs/_build/doctrees/environment.pickle` & `pjplan-0.0.8/docs/_build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/docs/_build/doctrees/index.doctree` & `pjplan-0.0.8/docs/_build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/docs/_build/doctrees/modules.doctree` & `pjplan-0.0.8/docs/_build/doctrees/modules.doctree`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/docs/_build/doctrees/pjplan.doctree` & `pjplan-0.0.8/docs/_build/doctrees/pjplan.doctree`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/docs/_build/doctrees/pjplan.io.doctree` & `pjplan-0.0.8/docs/_build/doctrees/pjplan.io.doctree`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/docs/_build/doctrees/pjplan.viz.dhtmlx.doctree` & `pjplan-0.0.8/docs/_build/doctrees/pjplan.viz.dhtmlx.doctree`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/docs/_build/doctrees/pjplan.viz.doctree` & `pjplan-0.0.8/docs/_build/doctrees/pjplan.viz.doctree`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/docs/_build/doctrees/pjplan.viz.mermaid.doctree` & `pjplan-0.0.8/docs/_build/doctrees/pjplan.viz.mermaid.doctree`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/docs/_build/html/genindex.html` & `pjplan-0.0.8/docs/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/docs/_build/html/index.html` & `pjplan-0.0.8/docs/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/docs/_build/html/modules.html` & `pjplan-0.0.8/docs/_build/html/modules.html`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/docs/_build/html/objects.inv` & `pjplan-0.0.8/docs/_build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/docs/_build/html/pjplan.html` & `pjplan-0.0.8/docs/_build/html/pjplan.html`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/docs/_build/html/pjplan.io.html` & `pjplan-0.0.8/docs/_build/html/pjplan.io.html`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/docs/_build/html/pjplan.viz.dhtmlx.html` & `pjplan-0.0.8/docs/_build/html/pjplan.viz.dhtmlx.html`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/docs/_build/html/pjplan.viz.html` & `pjplan-0.0.8/docs/_build/html/pjplan.viz.html`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/docs/_build/html/pjplan.viz.mermaid.html` & `pjplan-0.0.8/docs/_build/html/pjplan.viz.mermaid.html`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/docs/_build/html/py-modindex.html` & `pjplan-0.0.8/docs/_build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/docs/_build/html/search.html` & `pjplan-0.0.8/docs/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/docs/_build/html/searchindex.js` & `pjplan-0.0.8/docs/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/docs/_build/html/_sources/pjplan.io.rst.txt` & `pjplan-0.0.8/docs/_build/html/_sources/pjplan.io.rst.txt`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/docs/_build/html/_sources/pjplan.rst.txt` & `pjplan-0.0.8/docs/_build/html/_sources/pjplan.rst.txt`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/docs/_build/html/_sources/pjplan.viz.mermaid.rst.txt` & `pjplan-0.0.8/docs/_build/html/_sources/pjplan.viz.mermaid.rst.txt`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/docs/_build/html/_static/alabaster.css` & `pjplan-0.0.8/docs/_build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/docs/_build/html/_static/basic.css` & `pjplan-0.0.8/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/docs/_build/html/_static/doctools.js` & `pjplan-0.0.8/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/docs/_build/html/_static/language_data.js` & `pjplan-0.0.8/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/docs/_build/html/_static/pygments.css` & `pjplan-0.0.8/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/docs/_build/html/_static/searchtools.js` & `pjplan-0.0.8/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/docs/_build/html/_static/sphinx_highlight.js` & `pjplan-0.0.8/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/examples/jupyter/calendar/calendar.ipynb` & `pjplan-0.0.8/examples/jupyter/calendar/calendar.ipynb`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/examples/jupyter/calendar/.ipynb_checkpoints/calendar-checkpoint.ipynb` & `pjplan-0.0.8/examples/jupyter/calendar/.ipynb_checkpoints/calendar-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/examples/jupyter/critical-path/critical-path.ipynb` & `pjplan-0.0.8/examples/jupyter/critical-path/critical-path.ipynb`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/examples/jupyter/dhtmlx-gantt/dhtmlx-gantt.ipynb` & `pjplan-0.0.8/examples/jupyter/dhtmlx-gantt/dhtmlx-gantt.ipynb`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/examples/jupyter/dhtmlx-gantt/.ipynb_checkpoints/dhtmlx-gantt-checkpoint.ipynb` & `pjplan-0.0.8/examples/jupyter/dhtmlx-gantt/.ipynb_checkpoints/dhtmlx-gantt-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/examples/jupyter/forward-scheduler/forward-scheduler.ipynb` & `pjplan-0.0.8/examples/jupyter/forward-scheduler/forward-scheduler.ipynb`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/examples/jupyter/getting-started/getting-started.ipynb` & `pjplan-0.0.8/examples/jupyter/mermaid-network/mermaid-network.ipynb`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9555324074074074%*

 * *Differences: {"'cells'": "{0: {'metadata': {'ExecuteTime': {'start_time': '2023-04-06T09:23:04.104417Z', "*

 * *            "'end_time': '2023-04-06T09:23:04.114805Z'}}, 'source': {insert: [(2, 'from pjplan "*

 * *            "import Task, WBS, MermaidNetwork')], delete: [3, 1]}}, 1: {'source': ['### Sample "*

 * *            "project']}, 2: {'outputs': [OrderedDict([('data', OrderedDict([('text/plain', "*

 * *            "'\\x1b[92mID   NAME    RESOURCE   ESTIMATE   SPENT   START   END   PREDECESSORS "*

 * *            '\\x1b[0m\\n\\x1b[94m    […]*

```diff
@@ -1,142 +1,137 @@
 {
     "cells": [
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-12T16:47:26.325729Z",
-                    "start_time": "2023-04-12T16:47:26.300177Z"
+                    "end_time": "2023-04-06T09:23:04.114805Z",
+                    "start_time": "2023-04-06T09:23:04.104417Z"
                 },
                 "collapsed": true
             },
             "outputs": [],
             "source": [
                 "import sys\n",
-                "from datetime import datetime\n",
                 "sys.path.append('../../src')\n",
-                "from pjplan import Task, ForwardScheduler, WBS, MermaidGantt, WeeklyCalendar, Resource"
+                "from pjplan import Task, WBS, MermaidNetwork"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
             "source": [
-                "Let's define simple project WBS:"
+                "### Sample project"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-12T16:47:26.338909Z",
-                    "start_time": "2023-04-12T16:47:26.327730Z"
+                    "end_time": "2023-04-06T09:23:04.131807Z",
+                    "start_time": "2023-04-06T09:23:04.116805Z"
                 },
                 "collapsed": false
             },
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": "\u001b[92mID   NAME    RESOURCE   ESTIMATE   SPENT   START   END   PREDECESSORS \u001b[0m\n\u001b[94m     Task 1  Tester     -          -       -       -     []           \u001b[0m\n\u001b[94m     Task 2  Tester     20         -       -       -     [1]          \u001b[0m\n\u001b[94m     Task 3  -          20         -       -       -     [1]          \u001b[0m\n\u001b[94m     Task 4  -          20         -       -       -     [3]          \u001b[0m"
+                    },
+                    "execution_count": 2,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
                 "with WBS() as prj:\n",
-                "  prj // Task(1, 'Task 1', estimate=40, resource='Developer')\n",
-                "  prj // Task(2, 'Task 2', predecessors=[prj[1]], estimate=20, resource='Developer')\n",
-                "  with prj // Task(3, 'Task 3') as t3:\n",
-                "    t3 // Task(4, 'Task 4', predecessors=[prj[2]], estimate=100, resource='Tester')\n",
-                "    t3 // Task(5, 'Task 5', predecessors=[prj[2]], estimate=50, resource='Tester')"
+                "    prj // Task(1, 'Task 1', resource='Tester')\n",
+                "    prj // Task(2, 'Task 2', predecessors=[prj[1]], estimate=20, resource='Tester')\n",
+                "    prj // Task(3, 'Task 3', predecessors=[prj[1]], estimate=20)\n",
+                "    prj // Task(4, 'Task 4', predecessors=[prj[3]], estimate=20)\n",
+                "\n",
+                "prj"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
             "source": [
-                "Let's define resources:"
+                "### Simple diagram"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-12T16:47:26.367929Z",
-                    "start_time": "2023-04-12T16:47:26.339911Z"
+                    "end_time": "2023-04-06T09:23:04.176980Z",
+                    "start_time": "2023-04-06T09:23:04.132807Z"
                 },
                 "collapsed": false
             },
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "text/html": "<iframe srcdoc=\"&lt;html&gt;\n&lt;meta charset=&quot;UTF-8&quot;&gt;\n&lt;body&gt;\n&lt;div class=&quot;mermaid&quot;&gt;\nflowchart LR\n  0((Start)) --&gt; 1{{Task 1}}\n  1{{Task 1}} --&gt; 2{{Task 2}}\n  1{{Task 1}} --&gt; 3{{Task 3}}\n  3{{Task 3}} --&gt; 4{{Task 4}}\n\n&lt;/div&gt;\n\n&lt;script src=&quot;https://cdn.jsdelivr.net/npm/mermaid/dist/mermaid.min.js&quot;&gt;&lt;/script&gt;\n&lt;script&gt;\n    mermaid.ganttConfig = {\n        mirrorActor: true\n    }\n    mermaid.initialize({\n        startOnLoad: true\n    });\n&lt;/script&gt;\n&lt;/body&gt;\n&lt;/html&gt;\" width=\"100%\" height=\"160\" style=\"border:none !important;\" allowfullscreen webkitallowfullscreen mozallowfullscreen></iframe>",
+                        "text/plain": "<pjplan.viz.mermaid.network.MermaidNetwork at 0x2b9ef8e9c00>"
+                    },
+                    "execution_count": 3,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
-                "work_calendar = WeeklyCalendar(days=[0,1,2,3,4], units_per_day=8)\n",
-                "\n",
-                "developer = Resource(name='Developer', calendar=work_calendar)\n",
-                "tester = Resource(name='Tester', calendar=work_calendar)"
+                "MermaidNetwork(prj, height=160)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
             "source": [
-                "Now we can create schedule for out project:"
+                "### Custom bar styles"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-12T16:47:26.374929Z",
-                    "start_time": "2023-04-12T16:47:26.356929Z"
-                },
-                "collapsed": false
-            },
-            "outputs": [],
-            "source": [
-                "schedule = ForwardScheduler(\n",
-                "    start=datetime.now(),\n",
-                "    resources=[developer, tester]\n",
-                ").calc(prj)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
-            "source": [
-                "and visualise it as Mermaid Gantt:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 7,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2023-04-12T16:49:08.897045Z",
-                    "start_time": "2023-04-12T16:49:08.891672Z"
+                    "end_time": "2023-04-06T09:23:04.176980Z",
+                    "start_time": "2023-04-06T09:23:04.148803Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
-                        "text/html": "<iframe srcdoc=\"&lt;html&gt;\n&lt;meta charset=&quot;UTF-8&quot;&gt;\n&lt;body&gt;\n&lt;style&gt;\n\n&lt;/style&gt;\n\n&lt;div class=&quot;mermaid&quot;&gt;\ngantt\n  dateFormat DD.MM.YYYY HH:mm\n    Task 1: active, id_1, 12.04.2023 00:00, 19.04.2023 00:00\n    Task 2:  id_2, 19.04.2023 00:00, 21.04.2023 12:00\n    Task 3:  id_3, 21.04.2023 00:00, 17.05.2023 18:00\n    Task 4:  id_4, 21.04.2023 00:00, 09.05.2023 12:00\n    Task 5:  id_5, 09.05.2023 12:00, 17.05.2023 18:00\n\n&lt;/div&gt;\n\n&lt;script src=&quot;https://cdn.jsdelivr.net/npm/mermaid/dist/mermaid.min.js&quot;&gt;&lt;/script&gt;\n&lt;script&gt;\n    mermaid.ganttConfig = {\n        mirrorActor: true\n    }\n    mermaid.initialize({\n        startOnLoad: true\n    });\n&lt;/script&gt;\n&lt;/body&gt;\n&lt;/html&gt;\" width=\"100%\" height=\"300\" style=\"border:none !important;\" allowfullscreen webkitallowfullscreen mozallowfullscreen></iframe>",
-                        "text/plain": "<pjplan.viz.mermaid.gantt.MermaidGantt at 0x297e546c880>"
+                        "text/html": "<iframe srcdoc=\"&lt;html&gt;\n&lt;meta charset=&quot;UTF-8&quot;&gt;\n&lt;body&gt;\n&lt;div class=&quot;mermaid&quot;&gt;\nflowchart LR\n  0((Start)) --&gt; 1{{Task 1}}\n  1{{Task 1}} --&gt; 2{{Task 2}}\n  1{{Task 1}} --&gt; 3{{Task 3}}\n  3{{Task 3}} --&gt; 4{{Task 4}}\nstyle 1 fill:#A1FB8E,stroke:#333,stroke-width:4px\nstyle 2 fill:#A1FB8E,stroke:#333,stroke-width:4px\n\n&lt;/div&gt;\n\n&lt;script src=&quot;https://cdn.jsdelivr.net/npm/mermaid/dist/mermaid.min.js&quot;&gt;&lt;/script&gt;\n&lt;script&gt;\n    mermaid.ganttConfig = {\n        mirrorActor: true\n    }\n    mermaid.initialize({\n        startOnLoad: true\n    });\n&lt;/script&gt;\n&lt;/body&gt;\n&lt;/html&gt;\" width=\"100%\" height=\"160\" style=\"border:none !important;\" allowfullscreen webkitallowfullscreen mozallowfullscreen></iframe>",
+                        "text/plain": "<pjplan.viz.mermaid.network.MermaidNetwork at 0x2b9ef99d8d0>"
                     },
-                    "execution_count": 7,
+                    "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "MermaidGantt(schedule.schedule)"
+                "# Change bar style for tasks with resource='Tester'\n",
+                "prj.tasks(resource='Tester').network_bar_style={\n",
+                "    'fill':'#A1FB8E',\n",
+                "    'stroke':'#333',\n",
+                "    'stroke-width':'4px'\n",
+                "}\n",
+                "MermaidNetwork(prj, height=160)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
```

### Comparing `pjplan-0.0.7/examples/jupyter/getting-started/gs.html` & `pjplan-0.0.8/examples/jupyter/getting-started/gs.html`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/examples/jupyter/mermaid-gantt/mermaid-gantt.ipynb` & `pjplan-0.0.8/examples/jupyter/mermaid-gantt/mermaid-gantt.ipynb`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/examples/jupyter/mermaid-gantt/.ipynb_checkpoints/mermaid-checkpoint.ipynb` & `pjplan-0.0.8/examples/jupyter/mermaid-gantt/.ipynb_checkpoints/mermaid-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/examples/jupyter/mermaid-network/mermaid-network.ipynb` & `pjplan-0.0.8/examples/jupyter/getting-started/getting-started.ipynb`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.943515625%*

 * *Differences: {"'cells'": "{0: {'execution_count': 7, 'metadata': {'ExecuteTime': {'start_time': "*

 * *            "'2023-04-12T22:17:18.306151Z', 'end_time': '2023-04-12T22:17:18.333779Z'}}, 'source': "*

 * *            "{insert: [(1, 'from datetime import datetime\\n'), (3, 'from pjplan import Task, "*

 * *            "ForwardScheduler, WBS, MermaidGantt, WeeklyCalendar, Resource, MermaidNetwork')], "*

 * *            'delete: [2]}}, 3: {\'source\': ["Let\'s define resources:"]}, 4: '*

 * *            "{'execution_count': 9, 'outputs': [], 's […]*

```diff
@@ -1,137 +1,167 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 7,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-06T09:23:04.114805Z",
-                    "start_time": "2023-04-06T09:23:04.104417Z"
+                    "end_time": "2023-04-12T22:17:18.333779Z",
+                    "start_time": "2023-04-12T22:17:18.306151Z"
                 },
                 "collapsed": true
             },
             "outputs": [],
             "source": [
                 "import sys\n",
+                "from datetime import datetime\n",
                 "sys.path.append('../../src')\n",
-                "from pjplan import Task, WBS, MermaidNetwork"
+                "from pjplan import Task, ForwardScheduler, WBS, MermaidGantt, WeeklyCalendar, Resource, MermaidNetwork"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
             "source": [
-                "### Sample project"
+                "Let's define simple project WBS:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 8,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-06T09:23:04.131807Z",
-                    "start_time": "2023-04-06T09:23:04.116805Z"
+                    "end_time": "2023-04-12T22:17:18.352310Z",
+                    "start_time": "2023-04-12T22:17:18.322753Z"
                 },
                 "collapsed": false
             },
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": "\u001b[92mID   NAME    RESOURCE   ESTIMATE   SPENT   START   END   PREDECESSORS \u001b[0m\n\u001b[94m     Task 1  Tester     -          -       -       -     []           \u001b[0m\n\u001b[94m     Task 2  Tester     20         -       -       -     [1]          \u001b[0m\n\u001b[94m     Task 3  -          20         -       -       -     [1]          \u001b[0m\n\u001b[94m     Task 4  -          20         -       -       -     [3]          \u001b[0m"
-                    },
-                    "execution_count": 2,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
                 "with WBS() as prj:\n",
-                "    prj // Task(1, 'Task 1', resource='Tester')\n",
-                "    prj // Task(2, 'Task 2', predecessors=[prj[1]], estimate=20, resource='Tester')\n",
-                "    prj // Task(3, 'Task 3', predecessors=[prj[1]], estimate=20)\n",
-                "    prj // Task(4, 'Task 4', predecessors=[prj[3]], estimate=20)\n",
+                "  prj // Task(1, 'Task 1', estimate=40, resource='Developer')\n",
+                "  prj // Task(2, 'Task 2', predecessors=[prj[1]], estimate=20, resource='Developer')\n",
+                "  with prj // Task(3, 'Task 3') as t3:\n",
+                "    t3 // Task(4, 'Task 4', predecessors=[prj[2]], estimate=100, resource='Tester')\n",
+                "    t3 // Task(5, 'Task 5', predecessors=[prj[2]], estimate=50, resource='Tester')"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {
+                "collapsed": false
+            },
+            "source": [
+                "Let's define resources:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "metadata": {
+                "ExecuteTime": {
+                    "end_time": "2023-04-12T22:17:18.353310Z",
+                    "start_time": "2023-04-12T22:17:18.336788Z"
+                },
+                "collapsed": false
+            },
+            "outputs": [],
+            "source": [
+                "work_calendar = WeeklyCalendar(days=[0,1,2,3,4], units_per_day=8)\n",
                 "\n",
-                "prj"
+                "developer = Resource(name='Developer', calendar=work_calendar)\n",
+                "tester = Resource(name='Tester', calendar=work_calendar)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
             "source": [
-                "### Simple diagram"
+                "Now we can create schedule for out project:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 10,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-06T09:23:04.176980Z",
-                    "start_time": "2023-04-06T09:23:04.132807Z"
+                    "end_time": "2023-04-12T22:17:18.366308Z",
+                    "start_time": "2023-04-12T22:17:18.352310Z"
                 },
                 "collapsed": false
             },
-            "outputs": [
-                {
-                    "data": {
-                        "text/html": "<iframe srcdoc=\"&lt;html&gt;\n&lt;meta charset=&quot;UTF-8&quot;&gt;\n&lt;body&gt;\n&lt;div class=&quot;mermaid&quot;&gt;\nflowchart LR\n  0((Start)) --&gt; 1{{Task 1}}\n  1{{Task 1}} --&gt; 2{{Task 2}}\n  1{{Task 1}} --&gt; 3{{Task 3}}\n  3{{Task 3}} --&gt; 4{{Task 4}}\n\n&lt;/div&gt;\n\n&lt;script src=&quot;https://cdn.jsdelivr.net/npm/mermaid/dist/mermaid.min.js&quot;&gt;&lt;/script&gt;\n&lt;script&gt;\n    mermaid.ganttConfig = {\n        mirrorActor: true\n    }\n    mermaid.initialize({\n        startOnLoad: true\n    });\n&lt;/script&gt;\n&lt;/body&gt;\n&lt;/html&gt;\" width=\"100%\" height=\"160\" style=\"border:none !important;\" allowfullscreen webkitallowfullscreen mozallowfullscreen></iframe>",
-                        "text/plain": "<pjplan.viz.mermaid.network.MermaidNetwork at 0x2b9ef8e9c00>"
-                    },
-                    "execution_count": 3,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
-                "MermaidNetwork(prj, height=160)"
+                "schedule = ForwardScheduler(\n",
+                "    start=datetime.now(),\n",
+                "    resources=[developer, tester]\n",
+                ").calc(prj)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
             "source": [
-                "### Custom bar styles"
+                "and visualise it as Mermaid Gantt:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 11,
+            "metadata": {
+                "ExecuteTime": {
+                    "end_time": "2023-04-12T22:17:18.399521Z",
+                    "start_time": "2023-04-12T22:17:18.369309Z"
+                },
+                "collapsed": false
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/html": "<iframe srcdoc=\"&lt;html&gt;\n&lt;meta charset=&quot;UTF-8&quot;&gt;\n&lt;body&gt;\n&lt;style&gt;\n\n&lt;/style&gt;\n\n&lt;div class=&quot;mermaid&quot;&gt;\ngantt\n  dateFormat DD.MM.YYYY HH:mm\n  todayMarker off    Task 1: active, id_1, 12.04.2023 00:00, 19.04.2023 00:00\n    Task 2:  id_2, 19.04.2023 00:00, 21.04.2023 12:00\n    Task 3:  id_3, 21.04.2023 00:00, 17.05.2023 18:00\n    Task 4:  id_4, 21.04.2023 00:00, 09.05.2023 12:00\n    Task 5:  id_5, 09.05.2023 12:00, 17.05.2023 18:00\n\n&lt;/div&gt;\n\n&lt;script src=&quot;https://cdn.jsdelivr.net/npm/mermaid/dist/mermaid.min.js&quot;&gt;&lt;/script&gt;\n&lt;script&gt;\n    mermaid.ganttConfig = {\n        mirrorActor: true\n    }\n    mermaid.initialize({\n        startOnLoad: true\n    });\n&lt;/script&gt;\n&lt;/body&gt;\n&lt;/html&gt;\" width=\"100%\" height=\"300\" style=\"border:none !important;\" allowfullscreen webkitallowfullscreen mozallowfullscreen></iframe>",
+                        "text/plain": "<pjplan.viz.mermaid.gantt.MermaidGantt at 0x1c2da3f39d0>"
+                    },
+                    "execution_count": 11,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "MermaidGantt(schedule.schedule)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 12,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-06T09:23:04.176980Z",
-                    "start_time": "2023-04-06T09:23:04.148803Z"
+                    "end_time": "2023-04-12T22:17:18.399521Z",
+                    "start_time": "2023-04-12T22:17:18.383519Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
-                        "text/html": "<iframe srcdoc=\"&lt;html&gt;\n&lt;meta charset=&quot;UTF-8&quot;&gt;\n&lt;body&gt;\n&lt;div class=&quot;mermaid&quot;&gt;\nflowchart LR\n  0((Start)) --&gt; 1{{Task 1}}\n  1{{Task 1}} --&gt; 2{{Task 2}}\n  1{{Task 1}} --&gt; 3{{Task 3}}\n  3{{Task 3}} --&gt; 4{{Task 4}}\nstyle 1 fill:#A1FB8E,stroke:#333,stroke-width:4px\nstyle 2 fill:#A1FB8E,stroke:#333,stroke-width:4px\n\n&lt;/div&gt;\n\n&lt;script src=&quot;https://cdn.jsdelivr.net/npm/mermaid/dist/mermaid.min.js&quot;&gt;&lt;/script&gt;\n&lt;script&gt;\n    mermaid.ganttConfig = {\n        mirrorActor: true\n    }\n    mermaid.initialize({\n        startOnLoad: true\n    });\n&lt;/script&gt;\n&lt;/body&gt;\n&lt;/html&gt;\" width=\"100%\" height=\"160\" style=\"border:none !important;\" allowfullscreen webkitallowfullscreen mozallowfullscreen></iframe>",
-                        "text/plain": "<pjplan.viz.mermaid.network.MermaidNetwork at 0x2b9ef99d8d0>"
+                        "text/html": "<iframe srcdoc=\"&lt;html&gt;\n&lt;meta charset=&quot;UTF-8&quot;&gt;\n&lt;body&gt;\n&lt;div class=&quot;mermaid&quot;&gt;\nflowchart LR\n  0((Start)) --&gt; 1{{Task 1}}\n  1{{Task 1}} --&gt; 2{{Task 2}}\n  0((Start)) --&gt; 3{{Task 3}}\n  2{{Task 2}} --&gt; 4{{Task 4}}\n  2{{Task 2}} --&gt; 5{{Task 5}}\n\n&lt;/div&gt;\n\n&lt;script src=&quot;https://cdn.jsdelivr.net/npm/mermaid/dist/mermaid.min.js&quot;&gt;&lt;/script&gt;\n&lt;script&gt;\n    mermaid.ganttConfig = {\n        mirrorActor: true\n    }\n    mermaid.initialize({\n        startOnLoad: true\n    });\n&lt;/script&gt;\n&lt;/body&gt;\n&lt;/html&gt;\" width=\"100%\" height=\"300\" style=\"border:none !important;\" allowfullscreen webkitallowfullscreen mozallowfullscreen></iframe>",
+                        "text/plain": "<pjplan.viz.mermaid.network.MermaidNetwork at 0x1c2da3f1f90>"
                     },
-                    "execution_count": 4,
+                    "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "# Change bar style for tasks with resource='Tester'\n",
-                "prj.tasks(resource='Tester').network_bar_style={\n",
-                "    'fill':'#A1FB8E',\n",
-                "    'stroke':'#333',\n",
-                "    'stroke-width':'4px'\n",
-                "}\n",
-                "MermaidNetwork(prj, height=160)"
+                "MermaidNetwork(schedule.schedule)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
```

### Comparing `pjplan-0.0.7/examples/jupyter/pandas/pandas.ipynb` & `pjplan-0.0.8/examples/jupyter/pandas/pandas.ipynb`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/examples/jupyter/print/print.ipynb` & `pjplan-0.0.8/examples/jupyter/print/print.ipynb`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/examples/streamlit/dhtmlx-gantt/main.py` & `pjplan-0.0.8/examples/streamlit/dhtmlx-gantt/main.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/examples/streamlit/mermaid-gantt/main.py` & `pjplan-0.0.8/examples/streamlit/mermaid-gantt/main.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/examples/streamlit/mermaid-network/main.py` & `pjplan-0.0.8/examples/streamlit/mermaid-network/main.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/src/pjplan/__init__.py` & `pjplan-0.0.8/src/pjplan/__init__.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/src/pjplan/calendar.py` & `pjplan-0.0.8/src/pjplan/calendar.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/src/pjplan/resource.py` & `pjplan-0.0.8/src/pjplan/resource.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/src/pjplan/schedule.py` & `pjplan-0.0.8/src/pjplan/schedule.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/src/pjplan/task.py` & `pjplan-0.0.8/src/pjplan/task.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/src/pjplan/utils.py` & `pjplan-0.0.8/src/pjplan/utils.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/src/pjplan/wbs.py` & `pjplan-0.0.8/src/pjplan/wbs.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/src/pjplan/alg/critical_path.py` & `pjplan-0.0.8/src/pjplan/alg/critical_path.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/src/pjplan/io/csv_io.py` & `pjplan-0.0.8/src/pjplan/io/csv_io.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/src/pjplan/io/raw.py` & `pjplan-0.0.8/src/pjplan/io/raw.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/src/pjplan/viz/dhtmlx/gantt.py` & `pjplan-0.0.8/src/pjplan/viz/dhtmlx/gantt.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/src/pjplan/viz/dhtmlx/templates/gantt.html` & `pjplan-0.0.8/src/pjplan/viz/dhtmlx/templates/gantt.html`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/src/pjplan/viz/mermaid/gantt.py` & `pjplan-0.0.8/src/pjplan/viz/mermaid/gantt.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/src/pjplan/viz/mermaid/network.py` & `pjplan-0.0.8/src/pjplan/viz/mermaid/network.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/tests/test_pjplan/test_calendar.py` & `pjplan-0.0.8/tests/test_pjplan/test_calendar.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/tests/test_pjplan/test_schedule.py` & `pjplan-0.0.8/tests/test_pjplan/test_schedule.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/tests/test_pjplan/test_task.py` & `pjplan-0.0.8/tests/test_pjplan/test_task.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/tests/test_pjplan/test_wbs.py` & `pjplan-0.0.8/tests/test_pjplan/test_wbs.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/tests/test_pjplan/test_io/test_csv_io.py` & `pjplan-0.0.8/tests/test_pjplan/test_io/test_csv_io.py`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/LICENSE` & `pjplan-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.7/PKG-INFO` & `pjplan-0.0.8/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pjplan
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python library for plan projects
 Project-URL: Homepage, https://github.com/artem-snopkov/pjplan
 Project-URL: Bug Tracker, https://github.com/artem-snopkov/pjplan/issues
 Author-email: Artem Snopkov <artem.snopkov@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,27 +12,40 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # pjplan: Python library for project schedule and analysis
 
 ## What is it?
 
-**pjplan** turns your Jupyter Notebook into project management software. 
-This Python package gives you a simple API with following possibilities:
-- Describe Work Burndown Structure (WBS) of your project
+**pjplan** turns your [Jupyter Notebook](https://jupyter.org/) into project management software. 
+This Python package gives you a simple API with following features:
+- Describe Work Burn-down Structure (WBS) of your project in code or load it from external source.
+- Manipulate tasks: link them as successors/predecessors, find, delete, reorder, etc. A lot of batch operations are supported via simple commands.
 - Assign resources and estimates to tasks
-- Link tasks each other as successors/predecessors
 - Define work calendars for each resource
 - Calculate project schedule in several ways
-- Calculate critical path
-- Visualize schedule as Gantt diagramm
-- Save/Load your projects to csv files
+- Find critical path
+- Visualize WBS as Gantt or Network diagram
+- Save/Load your WBS to/from csv files
+- Export WBS to [pandas](https://pandas.pydata.org/)
+
+## Why to use it?
+There are several use cases for pjplan:
+- Work with project plan as code with your favourite IDE, VSC, etc.
+- Load tasks data from your tracker (Jira, Asure Devops, Trello, etc.) to pjplan, 
+link/modify/reorder/delete tasks using rich pjplan API, then create schedule and Gantt for them.
+- Create several schedules for same project and find optimal one.
+
+## Where to use it?
+
+**pjplan** created specially for use inside [Jupyter Notebook](https://jupyter.org/) 
+or similar software. All library objects (WBS, Task, Schedule, Calendar) have great visualisations 
+so you can easily work with them in notebooks. 
 
-**pjplan** created specially for use inside Jupyter Notebook or similar software, 
-but of course in can be used in any other python applications.
+But, of course, you can use pjplan in any other python applications.
 
 ## Installation
 
 ```bash
 pip install pjplan
 ```
 
@@ -56,38 +69,44 @@
 
 work_calendar = WeeklyCalendar(days=[0,1,2,3,4], units_per_day=8)
 
 developer = Resource(name='Developer', calendar=work_calendar)
 tester = Resource(name='Tester', calendar=work_calendar)
 ```
 
-Now we can create schedule for out project:
+Now we can create schedule for our project:
 ```python
 from datetime import datetime
 from pjplan import ForwardScheduler
 
 schedule = ForwardScheduler(
     start=datetime.now(), 
     resources=[developer, tester]
 ).calc(prj)
 ```
 
-and visualise it as Mermaid Gantt:
+visualise it as [Mermaid](https://mermaid.js.org/) Gantt:
 ```python
 from pjplan import MermaidGantt
 
 MermaidGantt(schedule.schedule)
 ```
-```mermaid
-gantt
-  dateFormat DD.MM.YYYY HH:mm
-  todayMarker off
-    Task 1: active, id_1, 12.04.2023 00:00, 19.04.2023 00:00
-    Task 2:  id_2, 19.04.2023 00:00, 21.04.2023 12:00
-    Task 3:  id_3, 21.04.2023 00:00, 17.05.2023 18:00
-    Task 4:  id_4, 21.04.2023 00:00, 09.05.2023 12:00
-    Task 5:  id_5, 09.05.2023 12:00, 17.05.2023 18:00
+![Mermaid Gantt](https://raw.githubusercontent.com/artem-snopkov/pjplan/main/docs/_static/img/readme/mermaid_gantt.png)
+
+or Network:
+```python
+from pjplan import MermaidNetwork
+
+MermaidNetwork(schedule.schedule)
+```
+![Mermaid Network](https://raw.githubusercontent.com/artem-snopkov/pjplan/main/docs/_static/img/readme/mermaid_network.png)
+
+save schedule to csv:
+```python
+from pjplan import write_csv
+
+write_csv(schedule.schedule, "schedule.csv")
 ```
 
 ## More examples
 
-More examples you can find at [examples](/examples) directory.
+More examples you can find at [examples](https://github.com/artem-snopkov/pjplan/tree/main/examples) directory.
```

