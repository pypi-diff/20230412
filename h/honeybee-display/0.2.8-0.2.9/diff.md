# Comparing `tmp/honeybee-display-0.2.8.tar.gz` & `tmp/honeybee-display-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/honeybee-display-0.2.8.tar", last modified: Mon Dec 12 20:38:25 2022, max compression
+gzip compressed data, was "dist/honeybee-display-0.2.9.tar", last modified: Tue Dec 13 16:01:02 2022, max compression
```

## Comparing `honeybee-display-0.2.8.tar` & `honeybee-display-0.2.9.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 20:38:25.000000 honeybee-display-0.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 20:38:25.000000 honeybee-display-0.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 20:38:25.000000 honeybee-display-0.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      149 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      317 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (123)      279 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2022-12-12 20:38:25.000000 honeybee-display-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      694 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (123)      811 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 20:38:25.000000 honeybee-display-0.2.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 20:38:25.000000 honeybee-display-0.2.8/docs/_build/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/docs/_build/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/docs/_build/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 20:38:25.000000 honeybee-display-0.2.8/docs/_build/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/docs/_build/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 20:38:25.000000 honeybee-display-0.2.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      899 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/docs/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 20:38:25.000000 honeybee-display-0.2.8/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/docs/_templates/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 20:38:25.000000 honeybee-display-0.2.8/docs/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/docs/cli/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    21503 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       86 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)       73 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/extras-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 20:38:25.000000 honeybee-display-0.2.8/honeybee_display/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/honeybee_display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/honeybee_display/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/honeybee_display/_extend_honeybee.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/honeybee_display/aperture.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 20:38:25.000000 honeybee-display-0.2.8/honeybee_display/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     9103 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/honeybee_display/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13520 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/honeybee_display/colorobj.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/honeybee_display/door.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 20:38:25.000000 honeybee-display-0.2.8/honeybee_display/energy/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/honeybee_display/energy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10464 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/honeybee_display/energy/colorobj.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/honeybee_display/face.py
--rw-r--r--   0 runner    (1001) docker     (123)    23735 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/honeybee_display/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 20:38:25.000000 honeybee-display-0.2.8/honeybee_display/radiance/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/honeybee_display/radiance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/honeybee_display/room.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/honeybee_display/shade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 20:38:25.000000 honeybee-display-0.2.8/honeybee_display.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2022-12-12 20:38:25.000000 honeybee-display-0.2.8/honeybee_display.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2022-12-12 20:38:25.000000 honeybee-display-0.2.8/honeybee_display.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-12 20:38:25.000000 honeybee-display-0.2.8/honeybee_display.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2022-12-12 20:38:25.000000 honeybee-display-0.2.8/honeybee_display.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2022-12-12 20:38:25.000000 honeybee-display-0.2.8/honeybee_display.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2022-12-12 20:38:25.000000 honeybee-display-0.2.8/honeybee_display.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2022-12-12 20:38:25.000000 honeybee-display-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 20:38:25.000000 honeybee-display-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/tests/aperture_extend_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/tests/door_extend_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/tests/face_extend_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 20:38:25.000000 honeybee-display-0.2.8/tests/json/
--rw-r--r--   0 runner    (1001) docker     (123)   102631 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/tests/json/single_family_home.hbjson
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/tests/model_extend_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/tests/room_extend_test.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 20:37:20.000000 honeybee-display-0.2.8/tests/shade_extend_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:01:02.000000 honeybee-display-0.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:01:02.000000 honeybee-display-0.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:01:02.000000 honeybee-display-0.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2022-12-13 16:01:02.000000 honeybee-display-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:01:02.000000 honeybee-display-0.2.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:01:02.000000 honeybee-display-0.2.9/docs/_build/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/docs/_build/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/docs/_build/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:01:02.000000 honeybee-display-0.2.9/docs/_build/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/docs/_build/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:01:02.000000 honeybee-display-0.2.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/docs/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:01:02.000000 honeybee-display-0.2.9/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/docs/_templates/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:01:02.000000 honeybee-display-0.2.9/docs/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/docs/cli/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21503 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/extras-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:01:02.000000 honeybee-display-0.2.9/honeybee_display/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/honeybee_display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/honeybee_display/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/honeybee_display/_extend_honeybee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/honeybee_display/aperture.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:01:02.000000 honeybee-display-0.2.9/honeybee_display/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     9103 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/honeybee_display/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13572 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/honeybee_display/colorobj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/honeybee_display/door.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:01:02.000000 honeybee-display-0.2.9/honeybee_display/energy/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/honeybee_display/energy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10512 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/honeybee_display/energy/colorobj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/honeybee_display/face.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23735 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/honeybee_display/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:01:02.000000 honeybee-display-0.2.9/honeybee_display/radiance/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/honeybee_display/radiance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/honeybee_display/room.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/honeybee_display/shade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:01:02.000000 honeybee-display-0.2.9/honeybee_display.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2022-12-13 16:01:01.000000 honeybee-display-0.2.9/honeybee_display.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2022-12-13 16:01:02.000000 honeybee-display-0.2.9/honeybee_display.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 16:01:01.000000 honeybee-display-0.2.9/honeybee_display.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2022-12-13 16:01:01.000000 honeybee-display-0.2.9/honeybee_display.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2022-12-13 16:01:01.000000 honeybee-display-0.2.9/honeybee_display.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2022-12-13 16:01:01.000000 honeybee-display-0.2.9/honeybee_display.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2022-12-13 16:01:02.000000 honeybee-display-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:01:02.000000 honeybee-display-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/tests/aperture_extend_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/tests/door_extend_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/tests/face_extend_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:01:02.000000 honeybee-display-0.2.9/tests/json/
+-rw-r--r--   0 runner    (1001) docker     (123)   102631 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/tests/json/single_family_home.hbjson
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/tests/model_extend_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/tests/room_extend_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 15:59:58.000000 honeybee-display-0.2.9/tests/shade_extend_test.py
```

### Comparing `honeybee-display-0.2.8/.github/workflows/ci.yaml` & `honeybee-display-0.2.9/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.2.8/Dockerfile` & `honeybee-display-0.2.9/Dockerfile`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.2.8/LICENSE` & `honeybee-display-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.2.8/PKG-INFO` & `honeybee-display-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-display
-Version: 0.2.8
+Version: 0.2.9
 Summary: Adds methods to translate honeybee objects to VisualizationSets.
 Home-page: https://github.com/ladybug-tools/honeybee-display
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `honeybee-display-0.2.8/README.md` & `honeybee-display-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.2.8/deploy.sh` & `honeybee-display-0.2.9/deploy.sh`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.2.8/dev-requirements.txt` & `honeybee-display-0.2.9/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.2.8/docs/_static/custom.css` & `honeybee-display-0.2.9/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.2.8/docs/_templates/layout.html` & `honeybee-display-0.2.9/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.2.8/docs/conf.py` & `honeybee-display-0.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.2.8/honeybee_display/_extend_honeybee.py` & `honeybee-display-0.2.9/honeybee_display/_extend_honeybee.py`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.2.8/honeybee_display/aperture.py` & `honeybee-display-0.2.9/honeybee_display/aperture.py`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.2.8/honeybee_display/cli/__init__.py` & `honeybee-display-0.2.9/honeybee_display/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.2.8/honeybee_display/colorobj.py` & `honeybee-display-0.2.9/honeybee_display/colorobj.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,26 +159,27 @@
         label_text = []
         txt_height = None if color_face.legend_parameters.is_text_height_default \
             else color_face.legend_parameters.text_height
         font = color_face.legend_parameters.font
         # loop through the faces and create the text labels
         for face_prop, f_geo in zip(color_face.attributes, color_face.flat_geometry):
             if face_prop != 'N/A':
-                cent_pt = f_geo.center  # base point for the text
+                cent_pt = f_geo.center if f_geo.is_convex else \
+                    f_geo.pole_of_inaccessibility(tolerance)
                 base_plane = Plane(f_geo.normal, cent_pt)
                 if base_plane.y.z < 0:  # base plane pointing downwards; rotate it
                     base_plane = base_plane.rotate(base_plane.n, math.pi, base_plane.o)
                 if txt_height is None:  # auto-calculate default text height
                     txt_len = len(face_prop) if len(face_prop) > 10 else 10
                     dims = [
                         (f_geo.max.x - f_geo.min.x),
                         (f_geo.max.y - f_geo.min.y),
                         (f_geo.max.z - f_geo.min.z)]
                     dims.sort()
-                    txt_h = dims[1] / (txt_len * 1.5)
+                    txt_h = dims[1] / txt_len
                 else:
                     txt_h = txt_height
                 if txt_h < tolerance:
                     continue
                 txt_h = max_txt_h if txt_h > max_txt_h else txt_h
                 # move base plane origin a little to avoid overlaps of adjacent labels
                 if base_plane.n.x != 0:
```

### Comparing `honeybee-display-0.2.8/honeybee_display/door.py` & `honeybee-display-0.2.9/honeybee_display/door.py`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.2.8/honeybee_display/energy/colorobj.py` & `honeybee-display-0.2.9/honeybee_display/energy/colorobj.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,27 +146,28 @@
             fac_to_m = conversion_factor_to_meters(units)
             max_txt_h = 0.25 / fac_to_m
         txt_height, font, f_str = _process_leg_par_for_text(color_face)
         # loop through the faces and create the text labels
         label_text = []
         face_zip_obj = zip(color_face.matched_values, color_face.matched_flat_geometry)
         for face_val, f_geo in face_zip_obj:
-            cent_pt = f_geo.center  # base point for the text
+            cent_pt = f_geo.center if f_geo.is_convex else \
+                f_geo.pole_of_inaccessibility(tolerance)
             base_plane = Plane(f_geo.normal, cent_pt)
             face_prop = f_str % face_val
             if base_plane.y.z < 0:  # base plane pointing downwards; rotate it
                 base_plane = base_plane.rotate(base_plane.n, math.pi, base_plane.o)
             if txt_height is None:  # auto-calculate default text height
                 txt_len = len(face_prop) if len(face_prop) > 10 else 10
                 dims = [
                     (f_geo.max.x - f_geo.min.x),
                     (f_geo.max.y - f_geo.min.y),
                     (f_geo.max.z - f_geo.min.z)]
                 dims.sort()
-                txt_h = dims[1] / (txt_len * 1.5)
+                txt_h = dims[1] / txt_len
             else:
                 txt_h = txt_height
             if txt_h < tolerance:
                 continue
             txt_h = max_txt_h if txt_h > max_txt_h else txt_h
             # move base plane origin a little to avoid overlaps of adjacent labels
             if base_plane.n.x != 0:
```

### Comparing `honeybee-display-0.2.8/honeybee_display/face.py` & `honeybee-display-0.2.9/honeybee_display/face.py`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.2.8/honeybee_display/model.py` & `honeybee-display-0.2.9/honeybee_display/model.py`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.2.8/honeybee_display/room.py` & `honeybee-display-0.2.9/honeybee_display/room.py`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.2.8/honeybee_display/shade.py` & `honeybee-display-0.2.9/honeybee_display/shade.py`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.2.8/honeybee_display.egg-info/PKG-INFO` & `honeybee-display-0.2.9/honeybee_display.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-display
-Version: 0.2.8
+Version: 0.2.9
 Summary: Adds methods to translate honeybee objects to VisualizationSets.
 Home-page: https://github.com/ladybug-tools/honeybee-display
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `honeybee-display-0.2.8/honeybee_display.egg-info/SOURCES.txt` & `honeybee-display-0.2.9/honeybee_display.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.2.8/setup.py` & `honeybee-display-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.2.8/tests/aperture_extend_test.py` & `honeybee-display-0.2.9/tests/aperture_extend_test.py`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.2.8/tests/door_extend_test.py` & `honeybee-display-0.2.9/tests/door_extend_test.py`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.2.8/tests/face_extend_test.py` & `honeybee-display-0.2.9/tests/face_extend_test.py`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.2.8/tests/json/single_family_home.hbjson` & `honeybee-display-0.2.9/tests/json/single_family_home.hbjson`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.2.8/tests/model_extend_test.py` & `honeybee-display-0.2.9/tests/model_extend_test.py`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.2.8/tests/room_extend_test.py` & `honeybee-display-0.2.9/tests/room_extend_test.py`

 * *Files identical despite different names*

