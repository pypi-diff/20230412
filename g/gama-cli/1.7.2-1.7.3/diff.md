# Comparing `tmp/gama_cli-1.7.2.tar.gz` & `tmp/gama_cli-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gama_cli-1.7.2.tar", last modified: Tue Apr 11 23:06:46 2023, max compression
+gzip compressed data, was "gama_cli-1.7.3.tar", last modified: Tue Apr 11 23:30:58 2023, max compression
```

## Comparing `gama_cli-1.7.2.tar` & `gama_cli-1.7.3.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-11 23:06:46.191477 gama_cli-1.7.2/
--rw-rw-r--   0 runner    (1000) runner    (1001)     2302 2023-04-11 23:06:46.191477 gama_cli-1.7.2/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)     1664 2023-04-11 23:05:58.000000 gama_cli-1.7.2/README.md
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-11 23:06:46.191477 gama_cli-1.7.2/gama_cli/
--rw-rw-r--   0 runner    (1000) runner    (1001)        0 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/__init__.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-11 23:06:46.187477 gama_cli-1.7.2/gama_cli/assets/
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-11 23:06:46.191477 gama_cli-1.7.2/gama_cli/assets/greenstream/
--rw-rw-r--   0 runner    (1000) runner    (1001)      173 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/assets/greenstream/config.sim.yml
--rw-rw-r--   0 runner    (1000) runner    (1001)      597 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/assets/greenstream/config.stubs.yml
--rw-rw-r--   0 runner    (1000) runner    (1001)      583 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/assets/greenstream/config.variant.bravo.yml
--rw-rw-r--   0 runner    (1000) runner    (1001)      184 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/assets/greenstream/config.variant.educat.yml
--rw-rw-r--   0 runner    (1000) runner    (1001)     2539 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/banner.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     1231 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/cli.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-11 23:06:46.191477 gama_cli-1.7.2/gama_cli/config/
--rw-rw-r--   0 runner    (1000) runner    (1001)     1417 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/config/gama_gs.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     1995 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/config/gama_vessel.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-11 23:06:46.187477 gama_cli-1.7.2/gama_cli/docker/
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-11 23:06:46.191477 gama_cli-1.7.2/gama_cli/docker/gs/
--rw-rw-r--   0 runner    (1000) runner    (1001)      503 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/docker/gs/docker-compose.dev.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)       73 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/docker/gs/docker-compose.network-host.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      172 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/docker/gs/docker-compose.network-shared.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      640 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/docker/gs/docker-compose.network-vpn.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)       68 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/docker/gs/docker-compose.prod.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      157 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/docker/gs/docker-compose.warthog-combo.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      430 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/docker/gs/docker-compose.yaml
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-11 23:06:46.191477 gama_cli-1.7.2/gama_cli/docker/sim/
--rw-rw-r--   0 runner    (1000) runner    (1001)     1038 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/docker/sim/docker-compose.dev.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      744 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/docker/sim/docker-compose.standalone.yaml
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-11 23:06:46.191477 gama_cli-1.7.2/gama_cli/docker/vessel/
--rw-rw-r--   0 runner    (1000) runner    (1001)     2582 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/docker/vessel/docker-compose.dev.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      193 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/docker/vessel/docker-compose.gpu.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      175 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/docker/vessel/docker-compose.network-host.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      459 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/docker/vessel/docker-compose.network-shared.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      912 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/docker/vessel/docker-compose.network-vpn.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      308 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/docker/vessel/docker-compose.prod.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      723 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/docker/vessel/docker-compose.variant-bravo.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      607 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/docker/vessel/docker-compose.variant-educat.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)     1942 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/docker/vessel/docker-compose.yaml
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-11 23:06:46.191477 gama_cli-1.7.2/gama_cli/groups/
--rw-rw-r--   0 runner    (1000) runner    (1001)        0 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/groups/__init__.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     1061 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/groups/attach.py
--rw-rw-r--   0 runner    (1000) runner    (1001)      445 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/groups/docker.py
--rw-rw-r--   0 runner    (1000) runner    (1001)      353 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/groups/git.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     7231 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/groups/gs.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     2523 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/groups/misc.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     1435 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/groups/setup.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     5830 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/groups/sim.py
--rw-rw-r--   0 runner    (1000) runner    (1001)    14887 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/groups/vessel.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     4959 2023-04-11 23:05:58.000000 gama_cli-1.7.2/gama_cli/helpers.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-11 23:06:46.191477 gama_cli-1.7.2/gama_cli.egg-info/
--rw-rw-r--   0 runner    (1000) runner    (1001)     2302 2023-04-11 23:06:46.000000 gama_cli-1.7.2/gama_cli.egg-info/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)     1701 2023-04-11 23:06:46.000000 gama_cli-1.7.2/gama_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-04-11 23:06:46.000000 gama_cli-1.7.2/gama_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       46 2023-04-11 23:06:46.000000 gama_cli-1.7.2/gama_cli.egg-info/entry_points.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       68 2023-04-11 23:06:46.000000 gama_cli-1.7.2/gama_cli.egg-info/requires.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        9 2023-04-11 23:06:46.000000 gama_cli-1.7.2/gama_cli.egg-info/top_level.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-04-11 23:06:34.000000 gama_cli-1.7.2/gama_cli.egg-info/zip-safe
--rw-rw-r--   0 runner    (1000) runner    (1001)      980 2023-04-11 23:06:46.191477 gama_cli-1.7.2/setup.cfg
--rw-rw-r--   0 runner    (1000) runner    (1001)       38 2023-04-11 23:05:58.000000 gama_cli-1.7.2/setup.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-11 23:30:58.392302 gama_cli-1.7.3/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2302 2023-04-11 23:30:58.392302 gama_cli-1.7.3/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1664 2023-04-11 23:30:08.000000 gama_cli-1.7.3/README.md
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-11 23:30:58.388302 gama_cli-1.7.3/gama_cli/
+-rw-rw-r--   0 runner    (1000) runner    (1001)        0 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/__init__.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-11 23:30:58.388302 gama_cli-1.7.3/gama_cli/assets/
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-11 23:30:58.388302 gama_cli-1.7.3/gama_cli/assets/greenstream/
+-rw-rw-r--   0 runner    (1000) runner    (1001)      173 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/assets/greenstream/config.sim.yml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      597 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/assets/greenstream/config.stubs.yml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      583 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/assets/greenstream/config.variant.bravo.yml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      184 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/assets/greenstream/config.variant.educat.yml
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2539 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/banner.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1231 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/cli.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-11 23:30:58.388302 gama_cli-1.7.3/gama_cli/config/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1417 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/config/gama_gs.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1995 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/config/gama_vessel.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-11 23:30:58.388302 gama_cli-1.7.3/gama_cli/docker/
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-11 23:30:58.392302 gama_cli-1.7.3/gama_cli/docker/gs/
+-rw-rw-r--   0 runner    (1000) runner    (1001)      503 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/docker/gs/docker-compose.dev.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)       73 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/docker/gs/docker-compose.network-host.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      172 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/docker/gs/docker-compose.network-shared.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      640 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/docker/gs/docker-compose.network-vpn.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)       68 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/docker/gs/docker-compose.prod.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      157 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/docker/gs/docker-compose.warthog-combo.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      430 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/docker/gs/docker-compose.yaml
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-11 23:30:58.392302 gama_cli-1.7.3/gama_cli/docker/sim/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1038 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/docker/sim/docker-compose.dev.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      744 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/docker/sim/docker-compose.standalone.yaml
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-11 23:30:58.392302 gama_cli-1.7.3/gama_cli/docker/vessel/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2582 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/docker/vessel/docker-compose.dev.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      193 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/docker/vessel/docker-compose.gpu.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      175 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/docker/vessel/docker-compose.network-host.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      459 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/docker/vessel/docker-compose.network-shared.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      912 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/docker/vessel/docker-compose.network-vpn.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      308 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/docker/vessel/docker-compose.prod.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      723 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/docker/vessel/docker-compose.variant-bravo.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      607 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/docker/vessel/docker-compose.variant-educat.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1942 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/docker/vessel/docker-compose.yaml
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-11 23:30:58.392302 gama_cli-1.7.3/gama_cli/groups/
+-rw-rw-r--   0 runner    (1000) runner    (1001)        0 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/groups/__init__.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1061 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/groups/attach.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      445 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/groups/docker.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      353 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/groups/git.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     7231 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/groups/gs.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2523 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/groups/misc.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1435 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/groups/setup.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     5830 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/groups/sim.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)    14887 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/groups/vessel.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     4959 2023-04-11 23:30:08.000000 gama_cli-1.7.3/gama_cli/helpers.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-11 23:30:58.388302 gama_cli-1.7.3/gama_cli.egg-info/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2302 2023-04-11 23:30:58.000000 gama_cli-1.7.3/gama_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1701 2023-04-11 23:30:58.000000 gama_cli-1.7.3/gama_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-04-11 23:30:58.000000 gama_cli-1.7.3/gama_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       46 2023-04-11 23:30:58.000000 gama_cli-1.7.3/gama_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       68 2023-04-11 23:30:58.000000 gama_cli-1.7.3/gama_cli.egg-info/requires.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        9 2023-04-11 23:30:58.000000 gama_cli-1.7.3/gama_cli.egg-info/top_level.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-04-11 23:30:47.000000 gama_cli-1.7.3/gama_cli.egg-info/zip-safe
+-rw-rw-r--   0 runner    (1000) runner    (1001)      980 2023-04-11 23:30:58.392302 gama_cli-1.7.3/setup.cfg
+-rw-rw-r--   0 runner    (1000) runner    (1001)       38 2023-04-11 23:30:08.000000 gama_cli-1.7.3/setup.py
```

### Comparing `gama_cli-1.7.2/PKG-INFO` & `gama_cli-1.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gama_cli
-Version: 1.7.2
+Version: 1.7.3
 Summary: A CLI for interacting with the GAMA platform
 Home-page: https://github.com/Greenroom-Robotics/gama_cli
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
```

### Comparing `gama_cli-1.7.2/README.md` & `gama_cli-1.7.3/README.md`

 * *Files identical despite different names*

### Comparing `gama_cli-1.7.2/gama_cli/assets/greenstream/config.stubs.yml` & `gama_cli-1.7.3/gama_cli/assets/greenstream/config.stubs.yml`

 * *Files identical despite different names*

### Comparing `gama_cli-1.7.2/gama_cli/assets/greenstream/config.variant.bravo.yml` & `gama_cli-1.7.3/gama_cli/assets/greenstream/config.variant.bravo.yml`

 * *Files identical despite different names*

### Comparing `gama_cli-1.7.2/gama_cli/banner.py` & `gama_cli-1.7.3/gama_cli/banner.py`

 * *Files identical despite different names*

### Comparing `gama_cli-1.7.2/gama_cli/cli.py` & `gama_cli-1.7.3/gama_cli/cli.py`

 * *Files identical despite different names*

### Comparing `gama_cli-1.7.2/gama_cli/config/gama_gs.py` & `gama_cli-1.7.3/gama_cli/config/gama_gs.py`

 * *Files identical despite different names*

### Comparing `gama_cli-1.7.2/gama_cli/config/gama_vessel.py` & `gama_cli-1.7.3/gama_cli/config/gama_vessel.py`

 * *Files identical despite different names*

### Comparing `gama_cli-1.7.2/gama_cli/docker/gs/docker-compose.network-vpn.yaml` & `gama_cli-1.7.3/gama_cli/docker/gs/docker-compose.network-vpn.yaml`

 * *Files identical despite different names*

### Comparing `gama_cli-1.7.2/gama_cli/docker/sim/docker-compose.dev.yaml` & `gama_cli-1.7.3/gama_cli/docker/sim/docker-compose.dev.yaml`

 * *Files identical despite different names*

### Comparing `gama_cli-1.7.2/gama_cli/docker/sim/docker-compose.standalone.yaml` & `gama_cli-1.7.3/gama_cli/docker/sim/docker-compose.standalone.yaml`

 * *Files identical despite different names*

### Comparing `gama_cli-1.7.2/gama_cli/docker/vessel/docker-compose.dev.yaml` & `gama_cli-1.7.3/gama_cli/docker/vessel/docker-compose.dev.yaml`

 * *Files identical despite different names*

### Comparing `gama_cli-1.7.2/gama_cli/docker/vessel/docker-compose.network-vpn.yaml` & `gama_cli-1.7.3/gama_cli/docker/vessel/docker-compose.network-vpn.yaml`

 * *Files identical despite different names*

### Comparing `gama_cli-1.7.2/gama_cli/docker/vessel/docker-compose.variant-bravo.yaml` & `gama_cli-1.7.3/gama_cli/docker/vessel/docker-compose.variant-bravo.yaml`

 * *Files identical despite different names*

### Comparing `gama_cli-1.7.2/gama_cli/docker/vessel/docker-compose.variant-educat.yaml` & `gama_cli-1.7.3/gama_cli/docker/vessel/docker-compose.variant-educat.yaml`

 * *Files identical despite different names*

### Comparing `gama_cli-1.7.2/gama_cli/docker/vessel/docker-compose.yaml` & `gama_cli-1.7.3/gama_cli/docker/vessel/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `gama_cli-1.7.2/gama_cli/groups/attach.py` & `gama_cli-1.7.3/gama_cli/groups/attach.py`

 * *Files identical despite different names*

### Comparing `gama_cli-1.7.2/gama_cli/groups/gs.py` & `gama_cli-1.7.3/gama_cli/groups/gs.py`

 * *Files identical despite different names*

### Comparing `gama_cli-1.7.2/gama_cli/groups/misc.py` & `gama_cli-1.7.3/gama_cli/groups/misc.py`

 * *Files identical despite different names*

### Comparing `gama_cli-1.7.2/gama_cli/groups/setup.py` & `gama_cli-1.7.3/gama_cli/groups/setup.py`

 * *Files identical despite different names*

### Comparing `gama_cli-1.7.2/gama_cli/groups/sim.py` & `gama_cli-1.7.3/gama_cli/groups/sim.py`

 * *Files identical despite different names*

### Comparing `gama_cli-1.7.2/gama_cli/groups/vessel.py` & `gama_cli-1.7.3/gama_cli/groups/vessel.py`

 * *Files identical despite different names*

### Comparing `gama_cli-1.7.2/gama_cli/helpers.py` & `gama_cli-1.7.3/gama_cli/helpers.py`

 * *Files identical despite different names*

### Comparing `gama_cli-1.7.2/gama_cli.egg-info/PKG-INFO` & `gama_cli-1.7.3/gama_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gama-cli
-Version: 1.7.2
+Version: 1.7.3
 Summary: A CLI for interacting with the GAMA platform
 Home-page: https://github.com/Greenroom-Robotics/gama_cli
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
```

### Comparing `gama_cli-1.7.2/gama_cli.egg-info/SOURCES.txt` & `gama_cli-1.7.3/gama_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gama_cli-1.7.2/setup.cfg` & `gama_cli-1.7.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gama_cli
-version = 1.7.2
+version = 1.7.3
 url = https://github.com/Greenroom-Robotics/gama_cli
 author = Greenroom Robotics
 author_email = team@greenroomrobotics.com
 maintainer = David Revay
 maintainer_email = david.revay@greenroomrobotics.com
 classifiers = 
 	Development Status :: 3 - Alpha
```

