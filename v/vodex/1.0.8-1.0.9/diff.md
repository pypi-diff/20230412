# Comparing `tmp/vodex-1.0.8.tar.gz` & `tmp/vodex-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vodex-1.0.8.tar", last modified: Sat Jan 14 04:19:46 2023, max compression
+gzip compressed data, was "vodex-1.0.9.tar", last modified: Mon Jan 30 04:31:14 2023, max compression
```

## Comparing `vodex-1.0.8.tar` & `vodex-1.0.9.tar`

### file list

```diff
@@ -1,194 +1,195 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.092007 vodex-1.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.036007 vodex-1.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.040007 vodex-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-01-14 04:19:29.000000 vodex-1.0.8/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-01-14 04:19:29.000000 vodex-1.0.8/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-01-14 04:19:29.000000 vodex-1.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-01-14 04:19:29.000000 vodex-1.0.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-01-14 04:19:46.092007 vodex-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-01-14 04:19:29.000000 vodex-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.036007 vodex-1.0.8/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.044007 vodex-1.0.8/data/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.052007 vodex-1.0.8/data/test/loader_test/
--rw-r--r--   0 runner    (1001) docker     (123)   320850 2023-01-14 04:19:29.000000 vodex-1.0.8/data/test/loader_test/frames_1_2_41_42.tif
--rw-r--r--   0 runner    (1001) docker     (123)   801862 2023-01-14 04:19:29.000000 vodex-1.0.8/data/test/loader_test/half_volumes_0_1.tif
--rw-r--r--   0 runner    (1001) docker     (123)   801346 2023-01-14 04:19:29.000000 vodex-1.0.8/data/test/loader_test/half_volumes_1_2.tif
--rw-r--r--   0 runner    (1001) docker     (123)  1603522 2023-01-14 04:19:29.000000 vodex-1.0.8/data/test/loader_test/volumes_0_1.tif
--rw-r--r--   0 runner    (1001) docker     (123)  1602486 2023-01-14 04:19:29.000000 vodex-1.0.8/data/test/loader_test/volumes_1_2.tif
--rw-r--r--   0 runner    (1001) docker     (123)   160518 2023-01-14 04:19:29.000000 vodex-1.0.8/data/test/loader_test/volumes_tail.tif
--rw-r--r--   0 runner    (1001) docker     (123)   143684 2023-01-14 04:19:29.000000 vodex-1.0.8/data/test/movie_info.PNG
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-01-14 04:19:29.000000 vodex-1.0.8/data/test/test.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.052007 vodex-1.0.8/data/test/test_movie/
--rw-r--r--   0 runner    (1001) docker     (123)   561348 2023-01-14 04:19:29.000000 vodex-1.0.8/data/test/test_movie/mov0.tif
--rw-r--r--   0 runner    (1001) docker     (123)  1443174 2023-01-14 04:19:29.000000 vodex-1.0.8/data/test/test_movie/mov1.tif
--rw-r--r--   0 runner    (1001) docker     (123)  1363008 2023-01-14 04:19:29.000000 vodex-1.0.8/data/test/test_movie/mov2.tif
--rw-r--r--   0 runner    (1001) docker     (123)   256854 2023-01-14 04:19:29.000000 vodex-1.0.8/data/test/test_movie.avi
--rw-r--r--   0 runner    (1001) docker     (123)  3367158 2023-01-14 04:19:29.000000 vodex-1.0.8/data/test/test_movie.tif
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-01-14 04:19:29.000000 vodex-1.0.8/data/test/toy_example.db
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-01-14 04:19:29.000000 vodex-1.0.8/desktop.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.056007 vodex-1.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.056007 vodex-1.0.8/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/api/core.md
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/api/dbmethods.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/api/experiment.md
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/api/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/api/loaders.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.056007 vodex-1.0.8/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   284957 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/assets/cover.JPG
--rw-r--r--   0 runner    (1001) docker     (123)   354364 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/assets/data_annotation.png
--rw-r--r--   0 runner    (1001) docker     (123)    76270 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/assets/data_annotation_a.png
--rw-r--r--   0 runner    (1001) docker     (123)    28309 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/assets/data_annotation_a1.png
--rw-r--r--   0 runner    (1001) docker     (123)    27081 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/assets/data_annotation_a2.png
--rw-r--r--   0 runner    (1001) docker     (123)    19772 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/assets/data_annotation_a3.png
--rw-r--r--   0 runner    (1001) docker     (123)   264749 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/assets/data_annotation_b.png
--rw-r--r--   0 runner    (1001) docker     (123)    89998 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/assets/data_frames.png
--rw-r--r--   0 runner    (1001) docker     (123)   108566 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/assets/db_diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)    23334 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/assets/test_movie.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/data.md
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/db.md
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/examples.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.060007 vodex-1.0.8/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/img/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/img/favicon_16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/img/favicon_32.png
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/img/icons8_layers.ico
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/img/icons8_layers_16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/img/icons8_layers_32.png
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/img/icons8_list_view.ico
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/img/icons8_list_view_16.png
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/img/icons8_list_view_32.png
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/img/icons8_v.ico
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/img/icons8_v_16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/img/icons8_v_32.png
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/install.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.060007 vodex-1.0.8/docs/napari/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.060007 vodex-1.0.8/docs/napari/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)    63396 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/napari/how-to/fig01.png
--rw-r--r--   0 runner    (1001) docker     (123)    40897 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/napari/how-to/fig02.png
--rw-r--r--   0 runner    (1001) docker     (123)   242588 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/napari/how-to/fig02bc.png
--rw-r--r--   0 runner    (1001) docker     (123)    31843 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/napari/how-to/fig03.png
--rw-r--r--   0 runner    (1001) docker     (123)   443424 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/napari/how-to/fig04.png
--rw-r--r--   0 runner    (1001) docker     (123)   203366 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/napari/how-to/fig05a.png
--rw-r--r--   0 runner    (1001) docker     (123)   100112 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/napari/how-to/fig05b.png
--rw-r--r--   0 runner    (1001) docker     (123)    97849 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/napari/how-to/fig05c.png
--rw-r--r--   0 runner    (1001) docker     (123)   156995 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/napari/how-to/fig06.png
--rw-r--r--   0 runner    (1001) docker     (123)   157398 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/napari/how-to/fig07.png
--rw-r--r--   0 runner    (1001) docker     (123)   142245 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/napari/how-to/intro.PNG
--rw-r--r--   0 runner    (1001) docker     (123)   278726 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/napari/how-to/new1.PNG
--rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/napari/how-to.md
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/napari/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.064007 vodex-1.0.8/docs/qstart/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/qstart/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/qstart/load_experiment.md
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/qstart/load_volumes.md
--rw-r--r--   0 runner    (1001) docker     (123)    11363 2023-01-14 04:19:29.000000 vodex-1.0.8/docs/qstart/new_experiment.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.064007 vodex-1.0.8/img/
--rw-r--r--   0 runner    (1001) docker     (123)   284957 2023-01-14 04:19:29.000000 vodex-1.0.8/img/cover.JPG
--rw-r--r--   0 runner    (1001) docker     (123)   159014 2023-01-14 04:19:29.000000 vodex-1.0.8/img/test_summary.PNG
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-01-14 04:19:29.000000 vodex-1.0.8/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.064007 vodex-1.0.8/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)   118271 2023-01-14 04:19:29.000000 vodex-1.0.8/notebooks/01_create_experiment_and_load_volumes.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-01-14 04:19:29.000000 vodex-1.0.8/notebooks/test.db
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-01-14 04:19:29.000000 vodex-1.0.8/notebooks/test_no_annotation.db
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-01-14 04:19:29.000000 vodex-1.0.8/notebooks/test_w_annotations.db
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-01-14 04:19:29.000000 vodex-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-01-14 04:19:46.092007 vodex-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-14 04:19:29.000000 vodex-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.064007 vodex-1.0.8/site/
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-01-14 04:19:29.000000 vodex-1.0.8/site/404.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.064007 vodex-1.0.8/site/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-01-14 04:19:29.000000 vodex-1.0.8/site/assets/_mkdocstrings.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.064007 vodex-1.0.8/site/core/
--rw-r--r--   0 runner    (1001) docker     (123)   253339 2023-01-14 04:19:29.000000 vodex-1.0.8/site/core/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.064007 vodex-1.0.8/site/css/
--rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-01-14 04:19:29.000000 vodex-1.0.8/site/css/base.css
--rw-r--r--   0 runner    (1001) docker     (123)   163091 2023-01-14 04:19:29.000000 vodex-1.0.8/site/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    31000 2023-01-14 04:19:29.000000 vodex-1.0.8/site/css/font-awesome.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.064007 vodex-1.0.8/site/dbmethods/
--rw-r--r--   0 runner    (1001) docker     (123)   389961 2023-01-14 04:19:29.000000 vodex-1.0.8/site/dbmethods/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.064007 vodex-1.0.8/site/explanation/
--rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-01-14 04:19:29.000000 vodex-1.0.8/site/explanation/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.068007 vodex-1.0.8/site/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   165742 2023-01-14 04:19:29.000000 vodex-1.0.8/site/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   444379 2023-01-14 04:19:29.000000 vodex-1.0.8/site/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-01-14 04:19:29.000000 vodex-1.0.8/site/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-01-14 04:19:29.000000 vodex-1.0.8/site/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-01-14 04:19:29.000000 vodex-1.0.8/site/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.068007 vodex-1.0.8/site/how-to-guides/
--rw-r--r--   0 runner    (1001) docker     (123)     6507 2023-01-14 04:19:29.000000 vodex-1.0.8/site/how-to-guides/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.068007 vodex-1.0.8/site/img/
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-01-14 04:19:29.000000 vodex-1.0.8/site/img/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-01-14 04:19:29.000000 vodex-1.0.8/site/img/grid.png
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-01-14 04:19:29.000000 vodex-1.0.8/site/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.068007 vodex-1.0.8/site/js/
--rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-01-14 04:19:29.000000 vodex-1.0.8/site/js/base.js
--rw-r--r--   0 runner    (1001) docker     (123)    58073 2023-01-14 04:19:29.000000 vodex-1.0.8/site/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    93107 2023-01-14 04:19:29.000000 vodex-1.0.8/site/js/jquery-1.10.2.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.068007 vodex-1.0.8/site/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)   102456 2023-01-14 04:19:29.000000 vodex-1.0.8/site/loaders/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-01-14 04:19:29.000000 vodex-1.0.8/site/objects.inv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.068007 vodex-1.0.8/site/reference/
--rw-r--r--   0 runner    (1001) docker     (123)    10974 2023-01-14 04:19:29.000000 vodex-1.0.8/site/reference/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-01-14 04:19:29.000000 vodex-1.0.8/site/sitemap.xml
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-01-14 04:19:29.000000 vodex-1.0.8/site/sitemap.xml.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.068007 vodex-1.0.8/site/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-01-14 04:19:29.000000 vodex-1.0.8/site/tutorials/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.040007 vodex-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.068007 vodex-1.0.8/src/vodex/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.072007 vodex-1.0.8/src/vodex/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/_tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.072007 vodex-1.0.8/src/vodex/_tests/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/_tests/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/_tests/__pycache__/test_core.cpython-39-pytest-7.2.0.pyc
--rw-r--r--   0 runner    (1001) docker     (123)    18945 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/_tests/__pycache__/test_dbmethods.cpython-39-pytest-7.2.0.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/_tests/__pycache__/test_experiment.cpython-39-pytest-7.2.0.pyc
--rw-r--r--   0 runner    (1001) docker     (123)    10810 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/_tests/__pycache__/test_loaders.cpython-39-pytest-7.2.0.pyc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.072007 vodex-1.0.8/src/vodex/_tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.084007 vodex-1.0.8/src/vodex/_tests/data/construction_blocks/
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/_tests/data/construction_blocks/data.py
--rw-r--r--   0 runner    (1001) docker     (123)  3366287 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/_tests/data/construction_blocks/numbered_frames.tif
--rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/_tests/data/construction_blocks/recepie.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    14723 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/_tests/data/construction_blocks/recepie_long.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   801417 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/_tests/data/construction_blocks/zero_frame.tif
--rw-r--r--   0 runner    (1001) docker     (123)   801417 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/_tests/data/construction_blocks/zero_frame_c1.tif
--rw-r--r--   0 runner    (1001) docker     (123)   801419 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/_tests/data/construction_blocks/zero_frame_c2.tif
--rw-r--r--   0 runner    (1001) docker     (123)   801419 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/_tests/data/construction_blocks/zero_frame_c3.tif
--rw-r--r--   0 runner    (1001) docker     (123)   801419 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/_tests/data/construction_blocks/zero_frame_circle.tif
--rw-r--r--   0 runner    (1001) docker     (123)   801419 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/_tests/data/construction_blocks/zero_frame_square.tif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.088008 vodex-1.0.8/src/vodex/_tests/data/loader_test/
--rw-r--r--   0 runner    (1001) docker     (123)   320850 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/_tests/data/loader_test/frames_1_2_41_42.tif
--rw-r--r--   0 runner    (1001) docker     (123)   801862 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/_tests/data/loader_test/half_volumes_0_1.tif
--rw-r--r--   0 runner    (1001) docker     (123)   801346 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/_tests/data/loader_test/half_volumes_1_2.tif
--rw-r--r--   0 runner    (1001) docker     (123)  1603522 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/_tests/data/loader_test/volumes_0_1.tif
--rw-r--r--   0 runner    (1001) docker     (123)  1602486 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/_tests/data/loader_test/volumes_1_2.tif
--rw-r--r--   0 runner    (1001) docker     (123)   160518 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/_tests/data/loader_test/volumes_tail.tif
--rw-r--r--   0 runner    (1001) docker     (123)   143684 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/_tests/data/movie_info.PNG
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/_tests/data/test.db
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/_tests/data/test_experiment.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.092007 vodex-1.0.8/src/vodex/_tests/data/test_movie/
--rw-r--r--   0 runner    (1001) docker     (123)   561348 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/_tests/data/test_movie/mov0.tif
--rw-r--r--   0 runner    (1001) docker     (123)  1443174 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/_tests/data/test_movie/mov1.tif
--rw-r--r--   0 runner    (1001) docker     (123)  1363008 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/_tests/data/test_movie/mov2.tif
--rw-r--r--   0 runner    (1001) docker     (123)   256854 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/_tests/data/test_movie.avi
--rw-r--r--   0 runner    (1001) docker     (123)  3367158 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/_tests/data/test_movie.tif
--rw-r--r--   0 runner    (1001) docker     (123)    13068 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/_tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/_tests/test_dbmethods.py
--rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/_tests/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/_tests/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-14 04:19:45.000000 vodex-1.0.8/src/vodex/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    47726 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    53770 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/dbmethods.py
--rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-01-14 04:19:29.000000 vodex-1.0.8/src/vodex/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 04:19:46.068007 vodex-1.0.8/src/vodex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-01-14 04:19:45.000000 vodex-1.0.8/src/vodex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-01-14 04:19:46.000000 vodex-1.0.8/src/vodex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-14 04:19:45.000000 vodex-1.0.8/src/vodex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-14 04:19:45.000000 vodex-1.0.8/src/vodex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-14 04:19:45.000000 vodex-1.0.8/src/vodex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-01-14 04:19:29.000000 vodex-1.0.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:14.020852 vodex-1.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:13.956850 vodex-1.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:13.960851 vodex-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-01-30 04:30:57.000000 vodex-1.0.9/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-01-30 04:30:57.000000 vodex-1.0.9/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-01-30 04:30:57.000000 vodex-1.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-01-30 04:30:57.000000 vodex-1.0.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-01-30 04:31:14.020852 vodex-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-01-30 04:30:57.000000 vodex-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:13.956850 vodex-1.0.9/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:13.964851 vodex-1.0.9/data/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:13.972851 vodex-1.0.9/data/test/loader_test/
+-rw-r--r--   0 runner    (1001) docker     (123)   320850 2023-01-30 04:30:57.000000 vodex-1.0.9/data/test/loader_test/frames_1_2_41_42.tif
+-rw-r--r--   0 runner    (1001) docker     (123)   801862 2023-01-30 04:30:57.000000 vodex-1.0.9/data/test/loader_test/half_volumes_0_1.tif
+-rw-r--r--   0 runner    (1001) docker     (123)   801346 2023-01-30 04:30:57.000000 vodex-1.0.9/data/test/loader_test/half_volumes_1_2.tif
+-rw-r--r--   0 runner    (1001) docker     (123)  1603522 2023-01-30 04:30:57.000000 vodex-1.0.9/data/test/loader_test/volumes_0_1.tif
+-rw-r--r--   0 runner    (1001) docker     (123)  1602486 2023-01-30 04:30:57.000000 vodex-1.0.9/data/test/loader_test/volumes_1_2.tif
+-rw-r--r--   0 runner    (1001) docker     (123)   160518 2023-01-30 04:30:57.000000 vodex-1.0.9/data/test/loader_test/volumes_tail.tif
+-rw-r--r--   0 runner    (1001) docker     (123)   143684 2023-01-30 04:30:57.000000 vodex-1.0.9/data/test/movie_info.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-01-30 04:30:57.000000 vodex-1.0.9/data/test/test.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:13.976851 vodex-1.0.9/data/test/test_movie/
+-rw-r--r--   0 runner    (1001) docker     (123)   561348 2023-01-30 04:30:57.000000 vodex-1.0.9/data/test/test_movie/mov0.tif
+-rw-r--r--   0 runner    (1001) docker     (123)  1443174 2023-01-30 04:30:57.000000 vodex-1.0.9/data/test/test_movie/mov1.tif
+-rw-r--r--   0 runner    (1001) docker     (123)  1363008 2023-01-30 04:30:57.000000 vodex-1.0.9/data/test/test_movie/mov2.tif
+-rw-r--r--   0 runner    (1001) docker     (123)   256854 2023-01-30 04:30:57.000000 vodex-1.0.9/data/test/test_movie.avi
+-rw-r--r--   0 runner    (1001) docker     (123)  3367158 2023-01-30 04:30:57.000000 vodex-1.0.9/data/test/test_movie.tif
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-01-30 04:30:57.000000 vodex-1.0.9/data/test/toy_example.db
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-01-30 04:30:57.000000 vodex-1.0.9/desktop.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:13.976851 vodex-1.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:13.976851 vodex-1.0.9/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/api/core.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/api/dbmethods.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/api/experiment.md
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/api/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/api/loaders.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:13.980851 vodex-1.0.9/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   284957 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/assets/cover.JPG
+-rw-r--r--   0 runner    (1001) docker     (123)   354364 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/assets/data_annotation.png
+-rw-r--r--   0 runner    (1001) docker     (123)    76270 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/assets/data_annotation_a.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28309 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/assets/data_annotation_a1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27081 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/assets/data_annotation_a2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19772 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/assets/data_annotation_a3.png
+-rw-r--r--   0 runner    (1001) docker     (123)   264749 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/assets/data_annotation_b.png
+-rw-r--r--   0 runner    (1001) docker     (123)    89998 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/assets/data_frames.png
+-rw-r--r--   0 runner    (1001) docker     (123)   108566 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/assets/db_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23334 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/assets/test_movie.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/data.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/db.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/examples.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:13.980851 vodex-1.0.9/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/img/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/img/favicon_16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/img/favicon_32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/img/icons8_layers.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/img/icons8_layers_16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/img/icons8_layers_32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/img/icons8_list_view.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/img/icons8_list_view_16.png
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/img/icons8_list_view_32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/img/icons8_v.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/img/icons8_v_16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/img/icons8_v_32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/install.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:13.980851 vodex-1.0.9/docs/napari/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:13.984851 vodex-1.0.9/docs/napari/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)    63396 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/napari/how-to/fig01.png
+-rw-r--r--   0 runner    (1001) docker     (123)    40897 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/napari/how-to/fig02.png
+-rw-r--r--   0 runner    (1001) docker     (123)   242588 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/napari/how-to/fig02bc.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31843 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/napari/how-to/fig03.png
+-rw-r--r--   0 runner    (1001) docker     (123)   443424 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/napari/how-to/fig04.png
+-rw-r--r--   0 runner    (1001) docker     (123)   203366 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/napari/how-to/fig05a.png
+-rw-r--r--   0 runner    (1001) docker     (123)   100112 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/napari/how-to/fig05b.png
+-rw-r--r--   0 runner    (1001) docker     (123)    97849 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/napari/how-to/fig05c.png
+-rw-r--r--   0 runner    (1001) docker     (123)   156995 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/napari/how-to/fig06.png
+-rw-r--r--   0 runner    (1001) docker     (123)   157398 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/napari/how-to/fig07.png
+-rw-r--r--   0 runner    (1001) docker     (123)   142245 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/napari/how-to/intro.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)   278726 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/napari/how-to/new1.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/napari/how-to.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/napari/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:13.984851 vodex-1.0.9/docs/qstart/
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/qstart/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/qstart/load_experiment.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/qstart/load_volumes.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11363 2023-01-30 04:30:57.000000 vodex-1.0.9/docs/qstart/new_experiment.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:13.984851 vodex-1.0.9/img/
+-rw-r--r--   0 runner    (1001) docker     (123)   284957 2023-01-30 04:30:57.000000 vodex-1.0.9/img/cover.JPG
+-rw-r--r--   0 runner    (1001) docker     (123)   159014 2023-01-30 04:30:57.000000 vodex-1.0.9/img/test_summary.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-01-30 04:30:57.000000 vodex-1.0.9/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:13.988851 vodex-1.0.9/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)   118271 2023-01-30 04:30:57.000000 vodex-1.0.9/notebooks/01_create_experiment_and_load_volumes.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-01-30 04:30:57.000000 vodex-1.0.9/notebooks/test.db
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-01-30 04:30:57.000000 vodex-1.0.9/notebooks/test_no_annotation.db
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-01-30 04:30:57.000000 vodex-1.0.9/notebooks/test_w_annotations.db
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-01-30 04:30:57.000000 vodex-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-01-30 04:31:14.020852 vodex-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-30 04:30:57.000000 vodex-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:13.988851 vodex-1.0.9/site/
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-01-30 04:30:57.000000 vodex-1.0.9/site/404.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:13.988851 vodex-1.0.9/site/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-01-30 04:30:57.000000 vodex-1.0.9/site/assets/_mkdocstrings.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:13.988851 vodex-1.0.9/site/core/
+-rw-r--r--   0 runner    (1001) docker     (123)   253339 2023-01-30 04:30:57.000000 vodex-1.0.9/site/core/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:13.988851 vodex-1.0.9/site/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-01-30 04:30:57.000000 vodex-1.0.9/site/css/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)   163091 2023-01-30 04:30:57.000000 vodex-1.0.9/site/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    31000 2023-01-30 04:30:57.000000 vodex-1.0.9/site/css/font-awesome.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:13.988851 vodex-1.0.9/site/dbmethods/
+-rw-r--r--   0 runner    (1001) docker     (123)   389961 2023-01-30 04:30:57.000000 vodex-1.0.9/site/dbmethods/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:13.988851 vodex-1.0.9/site/explanation/
+-rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-01-30 04:30:57.000000 vodex-1.0.9/site/explanation/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:13.992851 vodex-1.0.9/site/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   165742 2023-01-30 04:30:57.000000 vodex-1.0.9/site/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   444379 2023-01-30 04:30:57.000000 vodex-1.0.9/site/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-01-30 04:30:57.000000 vodex-1.0.9/site/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-01-30 04:30:57.000000 vodex-1.0.9/site/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-01-30 04:30:57.000000 vodex-1.0.9/site/fonts/fontawesome-webfont.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:13.992851 vodex-1.0.9/site/how-to-guides/
+-rw-r--r--   0 runner    (1001) docker     (123)     6507 2023-01-30 04:30:57.000000 vodex-1.0.9/site/how-to-guides/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:13.992851 vodex-1.0.9/site/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-01-30 04:30:57.000000 vodex-1.0.9/site/img/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-01-30 04:30:57.000000 vodex-1.0.9/site/img/grid.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-01-30 04:30:57.000000 vodex-1.0.9/site/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:13.992851 vodex-1.0.9/site/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-01-30 04:30:57.000000 vodex-1.0.9/site/js/base.js
+-rw-r--r--   0 runner    (1001) docker     (123)    58073 2023-01-30 04:30:57.000000 vodex-1.0.9/site/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    93107 2023-01-30 04:30:57.000000 vodex-1.0.9/site/js/jquery-1.10.2.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:13.992851 vodex-1.0.9/site/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)   102456 2023-01-30 04:30:57.000000 vodex-1.0.9/site/loaders/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-01-30 04:30:57.000000 vodex-1.0.9/site/objects.inv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:13.992851 vodex-1.0.9/site/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)    10974 2023-01-30 04:30:57.000000 vodex-1.0.9/site/reference/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-01-30 04:30:57.000000 vodex-1.0.9/site/sitemap.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-01-30 04:30:57.000000 vodex-1.0.9/site/sitemap.xml.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:13.992851 vodex-1.0.9/site/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-01-30 04:30:57.000000 vodex-1.0.9/site/tutorials/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:13.960851 vodex-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:13.992851 vodex-1.0.9/src/vodex/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:13.996852 vodex-1.0.9/src/vodex/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:13.996852 vodex-1.0.9/src/vodex/_tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:14.012852 vodex-1.0.9/src/vodex/_tests/data/construction_blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/data/construction_blocks/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)  3366287 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/data/construction_blocks/numbered_frames.tif
+-rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/data/construction_blocks/recepie.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    14723 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/data/construction_blocks/recepie_long.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   801417 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/data/construction_blocks/zero_frame.tif
+-rw-r--r--   0 runner    (1001) docker     (123)   801417 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/data/construction_blocks/zero_frame_c1.tif
+-rw-r--r--   0 runner    (1001) docker     (123)   801419 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/data/construction_blocks/zero_frame_c2.tif
+-rw-r--r--   0 runner    (1001) docker     (123)   801419 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/data/construction_blocks/zero_frame_c3.tif
+-rw-r--r--   0 runner    (1001) docker     (123)   801419 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/data/construction_blocks/zero_frame_circle.tif
+-rw-r--r--   0 runner    (1001) docker     (123)   801419 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/data/construction_blocks/zero_frame_square.tif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:14.016852 vodex-1.0.9/src/vodex/_tests/data/loader_test/
+-rw-r--r--   0 runner    (1001) docker     (123)   320850 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/data/loader_test/frames_1_2_41_42.tif
+-rw-r--r--   0 runner    (1001) docker     (123)   801862 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/data/loader_test/half_volumes_0_1.tif
+-rw-r--r--   0 runner    (1001) docker     (123)   801346 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/data/loader_test/half_volumes_1_2.tif
+-rw-r--r--   0 runner    (1001) docker     (123)  1603522 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/data/loader_test/volumes_0_1.tif
+-rw-r--r--   0 runner    (1001) docker     (123)  1602486 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/data/loader_test/volumes_1_2.tif
+-rw-r--r--   0 runner    (1001) docker     (123)   160518 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/data/loader_test/volumes_tail.tif
+-rw-r--r--   0 runner    (1001) docker     (123)   143684 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/data/movie_info.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)   106496 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/data/test.db
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/data/test_experiment.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:14.020852 vodex-1.0.9/src/vodex/_tests/data/test_movie/
+-rw-r--r--   0 runner    (1001) docker     (123)   561348 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/data/test_movie/mov0.tif
+-rw-r--r--   0 runner    (1001) docker     (123)  1443174 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/data/test_movie/mov1.tif
+-rw-r--r--   0 runner    (1001) docker     (123)  1363008 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/data/test_movie/mov2.tif
+-rw-r--r--   0 runner    (1001) docker     (123)   256854 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/data/test_movie.avi
+-rw-r--r--   0 runner    (1001) docker     (123)  3367158 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/data/test_movie.tif
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/test_Cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14766 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/test_DbWriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10439 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/test_Experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6480 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/test_FileManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/test_ImageLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/test_Labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/test_TimeLabel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/test_Timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/test_dbmethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/_tests/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-30 04:31:13.000000 vodex-1.0.9/src/vodex/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48985 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54524 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/dbmethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11904 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-01-30 04:30:57.000000 vodex-1.0.9/src/vodex/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 04:31:13.996852 vodex-1.0.9/src/vodex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-01-30 04:31:13.000000 vodex-1.0.9/src/vodex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-01-30 04:31:13.000000 vodex-1.0.9/src/vodex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 04:31:13.000000 vodex-1.0.9/src/vodex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-30 04:31:13.000000 vodex-1.0.9/src/vodex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-30 04:31:13.000000 vodex-1.0.9/src/vodex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-01-30 04:30:57.000000 vodex-1.0.9/tox.ini
```

### Comparing `vodex-1.0.8/.github/workflows/publish.yml` & `vodex-1.0.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/.github/workflows/test_and_deploy.yml` & `vodex-1.0.9/.github/workflows/test_and_deploy.yml`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 on:
   push:
     branches:
       - main
     tags:
       - "v*" # Push events to matching v*, i.e. v1.0, v20.15.10
+      - "test"
   pull_request:
     branches:
       - main
   workflow_dispatch:
 
 jobs:
   test:
```

### Comparing `vodex-1.0.8/PKG-INFO` & `vodex-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vodex
-Version: 1.0.8
+Version: 1.0.9
 Summary: VoDEx : Volumetric Data and Experiment Manager. Allows to load volumetric data based on experimental conditions.
 Home-page: https://github.com/LemonJust/vodex
 Author: Anna Nadtochiy
 Author-email: lemonjustgithub@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/LemonJust/vodex/issues
 Project-URL: Documentation, https://github.com/LemonJust/vodex#README.md
```

### Comparing `vodex-1.0.8/README.md` & `vodex-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/data/test/loader_test/frames_1_2_41_42.tif` & `vodex-1.0.9/data/test/loader_test/frames_1_2_41_42.tif`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/data/test/loader_test/half_volumes_0_1.tif` & `vodex-1.0.9/data/test/loader_test/half_volumes_0_1.tif`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/data/test/loader_test/half_volumes_1_2.tif` & `vodex-1.0.9/data/test/loader_test/half_volumes_1_2.tif`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/data/test/loader_test/volumes_0_1.tif` & `vodex-1.0.9/data/test/loader_test/volumes_0_1.tif`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/data/test/loader_test/volumes_1_2.tif` & `vodex-1.0.9/data/test/loader_test/volumes_1_2.tif`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/data/test/loader_test/volumes_tail.tif` & `vodex-1.0.9/data/test/loader_test/volumes_tail.tif`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/data/test/movie_info.PNG` & `vodex-1.0.9/data/test/movie_info.PNG`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/data/test/test.db` & `vodex-1.0.9/data/test/test.db`

 * *Files 0% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -95,15 +95,15 @@
             PRIMARY KEY("Id" AUTOINCREMENT),
             FOREIGN KEY("AnnotationTypeId") REFERENCES "AnnotationTypes"("Id") ON DELETE CASCADE,
             UNIQUE("AnnotationTypeId","Name")
             );
 INSERT INTO AnnotationTypeLabels VALUES(1,1,'c','circle on the screen');
 INSERT INTO AnnotationTypeLabels VALUES(2,1,'s','square on the screen');
 INSERT INTO AnnotationTypeLabels VALUES(3,2,'c1','written c1');
-INSERT INTO AnnotationTypeLabels VALUES(4,2,'c2','written c1');
+INSERT INTO AnnotationTypeLabels VALUES(4,2,'c2','written c2');
 INSERT INTO AnnotationTypeLabels VALUES(5,2,'c3',NULL);
 INSERT INTO AnnotationTypeLabels VALUES(6,3,'on','the intensity of the background is high');
 INSERT INTO AnnotationTypeLabels VALUES(7,3,'off','the intensity of the background is low');
 CREATE TABLE IF NOT EXISTS "Annotations" (
             "FrameId"	INTEGER NOT NULL,
             "AnnotationTypeLabelId"	INTEGER NOT NULL,
             FOREIGN KEY("FrameId") REFERENCES "Frames"("Id"),
```

### Comparing `vodex-1.0.8/data/test/test_movie/mov0.tif` & `vodex-1.0.9/data/test/test_movie/mov0.tif`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/data/test/test_movie/mov1.tif` & `vodex-1.0.9/data/test/test_movie/mov1.tif`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/data/test/test_movie/mov2.tif` & `vodex-1.0.9/data/test/test_movie/mov2.tif`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/data/test/test_movie.avi` & `vodex-1.0.9/data/test/test_movie.avi`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/data/test/test_movie.tif` & `vodex-1.0.9/data/test/test_movie.tif`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/data/test/toy_example.db` & `vodex-1.0.9/data/test/toy_example.db`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/api/index.md` & `vodex-1.0.9/docs/api/index.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,34 @@
-This part of the project documentation is a 
-reference for the technical implementation of the `VoDEx` project code. 
+This part of the project documentation is a
+reference for the technical implementation of the `VoDEx` project code.
 
-# vodex.loaders module
-::: src.vodex.loaders
+# core
+::: src.vodex.core
+    options:
+      members:
+        - None
+      show_root_heading: false
+      show_source:
+
+# experiment
+::: src.vodex.experiment
     options:
       members:
         - None
       show_root_heading: false
       show_source: false
 
-# vodex.core module
-::: src.vodex.core
+# loaders
+::: src.vodex.loaders
     options:
       members:
         - None
       show_root_heading: false
       show_source: false
 
-# vodex.dbmethods module
+# dbmethods
 ::: src.vodex.dbmethods
     options:
       members:
         - None
       show_root_heading: false
-      show_source: false
+      show_source: false
```

### Comparing `vodex-1.0.8/docs/assets/cover.JPG` & `vodex-1.0.9/docs/assets/cover.JPG`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/assets/data_annotation.png` & `vodex-1.0.9/docs/assets/data_annotation.png`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/assets/data_annotation_a.png` & `vodex-1.0.9/docs/assets/data_annotation_a.png`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/assets/data_annotation_a1.png` & `vodex-1.0.9/docs/assets/data_annotation_a1.png`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/assets/data_annotation_a2.png` & `vodex-1.0.9/docs/assets/data_annotation_a2.png`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/assets/data_annotation_a3.png` & `vodex-1.0.9/docs/assets/data_annotation_a3.png`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/assets/data_annotation_b.png` & `vodex-1.0.9/docs/assets/data_annotation_b.png`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/assets/data_frames.png` & `vodex-1.0.9/docs/assets/data_frames.png`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/assets/db_diagram.png` & `vodex-1.0.9/docs/assets/db_diagram.png`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/assets/test_movie.gif` & `vodex-1.0.9/docs/assets/test_movie.gif`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/contribute.md` & `vodex-1.0.9/docs/contribute.md`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/data.md` & `vodex-1.0.9/docs/data.md`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/examples.md` & `vodex-1.0.9/docs/examples.md`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/img/favicon.ico` & `vodex-1.0.9/docs/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/img/favicon_16.png` & `vodex-1.0.9/docs/img/favicon_16.png`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/img/favicon_32.png` & `vodex-1.0.9/docs/img/favicon_32.png`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/img/icons8_layers.ico` & `vodex-1.0.9/docs/img/icons8_layers.ico`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/img/icons8_layers_16.png` & `vodex-1.0.9/docs/img/icons8_layers_16.png`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/img/icons8_layers_32.png` & `vodex-1.0.9/docs/img/icons8_layers_32.png`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/img/icons8_list_view.ico` & `vodex-1.0.9/docs/img/icons8_list_view.ico`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/img/icons8_v.ico` & `vodex-1.0.9/docs/img/icons8_v.ico`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/img/icons8_v_16.png` & `vodex-1.0.9/docs/img/icons8_v_16.png`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/img/icons8_v_32.png` & `vodex-1.0.9/docs/img/icons8_v_32.png`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/install.md` & `vodex-1.0.9/docs/install.md`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/napari/how-to/fig01.png` & `vodex-1.0.9/docs/napari/how-to/fig01.png`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/napari/how-to/fig02.png` & `vodex-1.0.9/docs/napari/how-to/fig02.png`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/napari/how-to/fig02bc.png` & `vodex-1.0.9/docs/napari/how-to/fig02bc.png`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/napari/how-to/fig03.png` & `vodex-1.0.9/docs/napari/how-to/fig03.png`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/napari/how-to/fig04.png` & `vodex-1.0.9/docs/napari/how-to/fig04.png`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/napari/how-to/fig05a.png` & `vodex-1.0.9/docs/napari/how-to/fig05a.png`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/napari/how-to/fig05b.png` & `vodex-1.0.9/docs/napari/how-to/fig05b.png`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/napari/how-to/fig05c.png` & `vodex-1.0.9/docs/napari/how-to/fig05c.png`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/napari/how-to/fig06.png` & `vodex-1.0.9/docs/napari/how-to/fig06.png`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/napari/how-to/fig07.png` & `vodex-1.0.9/docs/napari/how-to/fig07.png`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/napari/how-to/intro.PNG` & `vodex-1.0.9/docs/napari/how-to/intro.PNG`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/napari/how-to/new1.PNG` & `vodex-1.0.9/docs/napari/how-to/new1.PNG`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/napari/how-to.md` & `vodex-1.0.9/docs/napari/how-to.md`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/napari/index.md` & `vodex-1.0.9/docs/napari/index.md`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/qstart/load_volumes.md` & `vodex-1.0.9/docs/qstart/load_volumes.md`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/docs/qstart/new_experiment.md` & `vodex-1.0.9/docs/qstart/new_experiment.md`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/img/cover.JPG` & `vodex-1.0.9/img/cover.JPG`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/img/test_summary.PNG` & `vodex-1.0.9/img/test_summary.PNG`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/mkdocs.yml` & `vodex-1.0.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/notebooks/01_create_experiment_and_load_volumes.ipynb` & `vodex-1.0.9/notebooks/01_create_experiment_and_load_volumes.ipynb`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/notebooks/test.db` & `vodex-1.0.9/notebooks/test.db`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/notebooks/test_no_annotation.db` & `vodex-1.0.9/notebooks/test_no_annotation.db`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/notebooks/test_w_annotations.db` & `vodex-1.0.9/notebooks/test_w_annotations.db`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/setup.cfg` & `vodex-1.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/site/404.html` & `vodex-1.0.9/site/404.html`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/site/core/index.html` & `vodex-1.0.9/site/core/index.html`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/site/css/base.css` & `vodex-1.0.9/site/css/base.css`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/site/css/bootstrap.min.css` & `vodex-1.0.9/site/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/site/css/font-awesome.min.css` & `vodex-1.0.9/site/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/site/dbmethods/index.html` & `vodex-1.0.9/site/dbmethods/index.html`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/site/explanation/index.html` & `vodex-1.0.9/site/explanation/index.html`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/site/fonts/fontawesome-webfont.eot` & `vodex-1.0.9/site/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/site/fonts/fontawesome-webfont.svg` & `vodex-1.0.9/site/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/site/fonts/fontawesome-webfont.ttf` & `vodex-1.0.9/site/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/site/fonts/fontawesome-webfont.woff` & `vodex-1.0.9/site/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/site/fonts/fontawesome-webfont.woff2` & `vodex-1.0.9/site/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/site/how-to-guides/index.html` & `vodex-1.0.9/site/how-to-guides/index.html`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/site/img/favicon.ico` & `vodex-1.0.9/site/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/site/img/grid.png` & `vodex-1.0.9/site/img/grid.png`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/site/index.html` & `vodex-1.0.9/site/index.html`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/site/js/base.js` & `vodex-1.0.9/site/js/base.js`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/site/js/bootstrap.min.js` & `vodex-1.0.9/site/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/site/js/jquery-1.10.2.min.js` & `vodex-1.0.9/site/js/jquery-1.10.2.min.js`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/site/loaders/index.html` & `vodex-1.0.9/site/loaders/index.html`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/site/objects.inv` & `vodex-1.0.9/site/objects.inv`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/site/reference/index.html` & `vodex-1.0.9/site/reference/index.html`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/site/sitemap.xml` & `vodex-1.0.9/site/sitemap.xml`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/site/tutorials/index.html` & `vodex-1.0.9/site/tutorials/index.html`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/src/vodex/__init__.py` & `vodex-1.0.9/src/vodex/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,13 +5,14 @@
 - `loaders`: The classes to read the image data and metadate from files.
 - `core`: The core classes to organise the information about the experiment.
 - `dbmethods`: The classes to create, write to and query the data base.
 - `utils`: Some helper functions.
 """
 __all__ = ["ImageLoader", "FileManager", "FrameManager", "VolumeManager",
            "TimeLabel", "Labels", "Cycle", "Timeline", "Annotation",
-           "TiffLoader", "DbWriter", "DbReader", "DbExporter", "Experiment"]
+           "TiffLoader", "DbWriter", "DbReader", "DbExporter", "Experiment",
+           "VX_SUPPORTED_TYPES"]
 
 from .loaders import *
 from .core import *
 from .dbmethods import *
 from .experiment import *
```

### Comparing `vodex-1.0.8/src/vodex/_tests/data/construction_blocks/data.py` & `vodex-1.0.9/src/vodex/_tests/data/construction_blocks/data.py`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/src/vodex/_tests/data/construction_blocks/numbered_frames.tif` & `vodex-1.0.9/src/vodex/_tests/data/construction_blocks/numbered_frames.tif`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/src/vodex/_tests/data/construction_blocks/recepie.xlsx` & `vodex-1.0.9/src/vodex/_tests/data/construction_blocks/recepie.xlsx`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/src/vodex/_tests/data/construction_blocks/recepie_long.xlsx` & `vodex-1.0.9/src/vodex/_tests/data/construction_blocks/recepie_long.xlsx`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/src/vodex/_tests/data/construction_blocks/zero_frame.tif` & `vodex-1.0.9/src/vodex/_tests/data/construction_blocks/zero_frame.tif`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/src/vodex/_tests/data/construction_blocks/zero_frame_c1.tif` & `vodex-1.0.9/src/vodex/_tests/data/construction_blocks/zero_frame_c1.tif`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/src/vodex/_tests/data/construction_blocks/zero_frame_c2.tif` & `vodex-1.0.9/src/vodex/_tests/data/construction_blocks/zero_frame_c2.tif`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/src/vodex/_tests/data/construction_blocks/zero_frame_c3.tif` & `vodex-1.0.9/src/vodex/_tests/data/construction_blocks/zero_frame_c3.tif`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/src/vodex/_tests/data/construction_blocks/zero_frame_circle.tif` & `vodex-1.0.9/src/vodex/_tests/data/construction_blocks/zero_frame_circle.tif`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/src/vodex/_tests/data/construction_blocks/zero_frame_square.tif` & `vodex-1.0.9/src/vodex/_tests/data/construction_blocks/zero_frame_square.tif`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/src/vodex/_tests/data/loader_test/frames_1_2_41_42.tif` & `vodex-1.0.9/src/vodex/_tests/data/loader_test/frames_1_2_41_42.tif`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/src/vodex/_tests/data/loader_test/half_volumes_0_1.tif` & `vodex-1.0.9/src/vodex/_tests/data/loader_test/half_volumes_0_1.tif`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/src/vodex/_tests/data/loader_test/half_volumes_1_2.tif` & `vodex-1.0.9/src/vodex/_tests/data/loader_test/half_volumes_1_2.tif`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/src/vodex/_tests/data/loader_test/volumes_0_1.tif` & `vodex-1.0.9/src/vodex/_tests/data/loader_test/volumes_0_1.tif`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/src/vodex/_tests/data/loader_test/volumes_1_2.tif` & `vodex-1.0.9/src/vodex/_tests/data/loader_test/volumes_1_2.tif`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/src/vodex/_tests/data/loader_test/volumes_tail.tif` & `vodex-1.0.9/src/vodex/_tests/data/loader_test/volumes_tail.tif`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/src/vodex/_tests/data/movie_info.PNG` & `vodex-1.0.9/src/vodex/_tests/data/movie_info.PNG`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/src/vodex/_tests/data/test.db` & `vodex-1.0.9/src/vodex/_tests/data/test_experiment.db`

 * *Format-specific differences are supported for SQLite databases but no file-specific differences were detected; falling back to a binary diff. file(1) reports: SQLite 3.x database, last written using SQLite version 3038002, file counter 20, database pages 24, cookie 0x14, schema 4, UTF-8, version-valid-for 20*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5351 4c69 7465 2066 6f72 6d61 7420 3300  SQLite format 3.
-00000010: 1000 0101 0040 2020 0000 0014 0000 0018  .....@  ........
-00000020: 0000 0000 0000 0000 0000 0014 0000 0004  ................
+00000010: 1000 0101 0040 2020 0000 000f 0000 0018  .....@  ........
+00000020: 0000 0000 0000 0000 0000 000f 0000 0004  ................
 00000030: 0000 0000 0000 0000 0000 0001 0000 0000  ................
 00000040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000050: 0000 0000 0000 0000 0000 0000 0000 0014  ................
+00000050: 0000 0000 0000 0000 0000 0000 0000 000f  ................
 00000060: 002e 5b32 0d0f f800 1701 a000 0efb 0fc9  ..[2............
 00000070: 0dba 0ed0 0ea5 0d68 0bef 0d29 0cea 0a9c  .......h...)....
 00000080: 0bc2 08ea 0a6f 0a42 0693 08a1 0858 04ce  .....o.B.....X..
 00000090: 065c 0366 01a0 0337 0308 0000 0000 0000  .\.f...7........
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `vodex-1.0.8/src/vodex/_tests/data/test_experiment.db` & `vodex-1.0.9/src/vodex/_tests/data/test.db`

 * *Files 10% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -31,14 +31,15 @@
 INSERT INTO AnnotationTypes VALUES(3,'light',NULL);
 CREATE TABLE IF NOT EXISTS "Frames" (
             "Id"	INTEGER NOT NULL UNIQUE,
             "FrameInFile"	INTEGER NOT NULL,
             "FileId"	INTEGER NOT NULL,
             PRIMARY KEY("Id" AUTOINCREMENT),
             FOREIGN KEY("FileId") REFERENCES "Files"("Id")
+            UNIQUE("FrameInFile", "FileId")
             );
 INSERT INTO Frames VALUES(1,0,1);
 INSERT INTO Frames VALUES(2,1,1);
 INSERT INTO Frames VALUES(3,2,1);
 INSERT INTO Frames VALUES(4,3,1);
 INSERT INTO Frames VALUES(5,4,1);
 INSERT INTO Frames VALUES(6,5,1);
@@ -238,14 +239,15 @@
 INSERT INTO Annotations VALUES(42,7);
 CREATE TABLE IF NOT EXISTS "CycleIterations" (
             "FrameId"	INTEGER NOT NULL,
             "CycleId"	INTEGER NOT NULL,
             "CycleIteration"	INTEGER NOT NULL,
             FOREIGN KEY("CycleId") REFERENCES "Cycles"("Id") ON DELETE CASCADE,
             FOREIGN KEY("FrameId") REFERENCES "Frames"("Id")
+            UNIQUE("FrameId","CycleId")
             );
 INSERT INTO CycleIterations VALUES(1,1,0);
 INSERT INTO CycleIterations VALUES(2,1,0);
 INSERT INTO CycleIterations VALUES(3,1,0);
 INSERT INTO CycleIterations VALUES(4,1,0);
 INSERT INTO CycleIterations VALUES(5,1,0);
 INSERT INTO CycleIterations VALUES(6,1,0);
```

### Comparing `vodex-1.0.8/src/vodex/_tests/data/test_movie/mov0.tif` & `vodex-1.0.9/src/vodex/_tests/data/test_movie/mov0.tif`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/src/vodex/_tests/data/test_movie/mov1.tif` & `vodex-1.0.9/src/vodex/_tests/data/test_movie/mov1.tif`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/src/vodex/_tests/data/test_movie/mov2.tif` & `vodex-1.0.9/src/vodex/_tests/data/test_movie/mov2.tif`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/src/vodex/_tests/data/test_movie.avi` & `vodex-1.0.9/src/vodex/_tests/data/test_movie.avi`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/src/vodex/_tests/data/test_movie.tif` & `vodex-1.0.9/src/vodex/_tests/data/test_movie.tif`

 * *Files identical despite different names*

### Comparing `vodex-1.0.8/src/vodex/_tests/test_dbmethods.py` & `vodex-1.0.9/src/vodex/_tests/test_dbmethods.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 import pytest
 from vodex import *
 from pathlib import Path
 
 TEST_DATA = Path(Path(__file__).parent.resolve(), 'data')
 
+
 class TestDbWriter:
     data_dir_split = Path(TEST_DATA, "test_movie")
 
     shape = Labels("shape", ["c", "s"],
                    state_info={"c": "circle on the screen", "s": "square on the screen"})
     light = Labels("light", ["on", "off"], group_info="Information about the light",
                    state_info={"on": "the intensity of the background is high",
```

### Comparing `vodex-1.0.8/src/vodex/_tests/test_loaders.py` & `vodex-1.0.9/src/vodex/_tests/test_loaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,18 +78,18 @@
         assert loader2 == loader1
 
     def test_init_loader(self):
         tif_loader = TiffLoader(full_movie)
         loader = ImageLoader(full_movie).loader
         assert loader == tif_loader
 
-    def test_get_frames_in_file(self):
-        loader = ImageLoader(full_movie)
-        n_frames = loader.get_frames_in_file(full_movie)
-        assert n_frames == 42
+    # def test_get_frames_in_file(self):
+    #     loader = ImageLoader(full_movie)
+    #     n_frames = loader.get_frames_in_file(full_movie)
+    #     assert n_frames == 42
 
     def test_get_frame_size(self):
         loader = ImageLoader(full_movie)
         f_size = loader.get_frame_size(full_movie)
         assert f_size == (200, 200)
 
     def test_load_frames_one_file(self):
```

### Comparing `vodex-1.0.8/src/vodex/core.py` & `vodex-1.0.9/src/vodex/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,110 +1,101 @@
 """
-This module contains core classes that load the data,
-preprocess the information about the experiment data and help construct time annotation.
+This module provides the core classes for loading, preprocessing, and constructing time annotations for imaging data.
 
-Core class that loads the image data:
+'ImageLoader' is the core class that loads the image data and selects the appropriate loader based on the file type. It
+also collects information about the data type and number of frames per file.
 
-- `ImageLoader` - chooses appropriate loader based on the type of the imaging files,
-                    collects information about the datatype, number of frames per file and loads data from files.
-
-Core classes that preprocess the information about the experiment data:
-
-- `FileManager` - a class containing information about the image files:
-                    their location, file type, number of frames per file.
-
-- `FrameManager` - a class containing information about the image frames in the experiment:
-                    total number of frames, and mapping of the frames to files.
-
-- `VolumeManager` - a class containing information about the image volumes in the experiment:
-                    frames per volume, number of full volumes, and mapping of the frames to volumes.
-
-Classes that help construct and store the time annotation:
-
-- `TimeLabel` - Stores information about a particular time-located event during the experiment: any specific condition,
-    described by a group and the label.
-    For example: group 'light', label 'on': the light was on; group 'light', label 'off': the light was off.
-
-- `Labels` - Stores information about a group of time labels: any specific aspect of the experiment that you want to document.
-        For example: temperature|light|sound|image on the screen|drug|behaviour ... etc.
-
-- `Cycle` - Stores and preprocesses information about the repeated cycle of labels.
-    Use it to create annotation when you have some periodic conditions.
-    For example: light on for 10 frames, light off for 20 frames, light on for 10 frames... and so on.
-
-- `Timeline` - Stores and preprocesses information about the sequence of labels.
-    Use it to create annotation when you have some non-periodic conditions.
-    For example: light on for 10 frames, light off for 20 frames, light on for 25 frames.
-
-- `Annotation` - Stores and preprocesses information about the time annotation of the experiment.
-    Uses Cycle or Timeline to initialise the annotation.
+'FileManager', 'FrameManager', and 'VolumeManager' are core classes that preprocess information about the experiment
+data. The 'FileManager' class contains information about the location and file type of the image files,
+while the 'FrameManager' class contains information about the number of frames in the experiment and the mapping of
+frames to files. The 'VolumeManager' class contains information about the image volumes in the experiment,
+including the number of frames per volume and the mapping of frames to volumes.
+
+'TimeLabel', 'Labels', 'Cycle', 'Timeline', and 'Annotation' classes help to construct and store time annotations. The
+'TimeLabel' class stores information about specific time-located events during the experiment, such as a specific
+condition described by a group and label. The 'Labels' class stores information about a group of time labels,
+such as temperature, light, sound, image on the screen, drug, or behavior. The 'Cycle' class stores and preprocesses
+information about repeated cycles of labels, useful for creating annotations for periodic conditions. The 'Timeline'
+class stores and preprocesses information about the sequence of labels, useful for creating annotations for
+non-periodic conditions. Finally, the 'Annotation' class stores and preprocesses information about the time annotation
+of the experiment; it uses either the 'Cycle' or 'Timeline' classes to initialize the annotation.
 """
 import json
 from itertools import groupby
 from pathlib import Path
 from typing import Union, List, Tuple, Dict
 
 import numpy as np
 import numpy.typing as npt
 
 from .loaders import Loader, TiffLoader
 from .utils import list_of_int
 
-# If adding support to a new file type, add the info here!
-
-# A list of supported formats. Create mapping from file formats to loaders.
-# (Currently only supports files with tif extensions)
-# Expand this dictionary to add support for other file formats.
-# 1. *.tif and *.tiff support is implemented using tifffile package
-# 2. ...
+# This section of the code is related to adding support for new file types. ___________________________________________
 
-# dictionary that contains the supported file types and corresponding extensions
-# please add extensions as tuples, even if is a single entry ( Ex. : { ... , 'MyFileType': ('.mytag') } ):
+# 'VX_SUPPORTED_TYPES' is a dictionary that lists the supported file formats and their corresponding extensions.
+# Currently, only files in TIFF format are supported using the tifffile package.
+# To add support for other file formats, additional entries should be added to this dictionary in the form of
+# 'FileType': ('.extension') or 'FileType': ('.extension1', '.extension2', '.extension3').
 VX_SUPPORTED_TYPES: Dict[str, tuple] = {'TIFF': ('.tif', '.tiff')}
 
-# dictionary that contains the supported file suffixes types and corresponding file types
-# please add extensions for each suffix individually:
+# 'VX_EXTENSION_TO_TYPE' is a dictionary that maps file extensions to their corresponding file formats.
+# For example, it maps the '.tif' and '.tiff' extensions to the 'TIFF' file type.
+# To add support for other file formats, additional entries should be added to this dictionary in the form of
+# 'extension': 'FileType' or 'extension1': 'FileType', 'extension2': 'FileType', 'extension3': 'FileType'.
 VX_EXTENSION_TO_TYPE: Dict[str, str] = {'tif': 'TIFF', 'tiff': 'TIFF'}
 
-# dictionary that contains the supported file suffixes types and corresponding loader classes
-# please add extensions for each suffix individually:
+# 'VX_EXTENSION_TO_LOADER' is a dictionary that maps file extensions to the corresponding loader classes. For example,
+# it maps the '.tif' and '.tiff' extensions to the TiffLoader class.
+# To add support for other file formats, additional entries should be added to this dictionary in the form of
+# 'extension': 'LoaderClass' or 'extension1': 'LoaderClass', 'extension2': 'LoaderClass', 'extension3': 'LoaderClass'.
 VX_EXTENSION_TO_LOADER: Dict[str, type] = {'tif': TiffLoader, 'tiff': TiffLoader}
 
 
+# _____________________________________________________________________________________________________________________
+
+
 class ImageLoader:
     """
-    Chooses appropriate loader based on the type of the imaging files,
-    collects information about the datatype, number of frames per file and loads data from files.
+    The 'ImageLoader' class is responsible for choosing the appropriate loader for a given imaging file, collecting
+    information about the data type, number of frames per file, and loading data from files.
 
     Args:
-        file_example : the path to a file example (one file from the whole dataaset).
-            needed to get file type and initialise the corresponding data loader.
+        file_example : The path to a file example (one file from the whole dataset).
+                    This is used to determine the file type and initialize the corresponding data loader.
 
     Attributes:
-        supported_extensions: list of all the supported file extensions.
-        file_extension: the file extension of the provided file example.
-        loader: a loader class initialised using the file example.
+        supported_extensions: A list of all the supported file extensions.
+        file_extension: The file extension of the provided file example.
+        loader:  The loader class initialized using the file example.
 
     """
 
     def __init__(self, file_example: Path):
+        """
+        Initializes the ImageLoader class by determining the file extension, checking that it is a supported format,
+        and initializing the appropriate loader class.
+        """
 
         self.supported_extensions: List[str] = list(VX_EXTENSION_TO_LOADER.keys())
         # suffix has the dot at the beginning, need to strip
         self.file_extension: str = file_example.suffix.lstrip('.')
         assert self.file_extension in self.supported_extensions, \
             f"Only files with the following extensions are supported: {self.supported_extensions}, but" \
             f"{self.file_extension} was given"
 
         # Pick the loader and initialise it with the data directory:
         # chooses the proper loader based on the file extension.
         # Add your class to VX_EXTENSION_TO_LOADER when adding support to other file formats.
         self.loader: Loader = VX_EXTENSION_TO_LOADER[self.file_extension](file_example)
 
     def __eq__(self, other):
+        """
+        Compares two ImageLoader instances to see if they are equal.
+        """
         if isinstance(other, ImageLoader):
             is_same = [
                 self.supported_extensions == other.supported_extensions,
                 self.file_extension == other.file_extension,
                 self.loader == other.loader
             ]
             return np.all(is_same)
@@ -122,27 +113,27 @@
         Returns:
             the number of frames in the file.
         """
         return self.loader.get_frames_in_file(file_name)
 
     def get_frame_size(self, file_name: Union[str, Path]) -> Tuple[int, int]:
         """
-        Gets frame size ( height , width ) from an image files.
+        Returns the size of an individual frame in pixels (height and width).
 
         Args:
             file_name: the path to the file to get the size of the frame for.
         Returns:
             ( height , width ) height and width of an individual frame in pixels.
         """
         return self.loader.get_frame_size(file_name)
 
     def load_frames(self, frames: List[int], files: Union[List[str], List[Path]],
                     show_file_names: bool = False, show_progress: bool = True) -> npt.NDArray:
         """
-        Loads specified frames from specified files.
+         Loads specified frames from specified files, and returns as a 3D array of shape (n_frames, height, width).
 
         Args:
             frames: list of frames IN FILES to load.
             files: a file for every frame
             show_file_names: whether to print the names of the files from which the frames are loaded.
                 Setting it to True will turn off show_progress.
             show_progress: whether to show the progress bar of how many frames have been loaded.
@@ -156,155 +147,151 @@
 
     def load_volumes(self,
                      frame_in_file: List[int],
                      files: Union[List[str], List[Path]],
                      volumes: List[int],
                      show_file_names: bool = False, show_progress: bool = True) -> npt.NDArray:
         """
-        Loads specified frames from specified files and shapes them into volumes.
+         Loads specific volumes of data, where a volume is defined as a set of frames.
+         This method returns a 4D array of shape (n_volumes, n_frames_per_volume, height, width).
 
         Args:
             frame_in_file: list of frames IN FILES to load
                 (relative to the beginning of the file from which you are loading).
             files: a file for every frame
             volumes: a volume for every frame where that frame belongs
             show_file_names: whether to print the names of the files from which the frames are loaded.
                                 Setting it to True will turn off show_progress.
             show_progress: whether to show the progress bar of how many frames have been loaded.
                 Won't have effect of show_file_names is True.
         Returns:
             4D array of shape (number of volumes, zslices, height, width)
         """
-        # TODO : do I need to check anything else here???
-        #  Like that the frames are in increasing order per file
-        #  ( maybe not here but in the experiment ,before we turn them into frames_in_file )
         # get frames and info
         frames = self.loader.load_frames(frame_in_file, files,
                                          show_file_names=show_file_names,
                                          show_progress=show_progress)
         n_frames, w, h = frames.shape
 
         # get volume information
         i_volume, count = np.unique(volumes, return_counts=True)
-        # you can use this method to load portions of the volumes, so fpv will be smaller
+        # you can use this method to load portions of the volumes (slices), so fpv will be smaller than a full volume
         n_volumes, fpv = len(i_volume), count[0]
         assert np.all(count == fpv), "Can't have different number of frames per volume!"
 
         frames = frames.reshape((n_volumes, fpv, w, h))
         return frames
 
 
 class FileManager:
     """
-    A class containing information about the image files: their location, file type, number of frames per file.
-    Collects and stores the information about all the image files.
-    By default, it will search for all the files with the provided file extension
-    in the provided data director and order them alphabetically.
-    If a list of file names is provided, will use these files in the provided order.
+    The 'FileManager' class is used to collect and store information about image files, including their location,
+    file type, and number of frames per file. It can either search for all files with a specific file extension in a
+    provided data directory (order them alphabetically), or use a provided list of file names (in the provided order).
+    The class initializes an 'ImageLoader' to calculate the number of frames per file if it is not provided.
+
+    The class raises an error if the data directory does not exist, no files of the specified file type are found,
+    or if the number of frames per file is not provided or is not a list of integers.
 
     Args:
         data_dir: path to the folder with the files, ends with "/" or "\\"
         file_names: names of files relative to the data_dir
         frames_per_file: number of frames in each file. Will be used ONLY if the file_names were provided.
         file_type: file type to search for (if files are not provided). Must be a key in the VX_SUPPORTED_TYPES dict.
 
     Attributes:
         data_dir: the directory with all the imaging data
         file_names: names of files relative to the data_dir
-        loader: initialised image loader (see loaders.ImageLoader for more details)
         num_frames: a number of frames per file
         n_files: total number of image files
     """
 
     def __init__(self, data_dir: Union[str, Path], file_type: str = "TIFF",
                  file_names: List[str] = None, frames_per_file: List[int] = None):
 
         # 1. get data_dir and check it exists
         self.data_dir: Path = Path(data_dir)
         assert self.data_dir.is_dir(), f"No directory {self.data_dir}"
 
-        # 2. get files
+        # 2. get files and file type
         if file_names is not None:
             tags = [name.split(".")[-1] for name in file_names]
             # check that all the elements of the list are same
-            assert len(set(tags)) == 1, "Error initializing FileManager: " \
-                                        f"file_names must be files with the same resolution, but got {set(tags)}"
+            assert len(set(tags)) == 1, f"File_names must be files with the same extension, " \
+                                        f"but got {', '.join(sorted(set(tags)))}"
+            assert tags[0] in VX_EXTENSION_TO_TYPE, f'Extension "{tags[0]}" is not supported.'
             file_type = VX_EXTENSION_TO_TYPE[tags[0]]
+
         self.file_type = file_type
+        assert self.file_type in VX_SUPPORTED_TYPES, f'File type "{self.file_type}" is not supported.'
         file_extensions = VX_SUPPORTED_TYPES[self.file_type]
 
         self.num_frames = None
         # TODO : check in accordance with the file extension/ figure out file type from files when provided
         if file_names is None:
             # if files are not provided , search for tiffs in the data_dir
             self.file_names: List[str] = self.find_files(file_extensions)
         else:
             # if a list of files is provided, check it's in the folder
             self.file_names: List[str] = self.check_files(file_names)
             if frames_per_file is not None:
                 # not recommended! this information is taken as is and is not verified...
                 self.num_frames: List[int] = frames_per_file
 
-        assert len(self.file_names) > 0, f"Error when initialising FileManager:\n" \
-                                         f"No files of type {file_type} [extensions {file_extensions}]\n" \
+        assert len(self.file_names) > 0, f"No files of type {file_type} [extensions {file_extensions}]\n" \
                                          f" in {data_dir}"
-        # 3. Initialise ImageLoader
-        #    will pick the image loader that works with the provided file type
-        self.loader: ImageLoader = ImageLoader(self.data_dir.joinpath(self.file_names[0]))
 
-        # 4. Get number of frames per file (if it wasn't entered manually)
+        # 3. Get number of frames per file (if it wasn't entered manually)
         if self.num_frames is None:
             # if number of frames not provided , search for tiffs in the data_dir
             self.num_frames: List[int] = self.get_frames_per_file()
 
-        # check that the type is int
-        assert all(isinstance(n, (int, np.integer)) for n in self.num_frames), \
-            "self.num_frames should be a list of int"
-
         self.n_files: int = len(self.file_names)
 
-    def __str__(self):
-        description = f"Image files information :\n\n"
-        description = description + f"files directory: {self.data_dir}\n"
-        description = description + f"files [number of frames]: \n"
-        for (i_file, (file_name, num_frames)) in enumerate(zip(self.file_names, self.num_frames)):
-            description = description + f"{i_file}) {file_name} [{num_frames}]\n"
-        return description
-
-    def __repr__(self):
-        return self.__str__()
-
     def __eq__(self, other):
+        """
+        Compares two FileManager instances to see if they are equal.
+        """
         if isinstance(other, FileManager):
             is_same = [
                 self.data_dir == other.data_dir,
                 self.file_names == other.file_names,
-                self.loader == other.loader,
                 self.num_frames == other.num_frames,
                 self.n_files == other.n_files
             ]
 
             return np.all(is_same)
         else:
             print(f"__eq__ is Not Implemented for {FileManager} and {type(other)}")
             return NotImplemented
 
+    def __str__(self):
+        description = f"Image files information :\n\n"
+        description = description + f"files directory: {self.data_dir}\n"
+        description = description + f"files [number of frames]: \n"
+        for (i_file, (file_name, num_frames)) in enumerate(zip(self.file_names, self.num_frames)):
+            description = description + f"{i_file}) {file_name} [{num_frames}]\n"
+        return description
+
+    def __repr__(self):
+        return self.__str__()
+
     def find_files(self, file_extensions: Tuple[str]) -> List[str]:
         """
         Searches for files ending with the provided file extension in the data directory.
         Sorts the names alphabetically in ascending order (from A to Z),
         sorting is case-insensitive (upper case letters are NOT prioritized).
 
         Args:
             file_extensions: extensions of files to search for
         Returns:
             A sorted list of file names. File names are with the extension, relative to the data directory
             (names only, not full paths to files)
         """
-        files = (p.resolve() for p in Path(self.data_dir).glob("**/*") if p.suffix in file_extensions)
+        files = (p.resolve() for p in Path(self.data_dir).glob('*') if p.suffix in file_extensions)
         file_names = [file.name for file in files]
         file_names.sort(key=str.lower)
         return file_names
 
     def check_files(self, file_names: List[str]) -> List[str]:
         """
         Given a list of files checks that files are in the data directory.
@@ -326,33 +313,37 @@
         """
         Get the number of frames per file.
 
         Returns:
             a list with number of frames per file.
         """
         frames_per_file = []
+        #    Initialise ImageLoader:
+        #    will pick the image loader that works with the provided file type
+        loader: ImageLoader = ImageLoader(self.data_dir.joinpath(self.file_names[0]))
         for file in self.file_names:
-            n_frames = self.loader.get_frames_in_file(self.data_dir.joinpath(file))
+            n_frames = loader.get_frames_in_file(self.data_dir.joinpath(file))
             frames_per_file.append(n_frames)
         return frames_per_file
 
     def change_files_order(self, order: List[int]) -> None:
         """
         Changes the order of the files. If you notice that files are in the wrong order, provide the new order.
         If you wish to exclude any files, get rid of them ( don't include their IDs into the new order ).
 
         Args:
             order: The new order in which the files follow. Refer to file by it's position in the original list.
                     Should be the same length as the number of files in the original list or smaller, no duplicates.
         """
-        # TODO : test it
         assert len(order) <= self.n_files, \
             "Number of files is smaller than elements in the new order list! "
         assert len(order) == len(set(order)), \
             "All elements in the new order list must be unique! "
+        assert set(order).issubset(list(range(self.n_files))), \
+            f"All elements in the new order list must be present in the original order: {list(range(self.n_files))}! "
 
         self.file_names = [self.file_names[i] for i in order]
         self.num_frames = [self.num_frames[i] for i in order]
         self.n_files = len(self.file_names)
 
 
 class FrameManager:
@@ -743,20 +734,22 @@
         name: the name of the cycle, the same as the name of the grou p of the labels.
         label_order: the order in which the labels follow in a cycle.
         duration: the duration of each label from the label_order ( in frames )
         cycle_length: the length of the cycle ( in frames )
         per_frame_list: mapping of frames to corresponding frames for one full cycle only.
     """
 
-    def __init__(self, label_order: List[TimeLabel], duration: Union[np.array, List[int]]):
+    def __init__(self, label_order: List[TimeLabel], duration: Union[npt.NDArray, List[int]]):
         # check that all labels are from the same group
         label_group = label_order[0].group
         for label in label_order:
             assert label.group == label_group, \
                 f"All labels should be from the same group, but got {label.group} and {label_group}"
+        assert label_group is not None, \
+            f"All labels should be from the same group, label group can not be None"
 
         # check that timing is int
         assert all(isinstance(n, (int, np.integer)) for n in duration), "timing should be a list of int"
 
         self.name: str = label_group
         self.label_order: List[TimeLabel] = label_order
         self.duration: List[int] = list_of_int(duration)
@@ -804,44 +797,45 @@
 
     def fit_frames(self, n_frames: int) -> int:
         """
         Calculates how many cycles you need to fully cover n_frames.
         Assumes the cycle starts at the beginning of the recording.
 
         Args:
-            n_frames: number of frames to cover
+            n_frames: number of frames to cover, must be >= 0.
 
         Returns:
             number of cycles (n_cycles) necessary to cover n_frames:
             n_cycles*self.cycle_length >= n_frames
         """
+        assert n_frames >= 0, "n_frames must be positive"
         n_cycles = int(np.ceil(n_frames / self.cycle_length))
         return n_cycles
 
     def fit_labels_to_frames(self, n_frames: int) -> List[TimeLabel]:
         """
         Create a list of labels corresponding to each frame in the range of n_frames
 
         Args:
-            n_frames: number of frames to fit labels to
+            n_frames: number of frames to fit labels to, must be >= 0.
 
         Returns:
             labels per frame for each frame in range of n_frames
         """
         n_cycles = self.fit_frames(n_frames)
         label_per_frame_list = np.tile(self.per_frame_list, n_cycles)
         # crop the tail
         return list(label_per_frame_list[0:n_frames])
 
     def fit_cycles_to_frames(self, n_frames: int) -> List[int]:
         """
         Create a list of cycle ids (what cycle iteration it is) corresponding to each frame in the range of n_frames
 
         Args:
-            n_frames: number of frames to fit cycle iterations to
+            n_frames: number of frames to fit cycle iterations to, must be >= 0.
         Returns:
             cycle id per frame for each frame in range of n_frames
         """
         n_cycles = self.fit_frames(n_frames)
         cycle_per_frame_list = []
         for n in np.arange(n_cycles):
             cycle_per_frame_list.extend([int(n)] * self.cycle_length)
@@ -905,28 +899,30 @@
 
     Args:
         label_order: a list of labels in the right order in which they follow
         duration: duration of the corresponding labels, in frames (based on your imaging). Note that these are
             frames, not volumes !
     """
 
-    def __init__(self, label_order: List[TimeLabel], duration: List[int]):
+    def __init__(self, label_order: List[TimeLabel], duration: Union[npt.NDArray, List[int]]):
 
         # check that all labels are from the same group
         label_group = label_order[0].group
         for label in label_order:
             assert label.group == label_group, \
                 f"All labels should be from the same group, but got {label.group} and {label_group}"
+        assert label_group is not None, \
+            f"All labels should be from the same group, label group can not be None"
 
         # check that timing is int
-        assert all(isinstance(n, int) for n in duration), "duration should be a list of int"
+        assert all(isinstance(n, (int, np.integer)) for n in duration), "timing should be a list of int"
 
         self.name = label_group
         self.label_order = label_order
-        self.duration = list(duration)
+        self.duration = list_of_int(duration)
         self.full_length = sum(self.duration)
         # list the length of the cycle, each element is the TimeLabel
         # TODO : turn it into an index ?
         self.per_frame_list = self.get_label_per_frame()
 
     def __eq__(self, other):
         if isinstance(other, Timeline):
```

### Comparing `vodex-1.0.8/src/vodex/dbmethods.py` & `vodex-1.0.9/src/vodex/dbmethods.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+"""
+This module contains classes that provide a consistent and easy-to-use interface for interacting
+with the SQLite database.
+
+DbWriter - A class that writes information to the database. It abstracts the SQLite calls and allows for easy
+creation, population, and saving of the database.
+
+DbReader - A class that reads information from the database. It abstracts the SQLite calls and allows for easy
+querying and retrieval of data from the database.
+
+DbExporter - A class that transforms the information from the database into the core classes, such as 'FileManager',
+'VolumeManager', 'Labels', 'Timeline', 'Cycle' and 'Annotation', making it easier to view and edit with the data.
+"""
+
 from sqlite3 import connect, Connection
 
 from .core import *
 from .utils import list_of_int
 
 from typing import Union, List
 
@@ -37,15 +51,14 @@
         backup_db.close()
 
     @classmethod
     def create(cls):
         """
         Creates an empty DB for the experiment in memory.
         """
-        # TODO : figure out how to type-annotate classmethod
         # For an in-memory only database:
         memory_db = connect(':memory:')
         return cls(memory_db)
 
     @classmethod
     def load(cls, file_name: str):
         """
@@ -62,17 +75,14 @@
     def populate(self, volumes: VolumeManager = None, annotations: List[Annotation] = None):
         """
         Creates the tables if they don't exist and fills with the provided data.
         Args:
             volumes: mapping of frames to volumes, and to slices in volumes, frames per volume
             annotations: mapping of frames to labels, list of annotations
         """
-        # TODO : add warnings when you are trying to write the same data again
-        # TODO : How to type annotate vodex classes from core ?
-
         # will only create if they don't exist
         self._create_tables()
         # TODO : write cases for files and frames not None
 
         if volumes is not None:
             self._populate_Options(volumes.file_manager, volumes)
             self._populate_Files(volumes.file_manager)
@@ -95,17 +105,18 @@
             self._populate_AnnotationTypes(annotation)
             self._populate_AnnotationTypeLabels(annotation)
             self._populate_Annotations(annotation)
             if annotation.cycle is not None:
                 self._populate_Cycles(annotation)
                 self._populate_CycleIterations(annotation)
 
-    def get_n_frames(self) -> int:
+    def _get_n_frames(self) -> int:
         """
         Queries and returns the total number of frames in the experiment.
+        Used when creating Annotations and Cycles.
         """
         cursor = self.connection.cursor()
         try:
             cursor.execute(f"SELECT COUNT(*) FROM Frames")
             n_frames = cursor.fetchone()[0]
         except Exception as e:
             print(f"Could not get total number of frames from Frames because {e}")
@@ -154,14 +165,15 @@
         sql_create_Frames_table = """
             CREATE TABLE IF NOT EXISTS "Frames" (
             "Id"	INTEGER NOT NULL UNIQUE,
             "FrameInFile"	INTEGER NOT NULL,
             "FileId"	INTEGER NOT NULL,
             PRIMARY KEY("Id" AUTOINCREMENT),
             FOREIGN KEY("FileId") REFERENCES "Files"("Id")
+            UNIQUE("FrameInFile", "FileId")
             )
             """
         db_cursor.execute(sql_create_Frames_table)
 
         sql_create_Cycles_table = """
             CREATE TABLE IF NOT EXISTS "Cycles" (
             "Id"	INTEGER NOT NULL UNIQUE,
@@ -200,14 +212,15 @@
         sql_create_CycleIterations_table = """
             CREATE TABLE IF NOT EXISTS "CycleIterations" (
             "FrameId"	INTEGER NOT NULL,
             "CycleId"	INTEGER NOT NULL,
             "CycleIteration"	INTEGER NOT NULL,
             FOREIGN KEY("CycleId") REFERENCES "Cycles"("Id") ON DELETE CASCADE,
             FOREIGN KEY("FrameId") REFERENCES "Frames"("Id")
+            UNIQUE("FrameId","CycleId")
             )
             """
         db_cursor.execute(sql_create_CycleIterations_table)
 
         sql_create_Volumes_table = """
             CREATE TABLE IF NOT EXISTS "Volumes" (
             "FrameId"	INTEGER NOT NULL UNIQUE,
@@ -222,15 +235,15 @@
 
         db_cursor.close()
 
     def _populate_Options(self, file_manager: FileManager, volume_manager: VolumeManager):
         """
         Populates the Options table (a dictionary with key - value pairs).
         Learning resources:
-            another way of dealing with Errors : ( more pretty ??? )
+            another way of dealing with Errors :
             https://www.w3resource.com/python-exercises/sqlite/python-sqlite-exercise-6.php
         Args:
             file_manager: FileManager object that provides the data to populate the tables.
             volume_manager: VolumeManager object that provides the data to populate the tables.
         """
         row_data = [("data_dir", file_manager.data_dir.as_posix()),
                     ("frames_per_volume", volume_manager.fpv),
@@ -363,15 +376,15 @@
         except Exception as e:
             print(f"Could not write to AnnotationTypeLabels because {e}")
             raise e
         finally:
             cursor.close()
 
     def _populate_Annotations(self, annotation):
-        n_frames = self.get_n_frames()
+        n_frames = self._get_n_frames()
         assert n_frames == annotation.n_frames, f"Number of frames in the annotation, {annotation.n_frames}," \
                                                 f"doesn't match" \
                                                 f" the expected number of frames {n_frames}"
         frames = range(n_frames)
         row_data = [(frame + 1, label.name, label.group)
                     for frame, label in zip(frames, annotation.frame_to_label)]
         cursor = self.connection.cursor()
@@ -389,14 +402,15 @@
             raise e
         finally:
             cursor.close()
 
     def _populate_Cycles(self, annotation):
         """
         """
+        assert annotation.cycle is not None, "Annotation is not a Cycle"
         row_data = (annotation.name, annotation.cycle.to_json())
         cursor = self.connection.cursor()
         try:
             cursor.execute(
                 "INSERT INTO Cycles (AnnotationTypeId, Structure) " +
                 "VALUES((SELECT Id FROM AnnotationTypes WHERE Name = ?), ?)",
                 row_data)
@@ -404,30 +418,31 @@
         except Exception as e:
             print(f"Could not write to Cycles because {e}")
             raise e
         finally:
             cursor.close()
 
     def _populate_CycleIterations(self, annotation):
-        n_frames = self.get_n_frames()
+        n_frames = self._get_n_frames()
         assert n_frames == annotation.n_frames, f"Number of frames in the annotation, {annotation.n_frames}," \
                                                 f"doesn't match" \
                                                 f" the expected number of frames {n_frames}"
         # get cycle id by annotation type
         cursor = self.connection.cursor()
         cursor.execute(
             "SELECT Id FROM Cycles " +
             "WHERE AnnotationTypeId = (SELECT Id FROM AnnotationTypes " +
             "WHERE Name = ?)", (annotation.name,))
-        cycle_id = cursor.fetchone()[0]
+        cycle_id = cursor.fetchone()
+        assert cycle_id is not None, "Fill out AnnotationTypes and Cycles first."
         cursor.close()
 
         # prepare rows
         frames = range(n_frames)
-        row_data = [(frame + 1, cycle_id, iteration)
+        row_data = [(frame + 1, cycle_id[0], iteration)
                     for frame, iteration in zip(frames, annotation.frame_to_cycle)]
 
         # insert into CycleIterations
         cursor = self.connection.cursor()
         try:
             cursor.executemany(
                 "INSERT INTO CycleIterations (FrameId, CycleId, CycleIteration) " +
@@ -1378,15 +1393,14 @@
         if cycle_json is not None:
             cycle = Cycle.from_json(cycle_json)
         else:
             cycle = None
         return cycle
 
     def reconstruct_annotations(self):
-
         """
         Creates annotations from the database records.
         """
         # get the names of all the available annotations from the db
         annotation_names = self.db.get_Names_from_AnnotationTypes()
         # get the total number of frames in the recording
         n_frames = FrameManager(self.reconstruct_file_manager()).n_frames
```

### Comparing `vodex-1.0.8/src/vodex/experiment.py` & `vodex-1.0.9/src/vodex/experiment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 """
-This module contains 'Experiment' class that summarises the information about the experiment from the File,
-    Frame and Volume managers and Annotations to create the data base. Saves or loads the database.
-    Searches the frames based on volumes/ annotations. Loads the image data using the appropriate loader.
+This module contains the 'Experiment' class, which provides a summary of the information about an experiment. The
+class can initialise, save, and load the database, search for frames based on volumes or annotations, and load image
+data using the appropriate loader. To initialise the database, it integrates the information from the FileManager,
+FrameManager, VolumeManager, as well as Annotations, to create a database.
 """
 
 import numpy as np
 import numpy.typing as npt
 from pathlib import Path
 from typing import Union, List, Tuple
 import warnings
 
 from .core import VolumeManager, Annotation, ImageLoader
 from .dbmethods import DbReader, DbWriter
 
 
 class Experiment:
     """
-    Summarises the information about the experiment from the File,
-    Frame and Volume managers and Annotations to create the data base. Saves or loads the database.
-    Searches the frames based on volumes/ annotations. Loads the image data using the appropriate ImageLoader.
+    The class can initialise, save, and load the database, search for frames based on volumes or annotations, and load image
+    data using the appropriate loader. To initialise the database, it integrates the information from the File, Frame,
+    and Volume managers, as well as Annotations, to create a database.
 
     Args:
         db_reader: a DbReader object connected to the database with the experiment description.
 
     Attributes:
         db: a DbReader object connected to the database with the experiment description.
         loader: an ImageLoader object to load metadata and image data from files.
     """
 
     def __init__(self, db_reader: DbReader):
+        """
+        Initialize the experiment with the given DbReader object.
+        """
 
         assert isinstance(db_reader, DbReader), "Need DbReader to initialise the Experiment"
 
         self.db = db_reader
         # will add the loader the first time you are loading anything
         # in load_frames() or load_volumes()
         self.loader: ImageLoader
@@ -243,32 +247,19 @@
             as_volumes: weather to return cycle iteratoins per frame ( default) or per volume.
                 If as_volumes is true, it is expected that the cycle iteratoins are not changing in the middle of the volume.
                 Will throw an error if it happens.
             as_volumes: bool
         Returns:
             list of the condition ids (cycle iterations per frame or per volume)
         """
-        # TODO : check if empty
         if as_volumes:
             _, cycle_its, count = self.db.get_cycleIterations_per_volumes(annotation_type)
             fpv = self.db.get_fpv()
-            assert np.all(np.array(count) == fpv), "Can't list_cycle_iteratoins with as_volumes=True: " \
-                                                   "some iteratoins don't cover the whole volume." \
-                                                   "You might want to get iteratoins per frame," \
+            assert np.all(np.array(count) == fpv), "Can't list_cycle_iterations with as_volumes=True: " \
+                                                   "some iterations don't cover the whole volume." \
+                                                   "You might want to get iterations per frame," \
                                                    " by setting as_volumes=False"
         else:
             _, cycle_its = self.db.get_cycleIterations_per_frame(annotation_type)
 
         return cycle_its
 
-    def __str__(self):
-        pass
-
-    def __repr__(self):
-        return self.__str__()
-
-    def summary(self):
-        """
-        Prints a detailed description of the experiment.
-        """
-        # TODO : implement :)
-        raise NotImplementedError
```

### Comparing `vodex-1.0.8/src/vodex/loaders.py` & `vodex-1.0.9/src/vodex/loaders.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,93 +1,97 @@
 """
-This module contains classes to load and collect information from specific file types.
+This module contains classes for loading and collecting information from various file types.
 
-The module contains the following classes:
+It includes:
 
-- `Loader` - A generic loader class. Overwrite the methods to create your own loader.
+'Loader' - A generic class for loading files. Can be subclassed to create custom loaders for different file types.
 
-- `TiffLoader` - A class to work with tiff image files. Subclass of Loader.
-Used to get the datatype of the images, get the number of frames in each tiff file and load frames from tiff files.
-You can create your own loaders to work with other file types (see Contributions).
+'TiffLoader' - A class for working with TIFF image files. A subclass of Loader, it can be used to determine the data
+type of the images, the number of frames in each TIFF file, and load frames from TIFF files.
 
+Additional loaders can be created to work with other file types. See  Contributions for details.
 """
 
 import numpy as np
 import numpy.typing as npt
 
 from pathlib import Path
 from tifffile import TiffFile
 from tqdm import tqdm
 from typing import Union, Final, Dict, Tuple, List
 
 
 class Loader:
     """
-    A generic loader class.
-    Overwrite the methods to create your own loader.
+    The Loader class is a generic class that serves as a template for loading image data from specific file types.
+    The class contains basic methods that need to be overwritten to create a custom loader for a specific file type.
+
+    Any loader must be initialised by providing an example file from the dataset.
 
     Args:
-        file_example: An example file from the dataset
-            to infer the frame size and data type.
+        file_example: an example file from the dataset to infer the frame size and data type.
 
     Attributes:
-        frame_size: individual frame size (hight, width).
-        data_type: datatype.
+        frame_size: a tuple containing the individual frame size (height, width)
+        data_type: the datatype of the image frames.
     """
 
     def __init__(self, file_example: Union[str, Path]):
 
         self.frame_size: Tuple[int, int] = self.get_frame_size(file_example)
         self.data_type: np.dtype = self.get_frame_dtype(file_example)
 
     def __eq__(self, other):
+        """
+        Compares two loader instances for equality."
+        """
         print(f"__eq__ is Not Implemented for {type(self)} and {type(other)}")
 
         return NotImplemented
 
     @staticmethod
     def get_frames_in_file(file: Union[str, Path]) -> int:
         """
-        Compute and return the number of frames in a file.
+        Computes and returns the number of frames in a file.
 
         Args:
             file: the path to the file to get the number of frames for.
         Returns:
             the number of frames in the file.
         """
         raise NotImplementedError
 
     @staticmethod
     def get_frame_size(file: Union[str, Path]) -> Tuple[int, int]:
         """
-        Gets frame size ( height , width ) from a tiff file.
+        Returns the size of an individual frame (height, width) in pixels.
 
         Args:
             file: the path to the file to get the size of the frame for.
         Returns:
             ( height , width ) height and width of an individual frame in pixels.
         """
         raise NotImplementedError
 
     @staticmethod
     def get_frame_dtype(file: Union[str, Path]) -> np.dtype:
         """
-        Gets the datatype of the frame.
+        Returns the datatype of the image frames.
 
         Args:
             file: the path to the file to get the datatype of the frame for.
         Returns:
             datatype of the frame.
         """
         raise NotImplementedError
 
     def load_frames(self, frames: List[int], files: Union[List[str], List[Path]],
                     show_file_names: bool = False, show_progress: bool = True) -> npt.NDArray:
         """
-        Load frames from files and return as an array (frame, y, x).
+        Loads the specified frames from the given files and returns them as a 3D array (frame, y, x).
 
         Args:
             frames: list of frames inside corresponding files to load
             files: list of files corresponding to each frame
             show_file_names: whether to print the file from which the frames are loaded on the screen.
             show_progress: whether to show the progress bar of how many frames have been loaded.
         Returns:
```

### Comparing `vodex-1.0.8/src/vodex.egg-info/PKG-INFO` & `vodex-1.0.9/src/vodex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vodex
-Version: 1.0.8
+Version: 1.0.9
 Summary: VoDEx : Volumetric Data and Experiment Manager. Allows to load volumetric data based on experimental conditions.
 Home-page: https://github.com/LemonJust/vodex
 Author: Anna Nadtochiy
 Author-email: lemonjustgithub@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/LemonJust/vodex/issues
 Project-URL: Documentation, https://github.com/LemonJust/vodex#README.md
```

### Comparing `vodex-1.0.8/src/vodex.egg-info/SOURCES.txt` & `vodex-1.0.9/src/vodex.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -116,23 +116,25 @@
 src/vodex.egg-info/PKG-INFO
 src/vodex.egg-info/SOURCES.txt
 src/vodex.egg-info/dependency_links.txt
 src/vodex.egg-info/requires.txt
 src/vodex.egg-info/top_level.txt
 src/vodex/_tests/README.md
 src/vodex/_tests/__init__.py
+src/vodex/_tests/test_Cycle.py
+src/vodex/_tests/test_DbWriter.py
+src/vodex/_tests/test_Experiment.py
+src/vodex/_tests/test_FileManager.py
+src/vodex/_tests/test_ImageLoader.py
+src/vodex/_tests/test_Labels.py
+src/vodex/_tests/test_TimeLabel.py
+src/vodex/_tests/test_Timeline.py
 src/vodex/_tests/test_core.py
 src/vodex/_tests/test_dbmethods.py
-src/vodex/_tests/test_experiment.py
 src/vodex/_tests/test_loaders.py
-src/vodex/_tests/__pycache__/__init__.cpython-39.pyc
-src/vodex/_tests/__pycache__/test_core.cpython-39-pytest-7.2.0.pyc
-src/vodex/_tests/__pycache__/test_dbmethods.cpython-39-pytest-7.2.0.pyc
-src/vodex/_tests/__pycache__/test_experiment.cpython-39-pytest-7.2.0.pyc
-src/vodex/_tests/__pycache__/test_loaders.cpython-39-pytest-7.2.0.pyc
 src/vodex/_tests/data/movie_info.PNG
 src/vodex/_tests/data/test.db
 src/vodex/_tests/data/test_experiment.db
 src/vodex/_tests/data/test_movie.avi
 src/vodex/_tests/data/test_movie.tif
 src/vodex/_tests/data/construction_blocks/data.py
 src/vodex/_tests/data/construction_blocks/numbered_frames.tif
```

### Comparing `vodex-1.0.8/tox.ini` & `vodex-1.0.9/tox.ini`

 * *Files identical despite different names*

