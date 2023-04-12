# Comparing `tmp/shellviz-0.1.5.tar.gz` & `tmp/shellviz-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/shellviz-0.1.5.tar", last modified: Tue Nov 27 08:11:42 2018, max compression
+gzip compressed data, was "shellviz-0.1.6.tar", max compression
```

## Comparing `shellviz-0.1.5.tar` & `shellviz-0.1.6.tar`

### file list

```diff
@@ -1,11 +1,5 @@
-drwxr-xr-x   0 jms        (501) staff       (20)        0 2018-11-27 08:11:42.000000 shellviz-0.1.5/
--rw-r--r--   0 jms        (501) staff       (20)      303 2018-11-27 08:11:42.000000 shellviz-0.1.5/PKG-INFO
--rw-r--r--   0 jms        (501) staff       (20)       38 2018-11-27 08:11:42.000000 shellviz-0.1.5/setup.cfg
--rw-r--r--   0 jms        (501) staff       (20)      390 2018-11-23 01:57:42.000000 shellviz-0.1.5/setup.py
-drwxr-xr-x   0 jms        (501) staff       (20)        0 2018-11-27 08:11:42.000000 shellviz-0.1.5/shellviz/
--rw-r--r--   0 jms        (501) staff       (20)     1616 2018-11-23 01:57:42.000000 shellviz-0.1.5/shellviz/__init__.py
-drwxr-xr-x   0 jms        (501) staff       (20)        0 2018-11-27 08:11:42.000000 shellviz-0.1.5/shellviz.egg-info/
--rw-r--r--   0 jms        (501) staff       (20)      303 2018-11-27 08:11:42.000000 shellviz-0.1.5/shellviz.egg-info/PKG-INFO
--rw-r--r--   0 jms        (501) staff       (20)      157 2018-11-27 08:11:42.000000 shellviz-0.1.5/shellviz.egg-info/SOURCES.txt
--rw-r--r--   0 jms        (501) staff       (20)        1 2018-11-27 08:11:42.000000 shellviz-0.1.5/shellviz.egg-info/dependency_links.txt
--rw-r--r--   0 jms        (501) staff       (20)        9 2018-11-27 08:11:42.000000 shellviz-0.1.5/shellviz.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1060 2023-04-12 06:44:46.797833 shellviz-0.1.6/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-04-12 06:44:46.797887 shellviz-0.1.6/README.md
+-rw-r--r--   0        0        0      328 2023-04-12 07:00:13.423040 shellviz-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1377 2023-04-12 07:00:06.750786 shellviz-0.1.6/shellviz/__init__.py
+-rw-r--r--   0        0        0      289 1970-01-01 00:00:00.000000 shellviz-0.1.6/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `shellviz-0.1.5/shellviz/__init__.py` & `shellviz-0.1.6/shellviz/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import urllib.request, urllib.parse, urllib.error
 import json
 import os
 from uuid import getnode as get_mac
 
-VERSION = '0.1.5'
-
-class ShellvizConnectionException(Exception):
-    pass
+VERSION = '0.1.6'
 
 def visualize(data, id=None):
 
     try:
         from django.db.models import QuerySet
         from django.db.models import Model
         from django.core import serializers
@@ -24,29 +21,25 @@
             data = [data]
         elif isinstance(data, QuerySet):
             data = list(data)
         if isinstance(data, list) and len(data) and isinstance(data[0], Model):
             data = json.loads(serializers.serialize('json', data))
             data = [serialized_model['fields'] for serialized_model in data]
 
-    shellviz_root = os.environ.get('SHELLVIZ_ROOT', 'http://localhost:3384')  # 'http://shellviz.com'
-    url = '%s/visualize' % shellviz_root
+    shellviz_root = os.environ.get('SHELLVIZ_ROOT', 'https://shellviz.com')
+    url = '%s/api/visualize' % shellviz_root
 
     api_key = os.environ.get('SHELLVIZ_API_KEY', '')
     mac_address = get_mac() or ''
 
     request_dict = {
         'data': json.dumps(data),
         'apiKey': api_key,
         'macAddress': mac_address,
         'libraryLanguage': 'python',
         'libraryVersion': VERSION
     }
     request_dict.update({'id': id} if id else {})
     request_str = urllib.parse.urlencode(request_dict).encode('utf-8')
 
-    try:
-        req = urllib.request.urlopen(url, request_str)
-    except urllib.error.URLError:
-        raise ShellvizConnectionException('Cannot connect to shellviz client', {'SHELLVIZ_ROOT': shellviz_root})
-
+    req = urllib.request.urlopen(url, request_str)
     return req.read()
```

