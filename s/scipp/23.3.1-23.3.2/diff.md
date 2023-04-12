# Comparing `tmp/scipp-23.3.1.tar.gz` & `tmp/scipp-23.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipp-23.3.1.tar", last modified: Mon Apr  3 07:46:21 2023, max compression
+gzip compressed data, was "scipp-23.3.2.tar", last modified: Wed Apr 12 09:46:59 2023, max compression
```

## Comparing `scipp-23.3.1.tar` & `scipp-23.3.2.tar`

### file list

```diff
@@ -1,160 +1,160 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 07:46:21.595952 scipp-23.3.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-04-03 07:45:50.000000 scipp-23.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     2535 2023-04-03 07:46:21.595952 scipp-23.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      226 2023-04-03 07:45:51.000000 scipp-23.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 07:46:21.571950 scipp-23.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 07:46:21.575950 scipp-23.3.1/src/scipp/
--rw-r--r--   0 runner    (1001) docker     (122)     6117 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3496 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/_binding.py
--rw-r--r--   0 runner    (1001) docker     (122)      217 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/_scipp.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 07:46:21.575950 scipp-23.3.1/src/scipp/binning/
--rw-r--r--   0 runner    (1001) docker     (122)      475 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/binning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 07:46:21.575950 scipp-23.3.1/src/scipp/compat/
--rw-r--r--   0 runner    (1001) docker     (122)      286 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5935 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/compat/dict.py
--rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/compat/pandas_compat.py
--rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/compat/wrapping.py
--rw-r--r--   0 runner    (1001) docker     (122)     5866 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/compat/xarray_compat.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 07:46:21.575950 scipp-23.3.1/src/scipp/configuration/
--rw-r--r--   0 runner    (1001) docker     (122)     4210 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3752 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/configuration/config_default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 07:46:21.575950 scipp-23.3.1/src/scipp/constants/
--rw-r--r--   0 runner    (1001) docker     (122)     4941 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/constants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 07:46:21.579951 scipp-23.3.1/src/scipp/coords/
--rw-r--r--   0 runner    (1001) docker     (122)      255 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/coords/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1086 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/coords/coord.py
--rw-r--r--   0 runner    (1001) docker     (122)     2601 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/coords/coord_table.py
--rw-r--r--   0 runner    (1001) docker     (122)     5211 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/coords/graph.py
--rw-r--r--   0 runner    (1001) docker     (122)      378 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/coords/options.py
--rw-r--r--   0 runner    (1001) docker     (122)     7528 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/coords/rule.py
--rw-r--r--   0 runner    (1001) docker     (122)    12893 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/coords/transform_coords.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 07:46:21.583951 scipp-23.3.1/src/scipp/core/
--rw-r--r--   0 runner    (1001) docker     (122)     3653 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      623 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/core/_cpp_wrapper_util.py
--rw-r--r--   0 runner    (1001) docker     (122)      727 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/core/_sizes.py
--rw-r--r--   0 runner    (1001) docker     (122)     5742 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/core/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (122)     6803 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/core/bin_remapping.py
--rw-r--r--   0 runner    (1001) docker     (122)    26466 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/core/binning.py
--rw-r--r--   0 runner    (1001) docker     (122)    17954 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/core/bins.py
--rw-r--r--   0 runner    (1001) docker     (122)     8807 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/core/comparison.py
--rw-r--r--   0 runner    (1001) docker     (122)     3103 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/core/concepts.py
--rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/core/counts.py
--rw-r--r--   0 runner    (1001) docker     (122)      479 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/core/cpp_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)    41780 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/core/cpp_classes.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     1362 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/core/cumulative.py
--rw-r--r--   0 runner    (1001) docker     (122)    19386 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/core/data_group.py
--rw-r--r--   0 runner    (1001) docker     (122)      858 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     5712 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/core/dimensions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/core/domains.py
--rw-r--r--   0 runner    (1001) docker     (122)      892 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/core/groupby.py
--rw-r--r--   0 runner    (1001) docker     (122)     5258 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/core/like.py
--rw-r--r--   0 runner    (1001) docker     (122)     1740 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/core/logical.py
--rw-r--r--   0 runner    (1001) docker     (122)     9715 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/core/math.py
--rw-r--r--   0 runner    (1001) docker     (122)     9671 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/core/operations.py
--rw-r--r--   0 runner    (1001) docker     (122)     8907 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/core/reduction.py
--rw-r--r--   0 runner    (1001) docker     (122)    14240 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/core/shape.py
--rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/core/structured.py
--rw-r--r--   0 runner    (1001) docker     (122)     3782 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/core/trigonometry.py
--rw-r--r--   0 runner    (1001) docker     (122)     2064 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/core/unary.py
--rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/core/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    29249 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/core/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 07:46:21.583951 scipp-23.3.1/src/scipp/data/
--rw-r--r--   0 runner    (1001) docker     (122)     3002 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      505 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/extend_units.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 07:46:21.583951 scipp-23.3.1/src/scipp/format/
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2151 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/format/_parse.py
--rw-r--r--   0 runner    (1001) docker     (122)     7534 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/format/formatter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1963 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 07:46:21.583951 scipp-23.3.1/src/scipp/html/
--rw-r--r--   0 runner    (1001) docker     (122)     1487 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5621 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/html/formatting_datagroup_html.py
--rw-r--r--   0 runner    (1001) docker     (122)    16472 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/html/formatting_html.py
--rw-r--r--   0 runner    (1001) docker     (122)     3221 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/html/resources.py
--rw-r--r--   0 runner    (1001) docker     (122)     7211 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/html/table.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 07:46:21.587951 scipp-23.3.1/src/scipp/html/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      154 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/html/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3254 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/html/templates/datagroup.css
--rw-r--r--   0 runner    (1001) docker     (122)      828 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/html/templates/dg_atomic_row.html
--rw-r--r--   0 runner    (1001) docker     (122)     1235 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/html/templates/dg_collapsible_row.html
--rw-r--r--   0 runner    (1001) docker     (122)      708 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/html/templates/dg_detail_list.html
--rw-r--r--   0 runner    (1001) docker     (122)      885 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/html/templates/dg_repr.html
--rw-r--r--   0 runner    (1001) docker     (122)     1574 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/html/templates/icons-svg-inline.html
--rw-r--r--   0 runner    (1001) docker     (122)     9794 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/html/templates/style.css.template
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 07:46:21.587951 scipp-23.3.1/src/scipp/io/
--rw-r--r--   0 runner    (1001) docker     (122)      196 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14803 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/io/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (122)     8046 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/logging.py
--rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/object_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 07:46:21.591952 scipp-23.3.1/src/scipp/plotting/
--rw-r--r--   0 runner    (1001) docker     (122)     6496 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12585 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/plotting/controller.py
--rw-r--r--   0 runner    (1001) docker     (122)     2139 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/plotting/controller1d.py
--rw-r--r--   0 runner    (1001) docker     (122)     1294 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/plotting/controller2d.py
--rw-r--r--   0 runner    (1001) docker     (122)     2242 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/plotting/controller3d.py
--rw-r--r--   0 runner    (1001) docker     (122)     1278 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/plotting/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (122)      664 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/plotting/displayable.py
--rw-r--r--   0 runner    (1001) docker     (122)     6999 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/plotting/figure.py
--rw-r--r--   0 runner    (1001) docker     (122)    12821 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/plotting/figure1d.py
--rw-r--r--   0 runner    (1001) docker     (122)     5401 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/plotting/figure2d.py
--rw-r--r--   0 runner    (1001) docker     (122)    17551 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/plotting/figure3d.py
--rw-r--r--   0 runner    (1001) docker     (122)     8403 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/plotting/formatters.py
--rw-r--r--   0 runner    (1001) docker     (122)     4894 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/plotting/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/plotting/model1d.py
--rw-r--r--   0 runner    (1001) docker     (122)     2035 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/plotting/model2d.py
--rw-r--r--   0 runner    (1001) docker     (122)     3449 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/plotting/model3d.py
--rw-r--r--   0 runner    (1001) docker     (122)    12741 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/plotting/objects.py
--rw-r--r--   0 runner    (1001) docker     (122)      747 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/plotting/panel.py
--rw-r--r--   0 runner    (1001) docker     (122)     3903 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/plotting/panel1d.py
--rw-r--r--   0 runner    (1001) docker     (122)     8410 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/plotting/panel3d.py
--rw-r--r--   0 runner    (1001) docker     (122)     2689 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/plotting/plot1d.py
--rw-r--r--   0 runner    (1001) docker     (122)     2474 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/plotting/plot2d.py
--rw-r--r--   0 runner    (1001) docker     (122)     3002 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/plotting/plot3d.py
--rw-r--r--   0 runner    (1001) docker     (122)     4631 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/plotting/profile.py
--rw-r--r--   0 runner    (1001) docker     (122)    13330 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/plotting/resampling_model.py
--rw-r--r--   0 runner    (1001) docker     (122)    10875 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/plotting/toolbar.py
--rw-r--r--   0 runner    (1001) docker     (122)     7515 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/plotting/tools.py
--rw-r--r--   0 runner    (1001) docker     (122)     5991 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/plotting/view.py
--rw-r--r--   0 runner    (1001) docker     (122)     4109 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/plotting/view1d.py
--rw-r--r--   0 runner    (1001) docker     (122)     6575 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/plotting/view2d.py
--rw-r--r--   0 runner    (1001) docker     (122)     2119 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/plotting/view3d.py
--rw-r--r--   0 runner    (1001) docker     (122)    13182 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/plotting/widgets.py
--rw-r--r--   0 runner    (1001) docker     (122)     6713 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/plotting/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     3139 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/reduction.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 07:46:21.591952 scipp-23.3.1/src/scipp/scipy/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/scipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 07:46:21.591952 scipp-23.3.1/src/scipp/scipy/integrate/
--rw-r--r--   0 runner    (1001) docker     (122)     2265 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/scipy/integrate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 07:46:21.591952 scipp-23.3.1/src/scipp/scipy/interpolate/
--rw-r--r--   0 runner    (1001) docker     (122)     7498 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/scipy/interpolate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 07:46:21.591952 scipp-23.3.1/src/scipp/scipy/ndimage/
--rw-r--r--   0 runner    (1001) docker     (122)    10453 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/scipy/ndimage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 07:46:21.591952 scipp-23.3.1/src/scipp/scipy/optimize/
--rw-r--r--   0 runner    (1001) docker     (122)     8944 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/scipy/optimize/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 07:46:21.591952 scipp-23.3.1/src/scipp/scipy/signal/
--rw-r--r--   0 runner    (1001) docker     (122)     5097 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/scipy/signal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/serialization.py
--rw-r--r--   0 runner    (1001) docker     (122)    19028 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/show.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 07:46:21.591952 scipp-23.3.1/src/scipp/spatial/
--rw-r--r--   0 runner    (1001) docker     (122)    11951 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/spatial/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 07:46:21.591952 scipp-23.3.1/src/scipp/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/sphinxext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4183 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/sphinxext/autoplot.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 07:46:21.591952 scipp-23.3.1/src/scipp/testing/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5042 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/testing/assertions.py
--rw-r--r--   0 runner    (1001) docker     (122)     7749 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/testing/strategies.py
--rw-r--r--   0 runner    (1001) docker     (122)     2877 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 07:46:21.591952 scipp-23.3.1/src/scipp/units/
--rw-r--r--   0 runner    (1001) docker     (122)     6561 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/units/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 07:46:21.595952 scipp-23.3.1/src/scipp/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      311 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3906 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/utils/collapse_and_slices.py
--rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (122)     2567 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/utils/comparison.py
--rw-r--r--   0 runner    (1001) docker     (122)      507 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/utils/graph.py
--rw-r--r--   0 runner    (1001) docker     (122)      766 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/utils/profile.py
--rw-r--r--   0 runner    (1001) docker     (122)      597 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/utils/pyshell.py
--rw-r--r--   0 runner    (1001) docker     (122)     1161 2023-04-03 07:45:51.000000 scipp-23.3.1/src/scipp/utils/to_string.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.716752 scipp-23.3.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-04-12 09:46:36.000000 scipp-23.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     2535 2023-04-12 09:46:59.716752 scipp-23.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2023-04-12 09:46:36.000000 scipp-23.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.700752 scipp-23.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.704752 scipp-23.3.2/src/scipp/
+-rw-r--r--   0 runner    (1001) docker     (122)     6117 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3496 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/_binding.py
+-rw-r--r--   0 runner    (1001) docker     (122)      217 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/_scipp.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.704752 scipp-23.3.2/src/scipp/binning/
+-rw-r--r--   0 runner    (1001) docker     (122)      475 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/binning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.704752 scipp-23.3.2/src/scipp/compat/
+-rw-r--r--   0 runner    (1001) docker     (122)      286 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5935 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/compat/dict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/compat/pandas_compat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/compat/wrapping.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5866 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/compat/xarray_compat.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.704752 scipp-23.3.2/src/scipp/configuration/
+-rw-r--r--   0 runner    (1001) docker     (122)     4210 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3752 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/configuration/config_default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.704752 scipp-23.3.2/src/scipp/constants/
+-rw-r--r--   0 runner    (1001) docker     (122)     4941 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/constants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.704752 scipp-23.3.2/src/scipp/coords/
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/coords/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1086 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/coords/coord.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2601 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/coords/coord_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5211 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/coords/graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)      378 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/coords/options.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7528 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/coords/rule.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12893 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/coords/transform_coords.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.708752 scipp-23.3.2/src/scipp/core/
+-rw-r--r--   0 runner    (1001) docker     (122)     3653 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      623 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/_cpp_wrapper_util.py
+-rw-r--r--   0 runner    (1001) docker     (122)      727 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5742 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6803 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/bin_remapping.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26466 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/binning.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17954 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/bins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8807 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3103 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/concepts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/counts.py
+-rw-r--r--   0 runner    (1001) docker     (122)      479 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/cpp_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    41780 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/cpp_classes.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1362 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/cumulative.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19386 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/data_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)      858 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5712 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/domains.py
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/groupby.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5258 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/like.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1740 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/logical.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9715 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/math.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9671 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/operations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8907 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/reduction.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14240 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/shape.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/structured.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3782 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/trigonometry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2064 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/unary.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29249 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.708752 scipp-23.3.2/src/scipp/data/
+-rw-r--r--   0 runner    (1001) docker     (122)     3002 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      505 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/extend_units.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.708752 scipp-23.3.2/src/scipp/format/
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2151 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/format/_parse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7534 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/format/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1963 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.708752 scipp-23.3.2/src/scipp/html/
+-rw-r--r--   0 runner    (1001) docker     (122)     1487 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5621 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/html/formatting_datagroup_html.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16472 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/html/formatting_html.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3221 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/html/resources.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7211 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/html/table.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.712752 scipp-23.3.2/src/scipp/html/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      154 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/html/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3254 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/html/templates/datagroup.css
+-rw-r--r--   0 runner    (1001) docker     (122)      828 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/html/templates/dg_atomic_row.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1235 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/html/templates/dg_collapsible_row.html
+-rw-r--r--   0 runner    (1001) docker     (122)      708 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/html/templates/dg_detail_list.html
+-rw-r--r--   0 runner    (1001) docker     (122)      885 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/html/templates/dg_repr.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1574 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/html/templates/icons-svg-inline.html
+-rw-r--r--   0 runner    (1001) docker     (122)     9794 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/html/templates/style.css.template
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.712752 scipp-23.3.2/src/scipp/io/
+-rw-r--r--   0 runner    (1001) docker     (122)      196 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14803 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/io/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8046 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/object_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.712752 scipp-23.3.2/src/scipp/plotting/
+-rw-r--r--   0 runner    (1001) docker     (122)     6496 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12585 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/controller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2139 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/controller1d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1294 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/controller2d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2242 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/controller3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1278 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      664 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/displayable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6999 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/figure.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12821 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/figure1d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5401 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/figure2d.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17551 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/figure3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8403 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4894 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/model1d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2035 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/model2d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3449 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/model3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12741 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)      747 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/panel.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3903 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/panel1d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8410 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/panel3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2689 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/plot1d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2474 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/plot2d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3002 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/plot3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4631 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/profile.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13330 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/resampling_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10875 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7515 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/tools.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5991 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/view.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4109 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/view1d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6575 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/view2d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2119 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/view3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13182 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6713 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     3139 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/reduction.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.712752 scipp-23.3.2/src/scipp/scipy/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/scipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.712752 scipp-23.3.2/src/scipp/scipy/integrate/
+-rw-r--r--   0 runner    (1001) docker     (122)     2265 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/scipy/integrate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.716752 scipp-23.3.2/src/scipp/scipy/interpolate/
+-rw-r--r--   0 runner    (1001) docker     (122)     7498 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/scipy/interpolate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.716752 scipp-23.3.2/src/scipp/scipy/ndimage/
+-rw-r--r--   0 runner    (1001) docker     (122)    10453 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/scipy/ndimage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.716752 scipp-23.3.2/src/scipp/scipy/optimize/
+-rw-r--r--   0 runner    (1001) docker     (122)     8944 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/scipy/optimize/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.716752 scipp-23.3.2/src/scipp/scipy/signal/
+-rw-r--r--   0 runner    (1001) docker     (122)     5097 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/scipy/signal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19028 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/show.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.716752 scipp-23.3.2/src/scipp/spatial/
+-rw-r--r--   0 runner    (1001) docker     (122)    11951 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/spatial/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.716752 scipp-23.3.2/src/scipp/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/sphinxext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4183 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/sphinxext/autoplot.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.716752 scipp-23.3.2/src/scipp/testing/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5042 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/testing/assertions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7749 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/testing/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2877 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.716752 scipp-23.3.2/src/scipp/units/
+-rw-r--r--   0 runner    (1001) docker     (122)     6561 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/units/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.716752 scipp-23.3.2/src/scipp/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      311 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3906 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/utils/collapse_and_slices.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2567 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/utils/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (122)      507 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/utils/graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)      766 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/utils/profile.py
+-rw-r--r--   0 runner    (1001) docker     (122)      597 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/utils/pyshell.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1161 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/utils/to_string.py
```

### Comparing `scipp-23.3.1/LICENSE` & `scipp-23.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/PKG-INFO` & `scipp-23.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scipp
-Version: 23.3.1
+Version: 23.3.2
 Summary: Multi-dimensional data arrays with labeled dimensions
 Home-page: https://github.com/scipp/scipp
 Author: Scipp contributors (https://github.com/scipp)
 License: BSD-3-Clause
 Project-URL: Documentation, https://scipp.github.io/
 Project-URL: Bug Tracker, https://github.com/scipp/scipp/issues
 Project-URL: Changelog, https://scipp.github.io/about/release-notes.html
```

### Comparing `scipp-23.3.1/src/scipp/__init__.py` & `scipp-23.3.2/src/scipp/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/_binding.py` & `scipp-23.3.2/src/scipp/_binding.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/compat/dict.py` & `scipp-23.3.2/src/scipp/compat/dict.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/compat/pandas_compat.py` & `scipp-23.3.2/src/scipp/compat/pandas_compat.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/compat/wrapping.py` & `scipp-23.3.2/src/scipp/compat/wrapping.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/compat/xarray_compat.py` & `scipp-23.3.2/src/scipp/compat/xarray_compat.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/configuration/__init__.py` & `scipp-23.3.2/src/scipp/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/configuration/config_default.yaml` & `scipp-23.3.2/src/scipp/configuration/config_default.yaml`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/constants/__init__.py` & `scipp-23.3.2/src/scipp/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/coords/coord.py` & `scipp-23.3.2/src/scipp/coords/coord.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/coords/coord_table.py` & `scipp-23.3.2/src/scipp/coords/coord_table.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/coords/graph.py` & `scipp-23.3.2/src/scipp/coords/graph.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/coords/rule.py` & `scipp-23.3.2/src/scipp/coords/rule.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/coords/transform_coords.py` & `scipp-23.3.2/src/scipp/coords/transform_coords.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/core/__init__.py` & `scipp-23.3.2/src/scipp/core/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/core/_cpp_wrapper_util.py` & `scipp-23.3.2/src/scipp/core/_cpp_wrapper_util.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/core/_sizes.py` & `scipp-23.3.2/src/scipp/core/_sizes.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/core/arithmetic.py` & `scipp-23.3.2/src/scipp/core/arithmetic.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/core/bin_remapping.py` & `scipp-23.3.2/src/scipp/core/bin_remapping.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/core/binning.py` & `scipp-23.3.2/src/scipp/core/binning.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/core/bins.py` & `scipp-23.3.2/src/scipp/core/bins.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/core/comparison.py` & `scipp-23.3.2/src/scipp/core/comparison.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/core/concepts.py` & `scipp-23.3.2/src/scipp/core/concepts.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/core/counts.py` & `scipp-23.3.2/src/scipp/core/counts.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/core/cpp_classes.pyi` & `scipp-23.3.2/src/scipp/core/cpp_classes.pyi`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/core/cumulative.py` & `scipp-23.3.2/src/scipp/core/cumulative.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/core/data_group.py` & `scipp-23.3.2/src/scipp/core/data_group.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/core/dataset.py` & `scipp-23.3.2/src/scipp/core/dataset.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/core/dimensions.py` & `scipp-23.3.2/src/scipp/core/dimensions.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/core/domains.py` & `scipp-23.3.2/src/scipp/core/domains.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/core/groupby.py` & `scipp-23.3.2/src/scipp/core/groupby.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/core/like.py` & `scipp-23.3.2/src/scipp/core/like.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/core/logical.py` & `scipp-23.3.2/src/scipp/core/logical.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/core/math.py` & `scipp-23.3.2/src/scipp/core/math.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/core/operations.py` & `scipp-23.3.2/src/scipp/core/operations.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/core/reduction.py` & `scipp-23.3.2/src/scipp/core/reduction.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/core/shape.py` & `scipp-23.3.2/src/scipp/core/shape.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/core/structured.py` & `scipp-23.3.2/src/scipp/core/structured.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/core/trigonometry.py` & `scipp-23.3.2/src/scipp/core/trigonometry.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/core/unary.py` & `scipp-23.3.2/src/scipp/core/unary.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/core/util.py` & `scipp-23.3.2/src/scipp/core/util.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/core/variable.py` & `scipp-23.3.2/src/scipp/core/variable.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/data/__init__.py` & `scipp-23.3.2/src/scipp/data/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/format/_parse.py` & `scipp-23.3.2/src/scipp/format/_parse.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/format/formatter.py` & `scipp-23.3.2/src/scipp/format/formatter.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/geometry.py` & `scipp-23.3.2/src/scipp/geometry.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/html/__init__.py` & `scipp-23.3.2/src/scipp/html/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/html/formatting_datagroup_html.py` & `scipp-23.3.2/src/scipp/html/formatting_datagroup_html.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/html/formatting_html.py` & `scipp-23.3.2/src/scipp/html/formatting_html.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/html/resources.py` & `scipp-23.3.2/src/scipp/html/resources.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/html/table.py` & `scipp-23.3.2/src/scipp/html/table.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/html/templates/datagroup.css` & `scipp-23.3.2/src/scipp/html/templates/datagroup.css`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/html/templates/dg_atomic_row.html` & `scipp-23.3.2/src/scipp/html/templates/dg_atomic_row.html`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/html/templates/dg_collapsible_row.html` & `scipp-23.3.2/src/scipp/html/templates/dg_collapsible_row.html`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/html/templates/dg_detail_list.html` & `scipp-23.3.2/src/scipp/html/templates/dg_detail_list.html`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/html/templates/dg_repr.html` & `scipp-23.3.2/src/scipp/html/templates/dg_repr.html`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/html/templates/icons-svg-inline.html` & `scipp-23.3.2/src/scipp/html/templates/icons-svg-inline.html`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/html/templates/style.css.template` & `scipp-23.3.2/src/scipp/html/templates/style.css.template`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/io/hdf5.py` & `scipp-23.3.2/src/scipp/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/logging.py` & `scipp-23.3.2/src/scipp/logging.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/object_list.py` & `scipp-23.3.2/src/scipp/object_list.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/operations.py` & `scipp-23.3.2/src/scipp/operations.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/plotting/__init__.py` & `scipp-23.3.2/src/scipp/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/plotting/controller.py` & `scipp-23.3.2/src/scipp/plotting/controller.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/plotting/controller1d.py` & `scipp-23.3.2/src/scipp/plotting/controller1d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/plotting/controller2d.py` & `scipp-23.3.2/src/scipp/plotting/controller2d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/plotting/controller3d.py` & `scipp-23.3.2/src/scipp/plotting/controller3d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/plotting/dispatch.py` & `scipp-23.3.2/src/scipp/plotting/dispatch.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/plotting/displayable.py` & `scipp-23.3.2/src/scipp/plotting/displayable.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/plotting/figure.py` & `scipp-23.3.2/src/scipp/plotting/figure.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/plotting/figure1d.py` & `scipp-23.3.2/src/scipp/plotting/figure1d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/plotting/figure2d.py` & `scipp-23.3.2/src/scipp/plotting/figure2d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/plotting/figure3d.py` & `scipp-23.3.2/src/scipp/plotting/figure3d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/plotting/formatters.py` & `scipp-23.3.2/src/scipp/plotting/formatters.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/plotting/model.py` & `scipp-23.3.2/src/scipp/plotting/model.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/plotting/model1d.py` & `scipp-23.3.2/src/scipp/plotting/model1d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/plotting/model2d.py` & `scipp-23.3.2/src/scipp/plotting/model2d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/plotting/model3d.py` & `scipp-23.3.2/src/scipp/plotting/model3d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/plotting/objects.py` & `scipp-23.3.2/src/scipp/plotting/objects.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/plotting/panel.py` & `scipp-23.3.2/src/scipp/plotting/panel.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/plotting/panel1d.py` & `scipp-23.3.2/src/scipp/plotting/panel1d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/plotting/panel3d.py` & `scipp-23.3.2/src/scipp/plotting/panel3d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/plotting/plot1d.py` & `scipp-23.3.2/src/scipp/plotting/plot1d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/plotting/plot2d.py` & `scipp-23.3.2/src/scipp/plotting/plot2d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/plotting/plot3d.py` & `scipp-23.3.2/src/scipp/plotting/plot3d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/plotting/profile.py` & `scipp-23.3.2/src/scipp/plotting/profile.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/plotting/resampling_model.py` & `scipp-23.3.2/src/scipp/plotting/resampling_model.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/plotting/toolbar.py` & `scipp-23.3.2/src/scipp/plotting/toolbar.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/plotting/tools.py` & `scipp-23.3.2/src/scipp/plotting/tools.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/plotting/view.py` & `scipp-23.3.2/src/scipp/plotting/view.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/plotting/view1d.py` & `scipp-23.3.2/src/scipp/plotting/view1d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/plotting/view2d.py` & `scipp-23.3.2/src/scipp/plotting/view2d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/plotting/view3d.py` & `scipp-23.3.2/src/scipp/plotting/view3d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/plotting/widgets.py` & `scipp-23.3.2/src/scipp/plotting/widgets.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/plotting/wrapper.py` & `scipp-23.3.2/src/scipp/plotting/wrapper.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/reduction.py` & `scipp-23.3.2/src/scipp/reduction.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/scipy/integrate/__init__.py` & `scipp-23.3.2/src/scipp/scipy/integrate/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/scipy/interpolate/__init__.py` & `scipp-23.3.2/src/scipp/scipy/interpolate/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/scipy/ndimage/__init__.py` & `scipp-23.3.2/src/scipp/scipy/ndimage/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/scipy/optimize/__init__.py` & `scipp-23.3.2/src/scipp/scipy/optimize/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/scipy/signal/__init__.py` & `scipp-23.3.2/src/scipp/scipy/signal/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/serialization.py` & `scipp-23.3.2/src/scipp/serialization.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/show.py` & `scipp-23.3.2/src/scipp/show.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/spatial/__init__.py` & `scipp-23.3.2/src/scipp/spatial/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/sphinxext/autoplot.py` & `scipp-23.3.2/src/scipp/sphinxext/autoplot.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/testing/assertions.py` & `scipp-23.3.2/src/scipp/testing/assertions.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/testing/strategies.py` & `scipp-23.3.2/src/scipp/testing/strategies.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/typing.py` & `scipp-23.3.2/src/scipp/typing.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/units/__init__.py` & `scipp-23.3.2/src/scipp/units/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/utils/collapse_and_slices.py` & `scipp-23.3.2/src/scipp/utils/collapse_and_slices.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/utils/colors.py` & `scipp-23.3.2/src/scipp/utils/colors.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/utils/comparison.py` & `scipp-23.3.2/src/scipp/utils/comparison.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/utils/profile.py` & `scipp-23.3.2/src/scipp/utils/profile.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/utils/pyshell.py` & `scipp-23.3.2/src/scipp/utils/pyshell.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.1/src/scipp/utils/to_string.py` & `scipp-23.3.2/src/scipp/utils/to_string.py`

 * *Files identical despite different names*

