# Comparing `tmp/pip-licenses-4.2.0rc2.tar.gz` & `tmp/pip-licenses-4.2.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pip-licenses-4.2.0rc2.tar", last modified: Sat Apr  8 09:12:59 2023, max compression
+gzip compressed data, was "dist/pip-licenses-4.2.0rc3.tar", last modified: Wed Apr 12 10:00:41 2023, max compression
```

## Comparing `pip-licenses-4.2.0rc2.tar` & `pip-licenses-4.2.0rc3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 raimon49  (1000) raimon49  (1000)        0 2023-04-08 09:12:59.266600 pip-licenses-4.2.0rc2/
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)     5194 2023-04-08 09:11:29.000000 pip-licenses-4.2.0rc2/CHANGELOG.md
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)     1063 2020-12-06 15:11:59.000000 pip-licenses-4.2.0rc2/LICENSE
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)      129 2022-12-04 03:57:54.000000 pip-licenses-4.2.0rc2/MANIFEST.in
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)    30479 2023-04-08 09:12:59.266600 pip-licenses-4.2.0rc2/PKG-INFO
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)    21411 2023-04-08 09:10:15.000000 pip-licenses-4.2.0rc2/README.md
-drwxr-xr-x   0 raimon49  (1000) raimon49  (1000)        0 2023-04-08 09:12:59.266600 pip-licenses-4.2.0rc2/pip_licenses.egg-info/
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)    30479 2023-04-08 09:12:59.000000 pip-licenses-4.2.0rc2/pip_licenses.egg-info/PKG-INFO
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)      361 2023-04-08 09:12:59.000000 pip-licenses-4.2.0rc2/pip_licenses.egg-info/SOURCES.txt
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)        1 2023-04-08 09:12:59.000000 pip-licenses-4.2.0rc2/pip_licenses.egg-info/dependency_links.txt
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)       51 2023-04-08 09:12:59.000000 pip-licenses-4.2.0rc2/pip_licenses.egg-info/entry_points.txt
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)       85 2023-04-08 09:12:59.000000 pip-licenses-4.2.0rc2/pip_licenses.egg-info/requires.txt
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)       12 2023-04-08 09:12:59.000000 pip-licenses-4.2.0rc2/pip_licenses.egg-info/top_level.txt
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)    30973 2023-04-08 09:10:59.000000 pip-licenses-4.2.0rc2/piplicenses.py
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)        0 2022-12-04 03:57:54.000000 pip-licenses-4.2.0rc2/py.typed
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)     1367 2023-04-08 09:12:59.266600 pip-licenses-4.2.0rc2/setup.cfg
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)     2347 2022-12-04 03:57:54.000000 pip-licenses-4.2.0rc2/setup.py
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)    32569 2023-04-08 09:10:15.000000 pip-licenses-4.2.0rc2/test_piplicenses.py
-drwxr-xr-x   0 raimon49  (1000) raimon49  (1000)        0 2023-04-08 09:12:59.266600 pip-licenses-4.2.0rc2/tests/
-drwxr-xr-x   0 raimon49  (1000) raimon49  (1000)        0 2023-04-08 09:12:59.266600 pip-licenses-4.2.0rc2/tests/fixtures/
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)       16 2020-12-06 15:11:59.000000 pip-licenses-4.2.0rc2/tests/fixtures/unicode_characters.txt
+drwxr-xr-x   0 raimon49  (1000) raimon49  (1000)        0 2023-04-12 10:00:41.622574 pip-licenses-4.2.0rc3/
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)     5294 2023-04-12 09:58:29.000000 pip-licenses-4.2.0rc3/CHANGELOG.md
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)     1063 2020-12-06 15:11:59.000000 pip-licenses-4.2.0rc3/LICENSE
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)      129 2022-12-04 03:57:54.000000 pip-licenses-4.2.0rc3/MANIFEST.in
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)    30589 2023-04-12 10:00:41.622574 pip-licenses-4.2.0rc3/PKG-INFO
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)    21411 2023-04-12 09:58:26.000000 pip-licenses-4.2.0rc3/README.md
+drwxr-xr-x   0 raimon49  (1000) raimon49  (1000)        0 2023-04-12 10:00:41.622574 pip-licenses-4.2.0rc3/pip_licenses.egg-info/
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)    30589 2023-04-12 10:00:41.000000 pip-licenses-4.2.0rc3/pip_licenses.egg-info/PKG-INFO
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)      361 2023-04-12 10:00:41.000000 pip-licenses-4.2.0rc3/pip_licenses.egg-info/SOURCES.txt
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)        1 2023-04-12 10:00:41.000000 pip-licenses-4.2.0rc3/pip_licenses.egg-info/dependency_links.txt
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)       51 2023-04-12 10:00:41.000000 pip-licenses-4.2.0rc3/pip_licenses.egg-info/entry_points.txt
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)       85 2023-04-12 10:00:41.000000 pip-licenses-4.2.0rc3/pip_licenses.egg-info/requires.txt
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)       12 2023-04-12 10:00:41.000000 pip-licenses-4.2.0rc3/pip_licenses.egg-info/top_level.txt
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)    32432 2023-04-12 09:58:40.000000 pip-licenses-4.2.0rc3/piplicenses.py
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)        0 2022-12-04 03:57:54.000000 pip-licenses-4.2.0rc3/py.typed
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)     1367 2023-04-12 10:00:41.622574 pip-licenses-4.2.0rc3/setup.cfg
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)     2347 2022-12-04 03:57:54.000000 pip-licenses-4.2.0rc3/setup.py
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)    34122 2023-04-12 09:58:29.000000 pip-licenses-4.2.0rc3/test_piplicenses.py
+drwxr-xr-x   0 raimon49  (1000) raimon49  (1000)        0 2023-04-12 10:00:41.622574 pip-licenses-4.2.0rc3/tests/
+drwxr-xr-x   0 raimon49  (1000) raimon49  (1000)        0 2023-04-12 10:00:41.622574 pip-licenses-4.2.0rc3/tests/fixtures/
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)       16 2020-12-06 15:11:59.000000 pip-licenses-4.2.0rc3/tests/fixtures/unicode_characters.txt
```

### Comparing `pip-licenses-4.2.0rc2/CHANGELOG.md` & `pip-licenses-4.2.0rc3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 ### 4.2.0
 
 * Implement new option `--with-maintainers`
 * Implement new option `--python`
 * Allow version spec in `--ignore-packages` parameters
 * When the `Author` field is `UNKNOWN`, the output is automatically completed from `Author-email`
+* When the `home-page` field is `UNKNOWN`, the output is automatically completed from `Project-URL`
 
 ### 4.1.0
 
 * Support case-insensitive license name matching around `--fail-on` and `--allow-only` parameters
 
 ### 4.0.3
```

### Comparing `pip-licenses-4.2.0rc2/LICENSE` & `pip-licenses-4.2.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `pip-licenses-4.2.0rc2/PKG-INFO` & `pip-licenses-4.2.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-licenses
-Version: 4.2.0rc2
+Version: 4.2.0rc3
 Summary: Dump the software license list of Python packages installed with pip.
 Home-page: https://github.com/raimon49/pip-licenses
 Author: raimon
 Author-email: raimon49@hotmail.com
 License: MIT
 Project-URL: Releases, https://github.com/raimon49/pip-licenses/releases
 Project-URL: Issues, https://github.com/raimon49/pip-licenses/issues
@@ -821,14 +821,16 @@
 ~~~~~
 
 -  Implement new option ``--with-maintainers``
 -  Implement new option ``--python``
 -  Allow version spec in ``--ignore-packages`` parameters
 -  When the ``Author`` field is ``UNKNOWN``, the output is automatically
    completed from ``Author-email``
+-  When the ``home-page`` field is ``UNKNOWN``, the output is
+   automatically completed from ``Project-URL``
 
 .. _410:
 
 4.1.0
 ~~~~~
 
 -  Support case-insensitive license name matching around ``--fail-on``
```

### Comparing `pip-licenses-4.2.0rc2/README.md` & `pip-licenses-4.2.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `pip-licenses-4.2.0rc2/pip_licenses.egg-info/PKG-INFO` & `pip-licenses-4.2.0rc3/pip_licenses.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-licenses
-Version: 4.2.0rc2
+Version: 4.2.0rc3
 Summary: Dump the software license list of Python packages installed with pip.
 Home-page: https://github.com/raimon49/pip-licenses
 Author: raimon
 Author-email: raimon49@hotmail.com
 License: MIT
 Project-URL: Releases, https://github.com/raimon49/pip-licenses/releases
 Project-URL: Issues, https://github.com/raimon49/pip-licenses/issues
@@ -821,14 +821,16 @@
 ~~~~~
 
 -  Implement new option ``--with-maintainers``
 -  Implement new option ``--python``
 -  Allow version spec in ``--ignore-packages`` parameters
 -  When the ``Author`` field is ``UNKNOWN``, the output is automatically
    completed from ``Author-email``
+-  When the ``home-page`` field is ``UNKNOWN``, the output is
+   automatically completed from ``Project-URL``
 
 .. _410:
 
 4.1.0
 ~~~~~
 
 -  Support case-insensitive license name matching around ``--fail-on``
```

### Comparing `pip-licenses-4.2.0rc2/piplicenses.py` & `pip-licenses-4.2.0rc3/piplicenses.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,21 +45,22 @@
 from prettytable import ALL as RULE_ALL
 from prettytable import FRAME as RULE_FRAME
 from prettytable import HEADER as RULE_HEADER
 from prettytable import NONE as RULE_NONE
 from prettytable import PrettyTable
 
 if TYPE_CHECKING:
-    from typing import Iterator, Optional, Sequence
+    from email.message import Message
+    from typing import Callable, Dict, Iterator, Optional, Sequence
 
 
 open = open  # allow monkey patching
 
 __pkgname__ = "pip-licenses"
-__version__ = "4.2.0rc2"
+__version__ = "4.2.0rc3"
 __author__ = "raimon"
 __license__ = "MIT"
 __summary__ = (
     "Dump the software license list of Python packages installed with pip."
 )
 __url__ = "https://github.com/raimon49/pip-licenses"
 
@@ -92,20 +93,58 @@
 
 
 SUMMARY_OUTPUT_FIELDS = (
     "Count",
     "License",
 )
 
-METADATA_KEYS = {
-    "home-page": ["home-page"],
-    "author": ["author", "author-email"],
-    "maintainer": ["maintainer", "maintainer-email"],
-    "license": ["license"],
-    "summary": ["summary"],
+
+def extract_homepage(metadata: Message) -> Optional[str]:
+    """Extracts the homepage attribute from the package metadata.
+
+    Not all python packages have defined a home-page attribute.
+    As a fallback, the `Project-URL` metadata can be used.
+    The python core metadata supports multiple (free text) values for
+    the `Project-URL` field that are comma separated.
+
+    Args:
+        metadata: The package metadata to extract the homepage from.
+
+    Returns:
+        The home page if applicable, None otherwise.
+    """
+    homepage = metadata.get("home-page", None)
+    if homepage is not None:
+        return homepage
+
+    candidates: Dict[str, str] = {}
+
+    for entry in metadata.get_all("Project-URL", []):
+        key, value = entry.split(",", 1)
+        candidates[key.strip()] = value.strip()
+
+    for priority_key in ["Homepage", "Source", "Changelog", "Bug Tracker"]:
+        if priority_key in candidates:
+            return candidates[priority_key]
+
+    return None
+
+
+METADATA_KEYS: Dict[str, List[Callable[[Message], Optional[str]]]] = {
+    "home-page": [extract_homepage],
+    "author": [
+        lambda metadata: metadata.get("author"),
+        lambda metadata: metadata.get("author-email"),
+    ],
+    "maintainer": [
+        lambda metadata: metadata.get("maintainer"),
+        lambda metadata: metadata.get("maintainer-email"),
+    ],
+    "license": [lambda metadata: metadata.get("license")],
+    "summary": [lambda metadata: metadata.get("summary")],
 }
 
 # Mapping of FIELD_NAMES to METADATA_KEYS where they differ by more than case
 FIELDS_TO_METADATA_KEYS = {
     "URL": "home-page",
     "Description": "summary",
     "License-Metadata": "license",
@@ -166,18 +205,20 @@
             "namever": "{} {}".format(pkg.metadata["name"], pkg.version),
             "licensefile": license_file,
             "licensetext": license_text,
             "noticefile": notice_file,
             "noticetext": notice_text,
         }
         metadata = pkg.metadata
-        for field_name, field_selectors in METADATA_KEYS.items():
+        for field_name, field_selector_fns in METADATA_KEYS.items():
             value = None
-            for selector in field_selectors:
-                value = metadata.get(selector, None)  # type: ignore[attr-defined] # noqa: E501
+            for field_selector_fn in field_selector_fns:
+                # Type hint of `Distribution.metadata` states `PackageMetadata`
+                # but it's actually of type `email.Message`
+                value = field_selector_fn(metadata)  # type: ignore
                 if value:
                     break
             pkg_info[field_name] = value or LICENSE_UNKNOWN
 
         classifiers: list[str] = metadata.get_all("classifier", [])
         pkg_info["license_classifier"] = find_license_from_classifier(
             classifiers
```

### Comparing `pip-licenses-4.2.0rc2/setup.cfg` & `pip-licenses-4.2.0rc3/setup.cfg`

 * *Files identical despite different names*

### Comparing `pip-licenses-4.2.0rc2/setup.py` & `pip-licenses-4.2.0rc3/setup.py`

 * *Files identical despite different names*

### Comparing `pip-licenses-4.2.0rc2/test_piplicenses.py` & `pip-licenses-4.2.0rc3/test_piplicenses.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import sys
 import unittest
 import venv
 from enum import Enum, auto
 from importlib.metadata import Distribution
 from types import SimpleNamespace
 from typing import TYPE_CHECKING, Any, List
+from unittest.mock import MagicMock
 
 import docutils.frontend
 import docutils.parsers.rst
 import docutils.utils
 import pytest
 from _pytest.capture import CaptureFixture
 
@@ -35,14 +36,15 @@
     case_insensitive_set_diff,
     case_insensitive_set_intersect,
     create_licenses_table,
     create_output_string,
     create_parser,
     create_warn_string,
     enum_key_to_value,
+    extract_homepage,
     factory_styled_table_with_args,
     find_license_from_classifier,
     get_output_fields,
     get_packages,
     get_sortby,
     output_colored,
     save_if_needs,
@@ -901,7 +903,60 @@
 
     # invalid code-page
     with pytest.raises(SystemExit) as ex:
         parser.parse_args(["--filter-strings", "--filter-code-page=XX"])
     capture = capsys.readouterr().err
     for arg in ("invalid code", "--filter-code-page"):
         assert arg in capture
+
+
+def test_extract_homepage_home_page_set() -> None:
+    metadata = MagicMock()
+    metadata.get.return_value = "Foobar"
+
+    assert "Foobar" == extract_homepage(metadata=metadata)  # type: ignore
+
+    metadata.get.assert_called_once_with("home-page", None)
+
+
+def test_extract_homepage_project_url_fallback() -> None:
+    metadata = MagicMock()
+    metadata.get.return_value = None
+
+    # `Homepage` is prioritized higher than `Source`
+    metadata.get_all.return_value = [
+        "Source, source",
+        "Homepage, homepage",
+    ]
+
+    assert "homepage" == extract_homepage(metadata=metadata)  # type: ignore
+
+    metadata.get_all.assert_called_once_with("Project-URL", [])
+
+
+def test_extract_homepage_project_url_fallback_multiple_parts() -> None:
+    metadata = MagicMock()
+    metadata.get.return_value = None
+
+    # `Homepage` is prioritized higher than `Source`
+    metadata.get_all.return_value = [
+        "Source, source",
+        "Homepage, homepage, foo, bar",
+    ]
+
+    assert "homepage, foo, bar" == extract_homepage(
+        metadata=metadata  # type: ignore
+    )
+
+    metadata.get_all.assert_called_once_with("Project-URL", [])
+
+
+def test_extract_homepage_empty() -> None:
+    metadata = MagicMock()
+
+    metadata.get.return_value = None
+    metadata.get_all.return_value = []
+
+    assert None is extract_homepage(metadata=metadata)  # type: ignore
+
+    metadata.get.assert_called_once_with("home-page", None)
+    metadata.get_all.assert_called_once_with("Project-URL", [])
```

