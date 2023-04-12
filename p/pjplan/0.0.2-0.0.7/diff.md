# Comparing `tmp/pjplan-0.0.2.tar.gz` & `tmp/pjplan-0.0.7.tar.gz`

## Comparing `pjplan-0.0.2.tar` & `pjplan-0.0.7.tar`

### file list

```diff
@@ -1,27 +1,107 @@
--rwxr-xr-x   0        0        0       79 2020-02-02 00:00:00.000000 pjplan-0.0.2/install.bat
--rwxr-xr-x   0        0        0       56 2020-02-02 00:00:00.000000 pjplan-0.0.2/publish.bat
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 pjplan-0.0.2/src/pjplan/__init__.py
--rw-r--r--   0        0        0     3840 2020-02-02 00:00:00.000000 pjplan-0.0.2/src/pjplan/calendar.py
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 pjplan-0.0.2/src/pjplan/resource.py
--rw-r--r--   0        0        0     8333 2020-02-02 00:00:00.000000 pjplan-0.0.2/src/pjplan/schedule.py
--rw-r--r--   0        0        0    18055 2020-02-02 00:00:00.000000 pjplan-0.0.2/src/pjplan/wbs.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pjplan-0.0.2/src/pjplan/io/__init__.py
--rw-r--r--   0        0        0     3813 2020-02-02 00:00:00.000000 pjplan-0.0.2/src/pjplan/io/csv_io.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 pjplan-0.0.2/src/pjplan/io/df_io.py
--rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 pjplan-0.0.2/src/pjplan/io/raw.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pjplan-0.0.2/src/pjplan/viz/__init__.py
--rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 pjplan-0.0.2/src/pjplan/viz/mermaid.py
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 pjplan-0.0.2/src/pjplan/viz/tasksheet.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pjplan-0.0.2/src/pjplan/viz/dhtmlx/__init__.py
--rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 pjplan-0.0.2/src/pjplan/viz/dhtmlx/dhtmlx.py
--rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 pjplan-0.0.2/src/pjplan/viz/dhtmlx/templates/gantt.html
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 pjplan-0.0.2/tests/test_pjplan/test_schedule.py
--rw-r--r--   0        0        0     7777 2020-02-02 00:00:00.000000 pjplan-0.0.2/tests/test_pjplan/test_task.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 pjplan-0.0.2/tests/test_pjplan/test_wbs.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 pjplan-0.0.2/tests/test_pjplan/io/test_csv_io.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 pjplan-0.0.2/tests/test_pjplan/viz/test_tasksheet.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 pjplan-0.0.2/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pjplan-0.0.2/LICENSE
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pjplan-0.0.2/README.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 pjplan-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 pjplan-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pjplan-0.0.7/.env
+-rwxr-xr-x   0        0        0       79 2020-02-02 00:00:00.000000 pjplan-0.0.7/install.bat
+-rwxr-xr-x   0        0        0       56 2020-02-02 00:00:00.000000 pjplan-0.0.7/publish.bat
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 pjplan-0.0.7/.vscode/settings.json
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/Makefile
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/conf.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/index.rst
+-rwxr-xr-x   0        0        0      800 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/make.bat
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/modules.rst
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/pjplan.io.rst
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/pjplan.rst
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/pjplan.viz.dhtmlx.rst
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/pjplan.viz.mermaid.rst
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/pjplan.viz.rst
+-rw-r--r--   0        0        0   446858 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/doctrees/environment.pickle
+-rw-r--r--   0        0        0     5580 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/doctrees/index.doctree
+-rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/doctrees/modules.doctree
+-rw-r--r--   0        0        0   196365 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/doctrees/pjplan.doctree
+-rw-r--r--   0        0        0    33626 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/doctrees/pjplan.io.doctree
+-rw-r--r--   0        0        0    22463 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/doctrees/pjplan.viz.dhtmlx.doctree
+-rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/doctrees/pjplan.viz.doctree
+-rw-r--r--   0        0        0    18945 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/doctrees/pjplan.viz.mermaid.doctree
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/.buildinfo
+-rw-r--r--   0        0        0    20224 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/genindex.html
+-rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/index.html
+-rw-r--r--   0        0        0    19015 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/modules.html
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/objects.inv
+-rw-r--r--   0        0        0    75565 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/pjplan.html
+-rw-r--r--   0        0        0    14983 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/pjplan.io.html
+-rw-r--r--   0        0        0    10720 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/pjplan.viz.dhtmlx.html
+-rw-r--r--   0        0        0     7865 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/pjplan.viz.html
+-rw-r--r--   0        0        0     9195 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/pjplan.viz.mermaid.html
+-rw-r--r--   0        0        0     6010 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/py-modindex.html
+-rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/search.html
+-rw-r--r--   0        0        0    21596 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/searchindex.js
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_sources/modules.rst.txt
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_sources/pjplan.io.rst.txt
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_sources/pjplan.rst.txt
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_sources/pjplan.viz.dhtmlx.rst.txt
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_sources/pjplan.viz.mermaid.rst.txt
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_sources/pjplan.viz.rst.txt
+-rw-r--r--   0        0        0    11932 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_static/alabaster.css
+-rw-r--r--   0        0        0    15715 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_static/basic.css
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_static/custom.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_static/doctools.js
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_static/file.png
+-rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_static/plus.png
+-rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_static/pygments.css
+-rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 pjplan-0.0.7/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/README.md
+-rw-r--r--   0        0        0    15655 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/jupyter/calendar/calendar.ipynb
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/jupyter/calendar/.ipynb_checkpoints/calendar-checkpoint.ipynb
+-rw-r--r--   0        0        0    14430 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/jupyter/critical-path/critical-path.ipynb
+-rw-r--r--   0        0        0    93575 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/jupyter/dhtmlx-gantt/dhtmlx-gantt.ipynb
+-rw-r--r--   0        0        0    80191 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/jupyter/dhtmlx-gantt/.ipynb_checkpoints/dhtmlx-gantt-checkpoint.ipynb
+-rw-r--r--   0        0        0     8977 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/jupyter/forward-scheduler/forward-scheduler.ipynb
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/jupyter/getting-started/getting-started.ipynb
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/jupyter/getting-started/gs.html
+-rw-r--r--   0        0        0    10375 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/jupyter/mermaid-gantt/mermaid-gantt.ipynb
+-rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/jupyter/mermaid-gantt/.ipynb_checkpoints/mermaid-checkpoint.ipynb
+-rw-r--r--   0        0        0     5396 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/jupyter/mermaid-network/mermaid-network.ipynb
+-rw-r--r--   0        0        0    12084 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/jupyter/pandas/pandas.ipynb
+-rw-r--r--   0        0        0    23893 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/jupyter/print/print.ipynb
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/streamlit/dhtmlx-gantt/main.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/streamlit/dhtmlx-gantt/.streamlit/config.toml
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/streamlit/mermaid-gantt/main.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/streamlit/mermaid-gantt/.streamlit/config.toml
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/streamlit/mermaid-network/main.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pjplan-0.0.7/examples/streamlit/mermaid-network/.streamlit/config.toml
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/__init__.py
+-rw-r--r--   0        0        0    12226 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/calendar.py
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/resource.py
+-rw-r--r--   0        0        0    16734 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/schedule.py
+-rw-r--r--   0        0        0    31938 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/task.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/utils.py
+-rw-r--r--   0        0        0     6372 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/wbs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/alg/__init__.py
+-rw-r--r--   0        0        0     4983 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/alg/critical_path.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/io/__init__.py
+-rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/io/csv_io.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/io/raw.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/viz/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/viz/dhtmlx/__init__.py
+-rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/viz/dhtmlx/gantt.py
+-rw-r--r--   0        0        0     3744 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/viz/dhtmlx/templates/gantt.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/viz/mermaid/__init__.py
+-rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/viz/mermaid/gantt.py
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/viz/mermaid/network.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/viz/mermaid/templates/gantt.html
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 pjplan-0.0.7/src/pjplan/viz/mermaid/templates/network.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pjplan-0.0.7/tests/test_pjplan/__init__.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 pjplan-0.0.7/tests/test_pjplan/test_calendar.py
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 pjplan-0.0.7/tests/test_pjplan/test_schedule.py
+-rw-r--r--   0        0        0    12361 2020-02-02 00:00:00.000000 pjplan-0.0.7/tests/test_pjplan/test_task.py
+-rw-r--r--   0        0        0     9655 2020-02-02 00:00:00.000000 pjplan-0.0.7/tests/test_pjplan/test_wbs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pjplan-0.0.7/tests/test_pjplan/test_io/__init__.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 pjplan-0.0.7/tests/test_pjplan/test_io/test_csv_io.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pjplan-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pjplan-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 pjplan-0.0.7/README.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 pjplan-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 pjplan-0.0.7/PKG-INFO
```

### Comparing `pjplan-0.0.2/src/pjplan/__init__.py` & `pjplan-0.0.7/src/pjplan/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Пакет содержит API для работы с проектами и расписаниями задач.
 """
 from pjplan.wbs import Task, WBS
-from pjplan.calendar import IWorkCalendar, GenericCalendar, CapacityCalendar, DEFAULT_CALENDAR
+from pjplan.calendar import IWorkCalendar, WeeklyCalendar, DirectCalendar, FixedCalendar, DEFAULT_CALENDAR
 from pjplan.resource import IResource, Resource, DEFAULT_RESOURCE
-from pjplan.schedule import DefaultScheduler, Sprint
+from pjplan.schedule import ForwardScheduler, BackwardScheduler
 from pjplan.io import TaskRaw
-from pjplan.io.df_io import to_df
 from pjplan.io.csv_io import read_csv, write_csv
-from pjplan.viz.tasksheet import task_sheet
-from pjplan.viz.dhtmlx.dhtmlx import DhtmlxTemplate
-from pjplan.viz.mermaid import mermaid_gantt, mermaid_network_diagram
+from pjplan.viz.dhtmlx.gantt import DhtmlxGantt, DhtmlxGanttColumn
+from pjplan.viz.mermaid.gantt import MermaidGantt
+from pjplan.viz.mermaid.network import MermaidNetwork
```

### Comparing `pjplan-0.0.2/src/pjplan/resource.py` & `pjplan-0.0.7/src/pjplan/resource.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,90 +1,84 @@
 from abc import ABC, abstractmethod
 from datetime import datetime, timedelta
-from typing import List, Tuple, Optional
 
 from pjplan import IWorkCalendar, DEFAULT_CALENDAR
 
 
 class IResource(ABC):
     """Ресурс - человек, машина или любая другая сущность, которая необходима для выполнения работы (Task)"""
 
     def __init__(self, name: str):
         """
         :param name: уникальное название ресурса.
         """
         self.name = name
 
     @abstractmethod
-    def available_hours_for_date(self, date: datetime) -> float:
+    def get_available_units(self, date: datetime) -> float:
         pass
 
-    def get_nearest_availability_date(self, start_date: datetime, max_days=100) -> datetime:
+    def get_nearest_availability_date(self, start_date: datetime, direction: int, max_days=100) -> datetime:
         """
         Возвращает ближайшую дату доступности ресурса, начиная со start_date
+        :param direction: 1 или -1
         :param start_date: дата начала поиска
         :param max_days: максимальный интервал поиска (в днях)
         :return: дата доступности
         """
         step = 0
         while step < max_days:
-            if self.available_hours_for_date(start_date) > 0:
-                return start_date
-            start_date += timedelta(days=1)
+            if direction < 0:
+                if self.get_available_units(start_date - timedelta(days=1)) > 0:
+                    return start_date
+            else:
+                if self.get_available_units(start_date) > 0:
+                    return start_date
+            start_date += timedelta(days=direction)
             step += 1
 
         raise RuntimeError(
-            "Can't find nearest availability time for resource", self.resource,
+            "Can't find nearest availability time for resource", self.name,
             "after", start_date.strftime('%Y-%m-%d')
         )
 
 
 class Resource(IResource):
 
     def __init__(
             self,
             name: str,
-            calendar: IWorkCalendar = DEFAULT_CALENDAR,
-            availability: List[Tuple[datetime, float]] = None
+            calendar: IWorkCalendar = DEFAULT_CALENDAR
     ):
         """
         :param name: уникальное наименование ресурса
         :param calendar: рабочий календарь
-        :param availability: процент доступности ресурса. Задается интервалами.
 
         Пример интервалов доступности:
         availability = [(datetime(2000, 1, 1), 50), (datetime(2000, 2, 1), 100)]
         означает, что:
         1. До 2000-01-01 ресурс недоступен
         2. В период с 2000-01-01 по 2000-02-01 ресурс доступен на 50%
         3. После 2000-02-01 ресурс доступен на 100%
         """
         super().__init__(name)
         self.calendar = calendar
-        self.availability = availability
 
-    def available_hours_for_date(self, date: datetime) -> float:
+    def get_available_units(self, date: datetime) -> float:
         """
         Возвращает количество доступных рабочих часов ресурса в указанную дату
         :param date: дата
         :return: количество доступных часов ресурса
         """
 
-        available_hours = self.calendar.get_available_hours(date)
-        if available_hours == 0:
-            return 0
+        return self.calendar.get_available_units(date)
 
-        # Определяем ближайший интервал доступности ресурса
-        usage: Optional[Tuple[datetime, float]] = None
-        for u in self.availability:
-            if u[0] > date:
-                continue
-            if usage is None or usage[0] < u[0]:
-                usage = u
+    def __str__(self):
+        return self.name
 
-        if usage is None:
-            return 0
+    def __repr__(self):
+        res = f'{self.name}\n'
+        res += self.calendar.__repr__()
+        return res
 
-        return available_hours * usage[1] / 100
 
-
-DEFAULT_RESOURCE = Resource("default", DEFAULT_CALENDAR, [(datetime(1970, 1, 1), 100)])
+DEFAULT_RESOURCE = Resource("default")
```

### Comparing `pjplan-0.0.2/src/pjplan/io/csv_io.py` & `pjplan-0.0.7/src/pjplan/io/csv_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import csv
 from datetime import datetime
-from typing import List, Optional, Iterable
+from typing import List, Optional
 
-from pjplan import Task, WBS
-from pjplan.io.raw import TaskRaw, raws_to_tasks, tasks_to_raws
+from pjplan import WBS
+from pjplan.io.raw import TaskRaw, raws_to_wbs, tasks_to_raws
 
 __DATE_FORMAT = '%d.%m.%y'
 
 
 def __parse_header(row) -> dict:
     res = {}
     for i in range(0, len(row)):
@@ -80,37 +80,38 @@
                     milestone=__parse_bool(row[header['milestone']]),
                     parent_id=__parse_int(row[header['parent_id']]),
                     predecessor_ids=__parse_predecessors(row[header['predecessor_ids']]),
                     **kwargs
                 )
             )
 
-    return WBS(tasks=raws_to_tasks(raws))
+    return raws_to_wbs(raws)
 
 
 def write_csv(wbs: WBS, path: str, encoding='utf-8', delimiter=';'):
-    raws = tasks_to_raws(wbs)
+    raws = tasks_to_raws(wbs.tasks)
 
     with open(path, mode='w', encoding=encoding, newline='\n') as output_file:
         csvwriter = csv.writer(output_file, delimiter=delimiter)
         fields = {}
         for t in raws:
-            for k,v in t.__dict__.items():
+            for k, v in t.__dict__.items():
                 if k not in __DEFAULT_FIELDS:
                     fields[k] = type(v).__name__
         field_list = [f"{k}" for k in fields.keys()]
         csvwriter.writerow(__DEFAULT_FIELDS + field_list)
+
         for task in raws:
             csvwriter.writerow([
                 task.id,
                 task.name if task.name else '',
                 task.resource if task.resource else '',
                 task.start.strftime(__DATE_FORMAT) if task.start is not None else None,
                 task.end.strftime(__DATE_FORMAT) if task.end is not None else None,
                 task.estimate,
                 task.spent,
                 task.milestone,
                 task.parent_id,
                 ';'.join([str(pid) for pid in task.predecessor_ids])
             ] + [
-                task.__getattribute__(k) if k in task.__dict__ else '' for k in field_list
+                task.__getattribute__(k) if k in task.__dict__ and not k.startswith('_') else '' for k in field_list
             ])
```

### Comparing `pjplan-0.0.2/src/pjplan/io/raw.py` & `pjplan-0.0.7/src/pjplan/io/raw.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from datetime import datetime
-from typing import List, Union, Iterable
+from typing import List, Iterable, Any
 
 from pjplan import Task, WBS
-from pjplan.wbs import TaskList
 
 
 class TaskRaw:
     def __init__(
             self,
-            id: int,
+            id: Any,
             name: str,
             resource: str = None,
             start: datetime = None,
             end: datetime = None,
             milestone: bool = False,
             estimate: float = None,
             spent: float = None,
@@ -36,62 +35,54 @@
     def to_dict(self) -> dict:
         res = {}
         for k in self.__dict__.keys():
             res[k] = self.__getattribute__(k)
         return res
 
 
-def tasks_to_raws(tasks: Iterable) -> List[TaskRaw]:
+def tasks_to_raws(tasks: Iterable[Task]) -> List[TaskRaw]:
     raws = []
     for t in tasks:
         raw = TaskRaw(
             id=t.id,
             name=t.name,
             resource=t.resource,
             start=t.start,
             end=t.end,
             estimate=t.estimate,
             spent=t.spent,
             milestone=t.milestone,
             parent_id=t.parent.id if t.parent and t.parent.id != 0 else None,
             predecessor_ids=[p.id for p in t.predecessors]
         )
-        keys_to_gnore = {
-            '_Task__parent',
-            '_Task__children',
-            '_Task__predecessors',
-            '_Task__successors'
-        }
         for k in t.__dict__.keys():
-            if k not in keys_to_gnore and k not in raw.__dict__:
+            if not k.startswith('_') and k not in raw.__dict__:
                 raw.__setattr__(k, t.__getattribute__(k))
 
         raws.append(raw)
 
     return raws
 
 
-def raws_to_tasks(raws: List[TaskRaw]) -> List[Task]:
+def raws_to_wbs(raws: List[TaskRaw]) -> WBS:
     tasks_by_id = {}
     for raw in raws:
         t = Task(
             id=raw.id,
             name=raw.name,
             resource=raw.resource,
             start=raw.start,
             end=raw.end,
             estimate=raw.estimate,
             spent=raw.spent,
-            milestone=raw.milestone,
-            children=[],
-            predecessors=[]
+            milestone=raw.milestone
         )
 
         for k in raw.__dict__.keys():
-            if k not in t.__dict__:
+            if k not in dir(t):
                 t.__setattr__(k, raw.__getattribute__(k))
 
         tasks_by_id[t.id] = t
 
     roots = []
     for raw in raws:
         task = tasks_by_id[raw.id]
@@ -102,13 +93,20 @@
                 parent_task.children.append(task)
                 task.parent = parent_task
             else:
                 roots.append(task)
         else:
             roots.append(task)
 
+    wbs = WBS()
+    for r in roots:
+        wbs.roots.append(r)
+
+    for raw in raws:
+        task = wbs[raw.id]
+
         for predecessor_id in raw.predecessor_ids:
-            predecessor_task = tasks_by_id.get(predecessor_id)
+            predecessor_task = wbs[predecessor_id]
             if predecessor_task is not None:
                 task.predecessors.append(predecessor_task)
 
-    return roots
+    return wbs
```

### Comparing `pjplan-0.0.2/src/pjplan/viz/dhtmlx/templates/gantt.html` & `pjplan-0.0.7/src/pjplan/viz/dhtmlx/templates/gantt.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,279 +1,234 @@
-00000000: 3c73 6372 6970 7420 7372 633d 2268 7474  <script src="htt
-00000010: 7073 3a2f 2f73 746f 7261 6765 2e79 616e  ps://storage.yan
-00000020: 6465 7863 6c6f 7564 2e6e 6574 2f67 796d  dexcloud.net/gym
-00000030: 626f 7373 2d74 6573 742f 6761 6e74 742f  boss-test/gantt/
-00000040: 6761 6e74 742f 6468 746d 6c78 6761 6e74  gantt/dhtmlxgant
-00000050: 742e 6a73 3f76 3d37 2e31 2e31 3322 3e3c  t.js?v=7.1.13"><
-00000060: 2f73 6372 6970 743e 0d0a 3c6c 696e 6b20  /script>..<link 
-00000070: 7265 6c3d 2273 7479 6c65 7368 6565 7422  rel="stylesheet"
-00000080: 2068 7265 663d 2268 7474 7073 3a2f 2f73   href="https://s
-00000090: 746f 7261 6765 2e79 616e 6465 7863 6c6f  torage.yandexclo
-000000a0: 7564 2e6e 6574 2f67 796d 626f 7373 2d74  ud.net/gymboss-t
-000000b0: 6573 742f 6761 6e74 742f 6761 6e74 742f  est/gantt/gantt/
-000000c0: 6468 746d 6c78 6761 6e74 742e 6373 733f  dhtmlxgantt.css?
-000000d0: 763d 372e 312e 3133 223e 0d0a 3c73 7479  v=7.1.13">..<sty
-000000e0: 6c65 3e0d 0a20 2020 2068 746d 6c2c 2062  le>..    html, b
-000000f0: 6f64 7920 7b0d 0a20 2020 2020 2020 2070  ody {..        p
-00000100: 6164 6469 6e67 3a20 3070 783b 0d0a 2020  adding: 0px;..  
-00000110: 2020 2020 2020 6d61 7267 696e 3a20 3070        margin: 0p
-00000120: 783b 0d0a 2020 2020 2020 2020 6865 6967  x;..        heig
-00000130: 6874 3a20 3130 3025 3b0d 0a20 2020 207d  ht: 100%;..    }
-00000140: 0d0a 0d0a 2020 2020 2e69 676e 7573 6172  ....    .ignusar
-00000150: 6b6f 7620 7b0d 0a20 2020 2020 2020 2062  kov {..        b
-00000160: 6163 6b67 726f 756e 643a 2023 3233 3936  ackground: #2396
-00000170: 3464 3b0d 0a20 2020 207d 0d0a 0d0a 2020  4d;..    }....  
-00000180: 2020 2e69 676e 7573 6172 6b6f 7620 2e67    .ignusarkov .g
-00000190: 616e 7474 5f74 6173 6b5f 7072 6f67 7265  antt_task_progre
-000001a0: 7373 207b 0d0a 2020 2020 2020 2020 6261  ss {..        ba
-000001b0: 636b 6772 6f75 6e64 3a20 2332 3337 3834  ckground: #23784
-000001c0: 643b 0d0a 2020 2020 7d0d 0a0d 0a20 2020  d;..    }....   
-000001d0: 202e 7374 726f 6669 6d6f 7669 6368 207b   .strofimovich {
-000001e0: 0d0a 2020 2020 2020 2020 6261 636b 6772  ..        backgr
-000001f0: 6f75 6e64 3a20 2364 3936 6334 3920 2169  ound: #d96c49 !i
-00000200: 6d70 6f72 7461 6e74 3b0d 0a20 2020 207d  mportant;..    }
-00000210: 0d0a 0d0a 2020 2020 2e73 7472 6f66 696d  ....    .strofim
-00000220: 6f76 6963 6820 2e67 616e 7474 5f74 6173  ovich .gantt_tas
-00000230: 6b5f 7072 6f67 7265 7373 207b 0d0a 2020  k_progress {..  
-00000240: 2020 2020 2020 6261 636b 6772 6f75 6e64        background
-00000250: 3a20 2364 3634 6334 3920 2169 6d70 6f72  : #d64c49 !impor
-00000260: 7461 6e74 3b0d 0a20 2020 207d 0d0a 0d0a  tant;..    }....
-00000270: 2020 2020 2e76 6265 7264 6f76 207b 0d0a      .vberdov {..
-00000280: 2020 2020 2020 2020 6261 636b 6772 6f75          backgrou
-00000290: 6e64 3a20 2335 3437 6461 6220 2169 6d70  nd: #547dab !imp
-000002a0: 6f72 7461 6e74 3b0d 0a20 2020 207d 0d0a  ortant;..    }..
-000002b0: 0d0a 2020 2020 2e76 6265 7264 6f76 202e  ..    .vberdov .
-000002c0: 6761 6e74 745f 7461 736b 5f70 726f 6772  gantt_task_progr
-000002d0: 6573 7320 7b0d 0a20 2020 2020 2020 2062  ess {..        b
-000002e0: 6163 6b67 726f 756e 643a 2023 3534 3661  ackground: #546a
-000002f0: 6162 2021 696d 706f 7274 616e 743b 0d0a  ab !important;..
-00000300: 2020 2020 7d0d 0a0d 0a20 2020 202e 6761      }....    .ga
-00000310: 6e74 745f 7369 6465 5f63 6f6e 7465 6e74  ntt_side_content
-00000320: 2e67 616e 7474 5f6c 696e 6b5f 6372 6f73  .gantt_link_cros
-00000330: 7369 6e67 207b 0d0a 2020 2020 2020 2020  sing {..        
-00000340: 746f 703a 300d 0a20 2020 207d 0d0a 3c2f  top:0..    }..</
-00000350: 7374 796c 653e 0d0a 3c64 6976 2069 643d  style>..<div id=
-00000360: 2267 616e 7474 5f68 6572 6522 2073 7479  "gantt_here" sty
-00000370: 6c65 3d27 7769 6474 683a 3130 3025 3b20  le='width:100%; 
-00000380: 6865 6967 6874 3a31 3030 253b 273e 3c2f  height:100%;'></
-00000390: 6469 763e 0d0a 3c73 6372 6970 743e 0d0a  div>..<script>..
-000003a0: 0d0a 2020 2020 6761 6e74 742e 706c 7567  ..    gantt.plug
-000003b0: 696e 7328 7b0d 0a20 2020 2020 2020 206d  ins({..        m
-000003c0: 6172 6b65 723a 2074 7275 652c 0d0a 2020  arker: true,..  
-000003d0: 2020 2020 2020 6772 6f75 7069 6e67 3a20        grouping: 
-000003e0: 7472 7565 0d0a 2020 2020 7d29 3b0d 0a0d  true..    });...
-000003f0: 0a20 2020 2067 616e 7474 2e65 7874 2e7a  .    gantt.ext.z
-00000400: 6f6f 6d2e 696e 6974 287b 0d0a 2020 2020  oom.init({..    
-00000410: 2020 2020 6d69 6e43 6f6c 756d 6e57 6964      minColumnWid
-00000420: 7468 3a20 3830 2c0d 0a20 2020 2020 2020  th: 80,..       
-00000430: 206d 6178 436f 6c75 6d6e 5769 6474 683a   maxColumnWidth:
-00000440: 2031 3530 2c0d 0a20 2020 2020 2020 206c   150,..        l
-00000450: 6576 656c 733a 205b 0d0a 2020 2020 2020  evels: [..      
-00000460: 2020 2020 2020 5b0d 0a20 2020 2020 2020        [..       
-00000470: 2020 2020 2020 2020 207b 756e 6974 3a20           {unit: 
-00000480: 2279 6561 7222 2c20 666f 726d 6174 3a20  "year", format: 
-00000490: 2225 5922 2c20 7374 6570 3a20 317d 2c0d  "%Y", step: 1},.
-000004a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000004b0: 207b 756e 6974 3a20 226d 6f6e 7468 222c   {unit: "month",
-000004c0: 2066 6f72 6d61 743a 2022 254d 222c 2073   format: "%M", s
-000004d0: 7465 703a 2031 7d2c 0d0a 2020 2020 2020  tep: 1},..      
-000004e0: 2020 2020 2020 5d2c 0d0a 2020 2020 2020        ],..      
-000004f0: 2020 2020 2020 5b0d 0a20 2020 2020 2020        [..       
-00000500: 2020 2020 2020 2020 207b 756e 6974 3a20           {unit: 
-00000510: 226d 6f6e 7468 222c 2066 6f72 6d61 743a  "month", format:
-00000520: 2022 254d 2025 5922 2c20 7374 6570 3a20   "%M %Y", step: 
-00000530: 317d 2c0d 0a20 2020 2020 2020 2020 2020  1},..           
-00000540: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
-00000550: 2020 2020 2020 2020 2020 2020 756e 6974              unit
-00000560: 3a20 2277 6565 6b22 2c20 7374 6570 3a20  : "week", step: 
-00000570: 312c 2066 6f72 6d61 743a 2066 756e 6374  1, format: funct
-00000580: 696f 6e20 2864 6174 6529 207b 0d0a 2020  ion (date) {..  
-00000590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005a0: 2020 2020 2020 7661 7220 6461 7465 546f        var dateTo
-000005b0: 5374 7220 3d20 6761 6e74 742e 6461 7465  Str = gantt.date
-000005c0: 2e64 6174 655f 746f 5f73 7472 2822 2564  .date_to_str("%d
-000005d0: 2e25 6d22 293b 0d0a 2020 2020 2020 2020  .%m");..        
-000005e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005f0: 7661 7220 656e 6444 6174 6520 3d20 6761  var endDate = ga
-00000600: 6e74 742e 6461 7465 2e61 6464 2864 6174  ntt.date.add(dat
-00000610: 652c 202d 362c 2022 6461 7922 293b 0d0a  e, -6, "day");..
-00000620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000630: 2020 2020 2020 2020 7265 7475 726e 2064          return d
-00000640: 6174 6554 6f53 7472 2864 6174 6529 202b  ateToStr(date) +
-00000650: 2022 202d 2022 202b 2064 6174 6554 6f53   " - " + dateToS
-00000660: 7472 2865 6e64 4461 7465 293b 0d0a 2020  tr(endDate);..  
-00000670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000680: 2020 7d0d 0a20 2020 2020 2020 2020 2020    }..           
-00000690: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
-000006a0: 2020 2020 5d2c 0d0a 2020 2020 2020 2020      ],..        
-000006b0: 2020 2020 5b0d 0a20 2020 2020 2020 2020      [..         
-000006c0: 2020 2020 2020 207b 756e 6974 3a20 226d         {unit: "m
-000006d0: 6f6e 7468 222c 2066 6f72 6d61 743a 2022  onth", format: "
-000006e0: 254d 2025 7922 2c20 7374 6570 3a20 317d  %M %y", step: 1}
-000006f0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00000700: 2020 207b 756e 6974 3a20 2264 6179 222c     {unit: "day",
-00000710: 2066 6f72 6d61 743a 2022 2564 2e25 6d22   format: "%d.%m"
-00000720: 2c20 7374 6570 3a20 317d 0d0a 2020 2020  , step: 1}..    
-00000730: 2020 2020 2020 2020 5d0d 0a20 2020 2020          ]..     
-00000740: 2020 205d 2c0d 0a20 2020 2020 2020 2075     ],..        u
-00000750: 7365 4b65 793a 2022 6374 726c 4b65 7922  seKey: "ctrlKey"
-00000760: 2c0d 0a20 2020 2020 2020 2074 7269 6767  ,..        trigg
-00000770: 6572 3a20 2277 6865 656c 222c 0d0a 2020  er: "wheel",..  
-00000780: 2020 2020 2020 656c 656d 656e 743a 2066        element: f
-00000790: 756e 6374 696f 6e20 2829 207b 0d0a 2020  unction () {..  
-000007a0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000007b0: 2067 616e 7474 2e24 726f 6f74 2e71 7565   gantt.$root.que
-000007c0: 7279 5365 6c65 6374 6f72 2822 2e67 616e  rySelector(".gan
-000007d0: 7474 5f74 6173 6b22 293b 0d0a 2020 2020  tt_task");..    
-000007e0: 2020 2020 7d0d 0a20 2020 207d 293b 0d0a      }..    });..
-000007f0: 0d0a 2020 2020 6761 6e74 742e 636f 6e66  ..    gantt.conf
-00000800: 6967 2e6d 696e 5f63 6f6c 756d 6e5f 7769  ig.min_column_wi
-00000810: 6474 6820 3d20 3230 3b0d 0a20 2020 2067  dth = 20;..    g
-00000820: 616e 7474 2e63 6f6e 6669 672e 6175 746f  antt.config.auto
-00000830: 5f74 7970 6573 203d 2074 7275 653b 0d0a  _types = true;..
-00000840: 0d0a 2020 2020 6761 6e74 742e 6164 644d  ..    gantt.addM
-00000850: 6172 6b65 7228 7b0d 0a20 2020 2020 2020  arker({..       
-00000860: 2073 7461 7274 5f64 6174 653a 206e 6577   start_date: new
-00000870: 2044 6174 6528 292c 0d0a 2020 2020 2020   Date(),..      
-00000880: 2020 6373 733a 2022 746f 6461 7922 2c0d    css: "today",.
-00000890: 0a20 2020 207d 293b 0d0a 0d0a 2020 2020  .    });....    
-000008a0: 6761 6e74 742e 636f 6e66 6967 2e63 6f6c  gantt.config.col
-000008b0: 756d 6e73 203d 205b 0d0a 2020 2020 2020  umns = [..      
-000008c0: 2020 7b6e 616d 653a 2022 7572 6c22 2c20    {name: "url", 
-000008d0: 7472 6565 3a20 7472 7565 2c20 7769 6474  tree: true, widt
-000008e0: 683a 2033 3030 2c20 7265 7369 7a65 3a20  h: 300, resize: 
-000008f0: 7472 7565 7d2c 0d0a 2020 2020 5d3b 0d0a  true},..    ];..
-00000900: 0d0a 2020 2020 6761 6e74 742e 636f 6e66  ..    gantt.conf
-00000910: 6967 2e72 6f77 5f68 6569 6768 7420 3d20  ig.row_height = 
-00000920: 3235 3b0d 0a0d 0a20 2020 2028 6675 6e63  25;....    (func
-00000930: 7469 6f6e 2028 2920 7b0d 0a20 2020 2020  tion () {..     
-00000940: 2020 2067 616e 7474 2e63 6f6e 6669 672e     gantt.config.
-00000950: 666f 6e74 5f77 6964 7468 5f72 6174 696f  font_width_ratio
-00000960: 203d 2037 3b0d 0a20 2020 2020 2020 2067   = 7;..        g
-00000970: 616e 7474 2e74 656d 706c 6174 6573 2e6c  antt.templates.l
-00000980: 6566 7473 6964 655f 7465 7874 203d 2066  eftside_text = f
-00000990: 756e 6374 696f 6e20 6c65 6674 5369 6465  unction leftSide
-000009a0: 5465 7874 5465 6d70 6c61 7465 2873 7461  TextTemplate(sta
-000009b0: 7274 2c20 656e 642c 2074 6173 6b29 207b  rt, end, task) {
-000009c0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-000009d0: 2028 6765 7454 6173 6b46 6974 5661 6c75   (getTaskFitValu
-000009e0: 6528 7461 736b 2920 3d3d 3d20 226c 6566  e(task) === "lef
-000009f0: 7422 2920 7b0d 0a20 2020 2020 2020 2020  t") {..         
-00000a00: 2020 2020 2020 2072 6574 7572 6e20 7461         return ta
-00000a10: 736b 2e74 6578 743b 0d0a 2020 2020 2020  sk.text;..      
-00000a20: 2020 2020 2020 7d0d 0a20 2020 2020 2020        }..       
-00000a30: 2020 2020 2072 6574 7572 6e20 2222 3b0d       return "";.
-00000a40: 0a20 2020 2020 2020 207d 3b0d 0a20 2020  .        };..   
-00000a50: 2020 2020 2067 616e 7474 2e74 656d 706c       gantt.templ
-00000a60: 6174 6573 2e72 6967 6874 7369 6465 5f74  ates.rightside_t
-00000a70: 6578 7420 3d20 6675 6e63 7469 6f6e 2072  ext = function r
-00000a80: 6967 6874 5369 6465 5465 7874 5465 6d70  ightSideTextTemp
-00000a90: 6c61 7465 2873 7461 7274 2c20 656e 642c  late(start, end,
-00000aa0: 2074 6173 6b29 207b 0d0a 2020 2020 2020   task) {..      
-00000ab0: 2020 2020 2020 6966 2028 6765 7454 6173        if (getTas
-00000ac0: 6b46 6974 5661 6c75 6528 7461 736b 2920  kFitValue(task) 
-00000ad0: 3d3d 3d20 2272 6967 6874 2229 207b 0d0a  === "right") {..
-00000ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000af0: 7265 7475 726e 2074 6173 6b2e 7465 7874  return task.text
-00000b00: 3b0d 0a20 2020 2020 2020 2020 2020 207d  ;..            }
-00000b10: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00000b20: 7475 726e 2022 223b 0d0a 2020 2020 2020  turn "";..      
-00000b30: 2020 7d3b 0d0a 2020 2020 2020 2020 6761    };..        ga
-00000b40: 6e74 742e 7465 6d70 6c61 7465 732e 7461  ntt.templates.ta
-00000b50: 736b 5f74 6578 7420 3d20 6675 6e63 7469  sk_text = functi
-00000b60: 6f6e 2074 6173 6b54 6578 7454 656d 706c  on taskTextTempl
-00000b70: 6174 6528 7374 6172 742c 2065 6e64 2c20  ate(start, end, 
-00000b80: 7461 736b 2920 7b0d 0a20 2020 2020 2020  task) {..       
-00000b90: 2020 2020 2069 6620 2867 6574 5461 736b       if (getTask
-00000ba0: 4669 7456 616c 7565 2874 6173 6b29 203d  FitValue(task) =
-00000bb0: 3d3d 2022 6365 6e74 6572 2229 207b 0d0a  == "center") {..
-00000bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000bd0: 7265 7475 726e 2074 6173 6b2e 7465 7874  return task.text
-00000be0: 3b0d 0a20 2020 2020 2020 2020 2020 207d  ;..            }
-00000bf0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00000c00: 7475 726e 2022 223b 0d0a 2020 2020 2020  turn "";..      
-00000c10: 2020 7d3b 0d0a 0d0a 2020 2020 2020 2020    };....        
-00000c20: 6675 6e63 7469 6f6e 2067 6574 5461 736b  function getTask
-00000c30: 4669 7456 616c 7565 2874 6173 6b29 207b  FitValue(task) {
-00000c40: 0d0a 2020 2020 2020 2020 2020 2020 7661  ..            va
-00000c50: 7220 7461 736b 5374 6172 7450 6f73 203d  r taskStartPos =
-00000c60: 2067 616e 7474 2e70 6f73 4672 6f6d 4461   gantt.posFromDa
-00000c70: 7465 2874 6173 6b2e 7374 6172 745f 6461  te(task.start_da
-00000c80: 7465 292c 0d0a 2020 2020 2020 2020 2020  te),..          
-00000c90: 2020 2020 2020 7461 736b 456e 6450 6f73        taskEndPos
-00000ca0: 203d 2067 616e 7474 2e70 6f73 4672 6f6d   = gantt.posFrom
-00000cb0: 4461 7465 2874 6173 6b2e 656e 645f 6461  Date(task.end_da
-00000cc0: 7465 293b 0d0a 0d0a 2020 2020 2020 2020  te);....        
-00000cd0: 2020 2020 7661 7220 7769 6474 6820 3d20      var width = 
-00000ce0: 7461 736b 456e 6450 6f73 202d 2074 6173  taskEndPos - tas
-00000cf0: 6b53 7461 7274 506f 733b 0d0a 2020 2020  kStartPos;..    
-00000d00: 2020 2020 2020 2020 7661 7220 7465 7874          var text
-00000d10: 5769 6474 6820 3d20 2874 6173 6b2e 7465  Width = (task.te
-00000d20: 7874 207c 7c20 2222 292e 6c65 6e67 7468  xt || "").length
-00000d30: 202a 2067 616e 7474 2e63 6f6e 6669 672e   * gantt.config.
-00000d40: 666f 6e74 5f77 6964 7468 5f72 6174 696f  font_width_ratio
-00000d50: 3b0d 0a0d 0a20 2020 2020 2020 2020 2020  ;....           
-00000d60: 2069 6620 2877 6964 7468 203c 2074 6578   if (width < tex
-00000d70: 7457 6964 7468 2920 7b0d 0a20 2020 2020  tWidth) {..     
-00000d80: 2020 2020 2020 2020 2020 2076 6172 2067             var g
-00000d90: 616e 7474 4c61 7374 4461 7465 203d 2067  anttLastDate = g
-00000da0: 616e 7474 2e67 6574 5374 6174 6528 292e  antt.getState().
-00000db0: 6d61 785f 6461 7465 3b0d 0a20 2020 2020  max_date;..     
-00000dc0: 2020 2020 2020 2020 2020 2076 6172 2067             var g
-00000dd0: 616e 7474 456e 6450 6f73 203d 2067 616e  anttEndPos = gan
-00000de0: 7474 2e70 6f73 4672 6f6d 4461 7465 2867  tt.posFromDate(g
-00000df0: 616e 7474 4c61 7374 4461 7465 293b 0d0a  anttLastDate);..
-00000e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e10: 6966 2028 6761 6e74 7445 6e64 506f 7320  if (ganttEndPos 
-00000e20: 2d20 7461 736b 456e 6450 6f73 203c 2074  - taskEndPos < t
-00000e30: 6578 7457 6964 7468 2920 7b0d 0a20 2020  extWidth) {..   
-00000e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e50: 2072 6574 7572 6e20 226c 6566 7422 0d0a   return "left"..
-00000e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e70: 7d20 656c 7365 207b 0d0a 2020 2020 2020  } else {..      
-00000e80: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00000e90: 7475 726e 2022 7269 6768 7422 0d0a 2020  turn "right"..  
-00000ea0: 2020 2020 2020 2020 2020 2020 2020 7d0d                }.
-00000eb0: 0a20 2020 2020 2020 2020 2020 207d 2065  .            } e
-00000ec0: 6c73 6520 7b0d 0a20 2020 2020 2020 2020  lse {..         
-00000ed0: 2020 2020 2020 2072 6574 7572 6e20 2263         return "c
-00000ee0: 656e 7465 7222 3b0d 0a20 2020 2020 2020  enter";..       
-00000ef0: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
-00000f00: 7d0d 0a20 2020 207d 2928 293b 0d0a 0d0a  }..    })();....
-00000f10: 2020 2020 6761 6e74 742e 7465 6d70 6c61      gantt.templa
-00000f20: 7465 732e 7461 736b 5f63 6c61 7373 203d  tes.task_class =
-00000f30: 2066 756e 6374 696f 6e20 2873 7461 7274   function (start
-00000f40: 2c20 656e 642c 2074 6173 6b29 207b 0d0a  , end, task) {..
-00000f50: 2020 2020 2020 2020 636f 6e73 6f6c 652e          console.
-00000f60: 6c6f 6728 7461 736b 2e70 6172 656e 7429  log(task.parent)
-00000f70: 0d0a 2020 2020 2020 2020 6966 2028 7461  ..        if (ta
-00000f80: 736b 2e70 6172 656e 7420 3d3d 2031 207c  sk.parent == 1 |
-00000f90: 7c20 2874 6173 6b2e 7061 7265 6e74 203d  | (task.parent =
-00000fa0: 3d20 3020 2626 2074 6173 6b2e 7265 736f  = 0 && task.reso
-00000fb0: 7572 6365 203d 3d20 2749 7661 6e20 476e  urce == 'Ivan Gn
-00000fc0: 7573 6172 6b6f 7627 2929 0d0a 2020 2020  usarkov'))..    
-00000fd0: 2020 2020 2020 2020 7265 7475 726e 2022          return "
-00000fe0: 6967 6e75 7361 726b 6f76 223b 0d0a 0d0a  ignusarkov";....
-00000ff0: 2020 2020 2020 2020 6966 2028 7461 736b          if (task
-00001000: 2e70 6172 656e 7420 3d3d 2032 207c 7c20  .parent == 2 || 
-00001010: 2874 6173 6b2e 7061 7265 6e74 203d 3d20  (task.parent == 
-00001020: 3020 2626 2074 6173 6b2e 7265 736f 7572  0 && task.resour
-00001030: 6365 203d 3d20 2753 7465 7061 6e20 5472  ce == 'Stepan Tr
-00001040: 6f66 696d 6f76 6963 6827 2929 0d0a 2020  ofimovich'))..  
-00001050: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00001060: 2022 7374 726f 6669 6d6f 7669 6368 223b   "strofimovich";
-00001070: 0d0a 0d0a 2020 2020 2020 2020 6966 2028  ....        if (
-00001080: 7461 736b 2e70 6172 656e 7420 3d3d 2033  task.parent == 3
-00001090: 207c 7c20 2874 6173 6b2e 7061 7265 6e74   || (task.parent
-000010a0: 203d 3d20 3020 2626 2074 6173 6b2e 7265   == 0 && task.re
-000010b0: 736f 7572 6365 203d 3d20 2756 616c 6572  source == 'Valer
-000010c0: 7920 4265 7264 6f76 2729 290d 0a20 2020  y Berdov'))..   
-000010d0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000010e0: 2276 6265 7264 6f76 223b 0d0a 2020 2020  "vberdov";..    
-000010f0: 7d3b 0d0a 0d0a 2020 2020 6761 6e74 742e  };....    gantt.
-00001100: 636f 6e66 6967 2e72 6561 646f 6e6c 7920  config.readonly 
-00001110: 3d20 7472 7565 3b0d 0a0d 0a20 2020 2067  = true;....    g
-00001120: 616e 7474 2e69 6e69 7428 2267 616e 7474  antt.init("gantt
-00001130: 5f68 6572 6522 293b 0d0a 0d0a 2020 2020  _here");....    
-00001140: 6761 6e74 742e 7061 7273 6528 2f2a 6761  gantt.parse(/*ga
-00001150: 6e74 2064 6174 6120 6865 7265 2a2f 293b  nt data here*/);
-00001160: 0d0a 0d0a 3c2f 7363 7269 7074 3e         ....</script>
+00000000: 3c68 746d 6c3e 0d0a 3c6d 6574 6120 6368  <html>..<meta ch
+00000010: 6172 7365 743d 2275 7466 2d38 223e 0d0a  arset="utf-8">..
+00000020: 3c62 6f64 793e 0d0a 3c73 6372 6970 7420  <body>..<script 
+00000030: 7372 633d 2268 7474 7073 3a2f 2f73 746f  src="https://sto
+00000040: 7261 6765 2e79 616e 6465 7863 6c6f 7564  rage.yandexcloud
+00000050: 2e6e 6574 2f67 796d 626f 7373 2d74 6573  .net/gymboss-tes
+00000060: 742f 6761 6e74 742f 6761 6e74 742f 6468  t/gantt/gantt/dh
+00000070: 746d 6c78 6761 6e74 742e 6a73 3f76 3d37  tmlxgantt.js?v=7
+00000080: 2e31 2e31 3322 3e3c 2f73 6372 6970 743e  .1.13"></script>
+00000090: 0d0a 3c6c 696e 6b20 7265 6c3d 2273 7479  ..<link rel="sty
+000000a0: 6c65 7368 6565 7422 2068 7265 663d 2268  lesheet" href="h
+000000b0: 7474 7073 3a2f 2f73 746f 7261 6765 2e79  ttps://storage.y
+000000c0: 616e 6465 7863 6c6f 7564 2e6e 6574 2f67  andexcloud.net/g
+000000d0: 796d 626f 7373 2d74 6573 742f 6761 6e74  ymboss-test/gant
+000000e0: 742f 6761 6e74 742f 6468 746d 6c78 6761  t/gantt/dhtmlxga
+000000f0: 6e74 742e 6373 733f 763d 372e 312e 3133  ntt.css?v=7.1.13
+00000100: 223e 0d0a 3c73 7479 6c65 3e0d 0a20 2020  ">..<style>..   
+00000110: 2068 746d 6c2c 2062 6f64 7920 7b0d 0a20   html, body {.. 
+00000120: 2020 2020 2020 2070 6164 6469 6e67 3a20         padding: 
+00000130: 3070 783b 0d0a 2020 2020 2020 2020 6d61  0px;..        ma
+00000140: 7267 696e 3a20 3070 783b 0d0a 2020 2020  rgin: 0px;..    
+00000150: 2020 2020 6865 6967 6874 3a20 3130 3025      height: 100%
+00000160: 3b0d 0a20 2020 207d 0d0a 0d0a 2020 2020  ;..    }....    
+00000170: 2e67 616e 7474 5f73 6964 655f 636f 6e74  .gantt_side_cont
+00000180: 656e 742e 6761 6e74 745f 6c69 6e6b 5f63  ent.gantt_link_c
+00000190: 726f 7373 696e 6720 7b0d 0a20 2020 2020  rossing {..     
+000001a0: 2020 2074 6f70 3a30 0d0a 2020 2020 7d0d     top:0..    }.
+000001b0: 0a0d 0a20 2020 2024 7461 736b 5f63 6c61  ...    $task_cla
+000001c0: 7373 6573 5f64 6566 0d0a 3c2f 7374 796c  sses_def..</styl
+000001d0: 653e 0d0a 3c64 6976 2069 643d 2267 616e  e>..<div id="gan
+000001e0: 7474 5f68 6572 6522 2073 7479 6c65 3d27  tt_here" style='
+000001f0: 7769 6474 683a 3130 3025 3b20 6865 6967  width:100%; heig
+00000200: 6874 3a31 3030 253b 273e 3c2f 6469 763e  ht:100%;'></div>
+00000210: 0d0a 3c73 6372 6970 743e 0d0a 0d0a 2020  ..<script>....  
+00000220: 2020 6761 6e74 742e 706c 7567 696e 7328    gantt.plugins(
+00000230: 7b0d 0a20 2020 2020 2020 206d 6172 6b65  {..        marke
+00000240: 723a 2074 7275 652c 0d0a 2020 2020 2020  r: true,..      
+00000250: 2020 6772 6f75 7069 6e67 3a20 7472 7565    grouping: true
+00000260: 0d0a 2020 2020 7d29 3b0d 0a0d 0a20 2020  ..    });....   
+00000270: 2067 616e 7474 2e65 7874 2e7a 6f6f 6d2e   gantt.ext.zoom.
+00000280: 696e 6974 287b 0d0a 2020 2020 2020 2020  init({..        
+00000290: 6d69 6e43 6f6c 756d 6e57 6964 7468 3a20  minColumnWidth: 
+000002a0: 3830 2c0d 0a20 2020 2020 2020 206d 6178  80,..        max
+000002b0: 436f 6c75 6d6e 5769 6474 683a 2031 3530  ColumnWidth: 150
+000002c0: 2c0d 0a20 2020 2020 2020 206c 6576 656c  ,..        level
+000002d0: 733a 205b 0d0a 2020 2020 2020 2020 2020  s: [..          
+000002e0: 2020 5b0d 0a20 2020 2020 2020 2020 2020    [..           
+000002f0: 2020 2020 207b 756e 6974 3a20 2279 6561       {unit: "yea
+00000300: 7222 2c20 666f 726d 6174 3a20 2225 5922  r", format: "%Y"
+00000310: 2c20 7374 6570 3a20 317d 2c0d 0a20 2020  , step: 1},..   
+00000320: 2020 2020 2020 2020 2020 2020 207b 756e               {un
+00000330: 6974 3a20 226d 6f6e 7468 222c 2066 6f72  it: "month", for
+00000340: 6d61 743a 2022 254d 222c 2073 7465 703a  mat: "%M", step:
+00000350: 2031 7d2c 0d0a 2020 2020 2020 2020 2020   1},..          
+00000360: 2020 5d2c 0d0a 2020 2020 2020 2020 2020    ],..          
+00000370: 2020 5b0d 0a20 2020 2020 2020 2020 2020    [..           
+00000380: 2020 2020 207b 756e 6974 3a20 226d 6f6e       {unit: "mon
+00000390: 7468 222c 2066 6f72 6d61 743a 2022 254d  th", format: "%M
+000003a0: 2025 5922 2c20 7374 6570 3a20 317d 2c0d   %Y", step: 1},.
+000003b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000003c0: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+000003d0: 2020 2020 2020 2020 756e 6974 3a20 2277          unit: "w
+000003e0: 6565 6b22 2c20 7374 6570 3a20 312c 2066  eek", step: 1, f
+000003f0: 6f72 6d61 743a 2066 756e 6374 696f 6e20  ormat: function 
+00000400: 2864 6174 6529 207b 0d0a 2020 2020 2020  (date) {..      
+00000410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000420: 2020 7661 7220 6461 7465 546f 5374 7220    var dateToStr 
+00000430: 3d20 6761 6e74 742e 6461 7465 2e64 6174  = gantt.date.dat
+00000440: 655f 746f 5f73 7472 2822 2564 2e25 6d22  e_to_str("%d.%m"
+00000450: 293b 0d0a 2020 2020 2020 2020 2020 2020  );..            
+00000460: 2020 2020 2020 2020 2020 2020 7661 7220              var 
+00000470: 656e 6444 6174 6520 3d20 6761 6e74 742e  endDate = gantt.
+00000480: 6461 7465 2e61 6464 2864 6174 652c 202d  date.add(date, -
+00000490: 362c 2022 6461 7922 293b 0d0a 2020 2020  6, "day");..    
+000004a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000004b0: 2020 2020 7265 7475 726e 2064 6174 6554      return dateT
+000004c0: 6f53 7472 2864 6174 6529 202b 2022 202d  oStr(date) + " -
+000004d0: 2022 202b 2064 6174 6554 6f53 7472 2865   " + dateToStr(e
+000004e0: 6e64 4461 7465 293b 0d0a 2020 2020 2020  ndDate);..      
+000004f0: 2020 2020 2020 2020 2020 2020 2020 7d0d                }.
+00000500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000510: 207d 0d0a 2020 2020 2020 2020 2020 2020   }..            
+00000520: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
+00000530: 5b0d 0a20 2020 2020 2020 2020 2020 2020  [..             
+00000540: 2020 207b 756e 6974 3a20 226d 6f6e 7468     {unit: "month
+00000550: 222c 2066 6f72 6d61 743a 2022 254d 2025  ", format: "%M %
+00000560: 7922 2c20 7374 6570 3a20 317d 2c0d 0a20  y", step: 1},.. 
+00000570: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00000580: 756e 6974 3a20 2264 6179 222c 2066 6f72  unit: "day", for
+00000590: 6d61 743a 2022 2564 222c 2073 7465 703a  mat: "%d", step:
+000005a0: 2031 7d0d 0a20 2020 2020 2020 2020 2020   1}..           
+000005b0: 205d 0d0a 2020 2020 2020 2020 5d2c 0d0a   ]..        ],..
+000005c0: 2020 2020 2020 2020 7573 654b 6579 3a20          useKey: 
+000005d0: 2263 7472 6c4b 6579 222c 0d0a 2020 2020  "ctrlKey",..    
+000005e0: 2020 2020 7472 6967 6765 723a 2022 7768      trigger: "wh
+000005f0: 6565 6c22 2c0d 0a20 2020 2020 2020 2065  eel",..        e
+00000600: 6c65 6d65 6e74 3a20 6675 6e63 7469 6f6e  lement: function
+00000610: 2028 2920 7b0d 0a20 2020 2020 2020 2020   () {..         
+00000620: 2020 2072 6574 7572 6e20 6761 6e74 742e     return gantt.
+00000630: 2424 726f 6f74 2e71 7565 7279 5365 6c65  $$root.querySele
+00000640: 6374 6f72 2822 2e67 616e 7474 5f74 6173  ctor(".gantt_tas
+00000650: 6b22 293b 0d0a 2020 2020 2020 2020 7d0d  k");..        }.
+00000660: 0a20 2020 207d 293b 0d0a 0d0a 2020 2020  .    });....    
+00000670: 6761 6e74 742e 6578 742e 7a6f 6f6d 2e73  gantt.ext.zoom.s
+00000680: 6574 4c65 7665 6c28 2473 6361 6c65 290d  etLevel($scale).
+00000690: 0a0d 0a20 2020 2067 616e 7474 2e63 6f6e  ...    gantt.con
+000006a0: 6669 672e 6d69 6e5f 636f 6c75 6d6e 5f77  fig.min_column_w
+000006b0: 6964 7468 203d 2032 303b 0d0a 2020 2020  idth = 20;..    
+000006c0: 6761 6e74 742e 636f 6e66 6967 2e61 7574  gantt.config.aut
+000006d0: 6f5f 7479 7065 7320 3d20 7472 7565 3b0d  o_types = true;.
+000006e0: 0a0d 0a20 2020 2069 6620 2824 746f 6461  ...    if ($toda
+000006f0: 795f 6d61 726b 6572 2920 7b0d 0a20 2020  y_marker) {..   
+00000700: 2020 2020 2067 616e 7474 2e61 6464 4d61       gantt.addMa
+00000710: 726b 6572 287b 0d0a 2020 2020 2020 2020  rker({..        
+00000720: 2020 2020 7374 6172 745f 6461 7465 3a20      start_date: 
+00000730: 6e65 7720 4461 7465 2829 2c0d 0a20 2020  new Date(),..   
+00000740: 2020 2020 2020 2020 2063 7373 3a20 2274           css: "t
+00000750: 6f64 6179 222c 0d0a 2020 2020 2020 2020  oday",..        
+00000760: 7d29 3b0d 0a20 2020 207d 0d0a 0d0a 2020  });..    }....  
+00000770: 2020 6761 6e74 742e 636f 6e66 6967 2e63    gantt.config.c
+00000780: 6f6c 756d 6e73 203d 2024 636f 6c75 6d6e  olumns = $column
+00000790: 733b 0d0a 0d0a 2020 2020 6761 6e74 742e  s;....    gantt.
+000007a0: 636f 6e66 6967 2e72 6f77 5f68 6569 6768  config.row_heigh
+000007b0: 7420 3d20 2472 6f77 5f68 6569 6768 743b  t = $row_height;
+000007c0: 0d0a 0d0a 2020 2020 2866 756e 6374 696f  ....    (functio
+000007d0: 6e20 2829 207b 0d0a 2020 2020 2020 2020  n () {..        
+000007e0: 6761 6e74 742e 636f 6e66 6967 2e66 6f6e  gantt.config.fon
+000007f0: 745f 7769 6474 685f 7261 7469 6f20 3d20  t_width_ratio = 
+00000800: 373b 0d0a 2020 2020 2020 2020 6761 6e74  7;..        gant
+00000810: 742e 7465 6d70 6c61 7465 732e 6c65 6674  t.templates.left
+00000820: 7369 6465 5f74 6578 7420 3d20 6675 6e63  side_text = func
+00000830: 7469 6f6e 206c 6566 7453 6964 6554 6578  tion leftSideTex
+00000840: 7454 656d 706c 6174 6528 7374 6172 742c  tTemplate(start,
+00000850: 2065 6e64 2c20 7461 736b 2920 7b0d 0a20   end, task) {.. 
+00000860: 2020 2020 2020 2020 2020 2069 6620 2867             if (g
+00000870: 6574 5461 736b 4669 7456 616c 7565 2874  etTaskFitValue(t
+00000880: 6173 6b29 203d 3d3d 2022 6c65 6674 2229  ask) === "left")
+00000890: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+000008a0: 2020 2020 7265 7475 726e 2074 6173 6b2e      return task.
+000008b0: 7465 7874 3b0d 0a20 2020 2020 2020 2020  text;..         
+000008c0: 2020 207d 0d0a 2020 2020 2020 2020 2020     }..          
+000008d0: 2020 7265 7475 726e 2022 223b 0d0a 2020    return "";..  
+000008e0: 2020 2020 2020 7d3b 0d0a 2020 2020 2020        };..      
+000008f0: 2020 6761 6e74 742e 7465 6d70 6c61 7465    gantt.template
+00000900: 732e 7269 6768 7473 6964 655f 7465 7874  s.rightside_text
+00000910: 203d 2066 756e 6374 696f 6e20 7269 6768   = function righ
+00000920: 7453 6964 6554 6578 7454 656d 706c 6174  tSideTextTemplat
+00000930: 6528 7374 6172 742c 2065 6e64 2c20 7461  e(start, end, ta
+00000940: 736b 2920 7b0d 0a20 2020 2020 2020 2020  sk) {..         
+00000950: 2020 2069 6620 2867 6574 5461 736b 4669     if (getTaskFi
+00000960: 7456 616c 7565 2874 6173 6b29 203d 3d3d  tValue(task) ===
+00000970: 2022 7269 6768 7422 2920 7b0d 0a20 2020   "right") {..   
+00000980: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00000990: 7572 6e20 7461 736b 2e74 6578 743b 0d0a  urn task.text;..
+000009a0: 2020 2020 2020 2020 2020 2020 7d0d 0a20              }.. 
+000009b0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000009c0: 6e20 2222 3b0d 0a20 2020 2020 2020 207d  n "";..        }
+000009d0: 3b0d 0a20 2020 2020 2020 2067 616e 7474  ;..        gantt
+000009e0: 2e74 656d 706c 6174 6573 2e74 6173 6b5f  .templates.task_
+000009f0: 7465 7874 203d 2066 756e 6374 696f 6e20  text = function 
+00000a00: 7461 736b 5465 7874 5465 6d70 6c61 7465  taskTextTemplate
+00000a10: 2873 7461 7274 2c20 656e 642c 2074 6173  (start, end, tas
+00000a20: 6b29 207b 0d0a 2020 2020 2020 2020 2020  k) {..          
+00000a30: 2020 6966 2028 6765 7454 6173 6b46 6974    if (getTaskFit
+00000a40: 5661 6c75 6528 7461 736b 2920 3d3d 3d20  Value(task) === 
+00000a50: 2263 656e 7465 7222 2920 7b0d 0a20 2020  "center") {..   
+00000a60: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00000a70: 7572 6e20 7461 736b 2e74 6578 743b 0d0a  urn task.text;..
+00000a80: 2020 2020 2020 2020 2020 2020 7d0d 0a20              }.. 
+00000a90: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00000aa0: 6e20 2222 3b0d 0a20 2020 2020 2020 207d  n "";..        }
+00000ab0: 3b0d 0a0d 0a20 2020 2020 2020 2066 756e  ;....        fun
+00000ac0: 6374 696f 6e20 6765 7454 6173 6b46 6974  ction getTaskFit
+00000ad0: 5661 6c75 6528 7461 736b 2920 7b0d 0a20  Value(task) {.. 
+00000ae0: 2020 2020 2020 2020 2020 2076 6172 2074             var t
+00000af0: 6173 6b53 7461 7274 506f 7320 3d20 6761  askStartPos = ga
+00000b00: 6e74 742e 706f 7346 726f 6d44 6174 6528  ntt.posFromDate(
+00000b10: 7461 736b 2e73 7461 7274 5f64 6174 6529  task.start_date)
+00000b20: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00000b30: 2020 2074 6173 6b45 6e64 506f 7320 3d20     taskEndPos = 
+00000b40: 6761 6e74 742e 706f 7346 726f 6d44 6174  gantt.posFromDat
+00000b50: 6528 7461 736b 2e65 6e64 5f64 6174 6529  e(task.end_date)
+00000b60: 3b0d 0a0d 0a20 2020 2020 2020 2020 2020  ;....           
+00000b70: 2076 6172 2077 6964 7468 203d 2074 6173   var width = tas
+00000b80: 6b45 6e64 506f 7320 2d20 7461 736b 5374  kEndPos - taskSt
+00000b90: 6172 7450 6f73 3b0d 0a20 2020 2020 2020  artPos;..       
+00000ba0: 2020 2020 2076 6172 2074 6578 7457 6964       var textWid
+00000bb0: 7468 203d 2028 7461 736b 2e74 6578 7420  th = (task.text 
+00000bc0: 7c7c 2022 2229 2e6c 656e 6774 6820 2a20  || "").length * 
+00000bd0: 6761 6e74 742e 636f 6e66 6967 2e66 6f6e  gantt.config.fon
+00000be0: 745f 7769 6474 685f 7261 7469 6f3b 0d0a  t_width_ratio;..
+00000bf0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00000c00: 2028 7769 6474 6820 3c20 7465 7874 5769   (width < textWi
+00000c10: 6474 6829 207b 0d0a 2020 2020 2020 2020  dth) {..        
+00000c20: 2020 2020 2020 2020 7661 7220 6761 6e74          var gant
+00000c30: 744c 6173 7444 6174 6520 3d20 6761 6e74  tLastDate = gant
+00000c40: 742e 6765 7453 7461 7465 2829 2e6d 6178  t.getState().max
+00000c50: 5f64 6174 653b 0d0a 2020 2020 2020 2020  _date;..        
+00000c60: 2020 2020 2020 2020 7661 7220 6761 6e74          var gant
+00000c70: 7445 6e64 506f 7320 3d20 6761 6e74 742e  tEndPos = gantt.
+00000c80: 706f 7346 726f 6d44 6174 6528 6761 6e74  posFromDate(gant
+00000c90: 744c 6173 7444 6174 6529 3b0d 0a20 2020  tLastDate);..   
+00000ca0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00000cb0: 2867 616e 7474 456e 6450 6f73 202d 2074  (ganttEndPos - t
+00000cc0: 6173 6b45 6e64 506f 7320 3c20 7465 7874  askEndPos < text
+00000cd0: 5769 6474 6829 207b 0d0a 2020 2020 2020  Width) {..      
+00000ce0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00000cf0: 7475 726e 2022 6c65 6674 220d 0a20 2020  turn "left"..   
+00000d00: 2020 2020 2020 2020 2020 2020 207d 2065               } e
+00000d10: 6c73 6520 7b0d 0a20 2020 2020 2020 2020  lse {..         
+00000d20: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00000d30: 6e20 2272 6967 6874 220d 0a20 2020 2020  n "right"..     
+00000d40: 2020 2020 2020 2020 2020 207d 0d0a 2020             }..  
+00000d50: 2020 2020 2020 2020 2020 7d20 656c 7365            } else
+00000d60: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+00000d70: 2020 2020 7265 7475 726e 2022 6365 6e74      return "cent
+00000d80: 6572 223b 0d0a 2020 2020 2020 2020 2020  er";..          
+00000d90: 2020 7d0d 0a20 2020 2020 2020 207d 0d0a    }..        }..
+00000da0: 2020 2020 7d29 2829 3b0d 0a0d 0a20 2020      })();....   
+00000db0: 2067 616e 7474 2e74 656d 706c 6174 6573   gantt.templates
+00000dc0: 2e74 6173 6b5f 636c 6173 7320 3d20 6675  .task_class = fu
+00000dd0: 6e63 7469 6f6e 2028 7374 6172 742c 2065  nction (start, e
+00000de0: 6e64 2c20 7461 736b 2920 7b0d 0a20 2020  nd, task) {..   
+00000df0: 2020 2020 2072 6574 7572 6e20 7461 736b       return task
+00000e00: 2e63 7373 5f63 6c61 7373 3b0d 0a20 2020  .css_class;..   
+00000e10: 207d 3b0d 0a0d 0a20 2020 2067 616e 7474   };....    gantt
+00000e20: 2e63 6f6e 6669 672e 7265 6164 6f6e 6c79  .config.readonly
+00000e30: 203d 2024 7265 6164 6f6e 6c79 3b0d 0a0d   = $readonly;...
+00000e40: 0a20 2020 2067 616e 7474 2e69 6e69 7428  .    gantt.init(
+00000e50: 2267 616e 7474 5f68 6572 6522 293b 0d0a  "gantt_here");..
+00000e60: 0d0a 2020 2020 6761 6e74 742e 7061 7273  ..    gantt.pars
+00000e70: 6528 2467 616e 7474 5f64 6174 6129 3b0d  e($gantt_data);.
+00000e80: 0a0d 0a3c 2f73 6372 6970 743e 0d0a 3c2f  ...</script>..</
+00000e90: 626f 6479 3e0d 0a3c 2f68 746d 6c3e 0d0a  body>..</html>..
```

### Comparing `pjplan-0.0.2/tests/test_pjplan/io/test_csv_io.py` & `pjplan-0.0.7/tests/test_pjplan/test_io/test_csv_io.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,27 +13,29 @@
     @classmethod
     def setUpClass(cls) -> None:
         if not os.path.exists(cls.TEST_DIR):
             os.mkdir('./test_data')
 
     @classmethod
     def tearDownClass(cls) -> None:
-        # shutil.rmtree(cls.TEST_DIR)
+        shutil.rmtree(cls.TEST_DIR)
         pass
 
     def assertTasksEqual(self, t1, t2):
         self.assertEqual(t1.name, t2.name)
         self.assertEqual(t1.resource, t2.resource)
         self.assertEqual(t1.start, t2.start)
         self.assertEqual(t1.end, t2.end)
         self.assertEqual(t1.estimate, t2.estimate)
         self.assertEqual(t1.spent, t2.spent)
         self.assertEqual(t1.milestone, t2.milestone)
 
         for k, v in t1.__dict__.items():
+            if k.startswith('_'):
+                continue
             self.assertTrue(k in t2.__dict__, f"{k} attr not found")
             self.assertEqual(t1.__getattribute__(k), t2.__getattribute__(k), f"{k} are not equals")
 
     # noinspection PyStatementEffect
     def test_read_write(self):
         p = WBS()
         t1 = p // Task(1)
@@ -48,24 +50,24 @@
 
         file = os.path.join(self.TEST_DIR, 'test.csv')
 
         write_csv(p, file)
 
         r = read_csv(file)
 
-        self.assertTasksEqual(t1, r(1))
+        self.assertTasksEqual(t1, r[1])
 
-        self.assertTasksEqual(t2, r(2))
-        self.assertTrue(r(2) in p(1).children)
-        self.assertTrue(r(1) == r(2).parent)
-
-        self.assertTasksEqual(t3, r(3))
-        self.assertTrue(r(3) in r(2).successors)
-        self.assertTrue(r(2) in r(3).predecessors)
-
-        self.assertTasksEqual(t4, r(4))
-
-        self.assertTasksEqual(t5, r(5))
-        self.assertTasksEqual(t6, r(6))
-        self.assertTasksEqual(t7, r(7))
-        self.assertTasksEqual(t8, r(8))
-        self.assertTasksEqual(t9, r(9))
+        self.assertTasksEqual(t2, r[2])
+        self.assertTrue(r[2] in r[1].children)
+        self.assertTrue(r[1] == r[2].parent)
+
+        self.assertTasksEqual(t3, r[3])
+        self.assertTrue(r[3] in r[2].successors)
+        self.assertTrue(r[2] in r[3].predecessors)
+
+        self.assertTasksEqual(t4, r[4])
+
+        self.assertTasksEqual(t5, r[5])
+        self.assertTasksEqual(t6, r[6])
+        self.assertTasksEqual(t7, r[7])
+        self.assertTasksEqual(t8, r[8])
+        self.assertTasksEqual(t9, r[9])
```

### Comparing `pjplan-0.0.2/LICENSE` & `pjplan-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pjplan-0.0.2/pyproject.toml` & `pjplan-0.0.7/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pjplan"
-version = "0.0.2"
+version = "0.0.7"
 authors = [
   { name="Artem Snopkov", email="artem.snopkov@gmail.com" },
 ]
 description = "Python library for plan projects"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

