# Comparing `tmp/radian-0.6.4.tar.gz` & `tmp/radian-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radian-0.6.4.tar", last modified: Tue Oct 11 20:00:26 2022, max compression
+gzip compressed data, was "radian-0.6.5.tar", last modified: Wed Apr 12 16:36:27 2023, max compression
```

## Comparing `radian-0.6.4.tar` & `radian-0.6.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 20:00:26.087898 radian-0.6.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1100 2022-10-11 20:00:19.000000 radian-0.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-10-11 20:00:19.000000 radian-0.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    12918 2022-10-11 20:00:26.087898 radian-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10408 2022-10-11 20:00:19.000000 radian-0.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 20:00:26.087898 radian-0.6.4/radian/
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-10-11 20:00:19.000000 radian-0.6.4/radian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      648 2022-10-11 20:00:19.000000 radian-0.6.4/radian/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9850 2022-10-11 20:00:19.000000 radian-0.6.4/radian/app.py
--rw-r--r--   0 runner    (1001) docker     (121)     5655 2022-10-11 20:00:19.000000 radian-0.6.4/radian/completion.py
--rw-r--r--   0 runner    (1001) docker     (121)     6796 2022-10-11 20:00:19.000000 radian-0.6.4/radian/console.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-10-11 20:00:19.000000 radian-0.6.4/radian/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (121)      515 2022-10-11 20:00:19.000000 radian-0.6.4/radian/document.py
--rw-r--r--   0 runner    (1001) docker     (121)     1109 2022-10-11 20:00:19.000000 radian-0.6.4/radian/io.py
--rw-r--r--   0 runner    (1001) docker     (121)    15876 2022-10-11 20:00:19.000000 radian-0.6.4/radian/key_bindings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 20:00:26.087898 radian-0.6.4/radian/latex/
--rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-10-11 20:00:19.000000 radian-0.6.4/radian/latex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    64127 2022-10-11 20:00:19.000000 radian-0.6.4/radian/latex/latex_symbols.py
--rw-r--r--   0 runner    (1001) docker     (121)     7583 2022-10-11 20:00:19.000000 radian-0.6.4/radian/lexer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 20:00:26.087898 radian-0.6.4/radian/lineedit/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 20:00:19.000000 radian-0.6.4/radian/lineedit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10154 2022-10-11 20:00:19.000000 radian-0.6.4/radian/lineedit/buffer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2811 2022-10-11 20:00:19.000000 radian-0.6.4/radian/lineedit/history.py
--rw-r--r--   0 runner    (1001) docker     (121)     7974 2022-10-11 20:00:19.000000 radian-0.6.4/radian/lineedit/prompt.py
--rw-r--r--   0 runner    (1001) docker     (121)     9776 2022-10-11 20:00:19.000000 radian-0.6.4/radian/prompt_session.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 20:00:26.087898 radian-0.6.4/radian/reticulate/
--rw-r--r--   0 runner    (1001) docker     (121)     4005 2022-10-11 20:00:19.000000 radian-0.6.4/radian/reticulate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1508 2022-10-11 20:00:19.000000 radian-0.6.4/radian/reticulate/config.R
--rw-r--r--   0 runner    (1001) docker     (121)     5360 2022-10-11 20:00:19.000000 radian-0.6.4/radian/reticulate/key_bindings.R
--rw-r--r--   0 runner    (1001) docker     (121)     2646 2022-10-11 20:00:19.000000 radian-0.6.4/radian/rutils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2727 2022-10-11 20:00:19.000000 radian-0.6.4/radian/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1666 2022-10-11 20:00:19.000000 radian-0.6.4/radian/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 20:00:26.087898 radian-0.6.4/radian.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12918 2022-10-11 20:00:25.000000 radian-0.6.4/radian.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-10-11 20:00:25.000000 radian-0.6.4/radian.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-11 20:00:25.000000 radian-0.6.4/radian.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-10-11 20:00:25.000000 radian-0.6.4/radian.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-10-11 20:00:25.000000 radian-0.6.4/radian.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-10-11 20:00:25.000000 radian-0.6.4/radian.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-10-11 20:00:26.087898 radian-0.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1516 2022-10-11 20:00:19.000000 radian-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:36:27.630395 radian-0.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-12 16:36:17.000000 radian-0.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-12 16:36:17.000000 radian-0.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-04-12 16:36:27.630395 radian-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10660 2023-04-12 16:36:17.000000 radian-0.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:36:27.630395 radian-0.6.5/radian/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-12 16:36:17.000000 radian-0.6.5/radian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-12 16:36:17.000000 radian-0.6.5/radian/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-04-12 16:36:17.000000 radian-0.6.5/radian/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-04-12 16:36:17.000000 radian-0.6.5/radian/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-04-12 16:36:17.000000 radian-0.6.5/radian/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-12 16:36:17.000000 radian-0.6.5/radian/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-12 16:36:17.000000 radian-0.6.5/radian/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:36:17.000000 radian-0.6.5/radian/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15876 2023-04-12 16:36:17.000000 radian-0.6.5/radian/key_bindings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:36:27.630395 radian-0.6.5/radian/latex/
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-12 16:36:17.000000 radian-0.6.5/radian/latex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64127 2023-04-12 16:36:17.000000 radian-0.6.5/radian/latex/latex_symbols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-04-12 16:36:17.000000 radian-0.6.5/radian/lexer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:36:27.630395 radian-0.6.5/radian/lineedit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:36:17.000000 radian-0.6.5/radian/lineedit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-04-12 16:36:17.000000 radian-0.6.5/radian/lineedit/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-12 16:36:17.000000 radian-0.6.5/radian/lineedit/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-04-12 16:36:17.000000 radian-0.6.5/radian/lineedit/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-04-12 16:36:17.000000 radian-0.6.5/radian/prompt_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:36:27.630395 radian-0.6.5/radian/reticulate/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-12 16:36:17.000000 radian-0.6.5/radian/reticulate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-12 16:36:17.000000 radian-0.6.5/radian/reticulate/config.R
+-rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-04-12 16:36:17.000000 radian-0.6.5/radian/reticulate/key_bindings.R
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-12 16:36:17.000000 radian-0.6.5/radian/rutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-12 16:36:17.000000 radian-0.6.5/radian/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-12 16:36:17.000000 radian-0.6.5/radian/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:36:27.630395 radian-0.6.5/radian.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-04-12 16:36:27.000000 radian-0.6.5/radian.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-12 16:36:27.000000 radian-0.6.5/radian.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:36:27.000000 radian-0.6.5/radian.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-12 16:36:27.000000 radian-0.6.5/radian.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-12 16:36:27.000000 radian-0.6.5/radian.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 16:36:27.000000 radian-0.6.5/radian.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-12 16:36:27.630395 radian-0.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-12 16:36:17.000000 radian-0.6.5/setup.py
```

### Comparing `radian-0.6.4/LICENSE` & `radian-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `radian-0.6.4/PKG-INFO` & `radian-0.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radian
-Version: 0.6.4
+Version: 0.6.5
 Summary: A 21 century R console
 Home-page: https://github.com/randy3k/radian
 Author: Randy Lai
 License: UNKNOWN
 Description: # radian: A 21 century R console
         
         [![Main](https://github.com/randy3k/radian/actions/workflows/main.yml/badge.svg)](https://github.com/randy3k/radian/actions/workflows/main.yml)
@@ -60,14 +60,15 @@
         pip3 install -U git+https://github.com/randy3k/radian
         ```
         
         Alternatively, if you use conda or miniconda,
         ```sh
         conda install -c conda-forge radian
         ```
+        In this case, it is recommended to install R via conda to ensure consistency in C runtime libraries.
         
         ## Alias on unix system
         
         You could alias `r` to _radian_ by putting
         
         ```bash
         alias r="radian"
@@ -169,20 +170,25 @@
         options(radian.enable_reticulate_prompt = TRUE)
         ```
         
         ### Custom key bindings
         
         ```r
         # allows user defined shortcuts, these keys should be escaped when send through the terminal.
-        # In the following example, `esc` + `-` sends `<-` and `esc` + `m` sends `%>%`.
+        # In the following example, `esc` + `-` sends `<-` and `ctrl` + `right` sends `%>%`.
         # Note that in some terminals, you could mark `alt` as `escape` so you could use `alt` + `-` instead.
-        options(radian.escape_key_map = list(
-            list(key = "-", value = " <- "),
-            list(key = "m", value = " %>% ")
-        ))
+        # Also, note that some ctrl mappings are reserved. You cannot remap m, i, h, d, or c
+        options(
+            radian.escape_key_map = list(
+                list(key = "-", value = " <- "),
+            ),
+            radian.ctrl_key_map = list(
+                list(key = "right", value = " %>% ")
+            )
+        )
         ```
         
         ## FAQ
         
         #### Unicode doesn't work in Windows and R 4.2+.
         
         The latest version of R supports Unicode codepage directly. However, radian relies on Python and Python doesn't support Unicode in the way that R supports it. A workaround could be found here: https://github.com/randy3k/radian/issues/269#issuecomment-1169663251
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: radian Version: 0.6.4 Summary: A 21 century R
+Metadata-Version: 2.1 Name: radian Version: 0.6.5 Summary: A 21 century R
 console Home-page: https://github.com/randy3k/radian Author: Randy Lai License:
 UNKNOWN Description: # radian: A 21 century R console [![Main](https://
 github.com/randy3k/radian/actions/workflows/main.yml/badge.svg)](https://
 github.com/randy3k/radian/actions/workflows/main.yml) [![codecov](https://
 codecov.io/gh/randy3k/radian/branch/master/graph/badge.svg)](https://
 codecov.io/gh/randy3k/radian) [![](https://img.shields.io/pypi/v/radian.svg)]
 (https://pypi.org/project/radian/) [![Conda version](https://img.shields.io/
@@ -25,38 +25,39 @@
 3.6 or above) is also required to install _radian_. If your system doesn't come
 with a python distribution, it can be downloaded from https://www.python.org/
 downloads/ or https://conda.io/en/latest/miniconda.html. - `pip` is optional
 but it makes the installation a bit easier. ```sh # install released version
 pip3 install -U radian # to run radian radian ``` ```sh # or the development
 version pip3 install -U git+https://github.com/randy3k/radian ```
 Alternatively, if you use conda or miniconda, ```sh conda install -c conda-
-forge radian ``` ## Alias on unix system You could alias `r` to _radian_ by
-putting ```bash alias r="radian" ``` in `~/.bash_profile` such that `r` would
-open _radian_ and `R` would still open the traditional R console. (`R` is still
-useful, e.g, running `R CMD BUILD`.) ## Settings _radian_ can be customized by
-specifying the below options in various locations - `$XDG_CONFIG_HOME/radian/
-profile` or `$HOME/.config/radian/profile` (Unix) - `%USERPROFILE%/radian/
-profile` (Windows) - `$HOME/.radian_profile` (Unix) -
-`%USERPROFILE%/.radian_profile` (Windows) - `.radian_profile` in the working
-directory The options could be also specified in the `.Rprofile` files,
-however, it is not recommended because 1. the settings are not persistent when
-vanilla mode is used; 2. it doesn't work well with `packrat` or `renv`. ```r #
-Do not copy the whole configuration, just specify what you need! # see https://
-help.farbox.com/pygments.html # for a list of supported color schemes, default
-scheme is "native" options(radian.color_scheme = "native") # either `"emacs"`
-(default) or `"vi"`. options(radian.editing_mode = "emacs") # enable various
-emacs bindings in vi insert mode options
-(radian.emacs_bindings_in_vi_insert_mode = FALSE) # show vi mode state when
-radian.editing_mode is `vi` options(radian.show_vi_mode_prompt = TRUE) options
-(radian.vi_mode_prompt = "\033[0;34m[{}]\033[0m ") # indent continuation lines
-# turn this off if you want to copy code without the extra indentation; # but
-it leads to less elegent layout options(radian.indent_lines = TRUE) # auto
-match brackets and quotes options(radian.auto_match = TRUE) # enable the
-[prompt_toolkit](https://python-prompt-toolkit.readthedocs.io/en/master/
-index.html) [`auto_suggest` feature](https://python-prompt-
+forge radian ``` In this case, it is recommended to install R via conda to
+ensure consistency in C runtime libraries. ## Alias on unix system You could
+alias `r` to _radian_ by putting ```bash alias r="radian" ``` in
+`~/.bash_profile` such that `r` would open _radian_ and `R` would still open
+the traditional R console. (`R` is still useful, e.g, running `R CMD BUILD`.)
+## Settings _radian_ can be customized by specifying the below options in
+various locations - `$XDG_CONFIG_HOME/radian/profile` or `$HOME/.config/radian/
+profile` (Unix) - `%USERPROFILE%/radian/profile` (Windows) -
+`$HOME/.radian_profile` (Unix) - `%USERPROFILE%/.radian_profile` (Windows) -
+`.radian_profile` in the working directory The options could be also specified
+in the `.Rprofile` files, however, it is not recommended because 1. the
+settings are not persistent when vanilla mode is used; 2. it doesn't work well
+with `packrat` or `renv`. ```r # Do not copy the whole configuration, just
+specify what you need! # see https://help.farbox.com/pygments.html # for a list
+of supported color schemes, default scheme is "native" options
+(radian.color_scheme = "native") # either `"emacs"` (default) or `"vi"`.
+options(radian.editing_mode = "emacs") # enable various emacs bindings in vi
+insert mode options(radian.emacs_bindings_in_vi_insert_mode = FALSE) # show vi
+mode state when radian.editing_mode is `vi` options(radian.show_vi_mode_prompt
+= TRUE) options(radian.vi_mode_prompt = "\033[0;34m[{}]\033[0m ") # indent
+continuation lines # turn this off if you want to copy code without the extra
+indentation; # but it leads to less elegent layout options(radian.indent_lines
+= TRUE) # auto match brackets and quotes options(radian.auto_match = TRUE) #
+enable the [prompt_toolkit](https://python-prompt-toolkit.readthedocs.io/en/
+master/index.html) [`auto_suggest` feature](https://python-prompt-
 toolkit.readthedocs.io/en/master/pages/asking_for_input.html#auto-suggestion) #
 this option is experimental and is known to break python prompt, use it with
 caution options(radian.auto_suggest = FALSE) # highlight matching bracket
 options(radian.highlight_matching_bracket = FALSE) # auto indentation for new
 line and curly braces options(radian.auto_indentation = TRUE) options
 (radian.tab_size = 4) # pop up completion while typing options
 (radian.complete_while_typing = TRUE) # the minimum length of prefix to trigger
@@ -81,59 +82,61 @@
 = TRUE) # custom prompt for different modes options(radian.prompt = "\033
 [0;34mr$>\033[0m ") options(radian.shell_prompt = "\033[0;31m#!>\033[0m ")
 options(radian.browse_prompt = "\033[0;33mBrowse[{}]>\033[0m ") # stderr color
 format options(radian.stderr_format = "\033[0;31m{}\033[0m") # enable
 reticulate prompt and trigger `~` options(radian.enable_reticulate_prompt =
 TRUE) ``` ### Custom key bindings ```r # allows user defined shortcuts, these
 keys should be escaped when send through the terminal. # In the following
-example, `esc` + `-` sends `<-` and `esc` + `m` sends `%>%`. # Note that in
-some terminals, you could mark `alt` as `escape` so you could use `alt` + `-
-` instead. options(radian.escape_key_map = list( list(key = "-", value = " <-
-"), list(key = "m", value = " %>% ") )) ``` ## FAQ #### Unicode doesn't work in
-Windows and R 4.2+. The latest version of R supports Unicode codepage directly.
-However, radian relies on Python and Python doesn't support Unicode in the way
-that R supports it. A workaround could be found here: https://github.com/
-randy3k/radian/issues/269#issuecomment-1169663251 #### I can't specify python
-runtime in reticulate. It is expected. `radian` runs on python and the python
-runtime used by radian is forced in reticulate. `reticulate::py_config()` gives
-the note: ``` NOTE: Python version was forced by the current process ``` In
-order to use radian with another python runtime, you will need to install
-`radian` on that python environment. #### How to switch to a different R or
-specify the version of R. There are serveral options. - The easiest option is
-to pass the path to the R binary with `--r-binary`, i.e., `radian --r-binary=/
-path/to/R` - Also, one could expose the path to the R binary in the `PATH`
-variable - The environment variable `R_BINARY` could also be used to specify
-the path to R. - The environment variable `R_HOME` could also be used to
-specify R home directory. Note that it is should be set as the result of
-`R.home()`, not the directory where `R` is located. For example, in Unix ```sh
-$ env R_HOME=/usr/local/lib/R radian ``` #### Cannot find shared library Please
-also make sure that R was installed with the R shared library `libR.so` or
-`libR.dylib` or `libR.dll`. On Linux, the configure flag `./configure --enable-
-R-shlib` may be needed to install R from the source. Do not forget to `make
-clean` to force the recompilation of the files with the correct compiler
-options. #### Outdated setuptools If you encounter > The package setup script
-has attempted to modify files on your system that are not within the
-EasyInstall build area. Please update your setuptools by ``` pip install -
-U setuptools ``` #### How to use local history file _radian_ maintains its own
-history file `.radian_history` and doesn't use the `.Rhistory` file. A local
-`.radian_history` is used if it is found in the launch directory. Otherwise,
-the global history file `~/.radian_history` would be used. To override the
-default behavior, you could launch _radian_ with the options: `radian --local-
-history`, `radian --global-history` or `radian --no-history`. #### Does it slow
-down my R program? _radian_ only provides a frontend to the R program, the
-actual running eventloop is the same as that of the traditional R console.
-There is no performance sacrifice (or gain) while using this modern command
-line interface. #### Nvim-R support Put ```vim let R_app = "radian" let R_cmd =
-"R" let R_hl_term = 0 let R_args = [] " if you had set any let
-R_bracketed_paste = 1 ``` in your vim config. #### `reticulate` Auto
-Completions To enable reticulate prompt completions, make sure that `jedi` is
-installed. ```sh pip install jedi ``` Alternatively, if you use conda, ```sh
-conda install -c conda-forge jedi ``` #### Prompt not shown inside a docker
-container It maybe caused by the invalid terminal size, try running `stty size`
-in your terminal to see if it returns a correct size. You could change the
-values of it from the environmental variables `$COLUMNS` and `$LINES` when you
-log-in the docker container. ``` docker exec -it  bash -c "stty cols $COLUMNS
-rows $LINES && bash" ``` ## Why called _radian_? _radian_ is powered by
-(Ï)thon. ## Credits _radian_ wouldn't be possible without the creative work
-[prompt_toolkit](https://github.com/jonathanslenders/python-prompt-toolkit/) by
-Jonathan Slenders. Platform: UNKNOWN Requires-Python: >=3.6 Description-
-Content-Type: text/markdown Provides-Extra: test
+example, `esc` + `-` sends `<-` and `ctrl` + `right` sends `%>%`. # Note that
+in some terminals, you could mark `alt` as `escape` so you could use `alt` + `-
+` instead. # Also, note that some ctrl mappings are reserved. You cannot remap
+m, i, h, d, or c options( radian.escape_key_map = list( list(key = "-", value =
+" <- "), ), radian.ctrl_key_map = list( list(key = "right", value = " %>% ") )
+) ``` ## FAQ #### Unicode doesn't work in Windows and R 4.2+. The latest
+version of R supports Unicode codepage directly. However, radian relies on
+Python and Python doesn't support Unicode in the way that R supports it. A
+workaround could be found here: https://github.com/randy3k/radian/issues/
+269#issuecomment-1169663251 #### I can't specify python runtime in reticulate.
+It is expected. `radian` runs on python and the python runtime used by radian
+is forced in reticulate. `reticulate::py_config()` gives the note: ``` NOTE:
+Python version was forced by the current process ``` In order to use radian
+with another python runtime, you will need to install `radian` on that python
+environment. #### How to switch to a different R or specify the version of R.
+There are serveral options. - The easiest option is to pass the path to the R
+binary with `--r-binary`, i.e., `radian --r-binary=/path/to/R` - Also, one
+could expose the path to the R binary in the `PATH` variable - The environment
+variable `R_BINARY` could also be used to specify the path to R. - The
+environment variable `R_HOME` could also be used to specify R home directory.
+Note that it is should be set as the result of `R.home()`, not the directory
+where `R` is located. For example, in Unix ```sh $ env R_HOME=/usr/local/lib/
+R radian ``` #### Cannot find shared library Please also make sure that R was
+installed with the R shared library `libR.so` or `libR.dylib` or `libR.dll`. On
+Linux, the configure flag `./configure --enable-R-shlib` may be needed to
+install R from the source. Do not forget to `make clean` to force the
+recompilation of the files with the correct compiler options. #### Outdated
+setuptools If you encounter > The package setup script has attempted to modify
+files on your system that are not within the EasyInstall build area. Please
+update your setuptools by ``` pip install -U setuptools ``` #### How to use
+local history file _radian_ maintains its own history file `.radian_history`
+and doesn't use the `.Rhistory` file. A local `.radian_history` is used if it
+is found in the launch directory. Otherwise, the global history file
+`~/.radian_history` would be used. To override the default behavior, you could
+launch _radian_ with the options: `radian --local-history`, `radian --global-
+history` or `radian --no-history`. #### Does it slow down my R program?
+_radian_ only provides a frontend to the R program, the actual running
+eventloop is the same as that of the traditional R console. There is no
+performance sacrifice (or gain) while using this modern command line interface.
+#### Nvim-R support Put ```vim let R_app = "radian" let R_cmd = "R" let
+R_hl_term = 0 let R_args = [] " if you had set any let R_bracketed_paste = 1
+``` in your vim config. #### `reticulate` Auto Completions To enable reticulate
+prompt completions, make sure that `jedi` is installed. ```sh pip install jedi
+``` Alternatively, if you use conda, ```sh conda install -c conda-forge jedi
+``` #### Prompt not shown inside a docker container It maybe caused by the
+invalid terminal size, try running `stty size` in your terminal to see if it
+returns a correct size. You could change the values of it from the
+environmental variables `$COLUMNS` and `$LINES` when you log-in the docker
+container. ``` docker exec -it  bash -c "stty cols $COLUMNS rows $LINES &&
+bash" ``` ## Why called _radian_? _radian_ is powered by (Ï)thon. ## Credits
+_radian_ wouldn't be possible without the creative work [prompt_toolkit](https:
+//github.com/jonathanslenders/python-prompt-toolkit/) by Jonathan Slenders.
+Platform: UNKNOWN Requires-Python: >=3.6 Description-Content-Type: text/
+markdown Provides-Extra: test
```

### Comparing `radian-0.6.4/README.md` & `radian-0.6.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 pip3 install -U git+https://github.com/randy3k/radian
 ```
 
 Alternatively, if you use conda or miniconda,
 ```sh
 conda install -c conda-forge radian
 ```
+In this case, it is recommended to install R via conda to ensure consistency in C runtime libraries.
 
 ## Alias on unix system
 
 You could alias `r` to _radian_ by putting
 
 ```bash
 alias r="radian"
@@ -162,20 +163,25 @@
 options(radian.enable_reticulate_prompt = TRUE)
 ```
 
 ### Custom key bindings
 
 ```r
 # allows user defined shortcuts, these keys should be escaped when send through the terminal.
-# In the following example, `esc` + `-` sends `<-` and `esc` + `m` sends `%>%`.
+# In the following example, `esc` + `-` sends `<-` and `ctrl` + `right` sends `%>%`.
 # Note that in some terminals, you could mark `alt` as `escape` so you could use `alt` + `-` instead.
-options(radian.escape_key_map = list(
-    list(key = "-", value = " <- "),
-    list(key = "m", value = " %>% ")
-))
+# Also, note that some ctrl mappings are reserved. You cannot remap m, i, h, d, or c
+options(
+    radian.escape_key_map = list(
+        list(key = "-", value = " <- "),
+    ),
+    radian.ctrl_key_map = list(
+        list(key = "right", value = " %>% ")
+    )
+)
 ```
 
 ## FAQ
 
 #### Unicode doesn't work in Windows and R 4.2+.
 
 The latest version of R supports Unicode codepage directly. However, radian relies on Python and Python doesn't support Unicode in the way that R supports it. A workaround could be found here: https://github.com/randy3k/radian/issues/269#issuecomment-1169663251
```

#### html2text {}

```diff
@@ -22,38 +22,40 @@
 downloaded from https://cran.r-project.org. - `python` (version 3.6 or above)
 is also required to install _radian_. If your system doesn't come with a python
 distribution, it can be downloaded from https://www.python.org/downloads/ or
 https://conda.io/en/latest/miniconda.html. - `pip` is optional but it makes the
 installation a bit easier. ```sh # install released version pip3 install -
 U radian # to run radian radian ``` ```sh # or the development version pip3
 install -U git+https://github.com/randy3k/radian ``` Alternatively, if you use
-conda or miniconda, ```sh conda install -c conda-forge radian ``` ## Alias on
-unix system You could alias `r` to _radian_ by putting ```bash alias r="radian"
-``` in `~/.bash_profile` such that `r` would open _radian_ and `R` would still
-open the traditional R console. (`R` is still useful, e.g, running `R CMD
-BUILD`.) ## Settings _radian_ can be customized by specifying the below options
-in various locations - `$XDG_CONFIG_HOME/radian/profile` or `$HOME/.config/
-radian/profile` (Unix) - `%USERPROFILE%/radian/profile` (Windows) -
-`$HOME/.radian_profile` (Unix) - `%USERPROFILE%/.radian_profile` (Windows) -
-`.radian_profile` in the working directory The options could be also specified
-in the `.Rprofile` files, however, it is not recommended because 1. the
-settings are not persistent when vanilla mode is used; 2. it doesn't work well
-with `packrat` or `renv`. ```r # Do not copy the whole configuration, just
-specify what you need! # see https://help.farbox.com/pygments.html # for a list
-of supported color schemes, default scheme is "native" options
-(radian.color_scheme = "native") # either `"emacs"` (default) or `"vi"`.
-options(radian.editing_mode = "emacs") # enable various emacs bindings in vi
-insert mode options(radian.emacs_bindings_in_vi_insert_mode = FALSE) # show vi
-mode state when radian.editing_mode is `vi` options(radian.show_vi_mode_prompt
-= TRUE) options(radian.vi_mode_prompt = "\033[0;34m[{}]\033[0m ") # indent
-continuation lines # turn this off if you want to copy code without the extra
-indentation; # but it leads to less elegent layout options(radian.indent_lines
-= TRUE) # auto match brackets and quotes options(radian.auto_match = TRUE) #
-enable the [prompt_toolkit](https://python-prompt-toolkit.readthedocs.io/en/
-master/index.html) [`auto_suggest` feature](https://python-prompt-
+conda or miniconda, ```sh conda install -c conda-forge radian ``` In this case,
+it is recommended to install R via conda to ensure consistency in C runtime
+libraries. ## Alias on unix system You could alias `r` to _radian_ by putting
+```bash alias r="radian" ``` in `~/.bash_profile` such that `r` would open
+_radian_ and `R` would still open the traditional R console. (`R` is still
+useful, e.g, running `R CMD BUILD`.) ## Settings _radian_ can be customized by
+specifying the below options in various locations - `$XDG_CONFIG_HOME/radian/
+profile` or `$HOME/.config/radian/profile` (Unix) - `%USERPROFILE%/radian/
+profile` (Windows) - `$HOME/.radian_profile` (Unix) -
+`%USERPROFILE%/.radian_profile` (Windows) - `.radian_profile` in the working
+directory The options could be also specified in the `.Rprofile` files,
+however, it is not recommended because 1. the settings are not persistent when
+vanilla mode is used; 2. it doesn't work well with `packrat` or `renv`. ```r #
+Do not copy the whole configuration, just specify what you need! # see https://
+help.farbox.com/pygments.html # for a list of supported color schemes, default
+scheme is "native" options(radian.color_scheme = "native") # either `"emacs"`
+(default) or `"vi"`. options(radian.editing_mode = "emacs") # enable various
+emacs bindings in vi insert mode options
+(radian.emacs_bindings_in_vi_insert_mode = FALSE) # show vi mode state when
+radian.editing_mode is `vi` options(radian.show_vi_mode_prompt = TRUE) options
+(radian.vi_mode_prompt = "\033[0;34m[{}]\033[0m ") # indent continuation lines
+# turn this off if you want to copy code without the extra indentation; # but
+it leads to less elegent layout options(radian.indent_lines = TRUE) # auto
+match brackets and quotes options(radian.auto_match = TRUE) # enable the
+[prompt_toolkit](https://python-prompt-toolkit.readthedocs.io/en/master/
+index.html) [`auto_suggest` feature](https://python-prompt-
 toolkit.readthedocs.io/en/master/pages/asking_for_input.html#auto-suggestion) #
 this option is experimental and is known to break python prompt, use it with
 caution options(radian.auto_suggest = FALSE) # highlight matching bracket
 options(radian.highlight_matching_bracket = FALSE) # auto indentation for new
 line and curly braces options(radian.auto_indentation = TRUE) options
 (radian.tab_size = 4) # pop up completion while typing options
 (radian.complete_while_typing = TRUE) # the minimum length of prefix to trigger
@@ -78,58 +80,59 @@
 = TRUE) # custom prompt for different modes options(radian.prompt = "\033
 [0;34mr$>\033[0m ") options(radian.shell_prompt = "\033[0;31m#!>\033[0m ")
 options(radian.browse_prompt = "\033[0;33mBrowse[{}]>\033[0m ") # stderr color
 format options(radian.stderr_format = "\033[0;31m{}\033[0m") # enable
 reticulate prompt and trigger `~` options(radian.enable_reticulate_prompt =
 TRUE) ``` ### Custom key bindings ```r # allows user defined shortcuts, these
 keys should be escaped when send through the terminal. # In the following
-example, `esc` + `-` sends `<-` and `esc` + `m` sends `%>%`. # Note that in
-some terminals, you could mark `alt` as `escape` so you could use `alt` + `-
-` instead. options(radian.escape_key_map = list( list(key = "-", value = " <-
-"), list(key = "m", value = " %>% ") )) ``` ## FAQ #### Unicode doesn't work in
-Windows and R 4.2+. The latest version of R supports Unicode codepage directly.
-However, radian relies on Python and Python doesn't support Unicode in the way
-that R supports it. A workaround could be found here: https://github.com/
-randy3k/radian/issues/269#issuecomment-1169663251 #### I can't specify python
-runtime in reticulate. It is expected. `radian` runs on python and the python
-runtime used by radian is forced in reticulate. `reticulate::py_config()` gives
-the note: ``` NOTE: Python version was forced by the current process ``` In
-order to use radian with another python runtime, you will need to install
-`radian` on that python environment. #### How to switch to a different R or
-specify the version of R. There are serveral options. - The easiest option is
-to pass the path to the R binary with `--r-binary`, i.e., `radian --r-binary=/
-path/to/R` - Also, one could expose the path to the R binary in the `PATH`
-variable - The environment variable `R_BINARY` could also be used to specify
-the path to R. - The environment variable `R_HOME` could also be used to
-specify R home directory. Note that it is should be set as the result of
-`R.home()`, not the directory where `R` is located. For example, in Unix ```sh
-$ env R_HOME=/usr/local/lib/R radian ``` #### Cannot find shared library Please
-also make sure that R was installed with the R shared library `libR.so` or
-`libR.dylib` or `libR.dll`. On Linux, the configure flag `./configure --enable-
-R-shlib` may be needed to install R from the source. Do not forget to `make
-clean` to force the recompilation of the files with the correct compiler
-options. #### Outdated setuptools If you encounter > The package setup script
-has attempted to modify files on your system that are not within the
-EasyInstall build area. Please update your setuptools by ``` pip install -
-U setuptools ``` #### How to use local history file _radian_ maintains its own
-history file `.radian_history` and doesn't use the `.Rhistory` file. A local
-`.radian_history` is used if it is found in the launch directory. Otherwise,
-the global history file `~/.radian_history` would be used. To override the
-default behavior, you could launch _radian_ with the options: `radian --local-
-history`, `radian --global-history` or `radian --no-history`. #### Does it slow
-down my R program? _radian_ only provides a frontend to the R program, the
-actual running eventloop is the same as that of the traditional R console.
-There is no performance sacrifice (or gain) while using this modern command
-line interface. #### Nvim-R support Put ```vim let R_app = "radian" let R_cmd =
-"R" let R_hl_term = 0 let R_args = [] " if you had set any let
-R_bracketed_paste = 1 ``` in your vim config. #### `reticulate` Auto
-Completions To enable reticulate prompt completions, make sure that `jedi` is
-installed. ```sh pip install jedi ``` Alternatively, if you use conda, ```sh
-conda install -c conda-forge jedi ``` #### Prompt not shown inside a docker
-container It maybe caused by the invalid terminal size, try running `stty size`
-in your terminal to see if it returns a correct size. You could change the
-values of it from the environmental variables `$COLUMNS` and `$LINES` when you
-log-in the docker container. ``` docker exec -it  bash -c "stty cols $COLUMNS
-rows $LINES && bash" ``` ## Why called _radian_? _radian_ is powered by
-(Ï)thon. ## Credits _radian_ wouldn't be possible without the creative work
-[prompt_toolkit](https://github.com/jonathanslenders/python-prompt-toolkit/) by
-Jonathan Slenders.
+example, `esc` + `-` sends `<-` and `ctrl` + `right` sends `%>%`. # Note that
+in some terminals, you could mark `alt` as `escape` so you could use `alt` + `-
+` instead. # Also, note that some ctrl mappings are reserved. You cannot remap
+m, i, h, d, or c options( radian.escape_key_map = list( list(key = "-", value =
+" <- "), ), radian.ctrl_key_map = list( list(key = "right", value = " %>% ") )
+) ``` ## FAQ #### Unicode doesn't work in Windows and R 4.2+. The latest
+version of R supports Unicode codepage directly. However, radian relies on
+Python and Python doesn't support Unicode in the way that R supports it. A
+workaround could be found here: https://github.com/randy3k/radian/issues/
+269#issuecomment-1169663251 #### I can't specify python runtime in reticulate.
+It is expected. `radian` runs on python and the python runtime used by radian
+is forced in reticulate. `reticulate::py_config()` gives the note: ``` NOTE:
+Python version was forced by the current process ``` In order to use radian
+with another python runtime, you will need to install `radian` on that python
+environment. #### How to switch to a different R or specify the version of R.
+There are serveral options. - The easiest option is to pass the path to the R
+binary with `--r-binary`, i.e., `radian --r-binary=/path/to/R` - Also, one
+could expose the path to the R binary in the `PATH` variable - The environment
+variable `R_BINARY` could also be used to specify the path to R. - The
+environment variable `R_HOME` could also be used to specify R home directory.
+Note that it is should be set as the result of `R.home()`, not the directory
+where `R` is located. For example, in Unix ```sh $ env R_HOME=/usr/local/lib/
+R radian ``` #### Cannot find shared library Please also make sure that R was
+installed with the R shared library `libR.so` or `libR.dylib` or `libR.dll`. On
+Linux, the configure flag `./configure --enable-R-shlib` may be needed to
+install R from the source. Do not forget to `make clean` to force the
+recompilation of the files with the correct compiler options. #### Outdated
+setuptools If you encounter > The package setup script has attempted to modify
+files on your system that are not within the EasyInstall build area. Please
+update your setuptools by ``` pip install -U setuptools ``` #### How to use
+local history file _radian_ maintains its own history file `.radian_history`
+and doesn't use the `.Rhistory` file. A local `.radian_history` is used if it
+is found in the launch directory. Otherwise, the global history file
+`~/.radian_history` would be used. To override the default behavior, you could
+launch _radian_ with the options: `radian --local-history`, `radian --global-
+history` or `radian --no-history`. #### Does it slow down my R program?
+_radian_ only provides a frontend to the R program, the actual running
+eventloop is the same as that of the traditional R console. There is no
+performance sacrifice (or gain) while using this modern command line interface.
+#### Nvim-R support Put ```vim let R_app = "radian" let R_cmd = "R" let
+R_hl_term = 0 let R_args = [] " if you had set any let R_bracketed_paste = 1
+``` in your vim config. #### `reticulate` Auto Completions To enable reticulate
+prompt completions, make sure that `jedi` is installed. ```sh pip install jedi
+``` Alternatively, if you use conda, ```sh conda install -c conda-forge jedi
+``` #### Prompt not shown inside a docker container It maybe caused by the
+invalid terminal size, try running `stty size` in your terminal to see if it
+returns a correct size. You could change the values of it from the
+environmental variables `$COLUMNS` and `$LINES` when you log-in the docker
+container. ``` docker exec -it  bash -c "stty cols $COLUMNS rows $LINES &&
+bash" ``` ## Why called _radian_? _radian_ is powered by (Ï)thon. ## Credits
+_radian_ wouldn't be possible without the creative work [prompt_toolkit](https:
+//github.com/jonathanslenders/python-prompt-toolkit/) by Jonathan Slenders.
```

### Comparing `radian-0.6.4/radian/__main__.py` & `radian-0.6.5/radian/__main__.py`

 * *Files identical despite different names*

### Comparing `radian-0.6.4/radian/app.py` & `radian-0.6.5/radian/app.py`

 * *Files identical despite different names*

### Comparing `radian-0.6.4/radian/completion.py` & `radian-0.6.5/radian/completion.py`

 * *Files identical despite different names*

### Comparing `radian-0.6.4/radian/console.py` & `radian-0.6.5/radian/console.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import signal
 import re
 from contextlib import contextmanager
 
 from .settings import radian_settings as settings
+from .rutils import is_long_non_ascii_multiline
 from rchitect import console
 
 TERMINAL_CURSOR_AT_BEGINNING = [True]
 
 SUPPRESS_STDOUT = False
 SUPPRESS_STDERR = False
 ANSI_ESCAPE_RE = re.compile(r'\x1B\[[0-?]*[ -/]*[@-~]')
@@ -115,38 +116,42 @@
                     os._exit(1)
 
             if text is None and settings.insert_new_line and current_mode_spec.insert_new_line:
                 app.output.write_raw("\n")
 
         return text
 
-    _text = [""]
-    startpos = [0]
+    _text_stored = ["", 0, False]  # text, startpos, sent_by_line
 
     def read_console(message, add_history):
         if session.current_mode in ["r", "browse"]:
             # this code is needed to allow new line breaks with strings, see #377
-            if _text[0]:
-                text = _text[0][startpos[0]:]
+            if _text_stored[0]:
+                text = _text_stored[0][_text_stored[1]:]
             else:
                 text = _read_console(message, add_history)
-                if text and "\n" in text:
+                if text and is_long_non_ascii_multiline(text):
                     # make sure the text is evaluated at once
+                    # in case it includes long multiline strings, see #379
                     text = "{\n" + text + "\n}"
-                _text[0] = text
-                startpos[0] = 0
+                    _text_stored[2] = True
+
+                _text_stored[0] = text
+                _text_stored[1] = 0
 
             if text:
+                sent_by_line = _text_stored[2]
                 index = text.find('\n')
-                if index >= 0:
-                    startpos[0] += index + 1
+                if sent_by_line and index >= 0:
+                    _text_stored[1] += index + 1
                     text = text[:index]
                 else:
-                    _text[0] = ""
-                    startpos[0] = 0
+                    _text_stored[0] = ""
+                    _text_stored[1] = 0
+                    _text_stored[1] = False
         else:
             text = _read_console(message, add_history)
 
         return text
 
     return read_console
```

### Comparing `radian-0.6.4/radian/document.py` & `radian-0.6.5/radian/document.py`

 * *Files identical despite different names*

### Comparing `radian-0.6.4/radian/io.py` & `radian-0.6.5/radian/io.py`

 * *Files identical despite different names*

### Comparing `radian-0.6.4/radian/key_bindings.py` & `radian-0.6.5/radian/key_bindings.py`

 * *Files identical despite different names*

### Comparing `radian-0.6.4/radian/latex/__init__.py` & `radian-0.6.5/radian/latex/__init__.py`

 * *Files identical despite different names*

### Comparing `radian-0.6.4/radian/latex/latex_symbols.py` & `radian-0.6.5/radian/latex/latex_symbols.py`

 * *Files identical despite different names*

### Comparing `radian-0.6.4/radian/lexer.py` & `radian-0.6.5/radian/lexer.py`

 * *Files identical despite different names*

### Comparing `radian-0.6.4/radian/lineedit/buffer.py` & `radian-0.6.5/radian/lineedit/buffer.py`

 * *Files identical despite different names*

### Comparing `radian-0.6.4/radian/lineedit/history.py` & `radian-0.6.5/radian/lineedit/history.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                             breaks.append(i)
                         lines = []
 
                 add()
 
             if len(breaks) > max(self.max_history_size, 10):
                 # trim history if it is too big
-                with open(self.filename, "r+") as f:
+                with open(self.filename, "r+", encoding="utf-8") as f:
                     backup = f.readlines()
                     f.seek(0)
                     f.truncate()
                     trimed = backup[breaks[-round(self.max_history_size * 0.9)]+1:]
                     f.writelines(trimed)
 
         # Reverse the order, because newest items have to go first.
```

### Comparing `radian-0.6.4/radian/lineedit/prompt.py` & `radian-0.6.5/radian/lineedit/prompt.py`

 * *Files identical despite different names*

### Comparing `radian-0.6.4/radian/prompt_session.py` & `radian-0.6.5/radian/prompt_session.py`

 * *Files identical despite different names*

### Comparing `radian-0.6.4/radian/reticulate/__init__.py` & `radian-0.6.5/radian/reticulate/__init__.py`

 * *Files identical despite different names*

### Comparing `radian-0.6.4/radian/reticulate/config.R` & `radian-0.6.5/radian/reticulate/config.R`

 * *Files identical despite different names*

### Comparing `radian-0.6.4/radian/reticulate/key_bindings.R` & `radian-0.6.5/radian/reticulate/key_bindings.R`

 * *Files identical despite different names*

### Comparing `radian-0.6.4/radian/rutils.py` & `radian-0.6.5/radian/rutils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 import os
 import sys
 from rchitect import rcopy, reval, rcall
 from rchitect.interface import roption
 from .key_bindings import map_key
 
 
+def is_long_non_ascii_multiline(text):
+    if text.isascii():
+        return False
+    if "\n" not in text:
+        return False
+    if len(text) < 1000:
+        return False
+    return True
+
+
 def package_is_loaded(pkg):
     return pkg in rcopy(rcall(("base", "loadedNamespaces")))
 
 
 def package_is_installed(pkg):
     return pkg in installed_packages()
 
@@ -64,14 +74,22 @@
 
 
 def load_custom_key_bindings(*args):
     esc_keymap = roption("radian.escape_key_map", [])
     for m in esc_keymap:
         map_key(("escape", m["key"]), m["value"], mode=m["mode"] if "mode" in m else "r")
 
+    keymap = roption("radian.ctrl_key_map", [])
+    for m in keymap:
+        if m["key"] in "mihdc":
+            print("WARNING: Cannot remap c-" + m["key"] + ". Please remove this mapping from radian.ctrl_key_map in your radian profile")
+        else:
+            map_key(("c-" + m["key"],), m["value"], mode=m["mode"] if "mode" in m else "r")
+
+
 
 def register_cleanup(cleanup):
     rcall(("base", "reg.finalizer"),
           rcall(("base", "getOption"), "rchitect.py_tools"),
           cleanup,
           onexit=True)
```

### Comparing `radian-0.6.4/radian/settings.py` & `radian-0.6.5/radian/settings.py`

 * *Files identical despite different names*

### Comparing `radian-0.6.4/radian/shell.py` & `radian-0.6.5/radian/shell.py`

 * *Files identical despite different names*

### Comparing `radian-0.6.4/radian.egg-info/PKG-INFO` & `radian-0.6.5/radian.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radian
-Version: 0.6.4
+Version: 0.6.5
 Summary: A 21 century R console
 Home-page: https://github.com/randy3k/radian
 Author: Randy Lai
 License: UNKNOWN
 Description: # radian: A 21 century R console
         
         [![Main](https://github.com/randy3k/radian/actions/workflows/main.yml/badge.svg)](https://github.com/randy3k/radian/actions/workflows/main.yml)
@@ -60,14 +60,15 @@
         pip3 install -U git+https://github.com/randy3k/radian
         ```
         
         Alternatively, if you use conda or miniconda,
         ```sh
         conda install -c conda-forge radian
         ```
+        In this case, it is recommended to install R via conda to ensure consistency in C runtime libraries.
         
         ## Alias on unix system
         
         You could alias `r` to _radian_ by putting
         
         ```bash
         alias r="radian"
@@ -169,20 +170,25 @@
         options(radian.enable_reticulate_prompt = TRUE)
         ```
         
         ### Custom key bindings
         
         ```r
         # allows user defined shortcuts, these keys should be escaped when send through the terminal.
-        # In the following example, `esc` + `-` sends `<-` and `esc` + `m` sends `%>%`.
+        # In the following example, `esc` + `-` sends `<-` and `ctrl` + `right` sends `%>%`.
         # Note that in some terminals, you could mark `alt` as `escape` so you could use `alt` + `-` instead.
-        options(radian.escape_key_map = list(
-            list(key = "-", value = " <- "),
-            list(key = "m", value = " %>% ")
-        ))
+        # Also, note that some ctrl mappings are reserved. You cannot remap m, i, h, d, or c
+        options(
+            radian.escape_key_map = list(
+                list(key = "-", value = " <- "),
+            ),
+            radian.ctrl_key_map = list(
+                list(key = "right", value = " %>% ")
+            )
+        )
         ```
         
         ## FAQ
         
         #### Unicode doesn't work in Windows and R 4.2+.
         
         The latest version of R supports Unicode codepage directly. However, radian relies on Python and Python doesn't support Unicode in the way that R supports it. A workaround could be found here: https://github.com/randy3k/radian/issues/269#issuecomment-1169663251
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: radian Version: 0.6.4 Summary: A 21 century R
+Metadata-Version: 2.1 Name: radian Version: 0.6.5 Summary: A 21 century R
 console Home-page: https://github.com/randy3k/radian Author: Randy Lai License:
 UNKNOWN Description: # radian: A 21 century R console [![Main](https://
 github.com/randy3k/radian/actions/workflows/main.yml/badge.svg)](https://
 github.com/randy3k/radian/actions/workflows/main.yml) [![codecov](https://
 codecov.io/gh/randy3k/radian/branch/master/graph/badge.svg)](https://
 codecov.io/gh/randy3k/radian) [![](https://img.shields.io/pypi/v/radian.svg)]
 (https://pypi.org/project/radian/) [![Conda version](https://img.shields.io/
@@ -25,38 +25,39 @@
 3.6 or above) is also required to install _radian_. If your system doesn't come
 with a python distribution, it can be downloaded from https://www.python.org/
 downloads/ or https://conda.io/en/latest/miniconda.html. - `pip` is optional
 but it makes the installation a bit easier. ```sh # install released version
 pip3 install -U radian # to run radian radian ``` ```sh # or the development
 version pip3 install -U git+https://github.com/randy3k/radian ```
 Alternatively, if you use conda or miniconda, ```sh conda install -c conda-
-forge radian ``` ## Alias on unix system You could alias `r` to _radian_ by
-putting ```bash alias r="radian" ``` in `~/.bash_profile` such that `r` would
-open _radian_ and `R` would still open the traditional R console. (`R` is still
-useful, e.g, running `R CMD BUILD`.) ## Settings _radian_ can be customized by
-specifying the below options in various locations - `$XDG_CONFIG_HOME/radian/
-profile` or `$HOME/.config/radian/profile` (Unix) - `%USERPROFILE%/radian/
-profile` (Windows) - `$HOME/.radian_profile` (Unix) -
-`%USERPROFILE%/.radian_profile` (Windows) - `.radian_profile` in the working
-directory The options could be also specified in the `.Rprofile` files,
-however, it is not recommended because 1. the settings are not persistent when
-vanilla mode is used; 2. it doesn't work well with `packrat` or `renv`. ```r #
-Do not copy the whole configuration, just specify what you need! # see https://
-help.farbox.com/pygments.html # for a list of supported color schemes, default
-scheme is "native" options(radian.color_scheme = "native") # either `"emacs"`
-(default) or `"vi"`. options(radian.editing_mode = "emacs") # enable various
-emacs bindings in vi insert mode options
-(radian.emacs_bindings_in_vi_insert_mode = FALSE) # show vi mode state when
-radian.editing_mode is `vi` options(radian.show_vi_mode_prompt = TRUE) options
-(radian.vi_mode_prompt = "\033[0;34m[{}]\033[0m ") # indent continuation lines
-# turn this off if you want to copy code without the extra indentation; # but
-it leads to less elegent layout options(radian.indent_lines = TRUE) # auto
-match brackets and quotes options(radian.auto_match = TRUE) # enable the
-[prompt_toolkit](https://python-prompt-toolkit.readthedocs.io/en/master/
-index.html) [`auto_suggest` feature](https://python-prompt-
+forge radian ``` In this case, it is recommended to install R via conda to
+ensure consistency in C runtime libraries. ## Alias on unix system You could
+alias `r` to _radian_ by putting ```bash alias r="radian" ``` in
+`~/.bash_profile` such that `r` would open _radian_ and `R` would still open
+the traditional R console. (`R` is still useful, e.g, running `R CMD BUILD`.)
+## Settings _radian_ can be customized by specifying the below options in
+various locations - `$XDG_CONFIG_HOME/radian/profile` or `$HOME/.config/radian/
+profile` (Unix) - `%USERPROFILE%/radian/profile` (Windows) -
+`$HOME/.radian_profile` (Unix) - `%USERPROFILE%/.radian_profile` (Windows) -
+`.radian_profile` in the working directory The options could be also specified
+in the `.Rprofile` files, however, it is not recommended because 1. the
+settings are not persistent when vanilla mode is used; 2. it doesn't work well
+with `packrat` or `renv`. ```r # Do not copy the whole configuration, just
+specify what you need! # see https://help.farbox.com/pygments.html # for a list
+of supported color schemes, default scheme is "native" options
+(radian.color_scheme = "native") # either `"emacs"` (default) or `"vi"`.
+options(radian.editing_mode = "emacs") # enable various emacs bindings in vi
+insert mode options(radian.emacs_bindings_in_vi_insert_mode = FALSE) # show vi
+mode state when radian.editing_mode is `vi` options(radian.show_vi_mode_prompt
+= TRUE) options(radian.vi_mode_prompt = "\033[0;34m[{}]\033[0m ") # indent
+continuation lines # turn this off if you want to copy code without the extra
+indentation; # but it leads to less elegent layout options(radian.indent_lines
+= TRUE) # auto match brackets and quotes options(radian.auto_match = TRUE) #
+enable the [prompt_toolkit](https://python-prompt-toolkit.readthedocs.io/en/
+master/index.html) [`auto_suggest` feature](https://python-prompt-
 toolkit.readthedocs.io/en/master/pages/asking_for_input.html#auto-suggestion) #
 this option is experimental and is known to break python prompt, use it with
 caution options(radian.auto_suggest = FALSE) # highlight matching bracket
 options(radian.highlight_matching_bracket = FALSE) # auto indentation for new
 line and curly braces options(radian.auto_indentation = TRUE) options
 (radian.tab_size = 4) # pop up completion while typing options
 (radian.complete_while_typing = TRUE) # the minimum length of prefix to trigger
@@ -81,59 +82,61 @@
 = TRUE) # custom prompt for different modes options(radian.prompt = "\033
 [0;34mr$>\033[0m ") options(radian.shell_prompt = "\033[0;31m#!>\033[0m ")
 options(radian.browse_prompt = "\033[0;33mBrowse[{}]>\033[0m ") # stderr color
 format options(radian.stderr_format = "\033[0;31m{}\033[0m") # enable
 reticulate prompt and trigger `~` options(radian.enable_reticulate_prompt =
 TRUE) ``` ### Custom key bindings ```r # allows user defined shortcuts, these
 keys should be escaped when send through the terminal. # In the following
-example, `esc` + `-` sends `<-` and `esc` + `m` sends `%>%`. # Note that in
-some terminals, you could mark `alt` as `escape` so you could use `alt` + `-
-` instead. options(radian.escape_key_map = list( list(key = "-", value = " <-
-"), list(key = "m", value = " %>% ") )) ``` ## FAQ #### Unicode doesn't work in
-Windows and R 4.2+. The latest version of R supports Unicode codepage directly.
-However, radian relies on Python and Python doesn't support Unicode in the way
-that R supports it. A workaround could be found here: https://github.com/
-randy3k/radian/issues/269#issuecomment-1169663251 #### I can't specify python
-runtime in reticulate. It is expected. `radian` runs on python and the python
-runtime used by radian is forced in reticulate. `reticulate::py_config()` gives
-the note: ``` NOTE: Python version was forced by the current process ``` In
-order to use radian with another python runtime, you will need to install
-`radian` on that python environment. #### How to switch to a different R or
-specify the version of R. There are serveral options. - The easiest option is
-to pass the path to the R binary with `--r-binary`, i.e., `radian --r-binary=/
-path/to/R` - Also, one could expose the path to the R binary in the `PATH`
-variable - The environment variable `R_BINARY` could also be used to specify
-the path to R. - The environment variable `R_HOME` could also be used to
-specify R home directory. Note that it is should be set as the result of
-`R.home()`, not the directory where `R` is located. For example, in Unix ```sh
-$ env R_HOME=/usr/local/lib/R radian ``` #### Cannot find shared library Please
-also make sure that R was installed with the R shared library `libR.so` or
-`libR.dylib` or `libR.dll`. On Linux, the configure flag `./configure --enable-
-R-shlib` may be needed to install R from the source. Do not forget to `make
-clean` to force the recompilation of the files with the correct compiler
-options. #### Outdated setuptools If you encounter > The package setup script
-has attempted to modify files on your system that are not within the
-EasyInstall build area. Please update your setuptools by ``` pip install -
-U setuptools ``` #### How to use local history file _radian_ maintains its own
-history file `.radian_history` and doesn't use the `.Rhistory` file. A local
-`.radian_history` is used if it is found in the launch directory. Otherwise,
-the global history file `~/.radian_history` would be used. To override the
-default behavior, you could launch _radian_ with the options: `radian --local-
-history`, `radian --global-history` or `radian --no-history`. #### Does it slow
-down my R program? _radian_ only provides a frontend to the R program, the
-actual running eventloop is the same as that of the traditional R console.
-There is no performance sacrifice (or gain) while using this modern command
-line interface. #### Nvim-R support Put ```vim let R_app = "radian" let R_cmd =
-"R" let R_hl_term = 0 let R_args = [] " if you had set any let
-R_bracketed_paste = 1 ``` in your vim config. #### `reticulate` Auto
-Completions To enable reticulate prompt completions, make sure that `jedi` is
-installed. ```sh pip install jedi ``` Alternatively, if you use conda, ```sh
-conda install -c conda-forge jedi ``` #### Prompt not shown inside a docker
-container It maybe caused by the invalid terminal size, try running `stty size`
-in your terminal to see if it returns a correct size. You could change the
-values of it from the environmental variables `$COLUMNS` and `$LINES` when you
-log-in the docker container. ``` docker exec -it  bash -c "stty cols $COLUMNS
-rows $LINES && bash" ``` ## Why called _radian_? _radian_ is powered by
-(Ï)thon. ## Credits _radian_ wouldn't be possible without the creative work
-[prompt_toolkit](https://github.com/jonathanslenders/python-prompt-toolkit/) by
-Jonathan Slenders. Platform: UNKNOWN Requires-Python: >=3.6 Description-
-Content-Type: text/markdown Provides-Extra: test
+example, `esc` + `-` sends `<-` and `ctrl` + `right` sends `%>%`. # Note that
+in some terminals, you could mark `alt` as `escape` so you could use `alt` + `-
+` instead. # Also, note that some ctrl mappings are reserved. You cannot remap
+m, i, h, d, or c options( radian.escape_key_map = list( list(key = "-", value =
+" <- "), ), radian.ctrl_key_map = list( list(key = "right", value = " %>% ") )
+) ``` ## FAQ #### Unicode doesn't work in Windows and R 4.2+. The latest
+version of R supports Unicode codepage directly. However, radian relies on
+Python and Python doesn't support Unicode in the way that R supports it. A
+workaround could be found here: https://github.com/randy3k/radian/issues/
+269#issuecomment-1169663251 #### I can't specify python runtime in reticulate.
+It is expected. `radian` runs on python and the python runtime used by radian
+is forced in reticulate. `reticulate::py_config()` gives the note: ``` NOTE:
+Python version was forced by the current process ``` In order to use radian
+with another python runtime, you will need to install `radian` on that python
+environment. #### How to switch to a different R or specify the version of R.
+There are serveral options. - The easiest option is to pass the path to the R
+binary with `--r-binary`, i.e., `radian --r-binary=/path/to/R` - Also, one
+could expose the path to the R binary in the `PATH` variable - The environment
+variable `R_BINARY` could also be used to specify the path to R. - The
+environment variable `R_HOME` could also be used to specify R home directory.
+Note that it is should be set as the result of `R.home()`, not the directory
+where `R` is located. For example, in Unix ```sh $ env R_HOME=/usr/local/lib/
+R radian ``` #### Cannot find shared library Please also make sure that R was
+installed with the R shared library `libR.so` or `libR.dylib` or `libR.dll`. On
+Linux, the configure flag `./configure --enable-R-shlib` may be needed to
+install R from the source. Do not forget to `make clean` to force the
+recompilation of the files with the correct compiler options. #### Outdated
+setuptools If you encounter > The package setup script has attempted to modify
+files on your system that are not within the EasyInstall build area. Please
+update your setuptools by ``` pip install -U setuptools ``` #### How to use
+local history file _radian_ maintains its own history file `.radian_history`
+and doesn't use the `.Rhistory` file. A local `.radian_history` is used if it
+is found in the launch directory. Otherwise, the global history file
+`~/.radian_history` would be used. To override the default behavior, you could
+launch _radian_ with the options: `radian --local-history`, `radian --global-
+history` or `radian --no-history`. #### Does it slow down my R program?
+_radian_ only provides a frontend to the R program, the actual running
+eventloop is the same as that of the traditional R console. There is no
+performance sacrifice (or gain) while using this modern command line interface.
+#### Nvim-R support Put ```vim let R_app = "radian" let R_cmd = "R" let
+R_hl_term = 0 let R_args = [] " if you had set any let R_bracketed_paste = 1
+``` in your vim config. #### `reticulate` Auto Completions To enable reticulate
+prompt completions, make sure that `jedi` is installed. ```sh pip install jedi
+``` Alternatively, if you use conda, ```sh conda install -c conda-forge jedi
+``` #### Prompt not shown inside a docker container It maybe caused by the
+invalid terminal size, try running `stty size` in your terminal to see if it
+returns a correct size. You could change the values of it from the
+environmental variables `$COLUMNS` and `$LINES` when you log-in the docker
+container. ``` docker exec -it  bash -c "stty cols $COLUMNS rows $LINES &&
+bash" ``` ## Why called _radian_? _radian_ is powered by (Ï)thon. ## Credits
+_radian_ wouldn't be possible without the creative work [prompt_toolkit](https:
+//github.com/jonathanslenders/python-prompt-toolkit/) by Jonathan Slenders.
+Platform: UNKNOWN Requires-Python: >=3.6 Description-Content-Type: text/
+markdown Provides-Extra: test
```

### Comparing `radian-0.6.4/radian.egg-info/SOURCES.txt` & `radian-0.6.5/radian.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `radian-0.6.4/setup.py` & `radian-0.6.5/setup.py`

 * *Files identical despite different names*

