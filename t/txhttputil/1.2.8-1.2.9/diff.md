# Comparing `tmp/txhttputil-1.2.8.tar.gz` & `tmp/txhttputil-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txhttputil-1.2.8.tar", last modified: Thu Jan 12 00:57:44 2023, max compression
+gzip compressed data, was "txhttputil-1.2.9.tar", last modified: Sun Feb 26 05:15:02 2023, max compression
```

## Comparing `txhttputil-1.2.8.tar` & `txhttputil-1.2.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-01-12 00:57:43.997705 txhttputil-1.2.8/
--rw-r--r--   0 jchesney   (501) staff       (20)     1057 2021-09-22 06:19:19.000000 txhttputil-1.2.8/LICENSE
--rw-r--r--   0 jchesney   (501) staff       (20)      473 2023-01-12 00:57:43.997846 txhttputil-1.2.8/PKG-INFO
--rw-r--r--   0 jchesney   (501) staff       (20)      917 2021-09-22 06:19:19.000000 txhttputil-1.2.8/README.md
--rw-r--r--   0 jchesney   (501) staff       (20)       79 2023-01-12 00:57:43.998281 txhttputil-1.2.8/setup.cfg
--rw-r--r--   0 jchesney   (501) staff       (20)     1010 2023-01-12 00:57:42.000000 txhttputil-1.2.8/setup.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-01-12 00:57:43.981002 txhttputil-1.2.8/txhttputil/
--rw-r--r--   0 jchesney   (501) staff       (20)       24 2023-01-12 00:57:42.000000 txhttputil-1.2.8/txhttputil/__init__.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-01-12 00:57:43.984248 txhttputil-1.2.8/txhttputil/downloader/
--rw-r--r--   0 jchesney   (501) staff       (20)     2820 2022-01-12 13:58:49.000000 txhttputil-1.2.8/txhttputil/downloader/HttpFileDownloader.py
--rw-r--r--   0 jchesney   (501) staff       (20)     4568 2022-08-30 02:23:53.000000 txhttputil-1.2.8/txhttputil/downloader/HttpResourceProxy.py
--rw-r--r--   0 jchesney   (501) staff       (20)        0 2021-09-22 06:19:19.000000 txhttputil-1.2.8/txhttputil/downloader/__init__.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-01-12 00:57:43.986407 txhttputil-1.2.8/txhttputil/login_page/
--rw-r--r--   0 jchesney   (501) staff       (20)      876 2021-09-22 06:19:19.000000 txhttputil-1.2.8/txhttputil/login_page/LoginElement.py
--rw-r--r--   0 jchesney   (501) staff       (20)    71705 2021-09-22 06:19:19.000000 txhttputil-1.2.8/txhttputil/login_page/LoginTemplate.xml
--rw-r--r--   0 jchesney   (501) staff       (20)        0 2021-09-22 06:19:19.000000 txhttputil-1.2.8/txhttputil/login_page/__init__.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-01-12 00:57:43.994869 txhttputil-1.2.8/txhttputil/site/
--rw-r--r--   0 jchesney   (501) staff       (20)      664 2021-09-22 06:19:19.000000 txhttputil-1.2.8/txhttputil/site/AuthCredentials.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1624 2021-09-22 06:19:19.000000 txhttputil-1.2.8/txhttputil/site/AuthResource.py
--rw-r--r--   0 jchesney   (501) staff       (20)     8098 2021-09-22 06:19:19.000000 txhttputil-1.2.8/txhttputil/site/AuthSessionWrapper.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1258 2021-09-22 06:19:19.000000 txhttputil-1.2.8/txhttputil/site/AuthUserDetails.py
--rw-r--r--   0 jchesney   (501) staff       (20)     4498 2021-09-22 06:19:19.000000 txhttputil-1.2.8/txhttputil/site/BasicResource.py
--rw-r--r--   0 jchesney   (501) staff       (20)     4353 2022-08-14 07:32:40.000000 txhttputil-1.2.8/txhttputil/site/FileUnderlayResource.py
--rw-r--r--   0 jchesney   (501) staff       (20)     2312 2022-01-12 13:05:11.000000 txhttputil-1.2.8/txhttputil/site/FileUnderlayResourceTest.py
--rw-r--r--   0 jchesney   (501) staff       (20)     8856 2022-01-12 13:58:49.000000 txhttputil-1.2.8/txhttputil/site/FileUploadRequest.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1085 2021-09-22 06:19:19.000000 txhttputil-1.2.8/txhttputil/site/RedirectToHttpsResource.py
--rw-r--r--   0 jchesney   (501) staff       (20)      519 2022-08-14 07:32:40.000000 txhttputil-1.2.8/txhttputil/site/RedirectionRule.py
--rw-r--r--   0 jchesney   (501) staff       (20)       54 2021-09-22 06:19:19.000000 txhttputil-1.2.8/txhttputil/site/ResourceCreator.py
--rw-r--r--   0 jchesney   (501) staff       (20)      863 2021-09-22 06:19:19.000000 txhttputil-1.2.8/txhttputil/site/RootResource.py
--rw-r--r--   0 jchesney   (501) staff       (20)        0 2021-09-22 06:19:19.000000 txhttputil-1.2.8/txhttputil/site/RootSiteTest.py
--rw-r--r--   0 jchesney   (501) staff       (20)     4713 2023-01-01 06:46:58.000000 txhttputil-1.2.8/txhttputil/site/SiteUtil.py
--rw-r--r--   0 jchesney   (501) staff       (20)     4932 2023-01-10 12:05:27.000000 txhttputil-1.2.8/txhttputil/site/StaticFileResource.py
--rw-r--r--   0 jchesney   (501) staff       (20)        1 2022-08-14 07:32:35.000000 txhttputil-1.2.8/txhttputil/site/__init__.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-01-12 00:57:43.997453 txhttputil-1.2.8/txhttputil/util/
--rw-r--r--   0 jchesney   (501) staff       (20)     1263 2021-09-22 06:19:19.000000 txhttputil-1.2.8/txhttputil/util/DeferUtil.py
--rw-r--r--   0 jchesney   (501) staff       (20)      616 2021-09-22 06:19:19.000000 txhttputil-1.2.8/txhttputil/util/ModuleUtil.py
--rw-r--r--   0 jchesney   (501) staff       (20)    24790 2022-10-24 03:10:30.000000 txhttputil-1.2.8/txhttputil/util/PemUtil.py
--rw-r--r--   0 jchesney   (501) staff       (20)    13172 2022-08-30 02:23:53.000000 txhttputil-1.2.8/txhttputil/util/SslUtil.py
--rw-r--r--   0 jchesney   (501) staff       (20)        0 2021-09-22 06:19:19.000000 txhttputil-1.2.8/txhttputil/util/__init__.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-01-12 00:57:43.982657 txhttputil-1.2.8/txhttputil.egg-info/
--rw-r--r--   0 jchesney   (501) staff       (20)      473 2023-01-12 00:57:43.000000 txhttputil-1.2.8/txhttputil.egg-info/PKG-INFO
--rw-r--r--   0 jchesney   (501) staff       (20)     1167 2023-01-12 00:57:43.000000 txhttputil-1.2.8/txhttputil.egg-info/SOURCES.txt
--rw-r--r--   0 jchesney   (501) staff       (20)        1 2023-01-12 00:57:43.000000 txhttputil-1.2.8/txhttputil.egg-info/dependency_links.txt
--rw-r--r--   0 jchesney   (501) staff       (20)       66 2023-01-12 00:57:43.000000 txhttputil-1.2.8/txhttputil.egg-info/requires.txt
--rw-r--r--   0 jchesney   (501) staff       (20)       11 2023-01-12 00:57:43.000000 txhttputil-1.2.8/txhttputil.egg-info/top_level.txt
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-02-26 05:15:02.685409 txhttputil-1.2.9/
+-rw-r--r--   0 jchesney   (501) staff       (20)     1057 2021-09-22 06:19:19.000000 txhttputil-1.2.9/LICENSE
+-rw-r--r--   0 jchesney   (501) staff       (20)      439 2023-02-26 05:15:02.685596 txhttputil-1.2.9/PKG-INFO
+-rw-r--r--   0 jchesney   (501) staff       (20)      917 2021-09-22 06:19:19.000000 txhttputil-1.2.9/README.md
+-rw-r--r--   0 jchesney   (501) staff       (20)       79 2023-02-26 05:15:02.686371 txhttputil-1.2.9/setup.cfg
+-rw-r--r--   0 jchesney   (501) staff       (20)     1010 2023-02-26 05:14:59.000000 txhttputil-1.2.9/setup.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-02-26 05:15:02.672520 txhttputil-1.2.9/txhttputil/
+-rw-r--r--   0 jchesney   (501) staff       (20)       24 2023-02-26 05:14:59.000000 txhttputil-1.2.9/txhttputil/__init__.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-02-26 05:15:02.675442 txhttputil-1.2.9/txhttputil/downloader/
+-rw-r--r--   0 jchesney   (501) staff       (20)     2820 2022-01-12 13:58:49.000000 txhttputil-1.2.9/txhttputil/downloader/HttpFileDownloader.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     4568 2022-08-30 02:23:53.000000 txhttputil-1.2.9/txhttputil/downloader/HttpResourceProxy.py
+-rw-r--r--   0 jchesney   (501) staff       (20)        0 2021-09-22 06:19:19.000000 txhttputil-1.2.9/txhttputil/downloader/__init__.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-02-26 05:15:02.676761 txhttputil-1.2.9/txhttputil/login_page/
+-rw-r--r--   0 jchesney   (501) staff       (20)      876 2021-09-22 06:19:19.000000 txhttputil-1.2.9/txhttputil/login_page/LoginElement.py
+-rw-r--r--   0 jchesney   (501) staff       (20)    71705 2021-09-22 06:19:19.000000 txhttputil-1.2.9/txhttputil/login_page/LoginTemplate.xml
+-rw-r--r--   0 jchesney   (501) staff       (20)        0 2021-09-22 06:19:19.000000 txhttputil-1.2.9/txhttputil/login_page/__init__.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-02-26 05:15:02.682839 txhttputil-1.2.9/txhttputil/site/
+-rw-r--r--   0 jchesney   (501) staff       (20)      664 2021-09-22 06:19:19.000000 txhttputil-1.2.9/txhttputil/site/AuthCredentials.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1624 2021-09-22 06:19:19.000000 txhttputil-1.2.9/txhttputil/site/AuthResource.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     8098 2021-09-22 06:19:19.000000 txhttputil-1.2.9/txhttputil/site/AuthSessionWrapper.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1258 2021-09-22 06:19:19.000000 txhttputil-1.2.9/txhttputil/site/AuthUserDetails.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     4498 2021-09-22 06:19:19.000000 txhttputil-1.2.9/txhttputil/site/BasicResource.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     4353 2022-08-14 07:32:40.000000 txhttputil-1.2.9/txhttputil/site/FileUnderlayResource.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     2312 2022-01-12 13:05:11.000000 txhttputil-1.2.9/txhttputil/site/FileUnderlayResourceTest.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     8856 2022-01-12 13:58:49.000000 txhttputil-1.2.9/txhttputil/site/FileUploadRequest.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1085 2021-09-22 06:19:19.000000 txhttputil-1.2.9/txhttputil/site/RedirectToHttpsResource.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      519 2022-08-14 07:32:40.000000 txhttputil-1.2.9/txhttputil/site/RedirectionRule.py
+-rw-r--r--   0 jchesney   (501) staff       (20)       54 2021-09-22 06:19:19.000000 txhttputil-1.2.9/txhttputil/site/ResourceCreator.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      863 2021-09-22 06:19:19.000000 txhttputil-1.2.9/txhttputil/site/RootResource.py
+-rw-r--r--   0 jchesney   (501) staff       (20)        0 2021-09-22 06:19:19.000000 txhttputil-1.2.9/txhttputil/site/RootSiteTest.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     5121 2023-02-26 05:02:48.000000 txhttputil-1.2.9/txhttputil/site/SiteUtil.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     4932 2023-01-10 12:05:27.000000 txhttputil-1.2.9/txhttputil/site/StaticFileResource.py
+-rw-r--r--   0 jchesney   (501) staff       (20)        1 2022-08-14 07:32:35.000000 txhttputil-1.2.9/txhttputil/site/__init__.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-02-26 05:15:02.685208 txhttputil-1.2.9/txhttputil/util/
+-rw-r--r--   0 jchesney   (501) staff       (20)     1263 2021-09-22 06:19:19.000000 txhttputil-1.2.9/txhttputil/util/DeferUtil.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      616 2021-09-22 06:19:19.000000 txhttputil-1.2.9/txhttputil/util/ModuleUtil.py
+-rw-r--r--   0 jchesney   (501) staff       (20)    24790 2022-10-24 03:10:30.000000 txhttputil-1.2.9/txhttputil/util/PemUtil.py
+-rw-r--r--   0 jchesney   (501) staff       (20)    13172 2022-08-30 02:23:53.000000 txhttputil-1.2.9/txhttputil/util/SslUtil.py
+-rw-r--r--   0 jchesney   (501) staff       (20)        0 2021-09-22 06:19:19.000000 txhttputil-1.2.9/txhttputil/util/__init__.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-02-26 05:15:02.674174 txhttputil-1.2.9/txhttputil.egg-info/
+-rw-r--r--   0 jchesney   (501) staff       (20)      439 2023-02-26 05:15:02.000000 txhttputil-1.2.9/txhttputil.egg-info/PKG-INFO
+-rw-r--r--   0 jchesney   (501) staff       (20)     1167 2023-02-26 05:15:02.000000 txhttputil-1.2.9/txhttputil.egg-info/SOURCES.txt
+-rw-r--r--   0 jchesney   (501) staff       (20)        1 2023-02-26 05:15:02.000000 txhttputil-1.2.9/txhttputil.egg-info/dependency_links.txt
+-rw-r--r--   0 jchesney   (501) staff       (20)       66 2023-02-26 05:15:02.000000 txhttputil-1.2.9/txhttputil.egg-info/requires.txt
+-rw-r--r--   0 jchesney   (501) staff       (20)       11 2023-02-26 05:15:02.000000 txhttputil-1.2.9/txhttputil.egg-info/top_level.txt
```

### Comparing `txhttputil-1.2.8/LICENSE` & `txhttputil-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `txhttputil-1.2.8/README.md` & `txhttputil-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `txhttputil-1.2.8/setup.py` & `txhttputil-1.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 package_name = "txhttputil"
-package_version = '1.2.8'
+package_version = '1.2.9'
 
 requirements = [
     "pytz",
     "txwebsocket>=1.0.1",
     "filetype",
     "pem",
     "pytmpdir",
```

### Comparing `txhttputil-1.2.8/txhttputil/downloader/HttpFileDownloader.py` & `txhttputil-1.2.9/txhttputil/downloader/HttpFileDownloader.py`

 * *Files identical despite different names*

### Comparing `txhttputil-1.2.8/txhttputil/downloader/HttpResourceProxy.py` & `txhttputil-1.2.9/txhttputil/downloader/HttpResourceProxy.py`

 * *Files identical despite different names*

### Comparing `txhttputil-1.2.8/txhttputil/login_page/LoginElement.py` & `txhttputil-1.2.9/txhttputil/login_page/LoginElement.py`

 * *Files identical despite different names*

### Comparing `txhttputil-1.2.8/txhttputil/login_page/LoginTemplate.xml` & `txhttputil-1.2.9/txhttputil/login_page/LoginTemplate.xml`

 * *Files identical despite different names*

### Comparing `txhttputil-1.2.8/txhttputil/site/AuthCredentials.py` & `txhttputil-1.2.9/txhttputil/site/AuthCredentials.py`

 * *Files identical despite different names*

### Comparing `txhttputil-1.2.8/txhttputil/site/AuthResource.py` & `txhttputil-1.2.9/txhttputil/site/AuthResource.py`

 * *Files identical despite different names*

### Comparing `txhttputil-1.2.8/txhttputil/site/AuthSessionWrapper.py` & `txhttputil-1.2.9/txhttputil/site/AuthSessionWrapper.py`

 * *Files identical despite different names*

### Comparing `txhttputil-1.2.8/txhttputil/site/AuthUserDetails.py` & `txhttputil-1.2.9/txhttputil/site/AuthUserDetails.py`

 * *Files identical despite different names*

### Comparing `txhttputil-1.2.8/txhttputil/site/BasicResource.py` & `txhttputil-1.2.9/txhttputil/site/BasicResource.py`

 * *Files identical despite different names*

### Comparing `txhttputil-1.2.8/txhttputil/site/FileUnderlayResource.py` & `txhttputil-1.2.9/txhttputil/site/FileUnderlayResource.py`

 * *Files identical despite different names*

### Comparing `txhttputil-1.2.8/txhttputil/site/FileUnderlayResourceTest.py` & `txhttputil-1.2.9/txhttputil/site/FileUnderlayResourceTest.py`

 * *Files identical despite different names*

### Comparing `txhttputil-1.2.8/txhttputil/site/FileUploadRequest.py` & `txhttputil-1.2.9/txhttputil/site/FileUploadRequest.py`

 * *Files identical despite different names*

### Comparing `txhttputil-1.2.8/txhttputil/site/RedirectToHttpsResource.py` & `txhttputil-1.2.9/txhttputil/site/RedirectToHttpsResource.py`

 * *Files identical despite different names*

### Comparing `txhttputil-1.2.8/txhttputil/site/RedirectionRule.py` & `txhttputil-1.2.9/txhttputil/site/RedirectionRule.py`

 * *Files identical despite different names*

### Comparing `txhttputil-1.2.8/txhttputil/site/RootResource.py` & `txhttputil-1.2.9/txhttputil/site/RootResource.py`

 * *Files identical despite different names*

### Comparing `txhttputil-1.2.8/txhttputil/site/SiteUtil.py` & `txhttputil-1.2.9/txhttputil/site/SiteUtil.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,23 +56,37 @@
 ):
     """Setup Site
     Sets up the web site to listen for connections and serve the site.
     Supports customisation of resources based on user details
 
     @return: Port object
     """
-    logger.info(
-        f"setting up http server '{name}' on port {portNum}, "
-        f"with ssl '{'on' if enableSsl else 'off'}', "
-        f"with ssl PEM bundle from '{sslBundleFilePath}', "
-        f"with mTLS '{'on' if enableSsl else 'off'}', "
-        f"with mTLS CA bundle from '{sslMutualTLSCertificateAuthorityBundleFilePath}', "
-        f"with mTLS trusted peer bundle from '{sslMutualTLSTrustedPeerCertificateBundleFilePath}', "
-        f"with Diffie-Hellman parameter from '{dhParamPemFilePath}'"
-    )
+    assert (
+        not sslEnableMutualTLS or enableSsl and sslEnableMutualTLS
+    ), "Mutual TLS only works if the server is using TLS"
+
+    logMsg = f"setting up http server '{name}' on port {portNum}, "
+    logMsg += f"with ssl '{'on' if enableSsl else 'off'}', "
+    if enableSsl:
+        logMsg += f"with ssl PEM bundle from '{sslBundleFilePath}', "
+        logMsg += f"with mTLS '{'on' if sslEnableMutualTLS else 'off'}', "
+        if sslEnableMutualTLS:
+            logMsg += (
+                f"with mTLS CA bundle from"
+                f" '{sslMutualTLSCertificateAuthorityBundleFilePath}', "
+            )
+            logMsg += (
+                f"with mTLS trusted peer bundle from"
+                f" '{sslMutualTLSTrustedPeerCertificateBundleFilePath}', "
+            )
+            logMsg += (
+                f"with Diffie-Hellman parameter from '{dhParamPemFilePath}'"
+            )
+
+    logger.info(logMsg)
     if redirectFromHttpPort is not None:
         setupSite(
             name="%s https redirect" % name,
             rootResource=RedirectToHttpsResource(portNum),
             portNum=redirectFromHttpPort,
             enableLogin=False,
         )
```

### Comparing `txhttputil-1.2.8/txhttputil/site/StaticFileResource.py` & `txhttputil-1.2.9/txhttputil/site/StaticFileResource.py`

 * *Files identical despite different names*

### Comparing `txhttputil-1.2.8/txhttputil/util/DeferUtil.py` & `txhttputil-1.2.9/txhttputil/util/DeferUtil.py`

 * *Files identical despite different names*

### Comparing `txhttputil-1.2.8/txhttputil/util/ModuleUtil.py` & `txhttputil-1.2.9/txhttputil/util/ModuleUtil.py`

 * *Files identical despite different names*

### Comparing `txhttputil-1.2.8/txhttputil/util/PemUtil.py` & `txhttputil-1.2.9/txhttputil/util/PemUtil.py`

 * *Files identical despite different names*

### Comparing `txhttputil-1.2.8/txhttputil/util/SslUtil.py` & `txhttputil-1.2.9/txhttputil/util/SslUtil.py`

 * *Files identical despite different names*

### Comparing `txhttputil-1.2.8/txhttputil.egg-info/SOURCES.txt` & `txhttputil-1.2.9/txhttputil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

