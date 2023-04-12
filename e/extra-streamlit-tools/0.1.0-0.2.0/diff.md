# Comparing `tmp/extra_streamlit_tools-0.1.0.tar.gz` & `tmp/extra_streamlit_tools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extra_streamlit_tools-0.1.0.tar", max compression
+gzip compressed data, was "extra_streamlit_tools-0.2.0.tar", max compression
```

## Comparing `extra_streamlit_tools-0.1.0.tar` & `extra_streamlit_tools-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1077 2023-03-20 07:33:58.740715 extra_streamlit_tools-0.1.0/LICENSE
--rw-r--r--   0        0        0      654 2023-03-20 12:42:23.746955 extra_streamlit_tools-0.1.0/README.md
--rw-r--r--   0        0        0     1075 2023-03-20 12:21:48.076093 extra_streamlit_tools-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-20 07:33:58.742335 extra_streamlit_tools-0.1.0/src/extra_streamlit_tools/__init__.py
--rw-r--r--   0        0        0       93 2023-03-20 11:33:29.569450 extra_streamlit_tools-0.1.0/src/extra_streamlit_tools/_logging.py
--rw-r--r--   0        0        0     4622 2023-03-20 11:33:40.042651 extra_streamlit_tools-0.1.0/src/extra_streamlit_tools/data.py
--rw-r--r--   0        0        0     2037 2023-03-20 11:31:46.487254 extra_streamlit_tools-0.1.0/src/extra_streamlit_tools/utils.py
--rw-r--r--   0        0        0     1230 1970-01-01 00:00:00.000000 extra_streamlit_tools-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-03-20 07:33:58.740715 extra_streamlit_tools-0.2.0/LICENSE
+-rw-r--r--   0        0        0      762 2023-04-12 13:14:02.816930 extra_streamlit_tools-0.2.0/README.md
+-rw-r--r--   0        0        0     1075 2023-04-12 13:14:02.822586 extra_streamlit_tools-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-12 13:14:02.822650 extra_streamlit_tools-0.2.0/src/extra_streamlit_tools/__init__.py
+-rw-r--r--   0        0        0       93 2023-04-12 13:14:02.822987 extra_streamlit_tools-0.2.0/src/extra_streamlit_tools/_logging.py
+-rw-r--r--   0        0        0     4622 2023-04-12 13:14:02.823402 extra_streamlit_tools-0.2.0/src/extra_streamlit_tools/data.py
+-rw-r--r--   0        0        0     2324 2023-04-12 13:14:02.823645 extra_streamlit_tools-0.2.0/src/extra_streamlit_tools/utils.py
+-rw-r--r--   0        0        0     1338 1970-01-01 00:00:00.000000 extra_streamlit_tools-0.2.0/PKG-INFO
```

### Comparing `extra_streamlit_tools-0.1.0/LICENSE` & `extra_streamlit_tools-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `extra_streamlit_tools-0.1.0/pyproject.toml` & `extra_streamlit_tools-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "extra-streamlit-tools"
-version = "0.1.0"
+version = "0.2.0"
 description = "Extra tools to use for streamlit applications"
 authors = ["Tomer Gabay <tomergabay001@gmail.com>"]
 readme = "README.md"
 packages = [{include = "extra_streamlit_tools", from = "src"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.9.7 || >3.9.7,<4.0"
```

### Comparing `extra_streamlit_tools-0.1.0/src/extra_streamlit_tools/data.py` & `extra_streamlit_tools-0.2.0/src/extra_streamlit_tools/data.py`

 * *Files identical despite different names*

### Comparing `extra_streamlit_tools-0.1.0/src/extra_streamlit_tools/utils.py` & `extra_streamlit_tools-0.2.0/src/extra_streamlit_tools/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 from extra_streamlit_tools._logging import logging as logger
 import streamlit as st
-from typing import Any
+from typing import Any, Optional
 
 
-def clear_cache() -> None:
+def clear_cache(keep_keys: Optional[list[str]] = None) -> None:
     """
     Resets the Streamlit cache.
+
+    Parameters
+    ----------
+        keep_keys:Optional[list[str]]
+            Keys to not be cleared from cache
     """
+
     logger.debug("Clearing cache")
     for key in st.session_state.keys():
-        logger.debug(f"Deleting key: {key}")
-        del st.session_state[key]
+        if keep_keys is None or key not in keep_keys:
+            logger.debug(f"Deleting key: {key}")
+            del st.session_state[key]
+        else:
+            logger.debug(f"Keeping key: {key}")
 
 
 def init_session_keys(key_value_pairs: dict[str, Any]) -> None:
     """
     The init_session_keys function is a helper function that initializes the session state with keys and values.
 
     Parameters
```

### Comparing `extra_streamlit_tools-0.1.0/PKG-INFO` & `extra_streamlit_tools-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extra-streamlit-tools
-Version: 0.1.0
+Version: 0.2.0
 Summary: Extra tools to use for streamlit applications
 Author: Tomer Gabay
 Author-email: tomergabay001@gmail.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -20,14 +20,16 @@
 
 ## Installation
 
 `pip install extra-streamlit-tools`
 
 ## Usage
 
+See [ReadTheDocs](https://extra-streamlit-tools.readthedocs.io/en/latest/) for its official documentation.
+
 ```
 import extra_streamlit_tools as est
 
 # for data related functions
 from est.data import ...
 
 # for e.g. cache related functions
```

