# Comparing `tmp/GameserverLister-1.0.6.tar.gz` & `tmp/GameserverLister-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GameserverLister-1.0.6.tar", last modified: Thu Mar 30 16:56:00 2023, max compression
+gzip compressed data, was "GameserverLister-1.0.7.tar", last modified: Wed Apr 12 20:50:10 2023, max compression
```

## Comparing `GameserverLister-1.0.6.tar` & `GameserverLister-1.0.7.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:00.204778 GameserverLister-1.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:00.196777 GameserverLister-1.0.6/GameserverLister/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:00.200778 GameserverLister-1.0.6/GameserverLister/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/commands/battlelog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/commands/bfbc2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/commands/gamespy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/commands/gametools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/commands/medalofhonor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:00.200778 GameserverLister-1.0.6/GameserverLister/commands/options/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/commands/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/commands/options/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/commands/options/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/commands/options/queryport.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/commands/quake3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/commands/unreal2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/commands/valve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:00.200778 GameserverLister-1.0.6/GameserverLister/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/common/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/common/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    16146 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/common/servers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/common/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/common/weblinks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:00.200778 GameserverLister-1.0.6/GameserverLister/games/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/games/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/games/battlelog.py
--rw-r--r--   0 runner    (1001) docker     (123)     9846 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/games/gamespy.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/games/gametools.py
--rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/games/quake3.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/games/unreal2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/games/valve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:00.204778 GameserverLister-1.0.6/GameserverLister/listers/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/listers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/listers/battlelog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/listers/bfbc2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/listers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    10020 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/listers/gamespy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/listers/gametools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/listers/medalofhonor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/listers/quake3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/listers/unreal2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/GameserverLister/listers/valve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:00.196777 GameserverLister-1.0.6/GameserverLister.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17254 2023-03-30 16:56:00.000000 GameserverLister-1.0.6/GameserverLister.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-03-30 16:56:00.000000 GameserverLister-1.0.6/GameserverLister.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 16:56:00.000000 GameserverLister-1.0.6/GameserverLister.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-30 16:56:00.000000 GameserverLister-1.0.6/GameserverLister.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-30 16:56:00.000000 GameserverLister-1.0.6/GameserverLister.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-30 16:56:00.000000 GameserverLister-1.0.6/GameserverLister.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    17254 2023-03-30 16:56:00.204778 GameserverLister-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16034 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-03-30 16:56:00.204778 GameserverLister-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 16:55:49.000000 GameserverLister-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:50:10.723283 GameserverLister-1.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:50:10.715283 GameserverLister-1.0.7/GameserverLister/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:50:10.719283 GameserverLister-1.0.7/GameserverLister/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/commands/battlelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/commands/bfbc2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/commands/gamespy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/commands/gametools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/commands/medalofhonor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:50:10.719283 GameserverLister-1.0.7/GameserverLister/commands/options/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/commands/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/commands/options/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/commands/options/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/commands/options/queryport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/commands/quake3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/commands/unreal2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/commands/valve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:50:10.719283 GameserverLister-1.0.7/GameserverLister/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/common/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/common/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16146 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/common/servers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/common/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/common/weblinks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:50:10.719283 GameserverLister-1.0.7/GameserverLister/games/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/games/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/games/battlelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9846 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/games/gamespy.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/games/gametools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/games/quake3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/games/unreal2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/games/valve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:50:10.723283 GameserverLister-1.0.7/GameserverLister/listers/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/listers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/listers/battlelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/listers/bfbc2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/listers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10020 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/listers/gamespy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/listers/gametools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/listers/medalofhonor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/listers/quake3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/listers/unreal2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/GameserverLister/listers/valve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:50:10.719283 GameserverLister-1.0.7/GameserverLister.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17988 2023-04-12 20:50:10.000000 GameserverLister-1.0.7/GameserverLister.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-12 20:50:10.000000 GameserverLister-1.0.7/GameserverLister.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 20:50:10.000000 GameserverLister-1.0.7/GameserverLister.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-12 20:50:10.000000 GameserverLister-1.0.7/GameserverLister.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-12 20:50:10.000000 GameserverLister-1.0.7/GameserverLister.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-12 20:50:10.000000 GameserverLister-1.0.7/GameserverLister.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17988 2023-04-12 20:50:10.723283 GameserverLister-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16768 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-12 20:50:10.723283 GameserverLister-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 20:50:02.000000 GameserverLister-1.0.7/setup.py
```

### Comparing `GameserverLister-1.0.6/GameserverLister/__main__.py` & `GameserverLister-1.0.7/GameserverLister/__main__.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.0.6/GameserverLister/commands/battlelog.py` & `GameserverLister-1.0.7/GameserverLister/commands/battlelog.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.0.6/GameserverLister/commands/bfbc2.py` & `GameserverLister-1.0.7/GameserverLister/commands/bfbc2.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.0.6/GameserverLister/commands/gamespy.py` & `GameserverLister-1.0.7/GameserverLister/commands/gamespy.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.0.6/GameserverLister/commands/gametools.py` & `GameserverLister-1.0.7/GameserverLister/commands/gametools.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.0.6/GameserverLister/commands/medalofhonor.py` & `GameserverLister-1.0.7/GameserverLister/commands/medalofhonor.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.0.6/GameserverLister/commands/options/common.py` & `GameserverLister-1.0.7/GameserverLister/commands/options/common.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.0.6/GameserverLister/commands/options/http.py` & `GameserverLister-1.0.7/GameserverLister/commands/options/http.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.0.6/GameserverLister/commands/quake3.py` & `GameserverLister-1.0.7/GameserverLister/commands/quake3.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.0.6/GameserverLister/commands/unreal2.py` & `GameserverLister-1.0.7/GameserverLister/commands/unreal2.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.0.6/GameserverLister/commands/valve.py` & `GameserverLister-1.0.7/GameserverLister/commands/valve.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.0.6/GameserverLister/common/helpers.py` & `GameserverLister-1.0.7/GameserverLister/common/helpers.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.0.6/GameserverLister/common/servers.py` & `GameserverLister-1.0.7/GameserverLister/common/servers.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.0.6/GameserverLister/common/types.py` & `GameserverLister-1.0.7/GameserverLister/common/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,14 +132,15 @@
     CounterStrikeConditionZero = 'cscz'
     CounterStrikeSource = 'css'
     CounterStrikeGlobalOffensive = 'csgo'
     DayZ = 'dayz'
     DayZMod = 'dayzmod'
     DoD = 'dod'
     DoDS = 'dods'
+    GarrysMod = 'gmod'
     Insurgency = 'insurgency'
     InsurgencySandstorm = 'insurgency-sandstorm'
     Left4Dead = 'left4dead'
     Left4Dead2 = 'left4dead2'
     RS2 = 'rs2'
     Rust = 'rust'
     SevenD2D = '7d2d'
```

### Comparing `GameserverLister-1.0.6/GameserverLister/common/weblinks.py` & `GameserverLister-1.0.7/GameserverLister/common/weblinks.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.0.6/GameserverLister/games/gamespy.py` & `GameserverLister-1.0.7/GameserverLister/games/gamespy.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.0.6/GameserverLister/games/quake3.py` & `GameserverLister-1.0.7/GameserverLister/games/quake3.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.0.6/GameserverLister/games/unreal2.py` & `GameserverLister-1.0.7/GameserverLister/games/unreal2.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.0.6/GameserverLister/games/valve.py` & `GameserverLister-1.0.7/GameserverLister/games/valve.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,20 @@
     ),
     ValveGame.DoDS: ValveGameConfig(
         app_id=300,
         principals=[
             ValvePrincipal.VALVE
         ]
     ),
+    ValveGame.GarrysMod: ValveGameConfig(
+        app_id=4000,
+        principals=[
+            ValvePrincipal.VALVE
+        ]
+    ),
     ValveGame.Insurgency: ValveGameConfig(
         app_id=222880,
         principals=[
             ValvePrincipal.VALVE
         ]
     ),
     ValveGame.InsurgencySandstorm: ValveGameConfig(
```

### Comparing `GameserverLister-1.0.6/GameserverLister/listers/__init__.py` & `GameserverLister-1.0.7/GameserverLister/listers/__init__.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.0.6/GameserverLister/listers/battlelog.py` & `GameserverLister-1.0.7/GameserverLister/listers/battlelog.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.0.6/GameserverLister/listers/bfbc2.py` & `GameserverLister-1.0.7/GameserverLister/listers/bfbc2.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.0.6/GameserverLister/listers/common.py` & `GameserverLister-1.0.7/GameserverLister/listers/common.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.0.6/GameserverLister/listers/gamespy.py` & `GameserverLister-1.0.7/GameserverLister/listers/gamespy.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.0.6/GameserverLister/listers/gametools.py` & `GameserverLister-1.0.7/GameserverLister/listers/gametools.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.0.6/GameserverLister/listers/medalofhonor.py` & `GameserverLister-1.0.7/GameserverLister/listers/medalofhonor.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.0.6/GameserverLister/listers/quake3.py` & `GameserverLister-1.0.7/GameserverLister/listers/quake3.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.0.6/GameserverLister/listers/unreal2.py` & `GameserverLister-1.0.7/GameserverLister/listers/unreal2.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.0.6/GameserverLister/listers/valve.py` & `GameserverLister-1.0.7/GameserverLister/listers/valve.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.0.6/GameserverLister.egg-info/PKG-INFO` & `GameserverLister-1.0.7/GameserverLister.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GameserverLister
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python command line tool to retrieve game server lists for various games
 Home-page: https://github.com/cetteup/GameserverLister
 Author: cetteup
 Author-email: me@cetteup.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cetteup/GameserverLister/issues
 Classifier: Development Status :: 4 - Beta
@@ -41,14 +41,48 @@
 
 - create/update lists of game servers stored as JSON
 - removal of servers not seen in a configurable timespan
 - search game server's query ports if not contained in server list
 - handle completely broken pagination on Battlelog
 - proxy support for requests to Battlelog
 
+## Usage
+
+You can easily install GameserverLister via pip.
+
+```bash
+pip install GameserverLister
+```
+
+Upgrading from an older version is equally simple.
+
+```bash
+pip install --upgrade GameserverLister
+```
+
+After installing through pip, you can get some help for the command line options through
+
+```bash
+$ python3 -m GameserverLister --help
+Usage: python -m GameserverLister [OPTIONS] COMMAND [ARGS]...
+
+Options:
+  --help  Show this message and exit.
+
+Commands:
+  battlelog
+  bfbc2
+  gamespy
+  gametools
+  medalofhonor
+  quake3
+  unreal2
+  valve
+```
+
 ## Required tools
 
 The server list retrieval for GameSpy-games requires an external tool. In order to retrieve GameSpy servers, you need to set up [gslist](http://aluigi.altervista.org/papers.htm#gslist). `gslist` was developed by Luigi Auriemma.
 
 ## Supported games
 
 The scripts support retrieval for following games from the listed sources. If you know more sources for any of the listed games or know other games that support the listed protocols, please create an issue, and I will add them.
@@ -84,14 +118,15 @@
 | Day of Defeat                          | Valve                | Valve ¹                                                                                                           |
 | Day of Defeat: Source                  | Valve                | Valve ¹                                                                                                           |
 | DayZ                                   | Valve                | Valve ¹                                                                                                           |
 | DayZ (Arma 2 mod)                      | Valve                | Valve ¹                                                                                                           |
 | Deus Ex                                | GameSpy              | 333networks.com, errorist.eu, newbiesplayground.net, oldunreal.com                                                |
 | Duke Nukem Forever                     | GameSpy              | 333networks.com                                                                                                   |
 | Forgotten Hope 2                       | GameSpy              | fh2.dev                                                                                                           |
+| Garry's Mod                            | Valve                | Valve ¹                                                                                                           |
 | Insurgency                             | Valve                | Valve ¹                                                                                                           |
 | Insurgency: Sandstorm                  | Valve                | Valve ¹                                                                                                           |
 | James Bond 007: Nightfire              | GameSpy              | openspy.net, nightfirepc.com                                                                                      |
 | Left 4 Dead                            | Valve                | Valve ¹                                                                                                           |
 | Left 4 Dead 2                          | Valve                | Valve ¹                                                                                                           |
 | Medal of Honor Warfighter              | Battlelog            | battlelog.com                                                                                                     |
 | Nexuiz                                 | Quake3               | deathmask.net                                                                                                     |
```

### Comparing `GameserverLister-1.0.6/GameserverLister.egg-info/SOURCES.txt` & `GameserverLister-1.0.7/GameserverLister.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.0.6/LICENSE.md` & `GameserverLister-1.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.0.6/PKG-INFO` & `GameserverLister-1.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GameserverLister
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python command line tool to retrieve game server lists for various games
 Home-page: https://github.com/cetteup/GameserverLister
 Author: cetteup
 Author-email: me@cetteup.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cetteup/GameserverLister/issues
 Classifier: Development Status :: 4 - Beta
@@ -41,14 +41,48 @@
 
 - create/update lists of game servers stored as JSON
 - removal of servers not seen in a configurable timespan
 - search game server's query ports if not contained in server list
 - handle completely broken pagination on Battlelog
 - proxy support for requests to Battlelog
 
+## Usage
+
+You can easily install GameserverLister via pip.
+
+```bash
+pip install GameserverLister
+```
+
+Upgrading from an older version is equally simple.
+
+```bash
+pip install --upgrade GameserverLister
+```
+
+After installing through pip, you can get some help for the command line options through
+
+```bash
+$ python3 -m GameserverLister --help
+Usage: python -m GameserverLister [OPTIONS] COMMAND [ARGS]...
+
+Options:
+  --help  Show this message and exit.
+
+Commands:
+  battlelog
+  bfbc2
+  gamespy
+  gametools
+  medalofhonor
+  quake3
+  unreal2
+  valve
+```
+
 ## Required tools
 
 The server list retrieval for GameSpy-games requires an external tool. In order to retrieve GameSpy servers, you need to set up [gslist](http://aluigi.altervista.org/papers.htm#gslist). `gslist` was developed by Luigi Auriemma.
 
 ## Supported games
 
 The scripts support retrieval for following games from the listed sources. If you know more sources for any of the listed games or know other games that support the listed protocols, please create an issue, and I will add them.
@@ -84,14 +118,15 @@
 | Day of Defeat                          | Valve                | Valve ¹                                                                                                           |
 | Day of Defeat: Source                  | Valve                | Valve ¹                                                                                                           |
 | DayZ                                   | Valve                | Valve ¹                                                                                                           |
 | DayZ (Arma 2 mod)                      | Valve                | Valve ¹                                                                                                           |
 | Deus Ex                                | GameSpy              | 333networks.com, errorist.eu, newbiesplayground.net, oldunreal.com                                                |
 | Duke Nukem Forever                     | GameSpy              | 333networks.com                                                                                                   |
 | Forgotten Hope 2                       | GameSpy              | fh2.dev                                                                                                           |
+| Garry's Mod                            | Valve                | Valve ¹                                                                                                           |
 | Insurgency                             | Valve                | Valve ¹                                                                                                           |
 | Insurgency: Sandstorm                  | Valve                | Valve ¹                                                                                                           |
 | James Bond 007: Nightfire              | GameSpy              | openspy.net, nightfirepc.com                                                                                      |
 | Left 4 Dead                            | Valve                | Valve ¹                                                                                                           |
 | Left 4 Dead 2                          | Valve                | Valve ¹                                                                                                           |
 | Medal of Honor Warfighter              | Battlelog            | battlelog.com                                                                                                     |
 | Nexuiz                                 | Quake3               | deathmask.net                                                                                                     |
```

### Comparing `GameserverLister-1.0.6/README.md` & `GameserverLister-1.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,48 @@
 
 - create/update lists of game servers stored as JSON
 - removal of servers not seen in a configurable timespan
 - search game server's query ports if not contained in server list
 - handle completely broken pagination on Battlelog
 - proxy support for requests to Battlelog
 
+## Usage
+
+You can easily install GameserverLister via pip.
+
+```bash
+pip install GameserverLister
+```
+
+Upgrading from an older version is equally simple.
+
+```bash
+pip install --upgrade GameserverLister
+```
+
+After installing through pip, you can get some help for the command line options through
+
+```bash
+$ python3 -m GameserverLister --help
+Usage: python -m GameserverLister [OPTIONS] COMMAND [ARGS]...
+
+Options:
+  --help  Show this message and exit.
+
+Commands:
+  battlelog
+  bfbc2
+  gamespy
+  gametools
+  medalofhonor
+  quake3
+  unreal2
+  valve
+```
+
 ## Required tools
 
 The server list retrieval for GameSpy-games requires an external tool. In order to retrieve GameSpy servers, you need to set up [gslist](http://aluigi.altervista.org/papers.htm#gslist). `gslist` was developed by Luigi Auriemma.
 
 ## Supported games
 
 The scripts support retrieval for following games from the listed sources. If you know more sources for any of the listed games or know other games that support the listed protocols, please create an issue, and I will add them.
@@ -54,14 +88,15 @@
 | Day of Defeat                          | Valve                | Valve ¹                                                                                                           |
 | Day of Defeat: Source                  | Valve                | Valve ¹                                                                                                           |
 | DayZ                                   | Valve                | Valve ¹                                                                                                           |
 | DayZ (Arma 2 mod)                      | Valve                | Valve ¹                                                                                                           |
 | Deus Ex                                | GameSpy              | 333networks.com, errorist.eu, newbiesplayground.net, oldunreal.com                                                |
 | Duke Nukem Forever                     | GameSpy              | 333networks.com                                                                                                   |
 | Forgotten Hope 2                       | GameSpy              | fh2.dev                                                                                                           |
+| Garry's Mod                            | Valve                | Valve ¹                                                                                                           |
 | Insurgency                             | Valve                | Valve ¹                                                                                                           |
 | Insurgency: Sandstorm                  | Valve                | Valve ¹                                                                                                           |
 | James Bond 007: Nightfire              | GameSpy              | openspy.net, nightfirepc.com                                                                                      |
 | Left 4 Dead                            | Valve                | Valve ¹                                                                                                           |
 | Left 4 Dead 2                          | Valve                | Valve ¹                                                                                                           |
 | Medal of Honor Warfighter              | Battlelog            | battlelog.com                                                                                                     |
 | Nexuiz                                 | Quake3               | deathmask.net                                                                                                     |
```

### Comparing `GameserverLister-1.0.6/setup.cfg` & `GameserverLister-1.0.7/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = GameserverLister
-version = 1.0.6
+version = 1.0.7
 description = Python command line tool to retrieve game server lists for various games
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/cetteup/GameserverLister
 project_urls = 
 	Bug Tracker = https://github.com/cetteup/GameserverLister/issues
 author = cetteup
```

