# Comparing `tmp/peek-field-service-3.3.3.tar.gz` & `tmp/peek-field-service-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-field-service-3.3.3.tar", last modified: Mon Nov 14 05:36:09 2022, max compression
+gzip compressed data, was "peek-field-service-3.4.0.tar", last modified: Wed Apr 12 11:04:53 2023, max compression
```

## Comparing `peek-field-service-3.3.3.tar` & `peek-field-service-3.4.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:09.607201 peek-field-service-3.3.3/
--rw-r--r--   0 root         (0) root         (0)      373 2022-11-14 05:36:09.607201 peek-field-service-3.3.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      245 2022-11-14 05:34:27.000000 peek-field-service-3.3.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:09.606201 peek-field-service-3.3.3/peek_field_service/
--rw-r--r--   0 root         (0) root         (0)     1506 2022-11-14 05:34:27.000000 peek-field-service-3.3.3/peek_field_service/PeekClientConfig.py
--rw-r--r--   0 root         (0) root         (0)     1295 2022-11-14 05:34:27.000000 peek-field-service-3.3.3/peek_field_service/PeekClientConfigTest.py
--rw-r--r--   0 root         (0) root         (0)      460 2022-11-14 05:34:27.000000 peek-field-service-3.3.3/peek_field_service/PlatformDependencyTest.py
--rw-r--r--   0 root         (0) root         (0)      146 2022-11-14 05:36:09.000000 peek-field-service-3.3.3/peek_field_service/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:09.606201 peek-field-service-3.3.3/peek_field_service/backend/
--rw-r--r--   0 root         (0) root         (0)      448 2022-11-14 05:34:27.000000 peek-field-service-3.3.3/peek_field_service/backend/ClientObservable.py
--rw-r--r--   0 root         (0) root         (0)     2357 2022-11-14 05:34:27.000000 peek-field-service-3.3.3/peek_field_service/backend/SiteRootResource.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-field-service-3.3.3/peek_field_service/backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:09.607201 peek-field-service-3.3.3/peek_field_service/plugin/
--rw-r--r--   0 root         (0) root         (0)     1575 2022-11-14 05:34:27.000000 peek-field-service-3.3.3/peek_field_service/plugin/ClientFrontendBuildersMixin.py
--rw-r--r--   0 root         (0) root         (0)     2779 2022-11-14 05:34:27.000000 peek-field-service-3.3.3/peek_field_service/plugin/ClientPluginLoader.py
--rw-r--r--   0 root         (0) root         (0)     1629 2022-11-14 05:34:27.000000 peek-field-service-3.3.3/peek_field_service/plugin/ClientPluginLoaderTest.py
--rw-r--r--   0 root         (0) root         (0)     3107 2022-11-14 05:34:27.000000 peek-field-service-3.3.3/peek_field_service/plugin/PeekClientPlatformHook.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-field-service-3.3.3/peek_field_service/plugin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9674 2022-11-14 05:34:32.000000 peek-field-service-3.3.3/peek_field_service/run_peek_field_service.py
--rw-r--r--   0 root         (0) root         (0)      600 2022-11-14 05:34:27.000000 peek-field-service-3.3.3/peek_field_service/run_peek_field_service_build_only.py
--rw-r--r--   0 root         (0) root         (0)      646 2022-11-14 05:34:27.000000 peek-field-service-3.3.3/peek_field_service/run_peek_field_service_offline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:09.607201 peek-field-service-3.3.3/peek_field_service/sw_install/
--rw-r--r--   0 root         (0) root         (0)      792 2022-11-14 05:34:27.000000 peek-field-service-3.3.3/peek_field_service/sw_install/PeekSwInstallManager.py
--rw-r--r--   0 root         (0) root         (0)      326 2022-11-14 05:34:27.000000 peek-field-service-3.3.3/peek_field_service/sw_install/PluginSwInstallManager.py
--rw-r--r--   0 root         (0) root         (0)      141 2022-11-14 05:34:27.000000 peek-field-service-3.3.3/peek_field_service/sw_install/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1405 2022-11-14 05:34:27.000000 peek-field-service-3.3.3/peek_field_service/winsvc_peek_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:09.606201 peek-field-service-3.3.3/peek_field_service.egg-info/
--rw-r--r--   0 root         (0) root         (0)      373 2022-11-14 05:36:09.000000 peek-field-service-3.3.3/peek_field_service.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1199 2022-11-14 05:36:09.000000 peek-field-service-3.3.3/peek_field_service.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-14 05:36:09.000000 peek-field-service-3.3.3/peek_field_service.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      351 2022-11-14 05:36:09.000000 peek-field-service-3.3.3/peek_field_service.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-14 05:36:09.000000 peek-field-service-3.3.3/peek_field_service.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      121 2022-11-14 05:36:09.000000 peek-field-service-3.3.3/peek_field_service.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2022-11-14 05:36:09.000000 peek-field-service-3.3.3/peek_field_service.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-14 05:36:09.607201 peek-field-service-3.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3259 2022-11-14 05:36:09.000000 peek-field-service-3.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:53.793210 peek-field-service-3.4.0/
+-rw-r--r--   0 root         (0) root         (0)      373 2023-04-12 11:04:53.793210 peek-field-service-3.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      245 2023-04-12 11:03:18.000000 peek-field-service-3.4.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:53.791210 peek-field-service-3.4.0/peek_field_service/
+-rw-r--r--   0 root         (0) root         (0)     1506 2023-04-12 11:03:18.000000 peek-field-service-3.4.0/peek_field_service/PeekClientConfig.py
+-rw-r--r--   0 root         (0) root         (0)     1295 2023-04-12 11:03:18.000000 peek-field-service-3.4.0/peek_field_service/PeekClientConfigTest.py
+-rw-r--r--   0 root         (0) root         (0)      460 2023-04-12 11:03:18.000000 peek-field-service-3.4.0/peek_field_service/PlatformDependencyTest.py
+-rw-r--r--   0 root         (0) root         (0)      146 2023-04-12 11:04:53.000000 peek-field-service-3.4.0/peek_field_service/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:53.792210 peek-field-service-3.4.0/peek_field_service/backend/
+-rw-r--r--   0 root         (0) root         (0)      448 2023-04-12 11:03:18.000000 peek-field-service-3.4.0/peek_field_service/backend/ClientObservable.py
+-rw-r--r--   0 root         (0) root         (0)     2247 2023-04-12 11:03:18.000000 peek-field-service-3.4.0/peek_field_service/backend/SiteRootResource.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:18.000000 peek-field-service-3.4.0/peek_field_service/backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:53.792210 peek-field-service-3.4.0/peek_field_service/plugin/
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-04-12 11:03:18.000000 peek-field-service-3.4.0/peek_field_service/plugin/ClientFrontendBuildersMixin.py
+-rw-r--r--   0 root         (0) root         (0)     2779 2023-04-12 11:03:18.000000 peek-field-service-3.4.0/peek_field_service/plugin/ClientPluginLoader.py
+-rw-r--r--   0 root         (0) root         (0)     1629 2023-04-12 11:03:18.000000 peek-field-service-3.4.0/peek_field_service/plugin/ClientPluginLoaderTest.py
+-rw-r--r--   0 root         (0) root         (0)     3107 2023-04-12 11:03:18.000000 peek-field-service-3.4.0/peek_field_service/plugin/PeekClientPlatformHook.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:18.000000 peek-field-service-3.4.0/peek_field_service/plugin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9797 2023-04-12 11:03:18.000000 peek-field-service-3.4.0/peek_field_service/run_peek_field_service.py
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-12 11:03:18.000000 peek-field-service-3.4.0/peek_field_service/run_peek_field_service_build_only.py
+-rw-r--r--   0 root         (0) root         (0)      646 2023-04-12 11:03:18.000000 peek-field-service-3.4.0/peek_field_service/run_peek_field_service_offline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:53.792210 peek-field-service-3.4.0/peek_field_service/sw_install/
+-rw-r--r--   0 root         (0) root         (0)      792 2023-04-12 11:03:18.000000 peek-field-service-3.4.0/peek_field_service/sw_install/PeekSwInstallManager.py
+-rw-r--r--   0 root         (0) root         (0)      326 2023-04-12 11:03:18.000000 peek-field-service-3.4.0/peek_field_service/sw_install/PluginSwInstallManager.py
+-rw-r--r--   0 root         (0) root         (0)      141 2023-04-12 11:03:18.000000 peek-field-service-3.4.0/peek_field_service/sw_install/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-04-12 11:03:18.000000 peek-field-service-3.4.0/peek_field_service/winsvc_peek_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:53.792210 peek-field-service-3.4.0/peek_field_service.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      373 2023-04-12 11:04:53.000000 peek-field-service-3.4.0/peek_field_service.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1199 2023-04-12 11:04:53.000000 peek-field-service-3.4.0/peek_field_service.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 11:04:53.000000 peek-field-service-3.4.0/peek_field_service.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      351 2023-04-12 11:04:53.000000 peek-field-service-3.4.0/peek_field_service.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 11:04:53.000000 peek-field-service-3.4.0/peek_field_service.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      121 2023-04-12 11:04:53.000000 peek-field-service-3.4.0/peek_field_service.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-12 11:04:53.000000 peek-field-service-3.4.0/peek_field_service.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 11:04:53.793210 peek-field-service-3.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3259 2023-04-12 11:04:53.000000 peek-field-service-3.4.0/setup.py
```

### Comparing `peek-field-service-3.3.3/peek_field_service/PeekClientConfig.py` & `peek-field-service-3.4.0/peek_field_service/PeekClientConfig.py`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.3.3/peek_field_service/PeekClientConfigTest.py` & `peek-field-service-3.4.0/peek_field_service/PeekClientConfigTest.py`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.3.3/peek_field_service/backend/SiteRootResource.py` & `peek-field-service-3.4.0/peek_field_service/backend/SiteRootResource.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,17 +46,14 @@
 
 def addVortexServers(siteRootResource):
     # Add the websocket to the site root
     VortexFactory.createHttpWebsocketServer(
         PeekPlatformConfig.componentName, siteRootResource
     )
 
-    # Add a HTTP vortex
-    # VortexFactory.createServer(PeekPlatformConfig.componentName, siteRootResource)
-
 
 def addDocSite(siteRootResource):
     # Setup properties for serving the site
     docSiteRoot = FileUnderlayResource()
     docSiteRoot.enableSinglePageApplication()
 
     # This dist dir is automatically generated, but check it's parent
```

### Comparing `peek-field-service-3.3.3/peek_field_service/plugin/ClientFrontendBuildersMixin.py` & `peek-field-service-3.4.0/peek_field_service/plugin/ClientFrontendBuildersMixin.py`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.3.3/peek_field_service/plugin/ClientPluginLoader.py` & `peek-field-service-3.4.0/peek_field_service/plugin/ClientPluginLoader.py`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.3.3/peek_field_service/plugin/ClientPluginLoaderTest.py` & `peek-field-service-3.4.0/peek_field_service/plugin/ClientPluginLoaderTest.py`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.3.3/peek_field_service/plugin/PeekClientPlatformHook.py` & `peek-field-service-3.4.0/peek_field_service/plugin/PeekClientPlatformHook.py`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.3.3/peek_field_service/run_peek_field_service.py` & `peek-field-service-3.4.0/peek_field_service/run_peek_field_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,14 +224,18 @@
         from peek_field_service.backend.SiteRootResource import (
             setupField,
             fieldRoot,
         )
 
         setupField(serveWebsocket=serveWebsocket)
 
+        VortexFactory.setPeerConnectionLimitPerIp(
+            httpServerConfig.concurrentPeerIpConnectionLimit
+        )
+
         setupSite(
             siteName,
             fieldRoot,
             portNum=httpServerConfig.sitePort,
             enableLogin=False,
             redirectFromHttpPort=httpServerConfig.redirectFromHttpPort,
             sslBundleFilePath=httpServerConfig.sslBundleFilePath,
```

### Comparing `peek-field-service-3.3.3/peek_field_service/run_peek_field_service_build_only.py` & `peek-field-service-3.4.0/peek_field_service/run_peek_field_service_build_only.py`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.3.3/peek_field_service/run_peek_field_service_offline.py` & `peek-field-service-3.4.0/peek_field_service/run_peek_field_service_offline.py`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.3.3/peek_field_service/sw_install/PeekSwInstallManager.py` & `peek-field-service-3.4.0/peek_field_service/sw_install/PeekSwInstallManager.py`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.3.3/peek_field_service/winsvc_peek_client.py` & `peek-field-service-3.4.0/peek_field_service/winsvc_peek_client.py`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.3.3/peek_field_service.egg-info/SOURCES.txt` & `peek-field-service-3.4.0/peek_field_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.3.3/setup.py` & `peek-field-service-3.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Modify these values to fork a new plugin
 #
 
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_field_service"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.3.3"
+package_version = "3.4.0"
 description = "Peek Field Service."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 ###############################################################################
```

