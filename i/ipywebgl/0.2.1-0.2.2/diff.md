# Comparing `tmp/ipywebgl-0.2.1.tar.gz` & `tmp/ipywebgl-0.2.2.tar.gz`

## Comparing `ipywebgl-0.2.1.tar` & `ipywebgl-0.2.2.tar`

### file list

```diff
@@ -1,96 +1,97 @@
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/.eslintignore
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/.eslintrc.js
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/.npmignore
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/.prettierignore
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/.prettierrc
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/MANIFEST.in
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/babel.config.js
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/dev_requirements.txt
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/install.json
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/ipywebgl.json
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/jest.config.js
--rw-r--r--   0        0        0   387684 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/logo.kra
--rw-r--r--   0        0        0   421627 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/logo.kra~
--rw-r--r--   0        0        0   626961 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/package-lock.json
--rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/package.json
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/readthedocs.yml
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/setup.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/tbump.toml
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/tsconfig.eslint.json
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/tsconfig.json
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/webpack.config.js
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/css/widget.css
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/docs/Makefile
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/docs/api.rst
--rw-r--r--   0        0        0     6542 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/docs/conf.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/docs/develop-install.rst
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/docs/index.rst
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/docs/installing.rst
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/docs/introduction.rst
--rwxr-xr-x   0        0        0      811 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/docs/make.bat
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/docs/requirements.in
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/docs/requirements.txt
--rw-r--r--   0        0        0    32633 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/docs/_static/embed-bundle.js
--rw-r--r--   0        0        0   106338 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/docs/_static/embed-bundle.js.map
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/docs/_static/helper.js
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/docs/examples/3d_camera.nblink
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/docs/examples/index.rst
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/docs/examples/indexed_vertices.nblink
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/docs/examples/instanced.nblink
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/docs/examples/introduction.nblink
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/docs/examples/introduction_extended.nblink
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/docs/examples/shadow.nblink
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/docs/examples/ssao.nblink
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/docs/examples/uniform_buffer.nblink
--rw-r--r--   0        0        0    96698 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/docs/images/logo_1024.png
--rw-r--r--   0        0        0     9645 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/docs/images/logo_128.png
--rw-r--r--   0        0        0   232980 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/docs/images/logo_2048.png
--rw-r--r--   0        0        0    20785 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/docs/images/logo_256.png
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/docs/images/logo_32.png
--rw-r--r--   0        0        0    43821 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/docs/images/logo_512.png
--rw-r--r--   0        0        0     4553 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/docs/images/logo_64.png
--rw-r--r--   0        0        0     8632 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/examples/3d_camera.ipynb
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/examples/draw_axis.ipynb
--rw-r--r--   0        0        0     5578 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/examples/indexed_vertices.ipynb
--rw-r--r--   0        0        0    15740 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/examples/instanced.ipynb
--rw-r--r--   0        0        0    13966 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/examples/introduction.ipynb
--rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/examples/introduction_extended.ipynb
--rw-r--r--   0        0        0    21494 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/examples/shadow.ipynb
--rw-r--r--   0        0        0    73970 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/examples/sky.ipynb
--rw-r--r--   0        0        0    40130 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/examples/ssao.ipynb
--rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/examples/texture.ipynb
--rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/examples/uniform_buffer.ipynb
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/ipywebgl/__init__.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/ipywebgl/_frontend.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/ipywebgl/_version.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/ipywebgl/arraybuffer.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/ipywebgl/glresource.py
--rw-r--r--   0        0        0    73504 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/ipywebgl/glviewer.py
--rw-r--r--   0        0        0    20663 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/ipywebgl/labextension/build_log.json
--rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/ipywebgl/labextension/package.json
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/ipywebgl/labextension/static/lib_index_js.115506ce89c3f4c34456.js
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/ipywebgl/labextension/static/lib_index_js.115506ce89c3f4c34456.js.map
--rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/ipywebgl/labextension/static/lib_plugin_js.a4fea4dfcfff14540990.js
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/ipywebgl/labextension/static/lib_plugin_js.a4fea4dfcfff14540990.js.map
--rw-r--r--   0        0        0    76116 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/ipywebgl/labextension/static/lib_widgets_js.9b129eb1485cff28d239.js
--rw-r--r--   0        0        0    84191 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/ipywebgl/labextension/static/lib_widgets_js.9b129eb1485cff28d239.js.map
--rw-r--r--   0        0        0    26426 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/ipywebgl/labextension/static/remoteEntry.21206eb8a87189c75dc8.js
--rw-r--r--   0        0        0    25148 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/ipywebgl/labextension/static/remoteEntry.21206eb8a87189c75dc8.js.map
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/ipywebgl/labextension/static/style.js
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/ipywebgl/nbextension/extension.js
--rw-r--r--   0        0        0    33420 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/ipywebgl/nbextension/index.js
--rw-r--r--   0        0        0   107839 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/ipywebgl/nbextension/index.js.map
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/src/arraybuffer.ts
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/src/extension.ts
--rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/src/glresource.ts
--rw-r--r--   0        0        0    39089 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/src/glviewer.ts
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/src/index.ts
--rw-r--r--   0        0        0     7192 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/src/matrix.ts
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/src/plugin.ts
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/src/version.ts
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/src/widgets.ts
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/.gitignore
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/LICENSE.txt
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/README.md
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4893 2020-02-02 00:00:00.000000 ipywebgl-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/.eslintignore
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/.eslintrc.js
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/.npmignore
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/.prettierignore
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/.prettierrc
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/MANIFEST.in
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/babel.config.js
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/dev_requirements.txt
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/install.json
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/ipywebgl.json
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/jest.config.js
+-rw-r--r--   0        0        0   387684 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/logo.kra
+-rw-r--r--   0        0        0   421627 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/logo.kra~
+-rw-r--r--   0        0        0   626961 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/package-lock.json
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/package.json
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/readthedocs.yml
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/setup.py
+-rw-r--r--   0        0        0    60202 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/social_preview.png
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/tbump.toml
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/tsconfig.eslint.json
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/tsconfig.json
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/webpack.config.js
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/css/widget.css
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/docs/Makefile
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/docs/api.rst
+-rw-r--r--   0        0        0     6542 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/docs/conf.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/docs/develop-install.rst
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/docs/index.rst
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/docs/installing.rst
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/docs/introduction.rst
+-rwxr-xr-x   0        0        0      811 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/docs/make.bat
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/docs/requirements.in
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/docs/requirements.txt
+-rw-r--r--   0        0        0    32633 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/docs/_static/embed-bundle.js
+-rw-r--r--   0        0        0   106338 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/docs/_static/embed-bundle.js.map
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/docs/_static/helper.js
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/docs/examples/3d_camera.nblink
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/docs/examples/index.rst
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/docs/examples/indexed_vertices.nblink
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/docs/examples/instanced.nblink
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/docs/examples/introduction.nblink
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/docs/examples/introduction_extended.nblink
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/docs/examples/shadow.nblink
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/docs/examples/ssao.nblink
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/docs/examples/uniform_buffer.nblink
+-rw-r--r--   0        0        0    96698 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/docs/images/logo_1024.png
+-rw-r--r--   0        0        0     9645 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/docs/images/logo_128.png
+-rw-r--r--   0        0        0   232980 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/docs/images/logo_2048.png
+-rw-r--r--   0        0        0    20785 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/docs/images/logo_256.png
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/docs/images/logo_32.png
+-rw-r--r--   0        0        0    43821 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/docs/images/logo_512.png
+-rw-r--r--   0        0        0     4553 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/docs/images/logo_64.png
+-rw-r--r--   0        0        0     8632 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/examples/3d_camera.ipynb
+-rw-r--r--   0        0        0     3596 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/examples/draw_axis.ipynb
+-rw-r--r--   0        0        0     5578 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/examples/indexed_vertices.ipynb
+-rw-r--r--   0        0        0    15740 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/examples/instanced.ipynb
+-rw-r--r--   0        0        0    13966 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/examples/introduction.ipynb
+-rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/examples/introduction_extended.ipynb
+-rw-r--r--   0        0        0    21495 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/examples/shadow.ipynb
+-rw-r--r--   0        0        0    73727 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/examples/sky.ipynb
+-rw-r--r--   0        0        0    40130 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/examples/ssao.ipynb
+-rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/examples/texture.ipynb
+-rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/examples/uniform_buffer.ipynb
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/ipywebgl/__init__.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/ipywebgl/_frontend.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/ipywebgl/_version.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/ipywebgl/arraybuffer.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/ipywebgl/glresource.py
+-rw-r--r--   0        0        0    73504 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/ipywebgl/glviewer.py
+-rw-r--r--   0        0        0    20663 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/ipywebgl/labextension/build_log.json
+-rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/ipywebgl/labextension/package.json
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/ipywebgl/labextension/static/lib_index_js.115506ce89c3f4c34456.js
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/ipywebgl/labextension/static/lib_index_js.115506ce89c3f4c34456.js.map
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/ipywebgl/labextension/static/lib_plugin_js.a4fea4dfcfff14540990.js
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/ipywebgl/labextension/static/lib_plugin_js.a4fea4dfcfff14540990.js.map
+-rw-r--r--   0        0        0    76116 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/ipywebgl/labextension/static/lib_widgets_js.417df79f43e89915d69a.js
+-rw-r--r--   0        0        0    84191 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/ipywebgl/labextension/static/lib_widgets_js.417df79f43e89915d69a.js.map
+-rw-r--r--   0        0        0    26426 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/ipywebgl/labextension/static/remoteEntry.8194deb74d0ed2d99f98.js
+-rw-r--r--   0        0        0    25148 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/ipywebgl/labextension/static/remoteEntry.8194deb74d0ed2d99f98.js.map
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/ipywebgl/labextension/static/style.js
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/ipywebgl/nbextension/extension.js
+-rw-r--r--   0        0        0    33420 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/ipywebgl/nbextension/index.js
+-rw-r--r--   0        0        0   107839 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/ipywebgl/nbextension/index.js.map
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/src/arraybuffer.ts
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/src/extension.ts
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/src/glresource.ts
+-rw-r--r--   0        0        0    39089 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/src/glviewer.ts
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/src/index.ts
+-rw-r--r--   0        0        0     7192 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/src/matrix.ts
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/src/plugin.ts
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/src/version.ts
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/src/widgets.ts
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/LICENSE.txt
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/README.md
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4893 2020-02-02 00:00:00.000000 ipywebgl-0.2.2/PKG-INFO
```

### Comparing `ipywebgl-0.2.1/.eslintrc.js` & `ipywebgl-0.2.2/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/MANIFEST.in` & `ipywebgl-0.2.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/logo.kra` & `ipywebgl-0.2.2/logo.kra`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/logo.kra~` & `ipywebgl-0.2.2/logo.kra~`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/package-lock.json` & `ipywebgl-0.2.2/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8999963181148749%*

 * *Differences: {"'packages'": "{'': {'version': '0.2.1'}}", "'version'": "'0.2.1'"}*

```diff
@@ -35,15 +35,15 @@
                 "ts-loader": "^8.0.0",
                 "typescript": "~4.1.3",
                 "webpack": "^5.61.0",
                 "webpack-cli": "^4.0.0"
             },
             "license": "BSD-3-Clause",
             "name": "ipywebgl",
-            "version": "0.1.0"
+            "version": "0.2.1"
         },
         "node_modules/@ampproject/remapping": {
             "dependencies": {
                 "@jridgewell/gen-mapping": "^0.1.0",
                 "@jridgewell/trace-mapping": "^0.3.9"
             },
             "dev": true,
@@ -16348,9 +16348,9 @@
             },
             "integrity": "sha512-rVksvsnNCdJ/ohGc6xgPwyN8eheCxsiLM8mxuE/t/mOVqJewPuO1miLpTHQiRgTKCLexL4MeAFVagts7HmNZ2Q==",
             "resolved": "https://registry.npmjs.org/yocto-queue/-/yocto-queue-0.1.0.tgz",
             "version": "0.1.0"
         }
     },
     "requires": true,
-    "version": "0.1.0"
+    "version": "0.2.1"
 }
```

### Comparing `ipywebgl-0.2.1/package.json` & `ipywebgl-0.2.2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "'0.2.2'"}*

```diff
@@ -86,9 +86,9 @@
         "prepack": "yarn run build:lib",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch --mode=development"
     },
     "types": "./lib/index.d.ts",
-    "version": "0.2.1"
+    "version": "0.2.2"
 }
```

### Comparing `ipywebgl-0.2.1/readthedocs.yml` & `ipywebgl-0.2.2/readthedocs.yml`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/tbump.toml` & `ipywebgl-0.2.2/tbump.toml`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 default = ""
 
 [[field]]
 name = "release"
 default = ""
 
 [version]
-current = "0.2.1"
+current = "0.2.2"
 regex = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)((?P<channel>a|b|rc|.dev)(?P<release>\\d+))?"
 
 [git]
 message_template = "Bump to {new_version}"
 tag_template = "v{new_version}"
 
 [[file]]
@@ -21,7 +21,10 @@
 
 [[file]]
 src = "ipywebgl/_version.py"
 
 [[file]]
 src = "package.json"
 version_template = "\"version\": \"{major}.{minor}.{patch}{channel}{release}\""
+
+[[file]]
+src = "ipywebgl/_frontend.py"
```

### Comparing `ipywebgl-0.2.1/tsconfig.json` & `ipywebgl-0.2.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/webpack.config.js` & `ipywebgl-0.2.2/webpack.config.js`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/docs/Makefile` & `ipywebgl-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/docs/api.rst` & `ipywebgl-0.2.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/docs/conf.py` & `ipywebgl-0.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/docs/develop-install.rst` & `ipywebgl-0.2.2/docs/develop-install.rst`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/docs/index.rst` & `ipywebgl-0.2.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/docs/installing.rst` & `ipywebgl-0.2.2/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/docs/introduction.rst` & `ipywebgl-0.2.2/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/docs/make.bat` & `ipywebgl-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/docs/requirements.txt` & `ipywebgl-0.2.2/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/docs/_static/embed-bundle.js` & `ipywebgl-0.2.2/docs/_static/embed-bundle.js`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/docs/_static/embed-bundle.js.map` & `ipywebgl-0.2.2/docs/_static/embed-bundle.js.map`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/docs/images/logo_1024.png` & `ipywebgl-0.2.2/docs/images/logo_1024.png`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/docs/images/logo_128.png` & `ipywebgl-0.2.2/docs/images/logo_128.png`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/docs/images/logo_2048.png` & `ipywebgl-0.2.2/docs/images/logo_2048.png`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/docs/images/logo_256.png` & `ipywebgl-0.2.2/docs/images/logo_256.png`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/docs/images/logo_32.png` & `ipywebgl-0.2.2/docs/images/logo_32.png`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/docs/images/logo_512.png` & `ipywebgl-0.2.2/docs/images/logo_512.png`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/docs/images/logo_64.png` & `ipywebgl-0.2.2/docs/images/logo_64.png`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/examples/3d_camera.ipynb` & `ipywebgl-0.2.2/examples/3d_camera.ipynb`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/examples/draw_axis.ipynb` & `ipywebgl-0.2.2/examples/draw_axis.ipynb`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583152488425926%*

 * *Differences: {"'cells'": "{1: {'outputs': {0: {'data': {'application/vnd.jupyter.widget-view+json': "*

 * *            "{'model_id': '9b08d581c5f34787b12600dd34659e76'}}}}}, insert: [(2, "*

 * *            "OrderedDict([('cell_type', 'code'), ('execution_count', None), ('id', "*

 * *            "'f2855ec2-200c-4cf6-b307-2c1322829abc'), ('metadata', OrderedDict()), ('outputs', "*

 * *            "[]), ('source', [])]))]}"}*

```diff
@@ -15,15 +15,15 @@
             "execution_count": 1,
             "id": "d8dc089e-6f77-45c2-b706-071f5e4d6113",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "59e8cd0ed2d84654afed386172e545d9",
+                            "model_id": "9b08d581c5f34787b12600dd34659e76",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "GLViewer(camera_pos=[0, 50, 200])"
                         ]
                     },
@@ -96,14 +96,22 @@
                 "w.uniform('u_scale', np.array([10.0], dtype=np.float32))\n",
                 "w.bind_vertex_array(axis_vao)\n",
                 "w.draw_arrays('LINES', 0, 6)\n",
                 "# render in loop if needed\n",
                 "w.execute_commands()\n",
                 "w"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "f2855ec2-200c-4cf6-b307-2c1322829abc",
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
```

### Comparing `ipywebgl-0.2.1/examples/indexed_vertices.ipynb` & `ipywebgl-0.2.2/examples/indexed_vertices.ipynb`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/examples/instanced.ipynb` & `ipywebgl-0.2.2/examples/instanced.ipynb`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/examples/introduction.ipynb` & `ipywebgl-0.2.2/examples/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/examples/introduction_extended.ipynb` & `ipywebgl-0.2.2/examples/introduction_extended.ipynb`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/examples/shadow.ipynb` & `ipywebgl-0.2.2/examples/shadow.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999844344204696%*

 * *Differences: {"'cells'": "{11: {'source': {insert: [(78, '    None,\\n')], delete: [78]}}, 19: {'outputs': {0: "*

 * *            "{'data': {'application/vnd.jupyter.widget-view+json': {'model_id': "*

 * *            "'f5eacf0906f047feb3fddada7c66467f'}}}, 1: {'data': "*

 * *            "{'application/vnd.jupyter.widget-view+json': {'model_id': "*

 * *            "'347573249fcb4608b6c5de2fc0d5cbc8'}}}}}}"}*

```diff
@@ -319,15 +319,15 @@
                 "       [-10  ,  0.  ,  10.  ,  0.  ,  1  ,  0.  ],\n",
                 "       [-10  ,  0.  ,  10.  ,  0.  ,  1  ,  0.  ],\n",
                 "       [10  ,  0.  ,  10.  ,  0.  ,  1  ,  0.  ],\n",
                 "       [10  ,  0.  ,  -10.  ,  0.  ,  1  ,  0.  ]], dtype=np.float32).flatten()\n",
                 ")\n",
                 "\n",
                 "plane_vao = w.create_vertex_array_ext(\n",
-                "    None\n",
+                "    None,\n",
                 "    [\n",
                 "        (plane_vbo, '3f32 3f32', 0, 1),\n",
                 "    ]\n",
                 ")"
             ]
         },
         {
@@ -561,29 +561,29 @@
             "execution_count": 10,
             "id": "709fcf32-9fb2-48e7-bde8-92a83546e540",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "e4ab0aa6166c4adf8d0d96d74f80876c",
+                            "model_id": "f5eacf0906f047feb3fddada7c66467f",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "interactive(children=(Checkbox(value=False, description='perspective projection'), Output()), _dom_classes=('w\u2026"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "68f212fb06d440628a1f9e17babbffac",
+                            "model_id": "347573249fcb4608b6c5de2fc0d5cbc8",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "GLViewer(camera_pitch=-37.0, camera_pos=[33.45616955516928, 37.90264690920414, 36.766131171063385], camera_yaw\u2026"
                         ]
                     },
```

### Comparing `ipywebgl-0.2.1/examples/sky.ipynb` & `ipywebgl-0.2.2/examples/sky.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9948879163451646%*

 * *Differences: {"'cells'": "{28: {'execution_count': 14}, 30: {'execution_count': 15}, 31: {'execution_count': "*

 * *            "16}, 33: {'execution_count': 17}, 34: {'execution_count': 18}, 36: "*

 * *            "{'execution_count': 19}, 38: {'execution_count': 20}, 40: {'execution_count': 21}, "*

 * *            "41: {'execution_count': 22}, 43: {'execution_count': 23, 'outputs': {0: {'data': "*

 * *            "{'application/vnd.jupyter.widget-view+json': {'model_id': "*

 * *            "'0815c0eaa770493cba3cccce08010d41'}}}, 1: {'data': " […]*

```diff
@@ -925,15 +925,15 @@
                 "\n",
                 "w.bind_framebuffer('FRAMEBUFFER', None)\n",
                 "w.execute_commands(execute_once=True)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 14,
             "id": "af8f1316-4aed-4d9f-b274-903f892cddd4",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "diffuse_importance_sampling_prog = w.create_program_ext(\n",
@@ -1046,15 +1046,15 @@
             "metadata": {},
             "source": [
                 "#### brdf integration"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 15,
             "id": "669eacc6-b961-4d88-9636-1dd35282b4cd",
             "metadata": {},
             "outputs": [],
             "source": [
                 "brdf_integration_buffer = w.create_framebuffer()\n",
                 "w.bind_framebuffer('FRAMEBUFFER', brdf_integration_buffer)\n",
                 "\n",
@@ -1070,15 +1070,15 @@
                 "\n",
                 "w.bind_framebuffer('FRAMEBUFFER', None)\n",
                 "w.execute_commands(execute_once=True)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": 16,
             "id": "b68a3f9c-8fab-4e4b-ad1f-890d1beae3a5",
             "metadata": {},
             "outputs": [],
             "source": [
                 "brdf_integration_prog = w.create_program_ext(\n",
                 "\"\"\"#version 300 es\n",
                 "\n",
@@ -1176,15 +1176,15 @@
             "metadata": {},
             "source": [
                 "#### brdf convolution"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": 17,
             "id": "e16ece02-e883-4d14-8db1-0e8e68b73d17",
             "metadata": {},
             "outputs": [],
             "source": [
                 "brdf_tex = w.create_texture()\n",
                 "w.active_texture(5)\n",
                 "w.bind_texture('TEXTURE_2D', brdf_tex)\n",
@@ -1202,15 +1202,15 @@
                 "\n",
                 "w.bind_framebuffer('FRAMEBUFFER', None)\n",
                 "w.execute_commands(execute_once=True)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 25,
+            "execution_count": 18,
             "id": "41fd30dc-c1ba-4cef-885e-6445d1910a7c",
             "metadata": {},
             "outputs": [],
             "source": [
                 "brdf_importance_sampling_prog = w.create_program_ext(\n",
                 "\"\"\"#version 300 es\n",
                 "\n",
@@ -1335,15 +1335,15 @@
             "source": [
                 "#### Display a grid\n",
                 "program and vao for a grid"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 26,
+            "execution_count": 19,
             "id": "b36bbfa3-791d-4a85-9c24-69ea9f7e63e0",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "grid_program = w.create_program_ext(\n",
@@ -1400,15 +1400,15 @@
             "source": [
                 "#### Sphere\n",
                 "IBL + PBR renderer for a sphere"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 29,
+            "execution_count": 20,
             "id": "26783bbb-66ab-4318-8422-f11e97899e42",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "sphere_prog = w.create_program_ext(\n",
@@ -1659,15 +1659,15 @@
             "source": [
                 "#### Debug program\n",
                 "helper program to render the texture created"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 30,
+            "execution_count": 21,
             "id": "0aab73f6-1a99-4863-acb1-926b7734c9cd",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "show_texture_prog = w.create_program_ext(\n",
@@ -1702,15 +1702,15 @@
                 "    'in_vert' : 0,\n",
                 "    'in_coord' : 1,\n",
                 "})"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 31,
+            "execution_count": 22,
             "id": "a74e5e08-ad70-4f20-bcde-913626895263",
             "metadata": {},
             "outputs": [],
             "source": [
                 "def getSunAltitude(time):\n",
                 "    periodSec = 120.0;\n",
                 "    halfPeriod = periodSec / 2.0\n",
@@ -1730,46 +1730,46 @@
             "metadata": {},
             "source": [
                 "## Final render"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 34,
+            "execution_count": 23,
             "id": "5bfccf30-ff2d-4872-8ea2-342d416e9fbc",
             "metadata": {
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "e14ee5a2112d43aebdde1e04e665fb6c",
+                            "model_id": "0815c0eaa770493cba3cccce08010d41",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "interactive(children=(FloatSlider(value=9.0, description='time', max=60.0), FloatSlider(value=0.1, description\u2026"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "34ef67c6cf94461cbaaea8bf15c70c46",
+                            "model_id": "a6c823f59e4c481c9fc6e23796926709",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
-                            "GLViewer(camera_pitch=-47.599999999999994, camera_pos=[-54.097238191754215, 129.11720284314038, -118.962350484\u2026"
+                            "GLViewer(camera_pos=[0, 50, 200])"
                         ]
                     },
-                    "execution_count": 34,
+                    "execution_count": 23,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from ipywidgets import widgets, interact\n",
                 "\n",
@@ -1897,22 +1897,14 @@
                 "    metal=widgets.FloatSlider(min=0, max=1, step=.01, value=0),\n",
                 "    reflectance=widgets.FloatSlider(min=0, max=1, step=.01, value=.5),\n",
                 "    debug_texture=widgets.IntSlider(min=0, max=6, value=0),\n",
                 "    debug_mip=widgets.IntSlider(min=0, max=5, value=0),\n",
                 ")\n",
                 "w"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "63a4af6a-b717-4802-8889-852ea8a9a713",
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
```

### Comparing `ipywebgl-0.2.1/examples/ssao.ipynb` & `ipywebgl-0.2.2/examples/ssao.ipynb`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/examples/texture.ipynb` & `ipywebgl-0.2.2/examples/texture.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9852484809027777%*

 * *Differences: {"'cells'": "{4: {'execution_count': 4}, 8: {'execution_count': 6, 'outputs': {0: {'data': "*

 * *            "{'application/vnd.jupyter.widget-view+json': {'model_id': "*

 * *            "'1747a8db2ad24a90beffec691f40499e'}, 'text/plain': ['GLViewer(camera_pos=[0, 50, "*

 * *            "200])']}, 'execution_count': 6}}}, delete: [9]}"}*

```diff
@@ -71,15 +71,15 @@
                 "    f_color = texture(u_texture, v_texcoord);\n",
                 "}\n",
                 "\"\"\")\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 4,
             "id": "89501424-7d18-458d-8a24-8ea70c9a601a",
             "metadata": {},
             "outputs": [],
             "source": [
                 "vbo = w.create_buffer_ext(\n",
                 "    #x z u v\n",
                 "    src_data=np.array([\n",
@@ -129,30 +129,30 @@
             "metadata": {},
             "source": [
                 "Bind the texture with a repeat pattern, because our UV's are from 0 to 10 and not 0 to 1"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 6,
             "id": "32255537-8b15-42eb-b502-847b46288b6c",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "157cef0b52d147d9bce2cd1047e40c60",
+                            "model_id": "1747a8db2ad24a90beffec691f40499e",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
-                            "GLViewer(camera_pitch=-26.2, camera_pos=[17.809647922495124, 27.95317454386815, 132.78695031297934], camera_ya\u2026"
+                            "GLViewer(camera_pos=[0, 50, 200])"
                         ]
                     },
-                    "execution_count": 8,
+                    "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "w.clear()\n",
                 "w.use_program(program)\n",
@@ -163,22 +163,14 @@
                 "w.tex_parameter('TEXTURE_2D', 'TEXTURE_WRAP_S', 'REPEAT')\n",
                 "w.tex_parameter('TEXTURE_2D', 'TEXTURE_WRAP_T', 'REPEAT')\n",
                 "w.bind_vertex_array(vao)\n",
                 "w.draw_arrays('TRIANGLE_FAN', 0, 4)\n",
                 "w.execute_commands()\n",
                 "w"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "d211efee-ca09-40b6-a7c7-a1e987316275",
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
```

### Comparing `ipywebgl-0.2.1/examples/uniform_buffer.ipynb` & `ipywebgl-0.2.2/examples/uniform_buffer.ipynb`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/ipywebgl/__init__.py` & `ipywebgl-0.2.2/ipywebgl/__init__.py`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/ipywebgl/arraybuffer.py` & `ipywebgl-0.2.2/ipywebgl/arraybuffer.py`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/ipywebgl/glresource.py` & `ipywebgl-0.2.2/ipywebgl/glresource.py`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/ipywebgl/glviewer.py` & `ipywebgl-0.2.2/ipywebgl/glviewer.py`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/ipywebgl/labextension/build_log.json` & `ipywebgl-0.2.2/ipywebgl/labextension/build_log.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999992985409654%*

 * *Differences: {'0': "{'plugins': {1: {'_options': {'shared': {'ipywebgl': {'version': '0.2.2'}}}}}}"}*

```diff
@@ -583,15 +583,15 @@
                             "import": false,
                             "requiredVersion": "^1.33.0",
                             "singleton": true
                         },
                         "ipywebgl": {
                             "import": "E:\\github\\research\\ipywebgl\\lib\\index.js",
                             "singleton": true,
-                            "version": "0.2.1"
+                            "version": "0.2.2"
                         },
                         "react": {
                             "import": false,
                             "requiredVersion": "^17.0.1",
                             "singleton": true
                         },
                         "react-dom": {
```

### Comparing `ipywebgl-0.2.1/ipywebgl/labextension/package.json` & `ipywebgl-0.2.2/ipywebgl/labextension/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9677734375%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static\\\\remoteEntry.8194deb74d0ed2d99f98.js'}}",*

 * * "'version'": "'0.2.2'"}*

```diff
@@ -46,15 +46,15 @@
         "dist/*.js",
         "css/*.css"
     ],
     "homepage": "https://github.com/JeromeEippers/ipywebgl",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static\\remoteEntry.21206eb8a87189c75dc8.js"
+            "load": "static\\remoteEntry.8194deb74d0ed2d99f98.js"
         },
         "extension": "lib/plugin",
         "outputDir": "ipywebgl/labextension/",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -90,9 +90,9 @@
         "prepack": "yarn run build:lib",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch --mode=development"
     },
     "types": "./lib/index.d.ts",
-    "version": "0.2.1"
+    "version": "0.2.2"
 }
```

### Comparing `ipywebgl-0.2.1/ipywebgl/labextension/static/lib_index_js.115506ce89c3f4c34456.js` & `ipywebgl-0.2.2/ipywebgl/labextension/static/lib_index_js.115506ce89c3f4c34456.js`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/ipywebgl/labextension/static/lib_index_js.115506ce89c3f4c34456.js.map` & `ipywebgl-0.2.2/ipywebgl/labextension/static/lib_index_js.115506ce89c3f4c34456.js.map`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/ipywebgl/labextension/static/lib_plugin_js.a4fea4dfcfff14540990.js` & `ipywebgl-0.2.2/ipywebgl/labextension/static/lib_plugin_js.a4fea4dfcfff14540990.js`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/ipywebgl/labextension/static/lib_plugin_js.a4fea4dfcfff14540990.js.map` & `ipywebgl-0.2.2/ipywebgl/labextension/static/lib_plugin_js.a4fea4dfcfff14540990.js.map`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/ipywebgl/labextension/static/lib_widgets_js.9b129eb1485cff28d239.js` & `ipywebgl-0.2.2/ipywebgl/labextension/static/lib_widgets_js.417df79f43e89915d69a.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1896,15 +1896,15 @@
             /*!**********************!*\
               !*** ./package.json ***!
               \**********************/
             /***/
             ((module) => {
 
                 "use strict";
-                module.exports = JSON.parse('{"name":"ipywebgl","version":"0.2.1","description":"A Custom Jupyter Widget Library","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/JeromeEippers/ipywebgl","bugs":{"url":"https://github.com/JeromeEippers/ipywebgl/issues"},"license":"BSD-3-Clause","author":{"name":"Jerome Eippers","email":"jerome@eippers.be"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/JeromeEippers/ipywebgl"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipywebgl/labextension","clean:nbextension":"rimraf ipywebgl/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipywebgl/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}');
+                module.exports = JSON.parse('{"name":"ipywebgl","version":"0.2.2","description":"A Custom Jupyter Widget Library","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/JeromeEippers/ipywebgl","bugs":{"url":"https://github.com/JeromeEippers/ipywebgl/issues"},"license":"BSD-3-Clause","author":{"name":"Jerome Eippers","email":"jerome@eippers.be"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/JeromeEippers/ipywebgl"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipywebgl/labextension","clean:nbextension":"rimraf ipywebgl/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipywebgl/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}');
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=lib_widgets_js.9b129eb1485cff28d239.js.map
+//# sourceMappingURL=lib_widgets_js.417df79f43e89915d69a.js.map
```

### Comparing `ipywebgl-0.2.1/ipywebgl/labextension/static/lib_widgets_js.9b129eb1485cff28d239.js.map` & `ipywebgl-0.2.2/ipywebgl/labextension/static/lib_widgets_js.417df79f43e89915d69a.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'file'": "'lib_widgets_js.417df79f43e89915d69a.js'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "lib_widgets_js.9b129eb1485cff28d239.js",
+    "file": "lib_widgets_js.417df79f43e89915d69a.js",
     "mappings": ";;;;;;;;;AAAa;AACb,8CAA6C,EAAE,aAAa,EAAC;AAC7D,uBAAuB;AACvB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,uBAAuB;AACvB;;;;;;;;;;;ACnCa;AACb,8CAA6C,EAAE,aAAa,EAAC;AAC7D,sBAAsB,GAAG,kBAAkB;AAC3C,eAAe,mBAAO,CAAC,oFAAuB;AAC9C,kBAAkB,mBAAO,CAAC,mCAAW;AACrC;AACA,mBAAO,CAAC,2CAAmB;AAC3B;AACA;AACA,6CAA6C,uBAAuB,6QAA6Q,iBAAiB,UAAU;AAC5W;AACA;AACA;AACA;AACA;AACA;AACA,kBAAkB;AAClB,uDAAuD,wCAAwC,YAAY,qCAAqC;AAChJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,qCAAqC,IAAI;AACzC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,sBAAsB;AACtB;;;;;;;;;;;ACxDa;AACb,8CAA6C,EAAE,aAAa,EAAC;AAC7D,gBAAgB,GAAG,eAAe;AAClC,eAAe,mBAAO,CAAC,oFAAuB;AAC9C,kBAAkB,mBAAO,CAAC,mCAAW;AACrC,iBAAiB,mBAAO,CAAC,iCAAU;AACnC,sBAAsB,mBAAO,CAAC,2CAAe;AAC7C;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,6CAA6C,uBAAuB,2bAA2b;AAC/f;AACA;AACA;AACA;AACA,sDAAsD,6BAA6B;AACnF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,qDAAqD,mBAAmB;AACxE;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,uCAAuC,iBAAiB;AACxD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,uCAAuC,oBAAoB;AAC3D;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,uCAAuC,iBAAiB;AACxD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,wCAAwC,iBAAiB;AACzD;AACA;AACA;AACA;AACA,oGAAoG,0CAA0C;AAC9I;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,kEAAkE,gGAAgG;AAClK;AACA;AACA,4DAA4D,6HAA6H;AACzL;AACA;AACA;AACA;AACA;AACA,wCAAwC,kBAAkB;AAC1D;AACA;AACA,0DAA0D,4HAA4H;AACtL;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,6EAA6E,sCAAsC;AACnH;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,8FAA8F,oDAAoD;AAClJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,uCAAuC,gBAAgB;AACvD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,+CAA+C,4CAA4C;AAC3F;AACA;AACA;AACA;AACA;AACA;AACA;AACA,+CAA+C,mDAAmD;AAClG;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iCAAiC;AACjC;AACA,+FAA+F,4CAA4C;AAC3I;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,sFAAsF,iDAAiD;AACvI;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,uCAAuC,2CAA2C;AAClF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,wGAAwG,uCAAuC;AAC/I;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,yFAAyF,0CAA0C;AACnI;AACA,qDAAqD;AACrD;AACA;AACA,+DAA+D,uIAAuI;AACtM;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,yFAAyF,0CAA0C;AACnI;AACA,qDAAqD;AACrD;AACA;AACA,+DAA+D,sKAAsK;AACrO;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,mDAAmD,eAAe;AAClE;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,uCAAuC,qBAAqB;AAC5D;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,uEAAuE,qBAAqB;AAC5F;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,eAAe;AACf,sCAAsC;AACtC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA,SAAS;AACT;AACA;AACA,SAAS;AACT;AACA;AACA,SAAS;AACT;AACA;AACA,SAAS;AACT;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,4BAA4B,oDAAoD,IAAI;AACpF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iBAAiB;AACjB;AACA;AACA,gBAAgB;AAChB;;;;;;;;;;;AC36Ba;AACb,8CAA6C,EAAE,aAAa,EAAC;AAC7D,iBAAiB,GAAG,aAAa,GAAG,eAAe,GAAG,mBAAmB,GAAG,mBAAmB,GAAG,mBAAmB,GAAG,qBAAqB,GAAG,iBAAiB,GAAG,eAAe,GAAG,oBAAoB,GAAG,oBAAoB,GAAG,oBAAoB,GAAG,wBAAwB,GAAG,mBAAmB,GAAG,sCAAsC,GAAG,0BAA0B;AAC/W;AACA;AACA;AACA;AACA;AACA,0BAA0B;AAC1B;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,sCAAsC;AACtC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,mBAAmB;AACnB;AACA;AACA;AACA;AACA;AACA,wBAAwB;AACxB;AACA;AACA;AACA;AACA;AACA,oBAAoB;AACpB;AACA;AACA;AACA;AACA;AACA,oBAAoB;AACpB;AACA;AACA;AACA;AACA;AACA,oBAAoB;AACpB;AACA;AACA;AACA;AACA;AACA;AACA;AACA,eAAe;AACf;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iBAAiB;AACjB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,qBAAqB;AACrB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,mBAAmB;AACnB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,mBAAmB;AACnB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,mBAAmB;AACnB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,eAAe;AACf;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iBAAiB;AACjB;;;;;;;;;;;AC/Na;AACb;AACA;AACA,8CAA6C,EAAE,aAAa,EAAC;AAC7D,mBAAmB,GAAG,sBAAsB;AAC5C;AACA;AACA;AACA,aAAa,mBAAO,CAAC,uCAAiB;AACtC;AACA;AACA;AACA;AACA;AACA;AACA,sBAAsB;AACtB;AACA;AACA;AACA,mBAAmB;AACnB;;;;;;;;;;;ACpBa;AACb;AACA;AACA,mCAAmC,oCAAoC,gBAAgB;AACvF,CAAC;AACD;AACA;AACA,CAAC;AACD;AACA;AACA;AACA,8CAA6C,EAAE,aAAa,EAAC;AAC7D,aAAa,mBAAO,CAAC,qCAAY;AACjC,aAAa,mBAAO,CAAC,yCAAc;AACnC;;;;;;;;;;ACdA;AACA,kCAAkC,mBAAO,CAAC,qGAAgD;AAC1F;AACA;AACA,kDAAkD,oBAAoB,8BAA8B,gCAAgC,wBAAwB,KAAK,4BAA4B,wBAAwB,kBAAkB,KAAK,8BAA8B,kBAAkB,KAAK;AACjS;AACA;;;;;;;;;;;;ACNa;;AAEb;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iBAAiB;;AAEjB;AACA;AACA;;AAEA;AACA,4CAA4C,qBAAqB;AACjE;;AAEA;AACA,KAAK;AACL,KAAK;AACL;;;AAGA;AACA;AACA;AACA;AACA;;AAEA;;AAEA;AACA,sBAAsB,iBAAiB;AACvC;AACA;;AAEA;AACA;AACA;AACA;AACA;;AAEA,qBAAqB,qBAAqB;AAC1C;;AAEA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA,UAAU;AACV;AACA;AACA;;AAEA;AACA;AACA;;AAEA;AACA;;AAEA;AACA,+BAA+B;;AAE/B;;AAEA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,KAAK;AACL;AACA;;AAEA;AACA,EAAE;;;AAGF;AACA;AACA;AACA,qDAAqD,cAAc;AACnE;AACA;;;;;;;;;;AC7FA,UAAU,mBAAO,CAAC,oJAAwE;AAC1F,0BAA0B,mBAAO,CAAC,qHAAuD;;AAEzF;;AAEA;AACA;AACA;;AAEA;;AAEA;AACA;;AAEA;;;;AAIA;;;;;;;;;;;AClBa;;AAEb;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA,CAAC;;AAED;AACA;AACA;AACA;AACA,wDAAwD;;AAExD;AACA;AACA;AACA;AACA;AACA,UAAU;AACV;AACA;AACA;AACA;;AAEA;AACA;;AAEA;AACA;AACA,CAAC;;AAED;;AAEA;AACA;;AAEA,kBAAkB,wBAAwB;AAC1C;AACA;AACA;AACA;AACA;;AAEA;AACA;;AAEA;AACA;AACA;;AAEA,kBAAkB,iBAAiB;AACnC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA,MAAM;AACN;AACA;AACA;AACA;AACA,OAAO;AACP;;AAEA;AACA;;AAEA;AACA;;AAEA;AACA;AACA;;AAEA;AACA,gBAAgB,KAAwC,GAAG,sBAAiB,GAAG,CAAI;;AAEnF;AACA;AACA;AACA;;AAEA;AACA;AACA,GAAG;;AAEH;AACA;AACA,IAAI;AACJ;;AAEA;AACA;AACA;;AAEA;AACA;;AAEA;AACA;;AAEA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;;;AAGA;AACA;AACA;AACA;AACA;AACA;AACA,CAAC;;AAED;AACA,qEAAqE,qBAAqB,cAAc;;AAExG;;AAEA;AACA;AACA,IAAI;AACJ;AACA;;AAEA;AACA;AACA;;AAEA;AACA;AACA,MAAM;AACN;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;;AAEA;AACA;AACA,IAAI;AACJ;AACA;;AAEA;AACA,yDAAyD;AACzD,IAAI;;AAEJ;;;AAGA;AACA;AACA,IAAI;AACJ;AACA;AACA;;AAEA;AACA;AACA;;AAEA;AACA;;AAEA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;;AAEA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA,MAAM;AACN;AACA;AACA;AACA;;AAEA;AACA,2BAA2B;AAC3B;;AAEA;AACA;AACA;;AAEA;AACA;AACA;AACA;;AAEA;AACA;AACA;;AAEA,oBAAoB,4BAA4B;AAChD;AACA;AACA;AACA;;AAEA;;AAEA,qBAAqB,6BAA6B;AAClD;;AAEA;;AAEA;AACA;;AAEA;AACA;AACA;;AAEA;AACA;AACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://ipywebgl/./lib/arraybuffer.js",
         "webpack://ipywebgl/./lib/glresource.js",
         "webpack://ipywebgl/./lib/glviewer.js",
```

### Comparing `ipywebgl-0.2.1/ipywebgl/labextension/static/remoteEntry.21206eb8a87189c75dc8.js` & `ipywebgl-0.2.2/ipywebgl/labextension/static/remoteEntry.8194deb74d0ed2d99f98.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -155,15 +155,15 @@
     (() => {
         /******/ // This function allow to reference async chunks
         /******/
         __webpack_require__.u = (chunkId) => {
             /******/ // return url for filenames based on template
             /******/
             return "" + chunkId + "." + {
-                "lib_widgets_js": "9b129eb1485cff28d239",
+                "lib_widgets_js": "417df79f43e89915d69a",
                 "lib_index_js": "115506ce89c3f4c34456",
                 "lib_plugin_js": "a4fea4dfcfff14540990"
             } [chunkId] + ".js";
             /******/
         };
         /******/
     })();
@@ -372,15 +372,15 @@
             /******/
             var promises = [];
             /******/
             switch (name) {
                 /******/
                 case "default": {
                     /******/
-                    register("ipywebgl", "0.2.1", () => (Promise.all([__webpack_require__.e("lib_widgets_js"), __webpack_require__.e("lib_index_js")]).then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
+                    register("ipywebgl", "0.2.2", () => (Promise.all([__webpack_require__.e("lib_widgets_js"), __webpack_require__.e("lib_index_js")]).then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
                     /******/
                 }
                 /******/
                 break;
                 /******/
             }
             /******/
@@ -1011,8 +1011,8 @@
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/ipywebgl");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB).ipywebgl = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.21206eb8a87189c75dc8.js.map
+//# sourceMappingURL=remoteEntry.8194deb74d0ed2d99f98.js.map
```

### Comparing `ipywebgl-0.2.1/ipywebgl/labextension/static/remoteEntry.21206eb8a87189c75dc8.js.map` & `ipywebgl-0.2.2/ipywebgl/labextension/static/remoteEntry.8194deb74d0ed2d99f98.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9126984126984128%*

 * *Differences: {"'file'": "'remoteEntry.8194deb74d0ed2d99f98.js'",*

 * * "'sourcesContent'": "{insert: [(4, '// This function allow to reference async "*

 * *                     'chunks\\n__webpack_require__.u = (chunkId) => {\\n\\t// return url for '*

 * *                     'filenames based on template\\n\\treturn "" + chunkId + "." + '*

 * *                     '{"lib_widgets_js":"417df79f43e89915d69a","lib_index_js":"115506ce89c3f4c34456","lib_plugin_js":"a4fea4dfcfff14540990"}[chunkId] '*

 * *                     '+ ".js";\\n};\'), (8, \'_ […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "remoteEntry.21206eb8a87189c75dc8.js",
+    "file": "remoteEntry.8194deb74d0ed2d99f98.js",
     "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCjCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,qHAAqH;WACnJ;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCxCA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC3CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WCfA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WCvKA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://ipywebgl/webpack/container-entry",
         "webpack://ipywebgl/webpack/bootstrap",
         "webpack://ipywebgl/webpack/runtime/define property getters",
@@ -22,19 +22,19 @@
         "webpack://ipywebgl/webpack/after-startup"
     ],
     "sourcesContent": [
         "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"lib_widgets_js\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"lib_widgets_js\"), __webpack_require__.e(\"lib_plugin_js\")]).then(() => (() => ((__webpack_require__(/*! ./lib/plugin */ \"./lib/plugin.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId].call(module.exports, module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_widgets_js\":\"9b129eb1485cff28d239\",\"lib_index_js\":\"115506ce89c3f4c34456\",\"lib_plugin_js\":\"a4fea4dfcfff14540990\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_widgets_js\":\"417df79f43e89915d69a\",\"lib_index_js\":\"115506ce89c3f4c34456\",\"lib_plugin_js\":\"a4fea4dfcfff14540990\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"ipywebgl:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t};\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"ipywebgl\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"ipywebgl\", \"0.2.1\", () => (Promise.all([__webpack_require__.e(\"lib_widgets_js\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"ipywebgl\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"ipywebgl\", \"0.2.2\", () => (Promise.all([__webpack_require__.e(\"lib_widgets_js\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) scriptUrl = scripts[scripts.length - 1].src\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
         "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) typeof console !== \"undefined\" && console.warn && console.warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\ttypeof console !== \"undefined\" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyter-widgets/base\": () => (loadSingletonVersionCheck(\"default\", \"@jupyter-widgets/base\", [,[1,6],[1,5],[1,4],[1,3],[1,2],[1,1,1,10],1,1,1,1,1]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_widgets_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyter-widgets/base\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"ipywebgl\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t} else installedChunks[chunkId] = 0;\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkipywebgl\"] = self[\"webpackChunkipywebgl\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "__webpack_require__.nc = undefined;",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/ipywebgl\");\n",
         ""
```

### Comparing `ipywebgl-0.2.1/ipywebgl/nbextension/index.js` & `ipywebgl-0.2.2/ipywebgl/nbextension/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -998,15 +998,15 @@
             },
             146: t => {
                 "use strict";
                 t.exports = e
             },
             147: e => {
                 "use strict";
-                e.exports = JSON.parse('{"name":"ipywebgl","version":"0.2.1","description":"A Custom Jupyter Widget Library","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/JeromeEippers/ipywebgl","bugs":{"url":"https://github.com/JeromeEippers/ipywebgl/issues"},"license":"BSD-3-Clause","author":{"name":"Jerome Eippers","email":"jerome@eippers.be"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/JeromeEippers/ipywebgl"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipywebgl/labextension","clean:nbextension":"rimraf ipywebgl/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipywebgl/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+                e.exports = JSON.parse('{"name":"ipywebgl","version":"0.2.2","description":"A Custom Jupyter Widget Library","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/JeromeEippers/ipywebgl","bugs":{"url":"https://github.com/JeromeEippers/ipywebgl/issues"},"license":"BSD-3-Clause","author":{"name":"Jerome Eippers","email":"jerome@eippers.be"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/JeromeEippers/ipywebgl"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipywebgl/labextension","clean:nbextension":"rimraf ipywebgl/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipywebgl/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
             }
         },
         r = {};
 
     function a(e) {
         var i = r[e];
         if (void 0 !== i) return i.exports;
```

### Comparing `ipywebgl-0.2.1/ipywebgl/nbextension/index.js.map` & `ipywebgl-0.2.2/ipywebgl/nbextension/index.js.map`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/src/arraybuffer.ts` & `ipywebgl-0.2.2/src/arraybuffer.ts`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/src/extension.ts` & `ipywebgl-0.2.2/src/extension.ts`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/src/glresource.ts` & `ipywebgl-0.2.2/src/glresource.ts`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/src/glviewer.ts` & `ipywebgl-0.2.2/src/glviewer.ts`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/src/matrix.ts` & `ipywebgl-0.2.2/src/matrix.ts`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/src/plugin.ts` & `ipywebgl-0.2.2/src/plugin.ts`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/src/version.ts` & `ipywebgl-0.2.2/src/version.ts`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/.gitignore` & `ipywebgl-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/LICENSE.txt` & `ipywebgl-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/README.md` & `ipywebgl-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ipywebgl-0.2.1/pyproject.toml` & `ipywebgl-0.2.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
     "ipywidgets>=7.0.0",
     "numpy",
 ]
-version = "0.2.1"
+version = "0.2.2"
 
 [project.optional-dependencies]
 docs = [
     "jupyter_sphinx",
     "nbsphinx",
     "nbsphinx-link",
     "pypandoc",
```

### Comparing `ipywebgl-0.2.1/PKG-INFO` & `ipywebgl-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipywebgl
-Version: 0.2.1
+Version: 0.2.2
 Summary: WebGL2 jupyter widget
 Project-URL: Homepage, https://github.com/JeromeEippers/ipywebgl
 Project-URL: Documentation, https://ipywebgl.readthedocs.io/en/latest/index.html
 Author-email: Jerome Eippers <jerome@eippers.be>
 License: Copyright (c) 2023 Jerome Eippers
         All rights reserved.
```

