# Comparing `tmp/analogic-framework-4.0.2.tar.gz` & `tmp/analogic-framework-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "analogic-framework-4.0.2.tar", last modified: Mon Oct  3 06:38:11 2022, max compression
+gzip compressed data, was "analogic-framework-4.1.0.tar", last modified: Wed Apr 12 09:33:36 2023, max compression
```

## Comparing `analogic-framework-4.0.2.tar` & `analogic-framework-4.1.0.tar`

### file list

```diff
@@ -1,234 +1,255 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 06:38:11.895883 analogic-framework-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-10-03 06:38:11.895883 analogic-framework-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5083 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 06:38:11.875883 analogic-framework-4.0.2/analogic/
--rw-r--r--   0 runner    (1001) docker     (121)      649 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10848 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/analogic.py
--rw-r--r--   0 runner    (1001) docker     (121)     6548 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/authentication_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     3938 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/cam.py
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/condition.py
--rw-r--r--   0 runner    (1001) docker     (121)     1766 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/core_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (121)     2540 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/email.py
--rw-r--r--   0 runner    (1001) docker     (121)     2245 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)      524 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     3219 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/logging.json
--rw-r--r--   0 runner    (1001) docker     (121)     2666 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/loginbasic.py
--rw-r--r--   0 runner    (1001) docker     (121)     1195 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/nologin.py
--rw-r--r--   0 runner    (1001) docker     (121)    13640 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/pivot.py
--rw-r--r--   0 runner    (1001) docker     (121)     6585 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/setting.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 06:38:11.871883 analogic-framework-4.0.2/analogic/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 06:38:11.875883 analogic-framework-4.0.2/analogic/static/assets/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 06:38:11.875883 analogic-framework-4.0.2/analogic/static/assets/css/
--rw-r--r--   0 runner    (1001) docker     (121)    48488 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/css/bootstrap-grid.min.css
--rw-r--r--   0 runner    (1001) docker     (121)   108539 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/css/bootstrap-grid.min.css.map
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 06:38:11.875883 analogic-framework-4.0.2/analogic/static/assets/css/lib/
--rw-r--r--   0 runner    (1001) docker     (121)      521 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/css/lib/Chart-2.9.3.min.css
--rw-r--r--   0 runner    (1001) docker     (121)     4220 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/css/lib/nouislider.min.css
--rw-r--r--   0 runner    (1001) docker     (121)    65538 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 06:38:11.875883 analogic-framework-4.0.2/analogic/static/assets/css/widgets/
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/css/widgets/loader.css
--rw-r--r--   0 runner    (1001) docker     (121)     2000 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/css/widgets/simulation-panel-slider.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 06:38:11.875883 analogic-framework-4.0.2/analogic/static/assets/images/
--rw-r--r--   0 runner    (1001) docker     (121)    10487 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/images/loading.gif
--rw-r--r--   0 runner    (1001) docker     (121)   120349 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/images/loading2.gif
--rw-r--r--   0 runner    (1001) docker     (121)    55508 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/images/loading2_transparent.gif
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/images/triangle.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 06:38:11.871883 analogic-framework-4.0.2/analogic/static/assets/js/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 06:38:11.879883 analogic-framework-4.0.2/analogic/static/assets/js/framework/
--rw-r--r--   0 runner    (1001) docker     (121)    20162 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/framework/api.js
--rw-r--r--   0 runner    (1001) docker     (121)     2817 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/framework/app.js
--rw-r--r--   0 runner    (1001) docker     (121)     3349 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/framework/authentication.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 06:38:11.879883 analogic-framework-4.0.2/analogic/static/assets/js/framework/extensions/
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/framework/extensions/authentication-provider.js
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/framework/extensions/write-executor.js
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/framework/listener.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 06:38:11.879883 analogic-framework-4.0.2/analogic/static/assets/js/framework/load-executor/
--rw-r--r--   0 runner    (1001) docker     (121)     2385 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/framework/load-executor/array.js
--rw-r--r--   0 runner    (1001) docker     (121)     3388 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/framework/load-executor/base.js
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/framework/load-executor/default.js
--rw-r--r--   0 runner    (1001) docker     (121)     3885 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/framework/load-executor/factory.js
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/framework/load-executor/skip.js
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/framework/load-executor/state.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 06:38:11.879883 analogic-framework-4.0.2/analogic/static/assets/js/framework/parsing-control/
--rw-r--r--   0 runner    (1001) docker     (121)      591 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/framework/parsing-control/base.js
--rw-r--r--   0 runner    (1001) docker     (121)     1425 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/framework/parsing-control/factory.js
--rw-r--r--   0 runner    (1001) docker     (121)      457 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/framework/parsing-control/list.js
--rw-r--r--   0 runner    (1001) docker     (121)      780 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/framework/parsing-control/matrix.js
--rw-r--r--   0 runner    (1001) docker     (121)      358 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/framework/parsing-control/object.js
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/framework/parsing-control/script.js
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/framework/parsing-control/skip.js
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/framework/pivot.js
--rw-r--r--   0 runner    (1001) docker     (121)     3550 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/framework/query-builder.js
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/framework/redirect.js
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/framework/render.js
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/framework/rest-request.js
--rw-r--r--   0 runner    (1001) docker     (121)     1523 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/framework/server.js
--rw-r--r--   0 runner    (1001) docker     (121)    20228 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/framework/utils.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 06:38:11.879883 analogic-framework-4.0.2/analogic/static/assets/js/framework/write-executor/
--rw-r--r--   0 runner    (1001) docker     (121)     4733 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/framework/write-executor/base.js
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/framework/write-executor/download.js
--rw-r--r--   0 runner    (1001) docker     (121)     5658 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/framework/write-executor/factory.js
--rw-r--r--   0 runner    (1001) docker     (121)      488 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/framework/write-executor/function.js
--rw-r--r--   0 runner    (1001) docker     (121)     2054 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/framework/write-executor/grid-table.js
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/framework/write-executor/skip.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 06:38:11.883883 analogic-framework-4.0.2/analogic/static/assets/js/lib/
--rw-r--r--   0 runner    (1001) docker     (121)   172689 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/lib/Chart-2.9.3.min.js
--rw-r--r--   0 runner    (1001) docker     (121)    44136 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/lib/Sortable.min.js
--rw-r--r--   0 runner    (1001) docker     (121)    12908 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/lib/chartjs-plugin-datalabels.min.js
--rw-r--r--   0 runner    (1001) docker     (121)    21295 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/lib/chartjs-plugin-dragdata.min.js
--rw-r--r--   0 runner    (1001) docker     (121)     1154 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/lib/debounceAndThrottle.1.8.3.min.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 06:38:11.883883 analogic-framework-4.0.2/analogic/static/assets/js/lib/jquery/
--rw-r--r--   0 runner    (1001) docker     (121)    89411 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/lib/jquery/jquery-3.6.0.min.js
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/lib/jquery/jquery.actual.min.js
--rw-r--r--   0 runner    (1001) docker     (121)     2981 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/lib/jquery/jquery.cookie.js
--rw-r--r--   0 runner    (1001) docker     (121)      896 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/lib/jquery/jquery.doubletap.js
--rw-r--r--   0 runner    (1001) docker     (121)     1460 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/lib/jquery/tableSort.js
--rw-r--r--   0 runner    (1001) docker     (121)    26460 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/lib/nouislider.min.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 06:38:11.887883 analogic-framework-4.0.2/analogic/static/assets/js/widgets/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 06:38:11.887883 analogic-framework-4.0.2/analogic/static/assets/js/widgets/base/
--rw-r--r--   0 runner    (1001) docker     (121)    22653 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/base/widget.js
--rw-r--r--   0 runner    (1001) docker     (121)    12486 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/button.js
--rw-r--r--   0 runner    (1001) docker     (121)    26849 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/combo-chart.js
--rw-r--r--   0 runner    (1001) docker     (121)     1664 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/container.js
--rw-r--r--   0 runner    (1001) docker     (121)    15772 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/datepicker.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 06:38:11.891883 analogic-framework-4.0.2/analogic/static/assets/js/widgets/default/
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/default/BubbleChartWidget.json
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/default/ButtonWidget.json
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/default/ComboChartWidget.json
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/default/ContainerWidget.json
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/default/DatePickerWidget.json
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/default/DropBoxWidget.json
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/default/GaugeWidget.json
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/default/GridCellWidget.json
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/default/GridRowWidget.json
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/default/GridWidget.json
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/default/HistogramComboChartWidget.json
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/default/HorizontalTableWidget.json
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/default/ImageWidget.json
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/default/LineAreaChartWidget.json
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/default/PanelWidget.json
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/default/PieChartWidget.json
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/default/PopupWidget.json
--rw-r--r--   0 runner    (1001) docker     (121)     1054 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/default/ScrollTableWidget.json
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/default/SegmentedBarWidget.json
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/default/SegmentedControlItemWidget.json
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/default/SegmentedControlWidget.json
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/default/SideBarWidget.json
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/default/SimulationPanelSliderWidget.json
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/default/SimulationPanelWidget.json
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/default/SliderWidget.json
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/default/SwipeWidget.json
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/default/TextAreaWidget.json
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/default/TextBoxWidget.json
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/default/TextWidget.json
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/default/ToggleWidget.json
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/default/TornadoChartWidget.json
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/default/VerticalLineBoxWidget.json
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/default/WaterFallWidget.json
--rw-r--r--   0 runner    (1001) docker     (121)    10938 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/dropbox.js
--rw-r--r--   0 runner    (1001) docker     (121)     9065 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/gauge.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 06:38:11.891883 analogic-framework-4.0.2/analogic/static/assets/js/widgets/grid/
--rw-r--r--   0 runner    (1001) docker     (121)     1109 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/grid/grid-cell.js
--rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/grid/grid-row.js
--rw-r--r--   0 runner    (1001) docker     (121)      994 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/grid/grid.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 06:38:11.891883 analogic-framework-4.0.2/analogic/static/assets/js/widgets/grid-table/
--rw-r--r--   0 runner    (1001) docker     (121)     4430 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/grid-table/grid-table-cell.js
--rw-r--r--   0 runner    (1001) docker     (121)     2650 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/grid-table/grid-table-header-cell.js
--rw-r--r--   0 runner    (1001) docker     (121)     1593 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/grid-table/grid-table-header-row.js
--rw-r--r--   0 runner    (1001) docker     (121)    15923 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/grid-table/grid-table.js
--rw-r--r--   0 runner    (1001) docker     (121)    18115 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/histogram-combo-chart.js
--rw-r--r--   0 runner    (1001) docker     (121)     2502 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/horizontal-bar-chart.js
--rw-r--r--   0 runner    (1001) docker     (121)    25660 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/horizontal-table.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 06:38:11.891883 analogic-framework-4.0.2/analogic/static/assets/js/widgets/horizontaltable/
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/horizontaltable/action-button-row.js
--rw-r--r--   0 runner    (1001) docker     (121)      953 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/horizontaltable/delete-button-row.js
--rw-r--r--   0 runner    (1001) docker     (121)      962 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/horizontaltable/radio-button-row.js
--rw-r--r--   0 runner    (1001) docker     (121)     1295 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/image.js
--rw-r--r--   0 runner    (1001) docker     (121)    15899 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/line-area-chart.js
--rw-r--r--   0 runner    (1001) docker     (121)    18104 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/line-scatter-combo.js
--rw-r--r--   0 runner    (1001) docker     (121)     1186 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/loader.js
--rw-r--r--   0 runner    (1001) docker     (121)      795 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/page.js
--rw-r--r--   0 runner    (1001) docker     (121)      309 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/panel.js
--rw-r--r--   0 runner    (1001) docker     (121)     6267 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/pie-chart.js
--rw-r--r--   0 runner    (1001) docker     (121)    80841 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/pivot-table.js
--rw-r--r--   0 runner    (1001) docker     (121)     7776 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/popup.js
--rw-r--r--   0 runner    (1001) docker     (121)     8149 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/radar-chart.js
--rw-r--r--   0 runner    (1001) docker     (121)    36457 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/scroll-table.js
--rw-r--r--   0 runner    (1001) docker     (121)     2741 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/segmented-bar.js
--rw-r--r--   0 runner    (1001) docker     (121)      828 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/segmented-control-item.js
--rw-r--r--   0 runner    (1001) docker     (121)     3667 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/segmented-control.js
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/shadow.js
--rw-r--r--   0 runner    (1001) docker     (121)     2067 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/simulation-panel-slider.js
--rw-r--r--   0 runner    (1001) docker     (121)     4840 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/simulation-panel.js
--rw-r--r--   0 runner    (1001) docker     (121)    19961 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/slider.js
--rw-r--r--   0 runner    (1001) docker     (121)     4956 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/swipe.js
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/system-popup.js
--rw-r--r--   0 runner    (1001) docker     (121)    20041 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/text.js
--rw-r--r--   0 runner    (1001) docker     (121)     4680 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/textarea.js
--rw-r--r--   0 runner    (1001) docker     (121)     5342 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/textbox.js
--rw-r--r--   0 runner    (1001) docker     (121)     7899 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/toggle.js
--rw-r--r--   0 runner    (1001) docker     (121)     4921 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/tornado-chart.js
--rw-r--r--   0 runner    (1001) docker     (121)     2779 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/vertical-line-box.js
--rw-r--r--   0 runner    (1001) docker     (121)    10542 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/js/widgets/water-fall.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 06:38:11.875883 analogic-framework-4.0.2/analogic/static/assets/skin/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 06:38:11.895883 analogic-framework-4.0.2/analogic/static/assets/skin/css/
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-button.css
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-combo-chart.css
--rw-r--r--   0 runner    (1001) docker     (121)     1462 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-container.css
--rw-r--r--   0 runner    (1001) docker     (121)     1435 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-datepicker.css
--rw-r--r--   0 runner    (1001) docker     (121)     1782 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-dropbox.css
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-gauge.css
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-grid-cell.css
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-grid-row.css
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-grid-table-cell.css
--rw-r--r--   0 runner    (1001) docker     (121)     1665 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-grid-table.css
--rw-r--r--   0 runner    (1001) docker     (121)     1310 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-grid.css
--rw-r--r--   0 runner    (1001) docker     (121)     2149 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-horizontal-table.css
--rw-r--r--   0 runner    (1001) docker     (121)     3706 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-horizontalbarchart.css
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-image.css
--rw-r--r--   0 runner    (1001) docker     (121)      175 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-legend.css
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-line-area-chart.css
--rw-r--r--   0 runner    (1001) docker     (121)     1601 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-line-scatter-combo.css
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-page.css
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-panel.css
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-pie-chart.css
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-pivot-table.css
--rw-r--r--   0 runner    (1001) docker     (121)     1388 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-popup.css
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-radar-chart.css
--rw-r--r--   0 runner    (1001) docker     (121)     1655 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-scrolltable.css
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-segmented.css
--rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-segmentedbar.css
--rw-r--r--   0 runner    (1001) docker     (121)      879 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-slider-touch.css
--rw-r--r--   0 runner    (1001) docker     (121)     1242 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-slider.css
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-text.css
--rw-r--r--   0 runner    (1001) docker     (121)      765 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-textarea.css
--rw-r--r--   0 runner    (1001) docker     (121)      819 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-textbox.css
--rw-r--r--   0 runner    (1001) docker     (121)      841 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-toggle.css
--rw-r--r--   0 runner    (1001) docker     (121)     2133 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-tornado.css
--rw-r--r--   0 runner    (1001) docker     (121)      667 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-vertical-line-box.css
--rw-r--r--   0 runner    (1001) docker     (121)     3003 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-waterfall.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 06:38:11.895883 analogic-framework-4.0.2/analogic/templates/
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/templates/500.html
--rw-r--r--   0 runner    (1001) docker     (121)     2135 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/templates/authenticated.html
--rw-r--r--   0 runner    (1001) docker     (121)      700 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/templates/config.html
--rw-r--r--   0 runner    (1001) docker     (121)    10403 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/templates/css.html
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (121)    11080 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/templates/javascripts.html
--rw-r--r--   0 runner    (1001) docker     (121)     2972 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (121)      585 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/templates/redirect.html
--rw-r--r--   0 runner    (1001) docker     (121)     2195 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/templates/sso_error.html
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/templates/unauthorized.html
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/version.config
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/analogic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 06:38:11.895883 analogic-framework-4.0.2/analogic_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-10-03 06:38:11.000000 analogic-framework-4.0.2/analogic_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10183 2022-10-03 06:38:11.000000 analogic-framework-4.0.2/analogic_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-03 06:38:11.000000 analogic-framework-4.0.2/analogic_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-10-03 06:38:11.000000 analogic-framework-4.0.2/analogic_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-10-03 06:38:11.000000 analogic-framework-4.0.2/analogic_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-03 06:38:11.895883 analogic-framework-4.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      822 2022-10-03 06:37:57.000000 analogic-framework-4.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.806396 analogic-framework-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-12 09:33:36.806396 analogic-framework-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.778396 analogic-framework-4.1.0/analogic/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11724 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/analogic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23429 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/analogic_tm1_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/authentication_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/cam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/camsecure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/core_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/logging.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/loginbasic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/logincam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/nologin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/pivot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/setting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.766396 analogic-framework-4.1.0/analogic/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.770396 analogic-framework-4.1.0/analogic/static/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.778396 analogic-framework-4.1.0/analogic/static/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    48488 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/css/bootstrap-grid.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   108539 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/css/bootstrap-grid.min.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.778396 analogic-framework-4.1.0/analogic/static/assets/css/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/css/lib/Chart-2.9.3.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/css/lib/nouislider.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    65538 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.778396 analogic-framework-4.1.0/analogic/static/assets/css/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/css/widgets/loader.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/css/widgets/simulation-panel-slider.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.778396 analogic-framework-4.1.0/analogic/static/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    10487 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/images/loading.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   120349 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/images/loading2.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    55508 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/images/loading2_transparent.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/images/triangle.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.770396 analogic-framework-4.1.0/analogic/static/assets/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.782396 analogic-framework-4.1.0/analogic/static/assets/js/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)    20536 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/api.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/authentication.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.782396 analogic-framework-4.1.0/analogic/static/assets/js/framework/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/extensions/authentication-provider.js
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/extensions/write-executor.js
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/listener.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.782396 analogic-framework-4.1.0/analogic/static/assets/js/framework/load-executor/
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/load-executor/array.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/load-executor/base.js
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/load-executor/default.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/load-executor/factory.js
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/load-executor/skip.js
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/load-executor/state.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.782396 analogic-framework-4.1.0/analogic/static/assets/js/framework/parsing-control/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/parsing-control/base.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/parsing-control/factory.js
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/parsing-control/list.js
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/parsing-control/matrix.js
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/parsing-control/object.js
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/parsing-control/script.js
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/parsing-control/skip.js
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/pivot.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/query-builder.js
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/redirect.js
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/render.js
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/rest-request.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/server.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22800 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/utils.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.782396 analogic-framework-4.1.0/analogic/static/assets/js/framework/write-executor/
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/write-executor/base.js
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/write-executor/download.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/write-executor/factory.js
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/write-executor/function.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/write-executor/grid-table.js
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/framework/write-executor/skip.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.786396 analogic-framework-4.1.0/analogic/static/assets/js/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)   172689 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/lib/Chart-2.9.3.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    44136 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/lib/Sortable.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12908 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/lib/chartjs-plugin-datalabels.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21295 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/lib/chartjs-plugin-dragdata.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/lib/debounceAndThrottle.1.8.3.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.786396 analogic-framework-4.1.0/analogic/static/assets/js/lib/jquery/
+-rw-r--r--   0 runner    (1001) docker     (123)    89411 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/lib/jquery/jquery-3.6.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/lib/jquery/jquery.actual.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/lib/jquery/jquery.cookie.js
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/lib/jquery/jquery.doubletap.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/lib/jquery/tableSort.js
+-rw-r--r--   0 runner    (1001) docker     (123)    26460 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/lib/nouislider.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.790396 analogic-framework-4.1.0/analogic/static/assets/js/widgets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.790396 analogic-framework-4.1.0/analogic/static/assets/js/widgets/base/
+-rw-r--r--   0 runner    (1001) docker     (123)    23255 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/base/widget.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/button.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27607 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/combo-chart.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/container.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15772 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/datepicker.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.794396 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/BubbleChartWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/ButtonWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/ComboChartWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/ContainerWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/DatePickerWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/DropBoxWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/GaugeWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/GridCellWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/GridRowWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/GridWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/HistogramComboChartWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/HorizontalTableWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/ImageWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/LineAreaChartWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/PanelWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/PieChartWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/PopupWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/ScrollTableWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/SegmentedBarWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/SegmentedControlItemWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/SegmentedControlWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/SideBarWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/SimulationPanelSliderWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/SimulationPanelWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/SliderWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/SwipeWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/TextAreaWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/TextBoxWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/TextWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/ToggleWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/TornadoChartWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/VerticalLineBoxWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/WaterFallWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10938 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/dropbox.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9323 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/gauge.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.794396 analogic-framework-4.1.0/analogic/static/assets/js/widgets/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/grid/grid-cell.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/grid/grid-row.js
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/grid/grid.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.798396 analogic-framework-4.1.0/analogic/static/assets/js/widgets/grid-table/
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/grid-table/grid-table-cell.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/grid-table/grid-table-header-cell.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/grid-table/grid-table-header-row.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18935 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/grid-table/grid-table.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18115 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/histogram-combo-chart.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/horizontal-bar-chart.js
+-rw-r--r--   0 runner    (1001) docker     (123)    25693 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/horizontal-table.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.798396 analogic-framework-4.1.0/analogic/static/assets/js/widgets/horizontaltable/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/horizontaltable/action-button-row.js
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/horizontaltable/delete-button-row.js
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/horizontaltable/radio-button-row.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/image.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15899 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/line-area-chart.js
+-rw-r--r--   0 runner    (1001) docker     (123)    26611 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/line-scatter-combo.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/loader.js
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/page.js
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/panel.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/pie-chart.js
+-rw-r--r--   0 runner    (1001) docker     (123)    81004 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/pivot-table.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/popup.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/radar-chart.js
+-rw-r--r--   0 runner    (1001) docker     (123)    36449 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/scroll-table.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/segmented-bar.js
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/segmented-control-item.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/segmented-control.js
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/shadow.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/simulation-panel-slider.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/simulation-panel.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19961 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/slider.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/swipe.js
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/system-popup.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20395 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/text.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/textarea.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/textbox.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/toggle.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/tornado-chart.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/vertical-line-box.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/js/widgets/water-fall.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.770396 analogic-framework-4.1.0/analogic/static/assets/skin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.802396 analogic-framework-4.1.0/analogic/static/assets/skin/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-button.css
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-combo-chart.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-container.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-datepicker.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-dropbox.css
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-gauge.css
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-general.css
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-grid-cell.css
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-grid-row.css
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-grid-table-cell.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-grid-table.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-grid.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-horizontal-table.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-horizontalbarchart.css
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-image.css
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-legend.css
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-line-area-chart.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-line-scatter-combo.css
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-page.css
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-panel.css
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-pie-chart.css
+-rw-r--r--   0 runner    (1001) docker     (123)    20239 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-pivot-table.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-popup.css
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-radar-chart.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-scrolltable.css
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-segmented.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-segmentedbar.css
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-slider-touch.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-slider.css
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-text.css
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-textarea.css
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-textbox.css
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-toggle.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-tornado.css
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-vertical-line-box.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-waterfall.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.806396 analogic-framework-4.1.0/analogic/static/assets/skin/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    75822 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/fonts/GothamNarrow-Bold.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   253851 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/fonts/GothamNarrow-Bold.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    75604 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/fonts/GothamNarrow-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    32032 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/fonts/GothamNarrow-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    23076 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/fonts/GothamNarrow-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    75582 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/fonts/GothamNarrow-Medium.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   256592 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/fonts/GothamNarrow-Medium.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    75356 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/fonts/GothamNarrow-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    32152 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/fonts/GothamNarrow-Medium.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    23124 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/fonts/GothamNarrow-Medium.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/fonts/pivot.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   108091 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/fonts/pivot.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    26028 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/fonts/pivot.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    26104 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/static/assets/skin/fonts/pivot.woff
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.806396 analogic-framework-4.1.0/analogic/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/templates/500.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/templates/authenticated.html
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/templates/config.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/templates/css.html
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11080 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/templates/javascripts.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/templates/redirect.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/templates/sso_error.html
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/templates/unauthorized.html
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/version.config
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/analogic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:36.806396 analogic-framework-4.1.0/analogic_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-12 09:33:36.000000 analogic-framework-4.1.0/analogic_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11099 2023-04-12 09:33:36.000000 analogic-framework-4.1.0/analogic_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 09:33:36.000000 analogic-framework-4.1.0/analogic_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-12 09:33:36.000000 analogic-framework-4.1.0/analogic_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 09:33:36.000000 analogic-framework-4.1.0/analogic_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 09:33:36.806396 analogic-framework-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-12 09:33:21.000000 analogic-framework-4.1.0/setup.py
```

### Comparing `analogic-framework-4.0.2/LICENSE` & `analogic-framework-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/analogic.py` & `analogic-framework-4.1.0/analogic/analogic.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 from analogic.condition import Condition
 import inspect
 from flask_caching import Cache
 from analogic.setting import SettingManager
 from datetime import timedelta
 import importlib
 from analogic.version import version
+from analogic.task import scheduler
+import atexit
 
 APPLICATIONS_DIR = 'apps'
 APPLICATIONS_DIR_EXTRA = os.environ.get('APPLICATIONS_DIR_EXTRA', '')
 EXTENSIONS_DIR = 'extensions'
 EXTENSIONS_DIR_EXTRA = os.environ.get('EXTENSIONS_DIR_EXTRA', '')
 ALLOWED_EXTENSION_PREFIX = 'analogic_'
 
@@ -29,15 +31,17 @@
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.endpoint_rules = []
         self.authentication_providers = {
             'Cam': 'analogic',
+            'CamSecure': 'analogic',
             'LoginBasic': 'analogic',
+            'LoginCam': 'analogic',
             'NoLogin': 'analogic'
         }
         self.conditions = {}
         self.extension_assets = {}
         self.add_url_rule('/extension_asset', methods=['GET'], view_func=self.extension_asset)
         self.analogic_applications = {}
 
@@ -63,27 +67,51 @@
     def get_condition_module_name(self, name):
         return self.conditions[name]
 
     def get_authentication_provider_module_name(self, name):
         return self.authentication_providers[name]
 
     def register_application(self, application_dir, blueprint: "Blueprint", **options: t.Any) -> None:
-        instance = '/' + blueprint.name
-        self.register_analogic_url_rules(instance)
+        try:
+            instance = '/' + blueprint.name
+            self.register_analogic_url_rules(instance)
 
-        self.analogic_applications[blueprint.name] = application_dir
+            self.analogic_applications[blueprint.name] = self.create_authentication_provider(blueprint.name,
+                                                                                         application_dir)
 
-        super().register_blueprint(blueprint, **options)
+            super().register_blueprint(blueprint, **options)
+        except Exception as e:
+            logging.getLogger(__name__).error('Error registering application' + blueprint.name + ': ' + str(e))
+
+    def create_authentication_provider(self, analogic_application, analogic_application_path):
+        with self.app_context():
+            setting = SettingManager(analogic_application_path, analogic_application)
+            config = setting.config
+
+            class_name = config['authenticationMode']
+            module_name = self.get_authentication_provider_module_name(class_name)
+
+            if module_name in sys.modules:
+                module = sys.modules[module_name]
+            else:
+                module = importlib.import_module(module_name)  # Todo ModuleNotFoundError
+
+            authentication_provider_class = getattr(module, class_name)
+            authentication_provider = authentication_provider_class(setting)
+
+            authentication_provider.initialize()
+
+            return authentication_provider
 
     def get_analogic_application(self):
         s = request.path.split('/')
         if len(s) > 2 and s[1] in self.analogic_applications:
-            return s[1], self.analogic_applications[s[1]]
+            return self.analogic_applications[s[1]]
         else:
-            return 'default', self.analogic_applications['default']
+            return self.analogic_applications['default']
 
     def register_extension_assets(self, assets):
         self.extension_assets.update(assets)
 
     def extension_asset(self):
         asset_name = request.args.get('asset_name')
         if asset_name in self.extension_assets:
@@ -96,33 +124,23 @@
     def get_extension_js_asset_names(self):
         return self._get_asset_by_ext('.js')
 
     def _get_asset_by_ext(self, ext):
         return list(filter(lambda x: x.endswith(ext), list(self.extension_assets.keys())))
 
     def get_authentication_provider(self):
-        analogic_application, analogic_application_path = self.get_analogic_application()
-        cache = self._get_cache()
-
-        setting = SettingManager(cache, analogic_application_path, analogic_application)
-        config = setting.get_config()
+        authentication_provider = self.get_analogic_application()
 
-        class_name = config['authenticationMode']
-        module_name = self.get_authentication_provider_module_name(class_name)
-
-        if module_name in sys.modules:
-            module = sys.modules[module_name]
+        session.permanent = True
+        config = authentication_provider.get_setting().get_config()
+        if config['authenticationMode'] != 'Cam':
+            self.permanent_session_lifetime = timedelta(minutes=config['sessionExpiresInMinutes'] - 1)
         else:
-            module = importlib.import_module(module_name)  # Todo ModuleNotFoundError
-
-        authentication_provider_class = getattr(module, class_name)
-        authentication_provider = authentication_provider_class(setting)
+            self.permanent_session_lifetime = timedelta(days=31)
 
-        session.permanent = True
-        self.permanent_session_lifetime = timedelta(minutes=config['sessionExpiresInMinutes'] - 1)
         return authentication_provider
 
     def evaluate_condition(self, config):
         class_name = config.get('authenticationModeCondition')
         module_name = self.get_condition_module_name(class_name)
 
         if module_name in sys.modules:
@@ -130,17 +148,18 @@
         else:
             module = importlib.import_module(module_name)  # Todo ModuleNotFoundError
 
         condition_class = getattr(module, class_name)
         condition = condition_class()
         return condition.get_authentication_provider_name(config)
 
-    def _get_cache(self):
-        cache_path = os.path.join(self.instance_path, 'cache')
-        return Cache(self, config={'CACHE_TYPE': 'FileSystemCache', 'CACHE_DIR': cache_path})
+    def on_exit(self):
+        print('on_exit')
+        for app_name in self.analogic_applications:
+            self.analogic_applications[app_name].on_exit()
 
 
 def page_not_found(e):
     return render_template('404.html'), 404
 
 
 def page_error(e):
@@ -170,14 +189,20 @@
         _load_applications(app, register_func=_register_application, module_dirs=APPLICATIONS_DIR_EXTRA)
 
     app.register_analogic_url_rules('')
 
     app.register_error_handler(404, page_not_found)
     app.register_error_handler(500, page_error)
 
+    scheduler.init_app(app)
+
+    scheduler.start()
+
+    atexit.register(app.on_exit)
+
     return app
 
 
 def _load_logging(app):
     logs_folder_path = os.path.join(app.instance_path, 'logs')
     if not os.path.exists(logs_folder_path):
         os.makedirs(logs_folder_path)
@@ -260,15 +285,15 @@
 
             # workaround to handle repeating names in module path
             if module_dir_name == modules_dir.rsplit('/', 1)[-1]:
                 module_dir_name = module_dir_name + '.' + module_dir_name
 
             files = resources.contents(module_dir_name)
 
-            modules = [f[:-3] for f in files if f.endswith(".py") and f[0] != "_" and f != 'setup.py']
+            modules = [f[:-3] for f in files if f.endswith(".py") and f[0] != "_" and 'setup' not in f]
             register_func(app, module_dir, module_dir_name, modules)
 
 
 def _register_application(app, application_dir, application_name, files):
     for file in files:
         module = application_name + '.' + file
```

### Comparing `analogic-framework-4.0.2/analogic/authentication_provider.py` & `analogic-framework-4.1.0/analogic/authentication_provider.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,61 @@
-from flask import session, current_app, send_file, json, request, jsonify
+from flask import session, current_app, send_file, request, jsonify
 from analogic.loader import ClassLoader
 import analogic.pivot as PivotApi
+from analogic.exceptions import AnalogicProxyException
 import logging
 import pandas as pd
 from abc import ABC, abstractmethod
 from functools import wraps
+import orjson
 
 pd.set_option('display.float_format', lambda x: '%.3f' % x)
 
 
 def get_authentication_provider():
     return current_app.get_authentication_provider()
 
 
 def endpoint_login_required(f):
     @wraps(f)
     def decorated_function(*args, **kwargs):
         auth_provider = get_authentication_provider()
-        if auth_provider.check_app_authenticated() is False:
+        if auth_provider.check_app_authenticated is False:
             return auth_provider.get_authentication_required_response()
         return f(*args, **kwargs)
 
     return decorated_function
 
 
 def login_required(f):
     @wraps(f)
     def decorated_function(*args, **kwargs):
         auth_provider = args[0]
-        if auth_provider.check_app_authenticated() is False:
+        if auth_provider.check_app_authenticated is False:
             return auth_provider.get_authentication_required_response()
         return f(*args, **kwargs)
 
     return decorated_function
 
 
 class AuthenticationProvider(ABC):
+    HEADERS = {'Connection': 'keep-alive',
+               'User-Agent': 'Analogic',
+               'Content-Type': 'application/json; odata.streaming=true; charset=utf-8',
+               'Accept': 'application/json;odata.metadata=none,text/plain',
+               'Accept-Encoding': 'gzip, deflate, br',
+               'TM1-SessionContext': 'Analogic'}
 
     def __init__(self, setting):
         self.setting = setting
         self.logged_in_user_session_name = self.setting.get_instance() + '_logged_in_user_name'
+        self._logger = logging.getLogger(self.setting.get_instance())
+
+    def initialize(self):
+        self.setting.initialize()
 
     def get_setting(self):
         return self.setting
 
     def get_logged_in_user_name(self):
         return session.get(self.logged_in_user_session_name)
 
@@ -55,15 +67,15 @@
         cube_name = v.get('cube_name')
         dimension_name = v.get('dimension_name')
         hierarchy_name = v.get('hierarchy_name')
         subset_name = v.get('subset_name')
         element_names = v.getlist('element_names[]')
         subset_name_to_remove = v.get('subset_name_to_remove')
         selected_cards = v.get('selected_cards')
-        options = json.loads(v.get('options', '{}'))
+        options = orjson.loads(v.get('options', '{}'))
         export_data = v.get('export_data')
 
         return PivotApi.call(self.get_tm1_service(), username, cube_name, dimension_name, hierarchy_name, subset_name,
                              element_names, subset_name_to_remove, selected_cards, options, export_data)
 
     @login_required
     def export(self):
@@ -95,23 +107,23 @@
         description = self.setting.get_custom_object_description(key)
 
         return ClassLoader().call(description, request, self.get_tm1_service(), self.setting, self)
 
     def _get_server_side_mdx(self):
         mdx = request.data
         if request.args.get('server') is not None:
-            body = json.loads(request.data)
+            body = orjson.loads(request.data)
             key = body['key']
             if body.get('key_suffix') is not None:
                 key = key + '_' + body['key_suffix']
             mdx = self.setting.get_mdx(key)
+            mdx = self._set_custom_mdx_data(mdx)
             for k in body:
                 mdx = mdx.replace('$' + k, body[k].replace('"', '\\"'))
 
-            mdx = self._set_custom_mdx_data(mdx)
             return mdx.encode('utf-8')
 
         return mdx
 
     @abstractmethod
     def index(self):
         pass
@@ -150,40 +162,46 @@
 
         url = target_url + "/" + sub_path + (
             "?" + request.query_string.decode('UTF-8') if len(
                 request.query_string) > 0 else "")
 
         method = request.method
 
-        headers: dict[str, str] = {'Content-Type': 'application/json; charset=utf-8',
-                                   'Accept-Encoding': 'gzip, deflate, br'}
+        headers: dict[str, str] = self.HEADERS.copy()
         cookies: dict[str, str] = {}
 
-        response = self.do_proxy_request(url, method, mdx, headers, cookies)
+        try:
+            response = self.do_proxy_request(url, method, mdx, headers, cookies, False)
+        except AnalogicProxyException as e:
+            self._logger.error(e)
+            return 'Something went wrong', 500, {'Content-Type': 'application/json'}
 
         if response.status_code == 400 or response.status_code == 500:
-            logger = self.getLogger()
-            logger.error('MDX error: ' + response.text)
-            logger.error('MDX: ' + mdx.decode('utf-8'))
+            self._logger.error('MDX error: ' + response.get_decompressed_data())
+            self._logger.error('MDX: ' + mdx.decode('utf-8'))
 
-        return response.text, response.status_code, {'Content-Type': 'application/json'}
+        if response.status_code == 401:
+            return 'Authentication required', 401, {'Content-Type': 'application/json'}
 
-    def do_proxy_request(self, url, method, mdx, headers=None, cookies=None):
+        return response.content, response.status_code, {
+            'Content-Type': 'application/json; odata.metadata=minimal; odata.streaming=true; charset=utf-8',
+            'Content-Encoding': 'gzip'}
+
+    def do_proxy_request(self, url, method, mdx, headers=None, cookies=None, decode_content=True):
 
         if headers is None:
-            headers: dict[str, str] = {'Content-Type': 'application/json; charset=utf-8',
-                                       'Accept-Encoding': 'gzip, deflate, br'}
+            headers: dict[str, str] = self.HEADERS.copy()
 
         if cookies is None:
             cookies: dict[str, str] = {}
 
-        return self._create_request_with_authenticated_user(url, method, mdx, headers, cookies)
+        return self._create_request_with_authenticated_user(url, method, mdx, headers, cookies, decode_content)
 
     @abstractmethod
-    def _create_request_with_authenticated_user(self, url, method, mdx, headers, cookies):
+    def _create_request_with_authenticated_user(self, url, method, mdx, headers, cookies, decode_content=True):
         pass
 
     @abstractmethod
     def _extend_login_session(self):
         pass
 
     @abstractmethod
@@ -195,8 +213,11 @@
         return jsonify({'username': self.get_logged_in_user_name()})
 
     def logout(self):
         session.clear()
         return 'ok'
 
     def getLogger(self):
-        return logging.getLogger(self.setting.get_instance())
+        return self._logger
+
+    def on_exit(self):
+        pass
```

### Comparing `analogic-framework-4.0.2/analogic/core_endpoints.py` & `analogic-framework-4.1.0/analogic/core_endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     return get_authentication_provider().active_user()
 
 
 @core_endpoints.analogic_endpoint_route('/auth', methods=['POST'])
 def auth():
     return get_authentication_provider().auth()
 
+
 @core_endpoints.analogic_endpoint_route('/logout', methods=['GET'])
 def logout():
     return get_authentication_provider().logout()
 
 
 @core_endpoints.analogic_endpoint_route('/export', methods=['GET', 'POST'])
 def export():
@@ -39,21 +40,20 @@
 
 
 @core_endpoints.analogic_endpoint_route('/clearcache', methods=['GET'])
 def clear_cache():
     return get_authentication_provider().setting.clear_cache()
 
 
-@core_endpoints.analogic_endpoint_route('/ping', methods=['GET'])
-def ping():
-    return get_authentication_provider().ping()
+# @core_endpoints.analogic_endpoint_route('/ping', methods=['GET'])
+# def ping():
+#     return get_authentication_provider().ping()
 
 
 @core_endpoints.analogic_endpoint_route('/pivot', methods=['GET', 'POST'])
 def pivot():
     return get_authentication_provider().pivot()
 
 
 @core_endpoints.analogic_endpoint_route('/middleware', methods=['GET', 'POST'])
 def middleware():
     return get_authentication_provider().middleware()
-
```

### Comparing `analogic-framework-4.0.2/analogic/email.py` & `analogic-framework-4.1.0/analogic/email.py`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/endpoint.py` & `analogic-framework-4.1.0/analogic/endpoint.py`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/loader.py` & `analogic-framework-4.1.0/analogic/loader.py`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/logging.json` & `analogic-framework-4.1.0/analogic/logging.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9638888888888889%*

 * *Differences: {"'handlers'": "{'scheduler_file_handler': OrderedDict([('class', "*

 * *               "'logging.handlers.RotatingFileHandler'), ('level', 'INFO'), ('formatter', "*

 * *               "'simple'), ('filename', 'logs/scheduler.log'), ('maxBytes', 10485760), "*

 * *               "('backupCount', 20), ('encoding', 'utf8')])}",*

 * * "'loggers'": "{'scheduler': OrderedDict([('level', 'INFO'), ('handlers', "*

 * *              "['scheduler_file_handler']), ('propagate', False)])}"}*

```diff
@@ -66,14 +66,23 @@
             "class": "logging.handlers.RotatingFileHandler",
             "encoding": "utf8",
             "filename": "logs/login_json.log",
             "formatter": "json",
             "level": "INFO",
             "maxBytes": 10485760
         },
+        "scheduler_file_handler": {
+            "backupCount": 20,
+            "class": "logging.handlers.RotatingFileHandler",
+            "encoding": "utf8",
+            "filename": "logs/scheduler.log",
+            "formatter": "simple",
+            "level": "INFO",
+            "maxBytes": 10485760
+        },
         "werkzeug_file_handler": {
             "backupCount": 20,
             "class": "logging.handlers.RotatingFileHandler",
             "encoding": "utf8",
             "filename": "logs/werkzeug.log",
             "formatter": "simple",
             "level": "INFO",
@@ -94,14 +103,21 @@
             "handlers": [
                 "login_file_handler",
                 "login_json_file_handler"
             ],
             "level": "INFO",
             "propagate": false
         },
+        "scheduler": {
+            "handlers": [
+                "scheduler_file_handler"
+            ],
+            "level": "INFO",
+            "propagate": false
+        },
         "werkzeug": {
             "handlers": [
                 "console",
                 "werkzeug_file_handler",
                 "werkzeug_json_file_handler"
             ],
             "level": "INFO",
```

### Comparing `analogic-framework-4.0.2/analogic/loginbasic.py` & `analogic-framework-4.1.0/analogic/nologin.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,75 +1,42 @@
-import requests
 from analogic.authentication_provider import AuthenticationProvider
-from flask import render_template, request, make_response, redirect, session
-from TM1py.Services import TM1Service
+from flask import render_template, make_response, redirect, session, jsonify
 import logging
 
 
-class LoginBasic(AuthenticationProvider):
+class NoLogin(AuthenticationProvider):
 
     def __init__(self, setting):
         super().__init__(setting)
 
     def index(self):
         cnf = self.setting.get_config()
-        if self.logged_in_user_session_name in session:
-            return render_template('index.html', authenticated=True, cnf=cnf)
-        return redirect(self.setting.get_base_url('login'))
 
-    def login(self):
-        cnf = self.setting.get_config()
-        if request.method == 'POST':
-
-            response = requests.request(url=self.setting.get_proxy_target_url() + cnf['apiSubPath'] + 'ActiveUser',
-                                        method='GET',
-                                        auth=(request.form['username'], request.form['password']),
-                                        verify=False)
+        resp = make_response(render_template('index.html', authenticated=True, cnf=cnf))
 
-            if response.status_code == 200:
-                session[self.logged_in_user_session_name] = request.form['username']
-                session['permanent'] = True
+        session[self.logged_in_user_session_name] = 'nologin'
 
-                self.setting.set_tm1_session_id(response.cookies.get('TM1SessionId'),
-                                                session[self.logged_in_user_session_name])
+        return self._add_authenticated_cookies(resp, 86400)
 
-                resp = make_response(redirect(self.setting.get_base_url()))
-
-                return self._add_authenticated_cookies(resp)
-
-        return render_template('login.html', cnf=cnf)
+    def login(self):
+        return redirect(self.setting.get_base_url())
 
     def _create_request_with_authenticated_user(self, url, method, mdx, headers, cookies):
-        tm1_session_id = self.setting.get_tm1_session_id(session[self.logged_in_user_session_name])
-
-        cookies["TM1SessionId"] = tm1_session_id
-
-        response = requests.request(
-            url=url,
-            method=method,
-            data=mdx,
-            headers=headers,
-            cookies=cookies,
-            verify=False)
-
-        return response
+        return {}
 
     def check_app_authenticated(self):
-        if self.logged_in_user_session_name in session:
-            return True
-        return False
+        return True
 
     def get_authentication_required_response(self):
-        return redirect(self.setting.get_base_url('login'))
+        return redirect(self.setting.get_base_url())
 
     def _extend_login_session(self):
         session.modified = True
 
     def get_tm1_service(self):
-        cnf = self.setting.get_config()
-
-        tm1_session_id = self.setting.get_tm1_session_id(session[self.logged_in_user_session_name])
+        return None
 
-        return TM1Service(base_url=cnf['apiHost'], session_id=tm1_session_id, ssl=False)
+    def active_user(self):
+        return jsonify({'username': session[self.logged_in_user_session_name]})
 
     def getLogger(self):
         return logging.getLogger(__name__)
```

### Comparing `analogic-framework-4.0.2/analogic/pivot.py` & `analogic-framework-4.1.0/analogic/pivot.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         p = options['processParams']
         p['pUser'] = username
         p['pValue'] = json.dumps(p['pValue'])
         r = tm1.processes.execute_with_return(options['process'], **p)
         return jsonify(r)
     elif dimension_name is None:
         children = tm1.cubes.get_dimension_names(cube_name)
-        data = get_presets_data(tm1, username)
+        data = get_presets_data(tm1, username, options['widgetId'])
     elif hierarchy_name is None:
         children = tm1.hierarchies.get_all_names(dimension_name)
     elif subset_name is None:
         hierarchy = tm1.hierarchies.get(dimension_name, hierarchy_name)
         data['defaultMember'] = hierarchy.default_member
         data['aliasAttributeNames'] = get_alias_attribute_names(hierarchy)
         children, data['privateSubsets'] = get_public_and_private_subsets(tm1, dimension_name, hierarchy_name, username, options)
@@ -61,41 +61,44 @@
             subset_name = username + '_' + subset_name
         subset = tm1.subsets.get(subset_name, dimension_name, hierarchy_name, is_private_subset)
         data['defaultAliasAttributeName'] = subset.alias
         data['children'] = get_elements_with_aliases(tm1, subset, is_private_subset)
 
     return jsonify({'children': children, 'data': data})
 
-def get_presets_data(tm1, username):
+def get_presets_data(tm1, username, widget_id):
     mdx = """WITH
 MEMBER [Measures zSYS Analogic Pivot Presets].[Measures zSYS Analogic Pivot Presets].[sType]
 AS [zSYS Analogic Pivot Presets].[zSYS Analogic Pivot Presets].CurrentMember.Properties('Type')
 MEMBER [Measures zSYS Analogic Pivot Presets].[Measures zSYS Analogic Pivot Presets].[sOwner]
 AS
 IIF('""" + username + """' = [zSYS Analogic Pivot Presets].[zSYS Analogic Pivot Presets].CurrentMember.Properties('CreatedBy'),
 1,0)
 MEMBER [Measures zSYS Analogic Pivot Presets].[Measures zSYS Analogic Pivot Presets].[sID]
 AS [zSYS Analogic Pivot Presets].[zSYS Analogic Pivot Presets].CurrentMember.Name
+MEMBER [Measures zSYS Analogic Pivot Presets].[Measures zSYS Analogic Pivot Presets].[sWidgetID]
+AS [zSYS Analogic Pivot Presets].[zSYS Analogic Pivot Presets].CurrentMember.Properties('WidgetID')
 SELECT
    {[Measures zSYS Analogic Pivot Presets].[Measures zSYS Analogic Pivot Presets].[sID],
+    [Measures zSYS Analogic Pivot Presets].[Measures zSYS Analogic Pivot Presets].[sWidgetID],
     [Measures zSYS Analogic Pivot Presets].[Measures zSYS Analogic Pivot Presets].[sType],
     [Measures zSYS Analogic Pivot Presets].[Measures zSYS Analogic Pivot Presets].[sOwner],
     [Measures zSYS Analogic Pivot Presets].[Measures zSYS Analogic Pivot Presets].[sName],
     [Measures zSYS Analogic Pivot Presets].[Measures zSYS Analogic Pivot Presets].[sValue]
    }
   ON COLUMNS ,
-   UNION({
+   FILTER(UNION({
         FILTER({
             [zSYS Analogic Pivot Presets].[zSYS Analogic Pivot Presets].Members
         }, INSTR([zSYS Analogic Pivot Presets].[zSYS Analogic Pivot Presets].CurrentMember.Properties('Type'), 'Public') > 0)
 },{
     FILTER({
         [zSYS Analogic Pivot Presets].[zSYS Analogic Pivot Presets].Members
     }, INSTR([zSYS Analogic Pivot Presets].[zSYS Analogic Pivot Presets].CurrentMember.Properties('CreatedBy'), '""" + username + """') > 0)
-})
+}),INSTR([zSYS Analogic Pivot Presets].[zSYS Analogic Pivot Presets].CurrentMember.Properties('WidgetID'), '""" + widget_id + """') > 0)
   ON ROWS
 FROM [zSYS Analogic Pivot Presets]"""
 
     cellset_id = tm1.cells.create_cellset(mdx)
     url = "/api/v1/Cellsets('" + cellset_id + "')?$expand=Cells($select=FormattedValue)"
     data = tm1._tm1_rest.GET(url).json()
```

### Comparing `analogic-framework-4.0.2/analogic/setting.py` & `analogic-framework-4.1.0/analogic/setting.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,171 +1,150 @@
-import datetime
 import yaml
 import os
 from flask import json, current_app, url_for, request, render_template
 import logging
 import uuid
+import sys
+import importlib
 
 
 class SettingManager:
-    CONFIG = 'dimension_framework_config'
-    REPOSITORY = 'dimension_framework_repository'
-    CLASSES = 'dimension_framework_classes'
-    TM1SessionId = 'dimension_framework_tm1_session_id'
-    TM1SessionExpires = 'dimension_framework_tm1_session_expires'
 
-    def __init__(self, cache, analogic_application_path, instance='default'):
-        self.cache = cache
+    def __init__(self, analogic_application_path, instance='default'):
         self.site_root = analogic_application_path
         self.instance = instance
+        self.config = self._create_config()
+        self.repository = self._create_repository()
+        self.custom_objects = self._create_custom_objects()
+        self._logger = logging.getLogger(self.get_instance())
+        self.tm1_services = {}
+
+    def initialize(self):
+        pass
 
     def clear_cache(self):
-        if self.cache is not None:
-            self.cache.delete(self._get_config_cache_key())
-            self.cache.delete(self._get_repository_cache_key())
-            self.cache.delete(self._get_tm1_session_id_cache_key())
-            self.cache.delete(self._get_tm1_session_expires_cache_key())
-            self.cache.delete(self._get_classes_cache_key())
+        self.repository = self._create_repository()
+        self.custom_objects = self._create_custom_objects()
+        self.config = None
+        self.config = self._create_config()
+        self.save_config_js()
+        self.reload_custom_objects()
         return "OK"
 
+    def reload_custom_objects(self):
+        namespaces = set(map(lambda o: self.custom_objects[o].get('namespace'), self.custom_objects))
+        for namespace in namespaces:
+            if namespace is not None:
+                try:
+                    importlib.reload(sys.modules[namespace])
+                except Exception as e:
+                    self._logger.error(e)
+
     def get_instance(self):
         return self.instance
 
-    def _get_config_cache_key(self):
-        return self._get_instance_cache_key(self.CONFIG)
-
-    def _get_repository_cache_key(self):
-        return self.get_instance() + '_' + self.REPOSITORY
+    def _create_config(self):
+        return self._get_json_setting('app')
 
-    def _get_tm1_session_id_cache_key(self):
-        return self._get_instance_cache_key(self.TM1SessionId)
-
-    def _get_tm1_session_expires_cache_key(self):
-        return self._get_instance_cache_key(self.TM1SessionExpires)
-
-    def _get_classes_cache_key(self):
-        return self._get_instance_cache_key(self.CLASSES)
+    def get_config(self):
+        if not os.path.exists(os.path.join(self.site_root, 'static', 'assets', 'js', 'config.js')):
+            self.save_config_js()
 
-    def _get_instance_cache_key(self, key):
-        return self.get_instance() + '_' + key
+        if self.config.get('authenticationModeCondition') is not None:
+            self.config['authenticationMode'] = current_app.evaluate_condition(self.config)
 
-    def get_config(self):
-        cnf = self._get_json_setting(self._get_config_cache_key(), 'app')
-        return cnf
+        if self.config is not None:
+            return self.config
+        self.config = self._get_json_setting('app')
+        self.save_config_js()
+        return self.config
 
     def _get_param(self, param_name):
-        cnf = self.get_config()
-        return cnf[param_name]
+        return self.config[param_name]
 
     def get_base_url(self, route=''):
         base = url_for('core_endpoints.index')
         url = request.environ.get('wsgi.url_scheme') + '://' + request.environ.get('HTTP_HOST')
         sub_path = [base[:-1], self.instance, route]
-        return url + ('/'.join(filter(lambda x : x != 'default' and x is not None, sub_path)))
+        return url + ('/'.join(filter(lambda x: x != 'default' and x is not None, sub_path)))
+
+    def _create_repository(self):
+        return self._get_yaml_setting(os.path.join('server', 'configs', 'repository'))
 
     def _get_repository(self):
-        return self._get_yaml_setting(self._get_repository_cache_key(), os.path.join('server', 'configs', 'repository'))
+        if self.repository is not None:
+            return self.repository
+        return self._get_yaml_setting(os.path.join('server', 'configs', 'repository'))
 
     def get_mdx(self, key):
         repository = self._get_repository()
         mdx = repository[key]
         return mdx
 
-    def _get_json_setting(self, key, file_name):
-        setting = self._cache_get(key)
-        if setting is None:
-            json_url = os.path.join(self.site_root, file_name + '.json')
-            with open(json_url, encoding="utf-8") as f:
-                setting = json.load(f)
-
-            if file_name == 'app':
-                setting['instance'] = self.instance
-                setting['blueprint_static'] = self.instance + '.static'
-                setting['extension_css_asset_names'] = current_app.get_extension_css_asset_names()
-                setting['extension_js_asset_names'] = current_app.get_extension_js_asset_names()
-                setting['version'] = uuid.uuid4().hex[:6].upper()
+    def _get_json_setting(self, file_name):
 
-                if setting.get('apiSubPath') is None:
-                    setting['apiSubPath'] = '/api/v1/'
+        json_url = os.path.join(self.site_root, file_name + '.json')
+        with open(json_url, encoding="utf-8") as f:
+            setting = json.load(f)
 
-                if setting.get('authenticationBridge') is None:
-                    setting['authenticationBridge'] = ''
+        if file_name == 'app':
+            setting['instance'] = self.instance
+            setting['blueprint_static'] = self.instance + '.static'
+            setting['extension_css_asset_names'] = current_app.get_extension_css_asset_names()
+            setting['extension_js_asset_names'] = current_app.get_extension_js_asset_names()
+            setting['version'] = uuid.uuid4().hex[:6].upper()
 
-                if setting.get('sessionExpiresInMinutes') is None:
-                    setting['sessionExpiresInMinutes'] = 20
+            if setting.get('apiSubPath') is None:
+                setting['apiSubPath'] = '/api/v1/'
 
-                if setting.get('useMinifiedAssets') is None:
-                    setting['useMinifiedAssets'] = False
+            if setting.get('authenticationBridge') is None:
+                setting['authenticationBridge'] = ''
 
-                if setting.get('ssl_verify') is None:
-                    setting['ssl_verify'] = True
+            if setting.get('sessionExpiresInMinutes') is None:
+                setting['sessionExpiresInMinutes'] = 20
 
-                self.save_config_js(setting)
+            if setting.get('useMinifiedAssets') is None:
+                setting['useMinifiedAssets'] = False
 
-            self._cache_set(key, setting, 0)
+            if setting.get('ssl_verify') is None:
+                setting['ssl_verify'] = True
 
-        if setting.get('authenticationModeCondition') is not None:
-            setting['authenticationMode'] = current_app.evaluate_condition(setting)
         return setting
 
-    def save_config_js(self, config):
+    def save_config_js(self):
         js_url = os.path.join(self.site_root, 'static', 'assets', 'js', 'config.js')
         with open(js_url, 'w', encoding="utf-8") as f:
-            f.write(render_template('config.html', cnf=config))
+            f.write(render_template('config.html', cnf=self.config))
 
-    def _get_yaml_setting(self, key, file_path):
-        setting = self._cache_get(key)
-        if setting is None:
-            with open(os.path.join(self.site_root, file_path + '.yml'), encoding="utf-8") as file:
-                setting = yaml.safe_load(file)
-                self._cache_set(key, setting, 0)
+    def _get_yaml_setting(self, file_path):
+        with open(os.path.join(self.site_root, file_path + '.yml'), encoding="utf-8") as file:
+            setting = yaml.safe_load(file)
         return setting
 
+    def _create_custom_objects(self):
+        return self._get_json_setting(os.path.join('server', 'configs', 'custom_objects'))
+
     def get_custom_object_description(self, key):
-        classes = self._get_json_setting(self._get_classes_cache_key(), os.path.join('server', 'configs', 'custom_objects'))
-        return classes[key]
+        if self.custom_objects is None:
+            self.custom_objects = self._create_custom_objects()
+        return self.custom_objects[key]
+
+    def set_tm1_service(self, user_name, tm1_service):
+        self.tm1_services[user_name] = tm1_service
 
-    def set_tm1_session_id(self, tm1_session_id, suffix=''):
-        cnf = self.get_config()
-        self._cache_set(self._get_tm1_session_id_cache_key() + suffix, tm1_session_id, 0)
-        expires = datetime.datetime.now() + datetime.timedelta(minutes=cnf['sessionExpiresInMinutes'] - 1)
-        self._cache_set(self._get_tm1_session_expires_cache_key() + suffix, expires, 0)
-
-    def get_tm1_session_id(self, suffix=''):
-        logger = self.getLogger()
-        logger.info(self._get_tm1_session_id_cache_key() + suffix)
-        tm1_session_id = self._cache_get(self._get_tm1_session_id_cache_key() + suffix)
-        logger.info(tm1_session_id)
-        tm1_session_id_exp = self._cache_get(self._get_tm1_session_expires_cache_key() + suffix)
-        logger.info(tm1_session_id_exp)
-        if tm1_session_id is None or (
-                tm1_session_id_exp is not None and datetime.datetime.now() >= tm1_session_id_exp):
-            return None
-        return tm1_session_id
+    def get_tm1_service(self, user_name):
+        return self.tm1_services.get(user_name)
 
     def get_proxy_target_url(self):
-        cnf = self.get_config()
-        return cnf['proxy']['target']
+        return self.config['proxy']['target']
 
     def get_app_cam_namespace(self):
-        cnf = self.get_config()
-        return cnf['camNamespace']
+        return self.config['camNamespace']
 
     def get_smtp_password(self):
-        cnf = self.get_config()
-        return cnf['smtp']['password']
+        return self.config['smtp']['password']
 
     def get_ssl_verify(self):
-        cnf = self.get_config()
-        return cnf['ssl_verify']
-
-    def _cache_get(self, key):
-        if self.cache is not None:
-            return self.cache.get(key)
-        return None
-
-    def _cache_set(self, key, value, expires=0):
-        if self.cache is not None:
-            self.cache.set(key, value, expires)
+        return self.config['ssl_verify']
 
     def getLogger(self):
-        return logging.getLogger(self.get_instance())
+        return self._logger
```

### Comparing `analogic-framework-4.0.2/analogic/static/assets/css/bootstrap-grid.min.css` & `analogic-framework-4.1.0/analogic/static/assets/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/css/bootstrap-grid.min.css.map` & `analogic-framework-4.1.0/analogic/static/assets/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/css/lib/Chart-2.9.3.min.css` & `analogic-framework-4.1.0/analogic/static/assets/css/lib/Chart-2.9.3.min.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/css/lib/nouislider.min.css` & `analogic-framework-4.1.0/analogic/static/assets/css/lib/nouislider.min.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/css/style.css` & `analogic-framework-4.1.0/analogic/static/assets/css/style.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/css/widgets/simulation-panel-slider.css` & `analogic-framework-4.1.0/analogic/static/assets/css/widgets/simulation-panel-slider.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/images/loading.gif` & `analogic-framework-4.1.0/analogic/static/assets/images/loading.gif`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/images/loading2.gif` & `analogic-framework-4.1.0/analogic/static/assets/images/loading2.gif`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/images/loading2_transparent.gif` & `analogic-framework-4.1.0/analogic/static/assets/images/loading2_transparent.gif`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/images/triangle.png` & `analogic-framework-4.1.0/analogic/static/assets/images/triangle.png`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/framework/api.js` & `analogic-framework-4.1.0/analogic/static/assets/js/framework/api.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -67,118 +67,123 @@
 };
 
 Api.jumpTo = function jumpTo(id) {
     window.location.href = '#' + id;
 };
 
 Api.openPage = function openPage(page) {
-    Render.showPage(page);
+    return Render.showPage(page);
 };
 
 Api.backToMain = function backToMain() {
-    Render.showPage(app.mainPage);
+    return Render.showPage(app.mainPage);
 };
 
 Api.openPrevPage = function openPrevPage() {
     if (PageState.previous !== '') {
-        Render.showPage(PageState.previous);
+        return Render.showPage(PageState.previous);
     }
+    return $.Deferred().resolve('');
 };
 
 Api.openPrevPageWithState = function openPrevPageWithState() {
     if (PageState.previous !== '') {
-        Render.showPage(PageState.previous, true);
+        return Render.showPage(PageState.previous, true);
     }
+    return $.Deferred().resolve('');
 };
 
 Api.openPageWithWaitingForEvent = function openPageWithWaitingForEvent(arg) {
     if (!Array.isArray(arg) || arg.length < 2) {
         alert('openPageWithWaitingForEvent has 2 mandatory argument: ["eventName", "pageId"] !');
 
-        return;
+        return $.Deferred().resolve('');;
     }
 
     Loader.start();
 
     El.body.on(arg[0], () => Render.showPage(arg[1]));
 };
 
 Api.openPageAndScrollToSection = function openPageAndScrollToSection(arg) {
-    Render.showPage(arg[0]);
+    let r = Render.showPage(arg[0]);
 
     El.body.on('bodyReady', () => {
         El.body.off('bodyReady');
         Api.jumpTo(arg[1]);
     });
+    return r;
 };
 
 Api.openPageWithWaitingForEventAndScrollToSection = function openPageWithWaitingForEventAndScrollToSection(arg) {
     if (!Array.isArray(arg) || arg.length < 3) {
         alert('openPageWithWaitingForEventAndScrollToSection has 3 mandatory argument: ["eventName", "pageId", "section"] !');
 
-        return;
+        return $.Deferred().resolve('');
     }
     Loader.start();
 
     El.body.on(arg[0], () => {
         Render.showPage(arg[1]);
 
         El.body.on('bodyReady', () => {
             El.body.off('bodyReady');
             Api.jumpTo(arg[2]);
         });
     });
 };
 
-Api.openPageWithState = function openPageWithState(page) {
+Api.openPageWithState = function openPageWithState(page, alsoForceRefreshWidgetsWithState = false) {
     if (Array.isArray(page)) {
         if (PageState[page[0]]) {
-            Render.showPage(page[0], true);
+            let r = Render.showPage(page[0], true);
             El.body.on('bodyReady', () => {
                 El.body.off('bodyReady');
 
                 if (page.length > 1) {
                     for (let i = 1; i < page.length; ++i) {
-                        Api.forceRefresh(page[i]);
+                        alsoForceRefreshWidgetsWithState ? Api.forceRefreshWithState(page[i]) : Api.forceRefresh(page[i]);
                     }
                 }
             });
+            return r;
         } else {
-            Render.showPage(page[0]);
+            return Render.showPage(page[0]);
 
         }
     } else {
         if (PageState[page]) {
-            Render.showPage(page, true);
+            return Render.showPage(page, true);
         } else {
-            Render.showPage(page);
+            return Render.showPage(page);
         }
     }
 };
 
 Api.openPageWithStateAndScrollToSection = function openPageWithStateAndScrollToSection(arg) {
-    Render.showPage(arg[0], true);
+    let r = Render.showPage(arg[0], true);
 
     El.body.on('bodyReady', () => {
         El.body.off('bodyReady');
         Api.jumpTo(arg[1]);
 
         if (arg.length > 2) {
             for (let i = 2; i < arg.length; ++i) {
                 Api.forceRefresh(arg[i]);
             }
         }
     });
+    return r;
 };
 
 Api.openPageWithStateAndWaitingForEvent = function openPageWithStateAndWaitingForEvent(arg) {
     if (!Array.isArray(arg) || arg.length < 2) {
         alert('openPageWithStateAndWaitingForEvent has 2 mandatory argument: ["eventName", "pageId"] !');
 
-        return;
+        return $.Deferred().resolve('');
     }
 
     Loader.start();
 
     El.body.on(arg[0], () => {
         Render.showPage(arg[1], true);
 
@@ -194,15 +199,15 @@
     });
 };
 
 Api.openPageWithStateAndWaitingForEventAndScrollToSection = function openPageWithStateAndWaitingForEventAndScrollToSection(arg) {
     if (!Array.isArray(arg) || arg.length < 3) {
         alert('openPageWithStateAndWaitingForEventAndScrollToSection has 3 mandatory argument: ["eventName", "pageId", "sectionName"] !');
 
-        return;
+        return $.Deferred().resolve('');
     }
 
     Loader.start();
 
     El.body.on(arg[0], () => {
         Render.showPage(arg[1], true);
 
@@ -234,22 +239,22 @@
 };
 
 Api.removePageValues = function removePageValues(pageId) {
     let page = WidgetConfig[pageId],
         w;
 
     for (w of page.widgets) {
-        Widgets[w.id] = new Widgets[id].reset();
+        Widgets[w.id].reset();
         Api.removeValuesRecursively(w.widgets);
     }
 };
 
 Api.removeValuesRecursively = function removeValuesRecursively(widgets) {
     for (let w of widgets || []) {
-        Widgets[w.id] = new Widgets[id].reset();
+        Widgets[w.id].reset();
         Api.removeValuesRecursively(w.widgets);
     }
 };
 
 Api.showToolTipsChanged = function showToolTipsChanged() {
     $('.ks-button-info').toggle(Widgets.ShowTooltips === true);
 };
```

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/framework/app.js` & `analogic-framework-4.1.0/analogic/static/assets/js/framework/app.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -63,42 +63,50 @@
         }
 
         QB.getUserData().then(start);
     }).on('touchstart', () => app.isTouched = true);
 
     function loadWidget(wc, parent = Widgets, parentId = null) {
         if (wc.import) {
-            let wci = v(wc.import, WidgetConfig),
-                w = new wci.type(wci);
+            let wci = v(wc.import, WidgetConfig);
+            if (wci === false) {
+                console.error('WidgetConfig import error: ' + wc.import+' not found');
+            }
+            let w = new wci.type(wci);
             if (!parent[wci.id]) {
                 parent[wci.id] = w;
                 (wci.widgets || []).forEach(w => loadWidget(w, parent, wci.id));
             }
         } else {
+            if (wc.id.includes('_')) {
+                console.warn('Widget id must not contain underscore: ' + wc.id);
+            }
             if (parent[wc.id]) {
-                L('duplicated widgetid: ' + wc.id);
+                console.error('duplicated widgetid: ' + wc.id);
             }
             let wcc = new wc.type(wc);
             parent[wc.id] = wcc;
             (wc.widgets || []).forEach(w => loadWidget(w, parent, parentId));
         }
     }
 
     function start() {
         if (app.hasError) {
             return;
         }
 
         app.id = Utils.getRandomId();
 
+        app.checkScreenResolutionWarningDisplayed = false;
+
         initEvents();
 
-        Widgets.systemValueGlobalCompanyProductPlanVersion = 'Budget'; //Todo ez mi? Ne töröld, amíg nem nézem meg a bpspben (Ote)
+        Widgets.systemValueGlobalCompanyProductPlanVersion = 'Budget';
 
-        Widgets[app.mainPage].renderWidget();
+        Widgets[app.mainPage].renderWidget().then(() => Utils.checkScreenResolution());
     }
 
     function initEvents() {
         window.onbeforeunload = () => 'Logout';
     }
 
     function requestClipboarReadPermissionForFireFox() {
```

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/framework/authentication.js` & `analogic-framework-4.1.0/analogic/static/assets/js/framework/authentication.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -54,41 +54,38 @@
 Auth.handleSuccessLogin = () => {
     if ('Cam' === app.authenticationMode && $.cookie('camPassport') !== '0') {
         let date = new Date();
         date.setTime(date.getTime() + (app.sessionExpiresInMinutes * 60 * 1000));
         $.cookie("authenticated", 'authenticated', {
             expires: date
         });
-        if ('Cam' === app.authenticationMode) {
-            app.handled401 = false;
-        }
+        app.handled401 = false;
         //$.cookie("camPassport", 0);
     }
 
-    if (('Cam' === app.authenticationMode) && ((new Date().getTime() - app.pingTime) / 1000 >= 30)) {
-        app.pingTime = new Date().getTime();
-        $.ajax({
-            url: 'ping',
-            method: 'GET',
-            global: false,
-            success: function(data) {},
-            error: function(response, e) {},
-            statusCode: {}
-        });
+    if (['LoginBasic', 'LoginCam', 'CamSecure'].includes(app.authenticationMode)) {
+        app.handled401 = false;
     }
 
     Extensions.authenticationProviders.forEach(ext => ext.handleSuccessLogin());
 };
 
 Auth.handle401 = () => {
-    if ('Cam' === app.authenticationMode && app.handled401 === false) {
+    if (['Cam', 'CamSecure'].includes(app.authenticationMode) && app.handled401 === false) {
         app.handled401 = true;
         $.cookie("authenticated", 0);
         window.location.href = app.authenticationBridge;
     }
+    if ('LoginBasic' === app.authenticationMode || 'LoginCam' === app.authenticationMode) {
+        if (app.handled401 === false) {
+            app.handled401 = true;
+            // $.cookie("authenticated", 0);
+            window.location.href = 'login';
+        }
+    }
     Extensions.authenticationProviders.forEach(ext => ext.handle401());
 };
 
 Auth.getHeader = (contentType = 'application/json; charset=utf-8', accept = 'application/json; charset=utf-8') => {
     let headers = {};
 
     if (accept) {
```

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/framework/load-executor/array.js` & `analogic-framework-4.1.0/analogic/static/assets/js/framework/load-executor/array.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/framework/load-executor/base.js` & `analogic-framework-4.1.0/analogic/static/assets/js/framework/load-executor/base.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -91,16 +91,23 @@
 
     }
 
     handleAjaxResponse(data) {
 
         const ctx = this.context;
 
+
         if (data && data.ID) {
-            ctx.getRepositoryObject().cellsetId = data.ID;
+            const loaderFunctionNames = ctx.getLoaderFunctionName().split('_');
+            if (loaderFunctionNames.length > 1 && Array.isArray(ctx.getRepositoryObject()[loaderFunctionNames[0]])) {
+                const index = parseInt(loaderFunctionNames[1]) - 1;
+                ctx.getRepositoryObject()[loaderFunctionNames[0]][index].cellsetId = data.ID;
+            } else {
+                ctx.getRepositoryObject().cellsetId = data.ID;
+            }
         }
 
         if (!this.context.runParsingControl()) {
             return data;
         }
 
         return ParsingControlFactory.createExecutor(ctx, data).execute();
```

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/framework/load-executor/factory.js` & `analogic-framework-4.1.0/analogic/static/assets/js/framework/load-executor/factory.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/framework/parsing-control/base.js` & `analogic-framework-4.1.0/analogic/static/assets/js/framework/parsing-control/base.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/framework/parsing-control/factory.js` & `analogic-framework-4.1.0/analogic/static/assets/js/framework/parsing-control/factory.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -6,23 +6,18 @@
 
     static createExecutor(context, data) {
 
         const widgetId = context.getWidgetId(),
             repositoryObject = context.getRepositoryObject(),
             p = context.getRestRequest() !== false ? context.getRestRequest() : context.getLoaderFunction();
 
-        let dataContext = {
-                getLoaderResponse() {
-                    return data;
-                }
-            },
-            ctx = {
-                ...context,
-                ...dataContext
-            };
+        let ctx = Object.create(context);
+        ctx.getLoaderResponse = () => {
+            return data;
+        };
 
         if (isClass(p.parsingControl)) {
             return new p.parsingControl(ctx); //Todo check
         }
 
         if (p.parsingControl instanceof ParsingControl) {
             return p.parsingControl; // Todo check
```

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/framework/parsing-control/matrix.js` & `analogic-framework-4.1.0/analogic/static/assets/js/framework/parsing-control/matrix.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/framework/pivot.js` & `analogic-framework-4.1.0/analogic/static/assets/js/framework/pivot.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/framework/query-builder.js` & `analogic-framework-4.1.0/analogic/static/assets/js/framework/query-builder.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -80,15 +80,15 @@
     }
 };
 
 QB.getServerSideUrlAndBody = (url, body, repositoryId, path) => {
     let params = [],
         keyAdded = false,
         subUrl = url.includes('?') ? url.indexOf('?') !== (url.length - 1) ? '&server=1' : '' : '?server=1';
-    let newUrl = url.includes('proxy') ? url : app.apiHost ? url.replace(app.apiHost, 'proxy') : 'proxy' + url;
+    let newUrl = url.includes('proxy') ? url : url.includes(app.apiHost) ? url.replace(app.apiHost, 'proxy') : 'proxy' + url;
 
     for (const [key, value] of Object.entries(body)) {
         params.push(`"${key}": "${value}"`);
         if ('key' === key) {
             keyAdded = true;
         }
     }!keyAdded && params.push(`"key" : "${repositoryId + "_" + path}"`);
@@ -96,9 +96,12 @@
     return {
         url: newUrl + subUrl,
         body: `{${params.join(',')}}`
     };
 };
 
 QB.getUrl = (url) => {
-    return app.apiHost ? app.apiHost + url : url.includes('proxy') ? url : 'proxy' + url;
+    if (url.includes('proxy')) {
+        return url;
+    }
+    return app.apiHost ? app.apiHost + url : 'proxy' + url;
 };
```

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/framework/server.js` & `analogic-framework-4.1.0/analogic/static/assets/js/framework/server.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/framework/utils.js` & `analogic-framework-4.1.0/analogic/static/assets/js/framework/utils.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,20 @@
-/* global app, El, Doc, Intl, Widgets, WidgetState */
+/* global Api, app, El, Doc, Intl, Widgets, WidgetState */
 
 'use strict';
 const L = console.log,
-    v = (path, obj = Widgets) => path.split(".").reduce((o, key) => o && o[key] ? o[key] : false, obj),
+    v = (path, obj = Widgets) => {
+        let p = path.split('.');
+        if (p.length > 1 && obj[p[0]] && obj[p[0]] instanceof Widget &&
+            typeof obj[p[0]]['value'] === 'object' &&
+            typeof w(path, obj) === 'undefined') {
+            p.splice(1, 0, 'value');
+        }
+        return p.reduce((o, key) => o && o[key] ? o[key] : false, obj)
+    },
     w = (path, obj = Widgets) => path.split('.').reduce((o, key) => (o || {})[key], obj);
 
 const isClass = fn => fn && /^\s*class/.test(fn.toString());
 
 const Utils = {
     sleep: ms => new Promise(resolve => setTimeout(resolve, ms)),
     stopEvent(e) {
@@ -162,18 +170,19 @@
                 maxHeight = height;
             }
         }
 
         elements.height(maxHeight);
     },
     formatIntForChart: intVal => intVal.toString().replace(/\B(?=(\d{3})+(?!\d))/g, " "),
-    precisionRound(number, precision) {
-        const factor = Math.pow(10, precision);
+    precisionRound(number, precision, toFixed = false) {
+        const factor = Math.pow(10, precision),
+            n = Math.round(number * factor) / factor;
 
-        return Math.round(number * factor) / factor;
+        return toFixed ? n.toFixed(precision) : n;
     },
     backdrop: {
         show: () => {
             app.backdrop = app.backdrop || $('<div class="ks-container-backdrop">');
             El.body.prepend(app.backdrop);
         },
         hide: () => (app.backdrop || {}).remove()
@@ -277,14 +286,17 @@
                 return true;
             }
         }
         return false;
     },
     getDropBoxSelectedItemAttribute(widgetId, attributeName) {
         let selectedValue = Widgets[widgetId].value;
+        if (!Widgets[widgetId].items) {
+            return false;
+        }
         let item = Widgets[widgetId].items.find(e => e.name === selectedValue);
         return item ? item[attributeName] : false;
     },
     getCellsFromClipboard(widgetId) {
         let text = v(widgetId + '.clipboard');
         if (text === false) {
             return [];
@@ -383,17 +395,26 @@
     setWidgetValueIfNotExistByOther(key1, key2) {
         if (!Widgets[key1]) {
             Widgets[key1] = Widgets[key2];
         }
         return Widgets[key1];
     },
     setWidgetValue(key, value) {
+        if (Widgets[key] && Widgets[key] instanceof Widget) {
+            if (!value) {
+                Widgets[key].reset();
+            }
+            return;
+        }
         Widgets[key] = value;
     },
     setWidgetValueByOther(key1, key2) {
+        if (Widgets[key1] && Widgets[key1] instanceof Widget) {
+            return;
+        }
         Widgets[key1] = Widgets[key2];
     },
     getPropertyOrFunctionValue(object, property) {
         if (typeof object[property] === 'function') {
             return object[property]();
         }
         return object[property];
@@ -536,11 +557,65 @@
     focus(idOrObj, moveCursorToEnd = true) {
         let o = 'object' === typeof idOrObj ? idOrObj : $('#' + idOrObj),
             len = moveCursorToEnd ? o.val().length * 2 : 0;
 
         o.focus().promise().then(() => o[0].setSelectionRange(len, len));
 
         return o;
+    },
+    separatesThousands(n, separator = ' ') {
+        var parts = n.toString().split(".");
+        const numberPart = parts[0];
+        const decimalPart = parts[1];
+        const thousands = /\B(?=(\d{3})+(?!\d))/g;
+        return numberPart.replace(thousands, separator) + (decimalPart ? "." + decimalPart : "");
+    },
+    saveGridTableToggles(widgetId, col) {
+        let cellData = v(widgetId + '.cellData'),
+            i, result = [],
+            len = cellData.length;
+
+        for (i = 0; i < len; ++i) {
+            result[i] = v(widgetId + '_' + i + '_' + col).switch ? v(widgetId + '_' + i + '_' + col).switch.value : cellData[i][col].value;
+        }
+
+        Utils.setWidgetValue('systemValue' + widgetId + 'Toggles', result);
+    },
+    getGridTableToggleValue(widgetId, index) {
+        let res = v('systemValue' + widgetId + 'Toggles');
+
+        if (index < res.length) {
+            return res[index];
+        }
+
+        return 0;
+    },
+    hexToRgb(hex, opacity = 1, asObject) {
+        hex = hex.replace(/^#?([a-f\d])([a-f\d])([a-f\d])$/i, (m, r, g, b) => r + r + g + g + b + b);
+
+        let r = /^#?([a-f\d]{2})([a-f\d]{2})([a-f\d]{2})$/i.exec(hex);
+
+        r = {
+            r: parseInt(r[1], 16),
+            g: parseInt(r[2], 16),
+            b: parseInt(r[3], 16),
+            a: opacity
+        };
+
+        if (asObject) {
+            return r;
+        }
+
+        return 'rgb' + (opacity < 1 ? 'a' : '') + '(' + Object.values(r).slice(0, opacity < 1 ? 4 : -1).join(',') + ')';
+    },
+    getActiveUserString(value) {
+        return value.includes('CAMID') ? value : value.replace(/\\/g, '/');
+    },
+    checkScreenResolution() {
+        if (!app.checkScreenResolutionWarningDisplayed && $('body').width() - 100 > window.innerWidth) {
+            Api.showPopup('Your current screen resolution is below the recommended 1920*1080. For optimal user experience please lower your browser zoom to 90% or 80%.');
+            app.checkScreenResolutionWarningDisplayed = true;
+        }
     }
 };
 
 app.utils = Utils;
```

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/framework/write-executor/base.js` & `analogic-framework-4.1.0/analogic/static/assets/js/framework/write-executor/base.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/framework/write-executor/factory.js` & `analogic-framework-4.1.0/analogic/static/assets/js/framework/write-executor/factory.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -47,27 +47,31 @@
 
         return new WriteExecutor(context);
     }
 
     static createContext(eventName, widgetId, jqueryEvent, jqueryElement, resent = false) {
         let z = widgetId.split('_'),
             context = Widgets,
-            widget, gridTableCell, gridTableInfo;
+            widget, gridTableCell, gridTableInfo, widgetEventValue;
 
         if (z.length > 2 && z[1] !== 'row') { //grid table
             widget = context[z[0]];
 
             widget.row && delete widget.row;
             widget.column && delete widget.column;
 
             widget.row = z[1];
             widget.column = z[2];
 
             if (v(widgetId + '.' + eventName)) {
                 widget[eventName] = v(widgetId + '.' + eventName);
+                widgetEventValue = v(widgetId + '.' + eventName + '.value');
+                if (widgetEventValue) {
+                    widget.value = widgetEventValue
+                }
             }
 
             gridTableCell = v(z[0] + '.cellData')[z[1]][z[2]];
 
             gridTableCell.dirty = true;
 
             gridTableInfo = WriteExecutorFactory.getGridTableInfo(gridTableCell, parseInt(z[1]), parseInt(z[2]), z, eventName + '.' + widgetId);
@@ -119,14 +123,17 @@
         };
         context.getEventValues = () => {
             return context.getWidgetValue(context.getEventName());
         };
         context.getCell = () => {
             return gridTableInfo !== null ? gridTableInfo.getCell() : null;
         };
+        context.getCellId = () => {
+            return context.getCell() ? context.getCell().id : null;
+        };
         context.getRow = () => {
             return gridTableInfo !== null ? gridTableInfo.getRow() : null;
         };
         context.getColumn = () => {
             return gridTableInfo !== null ? gridTableInfo.getColumn() : null;
         };
         context.getGridTableInfo = () => {
```

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/framework/write-executor/grid-table.js` & `analogic-framework-4.1.0/analogic/static/assets/js/framework/write-executor/grid-table.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/lib/Chart-2.9.3.min.js` & `analogic-framework-4.1.0/analogic/static/assets/js/lib/Chart-2.9.3.min.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/lib/Sortable.min.js` & `analogic-framework-4.1.0/analogic/static/assets/js/lib/Sortable.min.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/lib/chartjs-plugin-datalabels.min.js` & `analogic-framework-4.1.0/analogic/static/assets/js/lib/chartjs-plugin-datalabels.min.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/lib/chartjs-plugin-dragdata.min.js` & `analogic-framework-4.1.0/analogic/static/assets/js/lib/chartjs-plugin-dragdata.min.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/lib/debounceAndThrottle.1.8.3.min.js` & `analogic-framework-4.1.0/analogic/static/assets/js/lib/debounceAndThrottle.1.8.3.min.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/lib/jquery/jquery-3.6.0.min.js` & `analogic-framework-4.1.0/analogic/static/assets/js/lib/jquery/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/lib/jquery/jquery.actual.min.js` & `analogic-framework-4.1.0/analogic/static/assets/js/lib/jquery/jquery.actual.min.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/lib/jquery/jquery.cookie.js` & `analogic-framework-4.1.0/analogic/static/assets/js/lib/jquery/jquery.cookie.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/lib/jquery/jquery.doubletap.js` & `analogic-framework-4.1.0/analogic/static/assets/js/lib/jquery/jquery.doubletap.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/lib/jquery/tableSort.js` & `analogic-framework-4.1.0/analogic/static/assets/js/lib/jquery/tableSort.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/lib/nouislider.min.js` & `analogic-framework-4.1.0/analogic/static/assets/js/lib/nouislider.min.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/base/widget.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/base/widget.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -11,14 +11,15 @@
         }
 
         if (!this.getHtml) {
             throw new TypeError('The "getHtml" method must be implemented for the "' + this.name + '" object!');
         }
 
         this.options = options;
+        this.isRendering = false;
     }
 
     reset() {
 
     }
 
     renderStartLoader(withLoader) {
@@ -83,14 +84,18 @@
                     return 'refreshGridCell';
                 });
             });
         });
     }
 
     reRenderWidget(withState = false, withLoader = true, previouslyLoadedData = false) {
+        if (this.isRendering) {
+            this.renderError();
+        }
+        this.isRendering = true;
 
         const o = this.options,
             holder = this.getHolder(o.id),
             instance = this;
 
         this.renderStartLoader(withLoader);
 
@@ -154,15 +159,24 @@
 
                     return 'rerendered';
                 });
             });
         });
     }
 
+    renderError() {
+        console.error('Duplicate render calls at the same time for the ' + this.options.id + ' widget!');
+        console.error('Please check the forceRefresh function call');
+    }
+
     renderWidget(withState = false, withLoader = true, previouslyLoadedData = false) {
+        if (this.isRendering) {
+            this.renderError();
+        }
+        this.isRendering = true;
 
         const o = this.options,
             holder = this.getHolder(o.id),
             instance = this;
 
         this.renderStartLoader(withLoader);
 
@@ -253,14 +267,15 @@
     }
 
     updateHtml(data) {
 
     }
 
     render(withState, refresh, useDefaultData = false, loadFunction = QB.loadData, previouslyLoadedData = false) {
+        this.isRendering = true;
         const o = this.options,
             instance = this;
         let ww;
 
         let widgetOptions, widgets = [];
 
         for (widgetOptions of o.widgets || []) {
@@ -330,26 +345,27 @@
         html = this.getHtml(widgetHtmls, data, withState);
 
         return `<section ${write === 'off' ? `data-write="off"` : ''} ${originalId !== false ? `data-originalId="${o.originalId}"` : ''} ${o.ordinal ? `data-ordinal="${o.ordinal}"` : ''} ${o.margin ? 'class="wrapper"' : ''} style="${gs.join('')}" id="${o.id ? o.id : Utils.getRandomId()}">${html}</section>`;
 
     }
 
     embeddedRender(withState, data, loadFunction = QB.loadData) {
+        this.isRendering = true;
         const o = {
                 ...this.options,
                 ...data
             },
             instance = this,
             h = Listeners.handle;
 
         this.addListeners(false);
 
         this.addDependents();
 
-        if (new o.type(o).amIOnAGridTable()) { //Todo check
+        if (new o.type(o).amIOnAGridTable()) {
             Listeners.push({
                 options: o,
                 method: 'refreshGridCell',
                 eventName: 'forcerefresh.' + o.id,
                 handler: h
             });
         }
@@ -480,14 +496,16 @@
         }
 
         for (w of widgets) {
             w.initEvents(withState);
         }
 
         this.initEventHandlers(withState);
+
+        this.isRendering = false;
     }
 
     initEventHandlers() {
 
     }
 
     processData(data) {
@@ -556,21 +574,21 @@
         Widget.executeEventMapActions(columnEventMapId, event, element, write);
     }
 
     static executeEventMapActions(eventMapId, event, element, write = true, ...args) {
         L(eventMapId, event, element, args);
 
         let actions = EventMap[eventMapId],
-            a;
+            a, writeResponse = true;
 
         if (write === true) {
-            QB.writeData(eventMapId, event, element);
+            writeResponse = QB.writeData(eventMapId, event, element);
         }
 
-        if (actions) {
+        if (actions && writeResponse !== false) {
             for (a of actions) {
                 a.action(a.argument, event, element);
             }
         }
     }
 
     get id() {
```

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/button.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/button.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/combo-chart.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/combo-chart.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -174,24 +174,26 @@
             leftYAxesTicksFontColor: this.getRealValue('leftYAxesTicksFontColor', data, b),
             leftYAxesTicksOffset: this.getRealValue('leftYAxesTicksOffset', data, 0),
             leftYAxesMin: this.getRealValue('leftYAxesMin', data, false),
             leftYAxesMax: this.getRealValue('leftYAxesMax', data, false),
             leftYAxesStepSize: this.getRealValue('leftYAxesStepSize', data, false),
             leftYAxesLabelConcat: this.getRealValue('leftYAxesLabelConcat', data, false),
             leftYAxesZeroLineColor: this.getRealValue('leftYAxesZeroLineColor', data, 'black'),
+            leftYAxesLabelSeparatesThousands: this.getRealValue('leftYAxesLabelSeparatesThousands', data, true),
 
             canvasHeight: this.getRealValue('canvasHeight', data, false),
             canvasWidth: this.getRealValue('canvasWidth', data, false),
             draggable: this.getRealValue('draggable', data, false),
             responsive: this.getRealValue('responsive', data, true),
             aspectRatio: this.getRealValue('aspectRatio', data, null),
             maintainAspectRatio: this.getRealValue('maintainAspectRatio', data, true),
             bezierCurve: this.getRealValue('bezierCurve', data, false),
             showLinearXAxes: this.getRealValue('showLinearXAxes', data, false),
-            customLabelsForYAxes: this.getRealValue('customLabelsForYAxes', data, false)
+            customLabelsForYAxes: this.getRealValue('customLabelsForYAxes', data, false),
+            tooltipsSeparatesThousands: this.getRealValue('tooltipsSeparatesThousands', data, false)
         };
 
         this.value = v;
         return v;
     }
 
     updateHtml(data) {
@@ -349,14 +351,18 @@
             leftYAxesTicks.stepSize = v.leftYAxesStepSize;
         }
 
         if (v.leftYAxesLabelConcat !== false) {
             leftYAxesTicks.callback = (value, index, values) => value + v.leftYAxesLabelConcat;
         }
 
+        if (v.leftYAxesLabelSeparatesThousands !== false) {
+            leftYAxesTicks.callback = (value, index, values) => Utils.separatesThousands(value);
+        }
+
         yAxes.push({
             id: 'leftYAxes',
             display: v.leftYAxesDisplay,
             stacked: v.leftYAxesStacked,
             gridLines: {
                 display: v.leftYAxesGridLinesDisplay,
                 drawOnChartArea: v.leftYAxesGridLinesDrawOnChartArea,
@@ -476,15 +482,23 @@
                             return 'object' === typeof p ? p.y : p[1];
                         }
                     }
                 },
                 tooltips: {
                     enabled: v.tooltipsEnabled,
                     mode: v.tooltipsMode,
-                    intersect: true
+                    intersect: true,
+                    callbacks: {
+                        label: function(tooltipItem, data) {
+                            if (v.tooltipsSeparatesThousands) {
+                                return Utils.separatesThousands(tooltipItem.value);
+                            }
+                            return tooltipItem.value;
+                        }
+                    }
                 },
                 title: {
                     display: true
                 },
                 legend: {
                     display: false
                 },
```

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/container.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/container.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -36,14 +36,18 @@
         this.c.triggerFinishedEvent(eventType);
     }
 
     initEventHandlers(s) {
         this.c.initEventHandlers(s);
     }
 
+    reset() {
+        this.c.reset();
+    }
+
     open() {
         this.c.open();
     }
 
     setAnchor(a) {
         this.c.setAnchor(a);
     }
```

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/datepicker.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/datepicker.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/default/ScrollTableWidget.json` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/default/ScrollTableWidget.json`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/dropbox.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/dropbox.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/gauge.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/gauge.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,66 +1,62 @@
-/* global app, Chart, Utils */
+/* global app, Chart, Doc, El, Utils */
 
 'use strict';
 
 class GaugeWidget extends Widget {
 
     getHtml(widgets, d) {
         const labelsHtml = [],
-            valuesHtml = [];
+            valuesHtml = [],
+            id = this.options.id;
 
         if (!d) {
             d = {
                 values: [9.0, 9.1, 10],
                 labels: ['Modelled', 'Plan', 'Target'],
                 minRange: 0,
                 maxRange: 14,
                 title: 2020
             };
         }
 
         const v = {
-            canvasId: this.options.id + 'Canvas',
+            canvasId: id + 'Canvas',
             values: this.getRealValue('values', d),
             valueLabels: this.getRealValue('valueLabels', d, []),
             labels: this.getRealValue('labels', d),
             minRange: this.getRealValue('minRange', d),
             maxRange: this.getRealValue('maxRange', d),
+            showAxisValues: this.getRealValue('showAxisValues', d, true),
             colors: this.getRealValue('colors', d),
             title: this.getRealValue('title', d, ''),
             fontFamily: this.getRealValue('fontFamily', d, 'imago'),
-            skin: this.getRealValue('skin', d, 'standard')
+            skin: this.getRealValue('skin', d, 'standard'),
+            separatesThousands: this.getRealValue('separatesThousands', d, false)
         };
 
         if (v.maxRange === 0) {
             v.maxRange = 200;
         }
 
         this.value = v;
 
         for (let i = 0; i < v.labels.length; ++i) {
             labelsHtml.push('<div class="ks-gauge-label">', v.labels[i], '<\/div>');
             valuesHtml.push('<div class="ks-gauge-label ks-gauge-value" style="color: ', v.colors[i], '">', v.valueLabels.length > i ? v.valueLabels[i] : v.values[i].toFixed(1), '<\/div>');
         }
 
-        GaugeWidget.chartDataByIds = GaugeWidget.chartDataByIds || {};
-        GaugeWidget.chartDataByIds[v.canvasId] = {
-            minRange: v.minRange,
-            maxRange: v.maxRange,
-            fontFamily: v.fontFamily
-        };
-
         return `
 <div class="ks-gauge ks-gauge-${v.skin}" style="${this.getGeneralStyles(d).join('')}">
     <div class="ks-gauge-inner">
         <div class="ks-gauge-title">
             <div class="ks-gauge-title-content">${v.title}</div>
             <div class="ks-gauge-title-border"></div>
         </div>
-        <div class="ks-gauge-canvas"><canvas id="${v.canvasId}" height="1" width="2"></canvas></div>
+        <div class="ks-gauge-canvas"><canvas id="${v.canvasId}" data-widget_id="${id}" height="1" width="2"></canvas></div>
         <div class="ks-gauge-labels">
             <div class="ks-gauge-labels-col">${labelsHtml.join('')}</div>
             <div class="ks-gauge-labels-col">${valuesHtml.join('')}</div>
         </div>
     </div>
 </div>`;
     }
@@ -71,15 +67,14 @@
             ctx = canvas[0].getContext('2d'),
             c = new Chart(ctx, this.getGaugeConfig());
 
         this.initShowInFullScreenEventHandler(v);
     }
 
     initShowInFullScreenEventHandler(v) {
-
         const section = this.getSection();
 
         $('#' + v.id + 'FullScreenBtn').on('click', () => {
             this.showInFullScreen(v.title, '').promise().done(() => {
                 const chartDiv = section.find('.widget-financial-data-chart'),
                     prevChartDiv = chartDiv.prev();
 
@@ -135,24 +130,25 @@
             p = 40;
         } else {
             p = 45;
         }
 
         return {
             type: 'gauge',
+            separatesThousands: d.separatesThousands,
             data: {
                 datasets: datasets,
                 labels: []
             },
             options: {
                 layout: {
                     padding: {
                         left: p,
                         right: p,
-                        top: 15,
+                        top: d.showAxisValues ? 15 : 0,
                         bottom: 5
                     }
                 }
             }
         };
     }
 };
@@ -199,29 +195,33 @@
 Chart.controllers.gauge = Chart.controllers.doughnut.extend({
     name: 'gauge',
     draw: function() {
         Chart.controllers.doughnut.prototype.draw.apply(this, arguments);
 
         const chart = this.chart,
             x = chart.ctx,
-            chartData = GaugeWidget.chartDataByIds[chart.canvas.id];
+            chartData = Widgets[chart.canvas.dataset.widget_id].value;
+
+        if (!chartData.showAxisValues) {
+            return;
+        }
+
         const min = chartData.minRange,
             max = chartData.maxRange,
             step = (max - min) / 5 === 0 ? 1 : (max - min) / 5,
-            labels = [];
+            labels = [],
+            separatesThousands = chart.config.separatesThousands;
         const maxLen = max.toString().length,
             widthOffset = 6 * (maxLen - 2);
         const width = chart.width - widthOffset,
             height = chart.height,
             fontSize = (height / 140);
 
-        let i, m;
-
-        for (i = min; i <= max + min; i += step) {
-            labels.push(Math.round(i));
+        for (let i = min; i <= max + min; i += step) {
+            labels.push(separatesThousands ? Utils.separatesThousands(Math.round(i)) : Math.round(i));
         }
 
         x.font = fontSize + 'em ' + chartData.fontFamily;
         x.fillStyle = '#737B86';
         x.textAlign = 'left';
         x.textBaseline = 'bottom';
```

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/grid/grid-cell.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/grid/grid-cell.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/grid/grid-row.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/grid/grid-row.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/grid/grid.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/grid/grid.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/grid-table/grid-table-cell.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/grid-table/grid-table-cell.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -42,14 +42,15 @@
             width: this.getRealValue('width', data, 30)
         };
     }
 
     initEvents(withState, childId) {
         Widgets[childId].initEvents(withState);
         this.initEventHandlers(withState);
+        this.isRendering = false;
     }
 
     updateContent(data = false, loadFunction = QB.loadData) {
         const o = this.options;
         let widgetOptions, childrenData;
 
         for (widgetOptions of o.widgets || []) {
@@ -75,18 +76,19 @@
 
         paddingRight = p.cellPaddingRight !== false ? p.cellPaddingRight : o.paddingRight ? o.paddingRight : false;
         Widget.setOrRemoveMeasure(mainDiv, 'padding-right', paddingRight);
 
         paddingLeft = p.cellPaddingLeft !== false ? p.cellPaddingLeft : o.paddingLeft ? o.paddingLeft : false;
         Widget.setOrRemoveMeasure(mainDiv, 'padding-left', paddingLeft);
 
-        Widget.setSkin(mainDiv, 'ks-grid-table-cell-', p.cellSkin);
+        Widget.setSkin(mainDiv, 'ks-grid-table-cell-', p.cellSkin ? p.cellSkin : p.skin);
     }
 
     render(withState, childrenData) {
+        this.isRendering = true;
         const o = {
                 ...this.options,
                 ...childrenData
             },
             instance = this;
 
         let widgetOptions, w, widgetHtmls = [],
```

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/grid-table/grid-table-header-cell.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/grid-table/grid-table-header-cell.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -26,14 +26,15 @@
             cellHeaderSkin: this.getRealValue('cellHeaderSkin', d, false),
             cellVisible: this.getRealValue('cellVisible', d, true),
             width: this.getRealValue('width', d, false)
         };
     }
 
     render(withState, d, loadFunction = QB.loadData) {
+        this.isRendering = true;
         const o = this.options,
             instance = this;
 
         let widgetOptions, widgets = [],
             h = Listeners.handle;
 
         for (widgetOptions of o.widgets || []) {
```

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/grid-table/grid-table-header-row.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/grid-table/grid-table-header-row.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -11,14 +11,15 @@
             height: this.getRealValue('height', d, false)
         };
 
         return `<div class="ks-grid-table-row ${v.alignment !== false ? `ks-row-pos-${v.alignment}` : ''} ${v.borderBottom ? 'border-bottom' : ''} ${v.borderTop ? 'border-top' : ''}">${widgets.join('')}</div>`;
     }
 
     render(withState, d, loadFunction = QB.loadData) {
+        this.isRendering = true;
         const o = this.options,
             instance = this;
 
         let widgetOptions, widgets = [];
 
         for (widgetOptions of o.widgets || []) {
             widgets.push(this.getWidget(widgetOptions));
```

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/grid-table/grid-table.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/grid-table/grid-table.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -107,15 +107,16 @@
     }
 
     buildTableRowHtml(innerHtml, height, borderBottom = true) {
         return `<div class="ks-grid-table-row ${borderBottom ? 'border-bottom' : ''}"  ${height ? `style="height:${height}px;"` : ''}>${innerHtml}</div>`;
     }
 
     renderPage() {
-        return this.getHtml(this.state['widgets'], this.state['headerRowWidgetHtml'], this.cellData);
+        this.getHolder(this.id).html(this.getHtml(this.state['widgets'], this.state['headerRowWidgetHtml'], this.cellData));
+        this.initEvents();
     }
 
     isContentUpdatable(refreshedData) {
         const o = this.options;
         return refreshedData.length === v(o.id + '.cellData.length');
     }
 
@@ -200,16 +201,19 @@
                     processedData[i][j].cellId = o.id + 'Cell' + i + '-' + j;
                     processedData[i][j].originalId = instance.cellData[i][j].originalId;
 
                     if (vv.allowFullContentUpdated && i >= previousLength) {
                         Widgets[dd.cellId] = new w.type(w);
                         rendered.push(Widgets[dd.cellId].render(false, processedData[i][j]));
                     } else {
-                        if (false === vv.allowChangedDataUpdate ||
+                        if (false === vv.allowChangedDataUpdate || processedData[i][j].manipulated ||
                             !GridTableWidget.deepEqual(instance.cellData[i][j], processedData[i][j])) {
+                            if (processedData[i][j].manipulated) {
+                                delete processedData[i][j].manipulated;
+                            }
                             Widgets[processedData[i][j].cellId].updateContent(processedData[i][j]);
                             instance.cellData[i][j] = processedData[i][j];
                         }
                     }
                     ++j;
                 }
             }
@@ -238,14 +242,15 @@
         if (data.content && !section.hasClass('forcedByEventMap')) {
             v.hideIfNoData && section.css('display', data.content.length > 0 ? 'unset' : 'none');
         }
         return 'update';
     }
 
     render(withState, refresh, useDefaultData = false, loadFunction = QB.loadData, previouslyLoadedData = false) {
+        this.isRendering = true;
         const o = this.options,
             instance = this;
 
         let widgetOptions, widgets = [],
             headerRowWidget = false;
 
         for (widgetOptions of o.widgets || []) {
@@ -256,16 +261,14 @@
             }
         }
 
         this.addListeners(false);
 
         let afterLoad = (data) => {
 
-            L('start load', o.id, new Date(), data);
-
             let deferred = [],
                 w, cw, processedData = instance.processData(data),
                 i, j = 0,
                 rows, colNum,
                 widgetHtmls = [];
 
             if (!Array.isArray(processedData)) {
@@ -283,21 +286,18 @@
             }
 
             instance.state = {
                 rows: rows
             };
             instance.cellData = [];
 
-            L('render header', o.id, new Date());
-
             if (headerRowWidget !== false) {
                 deferred.push(headerRowWidget.render(withState, processedData.length > 0 ? processedData[0] : []));
             }
 
-            L('render cells', o.id, new Date());
             for (i = 0; i < rows; ++i) {
                 instance.cellData[i] = [];
                 j = 0;
                 for (w of widgets) {
                     processedData[i][j].id = o.id + '_' + i + '_' + j;
                     processedData[i][j].cellId = o.id + 'Cell' + i + '-' + j;
 
@@ -306,20 +306,16 @@
                     widgetHtmls.push(cw.render(withState, processedData[i][j]));
 
                     instance.cellData[i].push(processedData[i][j]);
                     ++j;
                 }
             }
 
-            L('end render cells', o.id, new Date());
-
             return $.when.apply($, deferred).then(function(...results) {
 
-                L('apply deferred', o.id, new Date());
-
                 let r, first = true,
                     headerRowWidgetHtml = false;
 
                 for (r of results) {
                     if (first === true && headerRowWidget !== false) {
                         headerRowWidgetHtml = r;
                     }
@@ -332,16 +328,14 @@
                     gs = instance.getWidthAndHeight(data);
                 }
 
                 if (visible === false) {
                     gs.push('display:none;');
                 }
 
-                L('return html', o.id, new Date());
-
                 return `<section ${o.margin ? 'class="wrapper"' : ''} title="${o.title || ''}"  style="${gs.join('')}"  id="${o.id}">${ghtml}</section>`;
             });
         };
 
         if (previouslyLoadedData !== false) {
             return afterLoad(previouslyLoadedData);
         }
@@ -350,48 +344,132 @@
             return afterLoad(data);
         });
     }
 
     initEvents(withState) {
         const o = this.options;
 
-        L('start init events', o.id, new Date());
-
         if (o.errorMessage) {
             return;
         }
 
         let w, i, j, colNum = (o.widgets.filter(e => e.type.name !== 'GridTableHeaderRowWidget') || []).length;
 
         for (i = 0; i < this.state.rows; ++i) {
             for (j = 0; j < colNum; ++j) {
                 Widgets[o.id + 'Cell' + i + '-' + j].initEvents(withState, o.id + '_' + i + '_' + j);
             }
         }
 
-        L('widget initialized', o.id, new Date());
-
         let headerRowWidget = o.widgets.filter(e => e.type.name === 'GridTableHeaderRowWidget');
 
         for (w of headerRowWidget) {
             Widgets[w.id].initEvents(withState);
         }
 
         this.initEventHandlers(withState);
-        L('init events finished', o.id, new Date());
+        this.isRendering = false;
     }
 
     initEventHandlers() {
 
     }
 
     reset() {
         delete this.cellData;
     }
 
+    triggerFillRight(params) {
+        let requests = this.getFillPatchRequest(params);
+        Repository[this.id]['fillRight'] = {
+            url: (db) => `/api/v1/Cellsets('${db.cellsetId}')/Cells`,
+            type: 'PATCH',
+            body: (db) => {
+                return requests;
+            }
+        };
+        return Api.executeRequest('fillRight.' + this.id);
+    }
+
+    triggerFillLeft(params) {
+        if (!params.iterationNumber) {
+            params.iterationNumber = -1;
+        }
+
+        let requests = this.getFillPatchRequest(params);
+
+        Repository[this.id]['fillLeft'] = {
+            url: (db) => `/api/v1/Cellsets('${db.cellsetId}')/Cells`,
+            type: 'PATCH',
+            body: (db) => {
+                return requests;
+            }
+        };
+        return Api.executeRequest('fillLeft.' + this.id);
+    }
+
+    getFillPatchRequest(params) {
+        //value, propertyName
+        //valueTransformation
+        //until, iterationNumber, cellCondition
+        if (this.cellData && this.row && this.column) {
+
+            if (typeof params.value == 'undefined' && !params.propertyName) {
+                alert(this.id + ' getFillPatchRequest must have value or propertyName parameters!');
+                return;
+            }
+
+            if (params.iterationNumber && params.iterationNumber === 0) {
+                alert(this.id + ' getFillPatchRequest params.iterationNumber can not be 0!');
+                return;
+            }
+
+            if (params.until && params.until < 0) {
+                alert(this.id + ' getFillPatchRequest params.until must be greater than or equal to 0!');
+                return;
+            }
+
+            let val = params.value !== false && typeof params.value !== 'undefined' ? params.value : this.cellData[this.row][this.column][params.propertyName],
+                requests = [],
+                start = parseInt(this.column),
+                iterationNumber = params.iterationNumber ? params.iterationNumber : 1,
+                end = params.until ? params.until : iterationNumber > 0 ? this.cellData[this.row].length : 0,
+                cell, cellCondition = params.cellCondition ? params.cellCondition : () => true,
+                template = (ordinal, value) => `{"Ordinal": \"${ordinal}\","Value": \"${value}\"}`;
+
+            if (iterationNumber < 0) {
+                const t = start;
+                start = end;
+                end = t;
+                iterationNumber *= -1;
+            }
+
+            if (end > this.cellData.length) {
+                alert(this.id + ' getFillPatchRequest wrong range params (params.until, params.iterationNumber)');
+                return;
+            }
+
+            if (params.valueTransformation) {
+                val = params.valueTransformation(val);
+            }
+
+            while (start < end) {
+                cell = this.cellData[this.row][start];
+                if (cellCondition(cell)) {
+                    requests.push(template(cell.ordinal, val));
+                }
+                start += iterationNumber;
+            }
+
+            return `[
+                       ${requests.join(',')}
+                   ]`;
+        }
+    }
+
     addGridTableListeners() {
         const cellData = v(this.options.id + '.cellData'),
             h = Listeners.handle;
         if (cellData && cellData.length > 0) {
             let widgetOptions, cells = [],
                 rowNum = cellData.length,
                 i, j, cw;
```

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/histogram-combo-chart.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/histogram-combo-chart.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/horizontal-bar-chart.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/horizontal-bar-chart.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/horizontal-table.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/horizontal-table.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -219,14 +219,15 @@
             s.push(`</div>`);
         }
 
         return s.join('');
     }
 
     render(withState) {
+        this.isRendering = true;
         const o = this.options,
             instance = this;
 
         let widgetOptions, widgets = [];
 
         for (widgetOptions of o.widgets || []) {
             widgets.push(this.getWidget(widgetOptions));
```

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/horizontaltable/action-button-row.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/horizontaltable/action-button-row.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/horizontaltable/delete-button-row.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/horizontaltable/delete-button-row.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/horizontaltable/radio-button-row.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/horizontaltable/radio-button-row.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/image.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/image.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/line-area-chart.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/line-area-chart.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/loader.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/loader.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/page.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/page.js`

 * *Files 21% similar despite different names*

#### js-beautify {}

```diff
@@ -21,14 +21,15 @@
     }
 
     getHolder(id) {
         return El.body;
     }
 
     render(withState, refresh, useDefaultData = false, loadFunction = QB.loadData, previouslyLoadedData = false) {
+        this.isRendering = true;
         const o = this.options;
 
         if (withState) {
             this.addListeners();
 
             return $.Deferred().resolve(PageState[o.id]);
         }
```

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/pie-chart.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/pie-chart.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -59,15 +59,15 @@
     </div>
     <div class="ks-legend ks-legend-${v.legendSkin}"></div>
 </div>`;
     }
 
     initEventHandlers() {
         const canvas = $('#' + this.options.id + 'Canvas'),
-            ctx = canvas[0].getctx('2d'),
+            ctx = canvas[0].getContext('2d'),
             c = new Chart(ctx, PieChartWidget.getChartConfig(this.value));
 
         canvas.parent().next().html(c.generateLegend()).on('click', '.ks-legend-item', e => {
             let legend = $(e.target).closest('.ks-legend-item').toggleClass('off'),
                 id = legend.data('id');
 
             c.getDatasetMeta(0).data[id].hidden = !c.getDatasetMeta(0).data[id].hidden;
```

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/pivot-table.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/pivot-table.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -108,15 +108,18 @@
         this.suppressOptions = {
             nonEmptyRows: true,
             nonEmptyColumns: true
         };
 
         Pivot.call({
             data: {
-                cube_name: o.cubeName
+                cube_name: o.cubeName,
+                options: JSON.stringify({
+                    widgetId: this.id
+                })
             }
         }).then(d => {
             this.presets = this.parsePresetsData(d.data);
 
             this.doLoadPreset(this.presetId);
 
             d.data = {};
@@ -154,23 +157,23 @@
 
 
         this.initControls();
     }
 
     parsePresetsData(d) {
         let i, p = [],
-            len = d.length - 4;
+            len = d.length - 5;
 
-        for (i = 0; i < len; i += 5) {
+        for (i = 0; i < len; i += 6) {
             p.push({
-                data: JSON.parse(d[i + 4].FormattedValue),
+                data: JSON.parse(d[i + 5].FormattedValue),
                 id: d[i].FormattedValue,
-                name: d[i + 3].FormattedValue,
-                type: d[i + 1].FormattedValue,
-                isOwner: parseInt(d[i + 2].FormattedValue)
+                name: d[i + 4].FormattedValue,
+                type: d[i + 2].FormattedValue,
+                isOwner: parseInt(d[i + 3].FormattedValue)
             });
         }
 
         return p;
     }
 
     initControls() {
@@ -936,20 +939,22 @@
             btn.siblings().children().addClass('off');
 
             this.adjustElementAliases(cols.eq(3).children('.ks-pivot-tag-add-col-content').children().slice(1), g.selectedAliasAttributeName, g.children);
         }
     }
 
     adjustElementAliases(elements, aliasAttrName, data) {
-        let i, n, e, len = elements.length;
+        let i, n, e, len = elements.length,
+            d;
 
         for (i = 0; i < len; ++i) {
             e = elements.eq(i);
             n = e.data('name');
-            e.contents().eq(1)[0].textContent = n + ' (' + data[n][aliasAttrName] + ')';
+            d = data[i];
+            e.contents().eq(1)[0].textContent = n + ' (' + (d[aliasAttrName] || d[0]) + ')';
         }
     }
 
     filterSelectorTreeColumn(e) {
         let inp = $(e.currentTarget),
             items = inp.closest('.ks-pivot-add-tag-search-holder').next().children().slice(1),
             searchTerm = Utils.cleanStr(inp.val().trim()).toLowerCase(),
@@ -1338,35 +1343,40 @@
 
         this.presetId = k;
 
         f = {
             pValue: d,
             pID: p[k].id,
             pName: presetName,
-            pType: p[k].type
+            pType: p[k].type,
+            pWidgetID: this.id
         };
 
         Pivot.call({
             data: {
                 options: JSON.stringify({
                     process: 'zSYS Analogic Save Pivot Preset',
-                    processParams: f
+                    processParams: f,
+                    widgetId: this.id
                 })
             }
         }).then(r => this.saveOrDeletePresetFinished(r));
     }
 
     saveOrDeletePresetFinished(r) {
         if (!r[0]) {
             return app.popup.show('Error during saving/deleting the Preset!', 400);
         }
 
         Pivot.call({
             data: {
-                cube_name: this.cubeName
+                cube_name: this.cubeName,
+                options: JSON.stringify({
+                    widgetId: this.id
+                })
             }
         }).then(d => {
             this.presets = this.parsePresetsData(d.data);
 
             this.doLoadPreset(this.presetId);
 
             this.closePopup();
```

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/popup.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/popup.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -52,15 +52,15 @@
 
         this.value = v;
 
         return `
 ${v.backdrop ? `<div style="${backdropStyle.join('')}" class="ks-container-backdrop ks-container-${v.skin}"  ${b}></div>` : ''}
 <div class="ks-container ${alignmentClass} ks-container-${v.skin}" style="${s.join('')}">
     <div style="${backgroundStyle.join('')}" class="ks-container-background">
-        <div style="${contentStyle.join('')}"  class="ks-container-content">${v.closeBtn ? `<div style="${closeBtnStyle.join('')}" class="div-x" onclick="$(this).trigger('close');"><span class="icon-x"></span></div>` : ''}${widgets.join('')}</div>
+        <div style="${contentStyle.join('')}"  class="ks-container-content">${v.closeBtn ? `<div style="${closeBtnStyle.join('')}" class="div-x"><span class="icon-x"></span></div>` : ''}${widgets.join('')}</div>
     </div>
 </div>`;
     }
 
     updateHtml(data) {
 
     }
@@ -103,15 +103,16 @@
         this.container = this.section.children().last();
         this.backdrop = this.container.prev();
 
         if (this.backdrop && v.closeOnClickBackdrop) {
             this.backdrop.on('click', () => this.close());
         }
 
-        this.section.on('open', () => this.open()).on('close', () => this.close());
+        this.section.on('open', () => this.open());
+        this.section.find('.div-x').on('click', () => this.close());
 
         if (a) {
             if ('string' === typeof a) {
                 const anchorSection = $('#' + a);
 
                 if (anchorSection.length) {
                     const anchorChildren = anchorSection.children();
```

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/radar-chart.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/radar-chart.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/scroll-table.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/scroll-table.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -7,15 +7,15 @@
         super(options);
 
         this.isMobile = Utils.isMobile() || app.isTouched;
         this.removableClasses = 'ks-cell-selected ks-editing ks-cell-active b s cell-range-top-left-corner cell-range-top-right-corner cell-range-top cell-range-bottom-left-corner cell-range-bottom-right-corner cell-range-bottom cell-range-left cell-range-right';
     }
 
     getHtml(widgets, data, withState) {
-        this.value = this.value.comment ? this.value : {};
+        this.value = this.value ? this.value : {};
         this.options.headerWidth = this.options.headerWidth || 160;
 
         let e, childId, parent, i, j, parentsByChildren = {},
             parentIdsByRowIds = {},
             hiddenRowIds = [],
             label, labelId, isExpanded;
```

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/segmented-bar.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/segmented-bar.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/segmented-control-item.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/segmented-control-item.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/segmented-control.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/segmented-control.js`

 * *Files 21% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,11 @@
 /* global app, Listeners, QB, Widget */
 
 'use strict';
+
 class SegmentedControlWidget extends Widget {
 
     getHtml(widgets, d) {
         const v = {
             skin: this.getRealValue('skin', d, 'standard')
         };
         const o = this.options;
@@ -38,30 +39,81 @@
             this.selected = selected.selected;
             this.value = selected.value;
         }
 
         return `<div class="ks-segmented ks-segmented-${v.skin}"  style="${this.getGeneralStyles(d).join('')}"><div class="ks-segmented-inner">${widgets.join('')}</div></div>`;
     }
 
+    embeddedRender(withState, data, loadFunction = QB.loadData) {
+        this.isRendering = true;
+        const o = {
+                ...this.options,
+                ...data
+            },
+            instance = this,
+            h = Listeners.handle;
+
+        let widgetOptions, widgets = [],
+            i = 0,
+            childrenData, w, widgetHtmls = [];
+
+        for (widgetOptions of o.widgets || []) {
+            widgets.push(this.getWidget(widgetOptions));
+        }
+
+        for (w of widgets) {
+            childrenData = {
+                id: o.id,
+                position: i,
+                originalId: w.id
+            };
+            widgetHtmls.push(w.embeddedRender(withState, {
+                ...childrenData,
+                ...data[i]
+            }));
+
+            ++i;
+        }
+
+        this.addListeners(false);
+
+        this.addDependents();
+
+        if (new o.type(o).amIOnAGridTable()) { //Todo check
+            Listeners.push({
+                options: o,
+                method: 'refreshGridCell',
+                eventName: 'forcerefresh.' + o.id,
+                handler: h
+            });
+        }
+
+        let visible = data && typeof data.visible !== 'undefined' ? data.visible : o.visible;
+
+        return instance.getMainHtmlElement(o, data, visible, widgetHtmls, withState)
+    }
+
     render(withState) {
+        this.isRendering = true;
         const o = this.options,
             instance = this;
 
         let widgetOptions, widgets = [];
 
         for (widgetOptions of o.widgets || []) {
             widgets.push(this.getWidget(widgetOptions));
         }
 
         this.addListeners(false);
 
         return QB.loadData(o.id, instance.name).then(function(data) {
             let deferred = [],
                 w, i = 0,
-                childrenData, widgetData = Array.isArray(data) ? data : (data && data.data) ? data.data : [];
+                childrenData,
+                widgetData = Array.isArray(data) ? data : (data && data.data) ? data.data : [];
 
             for (w of widgets) {
                 childrenData = {
                     id: o.id,
                     position: i,
                     originalId: w.id
                 };
@@ -78,15 +130,15 @@
                     r;
 
                 for (r of results) {
                     widgetHtmls.push(r);
                 }
 
                 let visible = data && typeof data.visible !== 'undefined' ? data.visible : o.visible;
-                return `<section title="${o.title || ''}" ${visible === false ? 'style="display:none"' : 'style="display:contents;"' } id="${o.id}">${instance.getHtml(widgetHtmls, instance.processData(data), withState)}</section>`;
+                return `<section title="${o.title || ''}" ${visible === false ? 'style="display:none"' : 'style="display:contents;"'} id="${o.id}">${instance.getHtml(widgetHtmls, instance.processData(data), withState)}</section>`;
             });
         });
     }
 
     initEventHandlers() {
 
         const section = this.getSection();
@@ -97,20 +149,25 @@
             this.selected = s.find('.ks-segment-label').html();
             this.value = s.data('value');
 
             let second = $('<div>').data('id', s.data('id')).data('action', 'switch');
 
             Widget.doHandleSystemEvent(s, e, false);
             Widget.doHandleSystemEvent(second, e, false);
+            if (this.amIOnAGridTable()) {
+                Widget.doHandleGridTableSystemEvent(s, e);
+                Widget.doHandleGridTableSystemEvent(second, e);
+            }
         });
 
         section.find('a').on('click', e => {
             let s = $(e.target).closest('section').parent().closest('section').find('.ks-segment'),
                 b = false,
-                i, w = $(e.target).closest('a');
+                i,
+                w = $(e.target).closest('a');
 
             $(e.target).closest('section').parent().closest('section').find('.ks-segment').removeClass('ks-on').removeClass('ks-right').removeClass('ks-left');
 
             w.addClass('ks-on');
 
             for (i = 0; i < s.length; ++i) {
                 e = $(s[i]);
```

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/simulation-panel-slider.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/simulation-panel-slider.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/simulation-panel.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/simulation-panel.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/slider.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/slider.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/swipe.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/swipe.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -60,24 +60,26 @@
 
         this.value = v;
 
         return `
 ${v.backdrop ? '<div class="ks-container-backdrop" style="display: none;"><\/div>' : ''}
 <div class="ks-container ${alignmentClass} ks-container-${v.skin}" style="${s.join('')}">
     <div class="ks-container-background">
-        <div class="ks-container-content">${v.closeBtn ? '<div class="div-x" onclick="$(this).trigger(\'close\');"><span class="icon-x"><\/span><\/div>' : ''}${widgets.join('')}</div>
+        <div class="ks-container-content">${v.closeBtn ? '<div class="div-x"><span class="icon-x"><\/span><\/div>' : ''}${widgets.join('')}</div>
     </div>
 </div>`;
     }
 
     initEventHandlers() {
         const section = this.getSection(),
             v = this.value;
 
-        this.section = section.on('close', () => this.close());
+        this.section = section;
+        this.section.find('.div-x').on('click', () => this.close());
+
         this.container = section.children().last();
         this.backdrop = this.container.prev();
 
         if (!v.pinned) {
             this.container.on(app.clickEvent + ' mouseenter swipeIn', () => this.swipeIn()).on('mouseleave swipeOut', () => this.swipeOut());
         }
```

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/system-popup.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/system-popup.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/text.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/text.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -7,15 +7,15 @@
     getHtml(widgets, d) {
         const o = this.options;
         const v = this.getParameters(d);
 
         this.setValues(v);
 
         let mainDivClass = [],
-            mainDivStyle = this.getGeneralStyles(d),
+            mainDivStyle = this.getGeneralStyles(d).concat(this.getHtmlComponentStylesArray('main', d)),
             titleStyles = this.getHtmlComponentStylesArray('title', d),
             bodyStyles = this.getHtmlComponentStylesArray('body', d),
             innerStyles = this.getHtmlComponentStylesArray('inner', d),
             iconStyles = this.getHtmlComponentStylesArray('icon', d);
 
         (v.title !== false || v.editable) && mainDivClass.push('has-title');
         v.body && mainDivClass.push('has-body');
@@ -46,15 +46,15 @@
         v.innerCursor && innerStyles.push(`cursor:${v.innerCursor};`);
 
         return `
 <div class="ks-text ${mainDivClass.join(' ')} ks-text-${v.skin}" style="${mainDivStyle.join('')}">
     <div class="ks-text-inner" style="${innerStyles.join('')}" data-id="${o.id}" data-action="text_click" data-ordinal="${v.ordinal}">
         <div class="ks-text-icon" data-id="${o.id}" data-action="${v.iconCustomEventName ? v.iconCustomEventName : 'perform'}" data-ordinal="${v.ordinal}"><span style="${iconStyles.join('')}" class="${v.icon}"></span></div>
         <div class="ks-text-title" data-performable="${v.performable ? '1' : '0'}" data-editable="${v.editable ? '1' : '0'}" title="${v.title ? Utils.htmlEncode(Utils.stripHtml(v.title))  : ''}" data-ordinal="${v.ordinal}" style="${titleStyles.join('')}">${v.title !== false ? v.title : ''}</div>
-        <div class="ks-text-body" style="${bodyStyles.join('')}">${v.body}</div>
+        <div class="ks-text-body" style="${bodyStyles.join('')}">${v.body !== false ? v.body : ''}</div>
     </div>
 </div>`;
     }
 
     setValues(v) {
         this.value = v.title;
         this.editable = v.editable;
@@ -86,14 +86,20 @@
 
         this.changeEvents(title, section, v.editable, v.performable);
         title.data('editable', v.editable ? '1' : '0');
         title.data('performable', v.performable ? '1' : '0');
 
         this.setValues(v);
 
+        this.updateHtmlComponent('main', data, mainDiv);
+        this.updateHtmlComponent('inner', data, inner);
+        this.updateHtmlComponent('title', data, title);
+        this.updateHtmlComponent('body', data, body);
+        this.updateHtmlComponent('icon', data, icon);
+
         //section
         if (v.applyMeasuresToSection) {
             Widget.setOrRemoveStyle(section, 'width', v.width ? Widget.getPercentOrPixel(v.width) : false);
             Widget.setOrRemoveStyle(section, 'height', v.height ? Widget.getPercentOrPixel(v.height) : false);
         }
 
         //main
```

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/textarea.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/textarea.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -103,15 +103,15 @@
         const p = this.getParameters(d),
             section = this.getSection(),
             textarea = section.find('textarea');
 
         this.editable = p.editable;
         this.value = Utils.escapeText(d.value);
 
-        textarea.html(d.value);
+        textarea.val(d.value);
     }
 
     reset() {
         delete this.value;
         delete this.editable;
     }
```

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/textbox.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/textbox.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -17,14 +17,16 @@
 
         this.value = d.value;
 
         let hide = o.hideIfNoData === true && d.value === '';
 
         const v = this.getParameters(d);
 
+        this.addDynamicData(d, v);
+
         let mainDivClass = [],
             mainDivStyle = this.getGeneralStyles(d),
             titleStyles = this.getHtmlComponentStylesArray('title', d),
             iconStyles = this.getHtmlComponentStylesArray('icon', d),
             textStyles = this.getHtmlComponentStylesArray('text', d);
 
         v.title && mainDivClass.push('has-title');
@@ -46,15 +48,15 @@
     <div class="ks-textbox-inner">
         <div class="ks-textbox-title" style="${titleStyles.join('')}">
             <span class="ks-textbox-title-primary">${v.title ? v.title : ''}</span>
             <span class="ks-textbox-title-secondary"></span>
         </div>
         <div class="ks-textbox-field">
             <div class="ks-textbox-field-inner ${v.editable === false ? 'readonly' : ''}">
-                <div class="ks-textbox-icon">${v.icon !== false ? `style="${iconStyles.join('')}"<img src="${app.applicationAssetsUrl}/skin/images/${v.icon}">` : ''}</div>
+                <div class="ks-textbox-icon" style="${iconStyles.join('')}">${v.icon !== false ? `<img src="${app.applicationAssetsUrl}/skin/images/${v.icon}">` : ''}</div>
                 <div class="ks-textbox-divider"></div>
                 <input ${v.editable === false ? 'readonly' : ''} style="${textStyles.join('')}" data-action="writeEnd" data-id="${o.id}"  type="${v.textBoxType}" value="${Utils.htmlEncode(d.value)}" class="ks-textbox-input" placeholder="${v.defaultText ? v.defaultText : ''}">
             </div>
         </div>
     </div>
 </div>`;
     }
@@ -71,20 +73,32 @@
 
         if (!data.value && data.value !== 0) {
             data.value = '';
         }
 
         this.value = data.value;
 
+        this.addDynamicData(data, p);
+
         input.attr('placeholder', p.defaultText === false ? '' : p.defaultText);
         input.attr('value', Utils.htmlEncode(data.value));
         input.val(data.value);
 
     }
 
+    addDynamicData(data, parameters) {
+        const exclude = Object.keys(parameters);
+        exclude.push('value', 'id', 'type', 'options');
+        for (const [key, value] of Object.entries(data)) {
+            if (exclude.indexOf(key) === -1) {
+                this[key] = value;
+            }
+        }
+    }
+
     getParameters(d) {
         return {
             icon: this.getRealValue('icon', d, false),
             highlight: this.getRealValue('highlight', d, false),
             defaultText: this.getRealValue('defaultText', d, false),
             editable: this.getRealValue('editable', d, true),
             skin: this.getRealValue('skin', d, 'standard'),
```

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/toggle.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/toggle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -101,15 +101,14 @@
         if (section.find('.ks-toggle-inner').hasClass('readonly')) {
             return;
         }
 
         const o = this.options;
 
         let isGridTableHierarchyExpander = this.isGridTableHierarchyExpander;
-
         section.find('.ks-toggle').on('click', e => {
             const s = $(e.currentTarget),
                 isActive = !s.hasClass('ks-on');
 
             if (o.groupId) {
                 if (isActive) {
                     $('.ks-toggle-' + o.groupId).removeClass('ks-on');
```

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/tornado-chart.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/tornado-chart.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/vertical-line-box.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/vertical-line-box.js`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/js/widgets/water-fall.js` & `analogic-framework-4.1.0/analogic/static/assets/js/widgets/water-fall.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -55,14 +55,15 @@
             }]),
             labelVisible: this.getRealValue('labelVisible', d, true),
             legendVisible: this.getRealValue('legendVisible', d, true),
             minYAxis: parseFloat(this.getRealValue('minYAxis', d, -10)),
             maxYAxis: parseFloat(this.getRealValue('maxYAxis', d, 60)),
             yAxisGridLineNum: parseInt(this.getRealValue('yAxisGridLineNum', d, 11)),
             yAxisDecimalNum: parseInt(this.getRealValue('yAxisDecimalNum', d, 2)),
+            yAxisSeparatesThousands: this.getRealValue('yAxisSeparatesThousands', d, false),
             height: parseFloat(Utils.getSize(this.getRealValue('height', d, 300), false, 'height')),
             defaultColor: this.getRealValue('defaultColor', d, '#F3F4F6'),
             skin: this.getRealValue('skin', d, 'attila-1'),
             hiddenDatasets: [false, false],
             allowLastColumnToZero: this.getRealValue('allowLastColumnToZero', d, true)
         };
 
@@ -120,20 +121,20 @@
         const resetBtnVisibility = (minYAxis && (minYAxis !== v.minYAxis)) ? '' : ' style="display: none;"',
             yAxisDecimalNum = v.yAxisDecimalNum;
         let i, j = max,
             d, label, isLastCol, hb, lastHeights = [zeroHeight, zeroHeight],
             val;
 
         for (i = 0; i < v.yAxisGridLineNum; ++i) {
-            yAxisHtml.push('<div class="ks-waterfall-y-line ks-primary"><div class="ks-waterfall-y-line-tick ks-left"><\/div><div class="ks-waterfall-y-line-label ks-left">', Utils.precisionRound(j, yAxisDecimalNum), '<\/div><div class="ks-waterfall-y-line-tick ks-right"><\/div><div class="ks-waterfall-y-line-label ks-right"><\/div><\/div>');
+            yAxisHtml.push('<div class="ks-waterfall-y-line ks-primary"><div class="ks-waterfall-y-line-tick ks-left"><\/div><div class="ks-waterfall-y-line-label ks-left">', v.yAxisSeparatesThousands ? Utils.separatesThousands(Utils.precisionRound(j, yAxisDecimalNum)) : Utils.precisionRound(j, yAxisDecimalNum), '<\/div><div class="ks-waterfall-y-line-tick ks-right"><\/div><div class="ks-waterfall-y-line-label ks-right"><\/div><\/div>');
 
             j -= yAxisStep;
         }
 
-        yAxisHtml.push('<div class="ks-waterfall-y-line ks-axis"><div class="ks-waterfall-y-line-tick ks-left"></div><div class="ks-waterfall-y-line-label ks-left ks-waterfall-label-origo">' + min + '</div><div class="ks-waterfall-y-line-tick ks-right"></div><div class="ks-waterfall-y-line-label ks-right"></div><div class="ks-waterfall-reset"' + resetBtnVisibility + '><span class="">i</span> Reset</div></div>');
+        yAxisHtml.push('<div class="ks-waterfall-y-line ks-axis"><div class="ks-waterfall-y-line-tick ks-left"></div><div class="ks-waterfall-y-line-label ks-left ks-waterfall-label-origo">' + (v.yAxisSeparatesThousands ? Utils.separatesThousands(min) : min) + '</div><div class="ks-waterfall-y-line-tick ks-right"></div><div class="ks-waterfall-y-line-label ks-right"></div><div class="ks-waterfall-reset"' + resetBtnVisibility + '><span class="">i</span> Reset</div></div>');
 
         for (i = 0; i < len; ++i) {
             d = datapoints1[i];
             label = labels[i];
 
             isLastCol = (len - 1 === i);
```

### Comparing `analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-button.css` & `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-button.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-container.css` & `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-container.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-datepicker.css` & `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-datepicker.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-dropbox.css` & `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-dropbox.css`

 * *Files 3% similar despite different names*

```diff
@@ -58,15 +58,16 @@
     -o-transform: translate(-50%, -50%);
     -ms-transform: translate(-50%, -50%);
     transform: translate(-50%, -50%);
 }
 
 .ks-dropbox-panel {
     left: 0;
-    overflow: hidden;
+    overflow: scroll;
+    max-height: 300px;
     position: absolute;
     right: 0;
     top: 100%;
     z-index: 99;
 }
 
 .ks-dropbox-panel-inner {
```

### Comparing `analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-grid-table.css` & `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-grid-table.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-grid.css` & `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-grid.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-horizontal-table.css` & `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-horizontal-table.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-horizontalbarchart.css` & `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-horizontalbarchart.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-line-scatter-combo.css` & `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-line-scatter-combo.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-popup.css` & `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-popup.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-scrolltable.css` & `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-scrolltable.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-segmentedbar.css` & `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-segmentedbar.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-slider-touch.css` & `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-slider-touch.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-slider.css` & `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-slider.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-text.css` & `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-text.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-textarea.css` & `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-textarea.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-textbox.css` & `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-textbox.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-toggle.css` & `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-toggle.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-tornado.css` & `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-tornado.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-vertical-line-box.css` & `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-vertical-line-box.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/static/assets/skin/css/ks-waterfall.css` & `analogic-framework-4.1.0/analogic/static/assets/skin/css/ks-waterfall.css`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/templates/authenticated.html` & `analogic-framework-4.1.0/analogic/templates/authenticated.html`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/templates/config.html` & `analogic-framework-4.1.0/analogic/templates/config.html`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/templates/css.html` & `analogic-framework-4.1.0/analogic/templates/css.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 <link href="{{url_for('static', filename='assets/css/bootstrap-grid.min.css')}}?v={{cnf.version}}" rel="stylesheet" type="text/css">
 <link href="{{url_for('static', filename='assets/css/widgets/loader.css')}}?v={{cnf.version}}" rel="stylesheet" type="text/css">
 <link href="{{url_for('static', filename='assets/css/widgets/simulation-panel-slider.css')}}?v={{cnf.version}}" rel="stylesheet" type="text/css">
 <link href="{{url_for('static', filename='assets/css/lib/Chart-2.9.3.min.css')}}?v={{cnf.version}}" rel="stylesheet" type="text/css">
 <link href="{{url_for('static', filename='assets/css/lib/nouislider.min.css')}}?v={{cnf.version}}" rel="stylesheet" type="text/css">
 
 <!-- widget skins -->
+<link href="{{url_for('static', filename='assets/skin/css/ks-general.css')}}?v={{cnf.version}}" rel="stylesheet" type="text/css">
 <link href="{{url_for(cnf.blueprint_static, filename='assets/skin/css/ks-general.css')}}?v={{cnf.version}}" rel="stylesheet" type="text/css">
 
 <link href="{{url_for('static', filename='assets/skin/css/ks-container.css')}}?v={{cnf.version}}" rel="stylesheet" type="text/css">
 <link href="{{url_for(cnf.blueprint_static, filename='assets/skin/css/ks-container-style.css')}}?v={{cnf.version}}" rel="stylesheet" type="text/css">
 
 <link href="{{url_for('static', filename='assets/skin/css/ks-button.css')}}?v={{cnf.version}}" rel="stylesheet" type="text/css">
 <link href="{{url_for(cnf.blueprint_static, filename='assets/skin/css/ks-button-style.css')}}?v={{cnf.version}}" rel="stylesheet" type="text/css">
```

### Comparing `analogic-framework-4.0.2/analogic/templates/javascripts.html` & `analogic-framework-4.1.0/analogic/templates/javascripts.html`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/templates/login.html` & `analogic-framework-4.1.0/analogic/templates/login.html`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/templates/redirect.html` & `analogic-framework-4.1.0/analogic/templates/redirect.html`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic/templates/sso_error.html` & `analogic-framework-4.1.0/analogic/templates/sso_error.html`

 * *Files identical despite different names*

### Comparing `analogic-framework-4.0.2/analogic_framework.egg-info/SOURCES.txt` & `analogic-framework-4.1.0/analogic_framework.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 analogic/__init__.py
 analogic/analogic.py
+analogic/analogic_tm1_service.py
 analogic/authentication_provider.py
 analogic/cam.py
+analogic/camsecure.py
 analogic/condition.py
 analogic/core_endpoints.py
 analogic/email.py
 analogic/endpoint.py
+analogic/exceptions.py
 analogic/loader.py
 analogic/logging.json
 analogic/loginbasic.py
+analogic/logincam.py
 analogic/nologin.py
 analogic/pivot.py
 analogic/setting.py
+analogic/task.py
 analogic/version.config
 analogic/version.py
 analogic/static/assets/css/bootstrap-grid.min.css
 analogic/static/assets/css/bootstrap-grid.min.css.map
 analogic/static/assets/css/style.css
 analogic/static/assets/css/lib/Chart-2.9.3.min.css
 analogic/static/assets/css/lib/nouislider.min.css
@@ -155,14 +160,15 @@
 analogic/static/assets/js/widgets/horizontaltable/radio-button-row.js
 analogic/static/assets/skin/css/ks-button.css
 analogic/static/assets/skin/css/ks-combo-chart.css
 analogic/static/assets/skin/css/ks-container.css
 analogic/static/assets/skin/css/ks-datepicker.css
 analogic/static/assets/skin/css/ks-dropbox.css
 analogic/static/assets/skin/css/ks-gauge.css
+analogic/static/assets/skin/css/ks-general.css
 analogic/static/assets/skin/css/ks-grid-cell.css
 analogic/static/assets/skin/css/ks-grid-row.css
 analogic/static/assets/skin/css/ks-grid-table-cell.css
 analogic/static/assets/skin/css/ks-grid-table.css
 analogic/static/assets/skin/css/ks-grid.css
 analogic/static/assets/skin/css/ks-horizontal-table.css
 analogic/static/assets/skin/css/ks-horizontalbarchart.css
@@ -184,14 +190,28 @@
 analogic/static/assets/skin/css/ks-text.css
 analogic/static/assets/skin/css/ks-textarea.css
 analogic/static/assets/skin/css/ks-textbox.css
 analogic/static/assets/skin/css/ks-toggle.css
 analogic/static/assets/skin/css/ks-tornado.css
 analogic/static/assets/skin/css/ks-vertical-line-box.css
 analogic/static/assets/skin/css/ks-waterfall.css
+analogic/static/assets/skin/fonts/GothamNarrow-Bold.eot
+analogic/static/assets/skin/fonts/GothamNarrow-Bold.svg
+analogic/static/assets/skin/fonts/GothamNarrow-Bold.ttf
+analogic/static/assets/skin/fonts/GothamNarrow-Bold.woff
+analogic/static/assets/skin/fonts/GothamNarrow-Bold.woff2
+analogic/static/assets/skin/fonts/GothamNarrow-Medium.eot
+analogic/static/assets/skin/fonts/GothamNarrow-Medium.svg
+analogic/static/assets/skin/fonts/GothamNarrow-Medium.ttf
+analogic/static/assets/skin/fonts/GothamNarrow-Medium.woff
+analogic/static/assets/skin/fonts/GothamNarrow-Medium.woff2
+analogic/static/assets/skin/fonts/pivot.eot
+analogic/static/assets/skin/fonts/pivot.svg
+analogic/static/assets/skin/fonts/pivot.ttf
+analogic/static/assets/skin/fonts/pivot.woff
 analogic/templates/404.html
 analogic/templates/500.html
 analogic/templates/authenticated.html
 analogic/templates/config.html
 analogic/templates/css.html
 analogic/templates/index.html
 analogic/templates/javascripts.html
```

### Comparing `analogic-framework-4.0.2/setup.py` & `analogic-framework-4.1.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -26,10 +26,12 @@
         'XlsxWriter==1.3.7',
         'matplotlib==3.5.2',
         'PyYaml==6.0',
         'xlrd==2.0.1',
         'openpyxl==3.0.10',
         'Flask-Cors==3.0.10',
         'json_logging==1.3.0',
-        'flask_talisman'
+        'flask_talisman',
+        'Flask-APScheduler==1.12.4',
+        'orjson==3.8.6'
     ],
 )
```

