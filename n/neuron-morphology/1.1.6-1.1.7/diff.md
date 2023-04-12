# Comparing `tmp/neuron-morphology-1.1.6.tar.gz` & `tmp/neuron-morphology-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/neuron-morphology-1.1.6.tar", last modified: Sat Mar 18 13:48:53 2023, max compression
+gzip compressed data, was "dist/neuron-morphology-1.1.7.tar", last modified: Wed Apr 12 15:56:56 2023, max compression
```

## Comparing `neuron-morphology-1.1.6.tar` & `neuron-morphology-1.1.7.tar`

### file list

```diff
@@ -1,207 +1,207 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     1955 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/LICENSE
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)      221 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1919 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/PKG-INFO
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     1206 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/README.md
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)    89079 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/feature_description.html
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/neuron_morphology/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        7 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/VERSION.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      372 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/constants.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/neuron_morphology/feature_extractor/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/feature_extractor/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3446 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/feature_extractor/__main__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5559 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/feature_extractor/_schemas.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      924 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/feature_extractor/data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3942 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/feature_extractor/feature_extraction_run.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3194 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/feature_extractor/feature_extractor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3807 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/feature_extractor/feature_specialization.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8503 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/feature_extractor/feature_writer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5576 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/feature_extractor/mark.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6747 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/feature_extractor/marked_feature.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5698 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/feature_extractor/run_feature_extraction.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      894 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/feature_extractor/utilities.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/neuron_morphology/features/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/features/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/neuron_morphology/features/branching/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/features/branching/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5786 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/features/branching/bifurcations.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3543 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/features/default_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2641 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/features/dimension.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10282 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/features/intrinsic.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/neuron_morphology/features/layer/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/features/layer/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12320 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/features/layer/layer_histogram.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2966 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/features/layer/layered_point_depths.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4180 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/features/layer/reference_layer_depths.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9283 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/features/path.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7262 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/features/size.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6623 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/features/soma.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/neuron_morphology/features/statistics/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/features/statistics/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4171 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/features/statistics/coordinates.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1641 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/features/statistics/moments.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2784 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/features/statistics/moments_along_max_distance_projection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4049 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/features/statistics/overlap.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/neuron_morphology/layered_point_depths/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/layered_point_depths/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11173 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/layered_point_depths/__main__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3218 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/layered_point_depths/_schemas.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8535 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/lims_apical_queries.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      308 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/logging_config.ini
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1736 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/marker.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    21975 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/morphology.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4321 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/morphology_builder.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/neuron_morphology/pipeline/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/pipeline/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3041 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/pipeline/_schemas.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4102 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/pipeline/post_data_to_s3.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/neuron_morphology/snap_polygons/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/snap_polygons/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3177 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/snap_polygons/__main__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10084 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/snap_polygons/_from_lims.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5244 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/snap_polygons/_schemas.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4580 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/snap_polygons/bounding_box.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5393 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/snap_polygons/cortex_surfaces.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    20493 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/snap_polygons/geometries.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7666 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/snap_polygons/image_outputter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3021 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/snap_polygons/types.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2494 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/swc_io.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/neuron_morphology/transforms/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/transforms/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8872 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/transforms/affine_transform.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/neuron_morphology/transforms/affine_transformer/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/transforms/affine_transformer/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2313 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/transforms/affine_transformer/_schemas.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1097 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/transforms/affine_transformer/apply_affine_transform.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3328 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/transforms/geometry.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/neuron_morphology/transforms/pia_wm_streamlines/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/transforms/pia_wm_streamlines/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2006 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/transforms/pia_wm_streamlines/_schemas.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3827 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/transforms/pia_wm_streamlines/calculate_pia_wm_streamlines.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/neuron_morphology/transforms/scale_correction/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/transforms/scale_correction/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1240 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/transforms/scale_correction/_schemas.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4915 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/transforms/scale_correction/compute_scale_correction.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5496 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/transforms/streamline.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/neuron_morphology/transforms/tilt_correction/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/transforms/tilt_correction/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2535 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/transforms/tilt_correction/_schemas.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8344 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/transforms/tilt_correction/compute_tilt_correction.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      775 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/transforms/transform_base.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/neuron_morphology/transforms/upright_angle/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/transforms/upright_angle/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2297 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/transforms/upright_angle/_schemas.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3502 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/transforms/upright_angle/compute_angle.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/neuron_morphology/validation/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      637 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/validation/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2663 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/validation/bits_validation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6419 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/validation/marker_validation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      635 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/validation/morphology_statistics.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5398 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/validation/radius_validation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1775 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/validation/report.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      757 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/validation/resample_validation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2720 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/validation/result.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      568 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/validation/structure_validation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5956 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/validation/type_validation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3529 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/validation/validate_reconstruction.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/neuron_morphology/vis/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/vis/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1260 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/neuron_morphology/vis/morphovis.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/neuron_morphology.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1919 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/neuron_morphology.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7818 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/neuron_morphology.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/neuron_morphology.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      592 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/neuron_morphology.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      206 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/neuron_morphology.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/neuron_morphology.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/setup.cfg
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     3090 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/tests/data/
--rw-r--r--   0 circleci  (3434) circleci  (3434)   172958 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/data/17545-6151-X24259-Y36270.swc
--rw-r--r--   0 circleci  (3434) circleci  (3434)   113784 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/data/Ctgf-2A-dgCre-D_Ai14_BT_-245170.06.06.01_539748835_m_pia.swc
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1306 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/data/cortex_morphology_summary.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8865 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/data/high_res_morphology_summary.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1454 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/data/morphology_summary.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6609 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/data/normalized_depth_morphology_summary.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)   356630 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/data/reconstruction_tile_viewer.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)       91 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/data/reconstruction_tile_viewer_input.csv
--rw-r--r--   0 circleci  (3434) circleci  (3434)    96407 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/data/reconstruction_tile_viewer_input_data.csv
--rw-r--r--   0 circleci  (3434) circleci  (3434)  1226128 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/data/test_swc.swc
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/tests/feature_extractor/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/tests/feature_extractor/branching_features/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7555 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/feature_extractor/branching_features/test_bifurcations.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/tests/feature_extractor/layer_features/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5432 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/feature_extractor/layer_features/test_layer_histogram_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1220 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/feature_extractor/layer_features/test_reference_layer_depths.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/tests/feature_extractor/statistic_features/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5759 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/feature_extractor/statistic_features/test_moment_along_max_distance_projection_feature.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4525 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/feature_extractor/statistic_features/test_moment_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4834 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/feature_extractor/statistic_features/test_overlap_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1002 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/feature_extractor/test_data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      568 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/feature_extractor/test_default_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4483 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/feature_extractor/test_dimension_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2364 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/feature_extractor/test_feature_extraction_run.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3546 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/feature_extractor/test_feature_writer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5918 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/feature_extractor/test_intrinsic_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4550 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/feature_extractor/test_main.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2251 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/feature_extractor/test_marked_feature.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7950 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/feature_extractor/test_path_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5192 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/feature_extractor/test_size_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6165 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/feature_extractor/test_soma_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      280 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/feature_extractor/test_utilities.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/tests/features/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3501 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/features/test_intrinsic.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1178 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/features/test_number_of_stems.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3431 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/features/test_path.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2271 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/features/test_stem_exit.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/tests/layered_point_depths/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/layered_point_depths/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4449 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/layered_point_depths/test_main.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9040 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/objects.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/tests/pipeline/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/pipeline/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1786 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/pipeline/test_post_data_to_s3.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/tests/snap_polygons/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/snap_polygons/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/tests/snap_polygons/data/
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     6097 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/snap_polygons/data/678492000_inputs.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)   421935 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/snap_polygons/data/678492000_outputs.json
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)    21195 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/snap_polygons/data/680352737_inputs.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)   487970 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/snap_polygons/data/680352737_outputs.json
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)    47959 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/snap_polygons/data/735355641_inputs.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)   241790 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/snap_polygons/data/735355641_outputs.json
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     6811 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/snap_polygons/data/839050458_inputs.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)   303683 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/snap_polygons/data/839050458_outputs.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1148 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/snap_polygons/test_bounding_box.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4740 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/snap_polygons/test_cortex_surfaces.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7969 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/snap_polygons/test_geometries.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5602 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/snap_polygons/test_image_outputter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1660 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/snap_polygons/test_integration.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1020 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/snap_polygons/test_types.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1332 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/test_morphology_builder.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1647 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/test_swc_io.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15951 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/test_tree.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/tests/transforms/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5889 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/transforms/test_affine_transform.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2468 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/transforms/test_apply_affine.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2010 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/transforms/test_calculate_pia_wm_streamlines.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1812 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/transforms/test_geometry.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4278 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/transforms/test_scale_correction.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1188 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/transforms/test_streamline.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4512 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/transforms/test_tilt_correction.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1133 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/transforms/test_transform_base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2674 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/transforms/test_upright_angle.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:53.000000 neuron-morphology-1.1.6/tests/validation/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/validation/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7217 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/validation/test_bits_validation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8101 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/validation/test_marker_validation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    22156 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/validation/test_radius_validation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1759 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/validation/test_resample_validation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1934 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/validation/test_statistics.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1527 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/validation/test_structure_validation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9838 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/validation/test_type_validation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      976 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/validation/test_validate_reconstruction.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1433 2023-03-18 13:48:41.000000 neuron-morphology-1.1.6/tests/validation/validation_test_case.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     1955 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/LICENSE
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      221 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1919 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/PKG-INFO
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     1206 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/README.md
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)    89079 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/feature_description.html
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/neuron_morphology/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        7 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/VERSION.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      372 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/constants.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/neuron_morphology/feature_extractor/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/feature_extractor/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3446 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/feature_extractor/__main__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5559 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/feature_extractor/_schemas.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      924 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/feature_extractor/data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3942 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/feature_extractor/feature_extraction_run.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3194 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/feature_extractor/feature_extractor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3807 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/feature_extractor/feature_specialization.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8503 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/feature_extractor/feature_writer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5576 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/feature_extractor/mark.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6747 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/feature_extractor/marked_feature.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5698 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/feature_extractor/run_feature_extraction.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      894 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/feature_extractor/utilities.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/neuron_morphology/features/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/features/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/neuron_morphology/features/branching/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/features/branching/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5786 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/features/branching/bifurcations.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3543 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/features/default_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2641 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/features/dimension.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10282 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/features/intrinsic.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/neuron_morphology/features/layer/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/features/layer/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12320 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/features/layer/layer_histogram.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2966 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/features/layer/layered_point_depths.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4180 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/features/layer/reference_layer_depths.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9283 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/features/path.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7262 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/features/size.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6623 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/features/soma.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/neuron_morphology/features/statistics/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/features/statistics/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4171 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/features/statistics/coordinates.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1641 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/features/statistics/moments.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2784 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/features/statistics/moments_along_max_distance_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4049 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/features/statistics/overlap.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/neuron_morphology/layered_point_depths/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/layered_point_depths/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11173 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/layered_point_depths/__main__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3218 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/layered_point_depths/_schemas.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8535 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/lims_apical_queries.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      308 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/logging_config.ini
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1736 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/marker.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    21975 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/morphology.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4321 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/morphology_builder.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/neuron_morphology/pipeline/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/pipeline/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3041 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/pipeline/_schemas.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4102 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/pipeline/post_data_to_s3.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/neuron_morphology/snap_polygons/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/snap_polygons/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3177 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/snap_polygons/__main__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10084 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/snap_polygons/_from_lims.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5244 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/snap_polygons/_schemas.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4580 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/snap_polygons/bounding_box.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5393 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/snap_polygons/cortex_surfaces.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    20493 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/snap_polygons/geometries.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7666 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/snap_polygons/image_outputter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3021 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/snap_polygons/types.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2494 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/swc_io.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/neuron_morphology/transforms/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/transforms/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8872 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/transforms/affine_transform.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/neuron_morphology/transforms/affine_transformer/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/transforms/affine_transformer/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2313 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/transforms/affine_transformer/_schemas.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1097 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/transforms/affine_transformer/apply_affine_transform.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3328 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/transforms/geometry.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/neuron_morphology/transforms/pia_wm_streamlines/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/transforms/pia_wm_streamlines/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2006 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/transforms/pia_wm_streamlines/_schemas.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3827 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/transforms/pia_wm_streamlines/calculate_pia_wm_streamlines.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/neuron_morphology/transforms/scale_correction/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/transforms/scale_correction/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1240 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/transforms/scale_correction/_schemas.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4915 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/transforms/scale_correction/compute_scale_correction.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5496 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/transforms/streamline.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/neuron_morphology/transforms/tilt_correction/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/transforms/tilt_correction/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2535 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/transforms/tilt_correction/_schemas.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8344 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/transforms/tilt_correction/compute_tilt_correction.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      775 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/transforms/transform_base.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/neuron_morphology/transforms/upright_angle/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/transforms/upright_angle/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2297 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/transforms/upright_angle/_schemas.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3502 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/transforms/upright_angle/compute_angle.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/neuron_morphology/validation/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      637 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/validation/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2663 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/validation/bits_validation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6419 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/validation/marker_validation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      635 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/validation/morphology_statistics.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5398 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/validation/radius_validation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1775 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/validation/report.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      757 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/validation/resample_validation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2720 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/validation/result.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      568 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/validation/structure_validation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5956 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/validation/type_validation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3529 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/validation/validate_reconstruction.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/neuron_morphology/vis/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/vis/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1260 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/neuron_morphology/vis/morphovis.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/neuron_morphology.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1919 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/neuron_morphology.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7818 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/neuron_morphology.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/neuron_morphology.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      592 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/neuron_morphology.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      237 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/neuron_morphology.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/neuron_morphology.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/setup.cfg
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     3097 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/tests/data/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   172958 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/data/17545-6151-X24259-Y36270.swc
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   113784 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/data/Ctgf-2A-dgCre-D_Ai14_BT_-245170.06.06.01_539748835_m_pia.swc
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1306 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/data/cortex_morphology_summary.png
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8865 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/data/high_res_morphology_summary.png
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1454 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/data/morphology_summary.png
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6609 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/data/normalized_depth_morphology_summary.png
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   356630 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/data/reconstruction_tile_viewer.html
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       91 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/data/reconstruction_tile_viewer_input.csv
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    96407 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/data/reconstruction_tile_viewer_input_data.csv
+-rw-r--r--   0 circleci  (3434) circleci  (3434)  1226128 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/data/test_swc.swc
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/tests/feature_extractor/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/tests/feature_extractor/branching_features/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7555 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/feature_extractor/branching_features/test_bifurcations.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/tests/feature_extractor/layer_features/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5432 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/feature_extractor/layer_features/test_layer_histogram_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1220 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/feature_extractor/layer_features/test_reference_layer_depths.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/tests/feature_extractor/statistic_features/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5759 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/feature_extractor/statistic_features/test_moment_along_max_distance_projection_feature.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4525 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/feature_extractor/statistic_features/test_moment_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4834 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/feature_extractor/statistic_features/test_overlap_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1002 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/feature_extractor/test_data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      568 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/feature_extractor/test_default_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4483 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/feature_extractor/test_dimension_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2364 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/feature_extractor/test_feature_extraction_run.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3546 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/feature_extractor/test_feature_writer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5918 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/feature_extractor/test_intrinsic_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4550 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/feature_extractor/test_main.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2251 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/feature_extractor/test_marked_feature.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7950 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/feature_extractor/test_path_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5192 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/feature_extractor/test_size_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6165 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/feature_extractor/test_soma_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      280 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/feature_extractor/test_utilities.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/tests/features/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3501 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/features/test_intrinsic.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1178 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/features/test_number_of_stems.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3431 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/features/test_path.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2271 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/features/test_stem_exit.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/tests/layered_point_depths/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/layered_point_depths/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4449 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/layered_point_depths/test_main.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9040 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/objects.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/tests/pipeline/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/pipeline/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1786 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/pipeline/test_post_data_to_s3.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/tests/snap_polygons/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/snap_polygons/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/tests/snap_polygons/data/
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     6097 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/snap_polygons/data/678492000_inputs.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   421935 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/snap_polygons/data/678492000_outputs.json
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)    21195 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/snap_polygons/data/680352737_inputs.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   487970 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/snap_polygons/data/680352737_outputs.json
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)    47959 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/snap_polygons/data/735355641_inputs.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   241790 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/snap_polygons/data/735355641_outputs.json
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     6811 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/snap_polygons/data/839050458_inputs.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   303683 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/snap_polygons/data/839050458_outputs.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1148 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/snap_polygons/test_bounding_box.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4740 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/snap_polygons/test_cortex_surfaces.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7969 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/snap_polygons/test_geometries.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5602 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/snap_polygons/test_image_outputter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1660 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/snap_polygons/test_integration.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1020 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/snap_polygons/test_types.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1332 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/test_morphology_builder.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1647 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/test_swc_io.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15951 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/test_tree.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/tests/transforms/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5889 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/transforms/test_affine_transform.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2468 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/transforms/test_apply_affine.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2010 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/transforms/test_calculate_pia_wm_streamlines.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1812 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/transforms/test_geometry.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4278 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/transforms/test_scale_correction.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1188 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/transforms/test_streamline.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4512 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/transforms/test_tilt_correction.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1133 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/transforms/test_transform_base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2674 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/transforms/test_upright_angle.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:56.000000 neuron-morphology-1.1.7/tests/validation/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/validation/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7217 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/validation/test_bits_validation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8101 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/validation/test_marker_validation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    22156 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/validation/test_radius_validation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1759 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/validation/test_resample_validation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1934 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/validation/test_statistics.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1527 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/validation/test_structure_validation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9838 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/validation/test_type_validation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      976 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/validation/test_validate_reconstruction.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1433 2023-04-12 15:56:41.000000 neuron-morphology-1.1.7/tests/validation/validation_test_case.py
```

### Comparing `neuron-morphology-1.1.6/LICENSE` & `neuron-morphology-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/PKG-INFO` & `neuron-morphology-1.1.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuron-morphology
-Version: 1.1.6
+Version: 1.1.7
 Summary: Tools for working with single-neuron morphological reconstructions
 Author: Allen Institute for Brain Science
 Author-email: Marmot@AllenInstitute.onmicrosoft.com
 Keywords: neuroscience,bioinformatics,scientific
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
```

### Comparing `neuron-morphology-1.1.6/README.md` & `neuron-morphology-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/feature_description.html` & `neuron-morphology-1.1.7/feature_description.html`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/feature_extractor/__main__.py` & `neuron-morphology-1.1.7/neuron_morphology/feature_extractor/__main__.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/feature_extractor/_schemas.py` & `neuron-morphology-1.1.7/neuron_morphology/feature_extractor/_schemas.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/feature_extractor/data.py` & `neuron-morphology-1.1.7/neuron_morphology/feature_extractor/data.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/feature_extractor/feature_extraction_run.py` & `neuron-morphology-1.1.7/neuron_morphology/feature_extractor/feature_extraction_run.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/feature_extractor/feature_extractor.py` & `neuron-morphology-1.1.7/neuron_morphology/feature_extractor/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/feature_extractor/feature_specialization.py` & `neuron-morphology-1.1.7/neuron_morphology/feature_extractor/feature_specialization.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/feature_extractor/feature_writer.py` & `neuron-morphology-1.1.7/neuron_morphology/feature_extractor/feature_writer.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/feature_extractor/mark.py` & `neuron-morphology-1.1.7/neuron_morphology/feature_extractor/mark.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/feature_extractor/marked_feature.py` & `neuron-morphology-1.1.7/neuron_morphology/feature_extractor/marked_feature.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/feature_extractor/run_feature_extraction.py` & `neuron-morphology-1.1.7/neuron_morphology/feature_extractor/run_feature_extraction.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/feature_extractor/utilities.py` & `neuron-morphology-1.1.7/neuron_morphology/feature_extractor/utilities.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/features/branching/bifurcations.py` & `neuron-morphology-1.1.7/neuron_morphology/features/branching/bifurcations.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/features/default_features.py` & `neuron-morphology-1.1.7/neuron_morphology/features/default_features.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/features/dimension.py` & `neuron-morphology-1.1.7/neuron_morphology/features/dimension.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/features/intrinsic.py` & `neuron-morphology-1.1.7/neuron_morphology/features/intrinsic.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/features/layer/layer_histogram.py` & `neuron-morphology-1.1.7/neuron_morphology/features/layer/layer_histogram.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/features/layer/layered_point_depths.py` & `neuron-morphology-1.1.7/neuron_morphology/features/layer/layered_point_depths.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/features/layer/reference_layer_depths.py` & `neuron-morphology-1.1.7/neuron_morphology/features/layer/reference_layer_depths.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/features/path.py` & `neuron-morphology-1.1.7/neuron_morphology/features/path.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/features/size.py` & `neuron-morphology-1.1.7/neuron_morphology/features/size.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/features/soma.py` & `neuron-morphology-1.1.7/neuron_morphology/features/soma.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/features/statistics/coordinates.py` & `neuron-morphology-1.1.7/neuron_morphology/features/statistics/coordinates.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/features/statistics/moments.py` & `neuron-morphology-1.1.7/neuron_morphology/features/statistics/moments.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/features/statistics/moments_along_max_distance_projection.py` & `neuron-morphology-1.1.7/neuron_morphology/features/statistics/moments_along_max_distance_projection.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/features/statistics/overlap.py` & `neuron-morphology-1.1.7/neuron_morphology/features/statistics/overlap.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/layered_point_depths/__main__.py` & `neuron-morphology-1.1.7/neuron_morphology/layered_point_depths/__main__.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/layered_point_depths/_schemas.py` & `neuron-morphology-1.1.7/neuron_morphology/layered_point_depths/_schemas.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/lims_apical_queries.py` & `neuron-morphology-1.1.7/neuron_morphology/lims_apical_queries.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/marker.py` & `neuron-morphology-1.1.7/neuron_morphology/marker.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/morphology.py` & `neuron-morphology-1.1.7/neuron_morphology/morphology.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/morphology_builder.py` & `neuron-morphology-1.1.7/neuron_morphology/morphology_builder.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/pipeline/_schemas.py` & `neuron-morphology-1.1.7/neuron_morphology/pipeline/_schemas.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/pipeline/post_data_to_s3.py` & `neuron-morphology-1.1.7/neuron_morphology/pipeline/post_data_to_s3.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/snap_polygons/__main__.py` & `neuron-morphology-1.1.7/neuron_morphology/snap_polygons/__main__.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/snap_polygons/_from_lims.py` & `neuron-morphology-1.1.7/neuron_morphology/snap_polygons/_from_lims.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/snap_polygons/_schemas.py` & `neuron-morphology-1.1.7/neuron_morphology/snap_polygons/_schemas.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/snap_polygons/bounding_box.py` & `neuron-morphology-1.1.7/neuron_morphology/snap_polygons/bounding_box.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/snap_polygons/cortex_surfaces.py` & `neuron-morphology-1.1.7/neuron_morphology/snap_polygons/cortex_surfaces.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/snap_polygons/geometries.py` & `neuron-morphology-1.1.7/neuron_morphology/snap_polygons/geometries.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/snap_polygons/image_outputter.py` & `neuron-morphology-1.1.7/neuron_morphology/snap_polygons/image_outputter.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/snap_polygons/types.py` & `neuron-morphology-1.1.7/neuron_morphology/snap_polygons/types.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/swc_io.py` & `neuron-morphology-1.1.7/neuron_morphology/swc_io.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/transforms/affine_transform.py` & `neuron-morphology-1.1.7/neuron_morphology/transforms/affine_transform.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/transforms/affine_transformer/_schemas.py` & `neuron-morphology-1.1.7/neuron_morphology/transforms/affine_transformer/_schemas.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/transforms/affine_transformer/apply_affine_transform.py` & `neuron-morphology-1.1.7/neuron_morphology/transforms/affine_transformer/apply_affine_transform.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/transforms/geometry.py` & `neuron-morphology-1.1.7/neuron_morphology/transforms/geometry.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/transforms/pia_wm_streamlines/_schemas.py` & `neuron-morphology-1.1.7/neuron_morphology/transforms/pia_wm_streamlines/_schemas.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/transforms/pia_wm_streamlines/calculate_pia_wm_streamlines.py` & `neuron-morphology-1.1.7/neuron_morphology/transforms/pia_wm_streamlines/calculate_pia_wm_streamlines.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/transforms/scale_correction/_schemas.py` & `neuron-morphology-1.1.7/neuron_morphology/transforms/scale_correction/_schemas.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/transforms/scale_correction/compute_scale_correction.py` & `neuron-morphology-1.1.7/neuron_morphology/transforms/scale_correction/compute_scale_correction.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/transforms/streamline.py` & `neuron-morphology-1.1.7/neuron_morphology/transforms/streamline.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/transforms/tilt_correction/_schemas.py` & `neuron-morphology-1.1.7/neuron_morphology/transforms/tilt_correction/_schemas.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/transforms/tilt_correction/compute_tilt_correction.py` & `neuron-morphology-1.1.7/neuron_morphology/transforms/tilt_correction/compute_tilt_correction.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/transforms/transform_base.py` & `neuron-morphology-1.1.7/neuron_morphology/transforms/transform_base.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/transforms/upright_angle/_schemas.py` & `neuron-morphology-1.1.7/neuron_morphology/transforms/upright_angle/_schemas.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/transforms/upright_angle/compute_angle.py` & `neuron-morphology-1.1.7/neuron_morphology/transforms/upright_angle/compute_angle.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/validation/__init__.py` & `neuron-morphology-1.1.7/neuron_morphology/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/validation/bits_validation.py` & `neuron-morphology-1.1.7/neuron_morphology/validation/bits_validation.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/validation/marker_validation.py` & `neuron-morphology-1.1.7/neuron_morphology/validation/marker_validation.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/validation/morphology_statistics.py` & `neuron-morphology-1.1.7/neuron_morphology/validation/morphology_statistics.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/validation/radius_validation.py` & `neuron-morphology-1.1.7/neuron_morphology/validation/radius_validation.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/validation/report.py` & `neuron-morphology-1.1.7/neuron_morphology/validation/report.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/validation/resample_validation.py` & `neuron-morphology-1.1.7/neuron_morphology/validation/resample_validation.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/validation/result.py` & `neuron-morphology-1.1.7/neuron_morphology/validation/result.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/validation/structure_validation.py` & `neuron-morphology-1.1.7/neuron_morphology/validation/structure_validation.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/validation/type_validation.py` & `neuron-morphology-1.1.7/neuron_morphology/validation/type_validation.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/validation/validate_reconstruction.py` & `neuron-morphology-1.1.7/neuron_morphology/validation/validate_reconstruction.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology/vis/morphovis.py` & `neuron-morphology-1.1.7/neuron_morphology/vis/morphovis.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology.egg-info/PKG-INFO` & `neuron-morphology-1.1.7/neuron_morphology.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuron-morphology
-Version: 1.1.6
+Version: 1.1.7
 Summary: Tools for working with single-neuron morphological reconstructions
 Author: Allen Institute for Brain Science
 Author-email: Marmot@AllenInstitute.onmicrosoft.com
 Keywords: neuroscience,bioinformatics,scientific
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
```

### Comparing `neuron-morphology-1.1.6/neuron_morphology.egg-info/SOURCES.txt` & `neuron-morphology-1.1.7/neuron_morphology.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/neuron_morphology.egg-info/entry_points.txt` & `neuron-morphology-1.1.7/neuron_morphology.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/setup.py` & `neuron-morphology-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     name="neuron-morphology",
     author="Allen Institute for Brain Science",
     author_email="Marmot@AllenInstitute.onmicrosoft.com",
     packages=find_packages(),
     include_package_data=True,
     description="Tools for working with single-neuron morphological reconstructions",
     long_description=readme,
-    extras_require={"streamlines": ["fenics-dolfinx", "gmsh", "rasterio"]},
+    extras_require={"streamlines": ["fenics-dolfinx", "python-gmsh", "rasterio"]},
     long_description_content_type="text/markdown",
     entry_points={
         "console_scripts": [
             "feature_extractor       = neuron_morphology.feature_extractor.__main__:main",
             "layered_point_depths    = neuron_morphology.layered_point_depths.__main__:main",
             "snap_polygons           = neuron_morphology.snap_polygons.__main__:main",
             "apply_affine_transform  = neuron_morphology.transforms.affine_transformer.apply_affine_transform:main",
```

### Comparing `neuron-morphology-1.1.6/tests/data/17545-6151-X24259-Y36270.swc` & `neuron-morphology-1.1.7/tests/data/17545-6151-X24259-Y36270.swc`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/data/Ctgf-2A-dgCre-D_Ai14_BT_-245170.06.06.01_539748835_m_pia.swc` & `neuron-morphology-1.1.7/tests/data/Ctgf-2A-dgCre-D_Ai14_BT_-245170.06.06.01_539748835_m_pia.swc`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/data/cortex_morphology_summary.png` & `neuron-morphology-1.1.7/tests/data/cortex_morphology_summary.png`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/data/high_res_morphology_summary.png` & `neuron-morphology-1.1.7/tests/data/high_res_morphology_summary.png`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/data/morphology_summary.png` & `neuron-morphology-1.1.7/tests/data/morphology_summary.png`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/data/normalized_depth_morphology_summary.png` & `neuron-morphology-1.1.7/tests/data/normalized_depth_morphology_summary.png`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/data/reconstruction_tile_viewer.html` & `neuron-morphology-1.1.7/tests/data/reconstruction_tile_viewer.html`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/data/reconstruction_tile_viewer_input_data.csv` & `neuron-morphology-1.1.7/tests/data/reconstruction_tile_viewer_input_data.csv`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/data/test_swc.swc` & `neuron-morphology-1.1.7/tests/data/test_swc.swc`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/feature_extractor/branching_features/test_bifurcations.py` & `neuron-morphology-1.1.7/tests/feature_extractor/branching_features/test_bifurcations.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/feature_extractor/layer_features/test_layer_histogram_features.py` & `neuron-morphology-1.1.7/tests/feature_extractor/layer_features/test_layer_histogram_features.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/feature_extractor/layer_features/test_reference_layer_depths.py` & `neuron-morphology-1.1.7/tests/feature_extractor/layer_features/test_reference_layer_depths.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/feature_extractor/statistic_features/test_moment_along_max_distance_projection_feature.py` & `neuron-morphology-1.1.7/tests/feature_extractor/statistic_features/test_moment_along_max_distance_projection_feature.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/feature_extractor/statistic_features/test_moment_features.py` & `neuron-morphology-1.1.7/tests/feature_extractor/statistic_features/test_moment_features.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/feature_extractor/statistic_features/test_overlap_features.py` & `neuron-morphology-1.1.7/tests/feature_extractor/statistic_features/test_overlap_features.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/feature_extractor/test_data.py` & `neuron-morphology-1.1.7/tests/feature_extractor/test_data.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/feature_extractor/test_default_features.py` & `neuron-morphology-1.1.7/tests/feature_extractor/test_default_features.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/feature_extractor/test_dimension_features.py` & `neuron-morphology-1.1.7/tests/feature_extractor/test_dimension_features.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/feature_extractor/test_feature_extraction_run.py` & `neuron-morphology-1.1.7/tests/feature_extractor/test_feature_extraction_run.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/feature_extractor/test_feature_writer.py` & `neuron-morphology-1.1.7/tests/feature_extractor/test_feature_writer.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/feature_extractor/test_intrinsic_features.py` & `neuron-morphology-1.1.7/tests/feature_extractor/test_intrinsic_features.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/feature_extractor/test_main.py` & `neuron-morphology-1.1.7/tests/feature_extractor/test_main.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/feature_extractor/test_marked_feature.py` & `neuron-morphology-1.1.7/tests/feature_extractor/test_marked_feature.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/feature_extractor/test_path_features.py` & `neuron-morphology-1.1.7/tests/feature_extractor/test_path_features.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/feature_extractor/test_size_features.py` & `neuron-morphology-1.1.7/tests/feature_extractor/test_size_features.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/feature_extractor/test_soma_features.py` & `neuron-morphology-1.1.7/tests/feature_extractor/test_soma_features.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/features/test_intrinsic.py` & `neuron-morphology-1.1.7/tests/features/test_intrinsic.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/features/test_number_of_stems.py` & `neuron-morphology-1.1.7/tests/features/test_number_of_stems.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/features/test_path.py` & `neuron-morphology-1.1.7/tests/features/test_path.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/features/test_stem_exit.py` & `neuron-morphology-1.1.7/tests/features/test_stem_exit.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/layered_point_depths/test_main.py` & `neuron-morphology-1.1.7/tests/layered_point_depths/test_main.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/objects.py` & `neuron-morphology-1.1.7/tests/objects.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/pipeline/test_post_data_to_s3.py` & `neuron-morphology-1.1.7/tests/pipeline/test_post_data_to_s3.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/snap_polygons/data/678492000_inputs.json` & `neuron-morphology-1.1.7/tests/snap_polygons/data/678492000_inputs.json`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/snap_polygons/data/678492000_outputs.json` & `neuron-morphology-1.1.7/tests/snap_polygons/data/678492000_outputs.json`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/snap_polygons/data/680352737_inputs.json` & `neuron-morphology-1.1.7/tests/snap_polygons/data/680352737_inputs.json`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/snap_polygons/data/680352737_outputs.json` & `neuron-morphology-1.1.7/tests/snap_polygons/data/680352737_outputs.json`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/snap_polygons/data/735355641_inputs.json` & `neuron-morphology-1.1.7/tests/snap_polygons/data/735355641_inputs.json`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/snap_polygons/data/735355641_outputs.json` & `neuron-morphology-1.1.7/tests/snap_polygons/data/735355641_outputs.json`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/snap_polygons/data/839050458_inputs.json` & `neuron-morphology-1.1.7/tests/snap_polygons/data/839050458_inputs.json`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/snap_polygons/data/839050458_outputs.json` & `neuron-morphology-1.1.7/tests/snap_polygons/data/839050458_outputs.json`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/snap_polygons/test_bounding_box.py` & `neuron-morphology-1.1.7/tests/snap_polygons/test_bounding_box.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/snap_polygons/test_cortex_surfaces.py` & `neuron-morphology-1.1.7/tests/snap_polygons/test_cortex_surfaces.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/snap_polygons/test_geometries.py` & `neuron-morphology-1.1.7/tests/snap_polygons/test_geometries.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/snap_polygons/test_image_outputter.py` & `neuron-morphology-1.1.7/tests/snap_polygons/test_image_outputter.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/snap_polygons/test_integration.py` & `neuron-morphology-1.1.7/tests/snap_polygons/test_integration.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/snap_polygons/test_types.py` & `neuron-morphology-1.1.7/tests/snap_polygons/test_types.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/test_morphology_builder.py` & `neuron-morphology-1.1.7/tests/test_morphology_builder.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/test_swc_io.py` & `neuron-morphology-1.1.7/tests/test_swc_io.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/test_tree.py` & `neuron-morphology-1.1.7/tests/test_tree.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/transforms/test_affine_transform.py` & `neuron-morphology-1.1.7/tests/transforms/test_affine_transform.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/transforms/test_apply_affine.py` & `neuron-morphology-1.1.7/tests/transforms/test_apply_affine.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/transforms/test_calculate_pia_wm_streamlines.py` & `neuron-morphology-1.1.7/tests/transforms/test_calculate_pia_wm_streamlines.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/transforms/test_geometry.py` & `neuron-morphology-1.1.7/tests/transforms/test_geometry.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/transforms/test_scale_correction.py` & `neuron-morphology-1.1.7/tests/transforms/test_scale_correction.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/transforms/test_streamline.py` & `neuron-morphology-1.1.7/tests/transforms/test_streamline.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/transforms/test_tilt_correction.py` & `neuron-morphology-1.1.7/tests/transforms/test_tilt_correction.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/transforms/test_transform_base.py` & `neuron-morphology-1.1.7/tests/transforms/test_transform_base.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/transforms/test_upright_angle.py` & `neuron-morphology-1.1.7/tests/transforms/test_upright_angle.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/validation/test_bits_validation.py` & `neuron-morphology-1.1.7/tests/validation/test_bits_validation.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/validation/test_marker_validation.py` & `neuron-morphology-1.1.7/tests/validation/test_marker_validation.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/validation/test_radius_validation.py` & `neuron-morphology-1.1.7/tests/validation/test_radius_validation.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/validation/test_resample_validation.py` & `neuron-morphology-1.1.7/tests/validation/test_resample_validation.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/validation/test_statistics.py` & `neuron-morphology-1.1.7/tests/validation/test_statistics.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/validation/test_structure_validation.py` & `neuron-morphology-1.1.7/tests/validation/test_structure_validation.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/validation/test_type_validation.py` & `neuron-morphology-1.1.7/tests/validation/test_type_validation.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/validation/test_validate_reconstruction.py` & `neuron-morphology-1.1.7/tests/validation/test_validate_reconstruction.py`

 * *Files identical despite different names*

### Comparing `neuron-morphology-1.1.6/tests/validation/validation_test_case.py` & `neuron-morphology-1.1.7/tests/validation/validation_test_case.py`

 * *Files identical despite different names*

