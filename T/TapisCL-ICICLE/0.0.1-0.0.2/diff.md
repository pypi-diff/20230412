# Comparing `tmp/TapisCL-ICICLE-0.0.1.tar.gz` & `tmp/TapisCL-ICICLE-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TapisCL-ICICLE-0.0.1.tar", last modified: Wed Apr  5 00:40:00 2023, max compression
+gzip compressed data, was "TapisCL-ICICLE-0.0.2.tar", last modified: Wed Apr 12 21:32:36 2023, max compression
```

## Comparing `TapisCL-ICICLE-0.0.1.tar` & `TapisCL-ICICLE-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 00:40:00.100747 TapisCL-ICICLE-0.0.1/
--rw-rw-rw-   0        0        0    35823 2023-04-05 00:09:53.000000 TapisCL-ICICLE-0.0.1/LICENSE
--rw-rw-rw-   0        0        0    42756 2023-04-05 00:40:00.099747 TapisCL-ICICLE-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      841 2023-04-05 00:09:53.000000 TapisCL-ICICLE-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-05 00:40:00.098749 TapisCL-ICICLE-0.0.1/TapisCL_ICICLE.egg-info/
--rw-rw-rw-   0        0        0    42756 2023-04-05 00:40:00.000000 TapisCL-ICICLE-0.0.1/TapisCL_ICICLE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-04-05 00:40:00.000000 TapisCL-ICICLE-0.0.1/TapisCL_ICICLE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 00:40:00.000000 TapisCL-ICICLE-0.0.1/TapisCL_ICICLE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-04-05 00:40:00.000000 TapisCL-ICICLE-0.0.1/TapisCL_ICICLE.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 00:40:00.000000 TapisCL-ICICLE-0.0.1/TapisCL_ICICLE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1008 2023-04-05 00:39:22.000000 TapisCL-ICICLE-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-05 00:40:00.101749 TapisCL-ICICLE-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-12 21:32:36.540827 TapisCL-ICICLE-0.0.2/
+-rw-rw-rw-   0        0        0    35823 2023-04-12 03:10:40.000000 TapisCL-ICICLE-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0    43023 2023-04-12 21:32:36.539829 TapisCL-ICICLE-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1114 2023-04-12 05:02:25.000000 TapisCL-ICICLE-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 21:32:36.532332 TapisCL-ICICLE-0.0.2/TapisCLICICLE/
+-rw-rw-rw-   0        0        0        0 2023-04-12 03:10:40.000000 TapisCL-ICICLE-0.0.2/TapisCLICICLE/__init__.py
+-rw-rw-rw-   0        0        0     1408 2023-04-12 20:12:15.000000 TapisCL-ICICLE-0.0.2/TapisCLICICLE/args.py
+-rw-rw-rw-   0        0        0    11151 2023-04-12 21:12:56.000000 TapisCL-ICICLE-0.0.2/TapisCLICICLE/cli.py
+-rw-rw-rw-   0        0        0     6873 2023-04-12 21:08:42.000000 TapisCL-ICICLE-0.0.2/TapisCLICICLE/decorators.py
+-rw-rw-rw-   0        0        0     1772 2023-04-12 03:10:40.000000 TapisCL-ICICLE-0.0.2/TapisCLICICLE/exceptions.py
+-rw-rw-rw-   0        0        0     4985 2023-04-12 20:49:51.000000 TapisCL-ICICLE-0.0.2/TapisCLICICLE/helpers.py
+-rw-rw-rw-   0        0        0     1049 2023-04-12 16:16:32.000000 TapisCL-ICICLE-0.0.2/TapisCLICICLE/schemas.py
+-rw-rw-rw-   0        0        0    10512 2023-04-12 21:18:32.000000 TapisCL-ICICLE-0.0.2/TapisCLICICLE/server.py
+-rw-rw-rw-   0        0        0     1757 2023-04-12 17:45:30.000000 TapisCL-ICICLE-0.0.2/TapisCLICICLE/socketOpts.py
+-rw-rw-rw-   0        0        0    16274 2023-04-12 21:21:11.000000 TapisCL-ICICLE-0.0.2/TapisCLICICLE/tapisObjectWrappers.py
+drwxrwxrwx   0        0        0        0 2023-04-12 21:32:36.538816 TapisCL-ICICLE-0.0.2/TapisCL_ICICLE.egg-info/
+-rw-rw-rw-   0        0        0    43023 2023-04-12 21:32:36.000000 TapisCL-ICICLE-0.0.2/TapisCL_ICICLE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      485 2023-04-12 21:32:36.000000 TapisCL-ICICLE-0.0.2/TapisCL_ICICLE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 21:32:36.000000 TapisCL-ICICLE-0.0.2/TapisCL_ICICLE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-04-12 21:32:36.000000 TapisCL-ICICLE-0.0.2/TapisCL_ICICLE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-12 21:32:36.000000 TapisCL-ICICLE-0.0.2/TapisCL_ICICLE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      982 2023-04-12 21:29:55.000000 TapisCL-ICICLE-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-12 21:32:36.540827 TapisCL-ICICLE-0.0.2/setup.cfg
```

### Comparing `TapisCL-ICICLE-0.0.1/LICENSE` & `TapisCL-ICICLE-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.1/PKG-INFO` & `TapisCL-ICICLE-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.1
+Version: 0.0.2
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <ahumanbeing189@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -674,26 +674,35 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
-Project-URL: Homepage, https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/ICICLE_Release_04_2023/CLI/TapisCL-ICICLE
+Project-URL: Homepage, https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_04_2023/CLI/TapisCL-ICICLE
 Keywords: Tapis,CLI,Agave,HPC,Tapis Pods,TACC
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # TapisCLI
+## Overview
 Tapis CLI is designed to provide a simple to use, versatile way to interface with Tapis services hosted on HPC resources. User can either start the app and use it as a traditional command line applications, or pass commands directly from bash.
 Allows you to work with all major Tapis services: Pods, Systems, Files, and Apps in one place. It can also interface directly with services being hosted on Tapis pods, like Neo4j. Although currently Neo4j is the only 3rd party application it can work with, adding support for Postgres and the like will not be difficult.
 
-## Operations
-1. to see a list of all commands and their parameters, just enter help
+### Dependencies
+* Dependencies are listed [here](https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/blob/main/icicle_rel_04_2023/CLI/TapisCL-ICICLE/requirements.txt)
 
-## Current bugs
-1. help menu does not list the arguments for server commands, most notably, switch_service. To run this, you must specify switch_service -n (service link)
+### Installation
+#### Using PyPi
+1. `pip install TapisCL-ICICLE`
+2. `python -m TapisCL-ICICLE`
+#### Running Python Code Directly
+1. Clone the repository to local machine.
+2. `python -m pip install -r requirements.txt`
+3. `python cli.py`
+### Operations
+1. to see a list of all commands and their parameters, just enter help
```

### Comparing `TapisCL-ICICLE-0.0.1/TapisCL_ICICLE.egg-info/PKG-INFO` & `TapisCL-ICICLE-0.0.2/TapisCL_ICICLE.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.1
+Version: 0.0.2
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <ahumanbeing189@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -674,26 +674,35 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
-Project-URL: Homepage, https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/ICICLE_Release_04_2023/CLI/TapisCL-ICICLE
+Project-URL: Homepage, https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_04_2023/CLI/TapisCL-ICICLE
 Keywords: Tapis,CLI,Agave,HPC,Tapis Pods,TACC
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # TapisCLI
+## Overview
 Tapis CLI is designed to provide a simple to use, versatile way to interface with Tapis services hosted on HPC resources. User can either start the app and use it as a traditional command line applications, or pass commands directly from bash.
 Allows you to work with all major Tapis services: Pods, Systems, Files, and Apps in one place. It can also interface directly with services being hosted on Tapis pods, like Neo4j. Although currently Neo4j is the only 3rd party application it can work with, adding support for Postgres and the like will not be difficult.
 
-## Operations
-1. to see a list of all commands and their parameters, just enter help
+### Dependencies
+* Dependencies are listed [here](https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/blob/main/icicle_rel_04_2023/CLI/TapisCL-ICICLE/requirements.txt)
 
-## Current bugs
-1. help menu does not list the arguments for server commands, most notably, switch_service. To run this, you must specify switch_service -n (service link)
+### Installation
+#### Using PyPi
+1. `pip install TapisCL-ICICLE`
+2. `python -m TapisCL-ICICLE`
+#### Running Python Code Directly
+1. Clone the repository to local machine.
+2. `python -m pip install -r requirements.txt`
+3. `python cli.py`
+### Operations
+1. to see a list of all commands and their parameters, just enter help
```

### Comparing `TapisCL-ICICLE-0.0.1/pyproject.toml` & `TapisCL-ICICLE-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,33 +2,32 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TapisCL-ICICLE"
-version = "0.0.1"
+version = "0.0.2"
 description = "Provide good performance command line user interface for Tapis services hosted on HPC clusters"
 readme = "README.md"
 authors = [{ name = "Michael Ray", email = "ahumanbeing189@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["Tapis", "CLI", "Agave", "HPC", "Tapis Pods", "TACC"]
 dependencies = [
     "pydantic",
-    "TypeEnforcement",
     "pyfiglet",
     "tapipy",
     "pyperclip",
     "py2neo"
 ]
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = []
 
 [project.urls]
-Homepage = "https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/ICICLE_Release_04_2023/CLI/TapisCL-ICICLE"
+Homepage = "https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_04_2023/CLI/TapisCL-ICICLE"
```

