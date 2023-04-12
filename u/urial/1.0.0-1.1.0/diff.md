# Comparing `tmp/urial-1.0.0.tar.gz` & `tmp/urial-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urial-1.0.0.tar", last modified: Mon Dec 27 23:14:07 2021, max compression
+gzip compressed data, was "urial-1.1.0.tar", last modified: Wed Apr 12 20:07:22 2023, max compression
```

## Comparing `urial-1.0.0.tar` & `urial-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 mhucka     (511) staff       (20)        0 2021-12-27 23:14:07.856906 urial-1.0.0/
--rw-r--r--   0 mhucka     (511) staff       (20)     1340 2021-12-05 19:39:00.000000 urial-1.0.0/LICENSE
--rw-r--r--   0 mhucka     (511) staff       (20)    17899 2021-12-27 23:14:07.857039 urial-1.0.0/PKG-INFO
--rw-r--r--   0 mhucka     (511) staff       (20)    17159 2021-12-27 23:13:07.000000 urial-1.0.0/README.md
--rw-r--r--   0 mhucka     (511) staff       (20)      885 2021-12-27 23:14:07.857514 urial-1.0.0/setup.cfg
--rw-r--r--   0 mhucka     (511) staff       (20)      809 2021-12-07 18:06:55.000000 urial-1.0.0/setup.py
-drwxr-xr-x   0 mhucka     (511) staff       (20)        0 2021-12-27 23:14:07.854684 urial-1.0.0/urial/
--rw-r--r--   0 mhucka     (511) staff       (20)     1657 2021-12-27 23:00:58.000000 urial-1.0.0/urial/__init__.py
--rw-r--r--   0 mhucka     (511) staff       (20)    15263 2021-12-27 21:34:42.000000 urial-1.0.0/urial/__main__.py
-drwxr-xr-x   0 mhucka     (511) staff       (20)        0 2021-12-27 23:14:07.856676 urial-1.0.0/urial.egg-info/
--rw-r--r--   0 mhucka     (511) staff       (20)    17899 2021-12-27 23:14:07.000000 urial-1.0.0/urial.egg-info/PKG-INFO
--rw-r--r--   0 mhucka     (511) staff       (20)      276 2021-12-27 23:14:07.000000 urial-1.0.0/urial.egg-info/SOURCES.txt
--rw-r--r--   0 mhucka     (511) staff       (20)        1 2021-12-27 23:14:07.000000 urial-1.0.0/urial.egg-info/dependency_links.txt
--rw-r--r--   0 mhucka     (511) staff       (20)       63 2021-12-27 23:14:07.000000 urial-1.0.0/urial.egg-info/entry_points.txt
--rw-r--r--   0 mhucka     (511) staff       (20)        1 2021-12-07 19:39:35.000000 urial-1.0.0/urial.egg-info/not-zip-safe
--rw-r--r--   0 mhucka     (511) staff       (20)       81 2021-12-27 23:14:07.000000 urial-1.0.0/urial.egg-info/requires.txt
--rw-r--r--   0 mhucka     (511) staff       (20)        6 2021-12-27 23:14:07.000000 urial-1.0.0/urial.egg-info/top_level.txt
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-12 20:07:22.161796 urial-1.1.0/
+-rw-r--r--   0 mhucka     (503) staff       (20)     1345 2023-04-09 18:04:57.000000 urial-1.1.0/LICENSE
+-rw-r--r--   0 mhucka     (503) staff       (20)    17888 2023-04-12 20:07:22.161866 urial-1.1.0/PKG-INFO
+-rw-r--r--   0 mhucka     (503) staff       (20)    17168 2023-04-12 20:03:35.000000 urial-1.1.0/README.md
+-rw-r--r--   0 mhucka     (503) staff       (20)      885 2023-04-12 20:07:22.162174 urial-1.1.0/setup.cfg
+-rw-r--r--   0 mhucka     (503) staff       (20)      809 2021-12-07 18:06:55.000000 urial-1.1.0/setup.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-12 20:07:22.160557 urial-1.1.0/tests/
+-rw-r--r--   0 mhucka     (503) staff       (20)     3786 2021-12-27 20:08:41.000000 urial-1.1.0/tests/test_uri_parsing.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-12 20:07:22.160824 urial-1.1.0/urial/
+-rw-r--r--   0 mhucka     (503) staff       (20)     1657 2023-04-12 19:57:51.000000 urial-1.1.0/urial/__init__.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    15752 2022-01-03 17:48:11.000000 urial-1.1.0/urial/__main__.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-12 20:07:22.161704 urial-1.1.0/urial.egg-info/
+-rw-r--r--   0 mhucka     (503) staff       (20)    17888 2023-04-12 20:07:22.000000 urial-1.1.0/urial.egg-info/PKG-INFO
+-rw-r--r--   0 mhucka     (503) staff       (20)      302 2023-04-12 20:07:22.000000 urial-1.1.0/urial.egg-info/SOURCES.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-04-12 20:07:22.000000 urial-1.1.0/urial.egg-info/dependency_links.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)       62 2023-04-12 20:07:22.000000 urial-1.1.0/urial.egg-info/entry_points.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        1 2021-12-07 19:39:35.000000 urial-1.1.0/urial.egg-info/not-zip-safe
+-rw-r--r--   0 mhucka     (503) staff       (20)       81 2023-04-12 20:07:22.000000 urial-1.1.0/urial.egg-info/requires.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        6 2023-04-12 20:07:22.000000 urial-1.1.0/urial.egg-info/top_level.txt
```

### Comparing `urial-1.0.0/LICENSE` & `urial-1.1.0/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2021 by Michael Hucka and the California Institute of
+Copyright (c) 2021-2023 by Michael Hucka and the California Institute of
 Technology (Pasadena, California, USA).
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
```

### Comparing `urial-1.0.0/PKG-INFO` & `urial-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: urial
-Version: 1.0.0
+Version: 1.1.0
 Summary: URI Addition tooL: add/update a URI in a macOS Finder comment
 Home-page: https://github.com/mhucka/urial
 Author: Michael Hucka
 Author-email: mhucka@caltech.edu
 License: BSD 3-clause
 Project-URL: Source Code, https://github.com/mhucka/urial
 Project-URL: Bug Tracker, https://github.com/mhucka/urial/issues
 Keywords: Python,utilities
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -21,15 +20,14 @@
 
 # Urial<img width="12%" align="right" src="https://github.com/mhucka/urial/raw/main/.graphics/urial-icon.png">
 
 Urial (_**URI** **a**ddition too**l**_) is a simple but intelligent command-line tool to add, view, or replace URIs in macOS Finder comments.
 
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg?style=flat-square)](https://choosealicense.com/licenses/bsd-3-clause)
 [![Python](https://img.shields.io/badge/Python-3.6+-brightgreen.svg?style=flat-square)](http://shields.io)
-[![DOI](https://img.shields.io/badge/dynamic/json.svg?label=DOI&style=flat-square&colorA=gray&colorB=navy&query=$.metadata.doi&uri=https://data.caltech.edu/api/record/8764)](https://data.caltech.edu/records/8764)
 [![Latest release](https://img.shields.io/github/v/release/mhucka/urial.svg?style=flat-square&color=b44e88)](https://github.com/mhucka/urial/releases)
 [![PyPI](https://img.shields.io/pypi/v/urial.svg?style=flat-square&color=orange&label=PyPI)](https://pypi.org/project/urial/)
 
 
 ## Table of contents
 
 * [Introduction](#introduction)
@@ -170,21 +168,22 @@
 
 These strict interpretations are usually unhelpful in Urial's domain of application. For this reason, `urial` tries to be intelligent about recognizing URIs in Finder comments by applying the following rules:
 
 1) it will assume that the following characters are not part of a URI if they come at the end of something that otherwise looks like a URI: `.` `,` `:` `;` `'` `?` `!` `$` `(` `[`
 2) it will assume that `)` and `]` characters at the end of something that looks like a URI are not part of the URI if there is no opening `(` or `[` character in the rest of the URI
 3) it will ignore strings that could be URIs with empty path components (e.g., `something:`, `abc-def:`, etc.)
 
-To disable this behavior, use the <nobr><code>--strict</code></nobr> option; then, the program will assume that URIs are separated from text only by (1) whitespace characters and (2) the characters `<` `>` `^` `"` <code>&#96;</code> `{` and `}`, and it will not ignore potential URIs with empty paths.
+To disable this behavior, use the <code>--strict</code> option; then, the program will assume that URIs are separated from text only by (1) whitespace characters and (2) the characters `<` `>` `^` `"` <code>&#96;</code> `{` and `}`, and it will not ignore potential URIs with empty paths.
 
 ### Options for handling existing Finder comments
 
 The `--mode` option can be used to change the behavior described above. The following are the possible values for this option:
 
 * `append`: in this mode, if the URI is _not_ found in the Finder comment string, `urial` will append the given URI to the end of the comment; otherwise (if the comment string already contains the URI) it will do nothing.
+* `prepend`: in this mode, if the URI is _not_ found in the Finder comment string, `urial` will prepend the given URI to the front of the comment; otherwise (if the comment string already contains the URI) it will do nothing.
 * `overwrite`: the program will overwrite the Finder comment completely with the given URI string, no matter what the Finder comment string contains (even if it already contains the given URI).
 * `update`: (default) if a URI of the same kind exists in the comment, `urial` will replace only the URI portion of the comment string (preserving the rest of the comment string), else (if a URI is NOT found in the comment string) it will do nothing.
 
 Note carefully that `--mode overwrite` makes `urial` replace unconditionally the entire Finder comment.  In other words, `--mode overwrite` will change a Finder comment such as
 
     Blah blah blah. URI. More blah blah blah.
 
@@ -218,22 +217,22 @@
 ### _Summary of command-line options_
 
 The following table summarizes all the command line options available.
 
 | Short&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;   | Long&nbsp;form&nbsp;opt&nbsp;&nbsp; | Meaning | Default |  |
 |---------- |-------------------|--------------------------------------|---------|---|
 | `-h`      | `--help`          | Display help text and exit | | |
-| `-m`      | `--mode`_M_       | Approach for handling existing comments | `update` | ⚑ |
-| `-p`      | `--print`_P_      | Print file's Finder comment or URIs found therein, and exit  | | ★ |
+| `-m`      | `--mode` _M_      | Approach for handling existing comments | `update` | ⚑ |
+| `-p`      | `--print` _P_     | Print Finder comment or URIs therein, and exit  | | ★ |
 | `-s`      | `--strict`        | Be strict about URI syntax | Don't be pedantic | |
 | `-U`      | `--no-gui`        | Print errors & warnings to terminal | Use GUI dialogs | |
 | `-V`      | `--version`       | Display program version info, and exit | | |
-| `-@`_OUT_ | `--debug`_OUT_    | Debugging mode; write trace to _OUT_ | Normal mode | ⬥ |
+| `-@`_OUT_ | `--debug` _OUT_   | Debugging mode; write trace to _OUT_ | Normal mode | ⬥ |
 
-⚑ &nbsp; Available values are `append`, `overwrite`, and `update`.<br>
+⚑ &nbsp; Available values are `append`, `prepend`, `overwrite`, and `update`.<br>
 ★ &nbsp; Available values are `comment` and `uri`.<br>
 ⬥ &nbsp; To write to the console, use the character `-` as the value of _OUT_; otherwise, _OUT_ must be the name of a file where the output should be written.<br>
 
 
 ## Getting help
 
 Some notes about how the author uses this program can be found in the [wiki](https://github.com/mhucka/urial/wiki).
@@ -244,15 +243,15 @@
 ## Contributing
 
 I would be happy to receive your help and participation if you are interested.  Everyone is asked to read and respect the [code of conduct](CONDUCT.md) when participating in this project.
 
 
 ## License
 
-This software is Copyright (C) 2021, by Michael Hucka and the California Institute of Technology (Pasadena, California, USA).  This software is freely distributed under a 3-clause BSD type license.  Please see the [LICENSE](LICENSE) file for more information.
+This software is Copyright (C) 2021&ndash;2023, by Michael Hucka and the California Institute of Technology (Pasadena, California, USA).  This software is freely distributed under a 3-clause BSD type license.  Please see the [LICENSE](LICENSE) file for more information.
 
 
 ## Acknowledgments
 
 This work is a personal project developed by the author, using computing facilities and other resources of the [California Institute of Technology Library](https://www.library.caltech.edu).
 
 The [vector artwork](https://thenounproject.com/icon/bighorn-sheep-head-2608122/) of a sheep with horns, used as the icon for Urial, was created by  [Vectors Point](https://thenounproject.com/vectorspoint/) from the Noun Project.  It is licensed under the Creative Commons [CC-BY 3.0](https://creativecommons.org/licenses/by/3.0/) license.
@@ -261,9 +260,7 @@
 
 * [appscript](http://appscript.sourceforge.net/py-appscript/doc.html) &ndash; high-level Apple event bridge for controlling scriptable Mac OS X applications
 * [plac](http://micheles.github.io/plac/) &ndash; a command line argument parser
 * [setuptools](https://github.com/pypa/setuptools) &ndash; library for `setup.py`
 * [Sidetrack](https://github.com/caltechlibrary/sidetrack) &ndash; simple debug logging/tracing package
 * [uritools](https://github.com/tkem/uritools/) &ndash; functions for parsing, classifying, and composing URIs
 * [wheel](https://pypi.org/project/wheel/) &ndash; setuptools extension for building wheels
-
-
```

### Comparing `urial-1.0.0/README.md` & `urial-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Urial<img width="12%" align="right" src="https://github.com/mhucka/urial/raw/main/.graphics/urial-icon.png">
 
 Urial (_**URI** **a**ddition too**l**_) is a simple but intelligent command-line tool to add, view, or replace URIs in macOS Finder comments.
 
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg?style=flat-square)](https://choosealicense.com/licenses/bsd-3-clause)
 [![Python](https://img.shields.io/badge/Python-3.6+-brightgreen.svg?style=flat-square)](http://shields.io)
-[![DOI](https://img.shields.io/badge/dynamic/json.svg?label=DOI&style=flat-square&colorA=gray&colorB=navy&query=$.metadata.doi&uri=https://data.caltech.edu/api/record/8764)](https://data.caltech.edu/records/8764)
 [![Latest release](https://img.shields.io/github/v/release/mhucka/urial.svg?style=flat-square&color=b44e88)](https://github.com/mhucka/urial/releases)
 [![PyPI](https://img.shields.io/pypi/v/urial.svg?style=flat-square&color=orange&label=PyPI)](https://pypi.org/project/urial/)
 
 
 ## Table of contents
 
 * [Introduction](#introduction)
@@ -149,21 +148,22 @@
 
 These strict interpretations are usually unhelpful in Urial's domain of application. For this reason, `urial` tries to be intelligent about recognizing URIs in Finder comments by applying the following rules:
 
 1) it will assume that the following characters are not part of a URI if they come at the end of something that otherwise looks like a URI: `.` `,` `:` `;` `'` `?` `!` `$` `(` `[`
 2) it will assume that `)` and `]` characters at the end of something that looks like a URI are not part of the URI if there is no opening `(` or `[` character in the rest of the URI
 3) it will ignore strings that could be URIs with empty path components (e.g., `something:`, `abc-def:`, etc.)
 
-To disable this behavior, use the <nobr><code>--strict</code></nobr> option; then, the program will assume that URIs are separated from text only by (1) whitespace characters and (2) the characters `<` `>` `^` `"` <code>&#96;</code> `{` and `}`, and it will not ignore potential URIs with empty paths.
+To disable this behavior, use the <code>--strict</code> option; then, the program will assume that URIs are separated from text only by (1) whitespace characters and (2) the characters `<` `>` `^` `"` <code>&#96;</code> `{` and `}`, and it will not ignore potential URIs with empty paths.
 
 ### Options for handling existing Finder comments
 
 The `--mode` option can be used to change the behavior described above. The following are the possible values for this option:
 
 * `append`: in this mode, if the URI is _not_ found in the Finder comment string, `urial` will append the given URI to the end of the comment; otherwise (if the comment string already contains the URI) it will do nothing.
+* `prepend`: in this mode, if the URI is _not_ found in the Finder comment string, `urial` will prepend the given URI to the front of the comment; otherwise (if the comment string already contains the URI) it will do nothing.
 * `overwrite`: the program will overwrite the Finder comment completely with the given URI string, no matter what the Finder comment string contains (even if it already contains the given URI).
 * `update`: (default) if a URI of the same kind exists in the comment, `urial` will replace only the URI portion of the comment string (preserving the rest of the comment string), else (if a URI is NOT found in the comment string) it will do nothing.
 
 Note carefully that `--mode overwrite` makes `urial` replace unconditionally the entire Finder comment.  In other words, `--mode overwrite` will change a Finder comment such as
 
     Blah blah blah. URI. More blah blah blah.
 
@@ -197,22 +197,22 @@
 ### _Summary of command-line options_
 
 The following table summarizes all the command line options available.
 
 | Short&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;   | Long&nbsp;form&nbsp;opt&nbsp;&nbsp; | Meaning | Default |  |
 |---------- |-------------------|--------------------------------------|---------|---|
 | `-h`      | `--help`          | Display help text and exit | | |
-| `-m`      | `--mode`_M_       | Approach for handling existing comments | `update` | ⚑ |
-| `-p`      | `--print`_P_      | Print file's Finder comment or URIs found therein, and exit  | | ★ |
+| `-m`      | `--mode` _M_      | Approach for handling existing comments | `update` | ⚑ |
+| `-p`      | `--print` _P_     | Print Finder comment or URIs therein, and exit  | | ★ |
 | `-s`      | `--strict`        | Be strict about URI syntax | Don't be pedantic | |
 | `-U`      | `--no-gui`        | Print errors & warnings to terminal | Use GUI dialogs | |
 | `-V`      | `--version`       | Display program version info, and exit | | |
-| `-@`_OUT_ | `--debug`_OUT_    | Debugging mode; write trace to _OUT_ | Normal mode | ⬥ |
+| `-@`_OUT_ | `--debug` _OUT_   | Debugging mode; write trace to _OUT_ | Normal mode | ⬥ |
 
-⚑ &nbsp; Available values are `append`, `overwrite`, and `update`.<br>
+⚑ &nbsp; Available values are `append`, `prepend`, `overwrite`, and `update`.<br>
 ★ &nbsp; Available values are `comment` and `uri`.<br>
 ⬥ &nbsp; To write to the console, use the character `-` as the value of _OUT_; otherwise, _OUT_ must be the name of a file where the output should be written.<br>
 
 
 ## Getting help
 
 Some notes about how the author uses this program can be found in the [wiki](https://github.com/mhucka/urial/wiki).
@@ -223,15 +223,15 @@
 ## Contributing
 
 I would be happy to receive your help and participation if you are interested.  Everyone is asked to read and respect the [code of conduct](CONDUCT.md) when participating in this project.
 
 
 ## License
 
-This software is Copyright (C) 2021, by Michael Hucka and the California Institute of Technology (Pasadena, California, USA).  This software is freely distributed under a 3-clause BSD type license.  Please see the [LICENSE](LICENSE) file for more information.
+This software is Copyright (C) 2021&ndash;2023, by Michael Hucka and the California Institute of Technology (Pasadena, California, USA).  This software is freely distributed under a 3-clause BSD type license.  Please see the [LICENSE](LICENSE) file for more information.
 
 
 ## Acknowledgments
 
 This work is a personal project developed by the author, using computing facilities and other resources of the [California Institute of Technology Library](https://www.library.caltech.edu).
 
 The [vector artwork](https://thenounproject.com/icon/bighorn-sheep-head-2608122/) of a sheep with horns, used as the icon for Urial, was created by  [Vectors Point](https://thenounproject.com/vectorspoint/) from the Noun Project.  It is licensed under the Creative Commons [CC-BY 3.0](https://creativecommons.org/licenses/by/3.0/) license.
```

### Comparing `urial-1.0.0/setup.cfg` & `urial-1.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = urial
-version = 1.0.0
+version = 1.1.0
 description = URI Addition tooL: add/update a URI in a macOS Finder comment
 author = Michael Hucka
 author_email = mhucka@caltech.edu
 license = BSD 3-clause
 license_files = LICENSE
 url = https://github.com/mhucka/urial
 project_urls =
```

### Comparing `urial-1.0.0/setup.py` & `urial-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `urial-1.0.0/urial/__init__.py` & `urial-1.1.0/urial/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 #
 #  ╭────────────────────── Notice ── Notice ── Notice ─────────────────────╮
 #  |    The following values are automatically updated at every release    |
 #  |    by the Makefile. Manual changes to these values will be lost.      |
 #  ╰────────────────────── Notice ── Notice ── Notice ─────────────────────╯
 
 __program__     = 'urial'
-__version__     = '1.0.0'
+__version__     = '1.1.0'
 __description__ = 'URI Addition tooL: add/update a URI in a macOS Finder comment'
 __url__         = 'https://github.com/mhucka/urial'
 __author__      = 'Michael Hucka'
 __email__       = 'mhucka@caltech.edu'
 __license__     = 'BSD 3-clause'
```

### Comparing `urial-1.0.0/urial/__main__.py` & `urial-1.1.0/urial/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,18 @@
 
 The --mode option can be used to change this program's behavior, as follows:
 
   append:    if the URI is NOT found in the Finder comment string, append the
              given URI to the end of the comment; otherwise (if the comment
              string already contains the URI) do nothing
 
+  prepend:   if the URI is NOT found in the Finder comment string, prepend the
+             given URI to the front of the comment; otherwise (if the comment
+             string already contains the URI) do nothing
+
   overwrite: overwrite the Finder comment completely with the given URI string,
              no matter what the Finder comment string contains (even if it
              already contains the given URI)
 
   update:    (default) if a URI of the same kind exists in the comment,
              replace only the URI portion of the comment string (preserving
              the rest of the comment string), else (if a URI is NOT found in
@@ -206,16 +210,16 @@
         set_debug(True, debug)
 
     if version:
         from urial import print_version
         print_version()
         sys.exit(0)
 
-    mode = 'update' if mode == 'M' else mode
-    if mode not in ['update', 'append', 'overwrite']:
+    mode = 'update' if mode == 'M' else mode.lower()
+    if mode not in ['update', 'append', 'prepend', 'overwrite']:
         stop(f'Unrecognized mode value: {mode}')
 
     show = print_.lower() if print_ != 'P' else False
     if show:
         if show not in ['comment', 'uri']:
             stop(f'Invalid option value for --print: {print_}. The valid'
                  + ' options are "comment" and "uri".')
@@ -226,15 +230,15 @@
         uri = args[0]
         file = args[1]
         scheme = urisplit(uri).scheme
         if not scheme:
             stop(f'Could not interpret argument value "' + uri + '" as a URI.')
 
     if file == '':
-        stop(f'File name is an empty string.')
+        stop(f'File name must not be an empty string.')
     from os.path import exists
     if not exists(file):
         stop(f'File does not appear to exist: {file}')
 
     # Do the real work --------------------------------------------------------
 
     import appscript
@@ -258,14 +262,17 @@
             log('overwriting existing Finder comment with ' + uri)
             finder_file.comment.set(uri)
         elif uri in comment:
             log('comment already contains the same URI: ' + uri)
         elif mode == 'append':
             log('appending to existing Finder comment the string ' + uri)
             finder_file.comment.set(comment + '\n' + uri)
+        elif mode == 'prepend':
+            log('prepending to existing Finder comment the string ' + uri)
+            finder_file.comment.set(uri + '\n' + comment)
         else:
             # Check if there's a URI with the same scheme in the comment.
             uris = uris_in_text(comment, strict)
             same_scheme_uris = [u for u in uris if urisplit(u).scheme == scheme]
             if any(same_scheme_uris):
                 log(f'replacing {same_scheme_uris[0]} with {uri}')
                 parts = comment.partition(same_scheme_uris[0])
@@ -279,14 +286,16 @@
         sys.exit(0)
     except Exception as ex:
        from traceback import format_exception
        exception = sys.exc_info()
        details = ''.join(format_exception(*exception))
        stop(f'Encountered error: ' + str(ex) + '\n\n' + details)
 
+    # If we get here, exit normally -------------------------------------------
+
     log('done.')
     sys.exit(0)
 
 
 # Miscellaneous helpers.
 # .............................................................................
 # The syntax of URIs is defined in https://www.rfc-editor.org/rfc/rfc3986.
```

### Comparing `urial-1.0.0/urial.egg-info/PKG-INFO` & `urial-1.1.0/urial.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: urial
-Version: 1.0.0
+Version: 1.1.0
 Summary: URI Addition tooL: add/update a URI in a macOS Finder comment
 Home-page: https://github.com/mhucka/urial
 Author: Michael Hucka
 Author-email: mhucka@caltech.edu
 License: BSD 3-clause
 Project-URL: Source Code, https://github.com/mhucka/urial
 Project-URL: Bug Tracker, https://github.com/mhucka/urial/issues
 Keywords: Python,utilities
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -21,15 +20,14 @@
 
 # Urial<img width="12%" align="right" src="https://github.com/mhucka/urial/raw/main/.graphics/urial-icon.png">
 
 Urial (_**URI** **a**ddition too**l**_) is a simple but intelligent command-line tool to add, view, or replace URIs in macOS Finder comments.
 
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg?style=flat-square)](https://choosealicense.com/licenses/bsd-3-clause)
 [![Python](https://img.shields.io/badge/Python-3.6+-brightgreen.svg?style=flat-square)](http://shields.io)
-[![DOI](https://img.shields.io/badge/dynamic/json.svg?label=DOI&style=flat-square&colorA=gray&colorB=navy&query=$.metadata.doi&uri=https://data.caltech.edu/api/record/8764)](https://data.caltech.edu/records/8764)
 [![Latest release](https://img.shields.io/github/v/release/mhucka/urial.svg?style=flat-square&color=b44e88)](https://github.com/mhucka/urial/releases)
 [![PyPI](https://img.shields.io/pypi/v/urial.svg?style=flat-square&color=orange&label=PyPI)](https://pypi.org/project/urial/)
 
 
 ## Table of contents
 
 * [Introduction](#introduction)
@@ -170,21 +168,22 @@
 
 These strict interpretations are usually unhelpful in Urial's domain of application. For this reason, `urial` tries to be intelligent about recognizing URIs in Finder comments by applying the following rules:
 
 1) it will assume that the following characters are not part of a URI if they come at the end of something that otherwise looks like a URI: `.` `,` `:` `;` `'` `?` `!` `$` `(` `[`
 2) it will assume that `)` and `]` characters at the end of something that looks like a URI are not part of the URI if there is no opening `(` or `[` character in the rest of the URI
 3) it will ignore strings that could be URIs with empty path components (e.g., `something:`, `abc-def:`, etc.)
 
-To disable this behavior, use the <nobr><code>--strict</code></nobr> option; then, the program will assume that URIs are separated from text only by (1) whitespace characters and (2) the characters `<` `>` `^` `"` <code>&#96;</code> `{` and `}`, and it will not ignore potential URIs with empty paths.
+To disable this behavior, use the <code>--strict</code> option; then, the program will assume that URIs are separated from text only by (1) whitespace characters and (2) the characters `<` `>` `^` `"` <code>&#96;</code> `{` and `}`, and it will not ignore potential URIs with empty paths.
 
 ### Options for handling existing Finder comments
 
 The `--mode` option can be used to change the behavior described above. The following are the possible values for this option:
 
 * `append`: in this mode, if the URI is _not_ found in the Finder comment string, `urial` will append the given URI to the end of the comment; otherwise (if the comment string already contains the URI) it will do nothing.
+* `prepend`: in this mode, if the URI is _not_ found in the Finder comment string, `urial` will prepend the given URI to the front of the comment; otherwise (if the comment string already contains the URI) it will do nothing.
 * `overwrite`: the program will overwrite the Finder comment completely with the given URI string, no matter what the Finder comment string contains (even if it already contains the given URI).
 * `update`: (default) if a URI of the same kind exists in the comment, `urial` will replace only the URI portion of the comment string (preserving the rest of the comment string), else (if a URI is NOT found in the comment string) it will do nothing.
 
 Note carefully that `--mode overwrite` makes `urial` replace unconditionally the entire Finder comment.  In other words, `--mode overwrite` will change a Finder comment such as
 
     Blah blah blah. URI. More blah blah blah.
 
@@ -218,22 +217,22 @@
 ### _Summary of command-line options_
 
 The following table summarizes all the command line options available.
 
 | Short&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;   | Long&nbsp;form&nbsp;opt&nbsp;&nbsp; | Meaning | Default |  |
 |---------- |-------------------|--------------------------------------|---------|---|
 | `-h`      | `--help`          | Display help text and exit | | |
-| `-m`      | `--mode`_M_       | Approach for handling existing comments | `update` | ⚑ |
-| `-p`      | `--print`_P_      | Print file's Finder comment or URIs found therein, and exit  | | ★ |
+| `-m`      | `--mode` _M_      | Approach for handling existing comments | `update` | ⚑ |
+| `-p`      | `--print` _P_     | Print Finder comment or URIs therein, and exit  | | ★ |
 | `-s`      | `--strict`        | Be strict about URI syntax | Don't be pedantic | |
 | `-U`      | `--no-gui`        | Print errors & warnings to terminal | Use GUI dialogs | |
 | `-V`      | `--version`       | Display program version info, and exit | | |
-| `-@`_OUT_ | `--debug`_OUT_    | Debugging mode; write trace to _OUT_ | Normal mode | ⬥ |
+| `-@`_OUT_ | `--debug` _OUT_   | Debugging mode; write trace to _OUT_ | Normal mode | ⬥ |
 
-⚑ &nbsp; Available values are `append`, `overwrite`, and `update`.<br>
+⚑ &nbsp; Available values are `append`, `prepend`, `overwrite`, and `update`.<br>
 ★ &nbsp; Available values are `comment` and `uri`.<br>
 ⬥ &nbsp; To write to the console, use the character `-` as the value of _OUT_; otherwise, _OUT_ must be the name of a file where the output should be written.<br>
 
 
 ## Getting help
 
 Some notes about how the author uses this program can be found in the [wiki](https://github.com/mhucka/urial/wiki).
@@ -244,15 +243,15 @@
 ## Contributing
 
 I would be happy to receive your help and participation if you are interested.  Everyone is asked to read and respect the [code of conduct](CONDUCT.md) when participating in this project.
 
 
 ## License
 
-This software is Copyright (C) 2021, by Michael Hucka and the California Institute of Technology (Pasadena, California, USA).  This software is freely distributed under a 3-clause BSD type license.  Please see the [LICENSE](LICENSE) file for more information.
+This software is Copyright (C) 2021&ndash;2023, by Michael Hucka and the California Institute of Technology (Pasadena, California, USA).  This software is freely distributed under a 3-clause BSD type license.  Please see the [LICENSE](LICENSE) file for more information.
 
 
 ## Acknowledgments
 
 This work is a personal project developed by the author, using computing facilities and other resources of the [California Institute of Technology Library](https://www.library.caltech.edu).
 
 The [vector artwork](https://thenounproject.com/icon/bighorn-sheep-head-2608122/) of a sheep with horns, used as the icon for Urial, was created by  [Vectors Point](https://thenounproject.com/vectorspoint/) from the Noun Project.  It is licensed under the Creative Commons [CC-BY 3.0](https://creativecommons.org/licenses/by/3.0/) license.
@@ -261,9 +260,7 @@
 
 * [appscript](http://appscript.sourceforge.net/py-appscript/doc.html) &ndash; high-level Apple event bridge for controlling scriptable Mac OS X applications
 * [plac](http://micheles.github.io/plac/) &ndash; a command line argument parser
 * [setuptools](https://github.com/pypa/setuptools) &ndash; library for `setup.py`
 * [Sidetrack](https://github.com/caltechlibrary/sidetrack) &ndash; simple debug logging/tracing package
 * [uritools](https://github.com/tkem/uritools/) &ndash; functions for parsing, classifying, and composing URIs
 * [wheel](https://pypi.org/project/wheel/) &ndash; setuptools extension for building wheels
-
-
```

