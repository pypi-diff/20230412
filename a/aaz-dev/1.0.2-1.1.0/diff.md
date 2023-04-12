# Comparing `tmp/aaz-dev-1.0.2.tar.gz` & `tmp/aaz-dev-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aaz-dev-1.0.2.tar", last modified: Mon Apr  3 10:46:07 2023, max compression
+gzip compressed data, was "aaz-dev-1.1.0.tar", last modified: Wed Apr 12 05:28:52 2023, max compression
```

## Comparing `aaz-dev-1.0.2.tar` & `aaz-dev-1.1.0.tar`

### file list

```diff
@@ -1,286 +1,286 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.963132 aaz-dev-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-04-03 10:46:07.963132 aaz-dev-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 10:46:07.963132 aaz-dev-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.879131 aaz-dev-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.891131 aaz-dev-1.0.2/src/aaz_dev/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.895131 aaz-dev-1.0.2/src/aaz_dev/app/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/app/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/app/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/app/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/app/url_converters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.895131 aaz-dev-1.0.2/src/aaz_dev/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.895131 aaz-dev-1.0.2/src/aaz_dev/cli/api/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/api/_cmds.py
--rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/api/az.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/api/portal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.895131 aaz-dev-1.0.2/src/aaz_dev/cli/controller/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17654 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/controller/az_arg_group_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/controller/az_atomic_profile_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    18759 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/controller/az_command_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    27518 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/controller/az_module_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    38350 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/controller/az_operation_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/controller/az_output_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/controller/az_profile_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/controller/az_selector_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19004 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/controller/portal_cli_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.899131 aaz-dev-1.0.2/src/aaz_dev/cli/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.899131 aaz-dev-1.0.2/src/aaz_dev/cli/model/atomic/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/model/atomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/model/atomic/_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/model/atomic/_command_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/model/atomic/_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/model/atomic/_help.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/model/atomic/_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/model/atomic/_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.899131 aaz-dev-1.0.2/src/aaz_dev/cli/model/common/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/model/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/model/common/_fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.903131 aaz-dev-1.0.2/src/aaz_dev/cli/model/view/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/model/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/model/view/_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/model/view/_command_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/model/view/_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/model/view/_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.903131 aaz-dev-1.0.2/src/aaz_dev/cli/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/templates/_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.903131 aaz-dev-1.0.2/src/aaz_dev/cli/templates/aaz/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/templates/aaz/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.903131 aaz-dev-1.0.2/src/aaz_dev/cli/templates/aaz/command/
--rw-r--r--   0 runner    (1001) docker     (123)    31616 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/templates/aaz/command/_cmd.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.903131 aaz-dev-1.0.2/src/aaz_dev/cli/templates/aaz/group/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/templates/aaz/group/__cmd_group.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/templates/aaz/group/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.903131 aaz-dev-1.0.2/src/aaz_dev/cli/templates/aaz/profile/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/templates/aaz/profile/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.903131 aaz-dev-1.0.2/src/aaz_dev/cli/templates/extension/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/templates/extension/HISTORY.rst.j2
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/templates/extension/README.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.907131 aaz-dev-1.0.2/src/aaz_dev/cli/templates/extension/azext_/
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/templates/extension/azext_/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/templates/extension/azext_/_help.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/templates/extension/azext_/_params.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/templates/extension/azext_/commands.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/templates/extension/azext_/custom.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.907131 aaz-dev-1.0.2/src/aaz_dev/cli/templates/extension/azext_/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/templates/extension/azext_/tests/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.907131 aaz-dev-1.0.2/src/aaz_dev/cli/templates/extension/azext_/tests/profile/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/templates/extension/azext_/tests/profile/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/templates/extension/azext_/tests/profile/test_.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/templates/extension/setup.cfg.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/templates/extension/setup.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.907131 aaz-dev-1.0.2/src/aaz_dev/cli/templates/main/
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/templates/main/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/templates/main/_help.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/templates/main/_params.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/templates/main/commands.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/templates/main/custom.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.907131 aaz-dev-1.0.2/src/aaz_dev/cli/templates/main/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/templates/main/tests/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.907131 aaz-dev-1.0.2/src/aaz_dev/cli/templates/main/tests/profile/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/templates/main/tests/profile/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/templates/main/tests/profile/test_.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/cli/templates/python.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.907131 aaz-dev-1.0.2/src/aaz_dev/command/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.911131 aaz-dev-1.0.2/src/aaz_dev/command/api/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/api/_cmds.py
--rw-r--r--   0 runner    (1001) docker     (123)    24148 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/api/editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/api/specs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.911131 aaz-dev-1.0.2/src/aaz_dev/command/controller/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41315 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/controller/cfg_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/controller/cfg_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22079 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/controller/specs_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    67447 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/controller/workspace_cfg_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    40663 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/controller/workspace_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.911131 aaz-dev-1.0.2/src/aaz_dev/command/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.919131 aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25437 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_arg.py
--rw-r--r--   0 runner    (1001) docker     (123)    15748 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_arg_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_arg_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    16261 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_command_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_content.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    10501 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_help.py
--rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_http_request_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_http_response_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_instance_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_instance_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_instance_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    36067 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_selector_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_subresource_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.919131 aaz-dev-1.0.2/src/aaz_dev/command/model/editor/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/model/editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/model/editor/_workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.919131 aaz-dev-1.0.2/src/aaz_dev/command/model/specs/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/model/specs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/model/specs/_command_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/model/specs/_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.923131 aaz-dev-1.0.2/src/aaz_dev/command/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/templates/_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/templates/command.md.j2
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/templates/group.md.j2
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/templates/resource_ref.md.j2
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/command/templates/tree.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.923131 aaz-dev-1.0.2/src/aaz_dev/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.923131 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.887131 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/diagrams/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.887131 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/diagrams/out/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.923131 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/diagrams/out/archutecture/
--rw-r--r--   0 runner    (1001) docker     (123)    44791 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/diagrams/out/archutecture/architecture.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.923131 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/diagrams/out/command_configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    41949 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/diagrams/out/command_configuration/file_structure.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.923131 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/diagrams/out/cross_version/
--rw-r--r--   0 runner    (1001) docker     (123)    34570 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/diagrams/out/cross_version/multi-api-versions.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.923131 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/diagrams/src/
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/diagrams/src/archutecture.puml
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/diagrams/src/atomic_cli_command.puml
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/diagrams/src/command_configuration.puml
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/diagrams/src/cross_version.puml
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/faq.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.931131 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)   430487 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/images/aaz_command_configuration.png
--rw-r--r--   0 runner    (1001) docker     (123)   214538 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/images/aaz_command_tree_command_md.png
--rw-r--r--   0 runner    (1001) docker     (123)   223978 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/images/aaz_command_tree_folder.png
--rw-r--r--   0 runner    (1001) docker     (123)    21118 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/images/add_resource.png
--rw-r--r--   0 runner    (1001) docker     (123)    41962 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/images/argument_edit.png
--rw-r--r--   0 runner    (1001) docker     (123)   118797 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/images/az_cli_and_az_cli_extension_command_modules.png
--rw-r--r--   0 runner    (1001) docker     (123)   108782 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/images/az_cli_bump_up_network_sdk.png
--rw-r--r--   0 runner    (1001) docker     (123)    68857 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/images/code_gen.png
--rw-r--r--   0 runner    (1001) docker     (123)    97787 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/images/command_edit.png
--rw-r--r--   0 runner    (1001) docker     (123)    10288 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/images/export.png
--rw-r--r--   0 runner    (1001) docker     (123)   121738 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/images/group_edit.png
--rw-r--r--   0 runner    (1001) docker     (123)    75040 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/images/group_edit1.png
--rw-r--r--   0 runner    (1001) docker     (123)    19994 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/images/module_select.png
--rw-r--r--   0 runner    (1001) docker     (123)   117848 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/images/pycharm_live.png
--rw-r--r--   0 runner    (1001) docker     (123)    50829 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/images/workspace.png
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/index.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13705 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.935131 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/usage/
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/usage/cli_generator_usage.md
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/usage/command_usage_testing.md
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/docs/Docs/usage/workspace_editor_usage.md
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/docs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.935131 aaz-dev-1.0.2/src/aaz_dev/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/docs/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/docs/api/docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.935131 aaz-dev-1.0.2/src/aaz_dev/docs/controller/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/docs/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/docs/controller/docs_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.935131 aaz-dev-1.0.2/src/aaz_dev/swagger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.935131 aaz-dev-1.0.2/src/aaz_dev/swagger/api/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/api/specs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.935131 aaz-dev-1.0.2/src/aaz_dev/swagger/controller/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23496 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/controller/command_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/controller/specs_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.935131 aaz-dev-1.0.2/src/aaz_dev/swagger/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.943132 aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24666 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/cmd_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/contact.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/external_documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17219 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/header.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/items.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/license.py
--rw-r--r--   0 runner    (1001) docker     (123)    11987 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11121 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/path_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    28430 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/security_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/swagger.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/x_ms_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/x_ms_long_running_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/x_ms_odata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/x_ms_pageable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/x_ms_parameter_grouping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/x_ms_parameterized_host.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.943132 aaz-dev-1.0.2/src/aaz_dev/swagger/model/specs/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/model/specs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/model/specs/_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/model/specs/_resource_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/model/specs/_swagger_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/model/specs/_swagger_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/model/specs/_swagger_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/model/specs/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.947131 aaz-dev-1.0.2/src/aaz_dev/swagger/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/swagger/utils/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.947131 aaz-dev-1.0.2/src/aaz_dev/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-03 10:46:06.000000 aaz-dev-1.0.2/src/aaz_dev/ui/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-04-03 10:45:25.000000 aaz-dev-1.0.2/src/aaz_dev/ui/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-03 10:46:06.000000 aaz-dev-1.0.2/src/aaz_dev/ui/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-04-03 10:45:25.000000 aaz-dev-1.0.2/src/aaz_dev/ui/logo192.png
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-04-03 10:45:25.000000 aaz-dev-1.0.2/src/aaz_dev/ui/logo512.png
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-03 10:45:25.000000 aaz-dev-1.0.2/src/aaz_dev/ui/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-03 10:45:25.000000 aaz-dev-1.0.2/src/aaz_dev/ui/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.887131 aaz-dev-1.0.2/src/aaz_dev/ui/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.947131 aaz-dev-1.0.2/src/aaz_dev/ui/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-03 10:46:06.000000 aaz-dev-1.0.2/src/aaz_dev/ui/static/css/main.6dea0f05.chunk.css
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-03 10:46:06.000000 aaz-dev-1.0.2/src/aaz_dev/ui/static/css/main.6dea0f05.chunk.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.959132 aaz-dev-1.0.2/src/aaz_dev/ui/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)  1403314 2023-04-03 10:46:06.000000 aaz-dev-1.0.2/src/aaz_dev/ui/static/js/2.7fb734b4.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-03 10:46:06.000000 aaz-dev-1.0.2/src/aaz_dev/ui/static/js/2.7fb734b4.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)  4447620 2023-04-03 10:46:06.000000 aaz-dev-1.0.2/src/aaz_dev/ui/static/js/2.7fb734b4.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   150327 2023-04-03 10:46:06.000000 aaz-dev-1.0.2/src/aaz_dev/ui/static/js/main.90cd0227.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)   485269 2023-04-03 10:46:06.000000 aaz-dev-1.0.2/src/aaz_dev/ui/static/js/main.90cd0227.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-03 10:46:06.000000 aaz-dev-1.0.2/src/aaz_dev/ui/static/js/runtime-main.f7313c7c.js
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-04-03 10:46:06.000000 aaz-dev-1.0.2/src/aaz_dev/ui/static/js/runtime-main.f7313c7c.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.963132 aaz-dev-1.0.2/src/aaz_dev/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/utils/base64.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/utils/case.py
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/utils/error_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/utils/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/utils/plane.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/utils/portal_file_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/src/aaz_dev/utils/stage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:46:07.891131 aaz-dev-1.0.2/src/aaz_dev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-04-03 10:46:07.000000 aaz-dev-1.0.2/src/aaz_dev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10103 2023-04-03 10:46:07.000000 aaz-dev-1.0.2/src/aaz_dev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 10:46:07.000000 aaz-dev-1.0.2/src/aaz_dev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-03 10:46:07.000000 aaz-dev-1.0.2/src/aaz_dev.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-03 10:46:07.000000 aaz-dev-1.0.2/src/aaz_dev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-03 10:46:07.000000 aaz-dev-1.0.2/src/aaz_dev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-03 10:45:07.000000 aaz-dev-1.0.2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.819145 aaz-dev-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-04-12 05:28:52.819145 aaz-dev-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 05:28:52.819145 aaz-dev-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.739145 aaz-dev-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.747145 aaz-dev-1.1.0/src/aaz_dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.751145 aaz-dev-1.1.0/src/aaz_dev/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/app/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/app/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/app/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/app/url_converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.751145 aaz-dev-1.1.0/src/aaz_dev/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.751145 aaz-dev-1.1.0/src/aaz_dev/cli/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/api/_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/api/az.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/api/portal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.755145 aaz-dev-1.1.0/src/aaz_dev/cli/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/controller/az_arg_group_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/controller/az_atomic_profile_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18759 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/controller/az_command_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27518 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/controller/az_module_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38422 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/controller/az_operation_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/controller/az_output_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/controller/az_profile_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/controller/az_selector_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19004 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/controller/portal_cli_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.755145 aaz-dev-1.1.0/src/aaz_dev/cli/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.755145 aaz-dev-1.1.0/src/aaz_dev/cli/model/atomic/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/model/atomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/model/atomic/_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/model/atomic/_command_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/model/atomic/_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/model/atomic/_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/model/atomic/_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/model/atomic/_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.759145 aaz-dev-1.1.0/src/aaz_dev/cli/model/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/model/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/model/common/_fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.759145 aaz-dev-1.1.0/src/aaz_dev/cli/model/view/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/model/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/model/view/_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/model/view/_command_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/model/view/_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/model/view/_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.759145 aaz-dev-1.1.0/src/aaz_dev/cli/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/templates/_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.759145 aaz-dev-1.1.0/src/aaz_dev/cli/templates/aaz/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/templates/aaz/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.759145 aaz-dev-1.1.0/src/aaz_dev/cli/templates/aaz/command/
+-rw-r--r--   0 runner    (1001) docker     (123)    31616 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/templates/aaz/command/_cmd.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.759145 aaz-dev-1.1.0/src/aaz_dev/cli/templates/aaz/group/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/templates/aaz/group/__cmd_group.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/templates/aaz/group/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.759145 aaz-dev-1.1.0/src/aaz_dev/cli/templates/aaz/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/templates/aaz/profile/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.763145 aaz-dev-1.1.0/src/aaz_dev/cli/templates/extension/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/templates/extension/HISTORY.rst.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/templates/extension/README.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.763145 aaz-dev-1.1.0/src/aaz_dev/cli/templates/extension/azext_/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/templates/extension/azext_/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/templates/extension/azext_/_help.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/templates/extension/azext_/_params.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/templates/extension/azext_/commands.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/templates/extension/azext_/custom.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.763145 aaz-dev-1.1.0/src/aaz_dev/cli/templates/extension/azext_/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/templates/extension/azext_/tests/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.763145 aaz-dev-1.1.0/src/aaz_dev/cli/templates/extension/azext_/tests/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/templates/extension/azext_/tests/profile/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/templates/extension/azext_/tests/profile/test_.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/templates/extension/setup.cfg.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/templates/extension/setup.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.763145 aaz-dev-1.1.0/src/aaz_dev/cli/templates/main/
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/templates/main/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/templates/main/_help.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/templates/main/_params.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/templates/main/commands.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/templates/main/custom.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.763145 aaz-dev-1.1.0/src/aaz_dev/cli/templates/main/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/templates/main/tests/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.763145 aaz-dev-1.1.0/src/aaz_dev/cli/templates/main/tests/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/templates/main/tests/profile/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/templates/main/tests/profile/test_.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/cli/templates/python.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.763145 aaz-dev-1.1.0/src/aaz_dev/command/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.767145 aaz-dev-1.1.0/src/aaz_dev/command/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/api/_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24148 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/api/editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/api/specs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.767145 aaz-dev-1.1.0/src/aaz_dev/command/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41315 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/controller/cfg_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/controller/cfg_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22079 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/controller/specs_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67447 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/controller/workspace_cfg_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40663 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/controller/workspace_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.767145 aaz-dev-1.1.0/src/aaz_dev/command/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.775145 aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25437 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15748 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_arg_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_arg_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16261 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_command_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10501 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_http_request_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_http_response_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_instance_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_instance_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_instance_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36320 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_selector_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_subresource_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.775145 aaz-dev-1.1.0/src/aaz_dev/command/model/editor/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/model/editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/model/editor/_workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.775145 aaz-dev-1.1.0/src/aaz_dev/command/model/specs/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/model/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/model/specs/_command_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/model/specs/_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.779145 aaz-dev-1.1.0/src/aaz_dev/command/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/templates/_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/templates/command.md.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/templates/group.md.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/templates/resource_ref.md.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/command/templates/tree.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.779145 aaz-dev-1.1.0/src/aaz_dev/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.779145 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.743145 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/diagrams/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.743145 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/diagrams/out/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.779145 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/diagrams/out/archutecture/
+-rw-r--r--   0 runner    (1001) docker     (123)    44791 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/diagrams/out/archutecture/architecture.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.779145 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/diagrams/out/command_configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)    41949 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/diagrams/out/command_configuration/file_structure.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.779145 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/diagrams/out/cross_version/
+-rw-r--r--   0 runner    (1001) docker     (123)    34570 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/diagrams/out/cross_version/multi-api-versions.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.779145 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/diagrams/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/diagrams/src/archutecture.puml
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/diagrams/src/atomic_cli_command.puml
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/diagrams/src/command_configuration.puml
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/diagrams/src/cross_version.puml
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/faq.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.787145 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   430487 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/images/aaz_command_configuration.png
+-rw-r--r--   0 runner    (1001) docker     (123)   214538 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/images/aaz_command_tree_command_md.png
+-rw-r--r--   0 runner    (1001) docker     (123)   223978 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/images/aaz_command_tree_folder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21118 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/images/add_resource.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41962 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/images/argument_edit.png
+-rw-r--r--   0 runner    (1001) docker     (123)   118797 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/images/az_cli_and_az_cli_extension_command_modules.png
+-rw-r--r--   0 runner    (1001) docker     (123)   108782 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/images/az_cli_bump_up_network_sdk.png
+-rw-r--r--   0 runner    (1001) docker     (123)    68857 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/images/code_gen.png
+-rw-r--r--   0 runner    (1001) docker     (123)    97787 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/images/command_edit.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10288 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/images/export.png
+-rw-r--r--   0 runner    (1001) docker     (123)   121738 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/images/group_edit.png
+-rw-r--r--   0 runner    (1001) docker     (123)    75040 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/images/group_edit1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19994 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/images/module_select.png
+-rw-r--r--   0 runner    (1001) docker     (123)   117848 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/images/pycharm_live.png
+-rw-r--r--   0 runner    (1001) docker     (123)    50829 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/images/workspace.png
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/index.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13705 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.787145 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/usage/
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/usage/cli_generator_usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/usage/command_usage_testing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/docs/Docs/usage/workspace_editor_usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/docs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.787145 aaz-dev-1.1.0/src/aaz_dev/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/docs/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/docs/api/docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.787145 aaz-dev-1.1.0/src/aaz_dev/docs/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/docs/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/docs/controller/docs_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.787145 aaz-dev-1.1.0/src/aaz_dev/swagger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.787145 aaz-dev-1.1.0/src/aaz_dev/swagger/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/api/specs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.791145 aaz-dev-1.1.0/src/aaz_dev/swagger/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23496 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/controller/command_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/controller/specs_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.791145 aaz-dev-1.1.0/src/aaz_dev/swagger/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.795145 aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25073 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/cmd_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/external_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17557 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/items.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/license.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11987 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/path_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28604 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/security_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/swagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/x_ms_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/x_ms_long_running_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/x_ms_odata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/x_ms_pageable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/x_ms_parameter_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/x_ms_parameterized_host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.795145 aaz-dev-1.1.0/src/aaz_dev/swagger/model/specs/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/model/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/model/specs/_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/model/specs/_resource_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/model/specs/_swagger_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/model/specs/_swagger_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/model/specs/_swagger_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/model/specs/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.799145 aaz-dev-1.1.0/src/aaz_dev/swagger/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/swagger/utils/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.799145 aaz-dev-1.1.0/src/aaz_dev/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-12 05:28:50.000000 aaz-dev-1.1.0/src/aaz_dev/ui/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-04-12 05:28:11.000000 aaz-dev-1.1.0/src/aaz_dev/ui/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-12 05:28:50.000000 aaz-dev-1.1.0/src/aaz_dev/ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-04-12 05:28:11.000000 aaz-dev-1.1.0/src/aaz_dev/ui/logo192.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-04-12 05:28:11.000000 aaz-dev-1.1.0/src/aaz_dev/ui/logo512.png
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-12 05:28:11.000000 aaz-dev-1.1.0/src/aaz_dev/ui/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-12 05:28:11.000000 aaz-dev-1.1.0/src/aaz_dev/ui/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.747145 aaz-dev-1.1.0/src/aaz_dev/ui/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.799145 aaz-dev-1.1.0/src/aaz_dev/ui/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-12 05:28:51.000000 aaz-dev-1.1.0/src/aaz_dev/ui/static/css/main.6dea0f05.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-12 05:28:51.000000 aaz-dev-1.1.0/src/aaz_dev/ui/static/css/main.6dea0f05.chunk.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.815145 aaz-dev-1.1.0/src/aaz_dev/ui/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)  1403314 2023-04-12 05:28:51.000000 aaz-dev-1.1.0/src/aaz_dev/ui/static/js/2.7fb734b4.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-12 05:28:51.000000 aaz-dev-1.1.0/src/aaz_dev/ui/static/js/2.7fb734b4.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  4447620 2023-04-12 05:28:51.000000 aaz-dev-1.1.0/src/aaz_dev/ui/static/js/2.7fb734b4.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   150327 2023-04-12 05:28:51.000000 aaz-dev-1.1.0/src/aaz_dev/ui/static/js/main.90cd0227.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)   485269 2023-04-12 05:28:51.000000 aaz-dev-1.1.0/src/aaz_dev/ui/static/js/main.90cd0227.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-12 05:28:51.000000 aaz-dev-1.1.0/src/aaz_dev/ui/static/js/runtime-main.f7313c7c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-04-12 05:28:51.000000 aaz-dev-1.1.0/src/aaz_dev/ui/static/js/runtime-main.f7313c7c.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.819145 aaz-dev-1.1.0/src/aaz_dev/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/utils/base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/utils/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/utils/error_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/utils/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/utils/plane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/utils/portal_file_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/src/aaz_dev/utils/stage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:28:52.751145 aaz-dev-1.1.0/src/aaz_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-04-12 05:28:51.000000 aaz-dev-1.1.0/src/aaz_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10103 2023-04-12 05:28:52.000000 aaz-dev-1.1.0/src/aaz_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 05:28:51.000000 aaz-dev-1.1.0/src/aaz_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-12 05:28:51.000000 aaz-dev-1.1.0/src/aaz_dev.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-12 05:28:51.000000 aaz-dev-1.1.0/src/aaz_dev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 05:28:51.000000 aaz-dev-1.1.0/src/aaz_dev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-12 05:27:49.000000 aaz-dev-1.1.0/version.py
```

### Comparing `aaz-dev-1.0.2/HISTORY.rst` & `aaz-dev-1.1.0/HISTORY.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 .. :changelog:
 
 Release History
 ===============
 
+1.1.0
+++++++
+* Support x-ms-secret of swagger (#235)
+* Add support to parse x-ms-arm-id-details and "arm-id" format in swagger (#234)
+
 1.0.2
 ++++++
 * Support PyPI installation (#230)
 * Fix cfg reader response.status_codes string join issue (#228)
 
 1.0.1
 ++++++
```

### Comparing `aaz-dev-1.0.2/LICENSE` & `aaz-dev-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/PKG-INFO` & `aaz-dev-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aaz-dev
-Version: 1.0.2
+Version: 1.1.0
 Summary: Microsoft Atomic Azure CLI Commands Developer Tools
 Home-page: https://github.com/Azure/aaz-dev-tools
 Author: Microsoft Corporation
 Author-email: azpycli@microsoft.com
 License: MIT
 Keywords: azure
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aaz-dev-1.0.2/README.md` & `aaz-dev-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/setup.py` & `aaz-dev-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/app/app.py` & `aaz-dev-1.1.0/src/aaz_dev/app/app.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/app/run.py` & `aaz-dev-1.1.0/src/aaz_dev/app/run.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/app/url_converters.py` & `aaz-dev-1.1.0/src/aaz_dev/app/url_converters.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/cli/api/_cmds.py` & `aaz-dev-1.1.0/src/aaz_dev/cli/api/_cmds.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/cli/api/az.py` & `aaz-dev-1.1.0/src/aaz_dev/cli/api/az.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/cli/api/portal.py` & `aaz-dev-1.1.0/src/aaz_dev/cli/api/portal.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/cli/controller/az_arg_group_generator.py` & `aaz-dev-1.1.0/src/aaz_dev/cli/controller/az_arg_group_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,16 +325,17 @@
             arg_type = "AAZDurationArg"
         elif isinstance(arg, CMDDateArgBase):
             arg_type = "AAZDateArg"
         elif isinstance(arg, CMDDateTimeArgBase):
             arg_type = "AAZDateTimeArg"
         elif isinstance(arg, CMDUuidArgBase):
             arg_type = "AAZUuidArg"
-        elif isinstance(arg, CMDPasswordArgBase):
-            raise NotImplementedError()
+        # TODO: Support Password Arg
+        # elif isinstance(arg, CMDPasswordArgBase):
+            # arg_type = "AAZPasswordArg"
 
     elif isinstance(arg, CMDIntegerArgBase):
         arg_type = "AAZIntArg"
         enum = parse_arg_enum(arg.enum)
         if enum:
             arg_kwargs['enum'] = enum
```

### Comparing `aaz-dev-1.0.2/src/aaz_dev/cli/controller/az_atomic_profile_builder.py` & `aaz-dev-1.1.0/src/aaz_dev/cli/controller/az_atomic_profile_builder.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/cli/controller/az_command_generator.py` & `aaz-dev-1.1.0/src/aaz_dev/cli/controller/az_command_generator.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/cli/controller/az_module_manager.py` & `aaz-dev-1.1.0/src/aaz_dev/cli/controller/az_module_manager.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/cli/controller/az_operation_generator.py` & `aaz-dev-1.1.0/src/aaz_dev/cli/controller/az_operation_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -894,14 +894,16 @@
 
     if schema.required:
         flags['required'] = True
     if schema.skip_url_encoding:
         flags['skip_quote'] = True
     if getattr(schema, 'client_flatten', False):
         flags['client_flatten'] = True
+    if getattr(schema, 'secret', False):
+        flags['secret'] = True
 
     if flags:
         schema_kwargs['flags'] = flags
 
     schema_type, schema_kwargs, cls_builder_name = render_schema_base(schema, cls_map, schema_kwargs)
 
     return schema_type, schema_kwargs, cls_builder_name
```

### Comparing `aaz-dev-1.0.2/src/aaz_dev/cli/controller/az_output_generator.py` & `aaz-dev-1.1.0/src/aaz_dev/cli/controller/az_output_generator.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/cli/controller/az_profile_generator.py` & `aaz-dev-1.1.0/src/aaz_dev/cli/controller/az_profile_generator.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/cli/controller/az_selector_generator.py` & `aaz-dev-1.1.0/src/aaz_dev/cli/controller/az_selector_generator.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/cli/controller/portal_cli_generator.py` & `aaz-dev-1.1.0/src/aaz_dev/cli/controller/portal_cli_generator.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/cli/model/atomic/_command.py` & `aaz-dev-1.1.0/src/aaz_dev/cli/model/atomic/_command.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/cli/model/atomic/_command_group.py` & `aaz-dev-1.1.0/src/aaz_dev/cli/model/atomic/_command_group.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/cli/model/atomic/_help.py` & `aaz-dev-1.1.0/src/aaz_dev/cli/model/atomic/_help.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/cli/model/common/_fields.py` & `aaz-dev-1.1.0/src/aaz_dev/cli/model/common/_fields.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/cli/model/view/_command.py` & `aaz-dev-1.1.0/src/aaz_dev/cli/model/view/_command.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/cli/model/view/_command_group.py` & `aaz-dev-1.1.0/src/aaz_dev/cli/model/view/_command_group.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/cli/model/view/_module.py` & `aaz-dev-1.1.0/src/aaz_dev/cli/model/view/_module.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/cli/model/view/_profile.py` & `aaz-dev-1.1.0/src/aaz_dev/cli/model/view/_profile.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/cli/templates/__init__.py` & `aaz-dev-1.1.0/src/aaz_dev/cli/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/cli/templates/_filters.py` & `aaz-dev-1.1.0/src/aaz_dev/cli/templates/_filters.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/cli/templates/aaz/command/_cmd.py.j2` & `aaz-dev-1.1.0/src/aaz_dev/cli/templates/aaz/command/_cmd.py.j2`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/cli/templates/aaz/group/__cmd_group.py.j2` & `aaz-dev-1.1.0/src/aaz_dev/cli/templates/aaz/group/__cmd_group.py.j2`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/cli/templates/extension/azext_/__init__.py.j2` & `aaz-dev-1.1.0/src/aaz_dev/cli/templates/extension/azext_/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/cli/templates/extension/setup.py.j2` & `aaz-dev-1.1.0/src/aaz_dev/cli/templates/extension/setup.py.j2`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/cli/templates/main/__init__.py.j2` & `aaz-dev-1.1.0/src/aaz_dev/cli/templates/main/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/api/_cmds.py` & `aaz-dev-1.1.0/src/aaz_dev/command/api/_cmds.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/api/editor.py` & `aaz-dev-1.1.0/src/aaz_dev/command/api/editor.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/api/specs.py` & `aaz-dev-1.1.0/src/aaz_dev/command/api/specs.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/controller/cfg_reader.py` & `aaz-dev-1.1.0/src/aaz_dev/command/controller/cfg_reader.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/controller/specs_manager.py` & `aaz-dev-1.1.0/src/aaz_dev/command/controller/specs_manager.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/controller/workspace_cfg_editor.py` & `aaz-dev-1.1.0/src/aaz_dev/command/controller/workspace_cfg_editor.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/controller/workspace_manager.py` & `aaz-dev-1.1.0/src/aaz_dev/command/controller/workspace_manager.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/__init__.py` & `aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_arg.py` & `aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_arg.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_arg_builder.py` & `aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_arg_builder.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_arg_group.py` & `aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_arg_group.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_command.py` & `aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_command.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_command_group.py` & `aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_command_group.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_condition.py` & `aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_condition.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_configuration.py` & `aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_configuration.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_content.py` & `aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_content.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_fields.py` & `aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_fields.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_format.py` & `aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_format.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_help.py` & `aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_help.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_http.py` & `aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_http.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_http_request_body.py` & `aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_http_request_body.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_http_response_body.py` & `aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_http_response_body.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_instance_create.py` & `aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_instance_create.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_instance_delete.py` & `aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_instance_delete.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_instance_update.py` & `aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_instance_update.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_operation.py` & `aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_operation.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_output.py` & `aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_output.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_resource.py` & `aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_resource.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_schema.py` & `aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -264,14 +264,16 @@
     description = CMDDescriptionField()
 
     skip_url_encoding = CMDBooleanField(
         serialized_name="skipUrlEncoding",
         deserialize_from="skipUrlEncoding",
     )  # used in path and query parameters
 
+    secret = CMDBooleanField()
+
     @classmethod
     def _claim_polymorphic(cls, data):
         if super(CMDSchema, cls)._claim_polymorphic(data):
             if isinstance(data, dict):
                 # distinguish with CMDSchemaBase and CMDSchema
                 return 'name' in data
             else:
@@ -282,18 +284,22 @@
         if level >= CMDDiffLevelEnum.BreakingChange:
             if self.name != old.name:
                 diff["name"] = f"{old.name} != {self.name}"
             if self.required and not old.required:
                 diff["required"] = f"it's required now."
             if (not self.skip_url_encoding) != (not old.skip_url_encoding):  # None should be same as false
                 diff["skip_url_encoding"] = f"{old.skip_url_encoding} != {self.skip_url_encoding}"
+            if not self.secret and old.secret:
+                diff["secret"] = f"it's not secret property now."
 
         if level >= CMDDiffLevelEnum.Structure:
             if (not self.required) != (not old.required):
                 diff["required"] = f"{old.required} != {self.required}"
+            if self.secret != old.secret:
+                diff["secret"] = f"{old.secret} != {self.secret}"
 
         if level >= CMDDiffLevelEnum.Associate:
             if self.arg != old.arg:
                 diff["arg"] = f"{old.arg} != {self.arg}"
 
         if level >= CMDDiffLevelEnum.All:
             if self.description != old.description:
```

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_selector_index.py` & `aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_selector_index.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_subresource_selector.py` & `aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_subresource_selector.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/model/configuration/_xml.py` & `aaz-dev-1.1.0/src/aaz_dev/command/model/configuration/_xml.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/model/editor/_workspace.py` & `aaz-dev-1.1.0/src/aaz_dev/command/model/editor/_workspace.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/model/specs/_command_tree.py` & `aaz-dev-1.1.0/src/aaz_dev/command/model/specs/_command_tree.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/templates/__init__.py` & `aaz-dev-1.1.0/src/aaz_dev/command/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/templates/_filters.py` & `aaz-dev-1.1.0/src/aaz_dev/command/templates/_filters.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/templates/command.md.j2` & `aaz-dev-1.1.0/src/aaz_dev/command/templates/command.md.j2`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/command/templates/group.md.j2` & `aaz-dev-1.1.0/src/aaz_dev/command/templates/group.md.j2`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/docs/Docs/diagrams/out/archutecture/architecture.svg` & `aaz-dev-1.1.0/src/aaz_dev/docs/Docs/diagrams/out/archutecture/architecture.svg`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/docs/Docs/diagrams/out/command_configuration/file_structure.svg` & `aaz-dev-1.1.0/src/aaz_dev/docs/Docs/diagrams/out/command_configuration/file_structure.svg`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/docs/Docs/diagrams/out/cross_version/multi-api-versions.svg` & `aaz-dev-1.1.0/src/aaz_dev/docs/Docs/diagrams/out/cross_version/multi-api-versions.svg`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/docs/Docs/diagrams/src/archutecture.puml` & `aaz-dev-1.1.0/src/aaz_dev/docs/Docs/diagrams/src/archutecture.puml`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/docs/Docs/diagrams/src/atomic_cli_command.puml` & `aaz-dev-1.1.0/src/aaz_dev/docs/Docs/diagrams/src/atomic_cli_command.puml`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/docs/Docs/diagrams/src/command_configuration.puml` & `aaz-dev-1.1.0/src/aaz_dev/docs/Docs/diagrams/src/command_configuration.puml`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/docs/Docs/diagrams/src/cross_version.puml` & `aaz-dev-1.1.0/src/aaz_dev/docs/Docs/diagrams/src/cross_version.puml`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/docs/Docs/faq.md` & `aaz-dev-1.1.0/src/aaz_dev/docs/Docs/faq.md`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/docs/Docs/images/aaz_command_configuration.png` & `aaz-dev-1.1.0/src/aaz_dev/docs/Docs/images/aaz_command_configuration.png`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/docs/Docs/images/aaz_command_tree_command_md.png` & `aaz-dev-1.1.0/src/aaz_dev/docs/Docs/images/aaz_command_tree_command_md.png`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/docs/Docs/images/aaz_command_tree_folder.png` & `aaz-dev-1.1.0/src/aaz_dev/docs/Docs/images/aaz_command_tree_folder.png`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/docs/Docs/images/add_resource.png` & `aaz-dev-1.1.0/src/aaz_dev/docs/Docs/images/add_resource.png`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/docs/Docs/images/argument_edit.png` & `aaz-dev-1.1.0/src/aaz_dev/docs/Docs/images/argument_edit.png`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/docs/Docs/images/az_cli_and_az_cli_extension_command_modules.png` & `aaz-dev-1.1.0/src/aaz_dev/docs/Docs/images/az_cli_and_az_cli_extension_command_modules.png`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/docs/Docs/images/az_cli_bump_up_network_sdk.png` & `aaz-dev-1.1.0/src/aaz_dev/docs/Docs/images/az_cli_bump_up_network_sdk.png`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/docs/Docs/images/code_gen.png` & `aaz-dev-1.1.0/src/aaz_dev/docs/Docs/images/code_gen.png`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/docs/Docs/images/command_edit.png` & `aaz-dev-1.1.0/src/aaz_dev/docs/Docs/images/command_edit.png`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/docs/Docs/images/export.png` & `aaz-dev-1.1.0/src/aaz_dev/docs/Docs/images/export.png`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/docs/Docs/images/group_edit.png` & `aaz-dev-1.1.0/src/aaz_dev/docs/Docs/images/group_edit.png`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/docs/Docs/images/group_edit1.png` & `aaz-dev-1.1.0/src/aaz_dev/docs/Docs/images/group_edit1.png`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/docs/Docs/images/module_select.png` & `aaz-dev-1.1.0/src/aaz_dev/docs/Docs/images/module_select.png`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/docs/Docs/images/pycharm_live.png` & `aaz-dev-1.1.0/src/aaz_dev/docs/Docs/images/pycharm_live.png`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/docs/Docs/images/workspace.png` & `aaz-dev-1.1.0/src/aaz_dev/docs/Docs/images/workspace.png`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/docs/Docs/readme.md` & `aaz-dev-1.1.0/src/aaz_dev/docs/Docs/readme.md`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/docs/Docs/usage/cli_generator_usage.md` & `aaz-dev-1.1.0/src/aaz_dev/docs/Docs/usage/cli_generator_usage.md`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/docs/Docs/usage/command_usage_testing.md` & `aaz-dev-1.1.0/src/aaz_dev/docs/Docs/usage/command_usage_testing.md`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/docs/Docs/usage/workspace_editor_usage.md` & `aaz-dev-1.1.0/src/aaz_dev/docs/Docs/usage/workspace_editor_usage.md`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/docs/api/docs.py` & `aaz-dev-1.1.0/src/aaz_dev/docs/api/docs.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/docs/controller/docs_manager.py` & `aaz-dev-1.1.0/src/aaz_dev/docs/controller/docs_manager.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/swagger/api/specs.py` & `aaz-dev-1.1.0/src/aaz_dev/swagger/api/specs.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/swagger/controller/command_generator.py` & `aaz-dev-1.1.0/src/aaz_dev/swagger/controller/command_generator.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/swagger/controller/specs_manager.py` & `aaz-dev-1.1.0/src/aaz_dev/swagger/controller/specs_manager.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/cmd_builder.py` & `aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/cmd_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     CMDByteSchema, CMDByteSchemaBase, \
     CMDBinarySchema, CMDBinarySchemaBase, \
     CMDDateSchema, CMDDateSchemaBase, \
     CMDDateTimeSchema, CMDDateTimeSchemaBase, \
     CMDPasswordSchema, CMDPasswordSchemaBase, \
     CMDDurationSchema, CMDDurationSchemaBase, \
     CMDUuidSchema, CMDUuidSchemaBase, \
+    CMDResourceIdSchema, CMDResourceIdSchemaBase, \
     CMDIntegerSchema, CMDIntegerSchemaBase, \
     CMDInteger32Schema, CMDInteger32SchemaBase, \
     CMDInteger64Schema, CMDInteger64SchemaBase, \
     CMDBooleanSchema, CMDBooleanSchemaBase, \
     CMDFloatSchema, CMDFloatSchemaBase, \
     CMDFloat32Schema, CMDFloat32SchemaBase, \
     CMDFloat64Schema, CMDFloat64SchemaBase, \
@@ -123,14 +124,19 @@
                 else:
                     model = CMDDurationSchema()
             elif schema.format == "uuid":
                 if self.in_base:
                     model = CMDUuidSchemaBase()
                 else:
                     model = CMDUuidSchema()
+            elif schema.format == "arm-id":
+                if self.in_base:
+                    model = CMDResourceIdSchemaBase()
+                else:
+                    model = CMDResourceIdSchema()
             else:
                 raise exceptions.InvalidSwaggerValueError(
                     f"format is not supported", key=getattr(schema, "traces", None), value=[schema_type, schema.format])
         elif schema_type == "integer":
             if schema.format is None:
                 if self.in_base:
                     model = CMDIntegerSchemaBase()
@@ -339,14 +345,19 @@
     def setup_description(model, schema):
         if schema.description:
             model.description = schema.description
         elif schema.title:
             model.description = schema.title
 
     @staticmethod
+    def setup_secret(model, schema):
+        if getattr(schema, 'x_ms_secret', False):
+            model.secret = schema.x_ms_secret
+
+    @staticmethod
     def build_cmd_string_format(schema):
         fmt_assigned = False
         fmt = CMDStringFormat()
 
         if schema.pattern is not None:
             try:
                 _ = re.compile(schema.pattern)  # verify schema pattern
```

### Comparing `aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/contact.py` & `aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/contact.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/fields.py` & `aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     VALID_TYPE_FORMATS = (
         "int32", "int64",
         "float", "double",
         "byte", "binary", "date", "date-time", "password",
         # additional formats
         "duration", "uuid",
         "file", "uri",
+        "arm-id",
     )
 
     def __init__(self, **kwargs):
         super().__init__(choices=self.VALID_TYPE_FORMATS, **kwargs)
 
 
 class MimeField(StringType):
@@ -260,14 +261,28 @@
         super().__init__(
             serialized_name='x-ms-client-default',
             deserialize_from='x-ms-client-default',
             **kwargs
         )
 
 
+class XmsArmIdDetailsField(BaseType):
+    """
+
+    http://azure.github.io/autorest/extensions/#x-ms-arm-id-details
+    """
+
+    def __init__(self, **kwargs):
+        super().__init__(
+            serialized_name='x-ms-arm-id-details',
+            deserialize_from='x-ms-arm-id-details',
+            **kwargs
+        )
+
+
 class XmsAzureResourceField(BooleanType):
     """
     Resource types as defined by the Resource Manager API are tagged by using a x-ms-azure-resource extension.
 
     https://github.com/Azure/autorest/blob/main/docs/extensions/readme.md#x-ms-azure-resource
     """
```

### Comparing `aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/info.py` & `aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/info.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/items.py` & `aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/items.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/operation.py` & `aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/operation.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/parameter.py` & `aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/parameter.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from schematics.models import Model
 from schematics.types import StringType, BooleanType, ModelType, PolyModelType, BaseType
 from swagger.utils import exceptions
 
 from .fields import XmsClientNameField, XmsClientFlattenField, XmsClientDefaultField
 from .fields import XmsClientRequestIdField, XNullableField, XPublishField, XRequiredField, XClientNameField, \
     XNewPatternField, XPreviousPatternField, XCommentField
-from .fields import XmsParameterLocationField, XmsApiVersionField, XmsSkipUrlEncodingField
+from .fields import XmsParameterLocationField, XmsApiVersionField, XmsSkipUrlEncodingField, XmsArmIdDetailsField
 from .fields import XmsSkipURLEncodingField, XAccessibilityField, XmsHeaderCollectionPrefix, XOriginalNameField
 from .items import Items
 from .reference import Reference, Linkable
 from .schema import Schema, ReferenceSchema, schema_and_reference_schema_claim_function
 from .x_ms_parameter_grouping import XmsParameterGroupingField
 
 logger = logging.getLogger('backend')
@@ -39,14 +39,15 @@
     )  # The location of the parameter. Possible values are "query", "header", "path", "formData" or "body".
 
     x_ms_parameter_grouping = XmsParameterGroupingField()  # TODO:
     x_ms_parameter_location = XmsParameterLocationField()  # TODO:
     x_ms_client_name = XmsClientNameField()  # TODO:
     x_ms_client_flatten = XmsClientFlattenField()  # TODO:
     x_ms_client_default = XmsClientDefaultField()
+    x_ms_arm_id_details = XmsArmIdDetailsField()  # TODO: Add support for it, can be used for resource id template
 
     # specific properties
     _x_accessibility = XAccessibilityField()  # only used in ContainerRegistry Data plane
     _x_required = XRequiredField()  # only used in ContainerRegistry Data plane
     _x_publish = XPublishField()  # only used in Maps Data Plane
     _x_example = BaseType(serialized_name='x-example', deserialize_from='x-example')  # deprecated
     _x_examples = BaseType(serialized_name='x-examples', deserialize_from='x-examples')  # deprecated
```

### Comparing `aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/path_item.py` & `aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/path_item.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/reference.py` & `aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/reference.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/response.py` & `aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/response.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/schema.py` & `aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     CMDObjectSchemaBase, CMDObjectSchemaDiscriminator, CMDObjectSchemaAdditionalProperties, \
     CMDArraySchemaBase, CMDObjectSchema, CMDIdentityObjectSchema, CMDIdentityObjectSchemaBase, CMDClsSchemaBase
 from command.model.configuration import CMDSchemaEnum, CMDSchemaEnumItem, CMDSchema, CMDSchemaBase
 from swagger.utils import exceptions
 from .external_documentation import ExternalDocumentation
 from .fields import DataTypeFormatEnum, RegularExpressionField, XmsClientNameField, XmsExternalField, \
     XmsDiscriminatorValueField, XmsClientFlattenField, XmsMutabilityField, XmsClientDefaultField, XNullableField, \
-    XmsAzureResourceField, MutabilityEnum
+    XmsAzureResourceField, MutabilityEnum, XmsArmIdDetailsField
 from .fields import XmsSecretField, XAccessibilityField, XAzSearchDeprecatedField, XSfClientLibField, \
     XApimCodeNillableField, XCommentField, XAbstractField, XADLNameField, XCadlNameField
 from .reference import ReferenceField, Linkable
 from .x_ms_enum import XmsEnumField
 from .xml import XML
 
 logger = logging.getLogger('backend')
@@ -231,18 +231,19 @@
 
     x_ms_client_name = XmsClientNameField()  # TODO: used for deserialized name
     x_ms_external = XmsExternalField()  # TODO:
     x_ms_discriminator_value = XmsDiscriminatorValueField()
     x_ms_client_flatten = XmsClientFlattenField()
     x_ms_mutability = XmsMutabilityField()
     x_ms_client_default = XmsClientDefaultField()
+    x_ms_arm_id_details = XmsArmIdDetailsField()  # TODO: Add support for it, can be used for resource id template
 
     x_ms_azure_resource = XmsAzureResourceField()
 
-    x_ms_secret = XmsSecretField()  # TODO:
+    x_ms_secret = XmsSecretField()
 
     x_nullable = XNullableField()  # when true, specifies that null is a valid value for the associated schema
 
     x_ms_identifiers = ListType(StringType(), serialized_name="x-ms-identifiers", deserialize_from="x-ms-identifiers")
 
     # specific properties, will not support
     _x_accessibility = XAccessibilityField()  # only used in ContainerRegistry Data plane
@@ -602,9 +603,10 @@
         builder.setup_fmt(model, self)
         builder.setup_enum(model, self)
         builder.setup_default(model, self)
         builder.setup_nullable(model, self)
 
         if isinstance(model, CMDSchema):
             builder.setup_description(model, self)
+            builder.setup_secret(model, self)
 
         return model
```

### Comparing `aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/security_scheme.py` & `aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/security_scheme.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/swagger.py` & `aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/swagger.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/tag.py` & `aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/tag.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/x_ms_enum.py` & `aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/x_ms_enum.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/x_ms_long_running_operation.py` & `aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/x_ms_long_running_operation.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/x_ms_odata.py` & `aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/x_ms_odata.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/x_ms_pageable.py` & `aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/x_ms_pageable.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/x_ms_parameter_grouping.py` & `aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/x_ms_parameter_grouping.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/x_ms_parameterized_host.py` & `aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/x_ms_parameterized_host.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/swagger/model/schema/xml.py` & `aaz-dev-1.1.0/src/aaz_dev/swagger/model/schema/xml.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/swagger/model/specs/_resource.py` & `aaz-dev-1.1.0/src/aaz_dev/swagger/model/specs/_resource.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/swagger/model/specs/_resource_provider.py` & `aaz-dev-1.1.0/src/aaz_dev/swagger/model/specs/_resource_provider.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/swagger/model/specs/_swagger_loader.py` & `aaz-dev-1.1.0/src/aaz_dev/swagger/model/specs/_swagger_loader.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/swagger/model/specs/_swagger_module.py` & `aaz-dev-1.1.0/src/aaz_dev/swagger/model/specs/_swagger_module.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/swagger/model/specs/_swagger_specs.py` & `aaz-dev-1.1.0/src/aaz_dev/swagger/model/specs/_swagger_specs.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/swagger/model/specs/_utils.py` & `aaz-dev-1.1.0/src/aaz_dev/swagger/model/specs/_utils.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/swagger/utils/tools.py` & `aaz-dev-1.1.0/src/aaz_dev/swagger/utils/tools.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/ui/asset-manifest.json` & `aaz-dev-1.1.0/src/aaz_dev/ui/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/ui/favicon.ico` & `aaz-dev-1.1.0/src/aaz_dev/ui/favicon.ico`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/ui/index.html` & `aaz-dev-1.1.0/src/aaz_dev/ui/index.html`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/ui/logo192.png` & `aaz-dev-1.1.0/src/aaz_dev/ui/logo192.png`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/ui/logo512.png` & `aaz-dev-1.1.0/src/aaz_dev/ui/logo512.png`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/ui/static/css/main.6dea0f05.chunk.css.map` & `aaz-dev-1.1.0/src/aaz_dev/ui/static/css/main.6dea0f05.chunk.css.map`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/ui/static/js/2.7fb734b4.chunk.js` & `aaz-dev-1.1.0/src/aaz_dev/ui/static/js/2.7fb734b4.chunk.js`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/ui/static/js/2.7fb734b4.chunk.js.LICENSE.txt` & `aaz-dev-1.1.0/src/aaz_dev/ui/static/js/2.7fb734b4.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/ui/static/js/2.7fb734b4.chunk.js.map` & `aaz-dev-1.1.0/src/aaz_dev/ui/static/js/2.7fb734b4.chunk.js.map`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/ui/static/js/main.90cd0227.chunk.js` & `aaz-dev-1.1.0/src/aaz_dev/ui/static/js/main.90cd0227.chunk.js`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/ui/static/js/main.90cd0227.chunk.js.map` & `aaz-dev-1.1.0/src/aaz_dev/ui/static/js/main.90cd0227.chunk.js.map`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/ui/static/js/runtime-main.f7313c7c.js` & `aaz-dev-1.1.0/src/aaz_dev/ui/static/js/runtime-main.f7313c7c.js`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/ui/static/js/runtime-main.f7313c7c.js.map` & `aaz-dev-1.1.0/src/aaz_dev/ui/static/js/runtime-main.f7313c7c.js.map`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/utils/config.py` & `aaz-dev-1.1.0/src/aaz_dev/utils/config.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/utils/error_format.py` & `aaz-dev-1.1.0/src/aaz_dev/utils/error_format.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/utils/exceptions.py` & `aaz-dev-1.1.0/src/aaz_dev/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/utils/plane.py` & `aaz-dev-1.1.0/src/aaz_dev/utils/plane.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/utils/portal_file_schema.py` & `aaz-dev-1.1.0/src/aaz_dev/utils/portal_file_schema.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev/utils/stage.py` & `aaz-dev-1.1.0/src/aaz_dev/utils/stage.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.0.2/src/aaz_dev.egg-info/PKG-INFO` & `aaz-dev-1.1.0/src/aaz_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aaz-dev
-Version: 1.0.2
+Version: 1.1.0
 Summary: Microsoft Atomic Azure CLI Commands Developer Tools
 Home-page: https://github.com/Azure/aaz-dev-tools
 Author: Microsoft Corporation
 Author-email: azpycli@microsoft.com
 License: MIT
 Keywords: azure
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aaz-dev-1.0.2/src/aaz_dev.egg-info/SOURCES.txt` & `aaz-dev-1.1.0/src/aaz_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

