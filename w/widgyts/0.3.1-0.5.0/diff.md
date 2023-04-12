# Comparing `tmp/widgyts-0.3.1.tar.gz` & `tmp/widgyts-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/widgyts-0.3.1.tar", last modified: Fri Jan  4 19:44:05 2019, max compression
+gzip compressed data, was "widgyts-0.5.0.tar", last modified: Wed Apr 12 16:28:34 2023, max compression
```

## Comparing `widgyts-0.3.1.tar` & `widgyts-0.5.0.tar`

### file list

```diff
@@ -1,33 +1,62 @@
-drwxr-xr-x   0 madicken   (501) staff       (20)        0 2019-01-04 19:44:05.000000 widgyts-0.3.1/
-drwxr-xr-x   0 madicken   (501) staff       (20)        0 2019-01-04 19:44:05.000000 widgyts-0.3.1/jupyter-config/
-drwxr-xr-x   0 madicken   (501) staff       (20)        0 2019-01-04 19:44:05.000000 widgyts-0.3.1/jupyter-config/jupyter_notebook_config.d/
--rw-r--r--   0 madicken   (501) staff       (20)       84 2018-12-19 23:32:55.000000 widgyts-0.3.1/jupyter-config/jupyter_notebook_config.d/widgyts.json
-drwxr-xr-x   0 madicken   (501) staff       (20)        0 2019-01-04 19:44:05.000000 widgyts-0.3.1/jupyter-config/nbconfig/
-drwxr-xr-x   0 madicken   (501) staff       (20)        0 2019-01-04 19:44:05.000000 widgyts-0.3.1/jupyter-config/nbconfig/notebook.d/
--rw-r--r--   0 madicken   (501) staff       (20)       64 2018-12-19 23:32:55.000000 widgyts-0.3.1/jupyter-config/nbconfig/notebook.d/widgyts.json
--rw-r--r--   0 madicken   (501) staff       (20)       77 2018-12-19 23:32:55.000000 widgyts-0.3.1/MANIFEST.in
--rw-r--r--   0 madicken   (501) staff       (20)      868 2019-01-04 19:44:05.000000 widgyts-0.3.1/PKG-INFO
--rw-r--r--   0 madicken   (501) staff       (20)     2283 2019-01-03 22:16:19.000000 widgyts-0.3.1/README.md
--rw-r--r--   0 madicken   (501) staff       (20)       67 2019-01-04 19:44:05.000000 widgyts-0.3.1/setup.cfg
--rw-r--r--   0 madicken   (501) staff       (20)     6086 2018-12-19 23:32:55.000000 widgyts-0.3.1/setup.py
-drwxr-xr-x   0 madicken   (501) staff       (20)        0 2019-01-04 19:44:05.000000 widgyts-0.3.1/widgyts/
--rw-r--r--   0 madicken   (501) staff       (20)      510 2018-12-19 23:32:55.000000 widgyts-0.3.1/widgyts/__init__.py
--rw-r--r--   0 madicken   (501) staff       (20)      331 2019-01-04 19:34:27.000000 widgyts-0.3.1/widgyts/_version.py
-drwxr-xr-x   0 madicken   (501) staff       (20)        0 2019-01-04 19:44:05.000000 widgyts-0.3.1/widgyts/colormaps/
--rw-r--r--   0 madicken   (501) staff       (20)       84 2018-12-19 23:32:55.000000 widgyts-0.3.1/widgyts/colormaps/__init__.py
--rw-r--r--   0 madicken   (501) staff       (20)     1759 2019-01-03 23:27:40.000000 widgyts-0.3.1/widgyts/colormaps/colormaps.py
--rw-r--r--   0 madicken   (501) staff       (20)     9090 2019-01-03 22:16:29.000000 widgyts-0.3.1/widgyts/image_canvas.py
-drwxr-xr-x   0 madicken   (501) staff       (20)        0 2019-01-04 19:44:05.000000 widgyts-0.3.1/widgyts/static/
--rw-r--r--   0 madicken   (501) staff       (20)     9492 2019-01-04 19:44:05.000000 widgyts-0.3.1/widgyts/static/0.index.js
--rw-r--r--   0 madicken   (501) staff       (20)     8040 2019-01-04 19:44:05.000000 widgyts-0.3.1/widgyts/static/0.index.js.map
--rw-r--r--   0 madicken   (501) staff       (20)    90229 2019-01-04 19:44:05.000000 widgyts-0.3.1/widgyts/static/bbdba2be3ee75f23889f.module.wasm
--rw-r--r--   0 madicken   (501) staff       (20)     4634 2019-01-04 19:44:03.000000 widgyts-0.3.1/widgyts/static/extension.js
--rw-r--r--   0 madicken   (501) staff       (20)   835713 2019-01-04 19:44:05.000000 widgyts-0.3.1/widgyts/static/index.js
--rw-r--r--   0 madicken   (501) staff       (20)  1002972 2019-01-04 19:44:05.000000 widgyts-0.3.1/widgyts/static/index.js.map
-drwxr-xr-x   0 madicken   (501) staff       (20)        0 2019-01-04 19:44:05.000000 widgyts-0.3.1/widgyts.egg-info/
--rw-r--r--   0 madicken   (501) staff       (20)        1 2019-01-04 19:44:05.000000 widgyts-0.3.1/widgyts.egg-info/dependency_links.txt
--rw-r--r--   0 madicken   (501) staff       (20)        1 2018-12-19 19:58:15.000000 widgyts-0.3.1/widgyts.egg-info/not-zip-safe
--rw-r--r--   0 madicken   (501) staff       (20)      868 2019-01-04 19:44:05.000000 widgyts-0.3.1/widgyts.egg-info/PKG-INFO
--rw-r--r--   0 madicken   (501) staff       (20)       43 2019-01-04 19:44:05.000000 widgyts-0.3.1/widgyts.egg-info/requires.txt
--rw-r--r--   0 madicken   (501) staff       (20)      635 2019-01-04 19:44:05.000000 widgyts-0.3.1/widgyts.egg-info/SOURCES.txt
--rw-r--r--   0 madicken   (501) staff       (20)        8 2019-01-04 19:44:05.000000 widgyts-0.3.1/widgyts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:28:34.955372 widgyts-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-12 16:27:17.000000 widgyts-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-12 16:27:17.000000 widgyts-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-04-12 16:28:34.955372 widgyts-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-12 16:27:17.000000 widgyts-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-12 16:27:17.000000 widgyts-0.5.0/install.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:28:34.947372 widgyts-0.5.0/jupyter-config/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-12 16:27:17.000000 widgyts-0.5.0/jupyter-config/widgyts.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-04-12 16:27:17.000000 widgyts-0.5.0/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-12 16:27:17.000000 widgyts-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-12 16:28:34.955372 widgyts-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-12 16:27:17.000000 widgyts-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:28:34.951372 widgyts-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:28:34.951372 widgyts-0.5.0/src/@types/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-12 16:27:17.000000 widgyts-0.5.0/src/@types/jupyter-threejs.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-12 16:27:17.000000 widgyts-0.5.0/src/colormap_container.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-04-12 16:27:17.000000 widgyts-0.5.0/src/fixed_res_buffer.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-04-12 16:27:17.000000 widgyts-0.5.0/src/fullscreen.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-12 16:27:17.000000 widgyts-0.5.0/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-12 16:27:17.000000 widgyts-0.5.0/src/plugin.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-12 16:27:17.000000 widgyts-0.5.0/src/utils.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-12 16:27:17.000000 widgyts-0.5.0/src/variable_mesh.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-12 16:27:17.000000 widgyts-0.5.0/src/version.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-12 16:27:17.000000 widgyts-0.5.0/src/widgyts.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-04-12 16:27:17.000000 widgyts-0.5.0/src/widgyts_canvas.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:28:34.951372 widgyts-0.5.0/style/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:27:17.000000 widgyts-0.5.0/style/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 16:27:17.000000 widgyts-0.5.0/style/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-12 16:27:17.000000 widgyts-0.5.0/style/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-12 16:27:17.000000 widgyts-0.5.0/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:28:34.951372 widgyts-0.5.0/widgyts/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-12 16:27:17.000000 widgyts-0.5.0/widgyts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-12 16:27:17.000000 widgyts-0.5.0/widgyts/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-12 16:27:17.000000 widgyts-0.5.0/widgyts/colormaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28666 2023-04-12 16:27:17.000000 widgyts-0.5.0/widgyts/dataset_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-04-12 16:27:17.000000 widgyts-0.5.0/widgyts/image_canvas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:28:34.951372 widgyts-0.5.0/widgyts/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-04-12 16:28:34.000000 widgyts-0.5.0/widgyts/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:28:34.951372 widgyts-0.5.0/widgyts/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    67838 2023-04-12 16:28:34.000000 widgyts-0.5.0/widgyts/labextension/static/353.b96de7a6ab53ee83a3e3.js
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-12 16:28:34.000000 widgyts-0.5.0/widgyts/labextension/static/353.b96de7a6ab53ee83a3e3.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   109061 2023-04-12 16:28:34.000000 widgyts-0.5.0/widgyts/labextension/static/35962d9a369f94cd12dc.module.wasm
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-12 16:28:34.000000 widgyts-0.5.0/widgyts/labextension/static/480.f221211101f033161e08.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-12 16:28:34.000000 widgyts-0.5.0/widgyts/labextension/static/568.dc67e4d4b7ec920ad835.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-12 16:28:34.000000 widgyts-0.5.0/widgyts/labextension/static/7.578ca98bdcc06909a72d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14299 2023-04-12 16:28:34.000000 widgyts-0.5.0/widgyts/labextension/static/724.68ad0e0a95918b09cc71.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-04-12 16:28:34.000000 widgyts-0.5.0/widgyts/labextension/static/776.034dd82e5586eada2301.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-04-12 16:28:34.000000 widgyts-0.5.0/widgyts/labextension/static/818.070644e61f231f18d729.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-04-12 16:28:34.000000 widgyts-0.5.0/widgyts/labextension/static/remoteEntry.59b399c5575c4621e134.js
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-12 16:28:31.000000 widgyts-0.5.0/widgyts/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16106 2023-04-12 16:28:34.000000 widgyts-0.5.0/widgyts/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:28:34.955372 widgyts-0.5.0/widgyts/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:27:17.000000 widgyts-0.5.0/widgyts/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-04-12 16:27:17.000000 widgyts-0.5.0/widgyts/tests/test_widgyts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:28:34.951372 widgyts-0.5.0/widgyts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-04-12 16:28:34.000000 widgyts-0.5.0/widgyts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-12 16:28:34.000000 widgyts-0.5.0/widgyts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:28:34.000000 widgyts-0.5.0/widgyts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:27:44.000000 widgyts-0.5.0/widgyts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-12 16:28:34.000000 widgyts-0.5.0/widgyts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 16:28:34.000000 widgyts-0.5.0/widgyts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   411000 2023-04-12 16:28:24.000000 widgyts-0.5.0/yarn.lock
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `widgyts-0.3.1/README.md` & `widgyts-0.5.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,50 @@
 widgyts
 ===============================
 
+[![Documentation
+Status](https://readthedocs.org/projects/widgyts/badge/?version=latest)](https://widgyts.readthedocs.io/en/latest/?badge=latest)
+[![codecov](https://codecov.io/gh/yt-project/widgyts/branch/master/graph/badge.svg)](https://codecov.io/gh/yt-project/widgyts)
+[![status](https://joss.theoj.org/papers/f86e07ce58fe8bb24d928943663d2751/status.svg)](https://joss.theoj.org/papers/f86e07ce58fe8bb24d928943663d2751)
+[![DOI](https://zenodo.org/badge/124116100.svg)](https://zenodo.org/badge/latestdoi/124116100)
+
+
 A fully client-side pan-and-zoom widget, using WebAssembly, for variable mesh
 datasets from yt.  It runs in the browser, so once the data hits your notebook,
 it's super fast and responsive!
 
 If you'd like to dig into the Rust and WebAssembly portion of the code, you can
 find it at https://github.com/data-exp-lab/rust-yt-tools/ and in the npm
 package `@data-exp-lab/yt-tools`.
 
 Check out our [SciPy 2018 talk](https://www.youtube.com/watch?v=5dl_m_6T2bU)
 and the [associated slides](https://munkm.github.io/2018-07-13-scipy/) for more info!
 
+Documentation
+-------------
+
+Our documentation is hosted at readthedocs. Take a look
+[here](https://widgyts.readthedocs.io/en/latest/).
+
 Installation
 ------------
 
 To install using pip from the most recent released version:
 
     $ pip install widgyts
 
 To install using pip from this directory:
 
-    $ git clone https://github.com/data-exp-lab/widgyts.git
+    $ git clone https://github.com/yt-project/widgyts.git
     $ cd widgyts
     $ pip install .
 
 For a development installation (requires npm),
 
-    $ git clone https://github.com/data-exp-lab/widgyts.git
+    $ git clone https://github.com/yt-project/widgyts.git
     $ cd widgyts
     $ pip install -e .
     $ jupyter serverextension enable --py --sys-prefix widgyts
     $ jupyter nbextension install --py --symlink --sys-prefix widgyts
     $ jupyter nbextension enable --py --sys-prefix widgyts
 
 Note that in previous versions, serverextension was not provided and you were
```

