# Comparing `tmp/toga-web-0.3.0.dev39.tar.gz` & `tmp/toga-web-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/toga-web-0.3.0.dev39.tar", last modified: Wed Oct 19 16:16:44 2022, max compression
+gzip compressed data, was "toga-web-0.3.1.tar", last modified: Wed Apr 12 01:58:58 2023, max compression
```

## Comparing `toga-web-0.3.0.dev39.tar` & `toga-web-0.3.1.tar`

### file list

```diff
@@ -1,37 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 16:16:44.000000 toga-web-0.3.0.dev39/
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-10-19 16:16:15.000000 toga-web-0.3.0.dev39/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1519 2022-10-19 16:16:15.000000 toga-web-0.3.0.dev39/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-10-19 16:16:15.000000 toga-web-0.3.0.dev39/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2651 2022-10-19 16:16:44.000000 toga-web-0.3.0.dev39/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1273 2022-10-19 16:16:15.000000 toga-web-0.3.0.dev39/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1551 2022-10-19 16:16:44.000000 toga-web-0.3.0.dev39/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      925 2022-10-19 16:16:15.000000 toga-web-0.3.0.dev39/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 16:16:44.000000 toga-web-0.3.0.dev39/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 16:16:44.000000 toga-web-0.3.0.dev39/src/toga_web/
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-10-19 16:16:15.000000 toga-web-0.3.0.dev39/src/toga_web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7305 2022-10-19 16:16:15.000000 toga-web-0.3.0.dev39/src/toga_web/app.py
--rw-r--r--   0 runner    (1001) docker     (121)      488 2022-10-19 16:16:15.000000 toga-web-0.3.0.dev39/src/toga_web/command.py
--rw-r--r--   0 runner    (1001) docker     (121)     2551 2022-10-19 16:16:15.000000 toga-web-0.3.0.dev39/src/toga_web/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1827 2022-10-19 16:16:15.000000 toga-web-0.3.0.dev39/src/toga_web/factory.py
--rw-r--r--   0 runner    (1001) docker     (121)      175 2022-10-19 16:16:15.000000 toga-web-0.3.0.dev39/src/toga_web/icons.py
--rw-r--r--   0 runner    (1001) docker     (121)     1471 2022-10-19 16:16:15.000000 toga-web-0.3.0.dev39/src/toga_web/libs.py
--rw-r--r--   0 runner    (1001) docker     (121)      749 2022-10-19 16:16:15.000000 toga-web-0.3.0.dev39/src/toga_web/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 16:16:44.000000 toga-web-0.3.0.dev39/src/toga_web/static/
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-10-19 16:16:15.000000 toga-web-0.3.0.dev39/src/toga_web/static/toga.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 16:16:44.000000 toga-web-0.3.0.dev39/src/toga_web/widgets/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 16:16:15.000000 toga-web-0.3.0.dev39/src/toga_web/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3260 2022-10-19 16:16:15.000000 toga-web-0.3.0.dev39/src/toga_web/widgets/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-10-19 16:16:15.000000 toga-web-0.3.0.dev39/src/toga_web/widgets/box.py
--rw-r--r--   0 runner    (1001) docker     (121)      612 2022-10-19 16:16:15.000000 toga-web-0.3.0.dev39/src/toga_web/widgets/button.py
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-10-19 16:16:15.000000 toga-web-0.3.0.dev39/src/toga_web/widgets/label.py
--rw-r--r--   0 runner    (1001) docker     (121)      844 2022-10-19 16:16:15.000000 toga-web-0.3.0.dev39/src/toga_web/widgets/textinput.py
--rw-r--r--   0 runner    (1001) docker     (121)     2359 2022-10-19 16:16:15.000000 toga-web-0.3.0.dev39/src/toga_web/window.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 16:16:44.000000 toga-web-0.3.0.dev39/src/toga_web.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2651 2022-10-19 16:16:44.000000 toga-web-0.3.0.dev39/src/toga_web.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      710 2022-10-19 16:16:44.000000 toga-web-0.3.0.dev39/src/toga_web.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-19 16:16:44.000000 toga-web-0.3.0.dev39/src/toga_web.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-19 16:16:43.000000 toga-web-0.3.0.dev39/src/toga_web.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-10-19 16:16:44.000000 toga-web-0.3.0.dev39/src/toga_web.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 16:16:44.000000 toga-web-0.3.0.dev39/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 16:16:15.000000 toga-web-0.3.0.dev39/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-10-19 16:16:15.000000 toga-web-0.3.0.dev39/tests/test_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:58.624592 toga-web-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-12 01:58:12.000000 toga-web-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-12 01:58:12.000000 toga-web-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-12 01:58:12.000000 toga-web-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-12 01:58:58.624592 toga-web-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-12 01:58:12.000000 toga-web-0.3.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-12 01:58:12.000000 toga-web-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-12 01:58:58.628592 toga-web-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-12 01:58:12.000000 toga-web-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:58.612592 toga-web-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:58.620592 toga-web-0.3.1/src/toga_web/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-12 01:58:12.000000 toga-web-0.3.1/src/toga_web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-04-12 01:58:12.000000 toga-web-0.3.1/src/toga_web/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-12 01:58:12.000000 toga-web-0.3.1/src/toga_web/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-04-12 01:58:12.000000 toga-web-0.3.1/src/toga_web/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-12 01:58:12.000000 toga-web-0.3.1/src/toga_web/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-12 01:58:12.000000 toga-web-0.3.1/src/toga_web/icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-12 01:58:12.000000 toga-web-0.3.1/src/toga_web/libs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-12 01:58:12.000000 toga-web-0.3.1/src/toga_web/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:58.624592 toga-web-0.3.1/src/toga_web/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-12 01:58:12.000000 toga-web-0.3.1/src/toga_web/static/toga.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:58.624592 toga-web-0.3.1/src/toga_web/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:12.000000 toga-web-0.3.1/src/toga_web/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-04-12 01:58:12.000000 toga-web-0.3.1/src/toga_web/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-12 01:58:12.000000 toga-web-0.3.1/src/toga_web/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-12 01:58:12.000000 toga-web-0.3.1/src/toga_web/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-12 01:58:12.000000 toga-web-0.3.1/src/toga_web/widgets/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-12 01:58:12.000000 toga-web-0.3.1/src/toga_web/widgets/textinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-12 01:58:12.000000 toga-web-0.3.1/src/toga_web/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:58.624592 toga-web-0.3.1/src/toga_web.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-12 01:58:58.000000 toga-web-0.3.1/src/toga_web.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-12 01:58:58.000000 toga-web-0.3.1/src/toga_web.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 01:58:58.000000 toga-web-0.3.1/src/toga_web.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-12 01:58:58.000000 toga-web-0.3.1/src/toga_web.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 01:58:44.000000 toga-web-0.3.1/src/toga_web.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-12 01:58:58.000000 toga-web-0.3.1/src/toga_web.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 01:58:58.000000 toga-web-0.3.1/src/toga_web.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:58.624592 toga-web-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:12.000000 toga-web-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-12 01:58:12.000000 toga-web-0.3.1/tests/test_implementation.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `toga-web-0.3.0.dev39/LICENSE` & `toga-web-0.3.1/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR
 ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `toga-web-0.3.0.dev39/PKG-INFO` & `toga-web-0.3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toga-web
-Version: 0.3.0.dev39
+Version: 0.3.1
 Summary: A common backend for the Toga widget toolkit on web platforms.
 Home-page: https://beeware.org/project/projects/libraries/toga/
 Author: Russell Keith-Magee
 Author-email: russell@keith-magee.com
 Maintainer: BeeWare Team
 Maintainer-email: team@beeware.org
 License: New BSD
@@ -18,52 +18,60 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Software Development :: Widget Sets
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst; charset=UTF-8
-License-File: LICENSE
 
 toga-web
 ========
 
 A common backend for the `Toga widget toolkit`_ on web platforms.
 
 This package isn't much use by itself; it needs to be combined with `the
 core Toga library`_, and a wrapper providing integration with a web framework:
 
 * `Django <https://pypi.python.org/pypi/toga-django>`__
 * `Flask <https://pypi.python.org/pypi/toga-flask>`__
 
 For more details, see the `Toga project on Github`_.
 
+.. _Toga widget toolkit: http://beeware.org/toga
+.. _the core Toga library: https://pypi.python.org/pypi/toga-core
+.. _Toga project on Github: https://github.com/beeware/toga
+
 Community
 ---------
 
 Toga is part of the `BeeWare suite`_. You can talk to the community through:
 
-* `@pybeeware on Twitter <https://twitter.com/pybeeware>`__
+* `@beeware@fosstodon.org on Mastodon`_
+* `Discord`_
+* The Toga `Github Discussions forum`_
 
-* `Discord <https://beeware.org/bee/chat/>`__
+We foster a welcoming and respectful community as described in our
+`BeeWare Community Code of Conduct`_.
 
-* The Toga `Github Discussions forum <https://github.com/beeware/toga/discussions>`__
+.. _BeeWare suite: http://beeware.org
+.. _@beeware@fosstodon.org on Mastodon: https://fosstodon.org/@beeware
+.. _Discord: https://beeware.org/bee/chat/
+.. _Github Discussions forum: https://github.com/beeware/toga/discussions
+.. _BeeWare Community Code of Conduct: http://beeware.org/community/behavior/
 
 Contributing
 ------------
 
 If you experience problems with this backend, `log them on GitHub`_. If you
 want to contribute code, please `fork the code`_ and `submit a pull request`_.
 
-.. _Toga widget toolkit: http://beeware.org/toga
-.. _the core Toga library: https://pypi.python.org/pypi/toga-core
-.. _Toga project on Github: https://github.com/beeware/toga
-.. _BeeWare suite: http://beeware.org
 .. _log them on Github: https://github.com/beeware/toga/issues
 .. _fork the code: https://github.com/beeware/toga
 .. _submit a pull request: https://github.com/beeware/toga/pulls
```

### Comparing `toga-web-0.3.0.dev39/README.rst` & `toga-web-0.3.1/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -7,31 +7,38 @@
 core Toga library`_, and a wrapper providing integration with a web framework:
 
 * `Django <https://pypi.python.org/pypi/toga-django>`__
 * `Flask <https://pypi.python.org/pypi/toga-flask>`__
 
 For more details, see the `Toga project on Github`_.
 
+.. _Toga widget toolkit: http://beeware.org/toga
+.. _the core Toga library: https://pypi.python.org/pypi/toga-core
+.. _Toga project on Github: https://github.com/beeware/toga
+
 Community
 ---------
 
 Toga is part of the `BeeWare suite`_. You can talk to the community through:
 
-* `@pybeeware on Twitter <https://twitter.com/pybeeware>`__
+* `@beeware@fosstodon.org on Mastodon`_
+* `Discord`_
+* The Toga `Github Discussions forum`_
 
-* `Discord <https://beeware.org/bee/chat/>`__
+We foster a welcoming and respectful community as described in our
+`BeeWare Community Code of Conduct`_.
 
-* The Toga `Github Discussions forum <https://github.com/beeware/toga/discussions>`__
+.. _BeeWare suite: http://beeware.org
+.. _@beeware@fosstodon.org on Mastodon: https://fosstodon.org/@beeware
+.. _Discord: https://beeware.org/bee/chat/
+.. _Github Discussions forum: https://github.com/beeware/toga/discussions
+.. _BeeWare Community Code of Conduct: http://beeware.org/community/behavior/
 
 Contributing
 ------------
 
 If you experience problems with this backend, `log them on GitHub`_. If you
 want to contribute code, please `fork the code`_ and `submit a pull request`_.
 
-.. _Toga widget toolkit: http://beeware.org/toga
-.. _the core Toga library: https://pypi.python.org/pypi/toga-core
-.. _Toga project on Github: https://github.com/beeware/toga
-.. _BeeWare suite: http://beeware.org
 .. _log them on Github: https://github.com/beeware/toga/issues
 .. _fork the code: https://github.com/beeware/toga
 .. _submit a pull request: https://github.com/beeware/toga/pulls
```

### Comparing `toga-web-0.3.0.dev39/src/toga_web/factory.py` & `toga-web-0.3.1/src/toga_web/factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,74 +1,75 @@
+from . import dialogs
 from .app import App, MainWindow  # DocumentApp
 from .command import Command
 
 # from .documents import Document
 # from .fonts import Font
 from .icons import Icon
+
 # from .images import Image
 from .paths import paths
-from . import dialogs
-
 from .widgets.box import Box
 from .widgets.button import Button
+
 # from .widgets.canvas import Canvas
 # from .widgets.detailedlist import DetailedList
 # from .widgets.imageview import ImageView
 from .widgets.label import Label
+
 # from .widgets.multilinetextinput import MultilineTextInput
 # from .widgets.numberinput import NumberInput
 # from .widgets.optioncontainer import OptionContainer
 # from .widgets.passwordinput import PasswordInput
 # from .widgets.progressbar import ProgressBar
 # from .widgets.scrollcontainer import ScrollContainer
 # from .widgets.selection import Selection
 # from .widgets.slider import Slider
 # from .widgets.splitcontainer import SplitContainer
 # from .widgets.switch import Switch
 # from .widgets.table import Table
 from .widgets.textinput import TextInput
+
 # from .widgets.tree import Tree
 # from .widgets.webview import WebView
 # from .window import Window
 
 
 def not_implemented(feature):
-    print('[Web] Not implemented: {}'.format(feature))
+    print(f"[Web] Not implemented: {feature}")  # pragma: nocover
 
 
 __all__ = [
-    'not_implemented',
-
-    'App', 'MainWindow',  # 'DocumentApp',
-    'Command',
+    "not_implemented",
+    "App",
+    "MainWindow",  # 'DocumentApp',
+    "Command",
     # 'Document',
-
     # # Resources
     # 'Font',
-    'Icon',
+    "Icon",
     # 'Image',
-    'paths',
-    'dialogs',
-
+    "paths",
+    "dialogs",
     # # Widgets
-    'Box',
-    'Button',
+    "Box",
+    "Button",
     # 'Canvas',
     # 'DetailedList',
     # 'ImageView',
-    'Label',
+    "Label",
     # 'MultilineTextInput',
     # 'NumberInput',
     # 'OptionContainer',
     # 'PasswordInput',
     # 'ProgressBar',
     # 'ScrollContainer',
     # 'Selection',
     # 'Slider',
     # 'SplitContainer',
     # 'Switch',
     # 'Table',
-    'TextInput',
+    "TextInput",
     # 'Tree',
     # 'WebView',
     # 'Window',
 ]
```

### Comparing `toga-web-0.3.0.dev39/src/toga_web/libs.py` & `toga-web-0.3.1/src/toga_web/libs.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,44 +3,57 @@
     import js
 except ModuleNotFoundError:
     # To ensure the code can be imported, provide a js symbol
     # as a fallback
     js = None
 
 
-def create_element(tag, id=None, classes=None, style=None, content=None, children=None, **properties):
+def create_element(
+    tag,
+    id=None,
+    classes=None,
+    style=None,
+    disabled=False,
+    content=None,
+    children=None,
+    **properties,
+):
     """Utility method for creating DOM elements.
 
     :param tag: The HTML tag of the element to create
     :param id: (Optional) The ID of the new element
-    :param classes: (Optional) A list of classes to attach to the
-        new element.
+    :param classes: (Optional) A list of classes to attach to the new element.
     :param style: (Optional) The CSS style for the element.
+    :param disabled: (Optional) Should the element be disabled at time of
+        creation? (Default: False)
     :param content: (Optional) The innerHTML content of the element.
-    :param children: (Optional) A list of direct descendents to add to
-        the element.
-    :param properties: Any additional properties that should be set.
-        These *must* be HTML DOM properties (e.g., ``readOnly``);
-        they cannot be events or methods.
+    :param children: (Optional) A list of direct descendents to add to the
+        element.
+    :param properties: Any additional properties that should be set. These
+        *must* be HTML DOM properties (e.g., ``readOnly``); they cannot be
+        events or methods.
     :returns: A newly created DOM element.
     """
     element = js.document.createElement(tag)
 
     if id:
         element.id = id
 
     if classes:
         for klass in classes:
             element.classList.add(klass)
 
     if style:
         element.style = style
 
+    if disabled:
+        element.setAttribute("disabled", "")
+
     for attr, value in properties.items():
-        element.setAttribute(attr.replace('_', '-'), value)
+        element.setAttribute(attr.replace("_", "-"), value)
 
     if content:
         element.innerHTML = content
 
     if children:
         for child in children:
             element.appendChild(child)
```

### Comparing `toga-web-0.3.0.dev39/src/toga_web/widgets/base.py` & `toga-web-0.3.1/src/toga_web/widgets/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,17 @@
     def __init__(self, interface):
         self.interface = interface
         self.interface._impl = self
         self._container = None
 
         self.create()
 
-    def _create_native_widget(self, tag, classes=None, content=None, children=None, **properties):
+    def _create_native_widget(
+        self, tag, classes=None, content=None, children=None, **properties
+    ):
         """Create a DOM element representing a native widget.
 
         The ID and style of the widget will be automatically set;
         ``toga``, and the name of the widget class (in lower case)
         will be added as a class name on the widget.
 
         :param widget: The web implementation being created.
@@ -41,37 +43,53 @@
             content=content,
             children=children,
             **properties,
         )
 
         return native
 
+    def create(self):
+        raise NotImplementedError()
+
     def set_app(self, app):
         pass
 
     def set_window(self, window):
         pass
 
     @property
+    def viewport(self):
+        return self._container
+
+    @property
     def container(self):
         return self._container
 
     @container.setter
     def container(self, container):
         self._container = container
 
         for child in self.interface.children:
             child._impl.container = container
 
+    def get_enabled(self):
+        return not self.native.disabled
+
     def set_enabled(self, value):
-        self.native.set_sensitive(self.interface.enabled)
+        self.native.disabled = not value
 
     def focus(self):
         self.interface.factory.not_implemented("Widget.focus()")
 
+    def get_tab_index(self):
+        self.interface.factory.not_implementated("Widget.get_tab_index()")
+
+    def set_tab_index(self, tab_index):
+        self.interface.factory.not_implementated("Widget.set_tab_index()")
+
     ######################################################################
     # APPLICATOR
     #
     # Web style is a little different to other platforms; we if there's
     # any change, we can just re-set the CSS styles and the browser
     # will reflect those changes as needed.
     ######################################################################
@@ -100,9 +118,18 @@
     ######################################################################
     # INTERFACE
     ######################################################################
 
     def add_child(self, child):
         pass
 
+    def insert_child(self, index, child):
+        self.add_child(child)
+
+    def remove_child(self, child):
+        child.container = None
+
+    def refresh(self):
+        self._reapply_style()
+
     def rehint(self):
         pass
```

### Comparing `toga-web-0.3.0.dev39/src/toga_web/widgets/button.py` & `toga-web-0.3.1/src/toga_web/widgets/button.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from .base import Widget
 
 
 class Button(Widget):
     def create(self):
-        self.native = self._create_native_widget("button", classes=["btn-block"],)
+        self.native = self._create_native_widget("sl-button")
         self.native.onclick = self.dom_onclick
 
     def dom_onclick(self, event):
-        if self.interface.on_press:
-            self.interface.on_press(self.interface)
+        self.interface.on_press(None)
+
+    def get_text(self):
+        return self.native.innerHTML
 
     def set_text(self, text):
         self.native.innerHTML = text
 
     def set_enabled(self, value):
         self.native.disabled = not value
 
     def set_background_color(self, value):
         pass
 
-    def set_on_press(self, handler):
-        pass
-
     def rehint(self):
         pass
```

### Comparing `toga-web-0.3.0.dev39/src/toga_web/widgets/textinput.py` & `toga-web-0.3.1/src/toga_web/widgets/textinput.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .base import Widget
 
 
 class TextInput(Widget):
     def create(self):
-        self.native = self._create_native_widget("input", classes=["btn-block"])
+        self.native = self._create_native_widget("sl-input")
 
     def set_readonly(self, value):
         self.native.readOnly = value
 
     def set_placeholder(self, value):
         if value:
             self.native.placeholder = value
@@ -37,7 +37,11 @@
         pass
 
     def set_error(self, error_message):
         pass
 
     def clear_error(self):
         pass
+
+    def is_valid(self):
+        self.interface.factory.not_implemented("TextInput.is_valid()")
+        return True
```

### Comparing `toga-web-0.3.0.dev39/src/toga_web/window.py` & `toga-web-0.3.1/src/toga_web/window.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,8 @@
-from toga_web.libs import js, create_element
-
-
-class WebViewport:
-    def __init__(self):
-        self.dpi = 96
-        self.baseline_dpi = 96
-
-    @property
-    def width(self):
-        return 1024
-
-    @property
-    def height(self):
-        return 768
+from toga_web.libs import create_element, js
 
 
 class Window:
     def __init__(self, interface, title, position, size):
         self.interface = interface
         self.interface._impl = self
 
@@ -38,24 +24,22 @@
     def set_title(self, title):
         js.document.title = title
 
     def set_app(self, app):
         pass
 
     def create_toolbar(self):
-        self.interface.factory.not_implemented('Window.create_toolbar()')
+        self.interface.factory.not_implemented("Window.create_toolbar()")
 
     def clear_content(self):
         if self.interface.content:
             for child in self.interface.content.children:
                 child._impl.container = None
 
     def set_content(self, widget):
-        widget.viewport = WebViewport()
-
         # Remove existing content of the window.
         for child in self.native.childNodes:
             self.native.removeChild(child)
 
         # Add all children to the content widget.
         self.native.appendChild(widget.native)
 
@@ -71,25 +55,25 @@
     def on_close(self, *args):
         pass
 
     def on_size_allocate(self, widget, allocation):
         pass
 
     def close(self):
-        self.interface.factory.not_implemented('Window.close()')
+        self.interface.factory.not_implemented("Window.close()")
 
     def get_position(self):
-        return (0, 0)
+        return 0, 0
 
     def set_position(self, position):
         # Does nothing on web
         pass
 
     def get_size(self):
-        return (self.content.viewport.width, self.content.viewport.height)
+        return self.native.offsetWidth, self.native.offsetHeight
 
     def set_size(self, size):
         # Does nothing on web
         pass
 
     def set_full_screen(self, is_full_screen):
-        self.interface.factory.not_implemented('Window.set_full_screen()')
+        self.interface.factory.not_implemented("Window.set_full_screen()")
```

### Comparing `toga-web-0.3.0.dev39/src/toga_web.egg-info/PKG-INFO` & `toga-web-0.3.1/src/toga_web.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toga-web
-Version: 0.3.0.dev39
+Version: 0.3.1
 Summary: A common backend for the Toga widget toolkit on web platforms.
 Home-page: https://beeware.org/project/projects/libraries/toga/
 Author: Russell Keith-Magee
 Author-email: russell@keith-magee.com
 Maintainer: BeeWare Team
 Maintainer-email: team@beeware.org
 License: New BSD
@@ -18,52 +18,60 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Software Development :: Widget Sets
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst; charset=UTF-8
-License-File: LICENSE
 
 toga-web
 ========
 
 A common backend for the `Toga widget toolkit`_ on web platforms.
 
 This package isn't much use by itself; it needs to be combined with `the
 core Toga library`_, and a wrapper providing integration with a web framework:
 
 * `Django <https://pypi.python.org/pypi/toga-django>`__
 * `Flask <https://pypi.python.org/pypi/toga-flask>`__
 
 For more details, see the `Toga project on Github`_.
 
+.. _Toga widget toolkit: http://beeware.org/toga
+.. _the core Toga library: https://pypi.python.org/pypi/toga-core
+.. _Toga project on Github: https://github.com/beeware/toga
+
 Community
 ---------
 
 Toga is part of the `BeeWare suite`_. You can talk to the community through:
 
-* `@pybeeware on Twitter <https://twitter.com/pybeeware>`__
+* `@beeware@fosstodon.org on Mastodon`_
+* `Discord`_
+* The Toga `Github Discussions forum`_
 
-* `Discord <https://beeware.org/bee/chat/>`__
+We foster a welcoming and respectful community as described in our
+`BeeWare Community Code of Conduct`_.
 
-* The Toga `Github Discussions forum <https://github.com/beeware/toga/discussions>`__
+.. _BeeWare suite: http://beeware.org
+.. _@beeware@fosstodon.org on Mastodon: https://fosstodon.org/@beeware
+.. _Discord: https://beeware.org/bee/chat/
+.. _Github Discussions forum: https://github.com/beeware/toga/discussions
+.. _BeeWare Community Code of Conduct: http://beeware.org/community/behavior/
 
 Contributing
 ------------
 
 If you experience problems with this backend, `log them on GitHub`_. If you
 want to contribute code, please `fork the code`_ and `submit a pull request`_.
 
-.. _Toga widget toolkit: http://beeware.org/toga
-.. _the core Toga library: https://pypi.python.org/pypi/toga-core
-.. _Toga project on Github: https://github.com/beeware/toga
-.. _BeeWare suite: http://beeware.org
 .. _log them on Github: https://github.com/beeware/toga/issues
 .. _fork the code: https://github.com/beeware/toga
 .. _submit a pull request: https://github.com/beeware/toga/pulls
```

