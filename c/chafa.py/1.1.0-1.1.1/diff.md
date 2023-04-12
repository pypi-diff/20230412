# Comparing `tmp/chafa.py-1.1.0.tar.gz` & `tmp/chafa.py-1.1.1.tar.gz`

## Comparing `chafa.py-1.1.0.tar` & `chafa.py-1.1.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 chafa_py-1.1.0/TODO.md
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 chafa_py-1.1.0/docs/Makefile
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 chafa_py-1.1.0/docs/conf.py
--rw-r--r--   0        0        0   182328 2020-02-02 00:00:00.000000 chafa_py-1.1.0/docs/crunchyfy.png
--rw-r--r--   0        0        0   123186 2020-02-02 00:00:00.000000 chafa_py-1.1.0/docs/crunchyfy.svg
--rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 chafa_py-1.1.0/docs/index.rst
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 chafa_py-1.1.0/docs/make.bat
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 chafa_py-1.1.0/docs/requirements.txt
--rw-r--r--   0        0        0    71540 2020-02-02 00:00:00.000000 chafa_py-1.1.0/docs/_chafa_img/snake.html
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 chafa_py-1.1.0/docs/_scripts/img_to_html.py
--rw-r--r--   0        0        0     6179 2020-02-02 00:00:00.000000 chafa_py-1.1.0/docs/_static/custom.css
--rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 chafa_py-1.1.0/docs/_static/table.js
--rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 chafa_py-1.1.0/docs/api/Canvas.rst
--rw-r--r--   0        0        0     7400 2020-02-02 00:00:00.000000 chafa_py-1.1.0/docs/api/CanvasConfig.rst
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 chafa_py-1.1.0/docs/api/Functions.rst
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 chafa_py-1.1.0/docs/api/Loader.rst
--rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 chafa_py-1.1.0/docs/api/SymbolMap.rst
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 chafa_py-1.1.0/docs/api/TermDb.rst
--rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 chafa_py-1.1.0/docs/api/TermInfo.rst
--rw-r--r--   0        0        0    14954 2020-02-02 00:00:00.000000 chafa_py-1.1.0/docs/api/enums.rst
--rw-r--r--   0        0        0     8919 2020-02-02 00:00:00.000000 chafa_py-1.1.0/docs/usage/examples.rst
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 chafa_py-1.1.0/docs/usage/installation.rst
--rw-r--r--   0        0        0    80589 2020-02-02 00:00:00.000000 chafa_py-1.1.0/docs/usage/snake.jpg
--rw-r--r--   0        0        0    15363 2020-02-02 00:00:00.000000 chafa_py-1.1.0/docs/usage/tutorial.rst
--rw-r--r--   0        0        0    71699 2020-02-02 00:00:00.000000 chafa_py-1.1.0/docs/usage/tutorial_img/afsnake.png
--rw-r--r--   0        0        0    71067 2020-02-02 00:00:00.000000 chafa_py-1.1.0/docs/usage/tutorial_img/alpha_snake.png
--rw-r--r--   0        0        0   485607 2020-02-02 00:00:00.000000 chafa_py-1.1.0/docs/usage/tutorial_img/grid_snake.png
--rw-r--r--   0        0        0   163677 2020-02-02 00:00:00.000000 chafa_py-1.1.0/docs/usage/tutorial_img/kitty_ok.png
--rw-r--r--   0        0        0    52962 2020-02-02 00:00:00.000000 chafa_py-1.1.0/docs/usage/tutorial_img/kitty_pixels.png
--rw-r--r--   0        0        0     9480 2020-02-02 00:00:00.000000 chafa_py-1.1.0/docs/usage/tutorial_img/selector_snake.png
--rw-r--r--   0        0        0    72741 2020-02-02 00:00:00.000000 chafa_py-1.1.0/docs/usage/tutorial_img/sixels.png
--rw-r--r--   0        0        0    10532 2020-02-02 00:00:00.000000 chafa_py-1.1.0/docs/usage/tutorial_img/snake_color.png
--rw-r--r--   0        0        0    10719 2020-02-02 00:00:00.000000 chafa_py-1.1.0/docs/usage/tutorial_img/snake_edit_char.png
--rw-r--r--   0        0        0     9496 2020-02-02 00:00:00.000000 chafa_py-1.1.0/docs/usage/tutorial_img/snake_right_aspect.png
--rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 chafa_py-1.1.0/docs/usage/tutorial_img/snake_with_a.png
--rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 chafa_py-1.1.0/docs/usage/tutorial_img/snake_wrong_aspect.png
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 chafa_py-1.1.0/examples/example_PIL.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 chafa_py-1.1.0/examples/example_aspect.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 chafa_py-1.1.0/examples/example_detect.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 chafa_py-1.1.0/examples/example_html.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 chafa_py-1.1.0/examples/example_pyvips.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 chafa_py-1.1.0/examples/example_raw_color.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 chafa_py-1.1.0/examples/example_simple.py
--rw-r--r--   0        0        0    80589 2020-02-02 00:00:00.000000 chafa_py-1.1.0/examples/snake.jpg
--rw-r--r--   0        0        0    16876 2020-02-02 00:00:00.000000 chafa_py-1.1.0/img/logo.svg
--rw-r--r--   0        0        0    12392 2020-02-02 00:00:00.000000 chafa_py-1.1.0/img/readme_snake.jpg
--rw-r--r--   0        0        0    12392 2020-02-02 00:00:00.000000 chafa_py-1.1.0/img/readme_snake.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chafa_py-1.1.0/libs/linux/LINUX_SOS_GO_HERE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chafa_py-1.1.0/libs/macos/MACOS_DYLIBS_GO_HERE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chafa_py-1.1.0/libs/windows/WINDOWS_DLLS_GO_HERE
--rw-r--r--   0        0        0   289788 2020-02-02 00:00:00.000000 chafa_py-1.1.0/libs/windows/libchafa-0.dll
--rw-r--r--   0        0        0  1383156 2020-02-02 00:00:00.000000 chafa_py-1.1.0/libs/windows/libglib-2.0-0.dll
--rw-r--r--   0        0        0  1114369 2020-02-02 00:00:00.000000 chafa_py-1.1.0/libs/windows/libiconv-2.dll
--rw-r--r--   0        0        0   136724 2020-02-02 00:00:00.000000 chafa_py-1.1.0/libs/windows/libintl-8.dll
--rw-r--r--   0        0        0   393081 2020-02-02 00:00:00.000000 chafa_py-1.1.0/libs/windows/libpcre2-8-0.dll
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 chafa_py-1.1.0/src/chafa/__init__.py
--rw-r--r--   0        0        0    83066 2020-02-02 00:00:00.000000 chafa_py-1.1.0/src/chafa/chafa.py
--rw-r--r--   0        0        0     5736 2020-02-02 00:00:00.000000 chafa_py-1.1.0/src/chafa/loader.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 chafa_py-1.1.0/tests/0_PIL_test.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 chafa_py-1.1.0/tests/1_aspect_test.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 chafa_py-1.1.0/tests/2_raw_test.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 chafa_py-1.1.0/tests/3_capabilities_test.py
--rw-r--r--   0        0        0    80589 2020-02-02 00:00:00.000000 chafa_py-1.1.0/tests/snake.jpg
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 chafa_py-1.1.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 chafa_py-1.1.0/COPYING
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 chafa_py-1.1.0/COPYING.LESSER
--rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 chafa_py-1.1.0/README.md
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 chafa_py-1.1.0/hatch_build.py
--rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 chafa_py-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 chafa_py-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 chafa_py-1.1.1/TODO.md
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/Makefile
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/conf.py
+-rw-r--r--   0        0        0   182328 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/crunchyfy.png
+-rw-r--r--   0        0        0   123186 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/crunchyfy.svg
+-rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/index.rst
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/make.bat
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/requirements.txt
+-rw-r--r--   0        0        0    71540 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/_chafa_img/snake.html
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/_scripts/img_to_html.py
+-rw-r--r--   0        0        0     6179 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/_static/custom.css
+-rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/_static/table.js
+-rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/api/Canvas.rst
+-rw-r--r--   0        0        0     7400 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/api/CanvasConfig.rst
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/api/Functions.rst
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/api/Loader.rst
+-rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/api/SymbolMap.rst
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/api/TermDb.rst
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/api/TermInfo.rst
+-rw-r--r--   0        0        0    14954 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/api/enums.rst
+-rw-r--r--   0        0        0     8851 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/usage/examples.rst
+-rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/usage/installation.rst
+-rw-r--r--   0        0        0    80589 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/usage/snake.jpg
+-rw-r--r--   0        0        0    15363 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/usage/tutorial.rst
+-rw-r--r--   0        0        0    71699 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/usage/tutorial_img/afsnake.png
+-rw-r--r--   0        0        0    71067 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/usage/tutorial_img/alpha_snake.png
+-rw-r--r--   0        0        0   485607 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/usage/tutorial_img/grid_snake.png
+-rw-r--r--   0        0        0   163677 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/usage/tutorial_img/kitty_ok.png
+-rw-r--r--   0        0        0    52962 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/usage/tutorial_img/kitty_pixels.png
+-rw-r--r--   0        0        0     9480 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/usage/tutorial_img/selector_snake.png
+-rw-r--r--   0        0        0    72741 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/usage/tutorial_img/sixels.png
+-rw-r--r--   0        0        0    10532 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/usage/tutorial_img/snake_color.png
+-rw-r--r--   0        0        0    10719 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/usage/tutorial_img/snake_edit_char.png
+-rw-r--r--   0        0        0     9496 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/usage/tutorial_img/snake_right_aspect.png
+-rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/usage/tutorial_img/snake_with_a.png
+-rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/usage/tutorial_img/snake_wrong_aspect.png
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 chafa_py-1.1.1/examples/example_PIL.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 chafa_py-1.1.1/examples/example_aspect.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 chafa_py-1.1.1/examples/example_detect.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 chafa_py-1.1.1/examples/example_html.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 chafa_py-1.1.1/examples/example_pyvips.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 chafa_py-1.1.1/examples/example_raw_color.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 chafa_py-1.1.1/examples/example_simple.py
+-rw-r--r--   0        0        0    80589 2020-02-02 00:00:00.000000 chafa_py-1.1.1/examples/snake.jpg
+-rw-r--r--   0        0        0    16876 2020-02-02 00:00:00.000000 chafa_py-1.1.1/img/logo.svg
+-rw-r--r--   0        0        0    12392 2020-02-02 00:00:00.000000 chafa_py-1.1.1/img/readme_snake.jpg
+-rw-r--r--   0        0        0    12392 2020-02-02 00:00:00.000000 chafa_py-1.1.1/img/readme_snake.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chafa_py-1.1.1/libs/linux/LINUX_SOS_GO_HERE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chafa_py-1.1.1/libs/macos/MACOS_DYLIBS_GO_HERE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chafa_py-1.1.1/libs/windows/WINDOWS_DLLS_GO_HERE
+-rw-r--r--   0        0        0   289788 2020-02-02 00:00:00.000000 chafa_py-1.1.1/libs/windows/libchafa-0.dll
+-rw-r--r--   0        0        0  1383156 2020-02-02 00:00:00.000000 chafa_py-1.1.1/libs/windows/libglib-2.0-0.dll
+-rw-r--r--   0        0        0  1114369 2020-02-02 00:00:00.000000 chafa_py-1.1.1/libs/windows/libiconv-2.dll
+-rw-r--r--   0        0        0   136724 2020-02-02 00:00:00.000000 chafa_py-1.1.1/libs/windows/libintl-8.dll
+-rw-r--r--   0        0        0   393081 2020-02-02 00:00:00.000000 chafa_py-1.1.1/libs/windows/libpcre2-8-0.dll
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 chafa_py-1.1.1/src/chafa/__init__.py
+-rw-r--r--   0        0        0    83257 2020-02-02 00:00:00.000000 chafa_py-1.1.1/src/chafa/chafa.py
+-rw-r--r--   0        0        0     5736 2020-02-02 00:00:00.000000 chafa_py-1.1.1/src/chafa/loader.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 chafa_py-1.1.1/tests/0_PIL_test.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 chafa_py-1.1.1/tests/1_aspect_test.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 chafa_py-1.1.1/tests/2_raw_test.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 chafa_py-1.1.1/tests/3_capabilities_test.py
+-rw-r--r--   0        0        0    80589 2020-02-02 00:00:00.000000 chafa_py-1.1.1/tests/snake.jpg
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 chafa_py-1.1.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 chafa_py-1.1.1/COPYING
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 chafa_py-1.1.1/COPYING.LESSER
+-rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 chafa_py-1.1.1/README.md
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 chafa_py-1.1.1/hatch_build.py
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 chafa_py-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 chafa_py-1.1.1/PKG-INFO
```

### Comparing `chafa_py-1.1.0/TODO.md` & `chafa_py-1.1.1/TODO.md`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/docs/Makefile` & `chafa_py-1.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/docs/conf.py` & `chafa_py-1.1.1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import sys
 sys.path.append('../src/chafa')
 
 project = 'chafa.py'
 copyright = '2022, Erica Ferrua Edwardsdóttir'
 author = 'Erica Ferrua Edwardsdóttir'
-release = '1.1.0'
+release = '1.1.1'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     'sphinxemoji.sphinxemoji',
     'sphinx.ext.intersphinx',
```

### Comparing `chafa_py-1.1.0/docs/crunchyfy.png` & `chafa_py-1.1.1/docs/crunchyfy.png`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/docs/crunchyfy.svg` & `chafa_py-1.1.1/docs/crunchyfy.svg`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/docs/index.rst` & `chafa_py-1.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/docs/make.bat` & `chafa_py-1.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/docs/_chafa_img/snake.html` & `chafa_py-1.1.1/docs/_chafa_img/snake.html`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/docs/_scripts/img_to_html.py` & `chafa_py-1.1.1/docs/_scripts/img_to_html.py`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/docs/_static/custom.css` & `chafa_py-1.1.1/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/docs/_static/table.js` & `chafa_py-1.1.1/docs/_static/table.js`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/docs/api/Canvas.rst` & `chafa_py-1.1.1/docs/api/Canvas.rst`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/docs/api/CanvasConfig.rst` & `chafa_py-1.1.1/docs/api/CanvasConfig.rst`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/docs/api/Functions.rst` & `chafa_py-1.1.1/docs/api/Functions.rst`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/docs/api/Loader.rst` & `chafa_py-1.1.1/docs/api/Loader.rst`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/docs/api/SymbolMap.rst` & `chafa_py-1.1.1/docs/api/SymbolMap.rst`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/docs/api/TermDb.rst` & `chafa_py-1.1.1/docs/api/TermDb.rst`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/docs/api/TermInfo.rst` & `chafa_py-1.1.1/docs/api/TermInfo.rst`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/docs/api/enums.rst` & `chafa_py-1.1.1/docs/api/enums.rst`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/docs/usage/examples.rst` & `chafa_py-1.1.1/docs/usage/examples.rst`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,14 @@
 
 When reading pixel data from an image opened with `Pillow`_, we get a 2D array which needs to be reshaped into a 1D array before passing to chafa. This is still pretty fast since both Pillow and NumPy are well optimized.
 
 ::
 
     from chafa import *
     from PIL import Image
-    import numpy as np
 
     # Init canvas config
     config = CanvasConfig()
 
     # Set canvas height and width
     config.height = 30
     config.width  = 30
@@ -83,16 +82,15 @@
     image = Image.open("./snake.jpg")
 
     width  = image.width
     height = image.height
     bands  = len(image.getbands())
 
     # Put image into correct format
-    pixels = np.array(image)
-    pixels = np.reshape(pixels, pixels.size)
+    pixels = image.tobytes()
 
     # Init the canvas
     canvas = Canvas(config)
 
     # Draw to canvas
     canvas.draw_all_pixels(
         PixelType.CHAFA_PIXEL_RGB8,
```

### Comparing `chafa_py-1.1.0/docs/usage/installation.rst` & `chafa_py-1.1.1/docs/usage/installation.rst`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/docs/usage/snake.jpg` & `chafa_py-1.1.1/docs/usage/snake.jpg`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/docs/usage/tutorial.rst` & `chafa_py-1.1.1/docs/usage/tutorial.rst`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/docs/usage/tutorial_img/afsnake.png` & `chafa_py-1.1.1/docs/usage/tutorial_img/afsnake.png`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/docs/usage/tutorial_img/alpha_snake.png` & `chafa_py-1.1.1/docs/usage/tutorial_img/alpha_snake.png`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/docs/usage/tutorial_img/grid_snake.png` & `chafa_py-1.1.1/docs/usage/tutorial_img/grid_snake.png`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/docs/usage/tutorial_img/kitty_ok.png` & `chafa_py-1.1.1/docs/usage/tutorial_img/kitty_ok.png`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/docs/usage/tutorial_img/kitty_pixels.png` & `chafa_py-1.1.1/docs/usage/tutorial_img/kitty_pixels.png`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/docs/usage/tutorial_img/selector_snake.png` & `chafa_py-1.1.1/docs/usage/tutorial_img/selector_snake.png`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/docs/usage/tutorial_img/sixels.png` & `chafa_py-1.1.1/docs/usage/tutorial_img/sixels.png`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/docs/usage/tutorial_img/snake_color.png` & `chafa_py-1.1.1/docs/usage/tutorial_img/snake_color.png`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/docs/usage/tutorial_img/snake_edit_char.png` & `chafa_py-1.1.1/docs/usage/tutorial_img/snake_edit_char.png`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/docs/usage/tutorial_img/snake_right_aspect.png` & `chafa_py-1.1.1/docs/usage/tutorial_img/snake_right_aspect.png`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/docs/usage/tutorial_img/snake_with_a.png` & `chafa_py-1.1.1/docs/usage/tutorial_img/snake_with_a.png`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/docs/usage/tutorial_img/snake_wrong_aspect.png` & `chafa_py-1.1.1/docs/usage/tutorial_img/snake_wrong_aspect.png`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/examples/example_aspect.py` & `chafa_py-1.1.1/examples/example_aspect.py`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/examples/example_detect.py` & `chafa_py-1.1.1/examples/example_detect.py`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/examples/example_html.py` & `chafa_py-1.1.1/examples/example_html.py`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/examples/example_pyvips.py` & `chafa_py-1.1.1/examples/example_pyvips.py`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/examples/example_raw_color.py` & `chafa_py-1.1.1/examples/example_raw_color.py`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/examples/example_simple.py` & `chafa_py-1.1.1/examples/example_simple.py`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/examples/snake.jpg` & `chafa_py-1.1.1/examples/snake.jpg`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/img/logo.svg` & `chafa_py-1.1.1/img/logo.svg`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/img/readme_snake.jpg` & `chafa_py-1.1.1/img/readme_snake.jpg`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/img/readme_snake.png` & `chafa_py-1.1.1/img/readme_snake.png`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/libs/windows/libchafa-0.dll` & `chafa_py-1.1.1/libs/windows/libchafa-0.dll`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/libs/windows/libglib-2.0-0.dll` & `chafa_py-1.1.1/libs/windows/libglib-2.0-0.dll`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/libs/windows/libiconv-2.dll` & `chafa_py-1.1.1/libs/windows/libiconv-2.dll`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/libs/windows/libintl-8.dll` & `chafa_py-1.1.1/libs/windows/libintl-8.dll`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/libs/windows/libpcre2-8-0.dll` & `chafa_py-1.1.1/libs/windows/libpcre2-8-0.dll`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/src/chafa/__init__.py` & `chafa_py-1.1.1/src/chafa/__init__.py`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/src/chafa/chafa.py` & `chafa_py-1.1.1/src/chafa/chafa.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,21 +338,30 @@
         char = sys.stdin.read(1)
 
     # Set terminal back to normal
     termios.tcsetattr(stdin_fileno, termios.TCSANOW, old_term)
 
     # Split attributes by ; and turn them into integers
     if len(attributes) >= 4:
-        attributes = "".join(attributes[3:])
-        attributes = tuple([int(i) for i in attributes.split(";")])
+        attributes = "".join(attributes[3:]).split(";")
+
+        # Convert all attributes to ints unless we can't, then we skip
+        out = []
+        for attrib in attributes:
+            try:
+                out.append(int(attrib))
+            except ValueError:
+                continue
+
+        out = tuple(out)
 
     else:
-        attributes = tuple()
+        out = tuple()
 
-    return attributes
+    return out
 
 
 class ReadOnlySymbolMap():
     def __init__(self):
         # Init map
         _Chafa.chafa_symbol_map_new.restype = ctypes.c_void_p
         self._symbol_map = _Chafa.chafa_symbol_map_new()
```

### Comparing `chafa_py-1.1.0/src/chafa/loader.py` & `chafa_py-1.1.1/src/chafa/loader.py`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/tests/0_PIL_test.py` & `chafa_py-1.1.1/tests/0_PIL_test.py`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/tests/1_aspect_test.py` & `chafa_py-1.1.1/tests/1_aspect_test.py`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/tests/2_raw_test.py` & `chafa_py-1.1.1/tests/2_raw_test.py`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/tests/snake.jpg` & `chafa_py-1.1.1/tests/snake.jpg`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/.gitignore` & `chafa_py-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/COPYING` & `chafa_py-1.1.1/COPYING`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/COPYING.LESSER` & `chafa_py-1.1.1/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/README.md` & `chafa_py-1.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -12,19 +12,14 @@
   <p>
     <img alt="PyPI" src="https://img.shields.io/pypi/v/chafa.py?label=version&style=flat-square">
     &nbsp;
     <img alt="GitHub Workflow Status" src="https://img.shields.io/github/actions/workflow/status/GuardKenzie/chafa.py/build_wheels.yml?style=flat-square">
     &nbsp;
     <img alt="Sneks" src="https://img.shields.io/badge/snakes%20go-sssss-cbd446?style=flat-square">  
   </p>
-  <p>
-    <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/chafa.py?style=flat-square">
-    &nbsp;
-    <img alt="GitHub commits since latest release (by SemVer)" src="https://img.shields.io/github/commits-since/GuardKenzie/chafa.py/latest?style=flat-square">
-  </p>
 </div>
 
 # What is this?
 
 Have you ever wanted to display an image your TUI Python application? Well, now you can!
 
 [Chafa](https://hpjansson.org/chafa/) is a wonderful command-line utility,
```

#### html2text {}

```diff
@@ -1,15 +1,14 @@
                                         
                                   [chafa.py]
                                         
                         Terminal graphics with Python!
                  ð_Docs  -  ð±_Tutorial  -  ð¾_Examples
                                       â
                   [PyPI]   [GitHub Workflow Status]   [Sneks]
-    [PyPI - Downloads]   [GitHub commits since latest release (by SemVer)]
 # What is this? Have you ever wanted to display an image your TUI Python
 application? Well, now you can! [Chafa](https://hpjansson.org/chafa/) is a
 wonderful command-line utility, created by [Hans Petter Jansson](https://
 hpjansson.org/), for visualizing images in the terminal. In Jansson's own
 words: > **The future is (still) now!** > > The premier UX of the 21st century
 just got a little better: > With `chafa`, you can now view very, very
 reasonable approximations > of pictures and animations in the comfort of your
```

### Comparing `chafa_py-1.1.0/hatch_build.py` & `chafa_py-1.1.1/hatch_build.py`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.0/pyproject.toml` & `chafa_py-1.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name    = "chafa.py"
-version = "1.1.0"
+version = "1.1.1"
 license = "LGPL-3.0"
 
 authors = [
     { name="Erica Ferrua Edwardsdóttir", email="e@mage.black" }
 ]
 
 description = "Python bindings for Chafa. Visualize images with text in python. "
@@ -55,14 +55,30 @@
     "make",
     "cd ../",
     "cp libchafa_src/chafa/.libs/*chafa.so linux/"
 ]
 
 repair-wheel-command = "auditwheel repair -w {dest_dir} {wheel}"
 
+[[tool.cibuildwheel.overrides]]
+select = "*linux_aarch64"
+
+before-all = [
+    "yum install -y libtool ImageMagick-devel",
+    "cd libs",
+    "git clone --branch 1.12.4 https://github.com/hpjansson/chafa libchafa_src",
+    "cd libchafa_src",
+    "mkdir m4",
+    "cp /usr/share/aclocal/pkg.m4 m4/",
+    "./autogen.sh --without-tools",
+    "make",
+    "cd ../",
+    "cp libchafa_src/chafa/.libs/*chafa.so linux/"
+]
+
 [tool.cibuildwheel.macos]
 before-all = [
     "NONINTERACTIVE=1 /bin/bash -c \"$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)\"",
     "brew install make libtool pkg-config glib automake imagemagick",
     "ln -s $(which glibtoolize) /usr/local/bin/libtoolize",
     "git clone --branch 1.12.4 https://github.com/hpjansson/chafa libchafa_src",
     "cd libchafa_src",
```

### Comparing `chafa_py-1.1.0/PKG-INFO` & `chafa_py-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chafa.py
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python bindings for Chafa. Visualize images with text in python. 
 Project-URL: Homepage, https://chafapy.mage.black
 Project-URL: Source, https://github.com/guardkenzie/chafa.py
 Project-URL: Bug Tracker, https://github.com/guardkenzie/chafa.py/issues
 Author-email: Erica Ferrua Edwardsdóttir <e@mage.black>
 License-Expression: LGPL-3.0
 License-File: COPYING
@@ -31,19 +31,14 @@
   <p>
     <img alt="PyPI" src="https://img.shields.io/pypi/v/chafa.py?label=version&style=flat-square">
     &nbsp;
     <img alt="GitHub Workflow Status" src="https://img.shields.io/github/actions/workflow/status/GuardKenzie/chafa.py/build_wheels.yml?style=flat-square">
     &nbsp;
     <img alt="Sneks" src="https://img.shields.io/badge/snakes%20go-sssss-cbd446?style=flat-square">  
   </p>
-  <p>
-    <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/chafa.py?style=flat-square">
-    &nbsp;
-    <img alt="GitHub commits since latest release (by SemVer)" src="https://img.shields.io/github/commits-since/GuardKenzie/chafa.py/latest?style=flat-square">
-  </p>
 </div>
 
 # What is this?
 
 Have you ever wanted to display an image your TUI Python application? Well, now you can!
 
 [Chafa](https://hpjansson.org/chafa/) is a wonderful command-line utility,
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chafa.py Version: 1.1.0 Summary: Python bindings
+Metadata-Version: 2.1 Name: chafa.py Version: 1.1.1 Summary: Python bindings
 for Chafa. Visualize images with text in python. Project-URL: Homepage, https:/
 /chafapy.mage.black Project-URL: Source, https://github.com/guardkenzie/
 chafa.py Project-URL: Bug Tracker, https://github.com/guardkenzie/chafa.py/
 issues Author-email: Erica Ferrua EdwardsdÃ³ttir
 mage.black> License-Expression: LGPL-3.0 License-File: COPYING License-File:
 COPYING.LESSER Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v3 (LGPLv3) Classifier: Operating System :: MacOS Classifier: Operating
@@ -12,15 +12,14 @@
                                         
                                   [chafa.py]
                                         
                         Terminal graphics with Python!
                  ð_Docs  -  ð±_Tutorial  -  ð¾_Examples
                                       â
                   [PyPI]   [GitHub Workflow Status]   [Sneks]
-    [PyPI - Downloads]   [GitHub commits since latest release (by SemVer)]
 # What is this? Have you ever wanted to display an image your TUI Python
 application? Well, now you can! [Chafa](https://hpjansson.org/chafa/) is a
 wonderful command-line utility, created by [Hans Petter Jansson](https://
 hpjansson.org/), for visualizing images in the terminal. In Jansson's own
 words: > **The future is (still) now!** > > The premier UX of the 21st century
 just got a little better: > With `chafa`, you can now view very, very
 reasonable approximations > of pictures and animations in the comfort of your
```

