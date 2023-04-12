# Comparing `tmp/toga-demo-0.3.0.dev9.tar.gz` & `tmp/toga-demo-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/toga-demo-0.3.0.dev9.tar", last modified: Sat Jul  7 05:55:22 2018, max compression
+gzip compressed data, was "toga-demo-0.3.1.tar", last modified: Wed Apr 12 01:58:44 2023, max compression
```

## Comparing `toga-demo-0.3.0.dev9.tar` & `toga-demo-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,28 @@
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:22.000000 toga-demo-0.3.0.dev9/
--rw-r--r--   0 rkm        (501) staff       (20)     2580 2018-07-07 05:55:22.000000 toga-demo-0.3.0.dev9/PKG-INFO
--rwxr-xr-x   0 rkm        (501) staff       (20)     1524 2017-12-22 11:14:05.000000 toga-demo-0.3.0.dev9/LICENSE
--rwxr-xr-x   0 rkm        (501) staff       (20)      344 2017-12-22 11:14:05.000000 toga-demo-0.3.0.dev9/AUTHORS
--rwxr-xr-x   0 rkm        (501) staff       (20)       84 2017-12-22 11:14:05.000000 toga-demo-0.3.0.dev9/MANIFEST.in
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:22.000000 toga-demo-0.3.0.dev9/toga_demo/
--rw-r--r--   0 rkm        (501) staff       (20)      351 2018-05-17 17:50:36.000000 toga-demo-0.3.0.dev9/toga_demo/__init__.py
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:22.000000 toga-demo-0.3.0.dev9/toga_demo/icons/
--rwxr-xr-x   0 rkm        (501) staff       (20)     2011 2017-12-22 11:14:05.000000 toga-demo-0.3.0.dev9/toga_demo/icons/brutus-32.png
--rwxr-xr-x   0 rkm        (501) staff       (20)     2659 2018-05-26 09:29:02.000000 toga-demo-0.3.0.dev9/toga_demo/app.py
--rwxr-xr-x   0 rkm        (501) staff       (20)      125 2017-12-22 11:14:05.000000 toga-demo-0.3.0.dev9/toga_demo/__main__.py
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:22.000000 toga-demo-0.3.0.dev9/toga_demo.egg-info/
--rw-r--r--   0 rkm        (501) staff       (20)     2580 2018-07-07 05:55:22.000000 toga-demo-0.3.0.dev9/toga_demo.egg-info/PKG-INFO
--rw-r--r--   0 rkm        (501) staff       (20)      338 2018-07-07 05:55:22.000000 toga-demo-0.3.0.dev9/toga_demo.egg-info/SOURCES.txt
--rw-r--r--   0 rkm        (501) staff       (20)       54 2018-07-07 05:55:22.000000 toga-demo-0.3.0.dev9/toga_demo.egg-info/entry_points.txt
--rw-r--r--   0 rkm        (501) staff       (20)       17 2018-07-07 05:55:22.000000 toga-demo-0.3.0.dev9/toga_demo.egg-info/requires.txt
--rw-r--r--   0 rkm        (501) staff       (20)       10 2018-07-07 05:55:22.000000 toga-demo-0.3.0.dev9/toga_demo.egg-info/top_level.txt
--rw-r--r--   0 rkm        (501) staff       (20)        1 2018-07-07 05:55:22.000000 toga-demo-0.3.0.dev9/toga_demo.egg-info/dependency_links.txt
--rwxr-xr-x   0 rkm        (501) staff       (20)     2504 2018-07-07 05:52:00.000000 toga-demo-0.3.0.dev9/setup.py
--rw-r--r--   0 rkm        (501) staff       (20)       38 2018-07-07 05:55:22.000000 toga-demo-0.3.0.dev9/setup.cfg
--rwxr-xr-x   0 rkm        (501) staff       (20)     1369 2017-12-22 11:14:05.000000 toga-demo-0.3.0.dev9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:44.011730 toga-demo-0.3.1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      344 2023-04-12 01:57:58.000000 toga-demo-0.3.1/AUTHORS
+-rwxr-xr-x   0 runner    (1001) docker     (123)      181 2023-04-12 01:57:58.000000 toga-demo-0.3.1/CONTRIBUTING.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1525 2023-04-12 01:57:58.000000 toga-demo-0.3.1/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-04-12 01:57:58.000000 toga-demo-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-12 01:58:44.011730 toga-demo-0.3.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1883 2023-04-12 01:57:58.000000 toga-demo-0.3.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-12 01:57:58.000000 toga-demo-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-12 01:58:44.011730 toga-demo-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-12 01:57:58.000000 toga-demo-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:44.003730 toga-demo-0.3.1/toga_demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:57:58.000000 toga-demo-0.3.1/toga_demo/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      128 2023-04-12 01:57:58.000000 toga-demo-0.3.1/toga_demo/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2725 2023-04-12 01:57:58.000000 toga-demo-0.3.1/toga_demo/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:44.011730 toga-demo-0.3.1/toga_demo/resources/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2011 2023-04-12 01:57:58.000000 toga-demo-0.3.1/toga_demo/resources/brutus-32.png
+-rw-r--r--   0 runner    (1001) docker     (123)   316755 2023-04-12 01:57:58.000000 toga-demo-0.3.1/toga_demo/resources/brutus.icns
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-12 01:57:58.000000 toga-demo-0.3.1/toga_demo/resources/brutus.ico
+-rw-r--r--   0 runner    (1001) docker     (123)   316755 2023-04-12 01:57:58.000000 toga-demo-0.3.1/toga_demo/resources/toga-demo.icns
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-12 01:57:58.000000 toga-demo-0.3.1/toga_demo/resources/toga-demo.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:44.007730 toga-demo-0.3.1/toga_demo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-12 01:58:43.000000 toga-demo-0.3.1/toga_demo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-12 01:58:43.000000 toga-demo-0.3.1/toga_demo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 01:58:43.000000 toga-demo-0.3.1/toga_demo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-12 01:58:43.000000 toga-demo-0.3.1/toga_demo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 01:58:28.000000 toga-demo-0.3.1/toga_demo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 01:58:43.000000 toga-demo-0.3.1/toga_demo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-12 01:58:43.000000 toga-demo-0.3.1/toga_demo.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `toga-demo-0.3.0.dev9/PKG-INFO` & `toga-demo-0.3.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,71 +1,100 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: toga-demo
-Version: 0.3.0.dev9
+Version: 0.3.1
 Summary: A demonstration of the capabilities of the Toga widget toolkit.
-Home-page: http://pybee.org/toga-demo
+Home-page: https://beeware.org/project/projects/libraries/toga/
 Author: Russell Keith-Magee
 Author-email: russell@keith-magee.com
+Maintainer: BeeWare Team
+Maintainer-email: team@beeware.org
 License: New BSD
-Description: Toga Demo
-        =========
-        
-        A demonstration of the capabilities of the `Toga widget toolkit`_.
-        
-        **Toga requires Python 3**
-        
-        Quickstart
-        ----------
-        
-        For details of Toga's pre-requisites, see the `toga repository on GitHub`_.
-        
-        Once those pre-requisites have been met, in your virtualenv, install Toga Demo,
-        and then run it::
-        
-            $ pip install toga-demo
-            $ toga-demo
-        
-        This will pop up a GUI window.
-        
-        If you have cloned the toga-demo repository, you can run the demo like this::
-        
-            $ pip install toga
-            $ python -m toga_demo
-        
-        Community
-        ---------
-        
-        Toga Demo is part of the `BeeWare suite`_. You can talk to the community through:
-        
-        * `@pybeeware on Twitter`_
-        
-        * The `pybee/general`_ channel on Gitter.
-        
-        Contributing
-        ------------
-        
-        If you experience problems with Toga Demo, `log them on GitHub`_. If you
-        want to contribute code, please `fork the code`_ and `submit a pull request`_.
-        
-        .. _BeeWare suite: http://pybee.org
-        .. _Read The Docs: http://toga-demo.readthedocs.org
-        .. _Toga widget toolkit: http://pybee.org/toga
-        .. _toga repository on GitHub: https://github.com/pybee/toga
-        .. _@pybeeware on Twitter: https://twitter.com/pybeeware
-        .. _pybee/general: https://gitter.im/pybee/general
-        .. _log them on Github: https://github.com/pybee/toga-demo/issues
-        .. _fork the code: https://github.com/pybee/toga-demo
-        .. _submit a pull request: https://github.com/pybee/toga-demo/pulls
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Project-URL: Funding, https://beeware.org/contributing/membership/
+Project-URL: Documentation, http://toga.readthedocs.io/en/latest/
+Project-URL: Tracker, https://github.com/beeware/toga/issues
+Project-URL: Source, https://github.com/beeware/toga
+Keywords: gui,widget,cross-platform,desktop,mobile,macOS,cocoa,iOS,android,windows,winforms,linux,gtk
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
-Classifier: Topic :: Utilities
-Requires-Python: >=3.5
+Classifier: Topic :: Software Development :: User Interfaces
+Classifier: Topic :: Software Development :: Widget Sets
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst; charset=UTF-8
+
+Toga Demo
+=========
+
+A demonstration of the capabilities of the `Toga widget toolkit`_.
+
+**Toga requires Python 3**
+
+.. _Toga widget toolkit: http://beeware.org/toga
+
+Quickstart
+----------
+
+For details of Toga's pre-requisites, see the `Toga project on GitHub`_.
+
+Once those pre-requisites have been met, in your virtualenv, install Toga Demo,
+and then run it::
+
+    $ pip install toga-demo
+    $ toga-demo
+
+This will pop up a GUI window.
+
+If you have cloned the toga repository, install the dependent packages in your virtualenv::
+
+    $ cd toga
+    $ pip install -e ./core
+
+Then install the platform specific code::
+
+    $ pip install -e ./cocoa      # macOS
+    $ pip install -e ./gtk        # Linux
+    $ pip install -e ./winforms   # Windows
+
+Finally navigate to the demo directory and run the application::
+
+    $ cd demo
+    $ python -m toga_demo
+
+.. _Toga project on Github: https://github.com/beeware/toga
+
+Community
+---------
+
+Toga Demo is part of the `BeeWare suite`_. You can talk to the community through:
+
+* `@beeware@fosstodon.org on Mastodon`_
+* `Discord`_
+* The Toga `Github Discussions forum`_
+
+We foster a welcoming and respectful community as described in our
+`BeeWare Community Code of Conduct`_.
+
+.. _BeeWare suite: http://beeware.org
+.. _@beeware@fosstodon.org on Mastodon: https://fosstodon.org/@beeware
+.. _Discord: https://beeware.org/bee/chat/
+.. _Github Discussions forum: https://github.com/beeware/toga/discussions
+.. _BeeWare Community Code of Conduct: http://beeware.org/community/behavior/
+
+Contributing
+------------
+
+If you experience problems with Toga Demo, `log them on GitHub`_. If you
+want to contribute code, please `fork the code`_ and `submit a pull request`_.
+
+.. _log them on Github: https://github.com/beeware/toga/issues
+.. _fork the code: https://github.com/beeware/toga
+.. _submit a pull request: https://github.com/beeware/toga/pulls
```

### Comparing `toga-demo-0.3.0.dev9/LICENSE` & `toga-demo-0.3.1/LICENSE`

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

### Comparing `toga-demo-0.3.0.dev9/toga_demo/icons/brutus-32.png` & `toga-demo-0.3.1/toga_demo/resources/brutus-32.png`

 * *Files identical despite different names*

### Comparing `toga-demo-0.3.0.dev9/toga_demo.egg-info/PKG-INFO` & `toga-demo-0.3.1/toga_demo.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,71 +1,100 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: toga-demo
-Version: 0.3.0.dev9
+Version: 0.3.1
 Summary: A demonstration of the capabilities of the Toga widget toolkit.
-Home-page: http://pybee.org/toga-demo
+Home-page: https://beeware.org/project/projects/libraries/toga/
 Author: Russell Keith-Magee
 Author-email: russell@keith-magee.com
+Maintainer: BeeWare Team
+Maintainer-email: team@beeware.org
 License: New BSD
-Description: Toga Demo
-        =========
-        
-        A demonstration of the capabilities of the `Toga widget toolkit`_.
-        
-        **Toga requires Python 3**
-        
-        Quickstart
-        ----------
-        
-        For details of Toga's pre-requisites, see the `toga repository on GitHub`_.
-        
-        Once those pre-requisites have been met, in your virtualenv, install Toga Demo,
-        and then run it::
-        
-            $ pip install toga-demo
-            $ toga-demo
-        
-        This will pop up a GUI window.
-        
-        If you have cloned the toga-demo repository, you can run the demo like this::
-        
-            $ pip install toga
-            $ python -m toga_demo
-        
-        Community
-        ---------
-        
-        Toga Demo is part of the `BeeWare suite`_. You can talk to the community through:
-        
-        * `@pybeeware on Twitter`_
-        
-        * The `pybee/general`_ channel on Gitter.
-        
-        Contributing
-        ------------
-        
-        If you experience problems with Toga Demo, `log them on GitHub`_. If you
-        want to contribute code, please `fork the code`_ and `submit a pull request`_.
-        
-        .. _BeeWare suite: http://pybee.org
-        .. _Read The Docs: http://toga-demo.readthedocs.org
-        .. _Toga widget toolkit: http://pybee.org/toga
-        .. _toga repository on GitHub: https://github.com/pybee/toga
-        .. _@pybeeware on Twitter: https://twitter.com/pybeeware
-        .. _pybee/general: https://gitter.im/pybee/general
-        .. _log them on Github: https://github.com/pybee/toga-demo/issues
-        .. _fork the code: https://github.com/pybee/toga-demo
-        .. _submit a pull request: https://github.com/pybee/toga-demo/pulls
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Project-URL: Funding, https://beeware.org/contributing/membership/
+Project-URL: Documentation, http://toga.readthedocs.io/en/latest/
+Project-URL: Tracker, https://github.com/beeware/toga/issues
+Project-URL: Source, https://github.com/beeware/toga
+Keywords: gui,widget,cross-platform,desktop,mobile,macOS,cocoa,iOS,android,windows,winforms,linux,gtk
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
-Classifier: Topic :: Utilities
-Requires-Python: >=3.5
+Classifier: Topic :: Software Development :: User Interfaces
+Classifier: Topic :: Software Development :: Widget Sets
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst; charset=UTF-8
+
+Toga Demo
+=========
+
+A demonstration of the capabilities of the `Toga widget toolkit`_.
+
+**Toga requires Python 3**
+
+.. _Toga widget toolkit: http://beeware.org/toga
+
+Quickstart
+----------
+
+For details of Toga's pre-requisites, see the `Toga project on GitHub`_.
+
+Once those pre-requisites have been met, in your virtualenv, install Toga Demo,
+and then run it::
+
+    $ pip install toga-demo
+    $ toga-demo
+
+This will pop up a GUI window.
+
+If you have cloned the toga repository, install the dependent packages in your virtualenv::
+
+    $ cd toga
+    $ pip install -e ./core
+
+Then install the platform specific code::
+
+    $ pip install -e ./cocoa      # macOS
+    $ pip install -e ./gtk        # Linux
+    $ pip install -e ./winforms   # Windows
+
+Finally navigate to the demo directory and run the application::
+
+    $ cd demo
+    $ python -m toga_demo
+
+.. _Toga project on Github: https://github.com/beeware/toga
+
+Community
+---------
+
+Toga Demo is part of the `BeeWare suite`_. You can talk to the community through:
+
+* `@beeware@fosstodon.org on Mastodon`_
+* `Discord`_
+* The Toga `Github Discussions forum`_
+
+We foster a welcoming and respectful community as described in our
+`BeeWare Community Code of Conduct`_.
+
+.. _BeeWare suite: http://beeware.org
+.. _@beeware@fosstodon.org on Mastodon: https://fosstodon.org/@beeware
+.. _Discord: https://beeware.org/bee/chat/
+.. _Github Discussions forum: https://github.com/beeware/toga/discussions
+.. _BeeWare Community Code of Conduct: http://beeware.org/community/behavior/
+
+Contributing
+------------
+
+If you experience problems with Toga Demo, `log them on GitHub`_. If you
+want to contribute code, please `fork the code`_ and `submit a pull request`_.
+
+.. _log them on Github: https://github.com/beeware/toga/issues
+.. _fork the code: https://github.com/beeware/toga
+.. _submit a pull request: https://github.com/beeware/toga/pulls
```

