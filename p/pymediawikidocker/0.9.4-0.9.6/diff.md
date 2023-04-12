# Comparing `tmp/pymediawikidocker-0.9.4.tar.gz` & `tmp/pymediawikidocker-0.9.6.tar.gz`

## Comparing `pymediawikidocker-0.9.4.tar` & `pymediawikidocker-0.9.6.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/.project
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/.pydevproject
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/.github/workflows/build.yml
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/.github/workflows/upload-to-pypi.yml
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/.DS_Store
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/__init__.py
--rw-r--r--   0        0        0     9834 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/config.py
--rw-r--r--   0        0        0    23246 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/docker.py
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/html_table.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/logger.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/mariadb.py
--rw-r--r--   0        0        0     7225 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/mw.py
--rw-r--r--   0        0        0     8471 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/mwcluster.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/version.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/webscrape.py
--rw-r--r--   0        0        0    11593 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/extensions.json
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/addCronTabEntry.sh
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/addSysopUser.sh
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/initdb.sh
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/installExtensions.sh
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/mwCompose.yml
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/mwDockerfile
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/mwLocalSettings.php
--rw-r--r--   0        0        0     4196 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/mwLocalSettings127.php
--rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/mwLocalSettings131.php
--rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/mwLocalSettings135.php
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/mwLocalSettings136.php
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/mwLocalSettings137.php
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/mwLocalSettings138.php
--rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/mwLocalSettings139.php
--rw-r--r--   0        0        0    56849 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/mwWiki127.sql
--rw-r--r--   0        0        0    66990 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/mwWiki131.sql
--rw-r--r--   0        0        0    64022 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/mwWiki135.sql
--rw-r--r--   0        0        0    63586 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/mwWiki136.sql
--rw-r--r--   0        0        0    63586 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/mwWiki137.sql
--rw-r--r--   0        0        0    66990 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/mwWiki138.sql
--rw-r--r--   0        0        0    64483 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/mwWiki139.sql
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/phpinfo.php
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/plantuml.sh
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/startRunJobs.sh
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/update.sh
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/mwdocker/resources/templates/upload.ini
--rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/scripts/install
--rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/scripts/test
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/tests/__init__.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/tests/basetest.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/tests/test_config.py
--rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/tests/test_extensions.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/tests/test_html_tables.py
--rw-r--r--   0        0        0    10738 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/tests/test_install.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/LICENSE
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/README.md
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/pyproject.toml
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/.project
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/.pydevproject
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/.github/workflows/build.yml
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/.github/workflows/upload-to-pypi.yml
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/.DS_Store
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/__init__.py
+-rw-r--r--   0        0        0    10648 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/config.py
+-rw-r--r--   0        0        0    23202 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/docker.py
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/html_table.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/logger.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/mariadb.py
+-rw-r--r--   0        0        0     7225 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/mw.py
+-rw-r--r--   0        0        0     8349 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/mwcluster.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/version.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/webscrape.py
+-rw-r--r--   0        0        0    11766 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/extensions.json
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/addCronTabEntry.sh
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/addSysopUser.sh
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/initdb.sh
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/installExtensions.sh
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/mwCompose.yml
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/mwDockerfile
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/mwLocalSettings.php
+-rw-r--r--   0        0        0     4196 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/mwLocalSettings127.php
+-rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/mwLocalSettings131.php
+-rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/mwLocalSettings135.php
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/mwLocalSettings136.php
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/mwLocalSettings137.php
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/mwLocalSettings138.php
+-rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/mwLocalSettings139.php
+-rw-r--r--   0        0        0    56849 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/mwWiki127.sql
+-rw-r--r--   0        0        0    66990 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/mwWiki131.sql
+-rw-r--r--   0        0        0    64022 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/mwWiki135.sql
+-rw-r--r--   0        0        0    63586 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/mwWiki136.sql
+-rw-r--r--   0        0        0    63586 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/mwWiki137.sql
+-rw-r--r--   0        0        0    66990 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/mwWiki138.sql
+-rw-r--r--   0        0        0    64483 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/mwWiki139.sql
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/phpinfo.php
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/plantuml.sh
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/startRunJobs.sh
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/update.sh
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/mwdocker/resources/templates/upload.ini
+-rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/scripts/install
+-rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/scripts/test
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/tests/__init__.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/tests/basetest.py
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/tests/test_config.py
+-rw-r--r--   0        0        0     4315 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/tests/test_extensions.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/tests/test_html_tables.py
+-rw-r--r--   0        0        0    11093 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/tests/test_install.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/LICENSE
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/README.md
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.6/PKG-INFO
```

### Comparing `pymediawikidocker-0.9.4/.github/workflows/build.yml` & `pymediawikidocker-0.9.6/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.4/.github/workflows/upload-to-pypi.yml` & `pymediawikidocker-0.9.6/.github/workflows/upload-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.4/mwdocker/.DS_Store` & `pymediawikidocker-0.9.6/mwdocker/.DS_Store`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.4/mwdocker/config.py` & `pymediawikidocker-0.9.6/mwdocker/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 '''
 Created on 2023-04-06
 
 @author: wf
 '''
 import dataclasses
 from dataclasses import dataclass, field
+from pathlib import Path
+import json
 import re
 import secrets
 import socket
 from typing import Optional, List
 from mwdocker.mw import ExtensionList
 
 class Host:
@@ -54,24 +56,32 @@
     container_base_name:str=None  
     networkName:str="mwNetwork"
     mariaDBVersion:str="10.11"
     forceRebuild:bool=False
     debug:bool=False
     verbose:bool=True
     wikiId:str=None
+    dockerPath:str=None
+    
+    def default_docker_path(self)->str:
+        home = str(Path.home())
+        docker_path=f'{home}/.pymediawikidocker' 
+        return docker_path
     
     def __post_init__(self):
         """
         post initialization configuration
         """
         self.fullVersion=f"MediaWiki {self.version}"
         self.underscoreVersion=self.version.replace(".","_")
         self.shortVersion=self.getShortVersion()
         self.base_url=f"{self.prot}://{self.host}"
         self.url=f"{self.base_url}{self.script_path}:{self.port}"
+        if not self.dockerPath:
+            self.dockerPath=self.default_docker_path()
         if not self.container_base_name:
             self.container_base_name=f"{self.prefix}-{self.shortVersion}"
           
     def reset_container_base_name(self,container_base_name:str=None):
         self.container_base_name=container_base_name
         self.__post_init__()
           
@@ -81,14 +91,25 @@
         dataclasses to dict conversion convenienc and information hiding
         
         Returns:
             dict: my fields in dict format
         """
         config_dict=dataclasses.asdict(self)
         return config_dict
+    
+    def as_json(self)->str:
+        """
+        return me as a json string
+        
+        Returns:
+            str: my json representation
+        """
+        config_dict=self.as_dict()
+        json_str=json.dumps(config_dict,indent=2)
+        return json_str
         
     def getShortVersion(self,separator=""):
         '''
         get my short version e.g. convert 1.27.7 to 127
         
         Returns:
             str: the short version string
@@ -161,14 +182,15 @@
         initialize me from the given commmand line arguments
         
         Args:
             args(Namespace): the command line arguments
         """
         self.prefix=args.prefix
         self.container_base_name=args.container_name
+        self.dockerPath=args.dockerPath
         self.extensionNameList=args.extensionNameList
         self.extensionJsonFile=args.extensionJsonFile
         self.forceRebuild=args.forceRebuild
         self.host=args.host
         self.logo=args.logo
         self.mariaDBVersion=args.mariaDBVersion
         # passwords
@@ -195,14 +217,16 @@
         parser.add_argument('-cn','--container_name',default=self.container_base_name,help="set container name (only valid and recommended for single version call)")
         parser.add_argument("-d", "--debug", dest="debug",   action="store_true", help="enable debug mode [default: %(default)s]")
         parser.add_argument('-el', '--extensionList', dest='extensionNameList', nargs="*",default=self.extensionNameList,help="list of extensions to be installed [default: %(default)s]")
         parser.add_argument('-ej', '--extensionJson',dest='extensionJsonFile',default=self.extensionJsonFile,help="additional extension descriptions default: [default: %(default)s]")
         parser.add_argument("-f", "--forceRebuild", action="store_true", help="force rebuilding  [default: %(default)s]")
         parser.add_argument("--host", default=Host.get_default_host(),
                             help="the host to serve / listen from [default: %(default)s]")
+        parser.add_argument("-dp","--dockerPath", default=self.default_docker_path(),
+                            help="the base directory to store docker and jinja template files [default: %(default)s]")
         parser.add_argument("--logo", default=self.logo, help="set Logo [default: %(default)s]")
         parser.add_argument('-mv', '--mariaDBVersion', dest='mariaDBVersion',default=self.mariaDBVersion,help="mariaDB Version to be installed [default: %(default)s]")
         parser.add_argument('--mysqlPassword',default=self.mySQLRootPassword, help="set sqlRootPassword [default: %(default)s] - random password if None")
         parser.add_argument('-p','--password',dest='password',default=self.password, help="set password for initial user [default: %(default)s] ")
         parser.add_argument('-pl','--passwordLength',default=self.password_length, help="set the password length for random passwords[default: %(default)s] ")
         parser.add_argument("--prefix",default=self.prefix,help="the container name prefix to use [default: %(default)s]")
         parser.add_argument("--prot",default=self.prot,help="change to https in case [default: %(default)s]")
```

### Comparing `pymediawikidocker-0.9.4/mwdocker/docker.py` & `pymediawikidocker-0.9.6/mwdocker/docker.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,16 +100,15 @@
         
 class DockerApplication(object):
     '''
     MediaWiki Docker image
     '''
 
     def __init__(self,
-                 config:MwClusterConfig,
-                 home:str=None):
+                 config:MwClusterConfig):
         '''
         Constructor
         
         Args:
             config: MwClusterConfig,
             home: the home directory to use
         '''
@@ -117,17 +116,16 @@
         # branch as need for git clone e.g. https://gerrit.wikimedia.org/g/mediawiki/extensions/MagicNoCache
         self.branch=f"REL{self.config.getShortVersion('_')}"
         self.composerVersion=1
         if self.config.shortVersion>="139":
             self.composerVersion=2
         # jinja and docker prerequisites
         self.env=self.getJinjaEnv()
-        if home is None:
-            home = str(Path.home())
-        self.dockerPath=f'{home}/.pymediawikidocker/{self.config.container_base_name}' 
+        # docker file location
+        self.dockerPath=f'{self.config.dockerPath}/{self.config.container_base_name}' 
         os.makedirs(self.dockerPath,exist_ok=True)
         
         self.getContainers()
         self.dbConn=None
         self.database="wiki"
         self.dbUser="wikiuser"
         self.wikiUser=None
@@ -284,15 +282,15 @@
         Args:
            store(bool): if True save my user data to the relevant ini File
         '''
         if not wikiId:
             wikiId=f"{self.config.container_base_name}"
         userDict={
             "wikiId":f"{wikiId}",
-            "url": f"{self.config.base_url}",
+            "url": f"{self.config.base_url}:{self.config.port}",
             "scriptPath": f"{self.config.script_path}",
             "user": f"{self.config.user}",
             "email":"noreply@nouser.com",
             "version": f"{self.config.fullVersion}",
             "password": f"{self.config.password}"
         }
         wikiUser=WikiUser.ofDict(userDict,encrypted=False)
```

### Comparing `pymediawikidocker-0.9.4/mwdocker/html_table.py` & `pymediawikidocker-0.9.6/mwdocker/html_table.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.4/mwdocker/logger.py` & `pymediawikidocker-0.9.6/mwdocker/logger.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.4/mwdocker/mariadb.py` & `pymediawikidocker-0.9.6/mwdocker/mariadb.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.4/mwdocker/mw.py` & `pymediawikidocker-0.9.6/mwdocker/mw.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.4/mwdocker/mwcluster.py` & `pymediawikidocker-0.9.6/mwdocker/mwcluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,28 +29,27 @@
         
         Args:
             config(MWClusterConfig): the MediaWiki Cluster Configuration to use
         '''
         self.config=config
         self.apps={}       
   
-    def createApps(self,home:str=None,withGenerate:bool=True)->dict:
+    def createApps(self,withGenerate:bool=True)->dict:
         '''
         create my apps
         
         Args:
-            home(str): the home path to use for the docker configuration files
             withGenerate(bool): if True generate the config files
             
         Returns:
             dict(str): a dict of apps by version
         '''  
         app_count=len(self.config.versions)
         for i,version in enumerate(self.config.versions):
-            mwApp=self.getDockerApplication(i,app_count,version,home)
+            mwApp=self.getDockerApplication(i,app_count,version)
             if withGenerate:
                 mwApp.generateAll(overwrite=self.config.forceRebuild)
             self.apps[version]=mwApp    
         return self.apps
         
     def checkDocker(self)->int: 
         """
@@ -131,15 +130,15 @@
     def close(self):
         """
         close my apps
         """
         for mwApp in self.apps.values():
             mwApp.close()
             
-    def getDockerApplication(self,i:int,count:int,version:str,home:str=None):
+    def getDockerApplication(self,i:int,count:int,version:str):
         '''
         get the docker application for the given version index and version
         
         Args:
             i(int): the index of the version
             count(int): total number of Docker applications in this cluster
             version(str): the mediawiki version to use
@@ -155,15 +154,15 @@
         appConfig.version=version
         appConfig.port=self.config.basePort+i
         appConfig.sqlPort=self.config.sqlPort+i   
         # let post_init create a new container_base_name
         if count>1:
             appConfig.container_base_name=None
         appConfig.__post_init__()            
-        mwApp=DockerApplication(config=appConfig,home=home)
+        mwApp=DockerApplication(config=appConfig)
         return mwApp
 
 DEBUG=False
 
 def main(argv=None): # IGNORE:C0111
     '''main program.'''
```

### Comparing `pymediawikidocker-0.9.4/mwdocker/version.py` & `pymediawikidocker-0.9.6/mwdocker/version.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.4/mwdocker/webscrape.py` & `pymediawikidocker-0.9.6/mwdocker/webscrape.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.4/mwdocker/resources/extensions.json` & `pymediawikidocker-0.9.6/mwdocker/resources/extensions.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9861111111111112%*

 * *Differences: {"'extensions'": "{insert: [(10, OrderedDict([('name', 'ImageLink'), ('extension', 'ImageLink'), "*

 * *                 "('giturl', 'https://github.com/BITPlan/ImageLink'), ('url', "*

 * *                 "'https://wiki.bitplan.com/index.php/ImageLink')]))]}"}*

```diff
@@ -76,14 +76,20 @@
             "name": "Header Tabs",
             "purpose": "The Header Tabs extension transforms top-level MediaWiki headers into tabs using the jQuery UI JavaScript library.",
             "require_once_until": "127",
             "since": "2008-03-20T00:00:00",
             "url": "https://www.mediawiki.org/wiki/Extension:Header_Tabs"
         },
         {
+            "extension": "ImageLink",
+            "giturl": "https://github.com/BITPlan/ImageLink",
+            "name": "ImageLink",
+            "url": "https://wiki.bitplan.com/index.php/ImageLink"
+        },
+        {
             "extension": "ImageMap",
             "giturl": "https://github.com/wikimedia/mediawiki-extensions-ImageMap",
             "localSettings": "$wgEnableUploads = true;\r\n$wgUseImageMagick = true;\r\n$wgImageMagickConvertCommand = \"/usr/bin/convert\";",
             "name": "ImageMap",
             "url": "https://www.mediawiki.org/wiki/Extension:ImageMap"
         },
         {
```

### Comparing `pymediawikidocker-0.9.4/mwdocker/resources/templates/mwCompose.yml` & `pymediawikidocker-0.9.6/mwdocker/resources/templates/mwCompose.yml`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.4/mwdocker/resources/templates/mwDockerfile` & `pymediawikidocker-0.9.6/mwdocker/resources/templates/mwDockerfile`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.4/mwdocker/resources/templates/mwLocalSettings.php` & `pymediawikidocker-0.9.6/mwdocker/resources/templates/mwLocalSettings.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.4/mwdocker/resources/templates/mwLocalSettings127.php` & `pymediawikidocker-0.9.6/mwdocker/resources/templates/mwLocalSettings127.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.4/mwdocker/resources/templates/mwLocalSettings131.php` & `pymediawikidocker-0.9.6/mwdocker/resources/templates/mwLocalSettings131.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.4/mwdocker/resources/templates/mwLocalSettings135.php` & `pymediawikidocker-0.9.6/mwdocker/resources/templates/mwLocalSettings135.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.4/mwdocker/resources/templates/mwLocalSettings136.php` & `pymediawikidocker-0.9.6/mwdocker/resources/templates/mwLocalSettings136.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.4/mwdocker/resources/templates/mwLocalSettings137.php` & `pymediawikidocker-0.9.6/mwdocker/resources/templates/mwLocalSettings137.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.4/mwdocker/resources/templates/mwLocalSettings138.php` & `pymediawikidocker-0.9.6/mwdocker/resources/templates/mwLocalSettings138.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.4/mwdocker/resources/templates/mwLocalSettings139.php` & `pymediawikidocker-0.9.6/mwdocker/resources/templates/mwLocalSettings139.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.4/mwdocker/resources/templates/mwWiki127.sql` & `pymediawikidocker-0.9.6/mwdocker/resources/templates/mwWiki127.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.4/mwdocker/resources/templates/mwWiki131.sql` & `pymediawikidocker-0.9.6/mwdocker/resources/templates/mwWiki131.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.4/mwdocker/resources/templates/mwWiki135.sql` & `pymediawikidocker-0.9.6/mwdocker/resources/templates/mwWiki135.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.4/mwdocker/resources/templates/mwWiki136.sql` & `pymediawikidocker-0.9.6/mwdocker/resources/templates/mwWiki136.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.4/mwdocker/resources/templates/mwWiki137.sql` & `pymediawikidocker-0.9.6/mwdocker/resources/templates/mwWiki137.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.4/mwdocker/resources/templates/mwWiki138.sql` & `pymediawikidocker-0.9.6/mwdocker/resources/templates/mwWiki138.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.4/mwdocker/resources/templates/mwWiki139.sql` & `pymediawikidocker-0.9.6/mwdocker/resources/templates/mwWiki139.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.4/mwdocker/resources/templates/plantuml.sh` & `pymediawikidocker-0.9.6/mwdocker/resources/templates/plantuml.sh`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.4/tests/basetest.py` & `pymediawikidocker-0.9.6/tests/basetest.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.4/tests/test_config.py` & `pymediawikidocker-0.9.6/tests/test_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 @author: wf
 '''
 from tests.basetest import Basetest
 from mwdocker.config import MwClusterConfig, Host
 import json
 from argparse import ArgumentParser
-import dataclasses
 
 class TestConfig(Basetest):
     '''
     test the Mediawiki Cluster configuration
     '''
     
     def testDefaults(self):
@@ -22,15 +21,17 @@
         expected={'version': '1.39.3', 'smwVersion': None, 
                   'extensionNameList': ['Admin Links', 'Header Tabs', 'SyntaxHighlight', 'Variables'], 
                   'extensionJsonFile': None, 'user': 'Sysop', 'prefix': 'mw', 
                   'password_length': 15, 'password': 'sysop-1234!', 
                   'mySQLRootPassword': None, 'mySQLPassword': None, 
                   'logo': '$wgResourceBasePath/resources/assets/wiki.png',
                    'port': 9080, 'sqlPort': 9306, 'prot': 'http', 
-                   'host': Host.get_default_host(), 'script_path': '', 'container_base_name': 'mw-139', 'networkName': 'mwNetwork', 'mariaDBVersion': '10.11', 'forceRebuild': False, 'debug': False, 'verbose': True, 'wikiId': None, 'versions': ['1.35.10','1.38.6', '1.39.3'], 'basePort': 9080}
+                   'host': Host.get_default_host(), 'script_path': '', 'container_base_name': 'mw-139', 'networkName': 'mwNetwork', 'mariaDBVersion': '10.11', 'forceRebuild': False, 'debug': False, 'verbose': True, 
+                   'wikiId': None, 'versions': ['1.35.10','1.38.6', '1.39.3'], 'basePort': 9080,
+                   'dockerPath': mwClusterConfig.dockerPath}
 
         mwd=mwClusterConfig.as_dict()
         debug=self.debug
         #debug=True
         if debug:
             print(mwd)
             print(json.dumps(mwd,indent=2))
@@ -42,19 +43,19 @@
         """
         parser = ArgumentParser()
         mwClusterConfig=MwClusterConfig()
         mwClusterConfig.addArgs(parser)
         argv=["--prot","https"]
         args = parser.parse_args(argv)
         mwClusterConfig.fromArgs(args)
-        mwd=dataclasses.asdict(mwClusterConfig)
+        json_str=mwClusterConfig.as_json()
         debug=self.debug
         #debug=True
         if debug:
-            print(json.dumps(mwd,indent=2))
+            print(json_str)
         self.assertEqual("https",mwClusterConfig.prot)
         
     def test_random_password(self):
         """
         test the random password generation
         """
         config=MwClusterConfig()
```

### Comparing `pymediawikidocker-0.9.4/tests/test_extensions.py` & `pymediawikidocker-0.9.6/tests/test_extensions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 '''
 Created on 2021-06-23
 
 @author: wf
 '''
 import unittest
 from mwdocker.config import MwClusterConfig
+from mwdocker.docker import DockerApplication
 from mwdocker.mw import ExtensionList, Extension
 from tests.basetest import Basetest
 
 class TestExtensions(Basetest):
     '''
     test the extension handling
     '''
 
     def setUp(self):
         Basetest.setUp(self)
         pass
     
+    def testReadExtensions(self):
+        """
+        read the extensions
+        """
+        extensionList=ExtensionList()
+        extensionList.restoreFromJsonFile(ExtensionList.storeFilePrefix())
+        self.assertTrue(len(extensionList.extensions)>=35)
+        pass
+    
     def testExtensionDetailsFromUrl(self):
         '''
         test getting details of an extension
         '''
         ext=Extension()
         ext.name="UrlGetParameters"
         ext.url="https://www.mediawiki.org/wiki/Extension:UrlGetParameters"
```

### Comparing `pymediawikidocker-0.9.4/tests/test_html_tables.py` & `pymediawikidocker-0.9.6/tests/test_html_tables.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.4/tests/test_install.py` & `pymediawikidocker-0.9.6/tests/test_install.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,39 +22,44 @@
 
 class TestInstall(Basetest):
     '''
     test MediaWiki Docker images installation using
     https://pypi.org/project/python-on-whales/
     '''
 
-    def setUp(self):
-        Basetest.setUp(self, debug=False)
-        # make sure we don't use the $HOME
-        self.home="/tmp"
+    def setUp(self, debug=False, profile=True):
+        Basetest.setUp(self, debug=debug, profile=profile)
+        # make sure we don't use the $HOME directory
+        self.docker_path="/tmp/.pmw" 
+        self.argv=["--dockerPath",self.docker_path]
         
-    def getMwConfig(self,argv=[]):
+    def getMwConfig(self,argv=None):
         """
         get a mediawiki configuration for the given command line arguments
         """
+        if not argv:
+            argv=self.argv
         parser = ArgumentParser()
         mwClusterConfig=MwClusterConfig()
         mwClusterConfig.addArgs(parser)
         args = parser.parse_args(argv)
         mwClusterConfig.fromArgs(args)
         return mwClusterConfig
     
-    def getMwCluster(self,argv=[],createApps:bool=True,withGenerate:bool=False):
+    def getMwCluster(self,argv=None,createApps:bool=True,withGenerate:bool=False):
         """
         get a mediawiki cluster as configured by the command line arguments
         """
+        if not argv:
+            argv=self.argv
         config=self.getMwConfig(argv)
         mwCluster=MediaWikiCluster(config=config)
         mwCluster.checkDocker()
         if createApps:
-            mwCluster.createApps(home=self.home,withGenerate=withGenerate)
+            mwCluster.createApps(withGenerate=withGenerate)
         return mwCluster
     
     def printCommand(self,options,args):
         """
         print the mw cluster command with the given options and args
         """
         arg_str=' '.join(args)
@@ -84,21 +89,20 @@
             for d in dirs:
                 shutil.rmtree(os.path.join(root, d))
         
     def testGenerateDockerFiles(self):
         '''
         test generating the docker files
         '''
-        config_path=f"{self.home}/.pymediawikidocker"
-        self.removeFolderContent(config_path)
+        self.removeFolderContent(self.docker_path)
         mwCluster=self.getMwCluster(withGenerate=True)
         for _index,version in enumerate(mwCluster.config.versions):
             mwApp=mwCluster.apps[version]
             config=mwApp.config
-            epath=f"{config_path}/{config.container_base_name}"
+            epath=f"{self.docker_path}/{config.container_base_name}"
             self.assertTrue(os.path.isdir(epath))
             for fname in [
                     'Dockerfile',
                     'docker-compose.yml',
                     'startRunJobs.sh',
                     'LocalSettings.php',
                     'initdb.sh',
@@ -115,42 +119,47 @@
                 fpath=f"{epath}/{fname}"
                 self.assertTrue(os.path.isfile(fpath))
     
     def testInstallation(self):
         '''
         test the MediaWiki docker image installation
         '''
-        if self.inPublicCI():
-            self.home=None
         mwCluster=self.getMwCluster(withGenerate=True)
         mwCluster.start(forceRebuild=True)
         apps=mwCluster.apps.values()
         self.assertEqual(len(mwCluster.config.versions),len(apps))
         for mwApp in apps:
             self.assertTrue(mwApp.dbContainer is not None)
             self.assertTrue(mwApp.mwContainer is not None)
             dbStatus=mwApp.checkDBConnection()
-            self.assertTrue(dbStatus.ok)
+            self.assertTrue(dbStatus.ok,f"{mwApp.config.version}")
             userCountRecords=mwApp.sqlQuery("select count(*) from user;")
-            print(userCountRecords)
+            print(f"{userCountRecords}")
         mwCluster.close()
         exitCode=mwCluster.check()
         self.assertEqual(0,exitCode)
         
     def testPortBindingAccess(self):
         """
         https://github.com/WolfgangFahl/pymediawikidocker/issues/48
         
         refactor port binding access 
         """    
         mwCluster=self.getMwCluster(withGenerate=False)
         apps=mwCluster.apps.values()
+        debug=self.debug
+        debug=True
         for mwApp in apps:
+            config_json=mwApp.config.as_json()
+            if debug:
+                print(config_json)
             self.assertTrue(mwApp.dbContainer is not None)
             self.assertTrue(mwApp.mwContainer is not None)
+            if debug:
+                print(mwApp.mwContainer.container)
             browser_port=mwApp.mwContainer.getHostPort(80)
             sql_port=mwApp.dbContainer.getHostPort(3306)
             self.assertEqual(str(browser_port),str(mwApp.config.port))
             self.assertEqual(str(sql_port),str(mwApp.config.sqlPort))
             pass
         
     def testSocketGetHostname(self):
```

### Comparing `pymediawikidocker-0.9.4/.gitignore` & `pymediawikidocker-0.9.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.4/LICENSE` & `pymediawikidocker-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.4/README.md` & `pymediawikidocker-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.4/pyproject.toml` & `pymediawikidocker-0.9.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.4/PKG-INFO` & `pymediawikidocker-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymediawikidocker
-Version: 0.9.4
+Version: 0.9.6
 Summary: Python controlled (semantic) mediawiki docker application cluster installation
 Project-URL: Home, https://github.com/WolfgangFahl/pymediawikidocker
 Project-URL: Documentation, https://wiki.bitplan.com/index.php/pymediawikidocker
 Project-URL: Source, https://github.com/WolfgangFahl/pymediawikidocker
 Author-email: Wolfgang Fahl <wf@bitplan.com>
 Maintainer-email: Wolfgang Fahl <wf@bitplan.com>
 License: Apache-2.0
```

