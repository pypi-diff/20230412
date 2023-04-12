# Comparing `tmp/medium-api-0.5.0.tar.gz` & `tmp/medium-api-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medium-api-0.5.0.tar", last modified: Sun Apr  2 23:17:19 2023, max compression
+gzip compressed data, was "medium-api-0.5.1.tar", last modified: Wed Apr 12 09:14:48 2023, max compression
```

## Comparing `medium-api-0.5.0.tar` & `medium-api-0.5.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-02 23:17:19.955298 medium-api-0.5.0/
--rw-r--r--   0 sanskar    (501) staff       (20)     1069 2022-01-02 12:36:51.000000 medium-api-0.5.0/LICENSE
--rw-r--r--   0 sanskar    (501) staff       (20)      232 2022-01-21 06:51:28.000000 medium-api-0.5.0/MANIFEST.in
--rw-r--r--   0 sanskar    (501) staff       (20)     6221 2023-04-02 23:17:19.955427 medium-api-0.5.0/PKG-INFO
-drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-02 23:17:19.930187 medium-api-0.5.0/docs/
--rw-r--r--   0 sanskar    (501) staff       (20)      611 2022-02-27 09:33:04.000000 medium-api-0.5.0/docs/Makefile
--rw-r--r--   0 sanskar    (501) staff       (20)     5287 2023-01-28 20:04:36.000000 medium-api-0.5.0/docs/README.rst
-drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-02 23:17:19.921702 medium-api-0.5.0/docs/_build/
-drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-02 23:17:19.921775 medium-api-0.5.0/docs/_build/html/
-drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-02 23:17:19.934508 medium-api-0.5.0/docs/_build/html/_static/
--rw-r--r--   0 sanskar    (501) staff       (20)   378551 2022-02-28 09:45:28.000000 medium-api-0.5.0/docs/_build/html/_static/MediumAPI-Banner.png
--rw-r--r--   0 sanskar    (501) staff       (20)   116988 2022-04-10 13:29:20.000000 medium-api-0.5.0/docs/_build/html/_static/MediumAPI-GettingStarted-Thumbnail.png
--rw-r--r--   0 sanskar    (501) staff       (20)      286 2022-01-17 09:33:23.000000 medium-api-0.5.0/docs/_build/html/_static/file.png
-drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-02 23:17:19.938032 medium-api-0.5.0/docs/_build/html/_static/logos/
--rw-r--r--   0 sanskar    (501) staff       (20)    26295 2022-02-04 15:57:31.000000 medium-api-0.5.0/docs/_build/html/_static/logos/Logo-encircled-no-background.png
--rw-r--r--   0 sanskar    (501) staff       (20)   275759 2022-02-04 15:54:27.000000 medium-api-0.5.0/docs/_build/html/_static/logos/Logo-encircled.png
--rw-r--r--   0 sanskar    (501) staff       (20)    25218 2022-02-28 05:20:48.000000 medium-api-0.5.0/docs/_build/html/_static/logos/Logo-with_name-no_background.png
--rw-r--r--   0 sanskar    (501) staff       (20)   303096 2022-02-28 05:20:07.000000 medium-api-0.5.0/docs/_build/html/_static/logos/Logo-with_name.png
--rw-r--r--   0 sanskar    (501) staff       (20)    16128 2022-02-04 15:08:14.000000 medium-api-0.5.0/docs/_build/html/_static/logos/Logo.png
--rw-r--r--   0 sanskar    (501) staff       (20)       90 2022-01-17 09:33:23.000000 medium-api-0.5.0/docs/_build/html/_static/minus.png
--rw-r--r--   0 sanskar    (501) staff       (20)       90 2022-01-17 09:33:23.000000 medium-api-0.5.0/docs/_build/html/_static/plus.png
-drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-02 23:17:19.941094 medium-api-0.5.0/docs/_static/
--rw-r--r--   0 sanskar    (501) staff       (20)   378551 2022-02-28 09:45:28.000000 medium-api-0.5.0/docs/_static/MediumAPI-Banner.png
--rw-r--r--   0 sanskar    (501) staff       (20)   116988 2022-04-10 13:29:20.000000 medium-api-0.5.0/docs/_static/MediumAPI-GettingStarted-Thumbnail.png
-drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-02 23:17:19.947789 medium-api-0.5.0/docs/_static/logos/
--rw-rw-rw-   0 sanskar    (501) staff       (20)    26295 2022-02-04 15:57:31.000000 medium-api-0.5.0/docs/_static/logos/Logo-encircled-no-background.png
--rw-rw-rw-   0 sanskar    (501) staff       (20)   275759 2022-02-04 15:54:27.000000 medium-api-0.5.0/docs/_static/logos/Logo-encircled.png
--rw-r--r--   0 sanskar    (501) staff       (20)    25218 2022-02-28 05:20:48.000000 medium-api-0.5.0/docs/_static/logos/Logo-with_name-no_background.png
--rw-r--r--   0 sanskar    (501) staff       (20)   303096 2022-02-28 05:20:07.000000 medium-api-0.5.0/docs/_static/logos/Logo-with_name.png
--rw-r--r--   0 sanskar    (501) staff       (20)    16128 2022-02-04 15:08:14.000000 medium-api-0.5.0/docs/_static/logos/Logo.png
--rw-r--r--   0 sanskar    (501) staff       (20)      154 2022-02-28 10:17:36.000000 medium-api-0.5.0/docs/authors.rst
--rwxr-xr-x   0 sanskar    (501) staff       (20)     5256 2022-02-28 10:04:39.000000 medium-api-0.5.0/docs/conf.py
--rw-r--r--   0 sanskar    (501) staff       (20)     3501 2022-02-27 09:29:20.000000 medium-api-0.5.0/docs/contributing.rst
--rw-r--r--   0 sanskar    (501) staff       (20)      755 2022-02-27 09:27:35.000000 medium-api-0.5.0/docs/documentation.rst
--rw-r--r--   0 sanskar    (501) staff       (20)      420 2022-02-07 11:18:24.000000 medium-api-0.5.0/docs/index.rst
--rw-r--r--   0 sanskar    (501) staff       (20)     1158 2022-02-27 09:18:02.000000 medium-api-0.5.0/docs/installation.rst
--rw-r--r--   0 sanskar    (501) staff       (20)      772 2022-02-27 09:32:51.000000 medium-api-0.5.0/docs/make.bat
--rw-r--r--   0 sanskar    (501) staff       (20)    34500 2022-02-27 09:32:17.000000 medium-api-0.5.0/docs/terms_of_use.rst
--rw-r--r--   0 sanskar    (501) staff       (20)     6141 2022-11-30 08:54:41.000000 medium-api-0.5.0/docs/usage.rst
--rw-r--r--   0 sanskar    (501) staff       (20)       89 2022-01-16 18:16:53.000000 medium-api-0.5.0/pyproject.toml
--rw-r--r--   0 sanskar    (501) staff       (20)       33 2022-02-01 20:42:59.000000 medium-api-0.5.0/requirements-dev.txt
--rw-r--r--   0 sanskar    (501) staff       (20)        0 2023-01-26 20:03:14.000000 medium-api-0.5.0/requirements.txt
--rw-r--r--   0 sanskar    (501) staff       (20)     1045 2023-04-02 23:17:19.955905 medium-api-0.5.0/setup.cfg
--rw-r--r--   0 sanskar    (501) staff       (20)       61 2022-01-16 19:30:09.000000 medium-api-0.5.0/setup.py
-drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-02 23:17:19.922515 medium-api-0.5.0/src/
-drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-02 23:17:19.950235 medium-api-0.5.0/src/medium_api/
--rw-r--r--   0 sanskar    (501) staff       (20)      157 2023-04-02 23:17:19.000000 medium-api-0.5.0/src/medium_api/__init__.py
--rw-r--r--   0 sanskar    (501) staff       (20)    14357 2023-03-31 14:31:16.000000 medium-api-0.5.0/src/medium_api/_article.py
--rw-r--r--   0 sanskar    (501) staff       (20)     3013 2023-03-30 10:20:57.000000 medium-api-0.5.0/src/medium_api/_latestposts.py
--rw-r--r--   0 sanskar    (501) staff       (20)     8382 2023-04-02 21:00:13.000000 medium-api-0.5.0/src/medium_api/_medium_list.py
--rw-r--r--   0 sanskar    (501) staff       (20)    11527 2023-03-30 10:20:44.000000 medium-api-0.5.0/src/medium_api/_publication.py
--rw-r--r--   0 sanskar    (501) staff       (20)     2450 2023-03-30 10:20:19.000000 medium-api-0.5.0/src/medium_api/_top_writers.py
--rw-r--r--   0 sanskar    (501) staff       (20)     3076 2023-03-30 10:21:46.000000 medium-api-0.5.0/src/medium_api/_topfeeds.py
--rw-r--r--   0 sanskar    (501) staff       (20)    16315 2023-04-02 21:02:22.000000 medium-api-0.5.0/src/medium_api/_user.py
--rw-r--r--   0 sanskar    (501) staff       (20)    26809 2023-04-02 23:07:14.000000 medium-api-0.5.0/src/medium_api/medium.py
-drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-02 23:17:19.951752 medium-api-0.5.0/src/medium_api.egg-info/
--rw-r--r--   0 sanskar    (501) staff       (20)     6221 2023-04-02 23:17:19.000000 medium-api-0.5.0/src/medium_api.egg-info/PKG-INFO
--rw-r--r--   0 sanskar    (501) staff       (20)     1740 2023-04-02 23:17:19.000000 medium-api-0.5.0/src/medium_api.egg-info/SOURCES.txt
--rw-r--r--   0 sanskar    (501) staff       (20)        1 2023-04-02 23:17:19.000000 medium-api-0.5.0/src/medium_api.egg-info/dependency_links.txt
--rw-r--r--   0 sanskar    (501) staff       (20)       11 2023-04-02 23:17:19.000000 medium-api-0.5.0/src/medium_api.egg-info/top_level.txt
--rw-r--r--   0 sanskar    (501) staff       (20)        1 2022-07-27 13:19:52.000000 medium-api-0.5.0/src/medium_api.egg-info/zip-safe
-drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-02 23:17:19.955040 medium-api-0.5.0/tests/
--rw-r--r--   0 sanskar    (501) staff       (20)     6148 2022-02-27 12:41:15.000000 medium-api-0.5.0/tests/.DS_Store
--rw-r--r--   0 sanskar    (501) staff       (20)        0 2022-01-16 17:06:47.000000 medium-api-0.5.0/tests/__init__.py
--rw-r--r--   0 sanskar    (501) staff       (20)     3390 2023-03-31 14:29:15.000000 medium-api-0.5.0/tests/test_article.py
--rw-r--r--   0 sanskar    (501) staff       (20)     1161 2022-07-22 09:09:55.000000 medium-api-0.5.0/tests/test_latestposts.py
--rw-r--r--   0 sanskar    (501) staff       (20)     2255 2023-03-28 12:57:03.000000 medium-api-0.5.0/tests/test_medium_list.py
--rw-r--r--   0 sanskar    (501) staff       (20)     2610 2022-11-30 08:22:20.000000 medium-api-0.5.0/tests/test_publication.py
--rw-r--r--   0 sanskar    (501) staff       (20)     1230 2023-03-30 19:21:06.000000 medium-api-0.5.0/tests/test_search.py
--rw-r--r--   0 sanskar    (501) staff       (20)      710 2023-04-02 23:13:37.000000 medium-api-0.5.0/tests/test_tag.py
--rw-r--r--   0 sanskar    (501) staff       (20)      877 2023-02-17 11:23:49.000000 medium-api-0.5.0/tests/test_top_writers.py
--rw-r--r--   0 sanskar    (501) staff       (20)     1010 2023-02-14 17:43:26.000000 medium-api-0.5.0/tests/test_topfeeds.py
--rw-r--r--   0 sanskar    (501) staff       (20)     4162 2023-03-30 10:58:55.000000 medium-api-0.5.0/tests/test_user.py
+drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-12 09:14:48.127500 medium-api-0.5.1/
+-rw-r--r--   0 sanskar    (501) staff       (20)     1069 2022-01-02 12:36:51.000000 medium-api-0.5.1/LICENSE
+-rw-r--r--   0 sanskar    (501) staff       (20)      232 2022-01-21 06:51:28.000000 medium-api-0.5.1/MANIFEST.in
+-rw-r--r--   0 sanskar    (501) staff       (20)     6221 2023-04-12 09:14:48.127622 medium-api-0.5.1/PKG-INFO
+drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-12 09:14:48.104498 medium-api-0.5.1/docs/
+-rw-r--r--   0 sanskar    (501) staff       (20)      611 2022-02-27 09:33:04.000000 medium-api-0.5.1/docs/Makefile
+-rw-r--r--   0 sanskar    (501) staff       (20)     5287 2023-01-28 20:04:36.000000 medium-api-0.5.1/docs/README.rst
+drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-12 09:14:48.097125 medium-api-0.5.1/docs/_build/
+drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-12 09:14:48.097194 medium-api-0.5.1/docs/_build/html/
+drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-12 09:14:48.108378 medium-api-0.5.1/docs/_build/html/_static/
+-rw-r--r--   0 sanskar    (501) staff       (20)   378551 2022-02-28 09:45:28.000000 medium-api-0.5.1/docs/_build/html/_static/MediumAPI-Banner.png
+-rw-r--r--   0 sanskar    (501) staff       (20)   116988 2022-04-10 13:29:20.000000 medium-api-0.5.1/docs/_build/html/_static/MediumAPI-GettingStarted-Thumbnail.png
+-rw-r--r--   0 sanskar    (501) staff       (20)      286 2022-01-17 09:33:23.000000 medium-api-0.5.1/docs/_build/html/_static/file.png
+drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-12 09:14:48.111975 medium-api-0.5.1/docs/_build/html/_static/logos/
+-rw-r--r--   0 sanskar    (501) staff       (20)    26295 2022-02-04 15:57:31.000000 medium-api-0.5.1/docs/_build/html/_static/logos/Logo-encircled-no-background.png
+-rw-r--r--   0 sanskar    (501) staff       (20)   275759 2022-02-04 15:54:27.000000 medium-api-0.5.1/docs/_build/html/_static/logos/Logo-encircled.png
+-rw-r--r--   0 sanskar    (501) staff       (20)    25218 2022-02-28 05:20:48.000000 medium-api-0.5.1/docs/_build/html/_static/logos/Logo-with_name-no_background.png
+-rw-r--r--   0 sanskar    (501) staff       (20)   303096 2022-02-28 05:20:07.000000 medium-api-0.5.1/docs/_build/html/_static/logos/Logo-with_name.png
+-rw-r--r--   0 sanskar    (501) staff       (20)    16128 2022-02-04 15:08:14.000000 medium-api-0.5.1/docs/_build/html/_static/logos/Logo.png
+-rw-r--r--   0 sanskar    (501) staff       (20)       90 2022-01-17 09:33:23.000000 medium-api-0.5.1/docs/_build/html/_static/minus.png
+-rw-r--r--   0 sanskar    (501) staff       (20)       90 2022-01-17 09:33:23.000000 medium-api-0.5.1/docs/_build/html/_static/plus.png
+drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-12 09:14:48.115023 medium-api-0.5.1/docs/_static/
+-rw-r--r--   0 sanskar    (501) staff       (20)   378551 2022-02-28 09:45:28.000000 medium-api-0.5.1/docs/_static/MediumAPI-Banner.png
+-rw-r--r--   0 sanskar    (501) staff       (20)   116988 2022-04-10 13:29:20.000000 medium-api-0.5.1/docs/_static/MediumAPI-GettingStarted-Thumbnail.png
+drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-12 09:14:48.120083 medium-api-0.5.1/docs/_static/logos/
+-rw-rw-rw-   0 sanskar    (501) staff       (20)    26295 2022-02-04 15:57:31.000000 medium-api-0.5.1/docs/_static/logos/Logo-encircled-no-background.png
+-rw-rw-rw-   0 sanskar    (501) staff       (20)   275759 2022-02-04 15:54:27.000000 medium-api-0.5.1/docs/_static/logos/Logo-encircled.png
+-rw-r--r--   0 sanskar    (501) staff       (20)    25218 2022-02-28 05:20:48.000000 medium-api-0.5.1/docs/_static/logos/Logo-with_name-no_background.png
+-rw-r--r--   0 sanskar    (501) staff       (20)   303096 2022-02-28 05:20:07.000000 medium-api-0.5.1/docs/_static/logos/Logo-with_name.png
+-rw-r--r--   0 sanskar    (501) staff       (20)    16128 2022-02-04 15:08:14.000000 medium-api-0.5.1/docs/_static/logos/Logo.png
+-rw-r--r--   0 sanskar    (501) staff       (20)      154 2022-02-28 10:17:36.000000 medium-api-0.5.1/docs/authors.rst
+-rwxr-xr-x   0 sanskar    (501) staff       (20)     5256 2022-02-28 10:04:39.000000 medium-api-0.5.1/docs/conf.py
+-rw-r--r--   0 sanskar    (501) staff       (20)     3501 2022-02-27 09:29:20.000000 medium-api-0.5.1/docs/contributing.rst
+-rw-r--r--   0 sanskar    (501) staff       (20)      855 2023-04-02 23:24:30.000000 medium-api-0.5.1/docs/documentation.rst
+-rw-r--r--   0 sanskar    (501) staff       (20)      420 2022-02-07 11:18:24.000000 medium-api-0.5.1/docs/index.rst
+-rw-r--r--   0 sanskar    (501) staff       (20)     1158 2022-02-27 09:18:02.000000 medium-api-0.5.1/docs/installation.rst
+-rw-r--r--   0 sanskar    (501) staff       (20)      772 2022-02-27 09:32:51.000000 medium-api-0.5.1/docs/make.bat
+-rw-r--r--   0 sanskar    (501) staff       (20)    34500 2022-02-27 09:32:17.000000 medium-api-0.5.1/docs/terms_of_use.rst
+-rw-r--r--   0 sanskar    (501) staff       (20)    10149 2023-04-04 09:22:14.000000 medium-api-0.5.1/docs/usage.rst
+-rw-r--r--   0 sanskar    (501) staff       (20)       89 2022-01-16 18:16:53.000000 medium-api-0.5.1/pyproject.toml
+-rw-r--r--   0 sanskar    (501) staff       (20)       33 2022-02-01 20:42:59.000000 medium-api-0.5.1/requirements-dev.txt
+-rw-r--r--   0 sanskar    (501) staff       (20)        0 2023-01-26 20:03:14.000000 medium-api-0.5.1/requirements.txt
+-rw-r--r--   0 sanskar    (501) staff       (20)     1045 2023-04-12 09:14:48.128061 medium-api-0.5.1/setup.cfg
+-rw-r--r--   0 sanskar    (501) staff       (20)       61 2022-01-16 19:30:09.000000 medium-api-0.5.1/setup.py
+drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-12 09:14:48.097772 medium-api-0.5.1/src/
+drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-12 09:14:48.122456 medium-api-0.5.1/src/medium_api/
+-rw-r--r--   0 sanskar    (501) staff       (20)      157 2023-04-12 09:14:47.000000 medium-api-0.5.1/src/medium_api/__init__.py
+-rw-r--r--   0 sanskar    (501) staff       (20)    15208 2023-04-12 09:13:58.000000 medium-api-0.5.1/src/medium_api/_article.py
+-rw-r--r--   0 sanskar    (501) staff       (20)     3013 2023-03-30 10:20:57.000000 medium-api-0.5.1/src/medium_api/_latestposts.py
+-rw-r--r--   0 sanskar    (501) staff       (20)     8382 2023-04-02 21:00:13.000000 medium-api-0.5.1/src/medium_api/_medium_list.py
+-rw-r--r--   0 sanskar    (501) staff       (20)    11527 2023-03-30 10:20:44.000000 medium-api-0.5.1/src/medium_api/_publication.py
+-rw-r--r--   0 sanskar    (501) staff       (20)     2450 2023-03-30 10:20:19.000000 medium-api-0.5.1/src/medium_api/_top_writers.py
+-rw-r--r--   0 sanskar    (501) staff       (20)     3076 2023-03-30 10:21:46.000000 medium-api-0.5.1/src/medium_api/_topfeeds.py
+-rw-r--r--   0 sanskar    (501) staff       (20)    16315 2023-04-02 21:02:22.000000 medium-api-0.5.1/src/medium_api/_user.py
+-rw-r--r--   0 sanskar    (501) staff       (20)    26747 2023-04-02 23:33:40.000000 medium-api-0.5.1/src/medium_api/medium.py
+drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-12 09:14:48.123367 medium-api-0.5.1/src/medium_api.egg-info/
+-rw-r--r--   0 sanskar    (501) staff       (20)     6221 2023-04-12 09:14:47.000000 medium-api-0.5.1/src/medium_api.egg-info/PKG-INFO
+-rw-r--r--   0 sanskar    (501) staff       (20)     1740 2023-04-12 09:14:47.000000 medium-api-0.5.1/src/medium_api.egg-info/SOURCES.txt
+-rw-r--r--   0 sanskar    (501) staff       (20)        1 2023-04-12 09:14:47.000000 medium-api-0.5.1/src/medium_api.egg-info/dependency_links.txt
+-rw-r--r--   0 sanskar    (501) staff       (20)       11 2023-04-12 09:14:47.000000 medium-api-0.5.1/src/medium_api.egg-info/top_level.txt
+-rw-r--r--   0 sanskar    (501) staff       (20)        1 2022-07-27 13:19:52.000000 medium-api-0.5.1/src/medium_api.egg-info/zip-safe
+drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-12 09:14:48.127158 medium-api-0.5.1/tests/
+-rw-r--r--   0 sanskar    (501) staff       (20)     6148 2022-02-27 12:41:15.000000 medium-api-0.5.1/tests/.DS_Store
+-rw-r--r--   0 sanskar    (501) staff       (20)        0 2022-01-16 17:06:47.000000 medium-api-0.5.1/tests/__init__.py
+-rw-r--r--   0 sanskar    (501) staff       (20)     3578 2023-04-12 09:09:51.000000 medium-api-0.5.1/tests/test_article.py
+-rw-r--r--   0 sanskar    (501) staff       (20)     1161 2022-07-22 09:09:55.000000 medium-api-0.5.1/tests/test_latestposts.py
+-rw-r--r--   0 sanskar    (501) staff       (20)     2255 2023-03-28 12:57:03.000000 medium-api-0.5.1/tests/test_medium_list.py
+-rw-r--r--   0 sanskar    (501) staff       (20)     2610 2022-11-30 08:22:20.000000 medium-api-0.5.1/tests/test_publication.py
+-rw-r--r--   0 sanskar    (501) staff       (20)     1230 2023-03-30 19:21:06.000000 medium-api-0.5.1/tests/test_search.py
+-rw-r--r--   0 sanskar    (501) staff       (20)      710 2023-04-02 23:13:37.000000 medium-api-0.5.1/tests/test_tag.py
+-rw-r--r--   0 sanskar    (501) staff       (20)      877 2023-02-17 11:23:49.000000 medium-api-0.5.1/tests/test_top_writers.py
+-rw-r--r--   0 sanskar    (501) staff       (20)     1010 2023-02-14 17:43:26.000000 medium-api-0.5.1/tests/test_topfeeds.py
+-rw-r--r--   0 sanskar    (501) staff       (20)     4162 2023-03-30 10:58:55.000000 medium-api-0.5.1/tests/test_user.py
```

### Comparing `medium-api-0.5.0/LICENSE` & `medium-api-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/PKG-INFO` & `medium-api-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medium-api
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python Wrapper on top of Medium API to quickly extract data from https://medium.com.
 Home-page: https://github.com/weeping-angel/medium-api
 Author: Nishu Jain
 Author-email: nishujain1997.19@gmail.com
 License: MIT
 Platform: unix
 Platform: linux
```

### Comparing `medium-api-0.5.0/docs/Makefile` & `medium-api-0.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/docs/README.rst` & `medium-api-0.5.1/docs/README.rst`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/docs/_build/html/_static/MediumAPI-Banner.png` & `medium-api-0.5.1/docs/_build/html/_static/MediumAPI-Banner.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/docs/_build/html/_static/MediumAPI-GettingStarted-Thumbnail.png` & `medium-api-0.5.1/docs/_build/html/_static/MediumAPI-GettingStarted-Thumbnail.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/docs/_build/html/_static/logos/Logo-encircled-no-background.png` & `medium-api-0.5.1/docs/_build/html/_static/logos/Logo-encircled-no-background.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/docs/_build/html/_static/logos/Logo-encircled.png` & `medium-api-0.5.1/docs/_build/html/_static/logos/Logo-encircled.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/docs/_build/html/_static/logos/Logo-with_name-no_background.png` & `medium-api-0.5.1/docs/_build/html/_static/logos/Logo-with_name-no_background.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/docs/_build/html/_static/logos/Logo-with_name.png` & `medium-api-0.5.1/docs/_build/html/_static/logos/Logo-with_name.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/docs/_build/html/_static/logos/Logo.png` & `medium-api-0.5.1/docs/_build/html/_static/logos/Logo.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/docs/_static/MediumAPI-Banner.png` & `medium-api-0.5.1/docs/_static/MediumAPI-Banner.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/docs/_static/MediumAPI-GettingStarted-Thumbnail.png` & `medium-api-0.5.1/docs/_static/MediumAPI-GettingStarted-Thumbnail.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/docs/_static/logos/Logo-encircled-no-background.png` & `medium-api-0.5.1/docs/_static/logos/Logo-encircled-no-background.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/docs/_static/logos/Logo-encircled.png` & `medium-api-0.5.1/docs/_static/logos/Logo-encircled.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/docs/_static/logos/Logo-with_name-no_background.png` & `medium-api-0.5.1/docs/_static/logos/Logo-with_name-no_background.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/docs/_static/logos/Logo-with_name.png` & `medium-api-0.5.1/docs/_static/logos/Logo-with_name.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/docs/_static/logos/Logo.png` & `medium-api-0.5.1/docs/_static/logos/Logo.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/docs/conf.py` & `medium-api-0.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/docs/contributing.rst` & `medium-api-0.5.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/docs/documentation.rst` & `medium-api-0.5.1/docs/documentation.rst`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,20 @@
 
 Publication class
 ^^^^^^^^^^^^^^^^^
 
 .. autoclass:: medium_api._publication.Publication
    :members:
 
+MediumList class
+^^^^^^^^^^^^^^^^^
+
+.. autoclass:: medium_api._medium_list.MediumList
+   :members:
+
 LatestPosts class
 ^^^^^^^^^^^^^^^^^
 
 .. autoclass:: medium_api._latestposts.LatestPosts
    :members:
 
 TopWriters class
```

### Comparing `medium-api-0.5.0/docs/installation.rst` & `medium-api-0.5.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/docs/make.bat` & `medium-api-0.5.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/docs/terms_of_use.rst` & `medium-api-0.5.1/docs/terms_of_use.rst`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/setup.cfg` & `medium-api-0.5.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = medium-api
 description = Python Wrapper on top of Medium API to quickly extract data from https://medium.com.
-version = 0.5.0
+version = 0.5.1
 long_description = file: docs/README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/weeping-angel/medium-api
 author = Nishu Jain
 author_email = nishujain1997.19@gmail.com
 platforms = unix, linux, osx, win32, cygwin
 description_file = README.rst
```

### Comparing `medium-api-0.5.0/src/medium_api/_article.py` & `medium-api-0.5.1/src/medium_api/_article.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
         self.is_locked = None
 
         self.publication = None
 
         self.__info = None
         self.__content = None
         self.__markdown = None
+        self.__html = None
         self.__response_ids = None
         self.__responses = None
         self.__fans_ids = None
         self.__fans = None
         self.__related_articles_ids = None
         self.__related_articles = None
 
@@ -350,14 +351,42 @@
             images, listicles, etc ...` within an article, in the markdown format 
         """
         if self.__markdown is None:
             resp, _ = self.__get_resp(f'/article/{self.article_id}/markdown')
             self.__markdown = str(resp['markdown'])
 
         return self.__markdown
+    
+    @property
+    def html(self):
+        """To get the Medium Article in plain HTML format
+
+        Returns:
+            str: A single string containing the entire article in HTML format 
+        """
+        if self.__html is None:
+            self.save_html(fullpage=False)
+
+        return self.__html
+    
+    def save_html(self, fullpage:bool=False):
+        """Saves the article in plain HTML format
+
+        Args:
+
+            fullpage (bool, optional): If 'True', saves full HTML page with head, body, title and meta tags. 
+                Else, saves HTML inside body only.
+        
+        Returns:
+            None
+
+        """
+        fullpage = 'true' if fullpage else 'false'
+        resp, _ = self.__get_resp(f'/article/{self.article_id}/html?fullpage={fullpage}')
+        self.__html = str(resp['html'])
 
     @property
     def json(self):
         """To get the articles information in JSON format
         
         Returns:
             dict: Returns a JSON object containing article `info`, `content`, and `markdown` if
```

### Comparing `medium-api-0.5.0/src/medium_api/_latestposts.py` & `medium-api-0.5.1/src/medium_api/_latestposts.py`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/src/medium_api/_medium_list.py` & `medium-api-0.5.1/src/medium_api/_medium_list.py`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/src/medium_api/_publication.py` & `medium-api-0.5.1/src/medium_api/_publication.py`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/src/medium_api/_top_writers.py` & `medium-api-0.5.1/src/medium_api/_top_writers.py`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/src/medium_api/_topfeeds.py` & `medium-api-0.5.1/src/medium_api/_topfeeds.py`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/src/medium_api/_user.py` & `medium-api-0.5.1/src/medium_api/_user.py`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/src/medium_api/medium.py` & `medium-api-0.5.1/src/medium_api/medium.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,15 @@
                 It's optional only if you've already provided the `username`.
 
             save_info (bool, optional): If `False`, creates an empty `User` object which
                 needs to be filled using ``user.save_info()`` method later. (Default is 
                 `True`)
 
         Returns:
-            User: Medium API's User Object (medium_api.user.User) that can be used 
+            User: Medium API's User Object (medium_api._user.User) that can be used 
             to access all the properties and methods associated to the given Medium
             user.
 
         Note:
             You have to provide either `username` or `user_id` to get the User object. You
             cannot omit both. 
         """
@@ -159,15 +159,15 @@
                 - https://nishu-jain.medium.com/about-me-nishu-jain-562c5821b5f0
 
             save_info (bool, optional): If `False`, creates an empty `Article` object which
                 needs to be filled using ``article.save_info()`` method later. (Default is 
                 `True`)
 
         Returns:
-            Article: Medium API `Article` Object (medium_api.article.Article) that can be
+            Article: Medium API `Article` Object (medium_api._article.Article) that can be
             used to access all the properties and methods related to a Medium Article.
 
         """
         return Article(article_id = article_id, 
                        get_resp = self.__get_resp, 
                        fetch_articles=self.fetch_articles,
                        fetch_users = self.fetch_users,
@@ -189,15 +189,15 @@
                 - https://nishu-jain.medium.com/list/medium-api-38f9e0f9bea6
 
             save_info (bool, optional): If `False`, creates an empty `Medium List` object which
                 needs to be filled using ``medium_list.save_info()`` method later. (Default is 
                 `True`)
 
         Returns:
-            Medium List: Medium API `Medium List` Object (medium_api.article.MediumList) that can be
+            MediumList: Medium API `Medium List` Object (medium_api._medium_list.MediumList) that can be
             used to access all the properties and methods related to a Medium List.
 
         """
         return MediumList(list_id = list_id, 
                        get_resp = self.__get_resp, 
                        fetch_articles=self.fetch_articles,
                        fetch_users = self.fetch_users,
@@ -222,15 +222,15 @@
                 It's optional only if you've already provided the `publication_slug`.
 
             save_info (bool, optional): If `False`, creates an empty `Publication` object which
                 needs to be filled using ``publication.save_info()`` method later. (Default is 
                 `True`)
 
         Returns:
-            Publication: Medium API `Publication` Object (medium_api.publication.Publication) 
+            Publication: Medium API `Publication` Object (medium_api._publication.Publication) 
             that can be used to access all the properties and methods related to a Medium 
             Publication.
 
         Note:
             You have to provide either `publication_slug` or `publication_id` to get the Publication object. 
             You cannot omit both. 
 
@@ -268,15 +268,15 @@
         Args:
             topic_slug (str): It's a string (smallcase, hyphen-separated) which specifies
                 a category/niche as classified by the Medium Platform.
 
             count (int): Number of Top writers you want to fetch (less than 250).
 
         Returns:
-            TopWriters: Medium API `TopWriters` Object (medium_api.top_writers.TopWriters) 
+            TopWriters: Medium API `TopWriters` Object (medium_api._top_writers.TopWriters) 
             that can be used to access all the properties and methods related to Medium's 
             Top Writers for the give `topic_slug`.
 
         """
         return TopWriters(topic_slug=topic_slug, 
                           count = count,
                           get_resp=self.__get_resp, 
@@ -294,15 +294,15 @@
             ``latestposts = medium.latestposts(topic_slug = "artificial-intelligence")``
 
         Args:
             topic_slug (str): It's a string (smallcase, hyphen-separated) which specifies
                 a category/niche as classified by the Medium Platform.
 
         Returns:
-            LatestPosts: Medium API `LatestPosts` Object (medium_api.latestposts.LatestPosts) 
+            LatestPosts: Medium API `LatestPosts` Object (medium_api._latestposts.LatestPosts) 
             that can be used to access all the properties and methods related to Medium's 
             LatestPosts within the given topic.
 
         """
         return LatestPosts(topic_slug=topic_slug, 
                            get_resp=self.__get_resp, 
                            fetch_articles=self.fetch_articles,
@@ -331,15 +331,15 @@
                     - ``top_year``: For getting best articles of the year
                     - ``top_month``: For getting best articles of the month
                     - ``top_week``: For getting best articles of the week
                     - ``top_all_time``: For getting best article of all time
 
 
         Returns:
-            TopFeeds: Medium API `TopFeeds` Object (medium_api.topfeeds.TopFeeds) 
+            TopFeeds: Medium API `TopFeeds` Object (medium_api._topfeeds.TopFeeds) 
             that can be used to access all the properties and methods, for given `tag` 
             and `mode`.
 
         """
         return TopFeeds(tag=tag, mode=mode, count=count,
                         get_resp=self.__get_resp, 
                         fetch_articles=self.fetch_articles,
@@ -365,16 +365,15 @@
         Returns:
             list[Article]: List of `Article` objects from the search results.
 
         Note:
             The resultant list will contain 1000 `Article` objects at max.
         
         Warnings:
-            OveruseWarning: Don't set ``save_info = True`` unless you have enough API calls in your 
-                subscribed plan. You might either exhaust your current plan or incur overage.
+            OveruseWarning: Don't set ``save_info = True`` unless you have enough API calls in your subscribed plan. You might either exhaust your current plan or incur overage.
         """
         resp, _ = self.__get_resp(f'/search/articles?query={quote(query)}')
 
         article_ids = resp['articles']
         articles = []
 
         if article_ids:
@@ -401,16 +400,15 @@
         Returns:
             list[Publication]: List of `Publication` objects from the search results.
 
         Note:
             The resultant list will contain 1000 `Publication` objects at max.
         
         Warnings:
-            OveruseWarning: Don't set ``save_info = True`` unless you have enough API calls in your 
-                subscribed plan. You might either exhaust your current plan or incur overage.
+            OveruseWarning: Don't set ``save_info = True`` unless you have enough API calls in your subscribed plan. You might either exhaust your current plan or incur overage.
         """
         resp, _ = self.__get_resp(f'/search/publications?query={quote(query)}')
 
         publication_ids = resp['publications']
         publications = []
         
         if publication_ids:
@@ -437,16 +435,15 @@
         Returns:
             list[User]: List of `User` objects from the search results.
 
         Note:
             The resultant list will contain 1000 `User` objects at max.
         
         Warnings:
-            OveruseWarning: Don't set ``save_info = True`` unless you have enough API calls in your 
-                subscribed plan. You might either exhaust your current plan or incur overage.
+            OveruseWarning: Don't set ``save_info = True`` unless you have enough API calls in your subscribed plan. You might either exhaust your current plan or incur overage.
         """
         resp, _ = self.__get_resp(f'/search/users?query={quote(query)}')
 
         user_ids = resp['users']
         users = []
         
         if user_ids:
@@ -473,16 +470,15 @@
         Returns:
             list[MediumList]: Array of `MediumList` objects from the search results.
 
         Note:
             The resultant list will contain 1000 `MediumList` objects at max.
         
         Warnings:
-            OveruseWarning: Don't set ``save_info = True`` unless you have enough API calls in your 
-                subscribed plan. You might either exhaust your current plan or incur overage.
+            OveruseWarning: Don't set ``save_info = True`` unless you have enough API calls in your subscribed plan. You might either exhaust your current plan or incur overage.
         """
         resp, _ = self.__get_resp(f'/search/lists?query={quote(query)}')
 
         list_ids = resp['lists']
         lists = []
         
         if list_ids:
@@ -499,15 +495,15 @@
 
             ``blockchain_tags = medium.search_tags(query = "blockchain")``
 
         Args:
             query (str): It's the search query to get results from Medium Platform.
 
         Returns:
-            list[str]: List of lowercased, hyphen-separated strings
+            list[str]: List of lowercased, hyphen-separated strings of tags
 
         Note:
             The resultant list will contain 1000 tags at max.
         """
         resp, _ = self.__get_resp(f'/search/tags?query={quote(query)}')
 
         tags = resp['tags']
@@ -542,15 +538,15 @@
 
         Args:
             tag (str): It's a string (lowercase, hyphen-separated) which specifies
                        a category/niche as classified by the Medium Platform.
 
         Returns:
             dict: Contains tag-related information
-            
+
         """
         resp, _ = self.__get_resp(f'/tag/{tag}')
 
         return resp
 
     def fetch_articles(self, articles:list, content:bool = False):
         """To quickly fetch articles (info and content) using multithreading
```

### Comparing `medium-api-0.5.0/src/medium_api.egg-info/PKG-INFO` & `medium-api-0.5.1/src/medium_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medium-api
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python Wrapper on top of Medium API to quickly extract data from https://medium.com.
 Home-page: https://github.com/weeping-angel/medium-api
 Author: Nishu Jain
 Author-email: nishujain1997.19@gmail.com
 License: MIT
 Platform: unix
 Platform: linux
```

### Comparing `medium-api-0.5.0/src/medium_api.egg-info/SOURCES.txt` & `medium-api-0.5.1/src/medium_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/tests/.DS_Store` & `medium-api-0.5.1/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/tests/test_article.py` & `medium-api-0.5.1/tests/test_article.py`

 * *Files 5% similar despite different names*

```diff
@@ -95,14 +95,21 @@
 
 def test_article_markdown():
     article.save_markdown()
 
     assert isinstance(article.markdown, str)
     assert len(article.markdown) > 0
 
+def test_article_html():
+    article.save_html(fullpage=True)
+
+    assert isinstance(article.html, str)
+    assert len(article.html) > 0
+    assert article.html[:len('<html')] == '<html'
+
 def test_article_json():
     article.save_info()
     article.save_content()
     article.save_markdown()
     
     article_json = article.json
```

### Comparing `medium-api-0.5.0/tests/test_latestposts.py` & `medium-api-0.5.1/tests/test_latestposts.py`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/tests/test_medium_list.py` & `medium-api-0.5.1/tests/test_medium_list.py`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/tests/test_publication.py` & `medium-api-0.5.1/tests/test_publication.py`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/tests/test_search.py` & `medium-api-0.5.1/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/tests/test_tag.py` & `medium-api-0.5.1/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/tests/test_top_writers.py` & `medium-api-0.5.1/tests/test_top_writers.py`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/tests/test_topfeeds.py` & `medium-api-0.5.1/tests/test_topfeeds.py`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.0/tests/test_user.py` & `medium-api-0.5.1/tests/test_user.py`

 * *Files identical despite different names*

