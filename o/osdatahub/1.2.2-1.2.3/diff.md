# Comparing `tmp/osdatahub-1.2.2.tar.gz` & `tmp/osdatahub-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osdatahub-1.2.2.tar", last modified: Thu Mar 16 13:35:37 2023, max compression
+gzip compressed data, was "osdatahub-1.2.3.tar", last modified: Wed Apr 12 14:40:39 2023, max compression
```

## Comparing `osdatahub-1.2.2.tar` & `osdatahub-1.2.3.tar`

### file list

```diff
@@ -1,131 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:35:37.933536 osdatahub-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-03-16 13:35:16.000000 osdatahub-1.2.2/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:35:37.913536 osdatahub-1.2.2/Examples/
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-03-16 13:35:16.000000 osdatahub-1.2.2/Examples/CRS pitfalls.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   231081 2023-03-16 13:35:16.000000 osdatahub-1.2.2/Examples/Converting API Results into Common Data Formats.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  1837789 2023-03-16 13:35:16.000000 osdatahub-1.2.2/Examples/Defining Extents for API Queries.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12538 2023-03-16 13:35:16.000000 osdatahub-1.2.2/Examples/Filtering Attributes for API Queries.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10298 2023-03-16 13:35:16.000000 osdatahub-1.2.2/Examples/Interactive Plotting for API Results - Folium.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   945983 2023-03-16 13:35:16.000000 osdatahub-1.2.2/Examples/Plotting API Results - GeoPandas, Matplotlib and Contextily.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    34430 2023-03-16 13:35:16.000000 osdatahub-1.2.2/Examples/Post Processing API Queries.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-03-16 13:35:16.000000 osdatahub-1.2.2/Examples/Quick Start Guide.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-03-16 13:35:16.000000 osdatahub-1.2.2/Examples/Setting up an API key.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    86367 2023-03-16 13:35:16.000000 osdatahub-1.2.2/Examples/Using the NGD Features API.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:35:37.917536 osdatahub-1.2.2/Examples/images/
--rw-r--r--   0 runner    (1001) docker     (123)  2124067 2023-03-16 13:35:16.000000 osdatahub-1.2.2/Examples/images/1_homescreen.PNG
--rw-r--r--   0 runner    (1001) docker     (123)   178174 2023-03-16 13:35:16.000000 osdatahub-1.2.2/Examples/images/2_sign_up.PNG
--rw-r--r--   0 runner    (1001) docker     (123)  1883255 2023-03-16 13:35:16.000000 osdatahub-1.2.2/Examples/images/3_datahub_homepage.PNG
--rw-r--r--   0 runner    (1001) docker     (123)   115385 2023-03-16 13:35:16.000000 osdatahub-1.2.2/Examples/images/4_new_project.PNG
--rw-r--r--   0 runner    (1001) docker     (123)   153664 2023-03-16 13:35:16.000000 osdatahub-1.2.2/Examples/images/5_add_api_to_project.PNG
--rw-r--r--   0 runner    (1001) docker     (123)   113078 2023-03-16 13:35:16.000000 osdatahub-1.2.2/Examples/images/6_view_api_key.PNG
--rw-r--r--   0 runner    (1001) docker     (123)  1790610 2023-03-16 13:35:16.000000 osdatahub-1.2.2/Examples/images/CRS.png
--rw-r--r--   0 runner    (1001) docker     (123)    33604 2023-03-16 13:35:16.000000 osdatahub-1.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-03-16 13:35:16.000000 osdatahub-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-03-16 13:35:37.933536 osdatahub-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13892 2023-03-16 13:35:16.000000 osdatahub-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:35:37.921536 osdatahub-1.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-03-16 13:35:16.000000 osdatahub-1.2.2/docs/DownloadsAPI.rst
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-16 13:35:16.000000 osdatahub-1.2.2/docs/Extent.rst
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-16 13:35:16.000000 osdatahub-1.2.2/docs/FeaturesAPI.rst
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-16 13:35:16.000000 osdatahub-1.2.2/docs/LinkedIdentifiersAPI.rst
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-16 13:35:16.000000 osdatahub-1.2.2/docs/NGD.rst
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-03-16 13:35:16.000000 osdatahub-1.2.2/docs/NamesAPI.rst
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-03-16 13:35:16.000000 osdatahub-1.2.2/docs/PlacesAPI.rst
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-03-16 13:35:16.000000 osdatahub-1.2.2/docs/Utilities.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-03-16 13:35:16.000000 osdatahub-1.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-03-16 13:35:16.000000 osdatahub-1.2.2/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:35:37.921536 osdatahub-1.2.2/docs/media/
--rw-r--r--   0 runner    (1001) docker     (123)    23309 2023-03-16 13:35:16.000000 osdatahub-1.2.2/docs/media/os-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-16 13:35:16.000000 osdatahub-1.2.2/docs/readme_link.rst
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-16 13:35:16.000000 osdatahub-1.2.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:35:37.921536 osdatahub-1.2.2/media/
--rw-r--r--   0 runner    (1001) docker     (123)    23309 2023-03-16 13:35:16.000000 osdatahub-1.2.2/media/os-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-16 13:35:16.000000 osdatahub-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-16 13:35:16.000000 osdatahub-1.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-03-16 13:35:37.933536 osdatahub-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-16 13:35:16.000000 osdatahub-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:35:37.905536 osdatahub-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:35:37.925536 osdatahub-1.2.2/src/osdatahub/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:35:37.925536 osdatahub-1.2.2/src/osdatahub/DownloadsAPI/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-16 13:35:16.000000 osdatahub-1.2.2/src/osdatahub/DownloadsAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-03-16 13:35:16.000000 osdatahub-1.2.2/src/osdatahub/DownloadsAPI/data_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     6789 2023-03-16 13:35:16.000000 osdatahub-1.2.2/src/osdatahub/DownloadsAPI/downloads_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-03-16 13:35:16.000000 osdatahub-1.2.2/src/osdatahub/DownloadsAPI/opendata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:35:37.925536 osdatahub-1.2.2/src/osdatahub/FeaturesAPI/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-16 13:35:16.000000 osdatahub-1.2.2/src/osdatahub/FeaturesAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-03-16 13:35:16.000000 osdatahub-1.2.2/src/osdatahub/FeaturesAPI/feature_products.py
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-03-16 13:35:16.000000 osdatahub-1.2.2/src/osdatahub/FeaturesAPI/features_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:35:37.925536 osdatahub-1.2.2/src/osdatahub/LinkedIdentifiersAPI/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-16 13:35:16.000000 osdatahub-1.2.2/src/osdatahub/LinkedIdentifiersAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-03-16 13:35:16.000000 osdatahub-1.2.2/src/osdatahub/LinkedIdentifiersAPI/linked_identifier_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-03-16 13:35:16.000000 osdatahub-1.2.2/src/osdatahub/LinkedIdentifiersAPI/linked_identifiers_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:35:37.925536 osdatahub-1.2.2/src/osdatahub/NGD/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-16 13:35:16.000000 osdatahub-1.2.2/src/osdatahub/NGD/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-03-16 13:35:16.000000 osdatahub-1.2.2/src/osdatahub/NGD/crs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-03-16 13:35:16.000000 osdatahub-1.2.2/src/osdatahub/NGD/ngd_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:35:37.925536 osdatahub-1.2.2/src/osdatahub/NamesAPI/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-16 13:35:16.000000 osdatahub-1.2.2/src/osdatahub/NamesAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-03-16 13:35:16.000000 osdatahub-1.2.2/src/osdatahub/NamesAPI/local_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7263 2023-03-16 13:35:16.000000 osdatahub-1.2.2/src/osdatahub/NamesAPI/names_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:35:37.925536 osdatahub-1.2.2/src/osdatahub/PlacesAPI/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-16 13:35:16.000000 osdatahub-1.2.2/src/osdatahub/PlacesAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12821 2023-03-16 13:35:16.000000 osdatahub-1.2.2/src/osdatahub/PlacesAPI/places_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-16 13:35:16.000000 osdatahub-1.2.2/src/osdatahub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-03-16 13:35:16.000000 osdatahub-1.2.2/src/osdatahub/bbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-03-16 13:35:16.000000 osdatahub-1.2.2/src/osdatahub/codes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-03-16 13:35:16.000000 osdatahub-1.2.2/src/osdatahub/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-03-16 13:35:16.000000 osdatahub-1.2.2/src/osdatahub/extent.py
--rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-03-16 13:35:16.000000 osdatahub-1.2.2/src/osdatahub/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-03-16 13:35:16.000000 osdatahub-1.2.2/src/osdatahub/grow_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-03-16 13:35:16.000000 osdatahub-1.2.2/src/osdatahub/ons_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-03-16 13:35:16.000000 osdatahub-1.2.2/src/osdatahub/spatial_filter_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-03-16 13:35:16.000000 osdatahub-1.2.2/src/osdatahub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:35:37.925536 osdatahub-1.2.2/src/osdatahub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-03-16 13:35:37.000000 osdatahub-1.2.2/src/osdatahub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-03-16 13:35:37.000000 osdatahub-1.2.2/src/osdatahub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 13:35:37.000000 osdatahub-1.2.2/src/osdatahub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-16 13:35:37.000000 osdatahub-1.2.2/src/osdatahub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-16 13:35:37.000000 osdatahub-1.2.2/src/osdatahub.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:35:37.929536 osdatahub-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:35:37.929536 osdatahub-1.2.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:35:37.929536 osdatahub-1.2.2/tests/data/clean_polygon_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:35:37.933536 osdatahub-1.2.2/tests/data/clean_polygon_data/API (uncleaned)/
--rw-r--r--   0 runner    (1001) docker     (123)    29650 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/data/clean_polygon_data/API (uncleaned)/sites_multipolygon.geojson
--rw-r--r--   0 runner    (1001) docker     (123)    45345 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/data/clean_polygon_data/API (uncleaned)/sites_multipolygon2.geojson
--rw-r--r--   0 runner    (1001) docker     (123)    32875 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/data/clean_polygon_data/API (uncleaned)/sites_multipolygon_with_hole.geojson
--rw-r--r--   0 runner    (1001) docker     (123)    20201 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/data/clean_polygon_data/API (uncleaned)/sites_polygon.geojson
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/data/clean_polygon_data/API (uncleaned)/sites_polygon_with_hole.geojson
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:35:37.933536 osdatahub-1.2.2/tests/data/clean_polygon_data/QGIS/
--rw-r--r--   0 runner    (1001) docker     (123)    37512 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/data/clean_polygon_data/QGIS/sites_multipolygon.geojson
--rw-r--r--   0 runner    (1001) docker     (123)    58496 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/data/clean_polygon_data/QGIS/sites_multipolygon2.geojson
--rw-r--r--   0 runner    (1001) docker     (123)    33032 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/data/clean_polygon_data/QGIS/sites_multipolygon_with_hole.geojson
--rw-r--r--   0 runner    (1001) docker     (123)    25361 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/data/clean_polygon_data/QGIS/sites_polygon.geojson
--rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/data/clean_polygon_data/QGIS/sites_polygon_with_hole.geojson
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/data/clean_polygon_data/get_uncleaned_polygons.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/data/clean_polygon_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/data/downloads_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/data/extent_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/data/features_api_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/data/filters_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/data/linked_identifiers_api_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/data/names_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/data/ngd_crs_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    24199 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/data/ngd_merge_geojsons_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/data/ngd_query_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/data/places_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/data/utils_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/run_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/test_clean_polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/test_downloads_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/test_extent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/test_features_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/test_grow_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/test_linked_identifiers_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/test_names_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/test_ngd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/test_places_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-03-16 13:35:16.000000 osdatahub-1.2.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.716413 osdatahub-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-12 14:40:17.000000 osdatahub-1.2.3/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.700413 osdatahub-1.2.3/Examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-04-12 14:40:17.000000 osdatahub-1.2.3/Examples/CRS pitfalls.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   231081 2023-04-12 14:40:17.000000 osdatahub-1.2.3/Examples/Converting API Results into Common Data Formats.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  1837789 2023-04-12 14:40:17.000000 osdatahub-1.2.3/Examples/Defining Extents for API Queries.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12538 2023-04-12 14:40:17.000000 osdatahub-1.2.3/Examples/Filtering Attributes for API Queries.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10298 2023-04-12 14:40:17.000000 osdatahub-1.2.3/Examples/Interactive Plotting for API Results - Folium.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   945983 2023-04-12 14:40:17.000000 osdatahub-1.2.3/Examples/Plotting API Results - GeoPandas, Matplotlib and Contextily.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    34430 2023-04-12 14:40:17.000000 osdatahub-1.2.3/Examples/Post Processing API Queries.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-04-12 14:40:17.000000 osdatahub-1.2.3/Examples/Quick Start Guide.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-04-12 14:40:17.000000 osdatahub-1.2.3/Examples/Setting up an API key.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    86367 2023-04-12 14:40:17.000000 osdatahub-1.2.3/Examples/Using the NGD Features API.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.704413 osdatahub-1.2.3/Examples/images/
+-rw-r--r--   0 runner    (1001) docker     (123)  2124067 2023-04-12 14:40:17.000000 osdatahub-1.2.3/Examples/images/1_homescreen.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)   178174 2023-04-12 14:40:17.000000 osdatahub-1.2.3/Examples/images/2_sign_up.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)  1883255 2023-04-12 14:40:17.000000 osdatahub-1.2.3/Examples/images/3_datahub_homepage.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)   115385 2023-04-12 14:40:17.000000 osdatahub-1.2.3/Examples/images/4_new_project.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)   153664 2023-04-12 14:40:17.000000 osdatahub-1.2.3/Examples/images/5_add_api_to_project.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)   113078 2023-04-12 14:40:17.000000 osdatahub-1.2.3/Examples/images/6_view_api_key.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)  1790610 2023-04-12 14:40:17.000000 osdatahub-1.2.3/Examples/images/CRS.png
+-rw-r--r--   0 runner    (1001) docker     (123)    33604 2023-04-12 14:40:17.000000 osdatahub-1.2.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-12 14:40:17.000000 osdatahub-1.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-04-12 14:40:39.716413 osdatahub-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13892 2023-04-12 14:40:17.000000 osdatahub-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.708413 osdatahub-1.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-12 14:40:17.000000 osdatahub-1.2.3/docs/DownloadsAPI.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-12 14:40:17.000000 osdatahub-1.2.3/docs/Extent.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-12 14:40:17.000000 osdatahub-1.2.3/docs/FeaturesAPI.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-12 14:40:17.000000 osdatahub-1.2.3/docs/LinkedIdentifiersAPI.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-12 14:40:17.000000 osdatahub-1.2.3/docs/NGD.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-12 14:40:17.000000 osdatahub-1.2.3/docs/NamesAPI.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-12 14:40:17.000000 osdatahub-1.2.3/docs/PlacesAPI.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-12 14:40:17.000000 osdatahub-1.2.3/docs/Utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-12 14:40:17.000000 osdatahub-1.2.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-12 14:40:17.000000 osdatahub-1.2.3/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.708413 osdatahub-1.2.3/docs/media/
+-rw-r--r--   0 runner    (1001) docker     (123)    23309 2023-04-12 14:40:17.000000 osdatahub-1.2.3/docs/media/os-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-12 14:40:17.000000 osdatahub-1.2.3/docs/readme_link.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-12 14:40:17.000000 osdatahub-1.2.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.708413 osdatahub-1.2.3/media/
+-rw-r--r--   0 runner    (1001) docker     (123)    23309 2023-04-12 14:40:17.000000 osdatahub-1.2.3/media/os-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-12 14:40:17.000000 osdatahub-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-12 14:40:17.000000 osdatahub-1.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-12 14:40:39.720413 osdatahub-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-12 14:40:17.000000 osdatahub-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.692412 osdatahub-1.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.712413 osdatahub-1.2.3/src/osdatahub/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.712413 osdatahub-1.2.3/src/osdatahub/DownloadsAPI/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/DownloadsAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/DownloadsAPI/data_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/DownloadsAPI/downloads_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/DownloadsAPI/opendata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.712413 osdatahub-1.2.3/src/osdatahub/FeaturesAPI/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/FeaturesAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/FeaturesAPI/feature_products.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/FeaturesAPI/features_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.712413 osdatahub-1.2.3/src/osdatahub/LinkedIdentifiersAPI/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/LinkedIdentifiersAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/LinkedIdentifiersAPI/linked_identifier_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/LinkedIdentifiersAPI/linked_identifiers_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.712413 osdatahub-1.2.3/src/osdatahub/NGD/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/NGD/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/NGD/crs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/NGD/ngd_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.712413 osdatahub-1.2.3/src/osdatahub/NamesAPI/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/NamesAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/NamesAPI/local_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/NamesAPI/names_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.712413 osdatahub-1.2.3/src/osdatahub/PlacesAPI/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/PlacesAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/PlacesAPI/places_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/extent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/grow_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/ons_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/requests_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/spatial_filter_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.712413 osdatahub-1.2.3/src/osdatahub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-04-12 14:40:39.000000 osdatahub-1.2.3/src/osdatahub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-04-12 14:40:39.000000 osdatahub-1.2.3/src/osdatahub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:40:39.000000 osdatahub-1.2.3/src/osdatahub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-12 14:40:39.000000 osdatahub-1.2.3/src/osdatahub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-12 14:40:39.000000 osdatahub-1.2.3/src/osdatahub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.716413 osdatahub-1.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.716413 osdatahub-1.2.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.716413 osdatahub-1.2.3/tests/data/clean_polygon_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.716413 osdatahub-1.2.3/tests/data/clean_polygon_data/API (uncleaned)/
+-rw-r--r--   0 runner    (1001) docker     (123)    29650 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/clean_polygon_data/API (uncleaned)/sites_multipolygon.geojson
+-rw-r--r--   0 runner    (1001) docker     (123)    45345 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/clean_polygon_data/API (uncleaned)/sites_multipolygon2.geojson
+-rw-r--r--   0 runner    (1001) docker     (123)    32875 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/clean_polygon_data/API (uncleaned)/sites_multipolygon_with_hole.geojson
+-rw-r--r--   0 runner    (1001) docker     (123)    20201 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/clean_polygon_data/API (uncleaned)/sites_polygon.geojson
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/clean_polygon_data/API (uncleaned)/sites_polygon_with_hole.geojson
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.716413 osdatahub-1.2.3/tests/data/clean_polygon_data/QGIS/
+-rw-r--r--   0 runner    (1001) docker     (123)    37512 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/clean_polygon_data/QGIS/sites_multipolygon.geojson
+-rw-r--r--   0 runner    (1001) docker     (123)    58496 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/clean_polygon_data/QGIS/sites_multipolygon2.geojson
+-rw-r--r--   0 runner    (1001) docker     (123)    33032 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/clean_polygon_data/QGIS/sites_multipolygon_with_hole.geojson
+-rw-r--r--   0 runner    (1001) docker     (123)    25361 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/clean_polygon_data/QGIS/sites_polygon.geojson
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/clean_polygon_data/QGIS/sites_polygon_with_hole.geojson
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/clean_polygon_data/get_uncleaned_polygons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/clean_polygon_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/downloads_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/extent_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/features_api_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/filters_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/linked_identifiers_api_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/names_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/ngd_crs_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24199 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/ngd_merge_geojsons_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/ngd_query_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/places_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/utils_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/run_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/test_clean_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/test_downloads_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/test_extent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/test_features_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/test_grow_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/test_linked_identifiers_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/test_names_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/test_ngd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/test_places_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tox.ini
```

### Comparing `osdatahub-1.2.2/.readthedocs.yaml` & `osdatahub-1.2.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/Examples/CRS pitfalls.ipynb` & `osdatahub-1.2.3/Examples/CRS pitfalls.ipynb`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/Examples/Converting API Results into Common Data Formats.ipynb` & `osdatahub-1.2.3/Examples/Converting API Results into Common Data Formats.ipynb`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/Examples/Defining Extents for API Queries.ipynb` & `osdatahub-1.2.3/Examples/Defining Extents for API Queries.ipynb`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/Examples/Filtering Attributes for API Queries.ipynb` & `osdatahub-1.2.3/Examples/Filtering Attributes for API Queries.ipynb`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/Examples/Interactive Plotting for API Results - Folium.ipynb` & `osdatahub-1.2.3/Examples/Interactive Plotting for API Results - Folium.ipynb`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/Examples/Plotting API Results - GeoPandas, Matplotlib and Contextily.ipynb` & `osdatahub-1.2.3/Examples/Plotting API Results - GeoPandas, Matplotlib and Contextily.ipynb`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/Examples/Post Processing API Queries.ipynb` & `osdatahub-1.2.3/Examples/Post Processing API Queries.ipynb`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/Examples/Quick Start Guide.ipynb` & `osdatahub-1.2.3/Examples/Quick Start Guide.ipynb`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/Examples/Setting up an API key.ipynb` & `osdatahub-1.2.3/Examples/Setting up an API key.ipynb`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/Examples/Using the NGD Features API.ipynb` & `osdatahub-1.2.3/Examples/Using the NGD Features API.ipynb`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/Examples/images/1_homescreen.PNG` & `osdatahub-1.2.3/Examples/images/1_homescreen.PNG`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/Examples/images/2_sign_up.PNG` & `osdatahub-1.2.3/Examples/images/2_sign_up.PNG`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/Examples/images/3_datahub_homepage.PNG` & `osdatahub-1.2.3/Examples/images/3_datahub_homepage.PNG`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/Examples/images/4_new_project.PNG` & `osdatahub-1.2.3/Examples/images/4_new_project.PNG`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/Examples/images/5_add_api_to_project.PNG` & `osdatahub-1.2.3/Examples/images/5_add_api_to_project.PNG`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/Examples/images/6_view_api_key.PNG` & `osdatahub-1.2.3/Examples/images/6_view_api_key.PNG`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/Examples/images/CRS.png` & `osdatahub-1.2.3/Examples/images/CRS.png`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/LICENSE.txt` & `osdatahub-1.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/PKG-INFO` & `osdatahub-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osdatahub
-Version: 1.2.2
+Version: 1.2.3
 Summary: osdatahub is Ordnance Survey's (OS) Python API wrapper, designed to make data from the OS Data Hub APIs readily accessible to developers.
 Home-page: https://github.com/OrdnanceSurvey/osdatahub
 Download-URL: https://pypi.org/project/osdatahub/
 Author: OS Rapid Prototyping
 Author-email: rapidprototyping@os.uk
 License: OGL
 Project-URL: Code, https://github.com/OrdnanceSurvey/osdatahub
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: osdatahub Version: 1.2.2 Summary: osdatahub is
+Metadata-Version: 2.1 Name: osdatahub Version: 1.2.3 Summary: osdatahub is
 Ordnance Survey's (OS) Python API wrapper, designed to make data from the OS
 Data Hub APIs readily accessible to developers. Home-page: https://github.com/
 OrdnanceSurvey/osdatahub Download-URL: https://pypi.org/project/osdatahub/
 Author: OS Rapid Prototyping Author-email: rapidprototyping@os.uk License: OGL
 Project-URL: Code, https://github.com/OrdnanceSurvey/osdatahub Project-URL:
 Documentation, https://osdatahub.readthedocs.io/en/latest/ Project-URL: Issues,
 https://github.com/OrdnanceSurvey/osdatahub/issues Keywords: Ordnance-
```

### Comparing `osdatahub-1.2.2/README.md` & `osdatahub-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/docs/Utilities.rst` & `osdatahub-1.2.3/docs/Utilities.rst`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/docs/conf.py` & `osdatahub-1.2.3/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "osdatahub"
 copyright = "2021, OS Rapid Prototyping Team"
 author = "OS Rapid Prototyping Team"
 
 # The full version, including alpha/beta/rc tags
-release = "1.2.2"
+release = "1.2.3"
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
```

### Comparing `osdatahub-1.2.2/docs/index.rst` & `osdatahub-1.2.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/docs/media/os-logo.png` & `osdatahub-1.2.3/docs/media/os-logo.png`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/media/os-logo.png` & `osdatahub-1.2.3/media/os-logo.png`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/setup.cfg` & `osdatahub-1.2.3/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = osdatahub
-version = 1.2.2
+version = 1.2.3
 author = OS Rapid Prototyping
 author_email = rapidprototyping@os.uk
 classifiers = 
 	Natural Language :: English
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Programming Language :: Python :: 3.7
```

### Comparing `osdatahub-1.2.2/src/osdatahub/DownloadsAPI/data_package.py` & `osdatahub-1.2.3/src/osdatahub/DownloadsAPI/data_package.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,30 +35,30 @@
 
         Args:
             key (str): A valid OS API Key. Get a free key here - https://osdatahub.os.uk/
 
         Returns: A list of dictionaries containing all available Data Packages
 
         """
-        response = requests.get(cls._ENDPOINT, params={"key": key}, proxies=osdatahub.get_proxies())
+        response = osdatahub.get(cls._ENDPOINT, params={"key": key}, proxies=osdatahub.get_proxies())
         response.raise_for_status()
         content = response.json()
         if not content:
             logging.warning(f"You have no premium data packages available. "
                             f"Make sure that you first ordered a data package at "
                             f"https://osdatahub.os.uk/downloads/premium")
         return content
 
     @property
     @functools.lru_cache()
     def versions(self) -> list:
         """
         Get all the available versions for the data package
         """
-        response = requests.get(self._endpoint(f"{self._id}/versions"), params={"key": self.key}, proxies=osdatahub.get_proxies())
+        response = osdatahub.get(self._endpoint(f"{self._id}/versions"), params={"key": self.key}, proxies=osdatahub.get_proxies())
         response.raise_for_status()
         return response.json()
 
     @typechecked
     def product_list(self, version_id: str, return_downloadobj: bool = False) -> Union[list, dict]:
         """
         Returns a list of possible downloads for a specific OS Premium Data Package based on given filters
@@ -69,15 +69,15 @@
                 json. Defaults to False
 
         Returns:
             List of downloadable files from Downloads API
         """
         endpoint = self._endpoint(f"{self._id}/versions/{version_id}")
         params = {"key": self.key}
-        response = requests.get(url=endpoint, params=params, proxies=osdatahub.get_proxies())
+        response = osdatahub.get(url=endpoint, params=params, proxies=osdatahub.get_proxies())
         response.raise_for_status()
         content = response.json()
         if not content:
             logging.warning(f"There are no premium data packages available with id={self.id} and "
                             f"version_id={version_id}. Make sure that you first ordered a data package at"
                             f"https://osdatahub.os.uk/downloads/premium")
         if return_downloadobj:
```

### Comparing `osdatahub-1.2.2/src/osdatahub/DownloadsAPI/downloads_api.py` & `osdatahub-1.2.3/src/osdatahub/DownloadsAPI/downloads_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,23 +39,23 @@
         output_path = os.path.join(output_dir, self.file_name)
 
         if os.path.isfile(output_path) and not overwrite:
             logging.warning(f"Overwrite is set to False and there is a file already in the location {output_path}. "
                             f"Skipping download...")
             return output_path
 
-        r = requests.get(self.url, stream=True, proxies=osdatahub.get_proxies())
-        r.raise_for_status()
-        size = int(r.headers.get('content-length'))
+        response = osdatahub.get(self.url, stream=True, proxies=osdatahub.get_proxies())
+        response.raise_for_status()
+        size = int(response.headers.get('content-length'))
         chunk_size = 1024
-        if r.status_code == 200:
+        if response.status_code == 200:
             with open(output_path, 'wb') as f:
                 if not pbar:
                     pbar = tqdm(total=size, desc=self.file_name, unit="B", unit_scale=True, leave=True)
-                for chunk in r.iter_content(chunk_size=chunk_size):
+                for chunk in response.iter_content(chunk_size=chunk_size):
                     f.write(chunk)
                     f.flush()
                     pbar.update(chunk_size)
 
         pbar.write(f"Finished downloading {self.file_name} to {output_path}")
         return output_path
 
@@ -91,27 +91,27 @@
 
     @property
     @functools.lru_cache()
     def details(self) -> dict:
         """
         Calls endpoint to return details about the product or data package
         """
-        response = requests.get(self._endpoint(self._id), proxies=osdatahub.get_proxies())
+        response = osdatahub.get(self._endpoint(self._id), proxies=osdatahub.get_proxies())
         response.raise_for_status()
         return response.json()
 
     @classmethod
     def all_products(cls, **kwargs) -> list:
         """
         Returns a list of all available products of the product type
 
         Returns: list of dictionaries containing all products available to download
 
         """
-        response = requests.get(cls._ENDPOINT, proxies=osdatahub.get_proxies())
+        response = osdatahub.get(cls._ENDPOINT, proxies=osdatahub.get_proxies())
         response.raise_for_status()
         return response.json()
 
     @abstractmethod
     def product_list(self):
         """
         Abstract method for returning a list of files available to download for a specific data package/opendata product
```

### Comparing `osdatahub-1.2.2/src/osdatahub/DownloadsAPI/opendata.py` & `osdatahub-1.2.3/src/osdatahub/DownloadsAPI/opendata.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         if file_format:
             params.update({"format": file_format})
         if file_subformat:
             params.update({"subformat": file_subformat})
         if area:
             params.update({"area": area})
 
-        response = requests.get(url=self._endpoint(f"{self._id}/downloads"), params=params, proxies=osdatahub.get_proxies())
+        response = osdatahub.get(url=self._endpoint(f"{self._id}/downloads"), params=params, proxies=osdatahub.get_proxies())
         response.raise_for_status()
         if return_downloadobj:
             return [_DownloadObj(url=download["url"], file_name=download["fileName"], size=download["size"])
                     for download in response.json()]
         else:
             return response.json()
```

### Comparing `osdatahub-1.2.2/src/osdatahub/FeaturesAPI/feature_products.py` & `osdatahub-1.2.3/src/osdatahub/FeaturesAPI/feature_products.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/src/osdatahub/FeaturesAPI/features_api.py` & `osdatahub-1.2.3/src/osdatahub/FeaturesAPI/features_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         n_required = min(limit, 100)
         if "srsName='EPSG:4326'" in params["filter"]:
             warnings.warn("The features API does not support EPSG:4326 and will return an empty features list.")
 
         try:
             while n_required > 0 and data.grown:
                 params.update({"count": n_required, "startIndex": len(data)})
-                response = requests.get(self.ENDPOINT, params=params, proxies=osdatahub.get_proxies())
+                response = osdatahub.get(self.ENDPOINT, params=params, proxies=osdatahub.get_proxies())
                 resp_json = response.json()
                 if "fault" in resp_json:
                     raise_http_error(response)
                 if is_new_api(resp_json):
                     self.new_api = True
                     self.product = self.__product_name
                 data.extend(resp_json["features"])
```

### Comparing `osdatahub-1.2.2/src/osdatahub/LinkedIdentifiersAPI/linked_identifier_options.py` & `osdatahub-1.2.3/src/osdatahub/LinkedIdentifiersAPI/linked_identifier_options.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/src/osdatahub/LinkedIdentifiersAPI/linked_identifiers_api.py` & `osdatahub-1.2.3/src/osdatahub/LinkedIdentifiersAPI/linked_identifiers_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     __ENDPOINT = r"https://api.os.uk/search/links/v1/"
 
     def __init__(self, key: str):
         self.key = key
 
     @staticmethod
     def __request(endpoint: str) -> dict:
-        response = requests.get(endpoint, proxies=osdatahub.get_proxies())
+        response = osdatahub.get(endpoint, proxies=osdatahub.get_proxies())
         if response.status_code != 200:
             raise_http_error(response)
         return response.json()
 
     def __get_endpoint(
             self, identifier: Union[int, str], feature_type: str, identifier_type: str
     ) -> str:
```

### Comparing `osdatahub-1.2.2/src/osdatahub/NGD/crs.py` & `osdatahub-1.2.3/src/osdatahub/NGD/crs.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/src/osdatahub/NGD/ngd_api.py` & `osdatahub-1.2.3/src/osdatahub/NGD/ngd_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     @functools.lru_cache()
     def get_collections(cls) -> dict:
         """
         Retrieves all OS NGD Feature Collections
         Returns:
             Dict: Dictionary containing all Feature Collections currently supported with details for each
         """
-        response = requests.get(cls.__ENDPOINT, proxies=osdatahub.get_proxies())
+        response = osdatahub.get(cls.__ENDPOINT, proxies=osdatahub.get_proxies())
         response.raise_for_status()
         return response.json()
 
     def query(self,
               extent: Extent = None,
               crs: Union[str, int] = None,
               start_datetime: datetime = None,
@@ -172,15 +172,15 @@
         headers.update({"key": self.key})
 
         while n_required > 0:
             limit = min(n_required, 100)
             offset = max(offset, data["numberReturned"] if "numberReturned" in data else 0)
             params.update({"limit": limit, "offset": offset})
             try:
-                response = requests.get(self.__endpoint(), params=params, headers=headers, proxies=osdatahub.get_proxies())
+                response = osdatahub.get(self.__endpoint(), params=params, headers=headers, proxies=osdatahub.get_proxies())
                 response.raise_for_status()
             except requests.exceptions.HTTPError as e:
                 logging.error(json.dumps(e.response.json(), indent=4))
                 raise e
 
             resp_json = response.json()
 
@@ -204,11 +204,11 @@
                 Available CRS values are: EPSG:27700, EPSG:4326, EPSG:7405, EPSG:3857, and CRS84. Defaults to CRS84
 
         Returns:
             Feature: A GeoJSON Feature containing the requested feature
         """
         params = {"crs": get_crs(crs)} if crs else {}
 
-        response = requests.get(self.__endpoint(feature_id), params=params, headers={"key": self.key}, proxies=osdatahub.get_proxies())
+        response = osdatahub.get(self.__endpoint(feature_id), params=params, headers={"key": self.key}, proxies=osdatahub.get_proxies())
         response.raise_for_status()
 
         return response.json()
```

### Comparing `osdatahub-1.2.2/src/osdatahub/NamesAPI/local_types.py` & `osdatahub-1.2.3/src/osdatahub/NamesAPI/local_types.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/src/osdatahub/NamesAPI/names_api.py` & `osdatahub-1.2.3/src/osdatahub/NamesAPI/names_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
                 raise TypeError("Bounding Box filter must be in British National Grid CRS (EPSG:27700)")
             params.update({"fq": self.__format_fq(bbox_filter, local_type)})
 
         try:
             n_required = min(limit, 100)
             while n_required > 0 and data.grown:
                 params.update({"offset": len(data), "maxresults": n_required})
-                response = requests.get(self.__endpoint("find"), params=params, proxies=osdatahub.get_proxies())
+                response = osdatahub.get(self.__endpoint("find"), params=params, proxies=osdatahub.get_proxies())
                 data.extend(self.__format_response(response))
                 n_required = min(100, limit - len(data))
         except KeyError:
             raise_http_error(response)
         return addresses_to_geojson(data.values, "EPSG:27700")
 
     def nearest(self, point: tuple, radius: float = 100, local_type: Union[Iterable, str] = None) -> FeatureCollection:
@@ -105,15 +105,15 @@
         if not 0.01 <= radius <= 1000:
             raise ValueError(f"Argument \"radius\" must be between 0.01 and 1000, but had value {radius}")
 
         params = {"point": ",".join([str(c) for c in point]), "radius": radius}
         if local_type:
             params.update({"fq": self.__format_fq(local_type=local_type)})
         try:
-            response = requests.get(self.__endpoint("nearest"), params=params, proxies=osdatahub.get_proxies())
+            response = osdatahub.get(self.__endpoint("nearest"), params=params, proxies=osdatahub.get_proxies())
             data.extend(self.__format_response(response))
         except KeyError:
             if response.status_code != 200:
                 raise_http_error(response)
         return addresses_to_geojson(data.values, crs="EPSG:27700")
 
     @staticmethod
```

### Comparing `osdatahub-1.2.2/src/osdatahub/PlacesAPI/places_api.py` & `osdatahub-1.2.3/src/osdatahub/PlacesAPI/places_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
                 {"fq": self.__format_fq(classification_code, logical_status_code)}
             )
 
         try:
             n_required = min(limit, 100)
             while n_required > 0 and data.grown:
                 params["params"].update({"offset": len(data), "maxresults": n_required})
-                response = requests.post(**params)
+                response = osdatahub.post(**params)
                 data.extend(self.__format_response(response))
                 n_required = min(100, limit - len(data))
         except KeyError:
             response.raise_for_status()
         return addresses_to_geojson(data.values, output_crs)
 
     def find(
@@ -121,15 +121,15 @@
                 {"fq": self.__format_fq(classification_code, logical_status_code)}
             )
 
         try:
             n_required = min(limit, 100)
             while n_required > 0 and data.grown:
                 params.update({"offset": len(data), "maxresults": n_required})
-                response = requests.get(self.__endpoint("find"), params=params, proxies=osdatahub.get_proxies())
+                response = osdatahub.get(self.__endpoint("find"), params=params, proxies=osdatahub.get_proxies())
                 data.extend(self.__format_response(response))
                 n_required = min(100, limit - len(data))
         except KeyError:
             response.raise_for_status()
         return addresses_to_geojson(data.values, output_crs)
 
     def postcode(
@@ -165,15 +165,15 @@
             params.update(
                 {"fq": self.__format_fq(classification_code, logical_status_code)}
             )
         try:
             n_required = min(limit, 100)
             while n_required > 0 and data.grown:
                 params.update({"offset": len(data), "maxresults": n_required})
-                response = requests.get(self.__endpoint("postcode"), params=params, proxies=osdatahub.get_proxies())
+                response = osdatahub.get(self.__endpoint("postcode"), params=params, proxies=osdatahub.get_proxies())
                 data.extend(self.__format_response(response))
                 n_required = min(100, limit - len(data))
         except KeyError:
             response.raise_for_status()
         return addresses_to_geojson(data.values, output_crs)
 
     def uprn(
@@ -199,15 +199,15 @@
         data = GrowList()
         params = {"uprn": uprn, "output_srs": output_crs}
         if classification_code or logical_status_code:
             params.update(
                 {"fq": self.__format_fq(classification_code, logical_status_code)}
             )
         try:
-            response = requests.get(self.__endpoint("uprn"), params=params, proxies=osdatahub.get_proxies())
+            response = osdatahub.get(self.__endpoint("uprn"), params=params, proxies=osdatahub.get_proxies())
             data.extend(self.__format_response(response))
         except KeyError:
             response.raise_for_status()
         return addresses_to_geojson(data.values, output_crs)
 
     def nearest(
             self,
@@ -244,15 +244,15 @@
             "radius": radius,
         }
         if classification_code or logical_status_code:
             params.update(
                 {"fq": self.__format_fq(classification_code, logical_status_code)}
             )
         try:
-            response = requests.get(self.__endpoint("nearest"), params=params, proxies=osdatahub.get_proxies())
+            response = osdatahub.get(self.__endpoint("nearest"), params=params, proxies=osdatahub.get_proxies())
             data.extend(self.__format_response(response))
         except KeyError:
             response.raise_for_status()
         return addresses_to_geojson(data.values, output_crs)
 
     @staticmethod
     def __format_response(response: requests.Response) -> list:
```

### Comparing `osdatahub-1.2.2/src/osdatahub/__init__.py` & `osdatahub-1.2.3/src/osdatahub/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 
 def set_proxies(proxies):
     os.environ["_OSDATAHUB_PROXIES"] = json.dumps(proxies)
 
 def get_proxies():
     return json.loads(os.environ["_OSDATAHUB_PROXIES"])
 
-__version__ = "1.2.2"
+__version__ = "1.2.3"
 
 from osdatahub.extent import Extent
 from osdatahub.FeaturesAPI import FeaturesAPI
 from osdatahub.PlacesAPI import PlacesAPI
 from osdatahub.NamesAPI import NamesAPI
 from osdatahub.LinkedIdentifiersAPI import LinkedIdentifiersAPI
 from osdatahub.DownloadsAPI import OpenDataDownload, DataPackageDownload
 from osdatahub.NGD import NGD
+from osdatahub.requests_wrapper import get
```

### Comparing `osdatahub-1.2.2/src/osdatahub/bbox.py` & `osdatahub-1.2.3/src/osdatahub/bbox.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/src/osdatahub/codes.py` & `osdatahub-1.2.3/src/osdatahub/codes.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/src/osdatahub/errors.py` & `osdatahub-1.2.3/src/osdatahub/errors.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/src/osdatahub/extent.py` & `osdatahub-1.2.3/src/osdatahub/extent.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/src/osdatahub/filters.py` & `osdatahub-1.2.3/src/osdatahub/filters.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/src/osdatahub/grow_list.py` & `osdatahub-1.2.3/src/osdatahub/grow_list.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/src/osdatahub/ons_api.py` & `osdatahub-1.2.3/src/osdatahub/ons_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,9 +41,9 @@
     Args:
         ons_code (str): ONS code
 
     Returns:
         response_json (dict): The json of the raw response
     """
     url = f"{ID_ENDPOINT}{ons_code}"
-    res = requests.get(url, proxies=osdatahub.get_proxies())
+    res = osdatahub.get(url, proxies=osdatahub.get_proxies())
     return _sanitise_response(res)
```

### Comparing `osdatahub-1.2.2/src/osdatahub/spatial_filter_types.py` & `osdatahub-1.2.3/src/osdatahub/spatial_filter_types.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/src/osdatahub/utils.py` & `osdatahub-1.2.3/src/osdatahub/utils.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/src/osdatahub.egg-info/PKG-INFO` & `osdatahub-1.2.3/src/osdatahub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osdatahub
-Version: 1.2.2
+Version: 1.2.3
 Summary: osdatahub is Ordnance Survey's (OS) Python API wrapper, designed to make data from the OS Data Hub APIs readily accessible to developers.
 Home-page: https://github.com/OrdnanceSurvey/osdatahub
 Download-URL: https://pypi.org/project/osdatahub/
 Author: OS Rapid Prototyping
 Author-email: rapidprototyping@os.uk
 License: OGL
 Project-URL: Code, https://github.com/OrdnanceSurvey/osdatahub
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: osdatahub Version: 1.2.2 Summary: osdatahub is
+Metadata-Version: 2.1 Name: osdatahub Version: 1.2.3 Summary: osdatahub is
 Ordnance Survey's (OS) Python API wrapper, designed to make data from the OS
 Data Hub APIs readily accessible to developers. Home-page: https://github.com/
 OrdnanceSurvey/osdatahub Download-URL: https://pypi.org/project/osdatahub/
 Author: OS Rapid Prototyping Author-email: rapidprototyping@os.uk License: OGL
 Project-URL: Code, https://github.com/OrdnanceSurvey/osdatahub Project-URL:
 Documentation, https://osdatahub.readthedocs.io/en/latest/ Project-URL: Issues,
 https://github.com/OrdnanceSurvey/osdatahub/issues Keywords: Ordnance-
```

### Comparing `osdatahub-1.2.2/src/osdatahub.egg-info/SOURCES.txt` & `osdatahub-1.2.3/src/osdatahub.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 src/osdatahub/bbox.py
 src/osdatahub/codes.py
 src/osdatahub/errors.py
 src/osdatahub/extent.py
 src/osdatahub/filters.py
 src/osdatahub/grow_list.py
 src/osdatahub/ons_api.py
+src/osdatahub/requests_wrapper.py
 src/osdatahub/spatial_filter_types.py
 src/osdatahub/utils.py
 src/osdatahub.egg-info/PKG-INFO
 src/osdatahub.egg-info/SOURCES.txt
 src/osdatahub.egg-info/dependency_links.txt
 src/osdatahub.egg-info/requires.txt
 src/osdatahub.egg-info/top_level.txt
```

### Comparing `osdatahub-1.2.2/tests/data/clean_polygon_data/API (uncleaned)/sites_multipolygon.geojson` & `osdatahub-1.2.3/tests/data/clean_polygon_data/API (uncleaned)/sites_multipolygon.geojson`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/tests/data/clean_polygon_data/API (uncleaned)/sites_multipolygon2.geojson` & `osdatahub-1.2.3/tests/data/clean_polygon_data/API (uncleaned)/sites_multipolygon2.geojson`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/tests/data/clean_polygon_data/API (uncleaned)/sites_multipolygon_with_hole.geojson` & `osdatahub-1.2.3/tests/data/clean_polygon_data/API (uncleaned)/sites_multipolygon_with_hole.geojson`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/tests/data/clean_polygon_data/API (uncleaned)/sites_polygon.geojson` & `osdatahub-1.2.3/tests/data/clean_polygon_data/API (uncleaned)/sites_polygon.geojson`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/tests/data/clean_polygon_data/API (uncleaned)/sites_polygon_with_hole.geojson` & `osdatahub-1.2.3/tests/data/clean_polygon_data/API (uncleaned)/sites_polygon_with_hole.geojson`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/tests/data/clean_polygon_data/QGIS/sites_multipolygon.geojson` & `osdatahub-1.2.3/tests/data/clean_polygon_data/QGIS/sites_multipolygon.geojson`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/tests/data/clean_polygon_data/QGIS/sites_multipolygon2.geojson` & `osdatahub-1.2.3/tests/data/clean_polygon_data/QGIS/sites_multipolygon2.geojson`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/tests/data/clean_polygon_data/QGIS/sites_multipolygon_with_hole.geojson` & `osdatahub-1.2.3/tests/data/clean_polygon_data/QGIS/sites_multipolygon_with_hole.geojson`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/tests/data/clean_polygon_data/QGIS/sites_polygon.geojson` & `osdatahub-1.2.3/tests/data/clean_polygon_data/QGIS/sites_polygon.geojson`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/tests/data/clean_polygon_data/QGIS/sites_polygon_with_hole.geojson` & `osdatahub-1.2.3/tests/data/clean_polygon_data/QGIS/sites_polygon_with_hole.geojson`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/tests/data/clean_polygon_data/get_uncleaned_polygons.py` & `osdatahub-1.2.3/tests/data/clean_polygon_data/get_uncleaned_polygons.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         """
         params = self._FeaturesAPI__params()
         data = GrowList()
         n_required = min(limit, 100)
         try:
             while n_required > 0 and data.grown:
                 params.update({"count": n_required, "startIndex": len(data)})
-                response = requests.get(self.ENDPOINT, params=params, proxies=osdatahub.get_proxies())
+                response = osdatahub.get(self.ENDPOINT, params=params, proxies=osdatahub.get_proxies())
                 data.extend(response.json()["features"])
                 n_required = min(100, limit - len(data))
         except json.decoder.JSONDecodeError:
             raise_http_error(response)
         # DOESN'T run features_to_geojson before returning result
         return FeatureCollection(data.values, crs=self.extent.crs)
```

### Comparing `osdatahub-1.2.2/tests/data/clean_polygon_data.py` & `osdatahub-1.2.3/tests/data/clean_polygon_data.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/tests/data/downloads_data.py` & `osdatahub-1.2.3/tests/data/downloads_data.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/tests/data/extent_data.py` & `osdatahub-1.2.3/tests/data/extent_data.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/tests/data/features_api_data.py` & `osdatahub-1.2.3/tests/data/features_api_data.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/tests/data/filters_data.py` & `osdatahub-1.2.3/tests/data/filters_data.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/tests/data/linked_identifiers_api_data.py` & `osdatahub-1.2.3/tests/data/linked_identifiers_api_data.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/tests/data/names_data.py` & `osdatahub-1.2.3/tests/data/names_data.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/tests/data/ngd_crs_data.py` & `osdatahub-1.2.3/tests/data/ngd_crs_data.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/tests/data/ngd_merge_geojsons_data.py` & `osdatahub-1.2.3/tests/data/ngd_merge_geojsons_data.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/tests/data/ngd_query_data.py` & `osdatahub-1.2.3/tests/data/ngd_query_data.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/tests/data/places_data.py` & `osdatahub-1.2.3/tests/data/places_data.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/tests/data/utils_data.py` & `osdatahub-1.2.3/tests/data/utils_data.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/tests/run_functions.py` & `osdatahub-1.2.3/tests/run_functions.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/tests/test_downloads_api.py` & `osdatahub-1.2.3/tests/test_downloads_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     def test_product_init(self, open_data_download):
         assert open_data_download._ENDPOINT == "https://api.os.uk/downloads/v1/products"
         assert open_data_download.id == "test_id"
 
     @pytest.mark.parametrize(*data.product_list_pass("test_id"))
     @pytest.mark.usefixtures("open_data_download")
-    @mock.patch('requests.get')
+    @mock.patch('osdatahub.get')
     def test_product_list_pass(self, request_mocked, open_data_download, file_name, file_format, file_subformat, area,
                                return_downloadobj, expected_url, expected_params):
         open_data_download.product_list(file_name=file_name, file_format=file_format, file_subformat=file_subformat,
                                         area=area, return_downloadobj=return_downloadobj)
         request_mocked.assert_called_with(url=expected_url,
                                           params=expected_params,
                                           proxies={})
```

### Comparing `osdatahub-1.2.2/tests/test_extent.py` & `osdatahub-1.2.3/tests/test_extent.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/tests/test_features_api.py` & `osdatahub-1.2.3/tests/test_features_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         # Act
         params = features_api._FeaturesAPI__params
 
         # Assert
         assert params == expected_result
 
     @pytest.mark.parametrize(*data.test_request_params())
-    @mock.patch('requests.get')
+    @mock.patch('osdatahub.get')
     def test_request_params(self, request_mocked, extent, product, filters,
                             limit, expected_url, expected_params):
         # Arrange
         request_mocked.return_value.configure_mock(json=lambda: {"features": []})
         features_api = FeaturesAPI("API-KEY", product, extent)
         for filter in filters:
             features_api.add_filters(filter)
```

### Comparing `osdatahub-1.2.2/tests/test_filters.py` & `osdatahub-1.2.3/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/tests/test_grow_list.py` & `osdatahub-1.2.3/tests/test_grow_list.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/tests/test_linked_identifiers_api.py` & `osdatahub-1.2.3/tests/test_linked_identifiers_api.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/tests/test_names_api.py` & `osdatahub-1.2.3/tests/test_names_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     @pytest.fixture()
     def names(self):
         names = NamesAPI("test")
         yield names
 
     @pytest.mark.parametrize(*data.test_find_pass())
     @pytest.mark.usefixtures("names")
-    @mock.patch('requests.get')
+    @mock.patch('osdatahub.get')
     def test_find_pass(self, request_mocked, names, text, limit, bounds, bbox_filter, local_type,
                        expected_url, expected_params):
         names.find(text, limit=limit, bounds=bounds, bbox_filter=bbox_filter, local_type=local_type)
         request_mocked.assert_called_with(expected_url,
                                           params=expected_params,
                                           proxies={})
 
@@ -34,15 +34,15 @@
     @pytest.fixture()
     def names(self):
         names = NamesAPI("test")
         yield names
 
     @pytest.mark.parametrize(*data.test_nearest_pass())
     @pytest.mark.usefixtures("names")
-    @mock.patch('requests.get')
+    @mock.patch('osdatahub.get')
     def test_nearest_pass(self, request_mocked, names, point, radius, local_type, expected_url, expected_params):
         names.nearest(point=point, radius=radius, local_type=local_type)
         request_mocked.assert_called_with(expected_url,
                                           params=expected_params,
                                           proxies={})
 
     @pytest.mark.parametrize(*data.test_nearest_fail())
```

### Comparing `osdatahub-1.2.2/tests/test_ngd.py` & `osdatahub-1.2.3/tests/test_ngd.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,28 +24,28 @@
     def test_ngd_crs_fail(self, crs, valid_crs, expected_result):
         with pytest.raises(expected_exception=expected_result):
             get_crs(crs, valid_crs)
 
 
 class TestNGDQuery:
     @pytest.mark.parametrize(*query_data.test_ngd_instantiation())
-    @mock.patch('requests.get')
+    @mock.patch('osdatahub.get')
     def test_ngd_instantiation(self, request_mocked, api_key, collection, expected_url, expected_headers):
         request_mocked.return_value.configure_mock(json=lambda: {"features": [], "numberReturned": 0})
 
         ngd = NGD(key=api_key, collection=collection)
         ngd.query()
 
         request_mocked.assert_called_with(expected_url,
                                           headers=expected_headers,
                                           params={"limit": 100, "offset": 0},
                                           proxies={})
 
     @pytest.mark.parametrize(*query_data.test_ngd_query())
-    @mock.patch('requests.get')
+    @mock.patch('osdatahub.get')
     def test_ngd_api_call(self, request_mocked, extent, crs, start_datetime, end_datetime, cql_filter, filter_crs,
                           max_results, offset, expected_url, expected_params):
         request_mocked.return_value.configure_mock(json=lambda: {"features": [], "numberReturned": 0})
 
         ngd = NGD(key="API-KEY", collection="bld-fts-buildingline")
 
         ngd.query(extent=extent,
@@ -92,27 +92,27 @@
                   offset=offset
                 )
 
         assert len(results["features"]) == max_results
 
 
 class TestNGDGetCollections:
-    @mock.patch('requests.get')
+    @mock.patch('osdatahub.get')
     def test_ngd_get_collections(self, request_mocked):
         request_mocked.return_value.configure_mock(json=lambda: {})
         NGD.get_collections()
 
         request_mocked.assert_called_with("https://api.os.uk/features/ngd/ofa/v1/collections",
                                           proxies={})
 
 
 class TestNGDQueryFeature:
 
     @pytest.mark.parametrize(*query_data.test_ngd_query_feature())
-    @mock.patch('requests.get')
+    @mock.patch('osdatahub.get')
     def test_ngd_query_filter(self, request_mocked, feature_id, crs, expected_url, expected_params):
         request_mocked.return_value.configure_mock(json=lambda: {})
         ngd = NGD("api_key", "bld-fts-buildingline")
         ngd.query_feature(feature_id=feature_id, crs=crs)
 
         request_mocked.assert_called_with(expected_url,
                                           params=expected_params,
```

### Comparing `osdatahub-1.2.2/tests/test_places_api.py` & `osdatahub-1.2.3/tests/test_places_api.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.2/tests/test_utils.py` & `osdatahub-1.2.3/tests/test_utils.py`

 * *Files identical despite different names*

