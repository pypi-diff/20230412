# Comparing `tmp/asreview-1.1rc0.tar.gz` & `tmp/asreview-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asreview-1.1rc0.tar", last modified: Thu Oct 20 09:21:21 2022, max compression
+gzip compressed data, was "asreview-1.2.tar", last modified: Wed Apr 12 12:16:48 2023, max compression
```

## Comparing `asreview-1.1rc0.tar` & `asreview-1.2.tar`

### file list

```diff
@@ -1,179 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 09:21:21.329145 asreview-1.1rc0/
--rw-r--r--   0 runner    (1001) docker     (121)    11416 2022-10-20 09:18:48.000000 asreview-1.1rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-10-20 09:18:48.000000 asreview-1.1rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6767 2022-10-20 09:21:21.329145 asreview-1.1rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5668 2022-10-20 09:18:48.000000 asreview-1.1rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 09:21:21.329145 asreview-1.1rc0/asreview/
--rw-r--r--   0 runner    (1001) docker     (121)     1436 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3493 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      498 2022-10-20 09:21:21.329145 asreview-1.1rc0/asreview/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      987 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/compat.py
--rw-r--r--   0 runner    (1001) docker     (121)    13679 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 09:21:21.289145 asreview-1.1rc0/asreview/data/
--rw-r--r--   0 runner    (1001) docker     (121)      697 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16977 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/data/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     5078 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/data/statistics.py
--rw-r--r--   0 runner    (1001) docker     (121)    12584 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 09:21:21.289145 asreview-1.1rc0/asreview/entry_points/
--rw-r--r--   0 runner    (1001) docker     (121)     1019 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2432 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/entry_points/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (121)     3005 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/entry_points/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2791 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/entry_points/lab.py
--rw-r--r--   0 runner    (1001) docker     (121)    14907 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/entry_points/simulate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1888 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/entry_points/state_inspect.py
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 09:21:21.293145 asreview-1.1rc0/asreview/io/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/io/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1594 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/io/csv_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1556 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/io/csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1854 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/io/excel_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/io/excel_writer.py
--rw-r--r--   0 runner    (1001) docker     (121)     5761 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/io/paper_record.py
--rw-r--r--   0 runner    (1001) docker     (121)     6155 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/io/ris_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     3373 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/io/ris_writer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1557 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/io/tsv_writer.py
--rw-r--r--   0 runner    (1001) docker     (121)     7173 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 09:21:21.293145 asreview-1.1rc0/asreview/models/
--rw-r--r--   0 runner    (1001) docker     (121)     1442 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 09:21:21.297145 asreview-1.1rc0/asreview/models/balance/
--rw-r--r--   0 runner    (1001) docker     (121)     1510 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/models/balance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1336 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/models/balance/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     5911 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/models/balance/double.py
--rw-r--r--   0 runner    (1001) docker     (121)     1334 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/models/balance/simple.py
--rw-r--r--   0 runner    (1001) docker     (121)     8869 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/models/balance/triple.py
--rw-r--r--   0 runner    (1001) docker     (121)     2879 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/models/balance/undersample.py
--rw-r--r--   0 runner    (1001) docker     (121)     2089 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/models/balance/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2319 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 09:21:21.297145 asreview-1.1rc0/asreview/models/classifiers/
--rw-r--r--   0 runner    (1001) docker     (121)     1472 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/models/classifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2336 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/models/classifiers/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2162 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/models/classifiers/logistic.py
--rw-r--r--   0 runner    (1001) docker     (121)     8772 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/models/classifiers/lstm_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     8455 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/models/classifiers/lstm_pool.py
--rw-r--r--   0 runner    (1001) docker     (121)     1809 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/models/classifiers/nb.py
--rw-r--r--   0 runner    (1001) docker     (121)     7044 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/models/classifiers/nn_2_layer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2619 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/models/classifiers/rf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2540 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/models/classifiers/svm.py
--rw-r--r--   0 runner    (1001) docker     (121)     2302 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/models/classifiers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 09:21:21.297145 asreview-1.1rc0/asreview/models/feature_extraction/
--rw-r--r--   0 runner    (1001) docker     (121)     1463 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/models/feature_extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3336 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/models/feature_extraction/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     6195 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/models/feature_extraction/doc2vec.py
--rw-r--r--   0 runner    (1001) docker     (121)     4490 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/models/feature_extraction/embedding_idf.py
--rw-r--r--   0 runner    (1001) docker     (121)    13910 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/models/feature_extraction/embedding_lstm.py
--rw-r--r--   0 runner    (1001) docker     (121)     2704 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/models/feature_extraction/sbert.py
--rw-r--r--   0 runner    (1001) docker     (121)     2864 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/models/feature_extraction/tfidf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2156 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/models/feature_extraction/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 09:21:21.301145 asreview-1.1rc0/asreview/models/query/
--rw-r--r--   0 runner    (1001) docker     (121)     1360 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/models/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2201 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/models/query/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3875 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/models/query/cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/models/query/max.py
--rw-r--r--   0 runner    (1001) docker     (121)     7587 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/models/query/mixed.py
--rw-r--r--   0 runner    (1001) docker     (121)     1517 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/models/query/random.py
--rw-r--r--   0 runner    (1001) docker     (121)     1301 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/models/query/uncertainty.py
--rw-r--r--   0 runner    (1001) docker     (121)     2411 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/models/query/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    22591 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/project.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 09:21:21.301145 asreview-1.1rc0/asreview/review/
--rw-r--r--   0 runner    (1001) docker     (121)      708 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/review/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11612 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/review/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    12900 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/review/simulate.py
--rw-r--r--   0 runner    (1001) docker     (121)     4927 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/search.py
--rw-r--r--   0 runner    (1001) docker     (121)     6698 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 09:21:21.301145 asreview-1.1rc0/asreview/state/
--rw-r--r--   0 runner    (1001) docker     (121)      702 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10002 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/state/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      754 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/state/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 09:21:21.301145 asreview-1.1rc0/asreview/state/legacy/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/state/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10139 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/state/legacy/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     9164 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/state/legacy/dict.py
--rw-r--r--   0 runner    (1001) docker     (121)     8719 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/state/legacy/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (121)     2826 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/state/legacy/json.py
--rw-r--r--   0 runner    (1001) docker     (121)     5069 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/state/legacy/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    22111 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/state/sql_converter.py
--rw-r--r--   0 runner    (1001) docker     (121)    41594 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/state/sqlstate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1779 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/state/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1193 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     8596 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 09:21:21.305145 asreview-1.1rc0/asreview/webapp/
--rw-r--r--   0 runner    (1001) docker     (121)      611 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/webapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    50545 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/webapp/api.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 09:21:21.305145 asreview-1.1rc0/asreview/webapp/build/
--rw-r--r--   0 runner    (1001) docker     (121)     4981 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-10-20 09:19:25.000000 asreview-1.1rc0/asreview/webapp/build/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)     2200 2022-10-20 09:19:25.000000 asreview-1.1rc0/asreview/webapp/build/favicon.png
--rw-r--r--   0 runner    (1001) docker     (121)      645 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/index.html
--rw-r--r--   0 runner    (1001) docker     (121)      492 2022-10-20 09:19:25.000000 asreview-1.1rc0/asreview/webapp/build/manifest.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-10-20 09:19:25.000000 asreview-1.1rc0/asreview/webapp/build/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 09:21:21.285145 asreview-1.1rc0/asreview/webapp/build/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 09:21:21.305145 asreview-1.1rc0/asreview/webapp/build/static/css/
--rw-r--r--   0 runner    (1001) docker     (121)     7779 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/css/main.8d8848ef.css
--rw-r--r--   0 runner    (1001) docker     (121)    12861 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/css/main.8d8848ef.css.map
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 09:21:21.309145 asreview-1.1rc0/asreview/webapp/build/static/js/
--rw-r--r--   0 runner    (1001) docker     (121)  1715718 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/js/main.c677ac13.js
--rw-r--r--   0 runner    (1001) docker     (121)     3616 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/js/main.c677ac13.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)  6118169 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/js/main.c677ac13.js.map
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 09:21:21.325145 asreview-1.1rc0/asreview/webapp/build/static/media/
--rw-r--r--   0 runner    (1001) docker     (121)    12660 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/ElasArrowLeft.3d9f15d9fdee806647bd3e13441d5cc8.svg
--rw-r--r--   0 runner    (1001) docker     (121)    14569 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/ElasArrowRightAhead.e624bdd7c691c7c4f6c01604979c8f07.svg
--rw-r--r--   0 runner    (1001) docker     (121)      866 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/ElasAvatar.8a0563d4e3d6ec692e336e7a7c110681.svg
--rw-r--r--   0 runner    (1001) docker     (121)    13067 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/ElasBalloons.e6975dc66810b6a21cad819d7f24f57f.svg
--rw-r--r--   0 runner    (1001) docker     (121)     7379 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/ElasConstructionWorkerOrange.4bf29224b2f512bb75423d1a105c4d15.svg
--rw-r--r--   0 runner    (1001) docker     (121)    14918 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/ElasFinished.815b2578a515e2d1fe90d9c06d688d8a.svg
--rw-r--r--   0 runner    (1001) docker     (121)    16262 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/ElasFireMan.671424f0ee89c6d6b83f1b1005760ec8.svg
--rw-r--r--   0 runner    (1001) docker     (121)    10756 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/ElasGrad.292bca7f09713935c41e97671da92415.svg
--rw-r--r--   0 runner    (1001) docker     (121)    10625 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/ElasHoldingSIGNS_Finished.417f4491e95fc76527da3e41f6b8186f.svg
--rw-r--r--   0 runner    (1001) docker     (121)    10063 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/ElasHoldingSIGNS_InReview.04961844accfd3c20a598a03fc431550.svg
--rw-r--r--   0 runner    (1001) docker     (121)    10496 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/ElasHoldingSIGNS_SetUp.24349b7fcb5b6de52f962115b250798d.svg
--rw-r--r--   0 runner    (1001) docker     (121)    13322 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/ElasPotter.c22288229b5fdc4cd9badbf79547d3ea.svg
--rw-r--r--   0 runner    (1001) docker     (121)    17059 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/ElasWithDuck.fe3cb1f535ead738fdef4acb389470dd.svg
--rw-r--r--   0 runner    (1001) docker     (121)   127458 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/asreview_sub_logo_lab_black_transparent.c4e14af313ba97465fff113a6b2e4fd7.svg
--rw-r--r--   0 runner    (1001) docker     (121)   121638 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/asreview_sub_logo_lab_white_transparent.b5866b056964d8ef947a6518c50c56ea.svg
--rw-r--r--   0 runner    (1001) docker     (121)    34703 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/progress_relevant_dark.a065bb26815b228497fa.png
--rw-r--r--   0 runner    (1001) docker     (121)    26562 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/progress_relevant_light.2fe631e84c13a286bd9a.png
--rw-r--r--   0 runner    (1001) docker     (121)    20368 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/roboto-latin-100.a45108d3b34af91f9113.woff
--rw-r--r--   0 runner    (1001) docker     (121)    15808 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/roboto-latin-100.c2aa4ab115bf9c6057cb.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    21704 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/roboto-latin-100italic.451d4e559d6f57cdf6a1.woff
--rw-r--r--   0 runner    (1001) docker     (121)    17008 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/roboto-latin-100italic.7f839a8652da29745ce4.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    15784 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/roboto-latin-300.37a7069dc30fc663c878.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    20348 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/roboto-latin-300.865f928cbabcc9f8f2b5.woff
--rw-r--r--   0 runner    (1001) docker     (121)    22204 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/roboto-latin-300italic.bd5b7a13f2c52b531a2a.woff
--rw-r--r--   0 runner    (1001) docker     (121)    17448 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/roboto-latin-300italic.c64e7e354c88e613c77c.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    15736 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/roboto-latin-400.176f8f5bd5f02b3abfcf.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    20268 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/roboto-latin-400.49ae34d4cc6b98c00c69.woff
--rw-r--r--   0 runner    (1001) docker     (121)    21952 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/roboto-latin-400italic.b1d9d9904bfca8802a63.woff
--rw-r--r--   0 runner    (1001) docker     (121)    17324 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/roboto-latin-400italic.d022bc70dc1bf7b3425d.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    20464 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/roboto-latin-500.cea99d3e3e13a3a599a0.woff
--rw-r--r--   0 runner    (1001) docker     (121)    15872 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/roboto-latin-500.f5b74d7ffcdf85b9dd60.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    17316 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/roboto-latin-500italic.0d8bb5b3ee5f5dac9e44.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    22020 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/roboto-latin-500italic.18d00f739ff1e1c52db1.woff
--rw-r--r--   0 runner    (1001) docker     (121)    20356 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/roboto-latin-700.2267169ee7270a22a963.woff
--rw-r--r--   0 runner    (1001) docker     (121)    15816 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/roboto-latin-700.c18ee39fb002ad58b6dc.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    17020 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/roboto-latin-700italic.7d8125ff7f707231fd89.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    21588 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/roboto-latin-700italic.9360531f9bb817f917f0.woff
--rw-r--r--   0 runner    (1001) docker     (121)    15712 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/roboto-latin-900.870c8c1486f76054301a.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    20392 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/roboto-latin-900.bac8362e7a6ea60b6983.woff
--rw-r--r--   0 runner    (1001) docker     (121)    22304 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/roboto-latin-900italic.c20d916c1a1b094c1cec.woff
--rw-r--r--   0 runner    (1001) docker     (121)    17520 2022-10-20 09:21:20.000000 asreview-1.1rc0/asreview/webapp/build/static/media/roboto-latin-900italic.cb5ad999740e9d8a8bd1.woff2
--rw-r--r--   0 runner    (1001) docker     (121)     3114 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/webapp/io.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5395 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/webapp/run_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     3939 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/webapp/sqlock.py
--rw-r--r--   0 runner    (1001) docker     (121)     6809 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/webapp/start_flask.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 09:21:21.329145 asreview-1.1rc0/asreview/webapp/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      611 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/webapp/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      848 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/webapp/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     9825 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/webapp/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     6997 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/webapp/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (121)     1174 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/webapp/tests/test_webapp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1530 2022-10-20 09:18:48.000000 asreview-1.1rc0/asreview/webapp/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 09:21:21.289145 asreview-1.1rc0/asreview.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6767 2022-10-20 09:21:21.000000 asreview-1.1rc0/asreview.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7112 2022-10-20 09:21:21.000000 asreview-1.1rc0/asreview.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-20 09:21:21.000000 asreview-1.1rc0/asreview.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2154 2022-10-20 09:21:21.000000 asreview-1.1rc0/asreview.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      322 2022-10-20 09:21:21.000000 asreview-1.1rc0/asreview.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-10-20 09:21:21.000000 asreview-1.1rc0/asreview.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      619 2022-10-20 09:21:21.329145 asreview-1.1rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     7105 2022-10-20 09:18:48.000000 asreview-1.1rc0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    68612 2022-10-20 09:18:48.000000 asreview-1.1rc0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:16:48.939936 asreview-1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-04-12 12:14:46.000000 asreview-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-12 12:14:46.000000 asreview-1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-04-12 12:16:48.939936 asreview-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-04-12 12:14:46.000000 asreview-1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:16:48.939936 asreview-1.2/asreview/
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-12 12:14:46.000000 asreview-1.2/asreview/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-12 12:14:46.000000 asreview-1.2/asreview/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-12 12:16:48.939936 asreview-1.2/asreview/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-12 12:14:46.000000 asreview-1.2/asreview/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13679 2023-04-12 12:14:46.000000 asreview-1.2/asreview/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:16:48.931936 asreview-1.2/asreview/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-12 12:14:46.000000 asreview-1.2/asreview/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17122 2023-04-12 12:14:46.000000 asreview-1.2/asreview/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-04-12 12:14:46.000000 asreview-1.2/asreview/data/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12584 2023-04-12 12:14:46.000000 asreview-1.2/asreview/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:16:48.931936 asreview-1.2/asreview/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-12 12:14:46.000000 asreview-1.2/asreview/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-04-12 12:14:46.000000 asreview-1.2/asreview/entry_points/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-12 12:14:46.000000 asreview-1.2/asreview/entry_points/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-04-12 12:14:46.000000 asreview-1.2/asreview/entry_points/lab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15252 2023-04-12 12:14:46.000000 asreview-1.2/asreview/entry_points/simulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-12 12:14:46.000000 asreview-1.2/asreview/entry_points/state_inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-12 12:14:46.000000 asreview-1.2/asreview/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:16:48.935936 asreview-1.2/asreview/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-12 12:14:46.000000 asreview-1.2/asreview/io/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1594 2023-04-12 12:14:46.000000 asreview-1.2/asreview/io/csv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-04-12 12:14:46.000000 asreview-1.2/asreview/io/csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-12 12:14:46.000000 asreview-1.2/asreview/io/excel_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-12 12:14:46.000000 asreview-1.2/asreview/io/excel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-04-12 12:14:46.000000 asreview-1.2/asreview/io/paper_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-04-12 12:14:46.000000 asreview-1.2/asreview/io/ris_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-12 12:14:46.000000 asreview-1.2/asreview/io/ris_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-12 12:14:46.000000 asreview-1.2/asreview/io/tsv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-04-12 12:14:46.000000 asreview-1.2/asreview/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:16:48.935936 asreview-1.2/asreview/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-12 12:14:46.000000 asreview-1.2/asreview/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:16:48.935936 asreview-1.2/asreview/models/balance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-12 12:14:46.000000 asreview-1.2/asreview/models/balance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-12 12:14:46.000000 asreview-1.2/asreview/models/balance/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-04-12 12:14:46.000000 asreview-1.2/asreview/models/balance/double.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-12 12:14:46.000000 asreview-1.2/asreview/models/balance/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-04-12 12:14:46.000000 asreview-1.2/asreview/models/balance/triple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-04-12 12:14:46.000000 asreview-1.2/asreview/models/balance/undersample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-12 12:14:46.000000 asreview-1.2/asreview/models/balance/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-12 12:14:46.000000 asreview-1.2/asreview/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:16:48.935936 asreview-1.2/asreview/models/classifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-12 12:14:46.000000 asreview-1.2/asreview/models/classifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-04-12 12:14:46.000000 asreview-1.2/asreview/models/classifiers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-12 12:14:46.000000 asreview-1.2/asreview/models/classifiers/logistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-04-12 12:14:46.000000 asreview-1.2/asreview/models/classifiers/lstm_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-04-12 12:14:46.000000 asreview-1.2/asreview/models/classifiers/lstm_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-12 12:14:46.000000 asreview-1.2/asreview/models/classifiers/nb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-04-12 12:14:46.000000 asreview-1.2/asreview/models/classifiers/nn_2_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-12 12:14:46.000000 asreview-1.2/asreview/models/classifiers/rf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-12 12:14:46.000000 asreview-1.2/asreview/models/classifiers/svm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-04-12 12:14:46.000000 asreview-1.2/asreview/models/classifiers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:16:48.935936 asreview-1.2/asreview/models/feature_extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-12 12:14:46.000000 asreview-1.2/asreview/models/feature_extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-04-12 12:14:46.000000 asreview-1.2/asreview/models/feature_extraction/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-04-12 12:14:46.000000 asreview-1.2/asreview/models/feature_extraction/doc2vec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-04-12 12:14:46.000000 asreview-1.2/asreview/models/feature_extraction/embedding_idf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-04-12 12:14:46.000000 asreview-1.2/asreview/models/feature_extraction/embedding_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-12 12:14:46.000000 asreview-1.2/asreview/models/feature_extraction/sbert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-12 12:14:46.000000 asreview-1.2/asreview/models/feature_extraction/tfidf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-12 12:14:46.000000 asreview-1.2/asreview/models/feature_extraction/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:16:48.935936 asreview-1.2/asreview/models/query/
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-12 12:14:46.000000 asreview-1.2/asreview/models/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-04-12 12:14:46.000000 asreview-1.2/asreview/models/query/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-04-12 12:14:46.000000 asreview-1.2/asreview/models/query/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-12 12:14:46.000000 asreview-1.2/asreview/models/query/max.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-04-12 12:14:46.000000 asreview-1.2/asreview/models/query/mixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-12 12:14:46.000000 asreview-1.2/asreview/models/query/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-12 12:14:46.000000 asreview-1.2/asreview/models/query/uncertainty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-12 12:14:46.000000 asreview-1.2/asreview/models/query/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22689 2023-04-12 12:14:46.000000 asreview-1.2/asreview/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:16:48.935936 asreview-1.2/asreview/review/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-12 12:14:46.000000 asreview-1.2/asreview/review/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11612 2023-04-12 12:14:46.000000 asreview-1.2/asreview/review/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-04-12 12:14:46.000000 asreview-1.2/asreview/review/simulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-04-12 12:14:46.000000 asreview-1.2/asreview/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-04-12 12:14:46.000000 asreview-1.2/asreview/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:16:48.935936 asreview-1.2/asreview/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-12 12:14:46.000000 asreview-1.2/asreview/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10002 2023-04-12 12:14:46.000000 asreview-1.2/asreview/state/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-12 12:14:46.000000 asreview-1.2/asreview/state/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:16:48.939936 asreview-1.2/asreview/state/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:14:46.000000 asreview-1.2/asreview/state/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-04-12 12:14:46.000000 asreview-1.2/asreview/state/legacy/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-04-12 12:14:46.000000 asreview-1.2/asreview/state/legacy/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-04-12 12:14:46.000000 asreview-1.2/asreview/state/legacy/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-12 12:14:46.000000 asreview-1.2/asreview/state/legacy/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-04-12 12:14:46.000000 asreview-1.2/asreview/state/legacy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22111 2023-04-12 12:14:46.000000 asreview-1.2/asreview/state/sql_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42032 2023-04-12 12:14:46.000000 asreview-1.2/asreview/state/sqlstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-12 12:14:46.000000 asreview-1.2/asreview/state/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-12 12:14:46.000000 asreview-1.2/asreview/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-04-12 12:14:46.000000 asreview-1.2/asreview/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:16:48.939936 asreview-1.2/asreview/webapp/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-12 12:14:46.000000 asreview-1.2/asreview/webapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52683 2023-04-12 12:14:46.000000 asreview-1.2/asreview/webapp/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-12 12:14:46.000000 asreview-1.2/asreview/webapp/io.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5395 2023-04-12 12:14:46.000000 asreview-1.2/asreview/webapp/run_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-04-12 12:14:46.000000 asreview-1.2/asreview/webapp/sqlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-04-12 12:14:46.000000 asreview-1.2/asreview/webapp/start_flask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:16:48.939936 asreview-1.2/asreview/webapp/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-12 12:14:46.000000 asreview-1.2/asreview/webapp/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-12 12:14:46.000000 asreview-1.2/asreview/webapp/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-04-12 12:14:46.000000 asreview-1.2/asreview/webapp/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-04-12 12:14:46.000000 asreview-1.2/asreview/webapp/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-12 12:14:46.000000 asreview-1.2/asreview/webapp/tests/test_webapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-12 12:14:46.000000 asreview-1.2/asreview/webapp/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:16:48.931936 asreview-1.2/asreview.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-04-12 12:16:48.000000 asreview-1.2/asreview.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-12 12:16:48.000000 asreview-1.2/asreview.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 12:16:48.000000 asreview-1.2/asreview.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-12 12:16:48.000000 asreview-1.2/asreview.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-12 12:16:48.000000 asreview-1.2/asreview.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 12:16:48.000000 asreview-1.2/asreview.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-12 12:16:48.939936 asreview-1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-04-12 12:14:46.000000 asreview-1.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68612 2023-04-12 12:14:46.000000 asreview-1.2/versioneer.py
```

### Comparing `asreview-1.1rc0/LICENSE` & `asreview-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/PKG-INFO` & `asreview-1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: asreview
-Version: 1.1rc0
+Version: 1.2
 Summary: ASReview LAB - A tool for AI-assisted systematic reviews
 Home-page: https://github.com/asreview/asreview
 Author: ASReview LAB developers
 Author-email: asreview@uu.nl
 Project-URL: Bug Reports, https://github.com/asreview/asreview/issues
 Project-URL: Source, https://github.com/asreview/asreview/
-Keywords: systematic review machine-learning
+Keywords: systematic review,machine-learning
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -32,15 +32,16 @@
   <a href="https://github.com/asreview/asreview">
     <img width="60%" height="60%" src="https://raw.githubusercontent.com/asreview/asreview-artwork/master/LogoASReview/SVG/GitHub_Repo_Card_Transparent.svg">
   </a>
 </p>
 
 ## ASReview: Active learning for Systematic Reviews
 
-[![PyPI version](https://badge.fury.io/py/asreview.svg)](https://badge.fury.io/py/asreview) [![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fasreview%2Fasreview%2Fbadge%3Fref%3Dmaster&style=flat)](https://actions-badge.atrox.dev/asreview/asreview/goto?ref=master) [![Documentation Status](https://readthedocs.org/projects/asreview/badge/?version=latest)](https://asreview.readthedocs.io/en/latest/?badge=latest) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3345592.svg)](https://doi.org/10.5281/zenodo.3345592) [![Downloads](https://pepy.tech/badge/asreview)](https://github.com/asreview/asreview#installation) [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/4755/badge)](https://bestpractices.coreinfrastructure.org/projects/4755)
+[![PyPI version](https://badge.fury.io/py/asreview.svg)](https://badge.fury.io/py/asreview) [![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fasreview%2Fasreview%2Fbadge%3Fref%3Dmaster&style=flat)](https://actions-badge.atrox.dev/asreview/asreview/goto?ref=master) [![Documentation Status](https://readthedocs.org/projects/asreview/badge/?version=latest)](https://asreview.readthedocs.io/en/latest/?badge=latest) [![DOI](https://zenodo.org/badge/164874894.svg)](https://zenodo.org/badge/latestdoi/164874894)
+ [![Downloads](https://pepy.tech/badge/asreview)](https://github.com/asreview/asreview#installation) [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/4755/badge)](https://bestpractices.coreinfrastructure.org/projects/4755)
 
 Systematically screening large amounts of textual data is time-consuming and
 often tiresome. The rapidly evolving field of Artificial Intelligence (AI) has
 allowed the development of AI-aided pipelines that assist in finding relevant
 texts for search tasks. A well-established approach to increasing efficiency
 is screening prioritization via [Active
 Learning](https://asreview.readthedocs.io/en/latest/guides/activelearning.html).
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: asreview Version: 1.1rc0 Summary: ASReview LAB - A
+Metadata-Version: 2.1 Name: asreview Version: 1.2 Summary: ASReview LAB - A
 tool for AI-assisted systematic reviews Home-page: https://github.com/asreview/
 asreview Author: ASReview LAB developers Author-email: asreview@uu.nl Project-
 URL: Bug Reports, https://github.com/asreview/asreview/issues Project-URL:
-Source, https://github.com/asreview/asreview/ Keywords: systematic review
-machine-learning Classifier: Development Status :: 5 - Production/Stable
+Source, https://github.com/asreview/asreview/ Keywords: systematic
+review,machine-learning Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Classifier: Topic :: Scientific/
 Engineering :: Information Analysis Classifier: Topic :: Text Processing ::
 General Classifier: Framework :: Flask Requires-Python: ~=3.7 Description-
@@ -19,46 +19,46 @@
 ## ASReview: Active learning for Systematic Reviews [![PyPI version](https://
 badge.fury.io/py/asreview.svg)](https://badge.fury.io/py/asreview) [![Build
 Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-
 badge.atrox.dev%2Fasreview%2Fasreview%2Fbadge%3Fref%3Dmaster&style=flat)]
 (https://actions-badge.atrox.dev/asreview/asreview/goto?ref=master) [!
 [Documentation Status](https://readthedocs.org/projects/asreview/badge/
 ?version=latest)](https://asreview.readthedocs.io/en/latest/?badge=latest) [!
-[DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3345592.svg)](https://
-doi.org/10.5281/zenodo.3345592) [![Downloads](https://pepy.tech/badge/
-asreview)](https://github.com/asreview/asreview#installation) [![CII Best
-Practices](https://bestpractices.coreinfrastructure.org/projects/4755/badge)]
-(https://bestpractices.coreinfrastructure.org/projects/4755) Systematically
-screening large amounts of textual data is time-consuming and often tiresome.
-The rapidly evolving field of Artificial Intelligence (AI) has allowed the
-development of AI-aided pipelines that assist in finding relevant texts for
-search tasks. A well-established approach to increasing efficiency is screening
-prioritization via [Active Learning](https://asreview.readthedocs.io/en/latest/
-guides/activelearning.html). The Active learning for Systematic Reviews
-(ASReview) project, published in [*Nature Machine Intelligence*](https://
-doi.org/10.1038/s42256-020-00287-7) implements different machine learning
-algorithms that interactively query the researcher. ASReview LAB is designed to
-accelerate the step of screening textual data with a minimum of records to be
-read by a human with no or very few false negatives. ASReview LAB will save
-time, increase the quality of output and strengthen the transparency of work
-when screening large amounts of textual data to retrieve relevant information.
-Active Learning will support decision-making in any discipline or industry.
-ASReview software implements three different modes: - **Oracle** Screen textual
-data in interaction with the active learning model. The reviewer is the
-'oracle', making the labeling decisions. - **Exploration** Explore or
-demonstrate ASReview LAB with a completely labeled dataset. This mode is
-suitable for teaching purposes. - **Simulation** Evaluate the performance of
-active learning models on fully labeled data. Simulations can be run in
-ASReview LAB or via the command line interface with more advanced options. ##
-Installation The ASReview software requires Python 3.7+. Detailed step-by-step
-instructions to install Python and ASReview are available for [Windows](https:/
-/asreview.ai/installation-guide-windows/) and [macOS](https://asreview.ai/
-installation-guide-macos/) users. ```bash pip install asreview ``` Upgrade
-ASReview with the following command: ```bash pip install --upgrade asreview ```
-To install ASReview LAB with Docker, see [Install with Docker](https://
+[DOI](https://zenodo.org/badge/164874894.svg)](https://zenodo.org/badge/
+latestdoi/164874894) [![Downloads](https://pepy.tech/badge/asreview)](https://
+github.com/asreview/asreview#installation) [![CII Best Practices](https://
+bestpractices.coreinfrastructure.org/projects/4755/badge)](https://
+bestpractices.coreinfrastructure.org/projects/4755) Systematically screening
+large amounts of textual data is time-consuming and often tiresome. The rapidly
+evolving field of Artificial Intelligence (AI) has allowed the development of
+AI-aided pipelines that assist in finding relevant texts for search tasks. A
+well-established approach to increasing efficiency is screening prioritization
+via [Active Learning](https://asreview.readthedocs.io/en/latest/guides/
+activelearning.html). The Active learning for Systematic Reviews (ASReview)
+project, published in [*Nature Machine Intelligence*](https://doi.org/10.1038/
+s42256-020-00287-7) implements different machine learning algorithms that
+interactively query the researcher. ASReview LAB is designed to accelerate the
+step of screening textual data with a minimum of records to be read by a human
+with no or very few false negatives. ASReview LAB will save time, increase the
+quality of output and strengthen the transparency of work when screening large
+amounts of textual data to retrieve relevant information. Active Learning will
+support decision-making in any discipline or industry. ASReview software
+implements three different modes: - **Oracle** Screen textual data in
+interaction with the active learning model. The reviewer is the 'oracle',
+making the labeling decisions. - **Exploration** Explore or demonstrate
+ASReview LAB with a completely labeled dataset. This mode is suitable for
+teaching purposes. - **Simulation** Evaluate the performance of active learning
+models on fully labeled data. Simulations can be run in ASReview LAB or via the
+command line interface with more advanced options. ## Installation The ASReview
+software requires Python 3.7+. Detailed step-by-step instructions to install
+Python and ASReview are available for [Windows](https://asreview.ai/
+installation-guide-windows/) and [macOS](https://asreview.ai/installation-
+guide-macos/) users. ```bash pip install asreview ``` Upgrade ASReview with the
+following command: ```bash pip install --upgrade asreview ``` To install
+ASReview LAB with Docker, see [Install with Docker](https://
 asreview.readthedocs.io/en/latest/installation.html). ## How it works [!
 [ASReview LAB explained - animation](https://img.youtube.com/vi/k-a2SCq-LtA/
 0.jpg)](https://www.youtube.com/watch?v=k-a2SCq-LtA) ## Getting started
 [Getting Started with ASReview LAB](https://asreview.readthedocs.io/en/latest/
 about.html). [![ASReview LAB](https://github.com/asreview/asreview/blob/master/
 images/ASReviewWebApp.png?raw=true)](https://asreview.readthedocs.io/en/latest/
 lab/overview_lab.html "ASReview LAB") ## Citation The following publication in
```

### Comparing `asreview-1.1rc0/README.md` & `asreview-1.2/asreview.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,47 @@
+Metadata-Version: 2.1
+Name: asreview
+Version: 1.2
+Summary: ASReview LAB - A tool for AI-assisted systematic reviews
+Home-page: https://github.com/asreview/asreview
+Author: ASReview LAB developers
+Author-email: asreview@uu.nl
+Project-URL: Bug Reports, https://github.com/asreview/asreview/issues
+Project-URL: Source, https://github.com/asreview/asreview/
+Keywords: systematic review,machine-learning
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Text Processing :: General
+Classifier: Framework :: Flask
+Requires-Python: ~=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: sbert
+Provides-Extra: doc2vec
+Provides-Extra: tensorflow
+Provides-Extra: dev
+Provides-Extra: test
+Provides-Extra: all
+License-File: LICENSE
+
 <p align="center">
   <a href="https://github.com/asreview/asreview">
     <img width="60%" height="60%" src="https://raw.githubusercontent.com/asreview/asreview-artwork/master/LogoASReview/SVG/GitHub_Repo_Card_Transparent.svg">
   </a>
 </p>
 
 ## ASReview: Active learning for Systematic Reviews
 
-[![PyPI version](https://badge.fury.io/py/asreview.svg)](https://badge.fury.io/py/asreview) [![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fasreview%2Fasreview%2Fbadge%3Fref%3Dmaster&style=flat)](https://actions-badge.atrox.dev/asreview/asreview/goto?ref=master) [![Documentation Status](https://readthedocs.org/projects/asreview/badge/?version=latest)](https://asreview.readthedocs.io/en/latest/?badge=latest) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3345592.svg)](https://doi.org/10.5281/zenodo.3345592) [![Downloads](https://pepy.tech/badge/asreview)](https://github.com/asreview/asreview#installation) [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/4755/badge)](https://bestpractices.coreinfrastructure.org/projects/4755)
+[![PyPI version](https://badge.fury.io/py/asreview.svg)](https://badge.fury.io/py/asreview) [![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fasreview%2Fasreview%2Fbadge%3Fref%3Dmaster&style=flat)](https://actions-badge.atrox.dev/asreview/asreview/goto?ref=master) [![Documentation Status](https://readthedocs.org/projects/asreview/badge/?version=latest)](https://asreview.readthedocs.io/en/latest/?badge=latest) [![DOI](https://zenodo.org/badge/164874894.svg)](https://zenodo.org/badge/latestdoi/164874894)
+ [![Downloads](https://pepy.tech/badge/asreview)](https://github.com/asreview/asreview#installation) [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/4755/badge)](https://bestpractices.coreinfrastructure.org/projects/4755)
 
 Systematically screening large amounts of textual data is time-consuming and
 often tiresome. The rapidly evolving field of Artificial Intelligence (AI) has
 allowed the development of AI-aided pipelines that assist in finding relevant
 texts for search tasks. A well-established approach to increasing efficiency
 is screening prioritization via [Active
 Learning](https://asreview.readthedocs.io/en/latest/guides/activelearning.html).
@@ -23,21 +54,21 @@
 few false negatives. ASReview LAB will save time, increase the quality of
 output and strengthen the transparency of work when screening large amounts of
 textual data to retrieve relevant information. Active Learning will support 
 decision-making in any discipline or industry.
 
 ASReview software implements three different modes:
 
-- **Oracle** :crystal_ball: Screen textual data in
+- **Oracle**  Screen textual data in
   interaction with the active learning model. The reviewer is the 'oracle',
   making the labeling decisions.
-- **Exploration** :triangular_ruler: Explore or
+- **Exploration**  Explore or
   demonstrate ASReview LAB with a completely labeled dataset. This mode is
   suitable for teaching purposes.
-- **Simulation** :chart_with_upwards_trend: Evaluate
+- **Simulation**  Evaluate
   the performance of active learning models on fully labeled data. Simulations
   can be run in ASReview LAB or via the command line interface with more
   advanced options.
 
 
 ## Installation
```

#### html2text {}

```diff
@@ -1,43 +1,58 @@
+Metadata-Version: 2.1 Name: asreview Version: 1.2 Summary: ASReview LAB - A
+tool for AI-assisted systematic reviews Home-page: https://github.com/asreview/
+asreview Author: ASReview LAB developers Author-email: asreview@uu.nl Project-
+URL: Bug Reports, https://github.com/asreview/asreview/issues Project-URL:
+Source, https://github.com/asreview/asreview/ Keywords: systematic
+review,machine-learning Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Topic :: Scientific/
+Engineering :: Artificial Intelligence Classifier: Topic :: Scientific/
+Engineering :: Information Analysis Classifier: Topic :: Text Processing ::
+General Classifier: Framework :: Flask Requires-Python: ~=3.7 Description-
+Content-Type: text/markdown Provides-Extra: sbert Provides-Extra: doc2vec
+Provides-Extra: tensorflow Provides-Extra: dev Provides-Extra: test Provides-
+Extra: all License-File: LICENSE
      [https://raw.githubusercontent.com/asreview/asreview-artwork/master/
               LogoASReview/SVG/GitHub_Repo_Card_Transparent.svg]
 ## ASReview: Active learning for Systematic Reviews [![PyPI version](https://
 badge.fury.io/py/asreview.svg)](https://badge.fury.io/py/asreview) [![Build
 Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-
 badge.atrox.dev%2Fasreview%2Fasreview%2Fbadge%3Fref%3Dmaster&style=flat)]
 (https://actions-badge.atrox.dev/asreview/asreview/goto?ref=master) [!
 [Documentation Status](https://readthedocs.org/projects/asreview/badge/
 ?version=latest)](https://asreview.readthedocs.io/en/latest/?badge=latest) [!
-[DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3345592.svg)](https://
-doi.org/10.5281/zenodo.3345592) [![Downloads](https://pepy.tech/badge/
-asreview)](https://github.com/asreview/asreview#installation) [![CII Best
-Practices](https://bestpractices.coreinfrastructure.org/projects/4755/badge)]
-(https://bestpractices.coreinfrastructure.org/projects/4755) Systematically
-screening large amounts of textual data is time-consuming and often tiresome.
-The rapidly evolving field of Artificial Intelligence (AI) has allowed the
-development of AI-aided pipelines that assist in finding relevant texts for
-search tasks. A well-established approach to increasing efficiency is screening
-prioritization via [Active Learning](https://asreview.readthedocs.io/en/latest/
-guides/activelearning.html). The Active learning for Systematic Reviews
-(ASReview) project, published in [*Nature Machine Intelligence*](https://
-doi.org/10.1038/s42256-020-00287-7) implements different machine learning
-algorithms that interactively query the researcher. ASReview LAB is designed to
-accelerate the step of screening textual data with a minimum of records to be
-read by a human with no or very few false negatives. ASReview LAB will save
-time, increase the quality of output and strengthen the transparency of work
-when screening large amounts of textual data to retrieve relevant information.
-Active Learning will support decision-making in any discipline or industry.
-ASReview software implements three different modes: - **Oracle** :crystal_ball:
-Screen textual data in interaction with the active learning model. The reviewer
-is the 'oracle', making the labeling decisions. - **Exploration** :
-triangular_ruler: Explore or demonstrate ASReview LAB with a completely labeled
-dataset. This mode is suitable for teaching purposes. - **Simulation** :
-chart_with_upwards_trend: Evaluate the performance of active learning models on
-fully labeled data. Simulations can be run in ASReview LAB or via the command
-line interface with more advanced options. ## Installation The ASReview
+[DOI](https://zenodo.org/badge/164874894.svg)](https://zenodo.org/badge/
+latestdoi/164874894) [![Downloads](https://pepy.tech/badge/asreview)](https://
+github.com/asreview/asreview#installation) [![CII Best Practices](https://
+bestpractices.coreinfrastructure.org/projects/4755/badge)](https://
+bestpractices.coreinfrastructure.org/projects/4755) Systematically screening
+large amounts of textual data is time-consuming and often tiresome. The rapidly
+evolving field of Artificial Intelligence (AI) has allowed the development of
+AI-aided pipelines that assist in finding relevant texts for search tasks. A
+well-established approach to increasing efficiency is screening prioritization
+via [Active Learning](https://asreview.readthedocs.io/en/latest/guides/
+activelearning.html). The Active learning for Systematic Reviews (ASReview)
+project, published in [*Nature Machine Intelligence*](https://doi.org/10.1038/
+s42256-020-00287-7) implements different machine learning algorithms that
+interactively query the researcher. ASReview LAB is designed to accelerate the
+step of screening textual data with a minimum of records to be read by a human
+with no or very few false negatives. ASReview LAB will save time, increase the
+quality of output and strengthen the transparency of work when screening large
+amounts of textual data to retrieve relevant information. Active Learning will
+support decision-making in any discipline or industry. ASReview software
+implements three different modes: - **Oracle** Screen textual data in
+interaction with the active learning model. The reviewer is the 'oracle',
+making the labeling decisions. - **Exploration** Explore or demonstrate
+ASReview LAB with a completely labeled dataset. This mode is suitable for
+teaching purposes. - **Simulation** Evaluate the performance of active learning
+models on fully labeled data. Simulations can be run in ASReview LAB or via the
+command line interface with more advanced options. ## Installation The ASReview
 software requires Python 3.7+. Detailed step-by-step instructions to install
 Python and ASReview are available for [Windows](https://asreview.ai/
 installation-guide-windows/) and [macOS](https://asreview.ai/installation-
 guide-macos/) users. ```bash pip install asreview ``` Upgrade ASReview with the
 following command: ```bash pip install --upgrade asreview ``` To install
 ASReview LAB with Docker, see [Install with Docker](https://
 asreview.readthedocs.io/en/latest/installation.html). ## How it works [!
```

### Comparing `asreview-1.1rc0/asreview/__init__.py` & `asreview-1.2/asreview/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/compat.py` & `asreview-1.2/asreview/compat.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/config.py` & `asreview-1.2/asreview/config.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/data/__init__.py` & `asreview-1.2/asreview/data/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/data/base.py` & `asreview-1.2/asreview/data/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,19 +10,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import hashlib
 from pathlib import Path
+from urllib.error import HTTPError
 from urllib.parse import urlparse
 from urllib.request import urlopen
 
 import numpy as np
 import pandas as pd
+from pandas.api.types import is_object_dtype
 from pandas.api.types import is_string_dtype
 
 from asreview.config import COLUMN_DEFINITIONS
 from asreview.config import LABEL_NA
 from asreview.datasets import DatasetManager
 from asreview.datasets import DatasetNotFoundError
 from asreview.exceptions import BadFileFormatError
@@ -60,14 +62,34 @@
         pass
 
     # Could not find dataset, return None.
     raise FileNotFoundError(
         f"File, URL, or dataset does not exist: '{name}'")
 
 
+def _get_filename_from_url(url):
+
+    if not is_url(url):
+        raise ValueError(f"'{url}' is not a valid URL.")
+
+    if Path(urlparse(url).path).suffix:
+        return Path(urlparse(url).path).name, url
+    else:
+
+        try:
+            return urlopen(url).headers.get_filename(), url
+        except HTTPError as err:
+            # 308 (Permanent Redirect) not supported
+            # See https://bugs.python.org/issue40321
+            if err.code == 308:
+                return _get_filename_from_url(err.headers.get("Location"))
+            else:
+                raise err
+
+
 class ASReviewData():
     """Data object to the dataset with texts, labels, DOIs etc.
 
     Arguments
     ---------
     df: pandas.DataFrame
         Dataframe containing the data for the ASReview data object.
@@ -147,57 +169,47 @@
         else:
             texts = " ".join(self.texts)
         return hashlib.sha1(" ".join(texts).encode(
             encoding='UTF-8', errors='ignore')).hexdigest()
 
     @classmethod
     def from_file(cls, fp, reader=None):
-        """Create instance from csv/ris/excel file.
+        """Create instance from supported file format.
 
         It works in two ways; either manual control where the conversion
         functions are supplied or automatic, where it searches in the entry
         points for the right conversion functions.
 
         Arguments
         ---------
         fp: str, pathlib.Path
-            Read the data from this file.
+            Read the data from this file or url.
         reader: class
             Reader to import the file.
         """
-        if is_url(fp):
-            path = urlparse(fp).path
-        else:
-            path = str(Path(fp).resolve())
 
         if reader is not None:
             return cls(reader.read_data(fp))
 
-        entry_points = get_entry_points(entry_name="asreview.readers")
-
-        best_suffix = None
-
-        for suffix, entry in entry_points.items():
-            if path.endswith(suffix):
-                if best_suffix is None or len(suffix) > len(best_suffix):
-                    best_suffix = suffix
+        # get the filename from a url else file path
+        if is_url(fp):
+            fn, fp = _get_filename_from_url(fp)
+        else:
+            fn = Path(fp).name
 
-        if best_suffix is None and is_url(fp):
-            url_filename = urlopen(fp).info().get_filename()
-            for suffix, entry in entry_points.items():
-                if url_filename.endswith(suffix):
-                    if best_suffix is None or len(suffix) > len(best_suffix):
-                        best_suffix = suffix
+        entry_points = get_entry_points(entry_name="asreview.readers")
 
-        if best_suffix is None:
-            raise BadFileFormatError(f"Error importing file {fp}, no capabilities "
-                                     "for importing such a file.")
+        try:
+            reader = entry_points[Path(fn).suffix].load()
+        except Exception:
+            raise BadFileFormatError(
+                f"Importing file {fp} not possible.")
 
-        reader = entry_points[best_suffix].load()
         df, column_spec = reader.read_data(fp)
+
         return cls(df, column_spec=column_spec)
 
     def record(self, i, by_index=True):
         """Create a record from an index.
 
         Arguments
         ---------
@@ -474,15 +486,15 @@
         Returns
         -------
         pandas.Series
             Boolean series for each duplicated rows.
         """
         if pid in self.df.columns:
             # in case of strings, strip whitespaces and replace empty strings with None
-            if is_string_dtype(self.df[pid]):
+            if is_string_dtype(self.df[pid]) or is_object_dtype(self.df[pid]):
                 s_pid = self.df[pid].str.strip().replace("", None)
             else:
                 s_pid = self.df[pid]
 
             # save boolean series for duplicates based on persistent identifiers
             s_dups_pid = ((s_pid.duplicated()) & (s_pid.notnull()))
         else:
```

### Comparing `asreview-1.1rc0/asreview/data/statistics.py` & `asreview-1.2/asreview/data/statistics.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/datasets.py` & `asreview-1.2/asreview/datasets.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/entry_points/__init__.py` & `asreview-1.2/asreview/entry_points/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/entry_points/algorithms.py` & `asreview-1.2/asreview/entry_points/algorithms.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/entry_points/base.py` & `asreview-1.2/asreview/entry_points/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,56 +9,41 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import argparse
+import warnings
 from abc import ABC
 from abc import abstractclassmethod
 from argparse import RawTextHelpFormatter
 
-from asreview import __version__
+
+class DeprecateAction(argparse.Action):
+    def __call__(self, parser, namespace, values, option_string=None):
+        warnings.warn(f"Argument {self.option_strings} is deprecated and is ignored.")
+        delattr(namespace, self.dest)
 
 
 class BaseEntryPoint(ABC):
     """Base class for defining entry points."""
 
-    description = "Base Entry point."
-    extension_name = "asreview"
-    version = __version__
-
     @abstractclassmethod
     def execute(self, argv):
         """Perform the functionality of the entry point.
 
         Arguments
         ---------
         argv: list
             Argument list, with the entry point and program removed.
             For example, if `asreview plot X` is executed, then argv == ['X'].
         """
         raise NotImplementedError
 
-    def format(self, entry_name="?"):
-        """Create a short formatted description of the entry point.
-
-        Arguments
-        ---------
-        entry_name: str
-            Name of the entry point. For example 'plot' in `asreview plot X`
-        """
-        description = self.description
-        version = getattr(self, "version", "?")
-        extension_name = getattr(self, "extension_name", "?")
-
-        display_name = f"{entry_name} [{extension_name}-{version}]"
-
-        return f"{display_name}\n    {description}"
-
 
 def _base_parser(prog=None, description=None):
     """Argument parser for simulate.
 
     Parameters
     ----------
     mode : str
@@ -81,23 +66,8 @@
     parser.add_argument(
         "--embedding",
         type=str,
         default=None,
         dest='embedding_fp',
         help="File path of embedding matrix. Required for LSTM models."
     )
-    parser.add_argument(
-        "--config_file",
-        type=str,
-        default=None,
-        help="Configuration file with model settings"
-             "and parameter values."
-    )
-    parser.add_argument(
-        "--seed",
-        default=None,
-        type=int,
-        help="Seed for the model (classifiers, balance "
-             "strategies, feature extraction techniques, and query "
-             "strategies). Use an integer between 0 and 2^32 - 1."
-    )
     return parser
```

### Comparing `asreview-1.1rc0/asreview/entry_points/lab.py` & `asreview-1.2/asreview/entry_points/lab.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,19 +8,23 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import os
 from asreview.entry_points.base import BaseEntryPoint
+from asreview.entry_points.base import DeprecateAction
 from asreview.entry_points.base import _base_parser
 from asreview.webapp.run_model import main as main_run_model
 
-HOST_NAME = "localhost"
+HOST_NAME = os.getenv("ASREVIEW_HOST")
+if HOST_NAME is None:
+    HOST_NAME = "localhost"
 PORT_NUMBER = 5000
 
 
 def _lab_parser(prog="lab"):
     parser = _base_parser(
         prog=prog,
         description="""ASReview LAB - Active learning for Systematic Reviews."""  # noqa
@@ -74,22 +78,34 @@
 
     parser.add_argument(
         "--keyfile",
         default="",
         type=str,
         help="The full path to a private key file for usage with SSL/TLS.")
 
+    parser.add_argument(
+        "--config_file",
+        type=str,
+        default=None,
+        help="Deprecated, see subcommand simulate.",
+        action=DeprecateAction
+    )
+    parser.add_argument(
+        "--seed",
+        default=None,
+        type=int,
+        help="Deprecated, see subcommand simulate.",
+        action=DeprecateAction
+    )
     return parser
 
 
 class LABEntryPoint(BaseEntryPoint):
     """Entry point to start the ASReview LAB webapp."""
 
-    description = "The ASReview LAB webapp."
-
     def execute(self, argv):
 
         from asreview.webapp.start_flask import main
 
         main(argv)
```

### Comparing `asreview-1.1rc0/asreview/entry_points/simulate.py` & `asreview-1.2/asreview/entry_points/simulate.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,16 +87,14 @@
     elif verbose >= 2:
         logging.getLogger().setLevel(logging.DEBUG)
 
 
 class SimulateEntryPoint(BaseEntryPoint):
     """Entry point for simulation with ASReview LAB."""
 
-    description = "Simulate the performance of ASReview."
-
     def execute(self, argv):  # noqa
 
         # parse arguments
         parser = _simulate_parser()
         args = parser.parse_args(argv)
 
         # change the verbosity
@@ -340,14 +338,28 @@
     parser.add_argument(
         '--init_seed',
         default=None,
         type=int,
         help="Seed for setting the prior indices if the --prior_idx option is "
         "not used. If the option --prior_idx is used with one or more "
         "index, this option is ignored.")
+    parser.add_argument(
+        "--seed",
+        default=None,
+        type=int,
+        help="Seed for the model (classifiers, balance strategies, "
+             "feature extraction techniques, and query strategies)."
+    )
+    parser.add_argument(
+        "--config_file",
+        type=str,
+        default=None,
+        help="Configuration file with model settings"
+             "and parameter values."
+    )
     parser.add_argument("--n_instances",
                         default=DEFAULT_N_INSTANCES,
                         type=int,
                         help="Number of papers queried each query."
                         f"Default {DEFAULT_N_INSTANCES}.")
     parser.add_argument(
         "--n_queries",
@@ -373,12 +385,12 @@
                         type=int,
                         help="Verbosity")
     parser.add_argument(
         "--write_interval",
         "-w",
         default=None,
         type=int,
-        help="The simulation data will be written away after each set of this"
-        "many labeled records. By default only writes away data at the end"
+        help="The simulation data will be written after each set of this"
+        "many labeled records. By default only writes data at the end"
         "of the simulation to make it as fast as possible.")
 
     return parser
```

### Comparing `asreview-1.1rc0/asreview/entry_points/state_inspect.py` & `asreview-1.2/asreview/entry_points/state_inspect.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,45 +9,51 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import argparse
+from pathlib import Path
 
 import pandas as pd
 
 from asreview.entry_points.base import BaseEntryPoint
 from asreview.project import get_project_path
 from asreview.project import open_state
 
 
 def _parse_state_inspect_args():
 
     # parse arguments if available
     parser = argparse.ArgumentParser(prog="state-inspect",
                                      description="Inspect state file.")
-    parser.add_argument("project_id", type=str, help="Project_id or url.")
+    parser.add_argument(
+        "project_id",
+        type=str,
+        help="Project_id or path to ASReview file.")
     parser.add_argument(
         "table",
         type=str,
         help="Table to view (e.g. results, record_table, last_ranking).")
 
     return parser
 
 
 class StateInspectEntryPoint(BaseEntryPoint):
     """Entry point to inspect ASReview LAB review progress."""
-    description = "Inspect ASReview LAB review progress."
 
     def execute(self, argv):
         parser = _parse_state_inspect_args()
         args = parser.parse_args(argv)
 
-        project_path = get_project_path(args.project_id)
+        if Path(args.project_id).suffix == ".asreview":
+            project_path = args.project_id
+        else:
+            project_path = get_project_path(args.project_id)
 
         with open_state(project_path) as s:
             conn = s._connect_to_sql()
 
         df = pd.read_sql(f"select * from {args.table}", conn)
 
         if args.table == "results":
```

### Comparing `asreview-1.1rc0/asreview/exceptions.py` & `asreview-1.2/asreview/exceptions.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/io/__init__.py` & `asreview-1.2/asreview/io/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/io/csv_reader.py` & `asreview-1.2/asreview/io/csv_reader.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/io/csv_writer.py` & `asreview-1.2/asreview/io/csv_writer.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/io/excel_reader.py` & `asreview-1.2/asreview/io/excel_reader.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/io/excel_writer.py` & `asreview-1.2/asreview/io/excel_writer.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/io/paper_record.py` & `asreview-1.2/asreview/io/paper_record.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/io/ris_reader.py` & `asreview-1.2/asreview/io/ris_reader.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/io/ris_writer.py` & `asreview-1.2/asreview/io/ris_writer.py`

 * *Files 16% similar despite different names*

```diff
@@ -67,25 +67,22 @@
             for m in ["authors", "keywords", "notes"]:  # AU, KW, N1
                 # Check the "authors" - AU
                 try:
                     rec_copy[m] = eval(rec_copy[m])
                 except Exception:
                     rec_copy[m] = []
 
-            # Relevant records
-            if "included" in rec_copy and rec_copy["included"] == 1:
-                rec_copy["notes"].append("ASReview_relevant")
-            # Irrelevant records
-            elif "included" in rec_copy and rec_copy["included"] == 0:
-                rec_copy["notes"].append("ASReview_irrelevant")
-            # Not seen records
-            elif "included" in rec_copy and rec_copy["included"] == -1:
-                rec_copy["notes"].append("ASReview_not_seen")
-            else:
-                rec_copy["notes"].append("ASReview_not_seen")
+            # Get label for record if specified, if not specified set to -1
+            included = rec_copy.pop("included", -1)
+
+            # Map labels to notes
+            dict_note = {-1: "ASReview_not_seen",
+                         0: "ASReview_irrelevant",
+                         1: "ASReview_relevant"}
+            rec_copy["notes"].insert(0, dict_note[included])
 
             # Append the deepcopied and updated record to a new array
             records_new.append(rec_copy)
 
         # From buffered dataframe
         if fp is None:
             # Write the whole content to buffer
```

### Comparing `asreview-1.1rc0/asreview/io/tsv_writer.py` & `asreview-1.2/asreview/io/tsv_writer.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/io/utils.py` & `asreview-1.2/asreview/io/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,15 +23,30 @@
 from asreview.utils import _reader_class_from_entry_point
 from asreview.utils import _writer_class_from_entry_point
 from asreview.utils import list_reader_names
 from asreview.utils import list_writer_names
 
 
 def type_from_column(col_name, col_definitions):
-    """Transform a column name to its standardized form."""
+    """Transform a column name to its standardized form.
+
+    Arguments
+    ---------
+    col_name: str
+        Name of the column in the dataframe.
+    col_definitions: dict
+        Dictionary of {standardized_name: [list of possible names]}.
+        Ex. {"title": ["title", "primary_title"],
+            "authors": ["authors", "author names", "first_authors"]}
+
+    Returns
+    -------
+    str:
+        The standardized name. If it wasn't found, return None.
+    """
     for name, definition in col_definitions.items():
         if col_name.lower() in definition:
             return name
     return None
 
 
 def convert_keywords(keywords):
@@ -43,35 +58,14 @@
     for splitter in [", ", "; ", ": ", ";", ":"]:
         new_split = keywords.split(splitter)
         if len(new_split) > len(current_best):
             current_best = new_split
     return current_best
 
 
-def type_from_column_spec(col_name, column_spec):
-    """Retrieve the standardized name of a column.
-
-    Arguments
-    ---------
-    col_name: str
-        Name of the column in the dataframe.
-    column_spec: dict
-        Dictionary of {possible name}:{standardized_name}.
-
-    Returns
-    -------
-    str:
-        The standardized name. If it wasn't found, return None.
-    """
-    for data_type, column_spec_name in column_spec.items():
-        if col_name.lower() == column_spec_name.lower():
-            return data_type
-    return None
-
-
 def _is_record_id_unique(s):
 
     if len(pd.unique(s)) != len(s.index):
         raise ValueError("Column 'record_id' contains duplicate values.")
 
 
 def _is_record_id_notnull(s):
@@ -84,15 +78,15 @@
 
     try:
         pd.to_numeric(s).astype(int)
     except Exception:
         raise ValueError("Column 'record_id' should contain integer values.")
 
 
-def _standardize_dataframe(df, column_spec={}):
+def _standardize_dataframe(df, column_def={}):
     """Create a ASReview readable dataframe.
 
     The main purpose is to rename columns with slightly different names;
     'authors' vs 'first_authors', etc. This greatly widens the compatibility
     with different datasets.
 
     Arguments
@@ -109,54 +103,58 @@
 
     # remove whitespace from colnames
     df.columns = df.columns.str.strip()
 
     # map columns on column specification
     col_names = list(df)
     for column_name in col_names:
-        # First try the supplied column specifications if supplied.
-        data_type = type_from_column_spec(column_name, column_spec)
+        # First try the custom column definitions if supplied.
+        data_type = type_from_column(column_name, column_def)
         if data_type is not None:
             all_column_spec[data_type] = column_name
             continue
         # Then try the standard specifications in ASReview.
         data_type = type_from_column(column_name, COLUMN_DEFINITIONS)
         if data_type is not None:
             all_column_spec[data_type] = column_name
 
     # Check if we either have abstracts or titles.
     col_names = list(all_column_spec)
     if "abstract" not in col_names and "title" not in col_names:
-        raise BadFileFormatError("File supplied without 'abstract' or 'title'"
-                                 " fields.")
+        raise BadFileFormatError(
+            "File supplied without 'abstract' or 'title'" " fields."
+        )
     if "abstract" not in col_names:
         logging.warning("Unable to detect abstracts in dataset.")
     if "title" not in col_names:
         logging.warning("Unable to detect titles in dataset.")
 
     # Replace NA values with empty strings.
     for col in ["title", "abstract", "authors", "keywords", "notes"]:
         try:
             df[all_column_spec[col]] = np.where(
                 pd.isnull(df[all_column_spec[col]]),
-                "", df[all_column_spec[col]].astype(str))
+                "",
+                df[all_column_spec[col]].astype(str),
+            )
         except KeyError:
             pass
 
     # Convert labels to integers.
     if "included" in col_names:
         try:
             col = all_column_spec["included"]
             df[col].fillna(LABEL_NA, inplace=True)
             df[col] = pd.to_numeric(df[col])
         except KeyError:
             pass
         except ValueError:
-            logging.warning("Failed to parse label column name, no labels will"
-                            " be present.")
+            logging.warning(
+                "Failed to parse label column name, no labels will" " be present."
+            )
             df.rename(columns={"label": "included"})
             all_column_spec.pop("included")
 
     # TODO: Make sure 'record_id' column in original dataset does not get overwritten.
     # # If the we have a record_id (for example from an ASReview export) use it.
     # if "record_id" in list(df):
     #
@@ -167,15 +165,15 @@
     #
     # # Create a new index if we haven't found it in the data.
     # else:
     #     df["record_id"] = np.arange(len(df.index))
     df["record_id"] = np.arange(len(df.index))
 
     # set the index
-    df.set_index('record_id', inplace=True)
+    df.set_index("record_id", inplace=True)
 
     return df, all_column_spec
 
 
 def list_readers():
     """List available dataset reader classes.
 
@@ -217,17 +215,15 @@
         Name of the dataset reader, e.g. '.csv', '.tsv' or '.xlsx'.
 
     Returns
     -------
     class:
         Class corresponding to the name.
     """
-    return _reader_class_from_entry_point(
-        name,
-        entry_name="asreview.readers")
+    return _reader_class_from_entry_point(name, entry_name="asreview.readers")
 
 
 def get_writer_class(name):
     """Get class of dataset writer from string.
 
     Arguments
     ---------
@@ -235,10 +231,8 @@
         Name of the dataset writer, e.g. '.csv', '.tsv' or '.xlsx'.
 
     Returns
     -------
     class:
         Class corresponding to the name.
     """
-    return _writer_class_from_entry_point(
-        name,
-        entry_name="asreview.writers")
+    return _writer_class_from_entry_point(name, entry_name="asreview.writers")
```

### Comparing `asreview-1.1rc0/asreview/models/__init__.py` & `asreview-1.2/asreview/models/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/models/balance/__init__.py` & `asreview-1.2/asreview/models/balance/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/models/balance/base.py` & `asreview-1.2/asreview/models/balance/base.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/models/balance/double.py` & `asreview-1.2/asreview/models/balance/double.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/models/balance/simple.py` & `asreview-1.2/asreview/models/balance/simple.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/models/balance/triple.py` & `asreview-1.2/asreview/models/balance/triple.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/models/balance/undersample.py` & `asreview-1.2/asreview/models/balance/undersample.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/models/balance/utils.py` & `asreview-1.2/asreview/models/balance/utils.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/models/base.py` & `asreview-1.2/asreview/models/base.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/models/classifiers/__init__.py` & `asreview-1.2/asreview/models/classifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/models/classifiers/base.py` & `asreview-1.2/asreview/models/classifiers/base.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/models/classifiers/logistic.py` & `asreview-1.2/asreview/models/classifiers/logistic.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/models/classifiers/lstm_base.py` & `asreview-1.2/asreview/models/classifiers/lstm_base.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/models/classifiers/lstm_pool.py` & `asreview-1.2/asreview/models/classifiers/lstm_pool.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/models/classifiers/nb.py` & `asreview-1.2/asreview/models/classifiers/nb.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/models/classifiers/nn_2_layer.py` & `asreview-1.2/asreview/models/classifiers/nn_2_layer.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/models/classifiers/rf.py` & `asreview-1.2/asreview/models/classifiers/rf.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/models/classifiers/svm.py` & `asreview-1.2/asreview/models/classifiers/svm.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/models/classifiers/utils.py` & `asreview-1.2/asreview/models/classifiers/utils.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/models/feature_extraction/__init__.py` & `asreview-1.2/asreview/models/feature_extraction/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/models/feature_extraction/base.py` & `asreview-1.2/asreview/models/feature_extraction/base.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/models/feature_extraction/doc2vec.py` & `asreview-1.2/asreview/models/feature_extraction/doc2vec.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/models/feature_extraction/embedding_idf.py` & `asreview-1.2/asreview/models/feature_extraction/embedding_idf.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/models/feature_extraction/embedding_lstm.py` & `asreview-1.2/asreview/models/feature_extraction/embedding_lstm.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/models/feature_extraction/sbert.py` & `asreview-1.2/asreview/models/feature_extraction/sbert.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/models/feature_extraction/tfidf.py` & `asreview-1.2/asreview/models/feature_extraction/tfidf.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/models/feature_extraction/utils.py` & `asreview-1.2/asreview/models/feature_extraction/utils.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/models/query/__init__.py` & `asreview-1.2/asreview/models/query/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/models/query/base.py` & `asreview-1.2/asreview/models/query/base.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/models/query/cluster.py` & `asreview-1.2/asreview/models/query/cluster.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/models/query/max.py` & `asreview-1.2/asreview/models/query/max.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/models/query/mixed.py` & `asreview-1.2/asreview/models/query/mixed.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/models/query/random.py` & `asreview-1.2/asreview/models/query/random.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/models/query/uncertainty.py` & `asreview-1.2/asreview/models/query/uncertainty.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/models/query/utils.py` & `asreview-1.2/asreview/models/query/utils.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/project.py` & `asreview-1.2/asreview/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -664,15 +664,17 @@
                 zip_filenames = zip_obj.namelist()
 
                 # raise error if no ASReview project file
                 if PATH_PROJECT_CONFIG not in zip_filenames:
                     raise ValueError("Project file is not valid project.")
 
                 # extract all files to folder
-                zip_obj.extractall(path=tmpdir)
+                for f in zip_filenames:
+                    if not f.endswith(".pickle"):
+                        zip_obj.extract(f, path=tmpdir)
 
         except zipfile.BadZipFile:
             raise ValueError("File is not an ASReview file.")
 
         with open(Path(tmpdir, PATH_PROJECT_CONFIG), "r") as f:
             project_config = json.load(f)
```

### Comparing `asreview-1.1rc0/asreview/review/__init__.py` & `asreview-1.2/asreview/review/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/review/base.py` & `asreview-1.2/asreview/review/base.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/review/simulate.py` & `asreview-1.2/asreview/review/simulate.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
     init_seed: int
         Seed for setting the prior indices if the --prior_idx option is
         not used. If the option prior_idx is used with one or more
         index, this option is ignored.
     state_file: str
         Path to state file.
     write_interval: int
-        After how many labeled records to write away the simulation data to the
+        After how many labeled records to write the simulation data to the
         state.
     """
 
     name = "simulate"
 
     def __init__(self,
                  as_data,
@@ -308,15 +308,15 @@
         if (self.write_interval is not None) and \
                 (len(self.results) >= self.write_interval):
             self._write_to_state()
 
         return labels
 
     def _write_to_state(self):
-        """Write the data that has not yet been written away to the state."""
+        """Write the data that has not yet been written to the state."""
         # Write the data to the state.
         if len(self.results) > 0:
             rows = [tuple(self.results.iloc[i])
                     for i in range(len(self.results))]
             with open_state(self.project, read_only=False) as state:
                 state._add_labeling_data_simulation_mode(rows)
```

### Comparing `asreview-1.1rc0/asreview/search.py` & `asreview-1.2/asreview/search.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/settings.py` & `asreview-1.2/asreview/settings.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/state/__init__.py` & `asreview-1.2/asreview/state/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/state/base.py` & `asreview-1.2/asreview/state/base.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/state/errors.py` & `asreview-1.2/asreview/state/errors.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/state/legacy/base.py` & `asreview-1.2/asreview/state/legacy/base.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/state/legacy/dict.py` & `asreview-1.2/asreview/state/legacy/dict.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/state/legacy/hdf5.py` & `asreview-1.2/asreview/state/legacy/hdf5.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/state/legacy/json.py` & `asreview-1.2/asreview/state/legacy/json.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/state/legacy/utils.py` & `asreview-1.2/asreview/state/legacy/utils.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/state/sql_converter.py` & `asreview-1.2/asreview/state/sql_converter.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/state/sqlstate.py` & `asreview-1.2/asreview/state/sqlstate.py`

 * *Files 1% similar despite different names*

```diff
@@ -419,15 +419,17 @@
         """
         record_sql_input = [(int(record_id), ) for record_id in record_ids]
 
         con = self._connect_to_sql()
         cur = con.cursor()
         cur.execute("DELETE FROM record_table")
         cur.executemany(
-            """INSERT INTO record_table VALUES (?)""", record_sql_input)
+            "INSERT INTO record_table (record_id) VALUES (?)",
+            record_sql_input
+        )
         con.commit()
 
     def add_last_probabilities(self, probabilities):
         """Save the probabilities produced by the last classifier.
 
         Arguments
         ---------
@@ -446,16 +448,17 @@
         if not ((proba_length == 0) or (proba_length == len(proba_sql_input))):
             raise ValueError(
                 f"There are {proba_length} probabilities in the database, "
                 f"but 'probabilities' has length {len(probabilities)}")
 
         cur.execute("""DELETE FROM last_probabilities""")
         cur.executemany(
-            """INSERT INTO last_probabilities VALUES
-                                            (?)""", proba_sql_input)
+            "INSERT INTO last_probabilities (proba) VALUES (?)",
+            proba_sql_input
+        )
         con.commit()
 
     def add_last_ranking(self, ranked_record_ids, classifier, query_strategy,
                          balance_strategy, feature_extraction, training_set):
         """Save the ranking of the last iteration of the model.
 
         Save the ranking of the last iteration of the model, in the ranking
@@ -496,16 +499,19 @@
                     feature_extractions[i], training_sets[i], ranking_times[i])
                    for i in range(len(record_ids))]
 
         con = self._connect_to_sql()
         cur = con.cursor()
         cur.execute("DELETE FROM last_ranking")
         cur.executemany(
-            """INSERT INTO last_ranking VALUES
-                                    (?, ?, ?, ?, ?, ?, ?, ?)""", db_rows)
+            ("INSERT INTO last_ranking (record_id, ranking, classifier, "
+             "query_strategy, balance_strategy, feature_extraction, "
+             "training_set, time) VALUES (?, ?, ?, ?, ?, ?, ?, ?)"),
+            db_rows
+        )
         con.commit()
         con.close()
 
         # If it's the first ranking table to be added, set model_has_trained.
         if not self.model_has_trained:
             self._add_settings_metadata('model_has_trained', True)
 
@@ -605,15 +611,18 @@
         Arguments
         ----------
         rows : list of tuples
             List of tuples (record_id: int, label: int, classifier: str,
             query_strategy: str, balance_strategy: str, feature_extraction: str,
              training_set: int, labeling_time: int, notes: str).
         """
-        query = "INSERT INTO results VALUES (?, ?, ?, ?, ?, ?, ?, ?, ?)"
+        query = ("INSERT INTO results (record_id, label, classifier, "
+                 "query_strategy, balance_strategy, feature_extraction, "
+                 "training_set, labeling_time, notes) "
+                 "VALUES (?, ?, ?, ?, ?, ?, ?, ?, ?)")
 
         con = self._connect_to_sql()
         cur = con.cursor()
         cur.executemany(query, rows)
         con.commit()
         con.close()
 
@@ -634,16 +643,19 @@
         cur = con.cursor()
 
         # Change the label.
         cur.execute("UPDATE results SET label = ?, notes = ? "
                     "WHERE record_id = ?", (label, note, record_id))
 
         # Add the change to the decision changes table.
-        cur.execute("INSERT INTO decision_changes VALUES (?,?, ?)",
-                    (record_id, label, datetime.now()))
+        cur.execute(
+            ("INSERT INTO decision_changes (record_id, new_label, time) "
+             "VALUES (?, ?, ?)"),
+            (record_id, label, datetime.now())
+        )
 
         con.commit()
         con.close()
 
     def delete_record_labeling_data(self, record_id):
         """Delete the labeling data for the given record id.
 
@@ -656,16 +668,19 @@
         current_time = datetime.now()
 
         con = self._connect_to_sql()
         cur = con.cursor()
         cur.execute('DELETE FROM results WHERE record_id=?', (record_id, ))
 
         # Add the change to the decision changes table.
-        cur.execute("INSERT INTO decision_changes VALUES (?,?, ?)",
-                    (record_id, None, current_time))
+        cur.execute(
+            ("INSERT INTO decision_changes (record_id, new_label, time) "
+             "VALUES (?,?, ?)"),
+            (record_id, None, current_time)
+        )
         con.commit()
         con.close()
 
     def get_decision_changes(self):
         """Get the record ids for any decision changes.
 
         Get the record ids of the records whose labels have been changed
```

### Comparing `asreview-1.1rc0/asreview/state/utils.py` & `asreview-1.2/asreview/state/utils.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/types.py` & `asreview-1.2/asreview/types.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/utils.py` & `asreview-1.2/asreview/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,21 +269,18 @@
     Parameters
     ----------
     random_state: int, numpy.RandomState
         If it is an integer, seed a new random state.
         If it is a RandomState, return it (nop).
         If it is None, return the random state of numpy.
     """
-    if random_state is None:
-        return np.random.random.__self__
-    else:
-        if isinstance(random_state, np.random.RandomState):
-            return random_state
-        else:
-            return np.random.RandomState(
-                random_state % (2**32))
+
+    if not isinstance(random_state, np.random.RandomState):
+        return np.random.RandomState(random_state)
+
+    return random_state
 
 
 def _get_executable():
     """Get the Python executable"""
 
     return sys.executable if sys.executable else 'python'
```

### Comparing `asreview-1.1rc0/asreview/webapp/__init__.py` & `asreview-1.2/asreview/webapp/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/webapp/api.py` & `asreview-1.2/asreview/webapp/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 # limitations under the License.
 
 import json
 import logging
 import shutil
 import subprocess
 import tempfile
-import urllib.parse
 from pathlib import Path
 from urllib.request import urlretrieve
 
+import datahugger
 from flask import Blueprint
 from flask import abort
 from flask import jsonify
 from flask import request
 from flask import send_file
 from flask_cors import CORS
 import numpy as np
@@ -35,14 +35,15 @@
 from asreview.config import DEFAULT_BALANCE_STRATEGY
 from asreview.config import DEFAULT_FEATURE_EXTRACTION
 from asreview.config import DEFAULT_MODEL
 from asreview.config import DEFAULT_QUERY_STRATEGY
 from asreview.config import PROJECT_MODE_EXPLORE
 from asreview.config import PROJECT_MODE_SIMULATE
 from asreview.data import ASReviewData
+from asreview.data.base import _get_filename_from_url
 from asreview.data.statistics import n_duplicates
 from asreview.datasets import DatasetManager
 from asreview.exceptions import BadFileFormatError
 from asreview.io import list_readers
 from asreview.io import list_writers
 from asreview.models.balance import get_balance_model
 from asreview.models.balance import list_balance_strategies
@@ -66,14 +67,15 @@
 from asreview.settings import ASReviewSettings
 from asreview.state.errors import StateError
 from asreview.state.errors import StateNotFoundError
 from asreview.state.sql_converter import upgrade_asreview_project_file
 from asreview.state.sql_converter import upgrade_project_config
 from asreview.utils import _get_executable
 from asreview.utils import asreview_path
+from asreview.utils import list_reader_names
 from asreview.webapp.io import read_data
 
 bp = Blueprint('api', __name__, url_prefix='/api')
 CORS(bp, resources={r"*": {"origins": "*"}})
 
 # error handlers
 
@@ -82,14 +84,22 @@
 def project_not_found(e):
 
     message = str(e) if str(e) else "Project not found."
     logging.error(message)
     return jsonify(message=message), 400
 
 
+@bp.errorhandler(ValueError)
+def value_error(e):
+
+    message = str(e) if str(e) else "Incorrect value."
+    logging.error(message)
+    return jsonify(message=message), 400
+
+
 @bp.errorhandler(InternalServerError)
 def error_500(e):
     original = getattr(e, "original_exception", None)
 
     if original is None or str(e.original_exception) == "":
         # direct 500 error, such as abort(500)
         logging.error(e)
@@ -308,38 +318,57 @@
         project.remove_dataset()
 
     # create dataset folder if not present
     Path(project.project_path, "data").mkdir(exist_ok=True)
 
     if request.form.get('plugin', None):
         url = DatasetManager().find(request.form['plugin']).filepath
+        filename, url = _get_filename_from_url(url)
 
     if request.form.get('benchmark', None):
         url = DatasetManager().find(request.form['benchmark']).filepath
+        filename, url = _get_filename_from_url(url)
 
     if request.form.get('url', None):
-        url = request.form['url']
 
-    if request.form.get('plugin', None) or request.form.get(
-            'benchmark', None) or request.form.get('url', None):
-        try:
-            url_parts = urllib.parse.urlparse(url)
-            filename = secure_filename(url_parts.path.rsplit('/', 1)[-1])
+        url = request.form.get('url')
 
-            urlretrieve(url, Path(project.project_path, "data") / filename)
+        # check if url value is actually DOI without netloc
+        if url.startswith("10."):
+            url = f"https://doi.org/{url}"
 
-        except ValueError as err:
+        filename, url = _get_filename_from_url(url)
 
-            logging.error(err)
-            message = f"Invalid URL '{url}'."
+        if bool(request.form.get('validate', None)):
 
-            if isinstance(url, str) and not url.startswith("http"):
-                message += " Usually, the URL starts with 'http' or 'https'."
+            reader_keys = list_reader_names()
 
-            return jsonify(message=message), 400
+            if filename and Path(filename).suffix and \
+                    Path(filename).suffix in reader_keys:
+                return jsonify(files=[{"link": url, "name": filename}]), 201
+            elif filename and not Path(filename).suffix:
+                raise BadFileFormatError("Can't determine file format.")
+            else:
+                try:
+                    # get file list from datahugger
+                    dh = datahugger.info(url)
+                    files = dh.files.copy()
+
+                    for i, f in enumerate(files):
+                        files[i]["disabled"] = Path(
+                            files[i]["name"]).suffix not in reader_keys
+
+                    return jsonify(files=files), 201
+                except Exception:
+                    raise BadFileFormatError("Can't retrieve files.")
+
+    if request.form.get('plugin', None) or request.form.get(
+            'benchmark', None) or request.form.get('url', None):
+        try:
+            urlretrieve(url, Path(project.project_path, "data") / filename)
 
         except Exception as err:
 
             logging.error(err)
             message = f"Can't retrieve data from URL {url}."
 
             return jsonify(message=message), 400
@@ -1117,42 +1146,73 @@
 @bp.route('/projects/<project_id>/export_dataset', methods=["GET"])
 @project_from_id
 def api_export_dataset(project):
     """Export dataset with relevant/irrelevant labels"""
 
     # get the export args
     file_format = request.args.get("file_format", None)
+    dataset_label = request.args.get("dataset_label", default="all")
 
     # create temporary folder to store exported dataset
-    tmp_path = tempfile.TemporaryDirectory(dir=project.project_path)
+    tmp_path = tempfile.TemporaryDirectory()
     tmp_path_dataset = Path(tmp_path.name, f"export_dataset.{file_format}")
 
     try:
         # get labels and ranking from state file
         with open_state(project.project_path) as s:
             pool, labeled, pending = s.get_pool_labeled_pending()
+            # get state dataset for accessing notes
+            state_df = s.get_dataset().set_index("record_id")
 
         included = labeled[labeled['label'] == 1]
         excluded = labeled[labeled['label'] != 1]
-        export_order = included['record_id'].to_list() + \
-            pending.to_list() + \
-            pool.to_list() + \
-            excluded['record_id'].to_list()
+
+        if dataset_label == "relevant":
+            export_order = included['record_id'].to_list()
+            labeled = included
+        else:
+            export_order = included['record_id'].to_list() + \
+                pending.to_list() + \
+                pool.to_list() + \
+                excluded['record_id'].to_list()
 
         # get writer corresponding to specified file format
         writers = list_writers()
         writer = None
         for c in writers:
             if writer is None:
                 if c.name == file_format:
                     writer = c
 
         # read the dataset into a ASReview data object
         as_data = read_data(project)
 
+        # Adding Notes from State file to the exported dataset
+        # Check if exported_notes column already exists due to multiple screenings
+        screening = 0
+        for col in as_data.df:
+            if col == "exported_notes":
+                screening = 0
+            elif col.startswith("exported_notes"):
+                try:
+                    screening = int(col.split("_")[2])
+                except IndexError:
+                    screening = 0
+        screening += 1
+
+        state_df.rename(
+            columns={"notes": f"exported_notes_{screening}", },
+            inplace=True,
+        )
+
+        as_data.df = as_data.df.join(
+            state_df[f"exported_notes_{screening}"],
+            on="record_id"
+        )
+
         as_data.to_file(
             fp=tmp_path_dataset,
             labels=labeled.values.tolist(),
             ranking=export_order,
             writer=writer)
 
         return send_file(
```

### Comparing `asreview-1.1rc0/asreview/webapp/io.py` & `asreview-1.2/asreview/webapp/io.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/webapp/run_model.py` & `asreview-1.2/asreview/webapp/run_model.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/webapp/sqlock.py` & `asreview-1.2/asreview/webapp/sqlock.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/webapp/start_flask.py` & `asreview-1.2/asreview/webapp/start_flask.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/webapp/tests/__init__.py` & `asreview-1.2/asreview/webapp/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/webapp/tests/conftest.py` & `asreview-1.2/asreview/webapp/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/webapp/tests/test_api.py` & `asreview-1.2/asreview/webapp/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/webapp/tests/test_project.py` & `asreview-1.2/asreview/webapp/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/webapp/tests/test_webapp.py` & `asreview-1.2/asreview/webapp/tests/test_webapp.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview/webapp/tests/utils.py` & `asreview-1.2/asreview/webapp/tests/utils.py`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/asreview.egg-info/PKG-INFO` & `asreview-1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,17 @@
-Metadata-Version: 2.1
-Name: asreview
-Version: 1.1rc0
-Summary: ASReview LAB - A tool for AI-assisted systematic reviews
-Home-page: https://github.com/asreview/asreview
-Author: ASReview LAB developers
-Author-email: asreview@uu.nl
-Project-URL: Bug Reports, https://github.com/asreview/asreview/issues
-Project-URL: Source, https://github.com/asreview/asreview/
-Keywords: systematic review machine-learning
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Text Processing :: General
-Classifier: Framework :: Flask
-Requires-Python: ~=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: sbert
-Provides-Extra: doc2vec
-Provides-Extra: tensorflow
-Provides-Extra: dev
-Provides-Extra: test
-Provides-Extra: all
-License-File: LICENSE
-
 <p align="center">
   <a href="https://github.com/asreview/asreview">
     <img width="60%" height="60%" src="https://raw.githubusercontent.com/asreview/asreview-artwork/master/LogoASReview/SVG/GitHub_Repo_Card_Transparent.svg">
   </a>
 </p>
 
 ## ASReview: Active learning for Systematic Reviews
 
-[![PyPI version](https://badge.fury.io/py/asreview.svg)](https://badge.fury.io/py/asreview) [![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fasreview%2Fasreview%2Fbadge%3Fref%3Dmaster&style=flat)](https://actions-badge.atrox.dev/asreview/asreview/goto?ref=master) [![Documentation Status](https://readthedocs.org/projects/asreview/badge/?version=latest)](https://asreview.readthedocs.io/en/latest/?badge=latest) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3345592.svg)](https://doi.org/10.5281/zenodo.3345592) [![Downloads](https://pepy.tech/badge/asreview)](https://github.com/asreview/asreview#installation) [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/4755/badge)](https://bestpractices.coreinfrastructure.org/projects/4755)
+[![PyPI version](https://badge.fury.io/py/asreview.svg)](https://badge.fury.io/py/asreview) [![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fasreview%2Fasreview%2Fbadge%3Fref%3Dmaster&style=flat)](https://actions-badge.atrox.dev/asreview/asreview/goto?ref=master) [![Documentation Status](https://readthedocs.org/projects/asreview/badge/?version=latest)](https://asreview.readthedocs.io/en/latest/?badge=latest) [![DOI](https://zenodo.org/badge/164874894.svg)](https://zenodo.org/badge/latestdoi/164874894)
+ [![Downloads](https://pepy.tech/badge/asreview)](https://github.com/asreview/asreview#installation) [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/4755/badge)](https://bestpractices.coreinfrastructure.org/projects/4755)
 
 Systematically screening large amounts of textual data is time-consuming and
 often tiresome. The rapidly evolving field of Artificial Intelligence (AI) has
 allowed the development of AI-aided pipelines that assist in finding relevant
 texts for search tasks. A well-established approach to increasing efficiency
 is screening prioritization via [Active
 Learning](https://asreview.readthedocs.io/en/latest/guides/activelearning.html).
@@ -53,21 +24,21 @@
 few false negatives. ASReview LAB will save time, increase the quality of
 output and strengthen the transparency of work when screening large amounts of
 textual data to retrieve relevant information. Active Learning will support 
 decision-making in any discipline or industry.
 
 ASReview software implements three different modes:
 
-- **Oracle**  Screen textual data in
+- **Oracle** :crystal_ball: Screen textual data in
   interaction with the active learning model. The reviewer is the 'oracle',
   making the labeling decisions.
-- **Exploration**  Explore or
+- **Exploration** :triangular_ruler: Explore or
   demonstrate ASReview LAB with a completely labeled dataset. This mode is
   suitable for teaching purposes.
-- **Simulation**  Evaluate
+- **Simulation** :chart_with_upwards_trend: Evaluate
   the performance of active learning models on fully labeled data. Simulations
   can be run in ASReview LAB or via the command line interface with more
   advanced options.
 
 
 ## Installation
```

#### html2text {}

```diff
@@ -1,64 +1,49 @@
-Metadata-Version: 2.1 Name: asreview Version: 1.1rc0 Summary: ASReview LAB - A
-tool for AI-assisted systematic reviews Home-page: https://github.com/asreview/
-asreview Author: ASReview LAB developers Author-email: asreview@uu.nl Project-
-URL: Bug Reports, https://github.com/asreview/asreview/issues Project-URL:
-Source, https://github.com/asreview/asreview/ Keywords: systematic review
-machine-learning Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Classifier: Topic :: Scientific/
-Engineering :: Information Analysis Classifier: Topic :: Text Processing ::
-General Classifier: Framework :: Flask Requires-Python: ~=3.7 Description-
-Content-Type: text/markdown Provides-Extra: sbert Provides-Extra: doc2vec
-Provides-Extra: tensorflow Provides-Extra: dev Provides-Extra: test Provides-
-Extra: all License-File: LICENSE
      [https://raw.githubusercontent.com/asreview/asreview-artwork/master/
               LogoASReview/SVG/GitHub_Repo_Card_Transparent.svg]
 ## ASReview: Active learning for Systematic Reviews [![PyPI version](https://
 badge.fury.io/py/asreview.svg)](https://badge.fury.io/py/asreview) [![Build
 Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-
 badge.atrox.dev%2Fasreview%2Fasreview%2Fbadge%3Fref%3Dmaster&style=flat)]
 (https://actions-badge.atrox.dev/asreview/asreview/goto?ref=master) [!
 [Documentation Status](https://readthedocs.org/projects/asreview/badge/
 ?version=latest)](https://asreview.readthedocs.io/en/latest/?badge=latest) [!
-[DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3345592.svg)](https://
-doi.org/10.5281/zenodo.3345592) [![Downloads](https://pepy.tech/badge/
-asreview)](https://github.com/asreview/asreview#installation) [![CII Best
-Practices](https://bestpractices.coreinfrastructure.org/projects/4755/badge)]
-(https://bestpractices.coreinfrastructure.org/projects/4755) Systematically
-screening large amounts of textual data is time-consuming and often tiresome.
-The rapidly evolving field of Artificial Intelligence (AI) has allowed the
-development of AI-aided pipelines that assist in finding relevant texts for
-search tasks. A well-established approach to increasing efficiency is screening
-prioritization via [Active Learning](https://asreview.readthedocs.io/en/latest/
-guides/activelearning.html). The Active learning for Systematic Reviews
-(ASReview) project, published in [*Nature Machine Intelligence*](https://
-doi.org/10.1038/s42256-020-00287-7) implements different machine learning
-algorithms that interactively query the researcher. ASReview LAB is designed to
-accelerate the step of screening textual data with a minimum of records to be
-read by a human with no or very few false negatives. ASReview LAB will save
-time, increase the quality of output and strengthen the transparency of work
-when screening large amounts of textual data to retrieve relevant information.
-Active Learning will support decision-making in any discipline or industry.
-ASReview software implements three different modes: - **Oracle** Screen textual
+[DOI](https://zenodo.org/badge/164874894.svg)](https://zenodo.org/badge/
+latestdoi/164874894) [![Downloads](https://pepy.tech/badge/asreview)](https://
+github.com/asreview/asreview#installation) [![CII Best Practices](https://
+bestpractices.coreinfrastructure.org/projects/4755/badge)](https://
+bestpractices.coreinfrastructure.org/projects/4755) Systematically screening
+large amounts of textual data is time-consuming and often tiresome. The rapidly
+evolving field of Artificial Intelligence (AI) has allowed the development of
+AI-aided pipelines that assist in finding relevant texts for search tasks. A
+well-established approach to increasing efficiency is screening prioritization
+via [Active Learning](https://asreview.readthedocs.io/en/latest/guides/
+activelearning.html). The Active learning for Systematic Reviews (ASReview)
+project, published in [*Nature Machine Intelligence*](https://doi.org/10.1038/
+s42256-020-00287-7) implements different machine learning algorithms that
+interactively query the researcher. ASReview LAB is designed to accelerate the
+step of screening textual data with a minimum of records to be read by a human
+with no or very few false negatives. ASReview LAB will save time, increase the
+quality of output and strengthen the transparency of work when screening large
+amounts of textual data to retrieve relevant information. Active Learning will
+support decision-making in any discipline or industry. ASReview software
+implements three different modes: - **Oracle** :crystal_ball: Screen textual
 data in interaction with the active learning model. The reviewer is the
-'oracle', making the labeling decisions. - **Exploration** Explore or
-demonstrate ASReview LAB with a completely labeled dataset. This mode is
-suitable for teaching purposes. - **Simulation** Evaluate the performance of
-active learning models on fully labeled data. Simulations can be run in
-ASReview LAB or via the command line interface with more advanced options. ##
-Installation The ASReview software requires Python 3.7+. Detailed step-by-step
-instructions to install Python and ASReview are available for [Windows](https:/
-/asreview.ai/installation-guide-windows/) and [macOS](https://asreview.ai/
-installation-guide-macos/) users. ```bash pip install asreview ``` Upgrade
-ASReview with the following command: ```bash pip install --upgrade asreview ```
-To install ASReview LAB with Docker, see [Install with Docker](https://
+'oracle', making the labeling decisions. - **Exploration** :triangular_ruler:
+Explore or demonstrate ASReview LAB with a completely labeled dataset. This
+mode is suitable for teaching purposes. - **Simulation** :
+chart_with_upwards_trend: Evaluate the performance of active learning models on
+fully labeled data. Simulations can be run in ASReview LAB or via the command
+line interface with more advanced options. ## Installation The ASReview
+software requires Python 3.7+. Detailed step-by-step instructions to install
+Python and ASReview are available for [Windows](https://asreview.ai/
+installation-guide-windows/) and [macOS](https://asreview.ai/installation-
+guide-macos/) users. ```bash pip install asreview ``` Upgrade ASReview with the
+following command: ```bash pip install --upgrade asreview ``` To install
+ASReview LAB with Docker, see [Install with Docker](https://
 asreview.readthedocs.io/en/latest/installation.html). ## How it works [!
 [ASReview LAB explained - animation](https://img.youtube.com/vi/k-a2SCq-LtA/
 0.jpg)](https://www.youtube.com/watch?v=k-a2SCq-LtA) ## Getting started
 [Getting Started with ASReview LAB](https://asreview.readthedocs.io/en/latest/
 about.html). [![ASReview LAB](https://github.com/asreview/asreview/blob/master/
 images/ASReviewWebApp.png?raw=true)](https://asreview.readthedocs.io/en/latest/
 lab/overview_lab.html "ASReview LAB") ## Citation The following publication in
```

### Comparing `asreview-1.1rc0/asreview.egg-info/entry_points.txt` & `asreview-1.2/asreview.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `asreview-1.1rc0/setup.py` & `asreview-1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,36 +99,37 @@
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Scientific/Engineering :: Information Analysis',
         'Topic :: Text Processing :: General',
         'Framework :: Flask',
     ],
-    keywords='systematic review machine-learning',
+    keywords=['systematic review', 'machine-learning'],
     packages=find_packages(exclude=['contrib', 'docs', 'tests']),
     package_data={'asreview': [
         'webapp/build/*',
         'webapp/build/static/*/*',
     ]},
     python_requires='~=3.7',
     install_requires=[
         'numpy',
         'scikit-learn',
-        'pandas',
+        'pandas>=1,<3',
         'rispy~=0.7.0',
         'dill',
         'xlrd>=1.0.0',
         'setuptools',
         'flask>=2.0',
         'flask_cors',
         'openpyxl',
-        'gevent',
+        'gevent>=20',
         'jsonschema',
         'filelock',
-        'tqdm'
+        'tqdm',
+        'datahugger>=0.2'
     ],
     extras_require=DEPS,
     entry_points={
         'console_scripts': [
             'asreview=asreview.__main__:main',
         ],
         'asreview.entry_points': [
```

### Comparing `asreview-1.1rc0/versioneer.py` & `asreview-1.2/versioneer.py`

 * *Files identical despite different names*

