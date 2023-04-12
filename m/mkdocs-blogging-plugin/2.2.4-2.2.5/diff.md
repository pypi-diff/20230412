# Comparing `tmp/mkdocs-blogging-plugin-2.2.4.tar.gz` & `tmp/mkdocs-blogging-plugin-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-blogging-plugin-2.2.4.tar", last modified: Tue Apr  4 02:07:13 2023, max compression
+gzip compressed data, was "mkdocs-blogging-plugin-2.2.5.tar", last modified: Wed Apr 12 17:34:47 2023, max compression
```

## Comparing `mkdocs-blogging-plugin-2.2.4.tar` & `mkdocs-blogging-plugin-2.2.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 02:07:13.322438 mkdocs-blogging-plugin-2.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-04 02:06:54.000000 mkdocs-blogging-plugin-2.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-04 02:06:54.000000 mkdocs-blogging-plugin-2.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-04 02:07:13.322438 mkdocs-blogging-plugin-2.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-04 02:06:54.000000 mkdocs-blogging-plugin-2.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 02:07:13.318438 mkdocs-blogging-plugin-2.2.4/mkdocs_blogging_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 02:06:54.000000 mkdocs-blogging-plugin-2.2.4/mkdocs_blogging_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-04 02:06:54.000000 mkdocs-blogging-plugin-2.2.4/mkdocs_blogging_plugin/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13628 2023-04-04 02:06:54.000000 mkdocs-blogging-plugin-2.2.4/mkdocs_blogging_plugin/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 02:07:13.322438 mkdocs-blogging-plugin-2.2.4/mkdocs_blogging_plugin/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-04 02:06:54.000000 mkdocs-blogging-plugin-2.2.4/mkdocs_blogging_plugin/templates/blog-button-theme.html
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-04 02:06:54.000000 mkdocs-blogging-plugin-2.2.4/mkdocs_blogging_plugin/templates/blog-card-theme.html
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-04 02:06:54.000000 mkdocs-blogging-plugin-2.2.4/mkdocs_blogging_plugin/templates/blog-tags-index.html
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-04 02:06:54.000000 mkdocs-blogging-plugin-2.2.4/mkdocs_blogging_plugin/templates/blog-tags-render.html
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-04 02:06:54.000000 mkdocs-blogging-plugin-2.2.4/mkdocs_blogging_plugin/templates/blog-tags.html
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-04 02:06:54.000000 mkdocs-blogging-plugin-2.2.4/mkdocs_blogging_plugin/templates/blog.html
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-04 02:06:54.000000 mkdocs-blogging-plugin-2.2.4/mkdocs_blogging_plugin/templates/pagination.js
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-04-04 02:06:54.000000 mkdocs-blogging-plugin-2.2.4/mkdocs_blogging_plugin/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 02:07:13.318438 mkdocs-blogging-plugin-2.2.4/mkdocs_blogging_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-04 02:07:13.000000 mkdocs-blogging-plugin-2.2.4/mkdocs_blogging_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-04 02:07:13.000000 mkdocs-blogging-plugin-2.2.4/mkdocs_blogging_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 02:07:13.000000 mkdocs-blogging-plugin-2.2.4/mkdocs_blogging_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-04 02:07:13.000000 mkdocs-blogging-plugin-2.2.4/mkdocs_blogging_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-04 02:07:13.000000 mkdocs-blogging-plugin-2.2.4/mkdocs_blogging_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-04 02:07:13.000000 mkdocs-blogging-plugin-2.2.4/mkdocs_blogging_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-04 02:06:54.000000 mkdocs-blogging-plugin-2.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 02:07:13.322438 mkdocs-blogging-plugin-2.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-04 02:06:54.000000 mkdocs-blogging-plugin-2.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 02:07:13.322438 mkdocs-blogging-plugin-2.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 02:06:54.000000 mkdocs-blogging-plugin-2.2.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-04 02:06:54.000000 mkdocs-blogging-plugin-2.2.4/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-04 02:06:54.000000 mkdocs-blogging-plugin-2.2.4/tests/test_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-04 02:06:54.000000 mkdocs-blogging-plugin-2.2.4/tests/test_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:34:47.960299 mkdocs-blogging-plugin-2.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-12 17:34:29.000000 mkdocs-blogging-plugin-2.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-12 17:34:29.000000 mkdocs-blogging-plugin-2.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-12 17:34:47.960299 mkdocs-blogging-plugin-2.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-12 17:34:29.000000 mkdocs-blogging-plugin-2.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:34:47.960299 mkdocs-blogging-plugin-2.2.5/mkdocs_blogging_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 17:34:29.000000 mkdocs-blogging-plugin-2.2.5/mkdocs_blogging_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-12 17:34:29.000000 mkdocs-blogging-plugin-2.2.5/mkdocs_blogging_plugin/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13877 2023-04-12 17:34:29.000000 mkdocs-blogging-plugin-2.2.5/mkdocs_blogging_plugin/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:34:47.960299 mkdocs-blogging-plugin-2.2.5/mkdocs_blogging_plugin/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-12 17:34:29.000000 mkdocs-blogging-plugin-2.2.5/mkdocs_blogging_plugin/templates/blog-button-theme.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-12 17:34:29.000000 mkdocs-blogging-plugin-2.2.5/mkdocs_blogging_plugin/templates/blog-card-theme.html
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-12 17:34:29.000000 mkdocs-blogging-plugin-2.2.5/mkdocs_blogging_plugin/templates/blog-tags-index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-12 17:34:29.000000 mkdocs-blogging-plugin-2.2.5/mkdocs_blogging_plugin/templates/blog-tags-render.html
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-12 17:34:29.000000 mkdocs-blogging-plugin-2.2.5/mkdocs_blogging_plugin/templates/blog-tags.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-12 17:34:29.000000 mkdocs-blogging-plugin-2.2.5/mkdocs_blogging_plugin/templates/blog.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-12 17:34:29.000000 mkdocs-blogging-plugin-2.2.5/mkdocs_blogging_plugin/templates/pagination.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-04-12 17:34:29.000000 mkdocs-blogging-plugin-2.2.5/mkdocs_blogging_plugin/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:34:47.960299 mkdocs-blogging-plugin-2.2.5/mkdocs_blogging_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-12 17:34:47.000000 mkdocs-blogging-plugin-2.2.5/mkdocs_blogging_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-12 17:34:47.000000 mkdocs-blogging-plugin-2.2.5/mkdocs_blogging_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 17:34:47.000000 mkdocs-blogging-plugin-2.2.5/mkdocs_blogging_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-12 17:34:47.000000 mkdocs-blogging-plugin-2.2.5/mkdocs_blogging_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-12 17:34:47.000000 mkdocs-blogging-plugin-2.2.5/mkdocs_blogging_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-12 17:34:47.000000 mkdocs-blogging-plugin-2.2.5/mkdocs_blogging_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-12 17:34:29.000000 mkdocs-blogging-plugin-2.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 17:34:47.960299 mkdocs-blogging-plugin-2.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-12 17:34:29.000000 mkdocs-blogging-plugin-2.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:34:47.960299 mkdocs-blogging-plugin-2.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 17:34:29.000000 mkdocs-blogging-plugin-2.2.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-12 17:34:29.000000 mkdocs-blogging-plugin-2.2.5/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-12 17:34:29.000000 mkdocs-blogging-plugin-2.2.5/tests/test_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-12 17:34:29.000000 mkdocs-blogging-plugin-2.2.5/tests/test_template.py
```

### Comparing `mkdocs-blogging-plugin-2.2.4/LICENSE` & `mkdocs-blogging-plugin-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.4/PKG-INFO` & `mkdocs-blogging-plugin-2.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-blogging-plugin
-Version: 2.2.4
+Version: 2.2.5
 Summary: Mkdocs plugin that generates a blog index page sorted by creation date.
 Author: Liang Yesheang
 Author-email: liang2kl@outlook.com
 License: MIT
 Project-URL: Source, https://github.com/liang2kl/mkdocs-blogging-plugin
 Keywords: mkdocs blog plugin
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mkdocs-blogging-plugin-2.2.4/README.md` & `mkdocs-blogging-plugin-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.4/mkdocs_blogging_plugin/config.py` & `mkdocs-blogging-plugin-2.2.5/mkdocs_blogging_plugin/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.4/mkdocs_blogging_plugin/plugin.py` & `mkdocs-blogging-plugin-2.2.5/mkdocs_blogging_plugin/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-import os
 import logging
+import os
 import re
+from datetime import date, datetime
+from pathlib import Path
 from typing import Dict
+
+from jinja2 import Environment, FileSystemLoader, Template, select_autoescape
 from mkdocs.config import config_options
-from mkdocs.plugins import BasePlugin
 from mkdocs.exceptions import PluginError
-from jinja2 import Environment, FileSystemLoader, Template, select_autoescape
+from mkdocs.plugins import BasePlugin
+
 from mkdocs_blogging_plugin.config import BloggingConfig
+
 from .util import Util
-from pathlib import Path
-from datetime import datetime
 
 DIR_PATH = Path(os.path.dirname(os.path.realpath(__file__)))
 BLOG_PAGE_PATTERN = re.compile(
     r"\{\{\s*blog_content\s+(([0-9]|[a-z]|[A-Z]|-|_)*)\s*\}\}", flags=re.IGNORECASE)
 TAG_PAGE_PATTERN = re.compile(
     r"\{\{\s*tag_content\s*\}\}", flags=re.IGNORECASE)
 THEMES = ["card", "button"]
@@ -328,22 +331,28 @@
             index_url=self.tags_index_url, show_tags="tags" in self.features,
             mkdocs_context=self.mkdocs_template_context,
             full_content=config.full_content,
         )
 
     def with_timestamp(self, page, by_revision):
         timestamp = None
-        if self.meta_time_format:
-            if "time" in page.meta:
-                timestamp = datetime.strptime(
-                    page.meta["time"], self.meta_time_format).timestamp()
-            elif "date" in page.meta:
-                timestamp = datetime.strptime(
-                    page.meta["date"], self.meta_time_format).timestamp()
+        if "time" in page.meta:
+            timestamp = self._parse_time(page.meta["time"])
+        if "date" in page.meta and timestamp is None:
+            timestamp = self._parse_time(page.meta["date"])
         if not timestamp:
             timestamp = self.util.get_git_commit_timestamp(
                 page.file.abs_src_path, is_first_commit=(not by_revision))
         page.meta["git-timestamp"] = timestamp
         page.meta["localized-time"] = self.util.get_localized_date(
             timestamp, False, format=self.time_format, _locale=self.locale)
 
         return page
+
+    def _parse_time(self, value):
+        if isinstance(value, datetime):
+            return value.timestamp()
+        if isinstance(value, date):
+            return datetime.combine(value, datetime.min.time()).timestamp()
+        if self.meta_time_format and isinstance(value, str):
+            return datetime.strptime(value, self.meta_time_format).timestamp()
+        return None
```

### Comparing `mkdocs-blogging-plugin-2.2.4/mkdocs_blogging_plugin/templates/blog-button-theme.html` & `mkdocs-blogging-plugin-2.2.5/mkdocs_blogging_plugin/templates/blog-button-theme.html`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.4/mkdocs_blogging_plugin/templates/blog-card-theme.html` & `mkdocs-blogging-plugin-2.2.5/mkdocs_blogging_plugin/templates/blog-card-theme.html`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.4/mkdocs_blogging_plugin/templates/blog-tags-index.html` & `mkdocs-blogging-plugin-2.2.5/mkdocs_blogging_plugin/templates/blog-tags-index.html`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.4/mkdocs_blogging_plugin/templates/blog-tags-render.html` & `mkdocs-blogging-plugin-2.2.5/mkdocs_blogging_plugin/templates/blog-tags-render.html`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.4/mkdocs_blogging_plugin/templates/blog.html` & `mkdocs-blogging-plugin-2.2.5/mkdocs_blogging_plugin/templates/blog.html`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.4/mkdocs_blogging_plugin/templates/pagination.js` & `mkdocs-blogging-plugin-2.2.5/mkdocs_blogging_plugin/templates/pagination.js`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.4/mkdocs_blogging_plugin/util.py` & `mkdocs-blogging-plugin-2.2.5/mkdocs_blogging_plugin/util.py`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.4/mkdocs_blogging_plugin.egg-info/PKG-INFO` & `mkdocs-blogging-plugin-2.2.5/mkdocs_blogging_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-blogging-plugin
-Version: 2.2.4
+Version: 2.2.5
 Summary: Mkdocs plugin that generates a blog index page sorted by creation date.
 Author: Liang Yesheang
 Author-email: liang2kl@outlook.com
 License: MIT
 Project-URL: Source, https://github.com/liang2kl/mkdocs-blogging-plugin
 Keywords: mkdocs blog plugin
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mkdocs-blogging-plugin-2.2.4/mkdocs_blogging_plugin.egg-info/SOURCES.txt` & `mkdocs-blogging-plugin-2.2.5/mkdocs_blogging_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.4/setup.py` & `mkdocs-blogging-plugin-2.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     LONG_DESCRIPTION = file.read()
 
 with open("requirements.txt", "r") as file:
     DEPENDENCIES = file.readlines()
 
 setup(
     name="mkdocs-blogging-plugin",
-    version="2.2.4",
+    version="2.2.5",
     description="Mkdocs plugin that generates a blog index page sorted by creation date.",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     keywords="mkdocs blog plugin",
     project_urls={
         "Source": "https://github.com/liang2kl/mkdocs-blogging-plugin"
     },
```

### Comparing `mkdocs-blogging-plugin-2.2.4/tests/test_config.py` & `mkdocs-blogging-plugin-2.2.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.4/tests/test_template.py` & `mkdocs-blogging-plugin-2.2.5/tests/test_template.py`

 * *Files identical despite different names*

