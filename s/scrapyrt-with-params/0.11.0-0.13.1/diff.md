# Comparing `tmp/scrapyrt-with-params-0.11.0.tar.gz` & `tmp/scrapyrt-with-params-0.13.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\scrapyrt-with-params-0.11.0.tar", last modified: Mon Jul 13 07:37:21 2020, max compression
+gzip compressed data, was "scrapyrt-with-params-0.13.1.tar", last modified: Wed Apr 12 12:41:23 2023, max compression
```

## Comparing `scrapyrt-with-params-0.11.0.tar` & `scrapyrt-with-params-0.13.1.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxrwxrwx   0        0        0        0 2020-07-13 07:37:21.000000 scrapyrt-with-params-0.11.0/
--rw-rw-rw-   0        0        0     3024 2020-07-13 07:37:21.000000 scrapyrt-with-params-0.11.0/PKG-INFO
--rw-rw-rw-   0        0        0     1718 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.11.0/README.rst
-drwxrwxrwx   0        0        0        0 2020-07-13 07:37:20.000000 scrapyrt-with-params-0.11.0/scrapyrt/
--rw-rw-rw-   0        0        0        8 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.11.0/scrapyrt/VERSION
--rw-rw-rw-   0        0        0      269 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.11.0/scrapyrt/__init__.py
--rw-rw-rw-   0        0        0     3467 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.11.0/scrapyrt/cmdline.py
-drwxrwxrwx   0        0        0        0 2020-07-13 07:37:20.000000 scrapyrt-with-params-0.11.0/scrapyrt/conf/
--rw-rw-rw-   0        0        0     1187 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.11.0/scrapyrt/conf/__init__.py
--rw-rw-rw-   0        0        0      766 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.11.0/scrapyrt/conf/default_settings.py
--rw-rw-rw-   0        0        0      999 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.11.0/scrapyrt/conf/spider_settings.py
--rw-rw-rw-   0        0        0     9774 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.11.0/scrapyrt/core.py
--rw-rw-rw-   0        0        0      898 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.11.0/scrapyrt/decorators.py
--rw-rw-rw-   0        0        0      211 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.11.0/scrapyrt/exceptions.py
--rw-rw-rw-   0        0        0     5439 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.11.0/scrapyrt/log.py
--rw-rw-rw-   0        0        0     9723 2020-07-13 07:00:32.000000 scrapyrt-with-params-0.11.0/scrapyrt/resources.py
--rw-rw-rw-   0        0        0     1426 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.11.0/scrapyrt/utils.py
-drwxrwxrwx   0        0        0        0 2020-07-13 07:37:21.000000 scrapyrt-with-params-0.11.0/scrapyrt_with_params.egg-info/
--rw-rw-rw-   0        0        0     3024 2020-07-13 07:37:20.000000 scrapyrt-with-params-0.11.0/scrapyrt_with_params.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1084 2020-07-13 07:37:20.000000 scrapyrt-with-params-0.11.0/scrapyrt_with_params.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-07-13 07:37:20.000000 scrapyrt-with-params-0.11.0/scrapyrt_with_params.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2020-07-13 07:37:20.000000 scrapyrt-with-params-0.11.0/scrapyrt_with_params.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2020-07-13 07:37:20.000000 scrapyrt-with-params-0.11.0/scrapyrt_with_params.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       49 2020-07-13 07:37:20.000000 scrapyrt-with-params-0.11.0/scrapyrt_with_params.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2020-07-13 07:37:20.000000 scrapyrt-with-params-0.11.0/scrapyrt_with_params.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       74 2020-07-13 07:37:21.000000 scrapyrt-with-params-0.11.0/setup.cfg
--rw-rw-rw-   0        0        0     1543 2020-07-13 07:30:11.000000 scrapyrt-with-params-0.11.0/setup.py
-drwxrwxrwx   0        0        0        0 2020-07-13 07:37:21.000000 scrapyrt-with-params-0.11.0/tests/
--rw-rw-rw-   0        0        0      216 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.11.0/tests/__init__.py
--rw-rw-rw-   0        0        0     3608 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.11.0/tests/servers.py
--rw-rw-rw-   0        0        0     1227 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.11.0/tests/spiders.py
--rw-rw-rw-   0        0        0     1481 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.11.0/tests/test_cmdline.py
--rw-rw-rw-   0        0        0    16480 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.11.0/tests/test_crawl_manager.py
--rw-rw-rw-   0        0        0     3021 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.11.0/tests/test_crawler.py
--rw-rw-rw-   0        0        0     1787 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.11.0/tests/test_crawler_process.py
--rw-rw-rw-   0        0        0      709 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.11.0/tests/test_decorators.py
--rw-rw-rw-   0        0        0     1692 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.11.0/tests/test_log_observer.py
--rw-rw-rw-   0        0        0    13995 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.11.0/tests/test_resource_crawl.py
--rw-rw-rw-   0        0        0     1966 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.11.0/tests/test_resource_realtimeapi.py
--rw-rw-rw-   0        0        0      748 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.11.0/tests/test_resource_root.py
--rw-rw-rw-   0        0        0     8158 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.11.0/tests/test_resource_serviceresource.py
-drwxrwxrwx   0        0        0        0 2020-07-13 07:37:21.000000 scrapyrt-with-params-0.11.0/tests/test_settings/
--rw-rw-rw-   0        0        0     2341 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.11.0/tests/test_settings/__init__.py
--rw-rw-rw-   0        0        0      113 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.11.0/tests/test_settings/default_settings.py
--rw-rw-rw-   0        0        0       34 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.11.0/tests/test_settings/settings.py
--rw-rw-rw-   0        0        0      908 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.11.0/tests/test_utils.py
--rw-rw-rw-   0        0        0     1786 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.11.0/tests/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 12:41:23.712447 scrapyrt-with-params-0.13.1/
+-rw-rw-rw-   0        0        0     1548 2023-04-12 12:09:35.000000 scrapyrt-with-params-0.13.1/LICENSE
+-rw-rw-rw-   0        0        0     4768 2023-04-12 12:41:23.713444 scrapyrt-with-params-0.13.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3547 2023-04-12 12:09:35.000000 scrapyrt-with-params-0.13.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-12 12:41:23.644628 scrapyrt-with-params-0.13.1/scrapyrt/
+-rw-rw-rw-   0        0        0        6 2023-04-12 12:41:20.000000 scrapyrt-with-params-0.13.1/scrapyrt/VERSION
+-rw-rw-rw-   0        0        0      252 2023-04-12 12:09:35.000000 scrapyrt-with-params-0.13.1/scrapyrt/__init__.py
+-rw-rw-rw-   0        0        0     4071 2023-04-12 12:09:35.000000 scrapyrt-with-params-0.13.1/scrapyrt/cmdline.py
+drwxrwxrwx   0        0        0        0 2023-04-12 12:41:23.650611 scrapyrt-with-params-0.13.1/scrapyrt/conf/
+-rw-rw-rw-   0        0        0     1166 2023-04-12 12:09:35.000000 scrapyrt-with-params-0.13.1/scrapyrt/conf/__init__.py
+-rw-rw-rw-   0        0        0      790 2023-04-12 12:09:35.000000 scrapyrt-with-params-0.13.1/scrapyrt/conf/default_settings.py
+-rw-rw-rw-   0        0        0     1007 2023-04-12 12:09:35.000000 scrapyrt-with-params-0.13.1/scrapyrt/conf/spider_settings.py
+-rw-rw-rw-   0        0        0    10189 2023-04-12 12:09:35.000000 scrapyrt-with-params-0.13.1/scrapyrt/core.py
+-rw-rw-rw-   0        0        0      898 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.13.1/scrapyrt/decorators.py
+-rw-rw-rw-   0        0        0      211 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.13.1/scrapyrt/exceptions.py
+-rw-rw-rw-   0        0        0     5392 2023-04-12 12:09:35.000000 scrapyrt-with-params-0.13.1/scrapyrt/log.py
+-rw-rw-rw-   0        0        0     9723 2023-04-12 12:35:33.000000 scrapyrt-with-params-0.13.1/scrapyrt/resources.py
+-rw-rw-rw-   0        0        0     2723 2023-04-12 12:09:35.000000 scrapyrt-with-params-0.13.1/scrapyrt/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 12:41:23.671557 scrapyrt-with-params-0.13.1/scrapyrt_with_params.egg-info/
+-rw-rw-rw-   0        0        0     4768 2023-04-12 12:41:23.000000 scrapyrt-with-params-0.13.1/scrapyrt_with_params.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1092 2023-04-12 12:41:23.000000 scrapyrt-with-params-0.13.1/scrapyrt_with_params.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 12:41:23.000000 scrapyrt-with-params-0.13.1/scrapyrt_with_params.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-04-12 12:41:23.000000 scrapyrt-with-params-0.13.1/scrapyrt_with_params.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2020-07-13 07:37:20.000000 scrapyrt-with-params-0.13.1/scrapyrt_with_params.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       14 2023-04-12 12:41:23.000000 scrapyrt-with-params-0.13.1/scrapyrt_with_params.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-12 12:41:23.000000 scrapyrt-with-params-0.13.1/scrapyrt_with_params.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       74 2023-04-12 12:41:23.715439 scrapyrt-with-params-0.13.1/setup.cfg
+-rw-rw-rw-   0        0        0     1844 2023-04-12 12:15:05.000000 scrapyrt-with-params-0.13.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 12:41:23.704468 scrapyrt-with-params-0.13.1/tests/
+-rw-rw-rw-   0        0        0      216 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.13.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     3598 2023-04-12 12:09:35.000000 scrapyrt-with-params-0.13.1/tests/servers.py
+-rw-rw-rw-   0        0        0     1227 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.13.1/tests/spiders.py
+-rw-rw-rw-   0        0        0     2979 2023-04-12 12:09:35.000000 scrapyrt-with-params-0.13.1/tests/test_cmdline.py
+-rw-rw-rw-   0        0        0    16488 2023-04-12 12:09:35.000000 scrapyrt-with-params-0.13.1/tests/test_crawl_manager.py
+-rw-rw-rw-   0        0        0     3021 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.13.1/tests/test_crawler.py
+-rw-rw-rw-   0        0        0     1787 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.13.1/tests/test_crawler_process.py
+-rw-rw-rw-   0        0        0      709 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.13.1/tests/test_decorators.py
+-rw-rw-rw-   0        0        0     1691 2023-04-12 12:09:35.000000 scrapyrt-with-params-0.13.1/tests/test_log_observer.py
+-rw-rw-rw-   0        0        0    18606 2023-04-12 12:09:35.000000 scrapyrt-with-params-0.13.1/tests/test_resource_crawl.py
+-rw-rw-rw-   0        0        0     2016 2023-04-12 12:09:35.000000 scrapyrt-with-params-0.13.1/tests/test_resource_realtimeapi.py
+-rw-rw-rw-   0        0        0      748 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.13.1/tests/test_resource_root.py
+-rw-rw-rw-   0        0        0     8158 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.13.1/tests/test_resource_serviceresource.py
+drwxrwxrwx   0        0        0        0 2023-04-12 12:41:23.711449 scrapyrt-with-params-0.13.1/tests/test_settings/
+-rw-rw-rw-   0        0        0     2341 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.13.1/tests/test_settings/__init__.py
+-rw-rw-rw-   0        0        0      113 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.13.1/tests/test_settings/default_settings.py
+-rw-rw-rw-   0        0        0       34 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.13.1/tests/test_settings/settings.py
+-rw-rw-rw-   0        0        0      908 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.13.1/tests/test_utils.py
+-rw-rw-rw-   0        0        0     1786 2020-07-13 06:59:34.000000 scrapyrt-with-params-0.13.1/tests/utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `scrapyrt-with-params-0.11.0/scrapyrt/cmdline.py` & `scrapyrt-with-params-0.13.1/scrapyrt/cmdline.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # -*- coding: utf-8 -*-
-from six.moves.configparser import (
-    SafeConfigParser, NoOptionError, NoSectionError
-)
 import argparse
 import os
 import sys
+from configparser import ConfigParser, NoOptionError, NoSectionError
 
 from scrapy.utils.conf import closest_scrapy_cfg
 from scrapy.utils.misc import load_object
 from twisted.application import app
 from twisted.application.internet import TCPServer
 from twisted.application.service import Application
-from twisted.internet import reactor
+from twisted.python import log
 from twisted.web.server import Site
+from scrapyrt.conf.spider_settings import get_project_settings
 
+from scrapyrt.utils import install_reactor
+
+from .conf import app_settings
 from .log import setup_logging
-from .conf import settings
 
 
 def parse_arguments():
 
     def valid_setting(string):
         key, sep, value = string.partition('=')
         if not key or not sep:
@@ -48,50 +49,67 @@
     parser.add_argument('-S', '--settings', dest='settings',
                         metavar='project.settings',
                         help='custom project settings module path')
     return parser.parse_args()
 
 
 def get_application(arguments):
-    ServiceRoot = load_object(settings.SERVICE_ROOT)
+    ServiceRoot = load_object(app_settings.SERVICE_ROOT)
     site = Site(ServiceRoot())
     application = Application('scrapyrt')
     server = TCPServer(arguments.port, site, interface=arguments.ip)
     server.setServiceParent(application)
     return application
 
 
 def find_scrapy_project(project):
     project_config_path = closest_scrapy_cfg()
     if not project_config_path:
         raise RuntimeError('Cannot find scrapy.cfg file')
-    project_config = SafeConfigParser()
+    project_config = ConfigParser()
     project_config.read(project_config_path)
     try:
         project_settings = project_config.get('settings', project)
     except (NoSectionError, NoOptionError) as e:
         raise RuntimeError(e.message)
     if not project_settings:
         raise RuntimeError('Cannot find scrapy project settings')
     project_location = os.path.dirname(project_config_path)
     sys.path.append(project_location)
     return project_settings
 
 
+def run_application(reactor_type, arguments, app_settings):
+    if reactor_type is not None:
+        install_reactor(reactor_type)
+
+    setup_logging()
+
+    application = get_application(arguments)
+    app_settings.freeze()
+    app.startApplication(application, save=False)
+    from twisted.internet import reactor
+    msg = f"Running with reactor: {reactor.__class__.__name__}. "
+    log.msg(msg)
+    reactor.run()
+
+
 def execute():
     sys.path.insert(0, os.getcwd())
+
     arguments = parse_arguments()
     if arguments.settings:
-        settings.setmodule(arguments.settings)
+        app_settings.setmodule(arguments.settings)
     if arguments.set:
         for name, value in arguments.set:
-            settings.set(name.upper(), value)
-    settings.set('PROJECT_SETTINGS', find_scrapy_project(arguments.project))
-    settings.freeze()
-    setup_logging()
-    application = get_application(arguments)
-    app.startApplication(application, save=False)
-    reactor.run()
+            app_settings.set(name.upper(), value)
+
+    app_settings.set('PROJECT_SETTINGS',
+                     find_scrapy_project(arguments.project))
+    project_settings = get_project_settings()
+    reactor_type = app_settings.TWISTED_REACTOR or project_settings.get(
+        'TWISTED_REACTOR')
+    run_application(reactor_type, arguments, app_settings)
 
 
 if __name__ == '__main__':
     execute()
```

### Comparing `scrapyrt-with-params-0.11.0/scrapyrt/conf/__init__.py` & `scrapyrt-with-params-0.13.1/scrapyrt/conf/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # -*- coding: utf-8 -*-
-import six
 from copy import deepcopy
 from importlib import import_module
 
 from . import default_settings
 
 
 class Settings(object):
 
     def __init__(self):
         self.setmodule(default_settings)
 
     def setmodule(self, module):
-        if isinstance(module, six.string_types):
+        if isinstance(module, str):
             module = import_module(module)
         for setting in dir(module):
             self.set(setting, getattr(module, setting))
 
     def __setattr__(self, key, value):
         if self.frozen:
             raise TypeError("Trying to modify a frozen Settings object")
@@ -33,8 +32,8 @@
         self._frozen = True
 
     @property
     def frozen(self):
         return bool(getattr(self, '_frozen', False))
 
 
-settings = Settings()
+app_settings = Settings()
```

### Comparing `scrapyrt-with-params-0.11.0/scrapyrt/conf/default_settings.py` & `scrapyrt-with-params-0.13.1/scrapyrt/conf/default_settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,7 +26,9 @@
 
 CRAWL_MANAGER = 'scrapyrt.core.CrawlManager'
 
 # Limit spider run time
 TIMEOUT_LIMIT = 1000
 # disable in production
 DEBUG = True
+
+TWISTED_REACTOR = None
```

### Comparing `scrapyrt-with-params-0.11.0/scrapyrt/conf/spider_settings.py` & `scrapyrt-with-params-0.13.1/scrapyrt/conf/spider_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 from scrapy.settings import Settings
 
-from . import settings
+from . import app_settings
 
 
 def get_scrapyrt_settings(log_file=None):
     spider_settings = {
         "LOG_LEVEL": "DEBUG",
         "LOG_ENABLED": bool(log_file),
         "LOG_FILE": log_file,
@@ -19,13 +19,13 @@
     }
     return spider_settings
 
 
 def get_project_settings(module=None, custom_settings=None):
     crawler_settings = Settings()
     if module is None:
-        module = settings.PROJECT_SETTINGS
+        module = app_settings.PROJECT_SETTINGS
     crawler_settings.setmodule(module, priority='project')
     if custom_settings:
         assert isinstance(custom_settings, dict)
         crawler_settings.setdict(custom_settings, priority='cmdline')
     return crawler_settings
```

### Comparing `scrapyrt-with-params-0.11.0/scrapyrt/core.py` & `scrapyrt-with-params-0.13.1/scrapyrt/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # -*- coding: utf-8 -*-
 from collections import OrderedDict
 from copy import deepcopy
 import datetime
 import os
-import six
 
 from scrapy import signals
 from scrapy.crawler import CrawlerRunner, Crawler
 from scrapy.exceptions import DontCloseSpider
 from scrapy.http import Request
 from twisted.web.error import Error
 from twisted.internet import defer
 
 from . import log
-from .conf import settings
+from .conf import app_settings
 from .conf.spider_settings import get_scrapyrt_settings, get_project_settings
 from .decorators import deprecated
 from .log import setup_spider_logging
 
 
 class ScrapyrtCrawler(Crawler):
     """Main and only difference from base class -
@@ -25,14 +24,15 @@
     start_requests.
 
     https://github.com/scrapy/scrapy/blob/master/scrapy/crawler.py#L52
 
     TODO: PR to scrapy - ability to set start_requests here.
 
     """
+
     def __init__(self, spidercls, crawler_settings, start_requests=False):
         super(ScrapyrtCrawler, self).__init__(spidercls, crawler_settings)
         self.start_requests = start_requests
 
     @defer.inlineCallbacks
     def crawl(self, *args, **kwargs):
         assert not self.crawling, "Crawling already taking place"
@@ -54,16 +54,24 @@
 class ScrapyrtCrawlerProcess(CrawlerRunner):
 
     def __init__(self, settings, scrapyrt_manager):
         super(ScrapyrtCrawlerProcess, self).__init__(settings)
         self.scrapyrt_manager = scrapyrt_manager
 
     def crawl(self, spidercls, *args, **kwargs):
-        if isinstance(spidercls, six.string_types):
+        if isinstance(spidercls, str):
             spidercls = self.spider_loader.load(spidercls)
+
+        for kw in kwargs:
+            attr_or_m = getattr(spidercls, kw, None)
+            if attr_or_m and callable(attr_or_m):
+                msg = 'Crawl argument cannot override spider method.'
+                msg += ' Got argument {} that overrides spider method {}'
+                raise Error('400', message=msg.format(
+                    kw, getattr(spidercls, kw)))
         # creating our own crawler that will allow us to disable start requests easily
         crawler = ScrapyrtCrawler(
             spidercls, self.settings, self.scrapyrt_manager.start_requests)
         self.scrapyrt_manager.crawler = crawler
         # Connecting signals to handlers that control crawl process
         crawler.signals.connect(self.scrapyrt_manager.get_item,
                                 signals.item_scraped)
@@ -71,39 +79,41 @@
                                 signals.item_dropped)
         crawler.signals.connect(self.scrapyrt_manager.spider_idle,
                                 signals.spider_idle)
         crawler.signals.connect(self.scrapyrt_manager.handle_spider_error,
                                 signals.spider_error)
         crawler.signals.connect(self.scrapyrt_manager.handle_scheduling,
                                 signals.request_scheduled)
-        dfd = super(ScrapyrtCrawlerProcess, self).crawl(crawler, *args, **kwargs)
+        dfd = super(ScrapyrtCrawlerProcess, self).crawl(
+            crawler, *args, **kwargs)
         _cleanup_handler = setup_spider_logging(crawler.spider, self.settings)
 
         def cleanup_logging(result):
             _cleanup_handler()
             return result
 
         return dfd.addBoth(cleanup_logging)
 
 
 class CrawlManager(object):
     """
     Runs crawls
     """
 
-    def __init__(self, spider_name, request_kwargs, max_requests=None, start_requests=False):
+    def __init__(self, spider_name, request_kwargs,
+                 max_requests=None, start_requests=False):
         self.spider_name = spider_name
-        self.log_dir = settings.LOG_DIR
+        self.log_dir = app_settings.LOG_DIR
         self.items = []
         self.items_dropped = []
         self.errors = []
         self.max_requests = int(max_requests) if max_requests else None
-        self.timeout_limit = int(settings.TIMEOUT_LIMIT)
+        self.timeout_limit = int(app_settings.TIMEOUT_LIMIT)
         self.request_count = 0
-        self.debug = settings.DEBUG
+        self.debug = app_settings.DEBUG
         self.crawler_process = None
         self.crawler = None
         # callback will be added after instantiation of crawler object
         # because we need to know if spider has method available
         self.callback_name = request_kwargs.pop('callback', None) or 'parse'
         # do the same for errback
         self.errback_name = request_kwargs.pop('errback', None) or 'parse'
@@ -126,15 +136,15 @@
         dfd.addCallback(self.return_items)
         return dfd
 
     def _get_log_file_path(self):
         log_dir = os.path.join(self.log_dir, self.spider_name)
         if not os.path.exists(log_dir):
             os.makedirs(log_dir)
-        time_format = settings.SPIDER_LOG_FILE_TIMEFORMAT
+        time_format = app_settings.SPIDER_LOG_FILE_TIMEFORMAT
         filename = datetime.datetime.now().strftime(time_format) + '.log'
         return os.path.join(log_dir, filename)
 
     def get_project_settings(self):
         # set logfile for a job
         log_file = self._get_log_file_path()
         custom_settings = get_scrapyrt_settings(log_file=log_file)
```

### Comparing `scrapyrt-with-params-0.11.0/scrapyrt/decorators.py` & `scrapyrt-with-params-0.13.1/scrapyrt/decorators.py`

 * *Files identical despite different names*

### Comparing `scrapyrt-with-params-0.11.0/scrapyrt/log.py` & `scrapyrt-with-params-0.13.1/scrapyrt/log.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from scrapy.settings import Settings
 from scrapy.utils.log import DEFAULT_LOGGING, TopLevelFormatter
 from twisted.python import log
 from twisted.python.log import startLoggingWithObserver
 from twisted.python.logfile import DailyLogFile
 
-from .conf import settings as scrapyrt_settings
+from .conf import app_settings
 from .utils import to_bytes
 
 DEBUG = logging.DEBUG
 INFO = logging.INFO
 WARNING = logging.WARNING
 ERROR = logging.ERROR
 CRITICAL = logging.CRITICAL
@@ -87,24 +87,24 @@
 
     def filter(self, record):
         spider = getattr(record, 'spider', None)
         return spider and spider is self.spider
 
 
 def setup_logging():
-    if not os.path.exists(scrapyrt_settings.LOG_DIR):
-        os.makedirs(scrapyrt_settings.LOG_DIR)
-    if scrapyrt_settings.LOG_FILE:
+    if not os.path.exists(app_settings.LOG_DIR):
+        os.makedirs(app_settings.LOG_DIR)
+    if app_settings.LOG_FILE:
         logfile = DailyLogFile.fromFullPath(
-            os.path.join(scrapyrt_settings.LOG_DIR,
-                         scrapyrt_settings.LOG_FILE)
+            os.path.join(app_settings.LOG_DIR,
+                         app_settings.LOG_FILE)
         )
     else:
         logfile = sys.stderr
-    observer = ScrapyrtFileLogObserver(logfile, scrapyrt_settings.LOG_ENCODING)
+    observer = ScrapyrtFileLogObserver(logfile, app_settings.LOG_ENCODING)
     startLoggingWithObserver(observer.emit, setStdout=False)
 
     # setup general logging for Scrapy
     if not sys.warnoptions:
         # Route warnings through python logging
         logging.captureWarnings(True)
```

### Comparing `scrapyrt-with-params-0.11.0/scrapyrt/resources.py` & `scrapyrt-with-params-0.13.1/scrapyrt/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,20 +209,20 @@
         spider_name = self.get_required_argument(api_params, 'spider_name')
         start_requests = api_params.get("start_requests", False)
         try:
             max_requests = api_params['max_requests']
         except (KeyError, IndexError):
             max_requests = None
 
-        """ INICIO NUEVO AÑADIDO MANUEL """
+        """ INICIO NUEVO ANYADIDO MANUEL """
         crawler_params = api_params.copy()
         for api_param in ['max_requests', 'start_requests', 'spider_name', 'url']:
             crawler_params.pop(api_param, None)
         kwargs.update(crawler_params)
-        """" FIN NUEVO AÑADIDO MANUEL """
+        """" FIN NUEVO ANYADIDO MANUEL """
 
         dfd = self.run_crawl(
             spider_name, scrapy_request_args, max_requests,
             start_requests=start_requests, *args, **kwargs)
         dfd.addCallback(
             self.prepare_response, request_data=api_params, *args, **kwargs)
         return dfd
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `scrapyrt-with-params-0.11.0/scrapyrt_with_params.egg-info/SOURCES.txt` & `scrapyrt-with-params-0.13.1/scrapyrt_with_params.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.rst
 setup.cfg
 setup.py
 scrapyrt/VERSION
 scrapyrt/__init__.py
 scrapyrt/cmdline.py
 scrapyrt/core.py
```

### Comparing `scrapyrt-with-params-0.11.0/setup.py` & `scrapyrt-with-params-0.13.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,29 +20,34 @@
     packages=find_packages(),
     entry_points={
         'console_scripts': ['scrapyrt = scrapyrt.cmdline:execute']
     },
     zip_safe=False,
     classifiers=[
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Operating System :: OS Independent',
         'Environment :: Console',
         'Environment :: No Input/Output (Daemon)',
         'Topic :: Internet :: WWW/HTTP',
         'License :: OSI Approved :: BSD License',
     ],
+    project_urls={
+        "Documentation": "https://scrapyrt.readthedocs.io/en/latest/index.html",
+        "Source": "https://github.com/scrapinghub/scrapyrt",
+        "Tracker": "https://github.com/scrapinghub/scrapyrt/issues"
+    },
     install_requires=[
-        'Twisted>=14.0.0',
-        'Scrapy>=1.0.0',
-        'demjson',
-        'six>=1.5.2'
+        'Scrapy>=1.0.0'
     ],
     package_data={
         'scrapyrt': [
             'VERSION',
         ]
     },
+    python_requires='>=3.6',
 )
```

### Comparing `scrapyrt-with-params-0.11.0/tests/servers.py` & `scrapyrt-with-params-0.13.1/tests/servers.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import os
 import shutil
 import socket
 import sys
 import tempfile
 import time
 from subprocess import Popen, PIPE
+from urllib.parse import urljoin
 
 import port_for
-from six.moves.urllib.parse import urljoin
 
 from . import TESTS_PATH
 from .utils import get_testenv, generate_project
 
 DEVNULL = open(os.devnull, 'wb')
```

### Comparing `scrapyrt-with-params-0.11.0/tests/spiders.py` & `scrapyrt-with-params-0.13.1/tests/spiders.py`

 * *Files identical despite different names*

### Comparing `scrapyrt-with-params-0.11.0/tests/test_cmdline.py` & `scrapyrt-with-params-0.13.1/tests/test_cmdline.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,23 @@
-import pytest
+import os
+import subprocess
 import sys
 import tempfile
 from collections import namedtuple
 from os import path, chdir
+from mock import patch
+
+import port_for
+import pytest
 from scrapy.utils.conf import closest_scrapy_cfg
 from twisted.python.components import Componentized
 
-from scrapyrt.cmdline import find_scrapy_project, get_application
-from tests.utils import generate_project
+from scrapyrt.cmdline import execute, find_scrapy_project, get_application
+from scrapyrt.conf import app_settings
+from tests.utils import generate_project, get_testenv
 
 
 def make_fake_args():
     fake_args = namedtuple('arguments', [
         'port',
         'ip',
         'set',
@@ -49,7 +55,41 @@
         with pytest.raises(RuntimeError) as err:
             find_scrapy_project('default')
         assert str(err.value) == "No section: 'settings'"
 
     def test_get_application(self):
         app = get_application(make_fake_args())
         assert isinstance(app, Componentized)
+
+    @patch('scrapyrt.cmdline.run_application')
+    @patch('scrapyrt.cmdline.parse_arguments',
+           new_callable=lambda: make_fake_args)
+    def test_execute(self, mock_pa, mock_run_app, workdir):
+        execute()
+        mock_run_app.assert_called_once_with(None, mock_pa(), app_settings)
+
+    @pytest.mark.parametrize('reactor,expected', [
+        ("twisted.internet.asyncioreactor.AsyncioSelectorReactor",
+         "AsyncioSelectorReactor"),
+        (None, 'EPollReactor')
+    ])
+    def test_reactor_launched(self, reactor, expected):
+        port = port_for.select_random()
+
+        tmp_dir = tempfile.mkdtemp()
+        cwd = os.path.join(tmp_dir, 'testproject')
+        generate_project(cwd)
+        cmd = [
+            sys.executable, '-m', 'scrapyrt.cmdline', '-p', str(port),
+        ]
+        if reactor is not None:
+            cmd.extend(['-s', f'TWISTED_REACTOR={reactor}'])
+
+        process = subprocess.Popen(cmd, cwd=cwd, stdout=subprocess.PIPE,
+                                   stderr=subprocess.PIPE,
+                                   env=get_testenv())
+        try:
+            _, logs = process.communicate(timeout=1)
+        except subprocess.TimeoutExpired:
+            process.kill()
+            _, logs = process.communicate()
+        assert f"Running with reactor: {expected}" in logs.decode()
```

### Comparing `scrapyrt-with-params-0.11.0/tests/test_crawl_manager.py` & `scrapyrt-with-params-0.13.1/tests/test_crawl_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from scrapy.utils.test import get_crawler
 from twisted.internet.defer import Deferred
 from twisted.python.failure import Failure
 from twisted.trial import unittest
 from twisted.web.error import Error
 
 from scrapyrt.core import CrawlManager
-from scrapyrt.conf import settings
+from scrapyrt.conf import app_settings
 
 from .spiders import MetaSpider
 
 
 class TestCrawlManager(unittest.TestCase):
 
     def setUp(self):
@@ -70,15 +70,15 @@
         spider_args = ['a', 'b']
         spider_kwargs = {'a': 1, 'b': 2}
         self.crawl_manager.crawl(*spider_args, **spider_kwargs)
         self.assertTrue(crawler_process_mock.called)
         call_args, call_kwargs = crawler_process_mock.call_args
         for arg in spider_args:
             self.assertIn(arg, call_args)
-        self.assertDictContainsSubset(spider_kwargs, call_kwargs)
+        self.assertEqual(spider_kwargs, call_kwargs)
 
 
 class TestGetProjectSettings(TestCrawlManager):
 
     def test_get_project_settings(self):
         result = self.crawl_manager.get_project_settings()
         self.assertIsInstance(result, Settings)
@@ -145,15 +145,15 @@
         try:
             with pytest.raises(AttributeError) as err:
                 mng.spider_idle(self.spider)
         except DontCloseSpider:
             pass
 
         assert mng.request.errback is None
-        msg = "AttributeError: 'MetaSpider' object has no attribute 'handle_error'"
+        msg = "has no attribute 'handle_error'"
         assert re.search(msg, str(err))
 
     def test_pass_good_spider_errback(self):
         mng = self.create_crawl_manager(
             {'url': 'http://localhost', 'errback': 'handle_error'}
         )
         self.crawler.spider.handle_error = lambda x: x
@@ -200,30 +200,30 @@
         self.crawl_manager.limit_runtime(self.spider)
         self.assertTrue(self.crawler.engine.close_spider.called)
 
     def test_limit_runtime(self):
         self._test_limit_runtime()
 
     def test_string_number_timeout_value(self):
-        _timeout = settings.TIMEOUT_LIMIT
+        _timeout = app_settings.TIMEOUT_LIMIT
         try:
-            settings.TIMEOUT_LIMIT = '1'
+            app_settings.TIMEOUT_LIMIT = '1'
             self.crawl_manager = self.create_crawl_manager()
             self._test_limit_runtime()
         finally:
-            settings.TIMEOUT_LIMIT = _timeout
+            app_settings.TIMEOUT_LIMIT = _timeout
 
     def test_wrong_timeout_value(self):
-        _timeout = settings.TIMEOUT_LIMIT
+        _timeout = app_settings.TIMEOUT_LIMIT
         try:
-            settings.TIMEOUT_LIMIT = 'foo'
+            app_settings.TIMEOUT_LIMIT = 'foo'
             self.assertRaises(
                 ValueError, CrawlManager, self.spider.name, self.kwargs.copy())
         finally:
-            settings.TIMEOUT_LIMIT = _timeout
+            app_settings.TIMEOUT_LIMIT = _timeout
 
 
 class TestHandleSpiderError(TestCrawlManager):
 
     def setUp(self):
         super(TestHandleSpiderError, self).setUp()
         self.exception_message = 'Foo'
@@ -330,16 +330,17 @@
             'items_dropped': self.crawl_manager.items_dropped,
             'stats': self.stats.copy(),
             'spider_name': self.spider.name,
         }
 
     def test_return_items(self):
         result = self.crawl_manager.return_items(None)
-        self.assertDictContainsSubset(self.expected_result, result)
-        self.assertEqual(list(sorted(self.stats.keys())), list(result['stats'].keys()))
+        self.assertEqual(dict(result, **self.expected_result), result)
+        self.assertEqual(list(sorted(self.stats.keys())),
+                         list(result['stats'].keys()))
         # debug = True by default
         self.assertIn('errors', result)
         self.assertEquals(result['errors'], self.crawl_manager.errors)
 
     def test_return_items_without_debug(self):
         self.crawl_manager.debug = False
         result = self.crawl_manager.return_items(None)
```

### Comparing `scrapyrt-with-params-0.11.0/tests/test_crawler.py` & `scrapyrt-with-params-0.13.1/tests/test_crawler.py`

 * *Files identical despite different names*

### Comparing `scrapyrt-with-params-0.11.0/tests/test_crawler_process.py` & `scrapyrt-with-params-0.13.1/tests/test_crawler_process.py`

 * *Files identical despite different names*

### Comparing `scrapyrt-with-params-0.11.0/tests/test_decorators.py` & `scrapyrt-with-params-0.13.1/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `scrapyrt-with-params-0.11.0/tests/test_log_observer.py` & `scrapyrt-with-params-0.13.1/tests/test_log_observer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-from six import StringIO
+from io import StringIO
 
 from mock import patch
 from twisted.python.log import startLoggingWithObserver, removeObserver
 from twisted.trial import unittest
 
 from scrapyrt.log import ScrapyrtFileLogObserver, msg
```

### Comparing `scrapyrt-with-params-0.11.0/tests/test_resource_realtimeapi.py` & `scrapyrt-with-params-0.13.1/tests/test_resource_realtimeapi.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # -*- coding: utf-8 -*-
 from copy import deepcopy
 import os
 
 from mock import patch
 from twisted.trial import unittest
 
-from scrapyrt.conf import settings
+from scrapyrt.conf import app_settings
 from scrapyrt.resources import RealtimeApi, ServiceResource, CrawlResource
 
 
-class TestResource(ServiceResource):
+class SampleResource(ServiceResource):
     isLeaf = True
     allowedMethods = ['GET', 'POST']
 
     def render_GET(self, request, **kwargs):
         return {'status': 'ok'}
 
 
@@ -28,21 +28,23 @@
         expected_entities = {b'crawl.json': CrawlResource}
         service_root = RealtimeApi()
         self._check_entities(service_root, expected_entities)
 
     # XXX: one inconvenience of singleton settings - complexities during tests,
     # e.g. settings are mutable, when you change them in one test -
     # changes will be kept unless you cleanup those changes or use mock.
-    @patch('scrapyrt.resources.settings', deepcopy(settings))
+    @patch('scrapyrt.resources.app_settings', deepcopy(app_settings))
     def test_realtimeapi_with_custom_settings(self):
-        from scrapyrt.resources import settings
-        settings.RESOURCES[b'test.json'] = self._get_class_path('TestResource')
+        from scrapyrt.resources import app_settings
+        app_settings.RESOURCES[b'test.json'] = self._get_class_path(
+            'SampleResource'
+        )
         expected_entities = {
             b'crawl.json': CrawlResource,
-            b'test.json': TestResource
+            b'test.json': SampleResource
         }
         service_root = RealtimeApi()
         self._check_entities(service_root, expected_entities)
 
     def _check_entities(self, service_root, expected_entities):
         self.assertFalse(service_root.isLeaf)
         entities = service_root.listEntities()
```

### Comparing `scrapyrt-with-params-0.11.0/tests/test_resource_root.py` & `scrapyrt-with-params-0.13.1/tests/test_resource_root.py`

 * *Files identical despite different names*

### Comparing `scrapyrt-with-params-0.11.0/tests/test_resource_serviceresource.py` & `scrapyrt-with-params-0.13.1/tests/test_resource_serviceresource.py`

 * *Files identical despite different names*

### Comparing `scrapyrt-with-params-0.11.0/tests/test_settings/__init__.py` & `scrapyrt-with-params-0.13.1/tests/test_settings/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapyrt-with-params-0.11.0/tests/test_utils.py` & `scrapyrt-with-params-0.13.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `scrapyrt-with-params-0.11.0/tests/utils.py` & `scrapyrt-with-params-0.13.1/tests/utils.py`

 * *Files identical despite different names*

