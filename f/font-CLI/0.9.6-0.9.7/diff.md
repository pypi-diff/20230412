# Comparing `tmp/font-CLI-0.9.6.tar.gz` & `tmp/font-CLI-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "font-CLI-0.9.6.tar", last modified: Wed Apr  5 06:14:48 2023, max compression
+gzip compressed data, was "font-CLI-0.9.7.tar", last modified: Wed Apr 12 10:52:25 2023, max compression
```

## Comparing `font-CLI-0.9.6.tar` & `font-CLI-0.9.7.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 06:14:48.497955 font-CLI-0.9.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-05 06:14:37.000000 font-CLI-0.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    87188 2023-04-05 06:14:48.497955 font-CLI-0.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    86796 2023-04-05 06:14:37.000000 font-CLI-0.9.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 06:14:48.485955 font-CLI-0.9.6/font_CLI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    87188 2023-04-05 06:14:48.000000 font-CLI-0.9.6/font_CLI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-05 06:14:48.000000 font-CLI-0.9.6/font_CLI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 06:14:48.000000 font-CLI-0.9.6/font_CLI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-05 06:14:48.000000 font-CLI-0.9.6/font_CLI.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 06:14:48.000000 font-CLI-0.9.6/font_CLI.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-05 06:14:48.000000 font-CLI-0.9.6/font_CLI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-05 06:14:48.000000 font-CLI-0.9.6/font_CLI.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 06:14:48.485955 font-CLI-0.9.6/ftCLI/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 06:14:48.485955 font-CLI-0.9.6/ftCLI/Lib/
--rw-r--r--   0 runner    (1001) docker     (123)    28621 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/Lib/Font.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/Lib/VFont.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/Lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 06:14:48.489955 font-CLI-0.9.6/ftCLI/Lib/assistant/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/Lib/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26380 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/Lib/assistant/fonts_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/Lib/assistant/styles_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/Lib/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 06:14:48.489955 font-CLI-0.9.6/ftCLI/Lib/converter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/Lib/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/Lib/converter/otf_to_ttf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/Lib/converter/ttf_to_otf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 06:14:48.489955 font-CLI-0.9.6/ftCLI/Lib/cui/
--rw-r--r--   0 runner    (1001) docker     (123)    30721 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/Lib/cui/CUI.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/Lib/cui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 06:14:48.493955 font-CLI-0.9.6/ftCLI/Lib/tables/
--rw-r--r--   0 runner    (1001) docker     (123)    10260 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/Lib/tables/OS_2.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/Lib/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/Lib/tables/head.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/Lib/tables/hhea.py
--rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/Lib/tables/name.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/Lib/tables/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 06:14:48.493955 font-CLI-0.9.6/ftCLI/Lib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/Lib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/Lib/utils/cli_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/Lib/utils/click_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/Lib/utils/glyphs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/Lib/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 06:14:48.497955 font-CLI-0.9.6/ftCLI/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17345 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/commands/ftcli_assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/commands/ftcli_cff.py
--rw-r--r--   0 runner    (1001) docker     (123)    17743 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/commands/ftcli_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    26876 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/commands/ftcli_fix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/commands/ftcli_hhea.py
--rw-r--r--   0 runner    (1001) docker     (123)     9899 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/commands/ftcli_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13340 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/commands/ftcli_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    13230 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/commands/ftcli_os2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/commands/ftcli_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/commands/ftcli_print.py
--rw-r--r--   0 runner    (1001) docker     (123)    23335 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/commands/ftcli_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-05 06:14:37.000000 font-CLI-0.9.6/ftCLI/ftCLI.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 06:14:48.497955 font-CLI-0.9.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-05 06:14:37.000000 font-CLI-0.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:52:25.212588 font-CLI-0.9.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-12 10:52:15.000000 font-CLI-0.9.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    87188 2023-04-12 10:52:25.212588 font-CLI-0.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    86796 2023-04-12 10:52:15.000000 font-CLI-0.9.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:52:25.208588 font-CLI-0.9.7/font_CLI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    87188 2023-04-12 10:52:25.000000 font-CLI-0.9.7/font_CLI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-12 10:52:25.000000 font-CLI-0.9.7/font_CLI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 10:52:25.000000 font-CLI-0.9.7/font_CLI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-12 10:52:25.000000 font-CLI-0.9.7/font_CLI.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 10:52:25.000000 font-CLI-0.9.7/font_CLI.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-12 10:52:25.000000 font-CLI-0.9.7/font_CLI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 10:52:25.000000 font-CLI-0.9.7/font_CLI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:52:25.208588 font-CLI-0.9.7/ftCLI/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:52:25.208588 font-CLI-0.9.7/ftCLI/Lib/
+-rw-r--r--   0 runner    (1001) docker     (123)    28621 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/Font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/VFont.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:52:25.208588 font-CLI-0.9.7/ftCLI/Lib/assistant/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26380 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/assistant/fonts_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/assistant/styles_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:52:25.212588 font-CLI-0.9.7/ftCLI/Lib/converter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/converter/otf_to_ttf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/converter/ttf_to_otf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:52:25.212588 font-CLI-0.9.7/ftCLI/Lib/cui/
+-rw-r--r--   0 runner    (1001) docker     (123)    30721 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/cui/CUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/cui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:52:25.212588 font-CLI-0.9.7/ftCLI/Lib/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)    10260 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/tables/OS_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/tables/head.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/tables/hhea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/tables/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/tables/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:52:25.212588 font-CLI-0.9.7/ftCLI/Lib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/utils/cli_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/utils/click_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/utils/glyphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/Lib/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:52:25.212588 font-CLI-0.9.7/ftCLI/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17345 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/commands/ftcli_assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/commands/ftcli_cff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17781 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/commands/ftcli_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26876 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/commands/ftcli_fix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/commands/ftcli_hhea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9899 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/commands/ftcli_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13340 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/commands/ftcli_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13230 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/commands/ftcli_os2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/commands/ftcli_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/commands/ftcli_print.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23335 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/commands/ftcli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-12 10:52:15.000000 font-CLI-0.9.7/ftCLI/ftCLI.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 10:52:25.212588 font-CLI-0.9.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-12 10:52:15.000000 font-CLI-0.9.7/setup.py
```

### Comparing `font-CLI-0.9.6/LICENSE` & `font-CLI-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.6/PKG-INFO` & `font-CLI-0.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: font-CLI
-Version: 0.9.6
+Version: 0.9.7
 Summary: A set of command line tools to edit fonts with FontTools
 Home-page: https://github.com/ftCLI/ftCLI
 Author: ftCLI
 Author-email: ftcli@proton.me
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7, <3.11
@@ -261,20 +261,20 @@
 retrieved values and the JSON data, trying to determine the proper style names. The results are written into the
 `fonts_data.csv` file.
 
 The `fonts_data.csv` contains the following columns:
 
 - `file_name`: path to the font file
 - `family_name`: the font's family name, retrieved reading the name table
-- `is_bold`: True if ths bold bits are set, False if they are not set. This column is present only for completeness,
+- `is_bold`: True if the bold bits are set, False if they are not set. This column is present only for completeness,
   but it's value will be ignored. A font will be set as bold only and only if, while running the `ftcli assistant commit`
   command, the user will choose to use linked styles.
   (-ls / --linked styles) option while writing data from CSV to fonts
-- `is_italic`: True if ths italic bits are set, False if they are not set
-- `is_oblique`: True if ths oblique bit is set, False if it's not set
+- `is_italic`: True if the italic bits are set, False if they are not set
+- `is_oblique`: True if the oblique bit is set, False if it's not set
 - `us_width_class`: usWidthClass value
 - `us_weight_class`: usWeightClass value
 - `wdt`: short literal for the Width style name
 - `width`: long literal for the Width style name
 - `wgt`: short literal for the Weight style name
 - `weight`: long literal for the Weight style name
 - `slp`: short literal for the Slope style name
```

### Comparing `font-CLI-0.9.6/README.md` & `font-CLI-0.9.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -248,20 +248,20 @@
 retrieved values and the JSON data, trying to determine the proper style names. The results are written into the
 `fonts_data.csv` file.
 
 The `fonts_data.csv` contains the following columns:
 
 - `file_name`: path to the font file
 - `family_name`: the font's family name, retrieved reading the name table
-- `is_bold`: True if ths bold bits are set, False if they are not set. This column is present only for completeness,
+- `is_bold`: True if the bold bits are set, False if they are not set. This column is present only for completeness,
   but it's value will be ignored. A font will be set as bold only and only if, while running the `ftcli assistant commit`
   command, the user will choose to use linked styles.
   (-ls / --linked styles) option while writing data from CSV to fonts
-- `is_italic`: True if ths italic bits are set, False if they are not set
-- `is_oblique`: True if ths oblique bit is set, False if it's not set
+- `is_italic`: True if the italic bits are set, False if they are not set
+- `is_oblique`: True if the oblique bit is set, False if it's not set
 - `us_width_class`: usWidthClass value
 - `us_weight_class`: usWeightClass value
 - `wdt`: short literal for the Width style name
 - `width`: long literal for the Width style name
 - `wgt`: short literal for the Weight style name
 - `weight`: long literal for the Weight style name
 - `slp`: short literal for the Slope style name
```

### Comparing `font-CLI-0.9.6/font_CLI.egg-info/PKG-INFO` & `font-CLI-0.9.7/font_CLI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: font-CLI
-Version: 0.9.6
+Version: 0.9.7
 Summary: A set of command line tools to edit fonts with FontTools
 Home-page: https://github.com/ftCLI/ftCLI
 Author: ftCLI
 Author-email: ftcli@proton.me
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7, <3.11
@@ -261,20 +261,20 @@
 retrieved values and the JSON data, trying to determine the proper style names. The results are written into the
 `fonts_data.csv` file.
 
 The `fonts_data.csv` contains the following columns:
 
 - `file_name`: path to the font file
 - `family_name`: the font's family name, retrieved reading the name table
-- `is_bold`: True if ths bold bits are set, False if they are not set. This column is present only for completeness,
+- `is_bold`: True if the bold bits are set, False if they are not set. This column is present only for completeness,
   but it's value will be ignored. A font will be set as bold only and only if, while running the `ftcli assistant commit`
   command, the user will choose to use linked styles.
   (-ls / --linked styles) option while writing data from CSV to fonts
-- `is_italic`: True if ths italic bits are set, False if they are not set
-- `is_oblique`: True if ths oblique bit is set, False if it's not set
+- `is_italic`: True if the italic bits are set, False if they are not set
+- `is_oblique`: True if the oblique bit is set, False if it's not set
 - `us_width_class`: usWidthClass value
 - `us_weight_class`: usWeightClass value
 - `wdt`: short literal for the Width style name
 - `width`: long literal for the Width style name
 - `wgt`: short literal for the Weight style name
 - `weight`: long literal for the Weight style name
 - `slp`: short literal for the Slope style name
```

### Comparing `font-CLI-0.9.6/font_CLI.egg-info/SOURCES.txt` & `font-CLI-0.9.7/font_CLI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.6/ftCLI/Lib/Font.py` & `font-CLI-0.9.7/ftCLI/Lib/Font.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.6/ftCLI/Lib/VFont.py` & `font-CLI-0.9.7/ftCLI/Lib/VFont.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.6/ftCLI/Lib/assistant/fonts_data.py` & `font-CLI-0.9.7/ftCLI/Lib/assistant/fonts_data.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.6/ftCLI/Lib/assistant/styles_mapping.py` & `font-CLI-0.9.7/ftCLI/Lib/assistant/styles_mapping.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.6/ftCLI/Lib/constants.py` & `font-CLI-0.9.7/ftCLI/Lib/constants.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.6/ftCLI/Lib/converter/otf_to_ttf.py` & `font-CLI-0.9.7/ftCLI/Lib/converter/otf_to_ttf.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 def update_hmtx(ttFont, glyf):
     hmtx = ttFont["hmtx"]
     for glyphName, glyph in glyf.glyphs.items():
         if hasattr(glyph, "xMin"):
             hmtx[glyphName] = (hmtx[glyphName][0], glyph.xMin)
 
 
-def otf_to_ttf(ttFont: Font, post_format=POST_FORMAT, **kwargs):
+def convert_font(ttFont: Font, post_format=POST_FORMAT, **kwargs):
     if ttFont.sfntVersion != "OTTO":
         raise TTLibError("Not a OpenType font (bad sfntVersion)")
     assert "CFF " in ttFont
 
     glyphOrder = ttFont.getGlyphOrder()
 
     ttFont["loca"] = newTable("loca")
@@ -80,9 +80,9 @@
         log.warning("Dropping glyph names, they do not fit in 'post' table.")
 
     ttFont.sfntVersion = "\000\001\000\000"
 
 
 def run(input_file, output_file, recalc_timestamp=False):
     font = Font(input_file, recalcTimestamp=recalc_timestamp)
-    otf_to_ttf(font, post_format=2.0, max_err=1.0, reverse_direction=True)
+    convert_font(font, post_format=2.0, max_err=1.0, reverse_direction=True)
     font.save(output_file)
```

### Comparing `font-CLI-0.9.6/ftCLI/Lib/converter/ttf_to_otf.py` & `font-CLI-0.9.7/ftCLI/Lib/converter/ttf_to_otf.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from fontTools.subset import Subsetter
 
 from ftCLI.Lib.Font import Font
 from ftCLI.Lib.utils.click_tools import generic_error_message, generic_warning_message
 
 
 class TrueTypeToCFF(object):
-    def __init__(self, font: Font, output_file: str):
+    def __init__(self, font: Font, output_file):
         self.font = font
         self.output_file = output_file
 
     def run(
         self,
         charstrings_source="qu2cu",
         tolerance=1,
@@ -25,19 +25,19 @@
             self.purge_glyphs()
 
         charstrings = {}
 
         if charstrings_source == "qu2cu":
             self.font.decomponentize()
             try:
-                charstrings = self.get_qu2u_charstrings(tolerance=tolerance, all_cubic=True)
+                charstrings = self.get_qu2cu_charstrings(tolerance=tolerance, all_cubic=True)
             except NotImplementedError:
                 generic_warning_message("all_cubic set to False")
                 try:
-                    charstrings = self.get_qu2u_charstrings(tolerance=tolerance, all_cubic=False)
+                    charstrings = self.get_qu2cu_charstrings(tolerance=tolerance, all_cubic=False)
                 except Exception as e:
                     generic_error_message(f"Failed to get charstring with Qu2CuPen ({e})")
                     return
 
         if charstrings_source == "t2":
             try:
                 charstrings = self.get_t2_charstrings()
@@ -127,15 +127,15 @@
             subsetter.options.name_legacy = True
             subsetter.options.name_languages = "*"
             subsetter.options.layout_features = "*"
             subsetter.options.hinting = False
             subsetter.glyph_ids_requested = glyph_ids
             Subsetter.subset(subsetter, self.font)
 
-    def get_qu2u_charstrings(self, tolerance: float = 1, all_cubic: bool = True):
+    def get_qu2cu_charstrings(self, tolerance: float = 1, all_cubic: bool = True):
         charstrings = {}
         glyph_set = self.font.getGlyphSet()
 
         for k, v in glyph_set.items():
             # Correct contours direction and remove overlaps with pathops
             pathops_path = pathops.Path()
             pathops_pen = pathops_path.getPen(glyphSet=glyph_set)
```

### Comparing `font-CLI-0.9.6/ftCLI/Lib/cui/CUI.py` & `font-CLI-0.9.7/ftCLI/Lib/cui/CUI.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.6/ftCLI/Lib/tables/OS_2.py` & `font-CLI-0.9.7/ftCLI/Lib/tables/OS_2.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.6/ftCLI/Lib/tables/head.py` & `font-CLI-0.9.7/ftCLI/Lib/tables/head.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.6/ftCLI/Lib/tables/hhea.py` & `font-CLI-0.9.7/ftCLI/Lib/tables/hhea.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.6/ftCLI/Lib/tables/name.py` & `font-CLI-0.9.7/ftCLI/Lib/tables/name.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.6/ftCLI/Lib/utils/cli_tools.py` & `font-CLI-0.9.7/ftCLI/Lib/utils/cli_tools.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.6/ftCLI/Lib/utils/click_tools.py` & `font-CLI-0.9.7/ftCLI/Lib/utils/click_tools.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.6/ftCLI/Lib/utils/glyphs.py` & `font-CLI-0.9.7/ftCLI/Lib/utils/glyphs.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.6/ftCLI/Lib/utils/misc.py` & `font-CLI-0.9.7/ftCLI/Lib/utils/misc.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.6/ftCLI/commands/ftcli_assistant.py` & `font-CLI-0.9.7/ftCLI/commands/ftcli_assistant.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.6/ftCLI/commands/ftcli_cff.py` & `font-CLI-0.9.7/ftCLI/commands/ftcli_cff.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.6/ftCLI/commands/ftcli_converter.py` & `font-CLI-0.9.7/ftCLI/commands/ftcli_converter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import time
+from io import BytesIO
 
 import click
 import fontTools.ttLib
 from afdko import checkoutlinesufo
 from fontTools.misc.cliTools import makeOutputFileName
 from fontTools.ttLib import TTCollection
 from fontTools.ttLib.tables._f_v_a_r import NamedInstance
@@ -117,34 +118,31 @@
             suffix = "" if source_font.flavor is None else ".otf"
             output_file = makeOutputFileName(
                 file, suffix=suffix, extension=ext, outputDir=output_dir, overWrite=overWrite
             )
 
             if safe:
                 # Create a temporary OTF file with T2CharStringPen...
-                temp_otf_file = makeOutputFileName(output_file, suffix="_tmp", overWrite=True)
-                ttf2otf_converter_temp = TrueTypeToCFF(source_font, output_file=temp_otf_file)
+                buf = BytesIO()
+                ttf2otf_converter_temp = TrueTypeToCFF(source_font, output_file=buf)
                 ttf2otf_converter_temp.run(charstrings_source="t2", purge_glyphs=purge_glyphs, subroutinize=False)
 
                 # ... and convert it back to a temporary TTF file that will be used for conversion
-                temp_ttf_file = makeOutputFileName(temp_otf_file, extension=".ttf", overWrite=True)
-                otf_to_ttf.run(input_file=temp_otf_file, output_file=temp_ttf_file, recalc_timestamp=recalcTimestamp)
-                os.remove(temp_otf_file)
-                input_font = Font(temp_ttf_file, recalcTimestamp=recalcTimestamp)
+                data = buf.getvalue()
+                temp_otf = Font(BytesIO(data), recalcTimestamp=recalcTimestamp)
+                otf_to_ttf.convert_font(temp_otf, post_format=2.0, max_err=1.0, reverse_direction=True)
+                input_font = Font(BytesIO(buf.getvalue()), recalcTimestamp=recalcTimestamp)
             else:
                 input_font = source_font
 
             ttf2otf_converter = TrueTypeToCFF(font=input_font, output_file=output_file)
             ttf2otf_converter.run(
                 charstrings_source="qu2cu", tolerance=tolerance, subroutinize=subroutinize, purge_glyphs=purge_glyphs
             )
 
-            if safe:
-                os.remove(input_font.file)
-
             if check_outlines:
                 generic_info_message("Checking outlines...")
                 checkoutlinesufo.run(args=[output_file, "--error-correction-mode", "--quiet-mode"])
 
             converted_files_counter += 1
             generic_info_message(f"Done in {round(time.time() - t, 3)} seconds")
             file_saved_message(ttf2otf_converter.output_file)
@@ -245,17 +243,24 @@
         try:
             web_font = Font(file, recalcTimestamp=recalcTimestamp)
             if web_font.flavor is None:
                 continue
             if flavor is not None:
                 if web_font.flavor != flavor:
                     continue
+            old_extension=web_font.get_real_extension()
             web_font.flavor = None
-            extension = web_font.get_real_extension()
-            desktop_font_file = makeOutputFileName(file, extension=extension, outputDir=output_dir, overWrite=overWrite)
+            new_extension = web_font.get_real_extension()
+            desktop_font_file = makeOutputFileName(
+                file,
+                extension=new_extension,
+                suffix=old_extension,
+                outputDir=output_dir,
+                overWrite=overWrite
+            )
             web_font.save(desktop_font_file, reorderTables=False)
             if delete_source_file:
                 os.remove(file)
             file_saved_message(desktop_font_file)
         except Exception as e:
             generic_error_message(e)
```

### Comparing `font-CLI-0.9.6/ftCLI/commands/ftcli_fix.py` & `font-CLI-0.9.7/ftCLI/commands/ftcli_fix.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.6/ftCLI/commands/ftcli_hhea.py` & `font-CLI-0.9.7/ftCLI/commands/ftcli_hhea.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.6/ftCLI/commands/ftcli_metrics.py` & `font-CLI-0.9.7/ftCLI/commands/ftcli_metrics.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.6/ftCLI/commands/ftcli_name.py` & `font-CLI-0.9.7/ftCLI/commands/ftcli_name.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.6/ftCLI/commands/ftcli_os2.py` & `font-CLI-0.9.7/ftCLI/commands/ftcli_os2.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.6/ftCLI/commands/ftcli_post.py` & `font-CLI-0.9.7/ftCLI/commands/ftcli_post.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.6/ftCLI/commands/ftcli_print.py` & `font-CLI-0.9.7/ftCLI/commands/ftcli_print.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.6/ftCLI/commands/ftcli_utils.py` & `font-CLI-0.9.7/ftCLI/commands/ftcli_utils.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.6/ftCLI/ftCLI.py` & `font-CLI-0.9.7/ftCLI/ftCLI.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,19 +10,19 @@
         rv = []
         for filename in os.listdir(plugin_folder):
             if filename.endswith(".py") and filename.startswith("ftcli_"):
                 rv.append(filename[6:-3])
         rv.sort()
         return rv
 
-    def get_command(self, ctx, name):
+    def get_command(self, ctx, cmd_name):
         try:
-            mod = __import__(f"ftCLI.commands.ftcli_{name}", None, None, ["cli"])
+            mod = __import__(f"ftCLI.commands.ftcli_{cmd_name}", None, None, ["cli"])
         except ImportError as e:
-            print(e)
+            click.secho(f"ERROR: {click.style(e, fg='red')}")
             return
 
         return mod.cli
 
 
 cli = FtCLI(help="A command line font editor.")
```

### Comparing `font-CLI-0.9.6/setup.py` & `font-CLI-0.9.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="font-CLI",
-    version="0.9.6",
+    version="0.9.7",
     description="A set of command line tools to edit fonts with FontTools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ftCLI",
     author_email="ftcli@proton.me",
     url="https://github.com/ftCLI/ftCLI",
     packages=setuptools.find_packages(),
```

