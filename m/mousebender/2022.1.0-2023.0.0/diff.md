# Comparing `tmp/mousebender-2022.1.0.tar.gz` & `tmp/mousebender-2023.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mousebender-2022.1.0.tar", last modified: Wed Dec 28 01:03:57 2022, max compression
+gzip compressed data, was "mousebender-2023.0.0.tar", last modified: Wed Apr 12 00:37:26 2023, max compression
```

## Comparing `mousebender-2022.1.0.tar` & `mousebender-2023.0.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      273 2022-11-20 23:35:56.198139 mousebender-2022.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0      323 2022-12-28 00:54:41.652515 mousebender-2022.1.0/.github/release.yml
--rw-r--r--   0        0        0     1076 2022-11-20 23:57:08.945531 mousebender-2022.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      670 2022-12-28 00:54:41.652845 mousebender-2022.1.0/.github/workflows/pr-labels.yml
--rw-r--r--   0        0        0     1183 2022-11-20 21:59:27.903740 mousebender-2022.1.0/.gitignore
--rw-r--r--   0        0        0      609 2022-12-03 03:07:04.431820 mousebender-2022.1.0/.readthedocs.yaml
--rw-r--r--   0        0        0      129 2022-12-03 23:33:36.202545 mousebender-2022.1.0/.vscode/extensions.json
--rw-r--r--   0        0        0      275 2022-11-14 01:16:12.080114 mousebender-2022.1.0/.vscode/settings.json
--rw-r--r--   0        0        0     1520 2020-02-29 19:17:56.553683 mousebender-2022.1.0/LICENSE
--rw-r--r--   0        0        0     1857 2022-12-03 03:07:04.432149 mousebender-2022.1.0/README.md
--rw-r--r--   0        0        0      634 2022-11-20 22:18:05.703813 mousebender-2022.1.0/docs/Makefile
--rw-r--r--   0        0        0     2463 2022-12-28 00:54:41.653533 mousebender-2022.1.0/docs/conf.py
--rw-r--r--   0        0        0      315 2022-12-10 20:06:48.625351 mousebender-2022.1.0/docs/index.rst
--rw-r--r--   0        0        0      800 2022-11-20 22:18:05.705215 mousebender-2022.1.0/docs/make.bat
--rw-r--r--   0        0        0     1753 2022-12-28 00:54:41.653938 mousebender-2022.1.0/docs/simple.rst
--rw-r--r--   0        0        0       69 2022-11-20 22:08:13.710157 mousebender-2022.1.0/mousebender/__init__.py
--rw-r--r--   0        0        0        1 2022-12-03 03:07:04.432484 mousebender-2022.1.0/mousebender/py.typed
--rw-r--r--   0        0        0    12226 2022-12-28 00:54:41.654432 mousebender-2022.1.0/mousebender/simple.py
--rw-r--r--   0        0        0     1527 2022-12-28 01:02:27.317719 mousebender-2022.1.0/noxfile.py
--rw-r--r--   0        0        0     1558 2022-12-28 00:56:14.643397 mousebender-2022.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-29 19:17:56.554524 mousebender-2022.1.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-29 19:17:56.554643 mousebender-2022.1.0/tests/data/__init__.py
--rw-r--r--   0        0        0        0 2020-04-07 03:40:04.272668 mousebender-2022.1.0/tests/data/simple/__init__.py
--rw-r--r--   0        0        0     3311 2022-11-12 19:01:21.974165 mousebender-2022.1.0/tests/data/simple/archive_links.aicoe-tensorflow.html
--rw-r--r--   0        0        0    54889 2020-04-11 19:50:46.780940 mousebender-2022.1.0/tests/data/simple/archive_links.numpy-piwheels.html
--rw-r--r--   0        0        0   481602 2020-04-08 02:48:29.052274 mousebender-2022.1.0/tests/data/simple/archive_links.numpy.html
--rw-r--r--   0        0        0   111268 2020-04-08 02:48:29.053799 mousebender-2022.1.0/tests/data/simple/archive_links.pulpcore-client.html
--rw-r--r--   0        0        0    62098 2020-04-08 02:48:29.054681 mousebender-2022.1.0/tests/data/simple/archive_links.pytorch.html
--rw-r--r--   0        0        0 10847162 2020-04-11 19:50:46.847943 mousebender-2022.1.0/tests/data/simple/index.piwheels.html
--rw-r--r--   0        0        0 11451535 2020-04-08 02:48:29.135841 mousebender-2022.1.0/tests/data/simple/index.pypi.html
--rw-r--r--   0        0        0    16002 2022-12-28 00:54:41.656760 mousebender-2022.1.0/tests/test_simple.py
--rw-r--r--   0        0        0     3178 1970-01-01 00:00:00.000000 mousebender-2022.1.0/PKG-INFO
+-rw-r--r--   0        0        0      273 2022-11-20 23:35:56.198139 mousebender-2023.0.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      323 2022-12-28 00:54:41.652515 mousebender-2023.0.0/.github/release.yml
+-rw-r--r--   0        0        0     1076 2022-11-20 23:57:08.945531 mousebender-2023.0.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      670 2023-04-12 00:37:01.066148 mousebender-2023.0.0/.github/workflows/pr-labels.yml
+-rw-r--r--   0        0        0     1183 2022-11-20 21:59:27.903740 mousebender-2023.0.0/.gitignore
+-rw-r--r--   0        0        0      609 2022-12-03 03:07:04.431820 mousebender-2023.0.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      129 2022-12-03 23:33:36.202545 mousebender-2023.0.0/.vscode/extensions.json
+-rw-r--r--   0        0        0      275 2022-11-14 01:16:12.080114 mousebender-2023.0.0/.vscode/settings.json
+-rw-r--r--   0        0        0     1520 2020-02-29 19:17:56.553683 mousebender-2023.0.0/LICENSE
+-rw-r--r--   0        0        0     1857 2022-12-03 03:07:04.432149 mousebender-2023.0.0/README.md
+-rw-r--r--   0        0        0      634 2022-11-20 22:18:05.703813 mousebender-2023.0.0/docs/Makefile
+-rw-r--r--   0        0        0     2463 2022-12-28 00:54:41.653533 mousebender-2023.0.0/docs/conf.py
+-rw-r--r--   0        0        0      315 2022-12-10 20:06:48.625351 mousebender-2023.0.0/docs/index.rst
+-rw-r--r--   0        0        0      800 2022-11-20 22:18:05.705215 mousebender-2023.0.0/docs/make.bat
+-rw-r--r--   0        0        0     1896 2023-04-12 00:37:01.067032 mousebender-2023.0.0/docs/simple.rst
+-rw-r--r--   0        0        0       69 2022-11-20 22:08:13.710157 mousebender-2023.0.0/mousebender/__init__.py
+-rw-r--r--   0        0        0        1 2022-12-03 03:07:04.432484 mousebender-2023.0.0/mousebender/py.typed
+-rw-r--r--   0        0        0    13389 2023-04-12 00:37:01.067870 mousebender-2023.0.0/mousebender/simple.py
+-rw-r--r--   0        0        0     1551 2023-04-12 00:37:01.068543 mousebender-2023.0.0/noxfile.py
+-rw-r--r--   0        0        0     1553 2023-04-12 00:37:01.069625 mousebender-2023.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-29 19:17:56.554524 mousebender-2023.0.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-29 19:17:56.554643 mousebender-2023.0.0/tests/data/__init__.py
+-rw-r--r--   0        0        0        0 2020-04-07 03:40:04.272668 mousebender-2023.0.0/tests/data/simple/__init__.py
+-rw-r--r--   0        0        0     3311 2022-11-12 19:01:21.974165 mousebender-2023.0.0/tests/data/simple/archive_links.aicoe-tensorflow.html
+-rw-r--r--   0        0        0    54889 2020-04-11 19:50:46.780940 mousebender-2023.0.0/tests/data/simple/archive_links.numpy-piwheels.html
+-rw-r--r--   0        0        0   481602 2020-04-08 02:48:29.052274 mousebender-2023.0.0/tests/data/simple/archive_links.numpy.html
+-rw-r--r--   0        0        0   111268 2020-04-08 02:48:29.053799 mousebender-2023.0.0/tests/data/simple/archive_links.pulpcore-client.html
+-rw-r--r--   0        0        0    62098 2020-04-08 02:48:29.054681 mousebender-2023.0.0/tests/data/simple/archive_links.pytorch.html
+-rw-r--r--   0        0        0 10847162 2020-04-11 19:50:46.847943 mousebender-2023.0.0/tests/data/simple/index.piwheels.html
+-rw-r--r--   0        0        0 11451535 2020-04-08 02:48:29.135841 mousebender-2023.0.0/tests/data/simple/index.pypi.html
+-rw-r--r--   0        0        0    18031 2023-04-12 00:37:01.072236 mousebender-2023.0.0/tests/test_simple.py
+-rw-r--r--   0        0        0     3178 1970-01-01 00:00:00.000000 mousebender-2023.0.0/PKG-INFO
```

### Comparing `mousebender-2022.1.0/.github/workflows/ci.yml` & `mousebender-2023.0.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `mousebender-2022.1.0/.github/workflows/pr-labels.yml` & `mousebender-2023.0.0/.github/workflows/pr-labels.yml`

 * *Files 1% similar despite different names*

```diff
@@ -14,12 +14,12 @@
 
 jobs:
   classify:
     name: "Classify PR"
     runs-on: ubuntu-latest
     steps:
       - name: "PR impact specified"
-        uses: mheap/github-action-required-labels@v2
+        uses: mheap/github-action-required-labels@v4
         with:
           mode: exactly
           count: 1
           labels: "impact-breaking, impact-feature, impact-bug, impact-project"
```

### Comparing `mousebender-2022.1.0/.gitignore` & `mousebender-2023.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mousebender-2022.1.0/.readthedocs.yaml` & `mousebender-2023.0.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `mousebender-2022.1.0/LICENSE` & `mousebender-2023.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mousebender-2022.1.0/README.md` & `mousebender-2023.0.0/README.md`

 * *Files identical despite different names*

### Comparing `mousebender-2022.1.0/docs/Makefile` & `mousebender-2023.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mousebender-2022.1.0/docs/conf.py` & `mousebender-2023.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mousebender-2022.1.0/docs/make.bat` & `mousebender-2023.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mousebender-2022.1.0/docs/simple.rst` & `mousebender-2023.0.0/docs/simple.rst`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,23 @@
 
    .. versionadded:: 2022.1.0
 
 .. autodata:: ACCEPT_SUPPORTED
 
    .. versionadded:: 2022.1.0
 
+.. autoexception:: UnsupportedAPIVersion
+
+   .. versionadded:: 2023.0.0
+
+
+.. autoexception:: APIVersionWarning
+
+   .. versionadded:: 2023.0.0
+
 .. autoexception:: UnsupportedMIMEType
 
    .. versionadded:: 2022.1.0
 
 .. autodata:: ProjectIndex_1_0
    :no-value:
```

### Comparing `mousebender-2022.1.0/mousebender/simple.py` & `mousebender-2023.0.0/mousebender/simple.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """Utilities to help with Simple repository API responses.
 
 This module helps with the JSON-based Simple repository API by providing
 :class:`~typing.TypedDict` definitions for API responses. For HTML-based
 responses, functions are provided to convert the HTML to the equivalent JSON
 response.
 
-This module implements :pep:`503`, :pep:`592`, :pep:`658`, and :pep:`691` of the
-:external:ref:`Simple repository API <simple-repository-api>` (it forgoes
-:pep:`629` as :pep:`691` makes it obsolete).
+This module implements :pep:`503`, :pep:`592`, :pep:`629`, :pep:`658`,
+:pep:`691`, and :pep:`700` of the
+:external:ref:`Simple repository API <simple-repository-api>`.
 
 """
 from __future__ import annotations
 
 import html
 import html.parser
 import json
 import urllib.parse
+import warnings
 from typing import Any, Dict, List, Optional, Union
 
-import packaging.specifiers
 import packaging.utils
 
 # Python 3.8+ only.
 from typing_extensions import Literal, TypeAlias, TypedDict
 
 ACCEPT_JSON_LATEST = "application/vnd.pypi.simple.latest+json"
 """The ``Accept`` header value for the latest version of the JSON API.
@@ -44,14 +44,30 @@
         f"{_ACCEPT_HTML_VALUES[1]};q=0.01",
     ]
 )
 """The ``Accept`` header for the MIME types that :func:`parse_project_index` and
 :func:`parse_project_details` support."""
 
 
+class UnsupportedAPIVersion(Exception):
+    """The major version of an API response is not supported."""
+
+    def __init__(self, version: str) -> None:
+        """Initialize the exception with a message based on the provided version."""
+        super().__init__(f"Unsupported API major version: {version!r}")
+
+
+class APIVersionWarning(Warning):
+    """The minor version of an API response is not supported."""
+
+    def __init__(self, version: str) -> None:
+        """Initialize the warning with a message based on the provided version."""
+        super().__init__(f"Unsupported API minor version: {version!r}")
+
+
 class UnsupportedMIMEType(Exception):
     """An unsupported MIME type was provided in a ``Content-Type`` header."""
 
 
 _Meta_1_0 = TypedDict("_Meta_1_0", {"api-version": Literal["1.0"]})
 _Meta_1_1 = TypedDict("_Meta_1_1", {"api-version": Literal["1.1"]})
 
@@ -136,27 +152,43 @@
     # PEP 700
     versions: List[str]
 
 
 ProjectDetails: TypeAlias = Union[ProjectDetails_1_0, ProjectDetails_1_1]
 
 
+def _check_version(tag: str, attrs: Dict[str, Optional[str]]) -> None:
+    if (
+        tag == "meta"
+        and attrs.get("name") == "pypi:repository-version"
+        and "content" in attrs
+        and attrs["content"]
+    ):
+        version = attrs["content"]
+        major_version, minor_version = map(int, version.split("."))
+        if major_version != 1:
+            raise UnsupportedAPIVersion(version)
+        elif minor_version > 1:
+            warnings.warn(APIVersionWarning(version), stacklevel=7)
+
+
 class _SimpleIndexHTMLParser(html.parser.HTMLParser):
     # PEP 503:
     # Within a repository, the root URL (/) MUST be a valid HTML5 page with a
     # single anchor element per project in the repository.
 
     def __init__(self) -> None:
         super().__init__()
         self._parsing_anchor = False
         self.names: List[str] = []
 
     def handle_starttag(
-        self, tag: str, _attrs_list: list[tuple[str, Optional[str]]]
+        self, tag: str, attrs_list: list[tuple[str, Optional[str]]]
     ) -> None:
+        _check_version(tag, dict(attrs_list))
         if tag != "a":
             return
         self._parsing_anchor = True
 
     def handle_endtag(self, tag: str) -> None:
         if tag != "a":
             return
@@ -183,14 +215,15 @@
         self.archive_links: List[Dict[str, Any]] = []
         super().__init__()
 
     def handle_starttag(
         self, tag: str, attrs_list: list[tuple[str, Optional[str]]]
     ) -> None:
         attrs = dict(attrs_list)
+        _check_version(tag, attrs)
         if tag != "a":
             return
         # PEP 503:
         # The href attribute MUST be a URL that links to the location of the
         # file for download ...
         if "href" not in attrs or not attrs["href"]:
             return
```

### Comparing `mousebender-2022.1.0/noxfile.py` & `mousebender-2023.0.0/noxfile.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Developer-related actions.
 
 All sessions prefixed with `check_` are non-destructive.
 
 """
-import nox
+import nox  # type: ignore[import]
 
 python_versions = ["3.7", "3.8", "3.9", "3.10", "3.11"]
 
 
 @nox.session(python=python_versions)
 def test(session, coverage=False):
     """Run the test suite."""
```

### Comparing `mousebender-2022.1.0/pyproject.toml` & `mousebender-2023.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 
 [project]
 name = "mousebender"
-version = "2022.1.0"
+version = "2023.0.0"
 authors = [
     { name = "Brett Cannon", email = "brett@python.org" },
     { name = "Derek Keeler", email = "derek@suchcool.ca" },
 ]
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
@@ -50,14 +50,14 @@
 run.branch = true
 report.fail_under = 100
 
 [tool.isort]
 profile = "black"
 
 [tool.ruff]
-select = ["E", "F", "W", "D", "C", "B", "A", "ANN", "RUF", "I"]
+select = ["E", "F", "W", "D", "B", "A", "ANN", "RUF", "I"]
 ignore = ["E501", "D203", "D213", "ANN101"]
 
 [tool.ruff.per-file-ignores]
 "tests/*" = ["D", "ANN"]
 "noxfile.py" = ["ANN", "A001"]
 "docs/conf.py" = ["D100"]
```

### Comparing `mousebender-2022.1.0/tests/data/simple/archive_links.aicoe-tensorflow.html` & `mousebender-2023.0.0/tests/data/simple/archive_links.aicoe-tensorflow.html`

 * *Files identical despite different names*

### Comparing `mousebender-2022.1.0/tests/data/simple/archive_links.numpy-piwheels.html` & `mousebender-2023.0.0/tests/data/simple/archive_links.numpy-piwheels.html`

 * *Files identical despite different names*

### Comparing `mousebender-2022.1.0/tests/data/simple/archive_links.numpy.html` & `mousebender-2023.0.0/tests/data/simple/archive_links.numpy.html`

 * *Files identical despite different names*

### Comparing `mousebender-2022.1.0/tests/data/simple/archive_links.pulpcore-client.html` & `mousebender-2023.0.0/tests/data/simple/archive_links.pulpcore-client.html`

 * *Files identical despite different names*

### Comparing `mousebender-2022.1.0/tests/data/simple/archive_links.pytorch.html` & `mousebender-2023.0.0/tests/data/simple/archive_links.pytorch.html`

 * *Files identical despite different names*

### Comparing `mousebender-2022.1.0/tests/data/simple/index.piwheels.html` & `mousebender-2023.0.0/tests/data/simple/index.piwheels.html`

 * *Files identical despite different names*

### Comparing `mousebender-2022.1.0/tests/data/simple/index.pypi.html` & `mousebender-2023.0.0/tests/data/simple/index.pypi.html`

 * *Files identical despite different names*

### Comparing `mousebender-2022.1.0/tests/test_simple.py` & `mousebender-2023.0.0/tests/test_simple.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Tests for mousebender.simple."""
 import json
+import warnings
 from typing import Dict, Union
 
 import importlib_resources
 import pytest
 
 from mousebender import simple
 
@@ -327,14 +328,63 @@
     )
     def test_yanked(self, html: str, expected: Union[bool, None]):
         details = simple.from_project_details_html(html, "test_yanked")
         assert len(details["files"]) == 1
         assert details["files"][0].get("yanked") == expected
 
 
+class TestPEP629Versioning:
+    @pytest.mark.parametrize(["version"], [("",), ("1.0",), ("1.1",)])
+    def test_supported_versions(self, version):
+        if not version:
+            meta_tag = ""
+        else:
+            meta_tag = f'<meta name="pypi:repository-version" content="{version}">'
+
+        index_html = (
+            f"<!DOCTYPE html><html><head>{meta_tag}</head>"
+            '<body><a href="/spamspamspam/">spamspamspam</a></body></html>'
+        )
+
+        assert simple.from_project_index_html(index_html)
+
+        details_html = (
+            f"<!DOCTYPE html><html><head>{meta_tag}</head>"
+            '<body><a href="mousebender-2022.1.0-py3-none-any.whl">'
+            "mousebender-2022.1.0-py3-none-any.whl/a></body></html>"
+        )
+
+        assert simple.from_project_details_html(details_html, "mousebender")
+
+    @pytest.mark.parametrize(["version"], [("0.1",), ("2.0",), ("2.1",), ("10.0",)])
+    def test_unsupported_major_versions(self, version):
+        meta_tag = f'<meta name="pypi:repository-version" content="{version}">'
+        index_html = (
+            f"<!DOCTYPE html><html><head>{meta_tag}</head>"
+            '<body><a href="/spamspamspam/">spamspamspam</a></body></html>'
+        )
+
+        with pytest.raises(simple.UnsupportedAPIVersion):
+            simple.from_project_index_html(index_html)
+
+    @pytest.mark.parametrize(["minor_version"], [("2",), ("10",)])
+    def test_unsupported_minor_version(self, minor_version):
+        meta_tag = f'<meta name="pypi:repository-version" content="1.{minor_version}">'
+        details_html = (
+            f"<!DOCTYPE html><html><head>{meta_tag}</head>"
+            '<body><a href="mousebender-2022.1.0-py3-none-any.whl">'
+            "mousebender-2022.1.0-py3-none-any.whl/a></body></html>"
+        )
+
+        with warnings.catch_warnings():
+            warnings.simplefilter("error")
+            with pytest.raises(simple.APIVersionWarning):
+                simple.from_project_details_html(details_html, "mousebender")
+
+
 class TestPEP658Metadata:
     def test_default(self):
         html = '<a href="spam-1.2.3-py3.none.any.whl">spam-1.2.3-py3.none.any.whl</a>'
         details = simple.from_project_details_html(html, "test_default")
         assert len(details["files"]) == 1
         # Need to make sure it isn't an empty dict.
         assert "dist-info-metadata" not in details["files"][0]
```

### Comparing `mousebender-2022.1.0/PKG-INFO` & `mousebender-2023.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mousebender
-Version: 2022.1.0
+Version: 2023.0.0
 Summary: A package for implementing various Python packaging standards.
 Keywords: packaging,Simple Repository API,PEP 503,PEP 592,PEP 658,PEP 691
 Author-email: Brett Cannon <brett@python.org>, Derek Keeler <derek@suchcool.ca>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: BSD License
```

