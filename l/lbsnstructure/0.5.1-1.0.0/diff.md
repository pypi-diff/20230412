# Comparing `tmp/lbsnstructure-0.5.1.tar.gz` & `tmp/lbsnstructure-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lbsnstructure-0.5.1.tar", last modified: Mon Feb  3 13:08:19 2020, max compression
+gzip compressed data, was "lbsnstructure-1.0.0.tar", last modified: Wed Apr 12 11:43:02 2023, max compression
```

## Comparing `lbsnstructure-0.5.1.tar` & `lbsnstructure-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,28 @@
-drwxrwxrwx   0 alex      (1000) alex      (1000)        0 2020-02-03 13:08:19.000000 lbsnstructure-0.5.1/
--rw-rw-rw-   0 alex      (1000) alex      (1000)     3403 2020-02-03 13:08:19.000000 lbsnstructure-0.5.1/PKG-INFO
--rwxrwxrwx   0 alex      (1000) alex      (1000)     2655 2019-10-21 11:34:47.000000 lbsnstructure-0.5.1/README.md
-drwxrwxrwx   0 alex      (1000) alex      (1000)        0 2020-02-03 13:08:19.000000 lbsnstructure-0.5.1/lbsnstructure/
--rw-rw-rw-   0 alex      (1000) alex      (1000)        0 2019-07-11 09:18:07.000000 lbsnstructure-0.5.1/lbsnstructure/__init__.py
--rw-rw-rw-   0 alex      (1000) alex      (1000)    77609 2020-01-09 08:42:59.000000 lbsnstructure-0.5.1/lbsnstructure/lbsnstructure_pb2.py
--rwxrwxrwx   0 alex      (1000) alex      (1000)       22 2020-02-03 13:08:10.000000 lbsnstructure-0.5.1/lbsnstructure/version.py
-drwxrwxrwx   0 alex      (1000) alex      (1000)        0 2020-02-03 13:08:19.000000 lbsnstructure-0.5.1/lbsnstructure.egg-info/
--rw-rw-rw-   0 alex      (1000) alex      (1000)     3403 2020-02-03 13:08:18.000000 lbsnstructure-0.5.1/lbsnstructure.egg-info/PKG-INFO
--rw-rw-rw-   0 alex      (1000) alex      (1000)      334 2020-02-03 13:08:18.000000 lbsnstructure-0.5.1/lbsnstructure.egg-info/SOURCES.txt
--rw-rw-rw-   0 alex      (1000) alex      (1000)        1 2020-02-03 13:08:18.000000 lbsnstructure-0.5.1/lbsnstructure.egg-info/dependency_links.txt
--rw-rw-rw-   0 alex      (1000) alex      (1000)        1 2019-07-11 11:04:14.000000 lbsnstructure-0.5.1/lbsnstructure.egg-info/not-zip-safe
--rw-rw-rw-   0 alex      (1000) alex      (1000)        9 2020-02-03 13:08:18.000000 lbsnstructure-0.5.1/lbsnstructure.egg-info/requires.txt
--rw-rw-rw-   0 alex      (1000) alex      (1000)       14 2020-02-03 13:08:18.000000 lbsnstructure-0.5.1/lbsnstructure.egg-info/top_level.txt
--rw-rw-rw-   0 alex      (1000) alex      (1000)      114 2020-02-03 13:08:19.000000 lbsnstructure-0.5.1/setup.cfg
--rw-rw-rw-   0 alex      (1000) alex      (1000)      909 2019-07-11 09:18:07.000000 lbsnstructure-0.5.1/setup.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-04-12 11:43:02.123729 lbsnstructure-1.0.0/
+-rw-rw-rw-   0 alex      (1000) alex      (1000)     1227 2019-07-11 09:18:07.000000 lbsnstructure-1.0.0/.gitignore
+-rwxrwxrwx   0 alex      (1000) alex      (1000)     1553 2020-02-28 07:54:54.000000 lbsnstructure-1.0.0/.gitlab-ci.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      409 2023-04-12 11:42:52.000000 lbsnstructure-1.0.0/CHANGELOG.md
+-rw-rw-rw-   0 alex      (1000) alex      (1000)     1121 2019-07-11 10:53:20.000000 lbsnstructure-1.0.0/LICENSE.md
+-rw-r--r--   0 alex      (1000) alex      (1000)     2993 2023-04-12 11:43:02.124728 lbsnstructure-1.0.0/PKG-INFO
+-rwxrwxrwx   0 alex      (1000) alex      (1000)     2655 2019-10-21 11:34:47.000000 lbsnstructure-1.0.0/README.md
+-rw-rw-rw-   0 alex      (1000) alex      (1000)     4124 2019-07-11 09:18:07.000000 lbsnstructure-1.0.0/StructureTest.ipynb
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-04-12 11:43:01.943079 lbsnstructure-1.0.0/google/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-04-12 11:43:01.996643 lbsnstructure-1.0.0/google/protobuf/
+-rw-rw-rw-   0 alex      (1000) alex      (1000)     2754 2019-07-11 10:53:20.000000 lbsnstructure-1.0.0/google/protobuf/timestamp_pb2.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-04-12 11:43:02.103892 lbsnstructure-1.0.0/lbsnstructure/
+-rw-rw-rw-   0 alex      (1000) alex      (1000)        0 2019-07-11 09:18:07.000000 lbsnstructure-1.0.0/lbsnstructure/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     7923 2023-04-12 11:33:49.000000 lbsnstructure-1.0.0/lbsnstructure/interlinkage_pb2.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    27308 2023-04-12 11:29:54.000000 lbsnstructure-1.0.0/lbsnstructure/social_pb2.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    20143 2023-04-12 11:35:11.000000 lbsnstructure-1.0.0/lbsnstructure/spatial_pb2.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    12612 2023-04-12 11:35:33.000000 lbsnstructure-1.0.0/lbsnstructure/temporal_pb2.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    26683 2023-04-12 11:35:46.000000 lbsnstructure-1.0.0/lbsnstructure/topical_pb2.py
+-rwxrwxrwx   0 alex      (1000) alex      (1000)       22 2023-04-12 11:42:52.000000 lbsnstructure-1.0.0/lbsnstructure/version.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-04-12 11:43:02.121729 lbsnstructure-1.0.0/lbsnstructure.egg-info/
+-rw-rw-rw-   0 alex      (1000) alex      (1000)     2993 2023-04-12 11:42:59.000000 lbsnstructure-1.0.0/lbsnstructure.egg-info/PKG-INFO
+-rw-rw-rw-   0 alex      (1000) alex      (1000)      552 2023-04-12 11:42:59.000000 lbsnstructure-1.0.0/lbsnstructure.egg-info/SOURCES.txt
+-rw-rw-rw-   0 alex      (1000) alex      (1000)        1 2023-04-12 11:42:59.000000 lbsnstructure-1.0.0/lbsnstructure.egg-info/dependency_links.txt
+-rw-rw-rw-   0 alex      (1000) alex      (1000)        1 2019-07-11 11:04:14.000000 lbsnstructure-1.0.0/lbsnstructure.egg-info/not-zip-safe
+-rw-rw-rw-   0 alex      (1000) alex      (1000)        9 2023-04-12 11:42:59.000000 lbsnstructure-1.0.0/lbsnstructure.egg-info/requires.txt
+-rw-rw-rw-   0 alex      (1000) alex      (1000)       14 2023-04-12 11:42:59.000000 lbsnstructure-1.0.0/lbsnstructure.egg-info/top_level.txt
+-rw-rw-rw-   0 alex      (1000) alex      (1000)      114 2023-04-12 11:43:02.126885 lbsnstructure-1.0.0/setup.cfg
+-rw-rw-rw-   0 alex      (1000) alex      (1000)      909 2019-07-11 09:18:07.000000 lbsnstructure-1.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `lbsnstructure-0.5.1/PKG-INFO` & `lbsnstructure-1.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,67 @@
 Metadata-Version: 2.1
 Name: lbsnstructure
-Version: 0.5.1
+Version: 1.0.0
 Summary: A common language independent and cross-network social-media data scheme.
 Home-page: https://gitlab.vgiscience.de/lbsn/concept
 Author: Filip Krumpe; Alexander Dunkel; Marc Löchner
 Author-email: alexander.dunkel@tu-dresden.de
 License: MIT
-Description: ![pypi version](https://lbsn.vgiscience.org/structure/python/pypi.svg) ![pipeline](https://lbsn.vgiscience.org/structure/python/pipeline.svg)
-        
-        # LBSNSTRUCTURE
-        
-        A python compiled version of the [common location based social network (LBSN) data structure concept](https://gitlab.vgiscience.de/lbsn/concept) (ProtoBuf) to handle cross network Social Media data in Python.
-        There are several motivations for prividing a common LBSN interchange data structure. Firstly, the [GDPR](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32016R0679) directly requests Social Media Network operators to allow users to transfer accounts and data inbetween services. 
-        While there are attempts by Google, Facebook etc. (see [data-transfer-project](https://github.com/google/data-transfer-project)), it is not currently possible. With this structure concept, we follow an independent road.
-        A primary goal is to systematically characterize LBSN data aspects in a common scheme that enables privacy-by-design for connected software, transfer scripts and database design.
-        
-        ## Quick Start
-        
-        Install with:  
-        ```shell
-        pip install --upgrade lbsnstructure
-        ```
-        
-        Import to python projecty with:  
-        ```python
-        import lbsnstructure
-        from lbsnstructure.lbsnstructure_pb2 import lbsnPost
-        ```
-        
-        .. or compile newest version from [Protofiles](https://gitlab.vgiscience.de/lbsn/concept)
-        
-        1. Clone git Repository `git clone git@gitlab.vgiscience.de/lbsn/concept`
-        2. Install [Protocoll Buffers](https://github.com/google/protobuf/releases)
-        3. Compile structure to python package `protoc --python_out=examples/python lbsnstructure/structure.proto`  
-        4. Install with `pip install .` in examples/python
-        
-        ## Developers
-        
-        For development & testing, make a local clone of this repository  
-        ```shell
-        git clone git@gitlab.vgiscience.de:lbsn/concept.git
-        ```
-        
-        Go to subfolder `examples\python` and (e.g.) symlink the folder to your  
-        Python's site-packages folder with:  
-        ```shell
-        python setup.py develop
-        ```
-        
-        Now, lbsnstructure should be available through your python path and directly link to the local git clone directory.
-        
-        ## Versioning
-        
-        For the releases available, see the [tags on this repository](/../tags). 
-        The versioning (major.minor.patch) is automated using [python-semantic-release](https://github.com/relekang/python-semantic-release).
-        Commit messages that follow the [Angular Commit Message Conventions](https://github.com/angular/angular.js/blob/master/DEVELOPERS.md#-git-commit-guidelines) will be automatically interpreted, 
-        followed by version bumps if necessary. 
-        
-        ## License
-        
-        This project is licensed under the  MIT License.
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+![pypi version](https://lbsn.vgiscience.org/structure/python/pypi.svg) ![pipeline](https://lbsn.vgiscience.org/structure/python/pipeline.svg)
+
+# LBSNSTRUCTURE
+
+A python compiled version of the [common location based social network (LBSN) data structure concept](https://gitlab.vgiscience.de/lbsn/concept) (ProtoBuf) to handle cross network Social Media data in Python.
+There are several motivations for prividing a common LBSN interchange data structure. Firstly, the [GDPR](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32016R0679) directly requests Social Media Network operators to allow users to transfer accounts and data inbetween services. 
+While there are attempts by Google, Facebook etc. (see [data-transfer-project](https://github.com/google/data-transfer-project)), it is not currently possible. With this structure concept, we follow an independent road.
+A primary goal is to systematically characterize LBSN data aspects in a common scheme that enables privacy-by-design for connected software, transfer scripts and database design.
+
+## Quick Start
+
+Install with:  
+```shell
+pip install --upgrade lbsnstructure
+```
+
+Import to python projecty with:  
+```python
+import lbsnstructure
+from lbsnstructure.lbsnstructure_pb2 import lbsnPost
+```
+
+.. or compile newest version from [Protofiles](https://gitlab.vgiscience.de/lbsn/concept)
+
+1. Clone git Repository `git clone git@gitlab.vgiscience.de/lbsn/concept`
+2. Install [Protocoll Buffers](https://github.com/google/protobuf/releases)
+3. Compile structure to python package `protoc --python_out=examples/python lbsnstructure/structure.proto`  
+4. Install with `pip install .` in examples/python
+
+## Developers
+
+For development & testing, make a local clone of this repository  
+```shell
+git clone git@gitlab.vgiscience.de:lbsn/concept.git
+```
+
+Go to subfolder `examples\python` and (e.g.) symlink the folder to your  
+Python's site-packages folder with:  
+```shell
+python setup.py develop
+```
+
+Now, lbsnstructure should be available through your python path and directly link to the local git clone directory.
+
+## Versioning
+
+For the releases available, see the [tags on this repository](/../tags). 
+The versioning (major.minor.patch) is automated using [python-semantic-release](https://github.com/relekang/python-semantic-release).
+Commit messages that follow the [Angular Commit Message Conventions](https://github.com/angular/angular.js/blob/master/DEVELOPERS.md#-git-commit-guidelines) will be automatically interpreted, 
+followed by version bumps if necessary. 
+
+## License
+
+This project is licensed under the  MIT License.
+
```

### Comparing `lbsnstructure-0.5.1/README.md` & `lbsnstructure-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `lbsnstructure-0.5.1/lbsnstructure.egg-info/PKG-INFO` & `lbsnstructure-1.0.0/lbsnstructure.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,67 @@
 Metadata-Version: 2.1
 Name: lbsnstructure
-Version: 0.5.1
+Version: 1.0.0
 Summary: A common language independent and cross-network social-media data scheme.
 Home-page: https://gitlab.vgiscience.de/lbsn/concept
 Author: Filip Krumpe; Alexander Dunkel; Marc Löchner
 Author-email: alexander.dunkel@tu-dresden.de
 License: MIT
-Description: ![pypi version](https://lbsn.vgiscience.org/structure/python/pypi.svg) ![pipeline](https://lbsn.vgiscience.org/structure/python/pipeline.svg)
-        
-        # LBSNSTRUCTURE
-        
-        A python compiled version of the [common location based social network (LBSN) data structure concept](https://gitlab.vgiscience.de/lbsn/concept) (ProtoBuf) to handle cross network Social Media data in Python.
-        There are several motivations for prividing a common LBSN interchange data structure. Firstly, the [GDPR](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32016R0679) directly requests Social Media Network operators to allow users to transfer accounts and data inbetween services. 
-        While there are attempts by Google, Facebook etc. (see [data-transfer-project](https://github.com/google/data-transfer-project)), it is not currently possible. With this structure concept, we follow an independent road.
-        A primary goal is to systematically characterize LBSN data aspects in a common scheme that enables privacy-by-design for connected software, transfer scripts and database design.
-        
-        ## Quick Start
-        
-        Install with:  
-        ```shell
-        pip install --upgrade lbsnstructure
-        ```
-        
-        Import to python projecty with:  
-        ```python
-        import lbsnstructure
-        from lbsnstructure.lbsnstructure_pb2 import lbsnPost
-        ```
-        
-        .. or compile newest version from [Protofiles](https://gitlab.vgiscience.de/lbsn/concept)
-        
-        1. Clone git Repository `git clone git@gitlab.vgiscience.de/lbsn/concept`
-        2. Install [Protocoll Buffers](https://github.com/google/protobuf/releases)
-        3. Compile structure to python package `protoc --python_out=examples/python lbsnstructure/structure.proto`  
-        4. Install with `pip install .` in examples/python
-        
-        ## Developers
-        
-        For development & testing, make a local clone of this repository  
-        ```shell
-        git clone git@gitlab.vgiscience.de:lbsn/concept.git
-        ```
-        
-        Go to subfolder `examples\python` and (e.g.) symlink the folder to your  
-        Python's site-packages folder with:  
-        ```shell
-        python setup.py develop
-        ```
-        
-        Now, lbsnstructure should be available through your python path and directly link to the local git clone directory.
-        
-        ## Versioning
-        
-        For the releases available, see the [tags on this repository](/../tags). 
-        The versioning (major.minor.patch) is automated using [python-semantic-release](https://github.com/relekang/python-semantic-release).
-        Commit messages that follow the [Angular Commit Message Conventions](https://github.com/angular/angular.js/blob/master/DEVELOPERS.md#-git-commit-guidelines) will be automatically interpreted, 
-        followed by version bumps if necessary. 
-        
-        ## License
-        
-        This project is licensed under the  MIT License.
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+![pypi version](https://lbsn.vgiscience.org/structure/python/pypi.svg) ![pipeline](https://lbsn.vgiscience.org/structure/python/pipeline.svg)
+
+# LBSNSTRUCTURE
+
+A python compiled version of the [common location based social network (LBSN) data structure concept](https://gitlab.vgiscience.de/lbsn/concept) (ProtoBuf) to handle cross network Social Media data in Python.
+There are several motivations for prividing a common LBSN interchange data structure. Firstly, the [GDPR](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32016R0679) directly requests Social Media Network operators to allow users to transfer accounts and data inbetween services. 
+While there are attempts by Google, Facebook etc. (see [data-transfer-project](https://github.com/google/data-transfer-project)), it is not currently possible. With this structure concept, we follow an independent road.
+A primary goal is to systematically characterize LBSN data aspects in a common scheme that enables privacy-by-design for connected software, transfer scripts and database design.
+
+## Quick Start
+
+Install with:  
+```shell
+pip install --upgrade lbsnstructure
+```
+
+Import to python projecty with:  
+```python
+import lbsnstructure
+from lbsnstructure.lbsnstructure_pb2 import lbsnPost
+```
+
+.. or compile newest version from [Protofiles](https://gitlab.vgiscience.de/lbsn/concept)
+
+1. Clone git Repository `git clone git@gitlab.vgiscience.de/lbsn/concept`
+2. Install [Protocoll Buffers](https://github.com/google/protobuf/releases)
+3. Compile structure to python package `protoc --python_out=examples/python lbsnstructure/structure.proto`  
+4. Install with `pip install .` in examples/python
+
+## Developers
+
+For development & testing, make a local clone of this repository  
+```shell
+git clone git@gitlab.vgiscience.de:lbsn/concept.git
+```
+
+Go to subfolder `examples\python` and (e.g.) symlink the folder to your  
+Python's site-packages folder with:  
+```shell
+python setup.py develop
+```
+
+Now, lbsnstructure should be available through your python path and directly link to the local git clone directory.
+
+## Versioning
+
+For the releases available, see the [tags on this repository](/../tags). 
+The versioning (major.minor.patch) is automated using [python-semantic-release](https://github.com/relekang/python-semantic-release).
+Commit messages that follow the [Angular Commit Message Conventions](https://github.com/angular/angular.js/blob/master/DEVELOPERS.md#-git-commit-guidelines) will be automatically interpreted, 
+followed by version bumps if necessary. 
+
+## License
+
+This project is licensed under the  MIT License.
+
```

### Comparing `lbsnstructure-0.5.1/setup.py` & `lbsnstructure-1.0.0/setup.py`

 * *Files identical despite different names*

