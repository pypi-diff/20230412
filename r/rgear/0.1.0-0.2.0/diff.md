# Comparing `tmp/rgear-0.1.0.tar.gz` & `tmp/rgear-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rgear-0.1.0.tar", max compression
+gzip compressed data, was "rgear-0.2.0.tar", max compression
```

## Comparing `rgear-0.1.0.tar` & `rgear-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1070 2023-03-22 10:38:15.240449 rgear-0.1.0/LICENSE
--rw-r--r--   0        0        0     1358 2023-04-11 18:07:12.495284 rgear-0.1.0/README.md
--rw-r--r--   0        0        0      468 2023-04-11 18:02:26.069649 rgear-0.1.0/pyproject.toml
--rwxr-xr-x   0        0        0     6505 2023-04-11 18:05:47.026589 rgear-0.1.0/rgear/__init__.py
--rw-r--r--   0        0        0     2007 1970-01-01 00:00:00.000000 rgear-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-03-22 10:38:15.240449 rgear-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3018 2023-04-12 11:35:49.011301 rgear-0.2.0/README.md
+-rw-r--r--   0        0        0      468 2023-04-12 10:08:55.763117 rgear-0.2.0/pyproject.toml
+-rwxr-xr-x   0        0        0     7178 2023-04-12 12:07:30.610858 rgear-0.2.0/rgear/__init__.py
+-rw-r--r--   0        0        0     3667 1970-01-01 00:00:00.000000 rgear-0.2.0/PKG-INFO
```

### Comparing `rgear-0.1.0/LICENSE` & `rgear-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rgear-0.1.0/rgear/__init__.py` & `rgear-0.2.0/rgear/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 #!/usr/bin/env python3
 """
-Command line utility to generate various types of helper script for using R in Domino
+Command line utility to generate various types of helper script for starting
+R based servers
 """
 
 import argparse
 import os.path
+from os import chmod
 import sys
 
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 
 
 # TEMPLATES
 
 SHINY_APP_START = """\
-# Simple shiny app startup script for use on Domino
+# Shiny app startup script
 # Generated with rgear (https://github.com/sellorm/rgear)
-R -e 'shiny::runApp("{}", host="0.0.0.0", port=8888)'
+R -e 'shiny::runApp("{}", host="0.0.0.0", port={})'
 """
 
 PLUMBER_APP_START = """\
-# Simple plumber API startup scriptt for use on Domino
+# Plumber API startup script
 # Generated with rgear (https://github.com/sellorm/rgear)
-R -e 'plumber::pr_run(plumber::pr("{}"), host = "0.0.0.0", port = 8888)'
+R -e 'plumber::pr_run(plumber::pr("{}"), host="0.0.0.0", port={})'
 """
 
 RMARKDOWN_APP_START = """\
-# quick web server for serving an Rmarkdown docuent for use on Domino
+# Web server for serving an Rmarkdown document
 # Generated with rgear (https://github.com/sellorm/rgear)
-python3 -m http.server --bind "0.0.0.0" 8888
+python3 -m http.server --bind "0.0.0.0" {}
 """
 
 RMARKDOWN_APP_INDEX = """\
 <!DOCTYPE html>
 <!-- redirect to the actual content -->
 <!-- Generated with rgear (https://github.com/sellorm/rgear) -->
 <html>
@@ -83,132 +85,161 @@
         return True
     return False
 
 
 # File generator functions
 
 
-def generate_shiny(shiny_app, overwrite=False, verbose=False):
+def generate_shiny(shiny_app, overwrite=False, verbose=False, port=8888):
     """
-    Generates helper file for serving shiny apps
+    Generate helper files for serving shiny apps
 
     Keyword Arguments:
     shiny_app      -- path to your shiny app
     overwrite      -- whether to overwrite existing helper files
     verbose        -- prints more verbose output
+    port           -- The port to listen on [default: 8888]
 
     Generated file:
-    * app.sh -- starts the shiny app with Domino specific parameters
+    * app.sh -- starts the shiny app
     """
     print("Generating app.sh...")
     if not overwrite:
         file_exists("app.sh", print_err=True)
     file_does_not_exist(shiny_app, print_err=True)
+    app_template = SHINY_APP_START.format(shiny_app, port)
     with open("app.sh", "w", encoding="utf8") as file:
-        file.write(SHINY_APP_START.format(shiny_app))
+        file.write(app_template)
+    chmod("app.sh", 0o755)
     if verbose:
         print("---- app.sh ----")
-        print(SHINY_APP_START.format(shiny_app))
+        print(app_template)
     print("Complete.")
 
 
-def generate_rmarkdown(rmarkdown_html, overwrite=False, verbose=False):
+def generate_rmarkdown(rmarkdown_html, overwrite=False, verbose=False, port=8888):
     """
     Generates helper files for serving Rmarkdown documents
 
     Keyword Arguments:
     rmarkdown_html -- path to your Rmarkdown file's html output
     overwrite      -- whether to overwrite existing helper files
     verbose        -- prints more verbose output
+    port           -- The port to listen on [default: 8888]
 
     Generated files:
     * app.sh     -- starts a webserver to serve the generated Rmarkdown html
     * index.html -- Redirects default browser path to the Rmarkdown page
     """
     print("Generating app.sh and index.html...")
     if not overwrite:
         file_exists("app.sh", print_err=True)
     if not overwrite:
         file_exists("index.html", print_err=True)
     file_does_not_exist(rmarkdown_html, print_err=True)
+    app_template = RMARKDOWN_APP_START.format(port)
+    index_template = RMARKDOWN_APP_INDEX.format(rmarkdown_html)
     with open("app.sh", "w", encoding="utf8") as file:
-        file.write(RMARKDOWN_APP_START)
+        file.write(app_template)
+    chmod("app.sh", 0o755)
     if verbose:
         print("---- app.sh ----")
-        print(RMARKDOWN_APP_START)
+        print(app_template)
     with open("index.html", "w", encoding="utf8") as file:
-        file.write(RMARKDOWN_APP_INDEX.format(rmarkdown_html))
+        file.write(index_template)
     if verbose:
-        print("---- app.sh ----")
-        print(RMARKDOWN_APP_INDEX.format(rmarkdown_html))
+        print("---- index.html ----")
+        print(index_template)
     print("Complete.")
 
 
-def generate_plumber(plumber_file, overwrite=False, verbose=False):
+def generate_plumber(plumber_file, overwrite=False, verbose=False, port=8888):
     """
     Generates helper files for serving plumber APIs
 
     Keyword Arguments:
     plumber_file   -- path to your plumber file to serve
     overwrite      -- whether to overwrite existing helper files
     verbose        -- prints more verbose output
+    port           -- The port to listen on [default: 8888]
 
     Generated file:
-    * app.sh -- starts the plumber API with Domino specific parameters
+    * app.sh -- starts the plumber API
     """
     print("Generating app.sh...")
     if not overwrite:
         file_exists("app.sh", print_err=True)
     file_does_not_exist(plumber_file, print_err=True)
+    app_template = PLUMBER_APP_START.format(plumber_file, port)
     with open("app.sh", "w", encoding="utf8") as file:
-        file.write(PLUMBER_APP_START.format(plumber_file))
+        file.write(app_template)
+    chmod("app.sh", 0o755)
     if verbose:
         print("---- app.sh ----")
-        print(PLUMBER_APP_START.format(plumber_file))
+        print(app_template)
     print("Complete.")
 
 
 # Main
 def cli_arg_parser(args=None):
     """
     CLI argument parsing (extracted from main to make testing easier)
     """
     parser = argparse.ArgumentParser(
         prog="rgear",
-        description="Generates R helpers for Domino",
+        description="Generates helper scripts for starting R based content servers",
         epilog="For detailed help, please see https://github.com/sellorm/rgear",
     )
     parser.add_argument(
         "content_type",
-        help="Choose the application type you want to serve",
+        help="choose the application type you want to serve",
         choices=["shiny", "plumber", "rmarkdown"],
     )
     parser.add_argument("path", help="path to the content to serve")
     parser.add_argument(
         "-f",
         "--force",
-        help="Forces overwrite if the output file(s) already exist",
+        help="force overwrite if the output file(s) already exist",
         action="store_true",
     )
-    parser.add_argument("-v", "--verbose", action="store_true")
-    parser.add_argument('--version', action='version', version= __version__)
+    parser.add_argument(
+        "-p",
+        "--port",
+        help="override the default port setting. [default: %(default)s]",
+        default=8888,
+    )
+    parser.add_argument(
+        "-v", "--verbose", help="enable verbose output", action="store_true"
+    )
+    parser.add_argument(
+        "--version",
+        help="print the version and exit",
+        action="version",
+        version=__version__,
+    )
     return parser.parse_args(args)
 
 
 def main():
     """
     Pulls everything together and runs the command line tool
     """
     args = cli_arg_parser(sys.argv[1:])
 
     if args.content_type == "shiny":
-        generate_shiny(args.path, overwrite=args.force, verbose=args.verbose)
+        generate_shiny(
+            args.path, overwrite=args.force, verbose=args.verbose, port=args.port
+        )
 
     if args.content_type == "rmarkdown":
-        generate_rmarkdown(args.path, overwrite=args.force, verbose=args.verbose)
+        generate_rmarkdown(
+            args.path, overwrite=args.force, verbose=args.verbose, port=args.port
+        )
 
     if args.content_type == "plumber":
-        generate_plumber(args.path, overwrite=args.force, verbose=args.verbose)
+        generate_plumber(
+            args.path, overwrite=args.force, verbose=args.verbose, port=args.port
+        )
 
 
 if __name__ == "__main__":
     main()
```

