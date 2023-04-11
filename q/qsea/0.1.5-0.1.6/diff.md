# Comparing `tmp/qsea-0.1.5.tar.gz` & `tmp/qsea-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\qsea-0.1.5.tar", last modified: Tue Apr 11 22:28:14 2023, max compression
+gzip compressed data, was "dist\qsea-0.1.6.tar", last modified: Tue Apr 11 22:32:00 2023, max compression
```

## Comparing `qsea-0.1.5.tar` & `qsea-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 22:28:14.313572 qsea-0.1.5/
--rw-rw-rw-   0        0        0     1061 2023-01-13 17:31:55.000000 qsea-0.1.5/LICENSE.txt
--rw-rw-rw-   0        0        0      606 2023-04-11 22:28:14.311491 qsea-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-01-13 17:37:30.000000 qsea-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 22:28:14.296498 qsea-0.1.5/qsea/
--rw-rw-rw-   0        0        0    61127 2023-04-11 22:27:08.000000 qsea-0.1.5/qsea/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 22:28:14.310491 qsea-0.1.5/qsea.egg-info/
--rw-rw-rw-   0        0        0      606 2023-04-11 22:28:13.000000 qsea-0.1.5/qsea.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2023-04-11 22:28:13.000000 qsea-0.1.5/qsea.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 22:28:13.000000 qsea-0.1.5/qsea.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-11 22:28:13.000000 qsea-0.1.5/qsea.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-11 22:28:13.000000 qsea-0.1.5/qsea.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 22:28:14.313572 qsea-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      829 2023-04-11 22:27:32.000000 qsea-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 22:32:00.237865 qsea-0.1.6/
+-rw-rw-rw-   0        0        0     1061 2023-01-13 17:31:55.000000 qsea-0.1.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      606 2023-04-11 22:32:00.235784 qsea-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-01-13 17:37:30.000000 qsea-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 22:32:00.222792 qsea-0.1.6/qsea/
+-rw-rw-rw-   0        0        0    61145 2023-04-11 22:30:58.000000 qsea-0.1.6/qsea/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 22:32:00.234783 qsea-0.1.6/qsea.egg-info/
+-rw-rw-rw-   0        0        0      606 2023-04-11 22:31:59.000000 qsea-0.1.6/qsea.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2023-04-11 22:31:59.000000 qsea-0.1.6/qsea.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 22:31:59.000000 qsea-0.1.6/qsea.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-04-11 22:31:59.000000 qsea-0.1.6/qsea.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-11 22:31:59.000000 qsea-0.1.6/qsea.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 22:32:00.237865 qsea-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      842 2023-04-11 22:31:48.000000 qsea-0.1.6/setup.py
```

### Comparing `qsea-0.1.5/LICENSE.txt` & `qsea-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qsea-0.1.5/PKG-INFO` & `qsea-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsea
-Version: 0.1.5
+Version: 0.1.6
 Summary: Convenient way to work with Qlik Sense Engine API from Python
 Home-page: https://github.com/ncthuc/qsea
 Download-URL: https://pypi.org/project/qsea/
 Author: Lev Biriukov
 Author-email: lbiryukov@gmail.com
 License: MIT
 Keywords: QlikSense,Qlik
```

### Comparing `qsea-0.1.5/qsea/__init__.py` & `qsea-0.1.6/qsea/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 #!/usr/bin/env python
 # coding: utf-8
 
-# In[1]:
+# In[77]:
 
 
 # beta-версия к публикации
 
 import json
 import pandas as pd
 import datetime as dt
 import logging
+import websocket
 
 
-# In[47]:
+# In[78]:
 
 
 # version 0.1.12-04-23
 
 def OpenConnection(qlik_url, header_user, timeout = 10):
     #to refine: review the overall config
     ws = websocket.create_connection(qlik_url, sslopt={"cert_reqs": ssl.CERT_NONE},header=header_user, timeout = timeout)
```

### Comparing `qsea-0.1.5/qsea.egg-info/PKG-INFO` & `qsea-0.1.6/qsea.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsea
-Version: 0.1.5
+Version: 0.1.6
 Summary: Convenient way to work with Qlik Sense Engine API from Python
 Home-page: https://github.com/ncthuc/qsea
 Download-URL: https://pypi.org/project/qsea/
 Author: Lev Biriukov
 Author-email: lbiryukov@gmail.com
 License: MIT
 Keywords: QlikSense,Qlik
```

### Comparing `qsea-0.1.5/setup.py` & `qsea-0.1.6/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,24 +3,24 @@
     README = readme_file.read()
 
 with open('HISTORY.md') as history_file:
     HISTORY = history_file.read()
 
 setup_args = dict(
     name='qsea',
-    version='0.1.5',
+    version='0.1.6',
     description='Convenient way to work with Qlik Sense Engine API from Python',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY,
     license='MIT',
     packages=find_packages(),
     author='Lev Biriukov',
     author_email='lbiryukov@gmail.com',
     keywords=['QlikSense', 'Qlik'],
     url='https://github.com/ncthuc/qsea',
     download_url='https://pypi.org/project/qsea/'
 )
 
-install_requires = ['pandas', 'datetime']
+install_requires = ['pandas', 'datetime', 'websocket']
 
 if __name__ == '__main__':
     setup(**setup_args, install_requires=install_requires)
```

