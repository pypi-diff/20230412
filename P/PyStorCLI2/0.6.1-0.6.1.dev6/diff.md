# Comparing `tmp/PyStorCLI2-0.6.1.tar.gz` & `tmp/PyStorCLI2-0.6.1.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyStorCLI2-0.6.1.tar", last modified: Wed Apr 12 14:37:11 2023, max compression
+gzip compressed data, was "PyStorCLI2-0.6.1.dev6.tar", last modified: Mon Apr 10 09:50:00 2023, max compression
```

## Comparing `PyStorCLI2-0.6.1.tar` & `PyStorCLI2-0.6.1.dev6.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:37:11.358103 PyStorCLI2-0.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:37:11.342103 PyStorCLI2-0.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:37:11.346103 PyStorCLI2-0.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:37:11.346103 PyStorCLI2-0.6.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-12 14:37:11.358103 PyStorCLI2-0.6.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:37:11.346103 PyStorCLI2-0.6.1/PyStorCLI2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-12 14:37:11.000000 PyStorCLI2-0.6.1/PyStorCLI2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-12 14:37:11.000000 PyStorCLI2-0.6.1/PyStorCLI2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:37:11.000000 PyStorCLI2-0.6.1/PyStorCLI2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-12 14:37:11.000000 PyStorCLI2-0.6.1/PyStorCLI2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-12 14:37:11.000000 PyStorCLI2-0.6.1/PyStorCLI2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-12 14:37:11.000000 PyStorCLI2-0.6.1/PyStorCLI2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:37:11.346103 PyStorCLI2-0.6.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-12 14:36:44.000000 PyStorCLI2-0.6.1/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (123)   808879 2023-04-12 14:36:44.000000 PyStorCLI2-0.6.1/docs/pystorcli2.html
--rw-r--r--   0 runner    (1001) docker     (123)   351830 2023-04-12 14:36:44.000000 PyStorCLI2-0.6.1/docs/search.js
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:37:11.350103 PyStorCLI2-0.6.1/pystorcli/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/pystorcli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/pystorcli/cachevault.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/pystorcli/cmdRunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/pystorcli/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    16861 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/pystorcli/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    26664 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/pystorcli/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/pystorcli/enclosure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/pystorcli/exc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/pystorcli/storcli.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 14:37:11.000000 PyStorCLI2-0.6.1/pystorcli/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    23267 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/pystorcli/virtualdrive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:37:11.350103 PyStorCLI2-0.6.1/pystorcli2/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/pystorcli2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/pystorcli2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:37:11.350103 PyStorCLI2-0.6.1/pystorcli2/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/pystorcli2/bin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5262 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/pystorcli2/bin/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/pystorcli2/cachevault.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/pystorcli2/cmdRunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/pystorcli2/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    16861 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/pystorcli2/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    26664 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/pystorcli2/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/pystorcli2/enclosure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/pystorcli2/exc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/pystorcli2/storcli.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 14:37:11.000000 PyStorCLI2-0.6.1/pystorcli2/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    23267 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/pystorcli2/virtualdrive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:37:11.350103 PyStorCLI2-0.6.1/pystorcli_mirror/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/pystorcli_mirror/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 14:37:11.358103 PyStorCLI2-0.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:37:11.350103 PyStorCLI2-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/baseTest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:37:11.346103 PyStorCLI2-0.6.1/tests/datatest/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:37:11.346103 PyStorCLI2-0.6.1/tests/datatest/controllerSet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:37:11.350103 PyStorCLI2-0.6.1/tests/datatest/controllerSet/test00/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/controllerSet/test00/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/controllerSet/test00/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:37:11.354103 PyStorCLI2-0.6.1/tests/datatest/controllerSet/test01/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/controllerSet/test01/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/controllerSet/test01/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:37:11.354103 PyStorCLI2-0.6.1/tests/datatest/controllerSet/test02/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/controllerSet/test02/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/controllerSet/test02/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:37:11.354103 PyStorCLI2-0.6.1/tests/datatest/namedSet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:37:11.354103 PyStorCLI2-0.6.1/tests/datatest/namedSet/create_vd_raid0_00/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/create_vd_raid0_00/__c0_add_vd_r0_name=create_vd_raid0_drives=35_12-13_strip=512_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/create_vd_raid0_00/__c0_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/create_vd_raid0_00/__c0_v1_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/create_vd_raid0_00/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/create_vd_raid0_00/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:37:11.354103 PyStorCLI2-0.6.1/tests/datatest/namedSet/create_vd_raid1_00/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/create_vd_raid1_00/__c0_add_vd_r1_name=create_vd_raid1_drives=35_12-13_strip=512_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/create_vd_raid1_00/__c0_add_vd_r1_name=create_vd_raid1_drives=35_12-13_strip=512_PDperArray=2_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/create_vd_raid1_00/__c0_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/create_vd_raid1_00/__c0_v1_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/create_vd_raid1_00/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/create_vd_raid1_00/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:37:11.354103 PyStorCLI2-0.6.1/tests/datatest/namedSet/delete_vd_00/
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/delete_vd_00/__c0_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/delete_vd_00/__c0_v1_del_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/delete_vd_00/__c0_v1_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/delete_vd_00/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/delete_vd_00/device.json
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:37:11.354103 PyStorCLI2-0.6.1/tests/datatest/namedSet/set_state_offline_00/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/set_state_offline_00/__c0_e35_s12_set_offline_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/set_state_offline_00/__c0_e35_s12_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/set_state_offline_00/__c0_e35_sall_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/set_state_offline_00/__c0_e35_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/set_state_offline_00/__c0_eall_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/set_state_offline_00/__c0_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/set_state_offline_00/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/set_state_offline_00/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:37:11.354103 PyStorCLI2-0.6.1/tests/datatest/namedSet/show_events_00/
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/show_events_00/__c0_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/show_events_00/__c0_show_events_file=_root_raid_events.log_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/show_events_00/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/show_events_00/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:37:11.358103 PyStorCLI2-0.6.1/tests/datatest/namedSet/spindown_disk_00/
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/spindown_disk_00/__c0_e35_s12_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/spindown_disk_00/__c0_e35_s12_spindown_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/spindown_disk_00/__c0_e35_sall_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/spindown_disk_00/__c0_e35_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/spindown_disk_00/__c0_eall_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/spindown_disk_00/__c0_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/spindown_disk_00/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/namedSet/spindown_disk_00/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:37:11.346103 PyStorCLI2-0.6.1/tests/datatest/storcliSet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:37:11.358103 PyStorCLI2-0.6.1/tests/datatest/storcliSet/dummy/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/datatest/storcliSet/dummy/device.json
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/storclifile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/test_controllers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/test_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-12 14:36:30.000000 PyStorCLI2-0.6.1/tests/test_storcli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.841245 PyStorCLI2-0.6.1.dev6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.825245 PyStorCLI2-0.6.1.dev6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.829245 PyStorCLI2-0.6.1.dev6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.829245 PyStorCLI2-0.6.1.dev6/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-10 09:50:00.841245 PyStorCLI2-0.6.1.dev6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.829245 PyStorCLI2-0.6.1.dev6/PyStorCLI2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-10 09:50:00.000000 PyStorCLI2-0.6.1.dev6/PyStorCLI2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-10 09:50:00.000000 PyStorCLI2-0.6.1.dev6/PyStorCLI2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 09:50:00.000000 PyStorCLI2-0.6.1.dev6/PyStorCLI2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-10 09:50:00.000000 PyStorCLI2-0.6.1.dev6/PyStorCLI2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-10 09:50:00.000000 PyStorCLI2-0.6.1.dev6/PyStorCLI2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-10 09:50:00.000000 PyStorCLI2-0.6.1.dev6/PyStorCLI2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.833245 PyStorCLI2-0.6.1.dev6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-10 09:49:34.000000 PyStorCLI2-0.6.1.dev6/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)   751593 2023-04-10 09:49:34.000000 PyStorCLI2-0.6.1.dev6/docs/pystorcli2.html
+-rw-r--r--   0 runner    (1001) docker     (123)   331389 2023-04-10 09:49:34.000000 PyStorCLI2-0.6.1.dev6/docs/search.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.833245 PyStorCLI2-0.6.1.dev6/pystorcli/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli/cachevault.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli/cmdRunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11885 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26664 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli/enclosure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli/exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli/storcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-10 09:50:00.000000 PyStorCLI2-0.6.1.dev6/pystorcli/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23267 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli/virtualdrive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.833245 PyStorCLI2-0.6.1.dev6/pystorcli2/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.833245 PyStorCLI2-0.6.1.dev6/pystorcli2/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli2/bin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5262 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli2/bin/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli2/cachevault.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli2/cmdRunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli2/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11885 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli2/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26664 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli2/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli2/enclosure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli2/exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli2/storcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-10 09:50:00.000000 PyStorCLI2-0.6.1.dev6/pystorcli2/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23267 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli2/virtualdrive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.833245 PyStorCLI2-0.6.1.dev6/pystorcli_mirror/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/pystorcli_mirror/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 09:50:00.841245 PyStorCLI2-0.6.1.dev6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.837245 PyStorCLI2-0.6.1.dev6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/baseTest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.829245 PyStorCLI2-0.6.1.dev6/tests/datatest/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.829245 PyStorCLI2-0.6.1.dev6/tests/datatest/controllerSet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.837245 PyStorCLI2-0.6.1.dev6/tests/datatest/controllerSet/test00/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/controllerSet/test00/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/controllerSet/test00/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.837245 PyStorCLI2-0.6.1.dev6/tests/datatest/controllerSet/test01/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/controllerSet/test01/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/controllerSet/test01/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.837245 PyStorCLI2-0.6.1.dev6/tests/datatest/controllerSet/test02/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/controllerSet/test02/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/controllerSet/test02/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.837245 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.837245 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid0_00/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid0_00/__c0_add_vd_r0_name=create_vd_raid0_drives=35_12-13_strip=512_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid0_00/__c0_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid0_00/__c0_v1_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid0_00/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid0_00/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.837245 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid1_00/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid1_00/__c0_add_vd_r1_name=create_vd_raid1_drives=35_12-13_strip=512_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid1_00/__c0_add_vd_r1_name=create_vd_raid1_drives=35_12-13_strip=512_PDperArray=2_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid1_00/__c0_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid1_00/__c0_v1_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid1_00/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid1_00/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.837245 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/delete_vd_00/
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/delete_vd_00/__c0_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/delete_vd_00/__c0_v1_del_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/delete_vd_00/__c0_v1_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/delete_vd_00/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/delete_vd_00/device.json
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.841245 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/set_state_offline_00/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/set_state_offline_00/__c0_e35_s12_set_offline_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/set_state_offline_00/__c0_e35_s12_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/set_state_offline_00/__c0_e35_sall_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/set_state_offline_00/__c0_e35_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/set_state_offline_00/__c0_eall_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/set_state_offline_00/__c0_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/set_state_offline_00/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/set_state_offline_00/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.841245 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/show_events_00/
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/show_events_00/__c0_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/show_events_00/__c0_show_events_file=_root_raid_events.log_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/show_events_00/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/show_events_00/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.841245 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/spindown_disk_00/
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/spindown_disk_00/__c0_e35_s12_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/spindown_disk_00/__c0_e35_s12_spindown_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/spindown_disk_00/__c0_e35_sall_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/spindown_disk_00/__c0_e35_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/spindown_disk_00/__c0_eall_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/spindown_disk_00/__c0_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/spindown_disk_00/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/spindown_disk_00/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.829245 PyStorCLI2-0.6.1.dev6/tests/datatest/storcliSet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:50:00.841245 PyStorCLI2-0.6.1.dev6/tests/datatest/storcliSet/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/datatest/storcliSet/dummy/device.json
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/storclifile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/test_controllers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/test_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-10 09:49:16.000000 PyStorCLI2-0.6.1.dev6/tests/test_storcli.py
```

### Comparing `PyStorCLI2-0.6.1/.github/workflows/check.yml` & `PyStorCLI2-0.6.1.dev6/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/.github/workflows/publish-to-pypi.yml` & `PyStorCLI2-0.6.1.dev6/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/CHANGELOG.md` & `PyStorCLI2-0.6.1.dev6/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Version 0.6.1
 =============
 
 - **New features**:
   -----------------
   - [**Controller**]        Added method drives_ids to get all pair of enclosure:drive_id
-  - [**Controller**]        Added methods to handle patrol read and background initialization (PR [#9](https://github.com/Naudit/pystorcli2/pull/9))
-  - [**Controller**]        Added properties to get/set `autorebuild`,  `foreignautoimport` and `patrolread`. (PR [#9](https://github.com/Naudit/pystorcli2/pull/9))
 
 - **Fixes**:
   ----------
   - [**Controller**]        Fixed device count on controller.create_vd. Requested in [#2](https://github.com/Naudit/pystorcli2/issues/2)
   - [**Controller**]        Fixed default pd on controller.create_vd in some scenarios. Requested in [#2](https://github.com/Naudit/pystorcli2/issues/2)
 
 Version 0.6.0
```

### Comparing `PyStorCLI2-0.6.1/LICENSE` & `PyStorCLI2-0.6.1.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/PKG-INFO` & `PyStorCLI2-0.6.1.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyStorCLI2
-Version: 0.6.1
+Version: 0.6.1.dev6
 Summary: StorCLI module wrapper 2
 Author-email: Rafael Leira <rafael.leira@naudit.es>, Martin Dojcak <martin.dojcak@lablabs.io>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/Naudit/pystorcli2
 Keywords: storcli,wrapper
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `PyStorCLI2-0.6.1/PyStorCLI2.egg-info/PKG-INFO` & `PyStorCLI2-0.6.1.dev6/PyStorCLI2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyStorCLI2
-Version: 0.6.1
+Version: 0.6.1.dev6
 Summary: StorCLI module wrapper 2
 Author-email: Rafael Leira <rafael.leira@naudit.es>, Martin Dojcak <martin.dojcak@lablabs.io>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/Naudit/pystorcli2
 Keywords: storcli,wrapper
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `PyStorCLI2-0.6.1/PyStorCLI2.egg-info/SOURCES.txt` & `PyStorCLI2-0.6.1.dev6/PyStorCLI2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/README.md` & `PyStorCLI2-0.6.1.dev6/README.md`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/docs/pystorcli2.html` & `PyStorCLI2-0.6.1.dev6/docs/pystorcli2.html`

 * *Files 4% similar despite different names*

```diff
@@ -97,41 +97,14 @@
                         </li>
                         <li>
                                 <a class="variable" href="#Controller.drives_ids">drives_ids</a>
                         </li>
                         <li>
                                 <a class="function" href="#Controller.create_vd">create_vd</a>
                         </li>
-                        <li>
-                                <a class="variable" href="#Controller.autorebuild">autorebuild</a>
-                        </li>
-                        <li>
-                                <a class="variable" href="#Controller.foreignautoimport">foreignautoimport</a>
-                        </li>
-                        <li>
-                                <a class="variable" href="#Controller.patrolread">patrolread</a>
-                        </li>
-                        <li>
-                                <a class="function" href="#Controller.set_patrolread">set_patrolread</a>
-                        </li>
-                        <li>
-                                <a class="function" href="#Controller.patrolread_start">patrolread_start</a>
-                        </li>
-                        <li>
-                                <a class="function" href="#Controller.patrolread_stop">patrolread_stop</a>
-                        </li>
-                        <li>
-                                <a class="function" href="#Controller.patrolread_pause">patrolread_pause</a>
-                        </li>
-                        <li>
-                                <a class="function" href="#Controller.patrolread_resume">patrolread_resume</a>
-                        </li>
-                        <li>
-                                <a class="variable" href="#Controller.patrolread_running">patrolread_running</a>
-                        </li>
                 </ul>
 
             </li>
             <li>
                     <a class="class" href="#Controllers">Controllers</a>
                             <ul class="memberlist">
                         <li>
@@ -580,15 +553,15 @@
 </span></pre></div>
 
 
             </section>
                 <section id="__version__">
                     <div class="attr variable">
             <span class="name">__version__</span>        =
-<span class="default_value">&#39;0.6.1&#39;</span>
+<span class="default_value">&#39;0.6.1.dev6&#39;</span>
 
         
     </div>
     <a class="headerlink" href="#__version__"></a>
     
     
 
@@ -1302,339 +1275,152 @@
 </span><span id="Controller-197"><a href="#Controller-197"><span class="linenos">197</span></a><span class="sd">    Properties:</span>
 </span><span id="Controller-198"><a href="#Controller-198"><span class="linenos">198</span></a><span class="sd">        id (str): controller id</span>
 </span><span id="Controller-199"><a href="#Controller-199"><span class="linenos">199</span></a><span class="sd">        name (str): controller cmd name</span>
 </span><span id="Controller-200"><a href="#Controller-200"><span class="linenos">200</span></a><span class="sd">        facts (dict): raw controller facts</span>
 </span><span id="Controller-201"><a href="#Controller-201"><span class="linenos">201</span></a><span class="sd">        metrics (:obj:ControllerMetrics): controller metrics</span>
 </span><span id="Controller-202"><a href="#Controller-202"><span class="linenos">202</span></a><span class="sd">        vds (list of :obj:virtualdrive.VirtualDrives): controller virtual drives</span>
 </span><span id="Controller-203"><a href="#Controller-203"><span class="linenos">203</span></a><span class="sd">        encls (:obj:enclosure.Enclosures): controller enclosures</span>
-</span><span id="Controller-204"><a href="#Controller-204"><span class="linenos">204</span></a><span class="sd">        autorebuild (dict): current auto rebuild state (also setter)</span>
-</span><span id="Controller-205"><a href="#Controller-205"><span class="linenos">205</span></a><span class="sd">        foreignautoimport (dict): imports foreign configuration automatically at boot (also setter)</span>
-</span><span id="Controller-206"><a href="#Controller-206"><span class="linenos">206</span></a><span class="sd">        patrolread (dict): current patrol read settings (also setter)</span>
+</span><span id="Controller-204"><a href="#Controller-204"><span class="linenos">204</span></a>
+</span><span id="Controller-205"><a href="#Controller-205"><span class="linenos">205</span></a><span class="sd">    Methods:</span>
+</span><span id="Controller-206"><a href="#Controller-206"><span class="linenos">206</span></a><span class="sd">        create_vd (:obj:VirtualDrive): create virtual drive</span>
 </span><span id="Controller-207"><a href="#Controller-207"><span class="linenos">207</span></a>
-</span><span id="Controller-208"><a href="#Controller-208"><span class="linenos">208</span></a><span class="sd">    Methods:</span>
-</span><span id="Controller-209"><a href="#Controller-209"><span class="linenos">209</span></a><span class="sd">        create_vd (:obj:VirtualDrive): create virtual drive</span>
-</span><span id="Controller-210"><a href="#Controller-210"><span class="linenos">210</span></a><span class="sd">        set_patrolread (dict): configures patrol read state and schedule</span>
-</span><span id="Controller-211"><a href="#Controller-211"><span class="linenos">211</span></a><span class="sd">        patrolread_start (dict): starts a patrol read on controller</span>
-</span><span id="Controller-212"><a href="#Controller-212"><span class="linenos">212</span></a><span class="sd">        patrolread_pause (dict): pauses patrol read on controller</span>
-</span><span id="Controller-213"><a href="#Controller-213"><span class="linenos">213</span></a><span class="sd">        patrolread_resume (dict): resumes patrol read on controller</span>
-</span><span id="Controller-214"><a href="#Controller-214"><span class="linenos">214</span></a><span class="sd">        patrolread_stop (dict): stops patrol read if running on controller</span>
-</span><span id="Controller-215"><a href="#Controller-215"><span class="linenos">215</span></a><span class="sd">        patrolread_running (bool): check if patrol read is running on controller</span>
-</span><span id="Controller-216"><a href="#Controller-216"><span class="linenos">216</span></a>
-</span><span id="Controller-217"><a href="#Controller-217"><span class="linenos">217</span></a><span class="sd">    TODO:</span>
-</span><span id="Controller-218"><a href="#Controller-218"><span class="linenos">218</span></a><span class="sd">        Implement missing methods:</span>
-</span><span id="Controller-219"><a href="#Controller-219"><span class="linenos">219</span></a><span class="sd">            * patrol read progress</span>
-</span><span id="Controller-220"><a href="#Controller-220"><span class="linenos">220</span></a><span class="sd">    &quot;&quot;&quot;</span>
+</span><span id="Controller-208"><a href="#Controller-208"><span class="linenos">208</span></a><span class="sd">    &quot;&quot;&quot;</span>
+</span><span id="Controller-209"><a href="#Controller-209"><span class="linenos">209</span></a>
+</span><span id="Controller-210"><a href="#Controller-210"><span class="linenos">210</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">ctl_id</span><span class="p">,</span> <span class="n">binary</span><span class="o">=</span><span class="s1">&#39;storcli64&#39;</span><span class="p">):</span>
+</span><span id="Controller-211"><a href="#Controller-211"><span class="linenos">211</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Constructor - create StorCLI Controller object</span>
+</span><span id="Controller-212"><a href="#Controller-212"><span class="linenos">212</span></a>
+</span><span id="Controller-213"><a href="#Controller-213"><span class="linenos">213</span></a><span class="sd">        Args:</span>
+</span><span id="Controller-214"><a href="#Controller-214"><span class="linenos">214</span></a><span class="sd">            ctl_id (str): controller id</span>
+</span><span id="Controller-215"><a href="#Controller-215"><span class="linenos">215</span></a><span class="sd">            binary (str): storcli binary or full path to the binary</span>
+</span><span id="Controller-216"><a href="#Controller-216"><span class="linenos">216</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="Controller-217"><a href="#Controller-217"><span class="linenos">217</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_ctl_id</span> <span class="o">=</span> <span class="n">ctl_id</span>
+</span><span id="Controller-218"><a href="#Controller-218"><span class="linenos">218</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_binary</span> <span class="o">=</span> <span class="n">binary</span>
+</span><span id="Controller-219"><a href="#Controller-219"><span class="linenos">219</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_storcli</span> <span class="o">=</span> <span class="n">StorCLI</span><span class="p">(</span><span class="n">binary</span><span class="p">)</span>
+</span><span id="Controller-220"><a href="#Controller-220"><span class="linenos">220</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_name</span> <span class="o">=</span> <span class="s1">&#39;/c</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_ctl_id</span><span class="p">)</span>
 </span><span id="Controller-221"><a href="#Controller-221"><span class="linenos">221</span></a>
-</span><span id="Controller-222"><a href="#Controller-222"><span class="linenos">222</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">ctl_id</span><span class="p">,</span> <span class="n">binary</span><span class="o">=</span><span class="s1">&#39;storcli64&#39;</span><span class="p">):</span>
-</span><span id="Controller-223"><a href="#Controller-223"><span class="linenos">223</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Constructor - create StorCLI Controller object</span>
-</span><span id="Controller-224"><a href="#Controller-224"><span class="linenos">224</span></a>
-</span><span id="Controller-225"><a href="#Controller-225"><span class="linenos">225</span></a><span class="sd">        Args:</span>
-</span><span id="Controller-226"><a href="#Controller-226"><span class="linenos">226</span></a><span class="sd">            ctl_id (str): controller id</span>
-</span><span id="Controller-227"><a href="#Controller-227"><span class="linenos">227</span></a><span class="sd">            binary (str): storcli binary or full path to the binary</span>
-</span><span id="Controller-228"><a href="#Controller-228"><span class="linenos">228</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controller-229"><a href="#Controller-229"><span class="linenos">229</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_ctl_id</span> <span class="o">=</span> <span class="n">ctl_id</span>
-</span><span id="Controller-230"><a href="#Controller-230"><span class="linenos">230</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_binary</span> <span class="o">=</span> <span class="n">binary</span>
-</span><span id="Controller-231"><a href="#Controller-231"><span class="linenos">231</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_storcli</span> <span class="o">=</span> <span class="n">StorCLI</span><span class="p">(</span><span class="n">binary</span><span class="p">)</span>
-</span><span id="Controller-232"><a href="#Controller-232"><span class="linenos">232</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_name</span> <span class="o">=</span> <span class="s1">&#39;/c</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_ctl_id</span><span class="p">)</span>
-</span><span id="Controller-233"><a href="#Controller-233"><span class="linenos">233</span></a>
-</span><span id="Controller-234"><a href="#Controller-234"><span class="linenos">234</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_exist</span><span class="p">()</span>
-</span><span id="Controller-235"><a href="#Controller-235"><span class="linenos">235</span></a>
-</span><span id="Controller-236"><a href="#Controller-236"><span class="linenos">236</span></a>    <span class="k">def</span> <span class="fm">__str__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Controller-237"><a href="#Controller-237"><span class="linenos">237</span></a>        <span class="k">return</span> <span class="s1">&#39;</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">common</span><span class="o">.</span><span class="n">response_data</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">([</span><span class="s1">&#39;show&#39;</span><span class="p">])))</span>
+</span><span id="Controller-222"><a href="#Controller-222"><span class="linenos">222</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_exist</span><span class="p">()</span>
+</span><span id="Controller-223"><a href="#Controller-223"><span class="linenos">223</span></a>
+</span><span id="Controller-224"><a href="#Controller-224"><span class="linenos">224</span></a>    <span class="k">def</span> <span class="fm">__str__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Controller-225"><a href="#Controller-225"><span class="linenos">225</span></a>        <span class="k">return</span> <span class="s1">&#39;</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">common</span><span class="o">.</span><span class="n">response_data</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">([</span><span class="s1">&#39;show&#39;</span><span class="p">])))</span>
+</span><span id="Controller-226"><a href="#Controller-226"><span class="linenos">226</span></a>
+</span><span id="Controller-227"><a href="#Controller-227"><span class="linenos">227</span></a>    <span class="k">def</span> <span class="nf">_run</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">):</span>
+</span><span id="Controller-228"><a href="#Controller-228"><span class="linenos">228</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">args</span><span class="p">[:]</span>
+</span><span id="Controller-229"><a href="#Controller-229"><span class="linenos">229</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="p">)</span>
+</span><span id="Controller-230"><a href="#Controller-230"><span class="linenos">230</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_storcli</span><span class="o">.</span><span class="n">run</span><span class="p">(</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span>
+</span><span id="Controller-231"><a href="#Controller-231"><span class="linenos">231</span></a>
+</span><span id="Controller-232"><a href="#Controller-232"><span class="linenos">232</span></a>    <span class="k">def</span> <span class="nf">_exist</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Controller-233"><a href="#Controller-233"><span class="linenos">233</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="Controller-234"><a href="#Controller-234"><span class="linenos">234</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">([</span><span class="s1">&#39;show&#39;</span><span class="p">])</span>
+</span><span id="Controller-235"><a href="#Controller-235"><span class="linenos">235</span></a>        <span class="k">except</span> <span class="n">exc</span><span class="o">.</span><span class="n">StorCliCmdError</span><span class="p">:</span>
+</span><span id="Controller-236"><a href="#Controller-236"><span class="linenos">236</span></a>            <span class="k">raise</span> <span class="n">exc</span><span class="o">.</span><span class="n">StorCliMissingError</span><span class="p">(</span>
+</span><span id="Controller-237"><a href="#Controller-237"><span class="linenos">237</span></a>                <span class="bp">self</span><span class="o">.</span><span class="vm">__class__</span><span class="o">.</span><span class="vm">__name__</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="p">)</span> <span class="kn">from</span> <span class="bp">None</span>
 </span><span id="Controller-238"><a href="#Controller-238"><span class="linenos">238</span></a>
-</span><span id="Controller-239"><a href="#Controller-239"><span class="linenos">239</span></a>    <span class="k">def</span> <span class="nf">_run</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">):</span>
-</span><span id="Controller-240"><a href="#Controller-240"><span class="linenos">240</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">args</span><span class="p">[:]</span>
-</span><span id="Controller-241"><a href="#Controller-241"><span class="linenos">241</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="p">)</span>
-</span><span id="Controller-242"><a href="#Controller-242"><span class="linenos">242</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_storcli</span><span class="o">.</span><span class="n">run</span><span class="p">(</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span>
-</span><span id="Controller-243"><a href="#Controller-243"><span class="linenos">243</span></a>
-</span><span id="Controller-244"><a href="#Controller-244"><span class="linenos">244</span></a>    <span class="k">def</span> <span class="nf">_exist</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Controller-245"><a href="#Controller-245"><span class="linenos">245</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="Controller-246"><a href="#Controller-246"><span class="linenos">246</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">([</span><span class="s1">&#39;show&#39;</span><span class="p">])</span>
-</span><span id="Controller-247"><a href="#Controller-247"><span class="linenos">247</span></a>        <span class="k">except</span> <span class="n">exc</span><span class="o">.</span><span class="n">StorCliCmdError</span><span class="p">:</span>
-</span><span id="Controller-248"><a href="#Controller-248"><span class="linenos">248</span></a>            <span class="k">raise</span> <span class="n">exc</span><span class="o">.</span><span class="n">StorCliMissingError</span><span class="p">(</span>
-</span><span id="Controller-249"><a href="#Controller-249"><span class="linenos">249</span></a>                <span class="bp">self</span><span class="o">.</span><span class="vm">__class__</span><span class="o">.</span><span class="vm">__name__</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="p">)</span> <span class="kn">from</span> <span class="kc">None</span>
+</span><span id="Controller-239"><a href="#Controller-239"><span class="linenos">239</span></a>    <span class="nd">@property</span>
+</span><span id="Controller-240"><a href="#Controller-240"><span class="linenos">240</span></a>    <span class="k">def</span> <span class="nf">id</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Controller-241"><a href="#Controller-241"><span class="linenos">241</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot; (str): controller id</span>
+</span><span id="Controller-242"><a href="#Controller-242"><span class="linenos">242</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="Controller-243"><a href="#Controller-243"><span class="linenos">243</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_ctl_id</span>
+</span><span id="Controller-244"><a href="#Controller-244"><span class="linenos">244</span></a>
+</span><span id="Controller-245"><a href="#Controller-245"><span class="linenos">245</span></a>    <span class="nd">@property</span>
+</span><span id="Controller-246"><a href="#Controller-246"><span class="linenos">246</span></a>    <span class="k">def</span> <span class="nf">name</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Controller-247"><a href="#Controller-247"><span class="linenos">247</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot; (str): controller cmd name</span>
+</span><span id="Controller-248"><a href="#Controller-248"><span class="linenos">248</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="Controller-249"><a href="#Controller-249"><span class="linenos">249</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_name</span>
 </span><span id="Controller-250"><a href="#Controller-250"><span class="linenos">250</span></a>
 </span><span id="Controller-251"><a href="#Controller-251"><span class="linenos">251</span></a>    <span class="nd">@property</span>
-</span><span id="Controller-252"><a href="#Controller-252"><span class="linenos">252</span></a>    <span class="k">def</span> <span class="nf">id</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Controller-253"><a href="#Controller-253"><span class="linenos">253</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot; (str): controller id</span>
+</span><span id="Controller-252"><a href="#Controller-252"><span class="linenos">252</span></a>    <span class="k">def</span> <span class="nf">facts</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Controller-253"><a href="#Controller-253"><span class="linenos">253</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot; (dict): raw controller facts</span>
 </span><span id="Controller-254"><a href="#Controller-254"><span class="linenos">254</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controller-255"><a href="#Controller-255"><span class="linenos">255</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_ctl_id</span>
-</span><span id="Controller-256"><a href="#Controller-256"><span class="linenos">256</span></a>
-</span><span id="Controller-257"><a href="#Controller-257"><span class="linenos">257</span></a>    <span class="nd">@property</span>
-</span><span id="Controller-258"><a href="#Controller-258"><span class="linenos">258</span></a>    <span class="k">def</span> <span class="nf">name</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Controller-259"><a href="#Controller-259"><span class="linenos">259</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot; (str): controller cmd name</span>
-</span><span id="Controller-260"><a href="#Controller-260"><span class="linenos">260</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controller-261"><a href="#Controller-261"><span class="linenos">261</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_name</span>
-</span><span id="Controller-262"><a href="#Controller-262"><span class="linenos">262</span></a>
-</span><span id="Controller-263"><a href="#Controller-263"><span class="linenos">263</span></a>    <span class="nd">@property</span>
-</span><span id="Controller-264"><a href="#Controller-264"><span class="linenos">264</span></a>    <span class="k">def</span> <span class="nf">facts</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Controller-265"><a href="#Controller-265"><span class="linenos">265</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot; (dict): raw controller facts</span>
-</span><span id="Controller-266"><a href="#Controller-266"><span class="linenos">266</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controller-267"><a href="#Controller-267"><span class="linenos">267</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="Controller-268"><a href="#Controller-268"><span class="linenos">268</span></a>            <span class="s1">&#39;show&#39;</span><span class="p">,</span>
-</span><span id="Controller-269"><a href="#Controller-269"><span class="linenos">269</span></a>            <span class="s1">&#39;all&#39;</span>
-</span><span id="Controller-270"><a href="#Controller-270"><span class="linenos">270</span></a>        <span class="p">]</span>
-</span><span id="Controller-271"><a href="#Controller-271"><span class="linenos">271</span></a>        <span class="k">return</span> <span class="n">common</span><span class="o">.</span><span class="n">response_data</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span><span class="n">args</span><span class="p">))</span>
+</span><span id="Controller-255"><a href="#Controller-255"><span class="linenos">255</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="Controller-256"><a href="#Controller-256"><span class="linenos">256</span></a>            <span class="s1">&#39;show&#39;</span><span class="p">,</span>
+</span><span id="Controller-257"><a href="#Controller-257"><span class="linenos">257</span></a>            <span class="s1">&#39;all&#39;</span>
+</span><span id="Controller-258"><a href="#Controller-258"><span class="linenos">258</span></a>        <span class="p">]</span>
+</span><span id="Controller-259"><a href="#Controller-259"><span class="linenos">259</span></a>        <span class="k">return</span> <span class="n">common</span><span class="o">.</span><span class="n">response_data</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span><span class="n">args</span><span class="p">))</span>
+</span><span id="Controller-260"><a href="#Controller-260"><span class="linenos">260</span></a>
+</span><span id="Controller-261"><a href="#Controller-261"><span class="linenos">261</span></a>    <span class="nd">@property</span>
+</span><span id="Controller-262"><a href="#Controller-262"><span class="linenos">262</span></a>    <span class="k">def</span> <span class="nf">metrics</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Controller-263"><a href="#Controller-263"><span class="linenos">263</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;(:obj:ControllerMetrics): controller metrics</span>
+</span><span id="Controller-264"><a href="#Controller-264"><span class="linenos">264</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="Controller-265"><a href="#Controller-265"><span class="linenos">265</span></a>        <span class="k">return</span> <span class="n">ControllerMetrics</span><span class="p">(</span><span class="n">ctl</span><span class="o">=</span><span class="bp">self</span><span class="p">)</span>
+</span><span id="Controller-266"><a href="#Controller-266"><span class="linenos">266</span></a>
+</span><span id="Controller-267"><a href="#Controller-267"><span class="linenos">267</span></a>    <span class="nd">@property</span>
+</span><span id="Controller-268"><a href="#Controller-268"><span class="linenos">268</span></a>    <span class="k">def</span> <span class="nf">vds</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Controller-269"><a href="#Controller-269"><span class="linenos">269</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;(:obj:virtualdrive.VirtualDrives): controllers virtual drives</span>
+</span><span id="Controller-270"><a href="#Controller-270"><span class="linenos">270</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="Controller-271"><a href="#Controller-271"><span class="linenos">271</span></a>        <span class="k">return</span> <span class="n">virtualdrive</span><span class="o">.</span><span class="n">VirtualDrives</span><span class="p">(</span><span class="n">ctl_id</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_ctl_id</span><span class="p">,</span> <span class="n">binary</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_binary</span><span class="p">)</span>
 </span><span id="Controller-272"><a href="#Controller-272"><span class="linenos">272</span></a>
 </span><span id="Controller-273"><a href="#Controller-273"><span class="linenos">273</span></a>    <span class="nd">@property</span>
-</span><span id="Controller-274"><a href="#Controller-274"><span class="linenos">274</span></a>    <span class="k">def</span> <span class="nf">metrics</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Controller-275"><a href="#Controller-275"><span class="linenos">275</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;(:obj:ControllerMetrics): controller metrics</span>
+</span><span id="Controller-274"><a href="#Controller-274"><span class="linenos">274</span></a>    <span class="k">def</span> <span class="nf">encls</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Controller-275"><a href="#Controller-275"><span class="linenos">275</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;(:obj:enclosure.Enclosures): controller enclosures</span>
 </span><span id="Controller-276"><a href="#Controller-276"><span class="linenos">276</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controller-277"><a href="#Controller-277"><span class="linenos">277</span></a>        <span class="k">return</span> <span class="n">ControllerMetrics</span><span class="p">(</span><span class="n">ctl</span><span class="o">=</span><span class="bp">self</span><span class="p">)</span>
+</span><span id="Controller-277"><a href="#Controller-277"><span class="linenos">277</span></a>        <span class="k">return</span> <span class="n">enclosure</span><span class="o">.</span><span class="n">Enclosures</span><span class="p">(</span><span class="n">ctl_id</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_ctl_id</span><span class="p">,</span> <span class="n">binary</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_binary</span><span class="p">)</span>
 </span><span id="Controller-278"><a href="#Controller-278"><span class="linenos">278</span></a>
 </span><span id="Controller-279"><a href="#Controller-279"><span class="linenos">279</span></a>    <span class="nd">@property</span>
-</span><span id="Controller-280"><a href="#Controller-280"><span class="linenos">280</span></a>    <span class="k">def</span> <span class="nf">vds</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Controller-281"><a href="#Controller-281"><span class="linenos">281</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;(:obj:virtualdrive.VirtualDrives): controllers virtual drives</span>
+</span><span id="Controller-280"><a href="#Controller-280"><span class="linenos">280</span></a>    <span class="k">def</span> <span class="nf">drives_ids</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">List</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="Controller-281"><a href="#Controller-281"><span class="linenos">281</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;(list of str): list of drives ids in format (e:s)</span>
 </span><span id="Controller-282"><a href="#Controller-282"><span class="linenos">282</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controller-283"><a href="#Controller-283"><span class="linenos">283</span></a>        <span class="k">return</span> <span class="n">virtualdrive</span><span class="o">.</span><span class="n">VirtualDrives</span><span class="p">(</span><span class="n">ctl_id</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_ctl_id</span><span class="p">,</span> <span class="n">binary</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_binary</span><span class="p">)</span>
-</span><span id="Controller-284"><a href="#Controller-284"><span class="linenos">284</span></a>
-</span><span id="Controller-285"><a href="#Controller-285"><span class="linenos">285</span></a>    <span class="nd">@property</span>
-</span><span id="Controller-286"><a href="#Controller-286"><span class="linenos">286</span></a>    <span class="k">def</span> <span class="nf">encls</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Controller-287"><a href="#Controller-287"><span class="linenos">287</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;(:obj:enclosure.Enclosures): controller enclosures</span>
-</span><span id="Controller-288"><a href="#Controller-288"><span class="linenos">288</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controller-289"><a href="#Controller-289"><span class="linenos">289</span></a>        <span class="k">return</span> <span class="n">enclosure</span><span class="o">.</span><span class="n">Enclosures</span><span class="p">(</span><span class="n">ctl_id</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_ctl_id</span><span class="p">,</span> <span class="n">binary</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_binary</span><span class="p">)</span>
-</span><span id="Controller-290"><a href="#Controller-290"><span class="linenos">290</span></a>
-</span><span id="Controller-291"><a href="#Controller-291"><span class="linenos">291</span></a>    <span class="nd">@property</span>
-</span><span id="Controller-292"><a href="#Controller-292"><span class="linenos">292</span></a>    <span class="k">def</span> <span class="nf">drives_ids</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">List</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
-</span><span id="Controller-293"><a href="#Controller-293"><span class="linenos">293</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;(list of str): list of drives ids in format (e:s)</span>
-</span><span id="Controller-294"><a href="#Controller-294"><span class="linenos">294</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controller-295"><a href="#Controller-295"><span class="linenos">295</span></a>        <span class="n">drives</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="Controller-296"><a href="#Controller-296"><span class="linenos">296</span></a>        <span class="k">for</span> <span class="n">encl</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">encls</span><span class="p">:</span>
-</span><span id="Controller-297"><a href="#Controller-297"><span class="linenos">297</span></a>            <span class="k">for</span> <span class="nb">id</span> <span class="ow">in</span> <span class="n">encl</span><span class="o">.</span><span class="n">drives</span><span class="o">.</span><span class="n">ids</span><span class="p">:</span>
-</span><span id="Controller-298"><a href="#Controller-298"><span class="linenos">298</span></a>                <span class="n">drives</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;</span><span class="si">{enc}</span><span class="s2">:</span><span class="si">{id}</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">enc</span><span class="o">=</span><span class="n">encl</span><span class="o">.</span><span class="n">id</span><span class="p">,</span> <span class="nb">id</span><span class="o">=</span><span class="nb">id</span><span class="p">))</span>
-</span><span id="Controller-299"><a href="#Controller-299"><span class="linenos">299</span></a>
-</span><span id="Controller-300"><a href="#Controller-300"><span class="linenos">300</span></a>        <span class="k">return</span> <span class="n">drives</span>
-</span><span id="Controller-301"><a href="#Controller-301"><span class="linenos">301</span></a>
-</span><span id="Controller-302"><a href="#Controller-302"><span class="linenos">302</span></a>    <span class="k">def</span> <span class="nf">create_vd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">raid</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">drives</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">strip</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;64&#39;</span><span class="p">,</span> <span class="n">PDperArray</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">int</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Optional</span><span class="p">[</span><span class="n">virtualdrive</span><span class="o">.</span><span class="n">VirtualDrive</span><span class="p">]:</span>
-</span><span id="Controller-303"><a href="#Controller-303"><span class="linenos">303</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Create virtual drive (raid) managed by current controller</span>
-</span><span id="Controller-304"><a href="#Controller-304"><span class="linenos">304</span></a>
-</span><span id="Controller-305"><a href="#Controller-305"><span class="linenos">305</span></a><span class="sd">        Args:</span>
-</span><span id="Controller-306"><a href="#Controller-306"><span class="linenos">306</span></a><span class="sd">            name (str): virtual drive name</span>
-</span><span id="Controller-307"><a href="#Controller-307"><span class="linenos">307</span></a><span class="sd">            raid (str): virtual drive raid level (raid0, raid1, ...)</span>
-</span><span id="Controller-308"><a href="#Controller-308"><span class="linenos">308</span></a><span class="sd">            drives (str): storcli drives expression (e:s|e:s-x|e:s-x,y;e:s-x,y,z)</span>
-</span><span id="Controller-309"><a href="#Controller-309"><span class="linenos">309</span></a><span class="sd">            strip (str, optional): virtual drive raid strip size</span>
-</span><span id="Controller-310"><a href="#Controller-310"><span class="linenos">310</span></a>
-</span><span id="Controller-311"><a href="#Controller-311"><span class="linenos">311</span></a><span class="sd">        Returns:</span>
-</span><span id="Controller-312"><a href="#Controller-312"><span class="linenos">312</span></a><span class="sd">            (None): no virtual drive created with name</span>
-</span><span id="Controller-313"><a href="#Controller-313"><span class="linenos">313</span></a><span class="sd">            (:obj:virtualdrive.VirtualDrive)</span>
-</span><span id="Controller-314"><a href="#Controller-314"><span class="linenos">314</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controller-315"><a href="#Controller-315"><span class="linenos">315</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="Controller-316"><a href="#Controller-316"><span class="linenos">316</span></a>            <span class="s1">&#39;add&#39;</span><span class="p">,</span>
-</span><span id="Controller-317"><a href="#Controller-317"><span class="linenos">317</span></a>            <span class="s1">&#39;vd&#39;</span><span class="p">,</span>
-</span><span id="Controller-318"><a href="#Controller-318"><span class="linenos">318</span></a>            <span class="s1">&#39;r</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">raid</span><span class="p">),</span>
-</span><span id="Controller-319"><a href="#Controller-319"><span class="linenos">319</span></a>            <span class="s1">&#39;name=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">name</span><span class="p">),</span>
-</span><span id="Controller-320"><a href="#Controller-320"><span class="linenos">320</span></a>            <span class="s1">&#39;drives=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">drives</span><span class="p">),</span>
-</span><span id="Controller-321"><a href="#Controller-321"><span class="linenos">321</span></a>            <span class="s1">&#39;strip=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">strip</span><span class="p">)</span>
-</span><span id="Controller-322"><a href="#Controller-322"><span class="linenos">322</span></a>        <span class="p">]</span>
-</span><span id="Controller-323"><a href="#Controller-323"><span class="linenos">323</span></a>
-</span><span id="Controller-324"><a href="#Controller-324"><span class="linenos">324</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="Controller-325"><a href="#Controller-325"><span class="linenos">325</span></a>            <span class="k">if</span> <span class="nb">int</span><span class="p">(</span><span class="n">raid</span><span class="p">)</span> <span class="o">&gt;=</span> <span class="mi">10</span> <span class="ow">and</span> <span class="n">PDperArray</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="Controller-326"><a href="#Controller-326"><span class="linenos">326</span></a>                <span class="c1"># Try to count the number of drives in the array</span>
-</span><span id="Controller-327"><a href="#Controller-327"><span class="linenos">327</span></a>                <span class="c1"># The format of the drives argument is e:s|e:s-x|e:s-x,y;e:s-x,y,z</span>
-</span><span id="Controller-328"><a href="#Controller-328"><span class="linenos">328</span></a>
-</span><span id="Controller-329"><a href="#Controller-329"><span class="linenos">329</span></a>                <span class="n">numDrives</span> <span class="o">=</span> <span class="n">common</span><span class="o">.</span><span class="n">count_drives</span><span class="p">(</span><span class="n">drives</span><span class="p">)</span>
-</span><span id="Controller-330"><a href="#Controller-330"><span class="linenos">330</span></a>
-</span><span id="Controller-331"><a href="#Controller-331"><span class="linenos">331</span></a>                <span class="k">if</span> <span class="n">numDrives</span> <span class="o">%</span> <span class="mi">2</span> <span class="o">!=</span> <span class="mi">0</span> <span class="ow">and</span> <span class="n">numDrives</span> <span class="o">%</span> <span class="mi">3</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="Controller-332"><a href="#Controller-332"><span class="linenos">332</span></a>                    <span class="c1"># In some scenarios, such as 9 drives with raid 60, 3 is a good pd number but 4 is not</span>
-</span><span id="Controller-333"><a href="#Controller-333"><span class="linenos">333</span></a>                    <span class="c1"># Must check for similar scenarios</span>
-</span><span id="Controller-334"><a href="#Controller-334"><span class="linenos">334</span></a>                    <span class="c1"># BTW we don&#39;t clearly understand what PDperArray is for and what exactly it does under the hood. More investigation is needed</span>
-</span><span id="Controller-335"><a href="#Controller-335"><span class="linenos">335</span></a>                    <span class="n">PDperArray</span> <span class="o">=</span> <span class="n">numDrives</span><span class="o">//</span><span class="mi">3</span>
-</span><span id="Controller-336"><a href="#Controller-336"><span class="linenos">336</span></a>                <span class="k">else</span><span class="p">:</span>
-</span><span id="Controller-337"><a href="#Controller-337"><span class="linenos">337</span></a>                    <span class="n">PDperArray</span> <span class="o">=</span> <span class="n">numDrives</span><span class="o">//</span><span class="mi">2</span>
-</span><span id="Controller-338"><a href="#Controller-338"><span class="linenos">338</span></a>
-</span><span id="Controller-339"><a href="#Controller-339"><span class="linenos">339</span></a>        <span class="k">except</span> <span class="ne">ValueError</span><span class="p">:</span>
-</span><span id="Controller-340"><a href="#Controller-340"><span class="linenos">340</span></a>            <span class="k">pass</span>
-</span><span id="Controller-341"><a href="#Controller-341"><span class="linenos">341</span></a>
-</span><span id="Controller-342"><a href="#Controller-342"><span class="linenos">342</span></a>        <span class="k">finally</span><span class="p">:</span>
-</span><span id="Controller-343"><a href="#Controller-343"><span class="linenos">343</span></a>            <span class="k">if</span> <span class="n">raid</span> <span class="o">==</span> <span class="s1">&#39;00&#39;</span> <span class="ow">and</span> <span class="n">PDperArray</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="Controller-344"><a href="#Controller-344"><span class="linenos">344</span></a>                <span class="n">PDperArray</span> <span class="o">=</span> <span class="mi">1</span>
-</span><span id="Controller-345"><a href="#Controller-345"><span class="linenos">345</span></a>
-</span><span id="Controller-346"><a href="#Controller-346"><span class="linenos">346</span></a>        <span class="k">if</span> <span class="n">PDperArray</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="Controller-347"><a href="#Controller-347"><span class="linenos">347</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">&#39;PDperArray=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">PDperArray</span><span class="p">))</span>
-</span><span id="Controller-348"><a href="#Controller-348"><span class="linenos">348</span></a>
-</span><span id="Controller-349"><a href="#Controller-349"><span class="linenos">349</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
-</span><span id="Controller-350"><a href="#Controller-350"><span class="linenos">350</span></a>        <span class="k">for</span> <span class="n">vd</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">vds</span><span class="p">:</span>
-</span><span id="Controller-351"><a href="#Controller-351"><span class="linenos">351</span></a>            <span class="k">if</span> <span class="n">name</span> <span class="o">==</span> <span class="n">vd</span><span class="o">.</span><span class="n">name</span><span class="p">:</span>
-</span><span id="Controller-352"><a href="#Controller-352"><span class="linenos">352</span></a>                <span class="k">return</span> <span class="n">vd</span>
-</span><span id="Controller-353"><a href="#Controller-353"><span class="linenos">353</span></a>        <span class="k">return</span> <span class="kc">None</span>
-</span><span id="Controller-354"><a href="#Controller-354"><span class="linenos">354</span></a>
-</span><span id="Controller-355"><a href="#Controller-355"><span class="linenos">355</span></a>    <span class="nd">@property</span>
-</span><span id="Controller-356"><a href="#Controller-356"><span class="linenos">356</span></a>    <span class="nd">@common</span><span class="o">.</span><span class="n">lower</span>
-</span><span id="Controller-357"><a href="#Controller-357"><span class="linenos">357</span></a>    <span class="k">def</span> <span class="nf">autorebuild</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Controller-358"><a href="#Controller-358"><span class="linenos">358</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Get/Set auto rebuild state</span>
-</span><span id="Controller-359"><a href="#Controller-359"><span class="linenos">359</span></a>
-</span><span id="Controller-360"><a href="#Controller-360"><span class="linenos">360</span></a><span class="sd">        One of the following options can be set (str):</span>
-</span><span id="Controller-361"><a href="#Controller-361"><span class="linenos">361</span></a><span class="sd">            on - enables autorebuild</span>
-</span><span id="Controller-362"><a href="#Controller-362"><span class="linenos">362</span></a><span class="sd">            off - disables autorebuild</span>
-</span><span id="Controller-363"><a href="#Controller-363"><span class="linenos">363</span></a>
-</span><span id="Controller-364"><a href="#Controller-364"><span class="linenos">364</span></a><span class="sd">        Returns:</span>
-</span><span id="Controller-365"><a href="#Controller-365"><span class="linenos">365</span></a><span class="sd">            (str): on / off</span>
-</span><span id="Controller-366"><a href="#Controller-366"><span class="linenos">366</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controller-367"><a href="#Controller-367"><span class="linenos">367</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="Controller-368"><a href="#Controller-368"><span class="linenos">368</span></a>            <span class="s1">&#39;show&#39;</span><span class="p">,</span>
-</span><span id="Controller-369"><a href="#Controller-369"><span class="linenos">369</span></a>            <span class="s1">&#39;autorebuild&#39;</span>
-</span><span id="Controller-370"><a href="#Controller-370"><span class="linenos">370</span></a>        <span class="p">]</span>
-</span><span id="Controller-371"><a href="#Controller-371"><span class="linenos">371</span></a>
-</span><span id="Controller-372"><a href="#Controller-372"><span class="linenos">372</span></a>        <span class="n">prop</span> <span class="o">=</span> <span class="n">common</span><span class="o">.</span><span class="n">response_property</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span><span class="n">args</span><span class="p">))[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="Controller-373"><a href="#Controller-373"><span class="linenos">373</span></a>        <span class="k">return</span> <span class="n">prop</span><span class="p">[</span><span class="s1">&#39;Value&#39;</span><span class="p">]</span>
-</span><span id="Controller-374"><a href="#Controller-374"><span class="linenos">374</span></a>
-</span><span id="Controller-375"><a href="#Controller-375"><span class="linenos">375</span></a>    <span class="nd">@autorebuild</span><span class="o">.</span><span class="n">setter</span>
-</span><span id="Controller-376"><a href="#Controller-376"><span class="linenos">376</span></a>    <span class="k">def</span> <span class="nf">autorebuild</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">):</span>
-</span><span id="Controller-377"><a href="#Controller-377"><span class="linenos">377</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="Controller-378"><a href="#Controller-378"><span class="linenos">378</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controller-379"><a href="#Controller-379"><span class="linenos">379</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="Controller-380"><a href="#Controller-380"><span class="linenos">380</span></a>            <span class="s1">&#39;set&#39;</span><span class="p">,</span>
-</span><span id="Controller-381"><a href="#Controller-381"><span class="linenos">381</span></a>            <span class="s1">&#39;autorebuild=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
-</span><span id="Controller-382"><a href="#Controller-382"><span class="linenos">382</span></a>        <span class="p">]</span>
-</span><span id="Controller-383"><a href="#Controller-383"><span class="linenos">383</span></a>        <span class="k">return</span> <span class="n">common</span><span class="o">.</span><span class="n">response_setter</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span><span class="n">args</span><span class="p">))</span>
-</span><span id="Controller-384"><a href="#Controller-384"><span class="linenos">384</span></a>
-</span><span id="Controller-385"><a href="#Controller-385"><span class="linenos">385</span></a>    <span class="nd">@property</span>
-</span><span id="Controller-386"><a href="#Controller-386"><span class="linenos">386</span></a>    <span class="nd">@common</span><span class="o">.</span><span class="n">lower</span>
-</span><span id="Controller-387"><a href="#Controller-387"><span class="linenos">387</span></a>    <span class="k">def</span> <span class="nf">foreignautoimport</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Controller-388"><a href="#Controller-388"><span class="linenos">388</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Get/Set auto foreign import configuration</span>
-</span><span id="Controller-389"><a href="#Controller-389"><span class="linenos">389</span></a>
-</span><span id="Controller-390"><a href="#Controller-390"><span class="linenos">390</span></a><span class="sd">        One of the following options can be set (str):</span>
-</span><span id="Controller-391"><a href="#Controller-391"><span class="linenos">391</span></a><span class="sd">            on - enables foreignautoimport</span>
-</span><span id="Controller-392"><a href="#Controller-392"><span class="linenos">392</span></a><span class="sd">            off - disables foreignautoimport</span>
-</span><span id="Controller-393"><a href="#Controller-393"><span class="linenos">393</span></a>
-</span><span id="Controller-394"><a href="#Controller-394"><span class="linenos">394</span></a><span class="sd">        Returns:</span>
-</span><span id="Controller-395"><a href="#Controller-395"><span class="linenos">395</span></a><span class="sd">            (str): on / off</span>
-</span><span id="Controller-396"><a href="#Controller-396"><span class="linenos">396</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controller-397"><a href="#Controller-397"><span class="linenos">397</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="Controller-398"><a href="#Controller-398"><span class="linenos">398</span></a>            <span class="s1">&#39;show&#39;</span><span class="p">,</span>
-</span><span id="Controller-399"><a href="#Controller-399"><span class="linenos">399</span></a>            <span class="s1">&#39;foreignautoimport&#39;</span>
-</span><span id="Controller-400"><a href="#Controller-400"><span class="linenos">400</span></a>        <span class="p">]</span>
-</span><span id="Controller-401"><a href="#Controller-401"><span class="linenos">401</span></a>        <span class="n">prop</span> <span class="o">=</span> <span class="n">common</span><span class="o">.</span><span class="n">response_property</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span><span class="n">args</span><span class="p">))[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="Controller-402"><a href="#Controller-402"><span class="linenos">402</span></a>        <span class="k">return</span> <span class="n">prop</span><span class="p">[</span><span class="s1">&#39;Value&#39;</span><span class="p">]</span>
-</span><span id="Controller-403"><a href="#Controller-403"><span class="linenos">403</span></a>
-</span><span id="Controller-404"><a href="#Controller-404"><span class="linenos">404</span></a>    <span class="nd">@foreignautoimport</span><span class="o">.</span><span class="n">setter</span>
-</span><span id="Controller-405"><a href="#Controller-405"><span class="linenos">405</span></a>    <span class="k">def</span> <span class="nf">foreignautoimport</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">):</span>
-</span><span id="Controller-406"><a href="#Controller-406"><span class="linenos">406</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="Controller-407"><a href="#Controller-407"><span class="linenos">407</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controller-408"><a href="#Controller-408"><span class="linenos">408</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="Controller-409"><a href="#Controller-409"><span class="linenos">409</span></a>            <span class="s1">&#39;set&#39;</span><span class="p">,</span>
-</span><span id="Controller-410"><a href="#Controller-410"><span class="linenos">410</span></a>            <span class="s1">&#39;foreignautoimport=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
-</span><span id="Controller-411"><a href="#Controller-411"><span class="linenos">411</span></a>        <span class="p">]</span>
-</span><span id="Controller-412"><a href="#Controller-412"><span class="linenos">412</span></a>        <span class="k">return</span> <span class="n">common</span><span class="o">.</span><span class="n">response_setter</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span><span class="n">args</span><span class="p">))</span>
-</span><span id="Controller-413"><a href="#Controller-413"><span class="linenos">413</span></a>
-</span><span id="Controller-414"><a href="#Controller-414"><span class="linenos">414</span></a>    <span class="nd">@property</span>
-</span><span id="Controller-415"><a href="#Controller-415"><span class="linenos">415</span></a>    <span class="nd">@common</span><span class="o">.</span><span class="n">lower</span>
-</span><span id="Controller-416"><a href="#Controller-416"><span class="linenos">416</span></a>    <span class="k">def</span> <span class="nf">patrolread</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Controller-417"><a href="#Controller-417"><span class="linenos">417</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Get/Set patrol read</span>
-</span><span id="Controller-418"><a href="#Controller-418"><span class="linenos">418</span></a>
-</span><span id="Controller-419"><a href="#Controller-419"><span class="linenos">419</span></a><span class="sd">        One of the following options can be set (str):</span>
-</span><span id="Controller-420"><a href="#Controller-420"><span class="linenos">420</span></a><span class="sd">            on - enables patrol read</span>
-</span><span id="Controller-421"><a href="#Controller-421"><span class="linenos">421</span></a><span class="sd">            off - disables patrol read</span>
-</span><span id="Controller-422"><a href="#Controller-422"><span class="linenos">422</span></a>
-</span><span id="Controller-423"><a href="#Controller-423"><span class="linenos">423</span></a><span class="sd">        Returns:</span>
-</span><span id="Controller-424"><a href="#Controller-424"><span class="linenos">424</span></a><span class="sd">            (str): on / off</span>
-</span><span id="Controller-425"><a href="#Controller-425"><span class="linenos">425</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controller-426"><a href="#Controller-426"><span class="linenos">426</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="Controller-427"><a href="#Controller-427"><span class="linenos">427</span></a>            <span class="s1">&#39;show&#39;</span><span class="p">,</span>
-</span><span id="Controller-428"><a href="#Controller-428"><span class="linenos">428</span></a>            <span class="s1">&#39;patrolread&#39;</span>
-</span><span id="Controller-429"><a href="#Controller-429"><span class="linenos">429</span></a>        <span class="p">]</span>
-</span><span id="Controller-430"><a href="#Controller-430"><span class="linenos">430</span></a>
-</span><span id="Controller-431"><a href="#Controller-431"><span class="linenos">431</span></a>        <span class="k">for</span> <span class="n">pr</span> <span class="ow">in</span> <span class="n">common</span><span class="o">.</span><span class="n">response_property</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span><span class="n">args</span><span class="p">)):</span>
-</span><span id="Controller-432"><a href="#Controller-432"><span class="linenos">432</span></a>            <span class="k">if</span> <span class="n">pr</span><span class="p">[</span><span class="s1">&#39;Ctrl_Prop&#39;</span><span class="p">]</span> <span class="o">==</span> <span class="s2">&quot;PR Mode&quot;</span><span class="p">:</span>
-</span><span id="Controller-433"><a href="#Controller-433"><span class="linenos">433</span></a>                <span class="k">if</span> <span class="n">pr</span><span class="p">[</span><span class="s1">&#39;Value&#39;</span><span class="p">]</span> <span class="o">==</span> <span class="s1">&#39;Disable&#39;</span><span class="p">:</span>
-</span><span id="Controller-434"><a href="#Controller-434"><span class="linenos">434</span></a>                    <span class="k">return</span> <span class="s1">&#39;off&#39;</span>
-</span><span id="Controller-435"><a href="#Controller-435"><span class="linenos">435</span></a>                <span class="k">else</span><span class="p">:</span>
-</span><span id="Controller-436"><a href="#Controller-436"><span class="linenos">436</span></a>                    <span class="k">return</span> <span class="s1">&#39;on&#39;</span>
-</span><span id="Controller-437"><a href="#Controller-437"><span class="linenos">437</span></a>        <span class="k">return</span> <span class="s1">&#39;off&#39;</span>
-</span><span id="Controller-438"><a href="#Controller-438"><span class="linenos">438</span></a>
-</span><span id="Controller-439"><a href="#Controller-439"><span class="linenos">439</span></a>
-</span><span id="Controller-440"><a href="#Controller-440"><span class="linenos">440</span></a>    <span class="nd">@patrolread</span><span class="o">.</span><span class="n">setter</span>
-</span><span id="Controller-441"><a href="#Controller-441"><span class="linenos">441</span></a>    <span class="k">def</span> <span class="nf">patrolread</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">):</span>
-</span><span id="Controller-442"><a href="#Controller-442"><span class="linenos">442</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="Controller-443"><a href="#Controller-443"><span class="linenos">443</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controller-444"><a href="#Controller-444"><span class="linenos">444</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">set_patrolread</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
-</span><span id="Controller-445"><a href="#Controller-445"><span class="linenos">445</span></a>
-</span><span id="Controller-446"><a href="#Controller-446"><span class="linenos">446</span></a>
-</span><span id="Controller-447"><a href="#Controller-447"><span class="linenos">447</span></a>    <span class="k">def</span> <span class="nf">set_patrolread</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">,</span> <span class="n">mode</span><span class="o">=</span><span class="s1">&#39;manual&#39;</span><span class="p">):</span>
-</span><span id="Controller-448"><a href="#Controller-448"><span class="linenos">448</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Set patrol read</span>
-</span><span id="Controller-449"><a href="#Controller-449"><span class="linenos">449</span></a>
-</span><span id="Controller-450"><a href="#Controller-450"><span class="linenos">450</span></a><span class="sd">        Args:</span>
-</span><span id="Controller-451"><a href="#Controller-451"><span class="linenos">451</span></a><span class="sd">            value (str): on / off to configure patrol read state</span>
-</span><span id="Controller-452"><a href="#Controller-452"><span class="linenos">452</span></a><span class="sd">            mode (str): auto | manual to configure patrol read schedule</span>
-</span><span id="Controller-453"><a href="#Controller-453"><span class="linenos">453</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controller-454"><a href="#Controller-454"><span class="linenos">454</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="Controller-455"><a href="#Controller-455"><span class="linenos">455</span></a>            <span class="s1">&#39;set&#39;</span><span class="p">,</span>
-</span><span id="Controller-456"><a href="#Controller-456"><span class="linenos">456</span></a>            <span class="s1">&#39;patrolread=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
-</span><span id="Controller-457"><a href="#Controller-457"><span class="linenos">457</span></a>        <span class="p">]</span>
-</span><span id="Controller-458"><a href="#Controller-458"><span class="linenos">458</span></a>
-</span><span id="Controller-459"><a href="#Controller-459"><span class="linenos">459</span></a>        <span class="k">if</span> <span class="n">value</span> <span class="o">==</span> <span class="s1">&#39;on&#39;</span><span class="p">:</span>
-</span><span id="Controller-460"><a href="#Controller-460"><span class="linenos">460</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">&#39;mode=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">mode</span><span class="p">))</span>
-</span><span id="Controller-461"><a href="#Controller-461"><span class="linenos">461</span></a>
-</span><span id="Controller-462"><a href="#Controller-462"><span class="linenos">462</span></a>        <span class="k">return</span> <span class="n">common</span><span class="o">.</span><span class="n">response_setter</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span><span class="n">args</span><span class="p">))</span>
-</span><span id="Controller-463"><a href="#Controller-463"><span class="linenos">463</span></a>
-</span><span id="Controller-464"><a href="#Controller-464"><span class="linenos">464</span></a>    <span class="k">def</span> <span class="nf">patrolread_start</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Controller-465"><a href="#Controller-465"><span class="linenos">465</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Starts the patrol read operation of the controller</span>
-</span><span id="Controller-466"><a href="#Controller-466"><span class="linenos">466</span></a>
-</span><span id="Controller-467"><a href="#Controller-467"><span class="linenos">467</span></a><span class="sd">        Returns:</span>
-</span><span id="Controller-468"><a href="#Controller-468"><span class="linenos">468</span></a><span class="sd">            (dict): response cmd data</span>
-</span><span id="Controller-469"><a href="#Controller-469"><span class="linenos">469</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controller-470"><a href="#Controller-470"><span class="linenos">470</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="Controller-471"><a href="#Controller-471"><span class="linenos">471</span></a>            <span class="s1">&#39;start&#39;</span><span class="p">,</span>
-</span><span id="Controller-472"><a href="#Controller-472"><span class="linenos">472</span></a>            <span class="s1">&#39;patrolread&#39;</span>
-</span><span id="Controller-473"><a href="#Controller-473"><span class="linenos">473</span></a>        <span class="p">]</span>
-</span><span id="Controller-474"><a href="#Controller-474"><span class="linenos">474</span></a>        <span class="k">return</span> <span class="n">common</span><span class="o">.</span><span class="n">response_cmd</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span><span class="n">args</span><span class="p">))</span>
-</span><span id="Controller-475"><a href="#Controller-475"><span class="linenos">475</span></a>
-</span><span id="Controller-476"><a href="#Controller-476"><span class="linenos">476</span></a>    <span class="k">def</span> <span class="nf">patrolread_stop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Controller-477"><a href="#Controller-477"><span class="linenos">477</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Stops the patrol read operation of the controller</span>
-</span><span id="Controller-478"><a href="#Controller-478"><span class="linenos">478</span></a>
-</span><span id="Controller-479"><a href="#Controller-479"><span class="linenos">479</span></a><span class="sd">        Returns:</span>
-</span><span id="Controller-480"><a href="#Controller-480"><span class="linenos">480</span></a><span class="sd">            (dict): response cmd data</span>
-</span><span id="Controller-481"><a href="#Controller-481"><span class="linenos">481</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controller-482"><a href="#Controller-482"><span class="linenos">482</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="Controller-483"><a href="#Controller-483"><span class="linenos">483</span></a>            <span class="s1">&#39;stop&#39;</span><span class="p">,</span>
-</span><span id="Controller-484"><a href="#Controller-484"><span class="linenos">484</span></a>            <span class="s1">&#39;patrolread&#39;</span>
-</span><span id="Controller-485"><a href="#Controller-485"><span class="linenos">485</span></a>        <span class="p">]</span>
-</span><span id="Controller-486"><a href="#Controller-486"><span class="linenos">486</span></a>        <span class="k">return</span> <span class="n">common</span><span class="o">.</span><span class="n">response_cmd</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span><span class="n">args</span><span class="p">))</span>
-</span><span id="Controller-487"><a href="#Controller-487"><span class="linenos">487</span></a>
-</span><span id="Controller-488"><a href="#Controller-488"><span class="linenos">488</span></a>    <span class="k">def</span> <span class="nf">patrolread_pause</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Controller-489"><a href="#Controller-489"><span class="linenos">489</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Pauses the patrol read operation of the controller</span>
-</span><span id="Controller-490"><a href="#Controller-490"><span class="linenos">490</span></a>
-</span><span id="Controller-491"><a href="#Controller-491"><span class="linenos">491</span></a><span class="sd">        Returns:</span>
-</span><span id="Controller-492"><a href="#Controller-492"><span class="linenos">492</span></a><span class="sd">            (dict): response cmd data</span>
-</span><span id="Controller-493"><a href="#Controller-493"><span class="linenos">493</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controller-494"><a href="#Controller-494"><span class="linenos">494</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="Controller-495"><a href="#Controller-495"><span class="linenos">495</span></a>            <span class="s1">&#39;pause&#39;</span><span class="p">,</span>
-</span><span id="Controller-496"><a href="#Controller-496"><span class="linenos">496</span></a>            <span class="s1">&#39;patrolread&#39;</span>
-</span><span id="Controller-497"><a href="#Controller-497"><span class="linenos">497</span></a>        <span class="p">]</span>
-</span><span id="Controller-498"><a href="#Controller-498"><span class="linenos">498</span></a>        <span class="k">return</span> <span class="n">common</span><span class="o">.</span><span class="n">response_cmd</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span><span class="n">args</span><span class="p">))</span>
-</span><span id="Controller-499"><a href="#Controller-499"><span class="linenos">499</span></a>
-</span><span id="Controller-500"><a href="#Controller-500"><span class="linenos">500</span></a>    <span class="k">def</span> <span class="nf">patrolread_resume</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Controller-501"><a href="#Controller-501"><span class="linenos">501</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Resumes the patrol read operation of the controller</span>
-</span><span id="Controller-502"><a href="#Controller-502"><span class="linenos">502</span></a>
-</span><span id="Controller-503"><a href="#Controller-503"><span class="linenos">503</span></a><span class="sd">        Returns:</span>
-</span><span id="Controller-504"><a href="#Controller-504"><span class="linenos">504</span></a><span class="sd">            (dict): response cmd data</span>
-</span><span id="Controller-505"><a href="#Controller-505"><span class="linenos">505</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controller-506"><a href="#Controller-506"><span class="linenos">506</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="Controller-507"><a href="#Controller-507"><span class="linenos">507</span></a>            <span class="s1">&#39;resume&#39;</span><span class="p">,</span>
-</span><span id="Controller-508"><a href="#Controller-508"><span class="linenos">508</span></a>            <span class="s1">&#39;patrolread&#39;</span>
-</span><span id="Controller-509"><a href="#Controller-509"><span class="linenos">509</span></a>        <span class="p">]</span>
-</span><span id="Controller-510"><a href="#Controller-510"><span class="linenos">510</span></a>        <span class="k">return</span> <span class="n">common</span><span class="o">.</span><span class="n">response_cmd</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span><span class="n">args</span><span class="p">))</span>
-</span><span id="Controller-511"><a href="#Controller-511"><span class="linenos">511</span></a>
-</span><span id="Controller-512"><a href="#Controller-512"><span class="linenos">512</span></a>    <span class="nd">@property</span>
-</span><span id="Controller-513"><a href="#Controller-513"><span class="linenos">513</span></a>    <span class="k">def</span> <span class="nf">patrolread_running</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Controller-514"><a href="#Controller-514"><span class="linenos">514</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Check if patrol read is running on the controller</span>
-</span><span id="Controller-515"><a href="#Controller-515"><span class="linenos">515</span></a>
-</span><span id="Controller-516"><a href="#Controller-516"><span class="linenos">516</span></a><span class="sd">        Returns:</span>
-</span><span id="Controller-517"><a href="#Controller-517"><span class="linenos">517</span></a><span class="sd">            (bool): true / false</span>
-</span><span id="Controller-518"><a href="#Controller-518"><span class="linenos">518</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controller-519"><a href="#Controller-519"><span class="linenos">519</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="Controller-520"><a href="#Controller-520"><span class="linenos">520</span></a>            <span class="s1">&#39;show&#39;</span><span class="p">,</span>
-</span><span id="Controller-521"><a href="#Controller-521"><span class="linenos">521</span></a>            <span class="s1">&#39;patrolread&#39;</span>
-</span><span id="Controller-522"><a href="#Controller-522"><span class="linenos">522</span></a>        <span class="p">]</span>
-</span><span id="Controller-523"><a href="#Controller-523"><span class="linenos">523</span></a>
-</span><span id="Controller-524"><a href="#Controller-524"><span class="linenos">524</span></a>        <span class="n">status</span> <span class="o">=</span> <span class="s1">&#39;&#39;</span>
-</span><span id="Controller-525"><a href="#Controller-525"><span class="linenos">525</span></a>        <span class="k">for</span> <span class="n">pr</span> <span class="ow">in</span> <span class="n">common</span><span class="o">.</span><span class="n">response_property</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span><span class="n">args</span><span class="p">)):</span>
-</span><span id="Controller-526"><a href="#Controller-526"><span class="linenos">526</span></a>            <span class="k">if</span> <span class="n">pr</span><span class="p">[</span><span class="s1">&#39;Ctrl_Prop&#39;</span><span class="p">]</span> <span class="o">==</span> <span class="s2">&quot;PR Current State&quot;</span><span class="p">:</span>
-</span><span id="Controller-527"><a href="#Controller-527"><span class="linenos">527</span></a>                <span class="n">status</span> <span class="o">=</span> <span class="n">pr</span><span class="p">[</span><span class="s1">&#39;Value&#39;</span><span class="p">]</span>
-</span><span id="Controller-528"><a href="#Controller-528"><span class="linenos">528</span></a>        <span class="k">return</span> <span class="nb">bool</span><span class="p">(</span><span class="s1">&#39;Active&#39;</span> <span class="ow">in</span> <span class="n">status</span><span class="p">)</span>
+</span><span id="Controller-283"><a href="#Controller-283"><span class="linenos">283</span></a>        <span class="n">drives</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="Controller-284"><a href="#Controller-284"><span class="linenos">284</span></a>        <span class="k">for</span> <span class="n">encl</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">encls</span><span class="p">:</span>
+</span><span id="Controller-285"><a href="#Controller-285"><span class="linenos">285</span></a>            <span class="k">for</span> <span class="nb">id</span> <span class="ow">in</span> <span class="n">encl</span><span class="o">.</span><span class="n">drives</span><span class="o">.</span><span class="n">ids</span><span class="p">:</span>
+</span><span id="Controller-286"><a href="#Controller-286"><span class="linenos">286</span></a>                <span class="n">drives</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;</span><span class="si">{enc}</span><span class="s2">:</span><span class="si">{id}</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">enc</span><span class="o">=</span><span class="n">encl</span><span class="o">.</span><span class="n">id</span><span class="p">,</span> <span class="nb">id</span><span class="o">=</span><span class="nb">id</span><span class="p">))</span>
+</span><span id="Controller-287"><a href="#Controller-287"><span class="linenos">287</span></a>
+</span><span id="Controller-288"><a href="#Controller-288"><span class="linenos">288</span></a>        <span class="k">return</span> <span class="n">drives</span>
+</span><span id="Controller-289"><a href="#Controller-289"><span class="linenos">289</span></a>
+</span><span id="Controller-290"><a href="#Controller-290"><span class="linenos">290</span></a>    <span class="k">def</span> <span class="nf">create_vd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">raid</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">drives</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">strip</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;64&#39;</span><span class="p">,</span> <span class="n">PDperArray</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">int</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Optional</span><span class="p">[</span><span class="n">virtualdrive</span><span class="o">.</span><span class="n">VirtualDrive</span><span class="p">]:</span>
+</span><span id="Controller-291"><a href="#Controller-291"><span class="linenos">291</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Create virtual drive (raid) managed by current controller</span>
+</span><span id="Controller-292"><a href="#Controller-292"><span class="linenos">292</span></a>
+</span><span id="Controller-293"><a href="#Controller-293"><span class="linenos">293</span></a><span class="sd">        Args:</span>
+</span><span id="Controller-294"><a href="#Controller-294"><span class="linenos">294</span></a><span class="sd">            name (str): virtual drive name</span>
+</span><span id="Controller-295"><a href="#Controller-295"><span class="linenos">295</span></a><span class="sd">            raid (str): virtual drive raid level (raid0, raid1, ...)</span>
+</span><span id="Controller-296"><a href="#Controller-296"><span class="linenos">296</span></a><span class="sd">            drives (str): storcli drives expression (e:s|e:s-x|e:s-x,y;e:s-x,y,z)</span>
+</span><span id="Controller-297"><a href="#Controller-297"><span class="linenos">297</span></a><span class="sd">            strip (str, optional): virtual drive raid strip size</span>
+</span><span id="Controller-298"><a href="#Controller-298"><span class="linenos">298</span></a>
+</span><span id="Controller-299"><a href="#Controller-299"><span class="linenos">299</span></a><span class="sd">        Returns:</span>
+</span><span id="Controller-300"><a href="#Controller-300"><span class="linenos">300</span></a><span class="sd">            (None): no virtual drive created with name</span>
+</span><span id="Controller-301"><a href="#Controller-301"><span class="linenos">301</span></a><span class="sd">            (:obj:virtualdrive.VirtualDrive)</span>
+</span><span id="Controller-302"><a href="#Controller-302"><span class="linenos">302</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="Controller-303"><a href="#Controller-303"><span class="linenos">303</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="Controller-304"><a href="#Controller-304"><span class="linenos">304</span></a>            <span class="s1">&#39;add&#39;</span><span class="p">,</span>
+</span><span id="Controller-305"><a href="#Controller-305"><span class="linenos">305</span></a>            <span class="s1">&#39;vd&#39;</span><span class="p">,</span>
+</span><span id="Controller-306"><a href="#Controller-306"><span class="linenos">306</span></a>            <span class="s1">&#39;r</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">raid</span><span class="p">),</span>
+</span><span id="Controller-307"><a href="#Controller-307"><span class="linenos">307</span></a>            <span class="s1">&#39;name=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">name</span><span class="p">),</span>
+</span><span id="Controller-308"><a href="#Controller-308"><span class="linenos">308</span></a>            <span class="s1">&#39;drives=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">drives</span><span class="p">),</span>
+</span><span id="Controller-309"><a href="#Controller-309"><span class="linenos">309</span></a>            <span class="s1">&#39;strip=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">strip</span><span class="p">)</span>
+</span><span id="Controller-310"><a href="#Controller-310"><span class="linenos">310</span></a>        <span class="p">]</span>
+</span><span id="Controller-311"><a href="#Controller-311"><span class="linenos">311</span></a>
+</span><span id="Controller-312"><a href="#Controller-312"><span class="linenos">312</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="Controller-313"><a href="#Controller-313"><span class="linenos">313</span></a>            <span class="k">if</span> <span class="nb">int</span><span class="p">(</span><span class="n">raid</span><span class="p">)</span> <span class="o">&gt;=</span> <span class="mi">10</span> <span class="ow">and</span> <span class="n">PDperArray</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="Controller-314"><a href="#Controller-314"><span class="linenos">314</span></a>                <span class="c1"># Try to count the number of drives in the array</span>
+</span><span id="Controller-315"><a href="#Controller-315"><span class="linenos">315</span></a>                <span class="c1"># The format of the drives argument is e:s|e:s-x|e:s-x,y;e:s-x,y,z</span>
+</span><span id="Controller-316"><a href="#Controller-316"><span class="linenos">316</span></a>
+</span><span id="Controller-317"><a href="#Controller-317"><span class="linenos">317</span></a>                <span class="n">numDrives</span> <span class="o">=</span> <span class="n">common</span><span class="o">.</span><span class="n">count_drives</span><span class="p">(</span><span class="n">drives</span><span class="p">)</span>
+</span><span id="Controller-318"><a href="#Controller-318"><span class="linenos">318</span></a>
+</span><span id="Controller-319"><a href="#Controller-319"><span class="linenos">319</span></a>                <span class="k">if</span> <span class="n">numDrives</span> <span class="o">%</span> <span class="mi">2</span> <span class="o">!=</span> <span class="mi">0</span> <span class="ow">and</span> <span class="n">numDrives</span> <span class="o">%</span> <span class="mi">3</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="Controller-320"><a href="#Controller-320"><span class="linenos">320</span></a>                    <span class="c1"># In some scenarios, such as 9 drives with raid 60, 3 is a good pd number but 4 is not</span>
+</span><span id="Controller-321"><a href="#Controller-321"><span class="linenos">321</span></a>                    <span class="c1"># Must check for similar scenarios</span>
+</span><span id="Controller-322"><a href="#Controller-322"><span class="linenos">322</span></a>                    <span class="c1"># BTW we don&#39;t clearly understand what PDperArray is for and what exactly it does under the hood. More investigation is needed</span>
+</span><span id="Controller-323"><a href="#Controller-323"><span class="linenos">323</span></a>                    <span class="n">PDperArray</span> <span class="o">=</span> <span class="n">numDrives</span><span class="o">//</span><span class="mi">3</span>
+</span><span id="Controller-324"><a href="#Controller-324"><span class="linenos">324</span></a>                <span class="k">else</span><span class="p">:</span>
+</span><span id="Controller-325"><a href="#Controller-325"><span class="linenos">325</span></a>                    <span class="n">PDperArray</span> <span class="o">=</span> <span class="n">numDrives</span><span class="o">//</span><span class="mi">2</span>
+</span><span id="Controller-326"><a href="#Controller-326"><span class="linenos">326</span></a>
+</span><span id="Controller-327"><a href="#Controller-327"><span class="linenos">327</span></a>        <span class="k">except</span> <span class="ne">ValueError</span><span class="p">:</span>
+</span><span id="Controller-328"><a href="#Controller-328"><span class="linenos">328</span></a>            <span class="k">pass</span>
+</span><span id="Controller-329"><a href="#Controller-329"><span class="linenos">329</span></a>
+</span><span id="Controller-330"><a href="#Controller-330"><span class="linenos">330</span></a>        <span class="k">finally</span><span class="p">:</span>
+</span><span id="Controller-331"><a href="#Controller-331"><span class="linenos">331</span></a>            <span class="k">if</span> <span class="n">raid</span> <span class="o">==</span> <span class="s1">&#39;00&#39;</span> <span class="ow">and</span> <span class="n">PDperArray</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="Controller-332"><a href="#Controller-332"><span class="linenos">332</span></a>                <span class="n">PDperArray</span> <span class="o">=</span> <span class="mi">1</span>
+</span><span id="Controller-333"><a href="#Controller-333"><span class="linenos">333</span></a>
+</span><span id="Controller-334"><a href="#Controller-334"><span class="linenos">334</span></a>        <span class="k">if</span> <span class="n">PDperArray</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="Controller-335"><a href="#Controller-335"><span class="linenos">335</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">&#39;PDperArray=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">PDperArray</span><span class="p">))</span>
+</span><span id="Controller-336"><a href="#Controller-336"><span class="linenos">336</span></a>
+</span><span id="Controller-337"><a href="#Controller-337"><span class="linenos">337</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+</span><span id="Controller-338"><a href="#Controller-338"><span class="linenos">338</span></a>        <span class="k">for</span> <span class="n">vd</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">vds</span><span class="p">:</span>
+</span><span id="Controller-339"><a href="#Controller-339"><span class="linenos">339</span></a>            <span class="k">if</span> <span class="n">name</span> <span class="o">==</span> <span class="n">vd</span><span class="o">.</span><span class="n">name</span><span class="p">:</span>
+</span><span id="Controller-340"><a href="#Controller-340"><span class="linenos">340</span></a>                <span class="k">return</span> <span class="n">vd</span>
+</span><span id="Controller-341"><a href="#Controller-341"><span class="linenos">341</span></a>        <span class="k">return</span> <span class="kc">None</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>StorCLI Controller</p>
 
 <p>Instance of this class represents controller in StorCLI hierarchy</p>
 
@@ -1644,57 +1430,44 @@
 
 <p>Properties:
     id (str): controller id
     name (str): controller cmd name
     facts (dict): raw controller facts
     metrics (:obj:ControllerMetrics): controller metrics
     vds (list of :obj:virtualdrive.VirtualDrives): controller virtual drives
-    encls (:obj:enclosure.Enclosures): controller enclosures
-    autorebuild (dict): current auto rebuild state (also setter)
-    foreignautoimport (dict): imports foreign configuration automatically at boot (also setter)
-    patrolread (dict): current patrol read settings (also setter)</p>
+    encls (:obj:enclosure.Enclosures): controller enclosures</p>
 
 <p>Methods:
-    create_vd (:obj:VirtualDrive): create virtual drive
-    set_patrolread (dict): configures patrol read state and schedule
-    patrolread_start (dict): starts a patrol read on controller
-    patrolread_pause (dict): pauses patrol read on controller
-    patrolread_resume (dict): resumes patrol read on controller
-    patrolread_stop (dict): stops patrol read if running on controller
-    patrolread_running (bool): check if patrol read is running on controller</p>
-
-<p>TODO:
-    Implement missing methods:
-        * patrol read progress</p>
+    create_vd (:obj:VirtualDrive): create virtual drive</p>
 </div>
 
 
                             <div id="Controller.__init__" class="classattr">
                                         <input id="Controller.__init__-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="name">Controller</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">ctl_id</span>, </span><span class="param"><span class="n">binary</span><span class="o">=</span><span class="s1">&#39;storcli64&#39;</span></span>)</span>
 
                 <label class="view-source-button" for="Controller.__init__-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Controller.__init__"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Controller.__init__-222"><a href="#Controller.__init__-222"><span class="linenos">222</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">ctl_id</span><span class="p">,</span> <span class="n">binary</span><span class="o">=</span><span class="s1">&#39;storcli64&#39;</span><span class="p">):</span>
-</span><span id="Controller.__init__-223"><a href="#Controller.__init__-223"><span class="linenos">223</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Constructor - create StorCLI Controller object</span>
-</span><span id="Controller.__init__-224"><a href="#Controller.__init__-224"><span class="linenos">224</span></a>
-</span><span id="Controller.__init__-225"><a href="#Controller.__init__-225"><span class="linenos">225</span></a><span class="sd">        Args:</span>
-</span><span id="Controller.__init__-226"><a href="#Controller.__init__-226"><span class="linenos">226</span></a><span class="sd">            ctl_id (str): controller id</span>
-</span><span id="Controller.__init__-227"><a href="#Controller.__init__-227"><span class="linenos">227</span></a><span class="sd">            binary (str): storcli binary or full path to the binary</span>
-</span><span id="Controller.__init__-228"><a href="#Controller.__init__-228"><span class="linenos">228</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controller.__init__-229"><a href="#Controller.__init__-229"><span class="linenos">229</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_ctl_id</span> <span class="o">=</span> <span class="n">ctl_id</span>
-</span><span id="Controller.__init__-230"><a href="#Controller.__init__-230"><span class="linenos">230</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_binary</span> <span class="o">=</span> <span class="n">binary</span>
-</span><span id="Controller.__init__-231"><a href="#Controller.__init__-231"><span class="linenos">231</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_storcli</span> <span class="o">=</span> <span class="n">StorCLI</span><span class="p">(</span><span class="n">binary</span><span class="p">)</span>
-</span><span id="Controller.__init__-232"><a href="#Controller.__init__-232"><span class="linenos">232</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_name</span> <span class="o">=</span> <span class="s1">&#39;/c</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_ctl_id</span><span class="p">)</span>
-</span><span id="Controller.__init__-233"><a href="#Controller.__init__-233"><span class="linenos">233</span></a>
-</span><span id="Controller.__init__-234"><a href="#Controller.__init__-234"><span class="linenos">234</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_exist</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Controller.__init__-210"><a href="#Controller.__init__-210"><span class="linenos">210</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">ctl_id</span><span class="p">,</span> <span class="n">binary</span><span class="o">=</span><span class="s1">&#39;storcli64&#39;</span><span class="p">):</span>
+</span><span id="Controller.__init__-211"><a href="#Controller.__init__-211"><span class="linenos">211</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Constructor - create StorCLI Controller object</span>
+</span><span id="Controller.__init__-212"><a href="#Controller.__init__-212"><span class="linenos">212</span></a>
+</span><span id="Controller.__init__-213"><a href="#Controller.__init__-213"><span class="linenos">213</span></a><span class="sd">        Args:</span>
+</span><span id="Controller.__init__-214"><a href="#Controller.__init__-214"><span class="linenos">214</span></a><span class="sd">            ctl_id (str): controller id</span>
+</span><span id="Controller.__init__-215"><a href="#Controller.__init__-215"><span class="linenos">215</span></a><span class="sd">            binary (str): storcli binary or full path to the binary</span>
+</span><span id="Controller.__init__-216"><a href="#Controller.__init__-216"><span class="linenos">216</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="Controller.__init__-217"><a href="#Controller.__init__-217"><span class="linenos">217</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_ctl_id</span> <span class="o">=</span> <span class="n">ctl_id</span>
+</span><span id="Controller.__init__-218"><a href="#Controller.__init__-218"><span class="linenos">218</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_binary</span> <span class="o">=</span> <span class="n">binary</span>
+</span><span id="Controller.__init__-219"><a href="#Controller.__init__-219"><span class="linenos">219</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_storcli</span> <span class="o">=</span> <span class="n">StorCLI</span><span class="p">(</span><span class="n">binary</span><span class="p">)</span>
+</span><span id="Controller.__init__-220"><a href="#Controller.__init__-220"><span class="linenos">220</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_name</span> <span class="o">=</span> <span class="s1">&#39;/c</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_ctl_id</span><span class="p">)</span>
+</span><span id="Controller.__init__-221"><a href="#Controller.__init__-221"><span class="linenos">221</span></a>
+</span><span id="Controller.__init__-222"><a href="#Controller.__init__-222"><span class="linenos">222</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_exist</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Constructor - create StorCLI Controller object</p>
 
 <p>Args:
     ctl_id (str): controller id
@@ -1801,66 +1574,66 @@
         <span class="def">def</span>
         <span class="name">create_vd</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">name</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">raid</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">drives</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">strip</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;64&#39;</span>,</span><span class="param">	<span class="n">PDperArray</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">int</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">) -> <span class="n">Optional</span><span class="p">[</span><span class="n"><a href="#VirtualDrive">pystorcli2.VirtualDrive</a></span><span class="p">]</span>:</span></span>
 
                 <label class="view-source-button" for="Controller.create_vd-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Controller.create_vd"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Controller.create_vd-302"><a href="#Controller.create_vd-302"><span class="linenos">302</span></a>    <span class="k">def</span> <span class="nf">create_vd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">raid</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">drives</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">strip</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;64&#39;</span><span class="p">,</span> <span class="n">PDperArray</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">int</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Optional</span><span class="p">[</span><span class="n">virtualdrive</span><span class="o">.</span><span class="n">VirtualDrive</span><span class="p">]:</span>
-</span><span id="Controller.create_vd-303"><a href="#Controller.create_vd-303"><span class="linenos">303</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Create virtual drive (raid) managed by current controller</span>
-</span><span id="Controller.create_vd-304"><a href="#Controller.create_vd-304"><span class="linenos">304</span></a>
-</span><span id="Controller.create_vd-305"><a href="#Controller.create_vd-305"><span class="linenos">305</span></a><span class="sd">        Args:</span>
-</span><span id="Controller.create_vd-306"><a href="#Controller.create_vd-306"><span class="linenos">306</span></a><span class="sd">            name (str): virtual drive name</span>
-</span><span id="Controller.create_vd-307"><a href="#Controller.create_vd-307"><span class="linenos">307</span></a><span class="sd">            raid (str): virtual drive raid level (raid0, raid1, ...)</span>
-</span><span id="Controller.create_vd-308"><a href="#Controller.create_vd-308"><span class="linenos">308</span></a><span class="sd">            drives (str): storcli drives expression (e:s|e:s-x|e:s-x,y;e:s-x,y,z)</span>
-</span><span id="Controller.create_vd-309"><a href="#Controller.create_vd-309"><span class="linenos">309</span></a><span class="sd">            strip (str, optional): virtual drive raid strip size</span>
-</span><span id="Controller.create_vd-310"><a href="#Controller.create_vd-310"><span class="linenos">310</span></a>
-</span><span id="Controller.create_vd-311"><a href="#Controller.create_vd-311"><span class="linenos">311</span></a><span class="sd">        Returns:</span>
-</span><span id="Controller.create_vd-312"><a href="#Controller.create_vd-312"><span class="linenos">312</span></a><span class="sd">            (None): no virtual drive created with name</span>
-</span><span id="Controller.create_vd-313"><a href="#Controller.create_vd-313"><span class="linenos">313</span></a><span class="sd">            (:obj:virtualdrive.VirtualDrive)</span>
-</span><span id="Controller.create_vd-314"><a href="#Controller.create_vd-314"><span class="linenos">314</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controller.create_vd-315"><a href="#Controller.create_vd-315"><span class="linenos">315</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="Controller.create_vd-316"><a href="#Controller.create_vd-316"><span class="linenos">316</span></a>            <span class="s1">&#39;add&#39;</span><span class="p">,</span>
-</span><span id="Controller.create_vd-317"><a href="#Controller.create_vd-317"><span class="linenos">317</span></a>            <span class="s1">&#39;vd&#39;</span><span class="p">,</span>
-</span><span id="Controller.create_vd-318"><a href="#Controller.create_vd-318"><span class="linenos">318</span></a>            <span class="s1">&#39;r</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">raid</span><span class="p">),</span>
-</span><span id="Controller.create_vd-319"><a href="#Controller.create_vd-319"><span class="linenos">319</span></a>            <span class="s1">&#39;name=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">name</span><span class="p">),</span>
-</span><span id="Controller.create_vd-320"><a href="#Controller.create_vd-320"><span class="linenos">320</span></a>            <span class="s1">&#39;drives=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">drives</span><span class="p">),</span>
-</span><span id="Controller.create_vd-321"><a href="#Controller.create_vd-321"><span class="linenos">321</span></a>            <span class="s1">&#39;strip=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">strip</span><span class="p">)</span>
-</span><span id="Controller.create_vd-322"><a href="#Controller.create_vd-322"><span class="linenos">322</span></a>        <span class="p">]</span>
-</span><span id="Controller.create_vd-323"><a href="#Controller.create_vd-323"><span class="linenos">323</span></a>
-</span><span id="Controller.create_vd-324"><a href="#Controller.create_vd-324"><span class="linenos">324</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="Controller.create_vd-325"><a href="#Controller.create_vd-325"><span class="linenos">325</span></a>            <span class="k">if</span> <span class="nb">int</span><span class="p">(</span><span class="n">raid</span><span class="p">)</span> <span class="o">&gt;=</span> <span class="mi">10</span> <span class="ow">and</span> <span class="n">PDperArray</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="Controller.create_vd-326"><a href="#Controller.create_vd-326"><span class="linenos">326</span></a>                <span class="c1"># Try to count the number of drives in the array</span>
-</span><span id="Controller.create_vd-327"><a href="#Controller.create_vd-327"><span class="linenos">327</span></a>                <span class="c1"># The format of the drives argument is e:s|e:s-x|e:s-x,y;e:s-x,y,z</span>
-</span><span id="Controller.create_vd-328"><a href="#Controller.create_vd-328"><span class="linenos">328</span></a>
-</span><span id="Controller.create_vd-329"><a href="#Controller.create_vd-329"><span class="linenos">329</span></a>                <span class="n">numDrives</span> <span class="o">=</span> <span class="n">common</span><span class="o">.</span><span class="n">count_drives</span><span class="p">(</span><span class="n">drives</span><span class="p">)</span>
-</span><span id="Controller.create_vd-330"><a href="#Controller.create_vd-330"><span class="linenos">330</span></a>
-</span><span id="Controller.create_vd-331"><a href="#Controller.create_vd-331"><span class="linenos">331</span></a>                <span class="k">if</span> <span class="n">numDrives</span> <span class="o">%</span> <span class="mi">2</span> <span class="o">!=</span> <span class="mi">0</span> <span class="ow">and</span> <span class="n">numDrives</span> <span class="o">%</span> <span class="mi">3</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="Controller.create_vd-332"><a href="#Controller.create_vd-332"><span class="linenos">332</span></a>                    <span class="c1"># In some scenarios, such as 9 drives with raid 60, 3 is a good pd number but 4 is not</span>
-</span><span id="Controller.create_vd-333"><a href="#Controller.create_vd-333"><span class="linenos">333</span></a>                    <span class="c1"># Must check for similar scenarios</span>
-</span><span id="Controller.create_vd-334"><a href="#Controller.create_vd-334"><span class="linenos">334</span></a>                    <span class="c1"># BTW we don&#39;t clearly understand what PDperArray is for and what exactly it does under the hood. More investigation is needed</span>
-</span><span id="Controller.create_vd-335"><a href="#Controller.create_vd-335"><span class="linenos">335</span></a>                    <span class="n">PDperArray</span> <span class="o">=</span> <span class="n">numDrives</span><span class="o">//</span><span class="mi">3</span>
-</span><span id="Controller.create_vd-336"><a href="#Controller.create_vd-336"><span class="linenos">336</span></a>                <span class="k">else</span><span class="p">:</span>
-</span><span id="Controller.create_vd-337"><a href="#Controller.create_vd-337"><span class="linenos">337</span></a>                    <span class="n">PDperArray</span> <span class="o">=</span> <span class="n">numDrives</span><span class="o">//</span><span class="mi">2</span>
-</span><span id="Controller.create_vd-338"><a href="#Controller.create_vd-338"><span class="linenos">338</span></a>
-</span><span id="Controller.create_vd-339"><a href="#Controller.create_vd-339"><span class="linenos">339</span></a>        <span class="k">except</span> <span class="ne">ValueError</span><span class="p">:</span>
-</span><span id="Controller.create_vd-340"><a href="#Controller.create_vd-340"><span class="linenos">340</span></a>            <span class="k">pass</span>
-</span><span id="Controller.create_vd-341"><a href="#Controller.create_vd-341"><span class="linenos">341</span></a>
-</span><span id="Controller.create_vd-342"><a href="#Controller.create_vd-342"><span class="linenos">342</span></a>        <span class="k">finally</span><span class="p">:</span>
-</span><span id="Controller.create_vd-343"><a href="#Controller.create_vd-343"><span class="linenos">343</span></a>            <span class="k">if</span> <span class="n">raid</span> <span class="o">==</span> <span class="s1">&#39;00&#39;</span> <span class="ow">and</span> <span class="n">PDperArray</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="Controller.create_vd-344"><a href="#Controller.create_vd-344"><span class="linenos">344</span></a>                <span class="n">PDperArray</span> <span class="o">=</span> <span class="mi">1</span>
-</span><span id="Controller.create_vd-345"><a href="#Controller.create_vd-345"><span class="linenos">345</span></a>
-</span><span id="Controller.create_vd-346"><a href="#Controller.create_vd-346"><span class="linenos">346</span></a>        <span class="k">if</span> <span class="n">PDperArray</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="Controller.create_vd-347"><a href="#Controller.create_vd-347"><span class="linenos">347</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">&#39;PDperArray=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">PDperArray</span><span class="p">))</span>
-</span><span id="Controller.create_vd-348"><a href="#Controller.create_vd-348"><span class="linenos">348</span></a>
-</span><span id="Controller.create_vd-349"><a href="#Controller.create_vd-349"><span class="linenos">349</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
-</span><span id="Controller.create_vd-350"><a href="#Controller.create_vd-350"><span class="linenos">350</span></a>        <span class="k">for</span> <span class="n">vd</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">vds</span><span class="p">:</span>
-</span><span id="Controller.create_vd-351"><a href="#Controller.create_vd-351"><span class="linenos">351</span></a>            <span class="k">if</span> <span class="n">name</span> <span class="o">==</span> <span class="n">vd</span><span class="o">.</span><span class="n">name</span><span class="p">:</span>
-</span><span id="Controller.create_vd-352"><a href="#Controller.create_vd-352"><span class="linenos">352</span></a>                <span class="k">return</span> <span class="n">vd</span>
-</span><span id="Controller.create_vd-353"><a href="#Controller.create_vd-353"><span class="linenos">353</span></a>        <span class="k">return</span> <span class="kc">None</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Controller.create_vd-290"><a href="#Controller.create_vd-290"><span class="linenos">290</span></a>    <span class="k">def</span> <span class="nf">create_vd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">raid</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">drives</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">strip</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;64&#39;</span><span class="p">,</span> <span class="n">PDperArray</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">int</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Optional</span><span class="p">[</span><span class="n">virtualdrive</span><span class="o">.</span><span class="n">VirtualDrive</span><span class="p">]:</span>
+</span><span id="Controller.create_vd-291"><a href="#Controller.create_vd-291"><span class="linenos">291</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Create virtual drive (raid) managed by current controller</span>
+</span><span id="Controller.create_vd-292"><a href="#Controller.create_vd-292"><span class="linenos">292</span></a>
+</span><span id="Controller.create_vd-293"><a href="#Controller.create_vd-293"><span class="linenos">293</span></a><span class="sd">        Args:</span>
+</span><span id="Controller.create_vd-294"><a href="#Controller.create_vd-294"><span class="linenos">294</span></a><span class="sd">            name (str): virtual drive name</span>
+</span><span id="Controller.create_vd-295"><a href="#Controller.create_vd-295"><span class="linenos">295</span></a><span class="sd">            raid (str): virtual drive raid level (raid0, raid1, ...)</span>
+</span><span id="Controller.create_vd-296"><a href="#Controller.create_vd-296"><span class="linenos">296</span></a><span class="sd">            drives (str): storcli drives expression (e:s|e:s-x|e:s-x,y;e:s-x,y,z)</span>
+</span><span id="Controller.create_vd-297"><a href="#Controller.create_vd-297"><span class="linenos">297</span></a><span class="sd">            strip (str, optional): virtual drive raid strip size</span>
+</span><span id="Controller.create_vd-298"><a href="#Controller.create_vd-298"><span class="linenos">298</span></a>
+</span><span id="Controller.create_vd-299"><a href="#Controller.create_vd-299"><span class="linenos">299</span></a><span class="sd">        Returns:</span>
+</span><span id="Controller.create_vd-300"><a href="#Controller.create_vd-300"><span class="linenos">300</span></a><span class="sd">            (None): no virtual drive created with name</span>
+</span><span id="Controller.create_vd-301"><a href="#Controller.create_vd-301"><span class="linenos">301</span></a><span class="sd">            (:obj:virtualdrive.VirtualDrive)</span>
+</span><span id="Controller.create_vd-302"><a href="#Controller.create_vd-302"><span class="linenos">302</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="Controller.create_vd-303"><a href="#Controller.create_vd-303"><span class="linenos">303</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="Controller.create_vd-304"><a href="#Controller.create_vd-304"><span class="linenos">304</span></a>            <span class="s1">&#39;add&#39;</span><span class="p">,</span>
+</span><span id="Controller.create_vd-305"><a href="#Controller.create_vd-305"><span class="linenos">305</span></a>            <span class="s1">&#39;vd&#39;</span><span class="p">,</span>
+</span><span id="Controller.create_vd-306"><a href="#Controller.create_vd-306"><span class="linenos">306</span></a>            <span class="s1">&#39;r</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">raid</span><span class="p">),</span>
+</span><span id="Controller.create_vd-307"><a href="#Controller.create_vd-307"><span class="linenos">307</span></a>            <span class="s1">&#39;name=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">name</span><span class="p">),</span>
+</span><span id="Controller.create_vd-308"><a href="#Controller.create_vd-308"><span class="linenos">308</span></a>            <span class="s1">&#39;drives=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">drives</span><span class="p">),</span>
+</span><span id="Controller.create_vd-309"><a href="#Controller.create_vd-309"><span class="linenos">309</span></a>            <span class="s1">&#39;strip=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">strip</span><span class="p">)</span>
+</span><span id="Controller.create_vd-310"><a href="#Controller.create_vd-310"><span class="linenos">310</span></a>        <span class="p">]</span>
+</span><span id="Controller.create_vd-311"><a href="#Controller.create_vd-311"><span class="linenos">311</span></a>
+</span><span id="Controller.create_vd-312"><a href="#Controller.create_vd-312"><span class="linenos">312</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="Controller.create_vd-313"><a href="#Controller.create_vd-313"><span class="linenos">313</span></a>            <span class="k">if</span> <span class="nb">int</span><span class="p">(</span><span class="n">raid</span><span class="p">)</span> <span class="o">&gt;=</span> <span class="mi">10</span> <span class="ow">and</span> <span class="n">PDperArray</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="Controller.create_vd-314"><a href="#Controller.create_vd-314"><span class="linenos">314</span></a>                <span class="c1"># Try to count the number of drives in the array</span>
+</span><span id="Controller.create_vd-315"><a href="#Controller.create_vd-315"><span class="linenos">315</span></a>                <span class="c1"># The format of the drives argument is e:s|e:s-x|e:s-x,y;e:s-x,y,z</span>
+</span><span id="Controller.create_vd-316"><a href="#Controller.create_vd-316"><span class="linenos">316</span></a>
+</span><span id="Controller.create_vd-317"><a href="#Controller.create_vd-317"><span class="linenos">317</span></a>                <span class="n">numDrives</span> <span class="o">=</span> <span class="n">common</span><span class="o">.</span><span class="n">count_drives</span><span class="p">(</span><span class="n">drives</span><span class="p">)</span>
+</span><span id="Controller.create_vd-318"><a href="#Controller.create_vd-318"><span class="linenos">318</span></a>
+</span><span id="Controller.create_vd-319"><a href="#Controller.create_vd-319"><span class="linenos">319</span></a>                <span class="k">if</span> <span class="n">numDrives</span> <span class="o">%</span> <span class="mi">2</span> <span class="o">!=</span> <span class="mi">0</span> <span class="ow">and</span> <span class="n">numDrives</span> <span class="o">%</span> <span class="mi">3</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="Controller.create_vd-320"><a href="#Controller.create_vd-320"><span class="linenos">320</span></a>                    <span class="c1"># In some scenarios, such as 9 drives with raid 60, 3 is a good pd number but 4 is not</span>
+</span><span id="Controller.create_vd-321"><a href="#Controller.create_vd-321"><span class="linenos">321</span></a>                    <span class="c1"># Must check for similar scenarios</span>
+</span><span id="Controller.create_vd-322"><a href="#Controller.create_vd-322"><span class="linenos">322</span></a>                    <span class="c1"># BTW we don&#39;t clearly understand what PDperArray is for and what exactly it does under the hood. More investigation is needed</span>
+</span><span id="Controller.create_vd-323"><a href="#Controller.create_vd-323"><span class="linenos">323</span></a>                    <span class="n">PDperArray</span> <span class="o">=</span> <span class="n">numDrives</span><span class="o">//</span><span class="mi">3</span>
+</span><span id="Controller.create_vd-324"><a href="#Controller.create_vd-324"><span class="linenos">324</span></a>                <span class="k">else</span><span class="p">:</span>
+</span><span id="Controller.create_vd-325"><a href="#Controller.create_vd-325"><span class="linenos">325</span></a>                    <span class="n">PDperArray</span> <span class="o">=</span> <span class="n">numDrives</span><span class="o">//</span><span class="mi">2</span>
+</span><span id="Controller.create_vd-326"><a href="#Controller.create_vd-326"><span class="linenos">326</span></a>
+</span><span id="Controller.create_vd-327"><a href="#Controller.create_vd-327"><span class="linenos">327</span></a>        <span class="k">except</span> <span class="ne">ValueError</span><span class="p">:</span>
+</span><span id="Controller.create_vd-328"><a href="#Controller.create_vd-328"><span class="linenos">328</span></a>            <span class="k">pass</span>
+</span><span id="Controller.create_vd-329"><a href="#Controller.create_vd-329"><span class="linenos">329</span></a>
+</span><span id="Controller.create_vd-330"><a href="#Controller.create_vd-330"><span class="linenos">330</span></a>        <span class="k">finally</span><span class="p">:</span>
+</span><span id="Controller.create_vd-331"><a href="#Controller.create_vd-331"><span class="linenos">331</span></a>            <span class="k">if</span> <span class="n">raid</span> <span class="o">==</span> <span class="s1">&#39;00&#39;</span> <span class="ow">and</span> <span class="n">PDperArray</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="Controller.create_vd-332"><a href="#Controller.create_vd-332"><span class="linenos">332</span></a>                <span class="n">PDperArray</span> <span class="o">=</span> <span class="mi">1</span>
+</span><span id="Controller.create_vd-333"><a href="#Controller.create_vd-333"><span class="linenos">333</span></a>
+</span><span id="Controller.create_vd-334"><a href="#Controller.create_vd-334"><span class="linenos">334</span></a>        <span class="k">if</span> <span class="n">PDperArray</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="Controller.create_vd-335"><a href="#Controller.create_vd-335"><span class="linenos">335</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">&#39;PDperArray=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">PDperArray</span><span class="p">))</span>
+</span><span id="Controller.create_vd-336"><a href="#Controller.create_vd-336"><span class="linenos">336</span></a>
+</span><span id="Controller.create_vd-337"><a href="#Controller.create_vd-337"><span class="linenos">337</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+</span><span id="Controller.create_vd-338"><a href="#Controller.create_vd-338"><span class="linenos">338</span></a>        <span class="k">for</span> <span class="n">vd</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">vds</span><span class="p">:</span>
+</span><span id="Controller.create_vd-339"><a href="#Controller.create_vd-339"><span class="linenos">339</span></a>            <span class="k">if</span> <span class="n">name</span> <span class="o">==</span> <span class="n">vd</span><span class="o">.</span><span class="n">name</span><span class="p">:</span>
+</span><span id="Controller.create_vd-340"><a href="#Controller.create_vd-340"><span class="linenos">340</span></a>                <span class="k">return</span> <span class="n">vd</span>
+</span><span id="Controller.create_vd-341"><a href="#Controller.create_vd-341"><span class="linenos">341</span></a>        <span class="k">return</span> <span class="kc">None</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create virtual drive (raid) managed by current controller</p>
 
 <p>Args:
     name (str): virtual drive name
@@ -1871,314 +1644,88 @@
 <p>Returns:
     (None): no virtual drive created with name
     (:obj:virtualdrive.VirtualDrive)</p>
 </div>
 
 
                             </div>
-                            <div id="Controller.autorebuild" class="classattr">
-                                <div class="attr variable">
-            <span class="name">autorebuild</span>
-
-        
-    </div>
-    <a class="headerlink" href="#Controller.autorebuild"></a>
-    
-            <div class="docstring"><p>func effective wrapper</p>
-</div>
-
-
-                            </div>
-                            <div id="Controller.foreignautoimport" class="classattr">
-                                <div class="attr variable">
-            <span class="name">foreignautoimport</span>
-
-        
-    </div>
-    <a class="headerlink" href="#Controller.foreignautoimport"></a>
-    
-            <div class="docstring"><p>func effective wrapper</p>
-</div>
-
-
-                            </div>
-                            <div id="Controller.patrolread" class="classattr">
-                                <div class="attr variable">
-            <span class="name">patrolread</span>
-
-        
-    </div>
-    <a class="headerlink" href="#Controller.patrolread"></a>
-    
-            <div class="docstring"><p>func effective wrapper</p>
-</div>
-
-
-                            </div>
-                            <div id="Controller.set_patrolread" class="classattr">
-                                        <input id="Controller.set_patrolread-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
-<div class="attr function">
-            
-        <span class="def">def</span>
-        <span class="name">set_patrolread</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">value</span>, </span><span class="param"><span class="n">mode</span><span class="o">=</span><span class="s1">&#39;manual&#39;</span></span><span class="return-annotation">):</span></span>
-
-                <label class="view-source-button" for="Controller.set_patrolread-view-source"><span>View Source</span></label>
-
-    </div>
-    <a class="headerlink" href="#Controller.set_patrolread"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Controller.set_patrolread-447"><a href="#Controller.set_patrolread-447"><span class="linenos">447</span></a>    <span class="k">def</span> <span class="nf">set_patrolread</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">,</span> <span class="n">mode</span><span class="o">=</span><span class="s1">&#39;manual&#39;</span><span class="p">):</span>
-</span><span id="Controller.set_patrolread-448"><a href="#Controller.set_patrolread-448"><span class="linenos">448</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Set patrol read</span>
-</span><span id="Controller.set_patrolread-449"><a href="#Controller.set_patrolread-449"><span class="linenos">449</span></a>
-</span><span id="Controller.set_patrolread-450"><a href="#Controller.set_patrolread-450"><span class="linenos">450</span></a><span class="sd">        Args:</span>
-</span><span id="Controller.set_patrolread-451"><a href="#Controller.set_patrolread-451"><span class="linenos">451</span></a><span class="sd">            value (str): on / off to configure patrol read state</span>
-</span><span id="Controller.set_patrolread-452"><a href="#Controller.set_patrolread-452"><span class="linenos">452</span></a><span class="sd">            mode (str): auto | manual to configure patrol read schedule</span>
-</span><span id="Controller.set_patrolread-453"><a href="#Controller.set_patrolread-453"><span class="linenos">453</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controller.set_patrolread-454"><a href="#Controller.set_patrolread-454"><span class="linenos">454</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="Controller.set_patrolread-455"><a href="#Controller.set_patrolread-455"><span class="linenos">455</span></a>            <span class="s1">&#39;set&#39;</span><span class="p">,</span>
-</span><span id="Controller.set_patrolread-456"><a href="#Controller.set_patrolread-456"><span class="linenos">456</span></a>            <span class="s1">&#39;patrolread=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
-</span><span id="Controller.set_patrolread-457"><a href="#Controller.set_patrolread-457"><span class="linenos">457</span></a>        <span class="p">]</span>
-</span><span id="Controller.set_patrolread-458"><a href="#Controller.set_patrolread-458"><span class="linenos">458</span></a>
-</span><span id="Controller.set_patrolread-459"><a href="#Controller.set_patrolread-459"><span class="linenos">459</span></a>        <span class="k">if</span> <span class="n">value</span> <span class="o">==</span> <span class="s1">&#39;on&#39;</span><span class="p">:</span>
-</span><span id="Controller.set_patrolread-460"><a href="#Controller.set_patrolread-460"><span class="linenos">460</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s1">&#39;mode=</span><span class="si">{0}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">mode</span><span class="p">))</span>
-</span><span id="Controller.set_patrolread-461"><a href="#Controller.set_patrolread-461"><span class="linenos">461</span></a>
-</span><span id="Controller.set_patrolread-462"><a href="#Controller.set_patrolread-462"><span class="linenos">462</span></a>        <span class="k">return</span> <span class="n">common</span><span class="o">.</span><span class="n">response_setter</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span><span class="n">args</span><span class="p">))</span>
-</span></pre></div>
-
-
-            <div class="docstring"><p>Set patrol read</p>
-
-<p>Args:
-    value (str): on / off to configure patrol read state
-    mode (str): auto | manual to configure patrol read schedule</p>
-</div>
-
-
-                            </div>
-                            <div id="Controller.patrolread_start" class="classattr">
-                                        <input id="Controller.patrolread_start-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
-<div class="attr function">
-            
-        <span class="def">def</span>
-        <span class="name">patrolread_start</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
-
-                <label class="view-source-button" for="Controller.patrolread_start-view-source"><span>View Source</span></label>
-
-    </div>
-    <a class="headerlink" href="#Controller.patrolread_start"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Controller.patrolread_start-464"><a href="#Controller.patrolread_start-464"><span class="linenos">464</span></a>    <span class="k">def</span> <span class="nf">patrolread_start</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Controller.patrolread_start-465"><a href="#Controller.patrolread_start-465"><span class="linenos">465</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Starts the patrol read operation of the controller</span>
-</span><span id="Controller.patrolread_start-466"><a href="#Controller.patrolread_start-466"><span class="linenos">466</span></a>
-</span><span id="Controller.patrolread_start-467"><a href="#Controller.patrolread_start-467"><span class="linenos">467</span></a><span class="sd">        Returns:</span>
-</span><span id="Controller.patrolread_start-468"><a href="#Controller.patrolread_start-468"><span class="linenos">468</span></a><span class="sd">            (dict): response cmd data</span>
-</span><span id="Controller.patrolread_start-469"><a href="#Controller.patrolread_start-469"><span class="linenos">469</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controller.patrolread_start-470"><a href="#Controller.patrolread_start-470"><span class="linenos">470</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="Controller.patrolread_start-471"><a href="#Controller.patrolread_start-471"><span class="linenos">471</span></a>            <span class="s1">&#39;start&#39;</span><span class="p">,</span>
-</span><span id="Controller.patrolread_start-472"><a href="#Controller.patrolread_start-472"><span class="linenos">472</span></a>            <span class="s1">&#39;patrolread&#39;</span>
-</span><span id="Controller.patrolread_start-473"><a href="#Controller.patrolread_start-473"><span class="linenos">473</span></a>        <span class="p">]</span>
-</span><span id="Controller.patrolread_start-474"><a href="#Controller.patrolread_start-474"><span class="linenos">474</span></a>        <span class="k">return</span> <span class="n">common</span><span class="o">.</span><span class="n">response_cmd</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span><span class="n">args</span><span class="p">))</span>
-</span></pre></div>
-
-
-            <div class="docstring"><p>Starts the patrol read operation of the controller</p>
-
-<p>Returns:
-    (dict): response cmd data</p>
-</div>
-
-
-                            </div>
-                            <div id="Controller.patrolread_stop" class="classattr">
-                                        <input id="Controller.patrolread_stop-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
-<div class="attr function">
-            
-        <span class="def">def</span>
-        <span class="name">patrolread_stop</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
-
-                <label class="view-source-button" for="Controller.patrolread_stop-view-source"><span>View Source</span></label>
-
-    </div>
-    <a class="headerlink" href="#Controller.patrolread_stop"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Controller.patrolread_stop-476"><a href="#Controller.patrolread_stop-476"><span class="linenos">476</span></a>    <span class="k">def</span> <span class="nf">patrolread_stop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Controller.patrolread_stop-477"><a href="#Controller.patrolread_stop-477"><span class="linenos">477</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Stops the patrol read operation of the controller</span>
-</span><span id="Controller.patrolread_stop-478"><a href="#Controller.patrolread_stop-478"><span class="linenos">478</span></a>
-</span><span id="Controller.patrolread_stop-479"><a href="#Controller.patrolread_stop-479"><span class="linenos">479</span></a><span class="sd">        Returns:</span>
-</span><span id="Controller.patrolread_stop-480"><a href="#Controller.patrolread_stop-480"><span class="linenos">480</span></a><span class="sd">            (dict): response cmd data</span>
-</span><span id="Controller.patrolread_stop-481"><a href="#Controller.patrolread_stop-481"><span class="linenos">481</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controller.patrolread_stop-482"><a href="#Controller.patrolread_stop-482"><span class="linenos">482</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="Controller.patrolread_stop-483"><a href="#Controller.patrolread_stop-483"><span class="linenos">483</span></a>            <span class="s1">&#39;stop&#39;</span><span class="p">,</span>
-</span><span id="Controller.patrolread_stop-484"><a href="#Controller.patrolread_stop-484"><span class="linenos">484</span></a>            <span class="s1">&#39;patrolread&#39;</span>
-</span><span id="Controller.patrolread_stop-485"><a href="#Controller.patrolread_stop-485"><span class="linenos">485</span></a>        <span class="p">]</span>
-</span><span id="Controller.patrolread_stop-486"><a href="#Controller.patrolread_stop-486"><span class="linenos">486</span></a>        <span class="k">return</span> <span class="n">common</span><span class="o">.</span><span class="n">response_cmd</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span><span class="n">args</span><span class="p">))</span>
-</span></pre></div>
-
-
-            <div class="docstring"><p>Stops the patrol read operation of the controller</p>
-
-<p>Returns:
-    (dict): response cmd data</p>
-</div>
-
-
-                            </div>
-                            <div id="Controller.patrolread_pause" class="classattr">
-                                        <input id="Controller.patrolread_pause-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
-<div class="attr function">
-            
-        <span class="def">def</span>
-        <span class="name">patrolread_pause</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
-
-                <label class="view-source-button" for="Controller.patrolread_pause-view-source"><span>View Source</span></label>
-
-    </div>
-    <a class="headerlink" href="#Controller.patrolread_pause"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Controller.patrolread_pause-488"><a href="#Controller.patrolread_pause-488"><span class="linenos">488</span></a>    <span class="k">def</span> <span class="nf">patrolread_pause</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Controller.patrolread_pause-489"><a href="#Controller.patrolread_pause-489"><span class="linenos">489</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Pauses the patrol read operation of the controller</span>
-</span><span id="Controller.patrolread_pause-490"><a href="#Controller.patrolread_pause-490"><span class="linenos">490</span></a>
-</span><span id="Controller.patrolread_pause-491"><a href="#Controller.patrolread_pause-491"><span class="linenos">491</span></a><span class="sd">        Returns:</span>
-</span><span id="Controller.patrolread_pause-492"><a href="#Controller.patrolread_pause-492"><span class="linenos">492</span></a><span class="sd">            (dict): response cmd data</span>
-</span><span id="Controller.patrolread_pause-493"><a href="#Controller.patrolread_pause-493"><span class="linenos">493</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controller.patrolread_pause-494"><a href="#Controller.patrolread_pause-494"><span class="linenos">494</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="Controller.patrolread_pause-495"><a href="#Controller.patrolread_pause-495"><span class="linenos">495</span></a>            <span class="s1">&#39;pause&#39;</span><span class="p">,</span>
-</span><span id="Controller.patrolread_pause-496"><a href="#Controller.patrolread_pause-496"><span class="linenos">496</span></a>            <span class="s1">&#39;patrolread&#39;</span>
-</span><span id="Controller.patrolread_pause-497"><a href="#Controller.patrolread_pause-497"><span class="linenos">497</span></a>        <span class="p">]</span>
-</span><span id="Controller.patrolread_pause-498"><a href="#Controller.patrolread_pause-498"><span class="linenos">498</span></a>        <span class="k">return</span> <span class="n">common</span><span class="o">.</span><span class="n">response_cmd</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span><span class="n">args</span><span class="p">))</span>
-</span></pre></div>
-
-
-            <div class="docstring"><p>Pauses the patrol read operation of the controller</p>
-
-<p>Returns:
-    (dict): response cmd data</p>
-</div>
-
-
-                            </div>
-                            <div id="Controller.patrolread_resume" class="classattr">
-                                        <input id="Controller.patrolread_resume-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
-<div class="attr function">
-            
-        <span class="def">def</span>
-        <span class="name">patrolread_resume</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
-
-                <label class="view-source-button" for="Controller.patrolread_resume-view-source"><span>View Source</span></label>
-
-    </div>
-    <a class="headerlink" href="#Controller.patrolread_resume"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Controller.patrolread_resume-500"><a href="#Controller.patrolread_resume-500"><span class="linenos">500</span></a>    <span class="k">def</span> <span class="nf">patrolread_resume</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Controller.patrolread_resume-501"><a href="#Controller.patrolread_resume-501"><span class="linenos">501</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Resumes the patrol read operation of the controller</span>
-</span><span id="Controller.patrolread_resume-502"><a href="#Controller.patrolread_resume-502"><span class="linenos">502</span></a>
-</span><span id="Controller.patrolread_resume-503"><a href="#Controller.patrolread_resume-503"><span class="linenos">503</span></a><span class="sd">        Returns:</span>
-</span><span id="Controller.patrolread_resume-504"><a href="#Controller.patrolread_resume-504"><span class="linenos">504</span></a><span class="sd">            (dict): response cmd data</span>
-</span><span id="Controller.patrolread_resume-505"><a href="#Controller.patrolread_resume-505"><span class="linenos">505</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controller.patrolread_resume-506"><a href="#Controller.patrolread_resume-506"><span class="linenos">506</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="Controller.patrolread_resume-507"><a href="#Controller.patrolread_resume-507"><span class="linenos">507</span></a>            <span class="s1">&#39;resume&#39;</span><span class="p">,</span>
-</span><span id="Controller.patrolread_resume-508"><a href="#Controller.patrolread_resume-508"><span class="linenos">508</span></a>            <span class="s1">&#39;patrolread&#39;</span>
-</span><span id="Controller.patrolread_resume-509"><a href="#Controller.patrolread_resume-509"><span class="linenos">509</span></a>        <span class="p">]</span>
-</span><span id="Controller.patrolread_resume-510"><a href="#Controller.patrolread_resume-510"><span class="linenos">510</span></a>        <span class="k">return</span> <span class="n">common</span><span class="o">.</span><span class="n">response_cmd</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span><span class="n">args</span><span class="p">))</span>
-</span></pre></div>
-
-
-            <div class="docstring"><p>Resumes the patrol read operation of the controller</p>
-
-<p>Returns:
-    (dict): response cmd data</p>
-</div>
-
-
-                            </div>
-                            <div id="Controller.patrolread_running" class="classattr">
-                                <div class="attr variable">
-            <span class="name">patrolread_running</span>
-
-        
-    </div>
-    <a class="headerlink" href="#Controller.patrolread_running"></a>
-    
-            <div class="docstring"><p>Check if patrol read is running on the controller</p>
-
-<p>Returns:
-    (bool): true / false</p>
-</div>
-
-
-                            </div>
                 </section>
                 <section id="Controllers">
                             <input id="Controllers-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr class">
             
     <span class="def">class</span>
     <span class="name">Controllers</span>:
 
                 <label class="view-source-button" for="Controllers-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Controllers"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Controllers-531"><a href="#Controllers-531"><span class="linenos">531</span></a><span class="k">class</span> <span class="nc">Controllers</span><span class="p">(</span><span class="nb">object</span><span class="p">):</span>
-</span><span id="Controllers-532"><a href="#Controllers-532"><span class="linenos">532</span></a><span class="w">    </span><span class="sd">&quot;&quot;&quot;StorCLI Controllers</span>
-</span><span id="Controllers-533"><a href="#Controllers-533"><span class="linenos">533</span></a>
-</span><span id="Controllers-534"><a href="#Controllers-534"><span class="linenos">534</span></a><span class="sd">    Instance of this class is iterable with :obj:Controller as item</span>
-</span><span id="Controllers-535"><a href="#Controllers-535"><span class="linenos">535</span></a>
-</span><span id="Controllers-536"><a href="#Controllers-536"><span class="linenos">536</span></a><span class="sd">    Args:</span>
-</span><span id="Controllers-537"><a href="#Controllers-537"><span class="linenos">537</span></a><span class="sd">        binary (str): storcli binary or full path to the binary</span>
-</span><span id="Controllers-538"><a href="#Controllers-538"><span class="linenos">538</span></a>
-</span><span id="Controllers-539"><a href="#Controllers-539"><span class="linenos">539</span></a><span class="sd">    Properties:</span>
-</span><span id="Controllers-540"><a href="#Controllers-540"><span class="linenos">540</span></a><span class="sd">        ids (list of str): list of controllers id</span>
-</span><span id="Controllers-541"><a href="#Controllers-541"><span class="linenos">541</span></a>
-</span><span id="Controllers-542"><a href="#Controllers-542"><span class="linenos">542</span></a><span class="sd">    Methods:</span>
-</span><span id="Controllers-543"><a href="#Controllers-543"><span class="linenos">543</span></a><span class="sd">        get_clt (:obj:Controller): return controller object by id</span>
-</span><span id="Controllers-544"><a href="#Controllers-544"><span class="linenos">544</span></a><span class="sd">    &quot;&quot;&quot;</span>
-</span><span id="Controllers-545"><a href="#Controllers-545"><span class="linenos">545</span></a>
-</span><span id="Controllers-546"><a href="#Controllers-546"><span class="linenos">546</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">binary</span><span class="o">=</span><span class="s1">&#39;storcli64&#39;</span><span class="p">):</span>
-</span><span id="Controllers-547"><a href="#Controllers-547"><span class="linenos">547</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Constructor - create StorCLI Controllers object</span>
-</span><span id="Controllers-548"><a href="#Controllers-548"><span class="linenos">548</span></a>
-</span><span id="Controllers-549"><a href="#Controllers-549"><span class="linenos">549</span></a><span class="sd">        Args:</span>
-</span><span id="Controllers-550"><a href="#Controllers-550"><span class="linenos">550</span></a><span class="sd">            binary (str): storcli binary or full path to the binary</span>
-</span><span id="Controllers-551"><a href="#Controllers-551"><span class="linenos">551</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controllers-552"><a href="#Controllers-552"><span class="linenos">552</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_binary</span> <span class="o">=</span> <span class="n">binary</span>
-</span><span id="Controllers-553"><a href="#Controllers-553"><span class="linenos">553</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_storcli</span> <span class="o">=</span> <span class="n">StorCLI</span><span class="p">(</span><span class="n">binary</span><span class="p">)</span>
-</span><span id="Controllers-554"><a href="#Controllers-554"><span class="linenos">554</span></a>
-</span><span id="Controllers-555"><a href="#Controllers-555"><span class="linenos">555</span></a>    <span class="o">@</span> <span class="nb">property</span>
-</span><span id="Controllers-556"><a href="#Controllers-556"><span class="linenos">556</span></a>    <span class="k">def</span> <span class="nf">_ctl_ids</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">List</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
-</span><span id="Controllers-557"><a href="#Controllers-557"><span class="linenos">557</span></a>        <span class="n">out</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_storcli</span><span class="o">.</span><span class="n">run</span><span class="p">([</span><span class="s1">&#39;show&#39;</span><span class="p">])</span>
-</span><span id="Controllers-558"><a href="#Controllers-558"><span class="linenos">558</span></a>        <span class="n">response</span> <span class="o">=</span> <span class="n">common</span><span class="o">.</span><span class="n">response_data</span><span class="p">(</span><span class="n">out</span><span class="p">)</span>
-</span><span id="Controllers-559"><a href="#Controllers-559"><span class="linenos">559</span></a>
-</span><span id="Controllers-560"><a href="#Controllers-560"><span class="linenos">560</span></a>        <span class="k">if</span> <span class="s2">&quot;Number of Controllers&quot;</span> <span class="ow">in</span> <span class="n">response</span> <span class="ow">and</span> <span class="n">response</span><span class="p">[</span><span class="s2">&quot;Number of Controllers&quot;</span><span class="p">]</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="Controllers-561"><a href="#Controllers-561"><span class="linenos">561</span></a>            <span class="k">return</span> <span class="p">[]</span>
-</span><span id="Controllers-562"><a href="#Controllers-562"><span class="linenos">562</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="Controllers-563"><a href="#Controllers-563"><span class="linenos">563</span></a>            <span class="k">return</span> <span class="p">[</span><span class="n">ctl</span><span class="p">[</span><span class="s1">&#39;Ctl&#39;</span><span class="p">]</span> <span class="k">for</span> <span class="n">ctl</span> <span class="ow">in</span> <span class="n">common</span><span class="o">.</span><span class="n">response_data_subkey</span><span class="p">(</span><span class="n">out</span><span class="p">,</span> <span class="p">[</span><span class="s1">&#39;System Overview&#39;</span><span class="p">,</span> <span class="s1">&#39;IT System Overview&#39;</span><span class="p">])]</span>
-</span><span id="Controllers-564"><a href="#Controllers-564"><span class="linenos">564</span></a>
-</span><span id="Controllers-565"><a href="#Controllers-565"><span class="linenos">565</span></a>    <span class="o">@</span> <span class="nb">property</span>
-</span><span id="Controllers-566"><a href="#Controllers-566"><span class="linenos">566</span></a>    <span class="k">def</span> <span class="nf">_ctls</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Controllers-567"><a href="#Controllers-567"><span class="linenos">567</span></a>        <span class="k">for</span> <span class="n">ctl_id</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_ctl_ids</span><span class="p">:</span>
-</span><span id="Controllers-568"><a href="#Controllers-568"><span class="linenos">568</span></a>            <span class="k">yield</span> <span class="n">Controller</span><span class="p">(</span><span class="n">ctl_id</span><span class="o">=</span><span class="n">ctl_id</span><span class="p">,</span> <span class="n">binary</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_binary</span><span class="p">)</span>
-</span><span id="Controllers-569"><a href="#Controllers-569"><span class="linenos">569</span></a>
-</span><span id="Controllers-570"><a href="#Controllers-570"><span class="linenos">570</span></a>    <span class="k">def</span> <span class="fm">__iter__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Controllers-571"><a href="#Controllers-571"><span class="linenos">571</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_ctls</span>
-</span><span id="Controllers-572"><a href="#Controllers-572"><span class="linenos">572</span></a>
-</span><span id="Controllers-573"><a href="#Controllers-573"><span class="linenos">573</span></a>    <span class="o">@</span> <span class="nb">property</span>
-</span><span id="Controllers-574"><a href="#Controllers-574"><span class="linenos">574</span></a>    <span class="k">def</span> <span class="nf">ids</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Controllers-575"><a href="#Controllers-575"><span class="linenos">575</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;(list of str): controllers id</span>
-</span><span id="Controllers-576"><a href="#Controllers-576"><span class="linenos">576</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controllers-577"><a href="#Controllers-577"><span class="linenos">577</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_ctl_ids</span>
-</span><span id="Controllers-578"><a href="#Controllers-578"><span class="linenos">578</span></a>
-</span><span id="Controllers-579"><a href="#Controllers-579"><span class="linenos">579</span></a>    <span class="k">def</span> <span class="nf">get_ctl</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">ctl_id</span><span class="p">:</span> <span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Optional</span><span class="p">[</span><span class="n">Controller</span><span class="p">]:</span>
-</span><span id="Controllers-580"><a href="#Controllers-580"><span class="linenos">580</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Get controller object by id</span>
-</span><span id="Controllers-581"><a href="#Controllers-581"><span class="linenos">581</span></a>
-</span><span id="Controllers-582"><a href="#Controllers-582"><span class="linenos">582</span></a><span class="sd">        Args:</span>
-</span><span id="Controllers-583"><a href="#Controllers-583"><span class="linenos">583</span></a><span class="sd">            ctl_id (str): controller id</span>
-</span><span id="Controllers-584"><a href="#Controllers-584"><span class="linenos">584</span></a>
-</span><span id="Controllers-585"><a href="#Controllers-585"><span class="linenos">585</span></a><span class="sd">        Returns:</span>
-</span><span id="Controllers-586"><a href="#Controllers-586"><span class="linenos">586</span></a><span class="sd">            (None): no controller with id</span>
-</span><span id="Controllers-587"><a href="#Controllers-587"><span class="linenos">587</span></a><span class="sd">            (:obj:Controller): controller object</span>
-</span><span id="Controllers-588"><a href="#Controllers-588"><span class="linenos">588</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controllers-589"><a href="#Controllers-589"><span class="linenos">589</span></a>        <span class="k">for</span> <span class="n">ctl</span> <span class="ow">in</span> <span class="bp">self</span><span class="p">:</span>
-</span><span id="Controllers-590"><a href="#Controllers-590"><span class="linenos">590</span></a>            <span class="k">if</span> <span class="n">ctl</span><span class="o">.</span><span class="n">id</span> <span class="o">==</span> <span class="n">ctl_id</span><span class="p">:</span>
-</span><span id="Controllers-591"><a href="#Controllers-591"><span class="linenos">591</span></a>                <span class="k">return</span> <span class="n">ctl</span>
-</span><span id="Controllers-592"><a href="#Controllers-592"><span class="linenos">592</span></a>        <span class="k">return</span> <span class="kc">None</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Controllers-344"><a href="#Controllers-344"><span class="linenos">344</span></a><span class="k">class</span> <span class="nc">Controllers</span><span class="p">(</span><span class="nb">object</span><span class="p">):</span>
+</span><span id="Controllers-345"><a href="#Controllers-345"><span class="linenos">345</span></a><span class="w">    </span><span class="sd">&quot;&quot;&quot;StorCLI Controllers</span>
+</span><span id="Controllers-346"><a href="#Controllers-346"><span class="linenos">346</span></a>
+</span><span id="Controllers-347"><a href="#Controllers-347"><span class="linenos">347</span></a><span class="sd">    Instance of this class is iterable with :obj:Controller as item</span>
+</span><span id="Controllers-348"><a href="#Controllers-348"><span class="linenos">348</span></a>
+</span><span id="Controllers-349"><a href="#Controllers-349"><span class="linenos">349</span></a><span class="sd">    Args:</span>
+</span><span id="Controllers-350"><a href="#Controllers-350"><span class="linenos">350</span></a><span class="sd">        binary (str): storcli binary or full path to the binary</span>
+</span><span id="Controllers-351"><a href="#Controllers-351"><span class="linenos">351</span></a>
+</span><span id="Controllers-352"><a href="#Controllers-352"><span class="linenos">352</span></a><span class="sd">    Properties:</span>
+</span><span id="Controllers-353"><a href="#Controllers-353"><span class="linenos">353</span></a><span class="sd">        ids (list of str): list of controllers id</span>
+</span><span id="Controllers-354"><a href="#Controllers-354"><span class="linenos">354</span></a>
+</span><span id="Controllers-355"><a href="#Controllers-355"><span class="linenos">355</span></a><span class="sd">    Methods:</span>
+</span><span id="Controllers-356"><a href="#Controllers-356"><span class="linenos">356</span></a><span class="sd">        get_clt (:obj:Controller): return controller object by id</span>
+</span><span id="Controllers-357"><a href="#Controllers-357"><span class="linenos">357</span></a><span class="sd">    &quot;&quot;&quot;</span>
+</span><span id="Controllers-358"><a href="#Controllers-358"><span class="linenos">358</span></a>
+</span><span id="Controllers-359"><a href="#Controllers-359"><span class="linenos">359</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">binary</span><span class="o">=</span><span class="s1">&#39;storcli64&#39;</span><span class="p">):</span>
+</span><span id="Controllers-360"><a href="#Controllers-360"><span class="linenos">360</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Constructor - create StorCLI Controllers object</span>
+</span><span id="Controllers-361"><a href="#Controllers-361"><span class="linenos">361</span></a>
+</span><span id="Controllers-362"><a href="#Controllers-362"><span class="linenos">362</span></a><span class="sd">        Args:</span>
+</span><span id="Controllers-363"><a href="#Controllers-363"><span class="linenos">363</span></a><span class="sd">            binary (str): storcli binary or full path to the binary</span>
+</span><span id="Controllers-364"><a href="#Controllers-364"><span class="linenos">364</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="Controllers-365"><a href="#Controllers-365"><span class="linenos">365</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_binary</span> <span class="o">=</span> <span class="n">binary</span>
+</span><span id="Controllers-366"><a href="#Controllers-366"><span class="linenos">366</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_storcli</span> <span class="o">=</span> <span class="n">StorCLI</span><span class="p">(</span><span class="n">binary</span><span class="p">)</span>
+</span><span id="Controllers-367"><a href="#Controllers-367"><span class="linenos">367</span></a>
+</span><span id="Controllers-368"><a href="#Controllers-368"><span class="linenos">368</span></a>    <span class="o">@</span> <span class="nb">property</span>
+</span><span id="Controllers-369"><a href="#Controllers-369"><span class="linenos">369</span></a>    <span class="k">def</span> <span class="nf">_ctl_ids</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">List</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="Controllers-370"><a href="#Controllers-370"><span class="linenos">370</span></a>        <span class="n">out</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_storcli</span><span class="o">.</span><span class="n">run</span><span class="p">([</span><span class="s1">&#39;show&#39;</span><span class="p">])</span>
+</span><span id="Controllers-371"><a href="#Controllers-371"><span class="linenos">371</span></a>        <span class="n">response</span> <span class="o">=</span> <span class="n">common</span><span class="o">.</span><span class="n">response_data</span><span class="p">(</span><span class="n">out</span><span class="p">)</span>
+</span><span id="Controllers-372"><a href="#Controllers-372"><span class="linenos">372</span></a>
+</span><span id="Controllers-373"><a href="#Controllers-373"><span class="linenos">373</span></a>        <span class="k">if</span> <span class="s2">&quot;Number of Controllers&quot;</span> <span class="ow">in</span> <span class="n">response</span> <span class="ow">and</span> <span class="n">response</span><span class="p">[</span><span class="s2">&quot;Number of Controllers&quot;</span><span class="p">]</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="Controllers-374"><a href="#Controllers-374"><span class="linenos">374</span></a>            <span class="k">return</span> <span class="p">[]</span>
+</span><span id="Controllers-375"><a href="#Controllers-375"><span class="linenos">375</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="Controllers-376"><a href="#Controllers-376"><span class="linenos">376</span></a>            <span class="k">return</span> <span class="p">[</span><span class="n">ctl</span><span class="p">[</span><span class="s1">&#39;Ctl&#39;</span><span class="p">]</span> <span class="k">for</span> <span class="n">ctl</span> <span class="ow">in</span> <span class="n">common</span><span class="o">.</span><span class="n">response_data_subkey</span><span class="p">(</span><span class="n">out</span><span class="p">,</span> <span class="p">[</span><span class="s1">&#39;System Overview&#39;</span><span class="p">,</span> <span class="s1">&#39;IT System Overview&#39;</span><span class="p">])]</span>
+</span><span id="Controllers-377"><a href="#Controllers-377"><span class="linenos">377</span></a>
+</span><span id="Controllers-378"><a href="#Controllers-378"><span class="linenos">378</span></a>    <span class="o">@</span> <span class="nb">property</span>
+</span><span id="Controllers-379"><a href="#Controllers-379"><span class="linenos">379</span></a>    <span class="k">def</span> <span class="nf">_ctls</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Controllers-380"><a href="#Controllers-380"><span class="linenos">380</span></a>        <span class="k">for</span> <span class="n">ctl_id</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_ctl_ids</span><span class="p">:</span>
+</span><span id="Controllers-381"><a href="#Controllers-381"><span class="linenos">381</span></a>            <span class="k">yield</span> <span class="n">Controller</span><span class="p">(</span><span class="n">ctl_id</span><span class="o">=</span><span class="n">ctl_id</span><span class="p">,</span> <span class="n">binary</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_binary</span><span class="p">)</span>
+</span><span id="Controllers-382"><a href="#Controllers-382"><span class="linenos">382</span></a>
+</span><span id="Controllers-383"><a href="#Controllers-383"><span class="linenos">383</span></a>    <span class="k">def</span> <span class="fm">__iter__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Controllers-384"><a href="#Controllers-384"><span class="linenos">384</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_ctls</span>
+</span><span id="Controllers-385"><a href="#Controllers-385"><span class="linenos">385</span></a>
+</span><span id="Controllers-386"><a href="#Controllers-386"><span class="linenos">386</span></a>    <span class="o">@</span> <span class="nb">property</span>
+</span><span id="Controllers-387"><a href="#Controllers-387"><span class="linenos">387</span></a>    <span class="k">def</span> <span class="nf">ids</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Controllers-388"><a href="#Controllers-388"><span class="linenos">388</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;(list of str): controllers id</span>
+</span><span id="Controllers-389"><a href="#Controllers-389"><span class="linenos">389</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="Controllers-390"><a href="#Controllers-390"><span class="linenos">390</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_ctl_ids</span>
+</span><span id="Controllers-391"><a href="#Controllers-391"><span class="linenos">391</span></a>
+</span><span id="Controllers-392"><a href="#Controllers-392"><span class="linenos">392</span></a>    <span class="k">def</span> <span class="nf">get_ctl</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">ctl_id</span><span class="p">:</span> <span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Optional</span><span class="p">[</span><span class="n">Controller</span><span class="p">]:</span>
+</span><span id="Controllers-393"><a href="#Controllers-393"><span class="linenos">393</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Get controller object by id</span>
+</span><span id="Controllers-394"><a href="#Controllers-394"><span class="linenos">394</span></a>
+</span><span id="Controllers-395"><a href="#Controllers-395"><span class="linenos">395</span></a><span class="sd">        Args:</span>
+</span><span id="Controllers-396"><a href="#Controllers-396"><span class="linenos">396</span></a><span class="sd">            ctl_id (str): controller id</span>
+</span><span id="Controllers-397"><a href="#Controllers-397"><span class="linenos">397</span></a>
+</span><span id="Controllers-398"><a href="#Controllers-398"><span class="linenos">398</span></a><span class="sd">        Returns:</span>
+</span><span id="Controllers-399"><a href="#Controllers-399"><span class="linenos">399</span></a><span class="sd">            (None): no controller with id</span>
+</span><span id="Controllers-400"><a href="#Controllers-400"><span class="linenos">400</span></a><span class="sd">            (:obj:Controller): controller object</span>
+</span><span id="Controllers-401"><a href="#Controllers-401"><span class="linenos">401</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="Controllers-402"><a href="#Controllers-402"><span class="linenos">402</span></a>        <span class="k">for</span> <span class="n">ctl</span> <span class="ow">in</span> <span class="bp">self</span><span class="p">:</span>
+</span><span id="Controllers-403"><a href="#Controllers-403"><span class="linenos">403</span></a>            <span class="k">if</span> <span class="n">ctl</span><span class="o">.</span><span class="n">id</span> <span class="o">==</span> <span class="n">ctl_id</span><span class="p">:</span>
+</span><span id="Controllers-404"><a href="#Controllers-404"><span class="linenos">404</span></a>                <span class="k">return</span> <span class="n">ctl</span>
+</span><span id="Controllers-405"><a href="#Controllers-405"><span class="linenos">405</span></a>        <span class="k">return</span> <span class="kc">None</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>StorCLI Controllers</p>
 
 <p>Instance of this class is iterable with :obj:Controller as item</p>
 
@@ -2199,22 +1746,22 @@
             
         <span class="name">Controllers</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">binary</span><span class="o">=</span><span class="s1">&#39;storcli64&#39;</span></span>)</span>
 
                 <label class="view-source-button" for="Controllers.__init__-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Controllers.__init__"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Controllers.__init__-546"><a href="#Controllers.__init__-546"><span class="linenos">546</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">binary</span><span class="o">=</span><span class="s1">&#39;storcli64&#39;</span><span class="p">):</span>
-</span><span id="Controllers.__init__-547"><a href="#Controllers.__init__-547"><span class="linenos">547</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Constructor - create StorCLI Controllers object</span>
-</span><span id="Controllers.__init__-548"><a href="#Controllers.__init__-548"><span class="linenos">548</span></a>
-</span><span id="Controllers.__init__-549"><a href="#Controllers.__init__-549"><span class="linenos">549</span></a><span class="sd">        Args:</span>
-</span><span id="Controllers.__init__-550"><a href="#Controllers.__init__-550"><span class="linenos">550</span></a><span class="sd">            binary (str): storcli binary or full path to the binary</span>
-</span><span id="Controllers.__init__-551"><a href="#Controllers.__init__-551"><span class="linenos">551</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controllers.__init__-552"><a href="#Controllers.__init__-552"><span class="linenos">552</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_binary</span> <span class="o">=</span> <span class="n">binary</span>
-</span><span id="Controllers.__init__-553"><a href="#Controllers.__init__-553"><span class="linenos">553</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_storcli</span> <span class="o">=</span> <span class="n">StorCLI</span><span class="p">(</span><span class="n">binary</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Controllers.__init__-359"><a href="#Controllers.__init__-359"><span class="linenos">359</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">binary</span><span class="o">=</span><span class="s1">&#39;storcli64&#39;</span><span class="p">):</span>
+</span><span id="Controllers.__init__-360"><a href="#Controllers.__init__-360"><span class="linenos">360</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Constructor - create StorCLI Controllers object</span>
+</span><span id="Controllers.__init__-361"><a href="#Controllers.__init__-361"><span class="linenos">361</span></a>
+</span><span id="Controllers.__init__-362"><a href="#Controllers.__init__-362"><span class="linenos">362</span></a><span class="sd">        Args:</span>
+</span><span id="Controllers.__init__-363"><a href="#Controllers.__init__-363"><span class="linenos">363</span></a><span class="sd">            binary (str): storcli binary or full path to the binary</span>
+</span><span id="Controllers.__init__-364"><a href="#Controllers.__init__-364"><span class="linenos">364</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="Controllers.__init__-365"><a href="#Controllers.__init__-365"><span class="linenos">365</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_binary</span> <span class="o">=</span> <span class="n">binary</span>
+</span><span id="Controllers.__init__-366"><a href="#Controllers.__init__-366"><span class="linenos">366</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_storcli</span> <span class="o">=</span> <span class="n">StorCLI</span><span class="p">(</span><span class="n">binary</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Constructor - create StorCLI Controllers object</p>
 
 <p>Args:
     binary (str): storcli binary or full path to the binary</p>
@@ -2242,28 +1789,28 @@
         <span class="def">def</span>
         <span class="name">get_ctl</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">ctl_id</span><span class="p">:</span> <span class="nb">int</span></span><span class="return-annotation">) -> <span class="n">Optional</span><span class="p">[</span><span class="n"><a href="#Controller">pystorcli2.Controller</a></span><span class="p">]</span>:</span></span>
 
                 <label class="view-source-button" for="Controllers.get_ctl-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Controllers.get_ctl"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Controllers.get_ctl-579"><a href="#Controllers.get_ctl-579"><span class="linenos">579</span></a>    <span class="k">def</span> <span class="nf">get_ctl</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">ctl_id</span><span class="p">:</span> <span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Optional</span><span class="p">[</span><span class="n">Controller</span><span class="p">]:</span>
-</span><span id="Controllers.get_ctl-580"><a href="#Controllers.get_ctl-580"><span class="linenos">580</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Get controller object by id</span>
-</span><span id="Controllers.get_ctl-581"><a href="#Controllers.get_ctl-581"><span class="linenos">581</span></a>
-</span><span id="Controllers.get_ctl-582"><a href="#Controllers.get_ctl-582"><span class="linenos">582</span></a><span class="sd">        Args:</span>
-</span><span id="Controllers.get_ctl-583"><a href="#Controllers.get_ctl-583"><span class="linenos">583</span></a><span class="sd">            ctl_id (str): controller id</span>
-</span><span id="Controllers.get_ctl-584"><a href="#Controllers.get_ctl-584"><span class="linenos">584</span></a>
-</span><span id="Controllers.get_ctl-585"><a href="#Controllers.get_ctl-585"><span class="linenos">585</span></a><span class="sd">        Returns:</span>
-</span><span id="Controllers.get_ctl-586"><a href="#Controllers.get_ctl-586"><span class="linenos">586</span></a><span class="sd">            (None): no controller with id</span>
-</span><span id="Controllers.get_ctl-587"><a href="#Controllers.get_ctl-587"><span class="linenos">587</span></a><span class="sd">            (:obj:Controller): controller object</span>
-</span><span id="Controllers.get_ctl-588"><a href="#Controllers.get_ctl-588"><span class="linenos">588</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Controllers.get_ctl-589"><a href="#Controllers.get_ctl-589"><span class="linenos">589</span></a>        <span class="k">for</span> <span class="n">ctl</span> <span class="ow">in</span> <span class="bp">self</span><span class="p">:</span>
-</span><span id="Controllers.get_ctl-590"><a href="#Controllers.get_ctl-590"><span class="linenos">590</span></a>            <span class="k">if</span> <span class="n">ctl</span><span class="o">.</span><span class="n">id</span> <span class="o">==</span> <span class="n">ctl_id</span><span class="p">:</span>
-</span><span id="Controllers.get_ctl-591"><a href="#Controllers.get_ctl-591"><span class="linenos">591</span></a>                <span class="k">return</span> <span class="n">ctl</span>
-</span><span id="Controllers.get_ctl-592"><a href="#Controllers.get_ctl-592"><span class="linenos">592</span></a>        <span class="k">return</span> <span class="kc">None</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Controllers.get_ctl-392"><a href="#Controllers.get_ctl-392"><span class="linenos">392</span></a>    <span class="k">def</span> <span class="nf">get_ctl</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">ctl_id</span><span class="p">:</span> <span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Optional</span><span class="p">[</span><span class="n">Controller</span><span class="p">]:</span>
+</span><span id="Controllers.get_ctl-393"><a href="#Controllers.get_ctl-393"><span class="linenos">393</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;Get controller object by id</span>
+</span><span id="Controllers.get_ctl-394"><a href="#Controllers.get_ctl-394"><span class="linenos">394</span></a>
+</span><span id="Controllers.get_ctl-395"><a href="#Controllers.get_ctl-395"><span class="linenos">395</span></a><span class="sd">        Args:</span>
+</span><span id="Controllers.get_ctl-396"><a href="#Controllers.get_ctl-396"><span class="linenos">396</span></a><span class="sd">            ctl_id (str): controller id</span>
+</span><span id="Controllers.get_ctl-397"><a href="#Controllers.get_ctl-397"><span class="linenos">397</span></a>
+</span><span id="Controllers.get_ctl-398"><a href="#Controllers.get_ctl-398"><span class="linenos">398</span></a><span class="sd">        Returns:</span>
+</span><span id="Controllers.get_ctl-399"><a href="#Controllers.get_ctl-399"><span class="linenos">399</span></a><span class="sd">            (None): no controller with id</span>
+</span><span id="Controllers.get_ctl-400"><a href="#Controllers.get_ctl-400"><span class="linenos">400</span></a><span class="sd">            (:obj:Controller): controller object</span>
+</span><span id="Controllers.get_ctl-401"><a href="#Controllers.get_ctl-401"><span class="linenos">401</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="Controllers.get_ctl-402"><a href="#Controllers.get_ctl-402"><span class="linenos">402</span></a>        <span class="k">for</span> <span class="n">ctl</span> <span class="ow">in</span> <span class="bp">self</span><span class="p">:</span>
+</span><span id="Controllers.get_ctl-403"><a href="#Controllers.get_ctl-403"><span class="linenos">403</span></a>            <span class="k">if</span> <span class="n">ctl</span><span class="o">.</span><span class="n">id</span> <span class="o">==</span> <span class="n">ctl_id</span><span class="p">:</span>
+</span><span id="Controllers.get_ctl-404"><a href="#Controllers.get_ctl-404"><span class="linenos">404</span></a>                <span class="k">return</span> <span class="n">ctl</span>
+</span><span id="Controllers.get_ctl-405"><a href="#Controllers.get_ctl-405"><span class="linenos">405</span></a>        <span class="k">return</span> <span class="kc">None</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Get controller object by id</p>
 
 <p>Args:
     ctl_id (str): controller id</p>
@@ -2329,15 +1876,15 @@
 </span><span id="Enclosure-59"><a href="#Enclosure-59"><span class="linenos"> 59</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_storcli</span><span class="o">.</span><span class="n">run</span><span class="p">(</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span>
 </span><span id="Enclosure-60"><a href="#Enclosure-60"><span class="linenos"> 60</span></a>
 </span><span id="Enclosure-61"><a href="#Enclosure-61"><span class="linenos"> 61</span></a>    <span class="k">def</span> <span class="nf">_exist</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
 </span><span id="Enclosure-62"><a href="#Enclosure-62"><span class="linenos"> 62</span></a>        <span class="k">try</span><span class="p">:</span>
 </span><span id="Enclosure-63"><a href="#Enclosure-63"><span class="linenos"> 63</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">([</span><span class="s1">&#39;show&#39;</span><span class="p">])</span>
 </span><span id="Enclosure-64"><a href="#Enclosure-64"><span class="linenos"> 64</span></a>        <span class="k">except</span> <span class="n">exc</span><span class="o">.</span><span class="n">StorCliCmdError</span><span class="p">:</span>
 </span><span id="Enclosure-65"><a href="#Enclosure-65"><span class="linenos"> 65</span></a>            <span class="k">raise</span> <span class="n">exc</span><span class="o">.</span><span class="n">StorCliMissingError</span><span class="p">(</span>
-</span><span id="Enclosure-66"><a href="#Enclosure-66"><span class="linenos"> 66</span></a>                <span class="bp">self</span><span class="o">.</span><span class="vm">__class__</span><span class="o">.</span><span class="vm">__name__</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="p">)</span> <span class="kn">from</span> <span class="kc">None</span>
+</span><span id="Enclosure-66"><a href="#Enclosure-66"><span class="linenos"> 66</span></a>                <span class="bp">self</span><span class="o">.</span><span class="vm">__class__</span><span class="o">.</span><span class="vm">__name__</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="p">)</span> <span class="kn">from</span> <span class="bp">None</span>
 </span><span id="Enclosure-67"><a href="#Enclosure-67"><span class="linenos"> 67</span></a>
 </span><span id="Enclosure-68"><a href="#Enclosure-68"><span class="linenos"> 68</span></a>    <span class="nd">@property</span>
 </span><span id="Enclosure-69"><a href="#Enclosure-69"><span class="linenos"> 69</span></a>    <span class="k">def</span> <span class="nf">id</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
 </span><span id="Enclosure-70"><a href="#Enclosure-70"><span class="linenos"> 70</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;(str): enclosure id</span>
 </span><span id="Enclosure-71"><a href="#Enclosure-71"><span class="linenos"> 71</span></a><span class="sd">        &quot;&quot;&quot;</span>
 </span><span id="Enclosure-72"><a href="#Enclosure-72"><span class="linenos"> 72</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_encl_id</span>
 </span><span id="Enclosure-73"><a href="#Enclosure-73"><span class="linenos"> 73</span></a>
@@ -3415,15 +2962,15 @@
 </span><span id="Drive-387"><a href="#Drive-387"><span class="linenos">387</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_storcli</span><span class="o">.</span><span class="n">run</span><span class="p">(</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span>
 </span><span id="Drive-388"><a href="#Drive-388"><span class="linenos">388</span></a>
 </span><span id="Drive-389"><a href="#Drive-389"><span class="linenos">389</span></a>    <span class="k">def</span> <span class="nf">_exist</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
 </span><span id="Drive-390"><a href="#Drive-390"><span class="linenos">390</span></a>        <span class="k">try</span><span class="p">:</span>
 </span><span id="Drive-391"><a href="#Drive-391"><span class="linenos">391</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">([</span><span class="s1">&#39;show&#39;</span><span class="p">])</span>
 </span><span id="Drive-392"><a href="#Drive-392"><span class="linenos">392</span></a>        <span class="k">except</span> <span class="n">exc</span><span class="o">.</span><span class="n">StorCliCmdError</span><span class="p">:</span>
 </span><span id="Drive-393"><a href="#Drive-393"><span class="linenos">393</span></a>            <span class="k">raise</span> <span class="n">exc</span><span class="o">.</span><span class="n">StorCliMissingError</span><span class="p">(</span>
-</span><span id="Drive-394"><a href="#Drive-394"><span class="linenos">394</span></a>                <span class="bp">self</span><span class="o">.</span><span class="vm">__class__</span><span class="o">.</span><span class="vm">__name__</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="p">)</span> <span class="kn">from</span> <span class="kc">None</span>
+</span><span id="Drive-394"><a href="#Drive-394"><span class="linenos">394</span></a>                <span class="bp">self</span><span class="o">.</span><span class="vm">__class__</span><span class="o">.</span><span class="vm">__name__</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="p">)</span> <span class="kn">from</span> <span class="bp">None</span>
 </span><span id="Drive-395"><a href="#Drive-395"><span class="linenos">395</span></a>
 </span><span id="Drive-396"><a href="#Drive-396"><span class="linenos">396</span></a>    <span class="nd">@property</span>
 </span><span id="Drive-397"><a href="#Drive-397"><span class="linenos">397</span></a>    <span class="k">def</span> <span class="nf">id</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
 </span><span id="Drive-398"><a href="#Drive-398"><span class="linenos">398</span></a><span class="w">        </span><span class="sd">&quot;&quot;&quot;(str): drive id</span>
 </span><span id="Drive-399"><a href="#Drive-399"><span class="linenos">399</span></a><span class="sd">        &quot;&quot;&quot;</span>
 </span><span id="Drive-400"><a href="#Drive-400"><span class="linenos">400</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_slot_id</span>
 </span><span id="Drive-401"><a href="#Drive-401"><span class="linenos">401</span></a>
@@ -5034,15 +4581,15 @@
 </span><span id="VirtualDrive-190"><a href="#VirtualDrive-190"><span class="linenos">190</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_storcli</span><span class="o">.</span><span class="n">run</span><span class="p">(</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span>
 </span><span id="VirtualDrive-191"><a href="#VirtualDrive-191"><span class="linenos">191</span></a>
 </span><span id="VirtualDrive-192"><a href="#VirtualDrive-192"><span class="linenos">192</span></a>    <span class="k">def</span> <span class="nf">_exist</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
 </span><span id="VirtualDrive-193"><a href="#VirtualDrive-193"><span class="linenos">193</span></a>        <span class="k">try</span><span class="p">:</span>
 </span><span id="VirtualDrive-194"><a href="#VirtualDrive-194"><span class="linenos">194</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">([</span><span class="s1">&#39;show&#39;</span><span class="p">])</span>
 </span><span id="VirtualDrive-195"><a href="#VirtualDrive-195"><span class="linenos">195</span></a>        <span class="k">except</span> <span class="n">exc</span><span class="o">.</span><span class="n">StorCliCmdError</span><span class="p">:</span>
 </span><span id="VirtualDrive-196"><a href="#VirtualDrive-196"><span class="linenos">196</span></a>            <span class="k">raise</span> <span class="n">exc</span><span class="o">.</span><span class="n">StorCliMissingError</span><span class="p">(</span>
-</span><span id="VirtualDrive-197"><a href="#VirtualDrive-197"><span class="linenos">197</span></a>                <span class="bp">self</span><span class="o">.</span><span class="vm">__class__</span><span class="o">.</span><span class="vm">__name__</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="p">)</span> <span class="kn">from</span> <span class="kc">None</span>
+</span><span id="VirtualDrive-197"><a href="#VirtualDrive-197"><span class="linenos">197</span></a>                <span class="bp">self</span><span class="o">.</span><span class="vm">__class__</span><span class="o">.</span><span class="vm">__name__</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="p">)</span> <span class="kn">from</span> <span class="bp">None</span>
 </span><span id="VirtualDrive-198"><a href="#VirtualDrive-198"><span class="linenos">198</span></a>
 </span><span id="VirtualDrive-199"><a href="#VirtualDrive-199"><span class="linenos">199</span></a>    <span class="nd">@staticmethod</span>
 </span><span id="VirtualDrive-200"><a href="#VirtualDrive-200"><span class="linenos">200</span></a>    <span class="k">def</span> <span class="nf">_response_properties</span><span class="p">(</span><span class="n">out</span><span class="p">):</span>
 </span><span id="VirtualDrive-201"><a href="#VirtualDrive-201"><span class="linenos">201</span></a>        <span class="k">return</span> <span class="n">common</span><span class="o">.</span><span class="n">response_data</span><span class="p">(</span><span class="n">out</span><span class="p">)[</span><span class="s1">&#39;Virtual Drives&#39;</span><span class="p">][</span><span class="mi">0</span><span class="p">]</span>
 </span><span id="VirtualDrive-202"><a href="#VirtualDrive-202"><span class="linenos">202</span></a>
 </span><span id="VirtualDrive-203"><a href="#VirtualDrive-203"><span class="linenos">203</span></a>    <span class="k">def</span> <span class="nf">_response_properties_all</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">out</span><span class="p">):</span>
 </span><span id="VirtualDrive-204"><a href="#VirtualDrive-204"><span class="linenos">204</span></a>        <span class="k">return</span> <span class="n">common</span><span class="o">.</span><span class="n">response_data</span><span class="p">(</span><span class="n">out</span><span class="p">)[</span><span class="s1">&#39;VD</span><span class="si">{0}</span><span class="s1"> Properties&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_vd_id</span><span class="p">)]</span>
```

#### html2text {}

```diff
@@ -23,23 +23,14 @@
           o name
           o facts
           o metrics
           o vds
           o encls
           o drives_ids
           o create_vd
-          o autorebuild
-          o foreignautoimport
-          o patrolread
-          o set_patrolread
-          o patrolread_start
-          o patrolread_stop
-          o patrolread_pause
-          o patrolread_resume
-          o patrolread_running
     * Controllers
           o Controllers
           o ids
           o get_ctl
     * Enclosure
           o Enclosure
           o id
@@ -185,15 +176,15 @@
 14from .drive import DriveState, Drive, Drives
 15from .virtualdrive import VirtualDrive, VirtualDrives
 16
 17__all__ = ['__version__', 'StorCLI', 'Controller', 'Controllers',
 18           'Enclosure', 'Enclosures', 'DriveState', 'Drive', 'Drives',
 'VirtualDrive', 'VirtualDrives']
 
-__version__ = '0.6.1'
+__version__ = '0.6.1.dev6'
    ⁰
 class StorCLI: View Source
 _27class StorCLI(object):
 _28    """StorCLI command line wrapper
 _29
 _30    Instance of this class is storcli command line wrapper
 _31
@@ -674,381 +665,183 @@
 198        id (str): controller id
 199        name (str): controller cmd name
 200        facts (dict): raw controller facts
 201        metrics (:obj:ControllerMetrics): controller metrics
 202        vds (list of :obj:virtualdrive.VirtualDrives): controller virtual
 drives
 203        encls (:obj:enclosure.Enclosures): controller enclosures
-204        autorebuild (dict): current auto rebuild state (also setter)
-205        foreignautoimport (dict): imports foreign configuration
-automatically at boot (also setter)
-206        patrolread (dict): current patrol read settings (also setter)
+204
+205    Methods:
+206        create_vd (:obj:VirtualDrive): create virtual drive
 207
-208    Methods:
-209        create_vd (:obj:VirtualDrive): create virtual drive
-210        set_patrolread (dict): configures patrol read state and schedule
-211        patrolread_start (dict): starts a patrol read on controller
-212        patrolread_pause (dict): pauses patrol read on controller
-213        patrolread_resume (dict): resumes patrol read on controller
-214        patrolread_stop (dict): stops patrol read if running on controller
-215        patrolread_running (bool): check if patrol read is running on
-controller
-216
-217    TODO:
-218        Implement missing methods:
-219            * patrol read progress
-220    """
+208    """
+209
+210    def __init__(self, ctl_id, binary='storcli64'):
+211        """Constructor - create StorCLI Controller object
+212
+213        Args:
+214            ctl_id (str): controller id
+215            binary (str): storcli binary or full path to the binary
+216        """
+217        self._ctl_id = ctl_id
+218        self._binary = binary
+219        self._storcli = StorCLI(binary)
+220        self._name = '/c{0}'.format(self._ctl_id)
 221
-222    def __init__(self, ctl_id, binary='storcli64'):
-223        """Constructor - create StorCLI Controller object
-224
-225        Args:
-226            ctl_id (str): controller id
-227            binary (str): storcli binary or full path to the binary
-228        """
-229        self._ctl_id = ctl_id
-230        self._binary = binary
-231        self._storcli = StorCLI(binary)
-232        self._name = '/c{0}'.format(self._ctl_id)
-233
-234        self._exist()
-235
-236    def __str__(self):
-237        return '{0}'.format(common.response_data(self._run(['show'])))
+222        self._exist()
+223
+224    def __str__(self):
+225        return '{0}'.format(common.response_data(self._run(['show'])))
+226
+227    def _run(self, args, **kwargs):
+228        args = args[:]
+229        args.insert(0, self._name)
+230        return self._storcli.run(args, **kwargs)
+231
+232    def _exist(self):
+233        try:
+234            self._run(['show'])
+235        except exc.StorCliCmdError:
+236            raise exc.StorCliMissingError(
+237                self.__class__.__name__, self._name) from None
 238
-239    def _run(self, args, **kwargs):
-240        args = args[:]
-241        args.insert(0, self._name)
-242        return self._storcli.run(args, **kwargs)
-243
-244    def _exist(self):
-245        try:
-246            self._run(['show'])
-247        except exc.StorCliCmdError:
-248            raise exc.StorCliMissingError(
-249                self.__class__.__name__, self._name) from None
+239    @property
+240    def id(self):
+241        """ (str): controller id
+242        """
+243        return self._ctl_id
+244
+245    @property
+246    def name(self):
+247        """ (str): controller cmd name
+248        """
+249        return self._name
 250
 251    @property
-252    def id(self):
-253        """ (str): controller id
+252    def facts(self):
+253        """ (dict): raw controller facts
 254        """
-255        return self._ctl_id
-256
-257    @property
-258    def name(self):
-259        """ (str): controller cmd name
-260        """
-261        return self._name
-262
-263    @property
-264    def facts(self):
-265        """ (dict): raw controller facts
-266        """
-267        args = [
-268            'show',
-269            'all'
-270        ]
-271        return common.response_data(self._run(args))
+255        args = [
+256            'show',
+257            'all'
+258        ]
+259        return common.response_data(self._run(args))
+260
+261    @property
+262    def metrics(self):
+263        """(:obj:ControllerMetrics): controller metrics
+264        """
+265        return ControllerMetrics(ctl=self)
+266
+267    @property
+268    def vds(self):
+269        """(:obj:virtualdrive.VirtualDrives): controllers virtual drives
+270        """
+271        return virtualdrive.VirtualDrives(ctl_id=self._ctl_id,
+binary=self._binary)
 272
 273    @property
-274    def metrics(self):
-275        """(:obj:ControllerMetrics): controller metrics
+274    def encls(self):
+275        """(:obj:enclosure.Enclosures): controller enclosures
 276        """
-277        return ControllerMetrics(ctl=self)
+277        return enclosure.Enclosures(ctl_id=self._ctl_id,
+binary=self._binary)
 278
 279    @property
-280    def vds(self):
-281        """(:obj:virtualdrive.VirtualDrives): controllers virtual drives
+280    def drives_ids(self) -> List[str]:
+281        """(list of str): list of drives ids in format (e:s)
 282        """
-283        return virtualdrive.VirtualDrives(ctl_id=self._ctl_id,
-binary=self._binary)
-284
-285    @property
-286    def encls(self):
-287        """(:obj:enclosure.Enclosures): controller enclosures
-288        """
-289        return enclosure.Enclosures(ctl_id=self._ctl_id,
-binary=self._binary)
-290
-291    @property
-292    def drives_ids(self) -> List[str]:
-293        """(list of str): list of drives ids in format (e:s)
-294        """
-295        drives = []
-296        for encl in self.encls:
-297            for id in encl.drives.ids:
-298                drives.append("{enc}:{id}".format(enc=encl.id, id=id))
-299
-300        return drives
-301
-302    def create_vd(self, name: str, raid: str, drives: str, strip: str =
+283        drives = []
+284        for encl in self.encls:
+285            for id in encl.drives.ids:
+286                drives.append("{enc}:{id}".format(enc=encl.id, id=id))
+287
+288        return drives
+289
+290    def create_vd(self, name: str, raid: str, drives: str, strip: str =
 '64', PDperArray: Optional[int] = None) -> Optional[virtualdrive.VirtualDrive]:
-303        """Create virtual drive (raid) managed by current controller
-304
-305        Args:
-306            name (str): virtual drive name
-307            raid (str): virtual drive raid level (raid0, raid1, ...)
-308            drives (str): storcli drives expression (e:s|e:s-x|e:s-x,y;e:s-
+291        """Create virtual drive (raid) managed by current controller
+292
+293        Args:
+294            name (str): virtual drive name
+295            raid (str): virtual drive raid level (raid0, raid1, ...)
+296            drives (str): storcli drives expression (e:s|e:s-x|e:s-x,y;e:s-
 x,y,z)
-309            strip (str, optional): virtual drive raid strip size
-310
-311        Returns:
-312            (None): no virtual drive created with name
-313            (:obj:virtualdrive.VirtualDrive)
-314        """
-315        args = [
-316            'add',
-317            'vd',
-318            'r{0}'.format(raid),
-319            'name={0}'.format(name),
-320            'drives={0}'.format(drives),
-321            'strip={0}'.format(strip)
-322        ]
-323
-324        try:
-325            if int(raid) >= 10 and PDperArray is None:
-326                # Try to count the number of drives in the array
-327                # The format of the drives argument is e:s|e:s-x|e:s-x,y;e:
+297            strip (str, optional): virtual drive raid strip size
+298
+299        Returns:
+300            (None): no virtual drive created with name
+301            (:obj:virtualdrive.VirtualDrive)
+302        """
+303        args = [
+304            'add',
+305            'vd',
+306            'r{0}'.format(raid),
+307            'name={0}'.format(name),
+308            'drives={0}'.format(drives),
+309            'strip={0}'.format(strip)
+310        ]
+311
+312        try:
+313            if int(raid) >= 10 and PDperArray is None:
+314                # Try to count the number of drives in the array
+315                # The format of the drives argument is e:s|e:s-x|e:s-x,y;e:
 s-x,y,z
-328
-329                numDrives = common.count_drives(drives)
-330
-331                if numDrives % 2 != 0 and numDrives % 3 == 0:
-332                    # In some scenarios, such as 9 drives with raid 60, 3 is
+316
+317                numDrives = common.count_drives(drives)
+318
+319                if numDrives % 2 != 0 and numDrives % 3 == 0:
+320                    # In some scenarios, such as 9 drives with raid 60, 3 is
 a good pd number but 4 is not
-333                    # Must check for similar scenarios
-334                    # BTW we don't clearly understand what PDperArray is for
+321                    # Must check for similar scenarios
+322                    # BTW we don't clearly understand what PDperArray is for
 and what exactly it does under the hood. More investigation is needed
-335                    PDperArray = numDrives//3
-336                else:
-337                    PDperArray = numDrives//2
-338
-339        except ValueError:
-340            pass
-341
-342        finally:
-343            if raid == '00' and PDperArray is None:
-344                PDperArray = 1
-345
-346        if PDperArray is not None:
-347            args.append('PDperArray={0}'.format(PDperArray))
-348
-349        self._run(args)
-350        for vd in self.vds:
-351            if name == vd.name:
-352                return vd
-353        return None
-354
-355    @property
-356    @common.lower
-357    def autorebuild(self):
-358        """Get/Set auto rebuild state
-359
-360        One of the following options can be set (str):
-361            on - enables autorebuild
-362            off - disables autorebuild
-363
-364        Returns:
-365            (str): on / off
-366        """
-367        args = [
-368            'show',
-369            'autorebuild'
-370        ]
-371
-372        prop = common.response_property(self._run(args))[0]
-373        return prop['Value']
-374
-375    @autorebuild.setter
-376    def autorebuild(self, value):
-377        """
-378        """
-379        args = [
-380            'set',
-381            'autorebuild={0}'.format(value)
-382        ]
-383        return common.response_setter(self._run(args))
-384
-385    @property
-386    @common.lower
-387    def foreignautoimport(self):
-388        """Get/Set auto foreign import configuration
-389
-390        One of the following options can be set (str):
-391            on - enables foreignautoimport
-392            off - disables foreignautoimport
-393
-394        Returns:
-395            (str): on / off
-396        """
-397        args = [
-398            'show',
-399            'foreignautoimport'
-400        ]
-401        prop = common.response_property(self._run(args))[0]
-402        return prop['Value']
-403
-404    @foreignautoimport.setter
-405    def foreignautoimport(self, value):
-406        """
-407        """
-408        args = [
-409            'set',
-410            'foreignautoimport={0}'.format(value)
-411        ]
-412        return common.response_setter(self._run(args))
-413
-414    @property
-415    @common.lower
-416    def patrolread(self):
-417        """Get/Set patrol read
-418
-419        One of the following options can be set (str):
-420            on - enables patrol read
-421            off - disables patrol read
-422
-423        Returns:
-424            (str): on / off
-425        """
-426        args = [
-427            'show',
-428            'patrolread'
-429        ]
-430
-431        for pr in common.response_property(self._run(args)):
-432            if pr['Ctrl_Prop'] == "PR Mode":
-433                if pr['Value'] == 'Disable':
-434                    return 'off'
-435                else:
-436                    return 'on'
-437        return 'off'
-438
-439
-440    @patrolread.setter
-441    def patrolread(self, value):
-442        """
-443        """
-444        return self.set_patrolread(value)
-445
-446
-447    def set_patrolread(self, value, mode='manual'):
-448        """Set patrol read
-449
-450        Args:
-451            value (str): on / off to configure patrol read state
-452            mode (str): auto | manual to configure patrol read schedule
-453        """
-454        args = [
-455            'set',
-456            'patrolread={0}'.format(value)
-457        ]
-458
-459        if value == 'on':
-460            args.append('mode={0}'.format(mode))
-461
-462        return common.response_setter(self._run(args))
-463
-464    def patrolread_start(self):
-465        """Starts the patrol read operation of the controller
-466
-467        Returns:
-468            (dict): response cmd data
-469        """
-470        args = [
-471            'start',
-472            'patrolread'
-473        ]
-474        return common.response_cmd(self._run(args))
-475
-476    def patrolread_stop(self):
-477        """Stops the patrol read operation of the controller
-478
-479        Returns:
-480            (dict): response cmd data
-481        """
-482        args = [
-483            'stop',
-484            'patrolread'
-485        ]
-486        return common.response_cmd(self._run(args))
-487
-488    def patrolread_pause(self):
-489        """Pauses the patrol read operation of the controller
-490
-491        Returns:
-492            (dict): response cmd data
-493        """
-494        args = [
-495            'pause',
-496            'patrolread'
-497        ]
-498        return common.response_cmd(self._run(args))
-499
-500    def patrolread_resume(self):
-501        """Resumes the patrol read operation of the controller
-502
-503        Returns:
-504            (dict): response cmd data
-505        """
-506        args = [
-507            'resume',
-508            'patrolread'
-509        ]
-510        return common.response_cmd(self._run(args))
-511
-512    @property
-513    def patrolread_running(self):
-514        """Check if patrol read is running on the controller
-515
-516        Returns:
-517            (bool): true / false
-518        """
-519        args = [
-520            'show',
-521            'patrolread'
-522        ]
-523
-524        status = ''
-525        for pr in common.response_property(self._run(args)):
-526            if pr['Ctrl_Prop'] == "PR Current State":
-527                status = pr['Value']
-528        return bool('Active' in status)
+323                    PDperArray = numDrives//3
+324                else:
+325                    PDperArray = numDrives//2
+326
+327        except ValueError:
+328            pass
+329
+330        finally:
+331            if raid == '00' and PDperArray is None:
+332                PDperArray = 1
+333
+334        if PDperArray is not None:
+335            args.append('PDperArray={0}'.format(PDperArray))
+336
+337        self._run(args)
+338        for vd in self.vds:
+339            if name == vd.name:
+340                return vd
+341        return None
 StorCLI Controller
 Instance of this class represents controller in StorCLI hierarchy
 Args: ctl_id (str): controller id binary (str): storcli binary or full path to
 the binary
 Properties: id (str): controller id name (str): controller cmd name facts
 (dict): raw controller facts metrics (:obj:ControllerMetrics): controller
 metrics vds (list of :obj:virtualdrive.VirtualDrives): controller virtual
-drives encls (:obj:enclosure.Enclosures): controller enclosures autorebuild
-(dict): current auto rebuild state (also setter) foreignautoimport (dict):
-imports foreign configuration automatically at boot (also setter) patrolread
-(dict): current patrol read settings (also setter)
-Methods: create_vd (:obj:VirtualDrive): create virtual drive set_patrolread
-(dict): configures patrol read state and schedule patrolread_start (dict):
-starts a patrol read on controller patrolread_pause (dict): pauses patrol read
-on controller patrolread_resume (dict): resumes patrol read on controller
-patrolread_stop (dict): stops patrol read if running on controller
-patrolread_running (bool): check if patrol read is running on controller
-TODO: Implement missing methods: * patrol read progress
+drives encls (:obj:enclosure.Enclosures): controller enclosures
+Methods: create_vd (:obj:VirtualDrive): create virtual drive
 ⁰
 Controller(ctl_id, binary='storcli64') View Source
-222    def __init__(self, ctl_id, binary='storcli64'):
-223        """Constructor - create StorCLI Controller object
-224
-225        Args:
-226            ctl_id (str): controller id
-227            binary (str): storcli binary or full path to the binary
-228        """
-229        self._ctl_id = ctl_id
-230        self._binary = binary
-231        self._storcli = StorCLI(binary)
-232        self._name = '/c{0}'.format(self._ctl_id)
-233
-234        self._exist()
+210    def __init__(self, ctl_id, binary='storcli64'):
+211        """Constructor - create StorCLI Controller object
+212
+213        Args:
+214            ctl_id (str): controller id
+215            binary (str): storcli binary or full path to the binary
+216        """
+217        self._ctl_id = ctl_id
+218        self._binary = binary
+219        self._storcli = StorCLI(binary)
+220        self._name = '/c{0}'.format(self._ctl_id)
+221
+222        self._exist()
 Constructor - create StorCLI Controller object
 Args: ctl_id (str): controller id binary (str): storcli binary or full path to
 the binary
 id
 (str): controller id
 name
 (str): controller cmd name
@@ -1067,268 +860,178 @@
 self,
 name: str,
 raid: str,
 drives: str,
 strip: str = '64',
 PDperArray: Optional[int] = None) -> Optional[pystorcli2.VirtualDrive]: View
 Source
-302    def create_vd(self, name: str, raid: str, drives: str, strip: str =
+290    def create_vd(self, name: str, raid: str, drives: str, strip: str =
 '64', PDperArray: Optional[int] = None) -> Optional[virtualdrive.VirtualDrive]:
-303        """Create virtual drive (raid) managed by current controller
-304
-305        Args:
-306            name (str): virtual drive name
-307            raid (str): virtual drive raid level (raid0, raid1, ...)
-308            drives (str): storcli drives expression (e:s|e:s-x|e:s-x,y;e:s-
+291        """Create virtual drive (raid) managed by current controller
+292
+293        Args:
+294            name (str): virtual drive name
+295            raid (str): virtual drive raid level (raid0, raid1, ...)
+296            drives (str): storcli drives expression (e:s|e:s-x|e:s-x,y;e:s-
 x,y,z)
-309            strip (str, optional): virtual drive raid strip size
-310
-311        Returns:
-312            (None): no virtual drive created with name
-313            (:obj:virtualdrive.VirtualDrive)
-314        """
-315        args = [
-316            'add',
-317            'vd',
-318            'r{0}'.format(raid),
-319            'name={0}'.format(name),
-320            'drives={0}'.format(drives),
-321            'strip={0}'.format(strip)
-322        ]
-323
-324        try:
-325            if int(raid) >= 10 and PDperArray is None:
-326                # Try to count the number of drives in the array
-327                # The format of the drives argument is e:s|e:s-x|e:s-x,y;e:
+297            strip (str, optional): virtual drive raid strip size
+298
+299        Returns:
+300            (None): no virtual drive created with name
+301            (:obj:virtualdrive.VirtualDrive)
+302        """
+303        args = [
+304            'add',
+305            'vd',
+306            'r{0}'.format(raid),
+307            'name={0}'.format(name),
+308            'drives={0}'.format(drives),
+309            'strip={0}'.format(strip)
+310        ]
+311
+312        try:
+313            if int(raid) >= 10 and PDperArray is None:
+314                # Try to count the number of drives in the array
+315                # The format of the drives argument is e:s|e:s-x|e:s-x,y;e:
 s-x,y,z
-328
-329                numDrives = common.count_drives(drives)
-330
-331                if numDrives % 2 != 0 and numDrives % 3 == 0:
-332                    # In some scenarios, such as 9 drives with raid 60, 3 is
+316
+317                numDrives = common.count_drives(drives)
+318
+319                if numDrives % 2 != 0 and numDrives % 3 == 0:
+320                    # In some scenarios, such as 9 drives with raid 60, 3 is
 a good pd number but 4 is not
-333                    # Must check for similar scenarios
-334                    # BTW we don't clearly understand what PDperArray is for
+321                    # Must check for similar scenarios
+322                    # BTW we don't clearly understand what PDperArray is for
 and what exactly it does under the hood. More investigation is needed
-335                    PDperArray = numDrives//3
-336                else:
-337                    PDperArray = numDrives//2
-338
-339        except ValueError:
-340            pass
-341
-342        finally:
-343            if raid == '00' and PDperArray is None:
-344                PDperArray = 1
-345
-346        if PDperArray is not None:
-347            args.append('PDperArray={0}'.format(PDperArray))
-348
-349        self._run(args)
-350        for vd in self.vds:
-351            if name == vd.name:
-352                return vd
-353        return None
+323                    PDperArray = numDrives//3
+324                else:
+325                    PDperArray = numDrives//2
+326
+327        except ValueError:
+328            pass
+329
+330        finally:
+331            if raid == '00' and PDperArray is None:
+332                PDperArray = 1
+333
+334        if PDperArray is not None:
+335            args.append('PDperArray={0}'.format(PDperArray))
+336
+337        self._run(args)
+338        for vd in self.vds:
+339            if name == vd.name:
+340                return vd
+341        return None
 Create virtual drive (raid) managed by current controller
 Args: name (str): virtual drive name raid (str): virtual drive raid level
 (raid0, raid1, ...) drives (str): storcli drives expression (e:s|e:s-x|e:s-
 x,y;e:s-x,y,z) strip (str, optional): virtual drive raid strip size
 Returns: (None): no virtual drive created with name (:obj:
 virtualdrive.VirtualDrive)
-autorebuild
-func effective wrapper
-foreignautoimport
-func effective wrapper
-patrolread
-func effective wrapper
-⁰
-def set_patrolread(self, value, mode='manual'): View Source
-447    def set_patrolread(self, value, mode='manual'):
-448        """Set patrol read
-449
-450        Args:
-451            value (str): on / off to configure patrol read state
-452            mode (str): auto | manual to configure patrol read schedule
-453        """
-454        args = [
-455            'set',
-456            'patrolread={0}'.format(value)
-457        ]
-458
-459        if value == 'on':
-460            args.append('mode={0}'.format(mode))
-461
-462        return common.response_setter(self._run(args))
-Set patrol read
-Args: value (str): on / off to configure patrol read state mode (str): auto |
-manual to configure patrol read schedule
-⁰
-def patrolread_start(self): View Source
-464    def patrolread_start(self):
-465        """Starts the patrol read operation of the controller
-466
-467        Returns:
-468            (dict): response cmd data
-469        """
-470        args = [
-471            'start',
-472            'patrolread'
-473        ]
-474        return common.response_cmd(self._run(args))
-Starts the patrol read operation of the controller
-Returns: (dict): response cmd data
-⁰
-def patrolread_stop(self): View Source
-476    def patrolread_stop(self):
-477        """Stops the patrol read operation of the controller
-478
-479        Returns:
-480            (dict): response cmd data
-481        """
-482        args = [
-483            'stop',
-484            'patrolread'
-485        ]
-486        return common.response_cmd(self._run(args))
-Stops the patrol read operation of the controller
-Returns: (dict): response cmd data
-⁰
-def patrolread_pause(self): View Source
-488    def patrolread_pause(self):
-489        """Pauses the patrol read operation of the controller
-490
-491        Returns:
-492            (dict): response cmd data
-493        """
-494        args = [
-495            'pause',
-496            'patrolread'
-497        ]
-498        return common.response_cmd(self._run(args))
-Pauses the patrol read operation of the controller
-Returns: (dict): response cmd data
-⁰
-def patrolread_resume(self): View Source
-500    def patrolread_resume(self):
-501        """Resumes the patrol read operation of the controller
-502
-503        Returns:
-504            (dict): response cmd data
-505        """
-506        args = [
-507            'resume',
-508            'patrolread'
-509        ]
-510        return common.response_cmd(self._run(args))
-Resumes the patrol read operation of the controller
-Returns: (dict): response cmd data
-patrolread_running
-Check if patrol read is running on the controller
-Returns: (bool): true / false
   ⁰
 class Controllers: View Source
-531class Controllers(object):
-532    """StorCLI Controllers
-533
-534    Instance of this class is iterable with :obj:Controller as item
-535
-536    Args:
-537        binary (str): storcli binary or full path to the binary
-538
-539    Properties:
-540        ids (list of str): list of controllers id
-541
-542    Methods:
-543        get_clt (:obj:Controller): return controller object by id
-544    """
-545
-546    def __init__(self, binary='storcli64'):
-547        """Constructor - create StorCLI Controllers object
-548
-549        Args:
-550            binary (str): storcli binary or full path to the binary
-551        """
-552        self._binary = binary
-553        self._storcli = StorCLI(binary)
-554
-555    @ property
-556    def _ctl_ids(self) -> List[str]:
-557        out = self._storcli.run(['show'])
-558        response = common.response_data(out)
-559
-560        if "Number of Controllers" in response and response["Number of
+344class Controllers(object):
+345    """StorCLI Controllers
+346
+347    Instance of this class is iterable with :obj:Controller as item
+348
+349    Args:
+350        binary (str): storcli binary or full path to the binary
+351
+352    Properties:
+353        ids (list of str): list of controllers id
+354
+355    Methods:
+356        get_clt (:obj:Controller): return controller object by id
+357    """
+358
+359    def __init__(self, binary='storcli64'):
+360        """Constructor - create StorCLI Controllers object
+361
+362        Args:
+363            binary (str): storcli binary or full path to the binary
+364        """
+365        self._binary = binary
+366        self._storcli = StorCLI(binary)
+367
+368    @ property
+369    def _ctl_ids(self) -> List[str]:
+370        out = self._storcli.run(['show'])
+371        response = common.response_data(out)
+372
+373        if "Number of Controllers" in response and response["Number of
 Controllers"] == 0:
-561            return []
-562        else:
-563            return [ctl['Ctl'] for ctl in common.response_data_subkey(out,
+374            return []
+375        else:
+376            return [ctl['Ctl'] for ctl in common.response_data_subkey(out,
 ['System Overview', 'IT System Overview'])]
-564
-565    @ property
-566    def _ctls(self):
-567        for ctl_id in self._ctl_ids:
-568            yield Controller(ctl_id=ctl_id, binary=self._binary)
-569
-570    def __iter__(self):
-571        return self._ctls
-572
-573    @ property
-574    def ids(self):
-575        """(list of str): controllers id
-576        """
-577        return self._ctl_ids
-578
-579    def get_ctl(self, ctl_id: int) -> Optional[Controller]:
-580        """Get controller object by id
-581
-582        Args:
-583            ctl_id (str): controller id
-584
-585        Returns:
-586            (None): no controller with id
-587            (:obj:Controller): controller object
-588        """
-589        for ctl in self:
-590            if ctl.id == ctl_id:
-591                return ctl
-592        return None
+377
+378    @ property
+379    def _ctls(self):
+380        for ctl_id in self._ctl_ids:
+381            yield Controller(ctl_id=ctl_id, binary=self._binary)
+382
+383    def __iter__(self):
+384        return self._ctls
+385
+386    @ property
+387    def ids(self):
+388        """(list of str): controllers id
+389        """
+390        return self._ctl_ids
+391
+392    def get_ctl(self, ctl_id: int) -> Optional[Controller]:
+393        """Get controller object by id
+394
+395        Args:
+396            ctl_id (str): controller id
+397
+398        Returns:
+399            (None): no controller with id
+400            (:obj:Controller): controller object
+401        """
+402        for ctl in self:
+403            if ctl.id == ctl_id:
+404                return ctl
+405        return None
 StorCLI Controllers
 Instance of this class is iterable with :obj:Controller as item
 Args: binary (str): storcli binary or full path to the binary
 Properties: ids (list of str): list of controllers id
 Methods: get_clt (:obj:Controller): return controller object by id
 ⁰
 Controllers(binary='storcli64') View Source
-546    def __init__(self, binary='storcli64'):
-547        """Constructor - create StorCLI Controllers object
-548
-549        Args:
-550            binary (str): storcli binary or full path to the binary
-551        """
-552        self._binary = binary
-553        self._storcli = StorCLI(binary)
+359    def __init__(self, binary='storcli64'):
+360        """Constructor - create StorCLI Controllers object
+361
+362        Args:
+363            binary (str): storcli binary or full path to the binary
+364        """
+365        self._binary = binary
+366        self._storcli = StorCLI(binary)
 Constructor - create StorCLI Controllers object
 Args: binary (str): storcli binary or full path to the binary
 ids
 (list of str): controllers id
 ⁰
 def get_ctl(self, ctl_id: int) -> Optional[pystorcli2.Controller]: View Source
-579    def get_ctl(self, ctl_id: int) -> Optional[Controller]:
-580        """Get controller object by id
-581
-582        Args:
-583            ctl_id (str): controller id
-584
-585        Returns:
-586            (None): no controller with id
-587            (:obj:Controller): controller object
-588        """
-589        for ctl in self:
-590            if ctl.id == ctl_id:
-591                return ctl
-592        return None
+392    def get_ctl(self, ctl_id: int) -> Optional[Controller]:
+393        """Get controller object by id
+394
+395        Args:
+396            ctl_id (str): controller id
+397
+398        Returns:
+399            (None): no controller with id
+400            (:obj:Controller): controller object
+401        """
+402        for ctl in self:
+403            if ctl.id == ctl_id:
+404                return ctl
+405        return None
 Get controller object by id
 Args: ctl_id (str): controller id
 Returns: (None): no controller with id (:obj:Controller): controller object
   ⁰
 class Enclosure: View Source
 _20class Enclosure(object):
 _21    """StorCLI enclosure
```

### Comparing `PyStorCLI2-0.6.1/docs/search.js` & `PyStorCLI2-0.6.1.dev6/docs/search.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -811,15 +811,15 @@
                     "annotation": ": pystorcli2.controller.Controllers"
                 },
                 "pystorcli2.Controller": {
                     "fullname": "pystorcli2.Controller",
                     "modulename": "pystorcli2",
                     "qualname": "Controller",
                     "kind": "class",
-                    "doc": "<p>StorCLI Controller</p>\n\n<p>Instance of this class represents controller in StorCLI hierarchy</p>\n\n<p>Args:\n    ctl_id (str): controller id\n    binary (str): storcli binary or full path to the binary</p>\n\n<p>Properties:\n    id (str): controller id\n    name (str): controller cmd name\n    facts (dict): raw controller facts\n    metrics (:obj:ControllerMetrics): controller metrics\n    vds (list of :obj:virtualdrive.VirtualDrives): controller virtual drives\n    encls (:obj:enclosure.Enclosures): controller enclosures\n    autorebuild (dict): current auto rebuild state (also setter)\n    foreignautoimport (dict): imports foreign configuration automatically at boot (also setter)\n    patrolread (dict): current patrol read settings (also setter)</p>\n\n<p>Methods:\n    create_vd (:obj:VirtualDrive): create virtual drive\n    set_patrolread (dict): configures patrol read state and schedule\n    patrolread_start (dict): starts a patrol read on controller\n    patrolread_pause (dict): pauses patrol read on controller\n    patrolread_resume (dict): resumes patrol read on controller\n    patrolread_stop (dict): stops patrol read if running on controller\n    patrolread_running (bool): check if patrol read is running on controller</p>\n\n<p>TODO:\n    Implement missing methods:\n        * patrol read progress</p>\n"
+                    "doc": "<p>StorCLI Controller</p>\n\n<p>Instance of this class represents controller in StorCLI hierarchy</p>\n\n<p>Args:\n    ctl_id (str): controller id\n    binary (str): storcli binary or full path to the binary</p>\n\n<p>Properties:\n    id (str): controller id\n    name (str): controller cmd name\n    facts (dict): raw controller facts\n    metrics (:obj:ControllerMetrics): controller metrics\n    vds (list of :obj:virtualdrive.VirtualDrives): controller virtual drives\n    encls (:obj:enclosure.Enclosures): controller enclosures</p>\n\n<p>Methods:\n    create_vd (:obj:VirtualDrive): create virtual drive</p>\n"
                 },
                 "pystorcli2.Controller.__init__": {
                     "fullname": "pystorcli2.Controller.__init__",
                     "modulename": "pystorcli2",
                     "qualname": "Controller.__init__",
                     "kind": "function",
                     "doc": "<p>Constructor - create StorCLI Controller object</p>\n\n<p>Args:\n    ctl_id (str): controller id\n    binary (str): storcli binary or full path to the binary</p>\n",
@@ -880,87 +880,14 @@
                     "modulename": "pystorcli2",
                     "qualname": "Controller.create_vd",
                     "kind": "function",
                     "doc": "<p>Create virtual drive (raid) managed by current controller</p>\n\n<p>Args:\n    name (str): virtual drive name\n    raid (str): virtual drive raid level (raid0, raid1, ...)\n    drives (str): storcli drives expression (e:s|e:s-x|e:s-x,y;e:s-x,y,z)\n    strip (str, optional): virtual drive raid strip size</p>\n\n<p>Returns:\n    (None): no virtual drive created with name\n    (:obj:virtualdrive.VirtualDrive)</p>\n",
                     "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">name</span><span class=\"p\">:</span> <span class=\"nb\">str</span>,</span><span class=\"param\">\t<span class=\"n\">raid</span><span class=\"p\">:</span> <span class=\"nb\">str</span>,</span><span class=\"param\">\t<span class=\"n\">drives</span><span class=\"p\">:</span> <span class=\"nb\">str</span>,</span><span class=\"param\">\t<span class=\"n\">strip</span><span class=\"p\">:</span> <span class=\"nb\">str</span> <span class=\"o\">=</span> <span class=\"s1\">&#39;64&#39;</span>,</span><span class=\"param\">\t<span class=\"n\">PDperArray</span><span class=\"p\">:</span> <span class=\"n\">Optional</span><span class=\"p\">[</span><span class=\"nb\">int</span><span class=\"p\">]</span> <span class=\"o\">=</span> <span class=\"kc\">None</span></span><span class=\"return-annotation\">) -> <span class=\"n\">Optional</span><span class=\"p\">[</span><span class=\"n\">pystorcli2</span><span class=\"o\">.</span><span class=\"n\">virtualdrive</span><span class=\"o\">.</span><span class=\"n\">VirtualDrive</span><span class=\"p\">]</span>:</span></span>",
                     "funcdef": "def"
                 },
-                "pystorcli2.Controller.autorebuild": {
-                    "fullname": "pystorcli2.Controller.autorebuild",
-                    "modulename": "pystorcli2",
-                    "qualname": "Controller.autorebuild",
-                    "kind": "variable",
-                    "doc": "<p>func effective wrapper</p>\n"
-                },
-                "pystorcli2.Controller.foreignautoimport": {
-                    "fullname": "pystorcli2.Controller.foreignautoimport",
-                    "modulename": "pystorcli2",
-                    "qualname": "Controller.foreignautoimport",
-                    "kind": "variable",
-                    "doc": "<p>func effective wrapper</p>\n"
-                },
-                "pystorcli2.Controller.patrolread": {
-                    "fullname": "pystorcli2.Controller.patrolread",
-                    "modulename": "pystorcli2",
-                    "qualname": "Controller.patrolread",
-                    "kind": "variable",
-                    "doc": "<p>func effective wrapper</p>\n"
-                },
-                "pystorcli2.Controller.set_patrolread": {
-                    "fullname": "pystorcli2.Controller.set_patrolread",
-                    "modulename": "pystorcli2",
-                    "qualname": "Controller.set_patrolread",
-                    "kind": "function",
-                    "doc": "<p>Set patrol read</p>\n\n<p>Args:\n    value (str): on / off to configure patrol read state\n    mode (str): auto | manual to configure patrol read schedule</p>\n",
-                    "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">value</span>, </span><span class=\"param\"><span class=\"n\">mode</span><span class=\"o\">=</span><span class=\"s1\">&#39;manual&#39;</span></span><span class=\"return-annotation\">):</span></span>",
-                    "funcdef": "def"
-                },
-                "pystorcli2.Controller.patrolread_start": {
-                    "fullname": "pystorcli2.Controller.patrolread_start",
-                    "modulename": "pystorcli2",
-                    "qualname": "Controller.patrolread_start",
-                    "kind": "function",
-                    "doc": "<p>Starts the patrol read operation of the controller</p>\n\n<p>Returns:\n    (dict): response cmd data</p>\n",
-                    "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span></span><span class=\"return-annotation\">):</span></span>",
-                    "funcdef": "def"
-                },
-                "pystorcli2.Controller.patrolread_stop": {
-                    "fullname": "pystorcli2.Controller.patrolread_stop",
-                    "modulename": "pystorcli2",
-                    "qualname": "Controller.patrolread_stop",
-                    "kind": "function",
-                    "doc": "<p>Stops the patrol read operation of the controller</p>\n\n<p>Returns:\n    (dict): response cmd data</p>\n",
-                    "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span></span><span class=\"return-annotation\">):</span></span>",
-                    "funcdef": "def"
-                },
-                "pystorcli2.Controller.patrolread_pause": {
-                    "fullname": "pystorcli2.Controller.patrolread_pause",
-                    "modulename": "pystorcli2",
-                    "qualname": "Controller.patrolread_pause",
-                    "kind": "function",
-                    "doc": "<p>Pauses the patrol read operation of the controller</p>\n\n<p>Returns:\n    (dict): response cmd data</p>\n",
-                    "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span></span><span class=\"return-annotation\">):</span></span>",
-                    "funcdef": "def"
-                },
-                "pystorcli2.Controller.patrolread_resume": {
-                    "fullname": "pystorcli2.Controller.patrolread_resume",
-                    "modulename": "pystorcli2",
-                    "qualname": "Controller.patrolread_resume",
-                    "kind": "function",
-                    "doc": "<p>Resumes the patrol read operation of the controller</p>\n\n<p>Returns:\n    (dict): response cmd data</p>\n",
-                    "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span></span><span class=\"return-annotation\">):</span></span>",
-                    "funcdef": "def"
-                },
-                "pystorcli2.Controller.patrolread_running": {
-                    "fullname": "pystorcli2.Controller.patrolread_running",
-                    "modulename": "pystorcli2",
-                    "qualname": "Controller.patrolread_running",
-                    "kind": "variable",
-                    "doc": "<p>Check if patrol read is running on the controller</p>\n\n<p>Returns:\n    (bool): true / false</p>\n"
-                },
                 "pystorcli2.Controllers": {
                     "fullname": "pystorcli2.Controllers",
                     "modulename": "pystorcli2",
                     "qualname": "Controllers",
                     "kind": "class",
                     "doc": "<p>StorCLI Controllers</p>\n\n<p>Instance of this class is iterable with :obj:Controller as item</p>\n\n<p>Args:\n    binary (str): storcli binary or full path to the binary</p>\n\n<p>Properties:\n    ids (list of str): list of controllers id</p>\n\n<p>Methods:\n    get_clt (:obj:Controller): return controller object by id</p>\n"
                 },
@@ -2076,15 +2003,15 @@
                 "pystorcli2.Controller": {
                     "qualname": 1,
                     "fullname": 2,
                     "annotation": 0,
                     "default_value": 0,
                     "signature": 0,
                     "bases": 0,
-                    "doc": 186
+                    "doc": 85
                 },
                 "pystorcli2.Controller.__init__": {
                     "qualname": 3,
                     "fullname": 4,
                     "annotation": 0,
                     "default_value": 0,
                     "signature": 24,
@@ -2159,95 +2086,14 @@
                     "fullname": 4,
                     "annotation": 0,
                     "default_value": 0,
                     "signature": 110,
                     "bases": 0,
                     "doc": 65
                 },
-                "pystorcli2.Controller.autorebuild": {
-                    "qualname": 2,
-                    "fullname": 3,
-                    "annotation": 0,
-                    "default_value": 0,
-                    "signature": 0,
-                    "bases": 0,
-                    "doc": 5
-                },
-                "pystorcli2.Controller.foreignautoimport": {
-                    "qualname": 2,
-                    "fullname": 3,
-                    "annotation": 0,
-                    "default_value": 0,
-                    "signature": 0,
-                    "bases": 0,
-                    "doc": 5
-                },
-                "pystorcli2.Controller.patrolread": {
-                    "qualname": 2,
-                    "fullname": 3,
-                    "annotation": 0,
-                    "default_value": 0,
-                    "signature": 0,
-                    "bases": 0,
-                    "doc": 5
-                },
-                "pystorcli2.Controller.set_patrolread": {
-                    "qualname": 3,
-                    "fullname": 4,
-                    "annotation": 0,
-                    "default_value": 0,
-                    "signature": 30,
-                    "bases": 0,
-                    "doc": 30
-                },
-                "pystorcli2.Controller.patrolread_start": {
-                    "qualname": 3,
-                    "fullname": 4,
-                    "annotation": 0,
-                    "default_value": 0,
-                    "signature": 11,
-                    "bases": 0,
-                    "doc": 18
-                },
-                "pystorcli2.Controller.patrolread_stop": {
-                    "qualname": 3,
-                    "fullname": 4,
-                    "annotation": 0,
-                    "default_value": 0,
-                    "signature": 11,
-                    "bases": 0,
-                    "doc": 18
-                },
-                "pystorcli2.Controller.patrolread_pause": {
-                    "qualname": 3,
-                    "fullname": 4,
-                    "annotation": 0,
-                    "default_value": 0,
-                    "signature": 11,
-                    "bases": 0,
-                    "doc": 18
-                },
-                "pystorcli2.Controller.patrolread_resume": {
-                    "qualname": 3,
-                    "fullname": 4,
-                    "annotation": 0,
-                    "default_value": 0,
-                    "signature": 11,
-                    "bases": 0,
-                    "doc": 18
-                },
-                "pystorcli2.Controller.patrolread_running": {
-                    "qualname": 3,
-                    "fullname": 4,
-                    "annotation": 0,
-                    "default_value": 0,
-                    "signature": 0,
-                    "bases": 0,
-                    "doc": 19
-                },
                 "pystorcli2.Controllers": {
                     "qualname": 1,
                     "fullname": 2,
                     "annotation": 0,
                     "default_value": 0,
                     "signature": 0,
                     "bases": 0,
@@ -3384,15 +3230,15 @@
                     "annotation": 0,
                     "default_value": 0,
                     "signature": 17,
                     "bases": 0,
                     "doc": 33
                 }
             },
-            "length": 161,
+            "length": 152,
             "save": true
         },
         "index": {
             "qualname": {
                 "root": {
                     "docs": {
                         "pystorcli2.StorCLI.__init__": {
@@ -3490,31 +3336,28 @@
                                                 "df": 14
                                             }
                                         }
                                     }
                                 },
                                 "p": {
                                     "docs": {
-                                        "pystorcli2.Controller.patrolread_stop": {
-                                            "tf": 1
-                                        },
                                         "pystorcli2.Drive.init_stop": {
                                             "tf": 1
                                         },
                                         "pystorcli2.Drive.erase_stop": {
                                             "tf": 1
                                         },
                                         "pystorcli2.VirtualDrive.init_stop": {
                                             "tf": 1
                                         },
                                         "pystorcli2.VirtualDrive.erase_stop": {
                                             "tf": 1
                                         }
                                     },
-                                    "df": 5
+                                    "df": 4
                                 }
                             },
                             "a": {
                                 "docs": {},
                                 "df": 0,
                                 "t": {
                                     "docs": {},
@@ -3547,17 +3390,14 @@
                                     }
                                 },
                                 "r": {
                                     "docs": {},
                                     "df": 0,
                                     "t": {
                                         "docs": {
-                                            "pystorcli2.Controller.patrolread_start": {
-                                                "tf": 1
-                                            },
                                             "pystorcli2.Drive.init_start": {
                                                 "tf": 1
                                             },
                                             "pystorcli2.Drive.erase_start": {
                                                 "tf": 1
                                             },
                                             "pystorcli2.VirtualDrive.init_start": {
@@ -3566,15 +3406,15 @@
                                             "pystorcli2.VirtualDrive.erase_start": {
                                                 "tf": 1
                                             },
                                             "pystorcli2.VirtualDrive.migrate_start": {
                                                 "tf": 1
                                             }
                                         },
-                                        "df": 6
+                                        "df": 5
                                     }
                                 }
                             },
                             "r": {
                                 "docs": {
                                     "pystorcli2.DriveState.settable_str": {
                                         "tf": 1
@@ -3611,22 +3451,19 @@
                             "docs": {},
                             "df": 0,
                             "t": {
                                 "docs": {
                                     "pystorcli2.StorCLI.set_cmdrunner": {
                                         "tf": 1
                                     },
-                                    "pystorcli2.Controller.set_patrolread": {
-                                        "tf": 1
-                                    },
                                     "pystorcli2.Drive.set_state": {
                                         "tf": 1
                                     }
                                 },
-                                "df": 3,
+                                "df": 2,
                                 "t": {
                                     "docs": {},
                                     "df": 0,
                                     "a": {
                                         "docs": {},
                                         "df": 0,
                                         "b": {
@@ -4159,44 +3996,17 @@
                                                                     "tf": 1
                                                                 },
                                                                 "pystorcli2.Controller.drives_ids": {
                                                                     "tf": 1
                                                                 },
                                                                 "pystorcli2.Controller.create_vd": {
                                                                     "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.autorebuild": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.foreignautoimport": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.patrolread": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.set_patrolread": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.patrolread_start": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.patrolread_stop": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.patrolread_pause": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.patrolread_resume": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.patrolread_running": {
-                                                                    "tf": 1
                                                                 }
                                                             },
-                                                            "df": 19,
+                                                            "df": 10,
                                                             "s": {
                                                                 "docs": {
                                                                     "pystorcli2.StorCLI.controllers": {
                                                                         "tf": 1
                                                                     },
                                                                     "pystorcli2.Controllers": {
                                                                         "tf": 1
@@ -4631,30 +4441,14 @@
                                                     },
                                                     "df": 1
                                                 }
                                             }
                                         }
                                     }
                                 },
-                                "u": {
-                                    "docs": {},
-                                    "df": 0,
-                                    "m": {
-                                        "docs": {},
-                                        "df": 0,
-                                        "e": {
-                                            "docs": {
-                                                "pystorcli2.Controller.patrolread_resume": {
-                                                    "tf": 1
-                                                }
-                                            },
-                                            "df": 1
-                                        }
-                                    }
-                                },
                                 "e": {
                                     "docs": {},
                                     "df": 0,
                                     "t": {
                                         "docs": {
                                             "pystorcli2.Drive.phyerrorcounters_reset": {
                                                 "tf": 1
@@ -4682,17 +4476,14 @@
                                         "docs": {},
                                         "df": 0,
                                         "n": {
                                             "docs": {},
                                             "df": 0,
                                             "g": {
                                                 "docs": {
-                                                    "pystorcli2.Controller.patrolread_running": {
-                                                        "tf": 1
-                                                    },
                                                     "pystorcli2.Drive.init_running": {
                                                         "tf": 1
                                                     },
                                                     "pystorcli2.Drive.erase_running": {
                                                         "tf": 1
                                                     },
                                                     "pystorcli2.VirtualDrive.init_running": {
@@ -4701,15 +4492,15 @@
                                                     "pystorcli2.VirtualDrive.erase_running": {
                                                         "tf": 1
                                                     },
                                                     "pystorcli2.VirtualDrive.migrate_running": {
                                                         "tf": 1
                                                     }
                                                 },
-                                                "df": 6
+                                                "df": 5
                                             }
                                         }
                                     }
                                 }
                             }
                         },
                         "b": {
@@ -5214,82 +5005,14 @@
                                             },
                                             "df": 1
                                         }
                                     }
                                 }
                             }
                         },
-                        "o": {
-                            "docs": {},
-                            "df": 0,
-                            "r": {
-                                "docs": {},
-                                "df": 0,
-                                "e": {
-                                    "docs": {},
-                                    "df": 0,
-                                    "i": {
-                                        "docs": {},
-                                        "df": 0,
-                                        "g": {
-                                            "docs": {},
-                                            "df": 0,
-                                            "n": {
-                                                "docs": {},
-                                                "df": 0,
-                                                "a": {
-                                                    "docs": {},
-                                                    "df": 0,
-                                                    "u": {
-                                                        "docs": {},
-                                                        "df": 0,
-                                                        "t": {
-                                                            "docs": {},
-                                                            "df": 0,
-                                                            "o": {
-                                                                "docs": {},
-                                                                "df": 0,
-                                                                "i": {
-                                                                    "docs": {},
-                                                                    "df": 0,
-                                                                    "m": {
-                                                                        "docs": {},
-                                                                        "df": 0,
-                                                                        "p": {
-                                                                            "docs": {},
-                                                                            "df": 0,
-                                                                            "o": {
-                                                                                "docs": {},
-                                                                                "df": 0,
-                                                                                "r": {
-                                                                                    "docs": {},
-                                                                                    "df": 0,
-                                                                                    "t": {
-                                                                                        "docs": {
-                                                                                            "pystorcli2.Controller.foreignautoimport": {
-                                                                                                "tf": 1
-                                                                                            }
-                                                                                        },
-                                                                                        "df": 1
-                                                                                    }
-                                                                                }
-                                                                            }
-                                                                        }
-                                                                    }
-                                                                }
-                                                            }
-                                                        }
-                                                    }
-                                                }
-                                            }
-                                        }
-                                    }
-                                }
-                            }
-                        },
                         "r": {
                             "docs": {},
                             "df": 0,
                             "o": {
                                 "docs": {},
                                 "df": 0,
                                 "m": {
@@ -5737,283 +5460,14 @@
                                         },
                                         "df": 1
                                     }
                                 }
                             }
                         }
                     },
-                    "a": {
-                        "docs": {},
-                        "df": 0,
-                        "u": {
-                            "docs": {},
-                            "df": 0,
-                            "t": {
-                                "docs": {},
-                                "df": 0,
-                                "o": {
-                                    "docs": {},
-                                    "df": 0,
-                                    "r": {
-                                        "docs": {},
-                                        "df": 0,
-                                        "e": {
-                                            "docs": {},
-                                            "df": 0,
-                                            "b": {
-                                                "docs": {},
-                                                "df": 0,
-                                                "u": {
-                                                    "docs": {},
-                                                    "df": 0,
-                                                    "i": {
-                                                        "docs": {},
-                                                        "df": 0,
-                                                        "l": {
-                                                            "docs": {},
-                                                            "df": 0,
-                                                            "d": {
-                                                                "docs": {
-                                                                    "pystorcli2.Controller.autorebuild": {
-                                                                        "tf": 1
-                                                                    }
-                                                                },
-                                                                "df": 1
-                                                            }
-                                                        }
-                                                    }
-                                                }
-                                            }
-                                        }
-                                    },
-                                    "b": {
-                                        "docs": {},
-                                        "df": 0,
-                                        "g": {
-                                            "docs": {},
-                                            "df": 0,
-                                            "i": {
-                                                "docs": {
-                                                    "pystorcli2.VirtualDrive.autobgi": {
-                                                        "tf": 1
-                                                    }
-                                                },
-                                                "df": 1
-                                            }
-                                        }
-                                    }
-                                }
-                            }
-                        }
-                    },
-                    "p": {
-                        "docs": {},
-                        "df": 0,
-                        "a": {
-                            "docs": {},
-                            "df": 0,
-                            "t": {
-                                "docs": {},
-                                "df": 0,
-                                "r": {
-                                    "docs": {},
-                                    "df": 0,
-                                    "o": {
-                                        "docs": {},
-                                        "df": 0,
-                                        "l": {
-                                            "docs": {},
-                                            "df": 0,
-                                            "r": {
-                                                "docs": {},
-                                                "df": 0,
-                                                "e": {
-                                                    "docs": {},
-                                                    "df": 0,
-                                                    "a": {
-                                                        "docs": {},
-                                                        "df": 0,
-                                                        "d": {
-                                                            "docs": {
-                                                                "pystorcli2.Controller.patrolread": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.set_patrolread": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.patrolread_start": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.patrolread_stop": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.patrolread_pause": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.patrolread_resume": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.patrolread_running": {
-                                                                    "tf": 1
-                                                                }
-                                                            },
-                                                            "df": 7
-                                                        }
-                                                    }
-                                                }
-                                            }
-                                        }
-                                    }
-                                }
-                            },
-                            "u": {
-                                "docs": {},
-                                "df": 0,
-                                "s": {
-                                    "docs": {},
-                                    "df": 0,
-                                    "e": {
-                                        "docs": {
-                                            "pystorcli2.Controller.patrolread_pause": {
-                                                "tf": 1
-                                            }
-                                        },
-                                        "df": 1
-                                    }
-                                }
-                            }
-                        },
-                        "h": {
-                            "docs": {},
-                            "df": 0,
-                            "y": {
-                                "docs": {},
-                                "df": 0,
-                                "e": {
-                                    "docs": {},
-                                    "df": 0,
-                                    "r": {
-                                        "docs": {},
-                                        "df": 0,
-                                        "r": {
-                                            "docs": {},
-                                            "df": 0,
-                                            "o": {
-                                                "docs": {},
-                                                "df": 0,
-                                                "r": {
-                                                    "docs": {},
-                                                    "df": 0,
-                                                    "c": {
-                                                        "docs": {},
-                                                        "df": 0,
-                                                        "o": {
-                                                            "docs": {},
-                                                            "df": 0,
-                                                            "u": {
-                                                                "docs": {},
-                                                                "df": 0,
-                                                                "n": {
-                                                                    "docs": {},
-                                                                    "df": 0,
-                                                                    "t": {
-                                                                        "docs": {},
-                                                                        "df": 0,
-                                                                        "e": {
-                                                                            "docs": {},
-                                                                            "df": 0,
-                                                                            "r": {
-                                                                                "docs": {},
-                                                                                "df": 0,
-                                                                                "s": {
-                                                                                    "docs": {
-                                                                                        "pystorcli2.Drive.phyerrorcounters": {
-                                                                                            "tf": 1
-                                                                                        },
-                                                                                        "pystorcli2.Drive.phyerrorcounters_reset": {
-                                                                                            "tf": 1
-                                                                                        }
-                                                                                    },
-                                                                                    "df": 2
-                                                                                }
-                                                                            }
-                                                                        }
-                                                                    }
-                                                                }
-                                                            }
-                                                        }
-                                                    }
-                                                }
-                                            }
-                                        }
-                                    }
-                                }
-                            }
-                        },
-                        "d": {
-                            "docs": {},
-                            "df": 0,
-                            "c": {
-                                "docs": {},
-                                "df": 0,
-                                "a": {
-                                    "docs": {},
-                                    "df": 0,
-                                    "c": {
-                                        "docs": {},
-                                        "df": 0,
-                                        "h": {
-                                            "docs": {},
-                                            "df": 0,
-                                            "e": {
-                                                "docs": {
-                                                    "pystorcli2.VirtualDrive.pdcache": {
-                                                        "tf": 1
-                                                    }
-                                                },
-                                                "df": 1
-                                            }
-                                        }
-                                    }
-                                }
-                            }
-                        },
-                        "r": {
-                            "docs": {},
-                            "df": 0,
-                            "o": {
-                                "docs": {},
-                                "df": 0,
-                                "g": {
-                                    "docs": {},
-                                    "df": 0,
-                                    "r": {
-                                        "docs": {},
-                                        "df": 0,
-                                        "e": {
-                                            "docs": {},
-                                            "df": 0,
-                                            "s": {
-                                                "docs": {},
-                                                "df": 0,
-                                                "s": {
-                                                    "docs": {
-                                                        "pystorcli2.VirtualDrive.erase_progress": {
-                                                            "tf": 1
-                                                        }
-                                                    },
-                                                    "df": 1
-                                                }
-                                            }
-                                        }
-                                    }
-                                }
-                            }
-                        }
-                    },
                     "g": {
                         "docs": {},
                         "df": 0,
                         "e": {
                             "docs": {},
                             "df": 0,
                             "t": {
@@ -6401,14 +5855,145 @@
                                         }
                                     },
                                     "df": 1
                                 }
                             }
                         }
                     },
+                    "p": {
+                        "docs": {},
+                        "df": 0,
+                        "h": {
+                            "docs": {},
+                            "df": 0,
+                            "y": {
+                                "docs": {},
+                                "df": 0,
+                                "e": {
+                                    "docs": {},
+                                    "df": 0,
+                                    "r": {
+                                        "docs": {},
+                                        "df": 0,
+                                        "r": {
+                                            "docs": {},
+                                            "df": 0,
+                                            "o": {
+                                                "docs": {},
+                                                "df": 0,
+                                                "r": {
+                                                    "docs": {},
+                                                    "df": 0,
+                                                    "c": {
+                                                        "docs": {},
+                                                        "df": 0,
+                                                        "o": {
+                                                            "docs": {},
+                                                            "df": 0,
+                                                            "u": {
+                                                                "docs": {},
+                                                                "df": 0,
+                                                                "n": {
+                                                                    "docs": {},
+                                                                    "df": 0,
+                                                                    "t": {
+                                                                        "docs": {},
+                                                                        "df": 0,
+                                                                        "e": {
+                                                                            "docs": {},
+                                                                            "df": 0,
+                                                                            "r": {
+                                                                                "docs": {},
+                                                                                "df": 0,
+                                                                                "s": {
+                                                                                    "docs": {
+                                                                                        "pystorcli2.Drive.phyerrorcounters": {
+                                                                                            "tf": 1
+                                                                                        },
+                                                                                        "pystorcli2.Drive.phyerrorcounters_reset": {
+                                                                                            "tf": 1
+                                                                                        }
+                                                                                    },
+                                                                                    "df": 2
+                                                                                }
+                                                                            }
+                                                                        }
+                                                                    }
+                                                                }
+                                                            }
+                                                        }
+                                                    }
+                                                }
+                                            }
+                                        }
+                                    }
+                                }
+                            }
+                        },
+                        "d": {
+                            "docs": {},
+                            "df": 0,
+                            "c": {
+                                "docs": {},
+                                "df": 0,
+                                "a": {
+                                    "docs": {},
+                                    "df": 0,
+                                    "c": {
+                                        "docs": {},
+                                        "df": 0,
+                                        "h": {
+                                            "docs": {},
+                                            "df": 0,
+                                            "e": {
+                                                "docs": {
+                                                    "pystorcli2.VirtualDrive.pdcache": {
+                                                        "tf": 1
+                                                    }
+                                                },
+                                                "df": 1
+                                            }
+                                        }
+                                    }
+                                }
+                            }
+                        },
+                        "r": {
+                            "docs": {},
+                            "df": 0,
+                            "o": {
+                                "docs": {},
+                                "df": 0,
+                                "g": {
+                                    "docs": {},
+                                    "df": 0,
+                                    "r": {
+                                        "docs": {},
+                                        "df": 0,
+                                        "e": {
+                                            "docs": {},
+                                            "df": 0,
+                                            "s": {
+                                                "docs": {},
+                                                "df": 0,
+                                                "s": {
+                                                    "docs": {
+                                                        "pystorcli2.VirtualDrive.erase_progress": {
+                                                            "tf": 1
+                                                        }
+                                                    },
+                                                    "df": 1
+                                                }
+                                            }
+                                        }
+                                    }
+                                }
+                            }
+                        }
+                    },
                     "b": {
                         "docs": {},
                         "df": 0,
                         "o": {
                             "docs": {},
                             "df": 0,
                             "o": {
@@ -6440,14 +6025,46 @@
                                                 }
                                             }
                                         }
                                     }
                                 }
                             }
                         }
+                    },
+                    "a": {
+                        "docs": {},
+                        "df": 0,
+                        "u": {
+                            "docs": {},
+                            "df": 0,
+                            "t": {
+                                "docs": {},
+                                "df": 0,
+                                "o": {
+                                    "docs": {},
+                                    "df": 0,
+                                    "b": {
+                                        "docs": {},
+                                        "df": 0,
+                                        "g": {
+                                            "docs": {},
+                                            "df": 0,
+                                            "i": {
+                                                "docs": {
+                                                    "pystorcli2.VirtualDrive.autobgi": {
+                                                        "tf": 1
+                                                    }
+                                                },
+                                                "df": 1
+                                            }
+                                        }
+                                    }
+                                }
+                            }
+                        }
                     }
                 }
             },
             "fullname": {
                 "root": {
                     "docs": {
                         "pystorcli2.StorCLI.__init__": {
@@ -6577,41 +6194,14 @@
                                                                 },
                                                                 "pystorcli2.Controller.drives_ids": {
                                                                     "tf": 1
                                                                 },
                                                                 "pystorcli2.Controller.create_vd": {
                                                                     "tf": 1
                                                                 },
-                                                                "pystorcli2.Controller.autorebuild": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.foreignautoimport": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.patrolread": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.set_patrolread": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.patrolread_start": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.patrolread_stop": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.patrolread_pause": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.patrolread_resume": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.patrolread_running": {
-                                                                    "tf": 1
-                                                                },
                                                                 "pystorcli2.Controllers": {
                                                                     "tf": 1
                                                                 },
                                                                 "pystorcli2.Controllers.__init__": {
                                                                     "tf": 1
                                                                 },
                                                                 "pystorcli2.Controllers.ids": {
@@ -6986,100 +6576,26 @@
                                                                 "pystorcli2.VirtualDrives.get_vd": {
                                                                     "tf": 1
                                                                 },
                                                                 "pystorcli2.VirtualDrives.get_named_vd": {
                                                                     "tf": 1
                                                                 }
                                                             },
-                                                            "df": 161
+                                                            "df": 152
                                                         },
                                                         "docs": {},
                                                         "df": 0
                                                     }
                                                 }
                                             }
                                         }
                                     }
                                 }
                             }
                         },
-                        "a": {
-                            "docs": {},
-                            "df": 0,
-                            "t": {
-                                "docs": {},
-                                "df": 0,
-                                "r": {
-                                    "docs": {},
-                                    "df": 0,
-                                    "o": {
-                                        "docs": {},
-                                        "df": 0,
-                                        "l": {
-                                            "docs": {},
-                                            "df": 0,
-                                            "r": {
-                                                "docs": {},
-                                                "df": 0,
-                                                "e": {
-                                                    "docs": {},
-                                                    "df": 0,
-                                                    "a": {
-                                                        "docs": {},
-                                                        "df": 0,
-                                                        "d": {
-                                                            "docs": {
-                                                                "pystorcli2.Controller.patrolread": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.set_patrolread": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.patrolread_start": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.patrolread_stop": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.patrolread_pause": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.patrolread_resume": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.patrolread_running": {
-                                                                    "tf": 1
-                                                                }
-                                                            },
-                                                            "df": 7
-                                                        }
-                                                    }
-                                                }
-                                            }
-                                        }
-                                    }
-                                }
-                            },
-                            "u": {
-                                "docs": {},
-                                "df": 0,
-                                "s": {
-                                    "docs": {},
-                                    "df": 0,
-                                    "e": {
-                                        "docs": {
-                                            "pystorcli2.Controller.patrolread_pause": {
-                                                "tf": 1
-                                            }
-                                        },
-                                        "df": 1
-                                    }
-                                }
-                            }
-                        },
                         "h": {
                             "docs": {},
                             "df": 0,
                             "y": {
                                 "docs": {},
                                 "df": 0,
                                 "e": {
@@ -7270,31 +6786,28 @@
                                                 "df": 14
                                             }
                                         }
                                     }
                                 },
                                 "p": {
                                     "docs": {
-                                        "pystorcli2.Controller.patrolread_stop": {
-                                            "tf": 1
-                                        },
                                         "pystorcli2.Drive.init_stop": {
                                             "tf": 1
                                         },
                                         "pystorcli2.Drive.erase_stop": {
                                             "tf": 1
                                         },
                                         "pystorcli2.VirtualDrive.init_stop": {
                                             "tf": 1
                                         },
                                         "pystorcli2.VirtualDrive.erase_stop": {
                                             "tf": 1
                                         }
                                     },
-                                    "df": 5
+                                    "df": 4
                                 }
                             },
                             "a": {
                                 "docs": {},
                                 "df": 0,
                                 "t": {
                                     "docs": {},
@@ -7327,17 +6840,14 @@
                                     }
                                 },
                                 "r": {
                                     "docs": {},
                                     "df": 0,
                                     "t": {
                                         "docs": {
-                                            "pystorcli2.Controller.patrolread_start": {
-                                                "tf": 1
-                                            },
                                             "pystorcli2.Drive.init_start": {
                                                 "tf": 1
                                             },
                                             "pystorcli2.Drive.erase_start": {
                                                 "tf": 1
                                             },
                                             "pystorcli2.VirtualDrive.init_start": {
@@ -7346,15 +6856,15 @@
                                             "pystorcli2.VirtualDrive.erase_start": {
                                                 "tf": 1
                                             },
                                             "pystorcli2.VirtualDrive.migrate_start": {
                                                 "tf": 1
                                             }
                                         },
-                                        "df": 6
+                                        "df": 5
                                     }
                                 }
                             },
                             "r": {
                                 "docs": {
                                     "pystorcli2.DriveState.settable_str": {
                                         "tf": 1
@@ -7391,22 +6901,19 @@
                             "docs": {},
                             "df": 0,
                             "t": {
                                 "docs": {
                                     "pystorcli2.StorCLI.set_cmdrunner": {
                                         "tf": 1
                                     },
-                                    "pystorcli2.Controller.set_patrolread": {
-                                        "tf": 1
-                                    },
                                     "pystorcli2.Drive.set_state": {
                                         "tf": 1
                                     }
                                 },
-                                "df": 3,
+                                "df": 2,
                                 "t": {
                                     "docs": {},
                                     "df": 0,
                                     "a": {
                                         "docs": {},
                                         "df": 0,
                                         "b": {
@@ -7939,44 +7446,17 @@
                                                                     "tf": 1
                                                                 },
                                                                 "pystorcli2.Controller.drives_ids": {
                                                                     "tf": 1
                                                                 },
                                                                 "pystorcli2.Controller.create_vd": {
                                                                     "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.autorebuild": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.foreignautoimport": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.patrolread": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.set_patrolread": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.patrolread_start": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.patrolread_stop": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.patrolread_pause": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.patrolread_resume": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.patrolread_running": {
-                                                                    "tf": 1
                                                                 }
                                                             },
-                                                            "df": 19,
+                                                            "df": 10,
                                                             "s": {
                                                                 "docs": {
                                                                     "pystorcli2.StorCLI.controllers": {
                                                                         "tf": 1
                                                                     },
                                                                     "pystorcli2.Controllers": {
                                                                         "tf": 1
@@ -8411,30 +7891,14 @@
                                                     },
                                                     "df": 1
                                                 }
                                             }
                                         }
                                     }
                                 },
-                                "u": {
-                                    "docs": {},
-                                    "df": 0,
-                                    "m": {
-                                        "docs": {},
-                                        "df": 0,
-                                        "e": {
-                                            "docs": {
-                                                "pystorcli2.Controller.patrolread_resume": {
-                                                    "tf": 1
-                                                }
-                                            },
-                                            "df": 1
-                                        }
-                                    }
-                                },
                                 "e": {
                                     "docs": {},
                                     "df": 0,
                                     "t": {
                                         "docs": {
                                             "pystorcli2.Drive.phyerrorcounters_reset": {
                                                 "tf": 1
@@ -8462,17 +7926,14 @@
                                         "docs": {},
                                         "df": 0,
                                         "n": {
                                             "docs": {},
                                             "df": 0,
                                             "g": {
                                                 "docs": {
-                                                    "pystorcli2.Controller.patrolread_running": {
-                                                        "tf": 1
-                                                    },
                                                     "pystorcli2.Drive.init_running": {
                                                         "tf": 1
                                                     },
                                                     "pystorcli2.Drive.erase_running": {
                                                         "tf": 1
                                                     },
                                                     "pystorcli2.VirtualDrive.init_running": {
@@ -8481,15 +7942,15 @@
                                                     "pystorcli2.VirtualDrive.erase_running": {
                                                         "tf": 1
                                                     },
                                                     "pystorcli2.VirtualDrive.migrate_running": {
                                                         "tf": 1
                                                     }
                                                 },
-                                                "df": 6
+                                                "df": 5
                                             }
                                         }
                                     }
                                 }
                             }
                         },
                         "b": {
@@ -8994,82 +8455,14 @@
                                             },
                                             "df": 1
                                         }
                                     }
                                 }
                             }
                         },
-                        "o": {
-                            "docs": {},
-                            "df": 0,
-                            "r": {
-                                "docs": {},
-                                "df": 0,
-                                "e": {
-                                    "docs": {},
-                                    "df": 0,
-                                    "i": {
-                                        "docs": {},
-                                        "df": 0,
-                                        "g": {
-                                            "docs": {},
-                                            "df": 0,
-                                            "n": {
-                                                "docs": {},
-                                                "df": 0,
-                                                "a": {
-                                                    "docs": {},
-                                                    "df": 0,
-                                                    "u": {
-                                                        "docs": {},
-                                                        "df": 0,
-                                                        "t": {
-                                                            "docs": {},
-                                                            "df": 0,
-                                                            "o": {
-                                                                "docs": {},
-                                                                "df": 0,
-                                                                "i": {
-                                                                    "docs": {},
-                                                                    "df": 0,
-                                                                    "m": {
-                                                                        "docs": {},
-                                                                        "df": 0,
-                                                                        "p": {
-                                                                            "docs": {},
-                                                                            "df": 0,
-                                                                            "o": {
-                                                                                "docs": {},
-                                                                                "df": 0,
-                                                                                "r": {
-                                                                                    "docs": {},
-                                                                                    "df": 0,
-                                                                                    "t": {
-                                                                                        "docs": {
-                                                                                            "pystorcli2.Controller.foreignautoimport": {
-                                                                                                "tf": 1
-                                                                                            }
-                                                                                        },
-                                                                                        "df": 1
-                                                                                    }
-                                                                                }
-                                                                            }
-                                                                        }
-                                                                    }
-                                                                }
-                                                            }
-                                                        }
-                                                    }
-                                                }
-                                            }
-                                        }
-                                    }
-                                }
-                            }
-                        },
                         "r": {
                             "docs": {},
                             "df": 0,
                             "o": {
                                 "docs": {},
                                 "df": 0,
                                 "m": {
@@ -9517,78 +8910,14 @@
                                         },
                                         "df": 1
                                     }
                                 }
                             }
                         }
                     },
-                    "a": {
-                        "docs": {},
-                        "df": 0,
-                        "u": {
-                            "docs": {},
-                            "df": 0,
-                            "t": {
-                                "docs": {},
-                                "df": 0,
-                                "o": {
-                                    "docs": {},
-                                    "df": 0,
-                                    "r": {
-                                        "docs": {},
-                                        "df": 0,
-                                        "e": {
-                                            "docs": {},
-                                            "df": 0,
-                                            "b": {
-                                                "docs": {},
-                                                "df": 0,
-                                                "u": {
-                                                    "docs": {},
-                                                    "df": 0,
-                                                    "i": {
-                                                        "docs": {},
-                                                        "df": 0,
-                                                        "l": {
-                                                            "docs": {},
-                                                            "df": 0,
-                                                            "d": {
-                                                                "docs": {
-                                                                    "pystorcli2.Controller.autorebuild": {
-                                                                        "tf": 1
-                                                                    }
-                                                                },
-                                                                "df": 1
-                                                            }
-                                                        }
-                                                    }
-                                                }
-                                            }
-                                        }
-                                    },
-                                    "b": {
-                                        "docs": {},
-                                        "df": 0,
-                                        "g": {
-                                            "docs": {},
-                                            "df": 0,
-                                            "i": {
-                                                "docs": {
-                                                    "pystorcli2.VirtualDrive.autobgi": {
-                                                        "tf": 1
-                                                    }
-                                                },
-                                                "df": 1
-                                            }
-                                        }
-                                    }
-                                }
-                            }
-                        }
-                    },
                     "g": {
                         "docs": {},
                         "df": 0,
                         "e": {
                             "docs": {},
                             "df": 0,
                             "t": {
@@ -10015,14 +9344,46 @@
                                                 }
                                             }
                                         }
                                     }
                                 }
                             }
                         }
+                    },
+                    "a": {
+                        "docs": {},
+                        "df": 0,
+                        "u": {
+                            "docs": {},
+                            "df": 0,
+                            "t": {
+                                "docs": {},
+                                "df": 0,
+                                "o": {
+                                    "docs": {},
+                                    "df": 0,
+                                    "b": {
+                                        "docs": {},
+                                        "df": 0,
+                                        "g": {
+                                            "docs": {},
+                                            "df": 0,
+                                            "i": {
+                                                "docs": {
+                                                    "pystorcli2.VirtualDrive.autobgi": {
+                                                        "tf": 1
+                                                    }
+                                                },
+                                                "df": 1
+                                            }
+                                        }
+                                    }
+                                }
+                            }
+                        }
                     }
                 }
             },
             "annotation": {
                 "root": {
                     "docs": {
                         "pystorcli2.StorCLI.full_version": {
@@ -11818,17 +11179,14 @@
                                 },
                                 "pystorcli2.Controller.__init__": {
                                     "tf": 1.4142135623730951
                                 },
                                 "pystorcli2.Controller.create_vd": {
                                     "tf": 1.4142135623730951
                                 },
-                                "pystorcli2.Controller.set_patrolread": {
-                                    "tf": 1.4142135623730951
-                                },
                                 "pystorcli2.Controllers.__init__": {
                                     "tf": 1.4142135623730951
                                 },
                                 "pystorcli2.Enclosure.__init__": {
                                     "tf": 1.4142135623730951
                                 },
                                 "pystorcli2.Enclosures.__init__": {
@@ -11849,15 +11207,15 @@
                                 "pystorcli2.VirtualDrive.erase_start": {
                                     "tf": 1.4142135623730951
                                 },
                                 "pystorcli2.VirtualDrives.__init__": {
                                     "tf": 1.4142135623730951
                                 }
                             },
-                            "df": 13
+                            "df": 12
                         },
                         "docs": {},
                         "df": 0
                     },
                     "6": {
                         "4": {
                             "docs": {
@@ -11897,29 +11255,14 @@
                         },
                         "pystorcli2.Controller.__init__": {
                             "tf": 4.242640687119285
                         },
                         "pystorcli2.Controller.create_vd": {
                             "tf": 9.486832980505138
                         },
-                        "pystorcli2.Controller.set_patrolread": {
-                            "tf": 4.898979485566356
-                        },
-                        "pystorcli2.Controller.patrolread_start": {
-                            "tf": 3.1622776601683795
-                        },
-                        "pystorcli2.Controller.patrolread_stop": {
-                            "tf": 3.1622776601683795
-                        },
-                        "pystorcli2.Controller.patrolread_pause": {
-                            "tf": 3.1622776601683795
-                        },
-                        "pystorcli2.Controller.patrolread_resume": {
-                            "tf": 3.1622776601683795
-                        },
                         "pystorcli2.Controllers.__init__": {
                             "tf": 3.7416573867739413
                         },
                         "pystorcli2.Controllers.get_ctl": {
                             "tf": 5.744562646538029
                         },
                         "pystorcli2.Enclosure.__init__": {
@@ -12009,15 +11352,15 @@
                         "pystorcli2.VirtualDrives.get_vd": {
                             "tf": 3.7416573867739413
                         },
                         "pystorcli2.VirtualDrives.get_named_vd": {
                             "tf": 3.7416573867739413
                         }
                     },
-                    "df": 47,
+                    "df": 42,
                     "b": {
                         "docs": {},
                         "df": 0,
                         "i": {
                             "docs": {},
                             "df": 0,
                             "n": {
@@ -12296,29 +11639,14 @@
                                         },
                                         "pystorcli2.StorCLI.run": {
                                             "tf": 1
                                         },
                                         "pystorcli2.Controller.create_vd": {
                                             "tf": 1
                                         },
-                                        "pystorcli2.Controller.set_patrolread": {
-                                            "tf": 1
-                                        },
-                                        "pystorcli2.Controller.patrolread_start": {
-                                            "tf": 1
-                                        },
-                                        "pystorcli2.Controller.patrolread_stop": {
-                                            "tf": 1
-                                        },
-                                        "pystorcli2.Controller.patrolread_pause": {
-                                            "tf": 1
-                                        },
-                                        "pystorcli2.Controller.patrolread_resume": {
-                                            "tf": 1
-                                        },
                                         "pystorcli2.Controllers.get_ctl": {
                                             "tf": 1
                                         },
                                         "pystorcli2.Enclosures.get_encl": {
                                             "tf": 1
                                         },
                                         "pystorcli2.DriveState.is_good": {
@@ -12384,15 +11712,15 @@
                                         "pystorcli2.VirtualDrives.get_vd": {
                                             "tf": 1
                                         },
                                         "pystorcli2.VirtualDrives.get_named_vd": {
                                             "tf": 1
                                         }
                                     },
-                                    "df": 33
+                                    "df": 28
                                 }
                             }
                         },
                         "l": {
                             "docs": {},
                             "df": 0,
                             "o": {
@@ -13121,22 +12449,19 @@
                                 "docs": {},
                                 "df": 0,
                                 "u": {
                                     "docs": {},
                                     "df": 0,
                                     "e": {
                                         "docs": {
-                                            "pystorcli2.Controller.set_patrolread": {
-                                                "tf": 1
-                                            },
                                             "pystorcli2.Drive.set_state": {
                                                 "tf": 1
                                             }
                                         },
-                                        "df": 2
+                                        "df": 1
                                     }
                                 }
                             }
                         },
                         "d": {
                             "docs": {
                                 "pystorcli2.VirtualDrive.__init__": {
@@ -13148,64 +12473,14 @@
                                 "pystorcli2.VirtualDrives.get_named_vd": {
                                     "tf": 1
                                 }
                             },
                             "df": 3
                         }
                     },
-                    "m": {
-                        "docs": {},
-                        "df": 0,
-                        "o": {
-                            "docs": {},
-                            "df": 0,
-                            "d": {
-                                "docs": {},
-                                "df": 0,
-                                "e": {
-                                    "docs": {
-                                        "pystorcli2.Controller.set_patrolread": {
-                                            "tf": 1
-                                        },
-                                        "pystorcli2.Drive.erase_start": {
-                                            "tf": 1
-                                        },
-                                        "pystorcli2.VirtualDrive.erase_start": {
-                                            "tf": 1
-                                        }
-                                    },
-                                    "df": 3
-                                }
-                            }
-                        },
-                        "a": {
-                            "docs": {},
-                            "df": 0,
-                            "n": {
-                                "docs": {},
-                                "df": 0,
-                                "u": {
-                                    "docs": {},
-                                    "df": 0,
-                                    "a": {
-                                        "docs": {},
-                                        "df": 0,
-                                        "l": {
-                                            "docs": {
-                                                "pystorcli2.Controller.set_patrolread": {
-                                                    "tf": 1
-                                                }
-                                            },
-                                            "df": 1
-                                        }
-                                    }
-                                }
-                            }
-                        }
-                    },
                     "e": {
                         "docs": {},
                         "df": 0,
                         "n": {
                             "docs": {},
                             "df": 0,
                             "c": {
@@ -13298,14 +12573,37 @@
                                         "tf": 1
                                     }
                                 },
                                 "df": 2
                             }
                         }
                     },
+                    "m": {
+                        "docs": {},
+                        "df": 0,
+                        "o": {
+                            "docs": {},
+                            "df": 0,
+                            "d": {
+                                "docs": {},
+                                "df": 0,
+                                "e": {
+                                    "docs": {
+                                        "pystorcli2.Drive.erase_start": {
+                                            "tf": 1
+                                        },
+                                        "pystorcli2.VirtualDrive.erase_start": {
+                                            "tf": 1
+                                        }
+                                    },
+                                    "df": 2
+                                }
+                            }
+                        }
+                    },
                     "u": {
                         "docs": {},
                         "df": 0,
                         "n": {
                             "docs": {},
                             "df": 0,
                             "i": {
@@ -13605,15 +12903,15 @@
                         "pystorcli2.StorCLI.version": {
                             "tf": 1.4142135623730951
                         },
                         "pystorcli2.StorCLI.controllers": {
                             "tf": 1.4142135623730951
                         },
                         "pystorcli2.Controller": {
-                            "tf": 5.656854249492381
+                            "tf": 4.358898943540674
                         },
                         "pystorcli2.Controller.__init__": {
                             "tf": 2.449489742783178
                         },
                         "pystorcli2.Controller.id": {
                             "tf": 2
                         },
@@ -13634,41 +12932,14 @@
                         },
                         "pystorcli2.Controller.drives_ids": {
                             "tf": 2.23606797749979
                         },
                         "pystorcli2.Controller.create_vd": {
                             "tf": 3.4641016151377544
                         },
-                        "pystorcli2.Controller.autorebuild": {
-                            "tf": 1.4142135623730951
-                        },
-                        "pystorcli2.Controller.foreignautoimport": {
-                            "tf": 1.4142135623730951
-                        },
-                        "pystorcli2.Controller.patrolread": {
-                            "tf": 1.4142135623730951
-                        },
-                        "pystorcli2.Controller.set_patrolread": {
-                            "tf": 2.8284271247461903
-                        },
-                        "pystorcli2.Controller.patrolread_start": {
-                            "tf": 2.23606797749979
-                        },
-                        "pystorcli2.Controller.patrolread_stop": {
-                            "tf": 2.23606797749979
-                        },
-                        "pystorcli2.Controller.patrolread_pause": {
-                            "tf": 2.23606797749979
-                        },
-                        "pystorcli2.Controller.patrolread_resume": {
-                            "tf": 2.23606797749979
-                        },
-                        "pystorcli2.Controller.patrolread_running": {
-                            "tf": 2.449489742783178
-                        },
                         "pystorcli2.Controllers": {
                             "tf": 3.605551275463989
                         },
                         "pystorcli2.Controllers.__init__": {
                             "tf": 2.23606797749979
                         },
                         "pystorcli2.Controllers.ids": {
@@ -14043,15 +13314,15 @@
                         "pystorcli2.VirtualDrives.get_vd": {
                             "tf": 3
                         },
                         "pystorcli2.VirtualDrives.get_named_vd": {
                             "tf": 3
                         }
                     },
-                    "df": 161,
+                    "df": 152,
                     "s": {
                         "docs": {
                             "pystorcli2.Drive.erase_start": {
                                 "tf": 1
                             },
                             "pystorcli2.VirtualDrive.erase_start": {
                                 "tf": 1
@@ -14287,36 +13558,27 @@
                                                 }
                                             }
                                         }
                                     }
                                 },
                                 "p": {
                                     "docs": {
-                                        "pystorcli2.Controller": {
-                                            "tf": 1
-                                        },
                                         "pystorcli2.Drive": {
                                             "tf": 1.7320508075688772
                                         },
                                         "pystorcli2.Drive.init_stop": {
                                             "tf": 1
                                         },
                                         "pystorcli2.VirtualDrive": {
                                             "tf": 2
                                         }
                                     },
-                                    "df": 4,
+                                    "df": 3,
                                     "s": {
                                         "docs": {
-                                            "pystorcli2.Controller": {
-                                                "tf": 1
-                                            },
-                                            "pystorcli2.Controller.patrolread_stop": {
-                                                "tf": 1
-                                            },
                                             "pystorcli2.Drive": {
                                                 "tf": 1.4142135623730951
                                             },
                                             "pystorcli2.Drive.erase_stop": {
                                                 "tf": 1
                                             },
                                             "pystorcli2.VirtualDrive": {
@@ -14325,15 +13587,15 @@
                                             "pystorcli2.VirtualDrive.init_stop": {
                                                 "tf": 1
                                             },
                                             "pystorcli2.VirtualDrive.erase_stop": {
                                                 "tf": 1
                                             }
                                         },
-                                        "df": 7
+                                        "df": 5
                                     },
                                     "p": {
                                         "docs": {},
                                         "df": 0,
                                         "e": {
                                             "docs": {},
                                             "df": 0,
@@ -14380,17 +13642,14 @@
                                     },
                                     "pystorcli2.Controller.drives_ids": {
                                         "tf": 1
                                     },
                                     "pystorcli2.Controller.create_vd": {
                                         "tf": 2
                                     },
-                                    "pystorcli2.Controller.set_patrolread": {
-                                        "tf": 1.4142135623730951
-                                    },
                                     "pystorcli2.Controllers": {
                                         "tf": 1.4142135623730951
                                     },
                                     "pystorcli2.Controllers.__init__": {
                                         "tf": 1
                                     },
                                     "pystorcli2.Controllers.ids": {
@@ -14582,15 +13841,15 @@
                                     "pystorcli2.VirtualDrives.get_vd": {
                                         "tf": 1
                                     },
                                     "pystorcli2.VirtualDrives.get_named_vd": {
                                         "tf": 1
                                     }
                                 },
-                                "df": 77,
+                                "df": 76,
                                 "i": {
                                     "docs": {},
                                     "df": 0,
                                     "p": {
                                         "docs": {
                                             "pystorcli2.Controller.create_vd": {
                                                 "tf": 1.4142135623730951
@@ -14678,20 +13937,14 @@
                                                     "df": 1
                                                 }
                                             }
                                         }
                                     },
                                     "e": {
                                         "docs": {
-                                            "pystorcli2.Controller": {
-                                                "tf": 1.4142135623730951
-                                            },
-                                            "pystorcli2.Controller.set_patrolread": {
-                                                "tf": 1
-                                            },
                                             "pystorcli2.Drive": {
                                                 "tf": 1.7320508075688772
                                             },
                                             "pystorcli2.Drive.state": {
                                                 "tf": 1
                                             },
                                             "pystorcli2.Drive.set_state": {
@@ -14700,15 +13953,15 @@
                                             "pystorcli2.VirtualDrive": {
                                                 "tf": 1.4142135623730951
                                             },
                                             "pystorcli2.VirtualDrive.state": {
                                                 "tf": 1
                                             }
                                         },
-                                        "df": 7,
+                                        "df": 5,
                                         "s": {
                                             "docs": {
                                                 "pystorcli2.Drive.spin": {
                                                     "tf": 1
                                                 }
                                             },
                                             "df": 1
@@ -14716,53 +13969,44 @@
                                     }
                                 },
                                 "r": {
                                     "docs": {},
                                     "df": 0,
                                     "t": {
                                         "docs": {
-                                            "pystorcli2.Controller": {
-                                                "tf": 1
-                                            },
                                             "pystorcli2.Drive": {
                                                 "tf": 1.7320508075688772
                                             },
                                             "pystorcli2.Drive.init_start": {
                                                 "tf": 1
                                             },
                                             "pystorcli2.VirtualDrive": {
                                                 "tf": 2
                                             },
                                             "pystorcli2.VirtualDrive.migrate_start": {
                                                 "tf": 1
                                             }
                                         },
-                                        "df": 5,
+                                        "df": 4,
                                         "s": {
                                             "docs": {
-                                                "pystorcli2.Controller": {
-                                                    "tf": 1
-                                                },
-                                                "pystorcli2.Controller.patrolread_start": {
-                                                    "tf": 1
-                                                },
                                                 "pystorcli2.Drive": {
                                                     "tf": 1
                                                 },
                                                 "pystorcli2.VirtualDrive": {
                                                     "tf": 1.4142135623730951
                                                 },
                                                 "pystorcli2.VirtualDrive.init_start": {
                                                     "tf": 1
                                                 },
                                                 "pystorcli2.VirtualDrive.migrate_start": {
                                                     "tf": 1
                                                 }
                                             },
-                                            "df": 6
+                                            "df": 4
                                         }
                                     }
                                 },
                                 "n": {
                                     "docs": {},
                                     "df": 0,
                                     "d": {
@@ -14850,20 +14094,14 @@
                                 "docs": {
                                     "pystorcli2.StorCLI": {
                                         "tf": 1
                                     },
                                     "pystorcli2.StorCLI.set_cmdrunner": {
                                         "tf": 1
                                     },
-                                    "pystorcli2.Controller": {
-                                        "tf": 1
-                                    },
-                                    "pystorcli2.Controller.set_patrolread": {
-                                        "tf": 1
-                                    },
                                     "pystorcli2.DriveState.is_settable": {
                                         "tf": 1.4142135623730951
                                     },
                                     "pystorcli2.DriveState.settable_str": {
                                         "tf": 1
                                     },
                                     "pystorcli2.Drive.state": {
@@ -14896,37 +14134,54 @@
                                     "pystorcli2.VirtualDrive.init_start": {
                                         "tf": 1
                                     },
                                     "pystorcli2.VirtualDrive.delete": {
                                         "tf": 1
                                     }
                                 },
-                                "df": 17,
+                                "df": 15,
                                 "t": {
                                     "docs": {},
                                     "df": 0,
                                     "e": {
                                         "docs": {},
                                         "df": 0,
                                         "r": {
                                             "docs": {
                                                 "pystorcli2.StorCLI": {
                                                     "tf": 1
                                                 },
-                                                "pystorcli2.Controller": {
-                                                    "tf": 1.7320508075688772
-                                                },
                                                 "pystorcli2.Drive": {
                                                     "tf": 1.7320508075688772
                                                 },
                                                 "pystorcli2.VirtualDrive": {
                                                     "tf": 2.6457513110645907
                                                 }
                                             },
-                                            "df": 4
+                                            "df": 3
+                                        }
+                                    },
+                                    "a": {
+                                        "docs": {},
+                                        "df": 0,
+                                        "b": {
+                                            "docs": {},
+                                            "df": 0,
+                                            "l": {
+                                                "docs": {},
+                                                "df": 0,
+                                                "e": {
+                                                    "docs": {
+                                                        "pystorcli2.DriveState.settable_str": {
+                                                            "tf": 1
+                                                        }
+                                                    },
+                                                    "df": 1
+                                                }
+                                            }
                                         }
                                     },
                                     "i": {
                                         "docs": {},
                                         "df": 0,
                                         "n": {
                                             "docs": {},
@@ -14945,43 +14200,15 @@
                                                     "pystorcli2.VirtualDrive.rdcache": {
                                                         "tf": 1
                                                     },
                                                     "pystorcli2.VirtualDrive.iopolicy": {
                                                         "tf": 1
                                                     }
                                                 },
-                                                "df": 5,
-                                                "s": {
-                                                    "docs": {
-                                                        "pystorcli2.Controller": {
-                                                            "tf": 1
-                                                        }
-                                                    },
-                                                    "df": 1
-                                                }
-                                            }
-                                        }
-                                    },
-                                    "a": {
-                                        "docs": {},
-                                        "df": 0,
-                                        "b": {
-                                            "docs": {},
-                                            "df": 0,
-                                            "l": {
-                                                "docs": {},
-                                                "df": 0,
-                                                "e": {
-                                                    "docs": {
-                                                        "pystorcli2.DriveState.settable_str": {
-                                                            "tf": 1
-                                                        }
-                                                    },
-                                                    "df": 1
-                                                }
+                                                "df": 5
                                             }
                                         }
                                     }
                                 },
                                 "s": {
                                     "docs": {
                                         "pystorcli2.Drive.hotparedrive_create": {
@@ -15381,49 +14608,14 @@
                                             }
                                         },
                                         "df": 1
                                     }
                                 }
                             }
                         },
-                        "c": {
-                            "docs": {},
-                            "df": 0,
-                            "h": {
-                                "docs": {},
-                                "df": 0,
-                                "e": {
-                                    "docs": {},
-                                    "df": 0,
-                                    "d": {
-                                        "docs": {},
-                                        "df": 0,
-                                        "u": {
-                                            "docs": {},
-                                            "df": 0,
-                                            "l": {
-                                                "docs": {},
-                                                "df": 0,
-                                                "e": {
-                                                    "docs": {
-                                                        "pystorcli2.Controller": {
-                                                            "tf": 1
-                                                        },
-                                                        "pystorcli2.Controller.set_patrolread": {
-                                                            "tf": 1
-                                                        }
-                                                    },
-                                                    "df": 2
-                                                }
-                                            }
-                                        }
-                                    }
-                                }
-                            }
-                        },
                         "h": {
                             "docs": {},
                             "df": 0,
                             "o": {
                                 "docs": {},
                                 "df": 0,
                                 "w": {
@@ -15655,68 +14847,14 @@
                                         },
                                         "pystorcli2.VirtualDrives.__init__": {
                                             "tf": 1
                                         }
                                     },
                                     "df": 19
                                 },
-                                "r": {
-                                    "docs": {},
-                                    "df": 0,
-                                    "o": {
-                                        "docs": {},
-                                        "df": 0,
-                                        "l": {
-                                            "docs": {
-                                                "pystorcli2.Controller": {
-                                                    "tf": 2.8284271247461903
-                                                },
-                                                "pystorcli2.Controller.set_patrolread": {
-                                                    "tf": 1.7320508075688772
-                                                },
-                                                "pystorcli2.Controller.patrolread_start": {
-                                                    "tf": 1
-                                                },
-                                                "pystorcli2.Controller.patrolread_stop": {
-                                                    "tf": 1
-                                                },
-                                                "pystorcli2.Controller.patrolread_pause": {
-                                                    "tf": 1
-                                                },
-                                                "pystorcli2.Controller.patrolread_resume": {
-                                                    "tf": 1
-                                                },
-                                                "pystorcli2.Controller.patrolread_running": {
-                                                    "tf": 1
-                                                }
-                                            },
-                                            "df": 7,
-                                            "r": {
-                                                "docs": {},
-                                                "df": 0,
-                                                "e": {
-                                                    "docs": {},
-                                                    "df": 0,
-                                                    "a": {
-                                                        "docs": {},
-                                                        "df": 0,
-                                                        "d": {
-                                                            "docs": {
-                                                                "pystorcli2.Controller": {
-                                                                    "tf": 2.6457513110645907
-                                                                }
-                                                            },
-                                                            "df": 1
-                                                        }
-                                                    }
-                                                }
-                                            }
-                                        }
-                                    }
-                                },
                                 "t": {
                                     "docs": {},
                                     "df": 0,
                                     "e": {
                                         "docs": {},
                                         "df": 0,
                                         "r": {
@@ -15788,36 +14926,22 @@
                                 "docs": {},
                                 "df": 0,
                                 "s": {
                                     "docs": {},
                                     "df": 0,
                                     "e": {
                                         "docs": {
-                                            "pystorcli2.Controller": {
-                                                "tf": 1
-                                            },
                                             "pystorcli2.Drive": {
                                                 "tf": 1
                                             },
                                             "pystorcli2.VirtualDrive": {
                                                 "tf": 1
                                             }
                                         },
-                                        "df": 3,
-                                        "s": {
-                                            "docs": {
-                                                "pystorcli2.Controller": {
-                                                    "tf": 1
-                                                },
-                                                "pystorcli2.Controller.patrolread_pause": {
-                                                    "tf": 1
-                                                }
-                                            },
-                                            "df": 2
-                                        }
+                                        "df": 2
                                     }
                                 }
                             },
                             "s": {
                                 "docs": {},
                                 "df": 0,
                                 "s": {
@@ -15963,44 +15087,14 @@
                                                         }
                                                     }
                                                 }
                                             }
                                         }
                                     }
                                 },
-                                "g": {
-                                    "docs": {},
-                                    "df": 0,
-                                    "r": {
-                                        "docs": {},
-                                        "df": 0,
-                                        "e": {
-                                            "docs": {},
-                                            "df": 0,
-                                            "s": {
-                                                "docs": {},
-                                                "df": 0,
-                                                "s": {
-                                                    "docs": {
-                                                        "pystorcli2.Controller": {
-                                                            "tf": 1
-                                                        },
-                                                        "pystorcli2.VirtualDrive": {
-                                                            "tf": 1.4142135623730951
-                                                        },
-                                                        "pystorcli2.VirtualDrive.erase_progress": {
-                                                            "tf": 1.4142135623730951
-                                                        }
-                                                    },
-                                                    "df": 3
-                                                }
-                                            }
-                                        }
-                                    }
-                                },
                                 "c": {
                                     "docs": {},
                                     "df": 0,
                                     "e": {
                                         "docs": {},
                                         "df": 0,
                                         "s": {
@@ -16028,14 +15122,41 @@
                                                     }
                                                 },
                                                 "df": 6
                                             }
                                         }
                                     }
                                 },
+                                "g": {
+                                    "docs": {},
+                                    "df": 0,
+                                    "r": {
+                                        "docs": {},
+                                        "df": 0,
+                                        "e": {
+                                            "docs": {},
+                                            "df": 0,
+                                            "s": {
+                                                "docs": {},
+                                                "df": 0,
+                                                "s": {
+                                                    "docs": {
+                                                        "pystorcli2.VirtualDrive": {
+                                                            "tf": 1.4142135623730951
+                                                        },
+                                                        "pystorcli2.VirtualDrive.erase_progress": {
+                                                            "tf": 1.4142135623730951
+                                                        }
+                                                    },
+                                                    "df": 2
+                                                }
+                                            }
+                                        }
+                                    }
+                                },
                                 "v": {
                                     "docs": {},
                                     "df": 0,
                                     "i": {
                                         "docs": {},
                                         "df": 0,
                                         "d": {
@@ -16319,25 +15440,22 @@
                                             },
                                             "df": 2
                                         }
                                     }
                                 },
                                 "e": {
                                     "docs": {
-                                        "pystorcli2.Controller.set_patrolread": {
-                                            "tf": 1
-                                        },
                                         "pystorcli2.Drive.erase_start": {
                                             "tf": 1
                                         },
                                         "pystorcli2.VirtualDrive.erase_start": {
                                             "tf": 1
                                         }
                                     },
-                                    "df": 3,
+                                    "df": 2,
                                     "l": {
                                         "docs": {
                                             "pystorcli2.Drive": {
                                                 "tf": 1.4142135623730951
                                             },
                                             "pystorcli2.Drive.model": {
                                                 "tf": 1
@@ -16401,15 +15519,15 @@
                                             "df": 0,
                                             "s": {
                                                 "docs": {
                                                     "pystorcli2.StorCLI": {
                                                         "tf": 1
                                                     },
                                                     "pystorcli2.Controller": {
-                                                        "tf": 1.4142135623730951
+                                                        "tf": 1
                                                     },
                                                     "pystorcli2.Controllers": {
                                                         "tf": 1
                                                     },
                                                     "pystorcli2.Enclosures": {
                                                         "tf": 1
                                                     },
@@ -16488,14 +15606,58 @@
                                             },
                                             "df": 1
                                         }
                                     }
                                 }
                             }
                         },
+                        "a": {
+                            "docs": {},
+                            "df": 0,
+                            "n": {
+                                "docs": {},
+                                "df": 0,
+                                "a": {
+                                    "docs": {},
+                                    "df": 0,
+                                    "g": {
+                                        "docs": {},
+                                        "df": 0,
+                                        "e": {
+                                            "docs": {},
+                                            "df": 0,
+                                            "d": {
+                                                "docs": {
+                                                    "pystorcli2.Controller.create_vd": {
+                                                        "tf": 1
+                                                    }
+                                                },
+                                                "df": 1
+                                            }
+                                        }
+                                    }
+                                }
+                            },
+                            "k": {
+                                "docs": {},
+                                "df": 0,
+                                "e": {
+                                    "docs": {},
+                                    "df": 0,
+                                    "s": {
+                                        "docs": {
+                                            "pystorcli2.VirtualDrive.delete": {
+                                                "tf": 1
+                                            }
+                                        },
+                                        "df": 1
+                                    }
+                                }
+                            }
+                        },
                         "i": {
                             "docs": {},
                             "df": 0,
                             "s": {
                                 "docs": {},
                                 "df": 0,
                                 "s": {
@@ -16505,25 +15667,22 @@
                                         "docs": {},
                                         "df": 0,
                                         "n": {
                                             "docs": {},
                                             "df": 0,
                                             "g": {
                                                 "docs": {
-                                                    "pystorcli2.Controller": {
-                                                        "tf": 1
-                                                    },
                                                     "pystorcli2.Drive": {
                                                         "tf": 1
                                                     },
                                                     "pystorcli2.VirtualDrive": {
                                                         "tf": 1
                                                     }
                                                 },
-                                                "df": 3
+                                                "df": 2
                                             }
                                         }
                                     }
                                 }
                             },
                             "g": {
                                 "docs": {},
@@ -16604,74 +15763,14 @@
                                                 }
                                             }
                                         }
                                     }
                                 }
                             }
                         },
-                        "a": {
-                            "docs": {},
-                            "df": 0,
-                            "n": {
-                                "docs": {},
-                                "df": 0,
-                                "a": {
-                                    "docs": {},
-                                    "df": 0,
-                                    "g": {
-                                        "docs": {},
-                                        "df": 0,
-                                        "e": {
-                                            "docs": {},
-                                            "df": 0,
-                                            "d": {
-                                                "docs": {
-                                                    "pystorcli2.Controller.create_vd": {
-                                                        "tf": 1
-                                                    }
-                                                },
-                                                "df": 1
-                                            }
-                                        }
-                                    }
-                                },
-                                "u": {
-                                    "docs": {},
-                                    "df": 0,
-                                    "a": {
-                                        "docs": {},
-                                        "df": 0,
-                                        "l": {
-                                            "docs": {
-                                                "pystorcli2.Controller.set_patrolread": {
-                                                    "tf": 1
-                                                }
-                                            },
-                                            "df": 1
-                                        }
-                                    }
-                                }
-                            },
-                            "k": {
-                                "docs": {},
-                                "df": 0,
-                                "e": {
-                                    "docs": {},
-                                    "df": 0,
-                                    "s": {
-                                        "docs": {
-                                            "pystorcli2.VirtualDrive.delete": {
-                                                "tf": 1
-                                            }
-                                        },
-                                        "df": 1
-                                    }
-                                }
-                            }
-                        },
                         "u": {
                             "docs": {},
                             "df": 0,
                             "s": {
                                 "docs": {},
                                 "df": 0,
                                 "t": {
@@ -16995,26 +16094,14 @@
                         },
                         "a": {
                             "docs": {},
                             "df": 0,
                             "l": {
                                 "docs": {},
                                 "df": 0,
-                                "u": {
-                                    "docs": {},
-                                    "df": 0,
-                                    "e": {
-                                        "docs": {
-                                            "pystorcli2.Controller.set_patrolread": {
-                                                "tf": 1
-                                            }
-                                        },
-                                        "df": 1
-                                    }
-                                },
                                 "i": {
                                     "docs": {},
                                     "df": 0,
                                     "d": {
                                         "docs": {
                                             "pystorcli2.VirtualDrive.delete": {
                                                 "tf": 1.4142135623730951
@@ -17166,15 +16253,15 @@
                                                     "df": 1,
                                                     "e": {
                                                         "docs": {},
                                                         "df": 0,
                                                         "r": {
                                                             "docs": {
                                                                 "pystorcli2.Controller": {
-                                                                    "tf": 3.7416573867739413
+                                                                    "tf": 3
                                                                 },
                                                                 "pystorcli2.Controller.__init__": {
                                                                     "tf": 1.4142135623730951
                                                                 },
                                                                 "pystorcli2.Controller.id": {
                                                                     "tf": 1
                                                                 },
@@ -17189,29 +16276,14 @@
                                                                 },
                                                                 "pystorcli2.Controller.encls": {
                                                                     "tf": 1
                                                                 },
                                                                 "pystorcli2.Controller.create_vd": {
                                                                     "tf": 1
                                                                 },
-                                                                "pystorcli2.Controller.patrolread_start": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.patrolread_stop": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.patrolread_pause": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.patrolread_resume": {
-                                                                    "tf": 1
-                                                                },
-                                                                "pystorcli2.Controller.patrolread_running": {
-                                                                    "tf": 1
-                                                                },
                                                                 "pystorcli2.Controllers": {
                                                                     "tf": 1
                                                                 },
                                                                 "pystorcli2.Controllers.get_ctl": {
                                                                     "tf": 2
                                                                 },
                                                                 "pystorcli2.Enclosure": {
@@ -17283,15 +16355,15 @@
                                                                 "pystorcli2.VirtualDrives.ctl_id": {
                                                                     "tf": 1
                                                                 },
                                                                 "pystorcli2.VirtualDrives.ctl": {
                                                                     "tf": 1.4142135623730951
                                                                 }
                                                             },
-                                                            "df": 39,
+                                                            "df": 34,
                                                             "s": {
                                                                 "docs": {
                                                                     "pystorcli2.StorCLI.controllers": {
                                                                         "tf": 1
                                                                     },
                                                                     "pystorcli2.Controller.vds": {
                                                                         "tf": 1
@@ -17386,53 +16458,17 @@
                                             "df": 0,
                                             "u": {
                                                 "docs": {},
                                                 "df": 0,
                                                 "r": {
                                                     "docs": {},
                                                     "df": 0,
-                                                    "a": {
+                                                    "e": {
                                                         "docs": {},
                                                         "df": 0,
-                                                        "t": {
-                                                            "docs": {},
-                                                            "df": 0,
-                                                            "i": {
-                                                                "docs": {},
-                                                                "df": 0,
-                                                                "o": {
-                                                                    "docs": {},
-                                                                    "df": 0,
-                                                                    "n": {
-                                                                        "docs": {
-                                                                            "pystorcli2.Controller": {
-                                                                                "tf": 1
-                                                                            }
-                                                                        },
-                                                                        "df": 1
-                                                                    }
-                                                                }
-                                                            }
-                                                        }
-                                                    },
-                                                    "e": {
-                                                        "docs": {
-                                                            "pystorcli2.Controller.set_patrolread": {
-                                                                "tf": 1.4142135623730951
-                                                            }
-                                                        },
-                                                        "df": 1,
-                                                        "s": {
-                                                            "docs": {
-                                                                "pystorcli2.Controller": {
-                                                                    "tf": 1
-                                                                }
-                                                            },
-                                                            "df": 1
-                                                        },
                                                         "d": {
                                                             "docs": {
                                                                 "pystorcli2.DriveState.is_configured": {
                                                                     "tf": 1
                                                                 }
                                                             },
                                                             "df": 1
@@ -17781,20 +16817,14 @@
                                             },
                                             "pystorcli2.StorCLI.run": {
                                                 "tf": 1
                                             },
                                             "pystorcli2.StorCLI.is_singleton": {
                                                 "tf": 1
                                             },
-                                            "pystorcli2.Controller": {
-                                                "tf": 1
-                                            },
-                                            "pystorcli2.Controller.patrolread_running": {
-                                                "tf": 1
-                                            },
                                             "pystorcli2.DriveState.is_good": {
                                                 "tf": 1
                                             },
                                             "pystorcli2.DriveState.is_configured": {
                                                 "tf": 1
                                             },
                                             "pystorcli2.DriveState.is_settable": {
@@ -17818,15 +16848,15 @@
                                             "pystorcli2.VirtualDrive.erase_running": {
                                                 "tf": 1
                                             },
                                             "pystorcli2.VirtualDrive.migrate_running": {
                                                 "tf": 1
                                             }
                                         },
-                                        "df": 16
+                                        "df": 14
                                     }
                                 }
                             },
                             "a": {
                                 "docs": {},
                                 "df": 0,
                                 "r": {
@@ -17975,26 +17005,14 @@
                                     },
                                     "pystorcli2.Controller": {
                                         "tf": 1
                                     },
                                     "pystorcli2.Controller.name": {
                                         "tf": 1
                                     },
-                                    "pystorcli2.Controller.patrolread_start": {
-                                        "tf": 1
-                                    },
-                                    "pystorcli2.Controller.patrolread_stop": {
-                                        "tf": 1
-                                    },
-                                    "pystorcli2.Controller.patrolread_pause": {
-                                        "tf": 1
-                                    },
-                                    "pystorcli2.Controller.patrolread_resume": {
-                                        "tf": 1
-                                    },
                                     "pystorcli2.Enclosure": {
                                         "tf": 1
                                     },
                                     "pystorcli2.Enclosure.name": {
                                         "tf": 1
                                     },
                                     "pystorcli2.Drive": {
@@ -18036,15 +17054,15 @@
                                     "pystorcli2.VirtualDrive.delete": {
                                         "tf": 1
                                     },
                                     "pystorcli2.VirtualDrive.migrate_start": {
                                         "tf": 1
                                     }
                                 },
-                                "df": 24
+                                "df": 20
                             }
                         },
                         "t": {
                             "docs": {},
                             "df": 0,
                             "l": {
                                 "docs": {
@@ -18110,31 +17128,28 @@
                                         "docs": {},
                                         "df": 0,
                                         "n": {
                                             "docs": {},
                                             "df": 0,
                                             "t": {
                                                 "docs": {
-                                                    "pystorcli2.Controller": {
-                                                        "tf": 1.4142135623730951
-                                                    },
                                                     "pystorcli2.Controller.create_vd": {
                                                         "tf": 1
                                                     },
                                                     "pystorcli2.Drives.get_drive_range_ids": {
                                                         "tf": 1
                                                     },
                                                     "pystorcli2.Drives.get_drive_range": {
                                                         "tf": 1
                                                     },
                                                     "pystorcli2.VirtualDrive": {
                                                         "tf": 1
                                                     }
                                                 },
-                                                "df": 5
+                                                "df": 4
                                             }
                                         }
                                     }
                                 }
                             }
                         },
                         "c": {
@@ -18366,28 +17381,19 @@
                                                 "docs": {
                                                     "pystorcli2.StorCLI": {
                                                         "tf": 1.4142135623730951
                                                     },
                                                     "pystorcli2.StorCLI.__init__": {
                                                         "tf": 1
                                                     },
-                                                    "pystorcli2.Controller.autorebuild": {
-                                                        "tf": 1
-                                                    },
-                                                    "pystorcli2.Controller.foreignautoimport": {
-                                                        "tf": 1
-                                                    },
-                                                    "pystorcli2.Controller.patrolread": {
-                                                        "tf": 1
-                                                    },
                                                     "pystorcli2.VirtualDrive.autobgi": {
                                                         "tf": 1
                                                     }
                                                 },
-                                                "df": 6
+                                                "df": 3
                                             }
                                         }
                                     }
                                 }
                             },
                             "i": {
                                 "docs": {},
@@ -18938,20 +17944,14 @@
                                 },
                                 "pystorcli2.StorCLI.set_cmdrunner": {
                                     "tf": 1
                                 },
                                 "pystorcli2.StorCLI.is_singleton": {
                                     "tf": 1
                                 },
-                                "pystorcli2.Controller": {
-                                    "tf": 1
-                                },
-                                "pystorcli2.Controller.patrolread_running": {
-                                    "tf": 1
-                                },
                                 "pystorcli2.Controllers": {
                                     "tf": 1
                                 },
                                 "pystorcli2.Enclosures": {
                                     "tf": 1
                                 },
                                 "pystorcli2.DriveState.is_good": {
@@ -18996,15 +17996,15 @@
                                 "pystorcli2.VirtualDrive.migrate_running": {
                                     "tf": 1
                                 },
                                 "pystorcli2.VirtualDrives": {
                                     "tf": 1
                                 }
                             },
-                            "df": 22,
+                            "df": 20,
                             "e": {
                                 "docs": {
                                     "pystorcli2.Drive.erase_start": {
                                         "tf": 1
                                     }
                                 },
                                 "df": 1
@@ -19032,64 +18032,35 @@
                                                     "docs": {},
                                                     "df": 0,
                                                     "t": {
                                                         "docs": {
                                                             "pystorcli2.StorCLI": {
                                                                 "tf": 1
                                                             },
-                                                            "pystorcli2.Controller": {
-                                                                "tf": 1
-                                                            },
                                                             "pystorcli2.Drive": {
                                                                 "tf": 1
                                                             },
                                                             "pystorcli2.VirtualDrive": {
                                                                 "tf": 1
                                                             }
                                                         },
-                                                        "df": 4
+                                                        "df": 3
                                                     }
                                                 }
                                             }
                                         }
                                     }
-                                },
-                                "o": {
-                                    "docs": {},
-                                    "df": 0,
-                                    "r": {
-                                        "docs": {},
-                                        "df": 0,
-                                        "t": {
-                                            "docs": {},
-                                            "df": 0,
-                                            "s": {
-                                                "docs": {
-                                                    "pystorcli2.Controller": {
-                                                        "tf": 1
-                                                    }
-                                                },
-                                                "df": 1
-                                            }
-                                        }
-                                    }
                                 }
                             }
                         },
                         "f": {
                             "docs": {
                                 "pystorcli2.StorCLI.is_singleton": {
                                     "tf": 1
                                 },
-                                "pystorcli2.Controller": {
-                                    "tf": 1.4142135623730951
-                                },
-                                "pystorcli2.Controller.patrolread_running": {
-                                    "tf": 1
-                                },
                                 "pystorcli2.Enclosure": {
                                     "tf": 1
                                 },
                                 "pystorcli2.Enclosure.has_drives": {
                                     "tf": 1
                                 },
                                 "pystorcli2.DriveState.is_good": {
@@ -19143,15 +18114,15 @@
                                 "pystorcli2.VirtualDrives": {
                                     "tf": 1.4142135623730951
                                 },
                                 "pystorcli2.VirtualDrives.has_vds": {
                                     "tf": 1
                                 }
                             },
-                            "df": 23
+                            "df": 21
                         },
                         "d": {
                             "docs": {
                                 "pystorcli2.Controller": {
                                     "tf": 2
                                 },
                                 "pystorcli2.Controller.__init__": {
@@ -19434,26 +18405,14 @@
                                 },
                                 "pystorcli2.Controller": {
                                     "tf": 1.4142135623730951
                                 },
                                 "pystorcli2.Controller.drives_ids": {
                                     "tf": 1.4142135623730951
                                 },
-                                "pystorcli2.Controller.patrolread_start": {
-                                    "tf": 1
-                                },
-                                "pystorcli2.Controller.patrolread_stop": {
-                                    "tf": 1
-                                },
-                                "pystorcli2.Controller.patrolread_pause": {
-                                    "tf": 1
-                                },
-                                "pystorcli2.Controller.patrolread_resume": {
-                                    "tf": 1
-                                },
                                 "pystorcli2.Controllers": {
                                     "tf": 1.7320508075688772
                                 },
                                 "pystorcli2.Controllers.ids": {
                                     "tf": 1
                                 },
                                 "pystorcli2.Enclosure": {
@@ -19531,28 +18490,25 @@
                                 "pystorcli2.VirtualDrives": {
                                     "tf": 1.7320508075688772
                                 },
                                 "pystorcli2.VirtualDrives.ids": {
                                     "tf": 1.4142135623730951
                                 }
                             },
-                            "df": 38,
+                            "df": 34,
                             "f": {
                                 "docs": {
-                                    "pystorcli2.Controller.set_patrolread": {
-                                        "tf": 1
-                                    },
                                     "pystorcli2.VirtualDrive.bootdrive": {
                                         "tf": 1.4142135623730951
                                     },
                                     "pystorcli2.VirtualDrive.pdcache": {
                                         "tf": 1.4142135623730951
                                     }
                                 },
-                                "df": 3,
+                                "df": 2,
                                 "l": {
                                     "docs": {},
                                     "df": 0,
                                     "i": {
                                         "docs": {},
                                         "df": 0,
                                         "n": {
@@ -20114,23 +19070,14 @@
                             }
                         },
                         "n": {
                             "docs": {
                                 "pystorcli2.StorCLI.enable_singleton": {
                                     "tf": 1
                                 },
-                                "pystorcli2.Controller": {
-                                    "tf": 2.23606797749979
-                                },
-                                "pystorcli2.Controller.set_patrolread": {
-                                    "tf": 1
-                                },
-                                "pystorcli2.Controller.patrolread_running": {
-                                    "tf": 1
-                                },
                                 "pystorcli2.Drive": {
                                     "tf": 2.23606797749979
                                 },
                                 "pystorcli2.Drive.init_stop": {
                                     "tf": 1
                                 },
                                 "pystorcli2.Drive.init_running": {
@@ -20157,15 +19104,15 @@
                                 "pystorcli2.VirtualDrive.migrate_start": {
                                     "tf": 1
                                 },
                                 "pystorcli2.VirtualDrive.migrate_running": {
                                     "tf": 1
                                 }
                             },
-                            "df": 15,
+                            "df": 12,
                             "l": {
                                 "docs": {},
                                 "df": 0,
                                 "y": {
                                     "docs": {
                                         "pystorcli2.StorCLI.set_cmdrunner": {
                                             "tf": 1
@@ -20353,34 +19300,22 @@
                                                 "docs": {},
                                                 "df": 0,
                                                 "o": {
                                                     "docs": {},
                                                     "df": 0,
                                                     "n": {
                                                         "docs": {
-                                                            "pystorcli2.Controller.patrolread_start": {
-                                                                "tf": 1
-                                                            },
-                                                            "pystorcli2.Controller.patrolread_stop": {
-                                                                "tf": 1
-                                                            },
-                                                            "pystorcli2.Controller.patrolread_pause": {
-                                                                "tf": 1
-                                                            },
-                                                            "pystorcli2.Controller.patrolread_resume": {
-                                                                "tf": 1
-                                                            },
                                                             "pystorcli2.Drive.erase_stop": {
                                                                 "tf": 1
                                                             },
                                                             "pystorcli2.VirtualDrive.erase_stop": {
                                                                 "tf": 1
                                                             }
                                                         },
-                                                        "df": 6
+                                                        "df": 2
                                                     }
                                                 }
                                             }
                                         }
                                     }
                                 }
                             }
@@ -20548,29 +19483,14 @@
                                     },
                                     "pystorcli2.Controller": {
                                         "tf": 1
                                     },
                                     "pystorcli2.Controller.__init__": {
                                         "tf": 1
                                     },
-                                    "pystorcli2.Controller.patrolread_start": {
-                                        "tf": 1.4142135623730951
-                                    },
-                                    "pystorcli2.Controller.patrolread_stop": {
-                                        "tf": 1.4142135623730951
-                                    },
-                                    "pystorcli2.Controller.patrolread_pause": {
-                                        "tf": 1.4142135623730951
-                                    },
-                                    "pystorcli2.Controller.patrolread_resume": {
-                                        "tf": 1.4142135623730951
-                                    },
-                                    "pystorcli2.Controller.patrolread_running": {
-                                        "tf": 1
-                                    },
                                     "pystorcli2.Controllers": {
                                         "tf": 1
                                     },
                                     "pystorcli2.Controllers.__init__": {
                                         "tf": 1
                                     },
                                     "pystorcli2.Enclosure": {
@@ -20672,15 +19592,15 @@
                                     "pystorcli2.VirtualDrives": {
                                         "tf": 1
                                     },
                                     "pystorcli2.VirtualDrives.__init__": {
                                         "tf": 1
                                     }
                                 },
-                                "df": 45,
+                                "df": 40,
                                 "i": {
                                     "docs": {},
                                     "df": 0,
                                     "r": {
                                         "docs": {
                                             "pystorcli2.StorCLI.enable_singleton": {
                                                 "tf": 1
@@ -20864,17 +19784,14 @@
                                 },
                                 "pystorcli2.Controller": {
                                     "tf": 1
                                 },
                                 "pystorcli2.Controller.__init__": {
                                     "tf": 1
                                 },
-                                "pystorcli2.Controller.set_patrolread": {
-                                    "tf": 1.4142135623730951
-                                },
                                 "pystorcli2.Controllers": {
                                     "tf": 1
                                 },
                                 "pystorcli2.Controllers.__init__": {
                                     "tf": 1
                                 },
                                 "pystorcli2.Enclosure": {
@@ -20940,34 +19857,31 @@
                                 "pystorcli2.VirtualDrives": {
                                     "tf": 1
                                 },
                                 "pystorcli2.VirtualDrives.__init__": {
                                     "tf": 1
                                 }
                             },
-                            "df": 31,
+                            "df": 30,
                             "d": {
                                 "docs": {},
                                 "df": 0,
                                 "o": {
                                     "docs": {
                                         "pystorcli2.StorCLI": {
                                             "tf": 1
                                         },
-                                        "pystorcli2.Controller": {
-                                            "tf": 1
-                                        },
                                         "pystorcli2.Drive": {
                                             "tf": 1
                                         },
                                         "pystorcli2.VirtualDrive": {
                                             "tf": 1
                                         }
                                     },
-                                    "df": 4
+                                    "df": 3
                                 }
                             }
                         },
                         "t": {
                             "docs": {},
                             "df": 0,
                             "l": {
@@ -21011,17 +19925,14 @@
                             "docs": {},
                             "df": 0,
                             "u": {
                                 "docs": {},
                                 "df": 0,
                                 "e": {
                                     "docs": {
-                                        "pystorcli2.Controller.patrolread_running": {
-                                            "tf": 1
-                                        },
                                         "pystorcli2.Enclosure": {
                                             "tf": 1
                                         },
                                         "pystorcli2.Enclosure.has_drives": {
                                             "tf": 1
                                         },
                                         "pystorcli2.Drive.init_running": {
@@ -21042,15 +19953,15 @@
                                         "pystorcli2.VirtualDrives": {
                                             "tf": 1.4142135623730951
                                         },
                                         "pystorcli2.VirtualDrives.has_vds": {
                                             "tf": 1
                                         }
                                     },
-                                    "df": 10,
+                                    "df": 9,
                                     "/": {
                                         "docs": {},
                                         "df": 0,
                                         "f": {
                                             "docs": {},
                                             "df": 0,
                                             "a": {
@@ -21103,17 +20014,14 @@
                         }
                     },
                     "a": {
                         "docs": {
                             "pystorcli2.StorCLI.version": {
                                 "tf": 1
                             },
-                            "pystorcli2.Controller": {
-                                "tf": 1
-                            },
                             "pystorcli2.Drive": {
                                 "tf": 2.23606797749979
                             },
                             "pystorcli2.Drive.init_start": {
                                 "tf": 1
                             },
                             "pystorcli2.Drive.init_stop": {
@@ -21158,15 +20066,15 @@
                             "pystorcli2.VirtualDrive.delete": {
                                 "tf": 2.23606797749979
                             },
                             "pystorcli2.VirtualDrive.migrate_running": {
                                 "tf": 1
                             }
                         },
-                        "df": 19,
+                        "df": 18,
                         "r": {
                             "docs": {},
                             "df": 0,
                             "g": {
                                 "docs": {},
                                 "df": 0,
                                 "s": {
@@ -21191,17 +20099,14 @@
                                         },
                                         "pystorcli2.Controller.__init__": {
                                             "tf": 1
                                         },
                                         "pystorcli2.Controller.create_vd": {
                                             "tf": 1
                                         },
-                                        "pystorcli2.Controller.set_patrolread": {
-                                            "tf": 1
-                                        },
                                         "pystorcli2.Controllers": {
                                             "tf": 1
                                         },
                                         "pystorcli2.Controllers.__init__": {
                                             "tf": 1
                                         },
                                         "pystorcli2.Controllers.get_ctl": {
@@ -21276,15 +20181,15 @@
                                         "pystorcli2.VirtualDrives.get_vd": {
                                             "tf": 1
                                         },
                                         "pystorcli2.VirtualDrives.get_named_vd": {
                                             "tf": 1
                                         }
                                     },
-                                    "df": 36
+                                    "df": 35
                                 },
                                 "u": {
                                     "docs": {},
                                     "df": 0,
                                     "m": {
                                         "docs": {},
                                         "df": 0,
@@ -21336,28 +20241,25 @@
                                 "docs": {},
                                 "df": 0,
                                 "o": {
                                     "docs": {
                                         "pystorcli2.StorCLI": {
                                             "tf": 1
                                         },
-                                        "pystorcli2.Controller": {
-                                            "tf": 1.7320508075688772
-                                        },
                                         "pystorcli2.Drive": {
                                             "tf": 1.7320508075688772
                                         },
                                         "pystorcli2.VirtualDrive": {
                                             "tf": 2.6457513110645907
                                         },
                                         "pystorcli2.VirtualDrive.wrcache": {
                                             "tf": 1
                                         }
                                     },
-                                    "df": 5
+                                    "df": 4
                                 }
                             },
                             "l": {
                                 "docs": {
                                     "pystorcli2.StorCLI.enable_singleton": {
                                         "tf": 1.4142135623730951
                                     },
@@ -21366,22 +20268,19 @@
                                     }
                                 },
                                 "df": 2
                             }
                         },
                         "t": {
                             "docs": {
-                                "pystorcli2.Controller": {
-                                    "tf": 1
-                                },
                                 "pystorcli2.VirtualDrive.delete": {
                                     "tf": 1
                                 }
                             },
-                            "df": 2,
+                            "df": 1,
                             "o": {
                                 "docs": {},
                                 "df": 0,
                                 "m": {
                                     "docs": {},
                                     "df": 0,
                                     "i": {
@@ -21428,25 +20327,22 @@
                             },
                             "df": 7,
                             "d": {
                                 "docs": {
                                     "pystorcli2.StorCLI.run": {
                                         "tf": 1
                                     },
-                                    "pystorcli2.Controller": {
-                                        "tf": 1
-                                    },
                                     "pystorcli2.Drive.spin": {
                                         "tf": 1.4142135623730951
                                     },
                                     "pystorcli2.VirtualDrive.delete": {
                                         "tf": 1.4142135623730951
                                     }
                                 },
-                                "df": 4
+                                "df": 3
                             },
                             "y": {
                                 "docs": {
                                     "pystorcli2.Drive.vd_id": {
                                         "tf": 1
                                     },
                                     "pystorcli2.Drive.vd": {
@@ -21582,124 +20478,14 @@
                                                 }
                                             }
                                         }
                                     }
                                 }
                             }
                         },
-                        "u": {
-                            "docs": {},
-                            "df": 0,
-                            "t": {
-                                "docs": {},
-                                "df": 0,
-                                "o": {
-                                    "docs": {
-                                        "pystorcli2.Controller": {
-                                            "tf": 1
-                                        },
-                                        "pystorcli2.Controller.set_patrolread": {
-                                            "tf": 1
-                                        },
-                                        "pystorcli2.VirtualDrive": {
-                                            "tf": 1
-                                        }
-                                    },
-                                    "df": 3,
-                                    "r": {
-                                        "docs": {},
-                                        "df": 0,
-                                        "e": {
-                                            "docs": {},
-                                            "df": 0,
-                                            "b": {
-                                                "docs": {},
-                                                "df": 0,
-                                                "u": {
-                                                    "docs": {},
-                                                    "df": 0,
-                                                    "i": {
-                                                        "docs": {},
-                                                        "df": 0,
-                                                        "l": {
-                                                            "docs": {},
-                                                            "df": 0,
-                                                            "d": {
-                                                                "docs": {
-                                                                    "pystorcli2.Controller": {
-                                                                        "tf": 1
-                                                                    }
-                                                                },
-                                                                "df": 1
-                                                            }
-                                                        }
-                                                    }
-                                                }
-                                            }
-                                        }
-                                    },
-                                    "m": {
-                                        "docs": {},
-                                        "df": 0,
-                                        "a": {
-                                            "docs": {},
-                                            "df": 0,
-                                            "t": {
-                                                "docs": {},
-                                                "df": 0,
-                                                "i": {
-                                                    "docs": {},
-                                                    "df": 0,
-                                                    "c": {
-                                                        "docs": {},
-                                                        "df": 0,
-                                                        "a": {
-                                                            "docs": {},
-                                                            "df": 0,
-                                                            "l": {
-                                                                "docs": {},
-                                                                "df": 0,
-                                                                "l": {
-                                                                    "docs": {},
-                                                                    "df": 0,
-                                                                    "y": {
-                                                                        "docs": {
-                                                                            "pystorcli2.Controller": {
-                                                                                "tf": 1
-                                                                            }
-                                                                        },
-                                                                        "df": 1
-                                                                    }
-                                                                }
-                                                            }
-                                                        }
-                                                    }
-                                                }
-                                            }
-                                        }
-                                    },
-                                    "b": {
-                                        "docs": {},
-                                        "df": 0,
-                                        "g": {
-                                            "docs": {},
-                                            "df": 0,
-                                            "i": {
-                                                "docs": {
-                                                    "pystorcli2.VirtualDrive": {
-                                                        "tf": 1
-                                                    }
-                                                },
-                                                "df": 1
-                                            }
-                                        }
-                                    }
-                                }
-                            }
-                        },
                         "d": {
                             "docs": {},
                             "df": 0,
                             "d": {
                                 "docs": {
                                     "pystorcli2.Drive": {
                                         "tf": 1
@@ -21802,14 +20588,46 @@
                                                 }
                                             }
                                         }
                                     }
                                 }
                             }
                         },
+                        "u": {
+                            "docs": {},
+                            "df": 0,
+                            "t": {
+                                "docs": {},
+                                "df": 0,
+                                "o": {
+                                    "docs": {
+                                        "pystorcli2.VirtualDrive": {
+                                            "tf": 1
+                                        }
+                                    },
+                                    "df": 1,
+                                    "b": {
+                                        "docs": {},
+                                        "df": 0,
+                                        "g": {
+                                            "docs": {},
+                                            "df": 0,
+                                            "i": {
+                                                "docs": {
+                                                    "pystorcli2.VirtualDrive": {
+                                                        "tf": 1
+                                                    }
+                                                },
+                                                "df": 1
+                                            }
+                                        }
+                                    }
+                                }
+                            }
+                        },
                         "w": {
                             "docs": {},
                             "df": 0,
                             "b": {
                                 "docs": {
                                     "pystorcli2.VirtualDrive.wrcache": {
                                         "tf": 1.4142135623730951
@@ -21944,20 +20762,14 @@
                                 "docs": {},
                                 "df": 0,
                                 "l": {
                                     "docs": {
                                         "pystorcli2.StorCLI.cache_enable": {
                                             "tf": 1
                                         },
-                                        "pystorcli2.Controller": {
-                                            "tf": 1
-                                        },
-                                        "pystorcli2.Controller.patrolread_running": {
-                                            "tf": 1
-                                        },
                                         "pystorcli2.Enclosure": {
                                             "tf": 1
                                         },
                                         "pystorcli2.Enclosure.has_drives": {
                                             "tf": 1
                                         },
                                         "pystorcli2.Drive": {
@@ -21996,15 +20808,15 @@
                                         "pystorcli2.VirtualDrives": {
                                             "tf": 1.4142135623730951
                                         },
                                         "pystorcli2.VirtualDrives.has_vds": {
                                             "tf": 1
                                         }
                                     },
-                                    "df": 18,
+                                    "df": 16,
                                     "e": {
                                         "docs": {},
                                         "df": 0,
                                         "a": {
                                             "docs": {},
                                             "df": 0,
                                             "n": {
@@ -22016,22 +20828,19 @@
                                                 "df": 1
                                             }
                                         }
                                     }
                                 },
                                 "t": {
                                     "docs": {
-                                        "pystorcli2.Controller": {
-                                            "tf": 1
-                                        },
                                         "pystorcli2.VirtualDrive.bootdrive": {
                                             "tf": 1.7320508075688772
                                         }
                                     },
-                                    "df": 2,
+                                    "df": 1,
                                     "d": {
                                         "docs": {},
                                         "df": 0,
                                         "r": {
                                             "docs": {},
                                             "df": 0,
                                             "i": {
@@ -22338,28 +21147,19 @@
                                 }
                             },
                             "n": {
                                 "docs": {},
                                 "df": 0,
                                 "c": {
                                     "docs": {
-                                        "pystorcli2.Controller.autorebuild": {
-                                            "tf": 1
-                                        },
-                                        "pystorcli2.Controller.foreignautoimport": {
-                                            "tf": 1
-                                        },
-                                        "pystorcli2.Controller.patrolread": {
-                                            "tf": 1
-                                        },
                                         "pystorcli2.VirtualDrive.autobgi": {
                                             "tf": 1
                                         }
                                     },
-                                    "df": 4
+                                    "df": 1
                                 }
                             }
                         },
                         "r": {
                             "docs": {},
                             "df": 0,
                             "o": {
@@ -22426,78 +21226,14 @@
                                         "tf": 1
                                     },
                                     "pystorcli2.VirtualDrive.erase_start": {
                                         "tf": 1
                                     }
                                 },
                                 "df": 10,
-                                "e": {
-                                    "docs": {},
-                                    "df": 0,
-                                    "i": {
-                                        "docs": {},
-                                        "df": 0,
-                                        "g": {
-                                            "docs": {},
-                                            "df": 0,
-                                            "n": {
-                                                "docs": {
-                                                    "pystorcli2.Controller": {
-                                                        "tf": 1
-                                                    }
-                                                },
-                                                "df": 1,
-                                                "a": {
-                                                    "docs": {},
-                                                    "df": 0,
-                                                    "u": {
-                                                        "docs": {},
-                                                        "df": 0,
-                                                        "t": {
-                                                            "docs": {},
-                                                            "df": 0,
-                                                            "o": {
-                                                                "docs": {},
-                                                                "df": 0,
-                                                                "i": {
-                                                                    "docs": {},
-                                                                    "df": 0,
-                                                                    "m": {
-                                                                        "docs": {},
-                                                                        "df": 0,
-                                                                        "p": {
-                                                                            "docs": {},
-                                                                            "df": 0,
-                                                                            "o": {
-                                                                                "docs": {},
-                                                                                "df": 0,
-                                                                                "r": {
-                                                                                    "docs": {},
-                                                                                    "df": 0,
-                                                                                    "t": {
-                                                                                        "docs": {
-                                                                                            "pystorcli2.Controller": {
-                                                                                                "tf": 1
-                                                                                            }
-                                                                                        },
-                                                                                        "df": 1
-                                                                                    }
-                                                                                }
-                                                                            }
-                                                                        }
-                                                                    }
-                                                                }
-                                                            }
-                                                        }
-                                                    }
-                                                }
-                                            }
-                                        }
-                                    }
-                                },
                                 "m": {
                                     "docs": {},
                                     "df": 0,
                                     "a": {
                                         "docs": {},
                                         "df": 0,
                                         "t": {
@@ -22638,17 +21374,14 @@
                                 "docs": {},
                                 "df": 0,
                                 "s": {
                                     "docs": {},
                                     "df": 0,
                                     "e": {
                                         "docs": {
-                                            "pystorcli2.Controller.patrolread_running": {
-                                                "tf": 1
-                                            },
                                             "pystorcli2.Drive.init_running": {
                                                 "tf": 1
                                             },
                                             "pystorcli2.Drive.erase_running": {
                                                 "tf": 1
                                             },
                                             "pystorcli2.VirtualDrive.init_running": {
@@ -22657,15 +21390,15 @@
                                             "pystorcli2.VirtualDrive.erase_running": {
                                                 "tf": 1
                                             },
                                             "pystorcli2.VirtualDrive.migrate_running": {
                                                 "tf": 1
                                             }
                                         },
-                                        "df": 6
+                                        "df": 5
                                     }
                                 }
                             },
                             "s": {
                                 "docs": {},
                                 "df": 0,
                                 "t": {
@@ -23322,14 +22055,33 @@
                                                 }
                                             }
                                         }
                                     }
                                 }
                             }
                         },
+                        "v": {
+                            "docs": {},
+                            "df": 0,
+                            "e": {
+                                "docs": {},
+                                "df": 0,
+                                "n": {
+                                    "docs": {
+                                        "pystorcli2.VirtualDrive.wrcache": {
+                                            "tf": 1
+                                        },
+                                        "pystorcli2.VirtualDrive.migrate_start": {
+                                            "tf": 1
+                                        }
+                                    },
+                                    "df": 2
+                                }
+                            }
+                        },
                         "f": {
                             "docs": {},
                             "df": 0,
                             "f": {
                                 "docs": {},
                                 "df": 0,
                                 "e": {
@@ -23345,54 +22097,26 @@
                                                 "docs": {},
                                                 "df": 0,
                                                 "v": {
                                                     "docs": {},
                                                     "df": 0,
                                                     "e": {
                                                         "docs": {
-                                                            "pystorcli2.Controller.autorebuild": {
-                                                                "tf": 1
-                                                            },
-                                                            "pystorcli2.Controller.foreignautoimport": {
-                                                                "tf": 1
-                                                            },
-                                                            "pystorcli2.Controller.patrolread": {
-                                                                "tf": 1
-                                                            },
                                                             "pystorcli2.VirtualDrive.autobgi": {
                                                                 "tf": 1
                                                             }
                                                         },
-                                                        "df": 4
+                                                        "df": 1
                                                     }
                                                 }
                                             }
                                         }
                                     }
                                 }
                             }
-                        },
-                        "v": {
-                            "docs": {},
-                            "df": 0,
-                            "e": {
-                                "docs": {},
-                                "df": 0,
-                                "n": {
-                                    "docs": {
-                                        "pystorcli2.VirtualDrive.wrcache": {
-                                            "tf": 1
-                                        },
-                                        "pystorcli2.VirtualDrive.migrate_start": {
-                                            "tf": 1
-                                        }
-                                    },
-                                    "df": 2
-                                }
-                            }
                         }
                     },
                     "d": {
                         "docs": {},
                         "df": 0,
                         "i": {
                             "docs": {},
@@ -23457,29 +22181,17 @@
                                         "pystorcli2.StorCLI.check_response_status": {
                                             "tf": 1
                                         },
                                         "pystorcli2.StorCLI.run": {
                                             "tf": 1
                                         },
                                         "pystorcli2.Controller": {
-                                            "tf": 3
-                                        },
-                                        "pystorcli2.Controller.facts": {
-                                            "tf": 1
-                                        },
-                                        "pystorcli2.Controller.patrolread_start": {
-                                            "tf": 1
-                                        },
-                                        "pystorcli2.Controller.patrolread_stop": {
                                             "tf": 1
                                         },
-                                        "pystorcli2.Controller.patrolread_pause": {
-                                            "tf": 1
-                                        },
-                                        "pystorcli2.Controller.patrolread_resume": {
+                                        "pystorcli2.Controller.facts": {
                                             "tf": 1
                                         },
                                         "pystorcli2.Enclosure": {
                                             "tf": 1
                                         },
                                         "pystorcli2.Enclosure.facts": {
                                             "tf": 1
@@ -23532,15 +22244,15 @@
                                         "pystorcli2.VirtualDrive.delete": {
                                             "tf": 1
                                         },
                                         "pystorcli2.VirtualDrive.migrate_start": {
                                             "tf": 1
                                         }
                                     },
-                                    "df": 29
+                                    "df": 25
                                 }
                             },
                             "r": {
                                 "docs": {},
                                 "df": 0,
                                 "e": {
                                     "docs": {},
@@ -23629,26 +22341,14 @@
                                     "docs": {
                                         "pystorcli2.StorCLI": {
                                             "tf": 1
                                         },
                                         "pystorcli2.StorCLI.run": {
                                             "tf": 1
                                         },
-                                        "pystorcli2.Controller.patrolread_start": {
-                                            "tf": 1
-                                        },
-                                        "pystorcli2.Controller.patrolread_stop": {
-                                            "tf": 1
-                                        },
-                                        "pystorcli2.Controller.patrolread_pause": {
-                                            "tf": 1
-                                        },
-                                        "pystorcli2.Controller.patrolread_resume": {
-                                            "tf": 1
-                                        },
                                         "pystorcli2.Drive.init_start": {
                                             "tf": 1
                                         },
                                         "pystorcli2.Drive.init_stop": {
                                             "tf": 1
                                         },
                                         "pystorcli2.Drive.erase_start": {
@@ -23678,15 +22378,15 @@
                                         "pystorcli2.VirtualDrive.delete": {
                                             "tf": 1.7320508075688772
                                         },
                                         "pystorcli2.VirtualDrive.migrate_start": {
                                             "tf": 1
                                         }
                                     },
-                                    "df": 18
+                                    "df": 14
                                 }
                             }
                         },
                         "r": {
                             "docs": {},
                             "df": 0,
                             "i": {
@@ -24291,64 +22991,38 @@
                                             "s": {
                                                 "docs": {},
                                                 "df": 0,
                                                 "e": {
                                                     "docs": {
                                                         "pystorcli2.StorCLI": {
                                                             "tf": 1
-                                                        },
-                                                        "pystorcli2.Controller.patrolread_start": {
-                                                            "tf": 1
-                                                        },
-                                                        "pystorcli2.Controller.patrolread_stop": {
-                                                            "tf": 1
-                                                        },
-                                                        "pystorcli2.Controller.patrolread_pause": {
-                                                            "tf": 1
-                                                        },
-                                                        "pystorcli2.Controller.patrolread_resume": {
-                                                            "tf": 1
                                                         }
                                                     },
-                                                    "df": 5
+                                                    "df": 1
                                                 }
                                             }
                                         }
                                     }
                                 },
                                 "u": {
                                     "docs": {},
                                     "df": 0,
                                     "m": {
                                         "docs": {},
                                         "df": 0,
                                         "e": {
                                             "docs": {
-                                                "pystorcli2.Controller": {
-                                                    "tf": 1
-                                                },
                                                 "pystorcli2.Drive": {
                                                     "tf": 1
                                                 },
                                                 "pystorcli2.VirtualDrive": {
                                                     "tf": 1
                                                 }
                                             },
-                                            "df": 3,
-                                            "s": {
-                                                "docs": {
-                                                    "pystorcli2.Controller": {
-                                                        "tf": 1
-                                                    },
-                                                    "pystorcli2.Controller.patrolread_resume": {
-                                                        "tf": 1
-                                                    }
-                                                },
-                                                "df": 2
-                                            },
+                                            "df": 2,
                                             "d": {
                                                 "docs": {
                                                     "pystorcli2.Drive.init_stop": {
                                                         "tf": 1
                                                     },
                                                     "pystorcli2.VirtualDrive.init_stop": {
                                                         "tf": 1
@@ -24442,29 +23116,14 @@
                                                     },
                                                     "pystorcli2.StorCLI.full_version": {
                                                         "tf": 1
                                                     },
                                                     "pystorcli2.Controller.create_vd": {
                                                         "tf": 1
                                                     },
-                                                    "pystorcli2.Controller.patrolread_start": {
-                                                        "tf": 1
-                                                    },
-                                                    "pystorcli2.Controller.patrolread_stop": {
-                                                        "tf": 1
-                                                    },
-                                                    "pystorcli2.Controller.patrolread_pause": {
-                                                        "tf": 1
-                                                    },
-                                                    "pystorcli2.Controller.patrolread_resume": {
-                                                        "tf": 1
-                                                    },
-                                                    "pystorcli2.Controller.patrolread_running": {
-                                                        "tf": 1
-                                                    },
                                                     "pystorcli2.Controllers.get_ctl": {
                                                         "tf": 1
                                                     },
                                                     "pystorcli2.Enclosures.get_encl": {
                                                         "tf": 1
                                                     },
                                                     "pystorcli2.Drive.init_start": {
@@ -24548,15 +23207,15 @@
                                                     "pystorcli2.VirtualDrives.get_vd": {
                                                         "tf": 1
                                                     },
                                                     "pystorcli2.VirtualDrives.get_named_vd": {
                                                         "tf": 1
                                                     }
                                                 },
-                                                "df": 40
+                                                "df": 35
                                             }
                                         }
                                     }
                                 }
                             },
                             "p": {
                                 "docs": {},
@@ -24660,63 +23319,24 @@
                                         "docs": {},
                                         "df": 0,
                                         "l": {
                                             "docs": {},
                                             "df": 0,
                                             "d": {
                                                 "docs": {
-                                                    "pystorcli2.Controller": {
-                                                        "tf": 1
-                                                    },
                                                     "pystorcli2.Drive": {
                                                         "tf": 2.23606797749979
                                                     }
                                                 },
-                                                "df": 2
+                                                "df": 1
                                             }
                                         }
                                     }
                                 }
                             },
-                            "a": {
-                                "docs": {},
-                                "df": 0,
-                                "d": {
-                                    "docs": {
-                                        "pystorcli2.Controller": {
-                                            "tf": 2.8284271247461903
-                                        },
-                                        "pystorcli2.Controller.set_patrolread": {
-                                            "tf": 1.7320508075688772
-                                        },
-                                        "pystorcli2.Controller.patrolread_start": {
-                                            "tf": 1
-                                        },
-                                        "pystorcli2.Controller.patrolread_stop": {
-                                            "tf": 1
-                                        },
-                                        "pystorcli2.Controller.patrolread_pause": {
-                                            "tf": 1
-                                        },
-                                        "pystorcli2.Controller.patrolread_resume": {
-                                            "tf": 1
-                                        },
-                                        "pystorcli2.Controller.patrolread_running": {
-                                            "tf": 1
-                                        },
-                                        "pystorcli2.VirtualDrive": {
-                                            "tf": 1
-                                        },
-                                        "pystorcli2.VirtualDrive.rdcache": {
-                                            "tf": 1.7320508075688772
-                                        }
-                                    },
-                                    "df": 9
-                                }
-                            },
                             "m": {
                                 "docs": {},
                                 "df": 0,
                                 "o": {
                                     "docs": {},
                                     "df": 0,
                                     "v": {
@@ -24760,14 +23380,29 @@
                                                 },
                                                 "df": 1
                                             }
                                         }
                                     }
                                 }
                             },
+                            "a": {
+                                "docs": {},
+                                "df": 0,
+                                "d": {
+                                    "docs": {
+                                        "pystorcli2.VirtualDrive": {
+                                            "tf": 1
+                                        },
+                                        "pystorcli2.VirtualDrive.rdcache": {
+                                            "tf": 1.7320508075688772
+                                        }
+                                    },
+                                    "df": 2
+                                }
+                            },
                             "c": {
                                 "docs": {},
                                 "df": 0,
                                 "o": {
                                     "docs": {},
                                     "df": 0,
                                     "v": {
@@ -24974,20 +23609,14 @@
                                         "docs": {},
                                         "df": 0,
                                         "n": {
                                             "docs": {},
                                             "df": 0,
                                             "g": {
                                                 "docs": {
-                                                    "pystorcli2.Controller": {
-                                                        "tf": 1.7320508075688772
-                                                    },
-                                                    "pystorcli2.Controller.patrolread_running": {
-                                                        "tf": 1
-                                                    },
                                                     "pystorcli2.Drive": {
                                                         "tf": 2.6457513110645907
                                                     },
                                                     "pystorcli2.Drive.init_running": {
                                                         "tf": 1
                                                     },
                                                     "pystorcli2.Drive.erase_running": {
@@ -25002,15 +23631,15 @@
                                                     "pystorcli2.VirtualDrive.erase_running": {
                                                         "tf": 1
                                                     },
                                                     "pystorcli2.VirtualDrive.migrate_running": {
                                                         "tf": 1
                                                     }
                                                 },
-                                                "df": 9
+                                                "df": 7
                                             }
                                         }
                                     }
                                 }
                             }
                         },
                         "d": {
```

### Comparing `PyStorCLI2-0.6.1/pyproject.toml` & `PyStorCLI2-0.6.1.dev6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/pystorcli/__init__.py` & `PyStorCLI2-0.6.1.dev6/pystorcli/__init__.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/pystorcli/cachevault.py` & `PyStorCLI2-0.6.1.dev6/pystorcli/cachevault.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/pystorcli/cmdRunner.py` & `PyStorCLI2-0.6.1.dev6/pystorcli/cmdRunner.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/pystorcli/common.py` & `PyStorCLI2-0.6.1.dev6/pystorcli/common.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/pystorcli/drive.py` & `PyStorCLI2-0.6.1.dev6/pystorcli/drive.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/pystorcli/enclosure.py` & `PyStorCLI2-0.6.1.dev6/pystorcli/enclosure.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/pystorcli/exc.py` & `PyStorCLI2-0.6.1.dev6/pystorcli/exc.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/pystorcli/storcli.py` & `PyStorCLI2-0.6.1.dev6/pystorcli/storcli.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/pystorcli/virtualdrive.py` & `PyStorCLI2-0.6.1.dev6/pystorcli/virtualdrive.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/pystorcli2/__init__.py` & `PyStorCLI2-0.6.1.dev6/pystorcli2/__init__.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/pystorcli2/bin/metrics.py` & `PyStorCLI2-0.6.1.dev6/pystorcli2/bin/metrics.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/pystorcli2/cachevault.py` & `PyStorCLI2-0.6.1.dev6/pystorcli2/cachevault.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/pystorcli2/cmdRunner.py` & `PyStorCLI2-0.6.1.dev6/pystorcli2/cmdRunner.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/pystorcli2/common.py` & `PyStorCLI2-0.6.1.dev6/pystorcli2/common.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/pystorcli2/drive.py` & `PyStorCLI2-0.6.1.dev6/pystorcli2/drive.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/pystorcli2/enclosure.py` & `PyStorCLI2-0.6.1.dev6/pystorcli2/enclosure.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/pystorcli2/exc.py` & `PyStorCLI2-0.6.1.dev6/pystorcli2/exc.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/pystorcli2/storcli.py` & `PyStorCLI2-0.6.1.dev6/pystorcli2/storcli.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/pystorcli2/virtualdrive.py` & `PyStorCLI2-0.6.1.dev6/pystorcli2/virtualdrive.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/pystorcli_mirror/__init__.py` & `PyStorCLI2-0.6.1.dev6/pystorcli_mirror/__init__.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/tests/baseTest.py` & `PyStorCLI2-0.6.1.dev6/tests/baseTest.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/tests/datatest/controllerSet/test01/_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/controllerSet/test01/_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/tests/datatest/controllerSet/test02/_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/controllerSet/test02/_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/tests/datatest/namedSet/create_vd_raid0_00/__c0_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid0_00/__c0_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/tests/datatest/namedSet/create_vd_raid0_00/__c0_v1_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid0_00/__c0_v1_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/tests/datatest/namedSet/create_vd_raid0_00/_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid0_00/_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/tests/datatest/namedSet/create_vd_raid1_00/__c0_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid1_00/__c0_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/tests/datatest/namedSet/create_vd_raid1_00/__c0_v1_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid1_00/__c0_v1_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/tests/datatest/namedSet/create_vd_raid1_00/_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/create_vd_raid1_00/_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/tests/datatest/namedSet/delete_vd_00/__c0_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/delete_vd_00/__c0_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/tests/datatest/namedSet/delete_vd_00/__c0_v1_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/delete_vd_00/__c0_v1_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/tests/datatest/namedSet/delete_vd_00/_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/delete_vd_00/_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/tests/datatest/namedSet/set_state_offline_00/__c0_e35_s12_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/set_state_offline_00/__c0_e35_s12_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/tests/datatest/namedSet/set_state_offline_00/__c0_e35_sall_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/set_state_offline_00/__c0_e35_sall_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/tests/datatest/namedSet/set_state_offline_00/__c0_e35_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/set_state_offline_00/__c0_e35_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/tests/datatest/namedSet/set_state_offline_00/__c0_eall_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/set_state_offline_00/__c0_eall_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/tests/datatest/namedSet/set_state_offline_00/__c0_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/set_state_offline_00/__c0_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/tests/datatest/namedSet/set_state_offline_00/_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/set_state_offline_00/_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/tests/datatest/namedSet/show_events_00/__c0_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/show_events_00/__c0_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/tests/datatest/namedSet/show_events_00/_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/show_events_00/_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/tests/datatest/namedSet/spindown_disk_00/__c0_e35_s12_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/spindown_disk_00/__c0_e35_s12_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/tests/datatest/namedSet/spindown_disk_00/__c0_e35_sall_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/spindown_disk_00/__c0_e35_sall_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/tests/datatest/namedSet/spindown_disk_00/__c0_e35_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/spindown_disk_00/__c0_e35_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/tests/datatest/namedSet/spindown_disk_00/__c0_eall_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/spindown_disk_00/__c0_eall_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/tests/datatest/namedSet/spindown_disk_00/__c0_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/spindown_disk_00/__c0_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/tests/datatest/namedSet/spindown_disk_00/_show_J.json` & `PyStorCLI2-0.6.1.dev6/tests/datatest/namedSet/spindown_disk_00/_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/tests/exceptions.py` & `PyStorCLI2-0.6.1.dev6/tests/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/tests/storclifile.py` & `PyStorCLI2-0.6.1.dev6/tests/storclifile.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/tests/test_common.py` & `PyStorCLI2-0.6.1.dev6/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/tests/test_controllers.py` & `PyStorCLI2-0.6.1.dev6/tests/test_controllers.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/tests/test_operations.py` & `PyStorCLI2-0.6.1.dev6/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.1/tests/test_storcli.py` & `PyStorCLI2-0.6.1.dev6/tests/test_storcli.py`

 * *Files identical despite different names*

