# Comparing `tmp/NferModule-0.9.8.tar.gz` & `tmp/NferModule-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NferModule-0.9.8.tar", last modified: Fri May 21 09:52:17 2021, max compression
+gzip compressed data, was "NferModule-0.9.9.tar", last modified: Fri May 21 12:23:35 2021, max compression
```

## Comparing `NferModule-0.9.8.tar` & `NferModule-0.9.9.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 sb37fk    (1000) sb37fk    (1000)        0 2021-05-21 09:52:17.871262 NferModule-0.9.8/
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)    34176 2021-05-07 11:17:34.000000 NferModule-0.9.8/COPYING
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)      161 2021-05-21 09:42:14.000000 NferModule-0.9.8/MANIFEST.in
-drwxr-xr-x   0 sb37fk    (1000) sb37fk    (1000)        0 2021-05-21 09:52:17.847929 NferModule-0.9.8/NferModule.egg-info/
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     4949 2021-05-21 09:52:17.000000 NferModule-0.9.8/NferModule.egg-info/PKG-INFO
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     1124 2021-05-21 09:52:17.000000 NferModule-0.9.8/NferModule.egg-info/SOURCES.txt
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)        1 2021-05-21 09:52:17.000000 NferModule-0.9.8/NferModule.egg-info/dependency_links.txt
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)        1 2021-05-21 09:24:22.000000 NferModule-0.9.8/NferModule.egg-info/not-zip-safe
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)       37 2021-05-21 09:52:17.000000 NferModule-0.9.8/NferModule.egg-info/requires.txt
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)       11 2021-05-21 09:52:17.000000 NferModule-0.9.8/NferModule.egg-info/top_level.txt
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     4949 2021-05-21 09:52:17.867929 NferModule-0.9.8/PKG-INFO
-drwxr-xr-x   0 sb37fk    (1000) sb37fk    (1000)        0 2021-05-21 09:52:17.841262 NferModule-0.9.8/gensrc/
-drwxr-xr-x   0 sb37fk    (1000) sb37fk    (1000)        0 2021-05-21 09:52:17.847929 NferModule-0.9.8/gensrc/parser/
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)    78516 2021-05-20 13:46:42.000000 NferModule-0.9.8/gensrc/parser/dsl.tab.c
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     6861 2021-05-20 13:46:42.000000 NferModule-0.9.8/gensrc/parser/dsl.tab.h
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)    71752 2021-05-20 13:46:42.000000 NferModule-0.9.8/gensrc/parser/dsl.yy.c
-drwxr-xr-x   0 sb37fk    (1000) sb37fk    (1000)        0 2021-05-21 09:52:17.854595 NferModule-0.9.8/inc/
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     1056 2021-05-07 11:17:35.000000 NferModule-0.9.8/inc/analysis.h
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     6688 2021-05-07 11:17:35.000000 NferModule-0.9.8/inc/ast.h
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     1044 2021-05-07 11:17:35.000000 NferModule-0.9.8/inc/astutil.h
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)      312 2021-05-07 11:17:35.000000 NferModule-0.9.8/inc/compile.h
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     1161 2021-05-12 15:51:15.000000 NferModule-0.9.8/inc/debug.h
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     1990 2021-05-07 11:17:35.000000 NferModule-0.9.8/inc/dict.h
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     1183 2021-05-11 13:52:21.000000 NferModule-0.9.8/inc/dsl.h
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     2305 2021-05-07 11:17:35.000000 NferModule-0.9.8/inc/expression.h
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     1370 2021-05-07 11:17:35.000000 NferModule-0.9.8/inc/file.h
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     1141 2021-05-07 11:17:35.000000 NferModule-0.9.8/inc/generate.h
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     2016 2021-05-07 11:17:35.000000 NferModule-0.9.8/inc/learn.h
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     1574 2021-05-07 11:17:35.000000 NferModule-0.9.8/inc/log.h
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     2216 2021-05-07 11:17:35.000000 NferModule-0.9.8/inc/map.h
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     1088 2021-05-07 11:17:35.000000 NferModule-0.9.8/inc/memory.h
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     4495 2021-05-07 11:17:35.000000 NferModule-0.9.8/inc/nfer.h
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     2730 2021-05-07 11:17:35.000000 NferModule-0.9.8/inc/pool.h
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)      635 2021-05-07 11:17:35.000000 NferModule-0.9.8/inc/rdc.h
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     1479 2021-05-07 11:17:35.000000 NferModule-0.9.8/inc/semantic.h
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     1320 2021-05-07 11:17:35.000000 NferModule-0.9.8/inc/stack.h
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     1261 2021-05-07 11:17:35.000000 NferModule-0.9.8/inc/strings.h
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     2269 2021-05-07 11:17:35.000000 NferModule-0.9.8/inc/target.h
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     2222 2021-05-07 11:17:35.000000 NferModule-0.9.8/inc/types.h
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)      103 2021-05-20 09:41:13.000000 NferModule-0.9.8/pyproject.toml
-drwxr-xr-x   0 sb37fk    (1000) sb37fk    (1000)        0 2021-05-21 09:52:17.854595 NferModule-0.9.8/python/
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     3820 2021-05-14 09:08:44.000000 NferModule-0.9.8/python/README.md
-drwxr-xr-x   0 sb37fk    (1000) sb37fk    (1000)        0 2021-05-21 09:52:17.857929 NferModule-0.9.8/python/nfer/
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)        0 2021-05-11 13:52:21.000000 NferModule-0.9.8/python/nfer/__init__.py
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     4584 2021-05-14 09:05:42.000000 NferModule-0.9.8/python/nfer/gui.py
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     6611 2021-05-11 13:52:21.000000 NferModule-0.9.8/python/nfer/instrument.py
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     4241 2021-05-14 07:36:39.000000 NferModule-0.9.8/python/nfer/nfer.py
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     6009 2021-05-11 13:52:21.000000 NferModule-0.9.8/python/nfer/rules.py
-drwxr-xr-x   0 sb37fk    (1000) sb37fk    (1000)        0 2021-05-21 09:52:17.857929 NferModule-0.9.8/python/nfer/static/
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)   242742 2021-05-11 13:52:21.000000 NferModule-0.9.8/python/nfer/static/d3.min.js
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     2958 2021-05-11 13:52:21.000000 NferModule-0.9.8/python/nfer/static/favicon.ico
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)    18158 2021-05-11 13:52:21.000000 NferModule-0.9.8/python/nfer/static/nfergui.js
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)    64273 2021-05-11 13:52:21.000000 NferModule-0.9.8/python/nfer/static/socket.io.min.js
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)   160264 2021-05-11 13:52:21.000000 NferModule-0.9.8/python/nfer/static/socket.io.min.js.map
-drwxr-xr-x   0 sb37fk    (1000) sb37fk    (1000)        0 2021-05-21 09:52:17.861262 NferModule-0.9.8/python/nfer/www/
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     7465 2021-05-11 13:52:21.000000 NferModule-0.9.8/python/nfer/www/index.html
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)       38 2021-05-21 09:52:17.871262 NferModule-0.9.8/setup.cfg
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     4184 2021-05-21 09:52:04.000000 NferModule-0.9.8/setup.py
-drwxr-xr-x   0 sb37fk    (1000) sb37fk    (1000)        0 2021-05-21 09:52:17.867929 NferModule-0.9.8/src/
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)    14175 2021-05-07 11:17:35.000000 NferModule-0.9.8/src/ast.c
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)    21334 2021-05-07 11:17:35.000000 NferModule-0.9.8/src/astutil.c
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     7235 2021-05-07 11:17:35.000000 NferModule-0.9.8/src/dict.c
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)    38928 2021-05-07 11:17:35.000000 NferModule-0.9.8/src/expression.c
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)    18108 2021-05-07 11:17:35.000000 NferModule-0.9.8/src/file.c
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)    23621 2021-05-07 11:17:35.000000 NferModule-0.9.8/src/generate.c
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)    10868 2021-05-11 13:52:21.000000 NferModule-0.9.8/src/learn.c
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     2938 2021-05-07 11:17:35.000000 NferModule-0.9.8/src/log.c
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)    10888 2021-05-07 11:17:35.000000 NferModule-0.9.8/src/map.c
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     2514 2021-05-07 11:17:35.000000 NferModule-0.9.8/src/memory.c
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)    34512 2021-05-07 11:17:35.000000 NferModule-0.9.8/src/nfer.c
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)    13277 2021-05-07 11:17:35.000000 NferModule-0.9.8/src/pool.c
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)    16130 2021-05-11 13:52:21.000000 NferModule-0.9.8/src/pyinterface.c
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)    51881 2021-05-07 11:17:35.000000 NferModule-0.9.8/src/semantic.c
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     3700 2021-05-07 11:17:35.000000 NferModule-0.9.8/src/stack.c
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     3594 2021-05-07 11:17:35.000000 NferModule-0.9.8/src/strings.c
--rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     2252 2021-05-07 11:17:35.000000 NferModule-0.9.8/src/types.c
+drwxr-xr-x   0 sb37fk    (1000) sb37fk    (1000)        0 2021-05-21 12:23:35.772992 NferModule-0.9.9/
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)    34176 2021-05-07 11:17:34.000000 NferModule-0.9.9/COPYING
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)      161 2021-05-21 09:42:14.000000 NferModule-0.9.9/MANIFEST.in
+drwxr-xr-x   0 sb37fk    (1000) sb37fk    (1000)        0 2021-05-21 12:23:35.766326 NferModule-0.9.9/NferModule.egg-info/
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     4949 2021-05-21 12:23:35.000000 NferModule-0.9.9/NferModule.egg-info/PKG-INFO
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     1124 2021-05-21 12:23:35.000000 NferModule-0.9.9/NferModule.egg-info/SOURCES.txt
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)        1 2021-05-21 12:23:35.000000 NferModule-0.9.9/NferModule.egg-info/dependency_links.txt
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)        1 2021-05-21 09:24:22.000000 NferModule-0.9.9/NferModule.egg-info/not-zip-safe
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)       37 2021-05-21 12:23:35.000000 NferModule-0.9.9/NferModule.egg-info/requires.txt
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)       11 2021-05-21 12:23:35.000000 NferModule-0.9.9/NferModule.egg-info/top_level.txt
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     4949 2021-05-21 12:23:35.772992 NferModule-0.9.9/PKG-INFO
+drwxr-xr-x   0 sb37fk    (1000) sb37fk    (1000)        0 2021-05-21 12:23:35.762992 NferModule-0.9.9/gensrc/
+drwxr-xr-x   0 sb37fk    (1000) sb37fk    (1000)        0 2021-05-21 12:23:35.766326 NferModule-0.9.9/gensrc/parser/
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)    78516 2021-05-20 13:46:42.000000 NferModule-0.9.9/gensrc/parser/dsl.tab.c
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     6861 2021-05-20 13:46:42.000000 NferModule-0.9.9/gensrc/parser/dsl.tab.h
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)    71752 2021-05-20 13:46:42.000000 NferModule-0.9.9/gensrc/parser/dsl.yy.c
+drwxr-xr-x   0 sb37fk    (1000) sb37fk    (1000)        0 2021-05-21 12:23:35.769659 NferModule-0.9.9/inc/
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     1056 2021-05-07 11:17:35.000000 NferModule-0.9.9/inc/analysis.h
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     6688 2021-05-07 11:17:35.000000 NferModule-0.9.9/inc/ast.h
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     1044 2021-05-07 11:17:35.000000 NferModule-0.9.9/inc/astutil.h
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)      312 2021-05-07 11:17:35.000000 NferModule-0.9.9/inc/compile.h
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     1161 2021-05-12 15:51:15.000000 NferModule-0.9.9/inc/debug.h
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     1990 2021-05-07 11:17:35.000000 NferModule-0.9.9/inc/dict.h
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     1183 2021-05-11 13:52:21.000000 NferModule-0.9.9/inc/dsl.h
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     2305 2021-05-07 11:17:35.000000 NferModule-0.9.9/inc/expression.h
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     1370 2021-05-07 11:17:35.000000 NferModule-0.9.9/inc/file.h
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     1141 2021-05-07 11:17:35.000000 NferModule-0.9.9/inc/generate.h
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     2016 2021-05-07 11:17:35.000000 NferModule-0.9.9/inc/learn.h
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     1574 2021-05-07 11:17:35.000000 NferModule-0.9.9/inc/log.h
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     2216 2021-05-07 11:17:35.000000 NferModule-0.9.9/inc/map.h
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     1088 2021-05-07 11:17:35.000000 NferModule-0.9.9/inc/memory.h
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     4495 2021-05-07 11:17:35.000000 NferModule-0.9.9/inc/nfer.h
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     2730 2021-05-07 11:17:35.000000 NferModule-0.9.9/inc/pool.h
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)      635 2021-05-07 11:17:35.000000 NferModule-0.9.9/inc/rdc.h
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     1479 2021-05-07 11:17:35.000000 NferModule-0.9.9/inc/semantic.h
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     1320 2021-05-07 11:17:35.000000 NferModule-0.9.9/inc/stack.h
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     1261 2021-05-07 11:17:35.000000 NferModule-0.9.9/inc/strings.h
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     2269 2021-05-07 11:17:35.000000 NferModule-0.9.9/inc/target.h
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     2222 2021-05-07 11:17:35.000000 NferModule-0.9.9/inc/types.h
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)      103 2021-05-20 09:41:13.000000 NferModule-0.9.9/pyproject.toml
+drwxr-xr-x   0 sb37fk    (1000) sb37fk    (1000)        0 2021-05-21 12:23:35.769659 NferModule-0.9.9/python/
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     3820 2021-05-14 09:08:44.000000 NferModule-0.9.9/python/README.md
+drwxr-xr-x   0 sb37fk    (1000) sb37fk    (1000)        0 2021-05-21 12:23:35.769659 NferModule-0.9.9/python/nfer/
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)        0 2021-05-11 13:52:21.000000 NferModule-0.9.9/python/nfer/__init__.py
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     4584 2021-05-14 09:05:42.000000 NferModule-0.9.9/python/nfer/gui.py
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     6611 2021-05-11 13:52:21.000000 NferModule-0.9.9/python/nfer/instrument.py
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     4241 2021-05-14 07:36:39.000000 NferModule-0.9.9/python/nfer/nfer.py
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     6009 2021-05-11 13:52:21.000000 NferModule-0.9.9/python/nfer/rules.py
+drwxr-xr-x   0 sb37fk    (1000) sb37fk    (1000)        0 2021-05-21 12:23:35.769659 NferModule-0.9.9/python/nfer/static/
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)   242742 2021-05-11 13:52:21.000000 NferModule-0.9.9/python/nfer/static/d3.min.js
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     2958 2021-05-11 13:52:21.000000 NferModule-0.9.9/python/nfer/static/favicon.ico
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)    18158 2021-05-11 13:52:21.000000 NferModule-0.9.9/python/nfer/static/nfergui.js
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)    64273 2021-05-11 13:52:21.000000 NferModule-0.9.9/python/nfer/static/socket.io.min.js
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)   160264 2021-05-11 13:52:21.000000 NferModule-0.9.9/python/nfer/static/socket.io.min.js.map
+drwxr-xr-x   0 sb37fk    (1000) sb37fk    (1000)        0 2021-05-21 12:23:35.769659 NferModule-0.9.9/python/nfer/www/
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     7465 2021-05-11 13:52:21.000000 NferModule-0.9.9/python/nfer/www/index.html
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)       38 2021-05-21 12:23:35.772992 NferModule-0.9.9/setup.cfg
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     4396 2021-05-21 12:23:29.000000 NferModule-0.9.9/setup.py
+drwxr-xr-x   0 sb37fk    (1000) sb37fk    (1000)        0 2021-05-21 12:23:35.772992 NferModule-0.9.9/src/
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)    14175 2021-05-07 11:17:35.000000 NferModule-0.9.9/src/ast.c
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)    21334 2021-05-07 11:17:35.000000 NferModule-0.9.9/src/astutil.c
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     7235 2021-05-07 11:17:35.000000 NferModule-0.9.9/src/dict.c
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)    38928 2021-05-07 11:17:35.000000 NferModule-0.9.9/src/expression.c
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)    18108 2021-05-07 11:17:35.000000 NferModule-0.9.9/src/file.c
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)    23621 2021-05-07 11:17:35.000000 NferModule-0.9.9/src/generate.c
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)    10868 2021-05-11 13:52:21.000000 NferModule-0.9.9/src/learn.c
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     2938 2021-05-07 11:17:35.000000 NferModule-0.9.9/src/log.c
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)    10888 2021-05-07 11:17:35.000000 NferModule-0.9.9/src/map.c
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     2514 2021-05-07 11:17:35.000000 NferModule-0.9.9/src/memory.c
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)    34512 2021-05-07 11:17:35.000000 NferModule-0.9.9/src/nfer.c
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)    13277 2021-05-07 11:17:35.000000 NferModule-0.9.9/src/pool.c
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)    16130 2021-05-11 13:52:21.000000 NferModule-0.9.9/src/pyinterface.c
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)    51881 2021-05-07 11:17:35.000000 NferModule-0.9.9/src/semantic.c
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     3700 2021-05-07 11:17:35.000000 NferModule-0.9.9/src/stack.c
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     3594 2021-05-07 11:17:35.000000 NferModule-0.9.9/src/strings.c
+-rw-r--r--   0 sb37fk    (1000) sb37fk    (1000)     2252 2021-05-07 11:17:35.000000 NferModule-0.9.9/src/types.c
```

### Comparing `NferModule-0.9.8/COPYING` & `NferModule-0.9.9/COPYING`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/NferModule.egg-info/PKG-INFO` & `NferModule-0.9.9/NferModule.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NferModule
-Version: 0.9.8
+Version: 0.9.9
 Summary: The nfer language for Python
 Home-page: http://nfer.io/
 Author: Sean Kauffman
 Author-email: skauffma@uwaterloo.ca
 License: UNKNOWN
 Description: Nfer for Python - Debugging Asynchronous Programs Made Easier
         =============================================================================
```

### Comparing `NferModule-0.9.8/NferModule.egg-info/SOURCES.txt` & `NferModule-0.9.9/NferModule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/PKG-INFO` & `NferModule-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NferModule
-Version: 0.9.8
+Version: 0.9.9
 Summary: The nfer language for Python
 Home-page: http://nfer.io/
 Author: Sean Kauffman
 Author-email: skauffma@uwaterloo.ca
 License: UNKNOWN
 Description: Nfer for Python - Debugging Asynchronous Programs Made Easier
         =============================================================================
```

### Comparing `NferModule-0.9.8/gensrc/parser/dsl.tab.c` & `NferModule-0.9.9/gensrc/parser/dsl.tab.c`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/gensrc/parser/dsl.tab.h` & `NferModule-0.9.9/gensrc/parser/dsl.tab.h`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/gensrc/parser/dsl.yy.c` & `NferModule-0.9.9/gensrc/parser/dsl.yy.c`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/inc/analysis.h` & `NferModule-0.9.9/inc/analysis.h`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/inc/ast.h` & `NferModule-0.9.9/inc/ast.h`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/inc/astutil.h` & `NferModule-0.9.9/inc/astutil.h`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/inc/debug.h` & `NferModule-0.9.9/inc/debug.h`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/inc/dict.h` & `NferModule-0.9.9/inc/dict.h`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/inc/dsl.h` & `NferModule-0.9.9/inc/dsl.h`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/inc/expression.h` & `NferModule-0.9.9/inc/expression.h`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/inc/file.h` & `NferModule-0.9.9/inc/file.h`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/inc/generate.h` & `NferModule-0.9.9/inc/generate.h`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/inc/learn.h` & `NferModule-0.9.9/inc/learn.h`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/inc/log.h` & `NferModule-0.9.9/inc/log.h`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/inc/map.h` & `NferModule-0.9.9/inc/map.h`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/inc/memory.h` & `NferModule-0.9.9/inc/memory.h`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/inc/nfer.h` & `NferModule-0.9.9/inc/nfer.h`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/inc/pool.h` & `NferModule-0.9.9/inc/pool.h`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/inc/rdc.h` & `NferModule-0.9.9/inc/rdc.h`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/inc/semantic.h` & `NferModule-0.9.9/inc/semantic.h`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/inc/stack.h` & `NferModule-0.9.9/inc/stack.h`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/inc/strings.h` & `NferModule-0.9.9/inc/strings.h`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/inc/target.h` & `NferModule-0.9.9/inc/target.h`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/inc/types.h` & `NferModule-0.9.9/inc/types.h`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/python/README.md` & `NferModule-0.9.9/python/README.md`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/python/nfer/gui.py` & `NferModule-0.9.9/python/nfer/gui.py`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/python/nfer/instrument.py` & `NferModule-0.9.9/python/nfer/instrument.py`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/python/nfer/nfer.py` & `NferModule-0.9.9/python/nfer/nfer.py`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/python/nfer/rules.py` & `NferModule-0.9.9/python/nfer/rules.py`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/python/nfer/static/d3.min.js` & `NferModule-0.9.9/python/nfer/static/d3.min.js`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/python/nfer/static/favicon.ico` & `NferModule-0.9.9/python/nfer/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/python/nfer/static/nfergui.js` & `NferModule-0.9.9/python/nfer/static/nfergui.js`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/python/nfer/static/socket.io.min.js` & `NferModule-0.9.9/python/nfer/static/socket.io.min.js`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/python/nfer/static/socket.io.min.js.map` & `NferModule-0.9.9/python/nfer/static/socket.io.min.js.map`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/python/nfer/www/index.html` & `NferModule-0.9.9/python/nfer/www/index.html`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/setup.py` & `NferModule-0.9.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,21 +46,29 @@
     # check if the parser source dir exists at all and create it if not
     if not os.path.exists(parser_dir):
         # using the distutils helper
         mkpath(parser_dir)
 
     # check for the lexer source and create it if it doesn't exist or is outdated
     lexer_l = os.path.join('src', 'dsl.l')
-    if not os.path.exists(lexer_src) or os.path.getmtime(lexer_src) < os.path.getmtime(lexer_l):
+    lexer_src_is_old = True
+    if os.path.exists(lexer_src) and os.path.exists(lexer_l):
+        lexer_src_is_old = os.path.getmtime(lexer_src) < os.path.getmtime(lexer_l)
+    
+    if lexer_src_is_old:
         print('running flex')
         os.system('flex -o ' + lexer_src + ' ' + lexer_l)
 
     # check for the parser source and create it if it doesn't exist or is outdated
     parser_y = os.path.join('src', 'dsl.y')
-    if not os.path.exists(parser_src) or os.path.getmtime(parser_src) < os.path.getmtime(parser_y):
+    parser_src_is_old = True
+    if os.path.exists(parser_src) and os.path.exists(parser_y):
+        parser_src_is_old = os.path.getmtime(parser_src) < os.path.getmtime(parser_y)
+
+    if parser_src_is_old:
         print('running bison')
         os.system('bison -d -o ' + parser_src + ' ' + parser_y)
 
 
 class NferBuildPy(build_ext):
     def run(self):
         "overriding the build_ext command called by install to ensure the lexer/parser source exists"
@@ -82,15 +90,15 @@
             generate_lexer_parser_source()
 
         # call the super class method
         return sdist.run(self)
 
 
 setup (name = 'NferModule',
-       version = '0.9.8',
+       version = '0.9.9',
        description = 'The nfer language for Python',
        long_description = README,
        long_description_content_type = 'text/markdown',
        author = 'Sean Kauffman',
        author_email = 'skauffma@uwaterloo.ca',
        url = 'http://nfer.io/',
        package_dir = {'nfer': os.path.join('python', 'nfer')},
```

### Comparing `NferModule-0.9.8/src/ast.c` & `NferModule-0.9.9/src/ast.c`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/src/astutil.c` & `NferModule-0.9.9/src/astutil.c`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/src/dict.c` & `NferModule-0.9.9/src/dict.c`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/src/expression.c` & `NferModule-0.9.9/src/expression.c`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/src/file.c` & `NferModule-0.9.9/src/file.c`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/src/generate.c` & `NferModule-0.9.9/src/generate.c`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/src/learn.c` & `NferModule-0.9.9/src/learn.c`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/src/log.c` & `NferModule-0.9.9/src/log.c`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/src/map.c` & `NferModule-0.9.9/src/map.c`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/src/memory.c` & `NferModule-0.9.9/src/memory.c`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/src/nfer.c` & `NferModule-0.9.9/src/nfer.c`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/src/pool.c` & `NferModule-0.9.9/src/pool.c`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/src/pyinterface.c` & `NferModule-0.9.9/src/pyinterface.c`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/src/semantic.c` & `NferModule-0.9.9/src/semantic.c`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/src/stack.c` & `NferModule-0.9.9/src/stack.c`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/src/strings.c` & `NferModule-0.9.9/src/strings.c`

 * *Files identical despite different names*

### Comparing `NferModule-0.9.8/src/types.c` & `NferModule-0.9.9/src/types.c`

 * *Files identical despite different names*

