# Comparing `tmp/freva_deployment-2303.1.0.tar.gz` & `tmp/freva_deployment-2304.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freva_deployment-2303.1.0.tar", last modified: Fri Mar 10 08:08:49 2023, max compression
+gzip compressed data, was "freva_deployment-2304.0.0.tar", last modified: Wed Apr 12 11:30:35 2023, max compression
```

## Comparing `freva_deployment-2303.1.0.tar` & `freva_deployment-2304.0.0.tar`

### file list

```diff
@@ -1,68 +1,67 @@
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-10 08:08:49.510378 freva_deployment-2303.1.0/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)       15 2022-07-22 12:42:01.000000 freva_deployment-2303.1.0/MANIFEST.in
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)    16402 2023-03-10 08:08:49.510378 freva_deployment-2303.1.0/PKG-INFO
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)    15470 2023-01-31 13:45:59.000000 freva_deployment-2303.1.0/README.md
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-10 08:08:49.507044 freva_deployment-2303.1.0/assets/
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-10 08:08:49.507044 freva_deployment-2303.1.0/assets/config/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)    11564 2022-07-20 13:36:06.000000 freva_deployment-2303.1.0/assets/config/create_tables.sql
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     2578 2023-03-10 07:24:44.000000 freva_deployment-2303.1.0/assets/config/evaluation_system.conf.tmpl
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     8889 2023-03-09 15:11:01.000000 freva_deployment-2303.1.0/assets/config/inventory.toml
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-10 08:08:49.507044 freva_deployment-2303.1.0/assets/db_service/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     1360 2022-07-20 13:36:06.000000 freva_deployment-2303.1.0/assets/db_service/password_rotate.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)      386 2022-07-21 13:16:38.000000 freva_deployment-2303.1.0/assets/db_service/reset_root_pw.sh
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-10 08:08:49.507044 freva_deployment-2303.1.0/assets/playbooks/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     5278 2022-10-11 13:04:53.000000 freva_deployment-2303.1.0/assets/playbooks/core-server-playbook.yml
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     5643 2022-10-11 13:04:53.000000 freva_deployment-2303.1.0/assets/playbooks/db-server-playbook.yml
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     2207 2022-07-20 13:36:06.000000 freva_deployment-2303.1.0/assets/playbooks/server-map-playbook.yml
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     3435 2023-03-07 14:53:50.000000 freva_deployment-2303.1.0/assets/playbooks/solr-server-playbook.yml
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     3263 2022-07-21 14:51:14.000000 freva_deployment-2303.1.0/assets/playbooks/vault-server-playbook.yml
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     7235 2023-03-10 07:56:37.000000 freva_deployment-2303.1.0/assets/playbooks/web-server-playbook.yml
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-10 08:08:49.507044 freva_deployment-2303.1.0/assets/scripts/
--rwxr-xr-x   0 wilfred   (1000) wilfred   (1001)      351 2022-07-20 13:36:06.000000 freva_deployment-2303.1.0/assets/scripts/create_cron.sh
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     2849 2022-07-20 13:36:06.000000 freva_deployment-2303.1.0/assets/scripts/create_systemd.py
--rwxr-xr-x   0 wilfred   (1000) wilfred   (1001)     3293 2022-07-22 05:50:10.000000 freva_deployment-2303.1.0/assets/scripts/docker-or-podman
--rwxr-xr-x   0 wilfred   (1000) wilfred   (1001)       66 2022-07-20 13:36:06.000000 freva_deployment-2303.1.0/assets/scripts/dump_sql
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-10 08:08:49.507044 freva_deployment-2303.1.0/assets/servers/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)      566 2022-10-11 13:04:53.000000 freva_deployment-2303.1.0/assets/servers/Dockerfile
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-10 08:08:49.507044 freva_deployment-2303.1.0/assets/servers/freva/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)      102 2022-07-20 13:36:06.000000 freva_deployment-2303.1.0/assets/servers/freva/servers.toml
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     5857 2022-07-20 13:36:06.000000 freva_deployment-2303.1.0/assets/servers/restservice.py
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-10 08:08:49.507044 freva_deployment-2303.1.0/assets/vault/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)      828 2022-10-11 13:04:53.000000 freva_deployment-2303.1.0/assets/vault/Dockerfile
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     1398 2022-07-20 13:36:06.000000 freva_deployment-2303.1.0/assets/vault/deploy_vault.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)       50 2022-07-20 13:36:06.000000 freva_deployment-2303.1.0/assets/vault/policy-file.hcl
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     4822 2022-07-20 13:36:06.000000 freva_deployment-2303.1.0/assets/vault/runserver.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)      175 2022-07-20 13:36:06.000000 freva_deployment-2303.1.0/assets/vault/vault-server-no-tls.hcl
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)      569 2022-07-20 13:36:06.000000 freva_deployment-2303.1.0/assets/vault/vault-server-tls.hcl
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-10 08:08:49.507044 freva_deployment-2303.1.0/assets/web/
--rwxr-xr-x   0 wilfred   (1000) wilfred   (1001)     2305 2022-07-20 13:36:06.000000 freva_deployment-2303.1.0/assets/web/Dockerfile
--rwxr-xr-x   0 wilfred   (1000) wilfred   (1001)       38 2022-07-20 13:36:06.000000 freva_deployment-2303.1.0/assets/web/docker_cmd.sh
--rwxr-xr-x   0 wilfred   (1000) wilfred   (1001)       17 2022-07-20 13:36:06.000000 freva_deployment-2303.1.0/assets/web/entrypoint.sh
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)    15874 2023-03-09 15:11:01.000000 freva_deployment-2303.1.0/assets/web/freva_web.conf
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)       38 2023-03-10 08:08:49.510378 freva_deployment-2303.1.0/setup.cfg
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     5931 2023-03-10 08:06:49.000000 freva_deployment-2303.1.0/setup.py
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-10 08:08:49.507044 freva_deployment-2303.1.0/src/
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-10 08:08:49.507044 freva_deployment-2303.1.0/src/freva_deployment/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)      221 2023-03-10 08:06:49.000000 freva_deployment-2303.1.0/src/freva_deployment/__init__.py
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-10 08:08:49.507044 freva_deployment-2303.1.0/src/freva_deployment/cli/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)      393 2023-03-10 08:06:49.000000 freva_deployment-2303.1.0/src/freva_deployment/cli/__init__.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     2254 2023-01-25 20:31:07.000000 freva_deployment-2303.1.0/src/freva_deployment/cli/_deploy.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     7594 2023-01-31 13:45:46.000000 freva_deployment-2303.1.0/src/freva_deployment/cli/_migrate.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     3747 2022-09-16 06:49:37.000000 freva_deployment-2303.1.0/src/freva_deployment/cli/_server_map.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     7201 2022-09-14 14:33:49.000000 freva_deployment-2303.1.0/src/freva_deployment/cli/_service.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)    21399 2023-03-09 15:11:01.000000 freva_deployment-2303.1.0/src/freva_deployment/deploy.py
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-10 08:08:49.507044 freva_deployment-2303.1.0/src/freva_deployment/ui/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)        0 2022-07-20 13:36:06.000000 freva_deployment-2303.1.0/src/freva_deployment/ui/__init__.py
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-10 08:08:49.510378 freva_deployment-2303.1.0/src/freva_deployment/ui/deployment_tui/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     1587 2022-11-01 08:06:40.000000 freva_deployment-2303.1.0/src/freva_deployment/ui/deployment_tui/__init__.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     9532 2023-03-09 15:11:01.000000 freva_deployment-2303.1.0/src/freva_deployment/ui/deployment_tui/base.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)    30976 2022-11-01 07:01:36.000000 freva_deployment-2303.1.0/src/freva_deployment/ui/deployment_tui/deploy_forms.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     9525 2023-01-31 13:45:59.000000 freva_deployment-2303.1.0/src/freva_deployment/ui/deployment_tui/main_window.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     9439 2023-03-10 08:06:49.000000 freva_deployment-2303.1.0/src/freva_deployment/utils.py
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-10 08:08:49.507044 freva_deployment-2303.1.0/src/freva_deployment.egg-info/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)    16402 2023-03-10 08:08:49.000000 freva_deployment-2303.1.0/src/freva_deployment.egg-info/PKG-INFO
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     1730 2023-03-10 08:08:49.000000 freva_deployment-2303.1.0/src/freva_deployment.egg-info/SOURCES.txt
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)        1 2023-03-10 08:08:49.000000 freva_deployment-2303.1.0/src/freva_deployment.egg-info/dependency_links.txt
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)      260 2023-03-10 08:08:49.000000 freva_deployment-2303.1.0/src/freva_deployment.egg-info/entry_points.txt
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)      215 2023-03-10 08:08:49.000000 freva_deployment-2303.1.0/src/freva_deployment.egg-info/requires.txt
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)       17 2023-03-10 08:08:49.000000 freva_deployment-2303.1.0/src/freva_deployment.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:35.649448 freva_deployment-2304.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16382 2023-04-12 11:30:35.645448 freva_deployment-2304.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:35.629447 freva_deployment-2304.0.0/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:35.629447 freva_deployment-2304.0.0/assets/config/
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/config/create_tables.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    10288 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/config/inventory.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:35.633447 freva_deployment-2304.0.0/assets/db_service/
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/db_service/password_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/db_service/reset_root_pw.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:35.633447 freva_deployment-2304.0.0/assets/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/playbooks/core-server-playbook.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/playbooks/db-server-playbook.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/playbooks/server-map-playbook.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/playbooks/solr-server-playbook.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/playbooks/vault-server-playbook.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/playbooks/web-server-playbook.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:35.633447 freva_deployment-2304.0.0/assets/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      351 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/scripts/create_cron.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/scripts/create_systemd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3293 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/scripts/docker-or-podman
+-rwxr-xr-x   0 runner    (1001) docker     (123)       66 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/scripts/dump_sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:35.633447 freva_deployment-2304.0.0/assets/servers/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/servers/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:35.633447 freva_deployment-2304.0.0/assets/servers/freva/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/servers/freva/servers.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/servers/restservice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:35.637447 freva_deployment-2304.0.0/assets/vault/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/vault/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/vault/deploy_vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/vault/policy-file.hcl
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/vault/runserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/vault/vault-server-no-tls.hcl
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/vault/vault-server-tls.hcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:35.637447 freva_deployment-2304.0.0/assets/web/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2305 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/web/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/web/docker_cmd.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)       17 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/web/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    15874 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/assets/web/freva_web.conf
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 11:30:35.649448 freva_deployment-2304.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:35.629447 freva_deployment-2304.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:35.641447 freva_deployment-2304.0.0/src/freva_deployment/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/src/freva_deployment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:35.645448 freva_deployment-2304.0.0/src/freva_deployment/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/src/freva_deployment/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/src/freva_deployment/cli/_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/src/freva_deployment/cli/_migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/src/freva_deployment/cli/_server_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/src/freva_deployment/cli/_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21910 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/src/freva_deployment/deploy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:35.645448 freva_deployment-2304.0.0/src/freva_deployment/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/src/freva_deployment/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:35.645448 freva_deployment-2304.0.0/src/freva_deployment/ui/deployment_tui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/src/freva_deployment/ui/deployment_tui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13252 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/src/freva_deployment/ui/deployment_tui/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33551 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/src/freva_deployment/ui/deployment_tui/deploy_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/src/freva_deployment/ui/deployment_tui/main_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11596 2023-04-12 11:30:21.000000 freva_deployment-2304.0.0/src/freva_deployment/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:30:35.641447 freva_deployment-2304.0.0/src/freva_deployment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16382 2023-04-12 11:30:35.000000 freva_deployment-2304.0.0/src/freva_deployment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-12 11:30:35.000000 freva_deployment-2304.0.0/src/freva_deployment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 11:30:35.000000 freva_deployment-2304.0.0/src/freva_deployment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-12 11:30:35.000000 freva_deployment-2304.0.0/src/freva_deployment.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-12 11:30:35.000000 freva_deployment-2304.0.0/src/freva_deployment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-12 11:30:35.000000 freva_deployment-2304.0.0/src/freva_deployment.egg-info/top_level.txt
```

### Comparing `freva_deployment-2303.1.0/PKG-INFO` & `freva_deployment-2304.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: freva_deployment
-Version: 2303.1.0
+Version: 2304.0.0
 Summary: Deploy freva and its services on different machines.
 Home-page: https://github.com/FREVA-CLINT/freva.git
 Author: Martin Bergemann
 Author-email: martin.bergemann@dkrz.de
 Maintainer: Martin Bergemann
 License: GPLv3
 Project-URL: Documentation, https://freva-deployment.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/FREVA-CLINT/freva/issues
 Project-URL: Source, https://github.com/FREVA-CLINT/freva
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
@@ -327,9 +326,7 @@
 git config --global user.name your_user
 git config --global user.email your@email.com
 ```
 
 
 # Advanced: Adjusting the playbook
 Playbook templates and be found the in the `playbooks` directory. You can also add new variables to the playbook if they are present in the `config/inventory` file.
-
-
```

### Comparing `freva_deployment-2303.1.0/README.md` & `freva_deployment-2304.0.0/README.md`

 * *Files identical despite different names*

### Comparing `freva_deployment-2303.1.0/assets/config/create_tables.sql` & `freva_deployment-2304.0.0/assets/config/create_tables.sql`

 * *Files identical despite different names*

### Comparing `freva_deployment-2303.1.0/assets/config/inventory.toml` & `freva_deployment-2304.0.0/assets/config/inventory.toml`

 * *Files 15% similar despite different names*

```diff
@@ -88,14 +88,22 @@
 
 #ansible_python_interpreter="/usr/bin/python3"
 
 ##Indicate whether or not to empty any pre-existing folders/docker volumes.
 ##(Useful for a truely fresh start) (default: False)
 wipe = false
 
+## In case you want to set a custom path to a ansible playbook,
+## you can do this here, by default the deployment will use the playbook
+## located in the user config directory.
+## NOTE: only adjust this if you know what you are doing, if you leave this
+## blank the system will used the default playbook (standard procedure)
+db_playbook = ""
+vault_playbook = ""
+
 [solr.config]
 ## Config variables for the solr service
 port = 8983
 
 # Set the memory for the solr server
 mem = "4g"
 ## Ansible needs a python3 interpreter, which can be set for custom python3 instances
@@ -104,14 +112,21 @@
 
 ## If you need a different user name you can set it here:
 #ansible_user = "username"
 
 ##Indicate whether or not to empty any pre-existing folders/docker volumes.
 ##(Useful for a truely fresh start) (default: False)
 wipe = false
+## In case you want to set a custom path to a ansible playbook,
+## you can do this here, by default the deployment will use the playbook
+## located in the user config directory.
+## NOTE: only adjust this if you know what you are doing, if you leave this
+## blank the system will used the default playbook (standard procedure)
+solr_playbook = ""
+
 
 
 [core.config]
 ## List of user(s) that can alter the configuration of the freva cmd line interface
 ## If blank, the user that runs the deployment is chosen
 admins = ""
 
@@ -170,14 +185,20 @@
 ## you can set the path to the git executable
 #git_path = ""
 
 ##Indicate whether or not to empty any pre-existing folders/docker volumes.
 ##(Useful for a truely fresh start) (default: False)
 wipe = false
 
+## In case you want to set a custom path to a ansible playbook,
+## you can do this here, by default the deployment will use the playbook
+## located in the user config directory.
+## NOTE: only adjust this if you know what you are doing, if you leave this
+## blank the system will used the default playbook (standard procedure)
+core_playbook = ""
 
 [web.config]
 ## List of user that can alter the configuration of freva web
 project_website = "www.freva.dkrz.de"
 
 ## Ansible needs a python3 interpreter, which can be set for custom python3 instances
 #ansible_python_interpreter = ""
@@ -275,7 +296,13 @@
 # Menu entries consist of three entries these are:
 # [Label, url, html_id] -> e.g Plugins, plugins:home, plugin_menu
 menu_entries = [["Data-Browser", "solr:data_browser","browser_menu"],
                 ["Plugins","plugins:home", "plugin_menu"],
                 ["History","history:history","history_menu"],
                 ["Result-Browser", "history:result_browser","result_browser_menu"],
                 ["Help", "plugins:about","doc_menu"]]
+## In case you want to set a custom path to a ansible playbook,
+## you can do this here, by default the deployment will use the playbook
+## located in the user config directory.
+## NOTE: only adjust this if you know what you are doing, if you leave this
+## blank the system will used the default playbook (standard procedure)
+web_playbook = ""
```

### Comparing `freva_deployment-2303.1.0/assets/db_service/password_rotate.py` & `freva_deployment-2304.0.0/assets/db_service/password_rotate.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2303.1.0/assets/playbooks/core-server-playbook.yml` & `freva_deployment-2304.0.0/assets/playbooks/core-server-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2303.1.0/assets/playbooks/db-server-playbook.yml` & `freva_deployment-2304.0.0/assets/playbooks/db-server-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2303.1.0/assets/playbooks/server-map-playbook.yml` & `freva_deployment-2304.0.0/assets/playbooks/server-map-playbook.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ---
 - hosts: freva_map
 
   vars:
-    - docker_cmd: "-v /opt/freva/server-map:/var/freva/:z --name freva-map -p {{ port }}:5008 -t freva-map:latest"
+    - docker_cmd: "-v /opt/freva/server-map:/var/freva/:z --dns 8.8.8.8 --name freva-map -p {{ port }}:5008 -t freva-map:latest"
   tasks:
     - name: Copying docker/podman wrapper script
       copy:
         src: "{{ asset_dir }}/scripts/docker-or-podman"
         dest: /usr/local/bin/docker-or-podman
         mode: "0775"
       become: true
@@ -39,15 +39,17 @@
         dest: /tmp/create_systemd.py
         mode: "0755"
     - name: Copying auxillary files to target machine
       copy: src="{{ asset_dir }}/servers" dest=/tmp
     - name: Building docker images
       shell:
         chdir: /tmp/servers
-        cmd: /usr/local/bin/docker-or-podman build -t freva-map:latest .
+        cmd: >
+          /usr/local/bin/docker-or-podman build
+          -t freva-map:latest .
       become: true
     - name: Creating directory structure
       file:
         path: /opt/freva/server-map
         state: directory
         owner: 9999
         group: 9999
```

### Comparing `freva_deployment-2303.1.0/assets/playbooks/solr-server-playbook.yml` & `freva_deployment-2304.0.0/assets/playbooks/solr-server-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2303.1.0/assets/playbooks/vault-server-playbook.yml` & `freva_deployment-2304.0.0/assets/playbooks/vault-server-playbook.yml`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 - hosts: vault
 
   vars:
     - ansible_python_interpreter: "{{ db_ansible_python_interpreter }}"
     - continer_name: "{{ vault_name }}"
     - docker_cmd: >
         --net {{ project_name }} --cap-add=IPC_LOCK
+        --dns 8.8.8.8
         -v /opt/freva/{{project_name}}/vault_service:/data:z
         -p 5002:5002 --name={{ vault_name }} {{ vault_name }}:latest
   tasks:
     - name: Copying docker/podman wrapper script
       copy:
         src: "{{ asset_dir }}/scripts/docker-or-podman"
         dest: /usr/local/bin/docker-or-podman
```

### Comparing `freva_deployment-2303.1.0/assets/playbooks/web-server-playbook.yml` & `freva_deployment-2304.0.0/assets/playbooks/web-server-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2303.1.0/assets/scripts/create_systemd.py` & `freva_deployment-2304.0.0/assets/scripts/create_systemd.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2303.1.0/assets/scripts/docker-or-podman` & `freva_deployment-2304.0.0/assets/scripts/docker-or-podman`

 * *Files identical despite different names*

### Comparing `freva_deployment-2303.1.0/assets/servers/Dockerfile` & `freva_deployment-2304.0.0/assets/servers/Dockerfile`

 * *Files 12% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 LABEL maintainer="DRKZ-CLINT"
 LABEL repository="https://github.com/FREVA-CLINT/freva.git"
 
 ENV SERVER_FILE="/var/freva/servers.toml"
 COPY restservice.py /usr/local/bin/restservice
 RUN groupadd -g 9999 python
 RUN useradd -ms /bin/bash -d /var/freva python -u 9999 -g 9999
-RUN python3 -m ensurepip && echo "nameserver 8.8.8.8" >> /etc/resolv.conf &&\
+RUN python3 -m ensurepip &&\
     chmod +x /usr/local/bin/restservice &&\
     pip3 install --no-cache --upgrade pip setuptools toml requests flask flask_restful
 USER python
 VOLUME /var/freva/
 CMD ["/usr/local/bin/restservice"]
```

### Comparing `freva_deployment-2303.1.0/assets/servers/restservice.py` & `freva_deployment-2304.0.0/assets/servers/restservice.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2303.1.0/assets/vault/deploy_vault.py` & `freva_deployment-2304.0.0/assets/vault/deploy_vault.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2303.1.0/assets/vault/runserver.py` & `freva_deployment-2304.0.0/assets/vault/runserver.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2303.1.0/assets/vault/vault-server-tls.hcl` & `freva_deployment-2304.0.0/assets/vault/vault-server-tls.hcl`

 * *Files identical despite different names*

### Comparing `freva_deployment-2303.1.0/assets/web/Dockerfile` & `freva_deployment-2304.0.0/assets/web/Dockerfile`

 * *Files identical despite different names*

### Comparing `freva_deployment-2303.1.0/assets/web/freva_web.conf` & `freva_deployment-2304.0.0/assets/web/freva_web.conf`

 * *Files identical despite different names*

### Comparing `freva_deployment-2303.1.0/setup.py` & `freva_deployment-2304.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,34 +105,26 @@
     with THIS_DIR.joinpath(*parts).open() as f:
         return f.read()
 
 
 def get_packages() -> List[str]:
     """Get the packages needed to install."""
     plf = sys.platform
-    if (
-        plf.startswith("win")
-        or plf.startswith("cygwin")
-        or plf.startswith("ms")
-    ):
+    if plf.startswith("win") or plf.startswith("cygwin") or plf.startswith("ms"):
         return INSTALL_REQUIRES
     INSTALL_REQUIRES.append("ansible")
     return INSTALL_REQUIRES
 
 
 def get_data_files() -> List[Tuple[str, List[str]]]:
     dirs = [d for d in ASSET_DIR.rglob("*") if d.is_dir()]
     data_files = []
     for d in dirs:
-        target_dir = (
-            Path("share") / "freva" / "deployment" / d.relative_to(ASSET_DIR)
-        )
-        add_files = [
-            str(f.relative_to(THIS_DIR)) for f in d.rglob("*") if f.is_file()
-        ]
+        target_dir = Path("share") / "freva" / "deployment" / d.relative_to(ASSET_DIR)
+        add_files = [str(f.relative_to(THIS_DIR)) for f in d.rglob("*") if f.is_file()]
         if add_files:
             data_files.append((str(target_dir), add_files))
     return data_files
 
 
 setup(
     name="freva_deployment",
@@ -167,14 +159,15 @@
             "deploy-freva = freva_deployment.ui.deployment_tui:tui",
         ]
     },
     setup_requires=["appdirs"],
     install_requires=get_packages(),
     extras_require={
         "docs": [
+            "furo",
             "sphinx",
             "nbsphinx",
             "recommonmark",
             "sphinx_rtd_theme",
             "ipython",  # For nbsphinx syntax highlighting
             "sphinxcontrib_github_alt",
         ],
```

### Comparing `freva_deployment-2303.1.0/src/freva_deployment/cli/_deploy.py` & `freva_deployment-2304.0.0/src/freva_deployment/cli/_deploy.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2303.1.0/src/freva_deployment/cli/_migrate.py` & `freva_deployment-2304.0.0/src/freva_deployment/cli/_migrate.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2303.1.0/src/freva_deployment/cli/_server_map.py` & `freva_deployment-2304.0.0/src/freva_deployment/cli/_server_map.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2303.1.0/src/freva_deployment/cli/_service.py` & `freva_deployment-2304.0.0/src/freva_deployment/cli/_service.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2303.1.0/src/freva_deployment/deploy.py` & `freva_deployment-2304.0.0/src/freva_deployment/deploy.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,21 @@
 from subprocess import run
 import sys
 from urllib.parse import urlparse
 from tempfile import TemporaryDirectory, mkdtemp
 from typing import Any
 
 from numpy import sign
-import toml
+import tomlkit
 import yaml
 
 from .utils import (
     asset_dir,
     config_dir,
+    load_config,
     get_passwd,
     get_email_credentials,
     logger,
     upload_server_map,
     RichConsole,
 )
 
@@ -65,14 +66,15 @@
         self.apache_config: Path = Path(self._td.name) / "freva_web.conf"
         self._db_pass: str = ""
         self._steps = steps or ["services", "core", "web"]
         self._inv_tmpl = Path(config_file or config_dir / "inventory.toml")
         self._cfg_tmpl = self.aux_dir / "evaluation_system.conf.tmpl"
         self.cfg = self._read_cfg()
         self.project_name = self.cfg.pop("project_name", None)
+        self.playbooks: dict[str, Path | None] = {}
         if not self.project_name:
             raise ValueError("You must set a project name")
 
     @property
     def public_key_file(self) -> str:
         """Path to the public certificate file."""
         public_keyfile = self.cfg["certificates"].get("public_keyfile")
@@ -99,14 +101,15 @@
             return str(Path(keyfile).expanduser().absolute())
         return ""
 
     def _prep_vault(self) -> None:
         """Prepare the vault."""
         self._config_keys.append("vault")
         self.cfg["vault"] = self.cfg["db"].copy()
+        self.playbooks["vault"] = self.cfg["db"]["config"].get("vault_playbook")
         if not self.master_pass:
             self.master_pass = get_passwd()
         self.cfg["vault"]["config"]["root_passwd"] = self.master_pass
         self.cfg["vault"]["config"]["passwd"] = self.db_pass
         self.cfg["vault"]["config"]["keyfile"] = self.public_key_file
         self.cfg["vault"]["config"]["email"] = self.cfg["web"]["config"].get(
             "contacts", ""
@@ -126,31 +129,34 @@
         db_host = self.cfg["db"]["config"].get("host", "")
         if not db_host:
             self.cfg["db"]["config"]["host"] = host
         self.cfg["db"]["config"].setdefault("port", "3306")
         self.cfg["db"]["config"]["email"] = self.cfg["web"]["config"].get(
             "contacts", ""
         )
+        self.playbooks["db"] = self.cfg["db"]["config"].get("db_playbook")
         self._prep_vault()
 
     def _prep_solr(self) -> None:
         """prepare the apache solr service."""
         self._config_keys.append("solr")
         self.cfg["solr"]["config"].pop("core", None)
+        self.playbooks["solr"] = self.cfg["solr"]["config"].get("solr_playbook")
         for key, default in dict(mem="4g", port=8983).items():
             self.cfg["solr"]["config"][key] = (
                 self.cfg["solr"]["config"].get(key) or default
             )
         self.cfg["solr"]["config"]["email"] = self.cfg["web"]["config"].get(
             "contacts", ""
         )
 
     def _prep_core(self) -> None:
         """prepare the core deployment."""
         self._config_keys.append("core")
+        self.playbooks["core"] = self.cfg["core"]["config"].get("core_playbook")
         self.cfg["core"]["config"]["admins"] = (
             self.cfg["core"]["config"].get("admins") or getuser()
         )
         if not self.cfg["core"]["config"]["admins"]:
             self.cfg["core"]["config"]["admins"] = getuser()
         install_dir = self.cfg["core"]["config"]["install_dir"]
         root_dir = self.cfg["core"]["config"].get("root_dir", "")
@@ -179,14 +185,15 @@
         self.cfg["core"]["config"][
             "git_url"
         ] = "https://github.com/FREVA-CLINT/freva.git"
 
     def _prep_web(self) -> None:
         """prepare the web deployment."""
         self._config_keys.append("web")
+        self.playbooks["web"] = self.cfg["web"]["config"].get("web_playbook")
         self._prep_core()
         admin = self.cfg["core"]["config"]["admins"]
         if not isinstance(admin, str):
             self.cfg["web"]["config"]["admin"] = admin[0]
         else:
             self.cfg["web"]["config"]["admin"] = admin
         _webserver_items = {}
@@ -238,15 +245,15 @@
         except (FileNotFoundError, IOError, KeyError):
             pass
         try:
             _webserver_items["IMPRINT"] = _webserver_items["IMPRINT"].split(",")
         except AttributeError:
             pass
         with self.web_conf_file.open("w") as f_obj:
-            toml.dump(_webserver_items, f_obj)
+            tomlkit.dump(_webserver_items, f_obj)
         for key in ("core", "web"):
             self.cfg[key]["config"]["config_toml_file"] = str(self.web_conf_file)
         if not self.master_pass:
             self.master_pass = get_passwd()
         email_user, self.email_password = get_email_credentials()
         self._prep_vault()
         self.cfg["vault"]["config"]["ansible_python_interpreter"] = self.cfg["db"][
@@ -277,16 +284,15 @@
         return self
 
     def __exit__(self, *args):
         self._td.cleanup()
 
     def _read_cfg(self) -> dict[str, Any]:
         try:
-            with self._inv_tmpl.open() as f_obj:
-                return dict(toml.load(f_obj))
+            return dict(load_config(self._inv_tmpl))
         except FileNotFoundError as error:
             raise FileNotFoundError(f"No such file {self._inv_tmpl}") from error
 
     def _check_config(self) -> None:
         sections = []
         for section in self.cfg.keys():
             for step in self._config_keys:
@@ -417,16 +423,19 @@
 
     def create_playbooks(self):
         """Create the ansible playbook form all steps."""
         logger.info("Creating Ansible playbooks")
         playbook = []
         for step in self.steps:
             getattr(self, f"_prep_{step}")()
-            playbook_file = self.playbook_dir / f"{step}-server-playbook.yml"
-            with playbook_file.open() as f_obj:
+            playbook_file = (
+                self.playbooks.get(step)
+                or self.playbook_dir / f"{step}-server-playbook.yml"
+            )
+            with Path(playbook_file).open() as f_obj:
                 playbook += yaml.safe_load(f_obj)
         with self._playbook_file.open("w") as f_obj:
             yaml.dump(playbook, f_obj)
 
     def create_eval_config(self) -> None:
         """Create and dump the evaluation_systme.config."""
         logger.info("Creating evaluation_system.conf")
```

### Comparing `freva_deployment-2303.1.0/src/freva_deployment/ui/deployment_tui/__init__.py` & `freva_deployment-2304.0.0/src/freva_deployment/ui/deployment_tui/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,19 +34,22 @@
     set_log_level(verbosity)
     try:
         main_app = MainApp()
         main_app.run()
     except KeyboardInterrupt:
         try:
             main_app.thread_stop.set()
-            main_app.save_config_to_file()
+            main_app.save_config_to_file(
+                save_file=main_app._setup_form.inventory_file.value
+            )
         except AttributeError:
             pass
         return
     setup = main_app.setup
+    main_app.thread_stop.set()
     if setup:
         server_map = setup.pop("server_map")
         ask_pass = setup.pop("ask_pass")
         steps = ", ".join(setup["steps"])
         RichConsole.print(f"Playing steps: [i]{steps}[/] with ansible")
         with DeployFactory(**setup) as DF:
             DF.play(server_map, ask_pass, verbosity)
```

### Comparing `freva_deployment-2303.1.0/src/freva_deployment/ui/deployment_tui/base.py` & `freva_deployment-2304.0.0/src/freva_deployment/ui/deployment_tui/main_window.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,253 +1,261 @@
+"""The Freva deployment Text User Interface (TUI) helps to configure a
+deployment setup for a new instance of freva."""
 from __future__ import annotations
-import os
+import json
 from pathlib import Path
-import logging
+import time
+import threading
+from typing import Any, Dict, List, cast
 
-import curses
+import appdirs
 import npyscreen
+import tomlkit
 
+from freva_deployment.utils import asset_dir, config_dir
+from .base import selectFile, BaseForm, VarForm
+from .deploy_forms import WebScreen, DBScreen, SolrScreen, CoreScreen, RunForm
 
-logging.basicConfig(level=logging.DEBUG)
-logger: logging.Logger = logging.getLogger("deploy-freva-tui")
 
+class MainApp(npyscreen.NPSAppManaged):
+    config: dict[str, Any] = dict()
 
-class FileSelector(npyscreen.FileSelector):
-    """FileSelector widget that allows for filtering file extensions."""
+    @property
+    def steps(self) -> list[str]:
+        """Get the deploy steps."""
+        steps = []
+        for step, form_obj in self._forms.items():
+            if form_obj.use.value and step not in steps:
+                steps.append(step)
+        return steps
+
+    def onStart(self) -> None:
+        """When Application starts, set up the Forms that will be used."""
+        npyscreen.setTheme(npyscreen.Themes.ElegantTheme)
+        self.cache_dir.mkdir(exist_ok=True, parents=True)
+        self.setup: dict[str, Any] = {}
+        self._forms: dict[str, BaseForm] = {}
+        self.current_form = "core"
+        self.init()
+        self.thread_stop = threading.Event()
+        # self.start_auto_save()
+
+    def init(self) -> None:
+        self._steps_lookup = {
+            "core": "MAIN",
+            "web": "SECOND",
+            "solr": "FOURTH",
+            "db": "THIRD",
+        }
+        self.config = cast(Dict[str, Any], self._read_cache("config", {}))
+        for step in self._steps_lookup.keys():
+            self.config.setdefault(step, {"hosts": "", "config": {}})
+        self._add_froms()
+
+    def reset(self) -> None:
+        npyscreen.blank_terminal()
+        self.init()
+
+    def start_auto_save(self) -> None:
+        """(Re)-Start the auto save thread."""
+        self._save_thread = threading.Thread(target=self._auto_save)
+        self._save_thread.daemon = True
+        self._save_thread.start()
+
+    def _add_froms(self) -> None:
+        """Add forms to edit the deploy steps to the main window."""
+        self._forms["core"] = self.addForm(
+            "MAIN",
+            CoreScreen,
+            name="Core deployment",
+        )
+        self._forms["web"] = self.addForm("SECOND", WebScreen, name="Web deployment")
+        self._forms["db"] = self.addForm("THIRD", DBScreen, name="Database deployment")
+        self._forms["solr"] = self.addForm("FOURTH", SolrScreen, name="Solr deployment")
+        self._setup_form = self.addForm("SETUP", RunForm, name="Apply the Deployment")
+
+    def exit_application(self, *args, **kwargs) -> None:
+        value = npyscreen.notify_ok_cancel(
+            kwargs.get("msg", "Exit Application?"), title=""
+        )
+        if value is True:
+            self.thread_stop.set()
+            self.setNextForm(None)
+            self.save_config_to_file(save_file=kwargs.get("save_file"))
+            self.editing = False
+            self.switchFormNow()
+
+    def change_form(self, name: str) -> None:
+        # Switch forms.  NB. Do *not* call the .edit() method directly (which
+        # would lead to a memory leak and ultimately a recursion error).
+        # Instead, use the method .switchForm to change forms.
+        self.switchForm(name)
+
+        # By default the application keeps track of every form visited.
+        # There's no harm in this, but we don't need it so:
+        self.resetHistory()
+
+    def check_missing_config(self, stop_at_missing: bool = True) -> str | None:
+        """Evaluate all forms."""
+        for step, form_obj in self._forms.items():
+            cfg = form_obj.check_config(notify=stop_at_missing)
+            if cfg is None and stop_at_missing:
+                return self._steps_lookup[step]
+            self.config[step] = cfg
+        return None
+
+    def _auto_save(self) -> None:
+        """Auto save the current configuration."""
+        while not self.thread_stop.is_set():
+            time.sleep(0.5)
+            if self.thread_stop.is_set():
+                break
+            try:
+                self.check_missing_config(stop_at_missing=False)
+                self.save_config_to_file()
+            except Exception:
+                pass
+
+    def save_dialog(self, *args, **kwargs) -> None:
+        """Create a dialoge that allows for saving the config file."""
+
+        the_selected_file = selectFile(
+            select_dir=False, must_exist=False, file_extentions=[".toml"]
+        )
+        if the_selected_file:
+            the_selected_file = Path(the_selected_file).with_suffix(".toml")
+            the_selected_file = str(the_selected_file.expanduser().absolute())
+            self.check_missing_config(stop_at_missing=False)
+            self._setup_form.inventory_file.value = the_selected_file
+            self.save_config_to_file(write_toml_file=True)
+
+    def _update_config(self, config_file: Path | str) -> None:
+        """Update the main window after a new configuration has been loaded."""
 
-    file_extentions: list[str]
-    """List of allowed file extensions."""
-    value: str
-    """The value of this file selector."""
-
-    def __init__(
-        self, *args, file_extentions: str | list[str] = [".toml"], **kwargs
-    ) -> None:
-        if isinstance(file_extentions, str):
-            self.file_extentions = [file_extentions]
-        else:
-            self.file_extentions = file_extentions
-        super().__init__(*args, **kwargs)
-        self.how_exited_handers[npyscreen.wgwidget.EXITED_ESCAPE] = self.exit
-
-    def exit(self) -> None:
-        """Exit the dialogue."""
-        self.wCommand.value = ""
-        self.value = ""
-        self.exit_editing()
-
-    def update_grid(self) -> None:
-        if self.value:
-            self.value = os.path.expanduser(self.value)
-        if not os.path.exists(self.value):
-            self.value = os.getcwd()
-        if os.path.isdir(self.value):
-            working_dir = Path(self.value)
-        else:
-            working_dir = Path(self.value).parent
-        self.wStatus1.value = working_dir
-        file_list, dir_list = [], []
-        if working_dir.parent != working_dir:
-            dir_list.append("..")
         try:
-            for fn in working_dir.glob("*"):
-                rel_path = str(fn.relative_to(working_dir))
-                if not rel_path.startswith("."):
-                    if fn.is_dir():
-                        dir_list.append(str(fn) + os.sep)
-                    elif fn.suffix in self.file_extentions:
-                        file_list.append(str(fn))
-        except OSError:
-            npyscreen.notify_wait(
-                title="Error", message="Could not read specified directory."
-            )
-        # DOES NOT CURRENTLY WORK - EXCEPT FOR THE WORKING DIRECTORY.  REFACTOR.
-        # sort Filelist
-        file_list.sort(key=str.casefold)
-        dir_list.sort(key=str.casefold)
-        if self.sort_by_extension:
-            file_list.sort(key=self.get_extension)
-        self.wMain.set_grid_values_from_flat_list(
-            dir_list + file_list, reset_cursor=False
+            with open(config_file) as f:
+                self.config = tomlkit.load(f)
+        except Exception:
+            return
+        self.resetHistory()
+        self.editing = True
+        self.switchFormNow()
+        self._add_froms()
+        self._setup_form.inventory_file.value = config_file
+
+    def load_dialog(self, *args, **kwargs) -> None:
+        """Create a dialoge that allows for loading a config file."""
+
+        the_selected_file = selectFile(
+            select_dir=False, must_exist=True, file_extentions=[".toml"]
         )
-        self.display()
+        if the_selected_file:
+            self._update_config(the_selected_file)
+            self.save_config_to_file()
 
+    def save_config_to_file(self, **kwargs) -> Path | None:
+        """Save the status of the tui to file."""
+        try:
+            return self._save_config_to_file(**kwargs)
+        except Exception as error:
+            npyscreen.notify_confirm(
+                title="Error",
+                message=f"Couldn't save config:\n{error}",
+            )
+        return None
 
-def selectFile(starting_value: str = "", *args, **keywords):
-    F = FileSelector(*args, **keywords)
-    F.set_colors()
-    F.wCommand.show_bold = True
-    if starting_value:
-        if not os.path.exists(os.path.abspath(os.path.expanduser(starting_value))):
-            F.value = os.getcwd()
-        else:
-            F.value = starting_value
-            F.wCommand.value = starting_value
-    else:
-        F.value = os.getcwd()
-    F.update_grid()
-    F.edit()
-    return F.wCommand.value
-
-
-class BaseForm(npyscreen.FormMultiPageWithMenus, npyscreen.FormWithMenus):
-    """Base class for forms."""
-
-    _num: int = 0
-    input_fields: dict[str, tuple[npyscreen.TitleText, bool]] = {}
-    """Dictionary of input fileds: the key of the dictionary represents the name
-       of the key in the in config toml input files. Values represent a tuple of
-       npysceen types that display the input information on this key to the
-       user and a boolean indicating whether or not this variable is mandatory.
-    """
-    certificates: list[str] = []
-    """The type of certificate files this step needs."""
+    def get_save_file(self, save_file: Path | None = None) -> str:
+        """Get the name of the file where the config should be stored to."""
+        cache_file = self.cache_dir / ".temp_file.toml"
+        if save_file:
+            save_file = Path(save_file).expanduser().absolute()
+        return str(save_file or cache_file)
 
-    def get_config(self, key) -> dict[str, str | bool | list[str]]:
-        """Read the configuration for a step."""
+    def _save_config_to_file(
+        self,
+        write_toml_file: bool = False,
+        save_file: Path | None = None,
+    ) -> Path | None:
+        cert_files = dict(
+            public_keyfile=self._setup_form.public_keyfile.value or "",
+            private_keyfile=self._setup_form.private_keyfile.value or "",
+            chain_keyfile=self._setup_form.chain_keyfile.value or "",
+        )
+        for key, value in cert_files.items():
+            if value and "cfd" not in value.lower():
+                cert_files[key] = str(Path(value).expanduser().absolute())
+        project_name = self._setup_form.project_name.value
+        server_map = self._setup_form.server_map.value
+        ssh_pw = self._setup_form.use_ssh_pw.value
+        if isinstance(ssh_pw, list):
+            ssh_pw = bool(ssh_pw[0])
+        self.config["certificates"] = cert_files
+        self.config["project_name"] = project_name or ""
+        config = {
+            "save_file": self.get_save_file(save_file),
+            "steps": self.steps,
+            "ssh_pw": ssh_pw,
+            "server_map": server_map,
+            "config": self.config,
+        }
+        with open(self.cache_dir / "freva_deployment.json", "w") as f:
+            json.dump({k: v for (k, v) in config.items()}, f, indent=3)
+        if write_toml_file is False:
+            return None
         try:
-            cfg = self.parentApp.config[key].copy()
-            if not isinstance(cfg, dict):
-                cfg = {"config": {}}
-        except (KeyError, AttributeError, TypeError):
-            cfg = {"config": {}}
-        cfg.setdefault("config", {})
-        for k, values in cfg["config"].items():
-            if values is None:
-                cfg["config"][k] = ""
-        return cfg["config"]
+            with open(asset_dir / "config" / "inventory.toml") as f:
+                config_tmpl = cast(Dict[str, Any], tomlkit.load(f))
+        except Exception:
+            config_tmpl = self.config
+        config_tmpl["certificates"] = cert_files
+        config_tmpl["project_name"] = project_name
+        for step, settings in self.config.items():
+            if step in ("certificates", "project_name"):
+                continue
+            config_tmpl[step]["hosts"] = settings["hosts"]
+            for key, config in settings["config"].items():
+                config_tmpl[step]["config"][key] = config
+        Path(self.save_file).parent.mkdir(exist_ok=True, parents=True)
+        with open(self.save_file, "w") as f:
+            toml_string = tomlkit.dumps(config_tmpl)
+            f.write(toml_string)
+        return Path(self.save_file)
 
-    def get_host(self, key) -> str:
-        """Read the host name(s) from the main windows config."""
+    @property
+    def cache_dir(self) -> Path:
+        """The user cachedir."""
+        return Path(appdirs.user_cache_dir()) / "freva-deployment"
+
+    def _read_cache(
+        self, key: str, default: str | list | bool | dict[str, str] = ""
+    ) -> str | bool | list | dict[str, str]:
         try:
-            host = self.parentApp.config[key]["hosts"]
-        except (TypeError, KeyError):
-            return ""
-        if isinstance(host, str):
-            host = [v.strip() for v in host.split(",") if v.strip()]
-        return ",".join(host)
+            with open(self.cache_dir / "freva_deployment.json", "r") as f:
+                return json.load(f).get(key, default)
+        except (FileNotFoundError, json.decoder.JSONDecodeError):
+            return default
 
     @property
-    def num(self) -> str:
-        """Calculate the number for enumerations of any input field."""
-        self._num += 1
-        return f"{self._num}. "
+    def _steps(self) -> list[str]:
+        """Read the deployment-steps from the cache."""
+        return cast(List[str], self._read_cache("steps", ["core", "web", "db", "solr"]))
+
+    def read_cert_file(self, key: str) -> str:
+        """Read the certificate file from the cache."""
+        cert_file = cast(str, self.config.get("certificates", {}).get(key, ""))
+        if cert_file:
+            return cert_file
+        return cast(str, self._read_cache(key, ""))
 
-    def check_config(
-        self,
-        notify: bool = True,
-    ) -> dict[str, str | dict[str, str | list | int | bool | None]] | None:
-        """Check if the from entries are valid."""
-        config = {}
-        for key, (obj, mandatory) in self.input_fields.items():
-            try:
-                value = obj.values[obj.value]
-            except AttributeError:
-                value = obj.value
-            if isinstance(value, str):
-                if not value and self.use.value and mandatory and notify:
-                    msg = f"MISSING ENTRY FOR {self.step}: {obj.name}"
-                    npyscreen.notify_confirm(msg, title="ERROR")
-                    return None
-                elif not value and not mandatory:
-                    continue
-            config[key] = value
-        cfg = dict(hosts=config.pop("hosts"))
-        cfg["config"] = config
-        for key, value in cfg["config"].items():
-            if key in self.list_keys:
-                cfg["config"][key] = value.split(",")
-        return cfg
-
-    def draw_form(self) -> None:
-        """Overload the draw_from method from, this is done to add menus."""
-        super().draw_form()
-        menus = [
-            " " + self.__class__.MENU_KEY + ":Main Menu ",
-            "^K:Prev. Tab ",
-            "^L:Next Tab ",
-            "^R:Run ",
-            "^S:Save ",
-            "^O:Load ",
-            "^E:Exit ",
-        ]
-        y, x = self.display_menu_advert_at()
-        for n, menu_advert in enumerate(menus):
-            if isinstance(menu_advert, bytes):
-                menu_advert = menu_advert.decode("utf-8", "replace")
-            X = sum([len(menu) for menu in menus[:n]]) + x
-            self.add_line(
-                y,
-                X,
-                menu_advert,
-                self.make_attributes_list(menu_advert, curses.A_NORMAL),
-                self.columns - X - 1,
-            )
+    @property
+    def save_file(self) -> str:
+        """Read the file that stores the configuration from the cache."""
+        fall_back = config_dir / "inventory.toml"
+        return cast(str, self._read_cache("save_file", str(fall_back)))
 
-    def previews_form(self, *args, **keywords) -> None:
-        return self.change_forms(*args, reverse=True, **keywords)
 
-    def change_forms(self, *args, reverse=False, **keywords) -> None:
-        """Cycle between the deployment config forms."""
-        for step in self.parentApp._steps_lookup.keys():
-            if self.name.lower().startswith(step):
-                name = step
-                break
-            elif self.name.lower().startswith("database"):
-                name = "db"
-                break
-        keys = self.parentApp._steps_lookup.keys()
-        steps = list(self.parentApp._steps_lookup.values())
-        if reverse:
-            change_to = dict(zip(keys, [steps[-1]] + steps[:-1]))
-        else:
-            change_to = dict(zip(keys, steps[1:] + [steps[0]]))
-        # raise ValueError(change_to, reverse, self.parentApp._steps_lookup)
-        self.parentApp.current_form = name
-        self.parentApp.change_form(change_to[name])
-
-    def run_deployment(self, *args) -> None:
-        """Switch to the deployment setup form."""
-        self.parentApp.current_form = self.name
-        self.parentApp.change_form("SETUP")
-
-    def create(self) -> None:
-        """Setup the form."""
-        self.how_exited_handers[
-            npyscreen.wgwidget.EXITED_ESCAPE
-        ] = self.parentApp.exit_application
-        self.add_handlers({"^O": self.parentApp.load_dialog})
-        self.add_handlers({"^S": self.parentApp.save_dialog})
-        self.add_handlers({"^K": self.previews_form})
-        self.add_handlers({"^L": self.change_forms})
-        self.add_handlers({"^R": self.run_deployment})
-        self.add_handlers({"^E": self.parentApp.exit_application})
-        # The menus are created here.
-        self.menu = self.add_menu(name="Main Menu", shortcut="^M")
-        self.submenu = self.menu.addNewSubmenu("Deployment Menu", "^D")
-        self._change_form = self.parentApp.change_form
-        self.menu.addItemsFromList(
-            [
-                ("Save Config", self.parentApp.save_dialog, "^S"),
-                ("Load Config", self.parentApp.load_dialog, "^L"),
-                ("Run Deployment", self.run_deployment, "^R"),
-                ("Exit Application", self.parentApp.exit_application, "^E"),
-            ]
-        )
-        self.submenu.addItemsFromList(
-            [
-                ("Core Deployment", self._change_form, "c", "c", ("MAIN",)),
-                ("Web Deployment", self._change_form, "w", "w", ("SECOND",)),
-                ("DB Deployment", self._change_form, "d", "d", ("THIRD",)),
-                ("Solr Deployment", self._change_form, "s", "s", ("FOURTH",)),
-                ("Run Deployment", self.run_deployment, "^R"),
-            ]
-        )
-        self.use = self.add(
-            npyscreen.CheckBox,
-            max_height=2,
-            value=self.step in self.parentApp._steps,
-            editable=True,
-            name="Check to set up the {}".format(self.step),
-            scroll_exit=True,
-        )
-        self._add_widgets()
+if __name__ == "__main__":
+    try:
+        main_app = MainApp()
+        main_app.run()
+    except KeyboardInterrupt:
+        pass
```

### Comparing `freva_deployment-2303.1.0/src/freva_deployment/ui/deployment_tui/deploy_forms.py` & `freva_deployment-2304.0.0/src/freva_deployment/ui/deployment_tui/deploy_forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from getpass import getuser
 import npyscreen
 from pathlib import Path
 from typing import cast, List, Dict
 
 from .base import BaseForm, logger
 from freva_deployment import AVAILABLE_PYTHON_VERSIONS, AVAILABLE_CONDA_ARCHS
+from freva_deployment.utils import get_current_file_dir
 
 
 def get_index(values: list[str], target: str, default: int = 0) -> int:
     """Get the target index of item in list.
 
     Parameters:
     ===========
@@ -181,14 +182,27 @@
                         "the backend will be installed:"
                     ),
                     value=arch_idx,
                     values=AVAILABLE_CONDA_ARCHS,
                 ),
                 True,
             ),
+            core_playbook=(
+                self.add_widget_intelligent(
+                    npyscreen.TitleFilename,
+                    name=(
+                        f"{self.num}Set the path to the playbook used for"
+                        " setting up the system."
+                    ),
+                    value=cfg.get(
+                        "core_playbook",
+                    ),
+                ),
+                False,
+            ),
             ansible_python_interpreter=(
                 self.add_widget_intelligent(
                     npyscreen.TitleFilename,
                     name=f"{self.num}Python path on remote machine:",
                     value=cfg.get("ansible_python_interpreter", "/usr/bin/python3"),
                 ),
                 False,
@@ -477,15 +491,15 @@
                 False,
             ),
             ldap_email_field=(
                 self.add_widget_intelligent(
                     npyscreen.TitleText,
                     name=(f"{self.num}Ldap search search key for email addr"),
                     value=cfg.get(
-                        "ldap_email_field",
+                        "ldap_email_name_field",
                         "mail",
                     ),
                 ),
                 False,
             ),
             ldap_group_class=(
                 self.add_widget_intelligent(
@@ -514,14 +528,27 @@
                 self.add_widget_intelligent(
                     npyscreen.TitleText,
                     name=(f"{self.num}Ldap tools class to be used for authentication."),
                     value=cfg.get("ldap_model", "MiklipUserInformation"),
                 ),
                 True,
             ),
+            web_playbook=(
+                self.add_widget_intelligent(
+                    npyscreen.TitleFilename,
+                    name=(
+                        f"{self.num}Set the path to the playbook used for"
+                        " setting up the system."
+                    ),
+                    value=cfg.get(
+                        "web_playbook",
+                    ),
+                ),
+                False,
+            ),
             ansible_python_interpreter=(
                 self.add_widget_intelligent(
                     npyscreen.TitleFilename,
                     name=f"{self.num}Pythonpath on remote machine:",
                     value=cfg.get("ansible_python_interpreter", "/usr/bin/python3"),
                 ),
                 False,
@@ -593,14 +620,40 @@
                     npyscreen.TitleCombo,
                     name=f"{self.num}Database Port:",
                     value=port_idx,
                     values=db_ports,
                 ),
                 True,
             ),
+            db_playbook=(
+                self.add_widget_intelligent(
+                    npyscreen.TitleFilename,
+                    name=(
+                        f"{self.num}Set the path to the db playbook used for"
+                        " setting up the system."
+                    ),
+                    value=cfg.get(
+                        "db_playbook",
+                    ),
+                ),
+                False,
+            ),
+            vault_playbook=(
+                self.add_widget_intelligent(
+                    npyscreen.TitleFilename,
+                    name=(
+                        f"{self.num}Set the path to the vault playbook used for"
+                        " setting up the system."
+                    ),
+                    value=cfg.get(
+                        "vault_playbook",
+                    ),
+                ),
+                False,
+            ),
             ansible_python_interpreter=(
                 self.add_widget_intelligent(
                     npyscreen.TitleFilename,
                     name=f"{self.num}Pythonpath on remote machine:",
                     value=cfg.get("ansible_python_interpreter", "/usr/bin/python3"),
                 ),
                 False,
@@ -663,14 +716,27 @@
                     npyscreen.TitleCombo,
                     name=f"{self.num}Solr port:",
                     value=port_idx,
                     values=solr_ports,
                 ),
                 True,
             ),
+            solr_playbook=(
+                self.add_widget_intelligent(
+                    npyscreen.TitleFilename,
+                    name=(
+                        f"{self.num}Set the path to the playbook used for"
+                        " setting up the system."
+                    ),
+                    value=cfg.get(
+                        "solr_playbook",
+                    ),
+                ),
+                False,
+            ),
             ansible_python_interpreter=(
                 self.add_widget_intelligent(
                     npyscreen.TitleFilename,
                     name=f"{self.num}Pythonpath on remote machine:",
                     value=cfg.get("ansible_python_interpreter", "/usr/bin/python3"),
                 ),
                 False,
@@ -717,47 +783,55 @@
             self.parentApp.change_form(missing_form)
             return
         public_keyfile = self.public_keyfile.value or self.chain_keyfile.value
         cert_files = dict(
             public=public_keyfile or "",
             private=self.private_keyfile.value or "",
         )
+        save_file = Path(
+            self.parentApp.get_save_file(self.inventory_file.value or None)
+        )
         for key_type, keyfile in cert_files.items():
+            key_file = Path(get_current_file_dir(save_file.parent, str(keyfile)))
             for step, deploy_form in self.parentApp._forms.items():
-                if not keyfile or not Path(keyfile).is_file():
+                if not keyfile or not Path(key_file).is_file():
                     if (
                         key_type in deploy_form.certificates
                         and step in self.parentApp.steps
                     ):
                         if keyfile:
-                            msg = f"{key_type} certificate file `{keyfile}` must exist."
+                            msg = (
+                                f"{key_type} certificate file `{key_file}` must exist."
+                            )
                         else:
                             msg = f"You must give a {key_type} certificate file."
                         npyscreen.notify_confirm(msg, title="ERROR")
                         return
 
         cert_files["chain"] = self.chain_keyfile.value or ""
         if not cert_files["chain"]:
             value = npyscreen.notify_yes_no(
                 "It is advised to create a chained certificate file. "
                 "This enhances the web ui security. Continue anyway?",
                 title="WARNING",
             )
             if not value:
                 return
-        save_file = self.parentApp.save_config_to_file(write_toml_file=True)
-        if isinstance(save_file, Path):
-            save_file = str(save_file)
+        _ = self.parentApp.save_config_to_file(
+            save_file=save_file, write_toml_file=True
+        )
         self.parentApp.setup = {
             "server_map": self.server_map.value,
             "steps": list(set(self.parentApp.steps)),
             "ask_pass": bool(self.use_ssh_pw.value),
-            "config_file": save_file or None,
+            "config_file": str(save_file) or None,
         }
-        self.parentApp.exit_application(msg="Do you want to continue?")
+        self.parentApp.exit_application(
+            save_file=save_file, msg="Do you want to continue?"
+        )
 
     def on_cancel(self) -> None:
         """Define what happens after the the cancel button is hit."""
         name = self.parentApp.current_form.lower()
         self.parentApp.setup = {}
         for step, form_name in self.parentApp._steps_lookup.items():
             if name.startswith(step):
```

### Comparing `freva_deployment-2303.1.0/src/freva_deployment/utils.py` & `freva_deployment-2304.0.0/src/freva_deployment/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,28 +5,42 @@
 import json
 from pathlib import Path
 import pkg_resources
 import re
 from subprocess import PIPE
 import sys
 import shutil
-from typing import cast, NamedTuple
+from typing import Any, NamedTuple, cast
 import warnings
 
 import appdirs
 import requests
 from rich.console import Console
 from rich.prompt import Prompt
 import toml
 
 logging.basicConfig(format="%(name)s - %(levelname)s - %(message)s", level=logging.INFO)
 logger = logging.getLogger("freva-deployment")
 
 RichConsole = Console(markup=True, force_terminal=True)
 
+config_text = """
+### This is the global config file for the freva deployment
+[general]
+[variables]
+### you can set here different *global* variables that are
+### evaluatated in the deployment configurations. For example
+### if you set here the variable USER = "foo" then you can
+### use the this defined variable in the inventory file to
+### set the ansible user: anisble_user="${USER}"
+
+# USER="myusername"
+# USER_GROUP = "myusergroup"
+"""
+
 password_prompt = (
     "[green]Choose[/] a [b]master password[/], this password will be used to:\n"
     "- create the [magenta]mysql root[/] password\n"
     "- set the [magenta]django admin[/] web password\n"
     "[b]Note:[/] Ideally this password can be shared amongst other [i]admins[/].\n"
     "[b][green]choose[/] master password[/]"
 )
@@ -75,18 +89,62 @@
         inventory_file = self._user_config_dir / "inventory.toml"
         if inventory_file.exists():
             return self._user_config_dir
         self._user_config_dir.mkdir(exist_ok=True, parents=True)
         shutil.copy(self.asset_dir / "config" / "inventory.toml", inventory_file)
         return self._user_config_dir
 
+    @property
+    def config_file(self):
+        cfg_file = self.config_dir / "freva-deployment.config"
+        if not cfg_file.exists():
+            cfg_file.parent.mkdir(exist_ok=True, parents=True)
+            with cfg_file.open("w", encoding="utf-8") as f_obj:
+                f_obj.write(config_text)
+        return cfg_file
+
 
 AD = AssetDir()
 asset_dir = AD.asset_dir
 config_dir = AD.config_dir
+config_file = AD.config_file
+
+
+def get_current_file_dir(inp_dir: str | Path, value: str) -> str:
+    """Get a path with the CFD as a variable."""
+    if "${CFD}" in value.upper() or "$CFD" in value.upper():
+        value = value.replace("${CFD}", "$CFD")
+        part_1, _, part_2 = value.partition("$CFD/")
+        return str(Path(inp_dir, *Path(part_2).parts))
+    return value
+
+
+def _convert_dict(
+    inp_dict: dict[str, str | dict[str, Any]],
+    variables: dict[str, str],
+    cfd: Path,
+) -> None:
+    for key, value in inp_dict.items():
+        if isinstance(value, dict):
+            _convert_dict(value, variables, cfd)
+        elif isinstance(value, str):
+            for varn, variable in variables.items():
+                if f"${{{varn}}}" in value or f"${varn}" in value:
+                    value = value.replace(f"${{{varn}}}", f"${varn}")
+                    value = value.replace(f"${varn}", variable)
+            inp_dict[key] = get_current_file_dir(cfd, value)
+
+
+def load_config(inp_file: str | Path) -> dict[str, Any]:
+    """Load the inventory toml file and replace all environment variables."""
+    inp_file = Path(inp_file).expanduser().absolute()
+    variables = cast(dict[str, str], toml.loads(config_file.read_text())["variables"])
+    config = toml.loads(inp_file.read_text())
+    _convert_dict(config, variables, inp_file.parent)
+    return config
 
 
 def guess_map_server(
     inp_server: str | None, default_port: int = 6111, mandatory: bool = True
 ) -> str:
     """Try to get the server name mapping the freva infrastructure.
```

### Comparing `freva_deployment-2303.1.0/src/freva_deployment.egg-info/PKG-INFO` & `freva_deployment-2304.0.0/src/freva_deployment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: freva-deployment
-Version: 2303.1.0
+Version: 2304.0.0
 Summary: Deploy freva and its services on different machines.
 Home-page: https://github.com/FREVA-CLINT/freva.git
 Author: Martin Bergemann
 Author-email: martin.bergemann@dkrz.de
 Maintainer: Martin Bergemann
 License: GPLv3
 Project-URL: Documentation, https://freva-deployment.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/FREVA-CLINT/freva/issues
 Project-URL: Source, https://github.com/FREVA-CLINT/freva
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
@@ -327,9 +326,7 @@
 git config --global user.name your_user
 git config --global user.email your@email.com
 ```
 
 
 # Advanced: Adjusting the playbook
 Playbook templates and be found the in the `playbooks` directory. You can also add new variables to the playbook if they are present in the `config/inventory` file.
-
-
```

### Comparing `freva_deployment-2303.1.0/src/freva_deployment.egg-info/SOURCES.txt` & `freva_deployment-2304.0.0/src/freva_deployment.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 MANIFEST.in
 README.md
 setup.py
 assets/config/create_tables.sql
-assets/config/evaluation_system.conf.tmpl
 assets/config/inventory.toml
 assets/db_service/password_rotate.py
 assets/db_service/reset_root_pw.sh
 assets/playbooks/core-server-playbook.yml
 assets/playbooks/db-server-playbook.yml
 assets/playbooks/server-map-playbook.yml
 assets/playbooks/solr-server-playbook.yml
```

