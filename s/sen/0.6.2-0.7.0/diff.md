# Comparing `tmp/sen-0.6.2.tar.gz` & `tmp/sen-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sen-0.6.2.tar", last modified: Mon Nov  1 09:40:20 2021, max compression
+gzip compressed data, was "sen-0.7.0.tar", last modified: Wed Apr 12 08:19:55 2023, max compression
```

## Comparing `sen-0.6.2.tar` & `sen-0.7.0.tar`

### file list

```diff
@@ -1,81 +1,98 @@
-drwxr-xr-x   0 tt        (1000) tt        (1000)        0 2021-11-01 09:40:20.727424 sen-0.6.2/
--rw-r--r--   0 tt        (1000) tt        (1000)     1081 2021-11-01 09:02:44.000000 sen-0.6.2/LICENSE
--rw-r--r--   0 tt        (1000) tt        (1000)      204 2021-11-01 09:02:44.000000 sen-0.6.2/MANIFEST.in
--rw-r--r--   0 tt        (1000) tt        (1000)      773 2021-11-01 09:40:20.727424 sen-0.6.2/PKG-INFO
--rw-r--r--   0 tt        (1000) tt        (1000)     7197 2021-11-01 09:37:08.000000 sen-0.6.2/README.md
-drwxr-xr-x   0 tt        (1000) tt        (1000)        0 2021-11-01 09:40:20.721423 sen-0.6.2/docs/
--rw-r--r--   0 tt        (1000) tt        (1000)     1211 2021-11-01 09:02:44.000000 sen-0.6.2/docs/devel.md
--rw-r--r--   0 tt        (1000) tt        (1000)      329 2021-11-01 09:02:44.000000 sen-0.6.2/docs/features.md
--rw-r--r--   0 tt        (1000) tt        (1000)      427 2021-11-01 09:02:44.000000 sen-0.6.2/docs/releasing.md
--rw-r--r--   0 tt        (1000) tt        (1000)     1407 2021-11-01 09:02:44.000000 sen-0.6.2/io.github.tomastomecek.sen.metainfo.xml
--rw-r--r--   0 tt        (1000) tt        (1000)       23 2021-11-01 09:02:44.000000 sen-0.6.2/requirements-test.txt
--rw-r--r--   0 tt        (1000) tt        (1000)      230 2021-11-01 09:02:44.000000 sen-0.6.2/requirements.txt
-drwxr-xr-x   0 tt        (1000) tt        (1000)        0 2021-11-01 09:40:20.722423 sen-0.6.2/sen/
--rw-r--r--   0 tt        (1000) tt        (1000)      695 2021-11-01 09:37:08.000000 sen-0.6.2/sen/__init__.py
--rwxr-xr-x   0 tt        (1000) tt        (1000)     2524 2021-11-01 09:02:44.000000 sen-0.6.2/sen/cli.py
--rw-r--r--   0 tt        (1000) tt        (1000)      146 2021-11-01 09:02:44.000000 sen-0.6.2/sen/constants.py
--rw-r--r--   0 tt        (1000) tt        (1000)    29705 2021-11-01 09:02:44.000000 sen-0.6.2/sen/docker_backend.py
--rw-r--r--   0 tt        (1000) tt        (1000)      289 2021-11-01 09:02:44.000000 sen-0.6.2/sen/exceptions.py
--rw-r--r--   0 tt        (1000) tt        (1000)     2650 2021-11-01 09:02:44.000000 sen-0.6.2/sen/net.py
-drwxr-xr-x   0 tt        (1000) tt        (1000)        0 2021-11-01 09:40:20.724424 sen-0.6.2/sen/tui/
--rw-r--r--   0 tt        (1000) tt        (1000)       18 2021-11-01 09:02:44.000000 sen-0.6.2/sen/tui/__init__.py
--rw-r--r--   0 tt        (1000) tt        (1000)    10717 2021-11-01 09:02:44.000000 sen-0.6.2/sen/tui/buffer.py
-drwxr-xr-x   0 tt        (1000) tt        (1000)        0 2021-11-01 09:40:20.724424 sen-0.6.2/sen/tui/chunks/
--rw-r--r--   0 tt        (1000) tt        (1000)       80 2021-11-01 09:02:44.000000 sen-0.6.2/sen/tui/chunks/__init__.py
--rw-r--r--   0 tt        (1000) tt        (1000)     2147 2021-11-01 09:02:44.000000 sen-0.6.2/sen/tui/chunks/container.py
--rw-r--r--   0 tt        (1000) tt        (1000)     3108 2021-11-01 09:02:44.000000 sen-0.6.2/sen/tui/chunks/image.py
--rw-r--r--   0 tt        (1000) tt        (1000)      544 2021-11-01 09:02:44.000000 sen-0.6.2/sen/tui/chunks/misc.py
-drwxr-xr-x   0 tt        (1000) tt        (1000)        0 2021-11-01 09:40:20.724424 sen-0.6.2/sen/tui/commands/
--rw-r--r--   0 tt        (1000) tt        (1000)      160 2021-11-01 09:02:44.000000 sen-0.6.2/sen/tui/commands/__init__.py
--rw-r--r--   0 tt        (1000) tt        (1000)     6845 2021-11-01 09:02:44.000000 sen-0.6.2/sen/tui/commands/backend.py
--rw-r--r--   0 tt        (1000) tt        (1000)     9229 2021-11-01 09:02:44.000000 sen-0.6.2/sen/tui/commands/base.py
--rw-r--r--   0 tt        (1000) tt        (1000)     2053 2021-11-01 09:02:44.000000 sen-0.6.2/sen/tui/commands/display.py
--rw-r--r--   0 tt        (1000) tt        (1000)     8746 2021-11-01 09:02:44.000000 sen-0.6.2/sen/tui/commands/ui.py
--rw-r--r--   0 tt        (1000) tt        (1000)     2603 2021-11-01 09:02:44.000000 sen-0.6.2/sen/tui/commands/widget.py
--rw-r--r--   0 tt        (1000) tt        (1000)     3740 2021-11-01 09:02:44.000000 sen-0.6.2/sen/tui/constants.py
--rw-r--r--   0 tt        (1000) tt        (1000)     1995 2021-11-01 09:02:44.000000 sen-0.6.2/sen/tui/init.py
--rw-r--r--   0 tt        (1000) tt        (1000)    13199 2021-11-01 09:02:44.000000 sen-0.6.2/sen/tui/ui.py
-drwxr-xr-x   0 tt        (1000) tt        (1000)        0 2021-11-01 09:40:20.725423 sen-0.6.2/sen/tui/views/
--rw-r--r--   0 tt        (1000) tt        (1000)      101 2021-11-01 09:02:44.000000 sen-0.6.2/sen/tui/views/__init__.py
--rw-r--r--   0 tt        (1000) tt        (1000)      253 2021-11-01 09:02:44.000000 sen-0.6.2/sen/tui/views/base.py
--rw-r--r--   0 tt        (1000) tt        (1000)    15627 2021-11-01 09:02:44.000000 sen-0.6.2/sen/tui/views/container_info.py
--rw-r--r--   0 tt        (1000) tt        (1000)     4990 2021-11-01 09:02:44.000000 sen-0.6.2/sen/tui/views/disk_usage.py
--rw-r--r--   0 tt        (1000) tt        (1000)     4575 2021-11-01 09:02:44.000000 sen-0.6.2/sen/tui/views/help.py
--rw-r--r--   0 tt        (1000) tt        (1000)     5152 2021-11-01 09:02:44.000000 sen-0.6.2/sen/tui/views/image_info.py
--rw-r--r--   0 tt        (1000) tt        (1000)     7865 2021-11-01 09:02:44.000000 sen-0.6.2/sen/tui/views/main.py
-drwxr-xr-x   0 tt        (1000) tt        (1000)        0 2021-11-01 09:40:20.725423 sen-0.6.2/sen/tui/widgets/
--rw-r--r--   0 tt        (1000) tt        (1000)      118 2021-11-01 09:02:44.000000 sen-0.6.2/sen/tui/widgets/__init__.py
--rw-r--r--   0 tt        (1000) tt        (1000)     1686 2021-11-01 09:02:44.000000 sen-0.6.2/sen/tui/widgets/graph.py
-drwxr-xr-x   0 tt        (1000) tt        (1000)        0 2021-11-01 09:40:20.726424 sen-0.6.2/sen/tui/widgets/list/
--rw-r--r--   0 tt        (1000) tt        (1000)       59 2021-11-01 09:02:44.000000 sen-0.6.2/sen/tui/widgets/list/__init__.py
--rw-r--r--   0 tt        (1000) tt        (1000)     4229 2021-11-01 09:02:44.000000 sen-0.6.2/sen/tui/widgets/list/base.py
--rw-r--r--   0 tt        (1000) tt        (1000)     5040 2021-11-01 09:02:44.000000 sen-0.6.2/sen/tui/widgets/list/common.py
--rw-r--r--   0 tt        (1000) tt        (1000)     3052 2021-11-01 09:02:44.000000 sen-0.6.2/sen/tui/widgets/list/util.py
--rw-r--r--   0 tt        (1000) tt        (1000)      581 2021-11-01 09:02:44.000000 sen-0.6.2/sen/tui/widgets/responsive_column.py
--rw-r--r--   0 tt        (1000) tt        (1000)     4607 2021-11-01 09:02:44.000000 sen-0.6.2/sen/tui/widgets/table.py
--rw-r--r--   0 tt        (1000) tt        (1000)     2337 2021-11-01 09:02:44.000000 sen-0.6.2/sen/tui/widgets/tree.py
--rw-r--r--   0 tt        (1000) tt        (1000)     2526 2021-11-01 09:02:44.000000 sen-0.6.2/sen/tui/widgets/util.py
--rw-r--r--   0 tt        (1000) tt        (1000)     8152 2021-11-01 09:02:44.000000 sen-0.6.2/sen/util.py
-drwxr-xr-x   0 tt        (1000) tt        (1000)        0 2021-11-01 09:40:20.723424 sen-0.6.2/sen.egg-info/
--rw-r--r--   0 tt        (1000) tt        (1000)      773 2021-11-01 09:40:20.000000 sen-0.6.2/sen.egg-info/PKG-INFO
--rw-r--r--   0 tt        (1000) tt        (1000)     1518 2021-11-01 09:40:20.000000 sen-0.6.2/sen.egg-info/SOURCES.txt
--rw-r--r--   0 tt        (1000) tt        (1000)      109 2021-11-01 09:40:20.000000 sen-0.6.2/sen.egg-info/dependency_links.txt
--rw-r--r--   0 tt        (1000) tt        (1000)       38 2021-11-01 09:40:20.000000 sen-0.6.2/sen.egg-info/entry_points.txt
--rw-r--r--   0 tt        (1000) tt        (1000)       24 2021-11-01 09:40:20.000000 sen-0.6.2/sen.egg-info/requires.txt
--rw-r--r--   0 tt        (1000) tt        (1000)        4 2021-11-01 09:40:20.000000 sen-0.6.2/sen.egg-info/top_level.txt
--rw-r--r--   0 tt        (1000) tt        (1000)    90618 2021-11-01 09:02:44.000000 sen-0.6.2/sen.svg
--rw-r--r--   0 tt        (1000) tt        (1000)       79 2021-11-01 09:40:20.727424 sen-0.6.2/setup.cfg
--rwxr-xr-x   0 tt        (1000) tt        (1000)     1539 2021-11-01 09:37:08.000000 sen-0.6.2/setup.py
-drwxr-xr-x   0 tt        (1000) tt        (1000)        0 2021-11-01 09:40:20.727424 sen-0.6.2/tests/
--rw-r--r--   0 tt        (1000) tt        (1000)        1 2021-11-01 09:02:44.000000 sen-0.6.2/tests/__init__.py
--rw-r--r--   0 tt        (1000) tt        (1000)       36 2021-11-01 09:02:44.000000 sen-0.6.2/tests/constants.py
--rw-r--r--   0 tt        (1000) tt        (1000)      256 2021-11-01 09:02:44.000000 sen-0.6.2/tests/full.fmf
--rw-r--r--   0 tt        (1000) tt        (1000)    29672 2021-11-01 09:02:44.000000 sen-0.6.2/tests/real.py
--rw-r--r--   0 tt        (1000) tt        (1000)     1984 2021-11-01 09:02:44.000000 sen-0.6.2/tests/test_commands.py
--rw-r--r--   0 tt        (1000) tt        (1000)     2113 2021-11-01 09:02:44.000000 sen-0.6.2/tests/test_concurrency.py
--rw-r--r--   0 tt        (1000) tt        (1000)     1658 2021-11-01 09:02:44.000000 sen-0.6.2/tests/test_container_info.py
--rw-r--r--   0 tt        (1000) tt        (1000)     2170 2021-11-01 09:02:44.000000 sen-0.6.2/tests/test_docker_backend.py
--rw-r--r--   0 tt        (1000) tt        (1000)     2618 2021-11-01 09:02:44.000000 sen-0.6.2/tests/test_net.py
--rw-r--r--   0 tt        (1000) tt        (1000)     4571 2021-11-01 09:02:44.000000 sen-0.6.2/tests/test_util.py
--rw-r--r--   0 tt        (1000) tt        (1000)     4463 2021-11-01 09:02:44.000000 sen-0.6.2/tests/test_widgets.py
--rw-r--r--   0 tt        (1000) tt        (1000)      315 2021-11-01 09:02:44.000000 sen-0.6.2/tests/utils.py
+drwxr-xr-x   0 tt        (1000) tt        (1000)        0 2023-04-12 08:19:55.138561 sen-0.7.0/
+drwxr-xr-x   0 tt        (1000) tt        (1000)        0 2023-04-12 08:19:55.121561 sen-0.7.0/.fmf/
+-rw-r--r--   0 tt        (1000) tt        (1000)        2 2021-11-01 09:02:44.000000 sen-0.7.0/.fmf/version
+-rw-r--r--   0 tt        (1000) tt        (1000)       38 2021-11-01 09:02:44.000000 sen-0.7.0/.gitignore
+-rw-r--r--   0 tt        (1000) tt        (1000)      242 2023-04-12 07:22:19.000000 sen-0.7.0/.packit.yaml
+-rw-r--r--   0 tt        (1000) tt        (1000)     1152 2021-11-01 09:02:44.000000 sen-0.7.0/.travis.yml
+-rw-r--r--   0 tt        (1000) tt        (1000)     5923 2023-04-12 07:22:19.000000 sen-0.7.0/CHANGELOG.md
+-rw-r--r--   0 tt        (1000) tt        (1000)      561 2023-04-12 08:19:29.000000 sen-0.7.0/Dockerfile
+-rw-r--r--   0 tt        (1000) tt        (1000)      416 2021-11-01 09:02:44.000000 sen-0.7.0/Dockerfile.fedora
+-rw-r--r--   0 tt        (1000) tt        (1000)     1081 2021-11-01 09:02:44.000000 sen-0.7.0/LICENSE
+-rw-r--r--   0 tt        (1000) tt        (1000)      204 2021-11-01 09:02:44.000000 sen-0.7.0/MANIFEST.in
+-rw-r--r--   0 tt        (1000) tt        (1000)      756 2023-04-12 08:19:55.138561 sen-0.7.0/PKG-INFO
+-rw-r--r--   0 tt        (1000) tt        (1000)     7197 2021-11-01 09:37:08.000000 sen-0.7.0/README.md
+drwxr-xr-x   0 tt        (1000) tt        (1000)        0 2023-04-12 08:19:55.123561 sen-0.7.0/data/
+-rw-r--r--   0 tt        (1000) tt        (1000)   165888 2021-11-01 09:02:44.000000 sen-0.7.0/data/container-info.gif
+-rw-r--r--   0 tt        (1000) tt        (1000)   268444 2021-11-01 09:02:44.000000 sen-0.7.0/data/image-info.gif
+-rw-r--r--   0 tt        (1000) tt        (1000)   270819 2021-11-01 09:02:44.000000 sen-0.7.0/data/image-tree.gif
+-rw-r--r--   0 tt        (1000) tt        (1000)  1166820 2021-11-01 09:02:44.000000 sen-0.7.0/data/sen-preview.gif
+drwxr-xr-x   0 tt        (1000) tt        (1000)        0 2023-04-12 08:19:55.125561 sen-0.7.0/docs/
+-rw-r--r--   0 tt        (1000) tt        (1000)     1211 2021-11-01 09:02:44.000000 sen-0.7.0/docs/devel.md
+-rw-r--r--   0 tt        (1000) tt        (1000)      329 2021-11-01 09:02:44.000000 sen-0.7.0/docs/features.md
+-rw-r--r--   0 tt        (1000) tt        (1000)      427 2021-11-01 09:02:44.000000 sen-0.7.0/docs/releasing.md
+-rw-r--r--   0 tt        (1000) tt        (1000)     1407 2021-11-01 09:02:44.000000 sen-0.7.0/io.github.tomastomecek.sen.metainfo.xml
+drwxr-xr-x   0 tt        (1000) tt        (1000)        0 2023-04-12 08:19:55.125561 sen-0.7.0/plans/
+-rw-r--r--   0 tt        (1000) tt        (1000)      434 2021-11-01 09:02:44.000000 sen-0.7.0/plans/README.md
+-rw-r--r--   0 tt        (1000) tt        (1000)      105 2021-11-01 09:02:44.000000 sen-0.7.0/plans/full.fmf
+-rw-r--r--   0 tt        (1000) tt        (1000)       23 2021-11-01 09:02:44.000000 sen-0.7.0/requirements-test.txt
+-rw-r--r--   0 tt        (1000) tt        (1000)      230 2023-04-12 08:19:29.000000 sen-0.7.0/requirements.txt
+drwxr-xr-x   0 tt        (1000) tt        (1000)        0 2023-04-12 08:19:55.126561 sen-0.7.0/sen/
+-rw-r--r--   0 tt        (1000) tt        (1000)      695 2023-04-12 07:22:19.000000 sen-0.7.0/sen/__init__.py
+-rwxr-xr-x   0 tt        (1000) tt        (1000)     2524 2021-11-01 09:02:44.000000 sen-0.7.0/sen/cli.py
+-rw-r--r--   0 tt        (1000) tt        (1000)      146 2021-11-01 09:02:44.000000 sen-0.7.0/sen/constants.py
+-rw-r--r--   0 tt        (1000) tt        (1000)    29705 2021-11-01 09:02:44.000000 sen-0.7.0/sen/docker_backend.py
+-rw-r--r--   0 tt        (1000) tt        (1000)      289 2021-11-01 09:02:44.000000 sen-0.7.0/sen/exceptions.py
+-rw-r--r--   0 tt        (1000) tt        (1000)     3145 2022-10-03 07:27:30.000000 sen-0.7.0/sen/net.py
+drwxr-xr-x   0 tt        (1000) tt        (1000)        0 2023-04-12 08:19:55.129561 sen-0.7.0/sen/tui/
+-rw-r--r--   0 tt        (1000) tt        (1000)       18 2021-11-01 09:02:44.000000 sen-0.7.0/sen/tui/__init__.py
+-rw-r--r--   0 tt        (1000) tt        (1000)    10717 2021-11-01 09:02:44.000000 sen-0.7.0/sen/tui/buffer.py
+drwxr-xr-x   0 tt        (1000) tt        (1000)        0 2023-04-12 08:19:55.129561 sen-0.7.0/sen/tui/chunks/
+-rw-r--r--   0 tt        (1000) tt        (1000)       80 2021-11-01 09:02:44.000000 sen-0.7.0/sen/tui/chunks/__init__.py
+-rw-r--r--   0 tt        (1000) tt        (1000)     2147 2021-11-01 09:02:44.000000 sen-0.7.0/sen/tui/chunks/container.py
+-rw-r--r--   0 tt        (1000) tt        (1000)     3108 2021-11-01 09:02:44.000000 sen-0.7.0/sen/tui/chunks/image.py
+-rw-r--r--   0 tt        (1000) tt        (1000)      544 2021-11-01 09:02:44.000000 sen-0.7.0/sen/tui/chunks/misc.py
+drwxr-xr-x   0 tt        (1000) tt        (1000)        0 2023-04-12 08:19:55.131561 sen-0.7.0/sen/tui/commands/
+-rw-r--r--   0 tt        (1000) tt        (1000)      160 2021-11-01 09:02:44.000000 sen-0.7.0/sen/tui/commands/__init__.py
+-rw-r--r--   0 tt        (1000) tt        (1000)     6845 2021-11-01 09:02:44.000000 sen-0.7.0/sen/tui/commands/backend.py
+-rw-r--r--   0 tt        (1000) tt        (1000)     9229 2021-11-01 09:02:44.000000 sen-0.7.0/sen/tui/commands/base.py
+-rw-r--r--   0 tt        (1000) tt        (1000)     2053 2021-11-01 09:02:44.000000 sen-0.7.0/sen/tui/commands/display.py
+-rw-r--r--   0 tt        (1000) tt        (1000)     8746 2021-11-01 09:02:44.000000 sen-0.7.0/sen/tui/commands/ui.py
+-rw-r--r--   0 tt        (1000) tt        (1000)     2603 2021-11-01 09:02:44.000000 sen-0.7.0/sen/tui/commands/widget.py
+-rw-r--r--   0 tt        (1000) tt        (1000)     3740 2021-11-01 09:02:44.000000 sen-0.7.0/sen/tui/constants.py
+-rw-r--r--   0 tt        (1000) tt        (1000)     1995 2021-11-01 09:02:44.000000 sen-0.7.0/sen/tui/init.py
+-rw-r--r--   0 tt        (1000) tt        (1000)    13199 2021-11-01 09:02:44.000000 sen-0.7.0/sen/tui/ui.py
+drwxr-xr-x   0 tt        (1000) tt        (1000)        0 2023-04-12 08:19:55.132561 sen-0.7.0/sen/tui/views/
+-rw-r--r--   0 tt        (1000) tt        (1000)      101 2021-11-01 09:02:44.000000 sen-0.7.0/sen/tui/views/__init__.py
+-rw-r--r--   0 tt        (1000) tt        (1000)      253 2021-11-01 09:02:44.000000 sen-0.7.0/sen/tui/views/base.py
+-rw-r--r--   0 tt        (1000) tt        (1000)    15627 2021-11-01 09:02:44.000000 sen-0.7.0/sen/tui/views/container_info.py
+-rw-r--r--   0 tt        (1000) tt        (1000)     4990 2021-11-01 09:02:44.000000 sen-0.7.0/sen/tui/views/disk_usage.py
+-rw-r--r--   0 tt        (1000) tt        (1000)     4575 2021-11-01 09:02:44.000000 sen-0.7.0/sen/tui/views/help.py
+-rw-r--r--   0 tt        (1000) tt        (1000)     5152 2021-11-01 09:02:44.000000 sen-0.7.0/sen/tui/views/image_info.py
+-rw-r--r--   0 tt        (1000) tt        (1000)     7865 2021-11-01 09:02:44.000000 sen-0.7.0/sen/tui/views/main.py
+drwxr-xr-x   0 tt        (1000) tt        (1000)        0 2023-04-12 08:19:55.133561 sen-0.7.0/sen/tui/widgets/
+-rw-r--r--   0 tt        (1000) tt        (1000)      118 2021-11-01 09:02:44.000000 sen-0.7.0/sen/tui/widgets/__init__.py
+-rw-r--r--   0 tt        (1000) tt        (1000)     1686 2021-11-01 09:02:44.000000 sen-0.7.0/sen/tui/widgets/graph.py
+drwxr-xr-x   0 tt        (1000) tt        (1000)        0 2023-04-12 08:19:55.135561 sen-0.7.0/sen/tui/widgets/list/
+-rw-r--r--   0 tt        (1000) tt        (1000)       59 2021-11-01 09:02:44.000000 sen-0.7.0/sen/tui/widgets/list/__init__.py
+-rw-r--r--   0 tt        (1000) tt        (1000)     4229 2021-11-01 09:02:44.000000 sen-0.7.0/sen/tui/widgets/list/base.py
+-rw-r--r--   0 tt        (1000) tt        (1000)     5040 2021-11-01 09:02:44.000000 sen-0.7.0/sen/tui/widgets/list/common.py
+-rw-r--r--   0 tt        (1000) tt        (1000)     3052 2021-11-01 09:02:44.000000 sen-0.7.0/sen/tui/widgets/list/util.py
+-rw-r--r--   0 tt        (1000) tt        (1000)      581 2021-11-01 09:02:44.000000 sen-0.7.0/sen/tui/widgets/responsive_column.py
+-rw-r--r--   0 tt        (1000) tt        (1000)     4607 2021-11-01 09:02:44.000000 sen-0.7.0/sen/tui/widgets/table.py
+-rw-r--r--   0 tt        (1000) tt        (1000)     2337 2021-11-01 09:02:44.000000 sen-0.7.0/sen/tui/widgets/tree.py
+-rw-r--r--   0 tt        (1000) tt        (1000)     2526 2021-11-01 09:02:44.000000 sen-0.7.0/sen/tui/widgets/util.py
+-rw-r--r--   0 tt        (1000) tt        (1000)     8164 2022-10-03 07:27:30.000000 sen-0.7.0/sen/util.py
+drwxr-xr-x   0 tt        (1000) tt        (1000)        0 2023-04-12 08:19:55.128561 sen-0.7.0/sen.egg-info/
+-rw-r--r--   0 tt        (1000) tt        (1000)      756 2023-04-12 08:19:54.000000 sen-0.7.0/sen.egg-info/PKG-INFO
+-rw-r--r--   0 tt        (1000) tt        (1000)     1734 2023-04-12 08:19:55.000000 sen-0.7.0/sen.egg-info/SOURCES.txt
+-rw-r--r--   0 tt        (1000) tt        (1000)      109 2023-04-12 08:19:54.000000 sen-0.7.0/sen.egg-info/dependency_links.txt
+-rw-r--r--   0 tt        (1000) tt        (1000)       37 2023-04-12 08:19:54.000000 sen-0.7.0/sen.egg-info/entry_points.txt
+-rw-r--r--   0 tt        (1000) tt        (1000)       24 2023-04-12 08:19:54.000000 sen-0.7.0/sen.egg-info/requires.txt
+-rw-r--r--   0 tt        (1000) tt        (1000)        4 2023-04-12 08:19:54.000000 sen-0.7.0/sen.egg-info/top_level.txt
+-rw-r--r--   0 tt        (1000) tt        (1000)     3705 2023-04-12 07:22:19.000000 sen-0.7.0/sen.spec
+-rw-r--r--   0 tt        (1000) tt        (1000)    90618 2021-11-01 09:02:44.000000 sen-0.7.0/sen.svg
+-rw-r--r--   0 tt        (1000) tt        (1000)       79 2023-04-12 08:19:55.138561 sen-0.7.0/setup.cfg
+-rwxr-xr-x   0 tt        (1000) tt        (1000)     1539 2023-04-12 07:22:19.000000 sen-0.7.0/setup.py
+drwxr-xr-x   0 tt        (1000) tt        (1000)        0 2023-04-12 08:19:55.138561 sen-0.7.0/tests/
+-rw-r--r--   0 tt        (1000) tt        (1000)        1 2021-11-01 09:02:44.000000 sen-0.7.0/tests/__init__.py
+-rw-r--r--   0 tt        (1000) tt        (1000)       36 2021-11-01 09:02:44.000000 sen-0.7.0/tests/constants.py
+-rw-r--r--   0 tt        (1000) tt        (1000)      228 2023-04-12 07:22:19.000000 sen-0.7.0/tests/full.fmf
+-rw-r--r--   0 tt        (1000) tt        (1000)    29672 2021-11-01 09:02:44.000000 sen-0.7.0/tests/real.py
+-rw-r--r--   0 tt        (1000) tt        (1000)     1984 2021-11-01 09:02:44.000000 sen-0.7.0/tests/test_commands.py
+-rw-r--r--   0 tt        (1000) tt        (1000)     2113 2021-11-01 09:02:44.000000 sen-0.7.0/tests/test_concurrency.py
+-rw-r--r--   0 tt        (1000) tt        (1000)     1658 2021-11-01 09:02:44.000000 sen-0.7.0/tests/test_container_info.py
+-rw-r--r--   0 tt        (1000) tt        (1000)     2170 2021-11-01 09:02:44.000000 sen-0.7.0/tests/test_docker_backend.py
+-rw-r--r--   0 tt        (1000) tt        (1000)     2618 2021-11-01 09:02:44.000000 sen-0.7.0/tests/test_net.py
+-rw-r--r--   0 tt        (1000) tt        (1000)     4571 2023-04-11 15:42:12.000000 sen-0.7.0/tests/test_util.py
+-rw-r--r--   0 tt        (1000) tt        (1000)     4463 2021-11-01 09:02:44.000000 sen-0.7.0/tests/test_widgets.py
+-rw-r--r--   0 tt        (1000) tt        (1000)      315 2021-11-01 09:02:44.000000 sen-0.7.0/tests/utils.py
```

### Comparing `sen-0.6.2/LICENSE` & `sen-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/PKG-INFO` & `sen-0.7.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: sen
-Version: 0.6.2
+Version: 0.7.0
 Summary: Terminal User Interface for Docker Engine
 Home-page: https://github.com/TomasTomecek/sen/
 Author: Tomas Tomecek
 Author-email: tomas@tomecek.net
 License: MIT
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Topic :: System :: Monitoring
+License-File: LICENSE
```

### Comparing `sen-0.6.2/README.md` & `sen-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/docs/devel.md` & `sen-0.7.0/docs/devel.md`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/io.github.tomastomecek.sen.metainfo.xml` & `sen-0.7.0/io.github.tomastomecek.sen.metainfo.xml`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/sen/__init__.py` & `sen-0.7.0/sen/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 
 from sen.constants import FALLBACK_LOG_PATH
 
-__version__ = '0.6.2'
+__version__ = '0.7.0'
 
 
 def set_logging(name="sen", level=logging.DEBUG, path=FALLBACK_LOG_PATH):
     logger = logging.getLogger(name)
     # do not propagate logs from logger 'sen' to root logger (as they could be accidentally
     # displayed in terminal)
     logger.propagate = False
```

### Comparing `sen-0.6.2/sen/cli.py` & `sen-0.7.0/sen/cli.py`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/sen/docker_backend.py` & `sen-0.7.0/sen/docker_backend.py`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/sen/net.py` & `sen-0.7.0/sen/net.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,20 +46,29 @@
 
         if self._ports is None:
             self._ports = {}
             if self.net_settings["Ports"]:
                 for key, value in self.net_settings["Ports"].items():
                     cleaned_port = key.split("/")[0]
                     self._ports[cleaned_port] = graceful_chain_get(value, 0, "HostPort")
+
             # in case of --net=host, there's nothing in network settings, let's get it from "Config"
+            exposed_ports_section = graceful_chain_get(self.inspect_data, "HostConfig", "PortBindings")
+            if exposed_ports_section:
+                for key, value in exposed_ports_section.items():
+                    cleaned_port = key.split("/")[0]
+                    if cleaned_port not in self._ports:
+                        self._ports[cleaned_port] = graceful_chain_get(value, 0, "HostPort")
+                        
             exposed_ports_section = graceful_chain_get(self.inspect_data, "Config", "ExposedPorts")
             if exposed_ports_section:
                 for key, value in exposed_ports_section.items():
                     cleaned_port = key.split("/")[0]
-                    self._ports[cleaned_port] = None  # extremely docker specific
+                    if cleaned_port not in self._ports:
+                        self._ports[cleaned_port] = None  # extremely docker specific
         return self._ports
 
     @property
     def ips(self):
         """
         :return: dict:
         {
```

### Comparing `sen-0.6.2/sen/tui/buffer.py` & `sen-0.7.0/sen/tui/buffer.py`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/sen/tui/chunks/container.py` & `sen-0.7.0/sen/tui/chunks/container.py`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/sen/tui/chunks/image.py` & `sen-0.7.0/sen/tui/chunks/image.py`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/sen/tui/chunks/misc.py` & `sen-0.7.0/sen/tui/chunks/misc.py`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/sen/tui/commands/backend.py` & `sen-0.7.0/sen/tui/commands/backend.py`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/sen/tui/commands/base.py` & `sen-0.7.0/sen/tui/commands/base.py`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/sen/tui/commands/display.py` & `sen-0.7.0/sen/tui/commands/display.py`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/sen/tui/commands/ui.py` & `sen-0.7.0/sen/tui/commands/ui.py`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/sen/tui/commands/widget.py` & `sen-0.7.0/sen/tui/commands/widget.py`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/sen/tui/constants.py` & `sen-0.7.0/sen/tui/constants.py`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/sen/tui/init.py` & `sen-0.7.0/sen/tui/init.py`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/sen/tui/ui.py` & `sen-0.7.0/sen/tui/ui.py`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/sen/tui/views/container_info.py` & `sen-0.7.0/sen/tui/views/container_info.py`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/sen/tui/views/disk_usage.py` & `sen-0.7.0/sen/tui/views/disk_usage.py`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/sen/tui/views/help.py` & `sen-0.7.0/sen/tui/views/help.py`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/sen/tui/views/image_info.py` & `sen-0.7.0/sen/tui/views/image_info.py`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/sen/tui/views/main.py` & `sen-0.7.0/sen/tui/views/main.py`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/sen/tui/widgets/graph.py` & `sen-0.7.0/sen/tui/widgets/graph.py`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/sen/tui/widgets/list/base.py` & `sen-0.7.0/sen/tui/widgets/list/base.py`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/sen/tui/widgets/list/common.py` & `sen-0.7.0/sen/tui/widgets/list/common.py`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/sen/tui/widgets/list/util.py` & `sen-0.7.0/sen/tui/widgets/list/util.py`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/sen/tui/widgets/responsive_column.py` & `sen-0.7.0/sen/tui/widgets/responsive_column.py`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/sen/tui/widgets/table.py` & `sen-0.7.0/sen/tui/widgets/table.py`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/sen/tui/widgets/tree.py` & `sen-0.7.0/sen/tui/widgets/tree.py`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/sen/tui/widgets/util.py` & `sen-0.7.0/sen/tui/widgets/util.py`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/sen/util.py` & `sen-0.7.0/sen/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,15 @@
     # du = json.dumps(d, indent=2)
     # logger.debug("XXX: %s", du)
     cpu_percent = 0.0
     cpu_total = float(d["cpu_stats"]["cpu_usage"]["total_usage"])
     cpu_delta = cpu_total - previous_cpu
     cpu_system = float(d["cpu_stats"]["system_cpu_usage"])
     system_delta = cpu_system - previous_system
-    online_cpus = d["cpu_stats"].get("online_cpus", len(d["cpu_stats"]["cpu_usage"]["percpu_usage"]))
+    online_cpus = d["cpu_stats"].get("online_cpus", len(d["cpu_stats"]["cpu_usage"].get("percpu_usage", [None])))
     if system_delta > 0.0:
         cpu_percent = (cpu_delta / system_delta) * online_cpus * 100.0
     return cpu_percent, cpu_system, cpu_total
 
 
 def calculate_blkio_bytes(d):
     """
```

### Comparing `sen-0.6.2/sen.egg-info/PKG-INFO` & `sen-0.7.0/sen.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: sen
-Version: 0.6.2
+Version: 0.7.0
 Summary: Terminal User Interface for Docker Engine
 Home-page: https://github.com/TomasTomecek/sen/
 Author: Tomas Tomecek
 Author-email: tomas@tomecek.net
 License: MIT
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Topic :: System :: Monitoring
+License-File: LICENSE
```

### Comparing `sen-0.6.2/sen.svg` & `sen-0.7.0/sen.svg`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/setup.py` & `sen-0.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "urwid",
     "docker",
     "urwidtrees"
 ]
 
 setup(
     name='sen',
-    version='0.6.2',
+    version='0.7.0',
     description="Terminal User Interface for Docker Engine",
     author='Tomas Tomecek',
     author_email='tomas@tomecek.net',
     url="https://github.com/TomasTomecek/sen/",
     license="MIT",
     entry_points={
         'console_scripts': ['sen=sen.cli:main'],
```

### Comparing `sen-0.6.2/tests/real.py` & `sen-0.7.0/tests/real.py`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/tests/test_commands.py` & `sen-0.7.0/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/tests/test_concurrency.py` & `sen-0.7.0/tests/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/tests/test_container_info.py` & `sen-0.7.0/tests/test_container_info.py`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/tests/test_docker_backend.py` & `sen-0.7.0/tests/test_docker_backend.py`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/tests/test_net.py` & `sen-0.7.0/tests/test_net.py`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/tests/test_util.py` & `sen-0.7.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `sen-0.6.2/tests/test_widgets.py` & `sen-0.7.0/tests/test_widgets.py`

 * *Files identical despite different names*

