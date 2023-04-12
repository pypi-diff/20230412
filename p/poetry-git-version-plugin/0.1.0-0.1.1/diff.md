# Comparing `tmp/poetry_git_version_plugin-0.1.0.tar.gz` & `tmp/poetry_git_version_plugin-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_git_version_plugin-0.1.0.tar", max compression
+gzip compressed data, was "poetry_git_version_plugin-0.1.1.tar", max compression
```

## Comparing `poetry_git_version_plugin-0.1.0.tar` & `poetry_git_version_plugin-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1055 2023-04-11 18:46:05.120987 poetry_git_version_plugin-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2023-04-11 20:05:16.315553 poetry_git_version_plugin-0.1.0/poetry_git_version_plugin/__init__.py
--rw-r--r--   0        0        0      310 2023-04-11 18:46:05.120987 poetry_git_version_plugin-0.1.0/poetry_git_version_plugin/commands.py
--rw-r--r--   0        0        0      902 2023-04-11 18:46:05.120987 poetry_git_version_plugin-0.1.0/poetry_git_version_plugin/config.py
--rw-r--r--   0        0        0      781 2023-04-11 18:46:05.120987 poetry_git_version_plugin-0.1.0/poetry_git_version_plugin/exceptions.py
--rw-r--r--   0        0        0     1535 2023-04-11 18:46:05.120987 poetry_git_version_plugin-0.1.0/poetry_git_version_plugin/plugins.py
--rw-r--r--   0        0        0     4295 2023-04-11 19:50:25.454388 poetry_git_version_plugin-0.1.0/poetry_git_version_plugin/services.py
--rw-r--r--   0        0        0     2172 2023-04-11 18:46:05.120987 poetry_git_version_plugin-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1075 2023-04-11 19:15:37.049099 poetry_git_version_plugin-0.1.0/readme.md
--rw-r--r--   0        0        0     2721 1970-01-01 00:00:00.000000 poetry_git_version_plugin-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-04-11 19:28:21.273926 poetry_git_version_plugin-0.1.1/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-12 18:36:34.455778 poetry_git_version_plugin-0.1.1/poetry_git_version_plugin/__init__.py
+-rw-r--r--   0        0        0      310 2023-04-11 19:28:21.273926 poetry_git_version_plugin-0.1.1/poetry_git_version_plugin/commands.py
+-rw-r--r--   0        0        0     1002 2023-04-12 18:36:34.375778 poetry_git_version_plugin-0.1.1/poetry_git_version_plugin/config.py
+-rw-r--r--   0        0        0      781 2023-04-11 19:28:21.273926 poetry_git_version_plugin-0.1.1/poetry_git_version_plugin/exceptions.py
+-rw-r--r--   0        0        0     1535 2023-04-11 19:28:21.273926 poetry_git_version_plugin-0.1.1/poetry_git_version_plugin/plugins.py
+-rw-r--r--   0        0        0     4295 2023-04-12 18:36:34.375778 poetry_git_version_plugin-0.1.1/poetry_git_version_plugin/services.py
+-rw-r--r--   0        0        0     2172 2023-04-11 19:28:21.273926 poetry_git_version_plugin-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1075 2023-04-11 19:28:21.273926 poetry_git_version_plugin-0.1.1/readme.md
+-rw-r--r--   0        0        0     2721 1970-01-01 00:00:00.000000 poetry_git_version_plugin-0.1.1/PKG-INFO
```

### Comparing `poetry_git_version_plugin-0.1.0/LICENSE` & `poetry_git_version_plugin-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.0/poetry_git_version_plugin/config.py` & `poetry_git_version_plugin-0.1.1/poetry_git_version_plugin/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from copy import deepcopy
+
 from poetry.core.pyproject.toml import PyProjectTOML
 
 PLUGIN_NAME = 'poetry-git-version-plugin'
 
 
 class PluginConfig(object):
     """Обертка над конфигурацией pyproject"""
@@ -17,15 +19,17 @@
 
     def __init__(self, pyproject: PyProjectTOML) -> None:
         self.pyproject = pyproject
 
     @property
     def settings(self):
         settings = self.pyproject.data.get('tool', {}).get(PLUGIN_NAME, {})
-        return self._default_setting | settings
+        new_settings = deepcopy(self._default_setting)
+        new_settings.update(settings)
+        return new_settings
 
     @property
     def ignore_exception(self) -> bool:
         return self.settings['ignore_exception']
 
     @property
     def use_last_tag(self) -> bool:
```

### Comparing `poetry_git_version_plugin-0.1.0/poetry_git_version_plugin/exceptions.py` & `poetry_git_version_plugin-0.1.1/poetry_git_version_plugin/exceptions.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.0/poetry_git_version_plugin/plugins.py` & `poetry_git_version_plugin-0.1.1/poetry_git_version_plugin/plugins.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.0/poetry_git_version_plugin/services.py` & `poetry_git_version_plugin-0.1.1/poetry_git_version_plugin/services.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.0/pyproject.toml` & `poetry_git_version_plugin-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.0/readme.md` & `poetry_git_version_plugin-0.1.1/readme.md`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.0/PKG-INFO` & `poetry_git_version_plugin-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-git-version-plugin
-Version: 0.1.0
+Version: 0.1.1
 Summary: Poetry plugin to get package version from git
 Home-page: https://gitlab.com/rocshers/python/poetry-git-version-plugin
 License: MIT
 Author: irocshers
 Author-email: develop.iam@rocshers.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
```

