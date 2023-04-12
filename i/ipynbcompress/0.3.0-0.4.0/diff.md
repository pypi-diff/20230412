# Comparing `tmp/ipynbcompress-0.3.0.tar.gz` & `tmp/ipynbcompress-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ipynbcompress-0.3.0.tar", last modified: Sat May  2 06:04:31 2015, max compression
+gzip compressed data, was "ipynbcompress-0.4.0.tar", last modified: Wed Apr 12 19:37:31 2023, max compression
```

## Comparing `ipynbcompress-0.3.0.tar` & `ipynbcompress-0.4.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 arve       (501) staff       (20)        0 2015-05-02 06:04:31.000000 ipynbcompress-0.3.0/
--rw-r--r--   0 arve       (501) staff       (20)      415 2015-04-23 09:14:25.000000 ipynbcompress-0.3.0/.gitignore
--rw-r--r--   0 arve       (501) staff       (20)      137 2015-04-23 08:24:29.000000 ipynbcompress-0.3.0/.travis.yml
-drwxr-xr-x   0 arve       (501) staff       (20)        0 2015-05-02 06:04:31.000000 ipynbcompress-0.3.0/docs/
--rw-r--r--   0 arve       (501) staff       (20)     8193 2015-04-23 08:24:29.000000 ipynbcompress-0.3.0/docs/conf.py
--rw-r--r--   0 arve       (501) staff       (20)      148 2015-04-23 08:24:29.000000 ipynbcompress-0.3.0/docs/index.rst
--rw-r--r--   0 arve       (501) staff       (20)      132 2015-04-23 11:02:35.000000 ipynbcompress-0.3.0/docs/ipynbcompress.rst
--rw-r--r--   0 arve       (501) staff       (20)     6467 2015-04-23 08:24:29.000000 ipynbcompress-0.3.0/docs/make.bat
--rw-r--r--   0 arve       (501) staff       (20)     6778 2015-04-23 08:24:29.000000 ipynbcompress-0.3.0/docs/Makefile
--rw-r--r--   0 arve       (501) staff       (20)       76 2015-04-23 11:02:16.000000 ipynbcompress-0.3.0/docs/modules.rst
--rw-r--r--   0 arve       (501) staff       (20)       44 2015-04-23 08:24:29.000000 ipynbcompress-0.3.0/docs/requirements.txt
-drwxr-xr-x   0 arve       (501) staff       (20)        0 2015-05-02 06:04:31.000000 ipynbcompress-0.3.0/ipynbcompress/
--rw-r--r--   0 arve       (501) staff       (20)      230 2015-04-23 09:09:37.000000 ipynbcompress-0.3.0/ipynbcompress/__init__.py
--rw-r--r--   0 arve       (501) staff       (20)     2490 2015-05-02 05:36:04.000000 ipynbcompress-0.3.0/ipynbcompress/ipynbcompress.py
--rw-r--r--   0 arve       (501) staff       (20)        6 2015-05-02 06:04:12.000000 ipynbcompress-0.3.0/ipynbcompress/VERSION
-drwxr-xr-x   0 arve       (501) staff       (20)        0 2015-05-02 06:04:31.000000 ipynbcompress-0.3.0/ipynbcompress.egg-info/
--rw-r--r--   0 arve       (501) staff       (20)        1 2015-05-02 06:04:29.000000 ipynbcompress-0.3.0/ipynbcompress.egg-info/dependency_links.txt
--rw-r--r--   0 arve       (501) staff       (20)        1 2015-05-02 06:04:29.000000 ipynbcompress-0.3.0/ipynbcompress.egg-info/not-zip-safe
--rw-r--r--   0 arve       (501) staff       (20)     3599 2015-05-02 06:04:29.000000 ipynbcompress-0.3.0/ipynbcompress.egg-info/PKG-INFO
--rw-r--r--   0 arve       (501) staff       (20)       49 2015-05-02 06:04:29.000000 ipynbcompress-0.3.0/ipynbcompress.egg-info/requires.txt
--rw-r--r--   0 arve       (501) staff       (20)      608 2015-05-02 06:04:31.000000 ipynbcompress-0.3.0/ipynbcompress.egg-info/SOURCES.txt
--rw-r--r--   0 arve       (501) staff       (20)       14 2015-05-02 06:04:29.000000 ipynbcompress-0.3.0/ipynbcompress.egg-info/top_level.txt
--rw-r--r--   0 arve       (501) staff       (20)     1079 2015-04-23 08:24:29.000000 ipynbcompress-0.3.0/LICENSE
--rw-r--r--   0 arve       (501) staff       (20)     1407 2015-04-23 08:24:29.000000 ipynbcompress-0.3.0/Makefile
--rw-r--r--   0 arve       (501) staff       (20)     3599 2015-05-02 06:04:31.000000 ipynbcompress-0.3.0/PKG-INFO
--rw-r--r--   0 arve       (501) staff       (20)     1895 2015-04-23 16:01:57.000000 ipynbcompress-0.3.0/README.md
--rw-r--r--   0 arve       (501) staff       (20)     2180 2015-05-02 06:04:29.000000 ipynbcompress-0.3.0/README.rst
--rw-r--r--   0 arve       (501) staff       (20)       96 2015-04-23 08:24:29.000000 ipynbcompress-0.3.0/requirements.txt
-drwxr-xr-x   0 arve       (501) staff       (20)        0 2015-05-02 06:04:31.000000 ipynbcompress-0.3.0/scripts/
--rwxr-xr-x   0 arve       (501) staff       (20)     2186 2015-05-02 06:02:23.000000 ipynbcompress-0.3.0/scripts/ipynb-compress
--rw-r--r--   0 arve       (501) staff       (20)       82 2015-05-02 06:04:31.000000 ipynbcompress-0.3.0/setup.cfg
--rwxr-xr-x   0 arve       (501) staff       (20)     1388 2015-04-23 13:32:43.000000 ipynbcompress-0.3.0/setup.py
-drwxr-xr-x   0 arve       (501) staff       (20)        0 2015-05-02 06:04:31.000000 ipynbcompress-0.3.0/test/
--rw-r--r--   0 arve       (501) staff       (20)   977054 2015-05-02 05:53:23.000000 ipynbcompress-0.3.0/test/notebook3.ipynb
--rwxr-xr-x   0 arve       (501) staff       (20) 11563736 2015-04-23 16:01:14.000000 ipynbcompress-0.3.0/test/notebook4.ipynb
--rwxr-xr-x   0 arve       (501) staff       (20)      949 2015-04-23 15:50:05.000000 ipynbcompress-0.3.0/test/test_compress.py
--rw-r--r--   0 arve       (501) staff       (20)      211 2015-04-23 08:24:29.000000 ipynbcompress-0.3.0/tox.ini
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-12 19:37:31.960601 ipynbcompress-0.4.0/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-12 19:37:31.520131 ipynbcompress-0.4.0/.devcontainer/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      977 2023-04-12 19:26:49.000000 ipynbcompress-0.4.0/.devcontainer/devcontainer.json
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      410 2023-04-12 19:26:49.000000 ipynbcompress-0.4.0/.gitignore
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      126 2023-04-12 19:26:49.000000 ipynbcompress-0.4.0/.travis.yml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1079 2021-02-10 18:01:48.000000 ipynbcompress-0.4.0/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1342 2023-04-12 19:37:28.000000 ipynbcompress-0.4.0/Makefile
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3302 2023-04-12 19:37:31.961870 ipynbcompress-0.4.0/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2467 2023-04-12 19:26:49.000000 ipynbcompress-0.4.0/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2742 2023-04-12 19:37:31.000000 ipynbcompress-0.4.0/README.rst
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-12 19:37:31.557229 ipynbcompress-0.4.0/docs/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6778 2021-02-10 18:01:48.000000 ipynbcompress-0.4.0/docs/Makefile
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8193 2021-02-10 18:01:48.000000 ipynbcompress-0.4.0/docs/conf.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      148 2021-02-10 18:01:48.000000 ipynbcompress-0.4.0/docs/index.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      132 2021-02-10 18:01:48.000000 ipynbcompress-0.4.0/docs/ipynbcompress.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6467 2021-02-10 18:01:48.000000 ipynbcompress-0.4.0/docs/make.bat
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       76 2021-02-10 18:01:48.000000 ipynbcompress-0.4.0/docs/modules.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       44 2023-04-12 19:17:47.000000 ipynbcompress-0.4.0/docs/requirements.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-12 19:37:31.572091 ipynbcompress-0.4.0/ipynbcompress/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        6 2023-04-12 19:26:49.000000 ipynbcompress-0.4.0/ipynbcompress/VERSION
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      230 2021-02-10 18:01:48.000000 ipynbcompress-0.4.0/ipynbcompress/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2564 2023-04-12 19:26:49.000000 ipynbcompress-0.4.0/ipynbcompress/ipynbcompress.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-12 19:37:31.609470 ipynbcompress-0.4.0/ipynbcompress.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3302 2023-04-12 19:37:31.000000 ipynbcompress-0.4.0/ipynbcompress.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      632 2023-04-12 19:37:31.000000 ipynbcompress-0.4.0/ipynbcompress.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-04-12 19:37:31.000000 ipynbcompress-0.4.0/ipynbcompress.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-04-12 19:33:23.000000 ipynbcompress-0.4.0/ipynbcompress.egg-info/not-zip-safe
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       49 2023-04-12 19:37:31.000000 ipynbcompress-0.4.0/ipynbcompress.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       14 2023-04-12 19:37:31.000000 ipynbcompress-0.4.0/ipynbcompress.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      101 2023-04-12 19:26:49.000000 ipynbcompress-0.4.0/requirements.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-12 19:37:31.614672 ipynbcompress-0.4.0/scripts/
+-rwxr-xr-x   0 vscode    (1000) vscode    (1000)     2186 2023-04-12 18:45:14.000000 ipynbcompress-0.4.0/scripts/ipynb-compress
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       61 2023-04-12 19:37:31.965649 ipynbcompress-0.4.0/setup.cfg
+-rwxr-xr-x   0 vscode    (1000) vscode    (1000)     1292 2023-04-12 19:34:36.000000 ipynbcompress-0.4.0/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-12 19:37:31.957727 ipynbcompress-0.4.0/test/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)   977054 2021-02-10 18:01:48.000000 ipynbcompress-0.4.0/test/notebook3.ipynb
+-rwxr-xr-x   0 vscode    (1000) vscode    (1000) 11563736 2021-02-10 18:01:48.000000 ipynbcompress-0.4.0/test/notebook4.ipynb
+-rwxr-xr-x   0 vscode    (1000) vscode    (1000)      948 2023-04-12 19:26:49.000000 ipynbcompress-0.4.0/test/test_compress.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ipynbcompress-0.3.0/docs/conf.py` & `ipynbcompress-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ipynbcompress-0.3.0/docs/make.bat` & `ipynbcompress-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ipynbcompress-0.3.0/docs/Makefile` & `ipynbcompress-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ipynbcompress-0.3.0/ipynbcompress/ipynbcompress.py` & `ipynbcompress-0.4.0/ipynbcompress/ipynbcompress.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 from base64 import b64decode, b64encode
 from PIL import Image
 from io import BytesIO
 from os import stat
-from IPython.nbformat import read, write
+from nbformat import read, write
 
 
 def compress(filename, output_filename=None, img_width=2048, img_format='png'):
     """Compress images in IPython notebooks.
 
     Parameters
     ----------
@@ -36,27 +36,28 @@
     outputs = [o for o in outputs if len(o)]
     # flatten
     outputs = [o for lines in outputs for o in lines]
     for output in outputs:
         data = output.get('data', {})
         if not data:
             continue
-        keys = data.keys()
+        keys = data.copy().keys()
         for key in keys:
             if 'image' in key:
                 string = ''.join(data[key])
                 bytes_img = b64decode(string)
                 io_img = BytesIO(bytes_img)
                 img = Image.open(io_img)
                 factor = float(img_width) / img.size[0]
                 if factor < 1:
                     # only resize large images
                     new_size = [int(s*factor+0.5) for s in img.size]
                     img = img.resize(new_size)
                 out = BytesIO()
+                img = img.convert("RGB")
                 img.save(out, img_format)
                 out.seek(0)
                 mime = 'image/' + img_format
                 del data[key]
                 data[mime] = b64encode(out.read()).decode('ascii')
 
     # save notebook
@@ -67,9 +68,12 @@
     except AttributeError:
         output_format = 4
     write(nb, output_filename, version=output_format)
 
     # calculate bytes saved
     bytes_saved = orig_filesize - stat(output_filename).st_size
     if bytes_saved <= 0:
-        print('%s: warning: no compression - %s bytes gained' % (filename, -bytes_saved))
+        print(
+            '%s: warning: no compression - %s bytes gained'
+            % (filename, -bytes_saved)
+        )
     return bytes_saved
```

### Comparing `ipynbcompress-0.3.0/ipynbcompress.egg-info/PKG-INFO` & `ipynbcompress-0.4.0/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,113 +1,104 @@
-Metadata-Version: 1.1
-Name: ipynbcompress
-Version: 0.3.0
-Summary: Compress images in IPython/Jupyter notebooks
-Home-page: https://github.com/arve0/ipynbcompress
-Author: Arve Seljebu
-Author-email: arve.seljebu@gmail.com
-License: MIT
-Description: ipynbcompress
-        =============
-        
-        |build-status-image| |pypi-version| |wheel|
-        
-        Overview
-        --------
-        
-        So you have included an image with ``IPython.display.Image()`` and the
-        file size of your IPython Notebook got huge? No problem! This package
-        will resize images in your notebook and compress them as JPG or PNG.
-        
-        Installation
-        ------------
-        
-        Install using ``pip``...
-        
-        .. code:: bash
-        
-            pip install ipynbcompress
-        
-        Example
-        -------
-        
-        From command line:
-        
-        .. code:: sh
-        
-            $ ipynb-compress notebook4.ipynb
-            notebook4.ipynb: 10 megabytes decrease
-        
-        In python:
-        
-        .. code:: python
-        
-            >>> import os
-            >>> from ipynbcompress import compress
-            >>> filename = '/path/to/notebook.ipynb'
-            >>> out = '/path/to/compressed.ipynb'
-            >>> # original size
-            ... os.stat(filename).st_size
-            11563736
-            >>> # return bytes saved
-            ... compress(filename, output_filename=out, img_width=800, img_format='jpeg')
-            11451545
-            >>> compress(filename, output_filename=out, img_width=800, img_format='png')
-            11205762
-            >>> # defaults to img_width = 1024px and jpeg compression
-            ... compress(filename, output_filename=out)
-            11411377
-            >>> # overwrite existing notebook
-            ... compress(filename)
-            11411377
-        
-        API reference
-        -------------
-        
-        API reference is at http://ipynbcompress.rtfd.org.
-        
-        Development
-        -----------
-        
-        Install dependencies and link development version of ipynbcompress to
-        pip:
-        
-        .. code:: bash
-        
-            git clone https://github.com/arve0/ipynbcompress
-            cd ipynbcompress
-            pip install -r requirements.txt # install dependencies and ipynbcompress-package
-        
-        Testing
-        ~~~~~~~
-        
-        .. code:: bash
-        
-            tox
-        
-        Build documentation locally
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        To build the documentation:
-        
-        .. code:: bash
-        
-            pip install -r docs/requirements.txt
-            make docs
-        
-        .. |build-status-image| image:: https://secure.travis-ci.org/arve0/ipynbcompress.png?branch=master
-           :target: http://travis-ci.org/arve0/ipynbcompress?branch=master
-        .. |pypi-version| image:: https://pypip.in/version/ipynbcompress/badge.svg
-           :target: https://pypi.python.org/pypi/ipynbcompress
-        .. |wheel| image:: https://pypip.in/wheel/ipynbcompress/badge.svg
-           :target: https://pypi.python.org/pypi/ipynbcompress
-        
-Keywords: ipynbcompress
-Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
+ipynbcompress
+=============
+
+|build-status-image| |pypi-version| |wheel|
+
+Overview
+--------
+
+So you have included an image with ``IPython.display.Image()`` and the
+file size of your IPython Notebook got huge? No problem! This package
+will resize images in your notebook and compress them as PNG or JPEG.
+Images are only resized if they are above the specified width. 2048px
+and PNG compression is the default, which should give relative high
+quality images and normal sized notebooks. JPEG compression is nice if
+you serve the notebooks over the web (eg nbviewer) and prefer fast
+loading times.
+
+Installation
+------------
+
+Install using ``pip``\ …
+
+.. code:: bash
+
+   pip install ipynbcompress
+
+Example
+-------
+
+From command line:
+
+.. code:: sh
+
+   $ ipynb-compress notebook4.ipynb
+   notebook4.ipynb: 10 megabytes decrease
+   $ find . -name "*ipynb" -size +2M -exec ipynb-compress {} \;
+   ./lab 03.21/automated scan.ipynb: warning: no compression - 0 bytes gained
+   ./lab 03.21/automated scan.ipynb: compression less than 100k bytes - keeping original
+   ./lab 03.21/trouble.ipynb: 9 megabytes decrease
+   ...
+
+In python:
+
+.. code:: python
+
+   >>> import os
+   >>> from ipynbcompress import compress
+   >>> filename = '/path/to/notebook.ipynb'
+   >>> out = '/path/to/compressed.ipynb'
+   >>> # original size
+   ... os.stat(filename).st_size
+   11563736
+   >>> # return bytes saved
+   ... compress(filename, output_filename=out, img_width=800, img_format='jpeg')
+   11451545
+   >>> compress(filename, output_filename=out, img_width=800, img_format='png')
+   11205762
+   >>> # defaults to img_width = 2048px and png compression
+   ... compress(filename, output_filename=out)
+   11411377
+   >>> # overwrite existing notebook
+   ... compress(filename)
+   11411377
+
+API reference
+-------------
+
+API reference is at http://ipynbcompress.rtfd.org.
+
+Development
+-----------
+
+Install dependencies and link development version of ipynbcompress to
+pip:
+
+.. code:: bash
+
+   git clone https://github.com/arve0/ipynbcompress
+   cd ipynbcompress
+   pip install -r requirements.txt # install dependencies and ipynbcompress-package
+
+Testing
+~~~~~~~
+
+.. code:: bash
+
+   pytest
+
+Build documentation locally
+~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+To build the documentation:
+
+.. code:: bash
+
+   pip install -r docs/requirements.txt
+   make docs
+
+.. |build-status-image| image:: https://secure.travis-ci.org/arve0/ipynbcompress.png?branch=master
+   :target: http://travis-ci.org/arve0/ipynbcompress?branch=master
+.. |pypi-version| image:: https://img.shields.io/pypi/v/ipynbcompress.svg
+   :target: https://pypi.python.org/pypi/ipynbcompress
+.. |wheel| image:: https://img.shields.io/pypi/wheel/ipynbcompress.svg
+   :target: https://pypi.python.org/pypi/ipynbcompress
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ipynbcompress-0.3.0/ipynbcompress.egg-info/SOURCES.txt` & `ipynbcompress-0.4.0/ipynbcompress.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 LICENSE
 Makefile
 README.md
 README.rst
 requirements.txt
 setup.cfg
 setup.py
-tox.ini
+.devcontainer/devcontainer.json
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/ipynbcompress.rst
 docs/make.bat
 docs/modules.rst
 docs/requirements.txt
```

### Comparing `ipynbcompress-0.3.0/LICENSE` & `ipynbcompress-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipynbcompress-0.3.0/Makefile` & `ipynbcompress-0.4.0/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 .PHONY: help clean clean-pyc clean-build list test test-all coverage docs release sdist
 
 help:
 	@echo "clean-build - remove build artifacts"
 	@echo "clean-pyc - remove Python file artifacts"
 	@echo "lint - check style with flake8"
 	@echo "test - run tests quickly with the default Python"
-	@echo "testall - run tests on every Python version with tox"
 	@echo "coverage - check code coverage quickly with the default Python"
 	@echo "docs - generate Sphinx HTML documentation, including API docs"
 	@echo "release - package and upload a release"
 	@echo "sdist - package"
 
 clean: clean-build clean-pyc
 
@@ -23,15 +22,15 @@
 	find . -name '*.pyo' -exec rm -f {} +
 	find . -name '*~' -exec rm -f {} +
 
 lint:
 	flake8 ipynbcompress test
 
 test:
-	tox
+	pytest
 
 coverage:
 	coverage run --source ipynbcompress setup.py test
 	coverage report -m
 	coverage html
 	open htmlcov/index.html
 
@@ -40,20 +39,20 @@
 
 docs:
 	$(MAKE) -C docs clean
 	$(MAKE) -C docs html
 	open docs/_build/html/index.html
 
 release: clean rst tag
-	python setup.py sdist upload
-	python setup.py bdist_wheel upload
+	python setup.py sdist
+	python setup.py bdist_wheel
 	git push && git push --tags
 
 tag:
-	git tag v`cat ipynbcompress/VERSION`
+	git tag v`cat ipynbcompress/VERSION` || true
 
 rst:
 	pandoc --from=markdown --to=rst README.md -o README.rst
 
 sdist: clean rst
 	python setup.py sdist
 	python setup.py bdist_wheel upload
```

### Comparing `ipynbcompress-0.3.0/PKG-INFO` & `ipynbcompress-0.4.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,113 +1,121 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: ipynbcompress
-Version: 0.3.0
+Version: 0.4.0
 Summary: Compress images in IPython/Jupyter notebooks
 Home-page: https://github.com/arve0/ipynbcompress
 Author: Arve Seljebu
 Author-email: arve.seljebu@gmail.com
 License: MIT
-Description: ipynbcompress
-        =============
-        
-        |build-status-image| |pypi-version| |wheel|
-        
-        Overview
-        --------
-        
-        So you have included an image with ``IPython.display.Image()`` and the
-        file size of your IPython Notebook got huge? No problem! This package
-        will resize images in your notebook and compress them as JPG or PNG.
-        
-        Installation
-        ------------
-        
-        Install using ``pip``...
-        
-        .. code:: bash
-        
-            pip install ipynbcompress
-        
-        Example
-        -------
-        
-        From command line:
-        
-        .. code:: sh
-        
-            $ ipynb-compress notebook4.ipynb
-            notebook4.ipynb: 10 megabytes decrease
-        
-        In python:
-        
-        .. code:: python
-        
-            >>> import os
-            >>> from ipynbcompress import compress
-            >>> filename = '/path/to/notebook.ipynb'
-            >>> out = '/path/to/compressed.ipynb'
-            >>> # original size
-            ... os.stat(filename).st_size
-            11563736
-            >>> # return bytes saved
-            ... compress(filename, output_filename=out, img_width=800, img_format='jpeg')
-            11451545
-            >>> compress(filename, output_filename=out, img_width=800, img_format='png')
-            11205762
-            >>> # defaults to img_width = 1024px and jpeg compression
-            ... compress(filename, output_filename=out)
-            11411377
-            >>> # overwrite existing notebook
-            ... compress(filename)
-            11411377
-        
-        API reference
-        -------------
-        
-        API reference is at http://ipynbcompress.rtfd.org.
-        
-        Development
-        -----------
-        
-        Install dependencies and link development version of ipynbcompress to
-        pip:
-        
-        .. code:: bash
-        
-            git clone https://github.com/arve0/ipynbcompress
-            cd ipynbcompress
-            pip install -r requirements.txt # install dependencies and ipynbcompress-package
-        
-        Testing
-        ~~~~~~~
-        
-        .. code:: bash
-        
-            tox
-        
-        Build documentation locally
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        To build the documentation:
-        
-        .. code:: bash
-        
-            pip install -r docs/requirements.txt
-            make docs
-        
-        .. |build-status-image| image:: https://secure.travis-ci.org/arve0/ipynbcompress.png?branch=master
-           :target: http://travis-ci.org/arve0/ipynbcompress?branch=master
-        .. |pypi-version| image:: https://pypip.in/version/ipynbcompress/badge.svg
-           :target: https://pypi.python.org/pypi/ipynbcompress
-        .. |wheel| image:: https://pypip.in/wheel/ipynbcompress/badge.svg
-           :target: https://pypi.python.org/pypi/ipynbcompress
-        
 Keywords: ipynbcompress
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.8
+License-File: LICENSE
+
+ipynbcompress
+=============
+
+|build-status-image| |pypi-version| |wheel|
+
+Overview
+--------
+
+So you have included an image with ``IPython.display.Image()`` and the
+file size of your IPython Notebook got huge? No problem! This package
+will resize images in your notebook and compress them as PNG or JPEG.
+Images are only resized if they are above the specified width. 2048px
+and PNG compression is the default, which should give relative high
+quality images and normal sized notebooks. JPEG compression is nice if
+you serve the notebooks over the web (eg nbviewer) and prefer fast
+loading times.
+
+Installation
+------------
+
+Install using ``pip``\ …
+
+.. code:: bash
+
+   pip install ipynbcompress
+
+Example
+-------
+
+From command line:
+
+.. code:: sh
+
+   $ ipynb-compress notebook4.ipynb
+   notebook4.ipynb: 10 megabytes decrease
+   $ find . -name "*ipynb" -size +2M -exec ipynb-compress {} \;
+   ./lab 03.21/automated scan.ipynb: warning: no compression - 0 bytes gained
+   ./lab 03.21/automated scan.ipynb: compression less than 100k bytes - keeping original
+   ./lab 03.21/trouble.ipynb: 9 megabytes decrease
+   ...
+
+In python:
+
+.. code:: python
+
+   >>> import os
+   >>> from ipynbcompress import compress
+   >>> filename = '/path/to/notebook.ipynb'
+   >>> out = '/path/to/compressed.ipynb'
+   >>> # original size
+   ... os.stat(filename).st_size
+   11563736
+   >>> # return bytes saved
+   ... compress(filename, output_filename=out, img_width=800, img_format='jpeg')
+   11451545
+   >>> compress(filename, output_filename=out, img_width=800, img_format='png')
+   11205762
+   >>> # defaults to img_width = 2048px and png compression
+   ... compress(filename, output_filename=out)
+   11411377
+   >>> # overwrite existing notebook
+   ... compress(filename)
+   11411377
+
+API reference
+-------------
+
+API reference is at http://ipynbcompress.rtfd.org.
+
+Development
+-----------
+
+Install dependencies and link development version of ipynbcompress to
+pip:
+
+.. code:: bash
+
+   git clone https://github.com/arve0/ipynbcompress
+   cd ipynbcompress
+   pip install -r requirements.txt # install dependencies and ipynbcompress-package
+
+Testing
+~~~~~~~
+
+.. code:: bash
+
+   pytest
+
+Build documentation locally
+~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+To build the documentation:
+
+.. code:: bash
+
+   pip install -r docs/requirements.txt
+   make docs
+
+.. |build-status-image| image:: https://secure.travis-ci.org/arve0/ipynbcompress.png?branch=master
+   :target: http://travis-ci.org/arve0/ipynbcompress?branch=master
+.. |pypi-version| image:: https://img.shields.io/pypi/v/ipynbcompress.svg
+   :target: https://pypi.python.org/pypi/ipynbcompress
+.. |wheel| image:: https://img.shields.io/pypi/wheel/ipynbcompress.svg
+   :target: https://pypi.python.org/pypi/ipynbcompress
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ipynbcompress-0.3.0/README.md` & `ipynbcompress-0.4.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -4,29 +4,38 @@
 [![pypi-version]][pypi]
 [![wheel]][pypi]
 
 ## Overview
 
 So you have included an image with `IPython.display.Image()` and the file size
 of your IPython Notebook got huge? No problem! This package will resize images
-in your notebook and compress them as JPG or PNG.
+in your notebook and compress them as PNG or JPEG. Images are only resized if
+they are above the specified width. 2048px and PNG compression is the default,
+which should give relative high quality images and normal sized notebooks. JPEG
+compression is nice if you serve the notebooks over the web (eg nbviewer) and
+prefer fast loading times.
 
 ## Installation
 
 Install using `pip`...
 
 ```bash
 pip install ipynbcompress
 ```
 
 ## Example
 From command line:
 ```sh
 $ ipynb-compress notebook4.ipynb
 notebook4.ipynb: 10 megabytes decrease
+$ find . -name "*ipynb" -size +2M -exec ipynb-compress {} \;
+./lab 03.21/automated scan.ipynb: warning: no compression - 0 bytes gained
+./lab 03.21/automated scan.ipynb: compression less than 100k bytes - keeping original
+./lab 03.21/trouble.ipynb: 9 megabytes decrease
+...
 ```
 
 In python:
 ```python
 >>> import os
 >>> from ipynbcompress import compress
 >>> filename = '/path/to/notebook.ipynb'
@@ -35,15 +44,15 @@
 ... os.stat(filename).st_size
 11563736
 >>> # return bytes saved
 ... compress(filename, output_filename=out, img_width=800, img_format='jpeg')
 11451545
 >>> compress(filename, output_filename=out, img_width=800, img_format='png')
 11205762
->>> # defaults to img_width = 1024px and jpeg compression
+>>> # defaults to img_width = 2048px and png compression
 ... compress(filename, output_filename=out)
 11411377
 >>> # overwrite existing notebook
 ... compress(filename)
 11411377
 ```
 
@@ -57,24 +66,24 @@
 git clone https://github.com/arve0/ipynbcompress
 cd ipynbcompress
 pip install -r requirements.txt # install dependencies and ipynbcompress-package
 ```
 
 ### Testing
 ```bash
-tox
+pytest
 ```
 
 ### Build documentation locally
 To build the documentation:
 ```bash
 pip install -r docs/requirements.txt
 make docs
 ```
 
 
 
 [build-status-image]: https://secure.travis-ci.org/arve0/ipynbcompress.png?branch=master
 [travis]: http://travis-ci.org/arve0/ipynbcompress?branch=master
-[pypi-version]: https://pypip.in/version/ipynbcompress/badge.svg
+[pypi-version]: https://img.shields.io/pypi/v/ipynbcompress.svg
 [pypi]: https://pypi.python.org/pypi/ipynbcompress
-[wheel]: https://pypip.in/wheel/ipynbcompress/badge.svg
+[wheel]: https://img.shields.io/pypi/wheel/ipynbcompress.svg
```

### Comparing `ipynbcompress-0.3.0/scripts/ipynb-compress` & `ipynbcompress-0.4.0/scripts/ipynb-compress`

 * *Files identical despite different names*

### Comparing `ipynbcompress-0.3.0/setup.py` & `ipynbcompress-0.4.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -39,13 +39,11 @@
     zip_safe=False,
     keywords='ipynbcompress',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
+        'Programming Language :: Python :: 3.8',
     ],
 )
```

### Comparing `ipynbcompress-0.3.0/test/notebook3.ipynb` & `ipynbcompress-0.4.0/test/notebook3.ipynb`

 * *Files identical despite different names*

### Comparing `ipynbcompress-0.3.0/test/notebook4.ipynb` & `ipynbcompress-0.4.0/test/notebook4.ipynb`

 * *Files identical despite different names*

### Comparing `ipynbcompress-0.3.0/test/test_compress.py` & `ipynbcompress-0.4.0/test/test_compress.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Tests for `ipynbcompress`.
 """
 import pytest
-from ipynbcompress import *
-from IPython.nbformat import validate, read, NO_CONVERT
+from ipynbcompress import compress
+from nbformat import validate, read, NO_CONVERT
 from py import path
 
 
 @pytest.fixture
 def notebooks(tmpdir):
     "v3 and v4 notebook in tmpdir. Returns list of py.path object."
     testdir = path.local(__file__).dirpath()
```

