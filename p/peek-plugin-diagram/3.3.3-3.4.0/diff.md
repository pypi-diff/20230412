# Comparing `tmp/peek-plugin-diagram-3.3.3.tar.gz` & `tmp/peek-plugin-diagram-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-plugin-diagram-3.3.3.tar", last modified: Mon Nov 14 05:37:11 2022, max compression
+gzip compressed data, was "peek-plugin-diagram-3.4.0.tar", last modified: Wed Apr 12 11:05:55 2023, max compression
```

## Comparing `peek-plugin-diagram-3.3.3.tar` & `peek-plugin-diagram-3.4.0.tar`

### file list

```diff
@@ -1,522 +1,561 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.206796 peek-plugin-diagram-3.3.3/
--rw-r--r--   0 root         (0) root         (0)      400 2022-11-14 05:37:11.206796 peek-plugin-diagram-3.3.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      580 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.175796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/
--rw-r--r--   0 root         (0) root         (0)     1155 2022-11-14 05:37:10.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.176796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/
--rw-r--r--   0 root         (0) root         (0)     2226 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/GridKeyIndexTest.py
--rw-r--r--   0 root         (0) root         (0)      334 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/PluginNames.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.176796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/admin-app/
--rw-r--r--   0 root         (0) root         (0)     2563 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/admin-app/diagram.component.html
--rw-r--r--   0 root         (0) root         (0)      212 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/admin-app/diagram.component.ts
--rw-r--r--   0 root         (0) root         (0)     2288 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/admin-app/diagram.module.web.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.176796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/admin-app/edit-setting-table/
--rw-r--r--   0 root         (0) root         (0)     2595 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/admin-app/edit-setting-table/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     1469 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/admin-app/edit-setting-table/edit.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.177796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/admin-app/status/
--rw-r--r--   0 root         (0) root         (0)     2125 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/admin-app/status/status.component.html
--rw-r--r--   0 root         (0) root         (0)     1064 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/admin-app/status/status.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.177796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/admin-app/tuples/
--rw-r--r--   0 root         (0) root         (0)     1065 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/admin-app/tuples/DiagramImporterStatusTuple.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.177796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/agent/
--rw-r--r--   0 root         (0) root         (0)      668 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/agent/AgentEntryHook.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.177796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/__init__.py
--rw-r--r--   0 root         (0) root         (0)      325 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      543 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.180796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     2809 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/0db3aedfee95_added_column_showforedit.py
--rw-r--r--   0 root         (0) root         (0)     1089 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/128b23798db0_add_text_border_for_curved_text.py
--rw-r--r--   0 root         (0) root         (0)     1057 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/1856b7fb8803_added_linetemplatesenabled.py
--rw-r--r--   0 root         (0) root         (0)     3292 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/1b17ef0cca17_removed_string_field_sizes.py
--rw-r--r--   0 root         (0) root         (0)      861 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/1fe753e1f369_disptext_textstyleid_not_null.py
--rw-r--r--   0 root         (0) root         (0)     1599 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/2127d894e46b_moved_smallest_sizes_to_grids.py
--rw-r--r--   0 root         (0) root         (0)     4444 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/23117803d414_added_location_index.py
--rw-r--r--   0 root         (0) root         (0)     1432 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/24b83c5e7e31_renamed_location_indexes.py
--rw-r--r--   0 root         (0) root         (0)      941 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/298b291aac2d_encoded_grids_are_now_gridtuples.py
--rw-r--r--   0 root         (0) root         (0)     1612 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/2c5f47322bda_removed_node_and_conn.py
--rw-r--r--   0 root         (0) root         (0)     1225 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/2fc6d3246717_added_compiler_q_indexes.py
--rw-r--r--   0 root         (0) root         (0)      741 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/34dd05f474df_rebuild_location_index.py
--rw-r--r--   0 root         (0) root         (0)     1061 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/361988cd327d_added_createddate_to_branchindex.py
--rw-r--r--   0 root         (0) root         (0)     1300 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/3b41dec74e46_added_overlay_flag.py
--rw-r--r--   0 root         (0) root         (0)      794 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/42a8dc25e588_add_disp_action.py
--rw-r--r--   0 root         (0) root         (0)     1601 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/473d5f6a97e8_removed_more_string_sizes.py
--rw-r--r--   0 root         (0) root         (0)      923 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/47879bec4c5f_added_texthstretch.py
--rw-r--r--   0 root         (0) root         (0)      663 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/4925c894757b_enabled_nulls_for_text.py
--rw-r--r--   0 root         (0) root         (0)     2239 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/4b943b584307_added_coordset_mx_c.py
--rw-r--r--   0 root         (0) root         (0)     1963 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/4f6ed1047562_added_branch_fields_to_dispbase.py
--rw-r--r--   0 root         (0) root         (0)     1151 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/5307eb21c742_added_spacingbetweentexts_in_textstyle.py
--rw-r--r--   0 root         (0) root         (0)     1366 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/558bc7fc4d36_added_polyline_startkey_endkey.py
--rw-r--r--   0 root         (0) root         (0)     2225 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/5e2f84d757f2_added_cascade_constraints.py
--rw-r--r--   0 root         (0) root         (0)      815 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/6a71c73c0606_added_polygon_isrectangle.py
--rw-r--r--   0 root         (0) root         (0)     4052 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/6a97dd344aed_added_coordset_gridsizes.py
--rw-r--r--   0 root         (0) root         (0)      950 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/6d3a96cf1955_added_dispnull.py
--rw-r--r--   0 root         (0) root         (0)      839 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/6f545d4166dc_remove_unique_constraint_for_dispgroup.py
--rw-r--r--   0 root         (0) root         (0)    30200 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/7eed363f5df5_initial.py
--rw-r--r--   0 root         (0) root         (0)     6602 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/81c1d2809046_added_coordset_editable_fields.py
--rw-r--r--   0 root         (0) root         (0)      637 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/8b8ebbe5ec7b_added_scalable_to_lookup_linestyle.py
--rw-r--r--   0 root         (0) root         (0)     2055 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/8ef78f862ac8_updates_for_dispgroup.py
--rw-r--r--   0 root         (0) root         (0)     1142 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/97990b4ca6a1_added_landingcoordsetid.py
--rw-r--r--   0 root         (0) root         (0)     3102 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/9e7ca1acd6be_fixed_importhash_indexes_for_lookups.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1665 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/a4c59bcaaf88_added_curved_text_disp.py
--rw-r--r--   0 root         (0) root         (0)     1088 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/a66e033b8227_updated_float_precision_in_zoom_levels.py
--rw-r--r--   0 root         (0) root         (0)     1018 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/a73574690197_coordset_positiononzoom.py
--rw-r--r--   0 root         (0) root         (0)     1839 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/a86e0317e22a_added_poly_template_name.py
--rw-r--r--   0 root         (0) root         (0)     3382 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/aa76b059b81e_added_default_group_ptr_to_coord_set.py
--rw-r--r--   0 root         (0) root         (0)     2076 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/bf8f559c4df9_removed_branchgridindex.py
--rw-r--r--   0 root         (0) root         (0)      779 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/bfdd4f46e293_added_coordset_key.py
--rw-r--r--   0 root         (0) root         (0)      773 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/c88ba8f6761f_added_disp_zorder.py
--rw-r--r--   0 root         (0) root         (0)      953 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/cbd5e370686f_increased_size_of_disp_json.py
--rw-r--r--   0 root         (0) root         (0)      657 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/cea17a52b9ae_timezone_aware.py
--rw-r--r--   0 root         (0) root         (0)      600 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/d103b9c1eba9_added_disp_data.py
--rw-r--r--   0 root         (0) root         (0)     1027 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/d6e25d8ba156_added_textheight_to_disptext.py
--rw-r--r--   0 root         (0) root         (0)     3887 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/da424430bf97_added_edgecolor_removed_lu_indexes.py
--rw-r--r--   0 root         (0) root         (0)     1323 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/e3c2c2580dea_add_text_border_color_and_width.py
--rw-r--r--   0 root         (0) root         (0)     1034 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/e8d6d02c0922_added_polyline_start_end_types.py
--rw-r--r--   0 root         (0) root         (0)      737 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/e9d80c4c087d_increased_size_of_importgrouphash.py
--rw-r--r--   0 root         (0) root         (0)     1569 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/ec97d31aebb0_added_line_templates.py
--rw-r--r--   0 root         (0) root         (0)     1016 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/f4dce3e782ec_added_coordset_dispgroup_enabled.py
--rw-r--r--   0 root         (0) root         (0)     3351 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/f697025b2013_updated_to_bigintegers.py
--rw-r--r--   0 root         (0) root         (0)     4968 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/f76791d27f6d_added_branch_tables.py
--rw-r--r--   0 root         (0) root         (0)       94 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.181796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/
--rw-r--r--   0 root         (0) root         (0)     3262 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/DiagramUtil.ts
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.181796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/branch-detail-component/
--rw-r--r--   0 root         (0) root         (0)     3124 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/branch-detail-component/branch-detail.component.web.html
--rw-r--r--   0 root         (0) root         (0)      255 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/branch-detail-component/branch-detail.component.web.scss
--rw-r--r--   0 root         (0) root         (0)     7472 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/branch-detail-component/branch-detail.component.web.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.181796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/cache/
--rw-r--r--   0 root         (0) root         (0)     7743 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/cache/GridCache.web.ts
--rw-r--r--   0 root         (0) root         (0)     4149 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/cache/GridObservable.web.ts
--rw-r--r--   0 root         (0) root         (0)     2498 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/cache/LinkedGrid.web.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.182796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas/
--rw-r--r--   0 root         (0) root         (0)     2375 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasActioner.ts
--rw-r--r--   0 root         (0) root         (0)       88 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasBounds.ts
--rw-r--r--   0 root         (0) root         (0)     5597 2022-11-14 05:34:34.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasConfig.web.ts
--rw-r--r--   0 root         (0) root         (0)     1281 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasEdgeTemplatePropsContext.ts
--rw-r--r--   0 root         (0) root         (0)     8139 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasEditor.web.ts
--rw-r--r--   0 root         (0) root         (0)     8888 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasEditorProps.ts
--rw-r--r--   0 root         (0) root         (0)      308 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasEditorToolType.web.ts
--rw-r--r--   0 root         (0) root         (0)     2361 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasExtensions.web.ts
--rw-r--r--   0 root         (0) root         (0)     1277 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasGroupPtrPropsContext.ts
--rw-r--r--   0 root         (0) root         (0)    17844 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasModel.web.ts
--rw-r--r--   0 root         (0) root         (0)     8528 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasModelQuery.web.ts
--rw-r--r--   0 root         (0) root         (0)     2489 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasModelSelection.web.ts
--rw-r--r--   0 root         (0) root         (0)      913 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasModelUtil.web.ts
--rw-r--r--   0 root         (0) root         (0)     3998 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasShapePropsContext.ts
--rw-r--r--   0 root         (0) root         (0)      142 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas/PeekInterfaces.web.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.183796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-component/
--rw-r--r--   0 root         (0) root         (0)     2546 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-component/canvas-component.web.html
--rw-r--r--   0 root         (0) root         (0)      305 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-component/canvas-component.web.scss
--rw-r--r--   0 root         (0) root         (0)    14545 2022-11-14 05:34:34.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-component/canvas-component.web.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.183796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-context-menu-component/
--rw-r--r--   0 root         (0) root         (0)      901 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-context-menu-component/canvas-context-menu.component.web.html
--rw-r--r--   0 root         (0) root         (0)      535 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-context-menu-component/canvas-context-menu.component.web.scss
--rw-r--r--   0 root         (0) root         (0)     2600 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-context-menu-component/canvas-context-menu.component.web.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.184796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-input/
--rw-r--r--   0 root         (0) root         (0)     9680 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInput.web.ts
--rw-r--r--   0 root         (0) root         (0)     4295 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputDelegate.web.ts
--rw-r--r--   0 root         (0) root         (0)     1942 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputDelegateUtil.web.ts
--rw-r--r--   0 root         (0) root         (0)     5068 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputEditMakeEllipseDelegate.web.ts
--rw-r--r--   0 root         (0) root         (0)     3718 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputEditMakeGroupPtrVertexDelegate.web.ts
--rw-r--r--   0 root         (0) root         (0)      967 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputEditMakeLineWithArrowDelegate.web.ts
--rw-r--r--   0 root         (0) root         (0)     9118 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputEditMakePolyDelegate.web.ts
--rw-r--r--   0 root         (0) root         (0)      955 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputEditMakePolygonDelegate.web.ts
--rw-r--r--   0 root         (0) root         (0)     1023 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputEditMakePolylineDelegate.web.ts
--rw-r--r--   0 root         (0) root         (0)     5090 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputEditMakeRectangleDelegate.web.ts
--rw-r--r--   0 root         (0) root         (0)     4347 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputEditMakeTextDelegate.web.ts
--rw-r--r--   0 root         (0) root         (0)    27281 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputEditSelectDelegate.web.ts
--rw-r--r--   0 root         (0) root         (0)     1550 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputMakeDispPolylineEdgeDelegate.web.ts
--rw-r--r--   0 root         (0) root         (0)    15112 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputSelectDelegate.web.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.184796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-override/
--rw-r--r--   0 root         (0) root         (0)      896 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-override/PeekCanvasModelOverrideA.ts
--rw-r--r--   0 root         (0) root         (0)     2889 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-override/PeekCanvasModelOverrideColor.ts
--rw-r--r--   0 root         (0) root         (0)     4206 2022-11-14 05:34:34.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-override/PeekCanvasModelOverrideHighlight.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.185796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-render/
--rw-r--r--   0 root         (0) root         (0)     8778 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-render/PeekCanvasRenderer.web.ts
--rw-r--r--   0 root         (0) root         (0)     1668 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-render/PeekDispRenderDelegateABC.web.ts
--rw-r--r--   0 root         (0) root         (0)    24015 2022-11-14 05:34:34.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-render/PeekDispRenderDelegateCurvedText.web.ts
--rw-r--r--   0 root         (0) root         (0)     3817 2022-11-14 05:34:34.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-render/PeekDispRenderDelegateEllipse.web.ts
--rw-r--r--   0 root         (0) root         (0)     4785 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-render/PeekDispRenderDelegateGroupPtr.web.ts
--rw-r--r--   0 root         (0) root         (0)     1144 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-render/PeekDispRenderDelegateNull.web.ts
--rw-r--r--   0 root         (0) root         (0)    13168 2022-11-14 05:34:34.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-render/PeekDispRenderDelegatePoly.web.ts
--rw-r--r--   0 root         (0) root         (0)     7325 2022-11-14 05:34:34.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-render/PeekDispRenderDelegateText.web.ts
--rw-r--r--   0 root         (0) root         (0)       83 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-render/PeekDispRenderDrawModeE.web.ts
--rw-r--r--   0 root         (0) root         (0)     4792 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-render/PeekDispRenderFactory.web.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.186796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-shapes/
--rw-r--r--   0 root         (0) root         (0)    11837 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-shapes/DispBase.ts
--rw-r--r--   0 root         (0) root         (0)     6382 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-shapes/DispCurvedText.ts
--rw-r--r--   0 root         (0) root         (0)     1468 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-shapes/DispEdgeTemplate.ts
--rw-r--r--   0 root         (0) root         (0)     6852 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-shapes/DispEllipse.ts
--rw-r--r--   0 root         (0) root         (0)     1270 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-shapes/DispFactory.ts
--rw-r--r--   0 root         (0) root         (0)     1994 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-shapes/DispGroup.ts
--rw-r--r--   0 root         (0) root         (0)     8284 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-shapes/DispGroupPointer.ts
--rw-r--r--   0 root         (0) root         (0)     1687 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-shapes/DispNull.ts
--rw-r--r--   0 root         (0) root         (0)     3669 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-shapes/DispPoly.ts
--rw-r--r--   0 root         (0) root         (0)     8021 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-shapes/DispPolygon.ts
--rw-r--r--   0 root         (0) root         (0)    13434 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-shapes/DispPolyline.ts
--rw-r--r--   0 root         (0) root         (0)     1909 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-shapes/DispRectangle.ts
--rw-r--r--   0 root         (0) root         (0)     5812 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-shapes/DispText.ts
--rw-r--r--   0 root         (0) root         (0)     1371 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-shapes/DispUtil.ts
--rw-r--r--   0 root         (0) root         (0)     3427 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-shapes/DispUtilRotate.ts
--rw-r--r--   0 root         (0) root         (0)     1792 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/diagram.component.ts
--rw-r--r--   0 root         (0) root         (0)      105 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/diagram.component.web.html
--rw-r--r--   0 root         (0) root         (0)       54 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/diagram.component.web.scss
--rw-r--r--   0 root         (0) root         (0)      817 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/diagram.component.web.ts
--rw-r--r--   0 root         (0) root         (0)     4466 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/diagram.module.web.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.186796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-component/
--rw-r--r--   0 root         (0) root         (0)     1652 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-component/edit-props.component.web.html
--rw-r--r--   0 root         (0) root         (0)     1710 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-component/edit-props.component.web.scss
--rw-r--r--   0 root         (0) root         (0)     3245 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-component/edit-props.component.web.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.186796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-edge-template-component/
--rw-r--r--   0 root         (0) root         (0)     1618 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-edge-template-component/edit-props-edge-template.component.html
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-edge-template-component/edit-props-edge-template.component.scss
--rw-r--r--   0 root         (0) root         (0)     7356 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-edge-template-component/edit-props-edge-template.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.186796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-group-ptr-component/
--rw-r--r--   0 root         (0) root         (0)     1603 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-group-ptr-component/edit-props-group-ptr.component.html
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-group-ptr-component/edit-props-group-ptr.component.scss
--rw-r--r--   0 root         (0) root         (0)     7126 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-group-ptr-component/edit-props-group-ptr.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.187796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-livedb-component/
--rw-r--r--   0 root         (0) root         (0)       40 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-livedb-component/edit-props-livedb.component.html
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-livedb-component/edit-props-livedb.component.scss
--rw-r--r--   0 root         (0) root         (0)      516 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-livedb-component/edit-props-livedb.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.187796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-shape-component/
--rw-r--r--   0 root         (0) root         (0)     4391 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-shape-component/edit-props-shape.component.html
--rw-r--r--   0 root         (0) root         (0)       36 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-shape-component/edit-props-shape.component.scss
--rw-r--r--   0 root         (0) root         (0)     6163 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-shape-component/edit-props-shape.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.187796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-toolbar-component/
--rw-r--r--   0 root         (0) root         (0)     1975 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-toolbar-component/edit-props-toolbar.component.web.html
--rw-r--r--   0 root         (0) root         (0)     1484 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-toolbar-component/edit-props-toolbar.component.web.scss
--rw-r--r--   0 root         (0) root         (0)     2777 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-toolbar-component/edit-props-toolbar.component.web.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.187796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-toolbar-component/
--rw-r--r--   0 root         (0) root         (0)     9120 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-toolbar-component/edit-toolbar.component.web.html
--rw-r--r--   0 root         (0) root         (0)     1996 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-toolbar-component/edit-toolbar.component.web.scss
--rw-r--r--   0 root         (0) root         (0)     8761 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-toolbar-component/edit-toolbar.component.web.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.187796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/print-component/
--rw-r--r--   0 root         (0) root         (0)      401 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/print-component/print.component.web.html
--rw-r--r--   0 root         (0) root         (0)      535 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/print-component/print.component.web.scss
--rw-r--r--   0 root         (0) root         (0)     1348 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/print-component/print.component.web.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.188796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/services/
--rw-r--r--   0 root         (0) root         (0)      561 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/services/canvas.service.ts
--rw-r--r--   0 root         (0) root         (0)      702 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/services/context-menu.service.ts
--rw-r--r--   0 root         (0) root         (0)     3905 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/services/copy-paste.service.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.188796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/set-position-component/
--rw-r--r--   0 root         (0) root         (0)      388 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/set-position-component/set-position.component.html
--rw-r--r--   0 root         (0) root         (0)       30 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/set-position-component/set-position.component.scss
--rw-r--r--   0 root         (0) root         (0)     9027 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/set-position-component/set-position.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.188796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/start-edit-component/
--rw-r--r--   0 root         (0) root         (0)     4142 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/start-edit-component/start-edit.component.web.html
--rw-r--r--   0 root         (0) root         (0)      801 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/start-edit-component/start-edit.component.web.scss
--rw-r--r--   0 root         (0) root         (0)     7149 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/start-edit-component/start-edit.component.web.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.188796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/view-select-branches-component/
--rw-r--r--   0 root         (0) root         (0)     2583 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/view-select-branches-component/select-branches.component.web.html
--rw-r--r--   0 root         (0) root         (0)      762 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/view-select-branches-component/select-branches.component.web.scss
--rw-r--r--   0 root         (0) root         (0)     7999 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/view-select-branches-component/select-branches.component.web.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.188796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/view-select-layers-component/
--rw-r--r--   0 root         (0) root         (0)     1084 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/view-select-layers-component/select-layers.component.web.html
--rw-r--r--   0 root         (0) root         (0)      559 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/view-select-layers-component/select-layers.component.web.scss
--rw-r--r--   0 root         (0) root         (0)     3948 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/view-select-layers-component/select-layers.component.web.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.189796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/view-toolbar-component/
--rw-r--r--   0 root         (0) root         (0)     3593 2022-11-14 05:34:34.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/view-toolbar-component/toolbar.component.web.html
--rw-r--r--   0 root         (0) root         (0)     1348 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/view-toolbar-component/toolbar.component.web.scss
--rw-r--r--   0 root         (0) root         (0)     7226 2022-11-14 05:34:34.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/view-toolbar-component/toolbar.component.web.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.189796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-assets/
--rw-r--r--   0 root         (0) root         (0)    12054 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-assets/icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.189796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-cfg/
--rw-r--r--   0 root         (0) root         (0)     1658 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-cfg/diagram-cfg.component.ts
--rw-r--r--   0 root         (0) root         (0)     1345 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-cfg/diagram-cfg.component.web.html
--rw-r--r--   0 root         (0) root         (0)     1179 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-cfg/diagram-cfg.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.189796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/
--rw-r--r--   0 root         (0) root         (0)     9541 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/ClientEntryHook.py
--rw-r--r--   0 root         (0) root         (0)     5994 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/TupleDataObservable.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.190796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/controller/
--rw-r--r--   0 root         (0) root         (0)     1312 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/controller/BranchIndexCacheController.py
--rw-r--r--   0 root         (0) root         (0)     1734 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/controller/CoordSetCacheController.py
--rw-r--r--   0 root         (0) root         (0)     2490 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/controller/GridCacheController.py
--rw-r--r--   0 root         (0) root         (0)     1391 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/controller/LocationIndexCacheController.py
--rw-r--r--   0 root         (0) root         (0)     4227 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/controller/LookupCacheController.py
--rw-r--r--   0 root         (0) root         (0)     1500 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/controller/ModelSetCacheController.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/controller/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.190796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/handlers/
--rw-r--r--   0 root         (0) root         (0)     1108 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/handlers/BranchIndexCacheHandler.py
--rw-r--r--   0 root         (0) root         (0)     8950 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/handlers/GridCacheHandler.py
--rw-r--r--   0 root         (0) root         (0)     1138 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/handlers/LocationIndexCacheHandler.py
--rw-r--r--   0 root         (0) root         (0)      176 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/handlers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.191796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/tuple_providers/
--rw-r--r--   0 root         (0) root         (0)     1012 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/tuple_providers/BranchIndexUpdateDateTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     2817 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/tuple_providers/BranchTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1026 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/tuple_providers/ClientCoordSetTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     3918 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/tuple_providers/ClientDispKeyLocationTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1658 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/tuple_providers/ClientGroupDispsTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1026 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/tuple_providers/ClientLocationIndexUpdateDateTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1028 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/tuple_providers/ClientLookupTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1024 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/tuple_providers/ClientModelSetTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1829 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/tuple_providers/GridCacheIndexTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/tuple_providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.191796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/
--rw-r--r--   0 root         (0) root         (0)    12532 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/LogicEntryHook.py
--rw-r--r--   0 root         (0) root         (0)     1322 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/TupleActionProcessor.py
--rw-r--r--   0 root         (0) root         (0)     3829 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/TupleDataObservable.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.191796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/admin_handlers/
--rw-r--r--   0 root         (0) root         (0)      983 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/admin_handlers/SettingPropertyHandler.py
--rw-r--r--   0 root         (0) root         (0)     1667 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/admin_handlers/StringIntTableHandler.py
--rw-r--r--   0 root         (0) root         (0)      446 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/admin_handlers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.191796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/api/
--rw-r--r--   0 root         (0) root         (0)     1766 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/api/DiagramApi.py
--rw-r--r--   0 root         (0) root         (0)     3036 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/api/DiagramImportApi.py
--rw-r--r--   0 root         (0) root         (0)     1111 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/api/DiagramViewerApi.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.192796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/client_handlers/
--rw-r--r--   0 root         (0) root         (0)     2052 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/client_handlers/BranchIndexChunkLoadRpc.py
--rw-r--r--   0 root         (0) root         (0)      808 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/client_handlers/BranchIndexChunkUpdateHandler.py
--rw-r--r--   0 root         (0) root         (0)     2866 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/client_handlers/ClientGridLoaderRpc.py
--rw-r--r--   0 root         (0) root         (0)      757 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/client_handlers/ClientGridUpdateHandler.py
--rw-r--r--   0 root         (0) root         (0)     2618 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/client_handlers/ClientLocationIndexLoaderRpc.py
--rw-r--r--   0 root         (0) root         (0)     1435 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/client_handlers/ClientLocationIndexUpdateHandler.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/client_handlers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.193796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/controller/
--rw-r--r--   0 root         (0) root         (0)     4006 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/controller/BranchIndexCompilerQueueController.py
--rw-r--r--   0 root         (0) root         (0)     4131 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/controller/BranchLiveEditController.py
--rw-r--r--   0 root         (0) root         (0)     4729 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/controller/BranchUpdateController.py
--rw-r--r--   0 root         (0) root         (0)     5206 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/controller/DispCompilerQueueController.py
--rw-r--r--   0 root         (0) root         (0)     3933 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/controller/DispImportController.py
--rw-r--r--   0 root         (0) root         (0)     3754 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/controller/GridKeyCompilerQueueController.py
--rw-r--r--   0 root         (0) root         (0)     2683 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/controller/LiveDbWatchController.py
--rw-r--r--   0 root         (0) root         (0)     4214 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/controller/LocationCompilerQueueController.py
--rw-r--r--   0 root         (0) root         (0)     7879 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/controller/LookupImportController.py
--rw-r--r--   0 root         (0) root         (0)      433 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/controller/StatusController.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/controller/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.193796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/tuple_providers/
--rw-r--r--   0 root         (0) root         (0)     1614 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/tuple_providers/BranchKeyToIdMapProvider.py
--rw-r--r--   0 root         (0) root         (0)     1125 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/tuple_providers/BranchLiveEditTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)      925 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/tuple_providers/DiagramLoaderStatusTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1267 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/tuple_providers/ServerCoordSetTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1769 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/tuple_providers/ServerLookupTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)      945 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/tuple_providers/ServerModelSetTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/tuple_providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.194796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/storage/
--rw-r--r--   0 root         (0) root         (0)     1006 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/storage/DeclarativeBase.py
--rw-r--r--   0 root         (0) root         (0)      928 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/storage/DispIndex.py
--rw-r--r--   0 root         (0) root         (0)    25375 2022-11-14 05:34:34.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/storage/Display.py
--rw-r--r--   0 root         (0) root         (0)     4274 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/storage/GridKeyIndex.py
--rw-r--r--   0 root         (0) root         (0)     3172 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/storage/LiveDbDispLink.py
--rw-r--r--   0 root         (0) root         (0)     4389 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/storage/LocationIndex.py
--rw-r--r--   0 root         (0) root         (0)     9320 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/storage/ModelSet.py
--rw-r--r--   0 root         (0) root         (0)     7986 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/storage/Setting.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.194796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/storage/branch/
--rw-r--r--   0 root         (0) root         (0)     2211 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/storage/branch/BranchIndex.py
--rw-r--r--   0 root         (0) root         (0)     1368 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/storage/branch/BranchIndexCompilerQueue.py
--rw-r--r--   0 root         (0) root         (0)     2412 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/storage/branch/BranchIndexEncodedChunk.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/storage/branch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.194796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)     1132 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/DiagramImporterStatusTuple.py
--rw-r--r--   0 root         (0) root         (0)      563 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/GroupDispsTuple.py
--rw-r--r--   0 root         (0) root         (0)      875 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.195796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/branch/
--rw-r--r--   0 root         (0) root         (0)     1283 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/branch/BranchIndexUpdateDateTuple.py
--rw-r--r--   0 root         (0) root         (0)      542 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/branch/BranchKeyToIdMapTuple.py
--rw-r--r--   0 root         (0) root         (0)     1197 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/branch/BranchLiveEditTuple.py
--rw-r--r--   0 root         (0) root         (0)      690 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/branch/BranchLiveEditTupleAction.py
--rw-r--r--   0 root         (0) root         (0)     4565 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/branch/BranchTuple.py
--rw-r--r--   0 root         (0) root         (0)      585 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/branch/BranchUpdateTupleAction.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/branch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.195796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/grid/
--rw-r--r--   0 root         (0) root         (0)     1022 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/grid/EncodedGridTuple.py
--rw-r--r--   0 root         (0) root         (0)      362 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/grid/GridTuple.py
--rw-r--r--   0 root         (0) root         (0)     1053 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/grid/GridUpdateDateTuple.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/grid/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.195796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/location_index/
--rw-r--r--   0 root         (0) root         (0)      893 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/location_index/DispKeyLocationTuple.py
--rw-r--r--   0 root         (0) root         (0)      955 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/location_index/EncodedLocationIndexTuple.py
--rw-r--r--   0 root         (0) root         (0)      457 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/location_index/LocationIndexTuple.py
--rw-r--r--   0 root         (0) root         (0)     1195 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/location_index/LocationIndexUpdateDateTuple.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/location_index/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.195796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/
--rw-r--r--   0 root         (0) root         (0)     1060 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/WorkerEntryHook.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.195796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/api/
--rw-r--r--   0 root         (0) root         (0)     2685 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/api/WorkerApiImpl.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.196796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/
--rw-r--r--   0 root         (0) root         (0)    24739 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/DispCompilerTask.py
--rw-r--r--   0 root         (0) root         (0)     5724 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/GridCompilerTask.py
--rw-r--r--   0 root         (0) root         (0)     3940 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/ImportDispLink.py
--rw-r--r--   0 root         (0) root         (0)    18374 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/ImportDispTask.py
--rw-r--r--   0 root         (0) root         (0)     3027 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/LiveDbDisplayValueConverter.py
--rw-r--r--   0 root         (0) root         (0)     6263 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/LocationIndexCompilerTask.py
--rw-r--r--   0 root         (0) root         (0)     7595 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/LookupHashConverter.py
--rw-r--r--   0 root         (0) root         (0)     2178 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/_CalcDisp.py
--rw-r--r--   0 root         (0) root         (0)     4116 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/_CalcDispFromLiveDb.py
--rw-r--r--   0 root         (0) root         (0)     5700 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/_CalcGridForDisp.py
--rw-r--r--   0 root         (0) root         (0)     1618 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/_CalcLocation.py
--rw-r--r--   0 root         (0) root         (0)     3285 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/_ModelSetUtil.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.197796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/branch/
--rw-r--r--   0 root         (0) root         (0)     5167 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/branch/BranchDispUpdater.py
--rw-r--r--   0 root         (0) root         (0)     6272 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/branch/BranchIndexCompiler.py
--rw-r--r--   0 root         (0) root         (0)     5705 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/branch/BranchIndexImporter.py
--rw-r--r--   0 root         (0) root         (0)    12088 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/branch/BranchIndexUpdater.py
--rw-r--r--   0 root         (0) root         (0)      696 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/branch/_BranchIndexCalcChunkKey.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/branch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.198796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/
--rw-r--r--   0 root         (0) root         (0)     6206 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/admin_tasks.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.199796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/dev/
--rw-r--r--   0 root         (0) root         (0)     5682 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/dev/dev.rst
--rw-r--r--   0 root         (0) root         (0)    41043 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/dev/dev_with_diagram_data_backend.png
--rw-r--r--   0 root         (0) root         (0)   153459 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/dev/ns_integration.png
--rw-r--r--   0 root         (0) root         (0)    75576 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/dev/other_diagram_integration.png
--rw-r--r--   0 root         (0) root         (0)    75293 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/dev/structure_Initial_load.png
--rw-r--r--   0 root         (0) root         (0)    88309 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/dev/web_integration.png
--rw-r--r--   0 root         (0) root         (0)   125066 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/diagram_layers.jpg
--rw-r--r--   0 root         (0) root         (0)   423204 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/edit_zoom_limit.png
--rw-r--r--   0 root         (0) root         (0)   479535 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/enable_markup.png
--rw-r--r--   0 root         (0) root         (0)   163339 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/example_diagram.png
--rw-r--r--   0 root         (0) root         (0)      482 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/index.rst
--rw-r--r--   0 root         (0) root         (0)     6144 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/overview.rst
--rwxr-xr-x   0 root         (0) root         (0)    38273 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/plugin_diagram_edit_settings.png
--rwxr-xr-x   0 root         (0) root         (0)    34310 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/plugin_diagram_edit_settings_reset.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.199796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/setup/
--rw-r--r--   0 root         (0) root         (0)      367 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/setup/setup.rst
--rw-r--r--   0 root         (0) root         (0)     1197 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/setup/setup_coord_set.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.199796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/status/
--rw-r--r--   0 root         (0) root         (0)    36473 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/status/status.png
--rw-r--r--   0 root         (0) root         (0)      829 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/status/status.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.199796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/both-doc/
--rw-r--r--   0 root         (0) root         (0)       90 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/both-doc/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.200796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/
--rw-r--r--   0 root         (0) root         (0)      906 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/DiagramBranchService.ts
--rw-r--r--   0 root         (0) root         (0)      550 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/DiagramConfigService.ts
--rw-r--r--   0 root         (0) root         (0)      438 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/DiagramCoordSetService.ts
--rw-r--r--   0 root         (0) root         (0)      525 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/DiagramItemSelectService.ts
--rw-r--r--   0 root         (0) root         (0)     1626 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/DiagramLookupService.ts
--rw-r--r--   0 root         (0) root         (0)      545 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/DiagramOverrideService.ts
--rw-r--r--   0 root         (0) root         (0)     3642 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/DiagramPositionService.ts
--rw-r--r--   0 root         (0) root         (0)      382 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/DiagramSnapshotService.ts
--rw-r--r--   0 root         (0) root         (0)     2629 2022-11-14 05:34:34.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/DiagramToolbarService.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.200796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/
--rw-r--r--   0 root         (0) root         (0)     4269 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/PeekCanvasBounds.ts
--rw-r--r--   0 root         (0) root         (0)      702 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/PluginNames.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.200796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/admin/
--rw-r--r--   0 root         (0) root         (0)      571 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/admin/SettingPropertyTuple.ts
--rw-r--r--   0 root         (0) root         (0)       63 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/admin/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.201796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/branch/
--rw-r--r--   0 root         (0) root         (0)      559 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/branch/BranchKeyToIdMapTuple.ts
--rw-r--r--   0 root         (0) root         (0)     1220 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/branch/BranchLiveEditTuple.ts
--rw-r--r--   0 root         (0) root         (0)      812 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/branch/BranchLiveEditTupleAction.ts
--rw-r--r--   0 root         (0) root         (0)    21464 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/branch/BranchTuple.ts
--rw-r--r--   0 root         (0) root         (0)      639 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/branch/BranchUpdateTupleAction.ts
--rw-r--r--   0 root         (0) root         (0)     6196 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/branch/PrivateDiagramBranchContext.ts
--rw-r--r--   0 root         (0) root         (0)    10924 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/branch/PrivateDiagramBranchService.ts
--rw-r--r--   0 root         (0) root         (0)      199 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/branch/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.201796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/branch-loader/
--rw-r--r--   0 root         (0) root         (0)      439 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/branch-loader/BranchIndexEncodedChunkTuple.ts
--rw-r--r--   0 root         (0) root         (0)    20987 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/branch-loader/BranchIndexLoaderService.ts
--rw-r--r--   0 root         (0) root         (0)      726 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/branch-loader/BranchIndexLoaderServiceA.ts
--rw-r--r--   0 root         (0) root         (0)      533 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/branch-loader/BranchIndexLoaderStatusTuple.ts
--rw-r--r--   0 root         (0) root         (0)      597 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/branch-loader/BranchIndexUpdateDateTuple.ts
--rw-r--r--   0 root         (0) root         (0)     3349 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/branch-loader/LocalBranchStorageService.ts
--rw-r--r--   0 root         (0) root         (0)      407 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/branch-loader/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.201796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/grid-loader/
--rw-r--r--   0 root         (0) root         (0)      926 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/grid-loader/EncodedGridTuple.ts
--rw-r--r--   0 root         (0) root         (0)      425 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/grid-loader/GridTuple.ts
--rw-r--r--   0 root         (0) root         (0)      878 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/grid-loader/GridUpdateDateTuple.ts
--rw-r--r--   0 root         (0) root         (0)    18522 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/grid-loader/PrivateDiagramGridLoaderService.ts
--rw-r--r--   0 root         (0) root         (0)      837 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/grid-loader/PrivateDiagramGridLoaderServiceA.ts
--rw-r--r--   0 root         (0) root         (0)      554 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/grid-loader/PrivateDiagramGridLoaderStatusTuple.ts
--rw-r--r--   0 root         (0) root         (0)      250 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/grid-loader/index.ts
--rw-r--r--   0 root         (0) root         (0)      100 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.202796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/location-loader/
--rw-r--r--   0 root         (0) root         (0)      723 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/location-loader/DispKeyLocationTuple.ts
--rw-r--r--   0 root         (0) root         (0)      769 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/location-loader/EncodedLocationIndexTuple.ts
--rw-r--r--   0 root         (0) root         (0)      485 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/location-loader/LocationIndexTuple.ts
--rw-r--r--   0 root         (0) root         (0)      465 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/location-loader/LocationIndexUpdateDateTuple.ts
--rw-r--r--   0 root         (0) root         (0)    18208 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/location-loader/PrivateDiagramLocationLoaderService.ts
--rw-r--r--   0 root         (0) root         (0)      566 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/location-loader/PrivateDiagramLocationLoaderStatusTuple.ts
--rw-r--r--   0 root         (0) root         (0)      370 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/location-loader/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.203796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/services/
--rw-r--r--   0 root         (0) root         (0)     3889 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramConfigService.ts
--rw-r--r--   0 root         (0) root         (0)     5891 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramCoordSetService.ts
--rw-r--r--   0 root         (0) root         (0)      891 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramItemSelectService.ts
--rw-r--r--   0 root         (0) root         (0)    13430 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramLookupService.ts
--rw-r--r--   0 root         (0) root         (0)     6253 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramOfflineCacherService.ts
--rw-r--r--   0 root         (0) root         (0)     1739 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramOverrideService.ts
--rw-r--r--   0 root         (0) root         (0)     7833 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramPositionService.ts
--rw-r--r--   0 root         (0) root         (0)      887 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramSnapshotService.ts
--rw-r--r--   0 root         (0) root         (0)     3111 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramToolbarService.ts
--rw-r--r--   0 root         (0) root         (0)     2736 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramTupleService.ts
--rw-r--r--   0 root         (0) root         (0)      401 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/services/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.203796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      584 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/tuples/GroupDispsTuple.ts
--rw-r--r--   0 root         (0) root         (0)     3771 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/tuples/ModelCoordSet.ts
--rw-r--r--   0 root         (0) root         (0)      496 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/tuples/ModelCoordSetGridSize.ts
--rw-r--r--   0 root         (0) root         (0)      372 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/tuples/ModelSet.ts
--rw-r--r--   0 root         (0) root         (0)      207 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/tuples/index.ts
--rw-r--r--   0 root         (0) root         (0)      904 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.203796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/lookups/
--rw-r--r--   0 root         (0) root         (0)      472 2022-11-14 05:34:34.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/lookups/DispColor.ts
--rw-r--r--   0 root         (0) root         (0)      473 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/lookups/DispLayer.ts
--rw-r--r--   0 root         (0) root         (0)      580 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/lookups/DispLevel.ts
--rw-r--r--   0 root         (0) root         (0)      959 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/lookups/DispLineStyle.ts
--rw-r--r--   0 root         (0) root         (0)      599 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/lookups/DispTextStyle.ts
--rw-r--r--   0 root         (0) root         (0)      221 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/lookups/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.204796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/override/
--rw-r--r--   0 root         (0) root         (0)      910 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/override/DiagramOverrideBase.ts
--rw-r--r--   0 root         (0) root         (0)     1607 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/override/DiagramOverrideColor.ts
--rw-r--r--   0 root         (0) root         (0)     1177 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/override/DiagramOverrideHighlight.ts
--rw-r--r--   0 root         (0) root         (0)      135 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/override/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.204796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/tuples/
--rw-r--r--   0 root         (0) root         (0)      472 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/tuples/DiagramCoordSetTuple.ts
--rw-r--r--   0 root         (0) root         (0)    11231 2022-11-14 05:37:10.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin_package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.204796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/server/
--rw-r--r--   0 root         (0) root         (0)      589 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/server/DiagramApiABC.py
--rw-r--r--   0 root         (0) root         (0)     3252 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/server/DiagramImportApiABC.py
--rw-r--r--   0 root         (0) root         (0)      527 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/server/DiagramViewerApiABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.204796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/
--rw-r--r--   0 root         (0) root         (0)      553 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/ImportGroupHashTuple.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/ImportTypes.py
--rw-r--r--   0 root         (0) root         (0)      619 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.204796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/branches/
--rw-r--r--   0 root         (0) root         (0)      769 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/branches/ImportBranchDeltaColorOverride.py
--rw-r--r--   0 root         (0) root         (0)      476 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/branches/ImportBranchDeltaCreateDisp.py
--rw-r--r--   0 root         (0) root         (0)     1104 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/branches/ImportBranchTuple.py
--rw-r--r--   0 root         (0) root         (0)      180 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/branches/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.205796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/lookups/
--rw-r--r--   0 root         (0) root         (0)      894 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/lookups/ImportDispColorTuple.py
--rw-r--r--   0 root         (0) root         (0)      603 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/lookups/ImportDispLayerTuple.py
--rw-r--r--   0 root         (0) root         (0)      602 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/lookups/ImportDispLevelTuple.py
--rw-r--r--   0 root         (0) root         (0)     1243 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/lookups/ImportDispLineStyleTuple.py
--rw-r--r--   0 root         (0) root         (0)     1154 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/lookups/ImportDispTextStyleTuple.py
--rw-r--r--   0 root         (0) root         (0)      174 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/lookups/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.205796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/model/
--rw-r--r--   0 root         (0) root         (0)      500 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/model/DiagramCoordSetTuple.py
--rw-r--r--   0 root         (0) root         (0)     1880 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/model/ImportLiveDbDispLinkTuple.py
--rw-r--r--   0 root         (0) root         (0)      173 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.206796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/shapes/
--rw-r--r--   0 root         (0) root         (0)     4694 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/shapes/ImportDispCurvedTextTuple.py
--rw-r--r--   0 root         (0) root         (0)     3412 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/shapes/ImportDispEdgeTemplateTuple.py
--rw-r--r--   0 root         (0) root         (0)     3818 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/shapes/ImportDispEllipseTuple.py
--rw-r--r--   0 root         (0) root         (0)     4218 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/shapes/ImportDispGroupPtrTuple.py
--rw-r--r--   0 root         (0) root         (0)     2836 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/shapes/ImportDispGroupTuple.py
--rw-r--r--   0 root         (0) root         (0)     3983 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/shapes/ImportDispPolygonTuple.py
--rw-r--r--   0 root         (0) root         (0)     4455 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/shapes/ImportDispPolylineTuple.py
--rw-r--r--   0 root         (0) root         (0)     4279 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/shapes/ImportDispTextTuple.py
--rw-r--r--   0 root         (0) root         (0)      173 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/shapes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.206796 peek-plugin-diagram-3.3.3/peek_plugin_diagram/worker/
--rw-r--r--   0 root         (0) root         (0)     1955 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/worker/WorkerApi.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:29.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram/worker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:37:11.176796 peek-plugin-diagram-3.3.3/peek_plugin_diagram.egg-info/
--rw-r--r--   0 root         (0) root         (0)      400 2022-11-14 05:37:10.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    31749 2022-11-14 05:37:11.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-14 05:37:10.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-14 05:37:10.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2022-11-14 05:37:10.000000 peek-plugin-diagram-3.3.3/peek_plugin_diagram.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-14 05:37:11.206796 peek-plugin-diagram-3.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2733 2022-11-14 05:37:10.000000 peek-plugin-diagram-3.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.436202 peek-plugin-diagram-3.4.0/
+-rw-r--r--   0 root         (0) root         (0)      400 2023-04-12 11:05:55.436202 peek-plugin-diagram-3.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      580 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.410202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/
+-rw-r--r--   0 root         (0) root         (0)     1155 2023-04-12 11:05:55.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.411202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/
+-rw-r--r--   0 root         (0) root         (0)     2226 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/GridKeyIndexTest.py
+-rw-r--r--   0 root         (0) root         (0)      334 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/PluginNames.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.411202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/admin-app/
+-rw-r--r--   0 root         (0) root         (0)     2563 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/admin-app/diagram.component.html
+-rw-r--r--   0 root         (0) root         (0)      212 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/admin-app/diagram.component.ts
+-rw-r--r--   0 root         (0) root         (0)     2288 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/admin-app/diagram.module.web.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.411202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/admin-app/edit-setting-table/
+-rw-r--r--   0 root         (0) root         (0)     2595 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/admin-app/edit-setting-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     1469 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/admin-app/edit-setting-table/edit.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.411202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/admin-app/status/
+-rw-r--r--   0 root         (0) root         (0)     2125 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/admin-app/status/status.component.html
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/admin-app/status/status.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.411202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/admin-app/tuples/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/admin-app/tuples/DiagramImporterStatusTuple.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.411202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/agent/
+-rw-r--r--   0 root         (0) root         (0)      668 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/agent/AgentEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.411202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      325 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.414202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     1453 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/0ad02369aaea_use_darkcolor_lightcolor.py
+-rw-r--r--   0 root         (0) root         (0)     2809 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/0db3aedfee95_added_column_showforedit.py
+-rw-r--r--   0 root         (0) root         (0)     1089 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/128b23798db0_add_text_border_for_curved_text.py
+-rw-r--r--   0 root         (0) root         (0)     1057 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/1856b7fb8803_added_linetemplatesenabled.py
+-rw-r--r--   0 root         (0) root         (0)     3292 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/1b17ef0cca17_removed_string_field_sizes.py
+-rw-r--r--   0 root         (0) root         (0)      861 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/1fe753e1f369_disptext_textstyleid_not_null.py
+-rw-r--r--   0 root         (0) root         (0)     1599 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/2127d894e46b_moved_smallest_sizes_to_grids.py
+-rw-r--r--   0 root         (0) root         (0)     4444 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/23117803d414_added_location_index.py
+-rw-r--r--   0 root         (0) root         (0)     1432 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/24b83c5e7e31_renamed_location_indexes.py
+-rw-r--r--   0 root         (0) root         (0)      941 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/298b291aac2d_encoded_grids_are_now_gridtuples.py
+-rw-r--r--   0 root         (0) root         (0)     1612 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/2c5f47322bda_removed_node_and_conn.py
+-rw-r--r--   0 root         (0) root         (0)     1225 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/2fc6d3246717_added_compiler_q_indexes.py
+-rw-r--r--   0 root         (0) root         (0)      741 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/34dd05f474df_rebuild_location_index.py
+-rw-r--r--   0 root         (0) root         (0)     1061 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/361988cd327d_added_createddate_to_branchindex.py
+-rw-r--r--   0 root         (0) root         (0)     1300 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/3b41dec74e46_added_overlay_flag.py
+-rw-r--r--   0 root         (0) root         (0)      794 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/42a8dc25e588_add_disp_action.py
+-rw-r--r--   0 root         (0) root         (0)     1601 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/473d5f6a97e8_removed_more_string_sizes.py
+-rw-r--r--   0 root         (0) root         (0)      923 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/47879bec4c5f_added_texthstretch.py
+-rw-r--r--   0 root         (0) root         (0)      663 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/4925c894757b_enabled_nulls_for_text.py
+-rw-r--r--   0 root         (0) root         (0)     2239 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/4b943b584307_added_coordset_mx_c.py
+-rw-r--r--   0 root         (0) root         (0)     1963 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/4f6ed1047562_added_branch_fields_to_dispbase.py
+-rw-r--r--   0 root         (0) root         (0)     1151 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/5307eb21c742_added_spacingbetweentexts_in_textstyle.py
+-rw-r--r--   0 root         (0) root         (0)     1366 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/558bc7fc4d36_added_polyline_startkey_endkey.py
+-rw-r--r--   0 root         (0) root         (0)      541 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/57e88ad9d5cb_add_dispbase_key_index.py
+-rw-r--r--   0 root         (0) root         (0)     2225 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/5e2f84d757f2_added_cascade_constraints.py
+-rw-r--r--   0 root         (0) root         (0)      815 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/6a71c73c0606_added_polygon_isrectangle.py
+-rw-r--r--   0 root         (0) root         (0)     4052 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/6a97dd344aed_added_coordset_gridsizes.py
+-rw-r--r--   0 root         (0) root         (0)      950 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/6d3a96cf1955_added_dispnull.py
+-rw-r--r--   0 root         (0) root         (0)      839 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/6f545d4166dc_remove_unique_constraint_for_dispgroup.py
+-rw-r--r--   0 root         (0) root         (0)    30200 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/7eed363f5df5_initial.py
+-rw-r--r--   0 root         (0) root         (0)     6602 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/81c1d2809046_added_coordset_editable_fields.py
+-rw-r--r--   0 root         (0) root         (0)      637 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/8b8ebbe5ec7b_added_scalable_to_lookup_linestyle.py
+-rw-r--r--   0 root         (0) root         (0)     2055 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/8ef78f862ac8_updates_for_dispgroup.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/97990b4ca6a1_added_landingcoordsetid.py
+-rw-r--r--   0 root         (0) root         (0)     3102 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/9e7ca1acd6be_fixed_importhash_indexes_for_lookups.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      677 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/a151fd42572b_added_wrap_text_at_chars.py
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/a4c59bcaaf88_added_curved_text_disp.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/a66e033b8227_updated_float_precision_in_zoom_levels.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/a73574690197_coordset_positiononzoom.py
+-rw-r--r--   0 root         (0) root         (0)     1839 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/a86e0317e22a_added_poly_template_name.py
+-rw-r--r--   0 root         (0) root         (0)     3382 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/aa76b059b81e_added_default_group_ptr_to_coord_set.py
+-rw-r--r--   0 root         (0) root         (0)     2076 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/bf8f559c4df9_removed_branchgridindex.py
+-rw-r--r--   0 root         (0) root         (0)      779 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/bfdd4f46e293_added_coordset_key.py
+-rw-r--r--   0 root         (0) root         (0)      773 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/c88ba8f6761f_added_disp_zorder.py
+-rw-r--r--   0 root         (0) root         (0)      953 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/cbd5e370686f_increased_size_of_disp_json.py
+-rw-r--r--   0 root         (0) root         (0)      657 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/cea17a52b9ae_timezone_aware.py
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/d103b9c1eba9_added_disp_data.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/d6e25d8ba156_added_textheight_to_disptext.py
+-rw-r--r--   0 root         (0) root         (0)     3887 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/da424430bf97_added_edgecolor_removed_lu_indexes.py
+-rw-r--r--   0 root         (0) root         (0)     1323 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/e3c2c2580dea_add_text_border_color_and_width.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/e8d6d02c0922_added_polyline_start_end_types.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/e9d80c4c087d_increased_size_of_importgrouphash.py
+-rw-r--r--   0 root         (0) root         (0)     1569 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/ec97d31aebb0_added_line_templates.py
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/f4dce3e782ec_added_coordset_dispgroup_enabled.py
+-rw-r--r--   0 root         (0) root         (0)     3351 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/f697025b2013_updated_to_bigintegers.py
+-rw-r--r--   0 root         (0) root         (0)     4968 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/f76791d27f6d_added_branch_tables.py
+-rw-r--r--   0 root         (0) root         (0)       94 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.414202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/
+-rw-r--r--   0 root         (0) root         (0)     3262 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/DiagramUtil.ts
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.415202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/branch-detail-component/
+-rw-r--r--   0 root         (0) root         (0)     3124 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/branch-detail-component/branch-detail.component.web.html
+-rw-r--r--   0 root         (0) root         (0)      255 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/branch-detail-component/branch-detail.component.web.scss
+-rw-r--r--   0 root         (0) root         (0)     7472 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/branch-detail-component/branch-detail.component.web.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.415202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/cache/
+-rw-r--r--   0 root         (0) root         (0)     7743 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/cache/GridCache.web.ts
+-rw-r--r--   0 root         (0) root         (0)     4154 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/cache/GridObservable.web.ts
+-rw-r--r--   0 root         (0) root         (0)     2498 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/cache/LinkedGrid.web.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.416202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas/
+-rw-r--r--   0 root         (0) root         (0)     2375 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasActioner.ts
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasBounds.ts
+-rw-r--r--   0 root         (0) root         (0)     6166 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasConfig.web.ts
+-rw-r--r--   0 root         (0) root         (0)     1281 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasEdgeTemplatePropsContext.ts
+-rw-r--r--   0 root         (0) root         (0)     8148 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasEditor.web.ts
+-rw-r--r--   0 root         (0) root         (0)     8888 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasEditorProps.ts
+-rw-r--r--   0 root         (0) root         (0)      308 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasEditorToolType.web.ts
+-rw-r--r--   0 root         (0) root         (0)     2361 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasExtensions.web.ts
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasGroupPtrPropsContext.ts
+-rw-r--r--   0 root         (0) root         (0)    17844 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasModel.web.ts
+-rw-r--r--   0 root         (0) root         (0)     8528 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasModelQuery.web.ts
+-rw-r--r--   0 root         (0) root         (0)     2489 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasModelSelection.web.ts
+-rw-r--r--   0 root         (0) root         (0)      913 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasModelUtil.web.ts
+-rw-r--r--   0 root         (0) root         (0)     3998 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasShapePropsContext.ts
+-rw-r--r--   0 root         (0) root         (0)      142 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas/PeekInterfaces.web.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.416202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-component/
+-rw-r--r--   0 root         (0) root         (0)     2546 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-component/canvas-component.web.html
+-rw-r--r--   0 root         (0) root         (0)      305 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-component/canvas-component.web.scss
+-rw-r--r--   0 root         (0) root         (0)    15170 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-component/canvas-component.web.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.416202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-context-menu-component/
+-rw-r--r--   0 root         (0) root         (0)      901 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-context-menu-component/canvas-context-menu.component.web.html
+-rw-r--r--   0 root         (0) root         (0)      535 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-context-menu-component/canvas-context-menu.component.web.scss
+-rw-r--r--   0 root         (0) root         (0)     2600 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-context-menu-component/canvas-context-menu.component.web.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.417202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-input/
+-rw-r--r--   0 root         (0) root         (0)     9680 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInput.web.ts
+-rw-r--r--   0 root         (0) root         (0)     4295 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputDelegate.web.ts
+-rw-r--r--   0 root         (0) root         (0)     1942 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputDelegateUtil.web.ts
+-rw-r--r--   0 root         (0) root         (0)     5068 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputEditMakeEllipseDelegate.web.ts
+-rw-r--r--   0 root         (0) root         (0)     3718 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputEditMakeGroupPtrVertexDelegate.web.ts
+-rw-r--r--   0 root         (0) root         (0)      967 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputEditMakeLineWithArrowDelegate.web.ts
+-rw-r--r--   0 root         (0) root         (0)     9118 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputEditMakePolyDelegate.web.ts
+-rw-r--r--   0 root         (0) root         (0)      955 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputEditMakePolygonDelegate.web.ts
+-rw-r--r--   0 root         (0) root         (0)     1023 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputEditMakePolylineDelegate.web.ts
+-rw-r--r--   0 root         (0) root         (0)     5090 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputEditMakeRectangleDelegate.web.ts
+-rw-r--r--   0 root         (0) root         (0)     4347 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputEditMakeTextDelegate.web.ts
+-rw-r--r--   0 root         (0) root         (0)    27281 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputEditSelectDelegate.web.ts
+-rw-r--r--   0 root         (0) root         (0)     1550 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputMakeDispPolylineEdgeDelegate.web.ts
+-rw-r--r--   0 root         (0) root         (0)    15557 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputSelectDelegate.web.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.417202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-override/
+-rw-r--r--   0 root         (0) root         (0)      896 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-override/PeekCanvasModelOverrideA.ts
+-rw-r--r--   0 root         (0) root         (0)     2889 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-override/PeekCanvasModelOverrideColor.ts
+-rw-r--r--   0 root         (0) root         (0)     4234 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-override/PeekCanvasModelOverrideHighlight.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.417202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-render/
+-rw-r--r--   0 root         (0) root         (0)     8778 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-render/PeekCanvasRenderer.web.ts
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-render/PeekDispRenderDelegateABC.web.ts
+-rw-r--r--   0 root         (0) root         (0)    24259 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-render/PeekDispRenderDelegateCurvedText.web.ts
+-rw-r--r--   0 root         (0) root         (0)     4017 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-render/PeekDispRenderDelegateEllipse.web.ts
+-rw-r--r--   0 root         (0) root         (0)     4785 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-render/PeekDispRenderDelegateGroupPtr.web.ts
+-rw-r--r--   0 root         (0) root         (0)     1144 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-render/PeekDispRenderDelegateNull.web.ts
+-rw-r--r--   0 root         (0) root         (0)    13360 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-render/PeekDispRenderDelegatePoly.web.ts
+-rw-r--r--   0 root         (0) root         (0)     8292 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-render/PeekDispRenderDelegateText.web.ts
+-rw-r--r--   0 root         (0) root         (0)       83 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-render/PeekDispRenderDrawModeE.web.ts
+-rw-r--r--   0 root         (0) root         (0)     4792 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-render/PeekDispRenderFactory.web.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.418202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-shapes/
+-rw-r--r--   0 root         (0) root         (0)    11855 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-shapes/DispBase.ts
+-rw-r--r--   0 root         (0) root         (0)     6400 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-shapes/DispCurvedText.ts
+-rw-r--r--   0 root         (0) root         (0)     1468 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-shapes/DispEdgeTemplate.ts
+-rw-r--r--   0 root         (0) root         (0)     6870 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-shapes/DispEllipse.ts
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-shapes/DispFactory.ts
+-rw-r--r--   0 root         (0) root         (0)      208 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-shapes/DispFactoryTypeMap.ts
+-rw-r--r--   0 root         (0) root         (0)     1994 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-shapes/DispGroup.ts
+-rw-r--r--   0 root         (0) root         (0)     8296 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-shapes/DispGroupPointer.ts
+-rw-r--r--   0 root         (0) root         (0)     1687 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-shapes/DispNull.ts
+-rw-r--r--   0 root         (0) root         (0)     3687 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-shapes/DispPoly.ts
+-rw-r--r--   0 root         (0) root         (0)     8208 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-shapes/DispPolygon.ts
+-rw-r--r--   0 root         (0) root         (0)    13443 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-shapes/DispPolyline.ts
+-rw-r--r--   0 root         (0) root         (0)     1909 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-shapes/DispRectangle.ts
+-rw-r--r--   0 root         (0) root         (0)     5830 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-shapes/DispText.ts
+-rw-r--r--   0 root         (0) root         (0)     1371 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-shapes/DispUtil.ts
+-rw-r--r--   0 root         (0) root         (0)     3427 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-shapes/DispUtilRotate.ts
+-rw-r--r--   0 root         (0) root         (0)     1792 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/diagram.component.ts
+-rw-r--r--   0 root         (0) root         (0)      105 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/diagram.component.web.html
+-rw-r--r--   0 root         (0) root         (0)       54 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/diagram.component.web.scss
+-rw-r--r--   0 root         (0) root         (0)      817 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/diagram.component.web.ts
+-rw-r--r--   0 root         (0) root         (0)     4466 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/diagram.module.web.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.418202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-component/
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-component/edit-props.component.web.html
+-rw-r--r--   0 root         (0) root         (0)     1710 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-component/edit-props.component.web.scss
+-rw-r--r--   0 root         (0) root         (0)     3245 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-component/edit-props.component.web.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.419202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-edge-template-component/
+-rw-r--r--   0 root         (0) root         (0)     1618 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-edge-template-component/edit-props-edge-template.component.html
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-edge-template-component/edit-props-edge-template.component.scss
+-rw-r--r--   0 root         (0) root         (0)     7356 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-edge-template-component/edit-props-edge-template.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.419202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-group-ptr-component/
+-rw-r--r--   0 root         (0) root         (0)     1603 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-group-ptr-component/edit-props-group-ptr.component.html
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-group-ptr-component/edit-props-group-ptr.component.scss
+-rw-r--r--   0 root         (0) root         (0)     7126 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-group-ptr-component/edit-props-group-ptr.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.419202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-livedb-component/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-livedb-component/edit-props-livedb.component.html
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-livedb-component/edit-props-livedb.component.scss
+-rw-r--r--   0 root         (0) root         (0)      516 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-livedb-component/edit-props-livedb.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.419202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-shape-component/
+-rw-r--r--   0 root         (0) root         (0)     4391 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-shape-component/edit-props-shape.component.html
+-rw-r--r--   0 root         (0) root         (0)       36 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-shape-component/edit-props-shape.component.scss
+-rw-r--r--   0 root         (0) root         (0)     6181 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-shape-component/edit-props-shape.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.419202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-toolbar-component/
+-rw-r--r--   0 root         (0) root         (0)     1975 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-toolbar-component/edit-props-toolbar.component.web.html
+-rw-r--r--   0 root         (0) root         (0)     1484 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-toolbar-component/edit-props-toolbar.component.web.scss
+-rw-r--r--   0 root         (0) root         (0)     2777 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-toolbar-component/edit-props-toolbar.component.web.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.419202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-toolbar-component/
+-rw-r--r--   0 root         (0) root         (0)     9120 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-toolbar-component/edit-toolbar.component.web.html
+-rw-r--r--   0 root         (0) root         (0)     1996 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-toolbar-component/edit-toolbar.component.web.scss
+-rw-r--r--   0 root         (0) root         (0)     8761 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-toolbar-component/edit-toolbar.component.web.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.420202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/print-component/
+-rw-r--r--   0 root         (0) root         (0)      401 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/print-component/print.component.web.html
+-rw-r--r--   0 root         (0) root         (0)      535 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/print-component/print.component.web.scss
+-rw-r--r--   0 root         (0) root         (0)     1348 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/print-component/print.component.web.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.420202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/services/
+-rw-r--r--   0 root         (0) root         (0)      561 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/services/canvas.service.ts
+-rw-r--r--   0 root         (0) root         (0)      702 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/services/context-menu.service.ts
+-rw-r--r--   0 root         (0) root         (0)     3905 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/services/copy-paste.service.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.420202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/set-position-component/
+-rw-r--r--   0 root         (0) root         (0)      388 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/set-position-component/set-position.component.html
+-rw-r--r--   0 root         (0) root         (0)       30 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/set-position-component/set-position.component.scss
+-rw-r--r--   0 root         (0) root         (0)     9027 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/set-position-component/set-position.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.420202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/start-edit-component/
+-rw-r--r--   0 root         (0) root         (0)     4142 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/start-edit-component/start-edit.component.web.html
+-rw-r--r--   0 root         (0) root         (0)      801 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/start-edit-component/start-edit.component.web.scss
+-rw-r--r--   0 root         (0) root         (0)     7149 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/start-edit-component/start-edit.component.web.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.420202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/view-select-branches-component/
+-rw-r--r--   0 root         (0) root         (0)     2583 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/view-select-branches-component/select-branches.component.web.html
+-rw-r--r--   0 root         (0) root         (0)      762 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/view-select-branches-component/select-branches.component.web.scss
+-rw-r--r--   0 root         (0) root         (0)     7765 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/view-select-branches-component/select-branches.component.web.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.420202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/view-select-layers-component/
+-rw-r--r--   0 root         (0) root         (0)     1084 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/view-select-layers-component/select-layers.component.web.html
+-rw-r--r--   0 root         (0) root         (0)      559 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/view-select-layers-component/select-layers.component.web.scss
+-rw-r--r--   0 root         (0) root         (0)     3812 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/view-select-layers-component/select-layers.component.web.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.420202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/view-toolbar-component/
+-rw-r--r--   0 root         (0) root         (0)     4434 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/view-toolbar-component/toolbar.component.web.html
+-rw-r--r--   0 root         (0) root         (0)     1348 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/view-toolbar-component/toolbar.component.web.scss
+-rw-r--r--   0 root         (0) root         (0)     7950 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/view-toolbar-component/toolbar.component.web.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.421202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-assets/
+-rw-r--r--   0 root         (0) root         (0)    12054 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-assets/icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.421202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/
+-rw-r--r--   0 root         (0) root         (0)     9541 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/ClientEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)     5994 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/TupleDataObservable.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.422202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/controller/
+-rw-r--r--   0 root         (0) root         (0)     1311 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/controller/BranchIndexCacheController.py
+-rw-r--r--   0 root         (0) root         (0)     2254 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/controller/CoordSetCacheController.py
+-rw-r--r--   0 root         (0) root         (0)     2623 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/controller/GridCacheController.py
+-rw-r--r--   0 root         (0) root         (0)     1390 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/controller/LocationIndexCacheController.py
+-rw-r--r--   0 root         (0) root         (0)     4899 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/controller/LookupCacheController.py
+-rw-r--r--   0 root         (0) root         (0)     2020 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/controller/ModelSetCacheController.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/controller/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.422202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/handlers/
+-rw-r--r--   0 root         (0) root         (0)     1108 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/handlers/BranchIndexCacheHandler.py
+-rw-r--r--   0 root         (0) root         (0)     9562 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/handlers/GridCacheHandler.py
+-rw-r--r--   0 root         (0) root         (0)     1138 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/handlers/LocationIndexCacheHandler.py
+-rw-r--r--   0 root         (0) root         (0)      176 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/handlers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.422202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/tuple_providers/
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/tuple_providers/BranchIndexUpdateDateTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     2817 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/tuple_providers/BranchTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)      843 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/tuple_providers/ClientCoordSetTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     3918 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/tuple_providers/ClientDispKeyLocationTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/tuple_providers/ClientGroupDispsTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/tuple_providers/ClientLocationIndexUpdateDateTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)      971 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/tuple_providers/ClientLookupTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)      841 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/tuple_providers/ClientModelSetTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/tuple_providers/GridCacheIndexTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/tuple_providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.423202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/
+-rw-r--r--   0 root         (0) root         (0)    12532 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/LogicEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/TupleActionProcessor.py
+-rw-r--r--   0 root         (0) root         (0)     4028 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/TupleDataObservable.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.423202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/admin_handlers/
+-rw-r--r--   0 root         (0) root         (0)      983 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/admin_handlers/SettingPropertyHandler.py
+-rw-r--r--   0 root         (0) root         (0)     1667 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/admin_handlers/StringIntTableHandler.py
+-rw-r--r--   0 root         (0) root         (0)      446 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/admin_handlers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.423202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/api/
+-rw-r--r--   0 root         (0) root         (0)     1766 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/api/DiagramApi.py
+-rw-r--r--   0 root         (0) root         (0)     3036 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/api/DiagramImportApi.py
+-rw-r--r--   0 root         (0) root         (0)     1111 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/api/DiagramViewerApi.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.423202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/client_handlers/
+-rw-r--r--   0 root         (0) root         (0)     2054 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/client_handlers/BranchIndexChunkLoadRpc.py
+-rw-r--r--   0 root         (0) root         (0)      808 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/client_handlers/BranchIndexChunkUpdateHandler.py
+-rw-r--r--   0 root         (0) root         (0)     2866 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/client_handlers/ClientGridLoaderRpc.py
+-rw-r--r--   0 root         (0) root         (0)      757 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/client_handlers/ClientGridUpdateHandler.py
+-rw-r--r--   0 root         (0) root         (0)     2620 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/client_handlers/ClientLocationIndexLoaderRpc.py
+-rw-r--r--   0 root         (0) root         (0)     1435 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/client_handlers/ClientLocationIndexUpdateHandler.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/client_handlers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.424202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/controller/
+-rw-r--r--   0 root         (0) root         (0)     4106 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/controller/BranchIndexCompilerQueueController.py
+-rw-r--r--   0 root         (0) root         (0)     4131 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/controller/BranchLiveEditController.py
+-rw-r--r--   0 root         (0) root         (0)     4789 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/controller/BranchUpdateController.py
+-rw-r--r--   0 root         (0) root         (0)     5206 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/controller/DispCompilerQueueController.py
+-rw-r--r--   0 root         (0) root         (0)     3933 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/controller/DispImportController.py
+-rw-r--r--   0 root         (0) root         (0)     3754 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/controller/GridKeyCompilerQueueController.py
+-rw-r--r--   0 root         (0) root         (0)     2683 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/controller/LiveDbWatchController.py
+-rw-r--r--   0 root         (0) root         (0)     4214 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/controller/LocationCompilerQueueController.py
+-rw-r--r--   0 root         (0) root         (0)     8074 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/controller/LookupImportController.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/controller/StatusController.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/controller/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.424202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/tuple_providers/
+-rw-r--r--   0 root         (0) root         (0)     1614 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/tuple_providers/BranchKeyToIdMapProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/tuple_providers/BranchLiveEditTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)      925 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/tuple_providers/DiagramLoaderStatusTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1267 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/tuple_providers/ServerCoordSetTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1708 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/tuple_providers/ServerLookupTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)      945 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/tuple_providers/ServerModelSetTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/tuple_providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.425202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/storage/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/storage/DeclarativeBase.py
+-rw-r--r--   0 root         (0) root         (0)      928 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/storage/DispIndex.py
+-rw-r--r--   0 root         (0) root         (0)    19919 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/storage/Display.py
+-rw-r--r--   0 root         (0) root         (0)     4505 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/storage/GridKeyIndex.py
+-rw-r--r--   0 root         (0) root         (0)     3172 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/storage/LiveDbDispLink.py
+-rw-r--r--   0 root         (0) root         (0)     4389 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/storage/LocationIndex.py
+-rw-r--r--   0 root         (0) root         (0)    12908 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/storage/Lookups.py
+-rw-r--r--   0 root         (0) root         (0)    10047 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/storage/ModelSet.py
+-rw-r--r--   0 root         (0) root         (0)     7986 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/storage/Setting.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.425202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/storage/branch/
+-rw-r--r--   0 root         (0) root         (0)     2211 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/storage/branch/BranchIndex.py
+-rw-r--r--   0 root         (0) root         (0)     1368 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/storage/branch/BranchIndexCompilerQueue.py
+-rw-r--r--   0 root         (0) root         (0)     2412 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/storage/branch/BranchIndexEncodedChunk.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/storage/branch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.425202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/DiagramImporterStatusTuple.py
+-rw-r--r--   0 root         (0) root         (0)      563 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/GroupDispsTuple.py
+-rw-r--r--   0 root         (0) root         (0)      875 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.425202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/branch/
+-rw-r--r--   0 root         (0) root         (0)     1283 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/branch/BranchIndexUpdateDateTuple.py
+-rw-r--r--   0 root         (0) root         (0)      542 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/branch/BranchKeyToIdMapTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/branch/BranchLiveEditTuple.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/branch/BranchLiveEditTupleAction.py
+-rw-r--r--   0 root         (0) root         (0)     4565 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/branch/BranchTuple.py
+-rw-r--r--   0 root         (0) root         (0)      585 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/branch/BranchUpdateTupleAction.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/branch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.426202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/grid/
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/grid/EncodedGridTuple.py
+-rw-r--r--   0 root         (0) root         (0)      817 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/grid/GridTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/grid/GridUpdateDateTuple.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/grid/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.426202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/location_index/
+-rw-r--r--   0 root         (0) root         (0)      893 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/location_index/DispKeyLocationTuple.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/location_index/EncodedLocationIndexTuple.py
+-rw-r--r--   0 root         (0) root         (0)      457 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/location_index/LocationIndexTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/location_index/LocationIndexUpdateDateTuple.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/location_index/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.426202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/
+-rw-r--r--   0 root         (0) root         (0)     1176 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/WorkerEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.426202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/api/
+-rw-r--r--   0 root         (0) root         (0)     2685 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/api/WorkerApiImpl.py
+-rw-r--r--   0 root         (0) root         (0)    20656 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/api/WorkerDiagramGridApiImpl.py
+-rw-r--r--   0 root         (0) root         (0)    15302 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/api/WorkerDiagramGridApiImplTest.py
+-rw-r--r--   0 root         (0) root         (0)     1061 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/api/WorkerDiagramGridApiImpl_SQLPrints.py
+-rw-r--r--   0 root         (0) root         (0)     2431 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/api/WorkerDiagramLookupApiImpl.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.427202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/
+-rw-r--r--   0 root         (0) root         (0)    25104 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/DispCompilerTask.py
+-rw-r--r--   0 root         (0) root         (0)     6054 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/GridCompilerTask.py
+-rw-r--r--   0 root         (0) root         (0)     3940 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/ImportDispLink.py
+-rw-r--r--   0 root         (0) root         (0)    18374 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/ImportDispTask.py
+-rw-r--r--   0 root         (0) root         (0)     3027 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/LiveDbDisplayValueConverter.py
+-rw-r--r--   0 root         (0) root         (0)     6560 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/LocationIndexCompilerTask.py
+-rw-r--r--   0 root         (0) root         (0)     7592 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/LookupHashConverter.py
+-rw-r--r--   0 root         (0) root         (0)     2178 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/_CalcDisp.py
+-rw-r--r--   0 root         (0) root         (0)     4116 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/_CalcDispFromLiveDb.py
+-rw-r--r--   0 root         (0) root         (0)     5862 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/_CalcGridForDisp.py
+-rw-r--r--   0 root         (0) root         (0)     1618 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/_CalcLocation.py
+-rw-r--r--   0 root         (0) root         (0)     3285 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/_ModelSetUtil.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.427202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/branch/
+-rw-r--r--   0 root         (0) root         (0)     5167 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/branch/BranchDispUpdater.py
+-rw-r--r--   0 root         (0) root         (0)     6709 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/branch/BranchIndexCompilerTask.py
+-rw-r--r--   0 root         (0) root         (0)     5802 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/branch/BranchIndexImporterTask.py
+-rw-r--r--   0 root         (0) root         (0)    12088 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/branch/BranchIndexUpdaterTask.py
+-rw-r--r--   0 root         (0) root         (0)      696 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/branch/_BranchIndexCalcChunkKey.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/branch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.427202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/utils/
+-rw-r--r--   0 root         (0) root         (0)     5211 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/utils/ShapeLookupLinker.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.428202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/
+-rw-r--r--   0 root         (0) root         (0)     6702 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/admin_tasks.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.429202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/dev/
+-rw-r--r--   0 root         (0) root         (0)     5682 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/dev/dev.rst
+-rw-r--r--   0 root         (0) root         (0)    41043 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/dev/dev_with_diagram_data_backend.png
+-rw-r--r--   0 root         (0) root         (0)   153459 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/dev/ns_integration.png
+-rw-r--r--   0 root         (0) root         (0)    75576 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/dev/other_diagram_integration.png
+-rw-r--r--   0 root         (0) root         (0)    75293 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/dev/structure_Initial_load.png
+-rw-r--r--   0 root         (0) root         (0)    88309 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/dev/web_integration.png
+-rw-r--r--   0 root         (0) root         (0)   125066 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/diagram_layers.jpg
+-rw-r--r--   0 root         (0) root         (0)   423204 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/edit_zoom_limit.png
+-rw-r--r--   0 root         (0) root         (0)   479535 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/enable_markup.png
+-rw-r--r--   0 root         (0) root         (0)   163339 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/example_diagram.png
+-rw-r--r--   0 root         (0) root         (0)      482 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/index.rst
+-rw-r--r--   0 root         (0) root         (0)     6144 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/overview.rst
+-rwxr-xr-x   0 root         (0) root         (0)    38273 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/plugin_diagram_edit_settings.png
+-rwxr-xr-x   0 root         (0) root         (0)    34310 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/plugin_diagram_edit_settings_reset.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.429202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/setup/
+-rw-r--r--   0 root         (0) root         (0)      367 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/setup/setup.rst
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/setup/setup_coord_set.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.429202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/status/
+-rw-r--r--   0 root         (0) root         (0)    36473 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/status/status.png
+-rw-r--r--   0 root         (0) root         (0)      829 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/status/status.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.429202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/both-doc/
+-rw-r--r--   0 root         (0) root         (0)       90 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/both-doc/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.430202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/
+-rw-r--r--   0 root         (0) root         (0)      963 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/DiagramBranchService.ts
+-rw-r--r--   0 root         (0) root         (0)      598 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/DiagramConfigService.ts
+-rw-r--r--   0 root         (0) root         (0)      438 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/DiagramCoordSetService.ts
+-rw-r--r--   0 root         (0) root         (0)      525 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/DiagramItemSelectService.ts
+-rw-r--r--   0 root         (0) root         (0)     2159 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/DiagramLookupService.ts
+-rw-r--r--   0 root         (0) root         (0)      545 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/DiagramOverrideService.ts
+-rw-r--r--   0 root         (0) root         (0)     4276 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/DiagramPositionService.ts
+-rw-r--r--   0 root         (0) root         (0)      382 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/DiagramSnapshotService.ts
+-rw-r--r--   0 root         (0) root         (0)     2662 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/DiagramToolbarService.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.430202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/
+-rw-r--r--   0 root         (0) root         (0)     4269 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/PeekCanvasBounds.ts
+-rw-r--r--   0 root         (0) root         (0)      702 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/PluginNames.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.430202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/admin/
+-rw-r--r--   0 root         (0) root         (0)      571 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/admin/SettingPropertyTuple.ts
+-rw-r--r--   0 root         (0) root         (0)       63 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/admin/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.431202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/branch/
+-rw-r--r--   0 root         (0) root         (0)      559 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/branch/BranchKeyToIdMapTuple.ts
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/branch/BranchLiveEditTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      812 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/branch/BranchLiveEditTupleAction.ts
+-rw-r--r--   0 root         (0) root         (0)    21464 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/branch/BranchTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      639 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/branch/BranchUpdateTupleAction.ts
+-rw-r--r--   0 root         (0) root         (0)     6196 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/branch/PrivateDiagramBranchContext.ts
+-rw-r--r--   0 root         (0) root         (0)    11024 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/branch/PrivateDiagramBranchService.ts
+-rw-r--r--   0 root         (0) root         (0)      199 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/branch/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.431202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/branch-loader/
+-rw-r--r--   0 root         (0) root         (0)      439 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/branch-loader/BranchIndexEncodedChunkTuple.ts
+-rw-r--r--   0 root         (0) root         (0)    20671 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/branch-loader/BranchIndexLoaderService.ts
+-rw-r--r--   0 root         (0) root         (0)      721 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/branch-loader/BranchIndexLoaderServiceA.ts
+-rw-r--r--   0 root         (0) root         (0)      597 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/branch-loader/BranchIndexUpdateDateTuple.ts
+-rw-r--r--   0 root         (0) root         (0)     3349 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/branch-loader/LocalBranchStorageService.ts
+-rw-r--r--   0 root         (0) root         (0)      328 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/branch-loader/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.431202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/grid-loader/
+-rw-r--r--   0 root         (0) root         (0)      926 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/grid-loader/EncodedGridTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      425 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/grid-loader/GridTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      878 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/grid-loader/GridUpdateDateTuple.ts
+-rw-r--r--   0 root         (0) root         (0)    18486 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/grid-loader/PrivateDiagramGridLoaderService.ts
+-rw-r--r--   0 root         (0) root         (0)      804 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/grid-loader/PrivateDiagramGridLoaderServiceA.ts
+-rw-r--r--   0 root         (0) root         (0)      157 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/grid-loader/index.ts
+-rw-r--r--   0 root         (0) root         (0)      100 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.431202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/location-loader/
+-rw-r--r--   0 root         (0) root         (0)      723 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/location-loader/DispKeyLocationTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      769 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/location-loader/EncodedLocationIndexTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      485 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/location-loader/LocationIndexTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      465 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/location-loader/LocationIndexUpdateDateTuple.ts
+-rw-r--r--   0 root         (0) root         (0)    18147 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/location-loader/PrivateDiagramLocationLoaderService.ts
+-rw-r--r--   0 root         (0) root         (0)      269 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/location-loader/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.432202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/lookups/
+-rw-r--r--   0 root         (0) root         (0)     1199 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/lookups/DispColor.ts
+-rw-r--r--   0 root         (0) root         (0)     1001 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/lookups/DispLayer.ts
+-rw-r--r--   0 root         (0) root         (0)     1200 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/lookups/DispLevel.ts
+-rw-r--r--   0 root         (0) root         (0)     1783 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/lookups/DispLineStyle.ts
+-rw-r--r--   0 root         (0) root         (0)     1427 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/lookups/DispTextStyle.ts
+-rw-r--r--   0 root         (0) root         (0)      221 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/lookups/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.432202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/services/
+-rw-r--r--   0 root         (0) root         (0)     4037 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramConfigService.ts
+-rw-r--r--   0 root         (0) root         (0)     5891 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramCoordSetService.ts
+-rw-r--r--   0 root         (0) root         (0)      891 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramItemSelectService.ts
+-rw-r--r--   0 root         (0) root         (0)    13729 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramLookupService.ts
+-rw-r--r--   0 root         (0) root         (0)     6250 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramOfflineCacherService.ts
+-rw-r--r--   0 root         (0) root         (0)     1739 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramOverrideService.ts
+-rw-r--r--   0 root         (0) root         (0)     8341 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramPositionService.ts
+-rw-r--r--   0 root         (0) root         (0)      887 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramSnapshotService.ts
+-rw-r--r--   0 root         (0) root         (0)     3111 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramToolbarService.ts
+-rw-r--r--   0 root         (0) root         (0)     2736 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramTupleService.ts
+-rw-r--r--   0 root         (0) root         (0)      401 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/services/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.433202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      584 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/tuples/GroupDispsTuple.ts
+-rw-r--r--   0 root         (0) root         (0)     3771 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/tuples/ModelCoordSet.ts
+-rw-r--r--   0 root         (0) root         (0)      496 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/tuples/ModelCoordSetGridSize.ts
+-rw-r--r--   0 root         (0) root         (0)      372 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/tuples/ModelSet.ts
+-rw-r--r--   0 root         (0) root         (0)      207 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/tuples/index.ts
+-rw-r--r--   0 root         (0) root         (0)      904 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.433202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/lookup_tuples/
+-rw-r--r--   0 root         (0) root         (0)      636 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/lookup_tuples/ShapeColorTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      493 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/lookup_tuples/ShapeLayerTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      625 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/lookup_tuples/ShapeLevelTuple.ts
+-rw-r--r--   0 root         (0) root         (0)     1029 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/lookup_tuples/ShapeLineStyleTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      657 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/lookup_tuples/ShapeTextStyleTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      281 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/lookup_tuples/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.433202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/override/
+-rw-r--r--   0 root         (0) root         (0)      910 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/override/DiagramOverrideBase.ts
+-rw-r--r--   0 root         (0) root         (0)     1696 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/override/DiagramOverrideColor.ts
+-rw-r--r--   0 root         (0) root         (0)     1186 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/override/DiagramOverrideHighlight.ts
+-rw-r--r--   0 root         (0) root         (0)      135 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/override/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.433202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/tuples/
+-rw-r--r--   0 root         (0) root         (0)      472 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/tuples/DiagramCoordSetTuple.ts
+-rw-r--r--   0 root         (0) root         (0)    11000 2023-04-12 11:05:55.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin_package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.433202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/server/
+-rw-r--r--   0 root         (0) root         (0)      589 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/server/DiagramApiABC.py
+-rw-r--r--   0 root         (0) root         (0)     3252 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/server/DiagramImportApiABC.py
+-rw-r--r--   0 root         (0) root         (0)      527 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/server/DiagramViewerApiABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.434202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/
+-rw-r--r--   0 root         (0) root         (0)     5557 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/ColorUtil.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/ColorUtilTest.py
+-rw-r--r--   0 root         (0) root         (0)      553 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/ImportGroupHashTuple.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/ImportTypes.py
+-rw-r--r--   0 root         (0) root         (0)      680 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.434202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/branches/
+-rw-r--r--   0 root         (0) root         (0)      769 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/branches/ImportBranchDeltaColorOverride.py
+-rw-r--r--   0 root         (0) root         (0)      476 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/branches/ImportBranchDeltaCreateDisp.py
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/branches/ImportBranchTuple.py
+-rw-r--r--   0 root         (0) root         (0)      180 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/branches/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.434202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/grids/
+-rw-r--r--   0 root         (0) root         (0)      838 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/grids/DecodedCompiledGridTuple.py
+-rw-r--r--   0 root         (0) root         (0)      731 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/grids/GridKeyTuple.py
+-rw-r--r--   0 root         (0) root         (0)      172 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/grids/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.434202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/lookup_tuples/
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/lookup_tuples/ShapeColorTuple.py
+-rw-r--r--   0 root         (0) root         (0)      806 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/lookup_tuples/ShapeLayerTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1201 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/lookup_tuples/ShapeLevelTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/lookup_tuples/ShapeLineStyleTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1411 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/lookup_tuples/ShapeTextStyleTuple.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/lookup_tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.435202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/lookups/
+-rw-r--r--   0 root         (0) root         (0)      894 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/lookups/ImportDispColorTuple.py
+-rw-r--r--   0 root         (0) root         (0)      603 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/lookups/ImportDispLayerTuple.py
+-rw-r--r--   0 root         (0) root         (0)      602 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/lookups/ImportDispLevelTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1243 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/lookups/ImportDispLineStyleTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1212 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/lookups/ImportDispTextStyleTuple.py
+-rw-r--r--   0 root         (0) root         (0)      174 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/lookups/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.435202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/model/
+-rw-r--r--   0 root         (0) root         (0)      500 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/model/DiagramCoordSetTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1880 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/model/ImportLiveDbDispLinkTuple.py
+-rw-r--r--   0 root         (0) root         (0)      173 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.435202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/shapes/
+-rw-r--r--   0 root         (0) root         (0)     4694 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/shapes/ImportDispCurvedTextTuple.py
+-rw-r--r--   0 root         (0) root         (0)     3412 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/shapes/ImportDispEdgeTemplateTuple.py
+-rw-r--r--   0 root         (0) root         (0)     3818 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/shapes/ImportDispEllipseTuple.py
+-rw-r--r--   0 root         (0) root         (0)     4218 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/shapes/ImportDispGroupPtrTuple.py
+-rw-r--r--   0 root         (0) root         (0)     2836 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/shapes/ImportDispGroupTuple.py
+-rw-r--r--   0 root         (0) root         (0)     3983 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/shapes/ImportDispPolygonTuple.py
+-rw-r--r--   0 root         (0) root         (0)     4455 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/shapes/ImportDispPolylineTuple.py
+-rw-r--r--   0 root         (0) root         (0)     4279 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/shapes/ImportDispTextTuple.py
+-rw-r--r--   0 root         (0) root         (0)      173 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/shapes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.436202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/worker/
+-rw-r--r--   0 root         (0) root         (0)     1955 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/worker/WorkerApi.py
+-rw-r--r--   0 root         (0) root         (0)     3176 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/worker/WorkerDiagramGridApi.py
+-rw-r--r--   0 root         (0) root         (0)      774 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/worker/WorkerDiagramLookupApi.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/worker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.436202 peek-plugin-diagram-3.4.0/peek_plugin_diagram/worker/canvas_shapes/
+-rw-r--r--   0 root         (0) root         (0)     3636 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/worker/canvas_shapes/ShapeBase.py
+-rw-r--r--   0 root         (0) root         (0)     2335 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/worker/canvas_shapes/ShapeCurvedText.py
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/worker/canvas_shapes/ShapeEllipse.py
+-rw-r--r--   0 root         (0) root         (0)      362 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/worker/canvas_shapes/ShapeGroup.py
+-rw-r--r--   0 root         (0) root         (0)     1354 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/worker/canvas_shapes/ShapeGroupPointer.py
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/worker/canvas_shapes/ShapeNull.py
+-rw-r--r--   0 root         (0) root         (0)     1035 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/worker/canvas_shapes/ShapePoly.py
+-rw-r--r--   0 root         (0) root         (0)     1784 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/worker/canvas_shapes/ShapePolyLine.py
+-rw-r--r--   0 root         (0) root         (0)     2039 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/worker/canvas_shapes/ShapePolygon.py
+-rw-r--r--   0 root         (0) root         (0)     2163 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/worker/canvas_shapes/ShapeText.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:20.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram/worker/canvas_shapes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:55.410202 peek-plugin-diagram-3.4.0/peek_plugin_diagram.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      400 2023-04-12 11:05:55.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    33846 2023-04-12 11:05:55.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 11:05:55.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       81 2023-04-12 11:05:55.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-04-12 11:05:55.000000 peek-plugin-diagram-3.4.0/peek_plugin_diagram.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 11:05:55.437202 peek-plugin-diagram-3.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2853 2023-04-12 11:05:55.000000 peek-plugin-diagram-3.4.0/setup.py
```

### Comparing `peek-plugin-diagram-3.3.3/README.rst` & `peek-plugin-diagram-3.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/__init__.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Type
 
 from peek_plugin_base.agent.PluginAgentEntryHookABC import PluginAgentEntryHookABC
 from peek_plugin_base.client.PluginClientEntryHookABC import PluginClientEntryHookABC
 from peek_plugin_base.server.PluginLogicEntryHookABC import PluginLogicEntryHookABC
 from peek_plugin_base.worker.PluginWorkerEntryHookABC import PluginWorkerEntryHookABC
 
-__version__ = '3.3.3'
+__version__ = '3.4.0'
 
 
 def peekLogicEntryHook() -> Type[PluginLogicEntryHookABC]:
     from ._private.server.LogicEntryHook import LogicEntryHook
 
     return LogicEntryHook
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/GridKeyIndexTest.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/GridKeyIndexTest.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/admin-app/diagram.component.html` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/admin-app/diagram.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/admin-app/diagram.module.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/admin-app/diagram.module.web.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/admin-app/edit-setting-table/edit.component.html` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/admin-app/edit-setting-table/edit.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/admin-app/edit-setting-table/edit.component.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/admin-app/edit-setting-table/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/admin-app/status/status.component.html` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/admin-app/status/status.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/admin-app/status/status.component.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/admin-app/status/status.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/admin-app/tuples/DiagramImporterStatusTuple.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/admin-app/tuples/DiagramImporterStatusTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/agent/AgentEntryHook.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/agent/AgentEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/script.py.mako` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/script.py.mako`

 * *Files 4% similar despite different names*

```diff
@@ -16,12 +16,12 @@
 
 from alembic import op
 import sqlalchemy as sa
 import geoalchemy2
 ${imports if imports else ""}
 
 def upgrade():
-${upgrades if upgrades else "pass"}
+    ${upgrades if upgrades else "pass"}
 
 
 def downgrade():
-${downgrades if downgrades else "pass"}
+    ${downgrades if downgrades else "pass"}
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/0db3aedfee95_added_column_showforedit.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/0db3aedfee95_added_column_showforedit.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/128b23798db0_add_text_border_for_curved_text.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/128b23798db0_add_text_border_for_curved_text.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/1856b7fb8803_added_linetemplatesenabled.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/1856b7fb8803_added_linetemplatesenabled.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/1b17ef0cca17_removed_string_field_sizes.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/1b17ef0cca17_removed_string_field_sizes.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/1fe753e1f369_disptext_textstyleid_not_null.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/1fe753e1f369_disptext_textstyleid_not_null.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/2127d894e46b_moved_smallest_sizes_to_grids.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/2127d894e46b_moved_smallest_sizes_to_grids.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/23117803d414_added_location_index.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/23117803d414_added_location_index.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/24b83c5e7e31_renamed_location_indexes.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/24b83c5e7e31_renamed_location_indexes.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/298b291aac2d_encoded_grids_are_now_gridtuples.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/298b291aac2d_encoded_grids_are_now_gridtuples.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/2c5f47322bda_removed_node_and_conn.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/2c5f47322bda_removed_node_and_conn.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/2fc6d3246717_added_compiler_q_indexes.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/2fc6d3246717_added_compiler_q_indexes.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/34dd05f474df_rebuild_location_index.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/34dd05f474df_rebuild_location_index.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/361988cd327d_added_createddate_to_branchindex.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/361988cd327d_added_createddate_to_branchindex.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/3b41dec74e46_added_overlay_flag.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/3b41dec74e46_added_overlay_flag.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/42a8dc25e588_add_disp_action.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/42a8dc25e588_add_disp_action.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/473d5f6a97e8_removed_more_string_sizes.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/473d5f6a97e8_removed_more_string_sizes.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/47879bec4c5f_added_texthstretch.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/47879bec4c5f_added_texthstretch.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/4925c894757b_enabled_nulls_for_text.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/4925c894757b_enabled_nulls_for_text.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/4b943b584307_added_coordset_mx_c.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/4b943b584307_added_coordset_mx_c.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/4f6ed1047562_added_branch_fields_to_dispbase.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/4f6ed1047562_added_branch_fields_to_dispbase.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/5307eb21c742_added_spacingbetweentexts_in_textstyle.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/5307eb21c742_added_spacingbetweentexts_in_textstyle.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/558bc7fc4d36_added_polyline_startkey_endkey.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/558bc7fc4d36_added_polyline_startkey_endkey.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/5e2f84d757f2_added_cascade_constraints.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/5e2f84d757f2_added_cascade_constraints.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/6a71c73c0606_added_polygon_isrectangle.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/6a71c73c0606_added_polygon_isrectangle.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/6a97dd344aed_added_coordset_gridsizes.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/6a97dd344aed_added_coordset_gridsizes.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/6d3a96cf1955_added_dispnull.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/6d3a96cf1955_added_dispnull.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/6f545d4166dc_remove_unique_constraint_for_dispgroup.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/6f545d4166dc_remove_unique_constraint_for_dispgroup.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/7eed363f5df5_initial.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/7eed363f5df5_initial.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/81c1d2809046_added_coordset_editable_fields.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/81c1d2809046_added_coordset_editable_fields.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/8b8ebbe5ec7b_added_scalable_to_lookup_linestyle.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/8b8ebbe5ec7b_added_scalable_to_lookup_linestyle.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/8ef78f862ac8_updates_for_dispgroup.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/8ef78f862ac8_updates_for_dispgroup.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/97990b4ca6a1_added_landingcoordsetid.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/97990b4ca6a1_added_landingcoordsetid.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/9e7ca1acd6be_fixed_importhash_indexes_for_lookups.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/9e7ca1acd6be_fixed_importhash_indexes_for_lookups.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/a4c59bcaaf88_added_curved_text_disp.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/a4c59bcaaf88_added_curved_text_disp.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/a66e033b8227_updated_float_precision_in_zoom_levels.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/a66e033b8227_updated_float_precision_in_zoom_levels.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/a73574690197_coordset_positiononzoom.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/a73574690197_coordset_positiononzoom.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/a86e0317e22a_added_poly_template_name.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/a86e0317e22a_added_poly_template_name.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/aa76b059b81e_added_default_group_ptr_to_coord_set.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/aa76b059b81e_added_default_group_ptr_to_coord_set.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/bf8f559c4df9_removed_branchgridindex.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/bf8f559c4df9_removed_branchgridindex.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/bfdd4f46e293_added_coordset_key.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/bfdd4f46e293_added_coordset_key.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/c88ba8f6761f_added_disp_zorder.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/c88ba8f6761f_added_disp_zorder.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/cbd5e370686f_increased_size_of_disp_json.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/cbd5e370686f_increased_size_of_disp_json.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/cea17a52b9ae_timezone_aware.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/cea17a52b9ae_timezone_aware.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/d103b9c1eba9_added_disp_data.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/d103b9c1eba9_added_disp_data.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/d6e25d8ba156_added_textheight_to_disptext.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/d6e25d8ba156_added_textheight_to_disptext.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/da424430bf97_added_edgecolor_removed_lu_indexes.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/da424430bf97_added_edgecolor_removed_lu_indexes.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/e3c2c2580dea_add_text_border_color_and_width.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/e3c2c2580dea_add_text_border_color_and_width.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/e8d6d02c0922_added_polyline_start_end_types.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/e8d6d02c0922_added_polyline_start_end_types.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/e9d80c4c087d_increased_size_of_importgrouphash.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/e9d80c4c087d_increased_size_of_importgrouphash.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/ec97d31aebb0_added_line_templates.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/ec97d31aebb0_added_line_templates.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/f4dce3e782ec_added_coordset_dispgroup_enabled.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/f4dce3e782ec_added_coordset_dispgroup_enabled.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/f697025b2013_updated_to_bigintegers.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/f697025b2013_updated_to_bigintegers.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/alembic/versions/f76791d27f6d_added_branch_tables.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/alembic/versions/f76791d27f6d_added_branch_tables.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/DiagramUtil.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/DiagramUtil.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/branch-detail-component/branch-detail.component.web.html` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/branch-detail-component/branch-detail.component.web.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/branch-detail-component/branch-detail.component.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/branch-detail-component/branch-detail.component.web.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/cache/GridCache.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/cache/GridCache.web.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/cache/GridObservable.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/cache/GridObservable.web.ts`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     private rebuildReverseLookup() {
         let newDict = {};
 
         // Iterate through the canvasIds
         for (let canvasId of dictKeysFromObject(this.gridKeysByCanvasId)) {
             let gridKeys = this.gridKeysByCanvasId[canvasId];
 
-            // Iterate through the gridKeys
+            // Iterate through the gridKeyTuples
             for (let gridKey of gridKeys) {
                 // Get the existing array or create one
                 let array: any[] = null;
                 if (newDict.hasOwnProperty(gridKey)) {
                     array = newDict[gridKey];
                 } else {
                     newDict[gridKey] = array = [];
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/cache/LinkedGrid.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/cache/LinkedGrid.web.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasActioner.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasActioner.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasConfig.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasConfig.web.ts`

 * *Files 17% similar despite different names*

```diff
@@ -9,28 +9,30 @@
  * Peek Canvas Data
  *
  * This class is responsible for storing all the data required for the canvas.
  * This includes storing referecnes to Model objects, and settings for this canvas
  */
 export class PeekCanvasConfig {
     private static canvasIdCounter = 0;
+    private static whiteBackground = "#ffffff";
+    private static blackBackground = "#000000";
 
     canvasId: number;
 
     controller = {
         updateInterval: 400,
         coordSetChange: new Subject<ModelCoordSet>(),
         coordSet: null,
         modelSetKey: "",
     };
 
     renderer = {
         invalidate: new Subject<void>(), // Set this to true to cause the renderer to redraw
         drawInterval: 60,
-        backgroundColor: "#000000",
+        backgroundColor: PeekCanvasConfig.blackBackground,
         useEdgeColors: false,
         selection: {
             color: "white",
             width: 8,
             lineGap: 6,
             dashLen: 3,
         },
@@ -123,14 +125,29 @@
     // Debug data
     debug = {};
 
     constructor() {
         this.canvasId = PeekCanvasConfig.canvasIdCounter++;
     }
 
+    get isLightMode(): boolean {
+        return this.renderer.backgroundColor ===
+            PeekCanvasConfig.whiteBackground
+            ? true
+            : false;
+    }
+
+    set isLightMode(value: boolean) {
+        value === true
+            ? (this.renderer.backgroundColor = PeekCanvasConfig.whiteBackground)
+            : (this.renderer.backgroundColor =
+                  PeekCanvasConfig.blackBackground);
+        this.invalidate();
+    }
+
     get coordSet(): ModelCoordSet | null {
         return this.controller.coordSet;
     }
 
     getSelectionDrawDetailsForDrawMode(drawMode: DrawModeE) {
         switch (drawMode) {
             case DrawModeE.ForView:
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasEdgeTemplatePropsContext.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasEdgeTemplatePropsContext.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasEditor.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasEditor.web.ts`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import { BalloonMsgService } from "@synerty/peek-plugin-base-js";
 import { PeekCanvasInput } from "../canvas-input/PeekCanvasInput.web";
 import { PeekCanvasInputEditSelectDelegate } from "../canvas-input/PeekCanvasInputEditSelectDelegate.web";
 import { PeekCanvasInputSelectDelegate } from "../canvas-input/PeekCanvasInputSelectDelegate.web";
 import { PeekCanvasModel } from "./PeekCanvasModel.web";
 import { PeekCanvasConfig } from "./PeekCanvasConfig.web";
 import { EditorToolType } from "./PeekCanvasEditorToolType.web";
-import { DispLevel } from "@peek/peek_plugin_diagram/lookups";
+import { DispLevel } from "@peek/peek_plugin_diagram/_private/lookups";
 import { PeekCanvasEditorProps } from "./PeekCanvasEditorProps";
 import { GridObservable } from "../cache/GridObservable.web";
 
 /**
  * Peek Canvas Editor
  *
  * This class is the central controller for Edit support.
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasEditorProps.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasEditorProps.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasExtensions.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasExtensions.web.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasGroupPtrPropsContext.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasGroupPtrPropsContext.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasModel.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasModel.web.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasModelQuery.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasModelQuery.web.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasModelSelection.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasModelSelection.web.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasModelUtil.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasModelUtil.web.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasShapePropsContext.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas/PeekCanvasShapePropsContext.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-component/canvas-component.web.html` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-component/canvas-component.web.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-component/canvas-component.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-component/canvas-component.web.ts`

 * *Files 2% similar despite different names*

```diff
@@ -7,28 +7,31 @@
 import { PeekCanvasInput } from "../canvas-input/PeekCanvasInput.web";
 import { PeekCanvasModel } from "../canvas/PeekCanvasModel.web";
 import { GridObservable } from "../cache/GridObservable.web";
 import { PrivateDiagramLookupService } from "@peek/peek_plugin_diagram/_private/services/PrivateDiagramLookupService";
 import { PrivateDiagramConfigService } from "@peek/peek_plugin_diagram/_private/services/PrivateDiagramConfigService";
 import { DispBase, DispBaseT } from "../canvas-shapes/DispBase";
 import { PeekCanvasBounds } from "../canvas/PeekCanvasBounds";
-import { PositionUpdatedI } from "@peek/peek_plugin_diagram/DiagramPositionService";
+import {
+    CoordSetViewWindowI,
+    PositionUpdatedI,
+} from "@peek/peek_plugin_diagram/DiagramPositionService";
 import { DocDbPopupService } from "@peek/peek_core_docdb";
 import { PrivateDiagramPositionService } from "@peek/peek_plugin_diagram/_private/services/PrivateDiagramPositionService";
 import { PrivateDiagramItemSelectService } from "@peek/peek_plugin_diagram/_private/services/PrivateDiagramItemSelectService";
 import { PrivateDiagramCoordSetService } from "@peek/peek_plugin_diagram/_private/services/PrivateDiagramCoordSetService";
 import { PeekCanvasEditor } from "../canvas/PeekCanvasEditor.web";
 import { BalloonMsgService } from "@synerty/peek-plugin-base-js";
 import { PrivateDiagramBranchService } from "@peek/peek_plugin_diagram/_private/branch/PrivateDiagramBranchService";
 import { PrivateDiagramSnapshotService } from "@peek/peek_plugin_diagram/_private/services/PrivateDiagramSnapshotService";
 import { PrivateDiagramOverrideService } from "@peek/peek_plugin_diagram/_private/services/PrivateDiagramOverrideService";
 import { PeekCanvasActioner } from "../canvas/PeekCanvasActioner";
 import { CopyPasteService } from "../services/copy-paste.service";
 import { ContextMenuService } from "../services/context-menu.service";
-import { DiagramToolbarService } from "@peek/peek_plugin_diagram";
+import { DiagramToolbarService } from "@peek/peek_plugin_diagram/DiagramToolbarService";
 import { PrivateDiagramToolbarService } from "@peek/peek_plugin_diagram/_private/services";
 import { DiagramToolbarBuiltinButtonEnum } from "@peek/peek_plugin_diagram/DiagramToolbarService";
 import { CanvasService } from "../services/canvas.service";
 
 /** Canvas Component
  *
  * This component ties in all the plain canvas TypeScript code with the Angular
@@ -49,15 +52,16 @@
 
     buttonBitmask: DiagramToolbarBuiltinButtonEnum =
         // show all default buttons by default
         DiagramToolbarBuiltinButtonEnum.BUTTON_CHANGE_COORDSET_MENU +
         DiagramToolbarBuiltinButtonEnum.BUTTOON_PRINT_DIAGRAM +
         DiagramToolbarBuiltinButtonEnum.BUTTON_EDIT_DIAGRAM +
         DiagramToolbarBuiltinButtonEnum.BUTTON_SELECT_BRANCHES +
-        DiagramToolbarBuiltinButtonEnum.BUTTON_SELECT_LAYERS;
+        DiagramToolbarBuiltinButtonEnum.BUTTON_SELECT_LAYERS +
+        DiagramToolbarBuiltinButtonEnum.BUTTON_COLOR_MODES;
 
     config: PeekCanvasConfig;
     model: PeekCanvasModel;
     input: PeekCanvasInput;
     editor: PeekCanvasEditor;
     // This is toggled by the toolbars
     showPrintPopup = false;
@@ -230,23 +234,35 @@
         let notify = () => {
             if (this.config.controller.coordSet == null) return;
 
             let editingBranch = null;
             if (this.config.editor.active)
                 editingBranch = this.editor.branchContext.branchTuple.key;
 
-            let data: PositionUpdatedI = {
+            const positionUpdatedData: PositionUpdatedI = {
                 coordSetKey: this.config.controller.coordSet.key,
                 x: this.config.viewPort.pan.x,
                 y: this.config.viewPort.pan.y,
                 zoom: this.config.viewPort.zoom,
                 editingBranch: editingBranch,
             };
 
-            this.privatePosService.positionUpdated(data);
+            const coordSetViewData: CoordSetViewWindowI = {
+                modelSetKey: this.config.controller.modelSetKey,
+                coordSetKey: this.config.controller.coordSet.key,
+                x: this.config.viewPort.window.x,
+                y: this.config.viewPort.window.y,
+                width: this.config.viewPort.window.w,
+                height: this.config.viewPort.window.h,
+            };
+
+            this.privatePosService.positionUpdated(
+                positionUpdatedData,
+                coordSetViewData
+            );
         };
 
         this.config.viewPort.panChange
             .pipe(takeUntil(this.onDestroyEvent))
             .subscribe(notify);
 
         this.config.viewPort.zoomChange
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-context-menu-component/canvas-context-menu.component.web.html` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-context-menu-component/canvas-context-menu.component.web.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-context-menu-component/canvas-context-menu.component.web.scss` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-context-menu-component/canvas-context-menu.component.web.scss`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-context-menu-component/canvas-context-menu.component.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-context-menu-component/canvas-context-menu.component.web.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInput.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInput.web.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputDelegate.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputDelegate.web.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputDelegateUtil.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputDelegateUtil.web.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputEditMakeEllipseDelegate.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputEditMakeEllipseDelegate.web.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputEditMakeGroupPtrVertexDelegate.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputEditMakeGroupPtrVertexDelegate.web.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputEditMakeLineWithArrowDelegate.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputEditMakeLineWithArrowDelegate.web.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputEditMakePolyDelegate.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputEditMakePolyDelegate.web.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputEditMakePolygonDelegate.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputEditMakePolygonDelegate.web.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputEditMakePolylineDelegate.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputEditMakePolylineDelegate.web.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputEditMakeRectangleDelegate.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputEditMakeRectangleDelegate.web.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputEditMakeTextDelegate.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputEditMakeTextDelegate.web.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputEditSelectDelegate.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputEditSelectDelegate.web.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputMakeDispPolylineEdgeDelegate.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputMakeDispPolylineEdgeDelegate.web.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputSelectDelegate.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-input/PeekCanvasInputSelectDelegate.web.ts`

 * *Files 4% similar despite different names*

```diff
@@ -99,23 +99,25 @@
     // fixes a problem where double clicking causes
     // text to get selected on the canvas
     // mouseSelectStart (event,
     // mouse) {
     // }
 
     touchStart(event: TouchEvent, mouse) {
+        this.clearPopupTimeout();
         if (event.targetTouches.length == 2) {
             this._state = this.STATE_CANVAS_ZOOMING;
             this._lastPinchDist = null;
         } else {
             this.mouseDown(event, mouse);
         }
     }
 
     mouseDown(event, mouse: CanvasInputPos) {
+        this.clearPopupTimeout();
         this.suggestedDispToSelect = null;
         this._mouseDownWithShift = event.shiftKey;
         this._mouseDownWithCtrl = event.ctrlKey;
         this._mouseDownMiddleButton = event.button == 1;
         this._mouseDownRightButton = event.button == 2;
         this._startMousePos = mouse;
         this._lastMousePos = mouse;
@@ -195,14 +197,16 @@
         this._zoomPan(center.clientX, center.clientY, delta);
     }
 
     _zoomPan(clientX, clientY, delta) {
         if (!delta) {
             return;
         }
+        this.clearPopupTimeout();
+        this.clearSelectableUnderMouse();
 
         // Correct the zooming to match google maps, etc
         delta = delta * -1;
 
         // begin
         let zoom = this.viewArgs.config.viewPort.zoom;
         let pan = this.viewArgs.config.viewPort.pan;
@@ -425,62 +429,80 @@
         mouse: MouseEvent
     ): void {
         const query = this.viewArgs.model.query;
 
         const hits = this.getUnderMouseHits(inputPos);
 
         if (!hits.length) {
-            clearTimeout(this.popupTimeout);
+            this.clearPopupTimeout();
             this.viewArgs.objectPopupService.hideHoverPopup();
             this.clearSelectableUnderMouse();
             return;
         }
 
         // Don't highlight already selected disps
         for (const selDisp of query.selectedDisps) {
             if (DispBase.id(selDisp) == DispBase.id(hits[0])) {
                 this.clearSelectableUnderMouse();
                 return;
             }
         }
-
-        if (!this.popupOpened) {
-            clearTimeout(this.popupTimeout);
-            this.popupTimeout = setTimeout(() => {
-                if (DispBase.key(newHit)) {
-                    this.popupOpened = true;
-                    this.viewArgs.objectPopupService.showPopup(
-                        false,
-                        DocDbPopupTypeE.tooltipPopup,
-                        diagramPluginName,
-                        mouse,
-                        this.viewArgs.config.controller.modelSetKey,
-                        DispBase.key(newHit),
-                        {
-                            triggeredForContext:
-                                this.viewArgs.config.coordSet.key,
-                        }
-                    );
-                }
-            }, 125);
-        }
-
         const newHit = hits[0];
+        this.popupTooltip(newHit, mouse);
 
         if (
             this.suggestedDispToSelect != null &&
             DispBase.id(newHit) == DispBase.id(this.suggestedDispToSelect)
         ) {
             return;
         }
 
         this.popupOpened = false;
         this.clearSelectableUnderMouse();
         this.suggestedDispToSelect = newHit;
         this.viewArgs.config.invalidate();
     }
 
+    private popupTooltip(newHit, mouse: MouseEvent) {
+        if (this.popupOpened) {
+            return;
+        }
+
+        if (DispBase.key(newHit) == null) {
+            return;
+        }
+
+        this.clearPopupTimeout();
+        this.popupTimeout = setTimeout(() => {
+            if (this.popupTimeout == null) {
+                return;
+            }
+
+            this.popupOpened = true;
+
+            this.viewArgs.objectPopupService.showPopup(
+                false,
+                DocDbPopupTypeE.tooltipPopup,
+                diagramPluginName,
+                mouse,
+                this.viewArgs.config.controller.modelSetKey,
+                DispBase.key(newHit),
+                {
+                    triggeredForContext: this.viewArgs.config.coordSet.key,
+                }
+            );
+        }, 250);
+    }
+
+    private clearPopupTimeout(): void {
+        if (this.popupTimeout != null) {
+            clearTimeout(this.popupTimeout);
+        }
+        this.popupTimeout = null;
+        this.viewArgs.objectPopupService.hideHoverPopup();
+    }
+
     private clearSelectableUnderMouse(): void {
         this.suggestedDispToSelect = null;
         this.viewArgs.config.invalidate();
     }
 }
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-override/PeekCanvasModelOverrideA.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-override/PeekCanvasModelOverrideA.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-override/PeekCanvasModelOverrideColor.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-override/PeekCanvasModelOverrideColor.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-override/PeekCanvasModelOverrideHighlight.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-override/PeekCanvasModelOverrideHighlight.ts`

 * *Files 1% similar despite different names*

```diff
@@ -111,12 +111,12 @@
         const twiceOffset = 2 * offset;
         const x = bounds.x - offset;
         const y = bounds.y - offset;
         const w = bounds.w + twiceOffset;
         const h = bounds.h + twiceOffset;
 
         ctx.dashedRect(x, y, w, h, selectionConfig.dashLen / zoom);
-        ctx.strokeStyle = override.color.color;
+        ctx.strokeStyle = override.color.getColor(this.config.isLightMode);
         ctx.lineWidth = selectionConfig.width / zoom;
         ctx.stroke();
     }
 }
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-render/PeekCanvasRenderer.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-render/PeekCanvasRenderer.web.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-render/PeekDispRenderDelegateABC.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-render/PeekDispRenderDelegateABC.web.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-render/PeekDispRenderDelegateCurvedText.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-render/PeekDispRenderDelegateCurvedText.web.ts`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,18 @@
     CurvedTextVerticalAlign,
     DispCurvedText,
 } from "../canvas-shapes/DispCurvedText";
 import { pointToPixel } from "../DiagramUtil";
 import { PeekCanvasBounds } from "../canvas/PeekCanvasBounds";
 import { DispBaseT, PointI } from "../canvas-shapes/DispBase";
 import { PeekCanvasModel } from "../canvas/PeekCanvasModel.web";
-import { DispColor, DispTextStyle } from "@peek/peek_plugin_diagram/lookups";
+import {
+    DispColor,
+    DispTextStyle,
+} from "@peek/peek_plugin_diagram/_private/lookups";
 import { DispPolygon } from "../canvas-shapes/DispPolygon";
 
 interface SubPathIndexRange {
     isReversed: boolean;
     rightExclusiveBoundaryIndex: number;
 }
 
@@ -120,16 +123,22 @@
         updateBounds: boolean
     ) {
         let textStyle = DispCurvedText.textStyle(disp);
         let fillColor = DispCurvedText.color(disp);
         let borderColor = DispCurvedText.borderColor(disp);
 
         // Null colors are also not drawn
-        fillColor = fillColor && fillColor.color ? fillColor : null;
-        borderColor = borderColor && borderColor.color ? borderColor : null;
+        fillColor =
+            fillColor && fillColor.getColor(this.config.isLightMode)
+                ? fillColor
+                : null;
+        borderColor =
+            borderColor && borderColor.getColor(this.config.isLightMode)
+                ? borderColor
+                : null;
 
         // TODO, Draw a box around the text, based on line style
 
         let horizontalStretchFactor = DispCurvedText.horizontalStretch(disp);
         let textHeight = DispCurvedText.height(disp);
 
         let fontSize = textStyle.fontSize * textStyle.scaleFactor;
@@ -603,15 +612,17 @@
                     ctx.translate(
                         curvedTextPathDrawingContext.nextPoint.location.x,
                         curvedTextPathDrawingContext.nextPoint.location.y
                     );
                     ctx.rotate(curvedTextPathDrawingContext.nextPoint.angle);
 
                     if (fillColor) {
-                        ctx.fillStyle = fillColor.color;
+                        ctx.fillStyle = fillColor.getColor(
+                            this.config.isLightMode
+                        );
                         ctx.fillText(char, 0, 0);
                     }
 
                     if (fontStyle.borderWidth && borderColor !== null) {
                         // apply border width if set
                         ctx.lineWidth = fontStyle.borderWidth;
                         ctx.strokeStyle = borderColor;
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-render/PeekDispRenderDelegateEllipse.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-render/PeekDispRenderDelegateEllipse.web.ts`

 * *Files 10% similar despite different names*

```diff
@@ -35,16 +35,22 @@
 
     draw(disp, ctx, zoom: number, pan: PointI, drawMode: DrawModeE) {
         let fillColor = DispEllipse.fillColor(disp);
         let lineColor = DispEllipse.lineColor(disp);
         let lineStyle = DispEllipse.lineStyle(disp);
 
         // Null colors are also not drawn
-        fillColor = fillColor && fillColor.color ? fillColor : null;
-        lineColor = lineColor && lineColor.color ? lineColor : null;
+        fillColor =
+            fillColor && fillColor.getColor(this.config.isLightMode)
+                ? fillColor
+                : null;
+        lineColor =
+            lineColor && lineColor.getColor(this.config.isLightMode)
+                ? lineColor
+                : null;
 
         let xRadius = DispEllipse.xRadius(disp);
         let yRadius = DispEllipse.yRadius(disp);
         let rotationRadian = (DispEllipse.rotation(disp) / 180.0) * Math.PI;
         let startAngle = DispEllipse.startAngle(disp);
         let endAngle = DispEllipse.endAngle(disp);
         let lineWidth = DispEllipse.lineWidth(disp);
@@ -65,20 +71,20 @@
 
         ctx.beginPath();
         ctx.arc(0, 0, xRadius, startRadian, endRadian, true);
         //ctx.closePath();
 
         if (fillColor) {
             ctx.lineTo(0, 0); // Make it fill to the center, not just the ends of the arc
-            ctx.fillStyle = fillColor.color;
+            ctx.fillStyle = fillColor.getColor(this.config.isLightMode);
             ctx.fill();
         }
 
         if (lineColor) {
-            ctx.strokeStyle = lineColor.color;
+            ctx.strokeStyle = lineColor.getColor(this.config.isLightMode);
             ctx.lineWidth = lineStyle.scalable ? lineWidth : lineWidth / zoom;
             ctx.stroke();
         }
 
         // restore to original state
         ctx.restore();
     }
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-render/PeekDispRenderDelegateGroupPtr.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-render/PeekDispRenderDelegateGroupPtr.web.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-render/PeekDispRenderDelegateNull.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-render/PeekDispRenderDelegateNull.web.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-render/PeekDispRenderDelegatePoly.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-render/PeekDispRenderDelegatePoly.web.ts`

 * *Files 14% similar despite different names*

```diff
@@ -36,49 +36,55 @@
         let lineColor = DispPoly.lineColor(disp);
         let lineStyle = DispPoly.lineStyle(disp);
         let lineWidth = DispPoly.lineWidth(disp);
 
         if (!isPolygon && this.config.renderer.useEdgeColors) {
             const edgeColor = DispPolyline.edgeColor(<DispPolylineT>disp);
 
-            if (edgeColor?.color != null) {
+            if (edgeColor?.getColor(this.config.isLightMode) != null) {
                 /* We expect both backgroundColour and edgeColour to be in the
                  format #AARRGGBB or #RRGGBB, take the last 6 letters and
                  compare them.
                  */
                 let bgColorStr = this.config.renderer.backgroundColor || "";
                 bgColorStr = bgColorStr.substr(bgColorStr.length - 6);
 
-                let edgeColorStr = edgeColor?.color || "";
+                let edgeColorStr =
+                    edgeColor?.getColor(this.config.isLightMode) || "";
                 edgeColorStr = edgeColorStr.substr(edgeColorStr.length - 6);
 
                 if (bgColorStr !== edgeColorStr) {
                     lineColor = edgeColor;
                 }
             }
         }
 
         let dashPattern = null;
         if (lineStyle != null && lineStyle.dashPatternParsed != null)
             dashPattern = lineStyle.dashPatternParsed;
 
         // Null colors are also not drawn
-        fillColor = fillColor && fillColor.color ? fillColor : null;
+        fillColor =
+            fillColor && fillColor.getColor(this.config.isLightMode)
+                ? fillColor
+                : null;
         lineColor =
-            lineStyle && lineColor && lineColor.color ? lineColor : null;
+            lineStyle &&
+            lineColor &&
+            lineColor.getColor(this.config.isLightMode)
+                ? lineColor
+                : null;
 
         let geom = DispPolygon.geom(disp);
 
         // If there are no colours defined then this is a selectable only shape
         if (!fillColor && !lineColor) return;
 
         let fillDirection = DispPolygon.fillDirection(disp);
         let fillPercentage = DispPolygon.fillPercent(disp);
-        if (fillPercentage != null)
-            fillPercentage = Math.min(100, fillPercentage);
 
         let firstPointX = geom[0]; // get details of point
         let firstPointY = geom[1]; // get details of point
 
         // Fill the background first, if required
         if (lineColor && lineStyle.backgroundFillDashSpace && dashPattern) {
             ctx.beginPath();
@@ -136,15 +142,15 @@
                     geom.length
                 );
             }
             ctx.closePath();
         }
 
         if (lineColor) {
-            ctx.strokeStyle = lineColor.color;
+            ctx.strokeStyle = lineColor.getColor(this.config.isLightMode);
             ctx.lineWidth = lineStyle.scalable ? lineWidth : lineWidth / zoom;
             ctx.lineJoin = lineStyle.joinStyle;
             ctx.lineCap = lineStyle.capStyle;
             ctx.stroke();
         }
 
         if (fillColor) {
@@ -153,15 +159,15 @@
                     ctx,
                     PeekCanvasBounds.fromGeom(geom),
                     lineColor,
                     fillDirection,
                     fillPercentage
                 );
             } else {
-                ctx.fillStyle = fillColor.color;
+                ctx.fillStyle = fillColor.getColor(this.config.isLightMode);
                 ctx.fill();
             }
         }
 
         // Draw the line ends
         if (!isPolygon && 4 <= geom.length) {
             this.drawPolyLineEnd(
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-render/PeekDispRenderDelegateText.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-render/PeekDispRenderDelegateText.web.ts`

 * *Files 14% similar despite different names*

```diff
@@ -93,16 +93,22 @@
         let rotationRadian = (DispText.rotation(disp) / 180.0) * Math.PI;
 
         let fontStyle = DispText.textStyle(disp);
         let fillColor = DispText.color(disp);
         let borderColor = DispText.borderColor(disp);
 
         // Null colors are also not drawn
-        fillColor = fillColor && fillColor.color ? fillColor : null;
-        borderColor = borderColor && borderColor.color ? borderColor : null;
+        fillColor =
+            fillColor && fillColor.getColor(this.config.isLightMode)
+                ? fillColor
+                : null;
+        borderColor =
+            borderColor && borderColor.getColor(this.config.isLightMode)
+                ? borderColor
+                : null;
 
         // TODO, Draw a box around the text, based on line style
 
         let horizontalStretchFactor = DispText.horizontalStretch(disp);
         let textHeight = DispText.height(disp);
 
         let fontSize = fontStyle.fontSize * fontStyle.scaleFactor;
@@ -159,41 +165,55 @@
         // Bounds can get serliased in branches, so check to see if it's actually the
         // class or just the restored object that it serialises to.
         if (updateBounds) {
             disp.bounds = new PeekCanvasBounds();
             disp.bounds.w = 0;
         }
 
-        let lines = DispText.text(disp).split("\n");
-        for (let lineIndex = 0; lineIndex < lines.length; ++lineIndex) {
-            let line = lines[lineIndex];
+        let renderedLines = [];
+        if ((fontStyle.wrapTextAtChars || 0) <= 0) {
+            renderedLines = DispText.text(disp).split("\n");
+        } else {
+            const wrappedLines = this.wrapText(
+                DispText.text(disp),
+                fontStyle.wrapTextAtChars
+            );
+            for (const wrappedLine of wrappedLines) {
+                for (const renderedLine of wrappedLine.split("\n")) {
+                    renderedLines.push(renderedLine);
+                }
+            }
+        }
+
+        for (let lineIndex = 0; lineIndex < renderedLines.length; ++lineIndex) {
+            let line = renderedLines[lineIndex];
             let yOffset = lineHeight * lineIndex;
 
             // Measure the width
             if (updateBounds) {
                 let thisWidth = ctx.measureText(line).width / zoom;
                 if (disp.bounds.w < thisWidth) disp.bounds.w = thisWidth;
             }
 
             if (fillColor) {
-                ctx.fillStyle = fillColor.color;
+                ctx.fillStyle = fillColor.getColor(this.config.isLightMode);
                 ctx.fillText(line, 0, yOffset);
             }
 
             if (fontStyle.borderWidth && borderColor !== null) {
                 // apply border width if set
                 ctx.lineWidth = fontStyle.borderWidth;
                 ctx.strokeStyle = borderColor;
                 ctx.strokeText(line, 0, yOffset);
             }
         }
 
         let singleLineHeight = lineHeight / zoom;
         if (updateBounds) {
-            disp.bounds.h = singleLineHeight * lines.length;
+            disp.bounds.h = singleLineHeight * renderedLines.length;
         }
 
         // restore to original state
         ctx.restore();
 
         if (updateBounds) {
             if (horizontalAlignEnum == TextHorizontalAlign.left)
@@ -207,8 +227,17 @@
                 disp.bounds.y = centerY;
             else if (verticalAlignEnum == TextVerticalAlign.center)
                 disp.bounds.y = centerY - singleLineHeight / 2;
             else if (verticalAlignEnum == TextVerticalAlign.bottom)
                 disp.bounds.y = centerY - singleLineHeight;
         }
     }
+
+    private wrapText(text: string, width: number): string[] {
+        const substrings: string[] = [];
+        for (let i = 0; i < text.length; i += width) {
+            const substring = text.slice(i, i + width);
+            substrings.push(substring);
+        }
+        return substrings;
+    }
 }
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-render/PeekDispRenderFactory.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-render/PeekDispRenderFactory.web.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-shapes/DispBase.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-shapes/DispBase.ts`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-import { DispLayer, DispLevel } from "@peek/peek_plugin_diagram/lookups";
+import {
+    DispLayer,
+    DispLevel,
+} from "@peek/peek_plugin_diagram/_private/lookups";
 import {
     PeekCanvasShapePropsContext,
     ShapeProp,
     ShapePropType,
 } from "../canvas/PeekCanvasShapePropsContext";
 import { PeekCanvasBounds } from "../canvas/PeekCanvasBounds";
 import { ModelCoordSet } from "@peek/peek_plugin_diagram/_private/tuples";
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-shapes/DispCurvedText.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-shapes/DispCurvedText.ts`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import { DispBase, DispBaseT, PointI } from "./DispBase";
-import { DispColor, DispTextStyle } from "@peek/peek_plugin_diagram/lookups";
+import {
+    DispColor,
+    DispTextStyle,
+} from "@peek/peek_plugin_diagram/_private/lookups";
 import {
     PeekCanvasShapePropsContext,
     ShapeProp,
     ShapePropType,
 } from "../canvas/PeekCanvasShapePropsContext";
 import { ModelCoordSet } from "@peek/peek_plugin_diagram/_private/tuples";
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-shapes/DispEdgeTemplate.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-shapes/DispEdgeTemplate.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-shapes/DispEllipse.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-shapes/DispEllipse.ts`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import { DispBase, DispBaseT, PointI } from "./DispBase";
-import { DispColor, DispLineStyle } from "@peek/peek_plugin_diagram/lookups";
+import {
+    DispColor,
+    DispLineStyle,
+} from "@peek/peek_plugin_diagram/_private/lookups";
 import { DispPoly } from "./DispPoly";
 import {
     PeekCanvasShapePropsContext,
     ShapeProp,
     ShapePropType,
 } from "../canvas/PeekCanvasShapePropsContext";
 import { ModelCoordSet } from "@peek/peek_plugin_diagram/_private/tuples/ModelCoordSet";
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-shapes/DispGroup.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-shapes/DispGroup.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-shapes/DispGroupPointer.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-shapes/DispGroupPointer.ts`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import { PrivateDiagramLookupService } from "@peek/peek_plugin_diagram/_private/services/PrivateDiagramLookupService";
 import { BranchTuple } from "@peek/peek_plugin_diagram/_private/branch/BranchTuple";
 import {
     calculateRotationFromHandleDelta,
     makeRotateHandlePoints,
 } from "./DispUtilRotate";
 import { DispText } from "./DispText";
-import { DispFactory } from "./DispFactory";
+import { getWrapper } from "./DispFactoryTypeMap";
 
 export interface DispGroupPointerT extends DispBaseT {
     // verticalScale
     vs: number;
 
     // horizontalScale
     hs: number;
@@ -131,15 +131,15 @@
         if (data == null) return;
 
         // We've rotate the disps, now store the current rotation
         DispGroupPointer.setRotation(disp, data.newRotation);
         disp.tempRotation = data.tempRotation;
 
         for (const childDisp of disp.disps) {
-            const Wrapper = DispFactory.wrapper(childDisp);
+            const Wrapper = getWrapper(DispBase.type(childDisp));
             Wrapper.rotateAboutAxis(childDisp, center, data.deltaRotation);
         }
         DispBase.setBoundsNull(disp);
     }
 
     static rotateAboutAxis(disp, center: PointI, rotationDegrees: number) {
         console.log("NOT IMPLEMENTED: Rotating child DispGroupPtrs");
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-shapes/DispNull.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-shapes/DispNull.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-shapes/DispPoly.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-shapes/DispPoly.ts`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import { DispBase, DispBaseT, PointI, PointsT } from "./DispBase";
-import { DispColor, DispLineStyle } from "@peek/peek_plugin_diagram/lookups";
+import {
+    DispColor,
+    DispLineStyle,
+} from "@peek/peek_plugin_diagram/_private/lookups";
 import {
     PeekCanvasShapePropsContext,
     ShapeProp,
     ShapePropType,
 } from "../canvas/PeekCanvasShapePropsContext";
 import { ModelCoordSet } from "@peek/peek_plugin_diagram/_private/tuples/ModelCoordSet";
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-shapes/DispPolygon.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-shapes/DispPolygon.ts`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import { DispColor } from "@peek/peek_plugin_diagram/lookups";
+import { DispColor } from "@peek/peek_plugin_diagram/_private/lookups";
 import { DispPoly, DispPolyT } from "./DispPoly";
 import { DispBase, PointI } from "./DispBase";
 import {
     PeekCanvasShapePropsContext,
     ShapeProp,
     ShapePropType,
 } from "../canvas/PeekCanvasShapePropsContext";
@@ -61,23 +61,27 @@
 
         if (val == PolygonFillDirection.fillRightToLeft)
             return PolygonFillDirection.fillRightToLeft;
 
         if (val == PolygonFillDirection.fillLeftToRight)
             return PolygonFillDirection.fillLeftToRight;
 
+        // Else, default to Top to Bottom
         return PolygonFillDirection.fillTopToBottom;
     }
 
     static setFillDirection(disp: DispPolygonT, val: number): void {
         disp.fd = val;
     }
 
-    static fillPercent(disp: DispPolygonT): number {
-        return disp.fp;
+    static fillPercent(disp: DispPolygonT): number | null {
+        const fillPercentage = disp.fp;
+        if (fillPercentage == null) return null;
+
+        return Math.max(0.0, Math.min(100.0, fillPercentage));
     }
 
     static setFillPercent(disp: DispPolygonT, val: number): void {
         disp.fp = val;
     }
 
     static isRectangle(disp: DispPolygonT): boolean {
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-shapes/DispPolyline.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-shapes/DispPolyline.ts`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 } from "./DispBase";
 import {
     PeekCanvasShapePropsContext,
     ShapeProp,
     ShapePropType,
 } from "../canvas/PeekCanvasShapePropsContext";
 import { ModelCoordSet } from "@peek/peek_plugin_diagram/_private/tuples/ModelCoordSet";
-import { DispColor } from "@peek/peek_plugin_diagram/lookups";
+import { DispColor } from "@peek/peek_plugin_diagram/_private/lookups";
 import { PeekCanvasBounds } from "../canvas/PeekCanvasBounds";
 import { BranchTuple } from "@peek/peek_plugin_diagram/_private/branch/BranchTuple";
 import { PrivateDiagramLookupService } from "@peek/peek_plugin_diagram/_private/services/PrivateDiagramLookupService";
 import { DispEdgeTemplate, DispEdgeTemplateT } from "./DispEdgeTemplate";
 
 export interface DispPolylineT extends DispPolyT {
     // Edge Color
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-shapes/DispRectangle.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-shapes/DispRectangle.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-shapes/DispText.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-shapes/DispText.ts`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import { DispBase, DispBaseT, PointI } from "./DispBase";
-import { DispColor, DispTextStyle } from "@peek/peek_plugin_diagram/lookups";
+import {
+    DispColor,
+    DispTextStyle,
+} from "@peek/peek_plugin_diagram/_private/lookups";
 import {
     PeekCanvasShapePropsContext,
     ShapeProp,
     ShapePropType,
 } from "../canvas/PeekCanvasShapePropsContext";
 import { ModelCoordSet } from "@peek/peek_plugin_diagram/_private/tuples";
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-shapes/DispUtil.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-shapes/DispUtil.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/canvas-shapes/DispUtilRotate.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/canvas-shapes/DispUtilRotate.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/diagram.component.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/diagram.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/diagram.component.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/diagram.component.web.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/diagram.module.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/diagram.module.web.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-component/edit-props.component.web.html` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-component/edit-props.component.web.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-component/edit-props.component.web.scss` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-component/edit-props.component.web.scss`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-component/edit-props.component.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-component/edit-props.component.web.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-edge-template-component/edit-props-edge-template.component.html` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-edge-template-component/edit-props-edge-template.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-edge-template-component/edit-props-edge-template.component.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-edge-template-component/edit-props-edge-template.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-group-ptr-component/edit-props-group-ptr.component.html` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-group-ptr-component/edit-props-group-ptr.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-group-ptr-component/edit-props-group-ptr.component.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-group-ptr-component/edit-props-group-ptr.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-livedb-component/edit-props-livedb.component.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-livedb-component/edit-props-livedb.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-shape-component/edit-props-shape.component.html` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-shape-component/edit-props-shape.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-shape-component/edit-props-shape.component.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-shape-component/edit-props-shape.component.ts`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 import { NgLifeCycleEvents } from "@synerty/vortexjs";
 import { PeekCanvasEditor } from "../canvas/PeekCanvasEditor.web";
 import {
     PeekCanvasShapePropsContext,
     ShapeProp,
     ShapePropType,
 } from "../canvas/PeekCanvasShapePropsContext";
-import { DispLayer, DispLevel } from "@peek/peek_plugin_diagram/lookups";
+import {
+    DispLayer,
+    DispLevel,
+} from "@peek/peek_plugin_diagram/_private/lookups";
 import { assert } from "../DiagramUtil";
 
 @Component({
     selector: "pl-diagram-edit-props-shape",
     templateUrl: "edit-props-shape.component.html",
     styleUrls: ["edit-props-shape.component.scss"],
 })
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-toolbar-component/edit-props-toolbar.component.web.html` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-toolbar-component/edit-props-toolbar.component.web.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-toolbar-component/edit-props-toolbar.component.web.scss` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-toolbar-component/edit-props-toolbar.component.web.scss`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-props-toolbar-component/edit-props-toolbar.component.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-props-toolbar-component/edit-props-toolbar.component.web.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-toolbar-component/edit-toolbar.component.web.html` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-toolbar-component/edit-toolbar.component.web.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-toolbar-component/edit-toolbar.component.web.scss` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-toolbar-component/edit-toolbar.component.web.scss`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/edit-toolbar-component/edit-toolbar.component.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/edit-toolbar-component/edit-toolbar.component.web.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/print-component/print.component.web.scss` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/print-component/print.component.web.scss`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/print-component/print.component.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/print-component/print.component.web.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/services/canvas.service.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/services/canvas.service.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/services/context-menu.service.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/services/context-menu.service.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/services/copy-paste.service.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/services/copy-paste.service.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/set-position-component/set-position.component.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/set-position-component/set-position.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/start-edit-component/start-edit.component.web.html` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/start-edit-component/start-edit.component.web.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/start-edit-component/start-edit.component.web.scss` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/start-edit-component/start-edit.component.web.scss`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/start-edit-component/start-edit.component.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/start-edit-component/start-edit.component.web.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/view-select-branches-component/select-branches.component.web.html` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/view-select-branches-component/select-branches.component.web.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/view-select-branches-component/select-branches.component.web.scss` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/view-select-branches-component/select-branches.component.web.scss`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/view-select-branches-component/select-branches.component.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/view-select-branches-component/select-branches.component.web.ts`

 * *Files 8% similar despite different names*

```diff
@@ -21,233 +21,227 @@
     selector: "pl-diagram-view-select-branches",
     templateUrl: "select-branches.component.web.html",
     styleUrls: ["select-branches.component.web.scss"],
 })
 export class SelectBranchesComponent extends NgLifeCycleEvents {
     @Input("coordSetKey")
     coordSetKey: string;
-    
+
     @Input("modelSetKey")
     modelSetKey: string;
-    
+
     @Input("config")
     config: PeekCanvasConfig;
-    
+
     popupShown: boolean = false;
     enabledBranches: { [branchKey: string]: BranchDetailTuple } = {};
     selectedGlobalBranch: BranchDetailTuple | null = null;
-    
+
     private coordSetService: PrivateDiagramCoordSetService;
-    
+
     private _filterText: string = "";
     private _showOnlyMine: boolean = true;
     private _sortByDate: boolean = true;
-    
+
     items$ = new BehaviorSubject<BranchDetailTuple[]>([]);
     private allItems: BranchDetailTuple[] = [];
-    
+
     constructor(
         private objectPopupService: DocDbPopupService,
         private headerService: HeaderService,
         private lookupService: PrivateDiagramLookupService,
         private configService: PrivateDiagramConfigService,
         private branchService: PrivateDiagramBranchService,
         abstractCoordSetService: DiagramCoordSetService,
         private globalBranchService: BranchService,
         private userService: UserService
     ) {
         super();
-        
+
         this.coordSetService = <PrivateDiagramCoordSetService>(
             abstractCoordSetService
         );
-        
+
         this.configService
             .popupBranchesSelectionObservable()
             .pipe(takeUntil(this.onDestroyEvent))
             .subscribe(() => this.openPopup());
-        
+
         this.objectPopupService
             .popupClosedObservable(DocDbPopupTypeE.summaryPopup)
             .pipe(
                 filter(
                     (reason) =>
                         reason == DocDbPopupClosedReasonE.userClickedAction
                 )
             )
             .subscribe(() => this.closePopupFull());
-        
+
         this.objectPopupService
             .popupClosedObservable(DocDbPopupTypeE.detailPopup)
             .pipe(
                 filter(
                     (reason) =>
                         reason == DocDbPopupClosedReasonE.userClickedAction
                 )
             )
             .subscribe(() => this.closePopupFull());
     }
-    
+
     closePopupFull(): void {
         this.clearBranchDetails();
         this.closePopup();
     }
-    
+
     closePopup(): void {
         if (this.showBranchDetails()) {
             this.clearBranchDetails();
             return;
         }
-        
+
         let branches = [];
         for (let key of Object.keys(this.enabledBranches)) {
             branches.push(this.enabledBranches[key]);
         }
         this.branchService.setVisibleBranches(branches);
         this.config.setModelNeedsCompiling();
         this.config.invalidate();
-        
+
         this.popupShown = false;
-        
+
         // Discard the integration additions
         this.items$.next([]);
     }
-    
+
     get items(): BranchDetailTuple[] {
         return this.items$.value;
     }
-    
+
     get showOnlyMine(): boolean {
         return this._showOnlyMine;
     }
-    
+
     set showOnlyMine(value: boolean) {
         this._showOnlyMine = value;
         this.refilter();
     }
-    
+
     get sortByDate(): boolean {
         return this._sortByDate;
     }
-    
+
     set sortByDate(value: boolean) {
         this._sortByDate = value;
         this.refilter();
     }
-    
+
     get filterText(): string {
         return this._filterText;
     }
-    
+
     set filterText(value: string) {
-        this._filterText = value;
+        this._filterText = value.toLowerCase();
         this.refilter();
     }
-    
+
     private refilter(): void {
-        const filtByStr = i => {
-            return this._filterText.length === 0
-                || i.name.indexOf(this._filterText) !== -1;
+        const filtByStr = (i) => {
+            return (
+                this._filterText.length === 0 ||
+                i.name.toLowerCase().indexOf(this._filterText) !== -1
+            );
         };
-        
-        const filtByName = i => {
-            return !this._showOnlyMine
-                || i.userName == this.userService.userDetails.userId;
+
+        const filtByName = (i) => {
+            return (
+                !this._showOnlyMine ||
+                i.userName?.toLowerCase() ==
+                    this.userService.userDetails.userId?.toLowerCase()
+            );
         };
-        
-        const compStr = (
-            a,
-            b
-        ) => a == b ? 0 : a < b ? -1 : 1;
-        
-        let items = this.allItems
-            .filter(i => filtByStr(i) && filtByName(i));
-        
+
+        const compStr = (a, b) => (a == b ? 0 : a < b ? -1 : 1);
+
+        let items = this.allItems.filter((i) => filtByStr(i) && filtByName(i));
+
         if (this._sortByDate) {
             items = items.sort(
-                (
-                    a,
-                    b
-                ) => b.createdDate.getTime() - a.createdDate.getTime()
+                (a, b) => b.createdDate.getTime() - a.createdDate.getTime()
             );
-        }
-        else {
-            items = items.sort(
-                (
-                    a,
-                    b
-                ) => compStr(a.name.toLowerCase(), b.name.toLowerCase())
+        } else {
+            items = items.sort((a, b) =>
+                compStr(a.name.toLowerCase(), b.name.toLowerCase())
             );
         }
         this.items$.next(items);
     }
-    
+
     noItems(): boolean {
-        return this.items.length == 0
-            && (this._filterText.length === 0 || this.noAllItems());
+        return (
+            this.items.length == 0 &&
+            (this._filterText.length === 0 || this.noAllItems())
+        );
     }
-    
+
     noAllItems(): boolean {
         return this.allItems.length === 0;
     }
-    
+
     noFilteredItems(): boolean {
-        return this.items.length == 0
-            && this._filterText.length !== 0;
+        return this.items.length == 0 && this._filterText.length !== 0;
     }
-    
+
     toggleBranchEnabled(branchDetail: BranchDetailTuple): void {
         if (this.enabledBranches[branchDetail.key] == null) {
             this.enabledBranches[branchDetail.key] = branchDetail;
-        }
-        else {
+        } else {
             delete this.enabledBranches[branchDetail.key];
         }
     }
-    
+
     isBranchEnabled(branchDetail: BranchDetailTuple): boolean {
         return this.enabledBranches[branchDetail.key] != null;
     }
-    
+
     branchSelected(branchDetail: BranchDetailTuple): void {
         this.selectedGlobalBranch = branchDetail;
     }
-    
+
     clearBranchDetails(): void {
         this.selectedGlobalBranch = null;
     }
-    
+
     showBranchDetails(): boolean {
         return this.selectedGlobalBranch != null;
     }
-    
+
     protected openPopup() {
         let coordSet = this.coordSetService.coordSetForKey(
             this.modelSetKey,
             this.coordSetKey
         );
         console.log("Opening Branch Select popup");
-        
+
         // Get a list of existing diagram branches, if there are no matching diagram
         // branches, then don't show them
         let diagramKeys = this.branchService.getDiagramBranchKeys(coordSet.id);
         let diagramKeyDict = {};
         for (let key of diagramKeys) {
             diagramKeyDict[key] = true;
         }
-        
+
         this.globalBranchService
             .branches(this.modelSetKey)
             .then((tuples: BranchDetailTuple[]) => {
                 this.allItems = [];
                 for (let item of tuples) {
                     if (diagramKeyDict[item.key] == null) continue;
                     this.allItems.push(item);
                     item["__enabled"] = this.enabledBranches[item.key] != null;
                 }
                 this.refilter();
             });
         this.allItems = [];
-        
+
         this.popupShown = true;
     }
 }
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/view-select-layers-component/select-layers.component.web.html` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/view-select-layers-component/select-layers.component.web.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/view-select-layers-component/select-layers.component.web.scss` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/view-select-layers-component/select-layers.component.web.scss`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/view-select-layers-component/select-layers.component.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/view-select-layers-component/select-layers.component.web.ts`

 * *Files 8% similar despite different names*

```diff
@@ -5,129 +5,124 @@
 
 import {
     PopupLayerSelectionArgsI,
     PrivateDiagramConfigService,
 } from "@peek/peek_plugin_diagram/_private/services/PrivateDiagramConfigService";
 import { PrivateDiagramLookupService } from "@peek/peek_plugin_diagram/_private/services/PrivateDiagramLookupService";
 import { DiagramCoordSetService } from "@peek/peek_plugin_diagram/DiagramCoordSetService";
-import { DispLayer } from "@peek/peek_plugin_diagram/lookups";
+import { DispLayer } from "@peek/peek_plugin_diagram/_private/lookups";
 
 import { PrivateDiagramCoordSetService } from "@peek/peek_plugin_diagram/_private/services/PrivateDiagramCoordSetService";
 import { PeekCanvasConfig } from "../canvas/PeekCanvasConfig.web";
 import { PeekCanvasModel } from "../canvas/PeekCanvasModel.web";
 import { BehaviorSubject } from "rxjs";
 import { BranchDetailTuple } from "@peek/peek_plugin_branch";
 
 @Component({
     selector: "pl-diagram-view-select-layers",
     templateUrl: "select-layers.component.web.html",
     styleUrls: ["select-layers.component.web.scss"],
 })
 export class SelectLayersComponent extends NgLifeCycleEvents implements OnInit {
     popupShown: boolean = false;
-    
+
     @Input("coordSetKey")
     coordSetKey: string;
-    
+
     @Input("modelSetKey")
     modelSetKey: string;
-    
+
     @Input("model")
     model: PeekCanvasModel;
-    
+
     @Input("config")
     config: PeekCanvasConfig;
-    
+
     allItems: DispLayer[] = [];
-    
+
     items$ = new BehaviorSubject<DispLayer[]>([]);
-    
+
     private coordSetService: PrivateDiagramCoordSetService;
-    
+
     private _filterText: string = "";
-    
+
     constructor(
         private headerService: HeaderService,
         private lookupService: PrivateDiagramLookupService,
         private configService: PrivateDiagramConfigService,
         abstractCoordSetService: DiagramCoordSetService
     ) {
         super();
-        
+
         this.coordSetService = <PrivateDiagramCoordSetService>(
             abstractCoordSetService
         );
-        
+
         this.configService
             .popupLayerSelectionObservable()
             .pipe(takeUntil(this.onDestroyEvent))
             .subscribe((v: PopupLayerSelectionArgsI) => this.openPopup(v));
     }
-    
-    ngOnInit() {
-    }
-    
+
+    ngOnInit() {}
+
     closePopup(): void {
         this.popupShown = false;
         this.allItems = [];
         this.refilter();
     }
-    
+
     noItems(): boolean {
         return this.items.length == 0;
     }
-    
+
     get items(): DispLayer[] {
         return this.items$.value;
     }
-    
+
     get filterText(): string {
         return this._filterText;
     }
-    
+
     set filterText(value: string) {
-        this._filterText = value;
+        this._filterText = value.toLowerCase();
         this.refilter();
     }
-    
+
     private refilter(): void {
-        const filtByStr = i => {
-            return this._filterText.length === 0
-                || i.name.indexOf(this._filterText) !== -1;
+        const filtByStr = (i) => {
+            return (
+                this._filterText.length === 0 ||
+                i.name.toLowerCase().indexOf(this._filterText) !== -1
+            );
         };
-        
-        let items = this.allItems.filter(i => filtByStr(i));
-        
-        const compStr = (
-            a,
-            b
-        ) => a == b ? 0 : a < b ? -1 : 1;
-        items = items.sort((
-                a,
-                b
-            ) =>
-                a.name == b.name ? 0 : a.name < b.name ? -1 : 1
+
+        let items = this.allItems.filter((i) => filtByStr(i));
+
+        const compStr = (a, b) => (a == b ? 0 : a < b ? -1 : 1);
+        items = items.sort((a, b) =>
+            compStr(a.name.toLowerCase(), b.name.toLowerCase())
         );
-        
+
         this.items$.next(items);
     }
-    
+
     toggleLayerVisible(layer: DispLayer): void {
         layer.visible = !layer.visible;
         if (this.model != null) this.model.recompileModel();
     }
-    
-    protected openPopup({coordSetKey, modelSetKey}) {
+
+    protected openPopup({ coordSetKey, modelSetKey }) {
         let coordSet = this.coordSetService.coordSetForKey(
             modelSetKey,
             coordSetKey
         );
         console.log("Opening Layer Select popup");
-        
+
         this.allItems = this.lookupService.layersOrderedByOrder(
             coordSet.modelSetId
         );
         this.refilter();
-        
+
         this.popupShown = true;
     }
 }
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/view-toolbar-component/toolbar.component.web.html` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/view-toolbar-component/toolbar.component.web.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<div class="toolbar">
+<div class="toolbar" style="border: 1px solid rgba(0, 0, 0, 0.1)">
     <div class="toolbar-buttons">
         <button
             *ngIf="showExitDiagramButton()"
             [nzDropdownMenu]="changeCoordSetMenu"
             nz-dropdown
             nzPlacement="bottomLeft"
         >
@@ -17,51 +17,70 @@
                 >
                     {{item.name}}
                 </li>
             </ul>
         </nz-dropdown-menu>
 
         <button
+            *ngIf="showToggleColorModeButton()"
+            (click)="toggleColorModeButton()"
+            nz-tooltip
+            [nzTooltipMouseEnterDelay]="1.0"
+            nzTooltipPlacement="bottom"
+            nzTooltipTitle="Toggle to dark/light mode"
+            [nzTooltipTrigger]="tooltipTrigger"
+        >
+            <i
+                nz-icon
+                [nzTheme]='isLightMode() === true ? "fill" : "outline"'
+                nzType="read"
+            ></i>
+        </button>
+        <button
             *ngIf="showPrintDiagramButton()"
             (click)="printDiagramClicked()"
             nz-tooltip
             [nzTooltipMouseEnterDelay]="1.0"
             nzTooltipPlacement="bottom"
             nzTooltipTitle="Show Diagram for Print"
+            [nzTooltipTrigger]="tooltipTrigger"
         >
             <i nz-icon nzTheme="outline" nzType="printer"></i>
         </button>
         <button
             (click)="editDiagramClicked()"
             *ngIf="showEditDiagramButton()"
             nz-tooltip
             [nzTooltipMouseEnterDelay]="1.0"
             nzTooltipPlacement="bottom"
             nzTooltipTitle="Edit Diagram"
+            [nzTooltipTrigger]="tooltipTrigger"
         >
             <i nz-icon nzTheme="outline" nzType="edit"></i>
         </button>
         <button
             (click)="selectBranchesClicked()"
             *ngIf="showSelectBranchesButton()"
             [class.btn-warning]="isBranchesActive()"
             [nzTooltipTitle]="showSelectBranchesTooltip()"
             nz-tooltip
             [nzTooltipMouseEnterDelay]="1.0"
             nzTooltipPlacement="bottom"
+            [nzTooltipTrigger]="tooltipTrigger"
         >
             <i nz-icon nzTheme="outline" nzType="branches"></i>
         </button>
         <button
             *ngIf="showSelectLayers()"
             (click)="selectLayersClicked()"
             nz-tooltip
             [nzTooltipMouseEnterDelay]="1.0"
             nzTooltipPlacement="bottom"
             nzTooltipTitle="Select Layers"
+            [nzTooltipTrigger]="tooltipTrigger"
         >
             <svg
                 height="1em"
                 viewBox="0 0 2048 2048"
                 width="1em"
                 xmlns="http://www.w3.org/2000/svg"
             >
@@ -76,26 +95,28 @@
         <button
             (click)="goUpParentButtonClicked(btn)"
             *ngIf="showGoUpParentButton()"
             nz-tooltip
             [nzTooltipMouseEnterDelay]="1.0"
             nzTooltipPlacement="bottom"
             nzTooltipTitle="Back"
+            [nzTooltipTrigger]="tooltipTrigger"
         >
             <i nz-icon nzTheme="outline" nzType="arrow-left"></i>
             Back
         </button>
         <button
             (click)="buttonClicked(btn)"
             *ngFor="let btn of shownPluginButtons"
             [class.active]="isButtonActive(btn)"
             [nzTooltipTitle]="btn.tooltip"
             nz-tooltip
             [nzTooltipMouseEnterDelay]="1.0"
             nzTooltipPlacement="bottom"
+            [nzTooltipTrigger]="tooltipTrigger"
         >
             <i
                 *ngIf="btn.icon"
                 nz-icon
                 nzTheme="outline"
                 nzType="{{btn.icon}}"
             ></i>
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/view-toolbar-component/toolbar.component.web.scss` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/view-toolbar-component/toolbar.component.web.scss`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-app/view-toolbar-component/toolbar.component.web.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-app/view-toolbar-component/toolbar.component.web.ts`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import { PrivateDiagramBranchService } from "@peek/peek_plugin_diagram/_private/branch/PrivateDiagramBranchService";
 import { NgLifeCycleEvents } from "@synerty/vortexjs";
 import { PeekCanvasConfig } from "../canvas/PeekCanvasConfig.web";
 import { ModelCoordSet } from "@peek/peek_plugin_diagram/_private/tuples";
 import { PrivateDiagramCoordSetService } from "@peek/peek_plugin_diagram/_private/services/PrivateDiagramCoordSetService";
 import { DiagramPositionService } from "@peek/peek_plugin_diagram/DiagramPositionService";
 import { DocDbPopupService, DocDbPopupTypeE } from "@peek/peek_core_docdb";
+import { DeviceEnrolmentService } from "@peek/peek_core_device";
 
 @Component({
     selector: "pl-diagram-view-toolbar",
     templateUrl: "toolbar.component.web.html",
     styleUrls: ["toolbar.component.web.scss"],
 })
 export class ToolbarComponent extends NgLifeCycleEvents implements OnInit {
@@ -38,24 +39,27 @@
 
     dispKey: string;
     coordSet: ModelCoordSet = new ModelCoordSet();
     shownPluginButtons: DiagramToolButtonI[] = [];
     toolbarIsOpen: boolean = false;
     coordSetsForMenu: ModelCoordSet[] = [];
 
+    tooltipTrigger = "hover";
+
     protected toolbarService: PrivateDiagramToolbarService;
     private parentPluginButtons: DiagramToolButtonI[][] = [];
 
     constructor(
         private objectPopupService: DocDbPopupService,
         private abstractToolbarService: DiagramToolbarService,
         private branchService: PrivateDiagramBranchService,
         private configService: PrivateDiagramConfigService,
         private coordSetService: PrivateDiagramCoordSetService,
-        private positionService: DiagramPositionService
+        private positionService: DiagramPositionService,
+        private deviceEnrolmentService: DeviceEnrolmentService
     ) {
         super();
 
         this.toolbarService = <PrivateDiagramToolbarService>(
             abstractToolbarService
         );
 
@@ -64,14 +68,19 @@
         this.toolbarService
             .toolButtonsUpdatedObservable()
             .pipe(takeUntil(this.onDestroyEvent))
             .subscribe((buttons: DiagramToolButtonI[]) => {
                 this.shownPluginButtons = buttons;
                 this.parentPluginButtons = [];
             });
+
+        // While we're using ant.design v10, disable tooltips for field / iOS
+        if (this.deviceEnrolmentService.isFieldService()) {
+            this.tooltipTrigger = null;
+        }
     }
 
     ngOnInit() {
         if (this.config.coordSet != null) this.coordSet = this.config.coordSet;
 
         this.config.controller.coordSetChange
             .pipe(takeUntil(this.onDestroyEvent))
@@ -132,14 +141,30 @@
     }
 
     changeCoordSetMenuItemClicked(coordSet: ModelCoordSet): void {
         this.objectPopupService.hidePopup(DocDbPopupTypeE.tooltipPopup);
         this.positionService.positionByCoordSet(this.modelSetKey, coordSet.key);
     }
 
+    showToggleColorModeButton(): boolean {
+        return (
+            (this.buttonBitmask &
+                DiagramToolbarBuiltinButtonEnum.BUTTON_COLOR_MODES) >
+            0
+        );
+    }
+
+    isLightMode(): boolean {
+        return this.config.isLightMode;
+    }
+
+    toggleColorModeButton(): void {
+        this.config.isLightMode = !this.config.isLightMode;
+    }
+
     showPrintDiagramButton(): boolean {
         return (
             (this.buttonBitmask &
                 DiagramToolbarBuiltinButtonEnum.BUTTOON_PRINT_DIAGRAM) >
             0
         );
     }
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/both-assets/icon.png` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/both-assets/icon.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/ClientEntryHook.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/ClientEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/TupleDataObservable.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/TupleDataObservable.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,19 +43,19 @@
 )
 from peek_plugin_diagram._private.client.tuple_providers.ClientModelSetTupleProvider import (
     ClientModelSetTupleProvider,
 )
 from peek_plugin_diagram._private.client.tuple_providers.GridCacheIndexTupleProvider import (
     GridCacheIndexTupleProvider,
 )
-from peek_plugin_diagram._private.storage.Display import DispColor
-from peek_plugin_diagram._private.storage.Display import DispLayer
-from peek_plugin_diagram._private.storage.Display import DispLevel
-from peek_plugin_diagram._private.storage.Display import DispLineStyle
-from peek_plugin_diagram._private.storage.Display import DispTextStyle
+from peek_plugin_diagram._private.storage.Lookups import DispColor
+from peek_plugin_diagram._private.storage.Lookups import DispLayer
+from peek_plugin_diagram._private.storage.Lookups import DispLevel
+from peek_plugin_diagram._private.storage.Lookups import DispLineStyle
+from peek_plugin_diagram._private.storage.Lookups import DispTextStyle
 from peek_plugin_diagram._private.storage.ModelSet import ModelCoordSet
 from peek_plugin_diagram._private.storage.ModelSet import ModelSet
 from peek_plugin_diagram._private.tuples.GroupDispsTuple import GroupDispsTuple
 from peek_plugin_diagram._private.tuples.branch.BranchIndexUpdateDateTuple import (
     BranchIndexUpdateDateTuple,
 )
 from peek_plugin_diagram._private.tuples.branch.BranchTuple import BranchTuple
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/controller/BranchIndexCacheController.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/controller/BranchIndexCacheController.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,9 +30,9 @@
 
     """
 
     _ChunkedTuple = BranchIndexEncodedChunk
     _UpdateDateTupleABC = BranchIndexUpdateDateTuple
     _chunkLoadRpcMethod = BranchIndexChunkLoadRpc.loadBranchIndexChunks
     _chunkIndexDeltaRpcMethod = BranchIndexChunkLoadRpc.loadBranchIndexDelta
-    _updateFromServerFilt = clientBranchIndexUpdateFromServerFilt
+    _updateFromLogicFilt = clientBranchIndexUpdateFromServerFilt
     _logger = logger
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/controller/CoordSetCacheController.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/controller/ModelSetCacheController.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,71 @@
 from typing import Dict
 from typing import List
-from typing import Optional
 
+from vortex.Payload import Payload
 from vortex.TupleSelector import TupleSelector
 from vortex.handler.TupleDataObservableHandler import TupleDataObservableHandler
 from vortex.handler.TupleDataObserverClient import TupleDataObserverClient
 
-from peek_plugin_diagram._private.storage.ModelSet import ModelCoordSet
+from peek_plugin_diagram._private.storage.ModelSet import ModelSet
 
 
-class CoordSetCacheController:
+class ModelSetCacheController:
     """Lookup Cache Controller
 
     This class caches the lookups in each client.
 
     """
 
     def __init__(self, tupleObserver: TupleDataObserverClient):
         self._tupleObserver = tupleObserver
         self._tupleObservable = None
 
         #: This stores the cache of grid data for the clients
-        self._coordSetCache: Dict[int, ModelCoordSet] = {}
+        self._cache: Dict[int, ModelSet] = {}
+
+        self._vortexMsgCache = None
 
     def setTupleObservable(self, tupleObservable: TupleDataObservableHandler):
         self._tupleObservable = tupleObservable
 
     def start(self):
         (
             self._tupleObserver.subscribeToTupleSelector(
-                TupleSelector(ModelCoordSet.tupleName(), {})
+                TupleSelector(ModelSet.tupleName(), {})
             ).subscribe(self._processNewTuples)
         )
 
     def shutdown(self):
         self._tupleObservable = None
         self._tupleObserver = None
-        self._coordSetCache = {}
+        self._cache = {}
+        self._vortexMsgCache = None
 
-    def _processNewTuples(self, coordSetTuples):
-        if not coordSetTuples:
+    def _processNewTuples(self, tuples):
+        if not tuples:
             return
 
-        self._coordSetCache = {c.id: c for c in coordSetTuples}
+        self._cache = {c.id: c for c in tuples}
+
+        self._vortexMsgCache = None
 
         self._tupleObservable.notifyOfTupleUpdate(
-            TupleSelector(ModelCoordSet.tupleName(), {})
+            TupleSelector(ModelSet.tupleName(), {})
         )
 
     @property
-    def coordSets(self) -> List[ModelCoordSet]:
-        return list(self._coordSetCache.values())
+    def modelSets(self) -> List[ModelSet]:
+        return list(self._cache.values())
 
-    def coordSetForId(self, coordSetId: int) -> Optional[ModelCoordSet]:
-        return self._coordSetCache.get(coordSetId)
+    def cachedVortexMsgBlocking(self, filt: dict) -> bytes:
+        if self._vortexMsgCache:
+            return self._vortexMsgCache
+
+        data = self.modelSets
+
+        # Create the vortex message
+        vortexMsg = (
+            Payload(filt, tuples=data).makePayloadEnvelope().toVortexMsg()
+        )
+        self._vortexMsgCache = vortexMsg
+        return vortexMsg
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/controller/GridCacheController.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/controller/GridCacheController.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,26 +41,27 @@
 
     """
 
     _ChunkedTuple = EncodedGridTuple
     _UpdateDateTupleABC = GridUpdateDateTuple
     _chunkLoadRpcMethod = ClientGridLoaderRpc.loadGrids
     _chunkIndexDeltaRpcMethod = ClientGridLoaderRpc.loadGridsIndexDelta
-    _updateFromServerFilt = clientGridUpdateFromServerFilt
+    _updateFromLogicFilt = clientGridUpdateFromServerFilt
     _logger = logger
 
     #: This stores the cache of grid data for the clients
     _cache: Dict[str, GridTuple] = None
 
-    _LOAD_CHUNK_SIZE = 75
-    _LOAD_CHUNK_PARALLELISM = 4
-
     def __init__(self, clientId: str, pluginDataDir: Path):
         ACICacheControllerABC.__init__(self, clientId, pluginDataDir)
 
+        self._loadFromLogicMixin._LOAD_CHUNK_SIZE = 75
+        self._loadFromLogicMixin._LOAD_CHUNK_INITIAL_PARALLELISM = 4
+        self._loadFromLogicMixin._LOAD_CHUNK_UPDATE_PARALLELISM = 1
+
         self._coordSetEndpoint = PayloadEndpoint(
             clientCoordSetUpdateFromServerFilt, self._processCoordSetPayload
         )
 
     def _processCoordSetPayload(self, *args, **kwargs):
         d: Deferred = self.reloadCache()
         d.addErrback(vortexLogFailure, logger, consumeError=True)
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/controller/LocationIndexCacheController.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/controller/LocationIndexCacheController.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,9 +32,9 @@
 
     _ChunkedTuple = EncodedLocationIndexTuple
     _UpdateDateTupleABC = LocationIndexUpdateDateTuple
     _chunkLoadRpcMethod = ClientLocationIndexLoaderRpc.loadLocationIndexes
     _chunkIndexDeltaRpcMethod = (
         ClientLocationIndexLoaderRpc.loadLocationIndexDelta
     )
-    _updateFromServerFilt = clientLocationIndexUpdateFromServerFilt
+    _updateFromLogicFilt = clientLocationIndexUpdateFromServerFilt
     _logger = logger
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/controller/LookupCacheController.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/controller/LookupCacheController.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from copy import copy
 from typing import List
 
+from vortex.Payload import Payload
 from vortex.TupleSelector import TupleSelector
 from vortex.handler.TupleDataObservableHandler import TupleDataObservableHandler
 from vortex.handler.TupleDataObserverClient import TupleDataObserverClient
 
 from peek_plugin_diagram._private.PluginNames import diagramFilt
-from peek_plugin_diagram._private.storage.Display import DispColor
-from peek_plugin_diagram._private.storage.Display import DispLayer
-from peek_plugin_diagram._private.storage.Display import DispLevel
-from peek_plugin_diagram._private.storage.Display import DispLineStyle
-from peek_plugin_diagram._private.storage.Display import DispTextStyle
+from peek_plugin_diagram._private.storage.Lookups import DispColor
+from peek_plugin_diagram._private.storage.Lookups import DispLayer
+from peek_plugin_diagram._private.storage.Lookups import DispLevel
+from peek_plugin_diagram._private.storage.Lookups import DispLineStyle
+from peek_plugin_diagram._private.storage.Lookups import DispTextStyle
 
 lookupCachePayloadFilt = dict(key="client.lookup.update")
 lookupCachePayloadFilt.update(diagramFilt)
 
 
 class LookupCacheController:
     """Lookup Cache Controller
@@ -29,14 +30,15 @@
     _colorLookups: List[DispColor] = None
     _lineStyleLookups: List[DispLineStyle] = None
     _textStyleLookups: List[DispTextStyle] = None
 
     def __init__(self, tupleObserver: TupleDataObserverClient):
         self._tupleObserver = tupleObserver
         self._tupleObservable = None
+        self._vortexMsgCache: dict[str, bytes] = {}
 
     def setTupleObservable(self, tupleObservable: TupleDataObservableHandler):
         self._tupleObservable = tupleObservable
 
     def start(self):
         (
             self._tupleObserver.subscribeToTupleSelector(
@@ -68,22 +70,23 @@
             ).subscribe(self._processNewTuples)
         )
 
     def shutdown(self):
         self._tupleObservable = None
         self._tupleObserver = None
 
+        self._vortexMsgCache = {}
+
         self._levelLookups = []
         self._layerLookups = []
         self._colorLookups = []
         self._lineStyleLookups = []
         self._textStyleLookups = []
 
     def _processNewTuples(self, lookupTuples):
-
         if not lookupTuples:
             return
 
         firstTupleType = lookupTuples[0].tupleType()
         if DispLevel.tupleType() == firstTupleType:
             self._levelLookups = lookupTuples
 
@@ -100,14 +103,16 @@
             self._textStyleLookups = lookupTuples
 
         else:
             raise NotImplementedError(
                 "Cache not implemented for %s" % firstTupleType
             )
 
+        self._vortexMsgCache.pop(firstTupleType, None)
+
         self._tupleObservable.notifyOfTupleUpdate(
             TupleSelector(firstTupleType, {})
         )
 
     def lookups(self, lookupTupleType) -> List:
         if DispLevel.tupleType() == lookupTupleType:
             return copy(self._levelLookups)
@@ -123,7 +128,22 @@
 
         if DispTextStyle.tupleType() == lookupTupleType:
             return copy(self._textStyleLookups)
 
         raise NotImplementedError(
             "Cache not implemented for %s" % lookupTupleType
         )
+
+    def cachedVortexMsgBlocking(
+        self, lookupTupleType: str, filt: dict
+    ) -> bytes:
+        if lookupTupleType in self._vortexMsgCache:
+            return self._vortexMsgCache[lookupTupleType]
+
+        data = self.lookups(lookupTupleType=lookupTupleType)
+
+        # Create the vortex message
+        vortexMsg = (
+            Payload(filt, tuples=data).makePayloadEnvelope().toVortexMsg()
+        )
+        self._vortexMsgCache[lookupTupleType] = vortexMsg
+        return vortexMsg
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/handlers/BranchIndexCacheHandler.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/handlers/BranchIndexCacheHandler.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/handlers/GridCacheHandler.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/handlers/GridCacheHandler.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import logging
 from collections import defaultdict
 from datetime import datetime
 from typing import Dict
 from typing import List
 
+import pytz
 from twisted.internet.defer import Deferred
 from twisted.internet.defer import DeferredList
 from twisted.internet.defer import inlineCallbacks
 from vortex.DeferUtil import vortexLogFailure
 from vortex.Payload import Payload
 from vortex.PayloadEnvelope import PayloadEnvelope
 from vortex.VortexABC import SendVortexMsgResponseCallable
-from vortex.VortexFactory import VortexFactory
+from vortex.VortexFactory import VortexFactory, NoVortexException
 
 from peek_abstract_chunked_index.private.client.handlers.ACICacheHandlerABC import (
     ACICacheHandlerABC,
 )
 from peek_abstract_chunked_index.private.tuples.ACIUpdateDateTupleABC import (
     ACIUpdateDateTupleABC,
 )
@@ -88,14 +89,15 @@
             del self._observedGridKeysByVortexUuid[vortexUuid]
 
         self._rebuildStructs()
 
     # ---------------
     # Process update from the server
 
+    @inlineCallbacks
     def notifyOfUpdate(self, gridKeys: List[str]):
         """Notify of Grid Updates
 
         This method is called by the client.GridCacheController when it receives updates
         from the server.
 
         """
@@ -123,53 +125,59 @@
                     "Sending unsolicited grid %s to vortex %s",
                     gridKey,
                     vortexUuid,
                 )
                 payloadsByVortexUuid[vortexUuid].data.append(gridTuple)
 
         # Send the updates to the clients
-        dl = []
-        for vortexUuid, payloadEnvelope in list(payloadsByVortexUuid.items()):
+        for vortexUuid, payloadEnvelope in payloadsByVortexUuid.items():
             payloadEnvelope.filt = clientGridWatchUpdateFromDeviceFilt
 
-            # Serliase in thread, and then send.
-            d = payloadEnvelope.toVortexMsgDefer(base64Encode=False)
-            d.addCallback(
-                VortexFactory.sendVortexMsg, destVortexUuid=vortexUuid
+            vortexMsg = yield payloadEnvelope.toVortexMsgDefer(
+                base64Encode=False
             )
-            dl.append(d)
 
-        # Log the errors, otherwise we don't care about them
-        dl = DeferredList(dl, fireOnOneErrback=True)
-        dl.addErrback(vortexLogFailure, logger, consumeError=True)
+            try:
+                yield VortexFactory.sendVortexMsg(
+                    vortexMsg, destVortexUuid=vortexUuid
+                )
+
+            except NoVortexException:
+                pass
+            except Exception as e:
+                self._logger.exception(e)
 
     # ---------------
     # Process observes from the devices
 
     @inlineCallbacks
     def _processObserve(
         self,
         payloadEnvelope: PayloadEnvelope,
         vortexUuid: str,
         sendResponse: SendVortexMsgResponseCallable,
         **kwargs
     ):
-        cacheAll = payloadEnvelope.filt.get("cacheAll") == True
+        cacheAll = payloadEnvelope.filt.get("cacheAll") is True
 
         payload = yield payloadEnvelope.decodePayloadDefer()
 
         lastUpdateByGridKey: DeviceGridT = payload.tuples[0]
 
         if not cacheAll:
             gridKeys = list(lastUpdateByGridKey.keys())
             self._observedGridKeysByVortexUuid[vortexUuid] = gridKeys
             self._rebuildStructs()
 
-        self._replyToObserve(
-            payload.filt, lastUpdateByGridKey, sendResponse, cacheAll=cacheAll
+        yield self._replyToObserve(
+            payload.filt,
+            lastUpdateByGridKey,
+            sendResponse,
+            vortexUuid=vortexUuid,
+            cacheAll=cacheAll,
         )
 
     def _rebuildStructs(self) -> None:
         """Rebuild Structs
 
         Rebuild the reverse index of uuids by grid key.
 
@@ -193,69 +201,89 @@
                 gridKeys=list(self._observedVortexUuidsByGridKey),
             )
             d.addErrback(vortexLogFailure, logger, consumeError=False)
 
     # ---------------
     # Reply to device observe
 
+    @inlineCallbacks
     def _replyToObserve(
         self,
         filt,
         lastUpdateByGridKey: DeviceGridT,
         sendResponse: SendVortexMsgResponseCallable,
+        vortexUuid: str,
         cacheAll=False,
     ) -> None:
         """Reply to Observe
 
         The client has told us that it's observing a new set of grids, and the lastUpdate
         it has for each of those grids. We will send them the grids that are out of date
         or missing.
 
         :param filt: The payload filter to respond to.
         :param lastUpdateByGridKey: The dict of gridKey:lastUpdate
         :param sendResponse: The callable provided by the Vortex (handy)
         :returns: None
 
         """
+        startTime = datetime.now(pytz.utc)
         gridTuplesToSend = []
-
-        def sendChunk(toSend):
-            if not toSend and not cacheAll:
-                return
-
-            payloadEnvelope = PayloadEnvelope(filt=filt, data=toSend)
-            d: Deferred = payloadEnvelope.toVortexMsgDefer(base64Encode=False)
-            d.addCallback(sendResponse)
-            d.addErrback(vortexLogFailure, logger, consumeError=True)
+        updateCount = 0
+        sameCount = 0
+        deletedCount = 0
 
         # Check and send any updates
         for gridKey, lastUpdate in lastUpdateByGridKey.items():
             # NOTE: lastUpdate can be null.
             gridTuple = self._cacheController.encodedChunk(gridKey)
 
             # Last update is not null, we need to send an empty grid.
             if not gridTuple:
+                deletedCount += 1
                 gridTuple = EncodedGridTuple()
                 gridTuple.gridKey = gridKey
                 gridTuple.lastUpdate = lastUpdate
                 gridTuple.encodedGridTuple = None
                 gridTuplesToSend.append(gridTuple)
-                logger.debug(
-                    "Grid %s is no longer in the cache, %s", gridKey, lastUpdate
-                )
+
+                if self._DEBUG_LOGGING:
+                    logger.debug(
+                        "Grid %s is no longer in the cache, %s",
+                        gridKey,
+                        lastUpdate,
+                    )
 
             elif gridTuple.lastUpdate == lastUpdate:
-                logger.debug(
-                    "Grid %s matches the cache, %s", gridKey, lastUpdate
-                )
+                sameCount += 1
+                if self._DEBUG_LOGGING:
+                    logger.debug(
+                        "Grid %s matches the cache, %s", gridKey, lastUpdate
+                    )
 
             else:
+                updateCount += 1
                 gridTuplesToSend.append(gridTuple)
-                logger.debug(
-                    "Sending grid %s from the cache, %s", gridKey, lastUpdate
-                )
+                if self._DEBUG_LOGGING:
+                    logger.debug(
+                        "Sending grid %s from the cache, %s",
+                        gridKey,
+                        lastUpdate,
+                    )
 
             if len(gridTuplesToSend) == 5 and not cacheAll:
-                sendChunk(gridTuplesToSend)
+                yield self._sendData(
+                    sendResponse, filt, cacheAll, gridTuplesToSend
+                )
                 gridTuplesToSend = []
 
-        sendChunk(gridTuplesToSend)
+        yield self._sendData(sendResponse, filt, cacheAll, gridTuplesToSend)
+
+        logger.debug(
+            "Sent %s updates and %s deletes, %s matched/not sent"
+            " to %s in %s",
+            updateCount,
+            deletedCount,
+            sameCount,
+            vortexUuid,
+            datetime.now(pytz.utc) - startTime,
+        )
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/handlers/LocationIndexCacheHandler.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/handlers/LocationIndexCacheHandler.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/tuple_providers/BranchIndexUpdateDateTupleProvider.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/tuple_providers/BranchIndexUpdateDateTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/tuple_providers/BranchTupleProvider.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/tuple_providers/BranchTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/tuple_providers/ClientDispKeyLocationTupleProvider.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/tuple_providers/ClientDispKeyLocationTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/tuple_providers/ClientGroupDispsTupleProvider.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/tuple_providers/ClientGroupDispsTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/tuple_providers/ClientLocationIndexUpdateDateTupleProvider.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/tuple_providers/ClientLocationIndexUpdateDateTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/tuple_providers/ClientLookupTupleProvider.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/tuple_providers/DiagramLoaderStatusTupleProvider.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 import logging
 from typing import Union
 
-from twisted.internet.defer import Deferred
-from twisted.internet.defer import inlineCallbacks
+from twisted.internet.defer import Deferred, inlineCallbacks
+
+from peek_plugin_diagram._private.server.controller.StatusController import (
+    StatusController,
+)
 from vortex.Payload import Payload
 from vortex.TupleSelector import TupleSelector
 from vortex.handler.TupleDataObservableHandler import TuplesProviderABC
 
-from peek_plugin_diagram._private.client.controller.LookupCacheController import (
-    LookupCacheController,
-)
-
 logger = logging.getLogger(__name__)
 
 
-class ClientLookupTupleProvider(TuplesProviderABC):
-    def __init__(self, lookupCacheController: LookupCacheController):
-        self._lookupCacheController = lookupCacheController
+class DiagramLoaderStatusTupleProvider(TuplesProviderABC):
+    def __init__(self, statusController: StatusController):
+        self._statusController = statusController
 
     @inlineCallbacks
     def makeVortexMsg(
         self, filt: dict, tupleSelector: TupleSelector
     ) -> Union[Deferred, bytes]:
-        tuples = self._lookupCacheController.lookups(tupleSelector.name)
+        tuples = [self._statusController.status]
 
-        payloadEnvelope = yield Payload(
-            filt, tuples=tuples
-        ).makePayloadEnvelopeDefer()
+        payloadEnvelope = yield Payload(filt, tuples=tuples).makePayloadEnvelopeDefer()
         vortexMsg = yield payloadEnvelope.toVortexMsgDefer()
         return vortexMsg
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/tuple_providers/ClientModelSetTupleProvider.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/tuple_providers/ServerModelSetTupleProvider.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import logging
 from typing import Union
 
 from twisted.internet.defer import Deferred
-from twisted.internet.defer import inlineCallbacks
+
+from peek_plugin_diagram._private.storage.ModelSet import ModelSet
+from vortex.DeferUtil import deferToThreadWrapWithLogger
 from vortex.Payload import Payload
 from vortex.TupleSelector import TupleSelector
 from vortex.handler.TupleDataObservableHandler import TuplesProviderABC
 
-from peek_plugin_diagram._private.client.controller.ModelSetCacheController import (
-    ModelSetCacheController,
-)
-
 logger = logging.getLogger(__name__)
 
 
-class ClientModelSetTupleProvider(TuplesProviderABC):
-    def __init__(self, modelSetCacheController: ModelSetCacheController):
-        self.modelSetCacheController = modelSetCacheController
+class ServerModelSetTupleProvider(TuplesProviderABC):
+    def __init__(self, ormSessionCreator):
+        self._ormSessionCreator = ormSessionCreator
 
-    @inlineCallbacks
+    @deferToThreadWrapWithLogger(logger)
     def makeVortexMsg(
         self, filt: dict, tupleSelector: TupleSelector
     ) -> Union[Deferred, bytes]:
-        tuples = self.modelSetCacheController.modelSets
 
-        payloadEnvelope = yield Payload(
-            filt, tuples=tuples
-        ).makePayloadEnvelopeDefer()
-        vortexMsg = yield payloadEnvelope.toVortexMsgDefer()
-        return vortexMsg
+        session = self._ormSessionCreator()
+        try:
+            tuples = session.query(ModelSet).all()
+            return Payload(filt, tuples=tuples).makePayloadEnvelope().toVortexMsg()
+
+        finally:
+            session.close()
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/client/tuple_providers/GridCacheIndexTupleProvider.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/client/tuple_providers/GridCacheIndexTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/LogicEntryHook.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/LogicEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/TupleActionProcessor.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/TupleActionProcessor.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/TupleDataObservable.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/TupleDataObservable.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,21 +22,19 @@
 )
 from peek_plugin_diagram._private.server.tuple_providers.ServerLookupTupleProvider import (
     ServerLookupTupleProvider,
 )
 from peek_plugin_diagram._private.server.tuple_providers.ServerModelSetTupleProvider import (
     ServerModelSetTupleProvider,
 )
-from peek_plugin_diagram._private.storage.Display import (
-    DispLevel,
-    DispLayer,
-    DispColor,
-    DispLineStyle,
-    DispTextStyle,
-)
+from peek_plugin_diagram._private.storage.Lookups import DispColor
+from peek_plugin_diagram._private.storage.Lookups import DispLineStyle
+from peek_plugin_diagram._private.storage.Lookups import DispTextStyle
+from peek_plugin_diagram._private.storage.Lookups import DispLevel
+from peek_plugin_diagram._private.storage.Lookups import DispLayer
 from peek_plugin_diagram._private.storage.ModelSet import ModelCoordSet, ModelSet
 from peek_plugin_diagram._private.tuples.DiagramImporterStatusTuple import (
     DiagramImporterStatusTuple,
 )
 from peek_plugin_diagram._private.tuples.branch.BranchKeyToIdMapTuple import (
     BranchKeyToIdMapTuple,
 )
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/admin_handlers/SettingPropertyHandler.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/admin_handlers/SettingPropertyHandler.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/admin_handlers/StringIntTableHandler.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/admin_handlers/StringIntTableHandler.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/api/DiagramApi.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/api/DiagramApi.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/api/DiagramImportApi.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/api/DiagramImportApi.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/api/DiagramViewerApi.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/api/DiagramViewerApi.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/client_handlers/BranchIndexChunkLoadRpc.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/client_handlers/BranchIndexChunkLoadRpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,30 +33,30 @@
         yield self.loadBranchIndexDelta.start(funcSelf=self)
         logger.debug("RPCs started")
 
     # -------------
     @vortexRPC(
         peekServerName,
         acceptOnlyFromVortex=peekBackendNames,
-        timeoutSeconds=60,
+        timeoutSeconds=120,
         additionalFilt=diagramFilt,
         deferToThread=True,
     )
     def loadBranchIndexDelta(self, indexEncodedPayload: bytes) -> bytes:
         return self.ckiChunkIndexDeltaBlocking(
             indexEncodedPayload,
             BranchIndexEncodedChunk,
             BranchIndexUpdateDateTuple,
         )
 
     # -------------
     @vortexRPC(
         peekServerName,
         acceptOnlyFromVortex=peekBackendNames,
-        timeoutSeconds=60,
+        timeoutSeconds=120,
         additionalFilt=diagramFilt,
         deferToThread=True,
     )
     def loadBranchIndexChunks(self, chunkKeys: list[str]) -> list[Tuple]:
         """Update Page Loader Status
 
         Tell the server of the latest status of the loader
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/client_handlers/BranchIndexChunkUpdateHandler.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/client_handlers/BranchIndexChunkUpdateHandler.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/client_handlers/ClientGridLoaderRpc.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/client_handlers/ClientGridLoaderRpc.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/client_handlers/ClientGridUpdateHandler.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/client_handlers/ClientGridUpdateHandler.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/client_handlers/ClientLocationIndexLoaderRpc.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/client_handlers/ClientLocationIndexLoaderRpc.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,30 +35,30 @@
         yield self.loadLocationIndexes.start(funcSelf=self)
         logger.debug("RPCs started")
 
     # -------------
     @vortexRPC(
         peekServerName,
         acceptOnlyFromVortex=peekBackendNames,
-        timeoutSeconds=60,
+        timeoutSeconds=120,
         additionalFilt=diagramFilt,
         deferToThread=True,
     )
     def loadLocationIndexDelta(self, indexEncodedPayload: bytes) -> bytes:
         return self.ckiChunkIndexDeltaBlocking(
             indexEncodedPayload,
             LocationIndexCompiled,
             LocationIndexUpdateDateTuple,
         )
 
     # -------------
     @vortexRPC(
         peekServerName,
         acceptOnlyFromVortex=peekBackendNames,
-        timeoutSeconds=60,
+        timeoutSeconds=120,
         additionalFilt=diagramFilt,
         deferToThread=True,
     )
     def loadLocationIndexes(self, chunkKeys: list[str]) -> list[Tuple]:
         """Update Page Loader Status
 
         Tell the server of the latest status of the loader
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/client_handlers/ClientLocationIndexUpdateHandler.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/client_handlers/ClientLocationIndexUpdateHandler.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/controller/BranchIndexCompilerQueueController.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/controller/BranchIndexCompilerQueueController.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,20 +28,26 @@
 
 
 class _Notifier(ACIProcessorStatusNotifierABC):
     def __init__(self, adminStatusController: StatusController):
         self._adminStatusController = adminStatusController
 
     def setProcessorStatus(self, state: bool, queueSize: int):
-        self._adminStatusController.status.branchIndexCompilerQueueStatus = state
-        self._adminStatusController.status.branchIndexCompilerQueueSize = queueSize
+        self._adminStatusController.status.branchIndexCompilerQueueStatus = (
+            state
+        )
+        self._adminStatusController.status.branchIndexCompilerQueueSize = (
+            queueSize
+        )
         self._adminStatusController.notify()
 
     def addToProcessorTotal(self, delta: int):
-        self._adminStatusController.status.branchIndexCompilerProcessedTotal += delta
+        self._adminStatusController.status.branchIndexCompilerProcessedTotal += (
+            delta
+        )
         self._adminStatusController.notify()
 
     def setProcessorError(self, error: str):
         self._adminStatusController.status.branchIndexCompilerLastError = error
         self._adminStatusController.notify()
 
 
@@ -68,18 +74,20 @@
         statusController: StatusController,
         clientUpdateHandler: BranchIndexChunkUpdateHandler,
     ):
         ACIProcessorQueueControllerABC.__init__(
             self, dbSessionCreator, _Notifier(statusController)
         )
 
-        self._clientUpdateHandler: BranchIndexChunkUpdateHandler = clientUpdateHandler
+        self._clientUpdateHandler: BranchIndexChunkUpdateHandler = (
+            clientUpdateHandler
+        )
 
     def _sendToWorker(self, block: ACIProcessorQueueBlockItem):
-        from peek_plugin_diagram._private.worker.tasks.branch.BranchIndexCompiler import (
+        from peek_plugin_diagram._private.worker.tasks.branch.BranchIndexCompilerTask import (
             compileBranchIndexChunk,
         )
 
         return compileBranchIndexChunk.delay(block.itemsEncodedPayload)
 
     def _processWorkerResults(self, results):
         self._clientUpdateHandler.sendChunks(results)
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/controller/BranchLiveEditController.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/controller/BranchLiveEditController.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/controller/BranchUpdateController.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/controller/BranchUpdateController.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 from peek_plugin_diagram._private.tuples.branch.BranchLiveEditTuple import (
     BranchLiveEditTuple,
 )
 from peek_plugin_diagram._private.tuples.branch.BranchTuple import BranchTuple
 from peek_plugin_diagram._private.tuples.branch.BranchUpdateTupleAction import (
     BranchUpdateTupleAction,
 )
-from peek_plugin_diagram._private.worker.tasks.branch.BranchIndexImporter import (
+from peek_plugin_diagram._private.worker.tasks.branch.BranchIndexImporterTask import (
     createOrUpdateBranches,
 )
-from peek_plugin_diagram._private.worker.tasks.branch.BranchIndexUpdater import (
+from peek_plugin_diagram._private.worker.tasks.branch.BranchIndexUpdaterTask import (
     updateBranches,
 )
 from peek_plugin_livedb.server.LiveDBWriteApiABC import LiveDBWriteApiABC
 from twisted.internet import defer
 from twisted.internet.defer import inlineCallbacks, Deferred
 from vortex.DeferUtil import vortexLogAndConsumeFailure
 from vortex.Payload import Payload
@@ -81,29 +81,33 @@
         )
 
         d = self.__processUpdateFromClient(tupleAction)
         d.addErrback(vortexLogAndConsumeFailure, logger)
         return defer.succeed([])
 
     @inlineCallbacks
-    def __processUpdateFromClient(self, tupleAction: TupleActionABC) -> Deferred:
+    def __processUpdateFromClient(
+        self, tupleAction: TupleActionABC
+    ) -> Deferred:
 
         dbSession = self._dbSessionCreator()
         try:
             encodedPayload = yield Payload(
                 tuples=[tupleAction.branchTuple]
             ).toEncodedPayloadDefer()
 
             yield updateBranches.delay(tupleAction.modelSetId, encodedPayload)
 
             # Load the branch from the DB and tell the LiveDb update
             # that there is an update.
             branchIndex = (
                 dbSession.query(BranchIndex)
-                .filter(BranchIndex.coordSetId == tupleAction.branchTuple.coordSetId)
+                .filter(
+                    BranchIndex.coordSetId == tupleAction.branchTuple.coordSetId
+                )
                 .filter(BranchIndex.key == tupleAction.branchTuple.key)
                 .one()
             )
 
             branchTuple = BranchTuple.loadFromJson(
                 branchIndex.packedJson,
                 branchIndex.importHash,
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/controller/DispCompilerQueueController.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/controller/DispCompilerQueueController.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/controller/DispImportController.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/controller/DispImportController.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/controller/GridKeyCompilerQueueController.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/controller/GridKeyCompilerQueueController.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/controller/LiveDbWatchController.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/controller/LiveDbWatchController.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/controller/LocationCompilerQueueController.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/controller/LocationCompilerQueueController.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/controller/LookupImportController.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/controller/LookupImportController.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,21 +4,19 @@
 
 from twisted.internet.defer import (
     inlineCallbacks,
     returnValue,
     DeferredSemaphore,
 )
 
-from peek_plugin_diagram._private.storage.Display import (
-    DispColor,
-    DispLayer,
-    DispLevel,
-    DispLineStyle,
-    DispTextStyle,
-)
+from peek_plugin_diagram._private.storage.Lookups import DispColor
+from peek_plugin_diagram._private.storage.Lookups import DispLineStyle
+from peek_plugin_diagram._private.storage.Lookups import DispTextStyle
+from peek_plugin_diagram._private.storage.Lookups import DispLevel
+from peek_plugin_diagram._private.storage.Lookups import DispLayer
 from peek_plugin_diagram._private.storage.ModelSet import (
     getOrCreateModelSet,
     getOrCreateCoordSet,
 )
 from peek_plugin_diagram.tuples.lookups.ImportDispColorTuple import (
     ImportDispColorTuple,
 )
@@ -63,15 +61,14 @@
         modelSetKey: str,
         coordSetKey: Optional[str],
         lookupTupleType: str,
         lookupTuples: List,
         deleteOthers: bool,
         updateExisting: bool,
     ):
-
         yield self._semaphore.run(
             self._importInThread,
             modelSetKey,
             coordSetKey,
             lookupTupleType,
             lookupTuples,
             deleteOthers,
@@ -101,15 +98,14 @@
 
         addCount = 0
         updateCount = 0
         deleteCount = 0
 
         ormSession = self._dbSessionCreator()
         try:
-
             modelSet = getOrCreateModelSet(ormSession, modelSetKey)
             coordSet = None
 
             if coordSetKey:
                 coordSet = getOrCreateCoordSet(
                     ormSession, modelSetKey, coordSetKey
                 )
@@ -203,20 +199,18 @@
         finally:
             ormSession.close()
 
     @deferToThreadWrapWithLogger(logger)
     def getLookups(
         self, modelSetKey: str, coordSetKey: Optional[str], tupleType: str
     ):
-
         LookupType = ORM_TUPLE_MAP[tupleType]
 
         ormSession = self._dbSessionCreator()
         try:
-
             modelSet = getOrCreateModelSet(ormSession, modelSetKey)
 
             if coordSetKey:
                 coordSet = getOrCreateCoordSet(
                     ormSession, modelSetKey, coordSetKey
                 )
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/tuple_providers/BranchKeyToIdMapProvider.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/tuple_providers/BranchKeyToIdMapProvider.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/tuple_providers/BranchLiveEditTupleProvider.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/tuple_providers/BranchLiveEditTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/tuple_providers/ServerCoordSetTupleProvider.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/tuple_providers/ServerCoordSetTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/server/tuple_providers/ServerLookupTupleProvider.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/server/tuple_providers/ServerLookupTupleProvider.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import logging
 from typing import Union
 
 from sqlalchemy.orm import joinedload
 from twisted.internet.defer import Deferred
-
-from peek_plugin_diagram._private.storage.Display import DispLevel
-from peek_plugin_diagram._private.storage.ModelSet import ModelCoordSet
 from vortex.DeferUtil import deferToThreadWrapWithLogger
 from vortex.Payload import Payload
 from vortex.Tuple import TUPLE_TYPES_BY_NAME
 from vortex.TupleSelector import TupleSelector
 from vortex.handler.TupleDataObservableHandler import TuplesProviderABC
 
+from peek_plugin_diagram._private.storage.Lookups import DispLevel
+from peek_plugin_diagram._private.storage.ModelSet import ModelCoordSet
+
 logger = logging.getLogger(__name__)
 
 
 class ServerLookupTupleProvider(TuplesProviderABC):
     def __init__(self, ormSessionCreator):
         self._ormSessionCreator = ormSessionCreator
 
@@ -34,20 +34,21 @@
                         joinedload(DispLevel.coordSet).joinedload(
                             ModelCoordSet.modelSet
                         )
                     )
                     .all()
                 )
 
-                for item in all:
-                    item.data = {"modelSetKey": item.coordSet.modelSet.key}
-
             else:
-                all = session.query(Lookup).options(joinedload(Lookup.modelSet)).all()
+                all = (
+                    session.query(Lookup)
+                    .options(joinedload(Lookup.modelSet))
+                    .all()
+                )
 
-                for item in all:
-                    item.data = {"modelSetKey": item.modelSet.key}
+            for item in all:
+                item.setTupleFields()
 
             return Payload(filt, tuples=all).makePayloadEnvelope().toVortexMsg()
 
         finally:
             session.close()
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/storage/DeclarativeBase.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/storage/DeclarativeBase.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/storage/DispIndex.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/storage/DispIndex.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/storage/Display.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/storage/Display.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,20 +14,25 @@
 
 from peek_plugin_diagram._private.PluginNames import diagramTuplePrefix
 from sqlalchemy import Column, orm, BigInteger, SmallInteger
 from sqlalchemy import ForeignKey
 from sqlalchemy import Integer, String, Boolean
 from sqlalchemy.orm import relationship
 from sqlalchemy.orm.mapper import reconstructor
-from sqlalchemy.sql.schema import Index, Sequence
+from sqlalchemy.sql.schema import Index
 from sqlalchemy.sql.sqltypes import Float, DateTime
 from vortex.Tuple import Tuple, addTupleType, TupleField, JSON_EXCLUDE
 
 from .DeclarativeBase import DeclarativeBase
-from .ModelSet import ModelCoordSet, ModelSet
+from .Lookups import DispColor
+from .Lookups import DispLayer
+from .Lookups import DispLevel
+from .Lookups import DispLineStyle
+from .Lookups import DispTextStyle
+from .ModelSet import ModelCoordSet
 from .branch.BranchIndex import BranchIndex
 
 DISP_SHORT_ATTR_NAME_MAP = {
     "colorId": "c",
     "fillColorId": "fc",
     "borderColorId": "bc",
     "lineColorId": "lc",
@@ -35,200 +40,14 @@
     "lineWidth": "w",
     "text": "te",
     "groupId": "gi",
     "targetGroupId": "tg",
 }
 
 
-@addTupleType
-class DispLayer(Tuple, DeclarativeBase):
-    __tablename__ = "DispLayer"
-    __tupleTypeShort__ = "DLA"
-    __tupleType__ = diagramTuplePrefix + __tablename__
-
-    #: Misc data holder
-    data = TupleField()
-
-    id = Column(Integer, primary_key=True, autoincrement=True)
-    name = Column(String(50), nullable=False)
-    order = Column(Integer, nullable=False, server_default="0")
-    selectable = Column(Boolean, nullable=False, server_default="false")
-    visible = Column(Boolean, nullable=False, server_default="true")
-
-    modelSetId = Column(
-        Integer, ForeignKey("ModelSet.id", ondelete="CASCADE"), nullable=False
-    )
-    modelSet = relationship(ModelSet)
-
-    importHash = Column(String(100), doc=JSON_EXCLUDE)
-
-    showForEdit = Column(Boolean, nullable=False)
-
-    blockApiUpdate = Column(Boolean, nullable=False)
-
-    __table_args__: typing.Tuple = (
-        Index("idx_DispLayer_modelSetId", modelSetId, unique=False),
-        Index("idx_DispLayer_importHash", modelSetId, importHash, unique=True),
-    )
-
-
-@addTupleType
-class DispLevel(Tuple, DeclarativeBase):
-    __tablename__ = "DispLevel"
-    __tupleTypeShort__ = "DLE"
-    __tupleType__ = diagramTuplePrefix + __tablename__
-
-    #: Misc data holder
-    data = TupleField()
-
-    id = Column(Integer, primary_key=True, autoincrement=True)
-    name = Column(String(50), nullable=False)
-    order = Column(Integer, nullable=False, server_default="0")
-    minZoom = Column(Float)
-    maxZoom = Column(Float)
-
-    coordSetId = Column(
-        Integer,
-        ForeignKey("ModelCoordSet.id", ondelete="CASCADE"),
-        nullable=False,
-    )
-    coordSet = relationship(ModelCoordSet, foreign_keys=[coordSetId])
-
-    importHash = Column(String(100), doc=JSON_EXCLUDE)
-
-    showForEdit = Column(Boolean, nullable=False)
-
-    blockApiUpdate = Column(Boolean, nullable=False)
-
-    __table_args__ = (
-        Index("idx_DispLevel_coordSetId", coordSetId, unique=False),
-        Index("idx_DispLevel_importHash", coordSetId, importHash, unique=True),
-    )
-
-
-@addTupleType
-class DispTextStyle(Tuple, DeclarativeBase):
-    __tupleTypeShort__ = "DTS"
-    __tablename__ = "DispTextStyle"
-    __tupleType__ = diagramTuplePrefix + __tablename__
-
-    #: Misc data holder
-    data = TupleField()
-
-    id = Column(Integer, primary_key=True, autoincrement=True)
-    name = Column(String(50), nullable=False)
-    fontName = Column(String(30), nullable=False, server_default="GillSans")
-    fontSize = Column(Integer, nullable=False, server_default="9")
-    fontStyle = Column(String(30))
-    scalable = Column(Boolean, nullable=False, server_default="true")
-    scaleFactor = Column(Integer, nullable=False, server_default="1")
-    spacingBetweenTexts = Column(Float, nullable=False, server_default="100")
-
-    modelSetId = Column(
-        Integer,
-        ForeignKey("ModelSet.id", ondelete="CASCADE"),
-        doc=JSON_EXCLUDE,
-        nullable=False,
-    )
-    modelSet = relationship(ModelSet)
-
-    importHash = Column(String(100), doc=JSON_EXCLUDE)
-
-    borderWidth = Column(Float, nullable=True)
-
-    showForEdit = Column(Boolean, nullable=False)
-
-    blockApiUpdate = Column(Boolean, nullable=False)
-
-    __table_args__ = (
-        Index("idx_DispTextStyle_modelSetId", modelSetId, unique=False),
-        Index(
-            "idx_DispTextStyle_importHash", modelSetId, importHash, unique=True
-        ),
-    )
-
-
-@addTupleType
-class DispLineStyle(Tuple, DeclarativeBase):
-    __tupleTypeShort__ = "DLS"
-    __tablename__ = "DispLineStyle"
-    __tupleType__ = diagramTuplePrefix + __tablename__
-
-    #: Misc data holder
-    data = TupleField()
-
-    id = Column(Integer, primary_key=True, autoincrement=True)
-    name = Column(String(50), nullable=False)
-    backgroundFillDashSpace = Column(
-        Boolean, nullable=False, server_default="false"
-    )
-    capStyle = Column(String(15), nullable=False)
-    joinStyle = Column(String(15), nullable=False)
-    dashPattern = Column(String(50))
-    startArrowSize = Column(Integer)
-    endArrowSize = Column(Integer)
-    winStyle = Column(Integer, nullable=False)
-
-    modelSetId = Column(
-        Integer,
-        ForeignKey("ModelSet.id", ondelete="CASCADE"),
-        doc=JSON_EXCLUDE,
-        nullable=False,
-    )
-    modelSet = relationship(ModelSet)
-
-    importHash = Column(String(100), doc=JSON_EXCLUDE)
-    scalable = Column(Boolean, nullable=False, server_default="false")
-
-    showForEdit = Column(Boolean, nullable=False)
-    blockApiUpdate = Column(Boolean, nullable=False)
-
-    __table_args__ = (
-        Index("idx_DispLineStyle_modelSetId", modelSetId, unique=False),
-        Index(
-            "idx_DispLineStyle_importHash", modelSetId, importHash, unique=True
-        ),
-    )
-
-
-@addTupleType
-class DispColor(Tuple, DeclarativeBase):
-    __tupleTypeShort__ = "DC"
-    __tablename__ = "DispColor"
-    __tupleType__ = diagramTuplePrefix + __tablename__
-
-    #: Misc data holder
-    data = TupleField()
-
-    id = Column(Integer, primary_key=True, autoincrement=True)
-    name = Column(String(50), doc=JSON_EXCLUDE, nullable=False)
-    color = Column(String(20), server_default="orange")
-    altColor = Column(String(20))
-    swapPeriod = Column(Float)
-
-    modelSetId = Column(
-        Integer,
-        ForeignKey("ModelSet.id", ondelete="CASCADE"),
-        doc=JSON_EXCLUDE,
-        nullable=False,
-    )
-    modelSet = relationship(ModelSet)
-
-    importHash = Column(String(100), doc=JSON_EXCLUDE)
-
-    showForEdit = Column(Boolean, nullable=False)
-
-    blockApiUpdate = Column(Boolean, nullable=False)
-
-    __table_args__ = (
-        Index("idx_DispColor_modelSetId", modelSetId, unique=False),
-        Index("idx_DispColor_importHash", modelSetId, importHash, unique=True),
-    )
-
-
 class DispBase(Tuple, DeclarativeBase):
     __tablename__ = "DispBase"
 
     # Types
     # Must align with constants in javascript DispBase class
     GROUP = 10
     GROUP_PTR = 11
@@ -328,14 +147,16 @@
         # Index("idx_Disp_importHash", importHash, unique=True),
         Index("idx_Disp_importUpdateDate", importUpdateDate, unique=False),
         Index("idx_Disp_layerId", layerId, unique=False),
         Index("idx_Disp_levelId", levelId, unique=False),
         Index("idx_Disp_coordSetId_", coordSetId, unique=False),
         Index("idx_Disp_groupId", groupId, unique=False),
         Index("idx_Disp_branchId", branchId, unique=False),
+        # We need this for the diagram API method getGridKeysFromShapeKeys
+        Index("idx_Disp_key", key, unique=False),
         # Index("idx_Disp_hashId", coordSetId, hashId, unique=True),
         # Index("idx_Disp_replacesHashId", replacesHashId),
     )
 
 
 @addTupleType
 class DispNull(DispBase):
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/storage/GridKeyIndex.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/storage/GridKeyIndex.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 
 from sqlalchemy import Column, BigInteger
 from sqlalchemy import ForeignKey
 from sqlalchemy import Integer, String
 from sqlalchemy.orm import relationship
 from sqlalchemy.sql.schema import Index
+from vortex.Payload import Payload
 from vortex.Tuple import Tuple, addTupleType
 
 from peek_abstract_chunked_index.private.tuples.ACIEncodedChunkTupleABC import (
     ACIEncodedChunkTupleABC,
 )
 from peek_abstract_chunked_index.private.tuples.ACIProcessorQueueTupleABC import (
     ACIProcessorQueueTupleABC,
@@ -112,14 +113,20 @@
         return self.gridKey
 
     @property
     def ckiEncodedData(self):
         return self.encodedGridTuple
 
     @property
+    def decodedDataBlocking(self) -> Payload:
+        if not self.ckiHasEncodedData:
+            return Payload()
+        return Payload().fromEncodedPayload(self.encodedGridTuple)
+
+    @property
     def ckiHasEncodedData(self) -> bool:
         return bool(self.encodedGridTuple)
 
     @property
     def ckiLastUpdate(self):
         return self.lastUpdate
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/storage/LiveDbDispLink.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/storage/LiveDbDispLink.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/storage/LocationIndex.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/storage/LocationIndex.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/storage/ModelSet.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/storage/ModelSet.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,41 +6,49 @@
  *  This software is proprietary, you are not free to copy
  *  or redistribute this code in any format.
  *
  *  All rights to this software are reserved by
  *  Synerty Pty Ltd
  *
 """
-from sqlalchemy.exc import IntegrityError
+import logging
 
-from peek_plugin_diagram._private.PluginNames import diagramTuplePrefix
 from sqlalchemy import Column
 from sqlalchemy import ForeignKey
-from sqlalchemy import Integer, String
+from sqlalchemy import Integer
+from sqlalchemy import String
+from sqlalchemy.exc import IntegrityError
 from sqlalchemy.orm import relationship
 from sqlalchemy.sql.schema import Index
 from sqlalchemy.sql.sqltypes import Boolean
 from sqlalchemy.types import Float
-from vortex.Tuple import addTupleType, Tuple, TupleField
+from vortex.Tuple import Tuple
+from vortex.Tuple import TupleField
+from vortex.Tuple import addTupleType
 
+from peek_plugin_diagram._private.PluginNames import diagramTuplePrefix
 from .DeclarativeBase import DeclarativeBase
 
+logger = logging.getLogger(__name__)
+
 
 @addTupleType
 class ModelSet(Tuple, DeclarativeBase):
     __tablename__ = "ModelSet"
     __tupleType__ = diagramTuplePrefix + __tablename__
 
     id = Column(Integer, primary_key=True, autoincrement=True)
     key = Column(String(50), nullable=False)
     name = Column(String(50), nullable=False)
     comment = Column(String)
 
     landingCoordSetId = Column(
-        Integer, ForeignKey("ModelCoordSet.id", ondelete="CASCADE"), nullable=True
+        Integer,
+        ForeignKey("ModelCoordSet.id", ondelete="CASCADE"),
+        nullable=True,
     )
 
     coordSets = relationship(
         "ModelCoordSet",
         remote_side="ModelCoordSet.modelSetId",
         primaryjoin="ModelSet.id==ModelCoordSet.modelSetId",
     )
@@ -75,15 +83,17 @@
         ModelSet,
         foreign_keys=[modelSetId],
         primaryjoin="ModelSet.id==ModelCoordSet.modelSetId",
     )
 
     # Grid size settings
     gridSizes = relationship(
-        "ModelCoordSetGridSize", lazy="subquery", order_by="ModelCoordSetGridSize.key"
+        "ModelCoordSetGridSize",
+        lazy="subquery",
+        order_by="ModelCoordSetGridSize.key",
     )
 
     minZoom = Column(Float, nullable=False, server_default="0.01")
     maxZoom = Column(Float, nullable=False, server_default="10.0")
 
     multiplierX = Column(Float, nullable=False, server_default="1")
     multiplierY = Column(Float, nullable=False, server_default="1")
@@ -97,18 +107,22 @@
     importId2 = Column(String(100))
 
     #: Misc data holder
     data = TupleField()
     isLanding = TupleField()
 
     #: Show this Coord Set as a group of DispGroups to choose from in the Editor
-    dispGroupTemplatesEnabled = Column(Boolean, nullable=False, server_default="false")
+    dispGroupTemplatesEnabled = Column(
+        Boolean, nullable=False, server_default="false"
+    )
 
     #: Show this Coord Set as a group of Line Templates to choose from in the Editor
-    edgeTemplatesEnabled = Column(Boolean, nullable=False, server_default="false")
+    edgeTemplatesEnabled = Column(
+        Boolean, nullable=False, server_default="false"
+    )
 
     #: Is Editing enabled? (Also ensure ALL editDefault fields are set.
     branchesEnabled = Column(Boolean, nullable=False, server_default="false")
 
     #: Is Editing enabled? (Also ensure ALL editDefault fields are set.
     editEnabled = Column(Boolean, nullable=False, server_default="false")
 
@@ -124,34 +138,46 @@
     #: Default Line for new shapes
     editDefaultLineStyleId = Column(Integer, ForeignKey("DispLineStyle.id"))
 
     #: Default Text for new shapes
     editDefaultTextStyleId = Column(Integer, ForeignKey("DispTextStyle.id"))
 
     #: Default Vertex/Node/Equipment Coord Set
-    editDefaultVertexCoordSetId = Column(Integer, ForeignKey("ModelCoordSet.id"))
+    editDefaultVertexCoordSetId = Column(
+        Integer, ForeignKey("ModelCoordSet.id")
+    )
     editDefaultVertexGroupName = Column(String)
 
     #: Default Edge/Conductor Coord Set
     editDefaultEdgeCoordSetId = Column(Integer, ForeignKey("ModelCoordSet.id"))
     editDefaultEdgeGroupName = Column(String)
 
     __table_args__ = (
         Index("idxCoordSetModelName", modelSetId, name, unique=True),
         Index("idxCoordSetImportId1", importId1, unique=False),
         Index("idxCoordSetImportId2", importId2, unique=False),
         Index("idxCoordModelSetId", modelSetId, unique=False),
-        Index("idxCoordModel_editDefaultLayerId", editDefaultLayerId, unique=False),
-        Index("idxCoordModel_editDefaultLevelId", editDefaultLevelId, unique=False),
-        Index("idxCoordModel_editDefaultColorId", editDefaultColorId, unique=False),
         Index(
-            "idxCoordModel_editDefaultLineStyleId", editDefaultLineStyleId, unique=False
+            "idxCoordModel_editDefaultLayerId", editDefaultLayerId, unique=False
+        ),
+        Index(
+            "idxCoordModel_editDefaultLevelId", editDefaultLevelId, unique=False
         ),
         Index(
-            "idxCoordModel_editDefaultTextStyleId", editDefaultTextStyleId, unique=False
+            "idxCoordModel_editDefaultColorId", editDefaultColorId, unique=False
+        ),
+        Index(
+            "idxCoordModel_editDefaultLineStyleId",
+            editDefaultLineStyleId,
+            unique=False,
+        ),
+        Index(
+            "idxCoordModel_editDefaultTextStyleId",
+            editDefaultTextStyleId,
+            unique=False,
         ),
         Index(
             "idxCoordModel_editDefaultVertexCoordSetId",
             editDefaultVertexCoordSetId,
             unique=False,
         ),
         Index(
@@ -181,19 +207,23 @@
     xGrid = Column(Integer, nullable=False)
     yGrid = Column(Integer, nullable=False)
 
     smallestTextSize = Column(Float, nullable=False, server_default="6.0")
     smallestShapeSize = Column(Float, nullable=False, server_default="2.0")
 
     coordSetId = Column(
-        Integer, ForeignKey("ModelCoordSet.id", ondelete="CASCADE"), nullable=False
+        Integer,
+        ForeignKey("ModelCoordSet.id", ondelete="CASCADE"),
+        nullable=False,
     )
     coordSet = relationship(ModelCoordSet)
 
-    __table_args__ = (Index("idx_CoordSetGridSize_key", coordSetId, key, unique=True),)
+    __table_args__ = (
+        Index("idx_CoordSetGridSize_key", coordSetId, key, unique=True),
+    )
 
     DEFAULT = [
         # These defaults are good for Aurora
         dict(
             min=0.0,
             max=0.04,
             key=0,
@@ -236,14 +266,26 @@
 
         coordSetId = ModelCoordSet.id
         gridSize = GridSize (above)
         x, y = Grid coordinates, top left
         """
         return "%s|%s.%sx%s" % (self.coordSetId, self.key, x, y)
 
+    @classmethod
+    def makeGridKeyStartsWith(cls, coordSetId: int, gridKeySize: int):
+        return "%s|%s." % (coordSetId, gridKeySize)
+
+    @classmethod
+    def gridSizeKeyFromGridKey(cls, gridKey: str):
+        try:
+            return int(gridKey.split("|")[1].split(".")[0])
+        except:
+            logger.error("Grid key [%s] is malformed", gridKey)
+            raise
+
 
 def makeDispGroupGridKey(coordSetId: int):
     """Make Disp Group Grid Key
 
     Make the special disp group grid key name.
     This is used to store all of the DispGroups that are not specifically stored in a
     grid, with the DispGroupPtr that uses it.
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/storage/Setting.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/storage/Setting.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/storage/branch/BranchIndex.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/storage/branch/BranchIndex.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/storage/branch/BranchIndexCompilerQueue.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/storage/branch/BranchIndexCompilerQueue.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/storage/branch/BranchIndexEncodedChunk.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/storage/branch/BranchIndexEncodedChunk.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/DiagramImporterStatusTuple.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/DiagramImporterStatusTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/GroupDispsTuple.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/GroupDispsTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/__init__.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/__init__.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/branch/BranchIndexUpdateDateTuple.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/branch/BranchIndexUpdateDateTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/branch/BranchKeyToIdMapTuple.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/branch/BranchKeyToIdMapTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/branch/BranchLiveEditTuple.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/branch/BranchLiveEditTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/branch/BranchLiveEditTupleAction.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/branch/BranchLiveEditTupleAction.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/branch/BranchTuple.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/branch/BranchTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/branch/BranchUpdateTupleAction.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/branch/BranchUpdateTupleAction.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/grid/EncodedGridTuple.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/grid/EncodedGridTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/grid/GridUpdateDateTuple.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/grid/GridUpdateDateTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/location_index/DispKeyLocationTuple.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/location_index/DispKeyLocationTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/location_index/EncodedLocationIndexTuple.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/location_index/EncodedLocationIndexTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/tuples/location_index/LocationIndexUpdateDateTuple.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/tuples/location_index/LocationIndexUpdateDateTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/WorkerEntryHook.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/WorkerEntryHook.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 import logging
 
-from peek_plugin_base.worker.PluginWorkerEntryHookABC import PluginWorkerEntryHookABC
+from peek_plugin_base.worker.PluginWorkerEntryHookABC import (
+    PluginWorkerEntryHookABC,
+)
 from peek_plugin_diagram._private.worker.tasks import (
     GridCompilerTask,
     ImportDispTask,
     DispCompilerTask,
     LocationIndexCompilerTask,
 )
 from peek_plugin_diagram._private.worker.tasks.branch import (
-    BranchIndexCompiler,
-    BranchIndexImporter,
-    BranchIndexUpdater,
+    BranchIndexCompilerTask,
+    BranchIndexImporterTask,
+    BranchIndexUpdaterTask,
 )
+from peek_plugin_diagram.tuples import loadPublicTuples
 
 logger = logging.getLogger(__name__)
 
 
 class WorkerEntryHook(PluginWorkerEntryHookABC):
     def load(self):
+        loadPublicTuples()
         logger.debug("loaded")
 
     def start(self):
         logger.debug("started")
 
     def stop(self):
         logger.debug("stopped")
 
     def unload(self):
         logger.debug("unloaded")
 
     @property
     def celeryAppIncludes(self):
         return [
-            BranchIndexUpdater.__name__,
-            BranchIndexCompiler.__name__,
-            BranchIndexImporter.__name__,
+            BranchIndexUpdaterTask.__name__,
+            BranchIndexCompilerTask.__name__,
+            BranchIndexImporterTask.__name__,
             DispCompilerTask.__name__,
             GridCompilerTask.__name__,
             ImportDispTask.__name__,
             LocationIndexCompilerTask.__name__,
         ]
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/api/WorkerApiImpl.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/api/WorkerApiImpl.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/DispCompilerTask.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/DispCompilerTask.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 from vortex.Payload import Payload
 
 from peek_plugin_base.worker import CeleryDbConn
 from peek_plugin_base.worker.CeleryApp import celeryApp
 from peek_plugin_diagram._private.storage.DispIndex import DispIndexerQueue
 from peek_plugin_diagram._private.storage.Display import (
     DispBase,
-    DispTextStyle,
     DispGroup,
     DispGroupPointer,
     DispEdgeTemplate,
 )
+from peek_plugin_diagram._private.storage.Lookups import DispTextStyle
 from peek_plugin_diagram._private.storage.GridKeyIndex import (
     GridKeyIndex,
     GridKeyCompilerQueue,
 )
 from peek_plugin_diagram._private.storage.LiveDbDispLink import LiveDbDispLink
 from peek_plugin_diagram._private.storage.LocationIndex import (
     LocationIndex,
@@ -50,15 +50,17 @@
     makeLocationJson,
     dispKeyHashBucket,
 )
 from peek_plugin_livedb.worker.WorkerApi import WorkerApi
 
 logger = logging.getLogger(__name__)
 
-CoordSetIdGridKeyData = namedtuple("CoordSetIdGridKeyTuple", ["coordSetId", "gridKey"])
+CoordSetIdGridKeyData = namedtuple(
+    "CoordSetIdGridKeyTuple", ["coordSetId", "gridKey"]
+)
 
 ModelSetIdIndexBucketData = namedtuple(
     "ModelSetIdIndexBucketTuple", ["modelSetId", "indexBucket"]
 )
 
 DispData = namedtuple("DispData", ["json", "levelOrder", "layerOrder"])
 
@@ -132,29 +134,30 @@
         )
 
         # Get Model Set Name Map
         coordSetById = {o.id: o for o in coordSets}
 
         # ---------------
         # Load Coord Sets
-        textStyleById = {ts.id: ts for ts in ormSession.query(DispTextStyle).all()}
+        textStyleById = {
+            ts.id: ts for ts in ormSession.query(DispTextStyle).all()
+        }
 
         ormSession.expunge_all()
 
     except Exception as e:
         logger.exception(e)
         raise self.retry(exc=e, countdown=2)
 
     finally:
         ormSession.close()
 
     # ==========================
     # This method will create new disps that will be compiled later.
     try:
-
         # ---------------
         # 1) Clone the disps for the group instances
         dispIdsIncludingClones = _cloneDispsForDispGroupPointer(dispIds)
 
     except Exception as e:
         logger.exception(e)
         raise self.retry(exc=e, countdown=2)
@@ -214,15 +217,14 @@
 
     finally:
         ormSession.close()
 
     # ==========================
     # 9) Run the bulk DB delete/insert methods
     try:
-
         _insertToDb(
             dispIdsIncludingClones,
             gridCompiledQueueItems,
             gridKeyIndexesByDispId,
             locationCompiledQueueItems,
             locationIndexByDispId,
             queueItemIds,
@@ -261,34 +263,36 @@
 
 
     """
     startTime = datetime.now(pytz.utc)
 
     ormSession = CeleryDbConn.getDbSession()
     try:
-
         # -----
         # Load the disp group pointers
         qry = (
             ormSession.query(DispGroupPointer)
             .filter(DispGroupPointer.targetDispGroupId != None)
             .filter(DispGroupPointer.id.in_(dispIds))
         )
 
         dispGroupPointers: List[DispGroupPointer] = qry.all()
 
         # If there are no DispGroupPointers that need cloning, then return.
         if not dispGroupPointers:
             logger.debug(
-                "Cloning skipped," " there are no disp group ptrs with targets, in %s",
+                "Cloning skipped,"
+                " there are no disp group ptrs with targets, in %s",
                 (datetime.now(pytz.utc) - startTime),
             )
             return dispIds
 
-        dispGroupPointerTargetIds = [o.targetDispGroupId for o in dispGroupPointers]
+        dispGroupPointerTargetIds = [
+            o.targetDispGroupId for o in dispGroupPointers
+        ]
 
         del qry
 
         # -----
         # Delete any existing disps are in these pointers
         ormSession.query(DispBase).filter(
             DispBase.groupId.in_([o.id for o in dispGroupPointers])
@@ -336,19 +340,22 @@
         cloneLiveDbDispLinks = []
 
         for dispPtr in dispGroupPointers:
             if not dispPtr.targetDispGroupId:
                 logger.debug("Pointer has no targetGroupId id=%s", dispPtr.id)
                 continue
 
-            dispGroupChilds = dispGroupChildsByGroupId.get(dispPtr.targetDispGroupId)
+            dispGroupChilds = dispGroupChildsByGroupId.get(
+                dispPtr.targetDispGroupId
+            )
 
             if not dispGroupChilds:
                 logger.warning(
-                    "Pointer points to missing DispGroup," " id=%s, targetGroupId=%s",
+                    "Pointer points to missing DispGroup,"
+                    " id=%s, targetGroupId=%s",
                     dispPtr.id,
                     dispPtr.targetDispGroupId,
                 )
                 continue
 
             x, y = json.loads(dispPtr.geomJson)
             dispPtr.targetDispGroupName = dispGroupNameByGroupId[
@@ -376,15 +383,17 @@
 
                     cloneDispLink.id = None
                     cloneDispLink.disp = cloneDisp
                     cloneDispLink.coordSetId = dispPtr.coordSetId
 
         # -----
         # Preallocate the IDs for performance on PostGreSQL
-        dispIdGen = CeleryDbConn.prefetchDeclarativeIds(DispBase, len(cloneDisps))
+        dispIdGen = CeleryDbConn.prefetchDeclarativeIds(
+            DispBase, len(cloneDisps)
+        )
         for cloneDisp in cloneDisps:
             cloneDisp.id = next(dispIdGen)
 
         # Preallocate the IDs for performance on PostGreSQL
         dispLinkIdGen = CeleryDbConn.prefetchDeclarativeIds(
             LiveDbDispLink, len(cloneLiveDbDispLinks)
         )
@@ -395,15 +404,17 @@
 
         # -----
         # Create the new list of IDs to compile
         # Do this here, otherwise it will cause a DB refresh if it's after the commit.
         dispIdsIncludingClones = dispIds + [o.id for o in cloneDisps]
 
         ormSession.bulk_save_objects(cloneDisps, update_changed_only=False)
-        ormSession.bulk_save_objects(cloneLiveDbDispLinks, update_changed_only=False)
+        ormSession.bulk_save_objects(
+            cloneLiveDbDispLinks, update_changed_only=False
+        )
 
         ormSession.commit()
 
         logger.debug(
             "Cloned %s disp group objects in %s",
             len(cloneDisps),
             (datetime.now(pytz.utc) - startTime),
@@ -427,15 +438,17 @@
     """
     startTime = datetime.now(pytz.utc)
 
     # -----
     # Begin the DISP merge from live data
     qry = (
         ormSession.query(DispBase)
-        .options(subqueryload(DispBase.liveDbLinks), subqueryload(DispBase.level))
+        .options(
+            subqueryload(DispBase.liveDbLinks), subqueryload(DispBase.level)
+        )
         .filter(DispBase.id.in_(dispIdsIncludingClones))
     )
 
     allDisps = qry.all()
 
     logger.debug(
         "Loaded %s disp objects in %s",
@@ -505,50 +518,58 @@
 
         # Create the JSON Dict
         dispDict = disp.tupleToSmallJsonDict()
 
         # Get and Scale the Geometry
         geomArray = None
         # Disp Groups have no geometry
-        if not isinstance(disp, DispGroup) and not isinstance(disp, DispEdgeTemplate):
+        if not isinstance(disp, DispGroup) and not isinstance(
+            disp, DispEdgeTemplate
+        ):
             geomArray = json.loads(disp.geomJson)
             geomArray = _scaleDispGeomWithCoordSet(geomArray, coordSet)
             dispDict["g"] = geomArray
 
         preparedDisps.append(PreparedDisp(disp, geomArray, dispDict))
 
     logger.debug(
-        "Scaled %s disps in %s", len(disps), (datetime.now(pytz.utc) - startTime)
+        "Scaled %s disps in %s",
+        len(disps),
+        (datetime.now(pytz.utc) - startTime),
     )
 
     return preparedDisps
 
 
 def _compileDispGroups(ormSession, preparedDisps: List[PreparedDisp]):
     """Compile Disp Groups
 
     This method will pack the child disps into the disp groups dispJson field.
 
     """
 
     def packDisp(disp):
         """Pack Disp"""
-        dispDict = disp.tupleToSmallJsonDict(includeFalse=False, includeNones=False)
+        dispDict = disp.tupleToSmallJsonDict(
+            includeFalse=False, includeNones=False
+        )
         dispDict["g"] = json.loads(disp.geomJson)
         return dispDict
 
     startTime = datetime.now(pytz.utc)
 
     preparedDispGroupByIds: Dict[int, PreparedDisp] = {
         o.disp.id: o for o in preparedDisps if isinstance(o.disp, DispGroup)
     }
 
     # Query for the disp groups with loaded child disps we'll need
 
-    childDispsByGroupId = _queryDispsForGroup(ormSession, preparedDispGroupByIds)
+    childDispsByGroupId = _queryDispsForGroup(
+        ormSession, preparedDispGroupByIds
+    )
 
     childDispCount = 0
 
     for groupId in preparedDispGroupByIds:
         preparedDispGroup = preparedDispGroupByIds[groupId]
         childDisps = childDispsByGroupId[groupId]
 
@@ -609,21 +630,25 @@
         locationIndexByDispId[pdisp.disp.id] = dict(
             indexBucket=indexBucket,
             dispId=pdisp.disp.id,
             modelSetId=coordSet.modelSetId,
         )
 
     logger.debug(
-        "Indexed %s disp Locations in %s", count, (datetime.now(pytz.utc) - startTime)
+        "Indexed %s disp Locations in %s",
+        count,
+        (datetime.now(pytz.utc) - startTime),
     )
 
     return locationCompiledQueueItems, locationIndexByDispId
 
 
-def _calculateGridKeys(preparedDisps: List[PreparedDisp], coordSetById, textStyleById):
+def _calculateGridKeys(
+    preparedDisps: List[PreparedDisp], coordSetById, textStyleById
+):
     """Calculate Grid Keys
 
     This method Determines which grids this disp will live in,
     and creates GridKeyIndex entries for those grid keys for this disp.
 
     """
 
@@ -706,15 +731,17 @@
     :param disp: The disp to assign the data back to
     :param dispDict: The updated dispDict prepared elsewhere
         The only updated done outside of this method is for the DispGroup
     :return: The updated dispDict (This result is used by the BranchDispUpdater)
 
     """
     # Strip out the nulls and falses, to make it even more compact
-    stripped = {k: v for k, v in dispDict.items() if v is not None and v is not False}
+    stripped = {
+        k: v for k, v in dispDict.items() if v is not None and v is not False
+    }
 
     hashId = _createHashId(stripped)
 
     # Assign the value
     stripped["hid"] = hashId
 
     # Write the "compiled" disp JSON back to the disp.
@@ -769,15 +796,17 @@
 
             if dispId in locationIndexByDispId:
                 locationIndexes.append(locationIndexByDispId[dispId])
 
         # Delete existing items in the location and grid index
 
         # grid index
-        conn.execute(gridKeyIndexTable.delete(gridKeyIndexTable.c.dispId.in_(dispIds)))
+        conn.execute(
+            gridKeyIndexTable.delete(gridKeyIndexTable.c.dispId.in_(dispIds))
+        )
 
         # location index
         conn.execute(
             locationIndexTable.delete(locationIndexTable.c.dispId.in_(dispIds))
         )
 
         # ---------------
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/GridCompilerTask.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/GridCompilerTask.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,27 +6,31 @@
 from datetime import datetime
 from functools import cmp_to_key
 from typing import List
 
 import pytz
 from peek_plugin_base.worker import CeleryDbConn
 from peek_plugin_base.worker.CeleryApp import celeryApp
-from peek_plugin_diagram._private.storage.Display import DispLevel, DispBase, DispLayer
+from peek_plugin_diagram._private.storage.Display import DispBase
+from peek_plugin_diagram._private.storage.Lookups import DispLevel
+from peek_plugin_diagram._private.storage.Lookups import DispLayer
 from peek_plugin_diagram._private.storage.GridKeyIndex import (
     GridKeyIndexCompiled,
     GridKeyCompilerQueue,
     GridKeyIndex,
 )
 from peek_plugin_diagram._private.tuples.grid.GridTuple import GridTuple
 from txcelery.defer import DeferrableTask
 from vortex.Payload import Payload
 
 logger = logging.getLogger(__name__)
 
-DispData = namedtuple("DispData", ["json", "id", "zOrder", "levelOrder", "layerOrder"])
+DispData = namedtuple(
+    "DispData", ["json", "id", "zOrder", "levelOrder", "layerOrder"]
+)
 
 """ Grid Compiler
 
 Compile the disp items into the grid data
 
 1) Query for queue
 2) Process queue
@@ -36,39 +40,40 @@
 
 class NotAllDispsCompiledException(Exception):
     pass
 
 
 @DeferrableTask
 @celeryApp.task(bind=True)
-def compileGrids(self, payloadEncodedArgs: bytes) -> List[str]:
+def compileGrids(self, payloadEncodedArgs: bytes) -> dict[str, str]:
     """Compile Grids Task
 
     :param self: A celery reference to this task
     :param payloadEncodedArgs: An encoded payload containing the queue tuples.
     :returns: A list of grid keys that have been updated.
     """
     argData = Payload().fromEncodedPayload(payloadEncodedArgs).tuples
     queueItems = argData[0]
     queueItemIds: List[int] = argData[1]
 
     gridKeys = list(set([i.gridKey for i in queueItems]))
     coordSetIdByGridKey = {i.gridKey: i.coordSetId for i in queueItems}
 
+    lastUpdateByChunkKey = {}
+
     queueTable = GridKeyCompilerQueue.__table__
     gridTable = GridKeyIndexCompiled.__table__
 
     startTime = datetime.now(pytz.utc)
 
     session = CeleryDbConn.getDbSession()
     engine = CeleryDbConn.getDbEngine()
     conn = engine.connect()
     transaction = conn.begin()
     try:
-
         logger.debug(
             "Staring compile of %s queueItems in %s",
             len(queueItems),
             (datetime.now(pytz.utc) - startTime),
         )
 
         total = 0
@@ -82,34 +87,40 @@
         inserts = []
         for gridKey, dispJsonStr in dispData.items():
             m = hashlib.sha256()
             m.update(gridKey.encode())
             m.update(dispJsonStr.encode())
             gridTupleHash = b64encode(m.digest()).decode()
 
+            lastUpdateByChunkKey[str(gridKey)] = gridTupleHash
+
             gridTuple = GridTuple(
-                gridKey=gridKey, dispJsonStr=dispJsonStr, lastUpdate=gridTupleHash
+                gridKey=gridKey,
+                dispJsonStr=dispJsonStr,
+                lastUpdate=gridTupleHash,
             )
 
-            encodedGridTuple = Payload(tuples=[gridTuple]).toEncodedPayload()
+            encodedGridTuple = (
+                Payload(tuples=[gridTuple]).toEncodedPayload().encode()
+            )
 
             inserts.append(
                 dict(
                     coordSetId=coordSetIdByGridKey[gridKey],
                     gridKey=gridKey,
                     lastUpdate=gridTupleHash,
                     encodedGridTuple=encodedGridTuple,
                 )
             )
 
         if inserts:
             conn.execute(gridTable.insert(), inserts)
 
         logger.debug(
-            "Compiled %s gridKeys, %s missing, in %s",
+            "Compiled %s gridKeyTuples, %s missing, in %s",
             len(inserts),
             len(gridKeys) - len(inserts),
             (datetime.now(pytz.utc) - startTime),
         )
 
         total += len(inserts)
 
@@ -118,18 +129,20 @@
         transaction.commit()
         logger.info(
             "Compiled and Committed %s GridKeyIndexCompileds in %s",
             total,
             (datetime.now(pytz.utc) - startTime),
         )
 
-        return gridKeys
+        return lastUpdateByChunkKey
 
     except NotAllDispsCompiledException as e:
-        logger.warning("Retrying, Not all disps for gridKey %s are compiled", gridKeys)
+        logger.warning(
+            "Retrying, Not all disps for gridKey %s are compiled", gridKeys
+        )
         raise self.retry(exc=e, countdown=1)
 
     except Exception as e:
         transaction.rollback()
         logger.debug("Compile of grids failed, retrying : %s", gridKeys)
         raise self.retry(exc=e, countdown=2)
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/ImportDispLink.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/ImportDispLink.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/ImportDispTask.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/ImportDispTask.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/LiveDbDisplayValueConverter.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/LiveDbDisplayValueConverter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 from typing import Dict
 
 from sqlalchemy import select
 
-from peek_plugin_diagram._private.storage.Display import DispColor
-from peek_plugin_diagram._private.storage.Display import DispLayer
-from peek_plugin_diagram._private.storage.Display import DispLevel
-from peek_plugin_diagram._private.storage.Display import DispLineStyle
-from peek_plugin_diagram._private.storage.Display import DispTextStyle
+from peek_plugin_diagram._private.storage.Lookups import DispColor
+from peek_plugin_diagram._private.storage.Lookups import DispLayer
+from peek_plugin_diagram._private.storage.Lookups import DispLevel
+from peek_plugin_diagram._private.storage.Lookups import DispLineStyle
+from peek_plugin_diagram._private.storage.Lookups import DispTextStyle
 from peek_plugin_livedb.tuples.ImportLiveDbItemTuple import (
     ImportLiveDbItemTuple,
 )
 
 logger = logging.getLogger(__name__)
 
 textTable = DispTextStyle.__table__
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/LocationIndexCompilerTask.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/LocationIndexCompilerTask.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 2) Process queue
 3) Delete from queue
 """
 
 
 @DeferrableTask
 @celeryApp.task(bind=True)
-def compileLocationIndex(self, payloadEncodedArgs: bytes) -> List[str]:
+def compileLocationIndex(self, payloadEncodedArgs: bytes) -> dict[str, str]:
     """Compile Location Index Task
 
     :param self: A celery reference to this task
     :param payloadEncodedArgs: An encoded payload containing the queue tuples.
     :returns: A list of grid keys that have been updated.
     """
     argData = Payload().fromEncodedPayload(payloadEncodedArgs).tuples
@@ -56,14 +56,16 @@
     indexBuckets = list(set([i.indexBucket for i in queueItems]))
     modelSetIdByIndexBucket = {i.indexBucket: i.modelSetId for i in queueItems}
 
     queueTable = LocationIndexCompilerQueue.__table__
     compiledTable = LocationIndexCompiled.__table__
     lastUpdate = datetime.now(pytz.utc).isoformat()
 
+    lastUpdateByChunkKey = {}
+
     startTime = datetime.now(pytz.utc)
 
     session = CeleryDbConn.getDbSession()
     engine = CeleryDbConn.getDbEngine()
     conn = engine.connect()
     transaction = conn.begin()
     try:
@@ -102,22 +104,26 @@
             modelSetKey = modelSetKeyByModelSetId[modelSetId]
 
             m = hashlib.sha256()
             m.update(modelSetKey.encode())
             m.update(jsonStr.encode())
             dataHash = b64encode(m.digest()).decode()
 
+            lastUpdateByChunkKey[str(indexBucket)] = dataHash
+
             locationIndexTuple = LocationIndexTuple(
                 modelSetKey=modelSetKey,
                 indexBucket=indexBucket,
                 jsonStr=jsonStr,
                 lastUpdate=dataHash,
             )
 
-            blobData = Payload(tuples=[locationIndexTuple]).toEncodedPayload()
+            blobData = (
+                Payload(tuples=[locationIndexTuple]).toEncodedPayload().encode()
+            )
 
             inserts.append(
                 dict(
                     modelSetId=modelSetId,
                     indexBucket=indexBucket,
                     lastUpdate=dataHash,
                     blobData=blobData,
@@ -134,26 +140,28 @@
             (datetime.now(pytz.utc) - startTime),
         )
 
         total += len(inserts)
 
         conn.execute(
             queueTable.delete(
-                makeCoreValuesSubqueryCondition(engine, queueTable.c.id, queueItemIds)
+                makeCoreValuesSubqueryCondition(
+                    engine, queueTable.c.id, queueItemIds
+                )
             )
         )
 
         transaction.commit()
         logger.info(
             "Compiled and Comitted %s LocationIndexCompileds in %s",
             total,
             (datetime.now(pytz.utc) - startTime),
         )
 
-        return indexBuckets
+        return lastUpdateByChunkKey
 
     except Exception as e:
         transaction.rollback()
         # logger.warning(e)  # Just a warning, it will retry
         logger.exception(e)
         raise self.retry(exc=e, countdown=2)
 
@@ -161,15 +169,18 @@
         conn.close()
         session.close()
 
 
 def _buildIndex(session, indexBuckets) -> Dict[str, str]:
     indexQry = (
         session.query(
-            LocationIndex.indexBucket, DispBase.id, DispBase.key, DispBase.locationJson
+            LocationIndex.indexBucket,
+            DispBase.id,
+            DispBase.key,
+            DispBase.locationJson,
         )
         .join(DispBase, DispBase.id == LocationIndex.dispId)
         .filter(
             makeOrmValuesSubqueryCondition(
                 session, LocationIndex.indexBucket, indexBuckets
             )
         )
@@ -177,26 +188,32 @@
     )
 
     jsonByIndexBucket = {}
 
     # Create the IndexBucket -> Key -> [Locations] structure
     locationByKeyByBucket = defaultdict(lambda: defaultdict(list))
     for item in indexQry:
-        locationByKeyByBucket[item.indexBucket][item.key].append(item.locationJson)
+        locationByKeyByBucket[item.indexBucket][item.key].append(
+            item.locationJson
+        )
 
     # Sort each bucket by the key
     for indexBucket, locationByKey in locationByKeyByBucket.items():
 
         # Create a list of of key, [locationJson, locationJson, locationJson]
-        sortedKeyLocations = list(sorted(locationByKey.items(), key=lambda i: i[0]))
+        sortedKeyLocations = list(
+            sorted(locationByKey.items(), key=lambda i: i[0])
+        )
 
         # [even] is a key, [odd] is the locations json string
         indexStructure = []
         for key, locationsJson in sortedKeyLocations:
             # Combine the key and locations into one json array
-            indexStructure.append('["%s",' % key + ",".join(locationsJson) + "]")
+            indexStructure.append(
+                '["%s",' % key + ",".join(locationsJson) + "]"
+            )
 
         # Create the blob data for this index.
         # It will be searched by a binary sort
         jsonByIndexBucket[indexBucket] = "[" + ",".join(indexStructure) + "]"
 
     return jsonByIndexBucket
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/LookupHashConverter.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/LookupHashConverter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 from typing import Dict
 
 from sqlalchemy import select
 
-from peek_plugin_diagram._private.storage.Display import DispColor
-from peek_plugin_diagram._private.storage.Display import DispLayer
-from peek_plugin_diagram._private.storage.Display import DispLevel
-from peek_plugin_diagram._private.storage.Display import DispLineStyle
-from peek_plugin_diagram._private.storage.Display import DispTextStyle
+from peek_plugin_diagram._private.storage.Lookups import DispColor
+from peek_plugin_diagram._private.storage.Lookups import DispLayer
+from peek_plugin_diagram._private.storage.Lookups import DispLevel
+from peek_plugin_diagram._private.storage.Lookups import DispLineStyle
+from peek_plugin_diagram._private.storage.Lookups import DispTextStyle
 from peek_plugin_diagram.tuples.model.ImportLiveDbDispLinkTuple import (
     ImportLiveDbDispLinkTuple,
 )
 
 # NO_SYMBOL = "NO_SYMBOL"
 #
 # DRESSING_GRID_KEY = "dressings"
@@ -38,35 +38,32 @@
         self._textStyleIdByImportHash = self._loadLookupByModelSet(textTable)
         self._lineStyleIdByImportHash = self._loadLookupByModelSet(lineTable)
         self._colorIdByImportHash = self._loadLookupByModelSet(colorTable)
         self._levelByImportHash = self._loadLookupByCoordSet(levelTable)
         self._layerByImportHash = self._loadLookupByModelSet(layerTable)
 
     def _loadLookupByModelSet(self, table) -> Dict[str, int]:
-
         resultSet = self._ormSession.execute(
             select([table.c.importHash, table.c.id]).where(
                 table.c.modelSetId == self._modelSetId
             )
         )
 
         return dict(resultSet.fetchall())
 
     def _loadLookupByCoordSet(self, table) -> Dict[str, int]:
-
         resultSet = self._ormSession.execute(
             select([table.c.importHash, table.c.id]).where(
                 table.c.coordSetId == self._coordSetId
             )
         )
 
         return dict(resultSet.fetchall())
 
     def convertLookups(self, disp):
-
         T = ImportLiveDbDispLinkTuple
 
         colourFields = {
             T.DISP_ATTR_FILL_COLOR,
             T.DISP_ATTR_COLOR,
             T.DISP_ATTR_LINE_COLOR,
             T.DISP_ATTR_EDGE_COLOR,
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/_CalcDisp.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/_CalcDisp.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/_CalcDispFromLiveDb.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/_CalcDispFromLiveDb.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/_CalcGridForDisp.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/_CalcGridForDisp.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,32 @@
 import math
 
 import logging
 from typing import Dict, List
 
 from peek_plugin_diagram._private.storage.Display import (
     DispText,
-    DispTextStyle,
     DispEllipse,
     DispGroup,
     DispGroupPointer,
 )
+from peek_plugin_diagram._private.storage.Lookups import DispTextStyle
 from peek_plugin_diagram._private.storage.ModelSet import (
     ModelCoordSet,
     ModelCoordSetGridSize,
 )
 
 logger = logging.getLogger(__name__)
 
 
 def makeGridKeysForDisp(
-    coordSet: ModelCoordSet, disp, geomJson, textStyleById: Dict[int, DispTextStyle]
+    coordSet: ModelCoordSet,
+    disp,
+    geomJson,
+    textStyleById: Dict[int, DispTextStyle],
 ) -> List[str]:
     points = geomJson
 
     if geomJson is None:
         logger.critical("geomJson is None : %s ", disp)
         return []
 
@@ -48,31 +51,35 @@
         if isinstance(disp, DispText) and _isTextTooSmall(
             disp, gridSize, textStyleById
         ):
             continue
 
         # If this is just a point shape/geom, then add it and continue
         if isinstance(disp, DispEllipse):
-            minx, miny, maxx, maxy = _calcEllipseBounds(disp, points[0], points[1])
+            minx, miny, maxx, maxy = _calcEllipseBounds(
+                disp, points[0], points[1]
+            )
 
         elif len(points) == 2:  # 2 = [x, y]
-
             # This should be a text
             if (
                 not isinstance(disp, DispText)
                 and not isinstance(disp, DispGroup)
                 and not isinstance(disp, DispGroupPointer)
             ):
-                logger.debug("TODO Determine size for disp type %s", disp.tupleType())
+                logger.debug(
+                    "TODO Determine size for disp type %s", disp.tupleType()
+                )
 
             # Texts on the boundaries of grids could be a problem
             # They will seem them if the pan over just a little.
             gridKeys.append(
                 gridSize.makeGridKey(
-                    int(points[0] / gridSize.xGrid), int(points[1] / gridSize.yGrid)
+                    int(points[0] / gridSize.xGrid),
+                    int(points[1] / gridSize.yGrid),
                 )
             )
             continue
 
         else:
             # Else, All other shapes
             # Get the bounding box
@@ -125,15 +132,17 @@
 
 
 def _pointToPixel(point: float) -> float:
     return point * 96 / 72
 
 
 def _isTextTooSmall(
-    disp, gridSize: ModelCoordSetGridSize, textStyleById: Dict[int, DispTextStyle]
+    disp,
+    gridSize: ModelCoordSetGridSize,
+    textStyleById: Dict[int, DispTextStyle],
 ) -> bool:
     """Is Text Too Small
 
     This method calculates the size that the text will appear on the diagram at max zoom
     for the provided gird.
 
     We'll only work this out based on the height
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/_CalcLocation.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/_CalcLocation.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/_ModelSetUtil.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/_ModelSetUtil.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/branch/BranchDispUpdater.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/branch/BranchDispUpdater.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/branch/BranchIndexCompiler.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/branch/BranchIndexCompilerTask.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 2) Process queue
 3) Delete from queue
 """
 
 
 @DeferrableTask
 @celeryApp.task(bind=True)
-def compileBranchIndexChunk(self, payloadEncodedArgs: bytes) -> List[int]:
+def compileBranchIndexChunk(self, payloadEncodedArgs: bytes) -> dict[str, str]:
     """Compile BranchIndex Index Task
 
     :param self: A bound parameter from celery
     :param payloadEncodedArgs: An encoded payload containing the queue tuples.
     :returns: A list of grid keys that have been updated.
     """
     argData = Payload().fromEncodedPayload(payloadEncodedArgs).tuples
@@ -51,16 +51,21 @@
     transaction = conn.begin()
     try:
         queueItemsByModelSetId = defaultdict(list)
 
         for queueItem in queueItems:
             queueItemsByModelSetId[queueItem.modelSetId].append(queueItem)
 
+        lastUpdateByChunkKey = {}
         for modelSetId, modelSetQueueItems in queueItemsByModelSetId.items():
-            _compileBranchIndexChunk(conn, transaction, modelSetId, modelSetQueueItems)
+            lastUpdateByChunkKey.update(
+                _compileBranchIndexChunk(
+                    conn, transaction, modelSetId, modelSetQueueItems
+                )
+            )
 
         queueTable = BranchIndexCompilerQueue.__table__
 
         transaction = conn.begin()
         conn.execute(queueTable.delete(queueTable.c.id.in_(queueItemIds)))
         transaction.commit()
 
@@ -68,20 +73,23 @@
         transaction.rollback()
         logger.debug("RETRYING task - %s", e)
         raise self.retry(exc=e, countdown=10)
 
     finally:
         conn.close()
 
-    return list(set([i.chunkKey for i in queueItems]))
+    return lastUpdateByChunkKey
 
 
 def _compileBranchIndexChunk(
-    conn, transaction, modelSetId: int, queueItems: List[BranchIndexCompilerQueue]
-) -> None:
+    conn,
+    transaction,
+    modelSetId: int,
+    queueItems: List[BranchIndexCompilerQueue],
+) -> dict[str, str]:
     chunkKeys = list(set([i.chunkKey for i in queueItems]))
 
     compiledTable = BranchIndexEncodedChunk.__table__
     lastUpdate = datetime.now(pytz.utc).isoformat()
 
     startTime = datetime.now(pytz.utc)
 
@@ -94,47 +102,58 @@
     # Get Model Sets
 
     total = 0
     existingHashes = _loadExistingHashes(conn, chunkKeys)
     encKwPayloadByChunkKey = _buildIndex(chunkKeys)
     chunksToDelete = []
 
+    lastUpdateByChunkKey = {}
+
     inserts = []
-    for chunkKey, diagramIndexChunkEncodedPayload in encKwPayloadByChunkKey.items():
+    for (
+        chunkKey,
+        diagramIndexChunkEncodedPayload,
+    ) in encKwPayloadByChunkKey.items():
         m = hashlib.sha256()
-        m.update(diagramIndexChunkEncodedPayload)
+        m.update(diagramIndexChunkEncodedPayload.encode())
         encodedHash = b64encode(m.digest()).decode()
 
         # Compare the hash, AND delete the chunk key
         if chunkKey in existingHashes:
             # At this point we could decide to do an update instead,
             # but inserts are quicker
             if encodedHash == existingHashes.pop(chunkKey):
                 continue
 
+        lastUpdateByChunkKey[chunkKey] = lastUpdate
+
         chunksToDelete.append(chunkKey)
         inserts.append(
             dict(
                 modelSetId=modelSetId,
                 chunkKey=chunkKey,
-                encodedData=diagramIndexChunkEncodedPayload,
+                encodedData=diagramIndexChunkEncodedPayload.encode(),
                 encodedHash=encodedHash,
                 lastUpdate=lastUpdate,
             )
         )
 
     # Add any chnuks that we need to delete that we don't have new data for, here
     chunksToDelete.extend(list(existingHashes))
 
     if chunksToDelete:
         # Delete the old chunks
-        conn.execute(compiledTable.delete(compiledTable.c.chunkKey.in_(chunksToDelete)))
+        conn.execute(
+            compiledTable.delete(compiledTable.c.chunkKey.in_(chunksToDelete))
+        )
 
     if inserts:
-        newIdGen = CeleryDbConn.prefetchDeclarativeIds(BranchIndex, len(inserts))
+        newIdGen = CeleryDbConn.prefetchDeclarativeIds(
+            BranchIndex, len(inserts)
+        )
         for insert in inserts:
             insert["id"] = next(newIdGen)
 
     transaction.commit()
     transaction = conn.begin()
 
     if inserts:
@@ -152,14 +171,16 @@
     transaction.commit()
     logger.debug(
         "Compiled and Committed %s EncodedBranchIndexChunks in %s",
         total,
         (datetime.now(pytz.utc) - startTime),
     )
 
+    return lastUpdateByChunkKey
+
 
 def _loadExistingHashes(conn, chunkKeys: List[str]) -> Dict[str, str]:
     compiledTable = BranchIndexEncodedChunk.__table__
 
     results = conn.execute(
         select(
             columns=[compiledTable.c.chunkKey, compiledTable.c.encodedHash],
@@ -171,15 +192,17 @@
 
 
 def _buildIndex(chunkKeys) -> Dict[str, bytes]:
     session = CeleryDbConn.getDbSession()
 
     try:
         indexQry = (
-            session.query(BranchIndex.chunkKey, BranchIndex.key, BranchIndex.packedJson)
+            session.query(
+                BranchIndex.chunkKey, BranchIndex.key, BranchIndex.packedJson
+            )
             .filter(BranchIndex.chunkKey.in_(chunkKeys))
             .order_by(BranchIndex.key)
             .yield_per(1000)
             .all()
         )
 
         # Create the ChunkKey -> {key -> packedJson, key -> packedJson, ....]
@@ -189,18 +212,23 @@
             packagedJsonsByObjKeyByChunkKey[item.chunkKey][item.key].append(
                 item.packedJson
             )
 
         encPayloadByChunkKey = {}
 
         # Sort each bucket by the key
-        for chunkKey, packedJsonsByKey in packagedJsonsByObjKeyByChunkKey.items():
+        for (
+            chunkKey,
+            packedJsonsByKey,
+        ) in packagedJsonsByObjKeyByChunkKey.items():
             tuples = json.dumps(packedJsonsByKey, sort_keys=True)
 
             # Create the blob data for this index.
             # It will be index-blueprint by a binary sort
-            encPayloadByChunkKey[chunkKey] = Payload(tuples=tuples).toEncodedPayload()
+            encPayloadByChunkKey[chunkKey] = Payload(
+                tuples=tuples
+            ).toEncodedPayload()
 
         return encPayloadByChunkKey
 
     finally:
         session.close()
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/branch/BranchIndexImporter.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/branch/BranchIndexImporterTask.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,28 +7,32 @@
 import pytz
 from peek_plugin_base.worker import CeleryDbConn
 from peek_plugin_diagram._private.server.controller.DispCompilerQueueController import (
     DispCompilerQueueController,
 )
 from peek_plugin_diagram._private.tuples.branch.BranchTuple import BranchTuple
 from peek_plugin_base.worker.CeleryApp import celeryApp
-from peek_plugin_diagram._private.worker.tasks.ImportDispTask import _bulkInsertDisps
+from peek_plugin_diagram._private.worker.tasks.ImportDispTask import (
+    _bulkInsertDisps,
+)
 from peek_plugin_diagram._private.worker.tasks.LookupHashConverter import (
     LookupHashConverter,
 )
 from peek_plugin_diagram._private.worker.tasks._ModelSetUtil import (
     getModelSetIdCoordSetId,
 )
 from peek_plugin_diagram._private.worker.tasks.branch.BranchDispUpdater import (
     _convertBranchDisps,
 )
-from peek_plugin_diagram._private.worker.tasks.branch.BranchIndexUpdater import (
+from peek_plugin_diagram._private.worker.tasks.branch.BranchIndexUpdaterTask import (
     _insertOrUpdateBranches,
 )
-from peek_plugin_diagram.tuples.branches.ImportBranchTuple import ImportBranchTuple
+from peek_plugin_diagram.tuples.branches.ImportBranchTuple import (
+    ImportBranchTuple,
+)
 from txcelery.defer import DeferrableTask
 from vortex.Payload import Payload
 
 logger = logging.getLogger(__name__)
 
 
 @DeferrableTask
@@ -58,15 +62,19 @@
     dbSession = CeleryDbConn.getDbSession()
 
     engine = CeleryDbConn.getDbEngine()
     conn = engine.connect()
     transaction = conn.begin()
 
     try:
-        for (modelSetKey, modelSetId, coordSetId), branches in groupedBranches.items():
+        for (
+            modelSetKey,
+            modelSetId,
+            coordSetId,
+        ), branches in groupedBranches.items():
             _insertOrUpdateBranches(conn, modelSetKey, modelSetId, branches)
 
             newDisps, dispIdsToCompile = _convertBranchDisps(branches)
 
             # NO TRANSACTION
             # Bulk load the Disps
             _bulkInsertDisps(engine, newDisps)
@@ -107,17 +115,21 @@
     branch format used throughout the diagram plugin.
 
     (Thats the packed JSON wrapped by an accessor class)
 
     """
 
     # Get a map for the coordSetIds
-    modelKeyCoordKeyTuples = [(b.modelSetKey, b.coordSetKey) for b in importBranches]
+    modelKeyCoordKeyTuples = [
+        (b.modelSetKey, b.coordSetKey) for b in importBranches
+    ]
 
-    coordSetIdByModelKeyCoordKeyTuple = getModelSetIdCoordSetId(modelKeyCoordKeyTuples)
+    coordSetIdByModelKeyCoordKeyTuple = getModelSetIdCoordSetId(
+        modelKeyCoordKeyTuples
+    )
 
     # Sort out the importBranches by coordSetKey
     branchByModelKeyByCoordKey = defaultdict(lambda: defaultdict(list))
     for importBranch in importBranches:
         branchByModelKeyByCoordKey[importBranch.modelSetKey][
             importBranch.coordSetKey
         ].append(importBranch)
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/branch/BranchIndexUpdater.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/branch/BranchIndexUpdaterTask.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/_private/worker/tasks/branch/_BranchIndexCalcChunkKey.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/_private/worker/tasks/branch/_BranchIndexCalcChunkKey.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/admin_tasks.rst` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/admin_tasks.rst`

 * *Files 6% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 ```````````````````````
 
 The coordinate sets can be edited in the database, they are located in the table
  :code:`pl_diagram."ModelCoordSet"`
 
 The fields most often customised are as follows :
 
-:name:  The name of the coordinaate set, this is displayed to the user.
+:name:  The name of the coordinate set, this is displayed to the user.
 
 :enabled: Is the coordinate set enabled, It's best to delete it if it's not.
 
-:initialPanX: The initial canvas X position when the coorinate set is loaded.
+:initialPanX: The initial canvas X position when the coordinate set is loaded.
 
-:initialPanY: The initial canvas Y position when the coorinate set is loaded.
+:initialPanY: The initial canvas Y position when the coordinate set is loaded.
 
-:initialZoom: The initial canvas zoom level when the coorinate set is loaded.
+:initialZoom: The initial canvas zoom level when the coordinate set is loaded.
 
 Update the values in the table accordingly, then restart the Peek Client service.
 
 .. _diagram_delete_coord_sets:
 
 Deleting Coord Sets
 ```````````````````
@@ -57,15 +57,15 @@
 To optimise the display of the diagram it's important to optimise the
 :code:`pl_diagram."ModelCoordSetGridSize"` table for each coordinate set.
 
 This represents the rules used by the Diagram compiler to compile the grids.
 
 Zoom ranges should not overlap.
 
-:min: The minumum zoom level that this Z Grid will be shown at.
+:min: The minimum zoom level that this Z Grid will be shown at.
 
 :max: The maximum zoom level that this Z Grid will be shown at.
 
 :xGrid: The horizontal size of each grid.
 
 :yGrid: The vertical size of each grid.
 
@@ -79,35 +79,35 @@
 
 Setting the Zoom Limits
 ```````````````````````
 
 This admin task will set the maximum and minimum zoom levels for a world view
 in the DMS diagram.
 
-Stop the Peek Services :code:`stop_peek.sh`
+Stop the Peek Services :code:`p_stop.sh`
 
 ----
 
 #. Navigate to the :code:`pl.diagram."ModelCoordSet"` table.
 #. Update the :code:`minZoom` value for the required world view.
 #. update the :code:`maxZoom` value for the required world view.
 #. Save the changes.
 
 .. image:: edit_zoom_limit.png
 
 ----
 
-Restart the Peek services. :code:`restart_peek.sh`
+Restart the Peek services. :code:`p_restart.sh`
 
 Enabling Markup Support
 ```````````````````````
 
 This admin task will enable Markup support for a world view.
 
-Stop the Peek Services :code:`stop_peek.sh`
+Stop the Peek Services :code:`p_stop.sh`
 
 ----
 
 #. Navigate to :code:`pl_diagram."ModelCoordSet"`
 #. Update :code:`editEnabled` to :code:`True`
 #. Update :code:`editDefaultColorId` to the default Fault Colour.
 #. Update :code:`editDefaultLayerId` to the Default Layer Id.
@@ -115,24 +115,24 @@
 #. Update :code:`editDefaultLineStyleId` to the default Line Style.
 #. Update :code:`editDefaultTextStyleId` to the default Text Style.
 
 .. image:: enable_markup.png
 
 ----
 
-Restart the Peek Services :code:`restart_peek.sh`
+Restart the Peek Services :code:`p_restart.sh`
 
 Recompiling Coord Sets
 ``````````````````````
 
 This admin task will recompile all grids for a given coordinate set.
 
 ----
 
-#.  Find the :code:`coordSetId` of the coorinate set to be recompiled.
+#.  Find the :code:`coordSetId` of the coordinate set to be recompiled.
 
 #.  Stop all peek services
 
 #.  Execute the following SQL replacing :code:`<ID>` with the :code:`coordSetId` ::
 
 
         -- Delete the existing grids for this coord set.
@@ -206,8 +206,29 @@
 .. image:: plugin_diagram_edit_settings.png
 
 To Discard your Changes
 ```````````````````````
 
 Click **Reset** at any time to discard your changed and return the value to the previous saved settings.
 
-.. image:: plugin_diagram_edit_settings_reset.png
+.. image:: plugin_diagram_edit_settings_reset.png
+
+Edit Light Mode Colours
+------------------------
+
+.. note:: The colour fields only accept hexadecimal colour codes in the form
+    #000000
+
+#. Using PSQL, update the blockApiUpdate value and new light colour::
+
+        UPDATE pl_diagram."DispColor"
+        SET
+        "blockApiUpdate" = TRUE,
+        "lightColor" = [New Color]
+        WHERE "lightColor" = [Old Color]
+
+
+#. Restart the Office and Field services.::
+
+        sudo systemctl restart peek_office
+        sudo systemctl restart peek_field
+
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/dev/dev.rst` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/dev/dev.rst`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/dev/dev_with_diagram_data_backend.png` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/dev/dev_with_diagram_data_backend.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/dev/ns_integration.png` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/dev/ns_integration.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/dev/other_diagram_integration.png` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/dev/other_diagram_integration.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/dev/structure_Initial_load.png` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/dev/structure_Initial_load.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/dev/web_integration.png` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/dev/web_integration.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/diagram_layers.jpg` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/diagram_layers.jpg`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/edit_zoom_limit.png` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/edit_zoom_limit.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/enable_markup.png` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/enable_markup.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/example_diagram.png` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/example_diagram.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/overview.rst` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/overview.rst`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/plugin_diagram_edit_settings.png` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/plugin_diagram_edit_settings.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/plugin_diagram_edit_settings_reset.png` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/plugin_diagram_edit_settings_reset.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/setup/setup_coord_set.rst` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/setup/setup_coord_set.rst`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/status/status.png` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/status/status.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/admin-doc/status/status.rst` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/admin-doc/status/status.rst`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/DiagramBranchService.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/DiagramBranchService.ts`

 * *Files 18% similar despite different names*

```diff
@@ -17,14 +17,16 @@
  *
  */
 export abstract class DiagramBranchService {
     constructor() {}
 
     abstract setVisibleBranches(commonBranches: BranchDetailTuple[]): void;
 
+    abstract getVisibleBranches(): BranchDetailTuple[];
+
     abstract getActiveBranchDetails(): Promise<DiagramBranchDetailsI | null>;
 
     abstract startEditing(
         modelSetKey: string,
         coordSetKey: string,
         branchKey: string
     ): Promise<void>;
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/DiagramConfigService.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/DiagramConfigService.ts`

 * *Files 11% similar despite different names*

```diff
@@ -8,13 +8,15 @@
 export abstract class DiagramConfigService {
     abstract setLayerVisible(
         modelSetKey: string,
         layerName: string,
         visible: boolean
     ): void;
 
+    abstract usePolylineEdgeColors(): boolean;
+
     abstract setUsePolylineEdgeColors(enabled: boolean): void;
 
     abstract setToolbarButtons(
         buttonBitmask: DiagramToolbarBuiltinButtonEnum
     ): void;
 }
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/DiagramItemSelectService.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/DiagramItemSelectService.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/DiagramOverrideService.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/DiagramOverrideService.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/DiagramPositionService.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/DiagramPositionService.ts`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,23 @@
 import { Observable } from "rxjs";
 
+export interface CoordSetViewWindowI {
+    modelSetKey: string;
+    coordSetKey: string;
+
+    // Left most X
+    x: number;
+
+    // Lowest Y
+    y: number;
+
+    width: number;
+    height: number;
+}
+
 export interface PositionUpdatedI {
     coordSetKey: string;
     x: number;
     y: number;
     zoom: number;
     editingBranch: string | null;
 }
@@ -114,14 +128,27 @@
 
     /** Position Updated Observable
      *
      * @return An observerable that fires when the canvas position is updated.
      */
     abstract positionUpdatedObservable(): Observable<PositionUpdatedI>;
 
+    /** Coordinate Set View Updated
+     *
+     * @returns an observable that is fired when the diagrams coordinate set
+     * or canvas window changes. For example, from zooming out.
+     */
+    abstract coordSetViewUpdatedObservable(): Observable<CoordSetViewWindowI | null>;
+
+    /** Last Coord Set View
+     *
+     * @returns the current coordinate set view window
+     */
+    abstract coordSetView(): CoordSetViewWindowI | null;
+
     /** isReady
      *
      * @returns an observable that is fired when the diagram loads a coordset
      * or the coord set changes
      */
     abstract isReadyObservable(): Observable<boolean>;
 }
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/DiagramToolbarService.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/DiagramToolbarService.ts`

 * *Files 2% similar despite different names*

```diff
@@ -86,8 +86,9 @@
 export enum DiagramToolbarBuiltinButtonEnum {
     BUTTON_NULL = 0,
     BUTTON_CHANGE_COORDSET_MENU = 1 << 0,
     BUTTOON_PRINT_DIAGRAM = 1 << 1,
     BUTTON_EDIT_DIAGRAM = 1 << 2,
     BUTTON_SELECT_BRANCHES = 1 << 3,
     BUTTON_SELECT_LAYERS = 1 << 4,
+    BUTTON_COLOR_MODES = 1 << 5,
 }
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/PeekCanvasBounds.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/PeekCanvasBounds.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/PluginNames.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/PluginNames.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/admin/SettingPropertyTuple.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/admin/SettingPropertyTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/branch/BranchKeyToIdMapTuple.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/branch/BranchKeyToIdMapTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/branch/BranchLiveEditTuple.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/branch/BranchLiveEditTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/branch/BranchLiveEditTupleAction.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/branch/BranchLiveEditTupleAction.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/branch/BranchTuple.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/branch/BranchTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/branch/BranchUpdateTupleAction.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/branch/BranchUpdateTupleAction.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/branch/PrivateDiagramBranchContext.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/branch/PrivateDiagramBranchContext.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/branch/PrivateDiagramBranchService.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/branch/PrivateDiagramBranchService.ts`

 * *Files 1% similar despite different names*

```diff
@@ -192,14 +192,18 @@
         return this._stopEditingObservable;
     }
 
     setVisibleBranches(commonBranches: BranchDetailTuple[]): void {
         this.enabledBranches = commonBranches;
     }
 
+    getVisibleBranches(): BranchDetailTuple[] {
+        return this.enabledBranches.slice();
+    }
+
     getActiveBranchDetails(): Promise<DiagramBranchDetailsI | null> {
         if (this.activeBranchContext == null) return Promise.resolve(null);
 
         return Promise.resolve({
             modelSetKey: this.activeBranchContext.modelSetKey,
             coordSetKey: this.activeBranchContext.coordSetKey,
             branchKey: this.activeBranchContext.branchTuple.key,
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/branch-loader/BranchIndexLoaderService.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/branch-loader/BranchIndexLoaderService.ts`

 * *Files 4% similar despite different names*

```diff
@@ -20,23 +20,20 @@
     diagramFilt,
     diagramTuplePrefix,
 } from "../PluginNames";
 import { BranchIndexEncodedChunkTuple } from "./BranchIndexEncodedChunkTuple";
 import { BranchIndexUpdateDateTuple } from "./BranchIndexUpdateDateTuple";
 import { BranchTuple } from "../branch/BranchTuple";
 import { PrivateDiagramTupleService } from "../services/PrivateDiagramTupleService";
-import { BranchIndexLoaderStatusTuple } from "./BranchIndexLoaderStatusTuple";
 import { ModelSet } from "../tuples/ModelSet";
 import { BranchIndexLoaderServiceA } from "./BranchIndexLoaderServiceA";
 import {
     DeviceOfflineCacheService,
-    OfflineCacheStatusTuple,
+    OfflineCacheLoaderStatusTuple,
 } from "@peek/peek_core_device";
-import { EncodedGridTuple } from "@peek/peek_plugin_diagram/_private/grid-loader/EncodedGridTuple";
-import { EncodedLocationIndexTuple } from "@peek/peek_plugin_diagram/_private/location-loader/EncodedLocationIndexTuple";
 
 // ----------------------------------------------------------------------------
 
 export interface BranchIndexResultI {
     [key: string]: BranchTuple[];
 }
 
@@ -126,37 +123,40 @@
 
     // Every 100 chunks from the server
     private SAVE_POINT_ITERATIONS = 100;
 
     // Saving the cache after each chunk is so expensive, we only do it every 20 or so
     private chunksSavedSinceLastIndexSave = 0;
 
-    private index = new BranchIndexUpdateDateTuple();
+    private index: BranchIndexUpdateDateTuple | null = null;
     private askServerChunks: BranchIndexUpdateDateTuple[] = [];
 
     private _hasLoaded = false;
 
     private _hasLoadedSubject: Subject<boolean> = new Subject<boolean>();
     private storage: TupleOfflineStorageService;
 
-    private _statusSubject = new Subject<BranchIndexLoaderStatusTuple>();
-    private _status = new BranchIndexLoaderStatusTuple();
+    private _statusSubject = new Subject<OfflineCacheLoaderStatusTuple>();
+    private _status = new OfflineCacheLoaderStatusTuple();
 
     private modelSetByIds: { [id: number]: ModelSet } = {};
     private _hasModelSetLoaded = false;
 
     constructor(
         private vortexService: VortexService,
         private vortexStatusService: VortexStatusService,
         storageFactory: TupleStorageFactoryService,
         private tupleService: PrivateDiagramTupleService,
         private deviceCacheControllerService: DeviceOfflineCacheService
     ) {
         super();
 
+        this._status.pluginName = "peek_plugin_diagram";
+        this._status.indexName = "Branch Index";
+
         let modelSetTs = new TupleSelector(ModelSet.tupleName, {});
         this.tupleService.offlineObserver
             .subscribeToTupleSelector(modelSetTs)
             .pipe(takeUntil(this.onDestroyEvent))
             .subscribe((tuples: ModelSet[]) => {
                 this.modelSetByIds = {};
                 for (let item of tuples) {
@@ -168,38 +168,53 @@
 
         this.storage = new TupleOfflineStorageService(
             storageFactory,
             new TupleOfflineStorageNameService(branchIndexStorageName)
         );
 
         this.setupVortexSubscriptions();
-        this._notifyStatus();
 
-        this.deviceCacheControllerService.triggerCachingObservable
+        this.deviceCacheControllerService.offlineModeEnabled$
             .pipe(takeUntil(this.onDestroyEvent))
             .pipe(filter((v) => v))
+            .pipe(first())
             .subscribe(() => {
                 this.initialLoad();
+            });
+
+        this.deviceCacheControllerService.triggerCachingStartObservable
+            .pipe(takeUntil(this.onDestroyEvent))
+            .pipe(filter((v) => v))
+            .subscribe(() => {
+                this.askServerForUpdates();
+                this._notifyStatus();
+            });
+
+        this.deviceCacheControllerService.triggerCachingResumeObservable
+            .pipe(takeUntil(this.onDestroyEvent))
+
+            .subscribe(() => {
                 this._notifyStatus();
+                this.askServerForNextUpdateChunk();
             });
     }
 
     isReady(): boolean {
         return this._hasLoaded;
     }
 
     isReadyObservable(): Observable<boolean> {
         return this._hasLoadedSubject;
     }
 
-    statusObservable(): Observable<BranchIndexLoaderStatusTuple> {
+    statusObservable(): Observable<OfflineCacheLoaderStatusTuple> {
         return this._statusSubject;
     }
 
-    status(): BranchIndexLoaderStatusTuple {
+    status(): OfflineCacheLoaderStatusTuple {
         return this._status;
     }
 
     /** Get BranchIndexs
      *
      * Get the objects with matching keywords from the index..
      *
@@ -264,81 +279,67 @@
     }
 
     private _notifyReady(): void {
         if (this._hasModelSetLoaded && this._hasLoaded)
             this._hasLoadedSubject.next();
     }
 
-    private _notifyStatus(): void {
-        this._status.cacheForOfflineEnabled =
-            this.deviceCacheControllerService.cachingEnabled;
-        this._status.initialLoadComplete = this.index.initialLoadComplete;
-
-        this._status.loadProgress = Object.keys(
-            this.index.updateDateByChunkKey
-        ).length;
-        for (let chunk of this.askServerChunks)
-            this._status.loadProgress -= Object.keys(
+    private _notifyStatus(paused: boolean = false): void {
+        this._status.lastCheckDate = new Date();
+        this._status.paused = paused;
+        this._status.initialFullLoadComplete = this.index.initialLoadComplete;
+
+        this._status.loadingQueueCount = 0;
+        for (let chunk of this.askServerChunks) {
+            this._status.loadingQueueCount += Object.keys(
                 chunk.updateDateByChunkKey
             ).length;
+        }
 
         this._statusSubject.next(this._status);
-
-        const status = new OfflineCacheStatusTuple();
-        status.pluginName = "peek_plugin_diagram";
-        status.indexName = "Branch Index";
-        status.loadingQueueCount = this._status.loadProgress;
-        status.totalLoadedCount = this._status.loadTotal;
-        status.lastCheckDate = new Date();
-        status.initialFullLoadComplete = this._status.initialLoadComplete;
-        this.deviceCacheControllerService.updateCachingStatus(status);
+        this.deviceCacheControllerService.updateLoaderCachingStatus(
+            this._status
+        );
     }
 
     /** Initial load
      *
      * Load the dates of the index buckets and ask the server if it has any updates.
      */
     private initialLoad(): void {
         this.storage
             .loadTuples(new UpdateDateTupleSelector())
             .then((tuplesAny: any[]) => {
                 let tuples: BranchIndexUpdateDateTuple[] = tuplesAny;
-                if (tuples.length != 0) {
+                if (tuples.length === 0) {
+                    this.index = new BranchIndexUpdateDateTuple();
+                } else {
                     this.index = tuples[0];
 
                     if (this.index.initialLoadComplete) {
                         this._hasLoaded = true;
                         this._notifyReady();
                     }
                 }
 
-                this.askServerForUpdates();
                 this._notifyStatus();
             });
-
-        this._notifyStatus();
     }
 
     private setupVortexSubscriptions(): void {
         // Services don't have destructors, I'm not sure how to unsubscribe.
         this.vortexService
             .createEndpointObservable(
                 this,
                 clientBranchIndexWatchUpdateFromDeviceFilt
             )
             .pipe(takeUntil(this.onDestroyEvent))
             .subscribe((payloadEnvelope: PayloadEnvelope) => {
                 this.processChunksFromServer(payloadEnvelope);
             });
-
-        // If the vortex service comes back online, update the watch grids.
-        this.vortexStatusService.isOnline
-            .pipe(filter((isOnline) => isOnline == true))
-            .pipe(takeUntil(this.onDestroyEvent))
-            .subscribe(() => this.askServerForUpdates());
     }
 
     private areWeTalkingToTheServer(): boolean {
         return (
             this.deviceCacheControllerService.offlineModeEnabled &&
             this.vortexStatusService.snapshot.isOnline
         );
@@ -362,15 +363,15 @@
         this.tupleService.observer
             .pollForTuples(new UpdateDateTupleSelector())
             .then((tuplesAny: any) => {
                 let serverIndex: BranchIndexUpdateDateTuple = tuplesAny[0];
                 let keys = Object.keys(serverIndex.updateDateByChunkKey);
                 let keysNeedingUpdate: string[] = [];
 
-                this._status.loadTotal = keys.length;
+                this._status.totalLoadedCount = keys.length;
 
                 // Tuples is an array of strings
                 for (let chunkKey of keys) {
                     if (
                         !this.index.updateDateByChunkKey.hasOwnProperty(
                             chunkKey
                         )
@@ -411,38 +412,37 @@
             }
         }
 
         if (count) this.askServerChunks.push(indexChunk);
 
         this.askServerForNextUpdateChunk();
 
-        this._status.lastCheck = new Date();
+        this._status.lastCheckDate = new Date();
     }
 
     private askServerForNextUpdateChunk() {
         if (!this.areWeTalkingToTheServer()) return;
 
         if (this.askServerChunks.length == 0) return;
 
-        this.deviceCacheControllerService //
-            .waitForGarbageCollector()
-            .then(() => {
-                let indexChunk: BranchIndexUpdateDateTuple =
-                    this.askServerChunks.pop();
-                let filt = extend(
-                    {},
-                    clientBranchIndexWatchUpdateFromDeviceFilt
-                );
-                filt[cacheAll] = true;
-                let pl = new Payload(filt, [indexChunk]);
-                this.vortexService.sendPayload(pl);
+        if (this.deviceCacheControllerService.isOfflineCachingPaused) {
+            this.saveChunkCacheIndex(true) //
+                .catch((e) => console.log(`ERROR saveChunkCacheIndex: ${e}`));
+            this._notifyStatus(true);
+            return;
+        }
 
-                this._status.lastCheck = new Date();
-                this._notifyStatus();
-            });
+        let indexChunk: BranchIndexUpdateDateTuple = this.askServerChunks.pop();
+        let filt = extend({}, clientBranchIndexWatchUpdateFromDeviceFilt);
+        filt[cacheAll] = true;
+        let pl = new Payload(filt, [indexChunk]);
+        this.vortexService.sendPayload(pl);
+
+        this._status.lastCheckDate = new Date();
+        this._notifyStatus();
     }
 
     /** Process BranchIndexes From Server
      *
      * Process the grids the server has sent us.
      */
     private async processChunksFromServer(
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/branch-loader/BranchIndexUpdateDateTuple.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/branch-loader/BranchIndexUpdateDateTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/branch-loader/LocalBranchStorageService.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/branch-loader/LocalBranchStorageService.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/grid-loader/EncodedGridTuple.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/grid-loader/EncodedGridTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/grid-loader/GridUpdateDateTuple.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/grid-loader/GridUpdateDateTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/grid-loader/PrivateDiagramGridLoaderService.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/grid-loader/PrivateDiagramGridLoaderService.ts`

 * *Files 9% similar despite different names*

```diff
@@ -15,19 +15,18 @@
     VortexService,
     VortexStatusService,
     TupleStorageBatchSaveArguments,
 } from "@synerty/vortexjs";
 import { diagramFilt, gridCacheStorageName } from "../PluginNames";
 import { GridUpdateDateTuple } from "./GridUpdateDateTuple";
 import { PrivateDiagramTupleService } from "../services";
-import { PrivateDiagramGridLoaderStatusTuple } from "./PrivateDiagramGridLoaderStatusTuple";
 import { EncodedGridTuple } from "./EncodedGridTuple";
 import {
     DeviceOfflineCacheService,
-    OfflineCacheStatusTuple,
+    OfflineCacheLoaderStatusTuple,
 } from "@peek/peek_core_device";
 
 // ----------------------------------------------------------------------------
 
 let clientGridWatchUpdateFromDeviceFilt = extend(
     { key: "clientGridWatchUpdateFromDevice" },
     diagramFilt
@@ -96,64 +95,82 @@
 
     // All cached grid dates
     private index: GridUpdateDateTuple = new GridUpdateDateTuple();
 
     // The queue of grids to cache
     private askServerChunks = [];
 
-    private _statusSubject = new Subject<PrivateDiagramGridLoaderStatusTuple>();
-    private _status = new PrivateDiagramGridLoaderStatusTuple();
+    private _statusSubject = new Subject<OfflineCacheLoaderStatusTuple>();
+    private _status = new OfflineCacheLoaderStatusTuple();
 
     constructor(
         private vortexService: VortexService,
         private vortexStatusService: VortexStatusService,
         private tupleService: PrivateDiagramTupleService,
         storageFactory: TupleStorageFactoryService,
         private deviceCacheControllerService: DeviceOfflineCacheService
     ) {
         super();
 
+        this._status.pluginName = "peek_plugin_diagram";
+        this._status.indexName = "Grids";
+
         this.storage = storageFactory.create(
             new TupleOfflineStorageNameService(gridCacheStorageName)
         );
         this.storage
             .open()
             .then(() => this.loadGridCacheIndex())
             .then(() => this.isReadySubject.next(true))
             .catch((e) => console.log(`Failed to open grid cache db ${e}`));
 
         this.setupVortexSubscriptions();
-        this._notifyStatus();
 
-        this.deviceCacheControllerService.triggerCachingObservable
+        // This is loaded regardless for the GridLoader
+        // this.deviceCacheControllerService.offlineModeEnabled$
+        //     .pipe(takeUntil(this.onDestroyEvent))
+        //     .pipe(filter((v) => v))
+        //     .pipe(first())
+        //     .subscribe(() => {
+        //         this.initialLoad();
+        //     });
+
+        this.deviceCacheControllerService.triggerCachingStartObservable
             .pipe(takeUntil(this.onDestroyEvent))
             .pipe(filter((v) => v))
             .subscribe(() => {
                 this.askServerForUpdates();
                 this._notifyStatus();
             });
+
+        this.deviceCacheControllerService.triggerCachingResumeObservable
+            .pipe(takeUntil(this.onDestroyEvent))
+            .subscribe(() => {
+                this._notifyStatus();
+                this.askServerForNextUpdateChunk();
+            });
     }
 
     get observable(): Observable<GridTuple[]> {
         return this.updatesObservable;
     }
 
     isReady(): Promise<boolean> {
         return this.storage.isOpen();
     }
 
     isReadyObservable(): Observable<boolean> {
         return this.isReadySubject;
     }
 
-    statusObservable(): Observable<PrivateDiagramGridLoaderStatusTuple> {
+    statusObservable(): Observable<OfflineCacheLoaderStatusTuple> {
         return this._statusSubject;
     }
 
-    status(): PrivateDiagramGridLoaderStatusTuple {
+    status(): OfflineCacheLoaderStatusTuple {
         return this._status;
     }
 
     /** Update Watched Grids
      *
      * Change the list of grids that the GridObserver is interested in.
      */
@@ -176,51 +193,36 @@
         // we can send to the server.
         for (let gridTuple of gridTuples)
             currentGridUpdateTimes[gridTuple.gridKey] = gridTuple.lastUpdate;
 
         this.sendWatchedGridsToServer(currentGridUpdateTimes);
     }
 
-    private _notifyStatus(): void {
-        this._status.cacheForOfflineEnabled =
-            this.deviceCacheControllerService.cachingEnabled;
-        this._status.initialLoadComplete = this.index.initialLoadComplete;
+    private _notifyStatus(paused: boolean = false): void {
+        this._status.lastCheckDate = new Date();
+        this._status.paused = paused;
+        this._status.initialFullLoadComplete = this.index.initialLoadComplete;
 
-        this._status.loadProgress = Object.values(
+        this._status.loadingQueueCount = Object.values(
             this.index.updateDateByChunkKey
-        ).filter((v) => v != null).length;
+        ).filter((v) => v == null).length;
 
         this._statusSubject.next(this._status);
-
-        const status = new OfflineCacheStatusTuple();
-        status.pluginName = "peek_plugin_diagram";
-        status.indexName = "Grids";
-        status.loadingQueueCount = this._status.loadProgress;
-        status.totalLoadedCount = this._status.loadTotal;
-        status.lastCheckDate = new Date();
-        status.initialFullLoadComplete = this._status.initialLoadComplete;
-        this.deviceCacheControllerService.updateCachingStatus(status);
+        this.deviceCacheControllerService.updateLoaderCachingStatus(
+            this._status
+        );
     }
 
     private setupVortexSubscriptions(): void {
         // Services don't have destructors, I'm not sure how to unsubscribe.
         this.vortexService
             .createEndpointObservable(this, clientGridWatchUpdateFromDeviceFilt)
             .subscribe((payloadEnvelope: PayloadEnvelope) =>
                 this.processChunksFromServer(payloadEnvelope)
             );
-
-        // If the vortex service comes back online, update the watch grids.
-        this.vortexStatusService.isOnline
-            .pipe(filter((isOnline) => isOnline == true))
-            .pipe(takeUntil(this.onDestroyEvent))
-            .subscribe(() => {
-                this.loadGrids({}, this.lastWatchedGridKeys);
-                this.askServerForUpdates();
-            });
     }
 
     private areWeTalkingToTheServer(): boolean {
         return (
             this.deviceCacheControllerService.offlineModeEnabled &&
             this.vortexStatusService.snapshot.isOnline
         );
@@ -242,15 +244,15 @@
 
         let keysNeedingUpdate: string[] = [];
         let total = 0;
         let start = 0;
         let chunkSize = 5000;
 
         let complete = () => {
-            this._status.loadTotal = total;
+            this._status.totalLoadedCount = total;
             this.queueChunksToAskServer(keysNeedingUpdate);
         };
 
         // This is one big hoop to avoid memory issues on older iOS devices
         let queueNext = () => {
             const offset = start + chunkSize;
             let ts = new TupleSelector(GridUpdateDateTuple.tupleName, {
@@ -273,15 +275,15 @@
                                 " Load of GridUpdateDateTuple Complete"
                         );
                         complete();
                         return;
                     }
 
                     total += tuples.length;
-                    this._status.loadTotal = total;
+                    this._status.totalLoadedCount = total;
 
                     for (let item of tuples) {
                         let chunkKey = item[0];
                         let lastUpdate = item[1];
 
                         if (
                             !this.index.updateDateByChunkKey.hasOwnProperty(
@@ -293,15 +295,15 @@
                         } else if (
                             this.index.updateDateByChunkKey[chunkKey] !=
                             lastUpdate
                         ) {
                             keysNeedingUpdate.push(chunkKey);
                         }
                     }
-                    this._status.lastCheck = new Date();
+                    this._status.lastCheckDate = new Date();
                     this._notifyStatus();
                     setTimeout(() => queueNext(), 0);
                 })
                 .catch((e) => console.log(`ERROR in cacheAll : ${e}`));
         };
         queueNext();
     }
@@ -329,39 +331,42 @@
             }
         }
 
         if (count) this.askServerChunks.push(indexChunk);
 
         this.askServerForNextUpdateChunk();
 
-        this._status.lastCheck = new Date();
+        this._status.lastCheckDate = new Date();
         this._notifyStatus();
     }
 
     /** Cache Request Next Chunk
      *
      * Request the next chunk of grids from the server
      */
     private askServerForNextUpdateChunk() {
         if (!this.areWeTalkingToTheServer()) return;
 
         if (this.askServerChunks.length == 0) return;
 
-        this.deviceCacheControllerService //
-            .waitForGarbageCollector()
-            .then(() => {
-                let nextChunk = this.askServerChunks.pop();
-
-                let payload = new Payload({ cacheAll: true }, [nextChunk]);
-                extend(payload.filt, clientGridWatchUpdateFromDeviceFilt);
-                this.vortexService.sendPayload(payload);
+        if (this.deviceCacheControllerService.isOfflineCachingPaused) {
+            this.saveChunkCacheIndex(true) //
+                .catch((e) => console.log(`ERROR saveChunkCacheIndex: ${e}`));
+            this._notifyStatus(true);
+            return;
+        }
 
-                this._status.lastCheck = new Date();
-                this._notifyStatus();
-            });
+        let nextChunk = this.askServerChunks.pop();
+
+        let payload = new Payload({ cacheAll: true }, [nextChunk]);
+        extend(payload.filt, clientGridWatchUpdateFromDeviceFilt);
+        this.vortexService.sendPayload(payload);
+
+        this._status.lastCheckDate = new Date();
+        this._notifyStatus();
     }
 
     //
     private sendWatchedGridsToServer(updateTimeByGridKey: {
         [gridKey: string]: string;
     }) {
         // There is no point talking to the server if it's offline
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/location-loader/DispKeyLocationTuple.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/location-loader/DispKeyLocationTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/location-loader/EncodedLocationIndexTuple.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/location-loader/EncodedLocationIndexTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/location-loader/PrivateDiagramLocationLoaderService.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/location-loader/PrivateDiagramLocationLoaderService.ts`

 * *Files 3% similar despite different names*

```diff
@@ -20,19 +20,18 @@
     locationIndexCacheStorageName,
 } from "@peek/peek_plugin_diagram/_private";
 import { DiagramCoordSetService } from "@peek/peek_plugin_diagram/DiagramCoordSetService";
 import { LocationIndexUpdateDateTuple } from "./LocationIndexUpdateDateTuple";
 import { DispKeyLocationTuple } from "./DispKeyLocationTuple";
 import { PrivateDiagramCoordSetService } from "../services/PrivateDiagramCoordSetService";
 import { EncodedLocationIndexTuple } from "./EncodedLocationIndexTuple";
-import { PrivateDiagramLocationLoaderStatusTuple } from "./PrivateDiagramLocationLoaderStatusTuple";
 import { PrivateDiagramTupleService } from "../services/PrivateDiagramTupleService";
 import {
     DeviceOfflineCacheService,
-    OfflineCacheStatusTuple,
+    OfflineCacheLoaderStatusTuple,
 } from "@peek/peek_core_device";
 
 // ----------------------------------------------------------------------------
 
 let clientLocationIndexWatchUpdateFromDeviceFilt = extend(
     { key: "clientLocationIndexWatchUpdateFromDevice" },
     diagramFilt
@@ -111,71 +110,89 @@
 
     // Every 100 chunks from the server
     private SAVE_POINT_ITERATIONS = 100;
 
     // Saving the cache after each chunk is so expensive, we only do it every 20 or so
     private chunksSavedSinceLastIndexSave = 0;
 
-    private index = new LocationIndexUpdateDateTuple();
+    private index: LocationIndexUpdateDateTuple | null = null;
     private askServerChunks: LocationIndexUpdateDateTuple[] = [];
 
     private _hasLoaded = false;
     private _hasLoadedSubject = new Subject<void>();
 
     private storage: TupleOfflineStorageService;
 
-    private _statusSubject =
-        new Subject<PrivateDiagramLocationLoaderStatusTuple>();
-    private _status = new PrivateDiagramLocationLoaderStatusTuple();
+    private _statusSubject = new Subject<OfflineCacheLoaderStatusTuple>();
+    private _status = new OfflineCacheLoaderStatusTuple();
 
     private coordSetService: PrivateDiagramCoordSetService;
 
     constructor(
         private vortexService: VortexService,
         private vortexStatusService: VortexStatusService,
         storageFactory: TupleStorageFactoryService,
         abstractCoordSetService: DiagramCoordSetService,
         private tupleService: PrivateDiagramTupleService,
         private deviceCacheControllerService: DeviceOfflineCacheService
     ) {
         super();
+
+        this._status.pluginName = "peek_plugin_diagram";
+        this._status.indexName = "Position";
+
         this.coordSetService = <PrivateDiagramCoordSetService>(
             abstractCoordSetService
         );
 
         this.storage = new TupleOfflineStorageService(
             storageFactory,
             new TupleOfflineStorageNameService(locationIndexCacheStorageName)
         );
 
         this.setupVortexSubscriptions();
-        this._notifyStatus();
 
-        this.deviceCacheControllerService.triggerCachingObservable
+        this.deviceCacheControllerService.offlineModeEnabled$
             .pipe(takeUntil(this.onDestroyEvent))
             .pipe(filter((v) => v))
+            .pipe(first())
             .subscribe(() => {
                 this.initialLoad();
+            });
+
+        this.deviceCacheControllerService.triggerCachingStartObservable
+            .pipe(takeUntil(this.onDestroyEvent))
+            .pipe(filter((v) => v))
+            .subscribe(() => {
+                this.askServerForUpdates();
+                this._notifyStatus();
+            });
+
+        this.deviceCacheControllerService.triggerCachingResumeObservable
+            .pipe(takeUntil(this.onDestroyEvent))
+
+            .subscribe(() => {
                 this._notifyStatus();
+                this.askServerForNextUpdateChunk();
             });
     }
 
     isReady(): boolean {
         return this._hasLoaded;
     }
 
     isReadyObservable(): Observable<void> {
         return this._hasLoadedSubject;
     }
 
-    statusObservable(): Observable<PrivateDiagramLocationLoaderStatusTuple> {
+    statusObservable(): Observable<OfflineCacheLoaderStatusTuple> {
         return this._statusSubject;
     }
 
-    status(): PrivateDiagramLocationLoaderStatusTuple {
+    status(): OfflineCacheLoaderStatusTuple {
         return this._status;
     }
 
     /** Get Locations
      *
      * Get the location of a Disp.key from the index..
      *
@@ -228,81 +245,71 @@
 
         return this.isReadyObservable()
             .pipe(first())
             .toPromise()
             .then(() => this.getLocationsFromLocal(modelSetKey, dispKey));
     }
 
-    private _notifyStatus(): void {
-        this._status.cacheForOfflineEnabled =
-            this.deviceCacheControllerService.cachingEnabled;
-        this._status.initialLoadComplete = this.index.initialLoadComplete;
-
-        this._status.loadProgress = Object.keys(
-            this.index.updateDateByChunkKey
-        ).length;
-        for (let chunk of this.askServerChunks)
-            this._status.loadProgress -= Object.keys(
+    private _notifyReady(): void {
+        if (this._hasLoaded) this._hasLoadedSubject.next();
+    }
+
+    private _notifyStatus(paused: boolean = false): void {
+        this._status.lastCheckDate = new Date();
+        this._status.paused = paused;
+        this._status.initialFullLoadComplete = this.index.initialLoadComplete;
+
+        this._status.loadingQueueCount = 0;
+        for (let chunk of this.askServerChunks) {
+            this._status.loadingQueueCount += Object.keys(
                 chunk.updateDateByChunkKey
             ).length;
+        }
 
         this._statusSubject.next(this._status);
-
-        const status = new OfflineCacheStatusTuple();
-        status.pluginName = "peek_plugin_diagram";
-        status.indexName = "Position";
-        status.loadingQueueCount = this._status.loadProgress;
-        status.totalLoadedCount = this._status.loadTotal;
-        status.lastCheckDate = new Date();
-        status.initialFullLoadComplete = this._status.initialLoadComplete;
-        this.deviceCacheControllerService.updateCachingStatus(status);
+        this.deviceCacheControllerService.updateLoaderCachingStatus(
+            this._status
+        );
     }
 
     /** Initial load
      *
      * Load the dates of the index buckets and ask the server if it has any updates.
      */
     private initialLoad(): void {
         this.storage
             .loadTuples(new UpdateDateTupleSelector())
             .then((tuplesAny: any[]) => {
                 let tuples: LocationIndexUpdateDateTuple[] = tuplesAny;
-                if (tuples.length != 0) {
+                if (tuples.length === 0) {
+                    this.index = new LocationIndexUpdateDateTuple();
+                } else {
                     this.index = tuples[0];
 
                     if (this.index.initialLoadComplete) {
                         this._hasLoaded = true;
-                        this._hasLoadedSubject.next();
+                        this._notifyReady();
                     }
                 }
 
-                this.askServerForUpdates();
                 this._notifyStatus();
             });
-
-        this._notifyStatus();
     }
 
     private setupVortexSubscriptions(): void {
         // Services don't have destructors, I'm not sure how to unsubscribe.
         this.vortexService
             .createEndpointObservable(
                 this,
                 clientLocationIndexWatchUpdateFromDeviceFilt
             )
             .pipe(takeUntil(this.onDestroyEvent))
             .subscribe((payloadEnvelope: PayloadEnvelope) => {
                 this.processChunksFromServer(payloadEnvelope);
             });
-
-        // If the vortex service comes back online, update the watch grids.
-        this.vortexStatusService.isOnline
-            .pipe(filter((isOnline) => isOnline == true))
-            .pipe(takeUntil(this.onDestroyEvent))
-            .subscribe(() => this.askServerForUpdates());
     }
 
     private areWeTalkingToTheServer(): boolean {
         return (
             this.deviceCacheControllerService.offlineModeEnabled &&
             this.vortexStatusService.snapshot.isOnline
         );
@@ -326,15 +333,15 @@
         this.tupleService.observer
             .pollForTuples(new UpdateDateTupleSelector())
             .then((tuplesAny: any) => {
                 let serverIndex: LocationIndexUpdateDateTuple = tuplesAny[0];
                 let keys = Object.keys(serverIndex.updateDateByChunkKey);
                 let keysNeedingUpdate: string[] = [];
 
-                this._status.loadTotal = keys.length;
+                this._status.totalLoadedCount = keys.length;
 
                 // Tuples is an array of strings
                 for (let chunkKey of keys) {
                     if (
                         !this.index.updateDateByChunkKey.hasOwnProperty(
                             chunkKey
                         )
@@ -382,40 +389,40 @@
             }
         }
 
         if (count) this.askServerChunks.push(indexChunk);
 
         this.askServerForNextUpdateChunk();
 
-        this._status.lastCheck = new Date();
+        this._status.lastCheckDate = new Date();
         this._notifyStatus();
     }
 
     private askServerForNextUpdateChunk() {
         if (!this.areWeTalkingToTheServer()) return;
 
         if (this.askServerChunks.length == 0) return;
 
-        this.deviceCacheControllerService //
-            .waitForGarbageCollector()
-            .then(() => {
-                let indexChunk: LocationIndexUpdateDateTuple =
-                    this.askServerChunks.pop();
-
-                let filt = extend(
-                    {},
-                    clientLocationIndexWatchUpdateFromDeviceFilt
-                );
-                filt[cacheAll] = true;
-                let payload = new Payload(filt, [indexChunk]);
-                this.vortexService.sendPayload(payload);
+        if (this.deviceCacheControllerService.isOfflineCachingPaused) {
+            this.saveChunkCacheIndex(true) //
+                .catch((e) => console.log(`ERROR saveChunkCacheIndex: ${e}`));
+            this._notifyStatus(true);
+            return;
+        }
 
-                this._status.lastCheck = new Date();
-                this._notifyStatus();
-            });
+        let indexChunk: LocationIndexUpdateDateTuple =
+            this.askServerChunks.pop();
+
+        let filt = extend({}, clientLocationIndexWatchUpdateFromDeviceFilt);
+        filt[cacheAll] = true;
+        let payload = new Payload(filt, [indexChunk]);
+        this.vortexService.sendPayload(payload);
+
+        this._status.lastCheckDate = new Date();
+        this._notifyStatus();
     }
 
     /** Process LocationIndexes From Server
      *
      * Process the grids the server has sent us.
      */
     private async processChunksFromServer(
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramConfigService.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramConfigService.ts`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import { Injectable } from "@angular/core";
-import { Observable, Subject } from "rxjs";
+import { BehaviorSubject, Observable, Subject } from "rxjs";
 import { NgLifeCycleEvents } from "@synerty/vortexjs";
 import { PrivateDiagramLookupService } from "./PrivateDiagramLookupService";
 import { DiagramConfigService } from "../../DiagramConfigService";
-import { DiagramToolbarService } from "@peek/peek_plugin_diagram";
+import { DiagramToolbarService } from "@peek/peek_plugin_diagram/DiagramToolbarService";
 import { DiagramToolbarBuiltinButtonEnum } from "@peek/peek_plugin_diagram/DiagramToolbarService";
 
 export interface PopupLayerSelectionArgsI {
     modelSetKey: string;
     coordSetKey: string;
 }
 
@@ -16,30 +16,29 @@
     coordSetKey: string;
 }
 
 /** CoordSetCache
  *
  * This class is responsible for buffering the coord sets in memory.
  *
- * Typically there will be less than 20 of these.
+ * Typically, there will be less than 20 of these.
  *
  */
 @Injectable()
 export class PrivateDiagramConfigService
     extends NgLifeCycleEvents
     implements DiagramConfigService
 {
     private _popupLayerSelectionSubject: Subject<PopupLayerSelectionArgsI> =
         new Subject<PopupLayerSelectionArgsI>();
 
     private _popupBranchSelectionSubject: Subject<PopupBranchSelectionArgsI> =
         new Subject<PopupBranchSelectionArgsI>();
 
-    private _useEdgeColorChangedSubject: Subject<boolean> =
-        new Subject<boolean>();
+    private _useEdgeColorChangedSubject = new BehaviorSubject<boolean>(false);
 
     private _layersUpdatedSubject: Subject<void> = new Subject<void>();
 
     constructor(
         private lookupService: PrivateDiagramLookupService,
         private diagramToolbarService: DiagramToolbarService
     ) {
@@ -79,17 +78,21 @@
     // ---------------
     // Use Polyline Edge Colors
     /** This is a published polyline */
     setUsePolylineEdgeColors(enabled: boolean): void {
         this._useEdgeColorChangedSubject.next(enabled);
     }
 
+    usePolylineEdgeColors(): boolean {
+        return this._useEdgeColorChangedSubject.getValue();
+    }
+
     /** This observable is subscribed to by the canvas component */
     usePolylineEdgeColorsObservable(): Observable<boolean> {
-        return this._useEdgeColorChangedSubject;
+        return this._useEdgeColorChangedSubject.asObservable();
     }
 
     // ---------------
     // Use Polyline Edge Colors
     /** This is a published polyline */
     setLayerVisible(
         modelSetKey: string,
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramCoordSetService.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramCoordSetService.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramItemSelectService.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramItemSelectService.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramLookupService.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramLookupService.ts`

 * *Files 6% similar despite different names*

```diff
@@ -4,17 +4,22 @@
 import { NgLifeCycleEvents, TupleSelector } from "@synerty/vortexjs";
 import {
     DispColor,
     DispLayer,
     DispLevel,
     DispLineStyle,
     DispTextStyle,
-} from "../../lookups";
+} from "../lookups";
 import { PrivateDiagramTupleService } from "./PrivateDiagramTupleService";
 import { ModelSet } from "../tuples";
+import { PrivateDiagramCoordSetService } from "@peek/peek_plugin_diagram/_private/services/PrivateDiagramCoordSetService";
+import {
+    ShapeLayerTuple,
+    ShapeLevelTuple,
+} from "@peek/peek_plugin_diagram/lookup_tuples";
 
 let dictValuesFromObject = (dict) => Object.keys(dict).map((key) => dict[key]);
 
 /** Lookup Cache
  *
  * This class provides handy access to the lookup objects
  *
@@ -48,15 +53,18 @@
     private subscriptions = [];
     private _isReady: boolean = false;
     private _isReadySubject: Subject<boolean> = new Subject<boolean>();
     private modelSetByKey: { [key: string]: ModelSet } = {};
     private dispsNeedRelinkingSubject = new Subject<void>();
     private dispsNeedRelinking = false;
 
-    constructor(private tupleService: PrivateDiagramTupleService) {
+    constructor(
+        private tupleService: PrivateDiagramTupleService,
+        private coordSetService: PrivateDiagramCoordSetService
+    ) {
         super();
 
         const modelSetTs = new TupleSelector(ModelSet.tupleName, {});
         this.tupleService.offlineObserver
             .subscribeToTupleSelector(modelSetTs)
             .pipe(takeUntil(this.onDestroyEvent))
             .subscribe((modelSets: ModelSet[]) => {
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramOfflineCacherService.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramOfflineCacherService.ts`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import { GroupDispsTuple, ModelCoordSet, ModelSet } from "../tuples";
 import {
     DispColor,
     DispLayer,
     DispLevel,
     DispLineStyle,
     DispTextStyle,
-} from "../../lookups";
+} from "../lookups";
 import { BranchKeyToIdMapTuple } from "../branch/BranchKeyToIdMapTuple";
 import { BranchService } from "@peek/peek_plugin_branch";
 
 /** Diagram Lookups offline cacher
  *
  * This Service is never unloaded, it makes sure that the lookups that the diagram
  * needs are always stored in the local DB.
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramOverrideService.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramOverrideService.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramPositionService.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramPositionService.ts`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import { Injectable } from "@angular/core";
 import {
+    CoordSetViewWindowI,
     DiagramPositionService,
     DispKeyLocation,
     OptionalPositionArgsI,
     PositionUpdatedI,
 } from "../../DiagramPositionService";
-import { Observable, Subject } from "rxjs";
+import { BehaviorSubject, Observable, Subject } from "rxjs";
 
 import { DispKeyLocationTuple } from "../location-loader/DispKeyLocationTuple";
 import { BalloonMsgService } from "@synerty/peek-plugin-base-js";
 import { PrivateDiagramLocationLoaderService } from "../location-loader";
 import { PrivateDiagramCoordSetService } from "./PrivateDiagramCoordSetService";
 
 export interface DiagramPositionI {
@@ -37,15 +38,19 @@
     // This observable is for when the canvas updates the title
     private titleUpdatedSubject: Subject<string> = new Subject<string>();
     private positionByCoordSetSubject =
         new Subject<DiagramPositionByCoordSetI>();
     private positionSubject = new Subject<DiagramPositionI>();
     private positionByKeySubject = new Subject<DiagramPositionByKeyI>();
     private isReadySubject = new Subject<boolean>();
+
     private positionUpdatedSubject = new Subject<PositionUpdatedI>();
+    private coordSetViewSubject =
+        new BehaviorSubject<null | CoordSetViewWindowI>(null);
+
     private selectKeysSubject = new Subject<string[]>();
 
     constructor(
         private coordSetService: PrivateDiagramCoordSetService,
         private locationIndexService: PrivateDiagramLocationLoaderService,
         private balloonMsg: BalloonMsgService
     ) {
@@ -228,26 +233,38 @@
         this.isReadySubject.next(true);
     }
 
     setTitle(value: string) {
         this.titleUpdatedSubject.next(value);
     }
 
-    positionUpdated(pos: PositionUpdatedI): void {
+    positionUpdated(
+        pos: PositionUpdatedI,
+        coordSetViewData: CoordSetViewWindowI
+    ): void {
         this.positionUpdatedSubject.next(pos);
+        this.coordSetViewSubject.next(coordSetViewData);
     }
 
     isReadyObservable(): Observable<boolean> {
         return this.isReadySubject;
     }
 
     positionUpdatedObservable(): Observable<PositionUpdatedI> {
         return this.positionUpdatedSubject;
     }
 
+    coordSetViewUpdatedObservable(): Observable<CoordSetViewWindowI | null> {
+        return this.coordSetViewSubject.asObservable();
+    }
+
+    coordSetView(): CoordSetViewWindowI | null {
+        return this.coordSetViewSubject.getValue();
+    }
+
     titleUpdatedObservable(): Observable<string> {
         return this.titleUpdatedSubject;
     }
 
     positionObservable(): Observable<DiagramPositionI> {
         return this.positionSubject;
     }
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramSnapshotService.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramSnapshotService.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramToolbarService.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramToolbarService.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramTupleService.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramTupleService.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/tuples/GroupDispsTuple.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/tuples/GroupDispsTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/_private/tuples/ModelCoordSet.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/_private/tuples/ModelCoordSet.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/index.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/index.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/lookups/DispLevel.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/lookup_tuples/ShapeLevelTuple.ts`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import { addTupleType, Tuple } from "@synerty/vortexjs";
 import { diagramTuplePrefix } from "@peek/peek_plugin_diagram/_private";
 
 @addTupleType
-export class DispLevel extends Tuple {
-    public static readonly tupleName = diagramTuplePrefix + "DispLevel";
+export class ShapeLevelTuple extends Tuple {
+    public static readonly tupleName = diagramTuplePrefix + "ShapeLevelTuple";
 
-    id: number;
+    key: string;
+    modelSetKey: string;
+    coordSetKey: string;
     name: string;
     order: number;
     minZoom: number;
     maxZoom: number;
-    coordSetId: number;
     showForEdit: boolean;
 
     constructor() {
-        super(DispLevel.tupleName);
+        super(ShapeLevelTuple.tupleName);
     }
 
     isVisibleAtZoom(zoom: number): boolean {
         return this.minZoom <= zoom && zoom < this.maxZoom;
     }
 }
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/lookups/DispTextStyle.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/lookup_tuples/ShapeTextStyleTuple.ts`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import { addTupleType, Tuple } from "@synerty/vortexjs";
 import { diagramTuplePrefix } from "@peek/peek_plugin_diagram/_private";
 
 @addTupleType
-export class DispTextStyle extends Tuple {
-    public static readonly tupleName = diagramTuplePrefix + "DispTextStyle";
+export class ShapeTextStyleTuple extends Tuple {
+    public static readonly tupleName =
+        diagramTuplePrefix + "ShapeTextStyleTuple";
+
+    key: string;
+    modelSetKey: string;
 
-    id: number;
     name: string;
     fontName: string;
     fontSize: number;
     fontStyle: string | null;
     scalable: boolean;
     scaleFactor: number;
-    modelSetId: number;
     spacingBetweenTexts: number;
     borderWidth: number;
     showForEdit: boolean;
+    wrapTextAtChars: number;
 
     constructor() {
-        super(DispTextStyle.tupleName);
+        super(ShapeTextStyleTuple.tupleName);
     }
 }
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/override/DiagramOverrideBase.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/override/DiagramOverrideBase.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/override/DiagramOverrideColor.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/override/DiagramOverrideColor.ts`

 * *Files 21% similar despite different names*

```diff
@@ -1,67 +1,67 @@
 import {
     DiagramOverrideBase,
     DiagramOverrideTypeE,
 } from "./DiagramOverrideBase";
 import { addTupleType } from "@synerty/vortexjs";
-import { DispColor } from "../lookups";
 import { diagramTuplePrefix } from "../_private/PluginNames";
+import { ShapeColorTuple } from "@peek/peek_plugin_diagram/lookup_tuples";
 
 /** Diagram Delta Color Override Tuple
  *
  * This delta applies an override colour to a set of display keys
  *
  */
 @addTupleType
 export class DiagramOverrideColor extends DiagramOverrideBase {
     public static readonly tupleName =
         diagramTuplePrefix + "DiagramOverrideColor";
 
     private dispKeys_ = [];
-    private lineColor_: DispColor | null = null;
-    private fillColor_: DispColor | null = null;
-    private color_: DispColor | null = null;
+    private lineColor_: ShapeColorTuple | null = null;
+    private fillColor_: ShapeColorTuple | null = null;
+    private color_: ShapeColorTuple | null = null;
 
     constructor(modelSetKey: string, coordSetKey: string) {
         super(
             modelSetKey,
             coordSetKey,
             DiagramOverrideTypeE.Color,
             DiagramOverrideColor.tupleName
         );
     }
 
     get dispKeys(): string[] {
         return this.dispKeys_;
     }
 
-    get lineColor(): DispColor {
+    get lineColor(): ShapeColorTuple {
         return this.lineColor_;
     }
 
-    get fillColor(): DispColor {
+    get fillColor(): ShapeColorTuple {
         return this.fillColor_;
     }
 
-    get color(): DispColor {
+    get color(): ShapeColorTuple {
         return this.color_;
     }
 
     addDispKeys(dispKeys: string[]): void {
         this.dispKeys_.add(dispKeys);
     }
 
     // Line Color
-    setLineColor(value: DispColor | null): void {
+    setLineColor(value: ShapeColorTuple | null): void {
         this.lineColor_ = value;
     }
 
     // Fill Color
-    setFillColor(value: DispColor | null): void {
+    setFillColor(value: ShapeColorTuple | null): void {
         this.fillColor_ = value;
     }
 
     // Color
-    setColor(value: DispColor | null): void {
+    setColor(value: ShapeColorTuple | null): void {
         this.color_ = value;
     }
 }
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin-module/override/DiagramOverrideHighlight.ts` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin-module/override/DiagramOverrideHighlight.ts`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import {
     DiagramOverrideBase,
     DiagramOverrideTypeE,
 } from "./DiagramOverrideBase";
 import { addTupleType } from "@synerty/vortexjs";
-import { DispColor } from "../lookups";
+import { DispColor } from "../_private/lookups";
 import { diagramTuplePrefix } from "../_private/PluginNames";
 
 /** Diagram Delta Color Override Tuple
  *
  * This delta applies an override colour to a set of display keys
  *
  */
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/plugin_package.json` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/plugin_package.json`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 00000000: 7b0a 2020 2020 2270 6c75 6769 6e22 3a20  {.    "plugin": 
 00000010: 7b0a 2020 2020 2020 2020 2274 6974 6c65  {.        "title
 00000020: 223a 2022 4469 6167 7261 6d22 2c0a 2020  ": "Diagram",.  
 00000030: 2020 2020 2020 2270 6163 6b61 6765 4e61        "packageNa
 00000040: 6d65 223a 2022 7065 656b 5f70 6c75 6769  me": "peek_plugi
 00000050: 6e5f 6469 6167 7261 6d22 2c0a 2020 2020  n_diagram",.    
 00000060: 2020 2020 2276 6572 7369 6f6e 223a 2022      "version": "
-00000070: 332e 332e 3322 2c0a 2020 2020 2020 2020  3.3.3",.        
+00000070: 332e 342e 3022 2c0a 2020 2020 2020 2020  3.4.0",.        
 00000080: 2262 7569 6c64 4e75 6d62 6572 223a 2022  "buildNumber": "
 00000090: 2350 4c55 4749 4e5f 4255 494c 4423 222c  #PLUGIN_BUILD#",
 000000a0: 0a20 2020 2020 2020 2022 6275 696c 6444  .        "buildD
 000000b0: 6174 6522 3a20 2223 4255 494c 445f 4441  ate": "#BUILD_DA
 000000c0: 5445 2322 2c0a 2020 2020 2020 2020 2263  TE#",.        "c
 000000d0: 7265 6174 6f72 223a 2022 5379 6e65 7274  reator": "Synert
 000000e0: 7920 5074 7920 4c74 6422 2c0a 2020 2020  y Pty Ltd",.    
@@ -65,638 +65,624 @@
 00000400: 6772 616d 222c 0a20 2020 2020 2020 2022  gram",.        "
 00000410: 7368 6f77 486f 6d65 4c69 6e6b 223a 2066  showHomeLink": f
 00000420: 616c 7365 2c0a 2020 2020 2020 2020 2261  alse,.        "a
 00000430: 7070 4469 7222 3a20 225f 7072 6976 6174  ppDir": "_privat
 00000440: 652f 626f 7468 2d61 7070 222c 0a20 2020  e/both-app",.   
 00000450: 2020 2020 2022 6d6f 6475 6c65 4469 7222       "moduleDir"
 00000460: 3a20 2270 6c75 6769 6e2d 6d6f 6475 6c65  : "plugin-module
-00000470: 222c 0a20 2020 2020 2020 2022 6366 6744  ",.        "cfgD
-00000480: 6972 223a 2022 5f70 7269 7661 7465 2f62  ir": "_private/b
-00000490: 6f74 682d 6366 6722 2c0a 2020 2020 2020  oth-cfg",.      
-000004a0: 2020 2263 6667 4d6f 6475 6c65 223a 2022    "cfgModule": "
-000004b0: 6469 6167 7261 6d2d 6366 672e 6d6f 6475  diagram-cfg.modu
-000004c0: 6c65 2344 6961 6772 616d 4366 674d 6f64  le#DiagramCfgMod
-000004d0: 756c 6522 2c0a 2020 2020 2020 2020 2272  ule",.        "r
-000004e0: 6f6f 7453 6572 7669 6365 7322 3a20 5b0a  ootServices": [.
-000004f0: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
-00000500: 2020 2020 2020 2020 2020 2020 2020 2266                "f
-00000510: 696c 6522 3a20 225f 7072 6976 6174 652f  ile": "_private/
-00000520: 7365 7276 6963 6573 2f50 7269 7661 7465  services/Private
-00000530: 4469 6167 7261 6d54 7570 6c65 5365 7276  DiagramTupleServ
-00000540: 6963 6522 2c0a 2020 2020 2020 2020 2020  ice",.          
-00000550: 2020 2020 2020 2263 6c61 7373 223a 2022        "class": "
-00000560: 5072 6976 6174 6544 6961 6772 616d 5475  PrivateDiagramTu
-00000570: 706c 6553 6572 7669 6365 220a 2020 2020  pleService".    
-00000580: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00000590: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-000005a0: 2020 2020 2020 2020 2022 6669 6c65 223a           "file":
-000005b0: 2022 5f70 7269 7661 7465 2f62 7261 6e63   "_private/branc
-000005c0: 682d 6c6f 6164 6572 2f4c 6f63 616c 4272  h-loader/LocalBr
-000005d0: 616e 6368 5374 6f72 6167 6553 6572 7669  anchStorageServi
-000005e0: 6365 222c 0a20 2020 2020 2020 2020 2020  ce",.           
-000005f0: 2020 2020 2022 636c 6173 7322 3a20 224c       "class": "L
-00000600: 6f63 616c 4272 616e 6368 5374 6f72 6167  ocalBranchStorag
-00000610: 6553 6572 7669 6365 220a 2020 2020 2020  eService".      
-00000620: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00000630: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
-00000640: 2020 2020 2020 2022 6669 6c65 223a 2022         "file": "
-00000650: 4469 6167 7261 6d4c 6f6f 6b75 7053 6572  DiagramLookupSer
-00000660: 7669 6365 222c 0a20 2020 2020 2020 2020  vice",.         
-00000670: 2020 2020 2020 2022 636c 6173 7322 3a20         "class": 
-00000680: 2244 6961 6772 616d 4c6f 6f6b 7570 5365  "DiagramLookupSe
-00000690: 7276 6963 6522 2c0a 2020 2020 2020 2020  rvice",.        
-000006a0: 2020 2020 2020 2020 2275 7365 4578 6973          "useExis
-000006b0: 7469 6e67 436c 6173 7322 3a20 2250 7269  tingClass": "Pri
-000006c0: 7661 7465 4469 6167 7261 6d4c 6f6f 6b75  vateDiagramLooku
-000006d0: 7053 6572 7669 6365 220a 2020 2020 2020  pService".      
-000006e0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-000006f0: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
-00000700: 2020 2020 2020 2022 6669 6c65 223a 2022         "file": "
-00000710: 5f70 7269 7661 7465 2f73 6572 7669 6365  _private/service
-00000720: 732f 5072 6976 6174 6544 6961 6772 616d  s/PrivateDiagram
-00000730: 4c6f 6f6b 7570 5365 7276 6963 6522 2c0a  LookupService",.
-00000740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000750: 2263 6c61 7373 223a 2022 5072 6976 6174  "class": "Privat
-00000760: 6544 6961 6772 616d 4c6f 6f6b 7570 5365  eDiagramLookupSe
-00000770: 7276 6963 6522 2c0a 2020 2020 2020 2020  rvice",.        
-00000780: 2020 2020 2020 2020 2270 6572 7369 7374          "persist
-00000790: 656e 7422 3a20 7472 7565 0a20 2020 2020  ent": true.     
-000007a0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-000007b0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-000007c0: 2020 2020 2020 2020 2266 696c 6522 3a20          "file": 
-000007d0: 225f 7072 6976 6174 652f 7365 7276 6963  "_private/servic
-000007e0: 6573 2f50 7269 7661 7465 4469 6167 7261  es/PrivateDiagra
-000007f0: 6d4f 7665 7272 6964 6553 6572 7669 6365  mOverrideService
-00000800: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00000810: 2020 2022 636c 6173 7322 3a20 2250 7269     "class": "Pri
-00000820: 7661 7465 4469 6167 7261 6d4f 7665 7272  vateDiagramOverr
+00000470: 222c 0a20 2020 2020 2020 2022 726f 6f74  ",.        "root
+00000480: 5365 7276 6963 6573 223a 205b 0a20 2020  Services": [.   
+00000490: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+000004a0: 2020 2020 2020 2020 2020 2022 6669 6c65             "file
+000004b0: 223a 2022 5f70 7269 7661 7465 2f73 6572  ": "_private/ser
+000004c0: 7669 6365 732f 5072 6976 6174 6544 6961  vices/PrivateDia
+000004d0: 6772 616d 5475 706c 6553 6572 7669 6365  gramTupleService
+000004e0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000004f0: 2020 2022 636c 6173 7322 3a20 2250 7269     "class": "Pri
+00000500: 7661 7465 4469 6167 7261 6d54 7570 6c65  vateDiagramTuple
+00000510: 5365 7276 6963 6522 0a20 2020 2020 2020  Service".       
+00000520: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00000530: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+00000540: 2020 2020 2020 2266 696c 6522 3a20 225f        "file": "_
+00000550: 7072 6976 6174 652f 6272 616e 6368 2d6c  private/branch-l
+00000560: 6f61 6465 722f 4c6f 6361 6c42 7261 6e63  oader/LocalBranc
+00000570: 6853 746f 7261 6765 5365 7276 6963 6522  hStorageService"
+00000580: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000590: 2020 2263 6c61 7373 223a 2022 4c6f 6361    "class": "Loca
+000005a0: 6c42 7261 6e63 6853 746f 7261 6765 5365  lBranchStorageSe
+000005b0: 7276 6963 6522 0a20 2020 2020 2020 2020  rvice".         
+000005c0: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
+000005d0: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
+000005e0: 2020 2020 2266 696c 6522 3a20 2244 6961      "file": "Dia
+000005f0: 6772 616d 4c6f 6f6b 7570 5365 7276 6963  gramLookupServic
+00000600: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+00000610: 2020 2020 2263 6c61 7373 223a 2022 4469      "class": "Di
+00000620: 6167 7261 6d4c 6f6f 6b75 7053 6572 7669  agramLookupServi
+00000630: 6365 222c 0a20 2020 2020 2020 2020 2020  ce",.           
+00000640: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
+00000650: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00000660: 2020 2266 696c 6522 3a20 225f 7072 6976    "file": "_priv
+00000670: 6174 652f 7365 7276 6963 6573 2f50 7269  ate/services/Pri
+00000680: 7661 7465 4469 6167 7261 6d4c 6f6f 6b75  vateDiagramLooku
+00000690: 7053 6572 7669 6365 222c 0a20 2020 2020  pService",.     
+000006a0: 2020 2020 2020 2020 2020 2022 636c 6173             "clas
+000006b0: 7322 3a20 2250 7269 7661 7465 4469 6167  s": "PrivateDiag
+000006c0: 7261 6d4c 6f6f 6b75 7053 6572 7669 6365  ramLookupService
+000006d0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000006e0: 2020 2022 7065 7273 6973 7465 6e74 223a     "persistent":
+000006f0: 2074 7275 650a 2020 2020 2020 2020 2020   true.          
+00000700: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
+00000710: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00000720: 2020 2022 6669 6c65 223a 2022 5f70 7269     "file": "_pri
+00000730: 7661 7465 2f73 6572 7669 6365 732f 5072  vate/services/Pr
+00000740: 6976 6174 6544 6961 6772 616d 4f76 6572  ivateDiagramOver
+00000750: 7269 6465 5365 7276 6963 6522 2c0a 2020  rideService",.  
+00000760: 2020 2020 2020 2020 2020 2020 2020 2263                "c
+00000770: 6c61 7373 223a 2022 5072 6976 6174 6544  lass": "PrivateD
+00000780: 6961 6772 616d 4f76 6572 7269 6465 5365  iagramOverrideSe
+00000790: 7276 6963 6522 2c0a 2020 2020 2020 2020  rvice",.        
+000007a0: 2020 2020 2020 2020 2270 6572 7369 7374          "persist
+000007b0: 656e 7422 3a20 7472 7565 0a20 2020 2020  ent": true.     
+000007c0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+000007d0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+000007e0: 2020 2020 2020 2020 2266 696c 6522 3a20          "file": 
+000007f0: 2244 6961 6772 616d 4f76 6572 7269 6465  "DiagramOverride
+00000800: 5365 7276 6963 6522 2c0a 2020 2020 2020  Service",.      
+00000810: 2020 2020 2020 2020 2020 2263 6c61 7373            "class
+00000820: 223a 2022 4469 6167 7261 6d4f 7665 7272  ": "DiagramOverr
 00000830: 6964 6553 6572 7669 6365 222c 0a20 2020  ideService",.   
-00000840: 2020 2020 2020 2020 2020 2020 2022 7065               "pe
-00000850: 7273 6973 7465 6e74 223a 2074 7275 650a  rsistent": true.
-00000860: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-00000870: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
-00000880: 2020 2020 2020 2020 2020 2020 2022 6669               "fi
-00000890: 6c65 223a 2022 4469 6167 7261 6d4f 7665  le": "DiagramOve
-000008a0: 7272 6964 6553 6572 7669 6365 222c 0a20  rrideService",. 
-000008b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000008c0: 636c 6173 7322 3a20 2244 6961 6772 616d  class": "Diagram
-000008d0: 4f76 6572 7269 6465 5365 7276 6963 6522  OverrideService"
-000008e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000008f0: 2020 2275 7365 4578 6973 7469 6e67 436c    "useExistingCl
-00000900: 6173 7322 3a20 2250 7269 7661 7465 4469  ass": "PrivateDi
-00000910: 6167 7261 6d4f 7665 7272 6964 6553 6572  agramOverrideSer
-00000920: 7669 6365 220a 2020 2020 2020 2020 2020  vice".          
-00000930: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-00000940: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00000950: 2020 2022 6669 6c65 223a 2022 4469 6167     "file": "Diag
-00000960: 7261 6d43 6f6f 7264 5365 7453 6572 7669  ramCoordSetServi
-00000970: 6365 222c 0a20 2020 2020 2020 2020 2020  ce",.           
-00000980: 2020 2020 2022 636c 6173 7322 3a20 2244       "class": "D
-00000990: 6961 6772 616d 436f 6f72 6453 6574 5365  iagramCoordSetSe
-000009a0: 7276 6963 6522 2c0a 2020 2020 2020 2020  rvice",.        
-000009b0: 2020 2020 2020 2020 2275 7365 4578 6973          "useExis
-000009c0: 7469 6e67 436c 6173 7322 3a20 2250 7269  tingClass": "Pri
-000009d0: 7661 7465 4469 6167 7261 6d43 6f6f 7264  vateDiagramCoord
-000009e0: 5365 7453 6572 7669 6365 220a 2020 2020  SetService".    
-000009f0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00000a00: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-00000a10: 2020 2020 2020 2020 2022 6669 6c65 223a           "file":
-00000a20: 2022 5f70 7269 7661 7465 2f73 6572 7669   "_private/servi
-00000a30: 6365 732f 5072 6976 6174 6544 6961 6772  ces/PrivateDiagr
-00000a40: 616d 436f 6f72 6453 6574 5365 7276 6963  amCoordSetServic
-00000a50: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
-00000a60: 2020 2020 2263 6c61 7373 223a 2022 5072      "class": "Pr
-00000a70: 6976 6174 6544 6961 6772 616d 436f 6f72  ivateDiagramCoor
-00000a80: 6453 6574 5365 7276 6963 6522 2c0a 2020  dSetService",.  
-00000a90: 2020 2020 2020 2020 2020 2020 2020 2270                "p
-00000aa0: 6572 7369 7374 656e 7422 3a20 7472 7565  ersistent": true
-00000ab0: 0a20 2020 2020 2020 2020 2020 207d 2c0a  .            },.
-00000ac0: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
-00000ad0: 2020 2020 2020 2020 2020 2020 2020 2266                "f
-00000ae0: 696c 6522 3a20 225f 7072 6976 6174 652f  ile": "_private/
-00000af0: 6272 616e 6368 2d6c 6f61 6465 722f 4272  branch-loader/Br
-00000b00: 616e 6368 496e 6465 784c 6f61 6465 7253  anchIndexLoaderS
-00000b10: 6572 7669 6365 4122 2c0a 2020 2020 2020  erviceA",.      
-00000b20: 2020 2020 2020 2020 2020 2263 6c61 7373            "class
-00000b30: 223a 2022 4272 616e 6368 496e 6465 784c  ": "BranchIndexL
-00000b40: 6f61 6465 7253 6572 7669 6365 4122 2c0a  oaderServiceA",.
-00000b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b60: 2275 7365 436c 6173 7346 696c 6522 3a20  "useClassFile": 
-00000b70: 225f 7072 6976 6174 652f 6272 616e 6368  "_private/branch
-00000b80: 2d6c 6f61 6465 722f 4272 616e 6368 496e  -loader/BranchIn
-00000b90: 6465 784c 6f61 6465 7253 6572 7669 6365  dexLoaderService
-00000ba0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00000bb0: 2020 2022 7573 6543 6c61 7373 436c 6173     "useClassClas
-00000bc0: 7322 3a20 2242 7261 6e63 6849 6e64 6578  s": "BranchIndex
-00000bd0: 4c6f 6164 6572 5365 7276 6963 6522 2c0a  LoaderService",.
-00000be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000bf0: 2270 6572 7369 7374 656e 7422 3a20 7472  "persistent": tr
-00000c00: 7565 0a20 2020 2020 2020 2020 2020 207d  ue.            }
-00000c10: 2c0a 2020 2020 2020 2020 2020 2020 7b0a  ,.            {.
-00000c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c30: 2266 696c 6522 3a20 225f 7072 6976 6174  "file": "_privat
-00000c40: 652f 6272 616e 6368 2f50 7269 7661 7465  e/branch/Private
-00000c50: 4469 6167 7261 6d42 7261 6e63 6853 6572  DiagramBranchSer
-00000c60: 7669 6365 222c 0a20 2020 2020 2020 2020  vice",.         
-00000c70: 2020 2020 2020 2022 636c 6173 7322 3a20         "class": 
-00000c80: 2250 7269 7661 7465 4469 6167 7261 6d42  "PrivateDiagramB
-00000c90: 7261 6e63 6853 6572 7669 6365 222c 0a20  ranchService",. 
-00000ca0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000cb0: 7065 7273 6973 7465 6e74 223a 2074 7275  persistent": tru
-00000cc0: 650a 2020 2020 2020 2020 2020 2020 7d2c  e.            },
-00000cd0: 0a20 2020 2020 2020 2020 2020 207b 0a20  .            {. 
-00000ce0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000cf0: 6669 6c65 223a 2022 4469 6167 7261 6d42  file": "DiagramB
-00000d00: 7261 6e63 6853 6572 7669 6365 222c 0a20  ranchService",. 
-00000d10: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000d20: 636c 6173 7322 3a20 2244 6961 6772 616d  class": "Diagram
-00000d30: 4272 616e 6368 5365 7276 6963 6522 2c0a  BranchService",.
-00000d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d50: 2275 7365 4578 6973 7469 6e67 436c 6173  "useExistingClas
-00000d60: 7322 3a20 2250 7269 7661 7465 4469 6167  s": "PrivateDiag
-00000d70: 7261 6d42 7261 6e63 6853 6572 7669 6365  ramBranchService
-00000d80: 220a 2020 2020 2020 2020 2020 2020 7d2c  ".            },
-00000d90: 0a20 2020 2020 2020 2020 2020 207b 0a20  .            {. 
-00000da0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000db0: 6669 6c65 223a 2022 5f70 7269 7661 7465  file": "_private
-00000dc0: 2f73 6572 7669 6365 732f 5072 6976 6174  /services/Privat
-00000dd0: 6544 6961 6772 616d 536e 6170 7368 6f74  eDiagramSnapshot
-00000de0: 5365 7276 6963 6522 2c0a 2020 2020 2020  Service",.      
-00000df0: 2020 2020 2020 2020 2020 2263 6c61 7373            "class
-00000e00: 223a 2022 5072 6976 6174 6544 6961 6772  ": "PrivateDiagr
+00000840: 2020 2020 2020 2020 2020 2020 2022 7573               "us
+00000850: 6545 7869 7374 696e 6743 6c61 7373 223a  eExistingClass":
+00000860: 2022 5072 6976 6174 6544 6961 6772 616d   "PrivateDiagram
+00000870: 4f76 6572 7269 6465 5365 7276 6963 6522  OverrideService"
+00000880: 0a20 2020 2020 2020 2020 2020 207d 2c0a  .            },.
+00000890: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
+000008a0: 2020 2020 2020 2020 2020 2020 2020 2266                "f
+000008b0: 696c 6522 3a20 2244 6961 6772 616d 436f  ile": "DiagramCo
+000008c0: 6f72 6453 6574 5365 7276 6963 6522 2c0a  ordSetService",.
+000008d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008e0: 2263 6c61 7373 223a 2022 4469 6167 7261  "class": "Diagra
+000008f0: 6d43 6f6f 7264 5365 7453 6572 7669 6365  mCoordSetService
+00000900: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00000910: 2020 2022 7573 6545 7869 7374 696e 6743     "useExistingC
+00000920: 6c61 7373 223a 2022 5072 6976 6174 6544  lass": "PrivateD
+00000930: 6961 6772 616d 436f 6f72 6453 6574 5365  iagramCoordSetSe
+00000940: 7276 6963 6522 0a20 2020 2020 2020 2020  rvice".         
+00000950: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
+00000960: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
+00000970: 2020 2020 2266 696c 6522 3a20 225f 7072      "file": "_pr
+00000980: 6976 6174 652f 7365 7276 6963 6573 2f50  ivate/services/P
+00000990: 7269 7661 7465 4469 6167 7261 6d43 6f6f  rivateDiagramCoo
+000009a0: 7264 5365 7453 6572 7669 6365 222c 0a20  rdSetService",. 
+000009b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000009c0: 636c 6173 7322 3a20 2250 7269 7661 7465  class": "Private
+000009d0: 4469 6167 7261 6d43 6f6f 7264 5365 7453  DiagramCoordSetS
+000009e0: 6572 7669 6365 222c 0a20 2020 2020 2020  ervice",.       
+000009f0: 2020 2020 2020 2020 2022 7065 7273 6973           "persis
+00000a00: 7465 6e74 223a 2074 7275 650a 2020 2020  tent": true.    
+00000a10: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00000a20: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00000a30: 2020 2020 2020 2020 2022 6669 6c65 223a           "file":
+00000a40: 2022 5f70 7269 7661 7465 2f62 7261 6e63   "_private/branc
+00000a50: 682d 6c6f 6164 6572 2f42 7261 6e63 6849  h-loader/BranchI
+00000a60: 6e64 6578 4c6f 6164 6572 5365 7276 6963  ndexLoaderServic
+00000a70: 6541 222c 0a20 2020 2020 2020 2020 2020  eA",.           
+00000a80: 2020 2020 2022 636c 6173 7322 3a20 2242       "class": "B
+00000a90: 7261 6e63 6849 6e64 6578 4c6f 6164 6572  ranchIndexLoader
+00000aa0: 5365 7276 6963 6541 222c 0a20 2020 2020  ServiceA",.     
+00000ab0: 2020 2020 2020 2020 2020 2022 7573 6543             "useC
+00000ac0: 6c61 7373 4669 6c65 223a 2022 5f70 7269  lassFile": "_pri
+00000ad0: 7661 7465 2f62 7261 6e63 682d 6c6f 6164  vate/branch-load
+00000ae0: 6572 2f42 7261 6e63 6849 6e64 6578 4c6f  er/BranchIndexLo
+00000af0: 6164 6572 5365 7276 6963 6522 2c0a 2020  aderService",.  
+00000b00: 2020 2020 2020 2020 2020 2020 2020 2275                "u
+00000b10: 7365 436c 6173 7343 6c61 7373 223a 2022  seClassClass": "
+00000b20: 4272 616e 6368 496e 6465 784c 6f61 6465  BranchIndexLoade
+00000b30: 7253 6572 7669 6365 222c 0a20 2020 2020  rService",.     
+00000b40: 2020 2020 2020 2020 2020 2022 7065 7273             "pers
+00000b50: 6973 7465 6e74 223a 2074 7275 650a 2020  istent": true.  
+00000b60: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
+00000b70: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+00000b80: 2020 2020 2020 2020 2020 2022 6669 6c65             "file
+00000b90: 223a 2022 5f70 7269 7661 7465 2f62 7261  ": "_private/bra
+00000ba0: 6e63 682f 5072 6976 6174 6544 6961 6772  nch/PrivateDiagr
+00000bb0: 616d 4272 616e 6368 5365 7276 6963 6522  amBranchService"
+00000bc0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000bd0: 2020 2263 6c61 7373 223a 2022 5072 6976    "class": "Priv
+00000be0: 6174 6544 6961 6772 616d 4272 616e 6368  ateDiagramBranch
+00000bf0: 5365 7276 6963 6522 2c0a 2020 2020 2020  Service",.      
+00000c00: 2020 2020 2020 2020 2020 2270 6572 7369            "persi
+00000c10: 7374 656e 7422 3a20 7472 7565 0a20 2020  stent": true.   
+00000c20: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+00000c30: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+00000c40: 2020 2020 2020 2020 2020 2266 696c 6522            "file"
+00000c50: 3a20 2244 6961 6772 616d 4272 616e 6368  : "DiagramBranch
+00000c60: 5365 7276 6963 6522 2c0a 2020 2020 2020  Service",.      
+00000c70: 2020 2020 2020 2020 2020 2263 6c61 7373            "class
+00000c80: 223a 2022 4469 6167 7261 6d42 7261 6e63  ": "DiagramBranc
+00000c90: 6853 6572 7669 6365 222c 0a20 2020 2020  hService",.     
+00000ca0: 2020 2020 2020 2020 2020 2022 7573 6545             "useE
+00000cb0: 7869 7374 696e 6743 6c61 7373 223a 2022  xistingClass": "
+00000cc0: 5072 6976 6174 6544 6961 6772 616d 4272  PrivateDiagramBr
+00000cd0: 616e 6368 5365 7276 6963 6522 0a20 2020  anchService".   
+00000ce0: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+00000cf0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+00000d00: 2020 2020 2020 2020 2020 2266 696c 6522            "file"
+00000d10: 3a20 225f 7072 6976 6174 652f 7365 7276  : "_private/serv
+00000d20: 6963 6573 2f50 7269 7661 7465 4469 6167  ices/PrivateDiag
+00000d30: 7261 6d53 6e61 7073 686f 7453 6572 7669  ramSnapshotServi
+00000d40: 6365 222c 0a20 2020 2020 2020 2020 2020  ce",.           
+00000d50: 2020 2020 2022 636c 6173 7322 3a20 2250       "class": "P
+00000d60: 7269 7661 7465 4469 6167 7261 6d53 6e61  rivateDiagramSna
+00000d70: 7073 686f 7453 6572 7669 6365 222c 0a20  pshotService",. 
+00000d80: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000d90: 7065 7273 6973 7465 6e74 223a 2074 7275  persistent": tru
+00000da0: 650a 2020 2020 2020 2020 2020 2020 7d2c  e.            },
+00000db0: 0a20 2020 2020 2020 2020 2020 207b 0a20  .            {. 
+00000dc0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000dd0: 6669 6c65 223a 2022 4469 6167 7261 6d53  file": "DiagramS
+00000de0: 6e61 7073 686f 7453 6572 7669 6365 222c  napshotService",
+00000df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000e00: 2022 636c 6173 7322 3a20 2244 6961 6772   "class": "Diagr
 00000e10: 616d 536e 6170 7368 6f74 5365 7276 6963  amSnapshotServic
 00000e20: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
-00000e30: 2020 2020 2270 6572 7369 7374 656e 7422      "persistent"
-00000e40: 3a20 7472 7565 0a20 2020 2020 2020 2020  : true.         
-00000e50: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-00000e60: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
-00000e70: 2020 2020 2266 696c 6522 3a20 2244 6961      "file": "Dia
-00000e80: 6772 616d 536e 6170 7368 6f74 5365 7276  gramSnapshotServ
-00000e90: 6963 6522 2c0a 2020 2020 2020 2020 2020  ice",.          
-00000ea0: 2020 2020 2020 2263 6c61 7373 223a 2022        "class": "
-00000eb0: 4469 6167 7261 6d53 6e61 7073 686f 7453  DiagramSnapshotS
-00000ec0: 6572 7669 6365 222c 0a20 2020 2020 2020  ervice",.       
-00000ed0: 2020 2020 2020 2020 2022 7573 6545 7869           "useExi
-00000ee0: 7374 696e 6743 6c61 7373 223a 2022 5072  stingClass": "Pr
-00000ef0: 6976 6174 6544 6961 6772 616d 536e 6170  ivateDiagramSnap
-00000f00: 7368 6f74 5365 7276 6963 6522 0a20 2020  shotService".   
-00000f10: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00000f20: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-00000f30: 2020 2020 2020 2020 2020 2266 696c 6522            "file"
-00000f40: 3a20 225f 7072 6976 6174 652f 7365 7276  : "_private/serv
-00000f50: 6963 6573 2f50 7269 7661 7465 4469 6167  ices/PrivateDiag
-00000f60: 7261 6d43 6f6e 6669 6753 6572 7669 6365  ramConfigService
-00000f70: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00000f80: 2020 2022 636c 6173 7322 3a20 2250 7269     "class": "Pri
-00000f90: 7661 7465 4469 6167 7261 6d43 6f6e 6669  vateDiagramConfi
-00000fa0: 6753 6572 7669 6365 222c 0a20 2020 2020  gService",.     
-00000fb0: 2020 2020 2020 2020 2020 2022 7065 7273             "pers
-00000fc0: 6973 7465 6e74 223a 2074 7275 650a 2020  istent": true.  
-00000fd0: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-00000fe0: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
-00000ff0: 2020 2020 2020 2020 2020 2022 6669 6c65             "file
-00001000: 223a 2022 4469 6167 7261 6d43 6f6e 6669  ": "DiagramConfi
-00001010: 6753 6572 7669 6365 222c 0a20 2020 2020  gService",.     
-00001020: 2020 2020 2020 2020 2020 2022 636c 6173             "clas
-00001030: 7322 3a20 2244 6961 6772 616d 436f 6e66  s": "DiagramConf
-00001040: 6967 5365 7276 6963 6522 2c0a 2020 2020  igService",.    
-00001050: 2020 2020 2020 2020 2020 2020 2275 7365              "use
-00001060: 4578 6973 7469 6e67 436c 6173 7322 3a20  ExistingClass": 
-00001070: 2250 7269 7661 7465 4469 6167 7261 6d43  "PrivateDiagramC
-00001080: 6f6e 6669 6753 6572 7669 6365 220a 2020  onfigService".  
-00001090: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-000010a0: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
-000010b0: 2020 2020 2020 2020 2020 2022 6669 6c65             "file
-000010c0: 223a 2022 5f70 7269 7661 7465 2f67 7269  ": "_private/gri
-000010d0: 642d 6c6f 6164 6572 2f50 7269 7661 7465  d-loader/Private
-000010e0: 4469 6167 7261 6d47 7269 644c 6f61 6465  DiagramGridLoade
-000010f0: 7253 6572 7669 6365 4122 2c0a 2020 2020  rServiceA",.    
-00001100: 2020 2020 2020 2020 2020 2020 2263 6c61              "cla
-00001110: 7373 223a 2022 5072 6976 6174 6544 6961  ss": "PrivateDia
-00001120: 6772 616d 4772 6964 4c6f 6164 6572 5365  gramGridLoaderSe
-00001130: 7276 6963 6541 222c 0a20 2020 2020 2020  rviceA",.       
-00001140: 2020 2020 2020 2020 2022 7573 6543 6c61           "useCla
-00001150: 7373 4669 6c65 223a 2022 5f70 7269 7661  ssFile": "_priva
-00001160: 7465 2f67 7269 642d 6c6f 6164 6572 2f50  te/grid-loader/P
-00001170: 7269 7661 7465 4469 6167 7261 6d47 7269  rivateDiagramGri
-00001180: 644c 6f61 6465 7253 6572 7669 6365 222c  dLoaderService",
-00001190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000011a0: 2022 7573 6543 6c61 7373 436c 6173 7322   "useClassClass"
-000011b0: 3a20 2250 7269 7661 7465 4469 6167 7261  : "PrivateDiagra
-000011c0: 6d47 7269 644c 6f61 6465 7253 6572 7669  mGridLoaderServi
-000011d0: 6365 222c 0a20 2020 2020 2020 2020 2020  ce",.           
-000011e0: 2020 2020 2022 7065 7273 6973 7465 6e74       "persistent
-000011f0: 223a 2074 7275 650a 2020 2020 2020 2020  ": true.        
-00001200: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-00001210: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
-00001220: 2020 2020 2022 6669 6c65 223a 2022 4469       "file": "Di
-00001230: 6167 7261 6d54 6f6f 6c62 6172 5365 7276  agramToolbarServ
-00001240: 6963 6522 2c0a 2020 2020 2020 2020 2020  ice",.          
-00001250: 2020 2020 2020 2263 6c61 7373 223a 2022        "class": "
-00001260: 4469 6167 7261 6d54 6f6f 6c62 6172 5365  DiagramToolbarSe
-00001270: 7276 6963 6522 2c0a 2020 2020 2020 2020  rvice",.        
-00001280: 2020 2020 2020 2020 2275 7365 436c 6173          "useClas
-00001290: 7346 696c 6522 3a20 225f 7072 6976 6174  sFile": "_privat
-000012a0: 652f 7365 7276 6963 6573 2f50 7269 7661  e/services/Priva
-000012b0: 7465 4469 6167 7261 6d54 6f6f 6c62 6172  teDiagramToolbar
-000012c0: 5365 7276 6963 6522 2c0a 2020 2020 2020  Service",.      
-000012d0: 2020 2020 2020 2020 2020 2275 7365 436c            "useCl
-000012e0: 6173 7343 6c61 7373 223a 2022 5072 6976  assClass": "Priv
-000012f0: 6174 6544 6961 6772 616d 546f 6f6c 6261  ateDiagramToolba
-00001300: 7253 6572 7669 6365 222c 0a20 2020 2020  rService",.     
-00001310: 2020 2020 2020 2020 2020 2022 7065 7273             "pers
-00001320: 6973 7465 6e74 223a 2074 7275 650a 2020  istent": true.  
-00001330: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-00001340: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
-00001350: 2020 2020 2020 2020 2020 2022 6669 6c65             "file
-00001360: 223a 2022 7365 7276 6963 6573 2f63 616e  ": "services/can
-00001370: 7661 732e 7365 7276 6963 6522 2c0a 2020  vas.service",.  
-00001380: 2020 2020 2020 2020 2020 2020 2020 2263                "c
-00001390: 6c61 7373 223a 2022 4361 6e76 6173 5365  lass": "CanvasSe
-000013a0: 7276 6963 6522 2c0a 2020 2020 2020 2020  rvice",.        
-000013b0: 2020 2020 2020 2020 226c 6f63 6174 6564          "located
-000013c0: 496e 4170 7044 6972 223a 2074 7275 650a  InAppDir": true.
-000013d0: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-000013e0: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
-000013f0: 2020 2020 2020 2020 2020 2020 2022 6669               "fi
-00001400: 6c65 223a 2022 4469 6167 7261 6d49 7465  le": "DiagramIte
-00001410: 6d53 656c 6563 7453 6572 7669 6365 222c  mSelectService",
-00001420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001430: 2022 636c 6173 7322 3a20 2244 6961 6772   "class": "Diagr
-00001440: 616d 4974 656d 5365 6c65 6374 5365 7276  amItemSelectServ
-00001450: 6963 6522 2c0a 2020 2020 2020 2020 2020  ice",.          
-00001460: 2020 2020 2020 2275 7365 4578 6973 7469        "useExisti
-00001470: 6e67 436c 6173 7322 3a20 2250 7269 7661  ngClass": "Priva
+00000e30: 2020 2020 2275 7365 4578 6973 7469 6e67      "useExisting
+00000e40: 436c 6173 7322 3a20 2250 7269 7661 7465  Class": "Private
+00000e50: 4469 6167 7261 6d53 6e61 7073 686f 7453  DiagramSnapshotS
+00000e60: 6572 7669 6365 220a 2020 2020 2020 2020  ervice".        
+00000e70: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
+00000e80: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
+00000e90: 2020 2020 2022 6669 6c65 223a 2022 5f70       "file": "_p
+00000ea0: 7269 7661 7465 2f73 6572 7669 6365 732f  rivate/services/
+00000eb0: 5072 6976 6174 6544 6961 6772 616d 436f  PrivateDiagramCo
+00000ec0: 6e66 6967 5365 7276 6963 6522 2c0a 2020  nfigService",.  
+00000ed0: 2020 2020 2020 2020 2020 2020 2020 2263                "c
+00000ee0: 6c61 7373 223a 2022 5072 6976 6174 6544  lass": "PrivateD
+00000ef0: 6961 6772 616d 436f 6e66 6967 5365 7276  iagramConfigServ
+00000f00: 6963 6522 2c0a 2020 2020 2020 2020 2020  ice",.          
+00000f10: 2020 2020 2020 2270 6572 7369 7374 656e        "persisten
+00000f20: 7422 3a20 7472 7565 0a20 2020 2020 2020  t": true.       
+00000f30: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00000f40: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+00000f50: 2020 2020 2020 2266 696c 6522 3a20 2244        "file": "D
+00000f60: 6961 6772 616d 436f 6e66 6967 5365 7276  iagramConfigServ
+00000f70: 6963 6522 2c0a 2020 2020 2020 2020 2020  ice",.          
+00000f80: 2020 2020 2020 2263 6c61 7373 223a 2022        "class": "
+00000f90: 4469 6167 7261 6d43 6f6e 6669 6753 6572  DiagramConfigSer
+00000fa0: 7669 6365 222c 0a20 2020 2020 2020 2020  vice",.         
+00000fb0: 2020 2020 2020 2022 7573 6545 7869 7374         "useExist
+00000fc0: 696e 6743 6c61 7373 223a 2022 5072 6976  ingClass": "Priv
+00000fd0: 6174 6544 6961 6772 616d 436f 6e66 6967  ateDiagramConfig
+00000fe0: 5365 7276 6963 6522 0a20 2020 2020 2020  Service".       
+00000ff0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00001000: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+00001010: 2020 2020 2020 2266 696c 6522 3a20 225f        "file": "_
+00001020: 7072 6976 6174 652f 6772 6964 2d6c 6f61  private/grid-loa
+00001030: 6465 722f 5072 6976 6174 6544 6961 6772  der/PrivateDiagr
+00001040: 616d 4772 6964 4c6f 6164 6572 5365 7276  amGridLoaderServ
+00001050: 6963 6541 222c 0a20 2020 2020 2020 2020  iceA",.         
+00001060: 2020 2020 2020 2022 636c 6173 7322 3a20         "class": 
+00001070: 2250 7269 7661 7465 4469 6167 7261 6d47  "PrivateDiagramG
+00001080: 7269 644c 6f61 6465 7253 6572 7669 6365  ridLoaderService
+00001090: 4122 2c0a 2020 2020 2020 2020 2020 2020  A",.            
+000010a0: 2020 2020 2275 7365 436c 6173 7346 696c      "useClassFil
+000010b0: 6522 3a20 225f 7072 6976 6174 652f 6772  e": "_private/gr
+000010c0: 6964 2d6c 6f61 6465 722f 5072 6976 6174  id-loader/Privat
+000010d0: 6544 6961 6772 616d 4772 6964 4c6f 6164  eDiagramGridLoad
+000010e0: 6572 5365 7276 6963 6522 2c0a 2020 2020  erService",.    
+000010f0: 2020 2020 2020 2020 2020 2020 2275 7365              "use
+00001100: 436c 6173 7343 6c61 7373 223a 2022 5072  ClassClass": "Pr
+00001110: 6976 6174 6544 6961 6772 616d 4772 6964  ivateDiagramGrid
+00001120: 4c6f 6164 6572 5365 7276 6963 6522 2c0a  LoaderService",.
+00001130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001140: 2270 6572 7369 7374 656e 7422 3a20 7472  "persistent": tr
+00001150: 7565 0a20 2020 2020 2020 2020 2020 207d  ue.            }
+00001160: 2c0a 2020 2020 2020 2020 2020 2020 7b0a  ,.            {.
+00001170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001180: 2266 696c 6522 3a20 2244 6961 6772 616d  "file": "Diagram
+00001190: 546f 6f6c 6261 7253 6572 7669 6365 222c  ToolbarService",
+000011a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000011b0: 2022 636c 6173 7322 3a20 2244 6961 6772   "class": "Diagr
+000011c0: 616d 546f 6f6c 6261 7253 6572 7669 6365  amToolbarService
+000011d0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000011e0: 2020 2022 7573 6543 6c61 7373 4669 6c65     "useClassFile
+000011f0: 223a 2022 5f70 7269 7661 7465 2f73 6572  ": "_private/ser
+00001200: 7669 6365 732f 5072 6976 6174 6544 6961  vices/PrivateDia
+00001210: 6772 616d 546f 6f6c 6261 7253 6572 7669  gramToolbarServi
+00001220: 6365 222c 0a20 2020 2020 2020 2020 2020  ce",.           
+00001230: 2020 2020 2022 7573 6543 6c61 7373 436c       "useClassCl
+00001240: 6173 7322 3a20 2250 7269 7661 7465 4469  ass": "PrivateDi
+00001250: 6167 7261 6d54 6f6f 6c62 6172 5365 7276  agramToolbarServ
+00001260: 6963 6522 2c0a 2020 2020 2020 2020 2020  ice",.          
+00001270: 2020 2020 2020 2270 6572 7369 7374 656e        "persisten
+00001280: 7422 3a20 7472 7565 0a20 2020 2020 2020  t": true.       
+00001290: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+000012a0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+000012b0: 2020 2020 2020 2266 696c 6522 3a20 2273        "file": "s
+000012c0: 6572 7669 6365 732f 6361 6e76 6173 2e73  ervices/canvas.s
+000012d0: 6572 7669 6365 222c 0a20 2020 2020 2020  ervice",.       
+000012e0: 2020 2020 2020 2020 2022 636c 6173 7322           "class"
+000012f0: 3a20 2243 616e 7661 7353 6572 7669 6365  : "CanvasService
+00001300: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00001310: 2020 2022 6c6f 6361 7465 6449 6e41 7070     "locatedInApp
+00001320: 4469 7222 3a20 7472 7565 0a20 2020 2020  Dir": true.     
+00001330: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00001340: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00001350: 2020 2020 2020 2020 2266 696c 6522 3a20          "file": 
+00001360: 2244 6961 6772 616d 4974 656d 5365 6c65  "DiagramItemSele
+00001370: 6374 5365 7276 6963 6522 2c0a 2020 2020  ctService",.    
+00001380: 2020 2020 2020 2020 2020 2020 2263 6c61              "cla
+00001390: 7373 223a 2022 4469 6167 7261 6d49 7465  ss": "DiagramIte
+000013a0: 6d53 656c 6563 7453 6572 7669 6365 222c  mSelectService",
+000013b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000013c0: 2022 7573 6545 7869 7374 696e 6743 6c61   "useExistingCla
+000013d0: 7373 223a 2022 5072 6976 6174 6544 6961  ss": "PrivateDia
+000013e0: 6772 616d 4974 656d 5365 6c65 6374 5365  gramItemSelectSe
+000013f0: 7276 6963 6522 0a20 2020 2020 2020 2020  rvice".         
+00001400: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
+00001410: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
+00001420: 2020 2020 2266 696c 6522 3a20 225f 7072      "file": "_pr
+00001430: 6976 6174 652f 7365 7276 6963 6573 2f50  ivate/services/P
+00001440: 7269 7661 7465 4469 6167 7261 6d49 7465  rivateDiagramIte
+00001450: 6d53 656c 6563 7453 6572 7669 6365 222c  mSelectService",
+00001460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001470: 2022 636c 6173 7322 3a20 2250 7269 7661   "class": "Priva
 00001480: 7465 4469 6167 7261 6d49 7465 6d53 656c  teDiagramItemSel
-00001490: 6563 7453 6572 7669 6365 220a 2020 2020  ectService".    
-000014a0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-000014b0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-000014c0: 2020 2020 2020 2020 2022 6669 6c65 223a           "file":
-000014d0: 2022 5f70 7269 7661 7465 2f73 6572 7669   "_private/servi
-000014e0: 6365 732f 5072 6976 6174 6544 6961 6772  ces/PrivateDiagr
-000014f0: 616d 4974 656d 5365 6c65 6374 5365 7276  amItemSelectServ
-00001500: 6963 6522 2c0a 2020 2020 2020 2020 2020  ice",.          
-00001510: 2020 2020 2020 2263 6c61 7373 223a 2022        "class": "
-00001520: 5072 6976 6174 6544 6961 6772 616d 4974  PrivateDiagramIt
-00001530: 656d 5365 6c65 6374 5365 7276 6963 6522  emSelectService"
-00001540: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001550: 2020 2270 6572 7369 7374 656e 7422 3a20    "persistent": 
-00001560: 7472 7565 0a20 2020 2020 2020 2020 2020  true.           
-00001570: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-00001580: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00001590: 2020 2266 696c 6522 3a20 225f 7072 6976    "file": "_priv
-000015a0: 6174 652f 6c6f 6361 7469 6f6e 2d6c 6f61  ate/location-loa
-000015b0: 6465 722f 5072 6976 6174 6544 6961 6772  der/PrivateDiagr
-000015c0: 616d 4c6f 6361 7469 6f6e 4c6f 6164 6572  amLocationLoader
-000015d0: 5365 7276 6963 6522 2c0a 2020 2020 2020  Service",.      
-000015e0: 2020 2020 2020 2020 2020 2263 6c61 7373            "class
-000015f0: 223a 2022 5072 6976 6174 6544 6961 6772  ": "PrivateDiagr
-00001600: 616d 4c6f 6361 7469 6f6e 4c6f 6164 6572  amLocationLoader
+00001490: 6563 7453 6572 7669 6365 222c 0a20 2020  ectService",.   
+000014a0: 2020 2020 2020 2020 2020 2020 2022 7065               "pe
+000014b0: 7273 6973 7465 6e74 223a 2074 7275 650a  rsistent": true.
+000014c0: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+000014d0: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
+000014e0: 2020 2020 2020 2020 2020 2020 2022 6669               "fi
+000014f0: 6c65 223a 2022 5f70 7269 7661 7465 2f6c  le": "_private/l
+00001500: 6f63 6174 696f 6e2d 6c6f 6164 6572 2f50  ocation-loader/P
+00001510: 7269 7661 7465 4469 6167 7261 6d4c 6f63  rivateDiagramLoc
+00001520: 6174 696f 6e4c 6f61 6465 7253 6572 7669  ationLoaderServi
+00001530: 6365 222c 0a20 2020 2020 2020 2020 2020  ce",.           
+00001540: 2020 2020 2022 636c 6173 7322 3a20 2250       "class": "P
+00001550: 7269 7661 7465 4469 6167 7261 6d4c 6f63  rivateDiagramLoc
+00001560: 6174 696f 6e4c 6f61 6465 7253 6572 7669  ationLoaderServi
+00001570: 6365 222c 0a20 2020 2020 2020 2020 2020  ce",.           
+00001580: 2020 2020 2022 7065 7273 6973 7465 6e74       "persistent
+00001590: 223a 2074 7275 650a 2020 2020 2020 2020  ": true.        
+000015a0: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
+000015b0: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
+000015c0: 2020 2020 2022 6669 6c65 223a 2022 4469       "file": "Di
+000015d0: 6167 7261 6d50 6f73 6974 696f 6e53 6572  agramPositionSer
+000015e0: 7669 6365 222c 0a20 2020 2020 2020 2020  vice",.         
+000015f0: 2020 2020 2020 2022 636c 6173 7322 3a20         "class": 
+00001600: 2244 6961 6772 616d 506f 7369 7469 6f6e  "DiagramPosition
 00001610: 5365 7276 6963 6522 2c0a 2020 2020 2020  Service",.      
-00001620: 2020 2020 2020 2020 2020 2270 6572 7369            "persi
-00001630: 7374 656e 7422 3a20 7472 7565 0a20 2020  stent": true.   
-00001640: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00001650: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-00001660: 2020 2020 2020 2020 2020 2266 696c 6522            "file"
-00001670: 3a20 2244 6961 6772 616d 506f 7369 7469  : "DiagramPositi
-00001680: 6f6e 5365 7276 6963 6522 2c0a 2020 2020  onService",.    
-00001690: 2020 2020 2020 2020 2020 2020 2263 6c61              "cla
-000016a0: 7373 223a 2022 4469 6167 7261 6d50 6f73  ss": "DiagramPos
-000016b0: 6974 696f 6e53 6572 7669 6365 222c 0a20  itionService",. 
-000016c0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000016d0: 7573 6545 7869 7374 696e 6743 6c61 7373  useExistingClass
-000016e0: 223a 2022 5072 6976 6174 6544 6961 6772  ": "PrivateDiagr
-000016f0: 616d 506f 7369 7469 6f6e 5365 7276 6963  amPositionServic
-00001700: 6522 0a20 2020 2020 2020 2020 2020 207d  e".            }
-00001710: 2c0a 2020 2020 2020 2020 2020 2020 7b0a  ,.            {.
-00001720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001730: 2266 696c 6522 3a20 225f 7072 6976 6174  "file": "_privat
-00001740: 652f 7365 7276 6963 6573 2f50 7269 7661  e/services/Priva
-00001750: 7465 4469 6167 7261 6d50 6f73 6974 696f  teDiagramPositio
-00001760: 6e53 6572 7669 6365 222c 0a20 2020 2020  nService",.     
-00001770: 2020 2020 2020 2020 2020 2022 636c 6173             "clas
-00001780: 7322 3a20 2250 7269 7661 7465 4469 6167  s": "PrivateDiag
-00001790: 7261 6d50 6f73 6974 696f 6e53 6572 7669  ramPositionServi
-000017a0: 6365 222c 0a20 2020 2020 2020 2020 2020  ce",.           
-000017b0: 2020 2020 2022 7065 7273 6973 7465 6e74       "persistent
-000017c0: 223a 2074 7275 650a 2020 2020 2020 2020  ": true.        
-000017d0: 2020 2020 7d0a 2020 2020 2020 2020 5d0a      }.        ].
-000017e0: 2020 2020 7d2c 0a20 2020 2022 6167 656e      },.    "agen
-000017f0: 7422 3a20 7b7d 2c0a 2020 2020 226f 6666  t": {},.    "off
-00001800: 6963 6522 3a20 7b0a 2020 2020 2020 2020  ice": {.        
-00001810: 2273 7562 7072 6f63 6573 7347 726f 7570  "subprocessGroup
-00001820: 223a 2022 6c69 7665 6462 2b64 6961 6772  ": "livedb+diagr
-00001830: 616d 222c 0a20 2020 2020 2020 2022 7368  am",.        "sh
-00001840: 6f77 486f 6d65 4c69 6e6b 223a 2066 616c  owHomeLink": fal
-00001850: 7365 2c0a 2020 2020 2020 2020 2261 7070  se,.        "app
-00001860: 4469 7222 3a20 225f 7072 6976 6174 652f  Dir": "_private/
-00001870: 626f 7468 2d61 7070 222c 0a20 2020 2020  both-app",.     
-00001880: 2020 2022 6173 7365 7444 6972 223a 2022     "assetDir": "
-00001890: 5f70 7269 7661 7465 2f62 6f74 682d 6173  _private/both-as
-000018a0: 7365 7473 222c 0a20 2020 2020 2020 2022  sets",.        "
-000018b0: 6d6f 6475 6c65 4469 7222 3a20 2270 6c75  moduleDir": "plu
-000018c0: 6769 6e2d 6d6f 6475 6c65 222c 0a20 2020  gin-module",.   
-000018d0: 2020 2020 2022 726f 6f74 5365 7276 6963       "rootServic
-000018e0: 6573 223a 205b 0a20 2020 2020 2020 2020  es": [.         
-000018f0: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
-00001900: 2020 2020 2022 6669 6c65 223a 2022 5f70       "file": "_p
-00001910: 7269 7661 7465 2f62 7261 6e63 682d 6c6f  rivate/branch-lo
-00001920: 6164 6572 2f4c 6f63 616c 4272 616e 6368  ader/LocalBranch
-00001930: 5374 6f72 6167 6553 6572 7669 6365 222c  StorageService",
-00001940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001950: 2022 636c 6173 7322 3a20 224c 6f63 616c   "class": "Local
-00001960: 4272 616e 6368 5374 6f72 6167 6553 6572  BranchStorageSer
-00001970: 7669 6365 220a 2020 2020 2020 2020 2020  vice".          
-00001980: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-00001990: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-000019a0: 2020 2022 6669 6c65 223a 2022 5f70 7269     "file": "_pri
-000019b0: 7661 7465 2f73 6572 7669 6365 732f 5072  vate/services/Pr
-000019c0: 6976 6174 6544 6961 6772 616d 5475 706c  ivateDiagramTupl
-000019d0: 6553 6572 7669 6365 222c 0a20 2020 2020  eService",.     
-000019e0: 2020 2020 2020 2020 2020 2022 636c 6173             "clas
-000019f0: 7322 3a20 2250 7269 7661 7465 4469 6167  s": "PrivateDiag
-00001a00: 7261 6d54 7570 6c65 5365 7276 6963 6522  ramTupleService"
-00001a10: 0a20 2020 2020 2020 2020 2020 207d 2c0a  .            },.
-00001a20: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
-00001a30: 2020 2020 2020 2020 2020 2020 2020 2266                "f
-00001a40: 696c 6522 3a20 2244 6961 6772 616d 4c6f  ile": "DiagramLo
-00001a50: 6f6b 7570 5365 7276 6963 6522 2c0a 2020  okupService",.  
-00001a60: 2020 2020 2020 2020 2020 2020 2020 2263                "c
-00001a70: 6c61 7373 223a 2022 4469 6167 7261 6d4c  lass": "DiagramL
-00001a80: 6f6f 6b75 7053 6572 7669 6365 222c 0a20  ookupService",. 
-00001a90: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00001aa0: 7573 6545 7869 7374 696e 6743 6c61 7373  useExistingClass
-00001ab0: 223a 2022 5072 6976 6174 6544 6961 6772  ": "PrivateDiagr
-00001ac0: 616d 4c6f 6f6b 7570 5365 7276 6963 6522  amLookupService"
-00001ad0: 0a20 2020 2020 2020 2020 2020 207d 2c0a  .            },.
-00001ae0: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
-00001af0: 2020 2020 2020 2020 2020 2020 2020 2266                "f
-00001b00: 696c 6522 3a20 225f 7072 6976 6174 652f  ile": "_private/
-00001b10: 7365 7276 6963 6573 2f50 7269 7661 7465  services/Private
-00001b20: 4469 6167 7261 6d4c 6f6f 6b75 7053 6572  DiagramLookupSer
-00001b30: 7669 6365 222c 0a20 2020 2020 2020 2020  vice",.         
-00001b40: 2020 2020 2020 2022 636c 6173 7322 3a20         "class": 
-00001b50: 2250 7269 7661 7465 4469 6167 7261 6d4c  "PrivateDiagramL
-00001b60: 6f6f 6b75 7053 6572 7669 6365 222c 0a20  ookupService",. 
-00001b70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00001b80: 7065 7273 6973 7465 6e74 223a 2074 7275  persistent": tru
-00001b90: 650a 2020 2020 2020 2020 2020 2020 7d2c  e.            },
-00001ba0: 0a20 2020 2020 2020 2020 2020 207b 0a20  .            {. 
-00001bb0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00001bc0: 6669 6c65 223a 2022 5f70 7269 7661 7465  file": "_private
-00001bd0: 2f73 6572 7669 6365 732f 5072 6976 6174  /services/Privat
-00001be0: 6544 6961 6772 616d 4f76 6572 7269 6465  eDiagramOverride
-00001bf0: 5365 7276 6963 6522 2c0a 2020 2020 2020  Service",.      
-00001c00: 2020 2020 2020 2020 2020 2263 6c61 7373            "class
-00001c10: 223a 2022 5072 6976 6174 6544 6961 6772  ": "PrivateDiagr
-00001c20: 616d 4f76 6572 7269 6465 5365 7276 6963  amOverrideServic
-00001c30: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
-00001c40: 2020 2020 2270 6572 7369 7374 656e 7422      "persistent"
-00001c50: 3a20 7472 7565 0a20 2020 2020 2020 2020  : true.         
-00001c60: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-00001c70: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
-00001c80: 2020 2020 2266 696c 6522 3a20 2244 6961      "file": "Dia
-00001c90: 6772 616d 4f76 6572 7269 6465 5365 7276  gramOverrideServ
-00001ca0: 6963 6522 2c0a 2020 2020 2020 2020 2020  ice",.          
-00001cb0: 2020 2020 2020 2263 6c61 7373 223a 2022        "class": "
-00001cc0: 4469 6167 7261 6d4f 7665 7272 6964 6553  DiagramOverrideS
-00001cd0: 6572 7669 6365 222c 0a20 2020 2020 2020  ervice",.       
-00001ce0: 2020 2020 2020 2020 2022 7573 6545 7869           "useExi
-00001cf0: 7374 696e 6743 6c61 7373 223a 2022 5072  stingClass": "Pr
-00001d00: 6976 6174 6544 6961 6772 616d 4f76 6572  ivateDiagramOver
-00001d10: 7269 6465 5365 7276 6963 6522 0a20 2020  rideService".   
-00001d20: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00001d30: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-00001d40: 2020 2020 2020 2020 2020 2266 696c 6522            "file"
-00001d50: 3a20 2244 6961 6772 616d 436f 6f72 6453  : "DiagramCoordS
-00001d60: 6574 5365 7276 6963 6522 2c0a 2020 2020  etService",.    
-00001d70: 2020 2020 2020 2020 2020 2020 2263 6c61              "cla
-00001d80: 7373 223a 2022 4469 6167 7261 6d43 6f6f  ss": "DiagramCoo
-00001d90: 7264 5365 7453 6572 7669 6365 222c 0a20  rdSetService",. 
-00001da0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00001db0: 7573 6545 7869 7374 696e 6743 6c61 7373  useExistingClass
-00001dc0: 223a 2022 5072 6976 6174 6544 6961 6772  ": "PrivateDiagr
-00001dd0: 616d 436f 6f72 6453 6574 5365 7276 6963  amCoordSetServic
-00001de0: 6522 0a20 2020 2020 2020 2020 2020 207d  e".            }
-00001df0: 2c0a 2020 2020 2020 2020 2020 2020 7b0a  ,.            {.
-00001e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e10: 2266 696c 6522 3a20 225f 7072 6976 6174  "file": "_privat
-00001e20: 652f 7365 7276 6963 6573 2f50 7269 7661  e/services/Priva
-00001e30: 7465 4469 6167 7261 6d43 6f6f 7264 5365  teDiagramCoordSe
-00001e40: 7453 6572 7669 6365 222c 0a20 2020 2020  tService",.     
-00001e50: 2020 2020 2020 2020 2020 2022 636c 6173             "clas
-00001e60: 7322 3a20 2250 7269 7661 7465 4469 6167  s": "PrivateDiag
-00001e70: 7261 6d43 6f6f 7264 5365 7453 6572 7669  ramCoordSetServi
-00001e80: 6365 222c 0a20 2020 2020 2020 2020 2020  ce",.           
-00001e90: 2020 2020 2022 7065 7273 6973 7465 6e74       "persistent
-00001ea0: 223a 2074 7275 650a 2020 2020 2020 2020  ": true.        
-00001eb0: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-00001ec0: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
-00001ed0: 2020 2020 2022 6669 6c65 223a 2022 5f70       "file": "_p
-00001ee0: 7269 7661 7465 2f62 7261 6e63 682d 6c6f  rivate/branch-lo
-00001ef0: 6164 6572 2f42 7261 6e63 6849 6e64 6578  ader/BranchIndex
-00001f00: 4c6f 6164 6572 5365 7276 6963 6541 222c  LoaderServiceA",
-00001f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001f20: 2022 636c 6173 7322 3a20 2242 7261 6e63   "class": "Branc
-00001f30: 6849 6e64 6578 4c6f 6164 6572 5365 7276  hIndexLoaderServ
-00001f40: 6963 6541 222c 0a20 2020 2020 2020 2020  iceA",.         
-00001f50: 2020 2020 2020 2022 7573 6543 6c61 7373         "useClass
-00001f60: 4669 6c65 223a 2022 5f70 7269 7661 7465  File": "_private
-00001f70: 2f62 7261 6e63 682d 6c6f 6164 6572 2f42  /branch-loader/B
-00001f80: 7261 6e63 6849 6e64 6578 4c6f 6164 6572  ranchIndexLoader
-00001f90: 5365 7276 6963 6522 2c0a 2020 2020 2020  Service",.      
-00001fa0: 2020 2020 2020 2020 2020 2275 7365 436c            "useCl
-00001fb0: 6173 7343 6c61 7373 223a 2022 4272 616e  assClass": "Bran
-00001fc0: 6368 496e 6465 784c 6f61 6465 7253 6572  chIndexLoaderSer
-00001fd0: 7669 6365 222c 0a20 2020 2020 2020 2020  vice",.         
-00001fe0: 2020 2020 2020 2022 7065 7273 6973 7465         "persiste
-00001ff0: 6e74 223a 2074 7275 650a 2020 2020 2020  nt": true.      
-00002000: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00002010: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
-00002020: 2020 2020 2020 2022 6669 6c65 223a 2022         "file": "
-00002030: 5f70 7269 7661 7465 2f62 7261 6e63 682f  _private/branch/
-00002040: 5072 6976 6174 6544 6961 6772 616d 4272  PrivateDiagramBr
-00002050: 616e 6368 5365 7276 6963 6522 2c0a 2020  anchService",.  
-00002060: 2020 2020 2020 2020 2020 2020 2020 2263                "c
-00002070: 6c61 7373 223a 2022 5072 6976 6174 6544  lass": "PrivateD
-00002080: 6961 6772 616d 4272 616e 6368 5365 7276  iagramBranchServ
-00002090: 6963 6522 2c0a 2020 2020 2020 2020 2020  ice",.          
-000020a0: 2020 2020 2020 2270 6572 7369 7374 656e        "persisten
-000020b0: 7422 3a20 7472 7565 0a20 2020 2020 2020  t": true.       
-000020c0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-000020d0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-000020e0: 2020 2020 2020 2266 696c 6522 3a20 2244        "file": "D
-000020f0: 6961 6772 616d 4272 616e 6368 5365 7276  iagramBranchServ
-00002100: 6963 6522 2c0a 2020 2020 2020 2020 2020  ice",.          
-00002110: 2020 2020 2020 2263 6c61 7373 223a 2022        "class": "
-00002120: 4469 6167 7261 6d42 7261 6e63 6853 6572  DiagramBranchSer
-00002130: 7669 6365 222c 0a20 2020 2020 2020 2020  vice",.         
-00002140: 2020 2020 2020 2022 7573 6545 7869 7374         "useExist
-00002150: 696e 6743 6c61 7373 223a 2022 5072 6976  ingClass": "Priv
-00002160: 6174 6544 6961 6772 616d 4272 616e 6368  ateDiagramBranch
-00002170: 5365 7276 6963 6522 0a20 2020 2020 2020  Service".       
-00002180: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-00002190: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-000021a0: 2020 2020 2020 2266 696c 6522 3a20 225f        "file": "_
-000021b0: 7072 6976 6174 652f 7365 7276 6963 6573  private/services
-000021c0: 2f50 7269 7661 7465 4469 6167 7261 6d53  /PrivateDiagramS
-000021d0: 6e61 7073 686f 7453 6572 7669 6365 222c  napshotService",
-000021e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000021f0: 2022 636c 6173 7322 3a20 2250 7269 7661   "class": "Priva
-00002200: 7465 4469 6167 7261 6d53 6e61 7073 686f  teDiagramSnapsho
-00002210: 7453 6572 7669 6365 222c 0a20 2020 2020  tService",.     
-00002220: 2020 2020 2020 2020 2020 2022 7065 7273             "pers
-00002230: 6973 7465 6e74 223a 2074 7275 650a 2020  istent": true.  
-00002240: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-00002250: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
-00002260: 2020 2020 2020 2020 2020 2022 6669 6c65             "file
-00002270: 223a 2022 4469 6167 7261 6d53 6e61 7073  ": "DiagramSnaps
-00002280: 686f 7453 6572 7669 6365 222c 0a20 2020  hotService",.   
-00002290: 2020 2020 2020 2020 2020 2020 2022 636c               "cl
-000022a0: 6173 7322 3a20 2244 6961 6772 616d 536e  ass": "DiagramSn
-000022b0: 6170 7368 6f74 5365 7276 6963 6522 2c0a  apshotService",.
-000022c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022d0: 2275 7365 4578 6973 7469 6e67 436c 6173  "useExistingClas
-000022e0: 7322 3a20 2250 7269 7661 7465 4469 6167  s": "PrivateDiag
-000022f0: 7261 6d53 6e61 7073 686f 7453 6572 7669  ramSnapshotServi
-00002300: 6365 220a 2020 2020 2020 2020 2020 2020  ce".            
-00002310: 7d2c 0a20 2020 2020 2020 2020 2020 207b  },.            {
-00002320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002330: 2022 6669 6c65 223a 2022 5f70 7269 7661   "file": "_priva
-00002340: 7465 2f73 6572 7669 6365 732f 5072 6976  te/services/Priv
-00002350: 6174 6544 6961 6772 616d 436f 6e66 6967  ateDiagramConfig
-00002360: 5365 7276 6963 6522 2c0a 2020 2020 2020  Service",.      
-00002370: 2020 2020 2020 2020 2020 2263 6c61 7373            "class
-00002380: 223a 2022 5072 6976 6174 6544 6961 6772  ": "PrivateDiagr
-00002390: 616d 436f 6e66 6967 5365 7276 6963 6522  amConfigService"
-000023a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000023b0: 2020 2270 6572 7369 7374 656e 7422 3a20    "persistent": 
-000023c0: 7472 7565 0a20 2020 2020 2020 2020 2020  true.           
-000023d0: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-000023e0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-000023f0: 2020 2266 696c 6522 3a20 2244 6961 6772    "file": "Diagr
-00002400: 616d 436f 6e66 6967 5365 7276 6963 6522  amConfigService"
-00002410: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002420: 2020 2263 6c61 7373 223a 2022 4469 6167    "class": "Diag
-00002430: 7261 6d43 6f6e 6669 6753 6572 7669 6365  ramConfigService
-00002440: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00002450: 2020 2022 7573 6545 7869 7374 696e 6743     "useExistingC
-00002460: 6c61 7373 223a 2022 5072 6976 6174 6544  lass": "PrivateD
-00002470: 6961 6772 616d 436f 6e66 6967 5365 7276  iagramConfigServ
-00002480: 6963 6522 0a20 2020 2020 2020 2020 2020  ice".           
-00002490: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-000024a0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-000024b0: 2020 2266 696c 6522 3a20 225f 7072 6976    "file": "_priv
-000024c0: 6174 652f 6772 6964 2d6c 6f61 6465 722f  ate/grid-loader/
-000024d0: 5072 6976 6174 6544 6961 6772 616d 4772  PrivateDiagramGr
-000024e0: 6964 4c6f 6164 6572 5365 7276 6963 6541  idLoaderServiceA
-000024f0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00002500: 2020 2022 636c 6173 7322 3a20 2250 7269     "class": "Pri
-00002510: 7661 7465 4469 6167 7261 6d47 7269 644c  vateDiagramGridL
-00002520: 6f61 6465 7253 6572 7669 6365 4122 2c0a  oaderServiceA",.
-00002530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002540: 2275 7365 436c 6173 7346 696c 6522 3a20  "useClassFile": 
-00002550: 225f 7072 6976 6174 652f 6772 6964 2d6c  "_private/grid-l
-00002560: 6f61 6465 722f 5072 6976 6174 6544 6961  oader/PrivateDia
-00002570: 6772 616d 4772 6964 4c6f 6164 6572 5365  gramGridLoaderSe
+00001620: 2020 2020 2020 2020 2020 2275 7365 4578            "useEx
+00001630: 6973 7469 6e67 436c 6173 7322 3a20 2250  istingClass": "P
+00001640: 7269 7661 7465 4469 6167 7261 6d50 6f73  rivateDiagramPos
+00001650: 6974 696f 6e53 6572 7669 6365 220a 2020  itionService".  
+00001660: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
+00001670: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+00001680: 2020 2020 2020 2020 2020 2022 6669 6c65             "file
+00001690: 223a 2022 5f70 7269 7661 7465 2f73 6572  ": "_private/ser
+000016a0: 7669 6365 732f 5072 6976 6174 6544 6961  vices/PrivateDia
+000016b0: 6772 616d 506f 7369 7469 6f6e 5365 7276  gramPositionServ
+000016c0: 6963 6522 2c0a 2020 2020 2020 2020 2020  ice",.          
+000016d0: 2020 2020 2020 2263 6c61 7373 223a 2022        "class": "
+000016e0: 5072 6976 6174 6544 6961 6772 616d 506f  PrivateDiagramPo
+000016f0: 7369 7469 6f6e 5365 7276 6963 6522 2c0a  sitionService",.
+00001700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001710: 2270 6572 7369 7374 656e 7422 3a20 7472  "persistent": tr
+00001720: 7565 0a20 2020 2020 2020 2020 2020 207d  ue.            }
+00001730: 0a20 2020 2020 2020 205d 0a20 2020 207d  .        ].    }
+00001740: 2c0a 2020 2020 2261 6765 6e74 223a 207b  ,.    "agent": {
+00001750: 7d2c 0a20 2020 2022 6f66 6669 6365 223a  },.    "office":
+00001760: 207b 0a20 2020 2020 2020 2022 7375 6270   {.        "subp
+00001770: 726f 6365 7373 4772 6f75 7022 3a20 226c  rocessGroup": "l
+00001780: 6976 6564 622b 6469 6167 7261 6d22 2c0a  ivedb+diagram",.
+00001790: 2020 2020 2020 2020 2273 686f 7748 6f6d          "showHom
+000017a0: 654c 696e 6b22 3a20 6661 6c73 652c 0a20  eLink": false,. 
+000017b0: 2020 2020 2020 2022 6170 7044 6972 223a         "appDir":
+000017c0: 2022 5f70 7269 7661 7465 2f62 6f74 682d   "_private/both-
+000017d0: 6170 7022 2c0a 2020 2020 2020 2020 2261  app",.        "a
+000017e0: 7373 6574 4469 7222 3a20 225f 7072 6976  ssetDir": "_priv
+000017f0: 6174 652f 626f 7468 2d61 7373 6574 7322  ate/both-assets"
+00001800: 2c0a 2020 2020 2020 2020 226d 6f64 756c  ,.        "modul
+00001810: 6544 6972 223a 2022 706c 7567 696e 2d6d  eDir": "plugin-m
+00001820: 6f64 756c 6522 2c0a 2020 2020 2020 2020  odule",.        
+00001830: 2272 6f6f 7453 6572 7669 6365 7322 3a20  "rootServices": 
+00001840: 5b0a 2020 2020 2020 2020 2020 2020 7b0a  [.            {.
+00001850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001860: 2266 696c 6522 3a20 225f 7072 6976 6174  "file": "_privat
+00001870: 652f 6272 616e 6368 2d6c 6f61 6465 722f  e/branch-loader/
+00001880: 4c6f 6361 6c42 7261 6e63 6853 746f 7261  LocalBranchStora
+00001890: 6765 5365 7276 6963 6522 2c0a 2020 2020  geService",.    
+000018a0: 2020 2020 2020 2020 2020 2020 2263 6c61              "cla
+000018b0: 7373 223a 2022 4c6f 6361 6c42 7261 6e63  ss": "LocalBranc
+000018c0: 6853 746f 7261 6765 5365 7276 6963 6522  hStorageService"
+000018d0: 0a20 2020 2020 2020 2020 2020 207d 2c0a  .            },.
+000018e0: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
+000018f0: 2020 2020 2020 2020 2020 2020 2020 2266                "f
+00001900: 696c 6522 3a20 225f 7072 6976 6174 652f  ile": "_private/
+00001910: 7365 7276 6963 6573 2f50 7269 7661 7465  services/Private
+00001920: 4469 6167 7261 6d54 7570 6c65 5365 7276  DiagramTupleServ
+00001930: 6963 6522 2c0a 2020 2020 2020 2020 2020  ice",.          
+00001940: 2020 2020 2020 2263 6c61 7373 223a 2022        "class": "
+00001950: 5072 6976 6174 6544 6961 6772 616d 5475  PrivateDiagramTu
+00001960: 706c 6553 6572 7669 6365 220a 2020 2020  pleService".    
+00001970: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00001980: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00001990: 2020 2020 2020 2020 2022 6669 6c65 223a           "file":
+000019a0: 2022 4469 6167 7261 6d4c 6f6f 6b75 7053   "DiagramLookupS
+000019b0: 6572 7669 6365 222c 0a20 2020 2020 2020  ervice",.       
+000019c0: 2020 2020 2020 2020 2022 636c 6173 7322           "class"
+000019d0: 3a20 2244 6961 6772 616d 4c6f 6f6b 7570  : "DiagramLookup
+000019e0: 5365 7276 6963 6522 2c0a 2020 2020 2020  Service",.      
+000019f0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00001a00: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00001a10: 2020 2020 2020 2022 6669 6c65 223a 2022         "file": "
+00001a20: 5f70 7269 7661 7465 2f73 6572 7669 6365  _private/service
+00001a30: 732f 5072 6976 6174 6544 6961 6772 616d  s/PrivateDiagram
+00001a40: 4c6f 6f6b 7570 5365 7276 6963 6522 2c0a  LookupService",.
+00001a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a60: 2263 6c61 7373 223a 2022 5072 6976 6174  "class": "Privat
+00001a70: 6544 6961 6772 616d 4c6f 6f6b 7570 5365  eDiagramLookupSe
+00001a80: 7276 6963 6522 2c0a 2020 2020 2020 2020  rvice",.        
+00001a90: 2020 2020 2020 2020 2270 6572 7369 7374          "persist
+00001aa0: 656e 7422 3a20 7472 7565 0a20 2020 2020  ent": true.     
+00001ab0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00001ac0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00001ad0: 2020 2020 2020 2020 2266 696c 6522 3a20          "file": 
+00001ae0: 225f 7072 6976 6174 652f 7365 7276 6963  "_private/servic
+00001af0: 6573 2f50 7269 7661 7465 4469 6167 7261  es/PrivateDiagra
+00001b00: 6d4f 7665 7272 6964 6553 6572 7669 6365  mOverrideService
+00001b10: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00001b20: 2020 2022 636c 6173 7322 3a20 2250 7269     "class": "Pri
+00001b30: 7661 7465 4469 6167 7261 6d4f 7665 7272  vateDiagramOverr
+00001b40: 6964 6553 6572 7669 6365 222c 0a20 2020  ideService",.   
+00001b50: 2020 2020 2020 2020 2020 2020 2022 7065               "pe
+00001b60: 7273 6973 7465 6e74 223a 2074 7275 650a  rsistent": true.
+00001b70: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+00001b80: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
+00001b90: 2020 2020 2020 2020 2020 2020 2022 6669               "fi
+00001ba0: 6c65 223a 2022 4469 6167 7261 6d4f 7665  le": "DiagramOve
+00001bb0: 7272 6964 6553 6572 7669 6365 222c 0a20  rrideService",. 
+00001bc0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001bd0: 636c 6173 7322 3a20 2244 6961 6772 616d  class": "Diagram
+00001be0: 4f76 6572 7269 6465 5365 7276 6963 6522  OverrideService"
+00001bf0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001c00: 2020 2275 7365 4578 6973 7469 6e67 436c    "useExistingCl
+00001c10: 6173 7322 3a20 2250 7269 7661 7465 4469  ass": "PrivateDi
+00001c20: 6167 7261 6d4f 7665 7272 6964 6553 6572  agramOverrideSer
+00001c30: 7669 6365 220a 2020 2020 2020 2020 2020  vice".          
+00001c40: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
+00001c50: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00001c60: 2020 2022 6669 6c65 223a 2022 4469 6167     "file": "Diag
+00001c70: 7261 6d43 6f6f 7264 5365 7453 6572 7669  ramCoordSetServi
+00001c80: 6365 222c 0a20 2020 2020 2020 2020 2020  ce",.           
+00001c90: 2020 2020 2022 636c 6173 7322 3a20 2244       "class": "D
+00001ca0: 6961 6772 616d 436f 6f72 6453 6574 5365  iagramCoordSetSe
+00001cb0: 7276 6963 6522 2c0a 2020 2020 2020 2020  rvice",.        
+00001cc0: 2020 2020 2020 2020 2275 7365 4578 6973          "useExis
+00001cd0: 7469 6e67 436c 6173 7322 3a20 2250 7269  tingClass": "Pri
+00001ce0: 7661 7465 4469 6167 7261 6d43 6f6f 7264  vateDiagramCoord
+00001cf0: 5365 7453 6572 7669 6365 220a 2020 2020  SetService".    
+00001d00: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00001d10: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00001d20: 2020 2020 2020 2020 2022 6669 6c65 223a           "file":
+00001d30: 2022 5f70 7269 7661 7465 2f73 6572 7669   "_private/servi
+00001d40: 6365 732f 5072 6976 6174 6544 6961 6772  ces/PrivateDiagr
+00001d50: 616d 436f 6f72 6453 6574 5365 7276 6963  amCoordSetServic
+00001d60: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+00001d70: 2020 2020 2263 6c61 7373 223a 2022 5072      "class": "Pr
+00001d80: 6976 6174 6544 6961 6772 616d 436f 6f72  ivateDiagramCoor
+00001d90: 6453 6574 5365 7276 6963 6522 2c0a 2020  dSetService",.  
+00001da0: 2020 2020 2020 2020 2020 2020 2020 2270                "p
+00001db0: 6572 7369 7374 656e 7422 3a20 7472 7565  ersistent": true
+00001dc0: 0a20 2020 2020 2020 2020 2020 207d 2c0a  .            },.
+00001dd0: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
+00001de0: 2020 2020 2020 2020 2020 2020 2020 2266                "f
+00001df0: 696c 6522 3a20 225f 7072 6976 6174 652f  ile": "_private/
+00001e00: 6272 616e 6368 2d6c 6f61 6465 722f 4272  branch-loader/Br
+00001e10: 616e 6368 496e 6465 784c 6f61 6465 7253  anchIndexLoaderS
+00001e20: 6572 7669 6365 4122 2c0a 2020 2020 2020  erviceA",.      
+00001e30: 2020 2020 2020 2020 2020 2263 6c61 7373            "class
+00001e40: 223a 2022 4272 616e 6368 496e 6465 784c  ": "BranchIndexL
+00001e50: 6f61 6465 7253 6572 7669 6365 4122 2c0a  oaderServiceA",.
+00001e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e70: 2275 7365 436c 6173 7346 696c 6522 3a20  "useClassFile": 
+00001e80: 225f 7072 6976 6174 652f 6272 616e 6368  "_private/branch
+00001e90: 2d6c 6f61 6465 722f 4272 616e 6368 496e  -loader/BranchIn
+00001ea0: 6465 784c 6f61 6465 7253 6572 7669 6365  dexLoaderService
+00001eb0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00001ec0: 2020 2022 7573 6543 6c61 7373 436c 6173     "useClassClas
+00001ed0: 7322 3a20 2242 7261 6e63 6849 6e64 6578  s": "BranchIndex
+00001ee0: 4c6f 6164 6572 5365 7276 6963 6522 2c0a  LoaderService",.
+00001ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f00: 2270 6572 7369 7374 656e 7422 3a20 7472  "persistent": tr
+00001f10: 7565 0a20 2020 2020 2020 2020 2020 207d  ue.            }
+00001f20: 2c0a 2020 2020 2020 2020 2020 2020 7b0a  ,.            {.
+00001f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f40: 2266 696c 6522 3a20 225f 7072 6976 6174  "file": "_privat
+00001f50: 652f 6272 616e 6368 2f50 7269 7661 7465  e/branch/Private
+00001f60: 4469 6167 7261 6d42 7261 6e63 6853 6572  DiagramBranchSer
+00001f70: 7669 6365 222c 0a20 2020 2020 2020 2020  vice",.         
+00001f80: 2020 2020 2020 2022 636c 6173 7322 3a20         "class": 
+00001f90: 2250 7269 7661 7465 4469 6167 7261 6d42  "PrivateDiagramB
+00001fa0: 7261 6e63 6853 6572 7669 6365 222c 0a20  ranchService",. 
+00001fb0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001fc0: 7065 7273 6973 7465 6e74 223a 2074 7275  persistent": tru
+00001fd0: 650a 2020 2020 2020 2020 2020 2020 7d2c  e.            },
+00001fe0: 0a20 2020 2020 2020 2020 2020 207b 0a20  .            {. 
+00001ff0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00002000: 6669 6c65 223a 2022 4469 6167 7261 6d42  file": "DiagramB
+00002010: 7261 6e63 6853 6572 7669 6365 222c 0a20  ranchService",. 
+00002020: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00002030: 636c 6173 7322 3a20 2244 6961 6772 616d  class": "Diagram
+00002040: 4272 616e 6368 5365 7276 6963 6522 2c0a  BranchService",.
+00002050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002060: 2275 7365 4578 6973 7469 6e67 436c 6173  "useExistingClas
+00002070: 7322 3a20 2250 7269 7661 7465 4469 6167  s": "PrivateDiag
+00002080: 7261 6d42 7261 6e63 6853 6572 7669 6365  ramBranchService
+00002090: 220a 2020 2020 2020 2020 2020 2020 7d2c  ".            },
+000020a0: 0a20 2020 2020 2020 2020 2020 207b 0a20  .            {. 
+000020b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000020c0: 6669 6c65 223a 2022 5f70 7269 7661 7465  file": "_private
+000020d0: 2f73 6572 7669 6365 732f 5072 6976 6174  /services/Privat
+000020e0: 6544 6961 6772 616d 536e 6170 7368 6f74  eDiagramSnapshot
+000020f0: 5365 7276 6963 6522 2c0a 2020 2020 2020  Service",.      
+00002100: 2020 2020 2020 2020 2020 2263 6c61 7373            "class
+00002110: 223a 2022 5072 6976 6174 6544 6961 6772  ": "PrivateDiagr
+00002120: 616d 536e 6170 7368 6f74 5365 7276 6963  amSnapshotServic
+00002130: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+00002140: 2020 2020 2270 6572 7369 7374 656e 7422      "persistent"
+00002150: 3a20 7472 7565 0a20 2020 2020 2020 2020  : true.         
+00002160: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
+00002170: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
+00002180: 2020 2020 2266 696c 6522 3a20 2244 6961      "file": "Dia
+00002190: 6772 616d 536e 6170 7368 6f74 5365 7276  gramSnapshotServ
+000021a0: 6963 6522 2c0a 2020 2020 2020 2020 2020  ice",.          
+000021b0: 2020 2020 2020 2263 6c61 7373 223a 2022        "class": "
+000021c0: 4469 6167 7261 6d53 6e61 7073 686f 7453  DiagramSnapshotS
+000021d0: 6572 7669 6365 222c 0a20 2020 2020 2020  ervice",.       
+000021e0: 2020 2020 2020 2020 2022 7573 6545 7869           "useExi
+000021f0: 7374 696e 6743 6c61 7373 223a 2022 5072  stingClass": "Pr
+00002200: 6976 6174 6544 6961 6772 616d 536e 6170  ivateDiagramSnap
+00002210: 7368 6f74 5365 7276 6963 6522 0a20 2020  shotService".   
+00002220: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+00002230: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+00002240: 2020 2020 2020 2020 2020 2266 696c 6522            "file"
+00002250: 3a20 225f 7072 6976 6174 652f 7365 7276  : "_private/serv
+00002260: 6963 6573 2f50 7269 7661 7465 4469 6167  ices/PrivateDiag
+00002270: 7261 6d43 6f6e 6669 6753 6572 7669 6365  ramConfigService
+00002280: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00002290: 2020 2022 636c 6173 7322 3a20 2250 7269     "class": "Pri
+000022a0: 7661 7465 4469 6167 7261 6d43 6f6e 6669  vateDiagramConfi
+000022b0: 6753 6572 7669 6365 222c 0a20 2020 2020  gService",.     
+000022c0: 2020 2020 2020 2020 2020 2022 7065 7273             "pers
+000022d0: 6973 7465 6e74 223a 2074 7275 650a 2020  istent": true.  
+000022e0: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
+000022f0: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+00002300: 2020 2020 2020 2020 2020 2022 6669 6c65             "file
+00002310: 223a 2022 4469 6167 7261 6d43 6f6e 6669  ": "DiagramConfi
+00002320: 6753 6572 7669 6365 222c 0a20 2020 2020  gService",.     
+00002330: 2020 2020 2020 2020 2020 2022 636c 6173             "clas
+00002340: 7322 3a20 2244 6961 6772 616d 436f 6e66  s": "DiagramConf
+00002350: 6967 5365 7276 6963 6522 2c0a 2020 2020  igService",.    
+00002360: 2020 2020 2020 2020 2020 2020 2275 7365              "use
+00002370: 4578 6973 7469 6e67 436c 6173 7322 3a20  ExistingClass": 
+00002380: 2250 7269 7661 7465 4469 6167 7261 6d43  "PrivateDiagramC
+00002390: 6f6e 6669 6753 6572 7669 6365 220a 2020  onfigService".  
+000023a0: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
+000023b0: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+000023c0: 2020 2020 2020 2020 2020 2022 6669 6c65             "file
+000023d0: 223a 2022 5f70 7269 7661 7465 2f67 7269  ": "_private/gri
+000023e0: 642d 6c6f 6164 6572 2f50 7269 7661 7465  d-loader/Private
+000023f0: 4469 6167 7261 6d47 7269 644c 6f61 6465  DiagramGridLoade
+00002400: 7253 6572 7669 6365 4122 2c0a 2020 2020  rServiceA",.    
+00002410: 2020 2020 2020 2020 2020 2020 2263 6c61              "cla
+00002420: 7373 223a 2022 5072 6976 6174 6544 6961  ss": "PrivateDia
+00002430: 6772 616d 4772 6964 4c6f 6164 6572 5365  gramGridLoaderSe
+00002440: 7276 6963 6541 222c 0a20 2020 2020 2020  rviceA",.       
+00002450: 2020 2020 2020 2020 2022 7573 6543 6c61           "useCla
+00002460: 7373 4669 6c65 223a 2022 5f70 7269 7661  ssFile": "_priva
+00002470: 7465 2f67 7269 642d 6c6f 6164 6572 2f50  te/grid-loader/P
+00002480: 7269 7661 7465 4469 6167 7261 6d47 7269  rivateDiagramGri
+00002490: 644c 6f61 6465 7253 6572 7669 6365 222c  dLoaderService",
+000024a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000024b0: 2022 7573 6543 6c61 7373 436c 6173 7322   "useClassClass"
+000024c0: 3a20 2250 7269 7661 7465 4469 6167 7261  : "PrivateDiagra
+000024d0: 6d47 7269 644c 6f61 6465 7253 6572 7669  mGridLoaderServi
+000024e0: 6365 222c 0a20 2020 2020 2020 2020 2020  ce",.           
+000024f0: 2020 2020 2022 7065 7273 6973 7465 6e74       "persistent
+00002500: 223a 2074 7275 650a 2020 2020 2020 2020  ": true.        
+00002510: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
+00002520: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
+00002530: 2020 2020 2022 6669 6c65 223a 2022 4469       "file": "Di
+00002540: 6167 7261 6d54 6f6f 6c62 6172 5365 7276  agramToolbarServ
+00002550: 6963 6522 2c0a 2020 2020 2020 2020 2020  ice",.          
+00002560: 2020 2020 2020 2263 6c61 7373 223a 2022        "class": "
+00002570: 4469 6167 7261 6d54 6f6f 6c62 6172 5365  DiagramToolbarSe
 00002580: 7276 6963 6522 2c0a 2020 2020 2020 2020  rvice",.        
 00002590: 2020 2020 2020 2020 2275 7365 436c 6173          "useClas
-000025a0: 7343 6c61 7373 223a 2022 5072 6976 6174  sClass": "Privat
-000025b0: 6544 6961 6772 616d 4772 6964 4c6f 6164  eDiagramGridLoad
-000025c0: 6572 5365 7276 6963 6522 2c0a 2020 2020  erService",.    
-000025d0: 2020 2020 2020 2020 2020 2020 2270 6572              "per
-000025e0: 7369 7374 656e 7422 3a20 7472 7565 0a20  sistent": true. 
-000025f0: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
-00002600: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
-00002610: 2020 2020 2020 2020 2020 2020 2266 696c              "fil
-00002620: 6522 3a20 2244 6961 6772 616d 546f 6f6c  e": "DiagramTool
-00002630: 6261 7253 6572 7669 6365 222c 0a20 2020  barService",.   
-00002640: 2020 2020 2020 2020 2020 2020 2022 636c               "cl
-00002650: 6173 7322 3a20 2244 6961 6772 616d 546f  ass": "DiagramTo
-00002660: 6f6c 6261 7253 6572 7669 6365 222c 0a20  olbarService",. 
-00002670: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00002680: 7573 6543 6c61 7373 4669 6c65 223a 2022  useClassFile": "
-00002690: 5f70 7269 7661 7465 2f73 6572 7669 6365  _private/service
-000026a0: 732f 5072 6976 6174 6544 6961 6772 616d  s/PrivateDiagram
-000026b0: 546f 6f6c 6261 7253 6572 7669 6365 222c  ToolbarService",
-000026c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000026d0: 2022 7573 6543 6c61 7373 436c 6173 7322   "useClassClass"
-000026e0: 3a20 2250 7269 7661 7465 4469 6167 7261  : "PrivateDiagra
-000026f0: 6d54 6f6f 6c62 6172 5365 7276 6963 6522  mToolbarService"
-00002700: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002710: 2020 2270 6572 7369 7374 656e 7422 3a20    "persistent": 
-00002720: 7472 7565 0a20 2020 2020 2020 2020 2020  true.           
-00002730: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-00002740: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00002750: 2020 2266 696c 6522 3a20 2273 6572 7669    "file": "servi
-00002760: 6365 732f 6361 6e76 6173 2e73 6572 7669  ces/canvas.servi
-00002770: 6365 222c 0a20 2020 2020 2020 2020 2020  ce",.           
-00002780: 2020 2020 2022 636c 6173 7322 3a20 2243       "class": "C
-00002790: 616e 7661 7353 6572 7669 6365 222c 0a20  anvasService",. 
-000027a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000027b0: 6c6f 6361 7465 6449 6e41 7070 4469 7222  locatedInAppDir"
-000027c0: 3a20 7472 7565 0a20 2020 2020 2020 2020  : true.         
-000027d0: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-000027e0: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
-000027f0: 2020 2020 2266 696c 6522 3a20 2244 6961      "file": "Dia
-00002800: 6772 616d 4974 656d 5365 6c65 6374 5365  gramItemSelectSe
-00002810: 7276 6963 6522 2c0a 2020 2020 2020 2020  rvice",.        
-00002820: 2020 2020 2020 2020 2263 6c61 7373 223a          "class":
-00002830: 2022 4469 6167 7261 6d49 7465 6d53 656c   "DiagramItemSel
-00002840: 6563 7453 6572 7669 6365 222c 0a20 2020  ectService",.   
-00002850: 2020 2020 2020 2020 2020 2020 2022 7573               "us
-00002860: 6545 7869 7374 696e 6743 6c61 7373 223a  eExistingClass":
-00002870: 2022 5072 6976 6174 6544 6961 6772 616d   "PrivateDiagram
-00002880: 4974 656d 5365 6c65 6374 5365 7276 6963  ItemSelectServic
-00002890: 6522 0a20 2020 2020 2020 2020 2020 207d  e".            }
-000028a0: 2c0a 2020 2020 2020 2020 2020 2020 7b0a  ,.            {.
-000028b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028c0: 2266 696c 6522 3a20 225f 7072 6976 6174  "file": "_privat
-000028d0: 652f 7365 7276 6963 6573 2f50 7269 7661  e/services/Priva
-000028e0: 7465 4469 6167 7261 6d49 7465 6d53 656c  teDiagramItemSel
-000028f0: 6563 7453 6572 7669 6365 222c 0a20 2020  ectService",.   
-00002900: 2020 2020 2020 2020 2020 2020 2022 636c               "cl
-00002910: 6173 7322 3a20 2250 7269 7661 7465 4469  ass": "PrivateDi
-00002920: 6167 7261 6d49 7465 6d53 656c 6563 7453  agramItemSelectS
-00002930: 6572 7669 6365 222c 0a20 2020 2020 2020  ervice",.       
-00002940: 2020 2020 2020 2020 2022 7065 7273 6973           "persis
-00002950: 7465 6e74 223a 2074 7275 650a 2020 2020  tent": true.    
-00002960: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00002970: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-00002980: 2020 2020 2020 2020 2022 6669 6c65 223a           "file":
-00002990: 2022 5f70 7269 7661 7465 2f6c 6f63 6174   "_private/locat
-000029a0: 696f 6e2d 6c6f 6164 6572 2f50 7269 7661  ion-loader/Priva
-000029b0: 7465 4469 6167 7261 6d4c 6f63 6174 696f  teDiagramLocatio
-000029c0: 6e4c 6f61 6465 7253 6572 7669 6365 222c  nLoaderService",
-000029d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000029e0: 2022 636c 6173 7322 3a20 2250 7269 7661   "class": "Priva
-000029f0: 7465 4469 6167 7261 6d4c 6f63 6174 696f  teDiagramLocatio
-00002a00: 6e4c 6f61 6465 7253 6572 7669 6365 222c  nLoaderService",
-00002a10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002a20: 2022 7065 7273 6973 7465 6e74 223a 2074   "persistent": t
-00002a30: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
-00002a40: 7d2c 0a20 2020 2020 2020 2020 2020 207b  },.            {
-00002a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002a60: 2022 6669 6c65 223a 2022 4469 6167 7261   "file": "Diagra
-00002a70: 6d50 6f73 6974 696f 6e53 6572 7669 6365  mPositionService
-00002a80: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00002a90: 2020 2022 636c 6173 7322 3a20 2244 6961     "class": "Dia
-00002aa0: 6772 616d 506f 7369 7469 6f6e 5365 7276  gramPositionServ
-00002ab0: 6963 6522 2c0a 2020 2020 2020 2020 2020  ice",.          
-00002ac0: 2020 2020 2020 2275 7365 4578 6973 7469        "useExisti
-00002ad0: 6e67 436c 6173 7322 3a20 2250 7269 7661  ngClass": "Priva
-00002ae0: 7465 4469 6167 7261 6d50 6f73 6974 696f  teDiagramPositio
-00002af0: 6e53 6572 7669 6365 220a 2020 2020 2020  nService".      
-00002b00: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00002b10: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
-00002b20: 2020 2020 2020 2022 6669 6c65 223a 2022         "file": "
-00002b30: 5f70 7269 7661 7465 2f73 6572 7669 6365  _private/service
-00002b40: 732f 5072 6976 6174 6544 6961 6772 616d  s/PrivateDiagram
-00002b50: 506f 7369 7469 6f6e 5365 7276 6963 6522  PositionService"
-00002b60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002b70: 2020 2263 6c61 7373 223a 2022 5072 6976    "class": "Priv
-00002b80: 6174 6544 6961 6772 616d 506f 7369 7469  ateDiagramPositi
-00002b90: 6f6e 5365 7276 6963 6522 2c0a 2020 2020  onService",.    
-00002ba0: 2020 2020 2020 2020 2020 2020 2270 6572              "per
-00002bb0: 7369 7374 656e 7422 3a20 7472 7565 0a20  sistent": true. 
-00002bc0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-00002bd0: 2020 2020 205d 0a20 2020 207d 0a7d 0a         ].    }.}.
+000025a0: 7346 696c 6522 3a20 225f 7072 6976 6174  sFile": "_privat
+000025b0: 652f 7365 7276 6963 6573 2f50 7269 7661  e/services/Priva
+000025c0: 7465 4469 6167 7261 6d54 6f6f 6c62 6172  teDiagramToolbar
+000025d0: 5365 7276 6963 6522 2c0a 2020 2020 2020  Service",.      
+000025e0: 2020 2020 2020 2020 2020 2275 7365 436c            "useCl
+000025f0: 6173 7343 6c61 7373 223a 2022 5072 6976  assClass": "Priv
+00002600: 6174 6544 6961 6772 616d 546f 6f6c 6261  ateDiagramToolba
+00002610: 7253 6572 7669 6365 222c 0a20 2020 2020  rService",.     
+00002620: 2020 2020 2020 2020 2020 2022 7065 7273             "pers
+00002630: 6973 7465 6e74 223a 2074 7275 650a 2020  istent": true.  
+00002640: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
+00002650: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+00002660: 2020 2020 2020 2020 2020 2022 6669 6c65             "file
+00002670: 223a 2022 7365 7276 6963 6573 2f63 616e  ": "services/can
+00002680: 7661 732e 7365 7276 6963 6522 2c0a 2020  vas.service",.  
+00002690: 2020 2020 2020 2020 2020 2020 2020 2263                "c
+000026a0: 6c61 7373 223a 2022 4361 6e76 6173 5365  lass": "CanvasSe
+000026b0: 7276 6963 6522 2c0a 2020 2020 2020 2020  rvice",.        
+000026c0: 2020 2020 2020 2020 226c 6f63 6174 6564          "located
+000026d0: 496e 4170 7044 6972 223a 2074 7275 650a  InAppDir": true.
+000026e0: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+000026f0: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
+00002700: 2020 2020 2020 2020 2020 2020 2022 6669               "fi
+00002710: 6c65 223a 2022 4469 6167 7261 6d49 7465  le": "DiagramIte
+00002720: 6d53 656c 6563 7453 6572 7669 6365 222c  mSelectService",
+00002730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002740: 2022 636c 6173 7322 3a20 2244 6961 6772   "class": "Diagr
+00002750: 616d 4974 656d 5365 6c65 6374 5365 7276  amItemSelectServ
+00002760: 6963 6522 2c0a 2020 2020 2020 2020 2020  ice",.          
+00002770: 2020 2020 2020 2275 7365 4578 6973 7469        "useExisti
+00002780: 6e67 436c 6173 7322 3a20 2250 7269 7661  ngClass": "Priva
+00002790: 7465 4469 6167 7261 6d49 7465 6d53 656c  teDiagramItemSel
+000027a0: 6563 7453 6572 7669 6365 220a 2020 2020  ectService".    
+000027b0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+000027c0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+000027d0: 2020 2020 2020 2020 2022 6669 6c65 223a           "file":
+000027e0: 2022 5f70 7269 7661 7465 2f73 6572 7669   "_private/servi
+000027f0: 6365 732f 5072 6976 6174 6544 6961 6772  ces/PrivateDiagr
+00002800: 616d 4974 656d 5365 6c65 6374 5365 7276  amItemSelectServ
+00002810: 6963 6522 2c0a 2020 2020 2020 2020 2020  ice",.          
+00002820: 2020 2020 2020 2263 6c61 7373 223a 2022        "class": "
+00002830: 5072 6976 6174 6544 6961 6772 616d 4974  PrivateDiagramIt
+00002840: 656d 5365 6c65 6374 5365 7276 6963 6522  emSelectService"
+00002850: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00002860: 2020 2270 6572 7369 7374 656e 7422 3a20    "persistent": 
+00002870: 7472 7565 0a20 2020 2020 2020 2020 2020  true.           
+00002880: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
+00002890: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+000028a0: 2020 2266 696c 6522 3a20 225f 7072 6976    "file": "_priv
+000028b0: 6174 652f 6c6f 6361 7469 6f6e 2d6c 6f61  ate/location-loa
+000028c0: 6465 722f 5072 6976 6174 6544 6961 6772  der/PrivateDiagr
+000028d0: 616d 4c6f 6361 7469 6f6e 4c6f 6164 6572  amLocationLoader
+000028e0: 5365 7276 6963 6522 2c0a 2020 2020 2020  Service",.      
+000028f0: 2020 2020 2020 2020 2020 2263 6c61 7373            "class
+00002900: 223a 2022 5072 6976 6174 6544 6961 6772  ": "PrivateDiagr
+00002910: 616d 4c6f 6361 7469 6f6e 4c6f 6164 6572  amLocationLoader
+00002920: 5365 7276 6963 6522 2c0a 2020 2020 2020  Service",.      
+00002930: 2020 2020 2020 2020 2020 2270 6572 7369            "persi
+00002940: 7374 656e 7422 3a20 7472 7565 0a20 2020  stent": true.   
+00002950: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+00002960: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+00002970: 2020 2020 2020 2020 2020 2266 696c 6522            "file"
+00002980: 3a20 2244 6961 6772 616d 506f 7369 7469  : "DiagramPositi
+00002990: 6f6e 5365 7276 6963 6522 2c0a 2020 2020  onService",.    
+000029a0: 2020 2020 2020 2020 2020 2020 2263 6c61              "cla
+000029b0: 7373 223a 2022 4469 6167 7261 6d50 6f73  ss": "DiagramPos
+000029c0: 6974 696f 6e53 6572 7669 6365 222c 0a20  itionService",. 
+000029d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000029e0: 7573 6545 7869 7374 696e 6743 6c61 7373  useExistingClass
+000029f0: 223a 2022 5072 6976 6174 6544 6961 6772  ": "PrivateDiagr
+00002a00: 616d 506f 7369 7469 6f6e 5365 7276 6963  amPositionServic
+00002a10: 6522 0a20 2020 2020 2020 2020 2020 207d  e".            }
+00002a20: 2c0a 2020 2020 2020 2020 2020 2020 7b0a  ,.            {.
+00002a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a40: 2266 696c 6522 3a20 225f 7072 6976 6174  "file": "_privat
+00002a50: 652f 7365 7276 6963 6573 2f50 7269 7661  e/services/Priva
+00002a60: 7465 4469 6167 7261 6d50 6f73 6974 696f  teDiagramPositio
+00002a70: 6e53 6572 7669 6365 222c 0a20 2020 2020  nService",.     
+00002a80: 2020 2020 2020 2020 2020 2022 636c 6173             "clas
+00002a90: 7322 3a20 2250 7269 7661 7465 4469 6167  s": "PrivateDiag
+00002aa0: 7261 6d50 6f73 6974 696f 6e53 6572 7669  ramPositionServi
+00002ab0: 6365 222c 0a20 2020 2020 2020 2020 2020  ce",.           
+00002ac0: 2020 2020 2022 7065 7273 6973 7465 6e74       "persistent
+00002ad0: 223a 2074 7275 650a 2020 2020 2020 2020  ": true.        
+00002ae0: 2020 2020 7d0a 2020 2020 2020 2020 5d0a      }.        ].
+00002af0: 2020 2020 7d0a 7d0a                          }.}.
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/server/DiagramApiABC.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/server/DiagramApiABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/server/DiagramImportApiABC.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/server/DiagramImportApiABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/server/DiagramViewerApiABC.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/server/DiagramViewerApiABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/ImportGroupHashTuple.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/ImportGroupHashTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/__init__.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,7 +24,11 @@
     from .shapes import loadShapeTuples
 
     loadShapeTuples()
 
     from .model import loadModelTuples
 
     loadModelTuples()
+
+    from .grids import loadGridTuples
+
+    loadGridTuples()
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/branches/ImportBranchDeltaColorOverride.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/branches/ImportBranchDeltaColorOverride.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/branches/ImportBranchTuple.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/branches/ImportBranchTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/lookups/ImportDispColorTuple.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/lookups/ImportDispColorTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/lookups/ImportDispLayerTuple.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/lookups/ImportDispLayerTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/lookups/ImportDispLevelTuple.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/lookups/ImportDispLevelTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/lookups/ImportDispLineStyleTuple.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/lookups/ImportDispLineStyleTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/lookups/ImportDispTextStyleTuple.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/lookups/ImportDispTextStyleTuple.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,7 +34,9 @@
     spacingBetweenTexts: float = TupleField(defaultValue=100)
 
     borderWidth: Optional[float] = TupleField()
 
     showForEdit: bool = TupleField(defaultValue=False)
 
     blockApiUpdate: bool = TupleField(defaultValue=False)
+
+    wrapTextAtChars: int = TupleField(defaultValue=None)
```

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/model/ImportLiveDbDispLinkTuple.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/model/ImportLiveDbDispLinkTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/shapes/ImportDispCurvedTextTuple.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/shapes/ImportDispCurvedTextTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/shapes/ImportDispEdgeTemplateTuple.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/shapes/ImportDispEdgeTemplateTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/shapes/ImportDispEllipseTuple.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/shapes/ImportDispEllipseTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/shapes/ImportDispGroupPtrTuple.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/shapes/ImportDispGroupPtrTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/shapes/ImportDispGroupTuple.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/shapes/ImportDispGroupTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/shapes/ImportDispPolygonTuple.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/shapes/ImportDispPolygonTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/shapes/ImportDispPolylineTuple.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/shapes/ImportDispPolylineTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/tuples/shapes/ImportDispTextTuple.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/tuples/shapes/ImportDispTextTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram/worker/WorkerApi.py` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram/worker/WorkerApi.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-3.3.3/peek_plugin_diagram.egg-info/SOURCES.txt` & `peek-plugin-diagram-3.4.0/peek_plugin_diagram.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 peek_plugin_diagram/_private/admin-app/status/status.component.ts
 peek_plugin_diagram/_private/admin-app/tuples/DiagramImporterStatusTuple.ts
 peek_plugin_diagram/_private/agent/AgentEntryHook.py
 peek_plugin_diagram/_private/agent/__init__.py
 peek_plugin_diagram/_private/alembic/__init__.py
 peek_plugin_diagram/_private/alembic/env.py
 peek_plugin_diagram/_private/alembic/script.py.mako
+peek_plugin_diagram/_private/alembic/versions/0ad02369aaea_use_darkcolor_lightcolor.py
 peek_plugin_diagram/_private/alembic/versions/0db3aedfee95_added_column_showforedit.py
 peek_plugin_diagram/_private/alembic/versions/128b23798db0_add_text_border_for_curved_text.py
 peek_plugin_diagram/_private/alembic/versions/1856b7fb8803_added_linetemplatesenabled.py
 peek_plugin_diagram/_private/alembic/versions/1b17ef0cca17_removed_string_field_sizes.py
 peek_plugin_diagram/_private/alembic/versions/1fe753e1f369_disptext_textstyleid_not_null.py
 peek_plugin_diagram/_private/alembic/versions/2127d894e46b_moved_smallest_sizes_to_grids.py
 peek_plugin_diagram/_private/alembic/versions/23117803d414_added_location_index.py
@@ -42,26 +43,28 @@
 peek_plugin_diagram/_private/alembic/versions/473d5f6a97e8_removed_more_string_sizes.py
 peek_plugin_diagram/_private/alembic/versions/47879bec4c5f_added_texthstretch.py
 peek_plugin_diagram/_private/alembic/versions/4925c894757b_enabled_nulls_for_text.py
 peek_plugin_diagram/_private/alembic/versions/4b943b584307_added_coordset_mx_c.py
 peek_plugin_diagram/_private/alembic/versions/4f6ed1047562_added_branch_fields_to_dispbase.py
 peek_plugin_diagram/_private/alembic/versions/5307eb21c742_added_spacingbetweentexts_in_textstyle.py
 peek_plugin_diagram/_private/alembic/versions/558bc7fc4d36_added_polyline_startkey_endkey.py
+peek_plugin_diagram/_private/alembic/versions/57e88ad9d5cb_add_dispbase_key_index.py
 peek_plugin_diagram/_private/alembic/versions/5e2f84d757f2_added_cascade_constraints.py
 peek_plugin_diagram/_private/alembic/versions/6a71c73c0606_added_polygon_isrectangle.py
 peek_plugin_diagram/_private/alembic/versions/6a97dd344aed_added_coordset_gridsizes.py
 peek_plugin_diagram/_private/alembic/versions/6d3a96cf1955_added_dispnull.py
 peek_plugin_diagram/_private/alembic/versions/6f545d4166dc_remove_unique_constraint_for_dispgroup.py
 peek_plugin_diagram/_private/alembic/versions/7eed363f5df5_initial.py
 peek_plugin_diagram/_private/alembic/versions/81c1d2809046_added_coordset_editable_fields.py
 peek_plugin_diagram/_private/alembic/versions/8b8ebbe5ec7b_added_scalable_to_lookup_linestyle.py
 peek_plugin_diagram/_private/alembic/versions/8ef78f862ac8_updates_for_dispgroup.py
 peek_plugin_diagram/_private/alembic/versions/97990b4ca6a1_added_landingcoordsetid.py
 peek_plugin_diagram/_private/alembic/versions/9e7ca1acd6be_fixed_importhash_indexes_for_lookups.py
 peek_plugin_diagram/_private/alembic/versions/__init__.py
+peek_plugin_diagram/_private/alembic/versions/a151fd42572b_added_wrap_text_at_chars.py
 peek_plugin_diagram/_private/alembic/versions/a4c59bcaaf88_added_curved_text_disp.py
 peek_plugin_diagram/_private/alembic/versions/a66e033b8227_updated_float_precision_in_zoom_levels.py
 peek_plugin_diagram/_private/alembic/versions/a73574690197_coordset_positiononzoom.py
 peek_plugin_diagram/_private/alembic/versions/a86e0317e22a_added_poly_template_name.py
 peek_plugin_diagram/_private/alembic/versions/aa76b059b81e_added_default_group_ptr_to_coord_set.py
 peek_plugin_diagram/_private/alembic/versions/bf8f559c4df9_removed_branchgridindex.py
 peek_plugin_diagram/_private/alembic/versions/bfdd4f46e293_added_coordset_key.py
@@ -140,14 +143,15 @@
 peek_plugin_diagram/_private/both-app/canvas-render/PeekDispRenderDrawModeE.web.ts
 peek_plugin_diagram/_private/both-app/canvas-render/PeekDispRenderFactory.web.ts
 peek_plugin_diagram/_private/both-app/canvas-shapes/DispBase.ts
 peek_plugin_diagram/_private/both-app/canvas-shapes/DispCurvedText.ts
 peek_plugin_diagram/_private/both-app/canvas-shapes/DispEdgeTemplate.ts
 peek_plugin_diagram/_private/both-app/canvas-shapes/DispEllipse.ts
 peek_plugin_diagram/_private/both-app/canvas-shapes/DispFactory.ts
+peek_plugin_diagram/_private/both-app/canvas-shapes/DispFactoryTypeMap.ts
 peek_plugin_diagram/_private/both-app/canvas-shapes/DispGroup.ts
 peek_plugin_diagram/_private/both-app/canvas-shapes/DispGroupPointer.ts
 peek_plugin_diagram/_private/both-app/canvas-shapes/DispNull.ts
 peek_plugin_diagram/_private/both-app/canvas-shapes/DispPoly.ts
 peek_plugin_diagram/_private/both-app/canvas-shapes/DispPolygon.ts
 peek_plugin_diagram/_private/both-app/canvas-shapes/DispPolyline.ts
 peek_plugin_diagram/_private/both-app/canvas-shapes/DispRectangle.ts
@@ -193,17 +197,14 @@
 peek_plugin_diagram/_private/both-app/view-select-layers-component/select-layers.component.web.html
 peek_plugin_diagram/_private/both-app/view-select-layers-component/select-layers.component.web.scss
 peek_plugin_diagram/_private/both-app/view-select-layers-component/select-layers.component.web.ts
 peek_plugin_diagram/_private/both-app/view-toolbar-component/toolbar.component.web.html
 peek_plugin_diagram/_private/both-app/view-toolbar-component/toolbar.component.web.scss
 peek_plugin_diagram/_private/both-app/view-toolbar-component/toolbar.component.web.ts
 peek_plugin_diagram/_private/both-assets/icon.png
-peek_plugin_diagram/_private/both-cfg/diagram-cfg.component.ts
-peek_plugin_diagram/_private/both-cfg/diagram-cfg.component.web.html
-peek_plugin_diagram/_private/both-cfg/diagram-cfg.module.ts
 peek_plugin_diagram/_private/client/ClientEntryHook.py
 peek_plugin_diagram/_private/client/TupleDataObservable.py
 peek_plugin_diagram/_private/client/__init__.py
 peek_plugin_diagram/_private/client/controller/BranchIndexCacheController.py
 peek_plugin_diagram/_private/client/controller/CoordSetCacheController.py
 peek_plugin_diagram/_private/client/controller/GridCacheController.py
 peek_plugin_diagram/_private/client/controller/LocationIndexCacheController.py
@@ -262,14 +263,15 @@
 peek_plugin_diagram/_private/server/tuple_providers/__init__.py
 peek_plugin_diagram/_private/storage/DeclarativeBase.py
 peek_plugin_diagram/_private/storage/DispIndex.py
 peek_plugin_diagram/_private/storage/Display.py
 peek_plugin_diagram/_private/storage/GridKeyIndex.py
 peek_plugin_diagram/_private/storage/LiveDbDispLink.py
 peek_plugin_diagram/_private/storage/LocationIndex.py
+peek_plugin_diagram/_private/storage/Lookups.py
 peek_plugin_diagram/_private/storage/ModelSet.py
 peek_plugin_diagram/_private/storage/Setting.py
 peek_plugin_diagram/_private/storage/__init__.py
 peek_plugin_diagram/_private/storage/branch/BranchIndex.py
 peek_plugin_diagram/_private/storage/branch/BranchIndexCompilerQueue.py
 peek_plugin_diagram/_private/storage/branch/BranchIndexEncodedChunk.py
 peek_plugin_diagram/_private/storage/branch/__init__.py
@@ -291,14 +293,18 @@
 peek_plugin_diagram/_private/tuples/location_index/EncodedLocationIndexTuple.py
 peek_plugin_diagram/_private/tuples/location_index/LocationIndexTuple.py
 peek_plugin_diagram/_private/tuples/location_index/LocationIndexUpdateDateTuple.py
 peek_plugin_diagram/_private/tuples/location_index/__init__.py
 peek_plugin_diagram/_private/worker/WorkerEntryHook.py
 peek_plugin_diagram/_private/worker/__init__.py
 peek_plugin_diagram/_private/worker/api/WorkerApiImpl.py
+peek_plugin_diagram/_private/worker/api/WorkerDiagramGridApiImpl.py
+peek_plugin_diagram/_private/worker/api/WorkerDiagramGridApiImplTest.py
+peek_plugin_diagram/_private/worker/api/WorkerDiagramGridApiImpl_SQLPrints.py
+peek_plugin_diagram/_private/worker/api/WorkerDiagramLookupApiImpl.py
 peek_plugin_diagram/_private/worker/api/__init__.py
 peek_plugin_diagram/_private/worker/tasks/DispCompilerTask.py
 peek_plugin_diagram/_private/worker/tasks/GridCompilerTask.py
 peek_plugin_diagram/_private/worker/tasks/ImportDispLink.py
 peek_plugin_diagram/_private/worker/tasks/ImportDispTask.py
 peek_plugin_diagram/_private/worker/tasks/LiveDbDisplayValueConverter.py
 peek_plugin_diagram/_private/worker/tasks/LocationIndexCompilerTask.py
@@ -306,19 +312,21 @@
 peek_plugin_diagram/_private/worker/tasks/_CalcDisp.py
 peek_plugin_diagram/_private/worker/tasks/_CalcDispFromLiveDb.py
 peek_plugin_diagram/_private/worker/tasks/_CalcGridForDisp.py
 peek_plugin_diagram/_private/worker/tasks/_CalcLocation.py
 peek_plugin_diagram/_private/worker/tasks/_ModelSetUtil.py
 peek_plugin_diagram/_private/worker/tasks/__init__.py
 peek_plugin_diagram/_private/worker/tasks/branch/BranchDispUpdater.py
-peek_plugin_diagram/_private/worker/tasks/branch/BranchIndexCompiler.py
-peek_plugin_diagram/_private/worker/tasks/branch/BranchIndexImporter.py
-peek_plugin_diagram/_private/worker/tasks/branch/BranchIndexUpdater.py
+peek_plugin_diagram/_private/worker/tasks/branch/BranchIndexCompilerTask.py
+peek_plugin_diagram/_private/worker/tasks/branch/BranchIndexImporterTask.py
+peek_plugin_diagram/_private/worker/tasks/branch/BranchIndexUpdaterTask.py
 peek_plugin_diagram/_private/worker/tasks/branch/_BranchIndexCalcChunkKey.py
 peek_plugin_diagram/_private/worker/tasks/branch/__init__.py
+peek_plugin_diagram/_private/worker/utils/ShapeLookupLinker.py
+peek_plugin_diagram/_private/worker/utils/__init__.py
 peek_plugin_diagram/admin-doc/admin_tasks.rst
 peek_plugin_diagram/admin-doc/diagram_layers.jpg
 peek_plugin_diagram/admin-doc/edit_zoom_limit.png
 peek_plugin_diagram/admin-doc/enable_markup.png
 peek_plugin_diagram/admin-doc/example_diagram.png
 peek_plugin_diagram/admin-doc/index.rst
 peek_plugin_diagram/admin-doc/overview.rst
@@ -357,32 +365,35 @@
 peek_plugin_diagram/plugin-module/_private/branch/BranchUpdateTupleAction.ts
 peek_plugin_diagram/plugin-module/_private/branch/PrivateDiagramBranchContext.ts
 peek_plugin_diagram/plugin-module/_private/branch/PrivateDiagramBranchService.ts
 peek_plugin_diagram/plugin-module/_private/branch/index.ts
 peek_plugin_diagram/plugin-module/_private/branch-loader/BranchIndexEncodedChunkTuple.ts
 peek_plugin_diagram/plugin-module/_private/branch-loader/BranchIndexLoaderService.ts
 peek_plugin_diagram/plugin-module/_private/branch-loader/BranchIndexLoaderServiceA.ts
-peek_plugin_diagram/plugin-module/_private/branch-loader/BranchIndexLoaderStatusTuple.ts
 peek_plugin_diagram/plugin-module/_private/branch-loader/BranchIndexUpdateDateTuple.ts
 peek_plugin_diagram/plugin-module/_private/branch-loader/LocalBranchStorageService.ts
 peek_plugin_diagram/plugin-module/_private/branch-loader/index.ts
 peek_plugin_diagram/plugin-module/_private/grid-loader/EncodedGridTuple.ts
 peek_plugin_diagram/plugin-module/_private/grid-loader/GridTuple.ts
 peek_plugin_diagram/plugin-module/_private/grid-loader/GridUpdateDateTuple.ts
 peek_plugin_diagram/plugin-module/_private/grid-loader/PrivateDiagramGridLoaderService.ts
 peek_plugin_diagram/plugin-module/_private/grid-loader/PrivateDiagramGridLoaderServiceA.ts
-peek_plugin_diagram/plugin-module/_private/grid-loader/PrivateDiagramGridLoaderStatusTuple.ts
 peek_plugin_diagram/plugin-module/_private/grid-loader/index.ts
 peek_plugin_diagram/plugin-module/_private/location-loader/DispKeyLocationTuple.ts
 peek_plugin_diagram/plugin-module/_private/location-loader/EncodedLocationIndexTuple.ts
 peek_plugin_diagram/plugin-module/_private/location-loader/LocationIndexTuple.ts
 peek_plugin_diagram/plugin-module/_private/location-loader/LocationIndexUpdateDateTuple.ts
 peek_plugin_diagram/plugin-module/_private/location-loader/PrivateDiagramLocationLoaderService.ts
-peek_plugin_diagram/plugin-module/_private/location-loader/PrivateDiagramLocationLoaderStatusTuple.ts
 peek_plugin_diagram/plugin-module/_private/location-loader/index.ts
+peek_plugin_diagram/plugin-module/_private/lookups/DispColor.ts
+peek_plugin_diagram/plugin-module/_private/lookups/DispLayer.ts
+peek_plugin_diagram/plugin-module/_private/lookups/DispLevel.ts
+peek_plugin_diagram/plugin-module/_private/lookups/DispLineStyle.ts
+peek_plugin_diagram/plugin-module/_private/lookups/DispTextStyle.ts
+peek_plugin_diagram/plugin-module/_private/lookups/index.ts
 peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramConfigService.ts
 peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramCoordSetService.ts
 peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramItemSelectService.ts
 peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramLookupService.ts
 peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramOfflineCacherService.ts
 peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramOverrideService.ts
 peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramPositionService.ts
@@ -391,36 +402,47 @@
 peek_plugin_diagram/plugin-module/_private/services/PrivateDiagramTupleService.ts
 peek_plugin_diagram/plugin-module/_private/services/index.ts
 peek_plugin_diagram/plugin-module/_private/tuples/GroupDispsTuple.ts
 peek_plugin_diagram/plugin-module/_private/tuples/ModelCoordSet.ts
 peek_plugin_diagram/plugin-module/_private/tuples/ModelCoordSetGridSize.ts
 peek_plugin_diagram/plugin-module/_private/tuples/ModelSet.ts
 peek_plugin_diagram/plugin-module/_private/tuples/index.ts
-peek_plugin_diagram/plugin-module/lookups/DispColor.ts
-peek_plugin_diagram/plugin-module/lookups/DispLayer.ts
-peek_plugin_diagram/plugin-module/lookups/DispLevel.ts
-peek_plugin_diagram/plugin-module/lookups/DispLineStyle.ts
-peek_plugin_diagram/plugin-module/lookups/DispTextStyle.ts
-peek_plugin_diagram/plugin-module/lookups/index.ts
+peek_plugin_diagram/plugin-module/lookup_tuples/ShapeColorTuple.ts
+peek_plugin_diagram/plugin-module/lookup_tuples/ShapeLayerTuple.ts
+peek_plugin_diagram/plugin-module/lookup_tuples/ShapeLevelTuple.ts
+peek_plugin_diagram/plugin-module/lookup_tuples/ShapeLineStyleTuple.ts
+peek_plugin_diagram/plugin-module/lookup_tuples/ShapeTextStyleTuple.ts
+peek_plugin_diagram/plugin-module/lookup_tuples/index.ts
 peek_plugin_diagram/plugin-module/override/DiagramOverrideBase.ts
 peek_plugin_diagram/plugin-module/override/DiagramOverrideColor.ts
 peek_plugin_diagram/plugin-module/override/DiagramOverrideHighlight.ts
 peek_plugin_diagram/plugin-module/override/index.ts
 peek_plugin_diagram/plugin-module/tuples/DiagramCoordSetTuple.ts
 peek_plugin_diagram/server/DiagramApiABC.py
 peek_plugin_diagram/server/DiagramImportApiABC.py
 peek_plugin_diagram/server/DiagramViewerApiABC.py
 peek_plugin_diagram/server/__init__.py
+peek_plugin_diagram/tuples/ColorUtil.py
+peek_plugin_diagram/tuples/ColorUtilTest.py
 peek_plugin_diagram/tuples/ImportGroupHashTuple.py
 peek_plugin_diagram/tuples/ImportTypes.py
 peek_plugin_diagram/tuples/__init__.py
 peek_plugin_diagram/tuples/branches/ImportBranchDeltaColorOverride.py
 peek_plugin_diagram/tuples/branches/ImportBranchDeltaCreateDisp.py
 peek_plugin_diagram/tuples/branches/ImportBranchTuple.py
 peek_plugin_diagram/tuples/branches/__init__.py
+peek_plugin_diagram/tuples/grids/DecodedCompiledGridTuple.py
+peek_plugin_diagram/tuples/grids/GridKeyTuple.py
+peek_plugin_diagram/tuples/grids/__init__.py
+peek_plugin_diagram/tuples/lookup_tuples/ShapeColorTuple.py
+peek_plugin_diagram/tuples/lookup_tuples/ShapeLayerTuple.py
+peek_plugin_diagram/tuples/lookup_tuples/ShapeLevelTuple.py
+peek_plugin_diagram/tuples/lookup_tuples/ShapeLineStyleTuple.py
+peek_plugin_diagram/tuples/lookup_tuples/ShapeTextStyleTuple.py
+peek_plugin_diagram/tuples/lookup_tuples/__init__.py
 peek_plugin_diagram/tuples/lookups/ImportDispColorTuple.py
 peek_plugin_diagram/tuples/lookups/ImportDispLayerTuple.py
 peek_plugin_diagram/tuples/lookups/ImportDispLevelTuple.py
 peek_plugin_diagram/tuples/lookups/ImportDispLineStyleTuple.py
 peek_plugin_diagram/tuples/lookups/ImportDispTextStyleTuple.py
 peek_plugin_diagram/tuples/lookups/__init__.py
 peek_plugin_diagram/tuples/model/DiagramCoordSetTuple.py
@@ -432,8 +454,21 @@
 peek_plugin_diagram/tuples/shapes/ImportDispGroupPtrTuple.py
 peek_plugin_diagram/tuples/shapes/ImportDispGroupTuple.py
 peek_plugin_diagram/tuples/shapes/ImportDispPolygonTuple.py
 peek_plugin_diagram/tuples/shapes/ImportDispPolylineTuple.py
 peek_plugin_diagram/tuples/shapes/ImportDispTextTuple.py
 peek_plugin_diagram/tuples/shapes/__init__.py
 peek_plugin_diagram/worker/WorkerApi.py
-peek_plugin_diagram/worker/__init__.py
+peek_plugin_diagram/worker/WorkerDiagramGridApi.py
+peek_plugin_diagram/worker/WorkerDiagramLookupApi.py
+peek_plugin_diagram/worker/__init__.py
+peek_plugin_diagram/worker/canvas_shapes/ShapeBase.py
+peek_plugin_diagram/worker/canvas_shapes/ShapeCurvedText.py
+peek_plugin_diagram/worker/canvas_shapes/ShapeEllipse.py
+peek_plugin_diagram/worker/canvas_shapes/ShapeGroup.py
+peek_plugin_diagram/worker/canvas_shapes/ShapeGroupPointer.py
+peek_plugin_diagram/worker/canvas_shapes/ShapeNull.py
+peek_plugin_diagram/worker/canvas_shapes/ShapePoly.py
+peek_plugin_diagram/worker/canvas_shapes/ShapePolyLine.py
+peek_plugin_diagram/worker/canvas_shapes/ShapePolygon.py
+peek_plugin_diagram/worker/canvas_shapes/ShapeText.py
+peek_plugin_diagram/worker/canvas_shapes/__init__.py
```

### Comparing `peek-plugin-diagram-3.3.3/setup.py` & `peek-plugin-diagram-3.4.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Modify these values to fork a new plugin
 #
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_plugin_diagram"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.3.3"
+package_version = "3.4.0"
 description = "Peek Plugin Diagram - My first enhancement."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 ###############################################################################
@@ -45,44 +45,55 @@
         for filename in filenames:
             if [e for e in excludeFilesEndWith if filename.endswith(e)]:
                 continue
 
             if [e for e in excludeFilesStartWith if filename.startswith(e)]:
                 continue
 
-            paths.append(os.path.join(path[len(py_package_name) + 1 :], filename))
+            paths.append(
+                os.path.join(path[len(py_package_name) + 1 :], filename)
+            )
 
     return paths
 
 
 package_files = find_package_files()
 
 ###############################################################################
 # Define the dependencies
 
 # Ensure the dependency is the same major number
 # and no older then this version
 
-requirements = ["peek-plugin-base", "Numpy"]
+requirements = [
+    "peek-plugin-base",
+    "Numpy",
+    "tinycss2>=1.2.1,<2.0",
+    "colormath>=3.0.0,<4.0",
+]
 
 # Force the dependencies to be the same branch
 reqVer = ".".join(package_version.split(".")[0:2]) + ".*"
 
 # >=2.0.*,>=2.0.6
 requirements = [
-    "%s==%s,>=%s" % (pkg, reqVer, package_version.split("+")[0]) if pkg.startswith("peek") else pkg
+    "%s==%s,>=%s" % (pkg, reqVer, package_version.split("+")[0])
+    if pkg.startswith("peek")
+    else pkg
     for pkg in requirements
 ]
 
 ###############################################################################
 # Call the setuptools
 
 setup(
     name=pip_package_name,
-    packages=find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests"]),
+    packages=find_packages(
+        exclude=["*.tests", "*.tests.*", "tests.*", "tests"]
+    ),
     package_data={"": package_files},
     install_requires=requirements,
     version=package_version,
     description=description,
     author=author,
     author_email=author_email,
     url=url,
```

