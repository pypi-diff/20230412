# Comparing `tmp/fenrirWeb-0.3.0.tar.gz` & `tmp/fenrirWeb-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenrirWeb-0.3.0.tar", last modified: Mon Apr 10 10:36:35 2023, max compression
+gzip compressed data, was "fenrirWeb-0.4.0.tar", last modified: Wed Apr 12 19:51:06 2023, max compression
```

## Comparing `fenrirWeb-0.3.0.tar` & `fenrirWeb-0.4.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-10 10:36:35.073625 fenrirWeb-0.3.0/
--rw-r--r--   0 hannes    (1000) users      (100)    18092 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/LICENSE
--rw-r--r--   0 hannes    (1000) users      (100)       80 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/MANIFEST.in
--rw-r--r--   0 hannes    (1000) users      (100)      340 2023-04-10 10:36:35.073625 fenrirWeb-0.3.0/PKG-INFO
--rw-r--r--   0 hannes    (1000) users      (100)      676 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/README.md
-drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-10 10:36:35.069625 fenrirWeb-0.3.0/fenrirWeb/
--rw-r--r--   0 hannes    (1000) users      (100)       22 2023-04-10 10:35:45.000000 fenrirWeb-0.3.0/fenrirWeb/__init__.py
--rw-r--r--   0 hannes    (1000) users      (100)    17010 2023-04-10 10:32:49.000000 fenrirWeb-0.3.0/fenrirWeb/lib.py
--rw-r--r--   0 hannes    (1000) users      (100)     1052 2023-04-10 10:34:59.000000 fenrirWeb-0.3.0/fenrirWeb/main.py
-drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-10 10:36:35.073625 fenrirWeb-0.3.0/fenrirWeb/static/
--rw-r--r--   0 hannes    (1000) users      (100)    80420 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/static/bootstrap.bundle.min.js
--rw-r--r--   0 hannes    (1000) users      (100)   194901 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/static/bootstrap.min.css
--rw-r--r--   0 hannes    (1000) users      (100)    60404 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/static/bootstrap.min.js
--rw-r--r--   0 hannes    (1000) users      (100)     9369 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/static/disabled.png
--rw-r--r--   0 hannes    (1000) users      (100)    20270 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/static/disabled.svg
--rw-r--r--   0 hannes    (1000) users      (100)     8004 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/static/enabled.png
--rw-r--r--   0 hannes    (1000) users      (100)    28344 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/static/enabled.svg
--rw-r--r--   0 hannes    (1000) users      (100)    93062 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/static/favicon.ico
--rw-r--r--   0 hannes    (1000) users      (100)    13258 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/static/fenrir.js
--rw-r--r--   0 hannes    (1000) users      (100)     2104 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/static/settings.png
--rw-r--r--   0 hannes    (1000) users      (100)     9046 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/view_config.py
--rw-r--r--   0 hannes    (1000) users      (100)     3152 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/view_main.py
-drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-10 10:36:35.073625 fenrirWeb-0.3.0/fenrirWeb/views/
--rw-r--r--   0 hannes    (1000) users      (100)     3046 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/views/changepassword.tpl
--rw-r--r--   0 hannes    (1000) users      (100)     2547 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/views/createpassword.tpl
--rw-r--r--   0 hannes    (1000) users      (100)     3064 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/views/index.tpl
--rw-r--r--   0 hannes    (1000) users      (100)     1697 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/views/mappinginput.tpl
--rw-r--r--   0 hannes    (1000) users      (100)      939 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/views/navbar.tpl
--rw-r--r--   0 hannes    (1000) users      (100)     8286 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/views/settings.tpl
--rw-r--r--   0 hannes    (1000) users      (100)     2501 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/fenrirWeb/views/vpninput.tpl
-drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-10 10:36:35.069625 fenrirWeb-0.3.0/fenrirWeb.egg-info/
--rw-r--r--   0 hannes    (1000) users      (100)      340 2023-04-10 10:36:35.000000 fenrirWeb-0.3.0/fenrirWeb.egg-info/PKG-INFO
--rw-r--r--   0 hannes    (1000) users      (100)      903 2023-04-10 10:36:35.000000 fenrirWeb-0.3.0/fenrirWeb.egg-info/SOURCES.txt
--rw-r--r--   0 hannes    (1000) users      (100)        1 2023-04-10 10:36:35.000000 fenrirWeb-0.3.0/fenrirWeb.egg-info/dependency_links.txt
--rw-r--r--   0 hannes    (1000) users      (100)       50 2023-04-10 10:36:35.000000 fenrirWeb-0.3.0/fenrirWeb.egg-info/entry_points.txt
--rw-r--r--   0 hannes    (1000) users      (100)        1 2023-04-10 10:16:52.000000 fenrirWeb-0.3.0/fenrirWeb.egg-info/not-zip-safe
--rw-r--r--   0 hannes    (1000) users      (100)       32 2023-04-10 10:36:35.000000 fenrirWeb-0.3.0/fenrirWeb.egg-info/requires.txt
--rw-r--r--   0 hannes    (1000) users      (100)       10 2023-04-10 10:36:35.000000 fenrirWeb-0.3.0/fenrirWeb.egg-info/top_level.txt
--rw-r--r--   0 hannes    (1000) users      (100)       38 2023-04-10 10:36:35.073625 fenrirWeb-0.3.0/setup.cfg
--rw-r--r--   0 hannes    (1000) users      (100)      693 2023-04-10 10:16:19.000000 fenrirWeb-0.3.0/setup.py
+drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-12 19:51:06.145783 fenrirWeb-0.4.0/
+-rw-r--r--   0 hannes    (1000) users      (100)    18092 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/LICENSE
+-rw-r--r--   0 hannes    (1000) users      (100)       80 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/MANIFEST.in
+-rw-r--r--   0 hannes    (1000) users      (100)      340 2023-04-12 19:51:06.145783 fenrirWeb-0.4.0/PKG-INFO
+-rw-r--r--   0 hannes    (1000) users      (100)      765 2023-04-10 10:59:05.000000 fenrirWeb-0.4.0/README.md
+drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-12 19:51:06.137783 fenrirWeb-0.4.0/fenrirWeb/
+-rw-r--r--   0 hannes    (1000) users      (100)       22 2023-04-11 19:55:18.000000 fenrirWeb-0.4.0/fenrirWeb/__init__.py
+-rw-r--r--   0 hannes    (1000) users      (100)    16875 2023-04-11 21:45:56.000000 fenrirWeb-0.4.0/fenrirWeb/lib.py
+-rw-r--r--   0 hannes    (1000) users      (100)     1052 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/main.py
+drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-12 19:51:06.141783 fenrirWeb-0.4.0/fenrirWeb/static/
+-rw-r--r--   0 hannes    (1000) users      (100)    80420 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/static/bootstrap.bundle.min.js
+-rw-r--r--   0 hannes    (1000) users      (100)   194901 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/static/bootstrap.min.css
+-rw-r--r--   0 hannes    (1000) users      (100)    60404 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/static/bootstrap.min.js
+-rw-r--r--   0 hannes    (1000) users      (100)     9369 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/static/disabled.png
+-rw-r--r--   0 hannes    (1000) users      (100)    20270 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/static/disabled.svg
+-rw-r--r--   0 hannes    (1000) users      (100)     8004 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/static/enabled.png
+-rw-r--r--   0 hannes    (1000) users      (100)    28344 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/static/enabled.svg
+-rw-r--r--   0 hannes    (1000) users      (100)    93062 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/static/favicon.ico
+-rw-r--r--   0 hannes    (1000) users      (100)    13258 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/static/fenrir.js
+-rw-r--r--   0 hannes    (1000) users      (100)     2104 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/static/settings.png
+-rw-r--r--   0 hannes    (1000) users      (100)     9046 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/view_config.py
+-rw-r--r--   0 hannes    (1000) users      (100)     3152 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/view_main.py
+drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-12 19:51:06.145783 fenrirWeb-0.4.0/fenrirWeb/views/
+-rw-r--r--   0 hannes    (1000) users      (100)     3046 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/views/changepassword.tpl
+-rw-r--r--   0 hannes    (1000) users      (100)     2547 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/views/createpassword.tpl
+-rw-r--r--   0 hannes    (1000) users      (100)     3064 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/views/index.tpl
+-rw-r--r--   0 hannes    (1000) users      (100)     1697 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/views/mappinginput.tpl
+-rw-r--r--   0 hannes    (1000) users      (100)      939 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/views/navbar.tpl
+-rw-r--r--   0 hannes    (1000) users      (100)     8286 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/views/settings.tpl
+-rw-r--r--   0 hannes    (1000) users      (100)     2501 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/views/vpninput.tpl
+drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-12 19:51:06.137783 fenrirWeb-0.4.0/fenrirWeb.egg-info/
+-rw-r--r--   0 hannes    (1000) users      (100)      340 2023-04-12 19:51:06.000000 fenrirWeb-0.4.0/fenrirWeb.egg-info/PKG-INFO
+-rw-r--r--   0 hannes    (1000) users      (100)      903 2023-04-12 19:51:06.000000 fenrirWeb-0.4.0/fenrirWeb.egg-info/SOURCES.txt
+-rw-r--r--   0 hannes    (1000) users      (100)        1 2023-04-12 19:51:06.000000 fenrirWeb-0.4.0/fenrirWeb.egg-info/dependency_links.txt
+-rw-r--r--   0 hannes    (1000) users      (100)       50 2023-04-12 19:51:06.000000 fenrirWeb-0.4.0/fenrirWeb.egg-info/entry_points.txt
+-rw-r--r--   0 hannes    (1000) users      (100)        1 2023-04-10 10:16:52.000000 fenrirWeb-0.4.0/fenrirWeb.egg-info/not-zip-safe
+-rw-r--r--   0 hannes    (1000) users      (100)       32 2023-04-12 19:51:06.000000 fenrirWeb-0.4.0/fenrirWeb.egg-info/requires.txt
+-rw-r--r--   0 hannes    (1000) users      (100)       10 2023-04-12 19:51:06.000000 fenrirWeb-0.4.0/fenrirWeb.egg-info/top_level.txt
+-rw-r--r--   0 hannes    (1000) users      (100)       38 2023-04-12 19:51:06.145783 fenrirWeb-0.4.0/setup.cfg
+-rw-r--r--   0 hannes    (1000) users      (100)      693 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/setup.py
```

### Comparing `fenrirWeb-0.3.0/LICENSE` & `fenrirWeb-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.3.0/README.md` & `fenrirWeb-0.4.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 
 ## Introduction
 Fenrir provides a user friendly way to route all traffic from configured trough a VPN tunnel.
 
 FenrirWeb is a webinterface for viewing/ configuring fenrir.
 Configuration is stored in `/var/cache/fenrir/fenrir.db`
 
+## Screenshots
+![Slideshow](https://hanneshofer.github.io/fenrirWeb/images/screens.gif)
+
 ## Installation
 Fenrir is a pure python3 application. (3.6+)
 
 ### pip releases
 ```sh
 > pip install fenrirweb
 > fenrirweb --help
```

### Comparing `fenrirWeb-0.3.0/fenrirWeb/lib.py` & `fenrirWeb-0.4.0/fenrirWeb/lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from bottle import TEMPLATE_PATH
 from sqlite3 import connect, OperationalError
 from os.path import dirname, realpath, exists
 from logging import debug
 from bcrypt import gensalt, hashpw
-from fenrir.filehandler import filehandler
-from fenrir.fenrir import Fenrir
+from fenrircore.filehandler import filehandler
+from fenrircore.fenrir import Fenrir
 from json import loads, dumps
 from os import O_RDWR, O_NONBLOCK, fdopen, open as osopen
 from select import select
 from time import sleep
-from cryptography.fernet import InvalidToken
 
 APPPATH = dirname(realpath(__file__))
 TEMPLATE_PATH[:] = [f'{APPPATH}/views']
 DBPATH = '/var/cache/fenrir/fenrir.sqlite'
 NEEDSPASSWORDCHECK = False
 
 
@@ -244,19 +243,19 @@
                 valuedict['profilename'] = result[0]
                 valuedict['description'] = result[1]
                 valuedict['isdefault'] = result[2]
                 valuedict['ondemand'] = result[3]
                 if getauth:
                     try:
                         fh = filehandler(passphrase=passphrase)
-                        valuedict['username'] = fh.decode(result[4].decode('utf-8')).decode('utf-8')
-                        valuedict['password'] = fh.decode(result[5].decode('utf-8')).decode('utf-8')
-                        valuedict['vpnconfig'] = fh.decode(result[6].decode('utf-8')).decode('utf-8')
+                        valuedict['username'] = fh.decode(result[4])
+                        valuedict['password'] = fh.decode(result[5])
+                        valuedict['vpnconfig'] = fh.decode(result[6])
                         valuedict['vpnprofileid'] = result[7]
-                    except InvalidToken:
+                    except ValueError:
                         if passphrase:
                             return getvpnconfig(profilename=profilename, getauth=getauth, dbpath=dbpath, passphrase=None)
                 returndict[f'profile{i}'] = valuedict.copy()
     except OperationalError as e:
         debug(f'unable to query Database {dbpath}: {e}')
 
     return returndict
```

### Comparing `fenrirWeb-0.3.0/fenrirWeb/main.py` & `fenrirWeb-0.4.0/fenrirWeb/main.py`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.3.0/fenrirWeb/static/bootstrap.bundle.min.js` & `fenrirWeb-0.4.0/fenrirWeb/static/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.3.0/fenrirWeb/static/bootstrap.min.css` & `fenrirWeb-0.4.0/fenrirWeb/static/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.3.0/fenrirWeb/static/bootstrap.min.js` & `fenrirWeb-0.4.0/fenrirWeb/static/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.3.0/fenrirWeb/static/disabled.png` & `fenrirWeb-0.4.0/fenrirWeb/static/disabled.png`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.3.0/fenrirWeb/static/disabled.svg` & `fenrirWeb-0.4.0/fenrirWeb/static/disabled.svg`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.3.0/fenrirWeb/static/enabled.png` & `fenrirWeb-0.4.0/fenrirWeb/static/enabled.png`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.3.0/fenrirWeb/static/enabled.svg` & `fenrirWeb-0.4.0/fenrirWeb/static/enabled.svg`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.3.0/fenrirWeb/static/favicon.ico` & `fenrirWeb-0.4.0/fenrirWeb/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.3.0/fenrirWeb/static/fenrir.js` & `fenrirWeb-0.4.0/fenrirWeb/static/fenrir.js`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.3.0/fenrirWeb/static/settings.png` & `fenrirWeb-0.4.0/fenrirWeb/static/settings.png`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.3.0/fenrirWeb/view_config.py` & `fenrirWeb-0.4.0/fenrirWeb/view_config.py`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.3.0/fenrirWeb/view_main.py` & `fenrirWeb-0.4.0/fenrirWeb/view_main.py`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.3.0/fenrirWeb/views/changepassword.tpl` & `fenrirWeb-0.4.0/fenrirWeb/views/changepassword.tpl`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.3.0/fenrirWeb/views/createpassword.tpl` & `fenrirWeb-0.4.0/fenrirWeb/views/createpassword.tpl`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.3.0/fenrirWeb/views/index.tpl` & `fenrirWeb-0.4.0/fenrirWeb/views/index.tpl`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.3.0/fenrirWeb/views/mappinginput.tpl` & `fenrirWeb-0.4.0/fenrirWeb/views/mappinginput.tpl`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.3.0/fenrirWeb/views/navbar.tpl` & `fenrirWeb-0.4.0/fenrirWeb/views/navbar.tpl`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.3.0/fenrirWeb/views/settings.tpl` & `fenrirWeb-0.4.0/fenrirWeb/views/settings.tpl`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.3.0/fenrirWeb/views/vpninput.tpl` & `fenrirWeb-0.4.0/fenrirWeb/views/vpninput.tpl`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.3.0/fenrirWeb.egg-info/SOURCES.txt` & `fenrirWeb-0.4.0/fenrirWeb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.3.0/setup.py` & `fenrirWeb-0.4.0/setup.py`

 * *Files identical despite different names*

