# Comparing `tmp/tansy-0.6.1.tar.gz` & `tmp/tansy-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tansy-0.6.1.tar", last modified: Mon Apr 10 19:58:43 2023, max compression
+gzip compressed data, was "tansy-0.7.0.tar", last modified: Wed Apr 12 16:42:27 2023, max compression
```

## Comparing `tansy-0.6.1.tar` & `tansy-0.7.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:58:43.764072 tansy-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-10 19:58:30.000000 tansy-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-10 19:58:43.764072 tansy-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-10 19:58:30.000000 tansy-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-10 19:58:30.000000 tansy-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 19:58:43.764072 tansy-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-10 19:58:30.000000 tansy-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:58:43.764072 tansy-0.6.1/tansy/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-10 19:58:30.000000 tansy-0.6.1/tansy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10728 2023-04-10 19:58:30.000000 tansy-0.6.1/tansy/class_slash.py
--rw-r--r--   0 runner    (1001) docker     (123)    20405 2023-04-10 19:58:30.000000 tansy-0.6.1/tansy/slash_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-04-10 19:58:30.000000 tansy-0.6.1/tansy/slash_param.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-10 19:58:30.000000 tansy-0.6.1/tansy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:58:43.764072 tansy-0.6.1/tansy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-10 19:58:43.000000 tansy-0.6.1/tansy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-10 19:58:43.000000 tansy-0.6.1/tansy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:58:43.000000 tansy-0.6.1/tansy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-10 19:58:43.000000 tansy-0.6.1/tansy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 19:58:43.000000 tansy-0.6.1/tansy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:42:27.825065 tansy-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-12 16:42:12.000000 tansy-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-12 16:42:27.821066 tansy-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-12 16:42:12.000000 tansy-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-12 16:42:12.000000 tansy-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 16:42:27.825065 tansy-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-12 16:42:12.000000 tansy-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:42:27.821066 tansy-0.7.0/tansy/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-12 16:42:12.000000 tansy-0.7.0/tansy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10728 2023-04-12 16:42:12.000000 tansy-0.7.0/tansy/class_slash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20796 2023-04-12 16:42:12.000000 tansy-0.7.0/tansy/slash_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-04-12 16:42:12.000000 tansy-0.7.0/tansy/slash_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-12 16:42:12.000000 tansy-0.7.0/tansy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:42:27.821066 tansy-0.7.0/tansy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-12 16:42:27.000000 tansy-0.7.0/tansy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-12 16:42:27.000000 tansy-0.7.0/tansy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:42:27.000000 tansy-0.7.0/tansy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-12 16:42:27.000000 tansy-0.7.0/tansy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 16:42:27.000000 tansy-0.7.0/tansy.egg-info/top_level.txt
```

### Comparing `tansy-0.6.1/LICENSE` & `tansy-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tansy-0.6.1/PKG-INFO` & `tansy-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tansy
-Version: 0.6.1
+Version: 0.7.0
 Summary: Unstable experiments with interactions.py.
 Home-page: https://github.com/Astrea49/tansy
 Author: AstreaTSS
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `tansy-0.6.1/README.md` & `tansy-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `tansy-0.6.1/setup.py` & `tansy-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 setup(
     name="tansy",
     description="Unstable experiments with interactions.py.",
     long_description=(Path(__file__).parent / "README.md").read_text(),
     long_description_content_type="text/markdown",
     author="AstreaTSS",
     url="https://github.com/Astrea49/tansy",
-    version="0.6.1",
+    version="0.7.0",
     packages=find_packages(),
     python_requires=">=3.10",
     install_requires=requirements,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `tansy-0.6.1/tansy/__init__.py` & `tansy-0.7.0/tansy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Tansy
 Unstable experiments with interactions.py.
 :copyright: (c) 2022-present AstreaTSS
 :license: MIT, see LICENSE for more details.
 """
 
-__version__ = "0.6.1"
+__version__ = "0.7.0"
 
 
 from .class_slash import *
 from .slash_commands import *
 from .slash_param import *
 
 __all__ = (
```

### Comparing `tansy-0.6.1/tansy/class_slash.py` & `tansy-0.7.0/tansy/class_slash.py`

 * *Files identical despite different names*

### Comparing `tansy-0.6.1/tansy/slash_commands.py` & `tansy-0.7.0/tansy/slash_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,57 +350,59 @@
     ) -> "TansySlashCommand":
         return TansySlashCommand(
             name=self.name,
             description=self.description,
             group_name=name,
             group_description=description,
             scopes=self.scopes,
-            checks=self.checks if inherit_checks else [],
+            checks=self.checks.copy() if inherit_checks else [],
         )
 
     def subcommand(
         self,
-        sub_cmd_name: ipy.LocalisedName | str,
+        sub_cmd_name: ipy.Absent[ipy.LocalisedName | str] = ipy.MISSING,
         group_name: ipy.LocalisedName | str = None,
         sub_cmd_description: ipy.Absent[ipy.LocalisedDesc | str] = ipy.MISSING,
         group_description: ipy.Absent[ipy.LocalisedDesc | str] = ipy.MISSING,
         nsfw: bool = False,
         inherit_checks: bool = True,
     ) -> typing.Callable[..., "TansySlashCommand"]:
         def wrapper(
             call: typing.Callable[..., typing.Coroutine]
         ) -> "TansySlashCommand":
-            nonlocal sub_cmd_description
+            nonlocal sub_cmd_name, sub_cmd_description
 
             if not asyncio.iscoroutinefunction(call):
                 raise TypeError("Subcommand must be coroutine")
 
             if sub_cmd_description is ipy.MISSING:
                 sub_cmd_description = call.__doc__ or "No Description Set"
+            if sub_cmd_name is ipy.MISSING:
+                sub_cmd_name = call.__name__
 
             return TansySlashCommand(
                 name=self.name,
                 description=self.description,
                 group_name=group_name or self.group_name,
                 group_description=group_description or self.group_description,
                 sub_cmd_name=sub_cmd_name,
                 sub_cmd_description=sub_cmd_description,
                 default_member_permissions=self.default_member_permissions,
                 dm_permission=self.dm_permission,
                 callback=call,
                 scopes=self.scopes,
                 nsfw=nsfw,
-                checks=self.checks if inherit_checks else [],
+                checks=self.checks.copy() if inherit_checks else [],
             )
 
         return wrapper
 
 
 def tansy_slash_command(
-    name: str | ipy.LocalisedName,
+    name: ipy.Absent[str | ipy.LocalisedName] = ipy.MISSING,
     *,
     description: ipy.Absent[str | ipy.LocalisedDesc] = ipy.MISSING,
     scopes: ipy.Absent[typing.List["ipy.Snowflake_Type"]] = ipy.MISSING,
     default_member_permissions: typing.Optional["ipy.Permissions"] = None,
     dm_permission: bool = True,
     sub_cmd_name: str | ipy.LocalisedName = None,
     group_name: str | ipy.LocalisedName = None,
@@ -411,15 +413,15 @@
     """
     A decorator to declare a coroutine as a Tansy slash command.
     note:
         While the base and group descriptions arent visible in the discord client, currently.
         We strongly advise defining them anyway, if you're using subcommands, as Discord has said they will be visible in
         one of the future ui updates.
     Args:
-        name: 1-32 character name of the command
+        name: 1-32 character name of the command, defaults to the name of the coroutine.
         description: 1-100 character description of the command
         scopes: The scope this command exists within
         default_member_permissions: What permissions members need to have by default to use this command.
         dm_permission: Should this command be available in DMs.
         sub_cmd_name: 1-32 character name of the subcommand
         sub_cmd_description: 1-100 character description of the subcommand
         group_name: 1-32 character name of the group
@@ -436,20 +438,24 @@
         perm = default_member_permissions
         if hasattr(func, "default_member_permissions"):
             if perm:
                 perm = perm | func.default_member_permissions
             else:
                 perm = func.default_member_permissions
 
+        _name = name
+        if _name is ipy.MISSING:
+            _name = func.__name__
+
         _description = description
         if _description is ipy.MISSING:
             _description = func.__doc__ or "No Description Set"
 
         return TansySlashCommand(
-            name=name,
+            name=_name,
             group_name=group_name,
             group_description=group_description,
             sub_cmd_name=sub_cmd_name,
             sub_cmd_description=sub_cmd_description,
             description=_description,
             scopes=scopes or [ipy.const.GLOBAL_SCOPE],
             default_member_permissions=perm,
@@ -461,15 +467,15 @@
     return wrapper
 
 
 def tansy_subcommand(
     base: str | ipy.LocalisedName,
     *,
     subcommand_group: typing.Optional[str | ipy.LocalisedName] = None,
-    name: typing.Optional[str | ipy.LocalisedName] = None,
+    name: ipy.Absent[str | ipy.LocalisedName] = ipy.MISSING,
     description: ipy.Absent[str | ipy.LocalisedDesc] = ipy.MISSING,
     base_description: typing.Optional[str | ipy.LocalisedDesc] = None,
     base_desc: typing.Optional[str | ipy.LocalisedDesc] = None,
     base_default_member_permissions: typing.Optional["ipy.Permissions"] = None,
     base_dm_permission: bool = True,
     subcommand_group_description: typing.Optional[str | ipy.LocalisedDesc] = None,
     sub_group_desc: typing.Optional[str | ipy.LocalisedDesc] = None,
@@ -495,25 +501,29 @@
         A SlashCommand object
     """
 
     def wrapper(func: ipy.const.AsyncCallable) -> TansySlashCommand:
         if not asyncio.iscoroutinefunction(func):
             raise ValueError("Commands must be coroutines")
 
+        _name = name
+        if _name is ipy.MISSING:
+            _name = func.__name__
+
         _description = description
         if _description is ipy.MISSING:
             _description = func.__doc__ or "No Description Set"
 
         cmd = TansySlashCommand(
             name=base,
             description=(base_description or base_desc) or "No Description Set",
             group_name=subcommand_group,
             group_description=(subcommand_group_description or sub_group_desc)
             or "No Description Set",
-            sub_cmd_name=name,
+            sub_cmd_name=_name,
             sub_cmd_description=_description,
             default_member_permissions=base_default_member_permissions,
             dm_permission=base_dm_permission,
             scopes=scopes or [ipy.const.GLOBAL_SCOPE],
             callback=func,
             nsfw=nsfw,
         )
```

### Comparing `tansy-0.6.1/tansy/slash_param.py` & `tansy-0.7.0/tansy/slash_param.py`

 * *Files identical despite different names*

### Comparing `tansy-0.6.1/tansy/utils.py` & `tansy-0.7.0/tansy/utils.py`

 * *Files identical despite different names*

### Comparing `tansy-0.6.1/tansy.egg-info/PKG-INFO` & `tansy-0.7.0/tansy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tansy
-Version: 0.6.1
+Version: 0.7.0
 Summary: Unstable experiments with interactions.py.
 Home-page: https://github.com/Astrea49/tansy
 Author: AstreaTSS
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

