# Comparing `tmp/hcs-cli-0.1.27.tar.gz` & `tmp/hcs-cli-0.1.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcs-cli-0.1.27.tar", last modified: Tue Apr 11 01:05:06 2023, max compression
+gzip compressed data, was "hcs-cli-0.1.28.tar", last modified: Tue Apr 11 23:24:51 2023, max compression
```

## Comparing `hcs-cli-0.1.27.tar` & `hcs-cli-0.1.28.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.155745 hcs-cli-0.1.27/
--rw-r--r--   0 nanw       (501) staff       (20)     2820 2023-01-11 22:10:27.000000 hcs-cli-0.1.27/.gitignore
--rw-r--r--   0 nanw       (501) staff       (20)       82 2023-04-07 18:36:38.000000 hcs-cli-0.1.27/CHANGELOG.md
--rw-r--r--   0 nanw       (501) staff       (20)      701 2023-04-08 01:22:34.000000 hcs-cli-0.1.27/Makefile
--rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-04-11 01:05:06.155325 hcs-cli-0.1.27/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     1486 2023-04-11 01:01:20.000000 hcs-cli-0.1.27/README.md
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.077664 hcs-cli-0.1.27/hcs_cli.egg-info/
--rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-04-11 01:05:05.000000 hcs-cli-0.1.27/hcs_cli.egg-info/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     2782 2023-04-11 01:05:05.000000 hcs-cli-0.1.27/hcs_cli.egg-info/SOURCES.txt
--rw-r--r--   0 nanw       (501) staff       (20)        1 2023-04-11 01:05:05.000000 hcs-cli-0.1.27/hcs_cli.egg-info/dependency_links.txt
--rw-r--r--   0 nanw       (501) staff       (20)       43 2023-04-11 01:05:05.000000 hcs-cli-0.1.27/hcs_cli.egg-info/entry_points.txt
--rw-r--r--   0 nanw       (501) staff       (20)      142 2023-04-11 01:05:05.000000 hcs-cli-0.1.27/hcs_cli.egg-info/requires.txt
--rw-r--r--   0 nanw       (501) staff       (20)       11 2023-04-11 01:05:05.000000 hcs-cli-0.1.27/hcs_cli.egg-info/top_level.txt
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.058620 hcs-cli-0.1.27/payload/
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.078530 hcs-cli-0.1.27/payload/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)      752 2023-04-11 00:40:07.000000 hcs-cli-0.1.27/payload/lcm/zero.json
--rw-r--r--   0 nanw       (501) staff       (20)     1125 2023-04-07 16:11:06.000000 hcs-cli-0.1.27/pyproject.toml
--rw-r--r--   0 nanw       (501) staff       (20)      142 2023-04-08 01:21:33.000000 hcs-cli-0.1.27/requirements.txt
--rw-r--r--   0 nanw       (501) staff       (20)       38 2023-04-11 01:05:06.156946 hcs-cli-0.1.27/setup.cfg
--rw-r--r--   0 nanw       (501) staff       (20)      544 2023-04-11 01:05:02.000000 hcs-cli-0.1.27/setup.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.080202 hcs-cli-0.1.27/tests/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:01:50.000000 hcs-cli-0.1.27/tests/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:01:42.000000 hcs-cli-0.1.27/tests/conftest.py
--rw-r--r--   0 nanw       (501) staff       (20)     2425 2023-04-08 01:06:36.000000 hcs-cli-0.1.27/tests/test_utils.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.081255 hcs-cli-0.1.27/tests/vhcs/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:35.000000 hcs-cli-0.1.27/tests/vhcs/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.081856 hcs-cli-0.1.27/tests/vhcs/cli/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:38.000000 hcs-cli-0.1.27/tests/vhcs/cli/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.084990 hcs-cli-0.1.27/tests/vhcs/cli/cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:39.000000 hcs-cli-0.1.27/tests/vhcs/cli/cmds/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.086622 hcs-cli-0.1.27/tests/vhcs/cli/cmds/pki/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:41.000000 hcs-cli-0.1.27/tests/vhcs/cli/cmds/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 21:57:30.000000 hcs-cli-0.1.27/tests/vhcs/cli/cmds/pki/get_root_ca.py
--rw-r--r--   0 nanw       (501) staff       (20)      290 2023-04-08 01:06:36.000000 hcs-cli-0.1.27/tests/vhcs/cli/cmds/test_auth.py
--rw-r--r--   0 nanw       (501) staff       (20)     1343 2023-04-08 01:06:36.000000 hcs-cli-0.1.27/tests/vhcs/cli/cmds/test_context.py
--rw-r--r--   0 nanw       (501) staff       (20)      551 2023-04-08 01:16:54.000000 hcs-cli-0.1.27/tests/vhcs/cli/cmds/test_profile.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.087292 hcs-cli-0.1.27/vhcs/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 21:25:27.000000 hcs-cli-0.1.27/vhcs/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.088410 hcs-cli-0.1.27/vhcs/cli/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.27/vhcs/cli/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.090302 hcs-cli-0.1.27/vhcs/cli/cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.27/vhcs/cli/cmds/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.090855 hcs-cli-0.1.27/vhcs/cli/cmds/admin/
--rw-r--r--   0 nanw       (501) staff       (20)       33 2023-04-10 16:58:33.000000 hcs-cli-0.1.27/vhcs/cli/cmds/admin/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.093681 hcs-cli-0.1.27/vhcs/cli/cmds/admin/edge/
--rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-10 16:21:00.000000 hcs-cli-0.1.27/vhcs/cli/cmds/admin/edge/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      343 2023-04-10 19:16:01.000000 hcs-cli-0.1.27/vhcs/cli/cmds/admin/edge/get.py
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-10 16:21:00.000000 hcs-cli-0.1.27/vhcs/cli/cmds/admin/edge/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.096148 hcs-cli-0.1.27/vhcs/cli/cmds/admin/template/
--rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-10 16:20:13.000000 hcs-cli-0.1.27/vhcs/cli/cmds/admin/template/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      351 2023-04-10 19:13:27.000000 hcs-cli-0.1.27/vhcs/cli/cmds/admin/template/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1393 2023-04-10 17:45:24.000000 hcs-cli-0.1.27/vhcs/cli/cmds/admin/template/list.py
--rw-r--r--   0 nanw       (501) staff       (20)      375 2023-04-07 18:22:47.000000 hcs-cli-0.1.27/vhcs/cli/cmds/auth.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.097537 hcs-cli-0.1.27/vhcs/cli/cmds/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)       31 2023-04-06 17:42:33.000000 hcs-cli-0.1.27/vhcs/cli/cmds/lcm/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.101967 hcs-cli-0.1.27/vhcs/cli/cmds/lcm/provider/
--rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-06 17:42:33.000000 hcs-cli-0.1.27/vhcs/cli/cmds/lcm/provider/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      196 2023-04-07 18:26:01.000000 hcs-cli-0.1.27/vhcs/cli/cmds/lcm/provider/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      187 2023-04-07 18:26:21.000000 hcs-cli-0.1.27/vhcs/cli/cmds/lcm/provider/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      380 2023-04-11 01:00:36.000000 hcs-cli-0.1.27/vhcs/cli/cmds/lcm/provider/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.107843 hcs-cli-0.1.27/vhcs/cli/cmds/lcm/template/
--rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-06 17:42:33.000000 hcs-cli-0.1.27/vhcs/cli/cmds/lcm/template/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1289 2023-04-11 00:52:05.000000 hcs-cli-0.1.27/vhcs/cli/cmds/lcm/template/create.py
--rw-r--r--   0 nanw       (501) staff       (20)      474 2023-04-11 00:46:01.000000 hcs-cli-0.1.27/vhcs/cli/cmds/lcm/template/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      235 2023-04-10 19:14:17.000000 hcs-cli-0.1.27/vhcs/cli/cmds/lcm/template/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      962 2023-04-10 19:04:36.000000 hcs-cli-0.1.27/vhcs/cli/cmds/lcm/template/list.py
--rw-r--r--   0 nanw       (501) staff       (20)     1693 2023-04-10 21:48:05.000000 hcs-cli-0.1.27/vhcs/cli/cmds/lcm/template/wait.py
--rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-07 18:18:56.000000 hcs-cli-0.1.27/vhcs/cli/cmds/lcm/test.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.111851 hcs-cli-0.1.27/vhcs/cli/cmds/pki/
--rw-r--r--   0 nanw       (501) staff       (20)       31 2023-04-06 17:42:33.000000 hcs-cli-0.1.27/vhcs/cli/cmds/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      551 2023-04-07 18:26:57.000000 hcs-cli-0.1.27/vhcs/cli/cmds/pki/delete_org_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      297 2023-04-07 18:27:02.000000 hcs-cli-0.1.27/vhcs/cli/cmds/pki/get_org_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      163 2023-04-07 18:27:20.000000 hcs-cli-0.1.27/vhcs/cli/cmds/pki/get_root_ca.py
--rw-r--r--   0 nanw       (501) staff       (20)     1220 2023-04-06 22:12:04.000000 hcs-cli-0.1.27/vhcs/cli/cmds/pki/sign_resource_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-07 18:21:03.000000 hcs-cli-0.1.27/vhcs/cli/cmds/pki/test.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.113119 hcs-cli-0.1.27/vhcs/cli/cmds/profile/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.27/vhcs/cli/cmds/profile/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     3644 2023-04-08 01:06:36.000000 hcs-cli-0.1.27/vhcs/cli/cmds/profile/init.py
--rw-r--r--   0 nanw       (501) staff       (20)      332 2023-04-07 18:23:32.000000 hcs-cli-0.1.27/vhcs/cli/cmds/upgrade.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.115770 hcs-cli-0.1.27/vhcs/cli/cmds/vmhub/
--rw-r--r--   0 nanw       (501) staff       (20)       33 2023-04-06 17:42:33.000000 hcs-cli-0.1.27/vhcs/cli/cmds/vmhub/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      662 2023-04-07 18:27:15.000000 hcs-cli-0.1.27/vhcs/cli/cmds/vmhub/redeem-otp.py
--rw-r--r--   0 nanw       (501) staff       (20)      567 2023-04-07 18:27:38.000000 hcs-cli-0.1.27/vhcs/cli/cmds/vmhub/request-otp.py
--rw-r--r--   0 nanw       (501) staff       (20)      110 2023-04-07 18:22:14.000000 hcs-cli-0.1.27/vhcs/cli/cmds/vmhub/test.py
--rwxr-xr-x   0 nanw       (501) staff       (20)     2381 2023-04-10 22:35:04.000000 hcs-cli-0.1.27/vhcs/cli/main.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.116993 hcs-cli-0.1.27/vhcs/common/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.27/vhcs/common/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.129155 hcs-cli-0.1.27/vhcs/common/ctxp/
--rw-r--r--   0 nanw       (501) staff       (20)     1839 2023-04-06 02:05:21.000000 hcs-cli-0.1.27/vhcs/common/ctxp/README.md
--rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-10 18:35:40.000000 hcs-cli-0.1.27/vhcs/common/ctxp/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.132440 hcs-cli-0.1.27/vhcs/common/ctxp/built_in_cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.27/vhcs/common/ctxp/built_in_cmds/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1419 2023-04-07 23:54:52.000000 hcs-cli-0.1.27/vhcs/common/ctxp/built_in_cmds/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     1817 2023-04-08 01:12:13.000000 hcs-cli-0.1.27/vhcs/common/ctxp/built_in_cmds/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     4097 2023-04-10 19:00:11.000000 hcs-cli-0.1.27/vhcs/common/ctxp/cli_processor.py
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.27/vhcs/common/ctxp/cli_state.py
--rw-r--r--   0 nanw       (501) staff       (20)      337 2023-04-07 00:28:47.000000 hcs-cli-0.1.27/vhcs/common/ctxp/config.py
--rw-r--r--   0 nanw       (501) staff       (20)     1656 2023-04-07 00:28:55.000000 hcs-cli-0.1.27/vhcs/common/ctxp/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     5680 2023-04-07 00:18:58.000000 hcs-cli-0.1.27/vhcs/common/ctxp/fstore.py
--rw-r--r--   0 nanw       (501) staff       (20)      548 2023-04-07 16:49:23.000000 hcs-cli-0.1.27/vhcs/common/ctxp/init.py
--rw-r--r--   0 nanw       (501) staff       (20)     2128 2023-04-06 02:05:21.000000 hcs-cli-0.1.27/vhcs/common/ctxp/jsondot.py
--rw-r--r--   0 nanw       (501) staff       (20)     3695 2023-04-08 01:06:36.000000 hcs-cli-0.1.27/vhcs/common/ctxp/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     1486 2023-04-10 19:10:32.000000 hcs-cli-0.1.27/vhcs/common/ctxp/util.py
--rw-r--r--   0 nanw       (501) staff       (20)     2633 2023-04-07 00:29:18.000000 hcs-cli-0.1.27/vhcs/common/ctxp/var_template.py
--rw-r--r--   0 nanw       (501) staff       (20)     4246 2023-04-07 00:37:01.000000 hcs-cli-0.1.27/vhcs/common/logger.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.138679 hcs-cli-0.1.27/vhcs/common/sglib/
--rw-r--r--   0 nanw       (501) staff       (20)       54 2023-04-06 02:05:21.000000 hcs-cli-0.1.27/vhcs/common/sglib/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     2504 2023-04-07 00:18:58.000000 hcs-cli-0.1.27/vhcs/common/sglib/auth.py
--rw-r--r--   0 nanw       (501) staff       (20)     3601 2023-04-07 00:18:58.000000 hcs-cli-0.1.27/vhcs/common/sglib/csp.py
--rw-r--r--   0 nanw       (501) staff       (20)     3866 2023-04-10 22:09:28.000000 hcs-cli-0.1.27/vhcs/common/sglib/ez_client.py
--rw-r--r--   0 nanw       (501) staff       (20)      549 2023-04-07 19:17:10.000000 hcs-cli-0.1.27/vhcs/common/sglib/hcs_client.py
--rw-r--r--   0 nanw       (501) staff       (20)      370 2023-04-10 18:29:50.000000 hcs-cli-0.1.27/vhcs/common/sglib/util.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.140877 hcs-cli-0.1.27/vhcs/config/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.27/vhcs/config/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     7327 2023-04-06 17:22:27.000000 hcs-cli-0.1.27/vhcs/config/hcs-deployments.yaml
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.148875 hcs-cli-0.1.27/vhcs/service/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.27/vhcs/service/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      986 2023-04-10 16:58:33.000000 hcs-cli-0.1.27/vhcs/service/_util.py
--rw-r--r--   0 nanw       (501) staff       (20)      822 2023-04-10 19:16:10.000000 hcs-cli-0.1.27/vhcs/service/admin.py
--rw-r--r--   0 nanw       (501) staff       (20)     3199 2023-04-11 01:04:04.000000 hcs-cli-0.1.27/vhcs/service/lcm.py
--rw-r--r--   0 nanw       (501) staff       (20)      610 2023-04-07 21:33:14.000000 hcs-cli-0.1.27/vhcs/service/pki.py
--rw-r--r--   0 nanw       (501) staff       (20)      929 2023-04-07 19:31:02.000000 hcs-cli-0.1.27/vhcs/service/vmhub.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 01:05:06.154451 hcs-cli-0.1.27/vhcs/util/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.27/vhcs/util/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     2160 2023-04-10 21:32:09.000000 hcs-cli-0.1.27/vhcs/util/duration.py
--rw-r--r--   0 nanw       (501) staff       (20)     4699 2023-04-06 02:05:21.000000 hcs-cli-0.1.27/vhcs/util/pki_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     1127 2023-04-10 19:16:42.000000 hcs-cli-0.1.27/vhcs/util/query_util.py
--rw-r--r--   0 nanw       (501) staff       (20)      832 2023-04-07 19:01:08.000000 hcs-cli-0.1.27/vhcs/util/versions.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.274489 hcs-cli-0.1.28/
+-rw-r--r--   0 nanw       (501) staff       (20)     2820 2023-01-11 22:10:27.000000 hcs-cli-0.1.28/.gitignore
+-rw-r--r--   0 nanw       (501) staff       (20)       82 2023-04-07 18:36:38.000000 hcs-cli-0.1.28/CHANGELOG.md
+-rw-r--r--   0 nanw       (501) staff       (20)      701 2023-04-08 01:22:34.000000 hcs-cli-0.1.28/Makefile
+-rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-04-11 23:24:51.274052 hcs-cli-0.1.28/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     1486 2023-04-11 01:01:20.000000 hcs-cli-0.1.28/README.md
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.168485 hcs-cli-0.1.28/hcs_cli.egg-info/
+-rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-04-11 23:24:50.000000 hcs-cli-0.1.28/hcs_cli.egg-info/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     2782 2023-04-11 23:24:51.000000 hcs-cli-0.1.28/hcs_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 nanw       (501) staff       (20)        1 2023-04-11 23:24:50.000000 hcs-cli-0.1.28/hcs_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       43 2023-04-11 23:24:50.000000 hcs-cli-0.1.28/hcs_cli.egg-info/entry_points.txt
+-rw-r--r--   0 nanw       (501) staff       (20)      142 2023-04-11 23:24:50.000000 hcs-cli-0.1.28/hcs_cli.egg-info/requires.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       11 2023-04-11 23:24:50.000000 hcs-cli-0.1.28/hcs_cli.egg-info/top_level.txt
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.148573 hcs-cli-0.1.28/payload/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.169422 hcs-cli-0.1.28/payload/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)      752 2023-04-11 00:40:07.000000 hcs-cli-0.1.28/payload/lcm/zero.json
+-rw-r--r--   0 nanw       (501) staff       (20)     1125 2023-04-07 16:11:06.000000 hcs-cli-0.1.28/pyproject.toml
+-rw-r--r--   0 nanw       (501) staff       (20)      142 2023-04-08 01:21:33.000000 hcs-cli-0.1.28/requirements.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       38 2023-04-11 23:24:51.275841 hcs-cli-0.1.28/setup.cfg
+-rw-r--r--   0 nanw       (501) staff       (20)      544 2023-04-11 23:24:25.000000 hcs-cli-0.1.28/setup.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.171269 hcs-cli-0.1.28/tests/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:01:50.000000 hcs-cli-0.1.28/tests/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:01:42.000000 hcs-cli-0.1.28/tests/conftest.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2425 2023-04-08 01:06:36.000000 hcs-cli-0.1.28/tests/test_utils.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.172366 hcs-cli-0.1.28/tests/vhcs/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:35.000000 hcs-cli-0.1.28/tests/vhcs/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.172941 hcs-cli-0.1.28/tests/vhcs/cli/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:38.000000 hcs-cli-0.1.28/tests/vhcs/cli/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.176741 hcs-cli-0.1.28/tests/vhcs/cli/cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:39.000000 hcs-cli-0.1.28/tests/vhcs/cli/cmds/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.178339 hcs-cli-0.1.28/tests/vhcs/cli/cmds/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:41.000000 hcs-cli-0.1.28/tests/vhcs/cli/cmds/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 21:57:30.000000 hcs-cli-0.1.28/tests/vhcs/cli/cmds/pki/get_root_ca.py
+-rw-r--r--   0 nanw       (501) staff       (20)      290 2023-04-08 01:06:36.000000 hcs-cli-0.1.28/tests/vhcs/cli/cmds/test_auth.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1343 2023-04-08 01:06:36.000000 hcs-cli-0.1.28/tests/vhcs/cli/cmds/test_context.py
+-rw-r--r--   0 nanw       (501) staff       (20)      551 2023-04-08 01:16:54.000000 hcs-cli-0.1.28/tests/vhcs/cli/cmds/test_profile.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.178900 hcs-cli-0.1.28/vhcs/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 21:25:27.000000 hcs-cli-0.1.28/vhcs/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.179920 hcs-cli-0.1.28/vhcs/cli/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.28/vhcs/cli/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.181564 hcs-cli-0.1.28/vhcs/cli/cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.28/vhcs/cli/cmds/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.182082 hcs-cli-0.1.28/vhcs/cli/cmds/admin/
+-rw-r--r--   0 nanw       (501) staff       (20)       33 2023-04-10 16:58:33.000000 hcs-cli-0.1.28/vhcs/cli/cmds/admin/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.184833 hcs-cli-0.1.28/vhcs/cli/cmds/admin/edge/
+-rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-10 16:21:00.000000 hcs-cli-0.1.28/vhcs/cli/cmds/admin/edge/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      343 2023-04-10 19:16:01.000000 hcs-cli-0.1.28/vhcs/cli/cmds/admin/edge/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-10 16:21:00.000000 hcs-cli-0.1.28/vhcs/cli/cmds/admin/edge/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.188605 hcs-cli-0.1.28/vhcs/cli/cmds/admin/template/
+-rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-10 16:20:13.000000 hcs-cli-0.1.28/vhcs/cli/cmds/admin/template/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      351 2023-04-10 19:13:27.000000 hcs-cli-0.1.28/vhcs/cli/cmds/admin/template/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1393 2023-04-10 17:45:24.000000 hcs-cli-0.1.28/vhcs/cli/cmds/admin/template/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)      375 2023-04-07 18:22:47.000000 hcs-cli-0.1.28/vhcs/cli/cmds/auth.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.191659 hcs-cli-0.1.28/vhcs/cli/cmds/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)       31 2023-04-06 17:42:33.000000 hcs-cli-0.1.28/vhcs/cli/cmds/lcm/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.195104 hcs-cli-0.1.28/vhcs/cli/cmds/lcm/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-06 17:42:33.000000 hcs-cli-0.1.28/vhcs/cli/cmds/lcm/provider/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      196 2023-04-07 18:26:01.000000 hcs-cli-0.1.28/vhcs/cli/cmds/lcm/provider/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      187 2023-04-07 18:26:21.000000 hcs-cli-0.1.28/vhcs/cli/cmds/lcm/provider/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      380 2023-04-11 01:00:36.000000 hcs-cli-0.1.28/vhcs/cli/cmds/lcm/provider/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.201698 hcs-cli-0.1.28/vhcs/cli/cmds/lcm/template/
+-rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-06 17:42:33.000000 hcs-cli-0.1.28/vhcs/cli/cmds/lcm/template/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1289 2023-04-11 00:52:05.000000 hcs-cli-0.1.28/vhcs/cli/cmds/lcm/template/create.py
+-rw-r--r--   0 nanw       (501) staff       (20)      474 2023-04-11 00:46:01.000000 hcs-cli-0.1.28/vhcs/cli/cmds/lcm/template/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      235 2023-04-11 23:21:14.000000 hcs-cli-0.1.28/vhcs/cli/cmds/lcm/template/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      962 2023-04-10 19:04:36.000000 hcs-cli-0.1.28/vhcs/cli/cmds/lcm/template/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1693 2023-04-10 21:48:05.000000 hcs-cli-0.1.28/vhcs/cli/cmds/lcm/template/wait.py
+-rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-07 18:18:56.000000 hcs-cli-0.1.28/vhcs/cli/cmds/lcm/test.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.208136 hcs-cli-0.1.28/vhcs/cli/cmds/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)       31 2023-04-06 17:42:33.000000 hcs-cli-0.1.28/vhcs/cli/cmds/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      551 2023-04-07 18:26:57.000000 hcs-cli-0.1.28/vhcs/cli/cmds/pki/delete_org_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      297 2023-04-07 18:27:02.000000 hcs-cli-0.1.28/vhcs/cli/cmds/pki/get_org_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      163 2023-04-07 18:27:20.000000 hcs-cli-0.1.28/vhcs/cli/cmds/pki/get_root_ca.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1220 2023-04-06 22:12:04.000000 hcs-cli-0.1.28/vhcs/cli/cmds/pki/sign_resource_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-07 18:21:03.000000 hcs-cli-0.1.28/vhcs/cli/cmds/pki/test.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.211043 hcs-cli-0.1.28/vhcs/cli/cmds/profile/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.28/vhcs/cli/cmds/profile/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3644 2023-04-08 01:06:36.000000 hcs-cli-0.1.28/vhcs/cli/cmds/profile/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)      332 2023-04-07 18:23:32.000000 hcs-cli-0.1.28/vhcs/cli/cmds/upgrade.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.215986 hcs-cli-0.1.28/vhcs/cli/cmds/vmhub/
+-rw-r--r--   0 nanw       (501) staff       (20)       33 2023-04-06 17:42:33.000000 hcs-cli-0.1.28/vhcs/cli/cmds/vmhub/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      662 2023-04-07 18:27:15.000000 hcs-cli-0.1.28/vhcs/cli/cmds/vmhub/redeem-otp.py
+-rw-r--r--   0 nanw       (501) staff       (20)      567 2023-04-07 18:27:38.000000 hcs-cli-0.1.28/vhcs/cli/cmds/vmhub/request-otp.py
+-rw-r--r--   0 nanw       (501) staff       (20)      110 2023-04-07 18:22:14.000000 hcs-cli-0.1.28/vhcs/cli/cmds/vmhub/test.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)     2397 2023-04-11 23:19:57.000000 hcs-cli-0.1.28/vhcs/cli/main.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.218441 hcs-cli-0.1.28/vhcs/common/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.28/vhcs/common/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.239035 hcs-cli-0.1.28/vhcs/common/ctxp/
+-rw-r--r--   0 nanw       (501) staff       (20)     1839 2023-04-06 02:05:21.000000 hcs-cli-0.1.28/vhcs/common/ctxp/README.md
+-rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-10 18:35:40.000000 hcs-cli-0.1.28/vhcs/common/ctxp/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.244025 hcs-cli-0.1.28/vhcs/common/ctxp/built_in_cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.28/vhcs/common/ctxp/built_in_cmds/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1419 2023-04-07 23:54:52.000000 hcs-cli-0.1.28/vhcs/common/ctxp/built_in_cmds/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1817 2023-04-08 01:12:13.000000 hcs-cli-0.1.28/vhcs/common/ctxp/built_in_cmds/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4139 2023-04-11 23:07:45.000000 hcs-cli-0.1.28/vhcs/common/ctxp/cli_processor.py
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.28/vhcs/common/ctxp/cli_state.py
+-rw-r--r--   0 nanw       (501) staff       (20)      337 2023-04-07 00:28:47.000000 hcs-cli-0.1.28/vhcs/common/ctxp/config.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1656 2023-04-07 00:28:55.000000 hcs-cli-0.1.28/vhcs/common/ctxp/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5680 2023-04-07 00:18:58.000000 hcs-cli-0.1.28/vhcs/common/ctxp/fstore.py
+-rw-r--r--   0 nanw       (501) staff       (20)      548 2023-04-07 16:49:23.000000 hcs-cli-0.1.28/vhcs/common/ctxp/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2128 2023-04-06 02:05:21.000000 hcs-cli-0.1.28/vhcs/common/ctxp/jsondot.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3695 2023-04-08 01:06:36.000000 hcs-cli-0.1.28/vhcs/common/ctxp/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2157 2023-04-11 23:18:54.000000 hcs-cli-0.1.28/vhcs/common/ctxp/util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2633 2023-04-07 00:29:18.000000 hcs-cli-0.1.28/vhcs/common/ctxp/var_template.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4246 2023-04-07 00:37:01.000000 hcs-cli-0.1.28/vhcs/common/logger.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.252591 hcs-cli-0.1.28/vhcs/common/sglib/
+-rw-r--r--   0 nanw       (501) staff       (20)       54 2023-04-06 02:05:21.000000 hcs-cli-0.1.28/vhcs/common/sglib/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2504 2023-04-07 00:18:58.000000 hcs-cli-0.1.28/vhcs/common/sglib/auth.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3601 2023-04-07 00:18:58.000000 hcs-cli-0.1.28/vhcs/common/sglib/csp.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3866 2023-04-10 22:09:28.000000 hcs-cli-0.1.28/vhcs/common/sglib/ez_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)      549 2023-04-07 19:17:10.000000 hcs-cli-0.1.28/vhcs/common/sglib/hcs_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)      370 2023-04-10 18:29:50.000000 hcs-cli-0.1.28/vhcs/common/sglib/util.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.255216 hcs-cli-0.1.28/vhcs/config/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.28/vhcs/config/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7327 2023-04-06 17:22:27.000000 hcs-cli-0.1.28/vhcs/config/hcs-deployments.yaml
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.264113 hcs-cli-0.1.28/vhcs/service/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.28/vhcs/service/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      986 2023-04-10 16:58:33.000000 hcs-cli-0.1.28/vhcs/service/_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)      822 2023-04-10 19:16:10.000000 hcs-cli-0.1.28/vhcs/service/admin.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3199 2023-04-11 01:04:04.000000 hcs-cli-0.1.28/vhcs/service/lcm.py
+-rw-r--r--   0 nanw       (501) staff       (20)      610 2023-04-07 21:33:14.000000 hcs-cli-0.1.28/vhcs/service/pki.py
+-rw-r--r--   0 nanw       (501) staff       (20)      929 2023-04-07 19:31:02.000000 hcs-cli-0.1.28/vhcs/service/vmhub.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.272030 hcs-cli-0.1.28/vhcs/util/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.28/vhcs/util/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2160 2023-04-10 21:32:09.000000 hcs-cli-0.1.28/vhcs/util/duration.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4699 2023-04-06 02:05:21.000000 hcs-cli-0.1.28/vhcs/util/pki_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1127 2023-04-10 19:16:42.000000 hcs-cli-0.1.28/vhcs/util/query_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)      832 2023-04-07 19:01:08.000000 hcs-cli-0.1.28/vhcs/util/versions.py
```

### Comparing `hcs-cli-0.1.27/.gitignore` & `hcs-cli-0.1.28/.gitignore`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/Makefile` & `hcs-cli-0.1.28/Makefile`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/PKG-INFO` & `hcs-cli-0.1.28/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-cli
-Version: 0.1.27
+Version: 0.1.28
 Summary: Horizon Cloud Service CLI
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/nanw1103/hcs-cli
 Project-URL: Bug Tracker, https://github.com/nanw1103/hcs-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/nanw1103/hcs-cli
 Project-URL: changelog, https://github.com/nanw1103/hcs-cli/blob/master/CHANGELOG.md
```

### Comparing `hcs-cli-0.1.27/README.md` & `hcs-cli-0.1.28/README.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/hcs_cli.egg-info/PKG-INFO` & `hcs-cli-0.1.28/hcs_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-cli
-Version: 0.1.27
+Version: 0.1.28
 Summary: Horizon Cloud Service CLI
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/nanw1103/hcs-cli
 Project-URL: Bug Tracker, https://github.com/nanw1103/hcs-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/nanw1103/hcs-cli
 Project-URL: changelog, https://github.com/nanw1103/hcs-cli/blob/master/CHANGELOG.md
```

### Comparing `hcs-cli-0.1.27/hcs_cli.egg-info/SOURCES.txt` & `hcs-cli-0.1.28/hcs_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/payload/lcm/zero.json` & `hcs-cli-0.1.28/payload/lcm/zero.json`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/pyproject.toml` & `hcs-cli-0.1.28/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/setup.py` & `hcs-cli-0.1.28/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools_scm import get_version
 import os
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
-VERSION = "0.1.27"
+VERSION = "0.1.28"
 
 def get_version():
     version = VERSION
     local_version = os.environ.get("SCM_REV")
     if local_version:
         version += "+" + local_version
     return version
```

### Comparing `hcs-cli-0.1.27/tests/test_utils.py` & `hcs-cli-0.1.28/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/tests/vhcs/cli/cmds/test_context.py` & `hcs-cli-0.1.28/tests/vhcs/cli/cmds/test_context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/tests/vhcs/cli/cmds/test_profile.py` & `hcs-cli-0.1.28/tests/vhcs/cli/cmds/test_profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/vhcs/cli/cmds/admin/template/list.py` & `hcs-cli-0.1.28/vhcs/cli/cmds/admin/template/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/vhcs/cli/cmds/lcm/template/create.py` & `hcs-cli-0.1.28/vhcs/cli/cmds/lcm/template/create.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/vhcs/cli/cmds/lcm/template/list.py` & `hcs-cli-0.1.28/vhcs/cli/cmds/lcm/template/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/vhcs/cli/cmds/lcm/template/wait.py` & `hcs-cli-0.1.28/vhcs/cli/cmds/lcm/template/wait.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/vhcs/cli/cmds/pki/delete_org_cert.py` & `hcs-cli-0.1.28/vhcs/cli/cmds/pki/delete_org_cert.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/vhcs/cli/cmds/pki/sign_resource_cert.py` & `hcs-cli-0.1.28/vhcs/cli/cmds/pki/sign_resource_cert.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/vhcs/cli/cmds/profile/init.py` & `hcs-cli-0.1.28/vhcs/cli/cmds/profile/init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/vhcs/cli/cmds/vmhub/redeem-otp.py` & `hcs-cli-0.1.28/vhcs/cli/cmds/vmhub/redeem-otp.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/vhcs/cli/cmds/vmhub/request-otp.py` & `hcs-cli-0.1.28/vhcs/cli/cmds/vmhub/request-otp.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/vhcs/cli/main.py` & `hcs-cli-0.1.28/vhcs/cli/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 _script_dir = path.abspath(path.join(path.dirname(path.realpath(__file__)), "."))
 _module_dir = path.dirname(_script_dir)
 if __name__ == "__main__":
     _cli_dir = path.dirname(_module_dir)
     sys.path.append(_cli_dir)
 
 import vhcs.common.ctxp as ctxp
-from vhcs.common.ctxp.util import option_output, option_verbose
+from vhcs.common.ctxp.util import option_output, option_verbose, option_field
 
 # -----------------------------------------------------------
 import vhcs.common.logger as logger
 
 logger.setup()
 logging.getLogger("charset_normalizer").setLevel(logging.WARN)
 logging.getLogger("csp").setLevel(logging.INFO)
@@ -28,23 +28,25 @@
 # -----------------------------------------------------------
 
 
 @click.group()
 @click.version_option(package_name="hcs-cli")
 @option_verbose
 @option_output
+@option_field
 @click.option("--profile", "-p", type=str, required=False, help="Specify the profile to use. Optional.")
 @click.option("--upgrade-check/--no-upgrade-check", default=True, help="Check new version of HCS CLI.")
 @click.option("--telemetry/--no-telemetry", default=True, help="Send telemetry")
-def cli(verbose: bool, output: str, profile: str, upgrade_check: bool, telemetry: bool):
+def cli(**kwargs):
 
-    if upgrade_check:
+    if kwargs.get('upgrade_check'):
         from vhcs.util.versions import check_upgrade
-
         check_upgrade()
+        
+    profile = kwargs.get('profile')
     if profile:
         ctxp.profile._active_profile_name = profile
 
 
 # @cli.result_callback()
 # def _process_result(result, **kwargs):
 #     print("_process_result", result, kwargs)
```

### Comparing `hcs-cli-0.1.27/vhcs/common/ctxp/README.md` & `hcs-cli-0.1.28/vhcs/common/ctxp/README.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/vhcs/common/ctxp/built_in_cmds/context.py` & `hcs-cli-0.1.28/vhcs/common/ctxp/built_in_cmds/context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/vhcs/common/ctxp/built_in_cmds/profile.py` & `hcs-cli-0.1.28/vhcs/common/ctxp/built_in_cmds/profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/vhcs/common/ctxp/cli_processor.py` & `hcs-cli-0.1.28/vhcs/common/ctxp/cli_processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,22 +108,22 @@
 
 
 def _process_result(result, **kwargs):
     if result is not None:
         if isinstance(result, tuple):
             data, return_code = result
             if data is not None:
-                util.print_output(data, kwargs.get("output"))
+                util.print_output(data, kwargs.get("output"), kwargs.get("field"))
             if isinstance(return_code, int):
                 ctx = click.get_current_context()
                 ctx.exit(return_code)
             else:
                 raise Exception("Invalid command return code. Expect int, actual=" + str(type(return_code)))
         else:
-            util.print_output(result, kwargs.get("output"))
+            util.print_output(result, kwargs.get("output"), kwargs.get("field"))
 
 
 def init(main_cli: click.Group, commands_dir: str):
     _add_built_in_commands(main_cli)
     _add_subcommands(commands_dir, main_cli)
     main_cli.result_callback()(_process_result)
     return main_cli(obj={})
```

### Comparing `hcs-cli-0.1.27/vhcs/common/ctxp/context.py` & `hcs-cli-0.1.28/vhcs/common/ctxp/context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/vhcs/common/ctxp/fstore.py` & `hcs-cli-0.1.28/vhcs/common/ctxp/fstore.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/vhcs/common/ctxp/init.py` & `hcs-cli-0.1.28/vhcs/common/ctxp/init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/vhcs/common/ctxp/jsondot.py` & `hcs-cli-0.1.28/vhcs/common/ctxp/jsondot.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/vhcs/common/ctxp/profile.py` & `hcs-cli-0.1.28/vhcs/common/ctxp/profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/vhcs/common/ctxp/util.py` & `hcs-cli-0.1.28/vhcs/common/ctxp/util.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,39 +4,58 @@
 import click
 
 
 class CtxpException(Exception):
     pass
 
 
-def print_output(data: any, output: str = "json"):
+def print_output(data: any, output: str = "json", fields: str = None):
     if type(data) is str:
         text = data
-    elif output == "json":
-        text = json.dumps(data, indent=4)
-    elif output == "json-compact":
-        text = json.dumps(data)
-    elif output == "yaml":
-        import vhcs.common.ctxp as ctxp
-        text = yaml.dump(ctxp.jsondot.plain(data))
-    elif output == "text":
-        if isinstance(data, list):
-            text = ""
-            for i in data:
-                line = i if type(i) is str else json.dumps(i)
-                text += line + "\n"
-        elif isinstance(data, dict):
+    else:
+        _filter_fields(data, fields)
+
+        if output == "json":
             text = json.dumps(data, indent=4)
+        elif output == "json-compact":
+            text = json.dumps(data)
+        elif output == "yaml":
+            import vhcs.common.ctxp as ctxp
+            text = yaml.dump(ctxp.jsondot.plain(data))
+        elif output == "text":
+            if isinstance(data, list):
+                text = ""
+                for i in data:
+                    line = i if type(i) is str else json.dumps(i)
+                    text += line + "\n"
+            elif isinstance(data, dict):
+                text = json.dumps(data, indent=4)
+            else:
+                text = json.dumps(data, indent=4)
         else:
-            text = json.dumps(data, indent=4)
-    else:
-        raise Exception(f"Unexpected output format: {output}")
+            raise Exception(f"Unexpected output format: {output}")
     
     print(text, end="")
 
+def _filter_fields(obj: any, fields: str):
+    if not fields:
+        return obj
+    parts = fields.split(",")
+
+    def _filter_obj(o):
+        if not isinstance(o, dict):
+            return o
+        for k in list(o.keys()):
+            if k not in parts:
+                del o[k]
+        return o
+
+    if isinstance(obj, list):
+        return list(map(_filter_obj, obj))
+    return _filter_obj(obj)
 
 def panic(reason: any = None, code: int = 1):
     print(reason, file=sys.stderr)
     sys.exit(code)
 
 
 option_verbose = click.option(
@@ -51,14 +70,22 @@
     "-o",
     "--output",
     type=click.Choice(["json", "json-compact", "yaml", "text"]),
     default="json",
     help="Specify output format",
 )
 
+option_field = click.option(
+    "-f",
+    "--field",
+    type=str,
+    required=False,
+    help="Specify fields to output",
+)
+
 option_id_only = click.option(
     "--id-only/--full-object",
     type=bool,
     default=False,
     required=False,
     help="Output only the object, instead of the full data object"
 )
```

### Comparing `hcs-cli-0.1.27/vhcs/common/ctxp/var_template.py` & `hcs-cli-0.1.28/vhcs/common/ctxp/var_template.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/vhcs/common/logger.py` & `hcs-cli-0.1.28/vhcs/common/logger.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/vhcs/common/sglib/auth.py` & `hcs-cli-0.1.28/vhcs/common/sglib/auth.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/vhcs/common/sglib/csp.py` & `hcs-cli-0.1.28/vhcs/common/sglib/csp.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/vhcs/common/sglib/ez_client.py` & `hcs-cli-0.1.28/vhcs/common/sglib/ez_client.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/vhcs/common/sglib/hcs_client.py` & `hcs-cli-0.1.28/vhcs/common/sglib/hcs_client.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/vhcs/config/hcs-deployments.yaml` & `hcs-cli-0.1.28/vhcs/config/hcs-deployments.yaml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/vhcs/service/_util.py` & `hcs-cli-0.1.28/vhcs/service/_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/vhcs/service/admin.py` & `hcs-cli-0.1.28/vhcs/service/admin.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/vhcs/service/lcm.py` & `hcs-cli-0.1.28/vhcs/service/lcm.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/vhcs/service/pki.py` & `hcs-cli-0.1.28/vhcs/service/pki.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/vhcs/service/vmhub.py` & `hcs-cli-0.1.28/vhcs/service/vmhub.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/vhcs/util/duration.py` & `hcs-cli-0.1.28/vhcs/util/duration.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/vhcs/util/pki_util.py` & `hcs-cli-0.1.28/vhcs/util/pki_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/vhcs/util/query_util.py` & `hcs-cli-0.1.28/vhcs/util/query_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.27/vhcs/util/versions.py` & `hcs-cli-0.1.28/vhcs/util/versions.py`

 * *Files identical despite different names*

