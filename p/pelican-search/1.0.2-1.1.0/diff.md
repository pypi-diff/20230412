# Comparing `tmp/pelican_search-1.0.2.tar.gz` & `tmp/pelican_search-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelican_search-1.0.2.tar", max compression
+gzip compressed data, was "pelican_search-1.1.0.tar", max compression
```

## Comparing `pelican_search-1.0.2.tar` & `pelican_search-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     8370 2023-02-09 06:55:53.522159 pelican_search-1.0.2/README.md
--rw-r--r--   0        0        0       30 2023-02-09 06:55:53.522159 pelican_search-1.0.2/pelican/plugins/search/__init__.py
--rw-r--r--   0        0        0     3922 2023-02-09 06:55:53.522159 pelican_search-1.0.2/pelican/plugins/search/search.py
--rw-r--r--   0        0        0     1562 2023-02-09 06:56:11.507471 pelican_search-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     9368 1970-01-01 00:00:00.000000 pelican_search-1.0.2/setup.py
--rw-r--r--   0        0        0     9857 1970-01-01 00:00:00.000000 pelican_search-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     9167 2023-04-12 08:51:19.320566 pelican_search-1.1.0/README.md
+-rw-r--r--   0        0        0       30 2023-04-12 08:51:19.320566 pelican_search-1.1.0/pelican/plugins/search/__init__.py
+-rw-r--r--   0        0        0     4919 2023-04-12 08:51:19.320566 pelican_search-1.1.0/pelican/plugins/search/search.py
+-rw-r--r--   0        0        0     1719 2023-04-12 08:51:32.204803 pelican_search-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    10595 1970-01-01 00:00:00.000000 pelican_search-1.1.0/PKG-INFO
```

### Comparing `pelican_search-1.0.2/README.md` & `pelican_search-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -39,19 +39,29 @@
 If you are using Pelican 4.5+ with namespace plugins and don’t have a `PLUGINS` setting defined in your configuration, then the Search plugin should be auto-discovered with no further action required. If, on the other hand, you _do_ have a `PLUGINS` setting defined (because you also use legacy plugins or because you want to be able to selectively disable installed plugins), then you must manually add `search` to the `PLUGINS` list, as described in the [Pelican plugins documentation][].
 
 
 ## Settings
 
 This plugin’s behavior can be customized via Pelican settings. Those settings, and their default values, follow below.
 
-### `SEARCH_MODE = "output"`
+### `STORK_INPUT_OPTIONS = ""`
 
-In addition to plain-text files, Stork can recognize and index HTML and Markdown-formatted content. The default behavior of this plugin is to index generated HTML files, since Stork is good at extracting content from tags, scripts, and styles. But that mode may require a slight theme modification that isn’t necessary when indexing Markdown source (see `SEARCH_HTML_SELECTOR` setting below). That said, indexing Markdown means that markup information may not be removed from the indexed content and will thus be visible in the search preview results. With that caveat aside, if you want to index Markdown source content files instead of the generated HTML output, you can use: `SEARCH_MODE = "source"`
+In addition to plain-text files, Stork can recognize and index HTML and Markdown-formatted content. The default behavior of this plugin is to index generated HTML files, since Stork is good at extracting content from tags, scripts, and styles. But that mode may require a slight theme modification that isn’t necessary when indexing Markdown source (see HTML selector setting below). That said, indexing Markdown means that markup information may not be removed from the indexed content and will thus be visible in the search preview results. With that caveat aside, if you want to index Markdown source content files instead of the generated HTML output, you can set `base_directory` to your content path.
 
-### `SEARCH_HTML_SELECTOR = "main"`
+Any other setting then the output path will toggle the plugin to switch to "source" mode.
+
+**Example**:
+
+```python
+STORK_INPUT_OPTIONS = {
+    base_directory = PATH
+}
+```
+
+#### Stork HTML Selector
 
 By default, Stork looks for `<main>[…]</main>` tags to determine where your main content is located. If such tags do not already exist in your theme’s template files, you can either (1) add `<main>` tags or (2) change the HTML selector that Stork should look for.
 
 To use the default `main` selector, in each of your theme’s relevant template files, wrap the content you want to index with `<main>` tags. For example:
 
 `article.html`:
 
@@ -68,14 +78,46 @@
 {{ page.content }}
 </main>
 
 ```
 
 For more information, refer to [Stork’s documentation on HTML tag selection](https://stork-search.net/docs/html).
 
+**Example**:
+
+To set it to a different selector (for example, `primary`), you can set it like this:
+
+```python
+STORK_INPUT_OPTIONS = {
+    html_selector = "primary"
+}
+```
+
+Additional [Input Options](https://stork-search.net/docs/config-ref) can be added here as a `dict`.
+
+**Example**:
+
+```python
+STORK_INPUT_OPTIONS = {
+    url_prefix = SITEURL
+}
+```
+
+### `STORK_OUTPUT_OPTIONS = ""`
+
+[Output Options](https://stork-search.net/docs/config-ref) can be configured as a `dict`.
+Keep in mind that keys are case-sensitive and must be lower case.
+
+**Example**:
+
+```python
+STORK_OUTPUT_OPTIONS = {
+    debug = true
+}
+```
 
 ## Static Assets
 
 There are two options for serving the necessary JavaScript, WebAssembly, and CSS static assets:
 
 1. Use a content delivery network (CDN) to serve Stork’s static assets
 2. Self-host the Stork static assets
@@ -91,25 +133,29 @@
 ```html
 <link rel="stylesheet" href="https://files.stork-search.net/basic.css" />
 ```
 
 If your theme supports dark mode, you may want to also add Stork’s dark CSS file:
 
 ```html
-<link rel="stylesheet" media="screen and (prefers-color-scheme: dark)" href="https://files.stork-search.net/dark.css">
+<link
+    rel="stylesheet"
+    media="screen and (prefers-color-scheme: dark)"
+    href="https://files.stork-search.net/dark.css"
+/>
 ```
 
 #### JavaScript
 
 Add the following script tags to your theme’s base template, just before your closing `</body>` tag, which will load the most recent Stork module along with the matching WASM binary:
 
 ```html
 <script src="https://files.stork-search.net/releases/v1.5.0/stork.js"></script>
 <script>
-    stork.register("sitesearch", "{{ SITEURL }}/search-index.st")
+    stork.register("sitesearch", "{{ SITEURL }}/search-index.st");
 </script>
 ```
 
 ### Static Assets — Option 2: Self-Host
 
 Download the Stork JavaScript, WebAssembly, and CSS files and put them in your theme’s respective static asset directories:
```

### Comparing `pelican_search-1.0.2/pelican/plugins/search/search.py` & `pelican_search-1.1.0/pelican/plugins/search/search.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,120 +3,139 @@
 ======
 
 A Pelican plugin to generate an index for static site searches.
 
 Copyright (c) Justin Mayer
 """
 
-from codecs import open
-from inspect import cleandoc
-from json import dumps
 import logging
-import os.path
+from pathlib import Path
 from shutil import which
 import subprocess
+from typing import Dict, List
 
 from jinja2.filters import do_striptags as striptags
+import rtoml
 
 from pelican import signals
 
 logger = logging.getLogger(__name__)
 
 
 class SearchSettingsGenerator:
     def __init__(self, context, settings, path, theme, output_path, *null):
         self.output_path = output_path
         self.context = context
         self.content = settings.get("PATH")
         self.tpages = settings.get("TEMPLATE_PAGES")
-        self.search_mode = settings.get("SEARCH_MODE", "output")
-        self.html_selector = settings.get("SEARCH_HTML_SELECTOR", "main")
+        self.input_options = settings.get("STORK_INPUT_OPTIONS", {})
+        self.output_options = settings.get("STORK_OUTPUT_OPTIONS")
+        # Set default values
+        self.input_options.setdefault("html_selector", "main")
+        self.input_options.setdefault("base_directory", self.output_path)
+
+        # Handle deprecated settings
+        if settings.get("SEARCH_HTML_SELECTOR") and not settings.get(
+            "STORK_INPUT_OPTIONS"
+        ):
+            logger.warning(
+                "The SEARCH_HTML_SELECTOR setting is deprecated "
+                "and will be removed in a future version. "
+                "Use the STORK_INPUT_OPTIONS setting instead."
+            )
+            self.input_options["html_selector"] = settings.get("SEARCH_HTML_SELECTOR")
+        if settings.get("SEARCH_MODE") and not settings.get("STORK_INPUT_OPTIONS"):
+            logger.warning(
+                f"SEARCH_MODE = {settings.get('SEARCH_MODE')} is deprecated "
+                "and will be removed in a future version. "
+                "Use the STORK_INPUT_OPTIONS setting instead."
+            )
+            self.input_options["base_directory"] = self.output_path
+            if settings.get("SEARCH_MODE") == "source":
+                self.input_options["base_directory"] = self.content
+
+    def generate_output(self, writer):
+        search_settings_path = Path(self.output_path) / "search.toml"
 
-    def build_search_index(self, search_settings_path):
+        self.generate_stork_settings(search_settings_path)
+
+        # Build the search index
+        build_log = self.build_search_index(search_settings_path)
+        build_log = "".join(["Search plugin reported ", build_log])
+        logger.error(build_log) if "error" in build_log else logger.debug(build_log)
+
+    def build_search_index(self, search_settings_path: Path):
         if not which("stork"):
             raise Exception("Stork must be installed and available on $PATH.")
         try:
             output = subprocess.run(
                 [
                     "stork",
                     "build",
                     "--input",
-                    search_settings_path,
+                    str(search_settings_path),
                     "--output",
                     f"{self.output_path}/search-index.st",
                 ],
                 capture_output=True,
                 encoding="utf-8",
                 check=True,
             )
         except subprocess.CalledProcessError as e:
             raise Exception("".join(["Search plugin reported ", e.stdout, e.stderr]))
 
         return output.stdout
 
-    def generate_output(self, writer):
-        search_settings_path = os.path.join(self.output_path, "search.toml")
+    def generate_stork_settings(self, search_settings_path: Path):
+        self.input_options["files"] = self.get_input_files()
+
+        search_settings = {"input": self.input_options}
+
+        if self.output_options:
+            search_settings["output"] = self.output_options
 
+        # Write the search settings file to disk
+        with search_settings_path.open("w") as fd:
+            rtoml.dump(obj=search_settings, file=fd)
+
+    def _index_output(self) -> bool:
+        return self.input_options["base_directory"] == self.output_path
+
+    def get_input_files(
+        self,
+    ) -> List[Dict]:
         pages = self.context["pages"] + self.context["articles"]
 
         for article in self.context["articles"]:
             pages += article.translations
 
-        input_files = ""
-
+        input_files = []
         # Generate list of articles and pages to index
         for page in pages:
-            if self.search_mode == "output":
-                page_to_index = page.save_as
-            if self.search_mode == "source":
-                page_to_index = page.relative_source_path
-            input_file = f"""
-                [[input.files]]
-                path = "{page_to_index}"
-                url = "/{page.url}"
-                title = {dumps(striptags(page.title))}
-            """
-            input_files = "".join([input_files, input_file])
+            page_to_index = (
+                page.save_as if self._index_output() else page.relative_source_path
+            )
+            # Escape double-quotation marks in the title
+            title = striptags(page.title).replace('"', '\\"')
+            input_files.append(
+                {
+                    "path": page_to_index,
+                    "url": f"/{page.url}",
+                    "title": f"{title}",
+                }
+            )
 
         # Generate list of *template* pages to index (if any)
         for tpage in self.tpages:
-            if self.search_mode == "output":
-                tpage_to_index = self.tpages[tpage]
-            if self.search_mode == "source":
-                tpage_to_index = tpage
-            input_file = f"""
-                [[input.files]]
-                path = "{tpage_to_index}"
-                url = "{self.tpages[tpage]}"
-                title = ""
-            """
-            input_files = "".join([input_files, input_file])
-
-        # Assemble the search settings file
-        if self.search_mode == "output":
-            base_dir = self.output_path
-        if self.search_mode == "source":
-            base_dir = self.content
-        search_settings = cleandoc(
-            f"""
-                [input]
-                base_directory = "{base_dir}"
-                html_selector = "{self.html_selector}"
-                {input_files}
-            """
-        )
-
-        # Write the search settings file to disk
-        with open(search_settings_path, "w", encoding="utf-8") as fd:
-            fd.write(search_settings)
+            tpage_to_index = self.tpages[tpage] if self._index_output() else tpage
+            input_files.append(
+                {"path": tpage_to_index, "url": self.tpages[tpage], "title": ""}
+            )
 
-        # Build the search index
-        build_log = self.build_search_index(search_settings_path)
-        build_log = "".join(["Search plugin reported ", build_log])
-        logger.error(build_log) if "error" in build_log else logger.debug(build_log)
+        return input_files
 
 
 def get_generators(generators):
     return SearchSettingsGenerator
 
 
 def register():
```

### Comparing `pelican_search-1.0.2/pyproject.toml` & `pelican_search-1.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pelican-search"
-version = "1.0.2"
+version = "1.1.0"
 description = "Pelican plugin that indexes content and enables static site searches"
 authors = ["Justin Mayer <entroP@gmail.com>"]
 license = "AGPL-3.0"
 readme = "README.md"
 keywords = ["pelican", "plugin", "search", "index"]
 repository = "https://github.com/pelican-plugins/search"
 documentation = "https://docs.getpelican.com"
@@ -24,35 +24,43 @@
 ]
 
 [tool.poetry.urls]
 "Funding" = "https://donate.getpelican.com/"
 "Issue Tracker" = "https://github.com/pelican-plugins/search/issues"
 
 [tool.poetry.dependencies]
-python = ">=3.7,<4.0"
+python = ">=3.8.1,<4.0"
 pelican = ">=4.5"
 markdown = {version = ">=3.2", optional = true}
+rtoml = "^0.9.0"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 black = "^23"
-flake8 = "^5.0"
+flake8 = "^6.0"
 flake8-black = "^0.3"
+flake8-pyproject = "^1.2"
 invoke = "^2.0"
-isort = "^5.4"
+isort = "^5.12.0"
 livereload = "^2.6"
 markdown = "^3.2"
+pytest = "^7.2.2"
+pytest-mock = "^3.10.0"
 
 [tool.poetry.extras]
 markdown = ["markdown"]
 
 [tool.autopub]
 project-name = "Search"
 git-username = "botpub"
 git-email = "botpub@autopub.rocks"
 
+[tool.flake8]
+extend-ignore = ["E203"]
+max-line-length = 88
+
 [tool.isort]
 profile = "black"
 
 # Sort imports within their section independent of the import type
 force_sort_within_sections = true
 
 [build-system]
```

### Comparing `pelican_search-1.0.2/setup.py` & `pelican_search-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,274 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pelican-search
+Version: 1.1.0
+Summary: Pelican plugin that indexes content and enables static site searches
+Home-page: https://github.com/pelican-plugins/search
+License: AGPL-3.0
+Keywords: pelican,plugin,search,index
+Author: Justin Mayer
+Author-email: entroP@gmail.com
+Requires-Python: >=3.8.1,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Framework :: Pelican
+Classifier: Framework :: Pelican :: Plugins
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: markdown
+Requires-Dist: markdown (>=3.2) ; extra == "markdown"
+Requires-Dist: pelican (>=4.5)
+Requires-Dist: rtoml (>=0.9.0,<0.10.0)
+Project-URL: Documentation, https://docs.getpelican.com
+Project-URL: Funding, https://donate.getpelican.com/
+Project-URL: Issue Tracker, https://github.com/pelican-plugins/search/issues
+Project-URL: Repository, https://github.com/pelican-plugins/search
+Description-Content-Type: text/markdown
 
-packages = \
-['pelican', 'pelican.plugins.search']
+# Search: A Plugin for Pelican
 
-package_data = \
-{'': ['*']}
+[![Build Status](https://img.shields.io/github/actions/workflow/status/pelican-plugins/search/main.yml?branch=main)](https://github.com/pelican-plugins/search/actions)
+[![PyPI Version](https://img.shields.io/pypi/v/pelican-search)](https://pypi.org/project/pelican-search/)
 
-install_requires = \
-['pelican>=4.5']
-
-extras_require = \
-{'markdown': ['markdown>=3.2']}
-
-setup_kwargs = {
-    'name': 'pelican-search',
-    'version': '1.0.2',
-    'description': 'Pelican plugin that indexes content and enables static site searches',
-    'long_description': '# Search: A Plugin for Pelican\n\n[![Build Status](https://img.shields.io/github/actions/workflow/status/pelican-plugins/search/main.yml?branch=main)](https://github.com/pelican-plugins/search/actions)\n[![PyPI Version](https://img.shields.io/pypi/v/pelican-search)](https://pypi.org/project/pelican-search/)\n\nThis plugin generates an index for searching content on a Pelican-powered site.\n\n\n## Why would you want this?\n\nStatic sites are, well, static… and thus usually don’t have an application server component that could be used to power site search functionality. Rather than give up control (and privacy) to third-party search engine corporations, this plugin adds elegant and self-hosted site search capability to your site. Last but not least, searches are **really** fast. 🚀\n\nWant to see just _how_ fast? Try it out for yourself. Following are some sites that use this plugin:\n\n* [Justin Mayer](https://justinmayer.com)\n* [Open Source Alternatives](https://opensourcealternatives.org)\n\n\n## Installation\n\nThis plugin uses [Stork](https://stork-search.net/) to generate a search index. Follow the [Stork installation instructions](https://stork-search.net/docs/install) to install this required command-line tool and ensure it is available within `/usr/local/bin/` or another `$PATH`-accessible location of your choosing. For example, Stork can be installed on macOS (Intel) via:\n\n    export STORKVERSION="v1.5.0"\n    wget -O /usr/local/bin/stork https://files.stork-search.net/releases/$STORKVERSION/stork-macos-10-15\n    chmod +x /usr/local/bin/stork\n\nFor macOS on ARM, install via Homebrew:\n\n    brew install stork-search/stork-tap/stork\n\nConfirm that Stork is properly installed via:\n\n    stork --help\n\nOnce Stork has been successfully installed and tested, this plugin can be installed via:\n\n    python -m pip install pelican-search\n\nIf you are using Pelican 4.5+ with namespace plugins and don’t have a `PLUGINS` setting defined in your configuration, then the Search plugin should be auto-discovered with no further action required. If, on the other hand, you _do_ have a `PLUGINS` setting defined (because you also use legacy plugins or because you want to be able to selectively disable installed plugins), then you must manually add `search` to the `PLUGINS` list, as described in the [Pelican plugins documentation][].\n\n\n## Settings\n\nThis plugin’s behavior can be customized via Pelican settings. Those settings, and their default values, follow below.\n\n### `SEARCH_MODE = "output"`\n\nIn addition to plain-text files, Stork can recognize and index HTML and Markdown-formatted content. The default behavior of this plugin is to index generated HTML files, since Stork is good at extracting content from tags, scripts, and styles. But that mode may require a slight theme modification that isn’t necessary when indexing Markdown source (see `SEARCH_HTML_SELECTOR` setting below). That said, indexing Markdown means that markup information may not be removed from the indexed content and will thus be visible in the search preview results. With that caveat aside, if you want to index Markdown source content files instead of the generated HTML output, you can use: `SEARCH_MODE = "source"`\n\n### `SEARCH_HTML_SELECTOR = "main"`\n\nBy default, Stork looks for `<main>[…]</main>` tags to determine where your main content is located. If such tags do not already exist in your theme’s template files, you can either (1) add `<main>` tags or (2) change the HTML selector that Stork should look for.\n\nTo use the default `main` selector, in each of your theme’s relevant template files, wrap the content you want to index with `<main>` tags. For example:\n\n`article.html`:\n\n```jinja\n<main>\n{{ article.content }}\n</main>\n```\n\n`page.html`:\n\n```jinja\n<main>\n{{ page.content }}\n</main>\n\n```\n\nFor more information, refer to [Stork’s documentation on HTML tag selection](https://stork-search.net/docs/html).\n\n\n## Static Assets\n\nThere are two options for serving the necessary JavaScript, WebAssembly, and CSS static assets:\n\n1. Use a content delivery network (CDN) to serve Stork’s static assets\n2. Self-host the Stork static assets\n\nThe first option is easier to set up. The second option is provided for folks who prefer to self-host everything. After you have decided which option you prefer, follow the relevant section’s instructions below.\n\n### Static Assets — Option 1: Use CDN\n\n#### CSS\n\nAdd the Stork CSS before the closing `</head>` tag in your theme’s base template file, such as `base.html`:\n\n```html\n<link rel="stylesheet" href="https://files.stork-search.net/basic.css" />\n```\n\nIf your theme supports dark mode, you may want to also add Stork’s dark CSS file:\n\n```html\n<link rel="stylesheet" media="screen and (prefers-color-scheme: dark)" href="https://files.stork-search.net/dark.css">\n```\n\n#### JavaScript\n\nAdd the following script tags to your theme’s base template, just before your closing `</body>` tag, which will load the most recent Stork module along with the matching WASM binary:\n\n```html\n<script src="https://files.stork-search.net/releases/v1.5.0/stork.js"></script>\n<script>\n    stork.register("sitesearch", "{{ SITEURL }}/search-index.st")\n</script>\n```\n\n### Static Assets — Option 2: Self-Host\n\nDownload the Stork JavaScript, WebAssembly, and CSS files and put them in your theme’s respective static asset directories:\n\n```shell\nexport STORKVERSION="v1.5.0"\ncd $YOUR-THEME-DIR\nmkdir -p static/{js,css}\nwget -O static/js/stork.js https://files.stork-search.net/releases/$STORKVERSION/stork.js\nwget -O static/js/stork.js.map https://files.stork-search.net/releases/$STORKVERSION/stork.js.map\nwget -O static/js/stork.wasm https://files.stork-search.net/releases/$STORKVERSION/stork.wasm\nwget -O static/css/stork.css https://files.stork-search.net/basic.css\nwget -O static/css/stork-dark.css https://files.stork-search.net/dark.css\n```\n\n#### CSS\n\nAdd the Stork CSS before the closing `</head>` tag in your theme’s base template file, such as `base.html`:\n\n```jinja\n<link rel="stylesheet" href="{{ SITEURL }}/{{ THEME_STATIC_DIR }}/css/stork.css">\n```\n\nIf your theme supports dark mode, you may want to also add Stork’s dark CSS file:\n\n```jinja\n<link rel="stylesheet" media="screen and (prefers-color-scheme: dark)" href="{{ SITEURL }}/{{ THEME_STATIC_DIR }}/css/stork-dark.css">\n```\n\n#### JavaScript & WebAssembly\n\nAdd the following script tags to your theme’s base template file, such as `base.html`, just before the closing `</body>` tag:\n\n```jinja\n<script src="{{ SITEURL }}/{{ THEME_STATIC_DIR }}/js/stork.js"></script>\n<script>\n    stork.initialize("{{ SITEURL }}/{{ THEME_STATIC_DIR }}/js/stork.wasm")\n    stork.downloadIndex("sitesearch", "{{ SITEURL }}/search-index.st")\n    stork.attach("sitesearch")\n</script>\n```\n\n### Search Input Form\n\nDecide in which place(s) on your site you want to put your search field, such as your `index.html` template file. Then add the search field to the template:\n\n```html\nSearch: <input data-stork="sitesearch" />\n<div data-stork="sitesearch-output"></div>\n```\n\nFor more information regarding this topic, see the [Stork search interface documentation](https://stork-search.net/docs/interface).\n\n\n## Deployment\n\nEnsure your production web server serves the WebAssembly file with the `application/wasm` MIME type. For folks using older versions of Nginx, that might look like the following:\n\n```nginx\n…\nhttp {\n    …\n    include             mime.types;\n    # Types not included in older Nginx versions:\n    types {\n        application/wasm                                 wasm;\n    }\n    …\n}\n```\n\nFor other self-hosting considerations, see the [Stork self-hosting documentation](https://stork-search.net/docs/self-hosting).\n\n\n## Contributing\n\nContributions are welcome and much appreciated. Every little bit helps. You can contribute by improving the documentation, adding missing features, and fixing bugs. You can also help out by reviewing and commenting on [existing issues][].\n\nTo start contributing to this plugin, review the [Contributing to Pelican][] documentation, beginning with the **Contributing Code** section.\n\n[Pelican plugins documentation]: https://docs.getpelican.com/en/latest/plugins.html\n[existing issues]: https://github.com/pelican-plugins/search/issues\n[Contributing to Pelican]: https://docs.getpelican.com/en/latest/contribute.html\n',
-    'author': 'Justin Mayer',
-    'author_email': 'entroP@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/pelican-plugins/search',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
+This plugin generates an index for searching content on a Pelican-powered site.
+
+
+## Why would you want this?
+
+Static sites are, well, static… and thus usually don’t have an application server component that could be used to power site search functionality. Rather than give up control (and privacy) to third-party search engine corporations, this plugin adds elegant and self-hosted site search capability to your site. Last but not least, searches are **really** fast. 🚀
+
+Want to see just _how_ fast? Try it out for yourself. Following are some sites that use this plugin:
+
+* [Justin Mayer](https://justinmayer.com)
+* [Open Source Alternatives](https://opensourcealternatives.org)
+
+
+## Installation
+
+This plugin uses [Stork](https://stork-search.net/) to generate a search index. Follow the [Stork installation instructions](https://stork-search.net/docs/install) to install this required command-line tool and ensure it is available within `/usr/local/bin/` or another `$PATH`-accessible location of your choosing. For example, Stork can be installed on macOS (Intel) via:
+
+    export STORKVERSION="v1.5.0"
+    wget -O /usr/local/bin/stork https://files.stork-search.net/releases/$STORKVERSION/stork-macos-10-15
+    chmod +x /usr/local/bin/stork
+
+For macOS on ARM, install via Homebrew:
+
+    brew install stork-search/stork-tap/stork
+
+Confirm that Stork is properly installed via:
+
+    stork --help
+
+Once Stork has been successfully installed and tested, this plugin can be installed via:
+
+    python -m pip install pelican-search
+
+If you are using Pelican 4.5+ with namespace plugins and don’t have a `PLUGINS` setting defined in your configuration, then the Search plugin should be auto-discovered with no further action required. If, on the other hand, you _do_ have a `PLUGINS` setting defined (because you also use legacy plugins or because you want to be able to selectively disable installed plugins), then you must manually add `search` to the `PLUGINS` list, as described in the [Pelican plugins documentation][].
+
+
+## Settings
+
+This plugin’s behavior can be customized via Pelican settings. Those settings, and their default values, follow below.
+
+### `STORK_INPUT_OPTIONS = ""`
+
+In addition to plain-text files, Stork can recognize and index HTML and Markdown-formatted content. The default behavior of this plugin is to index generated HTML files, since Stork is good at extracting content from tags, scripts, and styles. But that mode may require a slight theme modification that isn’t necessary when indexing Markdown source (see HTML selector setting below). That said, indexing Markdown means that markup information may not be removed from the indexed content and will thus be visible in the search preview results. With that caveat aside, if you want to index Markdown source content files instead of the generated HTML output, you can set `base_directory` to your content path.
+
+Any other setting then the output path will toggle the plugin to switch to "source" mode.
+
+**Example**:
+
+```python
+STORK_INPUT_OPTIONS = {
+    base_directory = PATH
+}
+```
+
+#### Stork HTML Selector
+
+By default, Stork looks for `<main>[…]</main>` tags to determine where your main content is located. If such tags do not already exist in your theme’s template files, you can either (1) add `<main>` tags or (2) change the HTML selector that Stork should look for.
+
+To use the default `main` selector, in each of your theme’s relevant template files, wrap the content you want to index with `<main>` tags. For example:
+
+`article.html`:
+
+```jinja
+<main>
+{{ article.content }}
+</main>
+```
+
+`page.html`:
+
+```jinja
+<main>
+{{ page.content }}
+</main>
+
+```
+
+For more information, refer to [Stork’s documentation on HTML tag selection](https://stork-search.net/docs/html).
+
+**Example**:
+
+To set it to a different selector (for example, `primary`), you can set it like this:
+
+```python
+STORK_INPUT_OPTIONS = {
+    html_selector = "primary"
+}
+```
+
+Additional [Input Options](https://stork-search.net/docs/config-ref) can be added here as a `dict`.
+
+**Example**:
+
+```python
+STORK_INPUT_OPTIONS = {
+    url_prefix = SITEURL
+}
+```
+
+### `STORK_OUTPUT_OPTIONS = ""`
+
+[Output Options](https://stork-search.net/docs/config-ref) can be configured as a `dict`.
+Keep in mind that keys are case-sensitive and must be lower case.
+
+**Example**:
+
+```python
+STORK_OUTPUT_OPTIONS = {
+    debug = true
+}
+```
+
+## Static Assets
+
+There are two options for serving the necessary JavaScript, WebAssembly, and CSS static assets:
+
+1. Use a content delivery network (CDN) to serve Stork’s static assets
+2. Self-host the Stork static assets
+
+The first option is easier to set up. The second option is provided for folks who prefer to self-host everything. After you have decided which option you prefer, follow the relevant section’s instructions below.
+
+### Static Assets — Option 1: Use CDN
+
+#### CSS
+
+Add the Stork CSS before the closing `</head>` tag in your theme’s base template file, such as `base.html`:
+
+```html
+<link rel="stylesheet" href="https://files.stork-search.net/basic.css" />
+```
+
+If your theme supports dark mode, you may want to also add Stork’s dark CSS file:
+
+```html
+<link
+    rel="stylesheet"
+    media="screen and (prefers-color-scheme: dark)"
+    href="https://files.stork-search.net/dark.css"
+/>
+```
+
+#### JavaScript
+
+Add the following script tags to your theme’s base template, just before your closing `</body>` tag, which will load the most recent Stork module along with the matching WASM binary:
+
+```html
+<script src="https://files.stork-search.net/releases/v1.5.0/stork.js"></script>
+<script>
+    stork.register("sitesearch", "{{ SITEURL }}/search-index.st");
+</script>
+```
+
+### Static Assets — Option 2: Self-Host
+
+Download the Stork JavaScript, WebAssembly, and CSS files and put them in your theme’s respective static asset directories:
+
+```shell
+export STORKVERSION="v1.5.0"
+cd $YOUR-THEME-DIR
+mkdir -p static/{js,css}
+wget -O static/js/stork.js https://files.stork-search.net/releases/$STORKVERSION/stork.js
+wget -O static/js/stork.js.map https://files.stork-search.net/releases/$STORKVERSION/stork.js.map
+wget -O static/js/stork.wasm https://files.stork-search.net/releases/$STORKVERSION/stork.wasm
+wget -O static/css/stork.css https://files.stork-search.net/basic.css
+wget -O static/css/stork-dark.css https://files.stork-search.net/dark.css
+```
+
+#### CSS
+
+Add the Stork CSS before the closing `</head>` tag in your theme’s base template file, such as `base.html`:
+
+```jinja
+<link rel="stylesheet" href="{{ SITEURL }}/{{ THEME_STATIC_DIR }}/css/stork.css">
+```
+
+If your theme supports dark mode, you may want to also add Stork’s dark CSS file:
+
+```jinja
+<link rel="stylesheet" media="screen and (prefers-color-scheme: dark)" href="{{ SITEURL }}/{{ THEME_STATIC_DIR }}/css/stork-dark.css">
+```
+
+#### JavaScript & WebAssembly
+
+Add the following script tags to your theme’s base template file, such as `base.html`, just before the closing `</body>` tag:
+
+```jinja
+<script src="{{ SITEURL }}/{{ THEME_STATIC_DIR }}/js/stork.js"></script>
+<script>
+    stork.initialize("{{ SITEURL }}/{{ THEME_STATIC_DIR }}/js/stork.wasm")
+    stork.downloadIndex("sitesearch", "{{ SITEURL }}/search-index.st")
+    stork.attach("sitesearch")
+</script>
+```
+
+### Search Input Form
+
+Decide in which place(s) on your site you want to put your search field, such as your `index.html` template file. Then add the search field to the template:
+
+```html
+Search: <input data-stork="sitesearch" />
+<div data-stork="sitesearch-output"></div>
+```
+
+For more information regarding this topic, see the [Stork search interface documentation](https://stork-search.net/docs/interface).
+
+
+## Deployment
+
+Ensure your production web server serves the WebAssembly file with the `application/wasm` MIME type. For folks using older versions of Nginx, that might look like the following:
+
+```nginx
+…
+http {
+    …
+    include             mime.types;
+    # Types not included in older Nginx versions:
+    types {
+        application/wasm                                 wasm;
+    }
+    …
 }
+```
+
+For other self-hosting considerations, see the [Stork self-hosting documentation](https://stork-search.net/docs/self-hosting).
+
+
+## Contributing
+
+Contributions are welcome and much appreciated. Every little bit helps. You can contribute by improving the documentation, adding missing features, and fixing bugs. You can also help out by reviewing and commenting on [existing issues][].
+
+To start contributing to this plugin, review the [Contributing to Pelican][] documentation, beginning with the **Contributing Code** section.
 
+[Pelican plugins documentation]: https://docs.getpelican.com/en/latest/plugins.html
+[existing issues]: https://github.com/pelican-plugins/search/issues
+[Contributing to Pelican]: https://docs.getpelican.com/en/latest/contribute.html
 
-setup(**setup_kwargs)
```

