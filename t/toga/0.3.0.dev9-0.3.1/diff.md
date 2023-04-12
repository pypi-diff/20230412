# Comparing `tmp/toga-0.3.0.dev9.tar.gz` & `tmp/toga-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/toga-0.3.0.dev9.tar", last modified: Sat Jul  7 05:55:17 2018, max compression
+gzip compressed data, was "toga-0.3.1.tar", last modified: Wed Apr 12 01:58:45 2023, max compression
```

## Comparing `toga-0.3.0.dev9.tar` & `toga-0.3.1.tar`

### file list

```diff
@@ -1,87 +1,16 @@
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:17.000000 toga-0.3.0.dev9/
--rw-r--r--   0 rkm        (501) staff       (20)     5405 2018-07-07 05:55:17.000000 toga-0.3.0.dev9/PKG-INFO
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:17.000000 toga-0.3.0.dev9/toga.egg-info/
--rw-r--r--   0 rkm        (501) staff       (20)     5405 2018-07-07 05:55:17.000000 toga-0.3.0.dev9/toga.egg-info/PKG-INFO
--rw-r--r--   0 rkm        (501) staff       (20)     2268 2018-07-07 05:55:17.000000 toga-0.3.0.dev9/toga.egg-info/SOURCES.txt
--rw-r--r--   0 rkm        (501) staff       (20)      149 2018-07-07 05:55:17.000000 toga-0.3.0.dev9/toga.egg-info/requires.txt
--rw-r--r--   0 rkm        (501) staff       (20)        1 2018-07-07 05:55:17.000000 toga-0.3.0.dev9/toga.egg-info/top_level.txt
--rw-r--r--   0 rkm        (501) staff       (20)        1 2018-07-07 05:55:17.000000 toga-0.3.0.dev9/toga.egg-info/dependency_links.txt
--rw-r--r--   0 rkm        (501) staff       (20)     1519 2016-10-23 02:22:46.000000 toga-0.3.0.dev9/LICENSE
--rw-r--r--   0 rkm        (501) staff       (20)      225 2016-10-23 02:22:46.000000 toga-0.3.0.dev9/MANIFEST.in
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:17.000000 toga-0.3.0.dev9/docs/
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:17.000000 toga-0.3.0.dev9/docs/background/
--rw-r--r--   0 rkm        (501) staff       (20)      196 2018-07-07 05:52:00.000000 toga-0.3.0.dev9/docs/background/index.rst
--rw-r--r--   0 rkm        (501) staff       (20)     6222 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/background/roadmap.rst
--rw-r--r--   0 rkm        (501) staff       (20)     3647 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/background/philosophy.rst
--rw-r--r--   0 rkm        (501) staff       (20)     4743 2017-12-23 03:47:56.000000 toga-0.3.0.dev9/docs/background/data-sources.rst
--rw-r--r--   0 rkm        (501) staff       (20)      240 2018-07-07 05:52:00.000000 toga-0.3.0.dev9/docs/background/success.rst
--rw-r--r--   0 rkm        (501) staff       (20)     2240 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/background/layout.rst
--rw-r--r--   0 rkm        (501) staff       (20)     4033 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/background/commands.rst
--rw-r--r--   0 rkm        (501) staff       (20)     1217 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/background/releases.rst
--rw-r--r--   0 rkm        (501) staff       (20)     3392 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/background/architecture.rst
--rw-r--r--   0 rkm        (501) staff       (20)     1791 2018-05-17 17:50:27.000000 toga-0.3.0.dev9/docs/background/faq.rst
--rw-r--r--   0 rkm        (501) staff       (20)     2120 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/index.rst
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:17.000000 toga-0.3.0.dev9/docs/tutorial/
--rw-r--r--   0 rkm        (501) staff       (20)     1552 2017-12-23 03:47:56.000000 toga-0.3.0.dev9/docs/tutorial/index.rst
--rw-r--r--   0 rkm        (501) staff       (20)     1868 2018-07-07 05:52:00.000000 toga-0.3.0.dev9/docs/tutorial/tutorial-4.rst
--rw-r--r--   0 rkm        (501) staff       (20)     1668 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/tutorial/tutorial-2.rst
--rw-r--r--   0 rkm        (501) staff       (20)      258 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/tutorial/tutorial-issues-note.rst
--rw-r--r--   0 rkm        (501) staff       (20)      895 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/tutorial/tutorial-3.rst
--rw-r--r--   0 rkm        (501) staff       (20)     1053 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/tutorial/tutorial-1.rst
--rw-r--r--   0 rkm        (501) staff       (20)     8171 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/tutorial/tutorial-0.rst
--rw-r--r--   0 rkm        (501) staff       (20)     6714 2017-12-22 11:14:05.000000 toga-0.3.0.dev9/docs/Makefile
--rw-r--r--   0 rkm        (501) staff       (20)     9678 2018-01-25 12:57:56.000000 toga-0.3.0.dev9/docs/conf.py
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:17.000000 toga-0.3.0.dev9/docs/how-to/
--rw-r--r--   0 rkm        (501) staff       (20)      160 2017-12-22 11:14:05.000000 toga-0.3.0.dev9/docs/how-to/index.rst
--rw-r--r--   0 rkm        (501) staff       (20)    19281 2018-06-10 23:51:35.000000 toga-0.3.0.dev9/docs/how-to/contribute.rst
--rw-r--r--   0 rkm        (501) staff       (20)      674 2017-12-22 11:14:05.000000 toga-0.3.0.dev9/docs/how-to/get-started.rst
--rw-r--r--   0 rkm        (501) staff       (20)     5101 2016-10-23 02:22:51.000000 toga-0.3.0.dev9/docs/make.bat
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:17.000000 toga-0.3.0.dev9/docs/mock_gtk/
--rw-r--r--   0 rkm        (501) staff       (20)      898 2018-06-10 23:51:35.000000 toga-0.3.0.dev9/docs/mock_gtk/setup.py
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:17.000000 toga-0.3.0.dev9/docs/reference/
--rw-r--r--   0 rkm        (501) staff       (20)      118 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/reference/index.rst
--rw-r--r--   0 rkm        (501) staff       (20)     4292 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/reference/platforms.rst
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:17.000000 toga-0.3.0.dev9/docs/reference/style/
--rw-r--r--   0 rkm        (501) staff       (20)       71 2017-12-23 03:47:56.000000 toga-0.3.0.dev9/docs/reference/style/index.rst
--rw-r--r--   0 rkm        (501) staff       (20)    15274 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/reference/style/pack.rst
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:17.000000 toga-0.3.0.dev9/docs/reference/api/
--rw-r--r--   0 rkm        (501) staff       (20)     1235 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/reference/api/app.rst
--rw-r--r--   0 rkm        (501) staff       (20)     4188 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/reference/api/index.rst
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:17.000000 toga-0.3.0.dev9/docs/reference/api/resources/
--rw-r--r--   0 rkm        (501) staff       (20)      432 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/reference/api/resources/group.rst
--rw-r--r--   0 rkm        (501) staff       (20)       80 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/reference/api/resources/index.rst
--rw-r--r--   0 rkm        (501) staff       (20)      410 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/reference/api/resources/icon.rst
--rw-r--r--   0 rkm        (501) staff       (20)      404 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/reference/api/resources/command.rst
--rw-r--r--   0 rkm        (501) staff       (20)      474 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/reference/api/resources/font.rst
--rw-r--r--   0 rkm        (501) staff       (20)      421 2018-06-10 23:51:35.000000 toga-0.3.0.dev9/docs/reference/api/resources/image.rst
--rw-r--r--   0 rkm        (501) staff       (20)      832 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/reference/api/mainwindow.rst
--rw-r--r--   0 rkm        (501) staff       (20)      823 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/reference/api/window.rst
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:17.000000 toga-0.3.0.dev9/docs/reference/api/containers/
--rw-r--r--   0 rkm        (501) staff       (20)      101 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/reference/api/containers/index.rst
--rw-r--r--   0 rkm        (501) staff       (20)      877 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/reference/api/containers/optioncontainer.rst
--rw-r--r--   0 rkm        (501) staff       (20)     1091 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/reference/api/containers/scrollcontainer.rst
--rw-r--r--   0 rkm        (501) staff       (20)     1324 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/reference/api/containers/box.rst
--rw-r--r--   0 rkm        (501) staff       (20)     1232 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/reference/api/containers/splitcontainer.rst
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:17.000000 toga-0.3.0.dev9/docs/reference/api/widgets/
--rw-r--r--   0 rkm        (501) staff       (20)      450 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/reference/api/widgets/detailedlist.rst
--rw-r--r--   0 rkm        (501) staff       (20)      713 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/reference/api/widgets/selection.rst
--rw-r--r--   0 rkm        (501) staff       (20)      242 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/reference/api/widgets/index.rst
--rw-r--r--   0 rkm        (501) staff       (20)      697 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/reference/api/widgets/multilinetextinput.rst
--rw-r--r--   0 rkm        (501) staff       (20)      427 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/reference/api/widgets/slider.rst
--rw-r--r--   0 rkm        (501) staff       (20)      695 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/reference/api/widgets/textinput.rst
--rw-r--r--   0 rkm        (501) staff       (20)      691 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/reference/api/widgets/webview.rst
--rw-r--r--   0 rkm        (501) staff       (20)      630 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/reference/api/widgets/label.rst
--rw-r--r--   0 rkm        (501) staff       (20)     2402 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/reference/api/widgets/progressbar.rst
--rw-r--r--   0 rkm        (501) staff       (20)      459 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/reference/api/widgets/passwordinput.rst
--rw-r--r--   0 rkm        (501) staff       (20)      608 2018-06-10 23:51:35.000000 toga-0.3.0.dev9/docs/reference/api/widgets/imageview.rst
--rw-r--r--   0 rkm        (501) staff       (20)      830 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/reference/api/widgets/tree.rst
--rw-r--r--   0 rkm        (501) staff       (20)      605 2018-06-10 23:51:35.000000 toga-0.3.0.dev9/docs/reference/api/widgets/switch.rst
--rw-r--r--   0 rkm        (501) staff       (20)      846 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/reference/api/widgets/table.rst
--rw-r--r--   0 rkm        (501) staff       (20)     2241 2018-07-07 05:52:00.000000 toga-0.3.0.dev9/docs/reference/api/widgets/canvas.rst
--rw-r--r--   0 rkm        (501) staff       (20)      935 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/reference/api/widgets/button.rst
--rw-r--r--   0 rkm        (501) staff       (20)      685 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/reference/api/widgets/numberinput.rst
--rw-r--r--   0 rkm        (501) staff       (20)      521 2018-05-26 09:29:22.000000 toga-0.3.0.dev9/docs/reference/api/widgets/widget.rst
--rw-r--r--   0 rkm        (501) staff       (20)     1898 2018-07-07 05:52:00.000000 toga-0.3.0.dev9/setup.py
--rw-r--r--   0 rkm        (501) staff       (20)      325 2017-12-22 11:14:05.000000 toga-0.3.0.dev9/tox.ini
--rw-r--r--   0 rkm        (501) staff       (20)      235 2018-07-07 05:55:17.000000 toga-0.3.0.dev9/setup.cfg
--rw-r--r--   0 rkm        (501) staff       (20)     3675 2018-07-07 05:52:00.000000 toga-0.3.0.dev9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:45.386572 toga-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-12 01:58:04.000000 toga-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-12 01:58:04.000000 toga-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-12 01:58:04.000000 toga-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-12 01:58:45.386572 toga-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-12 01:58:04.000000 toga-0.3.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-12 01:58:04.000000 toga-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-12 01:58:45.386572 toga-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-12 01:58:04.000000 toga-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:45.386572 toga-0.3.1/toga.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-12 01:58:45.000000 toga-0.3.1/toga.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-12 01:58:45.000000 toga-0.3.1/toga.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 01:58:45.000000 toga-0.3.1/toga.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 01:58:30.000000 toga-0.3.1/toga.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 01:58:45.000000 toga-0.3.1/toga.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 01:58:45.000000 toga-0.3.1/toga.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `toga-0.3.0.dev9/LICENSE` & `toga-0.3.1/LICENSE`

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

