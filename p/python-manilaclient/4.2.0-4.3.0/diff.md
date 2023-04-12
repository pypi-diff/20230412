# Comparing `tmp/python-manilaclient-4.2.0.tar.gz` & `tmp/python-manilaclient-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-manilaclient-4.2.0.tar", last modified: Fri Nov 18 15:23:19 2022, max compression
+gzip compressed data, was "python-manilaclient-4.3.0.tar", last modified: Fri Feb 17 12:50:02 2023, max compression
```

## Comparing `python-manilaclient-4.2.0.tar` & `python-manilaclient-4.3.0.tar`

### file list

```diff
@@ -1,439 +1,442 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.960028 python-manilaclient-4.2.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7037 2022-11-18 15:23:19.000000 python-manilaclient-4.2.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      649 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32039 2022-11-18 15:23:19.000000 python-manilaclient-4.2.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2275 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/HACKING
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11837 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5859 2022-11-18 15:23:19.960028 python-manilaclient-4.2.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4088 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      462 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.928022 python-manilaclient-4.2.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/doc/.gitignore
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3188 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/doc/Makefile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.928022 python-manilaclient-4.2.0/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.928022 python-manilaclient-4.2.0/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/doc/source/cli/.gitkeep
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.924021 python-manilaclient-4.2.0/doc/source/cli/osc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.928022 python-manilaclient-4.2.0/doc/source/cli/osc/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4421 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/doc/source/cli/osc/v2/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1695 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/doc/source/cli/osc_plugin_cli.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3599 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.928022 python-manilaclient-4.2.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2761 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8806 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/doc/source/contributor/functional-tests.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1193 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.928022 python-manilaclient-4.2.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2118 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/doc/source/user/api.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1389 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/doc/source/user/shell.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.924021 python-manilaclient-4.2.0/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.928022 python-manilaclient-4.2.0/etc/manilaclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/etc/manilaclient/README.manilaclient.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.928022 python-manilaclient-4.2.0/etc/oslo-config-generator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/etc/oslo-config-generator/manilaclient.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.928022 python-manilaclient-4.2.0/manilaclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1248 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15186 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/api_versions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12161 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2387 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.928022 python-manilaclient-4.2.0/manilaclient/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1131 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/common/_i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.928022 python-manilaclient-4.2.0/manilaclient/common/apiclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/common/apiclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12887 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/common/apiclient/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2781 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/common/apiclient/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8150 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/common/cliutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3503 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/common/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7277 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/common/httpclient.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10524 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1825 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1405 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/extension.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.928022 python-manilaclient-4.2.0/manilaclient/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/osc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4137 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/osc/plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4021 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/osc/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.932023 python-manilaclient-4.2.0/manilaclient/osc/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/osc/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1310 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/osc/v2/availability_zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6631 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/osc/v2/messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14775 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/osc/v2/quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16678 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/osc/v2/security_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4321 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/osc/v2/services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    53134 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/osc/v2/share.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13519 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/osc/v2/share_access_rules.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14824 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/osc/v2/share_group_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6315 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/osc/v2/share_group_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11713 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/osc/v2/share_group_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18730 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/osc/v2/share_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3089 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/osc/v2/share_instance_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7645 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/osc/v2/share_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2202 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/osc/v2/share_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7674 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/osc/v2/share_network_subnets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27489 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/osc/v2/share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3636 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/osc/v2/share_pools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2831 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/osc/v2/share_replica_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13722 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/osc/v2/share_replicas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23444 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/osc/v2/share_servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3244 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/osc/v2/share_snapshot_instance_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5018 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/osc/v2/share_snapshot_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26231 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/osc/v2/share_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3975 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/osc/v2/share_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16122 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/osc/v2/share_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30920 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/shell.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.932023 python-manilaclient-4.2.0/manilaclient/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.932023 python-manilaclient-4.2.0/manilaclient/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20081 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    87123 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2322 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/exceptions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.936023 python-manilaclient-4.2.0/manilaclient/tests/functional/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/osc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15215 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/osc/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      980 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/osc/test_availability_zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4110 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/osc/test_messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7049 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/osc/test_share_access_rules.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3533 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/osc/test_share_group_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1281 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/osc/test_share_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1418 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/osc/test_share_network_subnets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3896 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/osc/test_share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1539 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/osc/test_share_pools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2618 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/osc/test_share_replica_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2248 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/osc/test_share_replicas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2264 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/osc/test_share_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7773 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/osc/test_share_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5408 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/osc/test_share_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8626 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/osc/test_shares.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6111 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/osc/test_shares_group_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2146 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/test_availability_zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2274 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/test_common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6668 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/test_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1002 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/test_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2755 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/test_messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13085 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/test_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1896 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/test_scheduler_stats.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2435 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/test_security_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1729 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/test_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13367 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/test_share_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4622 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/test_share_network_subnets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23687 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/test_share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4371 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/test_share_replica_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1966 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/test_share_replicas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14265 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/test_share_servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20496 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/test_share_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11999 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/test_shares.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14916 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/test_shares_listing.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5391 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/test_shares_metadata.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7615 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/test_snapshot_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4968 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/test_snapshot_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4634 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/test_snapshot_instances_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3584 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/test_snapshots_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4955 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/functional/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.936023 python-manilaclient-4.2.0/manilaclient/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.936023 python-manilaclient-4.2.0/manilaclient/tests/unit/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/common/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.936023 python-manilaclient-4.2.0/manilaclient/tests/unit/common/apiclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/common/apiclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8145 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/common/test_httpclient.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2919 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/fakes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.936023 python-manilaclient-4.2.0/manilaclient/tests/unit/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/osc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6610 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/osc/osc_fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2555 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/osc/osc_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.940024 python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    46247 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1963 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_availability_zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6194 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15984 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19607 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_security_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6858 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    67678 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14621 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_access_rules.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21560 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_group_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17697 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_group_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6874 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_group_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24594 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5208 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_instance_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12339 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3044 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9753 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_network_subnets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27426 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5395 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_pools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3996 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_replica_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21955 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_replicas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24995 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5687 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_snapshot_instance_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8248 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_snapshot_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    39163 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20743 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6357 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14907 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/test_api_versions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2734 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5305 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7759 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/test_functional_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17561 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/test_shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3104 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.940024 python-manilaclient-4.2.0/manilaclient/tests/unit/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1187 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v1/test_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1212 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v1/test_quota_classes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1161 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v1/test_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1206 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v1/test_scheduler_stats.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1240 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v1/test_security_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1171 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v1/test_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1216 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v1/test_share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1208 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v1/test_share_servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1224 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v1/test_share_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1239 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v1/test_share_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1192 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v1/test_share_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1155 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v1/test_shares.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.944025 python-manilaclient-4.2.0/manilaclient/tests/unit/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6889 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v2/fake_clients.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    45444 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v2/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2129 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_availability_zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13669 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5456 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4375 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2780 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_quota_classes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12085 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2962 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_scheduler_stats.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7487 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_security_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3758 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1945 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_share_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9947 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_share_group_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4083 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_share_group_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7915 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_share_group_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11617 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_share_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2142 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_share_instance_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4436 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_share_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3029 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_share_network_subnets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11773 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1894 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_share_replica_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5851 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_share_replicas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11823 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_share_servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1653 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_share_snapshot_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1831 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_share_snapshot_instance_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3612 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_share_snapshot_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8470 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_share_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30366 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_shares.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   156433 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3595 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18918 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2107 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.944025 python-manilaclient-4.2.0/manilaclient/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      917 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10490 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v1/client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.944025 python-manilaclient-4.2.0/manilaclient/v1/contrib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v1/contrib/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1253 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v1/contrib/list_extensions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1225 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v1/limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1260 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v1/quota_classes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1225 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v1/quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1269 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v1/scheduler_stats.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1285 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v1/security_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1235 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v1/services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1265 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v1/share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1260 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v1/share_servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1256 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v1/share_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1285 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v1/share_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1252 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v1/share_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1211 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v1/shares.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.948026 python-manilaclient-4.2.0/manilaclient/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      681 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1313 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v2/availability_zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12841 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v2/client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.948026 python-manilaclient-4.2.0/manilaclient/v2/contrib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v2/contrib/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1448 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v2/contrib/list_extensions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2873 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v2/limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2710 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v2/messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6071 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v2/quota_classes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11053 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v2/quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1528 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v2/scheduler_stats.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5486 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v2/security_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3357 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v2/services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2994 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v2/share_access_rules.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1801 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v2/share_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9326 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v2/share_group_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3695 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v2/share_group_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7367 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v2/share_group_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11213 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v2/share_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1994 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v2/share_instance_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4228 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v2/share_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3358 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v2/share_network_subnets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13094 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v2/share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2943 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v2/share_replica_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10782 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v2/share_replicas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10761 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v2/share_servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1826 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v2/share_snapshot_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1940 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v2/share_snapshot_instance_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2700 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v2/share_snapshot_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8597 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v2/share_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2373 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v2/share_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10288 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v2/share_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31580 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v2/shares.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   215612 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/manilaclient/v2/shell.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.948026 python-manilaclient-4.2.0/playbooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       40 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/playbooks/enable-fips.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.948026 python-manilaclient-4.2.0/playbooks/python-manilaclient-functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/playbooks/python-manilaclient-functional/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/playbooks/python-manilaclient-functional/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.948026 python-manilaclient-4.2.0/python_manilaclient.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5859 2022-11-18 15:23:19.000000 python-manilaclient-4.2.0/python_manilaclient.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19925 2022-11-18 15:23:19.000000 python-manilaclient-4.2.0/python_manilaclient.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-11-18 15:23:19.000000 python-manilaclient-4.2.0/python_manilaclient.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10116 2022-11-18 15:23:19.000000 python-manilaclient-4.2.0/python_manilaclient.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-11-18 15:23:19.000000 python-manilaclient-4.2.0/python_manilaclient.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2022-11-18 15:23:19.000000 python-manilaclient-4.2.0/python_manilaclient.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2022-11-18 15:23:19.000000 python-manilaclient-4.2.0/python_manilaclient.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2022-11-18 15:23:19.000000 python-manilaclient-4.2.0/python_manilaclient.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.948026 python-manilaclient-4.2.0/rally-jobs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1890 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/rally-jobs/rally-manila-no-ss.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4247 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/rally-jobs/rally-manila.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.924021 python-manilaclient-4.2.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.956027 python-manilaclient-4.2.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/Bug-1990013-fix-share-grou-from-snapshot-create-fa3629cf1417ba20.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/add-count-info-in-share-21a6b36c0f4c87b2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/add-dash-dash-help-subcomand-ad4226454aa07bc6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/add-export-location-filter-4cf3114doe40k598.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/add-ipv6-access-type-4dko90r1a9a1e0b8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/add-like-filter-591572762357ef4b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/add-message-list-and-delete-41b3323edd63d894.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/add-metadata-for-share-access-rule-11a6b36c0f4c87c2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/add-per-share-gigabytes-quotas-40bc404bd3cbdd89.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/add-query-params-pools-list-api-12cf1s14ddf40kdd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/add-quota-per-share-type-support-3b2708ea232e69bc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/add-scheduler-hints-to-share-create-70d429cb0aaf8f11.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/add-scheduler-hints-to-share-replica-create-d152a3934e5ad3a7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/add-share-group-quotas-support-b6563cec58209a1d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/add-share-group-support-a3166f6ca4d06a81.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/add-share-network-sec-service-add-update-to-in-use-networks-ec7a60d07ebceaf4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/add-share-replicas-and-replica-gigabytes-quotas-909436c2b2420f2c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/add-snapshot-instances-admin-api-3cf3114doe40k598.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/add-support-filter-search-for-share-type-fdbaaa9510cc59dd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/add-support-to-check-quota-usage-scfdg14dod40k71a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/add_support_multiple_subnet_per_az-46145c3e90e097be.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bp-export-locations-replica-az-commands-03aa32c08f59c42d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bp-integrate-os-profiler-4818066dc2fbf7b7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      339 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bp-ocata-migration-improvements-f63c5d233856fbee.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bp-support-group-spec-search-share-group-type-api-d5d9a6096f084b91.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bp-support-query-user-messages-by-timestamp-34b70bba2d1b4d13.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bp-update-share-type-name-or-description-32d98b5a42cd8090.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1558995-fix-endpoint-not-found.yaml-a06a3b0ba5006718.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1608664-add-support-columns-share-replica-list-885bd8c8b4bfa8f1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1611506-allow-deletion-multiple-resources
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1622540-add-missing-az-list-command-f90265de5c2f261b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1650774-share-instance-reset-state-9c4b26f44b5da0e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      380 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1664877-c462bfad92ce03e5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1674915-allow-user-access-fix-495b3e42bdc985ec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1682726-remove-sort-key-export-location-from-list-885des26bd5ea2de.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1707303-fix-list-command-when-not-given-search-opts-c06af7b344e9cb91.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1709746-add-group-specs-in-share-group-type-create-command-f91265de5c2f251b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1717940-dash-dash-column-reports-nothing-for-capabilities-db8c1234fae91af5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1724183-add-share-type-description-8c4b26f44b5da1e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1733494-allow-user-group-name-with-blank-access-fix-885a3e42bdc985ec.yaml
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      118 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1738917-and-1738918-fix-access-share-group-type-by-name-3a8760522c147f28.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1798229-fix-create-share-from-snap-using-name-44100b907ea6a040.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1799934-add-ou-parameter-260f9aaf939d1919.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1802059-fix-is_default-a8d3d95ffa0aede9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1811516-bug-1811627-python3-fixes-4b26130027b2c076.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1814094-fix-_get_base_url-method-168e12292aeec8f1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1830677-fix-13b30d6a89f43246.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1855391-support-force-extend-share-6b5ebcfe1de0ca7b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1871252-update-default-quotas-via-quota-class-share-groups-share-group-snapshots-20ec1dfcc0a7e81c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1898304-add-wait-to-share-create-delete-f121073f2f4402ff.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1898308-add-wait-to-share-extend-shrink-c9cc413c50d9832a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1898309-add-wait-to-share-manage-unmanage-d2060c61cc295bfd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1898315-add-wait-flag-to-manage-share-server-operation-be6488c2a57536e1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1898316-add-wait-option-for-deleting-a-share-server-e2228018585de5cb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1898317-add-wait-option-for-force-deleting-share-snapshot-share-instance-fb2531b6033f0ae5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1898318-add-wait-flag-for-deleting-a-share-group-operation-c602ba9faad411be.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1898318-add-wait-flag-to-create-sharee-group-operation-cd8310b241d377b0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1899325-implement-usage-of-c-or-column-without-additional-logic-2970ee294f32bd31.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1902873-fix-py-raw-error-msg-a839fee2ac7b9d3d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1909477-fix-forbid-users-to-create-shares-with-the-name-none-cfb0a59baa597803.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1920888-fix-error-in-cli-manila-list-with-sorting-key-availabilityzone-cea5a1f5d8a38fc3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1925486-add-share-network-option-to-replica-create-api-7d2ff3628e93fc77.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1953670-fix-id-attr-for-share-group-type-access-repr-008338a53d7a6a50.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1959329-fix-server-listing-by-subnets-fa6447fd43093cae.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1960422-fix-no-default-share-type-d6191ea0aa1e57fa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1975488-skip-force-kwarg-if-unspecified-f98c717df1d6e364.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-1980985-dont-use-share-type-with-snapshot-ref-de0331c640afbbd3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug-share-access-list-3cf3114doe40k599.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug_1570085_fix-905786b797379309.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug_1603387_fix_env_variable_8ed5450aab41aa5f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug_1606168_fix-54d3c3bb78389f01.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug_1715769_fix-3ec701b0fb9d7910.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug_1777849_1779935_fix-344cb8f09b7df502.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/bug_1782672-1954059b373f03de.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      589 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/deprecate-v1-a0cfa6fd723c2f46.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/drop-py36-and-py37-85cf389b2842f045.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/drop-python2-support-71c7b9e1dcf8c890.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/expose-access-key-in-access-list-API-b57c386c9048ae55.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/fix-and-improve-access-rules-a118a7f8e22f65bb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/fix-is-default-empty-557844001e0401e2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      499 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/graduate-share-replication-feature-49770e921b4338fb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/handle-missing-api-minor-version-5a6d242f28883442.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/manage-unmanage-share-servers-8c7b27a1fe80e5fa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/manila-client-support-recycle-bin-4ecb5de770bd525f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2119 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/manila-openstackclient-bf61ceb270d3afb7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/migration-share-type-4fc3b7c6187f5201.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/mountable_snapshot-ced01da7dffc6d7e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/newton-migration-improvements-166a03472948bdef.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      582 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/remove-experimental-flag-from-share-groups-feature-dcf2b0b67fe4cac4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/remove-nova-net-id-option-for-share-nets-82e424b75221528b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      550 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/share-network-multiple-subnets-732309abfbf5987c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/share-revert-to-snapshot-e899a4b7e1126749.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      304 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/share_type-skip-format-119595e62900e571.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/start-using-reno-b744cd0259c7a88c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/support-create-share-from-snapshot-extra-spec-cdba92f179c1c5c6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      322 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/support-share-server-migration-9804752270c6b153.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/support-show-type-6380b7c539c95ba8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/type-create-extra-specs-691572762357ef3b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/update-api-version-create-share-from-snapshot-another-pool-or-backend-694cfda84a41c4ff.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/notes/v2-0-0-deprecated-opts-removal-863565618535733d.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.956027 python-manilaclient-4.2.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.956027 python-manilaclient-4.2.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.956027 python-manilaclient-4.2.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8911 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      847 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.924021 python-manilaclient-4.2.0/roles/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.956027 python-manilaclient-4.2.0/roles/populate-manilaclient-config/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1257 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/roles/populate-manilaclient-config/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.956027 python-manilaclient-4.2.0/roles/populate-manilaclient-config/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/roles/populate-manilaclient-config/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.956027 python-manilaclient-4.2.0/roles/populate-manilaclient-config/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2538 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/roles/populate-manilaclient-config/tasks/main.yaml
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5570 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/run_tests.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11142 2022-11-18 15:23:19.960028 python-manilaclient-4.2.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      241 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.956027 python-manilaclient-4.2.0/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      367 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/tools/manila.bash_completion
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2648 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 15:23:19.960028 python-manilaclient-4.2.0/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      492 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/zuul.d/project.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4755 2022-11-18 15:22:52.000000 python-manilaclient-4.2.0/zuul.d/python-manilaclient-jobs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.040638 python-manilaclient-4.3.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7070 2023-02-17 12:50:01.000000 python-manilaclient-4.3.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      649 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32302 2023-02-17 12:50:01.000000 python-manilaclient-4.3.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2275 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/HACKING
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11837 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5859 2023-02-17 12:50:02.040638 python-manilaclient-4.3.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4088 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      462 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.000640 python-manilaclient-4.3.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/doc/.gitignore
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3188 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/doc/Makefile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.000640 python-manilaclient-4.3.0/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.000640 python-manilaclient-4.3.0/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/doc/source/cli/.gitkeep
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:01.996641 python-manilaclient-4.3.0/doc/source/cli/osc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.000640 python-manilaclient-4.3.0/doc/source/cli/osc/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4421 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/doc/source/cli/osc/v2/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1695 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/doc/source/cli/osc_plugin_cli.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3599 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.000640 python-manilaclient-4.3.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2761 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8806 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/doc/source/contributor/functional-tests.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1193 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.000640 python-manilaclient-4.3.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2118 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/doc/source/user/api.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1389 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/doc/source/user/shell.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:01.996641 python-manilaclient-4.3.0/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.000640 python-manilaclient-4.3.0/etc/manilaclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/etc/manilaclient/README.manilaclient.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.000640 python-manilaclient-4.3.0/etc/oslo-config-generator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/etc/oslo-config-generator/manilaclient.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.000640 python-manilaclient-4.3.0/manilaclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1248 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15186 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/api_versions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18067 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2387 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.004640 python-manilaclient-4.3.0/manilaclient/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1131 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/common/_i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.004640 python-manilaclient-4.3.0/manilaclient/common/apiclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/common/apiclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12887 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/common/apiclient/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2781 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/common/apiclient/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8150 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/common/cliutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3503 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/common/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7277 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/common/httpclient.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10524 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1825 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1405 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/extension.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.004640 python-manilaclient-4.3.0/manilaclient/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4137 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4021 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.008640 python-manilaclient-4.3.0/manilaclient/osc/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1310 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/availability_zones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6631 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14775 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16678 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/security_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4321 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    53048 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13519 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_access_rules.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14824 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_group_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6315 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_group_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11713 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_group_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18730 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3089 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_instance_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7645 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2202 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7674 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_network_subnets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27489 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3636 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_pools.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2831 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_replica_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14367 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_replicas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23898 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3244 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_snapshot_instance_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5018 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_snapshot_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29068 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3975 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16122 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31317 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/shell.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.008640 python-manilaclient-4.3.0/manilaclient/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.012640 python-manilaclient-4.3.0/manilaclient/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20087 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    87123 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2322 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/exceptions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.012640 python-manilaclient-4.3.0/manilaclient/tests/functional/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/osc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15215 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/osc/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      980 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_availability_zones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4110 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7049 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_access_rules.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3533 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_group_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1281 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1418 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_network_subnets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3896 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1539 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_pools.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2618 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_replica_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2248 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_replicas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2264 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7773 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5408 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8626 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_shares.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6111 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_shares_group_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2146 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_availability_zones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2442 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6668 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1002 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2755 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13085 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1896 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_scheduler_stats.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2435 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_security_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1729 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13367 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_share_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4622 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_share_network_subnets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23687 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4371 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_share_replica_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1966 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_share_replicas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14265 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_share_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20496 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_share_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11999 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_shares.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14916 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_shares_listing.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5391 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_shares_metadata.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7615 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_snapshot_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4968 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_snapshot_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4634 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_snapshot_instances_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3584 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_snapshots_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4955 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.012640 python-manilaclient-4.3.0/manilaclient/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.012640 python-manilaclient-4.3.0/manilaclient/tests/unit/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/common/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.012640 python-manilaclient-4.3.0/manilaclient/tests/unit/common/apiclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/common/apiclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8145 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/common/test_httpclient.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2919 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.012640 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6610 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/osc_fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2555 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/osc_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.016639 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    46247 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1963 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_availability_zones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6194 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15984 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19607 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_security_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6858 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    67674 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14621 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_access_rules.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21560 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_group_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17697 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_group_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6874 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_group_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24594 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5208 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_instance_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12339 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3044 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9753 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_network_subnets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27426 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5395 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_pools.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3996 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_replica_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22544 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_replicas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24995 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5687 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_snapshot_instance_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8248 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_snapshot_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    43220 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20743 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6357 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14907 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/test_api_versions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2734 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5305 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/test_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7759 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/test_functional_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17744 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/test_shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3104 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.016639 python-manilaclient-4.3.0/manilaclient/tests/unit/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1187 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1212 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_quota_classes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1161 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1206 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_scheduler_stats.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1240 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_security_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1171 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1216 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1208 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_share_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1224 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_share_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1239 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_share_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1192 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_share_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1155 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_shares.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.020639 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6889 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/fake_clients.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    46114 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2129 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_availability_zones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13669 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5456 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4375 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2780 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_quota_classes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12085 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2962 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_scheduler_stats.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7487 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_security_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3758 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1945 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9947 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_group_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4083 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_group_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7915 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_group_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11617 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2142 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_instance_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4436 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3029 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_network_subnets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11773 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1894 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_replica_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5851 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_replicas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11823 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1653 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_snapshot_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1831 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_snapshot_instance_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3612 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_snapshot_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9545 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30366 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_shares.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   156971 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3595 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18918 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2107 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.024639 python-manilaclient-4.3.0/manilaclient/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      917 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10490 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v1/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.024639 python-manilaclient-4.3.0/manilaclient/v1/contrib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v1/contrib/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1253 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v1/contrib/list_extensions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1225 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v1/limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1260 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v1/quota_classes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1225 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v1/quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1269 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v1/scheduler_stats.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1285 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v1/security_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1235 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v1/services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1265 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v1/share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1260 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v1/share_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1256 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v1/share_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1285 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v1/share_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1252 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v1/share_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1211 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v1/shares.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.024639 python-manilaclient-4.3.0/manilaclient/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      681 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1313 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/availability_zones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12841 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.028639 python-manilaclient-4.3.0/manilaclient/v2/contrib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/contrib/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1448 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/contrib/list_extensions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2873 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2710 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6071 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/quota_classes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11053 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1528 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/scheduler_stats.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5486 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/security_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3357 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2994 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_access_rules.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1801 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9326 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_group_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3695 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_group_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7367 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_group_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11213 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1994 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_instance_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4228 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3358 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_network_subnets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13094 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2943 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_replica_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11234 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_replicas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10761 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1826 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_snapshot_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1940 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_snapshot_instance_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2700 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_snapshot_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9276 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2373 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10288 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30069 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/shares.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   216521 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/shell.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.028639 python-manilaclient-4.3.0/playbooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       40 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/playbooks/enable-fips.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.028639 python-manilaclient-4.3.0/playbooks/python-manilaclient-functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/playbooks/python-manilaclient-functional/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/playbooks/python-manilaclient-functional/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.028639 python-manilaclient-4.3.0/python_manilaclient.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5859 2023-02-17 12:50:01.000000 python-manilaclient-4.3.0/python_manilaclient.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20135 2023-02-17 12:50:01.000000 python-manilaclient-4.3.0/python_manilaclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-17 12:50:01.000000 python-manilaclient-4.3.0/python_manilaclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10116 2023-02-17 12:50:01.000000 python-manilaclient-4.3.0/python_manilaclient.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-17 12:50:01.000000 python-manilaclient-4.3.0/python_manilaclient.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-02-17 12:50:01.000000 python-manilaclient-4.3.0/python_manilaclient.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2023-02-17 12:50:01.000000 python-manilaclient-4.3.0/python_manilaclient.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2023-02-17 12:50:01.000000 python-manilaclient-4.3.0/python_manilaclient.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.028639 python-manilaclient-4.3.0/rally-jobs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1890 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/rally-jobs/rally-manila-no-ss.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4247 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/rally-jobs/rally-manila.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:01.996641 python-manilaclient-4.3.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.040638 python-manilaclient-4.3.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/Bug-1990013-fix-share-grou-from-snapshot-create-fa3629cf1417ba20.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-count-info-in-share-21a6b36c0f4c87b2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-dash-dash-help-subcomand-ad4226454aa07bc6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-export-location-filter-4cf3114doe40k598.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-ipv6-access-type-4dko90r1a9a1e0b8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-like-filter-591572762357ef4b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-message-list-and-delete-41b3323edd63d894.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-metadata-for-share-access-rule-11a6b36c0f4c87c2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-per-share-gigabytes-quotas-40bc404bd3cbdd89.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-query-params-pools-list-api-12cf1s14ddf40kdd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-quiesce-wait-time-for-replica-promote-30d9fa66afc854f2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-quota-per-share-type-support-3b2708ea232e69bc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-scheduler-hints-to-share-create-70d429cb0aaf8f11.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-scheduler-hints-to-share-replica-create-d152a3934e5ad3a7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-share-group-quotas-support-b6563cec58209a1d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-share-group-support-a3166f6ca4d06a81.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-share-network-sec-service-add-update-to-in-use-networks-ec7a60d07ebceaf4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-share-replicas-and-replica-gigabytes-quotas-909436c2b2420f2c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-snapshot-instances-admin-api-3cf3114doe40k598.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-snapshot-metadata-49b0288bf2f12bf0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-support-filter-search-for-share-type-fdbaaa9510cc59dd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-support-to-check-quota-usage-scfdg14dod40k71a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add_support_multiple_subnet_per_az-46145c3e90e097be.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bp-export-locations-replica-az-commands-03aa32c08f59c42d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bp-integrate-os-profiler-4818066dc2fbf7b7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      339 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bp-ocata-migration-improvements-f63c5d233856fbee.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bp-support-group-spec-search-share-group-type-api-d5d9a6096f084b91.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bp-support-query-user-messages-by-timestamp-34b70bba2d1b4d13.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bp-update-share-type-name-or-description-32d98b5a42cd8090.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1558995-fix-endpoint-not-found.yaml-a06a3b0ba5006718.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1608664-add-support-columns-share-replica-list-885bd8c8b4bfa8f1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1611506-allow-deletion-multiple-resources
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1622540-add-missing-az-list-command-f90265de5c2f261b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1650774-share-instance-reset-state-9c4b26f44b5da0e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      380 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1664877-c462bfad92ce03e5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1674915-allow-user-access-fix-495b3e42bdc985ec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1682726-remove-sort-key-export-location-from-list-885des26bd5ea2de.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1707303-fix-list-command-when-not-given-search-opts-c06af7b344e9cb91.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1709746-add-group-specs-in-share-group-type-create-command-f91265de5c2f251b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1717940-dash-dash-column-reports-nothing-for-capabilities-db8c1234fae91af5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1724183-add-share-type-description-8c4b26f44b5da1e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1733494-allow-user-group-name-with-blank-access-fix-885a3e42bdc985ec.yaml
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      118 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1738917-and-1738918-fix-access-share-group-type-by-name-3a8760522c147f28.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1798229-fix-create-share-from-snap-using-name-44100b907ea6a040.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1799934-add-ou-parameter-260f9aaf939d1919.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1802059-fix-is_default-a8d3d95ffa0aede9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1811516-bug-1811627-python3-fixes-4b26130027b2c076.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1814094-fix-_get_base_url-method-168e12292aeec8f1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1830677-fix-13b30d6a89f43246.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1855391-support-force-extend-share-6b5ebcfe1de0ca7b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1871252-update-default-quotas-via-quota-class-share-groups-share-group-snapshots-20ec1dfcc0a7e81c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1898304-add-wait-to-share-create-delete-f121073f2f4402ff.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1898308-add-wait-to-share-extend-shrink-c9cc413c50d9832a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1898309-add-wait-to-share-manage-unmanage-d2060c61cc295bfd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1898315-add-wait-flag-to-manage-share-server-operation-be6488c2a57536e1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1898316-add-wait-option-for-deleting-a-share-server-e2228018585de5cb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1898317-add-wait-option-for-force-deleting-share-snapshot-share-instance-fb2531b6033f0ae5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1898318-add-wait-flag-for-deleting-a-share-group-operation-c602ba9faad411be.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1898318-add-wait-flag-to-create-sharee-group-operation-cd8310b241d377b0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1899325-implement-usage-of-c-or-column-without-additional-logic-2970ee294f32bd31.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1902873-fix-py-raw-error-msg-a839fee2ac7b9d3d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1909477-fix-forbid-users-to-create-shares-with-the-name-none-cfb0a59baa597803.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1920888-fix-error-in-cli-manila-list-with-sorting-key-availabilityzone-cea5a1f5d8a38fc3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1925486-add-share-network-option-to-replica-create-api-7d2ff3628e93fc77.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1953670-fix-id-attr-for-share-group-type-access-repr-008338a53d7a6a50.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1959329-fix-server-listing-by-subnets-fa6447fd43093cae.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1960422-fix-no-default-share-type-d6191ea0aa1e57fa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1975488-skip-force-kwarg-if-unspecified-f98c717df1d6e364.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1980985-dont-use-share-type-with-snapshot-ref-de0331c640afbbd3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1999775-add-os-key-0cfc95c7b480df05.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-share-access-list-3cf3114doe40k599.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug_1570085_fix-905786b797379309.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug_1603387_fix_env_variable_8ed5450aab41aa5f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug_1606168_fix-54d3c3bb78389f01.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug_1715769_fix-3ec701b0fb9d7910.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug_1777849_1779935_fix-344cb8f09b7df502.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug_1782672-1954059b373f03de.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      589 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/deprecate-v1-a0cfa6fd723c2f46.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/drop-py36-and-py37-85cf389b2842f045.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/drop-python2-support-71c7b9e1dcf8c890.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/expose-access-key-in-access-list-API-b57c386c9048ae55.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/fix-and-improve-access-rules-a118a7f8e22f65bb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/fix-is-default-empty-557844001e0401e2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      499 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/graduate-share-replication-feature-49770e921b4338fb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/handle-missing-api-minor-version-5a6d242f28883442.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/manage-unmanage-share-servers-8c7b27a1fe80e5fa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/manila-client-support-recycle-bin-4ecb5de770bd525f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2119 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/manila-openstackclient-bf61ceb270d3afb7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/migration-share-type-4fc3b7c6187f5201.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/mountable_snapshot-ced01da7dffc6d7e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/newton-migration-improvements-166a03472948bdef.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      582 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/remove-experimental-flag-from-share-groups-feature-dcf2b0b67fe4cac4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/remove-nova-net-id-option-for-share-nets-82e424b75221528b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      550 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/share-network-multiple-subnets-732309abfbf5987c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/share-revert-to-snapshot-e899a4b7e1126749.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      304 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/share_type-skip-format-119595e62900e571.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/start-using-reno-b744cd0259c7a88c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/support-create-share-from-snapshot-extra-spec-cdba92f179c1c5c6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      322 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/support-share-server-migration-9804752270c6b153.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/support-show-type-6380b7c539c95ba8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/type-create-extra-specs-691572762357ef3b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/update-api-version-create-share-from-snapshot-another-pool-or-backend-694cfda84a41c4ff.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/v2-0-0-deprecated-opts-removal-863565618535733d.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.040638 python-manilaclient-4.3.0/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.040638 python-manilaclient-4.3.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.040638 python-manilaclient-4.3.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8911 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      847 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:01.996641 python-manilaclient-4.3.0/roles/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.040638 python-manilaclient-4.3.0/roles/populate-manilaclient-config/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1257 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/roles/populate-manilaclient-config/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.040638 python-manilaclient-4.3.0/roles/populate-manilaclient-config/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/roles/populate-manilaclient-config/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.040638 python-manilaclient-4.3.0/roles/populate-manilaclient-config/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2538 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/roles/populate-manilaclient-config/tasks/main.yaml
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5570 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/run_tests.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11142 2023-02-17 12:50:02.044638 python-manilaclient-4.3.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      241 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.040638 python-manilaclient-4.3.0/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      367 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/tools/manila.bash_completion
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2595 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.040638 python-manilaclient-4.3.0/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      492 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/zuul.d/project.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4755 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/zuul.d/python-manilaclient-jobs.yaml
```

### Comparing `python-manilaclient-4.2.0/AUTHORS` & `python-manilaclient-4.3.0/AUTHORS`

 * *Files 1% similar despite different names*

```diff
@@ -143,14 +143,15 @@
 ji-xuepeng <ji.xuepeng@zte.com.cn>
 junboli <junbo85.li@gmail.com>
 kafilat-adeleke <adelekekafilatadenike@gmail.com>
 kayrus <kay.diam@gmail.com>
 kedy <zhao.kaiA@h3c.com>
 kpdev <kinpaa@gmail.com>
 kuangcx <kuangcx@inspur.com>
+kushalaa <kushi.hande@gmail.com>
 lijunbo <lijunbo@fiberhome.com>
 lingyongxu <lyxu@fiberhome.com>
 liusheng <liusheng@huawei.com>
 liuyamin <liuyamin@fiberhome.com>
 lkuchlan <lkuchlan@redhat.com>
 luke.li <lilu7189@fiberhome.com>
 maaoyu <maaoyu@inspur.com>
```

### Comparing `python-manilaclient-4.2.0/CONTRIBUTING.rst` & `python-manilaclient-4.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/ChangeLog` & `python-manilaclient-4.3.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 CHANGES
 =======
 
+4.3.0
+-----
+
+* Add quiesce\_wait\_time for replica promote
+* Metadata for Share Snapshots
+* Drop duplicate tox config
+* Fix tox4 errors
+* Support --os-key option
+* Fix functional tests failing with python 3.10
+* Fix formatting of OSC server migration check-only
+
 4.2.0
 -----
 
 * Fix the Create Share Group from Snap Shot create
 * Respect OS\_CACERT when using Manila OSC plugin
 * Switch to 2023.1 Python3 unit tests and generic template name
 * Update master for stable/zed
```

### Comparing `python-manilaclient-4.2.0/HACKING` & `python-manilaclient-4.3.0/HACKING`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/LICENSE` & `python-manilaclient-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/PKG-INFO` & `python-manilaclient-4.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-manilaclient
-Version: 4.2.0
+Version: 4.3.0
 Summary: Client library for OpenStack Manila API.
 Home-page: https://docs.openstack.org/python-manilaclient/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `python-manilaclient-4.2.0/README.rst` & `python-manilaclient-4.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/doc/Makefile` & `python-manilaclient-4.3.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/doc/source/cli/osc/v2/index.rst` & `python-manilaclient-4.3.0/doc/source/cli/osc/v2/index.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/doc/source/cli/osc_plugin_cli.rst` & `python-manilaclient-4.3.0/doc/source/cli/osc_plugin_cli.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/doc/source/conf.py` & `python-manilaclient-4.3.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/doc/source/contributor/contributing.rst` & `python-manilaclient-4.3.0/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/doc/source/contributor/functional-tests.rst` & `python-manilaclient-4.3.0/doc/source/contributor/functional-tests.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/doc/source/index.rst` & `python-manilaclient-4.3.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/doc/source/user/api.rst` & `python-manilaclient-4.3.0/doc/source/user/api.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/doc/source/user/shell.rst` & `python-manilaclient-4.3.0/doc/source/user/shell.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/__init__.py` & `python-manilaclient-4.3.0/manilaclient/__init__.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/api_versions.py` & `python-manilaclient-4.3.0/manilaclient/api_versions.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from manilaclient.common import cliutils
 from manilaclient.common import constants
 from manilaclient import exceptions
 from manilaclient import utils
 
 LOG = logging.getLogger(__name__)
 
-MAX_VERSION = '2.72'
+MAX_VERSION = '2.75'
 MIN_VERSION = '2.0'
 DEPRECATED_VERSION = '1.0'
 _VERSIONED_METHOD_MAP = {}
 
 
 class APIVersion(object):
     """Top level object to support Manila API Versioning.
```

### Comparing `python-manilaclient-4.2.0/manilaclient/client.py` & `python-manilaclient-4.3.0/manilaclient/client.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/common/_i18n.py` & `python-manilaclient-4.3.0/manilaclient/common/_i18n.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/common/apiclient/exceptions.py` & `python-manilaclient-4.3.0/manilaclient/common/apiclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/common/apiclient/utils.py` & `python-manilaclient-4.3.0/manilaclient/common/apiclient/utils.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/common/cliutils.py` & `python-manilaclient-4.3.0/manilaclient/common/cliutils.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/common/constants.py` & `python-manilaclient-4.3.0/manilaclient/common/constants.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/common/httpclient.py` & `python-manilaclient-4.3.0/manilaclient/common/httpclient.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/config.py` & `python-manilaclient-4.3.0/manilaclient/config.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/exceptions.py` & `python-manilaclient-4.3.0/manilaclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/extension.py` & `python-manilaclient-4.3.0/manilaclient/extension.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/osc/plugin.py` & `python-manilaclient-4.3.0/manilaclient/osc/plugin.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/osc/utils.py` & `python-manilaclient-4.3.0/manilaclient/osc/utils.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/osc/v2/availability_zones.py` & `python-manilaclient-4.3.0/manilaclient/osc/v2/availability_zones.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/osc/v2/messages.py` & `python-manilaclient-4.3.0/manilaclient/osc/v2/messages.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/osc/v2/quotas.py` & `python-manilaclient-4.3.0/manilaclient/osc/v2/quotas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/osc/v2/security_services.py` & `python-manilaclient-4.3.0/manilaclient/osc/v2/security_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/osc/v2/services.py` & `python-manilaclient-4.3.0/manilaclient/osc/v2/services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/osc/v2/share.py` & `python-manilaclient-4.3.0/manilaclient/osc/v2/share.py`

 * *Files 1% similar despite different names*

```diff
@@ -761,16 +761,15 @@
         share_client = self.app.client_manager.share
         share_obj = apiutils.find_resource(share_client.shares,
                                            parsed_args.share)
         result = 0
 
         if parsed_args.property:
             try:
-                share_client.shares.set_metadata(
-                    share_obj.id, parsed_args.property)
+                share_obj.set_metadata(parsed_args.property)
             except Exception as e:
                 LOG.error(_("Failed to set share properties "
                             "'%(properties)s': %(exception)s"),
                           {'properties': parsed_args.property,
                            'exception': e})
                 result += 1
 
@@ -856,16 +855,15 @@
                 LOG.error(_("Failed to unset share display name "
                             "or display description: %s"), e)
                 result += 1
 
         if parsed_args.property:
             for key in parsed_args.property:
                 try:
-                    share_client.shares.delete_metadata(
-                        share_obj.id, [key])
+                    share_obj.delete_metadata([key])
                 except Exception as e:
                     LOG.error(_("Failed to unset share property "
                                 "'%(key)s': %(e)s"),
                               {'key': key, 'e': e})
                     result += 1
 
         if result > 0:
@@ -1214,17 +1212,17 @@
             metavar="<share>",
             help=_('Name or ID of share')
         )
         return parser
 
     def take_action(self, parsed_args):
         share_client = self.app.client_manager.share
-        share = apiutils.find_resource(
+        share_obj = apiutils.find_resource(
             share_client.shares, parsed_args.share)
-        share_properties = share_client.shares.get_metadata(share)
+        share_properties = share_client.shares.get_metadata(share_obj)
 
         return self.dict2columns(share_properties._info)
 
 
 class RevertShare(command.Command):
     """Revert a share to snapshot."""
```

### Comparing `python-manilaclient-4.2.0/manilaclient/osc/v2/share_access_rules.py` & `python-manilaclient-4.3.0/manilaclient/osc/v2/share_access_rules.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/osc/v2/share_group_snapshots.py` & `python-manilaclient-4.3.0/manilaclient/osc/v2/share_group_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/osc/v2/share_group_type_access.py` & `python-manilaclient-4.3.0/manilaclient/osc/v2/share_group_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/osc/v2/share_group_types.py` & `python-manilaclient-4.3.0/manilaclient/osc/v2/share_group_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/osc/v2/share_groups.py` & `python-manilaclient-4.3.0/manilaclient/osc/v2/share_groups.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/osc/v2/share_instance_export_locations.py` & `python-manilaclient-4.3.0/manilaclient/osc/v2/share_instance_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/osc/v2/share_instances.py` & `python-manilaclient-4.3.0/manilaclient/osc/v2/share_instances.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/osc/v2/share_limits.py` & `python-manilaclient-4.3.0/manilaclient/osc/v2/share_limits.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/osc/v2/share_network_subnets.py` & `python-manilaclient-4.3.0/manilaclient/osc/v2/share_network_subnets.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/osc/v2/share_networks.py` & `python-manilaclient-4.3.0/manilaclient/osc/v2/share_networks.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/osc/v2/share_pools.py` & `python-manilaclient-4.3.0/manilaclient/osc/v2/share_pools.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/osc/v2/share_replica_export_locations.py` & `python-manilaclient-4.3.0/manilaclient/osc/v2/share_replica_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/osc/v2/share_replicas.py` & `python-manilaclient-4.3.0/manilaclient/osc/v2/share_replicas.py`

 * *Files 2% similar despite different names*

```diff
@@ -345,25 +345,42 @@
     def get_parser(self, prog_name):
         parser = super(PromoteShareReplica, self).get_parser(prog_name)
         parser.add_argument(
             "replica",
             metavar="<replica>",
             help=_("ID of the share replica.")
         )
+        parser.add_argument(
+            '--quiesce-wait-time',
+            metavar='<quiesce-wait-time>',
+            default=None,
+            help=_('Quiesce wait time in seconds. Available for '
+                   'microversion >= 2.75')
+        )
         return parser
 
     def take_action(self, parsed_args):
         share_client = self.app.client_manager.share
 
         replica = osc_utils.find_resource(
             share_client.share_replicas,
             parsed_args.replica)
 
+        args = [
+            replica,
+        ]
+        if parsed_args.quiesce_wait_time:
+            if share_client.api_version < api_versions.APIVersion("2.75"):
+                raise exceptions.CommandError(
+                    "'quiesce-wait-time' option is available only starting "
+                    "with '2.75' API microversion.")
+            args += [parsed_args.quiesce_wait_time]
+
         try:
-            share_client.share_replicas.promote(replica)
+            share_client.share_replicas.promote(*args)
         except Exception as e:
             raise exceptions.CommandError(_(
                 "Failed to promote replica to 'active': %s" % (e)))
 
 
 class ResyncShareReplica(command.Command):
     """Resync share replica"""
```

### Comparing `python-manilaclient-4.2.0/manilaclient/osc/v2/share_servers.py` & `python-manilaclient-4.3.0/manilaclient/osc/v2/share_servers.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from osc_lib.command import command
 from osc_lib import exceptions
 from osc_lib import utils as osc_utils
 
 from manilaclient import api_versions
 from manilaclient.common._i18n import _
 from manilaclient.common.apiclient import utils as apiutils
+from manilaclient.common import cliutils
 from manilaclient.common import constants
 
 LOG = logging.getLogger(__name__)
 
 
 class DeleteShareServer(command.Command):
     """Delete one or more share servers (Admin only)"""
@@ -620,14 +621,22 @@
             if parsed_args.check_only:
                 result = share_server.migration_check(
                     parsed_args.host, parsed_args.writable,
                     parsed_args.nondisruptive, parsed_args.preserve_snapshots,
                     new_share_net_id
                 )
             if result:
+                if parsed_args.formatter == 'table':
+                    for k, v in result.items():
+                        if isinstance(v, dict):
+                            capabilities_list = [v]
+                            dict_values = cliutils.convert_dict_list_to_string(
+                                capabilities_list
+                            )
+                            result[k] = dict_values
                 return self.dict2columns(result)
             else:
                 share_server.migration_start(parsed_args.host,
                                              parsed_args.writable,
                                              parsed_args.nondisruptive,
                                              parsed_args.preserve_snapshots,
                                              new_share_net_id)
```

### Comparing `python-manilaclient-4.2.0/manilaclient/osc/v2/share_snapshot_instance_export_locations.py` & `python-manilaclient-4.3.0/manilaclient/osc/v2/share_snapshot_instance_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/osc/v2/share_snapshot_instances.py` & `python-manilaclient-4.3.0/manilaclient/osc/v2/share_snapshot_instances.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/osc/v2/share_snapshots.py` & `python-manilaclient-4.3.0/manilaclient/osc/v2/share_snapshots.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,22 +8,24 @@
 #   distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #   WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #   License for the specific language governing permissions and limitations
 #   under the License.
 
 import logging
 
+from osc_lib.cli import format_columns
 from osc_lib.cli import parseractions
 from osc_lib.command import command
 from osc_lib import exceptions
 from osc_lib import utils
 
 from manilaclient import api_versions
 from manilaclient.common._i18n import _
 from manilaclient.common import cliutils
+from manilaclient.osc import utils as oscutils
 
 LOG = logging.getLogger(__name__)
 
 
 class CreateShareSnapshot(command.ShowOne):
     """Create a share snapshot."""
     _description = _(
@@ -57,27 +59,44 @@
         )
         parser.add_argument(
             '--wait',
             action='store_true',
             default=False,
             help=_('Wait for share snapshot creation')
         )
+        parser.add_argument(
+            "--property",
+            metavar="<key=value>",
+            default={},
+            action=parseractions.KeyValueAction,
+            help=_("Set a property to this snapshot "
+                   "(repeat option to set multiple properties)."
+                   "Available only for microversion >= 2.73"),
+        )
         return parser
 
     def take_action(self, parsed_args):
         share_client = self.app.client_manager.share
 
         share = utils.find_resource(share_client.shares,
                                     parsed_args.share)
 
+        if share_client.api_version >= api_versions.APIVersion("2.73"):
+            property = parsed_args.property or {}
+        elif parsed_args.property:
+            raise exceptions.CommandError(
+                "Setting metadtaa is only available with manila API version "
+                ">= 2.73")
+
         share_snapshot = share_client.share_snapshots.create(
             share=share,
             force=parsed_args.force,
             name=parsed_args.name or None,
-            description=parsed_args.description or None
+            description=parsed_args.description or None,
+            metadata=property
         )
         if parsed_args.wait:
             if not utils.wait_for_status(
                 status_f=share_client.share_snapshots.get,
                 res_id=share_snapshot.id,
                 success_status=['available']
             ):
@@ -184,14 +203,22 @@
 
         if parsed_args.formatter == 'table':
             locations = cliutils.convert_dict_list_to_string(
                 locations)
 
         data = share_snapshot._info
         data['export_locations'] = locations
+        # Special mapping for columns to make the output easier to read:
+        # 'metadata' --> 'properties'
+        data.update(
+            {
+                'properties':
+                    format_columns.DictColumn(data.pop('metadata', {})),
+            },
+        )
         data.pop('links', None)
 
         return self.dict2columns(data)
 
 
 class SetShareSnapshot(command.Command):
     """Set share snapshot properties."""
@@ -224,14 +251,22 @@
                      'unmanage_starting', 'unmanage_error',
                      'error_deleting'],
             help=_("Assign a status to the snapshot (Admin only). "
                    "Options include : available, error, creating, "
                    "deleting, manage_starting, manage_error, "
                    "unmanage_starting, unmanage_error, error_deleting.")
         )
+        parser.add_argument(
+            "--property",
+            metavar="<key=value>",
+            default={},
+            action=parseractions.KeyValueAction,
+            help=_("Set a property to this snapshot "
+                   "(repeat option to set multiple properties)"),
+        )
         return parser
 
     def take_action(self, parsed_args):
         share_client = self.app.client_manager.share
         result = 0
 
         share_snapshot = utils.find_resource(
@@ -266,15 +301,23 @@
                 )
             except Exception as e:
                 result += 1
                 LOG.error(_(
                     "Failed to update snapshot status to "
                     "'%(status)s': %(e)s"),
                     {'status': parsed_args.status, 'e': e})
-
+        if parsed_args.property:
+            try:
+                share_snapshot.set_metadata(parsed_args.property)
+            except Exception as e:
+                LOG.error(_("Failed to set share snapshot properties "
+                            "'%(properties)s': %(exception)s"),
+                          {'properties': parsed_args.property,
+                           'exception': e})
+                result += 1
         if result > 0:
             raise exceptions.CommandError(_("One or more of the "
                                           "set operations failed"))
 
 
 class UnsetShareSnapshot(command.Command):
     """Unset a share snapshot property."""
@@ -293,14 +336,21 @@
             help=_("Unset snapshot name."),
         )
         parser.add_argument(
             "--description",
             action='store_true',
             help=_("Unset snapshot description."),
         )
+        parser.add_argument(
+            '--property',
+            metavar='<key>',
+            action='append',
+            help=_('Remove a property from snapshot '
+                   '(repeat option to remove multiple properties)'),
+        )
         return parser
 
     def take_action(self, parsed_args):
         share_client = self.app.client_manager.share
 
         share_snapshot = utils.find_resource(
             share_client.share_snapshots,
@@ -317,14 +367,23 @@
                     share_snapshot,
                     **kwargs
                 )
             except Exception as e:
                 raise exceptions.CommandError(_(
                     "Failed to unset snapshot display name "
                     "or display description : %s" % e))
+        if parsed_args.property:
+            for key in parsed_args.property:
+                try:
+                    share_snapshot.delete_metadata([key])
+                except Exception as e:
+                    raise exceptions.CommandError(_(
+                        "Failed to unset snapshot property "
+                        "'%(key)s': %(e)s"),
+                        {'key': key, 'e': e})
 
 
 class ListShareSnapshot(command.Lister):
     """List snapshots."""
     _description = _("List snapshots")
 
     def get_parser(self, prog_name):
@@ -404,14 +463,22 @@
         )
         parser.add_argument(
             '--detail',
             action='store_true',
             default=False,
             help=_("List share snapshots with details")
         )
+        parser.add_argument(
+            '--property',
+            metavar='<key=value>',
+            action=parseractions.KeyValueAction,
+            help=_('Filter snapshots having a given metadata key=value '
+                   'property. (repeat option to filter by multiple '
+                   'properties)'),
+        )
         return parser
 
     def take_action(self, parsed_args):
         share_client = self.app.client_manager.share
 
         share_id = None
         if parsed_args.share:
@@ -423,14 +490,16 @@
             'offset': parsed_args.marker,
             'limit': parsed_args.limit,
             'all_tenants': parsed_args.all_projects,
             'name': parsed_args.name,
             'status': parsed_args.status,
             'share_id': share_id,
             'usage': parsed_args.usage,
+            'metadata': oscutils.extract_key_value_options(
+                parsed_args.property),
         }
 
         if share_client.api_version >= api_versions.APIVersion("2.36"):
             search_opts['name~'] = getattr(parsed_args, 'name~')
             search_opts['description~'] = getattr(parsed_args, 'description~')
             search_opts['description'] = parsed_args.description
         elif (parsed_args.description or getattr(parsed_args, 'name~') or
```

### Comparing `python-manilaclient-4.2.0/manilaclient/osc/v2/share_type_access.py` & `python-manilaclient-4.3.0/manilaclient/osc/v2/share_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/osc/v2/share_types.py` & `python-manilaclient-4.3.0/manilaclient/osc/v2/share_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/shell.py` & `python-manilaclient-4.3.0/manilaclient/shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -347,14 +347,21 @@
         parser.add_argument('--os-cert',
                             metavar='<certificate>',
                             default=cliutils.env('OS_CERT'),
                             help='Defaults to env[OS_CERT].')
         parser.add_argument('--os_cert',
                             help=argparse.SUPPRESS)
 
+        parser.add_argument('--os-key',
+                            metavar='<key>',
+                            default=cliutils.env('OS_KEY'),
+                            help='Defaults to env[OS_KEY].')
+        parser.add_argument('--os_key',
+                            help=argparse.SUPPRESS)
+
         if osprofiler_profiler:
             parser.add_argument('--profile',
                                 metavar='HMAC_KEY',
                                 default=cliutils.env('OS_PROFILE'),
                                 help='HMAC key to use for encrypting '
                                 'context data for performance profiling '
                                 'of operation. This key needs to match the '
@@ -538,14 +545,17 @@
 
         major_version_string = str(api_version.ver_major)
         os_service_type = args.service_type
         if not os_service_type:
             os_service_type = constants.SERVICE_TYPES[major_version_string]
 
         os_endpoint_type = args.endpoint_type or DEFAULT_MANILA_ENDPOINT_TYPE
+        cert = args.os_cert or None
+        if cert and args.os_key:
+            cert = cert, args.os_key
 
         client_args = dict(
             username=args.os_username,
             password=args.os_password,
             project_name=args.os_project_name or args.os_tenant_name,
             auth_url=args.os_auth_url,
             insecure=args.insecure,
@@ -561,15 +571,15 @@
             use_keyring=args.os_cache,
             force_new_token=args.os_reset_cache,
             user_id=args.os_user_id,
             user_domain_id=args.os_user_domain_id,
             user_domain_name=args.os_user_domain_name,
             project_domain_id=args.os_project_domain_id,
             project_domain_name=args.os_project_domain_name,
-            cert=args.os_cert,
+            cert=cert,
             input_auth_token=args.os_token,
             service_catalog_url=args.bypass_url,
         )
 
         # Handle deprecated parameters
         if args.share_service_name:
             client_args['share_service_name'] = args.share_service_name
```

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/base.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -316,15 +316,15 @@
         data = {
             'share_protocol': share_protocol or client.share_protocol,
             'size': size or 1,
             'name': name,
             'description': description,
             'public': public,
             'snapshot': snapshot,
-            'metadata': metadata,
+            'metadata': metadata or {},
             'microversion': microversion,
             'wait': use_wait_option,
         }
 
         share_type = share_type or CONF.share_type
         share_network = share_network or cls._determine_share_network_to_use(
             client, share_type, microversion=microversion)
```

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/client.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/client.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/exceptions.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/osc/base.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/osc/base.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/osc/test_availability_zones.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_availability_zones.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/osc/test_messages.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_messages.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/osc/test_share_access_rules.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_access_rules.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/osc/test_share_group_type_access.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_group_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/osc/test_share_limits.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_limits.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/osc/test_share_network_subnets.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_network_subnets.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/osc/test_share_networks.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_networks.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/osc/test_share_pools.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_pools.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/osc/test_share_replica_export_locations.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_replica_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/osc/test_share_replicas.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_replicas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/osc/test_share_services.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/osc/test_share_snapshots.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/osc/test_share_types.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/osc/test_shares.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_shares.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/osc/test_shares_group_type.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_shares_group_type.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/test_availability_zones.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/test_availability_zones.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/test_common.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/test_common.py`

 * *Files 17% similar despite different names*

```diff
@@ -31,15 +31,19 @@
     def test_help(self, role):
         help_text = self.clients[role].manila('help')
         lines = help_text.split('\n')
         self.assertFirstLineStartsWith(lines, 'usage: manila')
 
         commands = []
         cmds_start = lines.index('Positional arguments:')
-        cmds_end = lines.index('Optional arguments:')
+        try:
+            # TODO(gouthamr): Drop when py3.10 becomes min supported version
+            cmds_end = lines.index('Optional arguments:')
+        except ValueError:
+            cmds_end = lines.index('Options:')
         command_pattern = re.compile(r'^ {4}([a-z0-9\-\_]+)')
         for line in lines[cmds_start:cmds_end]:
             match = command_pattern.match(line)
             if match:
                 commands.append(match.group(1))
         commands = set(commands)
         wanted_commands = set((
```

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/test_export_locations.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/test_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/test_limits.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/test_limits.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/test_messages.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/test_messages.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/test_quotas.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/test_quotas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/test_scheduler_stats.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/test_scheduler_stats.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/test_security_services.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/test_security_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/test_services.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/test_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/test_share_access.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/test_share_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/test_share_network_subnets.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/test_share_network_subnets.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/test_share_networks.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/test_share_networks.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/test_share_replica_export_locations.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/test_share_replica_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/test_share_replicas.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/test_share_replicas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/test_share_servers.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/test_share_servers.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/test_share_types.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/test_share_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/test_shares.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/test_shares.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/test_shares_listing.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/test_shares_listing.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/test_shares_metadata.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/test_shares_metadata.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/test_snapshot_access.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/test_snapshot_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/test_snapshot_instances.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/test_snapshot_instances.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/test_snapshot_instances_export_locations.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/test_snapshot_instances_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/test_snapshots_export_locations.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/test_snapshots_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/functional/utils.py` & `python-manilaclient-4.3.0/manilaclient/tests/functional/utils.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/common/test_httpclient.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/common/test_httpclient.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/fakes.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/fakes.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/osc/osc_fakes.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/osc_fakes.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/osc/osc_utils.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/osc_utils.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/fakes.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/fakes.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_availability_zones.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_availability_zones.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_messages.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_messages.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_quotas.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_quotas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_security_services.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_security_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_services.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share.py`

 * *Files 0% similar despite different names*

```diff
@@ -1108,15 +1108,16 @@
 
 class TestShareSet(TestShare):
 
     def setUp(self):
         super(TestShareSet, self).setUp()
 
         self._share = manila_fakes.FakeShare.create_one_share(
-            methods={"reset_state": None, "reset_task_state": None}
+            methods={"reset_state": None, "reset_task_state": None,
+                     "set_metadata": None}
         )
         self.shares_mock.get.return_value = self._share
 
         # Get the command object to test
         self.cmd = osc_shares.SetShare(self.app, None)
 
     def test_share_set_property(self):
@@ -1128,16 +1129,15 @@
             ('property', {'Zorilla': 'manila'}),
             ('share', self._share.id)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
-        self.shares_mock.set_metadata.assert_called_with(
-            self._share.id,
+        self._share.set_metadata.assert_called_with(
             {'Zorilla': 'manila'})
 
     def test_share_set_name(self):
         new_name = uuid.uuid4().hex
         arglist = [
             '--name', new_name,
             self._share.id,
@@ -1220,21 +1220,20 @@
             ('property', {'key': ''}),
             ('share', self._share.id)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
-        self.shares_mock.set_metadata.assert_called_with(
-            self._share.id,
+        self._share.set_metadata.assert_called_with(
             {'key': ''})
 
         # '--property' takes key=value arguments
         # missing a value would raise a BadRequest
-        self.shares_mock.set_metadata.side_effect = exceptions.BadRequest()
+        self._share.set_metadata.side_effect = exceptions.BadRequest
         self.assertRaises(
             osc_exceptions.CommandError, self.cmd.take_action, parsed_args)
 
     def test_share_set_status(self):
         new_status = 'available'
         arglist = [
             self._share.id,
@@ -1286,15 +1285,17 @@
 
 
 class TestShareUnset(TestShare):
 
     def setUp(self):
         super(TestShareUnset, self).setUp()
 
-        self._share = manila_fakes.FakeShare.create_one_share()
+        self._share = manila_fakes.FakeShare.create_one_share(
+            methods={"delete_metadata": None}
+        )
         self.shares_mock.get.return_value = self._share
 
         # Get the command objects to test
         self.cmd = osc_shares.UnsetShare(self.app, None)
 
     def test_share_unset_property(self):
         arglist = [
@@ -1305,16 +1306,15 @@
             ('property', ['Manila']),
             ('share', self._share.id)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
-        self.shares_mock.delete_metadata.assert_called_with(
-            self._share.id,
+        self._share.delete_metadata.assert_called_with(
             parsed_args.property)
 
     def test_share_unset_name(self):
         arglist = [
             '--name',
             self._share.id,
         ]
@@ -1372,20 +1372,19 @@
             ('property', ['Manila']),
             ('share', self._share.id)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
-        self.shares_mock.delete_metadata.assert_called_with(
-            self._share.id,
+        self._share.delete_metadata.assert_called_with(
             parsed_args.property)
 
         # 404 Not Found would be raised, if property 'Manila' doesn't exist
-        self.shares_mock.delete_metadata.side_effect = exceptions.NotFound()
+        self._share.delete_metadata.side_effect = exceptions.NotFound
         self.assertRaises(
             osc_exceptions.CommandError, self.cmd.take_action, parsed_args)
 
 
 class TestResizeShare(TestShare):
 
     def setUp(self):
@@ -1865,15 +1864,16 @@
     def setUp(self):
         super(TestShowShareProperties, self).setUp()
 
         self._share = manila_fakes.FakeShare.create_one_share(
             attrs={
                 'metadata': osc_fakes.FakeResource(
                     info=self.properties)
-            }
+            },
+            methods={'get_metadata': None}
         )
         self.shares_mock.get.return_value = self._share
         self.shares_mock.get_metadata.return_value = self._share.metadata
 
         # Get the command object to test
         self.cmd = osc_shares.ShowShareProperties(self.app, None)
```

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_access_rules.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_access_rules.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_group_snapshots.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_group_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_group_type.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_group_type.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_group_type_access.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_group_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_groups.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_groups.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_instance_export_locations.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_instance_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_instances.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_instances.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_limits.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_limits.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_network_subnets.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_network_subnets.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_networks.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_networks.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_pools.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_pools.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_replica_export_locations.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_replica_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_replicas.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_replicas.py`

 * *Files 4% similar despite different names*

```diff
@@ -635,14 +635,33 @@
 
         result = self.cmd.take_action(parsed_args)
 
         self.replicas_mock.promote.assert_called_with(
             self.share_replica)
         self.assertIsNone(result)
 
+    def test_share_replica_promote_quiesce_wait_time(self):
+        wait_time = '5'
+        arglist = [
+            self.share_replica.id,
+            '--quiesce-wait-time', wait_time
+        ]
+        verifylist = [
+            ('replica', self.share_replica.id),
+            ('quiesce_wait_time', wait_time)
+        ]
+        parsed_args = self.check_parser(self.cmd, arglist, verifylist)
+
+        result = self.cmd.take_action(parsed_args)
+
+        self.replicas_mock.promote.assert_called_with(
+            self.share_replica,
+            wait_time)
+        self.assertIsNone(result)
+
     def test_share_replica_promote_exception(self):
         arglist = [
             self.share_replica.id,
         ]
         verifylist = [
             ('replica', self.share_replica.id),
         ]
```

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_servers.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_servers.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_snapshot_instance_export_locations.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_snapshot_instance_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_snapshot_instances.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_snapshot_instances.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_snapshots.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_snapshots.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,17 @@
         self.app.client_manager.share.api_version = api_versions.APIVersion(
             api_versions.MAX_VERSION)
 
         self.export_locations_mock = (
             self.app.client_manager.share.share_snapshot_export_locations)
         self.export_locations_mock.reset_mock()
 
+        self.app.client_manager.share.api_version = api_versions.APIVersion(
+            api_versions.MAX_VERSION)
+
 
 class TestShareSnapshotCreate(TestShareSnapshot):
 
     def setUp(self):
         super(TestShareSnapshotCreate, self).setUp()
 
         self.share = manila_fakes.FakeShare.create_one_share()
@@ -101,15 +104,16 @@
 
         columns, data = self.cmd.take_action(parsed_args)
 
         self.snapshots_mock.create.assert_called_with(
             share=self.share,
             force=False,
             name=None,
-            description=None
+            description=None,
+            metadata={}
         )
 
         self.assertCountEqual(self.columns, columns)
         self.assertCountEqual(self.data, data)
 
     def test_share_snapshot_create_force(self):
         arglist = [
@@ -125,15 +129,16 @@
 
         columns, data = self.cmd.take_action(parsed_args)
 
         self.snapshots_mock.create.assert_called_with(
             share=self.share,
             force=True,
             name=None,
-            description=None
+            description=None,
+            metadata={}
         )
 
         self.assertCountEqual(columns, columns)
         self.assertCountEqual(self.data, data)
 
     def test_share_snapshot_create(self):
         arglist = [
@@ -151,15 +156,46 @@
 
         columns, data = self.cmd.take_action(parsed_args)
 
         self.snapshots_mock.create.assert_called_with(
             share=self.share,
             force=False,
             name=self.share_snapshot.name,
-            description=self.share_snapshot.description
+            description=self.share_snapshot.description,
+            metadata={}
+        )
+
+        self.assertCountEqual(self.columns, columns)
+        self.assertCountEqual(self.data, data)
+
+    def test_share_snapshot_create_metadata(self):
+        arglist = [
+            self.share.id,
+            '--name', self.share_snapshot.name,
+            '--description', self.share_snapshot.description,
+            '--property', 'Manila=zorilla',
+            '--property', 'Zorilla=manila'
+        ]
+        verifylist = [
+            ('share', self.share.id),
+            ('name', self.share_snapshot.name),
+            ('description', self.share_snapshot.description),
+            ('property', {'Manila': 'zorilla', 'Zorilla': 'manila'}),
+        ]
+
+        parsed_args = self.check_parser(self.cmd, arglist, verifylist)
+
+        columns, data = self.cmd.take_action(parsed_args)
+
+        self.snapshots_mock.create.assert_called_with(
+            share=self.share,
+            force=False,
+            name=self.share_snapshot.name,
+            description=self.share_snapshot.description,
+            metadata={'Manila': 'zorilla', 'Zorilla': 'manila'},
         )
 
         self.assertCountEqual(self.columns, columns)
         self.assertCountEqual(self.data, data)
 
     def test_share_snapshot_create_wait(self):
         arglist = [
@@ -175,15 +211,16 @@
 
         columns, data = self.cmd.take_action(parsed_args)
 
         self.snapshots_mock.create.assert_called_with(
             share=self.share,
             force=False,
             name=None,
-            description=None
+            description=None,
+            metadata={}
         )
 
         self.snapshots_mock.get.assert_called_with(
             self.share_snapshot.id)
         self.assertCountEqual(self.columns, columns)
         self.assertCountEqual(self.data, data)
 
@@ -203,15 +240,16 @@
         with mock.patch('osc_lib.utils.wait_for_status', return_value=False):
             columns, data = self.cmd.take_action(parsed_args)
 
             self.snapshots_mock.create.assert_called_with(
                 share=self.share,
                 force=False,
                 name=None,
-                description=None
+                description=None,
+                metadata={}
             )
 
             mock_logger.error.assert_called_with(
                 "ERROR: Share snapshot is in error state.")
 
             self.snapshots_mock.get.assert_called_with(
                 self.share_snapshot.id)
@@ -392,15 +430,17 @@
 
 class TestShareSnapshotSet(TestShareSnapshot):
 
     def setUp(self):
         super(TestShareSnapshotSet, self).setUp()
 
         self.share_snapshot = (
-            manila_fakes.FakeShareSnapshot.create_one_snapshot())
+            manila_fakes.FakeShareSnapshot.create_one_snapshot(
+                methods={"set_metadata": None}
+            ))
 
         self.snapshots_mock.get.return_value = self.share_snapshot
 
         self.cmd = osc_share_snapshots.SetShareSnapshot(self.app, None)
 
     def test_set_snapshot_name(self):
         snapshot_name = 'snapshot-name-' + uuid.uuid4().hex
@@ -454,14 +494,30 @@
         result = self.cmd.take_action(parsed_args)
 
         self.snapshots_mock.reset_state.assert_called_with(
             self.share_snapshot,
             parsed_args.status)
         self.assertIsNone(result)
 
+    def test_set_snapshot_property(self):
+        arglist = [
+            self.share_snapshot.id,
+            '--property', 'Zorilla=manila',
+        ]
+        verifylist = [
+            ('snapshot', self.share_snapshot.id),
+            ('property', {'Zorilla': 'manila'}),
+        ]
+
+        parsed_args = self.check_parser(self.cmd, arglist, verifylist)
+
+        self.cmd.take_action(parsed_args)
+        self.share_snapshot.set_metadata.assert_called_with(
+            {'Zorilla': 'manila'})
+
     def test_set_snapshot_update_exception(self):
         snapshot_name = 'snapshot-name-' + uuid.uuid4().hex
         arglist = [
             self.share_snapshot.id,
             '--name', snapshot_name
         ]
         verifylist = [
@@ -491,22 +547,47 @@
         self.snapshots_mock.reset_state.side_effect = Exception()
 
         self.assertRaises(
             exceptions.CommandError,
             self.cmd.take_action,
             parsed_args)
 
+    def test_set_snapshot_property_exception(self):
+        arglist = [
+            '--property', 'key=',
+            self.share_snapshot.id,
+        ]
+        verifylist = [
+            ('property', {'key': ''}),
+            ('snapshot', self.share_snapshot.id)
+        ]
+
+        parsed_args = self.check_parser(self.cmd, arglist, verifylist)
+
+        self.cmd.take_action(parsed_args)
+        self.share_snapshot.set_metadata.assert_called_with(
+            {'key': ''})
+
+        # '--property' takes key=value arguments
+        # missing a value would raise a BadRequest
+        self.share_snapshot.set_metadata.side_effect = exceptions.BadRequest
+        self.assertRaises(
+            exceptions.CommandError, self.cmd.take_action,
+            parsed_args)
+
 
 class TestShareSnapshotUnset(TestShareSnapshot):
 
     def setUp(self):
         super(TestShareSnapshotUnset, self).setUp()
 
         self.share_snapshot = (
-            manila_fakes.FakeShareSnapshot.create_one_snapshot())
+            manila_fakes.FakeShareSnapshot.create_one_snapshot(
+                methods={"delete_metadata": None}
+            ))
 
         self.snapshots_mock.get.return_value = self.share_snapshot
 
         self.cmd = osc_share_snapshots.UnsetShareSnapshot(self.app, None)
 
     def test_unset_snapshot_name(self):
         arglist = [
@@ -540,14 +621,30 @@
         result = self.cmd.take_action(parsed_args)
 
         self.snapshots_mock.update.assert_called_with(
             self.share_snapshot,
             display_description=None)
         self.assertIsNone(result)
 
+    def test_unset_snapshot_property(self):
+        arglist = [
+            '--property', 'Manila',
+            self.share_snapshot.id,
+        ]
+        verifylist = [
+            ('property', ['Manila']),
+            ('snapshot', self.share_snapshot.id)
+        ]
+
+        parsed_args = self.check_parser(self.cmd, arglist, verifylist)
+
+        self.cmd.take_action(parsed_args)
+        self.share_snapshot.delete_metadata.assert_called_with(
+            parsed_args.property)
+
     def test_unset_snapshot_name_exception(self):
         arglist = [
             self.share_snapshot.id,
             '--name'
         ]
         verifylist = [
             ('snapshot', self.share_snapshot.id),
@@ -558,14 +655,35 @@
         self.snapshots_mock.update.side_effect = Exception()
 
         self.assertRaises(
             exceptions.CommandError,
             self.cmd.take_action,
             parsed_args)
 
+    def test_unset_snapshot_property_exception(self):
+        arglist = [
+            '--property', 'Manila',
+            self.share_snapshot.id,
+        ]
+        verifylist = [
+            ('property', ['Manila']),
+            ('snapshot', self.share_snapshot.id)
+        ]
+
+        parsed_args = self.check_parser(self.cmd, arglist, verifylist)
+
+        self.cmd.take_action(parsed_args)
+        self.share_snapshot.delete_metadata.assert_called_with(
+            parsed_args.property)
+
+        # 404 Not Found would be raised, if property 'Manila' doesn't exist
+        self.share_snapshot.delete_metadata.side_effect = exceptions.NotFound
+        self.assertRaises(
+            exceptions.CommandError, self.cmd.take_action, parsed_args)
+
 
 class TestShareSnapshotList(TestShareSnapshot):
 
     def setUp(self):
         super(TestShareSnapshotList, self).setUp()
 
         self.share_snapshots = (
@@ -596,17 +714,18 @@
                 'offset': None,
                 'limit': None,
                 'all_tenants': False,
                 'name': None,
                 'status': None,
                 'share_id': None,
                 'usage': None,
+                'metadata': {},
                 'name~': None,
                 'description~': None,
-                'description': None
+                'description': None,
             })
 
         self.assertEqual(COLUMNS, columns)
         self.assertEqual(list(self.values), list(data))
 
     def test_list_snapshots_all_projects(self):
         all_tenants_list = COLUMNS.copy()
@@ -631,17 +750,18 @@
                 'offset': None,
                 'limit': None,
                 'all_tenants': True,
                 'name': None,
                 'status': None,
                 'share_id': None,
                 'usage': None,
+                'metadata': {},
                 'name~': None,
                 'description~': None,
-                'description': None
+                'description': None,
             })
 
         self.assertEqual(all_tenants_list, columns)
         self.assertEqual(list(list_values), list(data))
 
     def test_list_snapshots_detail(self):
         values = (oscutils.get_dict_properties(
@@ -664,14 +784,15 @@
                 'offset': None,
                 'limit': None,
                 'all_tenants': False,
                 'name': None,
                 'status': None,
                 'share_id': None,
                 'usage': None,
+                'metadata': {},
                 'name~': None,
                 'description~': None,
                 'description': None
             })
 
         self.assertEqual(COLUMNS_DETAIL, columns)
         self.assertEqual(list(values), list(data))
@@ -720,14 +841,15 @@
                 'offset': None,
                 'limit': None,
                 'all_tenants': False,
                 'name': None,
                 'status': None,
                 'share_id': self.share.id,
                 'usage': None,
+                'metadata': {},
                 'name~': None,
                 'description~': None,
                 'description': None
             })
 
         self.assertEqual(COLUMNS, columns)
         self.assertEqual(list(values), list(data))
```

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_type.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_type.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/osc/v2/test_share_type_access.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/test_api_versions.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/test_api_versions.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/test_base.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/test_base.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/test_client.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/test_functional_utils.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/test_functional_utils.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/test_shell.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/test_shell.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,16 @@
     )
     def test_main_failure(self, env_vars):
         self.set_env_vars(env_vars)
         with mock.patch.object(shell, 'client') as mock_client:
             self.assertRaises(exceptions.CommandError, self.shell, 'list')
             self.assertFalse(mock_client.Client.called)
 
-    def test_main_success(self):
+    @ddt.data(None, 'foo_key')
+    def test_main_success(self, os_key):
         env_vars = {
             'OS_AUTH_URL': 'http://foo.bar',
             'OS_USERNAME': 'foo_username',
             'OS_USER_ID': 'foo_user_id',
             'OS_PASSWORD': 'foo_password',
             'OS_TENANT_NAME': 'foo_tenant',
             'OS_TENANT_ID': 'foo_tenant_id',
@@ -98,16 +99,21 @@
             'OS_PROJECT_ID': 'foo_project_id',
             'OS_PROJECT_DOMAIN_ID': 'foo_project_domain_id',
             'OS_PROJECT_DOMAIN_NAME': 'foo_project_domain_name',
             'OS_PROJECT_DOMAIN_ID': 'foo_project_domain_id',
             'OS_USER_DOMAIN_NAME': 'foo_user_domain_name',
             'OS_USER_DOMAIN_ID': 'foo_user_domain_id',
             'OS_CERT': 'foo_cert',
+            'OS_KEY': os_key,
         }
         self.set_env_vars(env_vars)
+        cert = env_vars['OS_CERT']
+        if os_key:
+            cert = (cert, env_vars['OS_KEY'])
+
         with mock.patch.object(shell, 'client') as mock_client:
 
             self.shell('list')
 
             mock_client.Client.assert_called_with(
                 manilaclient.API_MAX_VERSION,
                 username=env_vars['OS_USERNAME'],
@@ -127,15 +133,15 @@
                 use_keyring=False,
                 force_new_token=False,
                 user_id=env_vars['OS_USER_ID'],
                 user_domain_id=env_vars['OS_USER_DOMAIN_ID'],
                 user_domain_name=env_vars['OS_USER_DOMAIN_NAME'],
                 project_domain_id=env_vars['OS_PROJECT_DOMAIN_ID'],
                 project_domain_name=env_vars['OS_PROJECT_DOMAIN_NAME'],
-                cert=env_vars['OS_CERT'],
+                cert=cert,
                 input_auth_token='',
                 service_catalog_url='',
             )
 
     @ddt.data(
         {"env_vars": {"OS_MANILA_BYPASS_URL": "http://foo.url",
                       "OS_TOKEN": "foo_token"},
@@ -199,15 +205,15 @@
                 use_keyring=False,
                 force_new_token=False,
                 user_id="",
                 user_domain_id="",
                 user_domain_name="",
                 project_domain_id="",
                 project_domain_name="",
-                cert="",
+                cert=None,
                 input_auth_token=expected["input_auth_token"],
                 service_catalog_url=expected["service_catalog_url"],
             )
 
     @ddt.data(
         # default without any env var or kwargs
         {
@@ -278,15 +284,15 @@
                 use_keyring=False,
                 force_new_token=False,
                 user_id="",
                 user_domain_id="",
                 user_domain_name="",
                 project_domain_id="",
                 project_domain_name="",
-                cert="",
+                cert=None,
                 input_auth_token=expected["input_auth_token"],
                 service_catalog_url=expected["service_catalog_url"],
             )
 
     def test_help_unknown_command(self):
         self.assertRaises(exceptions.CommandError, self.shell, 'help foofoo')
 
@@ -307,14 +313,15 @@
             '--os-user-id', '--os-username', '--os-password',
             '--os-tenant-name', '--os-project-name', '--os-tenant-id',
             '--os-project-id', '--os-user-domain-id', '--os-user-domain-name',
             '--os-project-domain-id', '--os-project-domain-name',
             '--os-auth-url', '--os-region-name', '--service-type',
             '--service-name', '--share-service-name', '--endpoint-type',
             '--os-share-api-version', '--os-cacert', '--retries', '--os-cert',
+            '--os-key',
         )
 
         help_text = self.shell('help')
 
         for expected_arg in expected_args:
             self.assertIn(expected_arg, help_text)
```

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/utils.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v1/test_limits.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_limits.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v1/test_quota_classes.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_quota_classes.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v1/test_quotas.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_quotas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v1/test_scheduler_stats.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_scheduler_stats.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v1/test_security_services.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_security_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v1/test_services.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v1/test_share_networks.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_share_networks.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v1/test_share_servers.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_share_servers.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v1/test_share_snapshots.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_share_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v1/test_share_type_access.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_share_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v1/test_share_types.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_share_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v1/test_shares.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_shares.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v2/fake_clients.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/fake_clients.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v2/fakes.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/fakes.py`

 * *Files 2% similar despite different names*

```diff
@@ -950,18 +950,19 @@
         _body = None
         resp = 202
         assert len(list(body)) == 1
         action = list(body)[0]
         if action in ('reset_status', 'reset_replica_state'):
             attr = action.split('reset_')[1]
             assert attr in body.get(action)
-        elif action in ('force_delete', 'resync', 'promote'):
+        elif action in ('force_delete', 'resync'):
             assert body[action] is None
         else:
-            raise AssertionError("Unexpected share action: %s" % action)
+            if action not in ('promote'):
+                raise AssertionError("Unexpected share action: %s" % action)
         return (resp, {}, _body)
 
     #
     # Set/Unset metadata
     #
     def delete_shares_1234_metadata_test_key(self, **kw):
         return (204, {}, None)
@@ -1156,14 +1157,32 @@
             'state': 'active',
             'id': '1234',
             'access_type': 'ip',
             'access_to': '6.6.6.6'
         }]}
         return (200, {}, access_list)
 
+    def delete_snapshots_1234_metadata_test_key(self, **kw):
+        return (204, {}, None)
+
+    def delete_snapshots_1234_metadata_key1(self, **kw):
+        return (204, {}, None)
+
+    def delete_snapshots_1234_metadata_key2(self, **kw):
+        return (204, {}, None)
+
+    def post_snapshots_1234_metadata(self, **kw):
+        return (204, {}, {'metadata': {'test_key': 'test_value'}})
+
+    def put_snapshots_1234_metadata(self, **kw):
+        return (200, {}, {"metadata": {"key1": "val1", "key2": "val2"}})
+
+    def get_snapshots_1234_metadata(self, **kw):
+        return (200, {}, {"metadata": {"key1": "val1", "key2": "val2"}})
+
     def post_snapshot_instances_1234_action(self, body, **kw):
         _body = None
         resp = 202
         assert len(list(body)) == 1
         action = list(body)[0]
         if action == 'reset_status':
             assert 'status' in body.get(action)
```

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_availability_zones.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_availability_zones.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_client.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_client.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_limits.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_limits.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_messages.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_messages.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_quota_classes.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_quota_classes.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_quotas.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_quotas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_scheduler_stats.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_scheduler_stats.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_security_services.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_security_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_services.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_share_export_locations.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_share_group_snapshots.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_group_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_share_group_type_access.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_group_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_share_group_types.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_group_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_share_groups.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_groups.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_share_instance_export_locations.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_instance_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_share_instances.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_instances.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_share_network_subnets.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_network_subnets.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_share_networks.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_networks.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_share_replica_export_locations.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_replica_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_share_replicas.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_replicas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_share_servers.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_servers.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_share_snapshot_export_locations.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_snapshot_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_share_snapshot_instance_export_locations.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_snapshot_instance_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_share_snapshot_instances.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_snapshot_instances.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_share_snapshots.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_snapshots.py`

 * *Files 10% similar despite different names*

```diff
@@ -211,7 +211,34 @@
             manager.deny(snapshot, access_id)
             manager._action.assert_called_once_with(
                 "deny_access", snapshot, {'access_id': access_id})
 
     def test_access_list(self):
         cs.share_snapshots.access_list(1234)
         cs.assert_called('GET', '/snapshots/1234/access-list')
+
+    def test_get_metadata(self):
+        cs.share_snapshots.get_metadata(1234)
+        cs.assert_called('GET', '/snapshots/1234/metadata')
+
+    def test_set_metadata(self):
+        cs.share_snapshots.set_metadata(1234, {'k1': 'v2'})
+        cs.assert_called('POST', '/snapshots/1234/metadata',
+                         {'metadata': {'k1': 'v2'}})
+
+    @ddt.data(
+        type('SnapshotUUID', (object, ), {'uuid': '1234'}),
+        type('SnapshotID', (object, ), {'id': '1234'}),
+        '1234')
+    def test_delete_metadata(self, snapshot):
+        keys = ['key1']
+        cs.share_snapshots.delete_metadata(snapshot, keys)
+        cs.assert_called('DELETE', '/snapshots/1234/metadata/key1')
+
+    @ddt.data(
+        type('SnapshotUUID', (object, ), {'uuid': '1234'}),
+        type('SnapshotID', (object, ), {'id': '1234'}),
+        '1234')
+    def test_metadata_update_all(self, snapshot):
+        cs.share_snapshots.update_all_metadata(snapshot, {'k1': 'v1'})
+        cs.assert_called('PUT', '/snapshots/1234/metadata',
+                         {'metadata': {'k1': 'v1'}})
```

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_shares.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_shares.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_shell.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_shell.py`

 * *Files 0% similar despite different names*

```diff
@@ -3426,14 +3426,25 @@
 
     def test_share_replica_show(self):
 
         self.run_command('share-replica-show 5678')
 
         self.assert_called_anytime('GET', '/share-replicas/5678')
 
+    @mock.patch.object(shell_v2, '_find_share_replica', mock.Mock())
+    def test_share_replica_promote_quiesce_wait_time(self):
+        fake_replica = type('FakeShareReplica', (object,), {'id': '1234'})
+        shell_v2._find_share_replica.return_value = fake_replica
+        cmd = ('share-replica-promote ' + fake_replica.id +
+               ' --quiesce-wait-time 5')
+        self.run_command(cmd)
+        self.assert_called(
+            'POST', '/share-replicas/1234/action',
+            body={'promote': {'quiesce_wait_time': '5'}})
+
     @ddt.data('promote', 'resync')
     @mock.patch.object(shell_v2, '_find_share_replica', mock.Mock())
     def test_share_replica_actions(self, action):
         fake_replica = type('FakeShareReplica', (object,), {'id': '1234'})
         shell_v2._find_share_replica.return_value = fake_replica
         cmd = 'share-replica-' + action + ' ' + fake_replica.id
```

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_type_access.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/tests/unit/v2/test_types.py` & `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/utils.py` & `python-manilaclient-4.3.0/manilaclient/utils.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v1/__init__.py` & `python-manilaclient-4.3.0/manilaclient/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v1/client.py` & `python-manilaclient-4.3.0/manilaclient/v1/client.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v1/contrib/list_extensions.py` & `python-manilaclient-4.3.0/manilaclient/v1/contrib/list_extensions.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v1/limits.py` & `python-manilaclient-4.3.0/manilaclient/v1/limits.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v1/quota_classes.py` & `python-manilaclient-4.3.0/manilaclient/v1/quota_classes.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v1/quotas.py` & `python-manilaclient-4.3.0/manilaclient/v1/quotas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v1/scheduler_stats.py` & `python-manilaclient-4.3.0/manilaclient/v1/scheduler_stats.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v1/security_services.py` & `python-manilaclient-4.3.0/manilaclient/v1/security_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v1/services.py` & `python-manilaclient-4.3.0/manilaclient/v1/services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v1/share_networks.py` & `python-manilaclient-4.3.0/manilaclient/v1/share_networks.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v1/share_servers.py` & `python-manilaclient-4.3.0/manilaclient/v1/share_servers.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v1/share_snapshots.py` & `python-manilaclient-4.3.0/manilaclient/v1/share_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v1/share_type_access.py` & `python-manilaclient-4.3.0/manilaclient/v1/share_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v1/share_types.py` & `python-manilaclient-4.3.0/manilaclient/v1/share_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v1/shares.py` & `python-manilaclient-4.3.0/manilaclient/v1/shares.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v2/__init__.py` & `python-manilaclient-4.3.0/manilaclient/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v2/availability_zones.py` & `python-manilaclient-4.3.0/manilaclient/v2/availability_zones.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v2/client.py` & `python-manilaclient-4.3.0/manilaclient/v2/client.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v2/contrib/list_extensions.py` & `python-manilaclient-4.3.0/manilaclient/v2/contrib/list_extensions.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v2/limits.py` & `python-manilaclient-4.3.0/manilaclient/v2/limits.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v2/messages.py` & `python-manilaclient-4.3.0/manilaclient/v2/messages.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v2/quota_classes.py` & `python-manilaclient-4.3.0/manilaclient/v2/quota_classes.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v2/quotas.py` & `python-manilaclient-4.3.0/manilaclient/v2/quotas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v2/scheduler_stats.py` & `python-manilaclient-4.3.0/manilaclient/v2/scheduler_stats.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v2/security_services.py` & `python-manilaclient-4.3.0/manilaclient/v2/security_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v2/services.py` & `python-manilaclient-4.3.0/manilaclient/v2/services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v2/share_access_rules.py` & `python-manilaclient-4.3.0/manilaclient/v2/share_access_rules.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v2/share_export_locations.py` & `python-manilaclient-4.3.0/manilaclient/v2/share_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v2/share_group_snapshots.py` & `python-manilaclient-4.3.0/manilaclient/v2/share_group_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v2/share_group_type_access.py` & `python-manilaclient-4.3.0/manilaclient/v2/share_group_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v2/share_group_types.py` & `python-manilaclient-4.3.0/manilaclient/v2/share_group_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v2/share_groups.py` & `python-manilaclient-4.3.0/manilaclient/v2/share_groups.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v2/share_instance_export_locations.py` & `python-manilaclient-4.3.0/manilaclient/v2/share_instance_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v2/share_instances.py` & `python-manilaclient-4.3.0/manilaclient/v2/share_instances.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v2/share_network_subnets.py` & `python-manilaclient-4.3.0/manilaclient/v2/share_network_subnets.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v2/share_networks.py` & `python-manilaclient-4.3.0/manilaclient/v2/share_networks.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v2/share_replica_export_locations.py` & `python-manilaclient-4.3.0/manilaclient/v2/share_replica_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v2/share_replicas.py` & `python-manilaclient-4.3.0/manilaclient/v2/share_replicas.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,22 +97,34 @@
     def promote(self, replica):
         """Promote the provided replica.
 
         :param replica: either replica object or its UUID.
         """
         return self._action('promote', replica)
 
-    @api_versions.wraps(constants.REPLICA_GRADUATION_VERSION)  # noqa
+    @api_versions.wraps(constants.REPLICA_GRADUATION_VERSION, '2.74')  # noqa
     def promote(self, replica):  # noqa F811
         """Promote the provided replica.
 
         :param replica: either replica object or its UUID.
         """
         return self._action('promote', replica)
 
+    @api_versions.wraps('2.75')  # noqa
+    def promote(self, replica, quiesce_wait_time=None):  # noqa F811
+        """Promote the provided replica.
+
+        :param replica: either replica object or its UUID.
+        :param body: either replica object or its UUID.
+        """
+        body = None
+        if quiesce_wait_time:
+            body = dict(quiesce_wait_time=quiesce_wait_time)
+        return self._action('promote', replica, body)
+
     @api_versions.wraps("2.11", constants.REPLICA_PRE_GRADUATION_VERSION)
     @api_versions.experimental_api
     def create(self, share, availability_zone=None):
         return self._create_share_replica(
             share, availability_zone=availability_zone)
 
     @api_versions.wraps(constants.REPLICA_GRADUATION_VERSION, '2.66')  # noqa
```

### Comparing `python-manilaclient-4.2.0/manilaclient/v2/share_servers.py` & `python-manilaclient-4.3.0/manilaclient/v2/share_servers.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v2/share_snapshot_export_locations.py` & `python-manilaclient-4.3.0/manilaclient/v2/share_snapshot_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v2/share_snapshot_instance_export_locations.py` & `python-manilaclient-4.3.0/manilaclient/v2/share_snapshot_instance_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v2/share_snapshot_instances.py` & `python-manilaclient-4.3.0/manilaclient/v2/share_snapshot_instances.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v2/share_snapshots.py` & `python-manilaclient-4.3.0/manilaclient/v2/share_snapshots.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 """Interface for shares extension."""
 
 from manilaclient import api_versions
 from manilaclient import base
 from manilaclient.common import constants
 
 
-class ShareSnapshot(base.Resource):
+class ShareSnapshot(base.MetadataCapableResource):
+
     """Represent a snapshot of a share."""
 
     def __repr__(self):
         return "<ShareSnapshot: %s>" % self.id
 
     def update(self, **kwargs):
         """Update this snapshot."""
@@ -53,34 +54,49 @@
         """Denies access to a share snapshot."""
         return self.manager.deny(self, id)
 
     def access_list(self):
         return self.manager.access_list(self)
 
 
-class ShareSnapshotManager(base.ManagerWithFind):
+class ShareSnapshotManager(base.MetadataCapableManager):
     """Manage :class:`ShareSnapshot` resources."""
     resource_class = ShareSnapshot
+    resource_path = '/snapshots'
 
-    def create(self, share, force=False, name=None, description=None):
+    def _do_create(self, share, force=False, name=None, description=None,
+                   metadata=None):
         """Create a snapshot of the given share.
 
         :param share_id: The ID of the share to snapshot.
         :param force: If force is True, create a snapshot even if the
                       share is busy. Default is False.
         :param name: Name of the snapshot
         :param description: Description of the snapshot
+        :param metadata: dict - optional metadata to set on share creation
         :rtype: :class:`ShareSnapshot`
         """
+
+        metadata = metadata if metadata is not None else dict()
         body = {'snapshot': {'share_id': base.getid(share),
                              'force': force,
                              'name': name,
-                             'description': description}}
+                             'description': description,
+                             'metadata': metadata}}
         return self._create('/snapshots', body, 'snapshot')
 
+    @api_versions.wraps("2.0", "2.72")
+    def create(self, share, force=False, name=None, description=None):
+        return self._do_create(share, force, name, description)
+
+    @api_versions.wraps("2.73")
+    def create(self, share, force=False, name=None, description=None,# noqa F811
+               metadata=None):
+        return self._do_create(share, force, name, description, metadata)
+
     @api_versions.wraps("2.12")
     def manage(self, share, provider_location,
                driver_options=None,
                name=None, description=None):
         """Manage an existing share snapshot.
 
         :param share: The share object.
```

### Comparing `python-manilaclient-4.2.0/manilaclient/v2/share_type_access.py` & `python-manilaclient-4.3.0/manilaclient/v2/share_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v2/share_types.py` & `python-manilaclient-4.3.0/manilaclient/v2/share_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/manilaclient/v2/shares.py` & `python-manilaclient-4.3.0/manilaclient/v2/shares.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 from manilaclient import api_versions
 from manilaclient import base
 from manilaclient.common import constants
 from manilaclient import exceptions
 from manilaclient.v2 import share_instances
 
 
-class Share(base.Resource):
+class Share(base.MetadataCapableResource):
+
     """A share is an extra block level storage to the OpenStack instances."""
     def __repr__(self):
         return "<Share: %s>" % self.id
 
     def update(self, **kwargs):
         """Update this share."""
         self.manager.update(self, **kwargs)
@@ -83,18 +84,14 @@
         """Deny access from IP to a share."""
         return self.manager.deny(self, id)
 
     def access_list(self):
         """Get access list from a share."""
         return self.manager.access_list(self)
 
-    def update_all_metadata(self, metadata):
-        """Update all metadata of this share."""
-        return self.manager.update_all_metadata(self, metadata)
-
     def reset_state(self, state):
         """Update the share with the provided state."""
         self.manager.reset_state(self, state)
 
     def extend(self, new_size, **kwargs):
         """Extend the size of the specified share."""
         self.manager.extend(self, new_size, **kwargs)
@@ -116,17 +113,18 @@
         self.manager.soft_delete(self)
 
     def restore(self):
         """Restore a share from recycle bin"""
         self.manager.restore(self)
 
 
-class ShareManager(base.ManagerWithFind):
+class ShareManager(base.MetadataCapableManager):
     """Manage :class:`Share` resources."""
     resource_class = Share
+    resource_path = '/shares'
 
     def create(self, share_proto, size, snapshot_id=None, name=None,
                description=None, metadata=None, share_network=None,
                share_type=None, is_public=False, availability_zone=None,
                share_group_id=None, scheduler_hints=None):
         """Create a share.
 
@@ -655,53 +653,14 @@
     def access_list(self, share):
         return self._do_access_list(share, "os-access_list")
 
     @api_versions.wraps("2.7", "2.44")  # noqa
     def access_list(self, share):   # noqa
         return self._do_access_list(share, "access_list")
 
-    def get_metadata(self, share):
-        """Get metadata of a share.
-
-        :param share: either share object or text with its ID.
-        """
-        return self._get("/shares/%s/metadata" % base.getid(share),
-                         "metadata")
-
-    def set_metadata(self, share, metadata):
-        """Set or update metadata for share.
-
-        :param share: either share object or text with its ID.
-        :param metadata: A list of keys to be set.
-        """
-        body = {'metadata': metadata}
-        return self._create("/shares/%s/metadata" % base.getid(share),
-                            body, "metadata")
-
-    def delete_metadata(self, share, keys):
-        """Delete specified keys from shares metadata.
-
-        :param share: either share object or text with its ID.
-        :param keys: A list of keys to be removed.
-        """
-        share_id = base.getid(share)
-        for key in keys:
-            self._delete("/shares/%(share_id)s/metadata/%(key)s" % {
-                'share_id': share_id, 'key': key})
-
-    def update_all_metadata(self, share, metadata):
-        """Update all metadata of a share.
-
-        :param share: either share object or text with its ID.
-        :param metadata: A list of keys to be updated.
-        """
-        body = {'metadata': metadata}
-        return self._update("/shares/%s/metadata" % base.getid(share),
-                            body)
-
     def _action(self, action, share, info=None, **kwargs):
         """Perform a share 'action'.
 
         :param action: text with action name.
         :param share: either share object or text with its ID.
         :param info: dict with data for specified 'action'.
         :param kwargs: dict with data to be provided for action hooks.
```

### Comparing `python-manilaclient-4.2.0/manilaclient/v2/shell.py` & `python-manilaclient-4.3.0/manilaclient/v2/shell.py`

 * *Files 0% similar despite different names*

```diff
@@ -1404,34 +1404,34 @@
     choices=['set', 'unset'],
     help="Actions: 'set' or 'unset'.")
 @cliutils.arg(
     'metadata',
     metavar='<key=value>',
     nargs='+',
     default=[],
-    help='Metadata to set or unset (key is only necessary on unset).')
+    help='Metadata to set or unset (only key is necessary to unset).')
 def do_metadata(cs, args):
     """Set or delete metadata on a share."""
     share = _find_share(cs, args.share)
     metadata = _extract_metadata(args)
 
     if args.action == 'set':
-        cs.shares.set_metadata(share, metadata)
+        share.set_metadata(metadata)
     elif args.action == 'unset':
-        cs.shares.delete_metadata(share, sorted(list(metadata), reverse=True))
+        share.delete_metadata(sorted(list(metadata), reverse=True))
 
 
 @cliutils.arg(
     'share',
     metavar='<share>',
     help='Name or ID of the share.')
 def do_metadata_show(cs, args):
     """Show metadata of given share."""
     share = _find_share(cs, args.share)
-    metadata = cs.shares.get_metadata(share)._info
+    metadata = share.get_metadata()._info
     cliutils.print_dict(metadata, 'Property')
 
 
 @cliutils.arg(
     'share',
     metavar='<share>',
     help='Name or ID of the share to update metadata on.')
@@ -2822,14 +2822,22 @@
 @cliutils.arg(
     '--description~',
     metavar='<description~>',
     type=str,
     default=None,
     help='Filter results matching a share snapshot description pattern. '
          'Available only for microversion >= 2.36.')
+@cliutils.arg(
+    '--metadata',
+    metavar='<key=value>',
+    type=str,
+    default=None,
+    nargs='*',
+    help='Filters results by a metadata key and value. OPTIONAL: '
+         'Default=None, Available only for microversion >= 2.73. ')
 def do_snapshot_list(cs, args):
     """List all the snapshots."""
     all_projects = int(
         os.environ.get("ALL_TENANTS",
                        os.environ.get("ALL_PROJECTS",
                                       args.all_projects))
     )
@@ -2848,14 +2856,15 @@
         'offset': args.offset,
         'limit': args.limit,
         'all_tenants': all_projects,
         'name': args.name,
         'status': args.status,
         'share_id': share.id,
         'usage': args.usage,
+        'metadata': _extract_metadata(args),
     }
     if cs.api_version.matches(api_versions.APIVersion("2.36"),
                               api_versions.APIVersion()):
         search_opts['name~'] = getattr(args, 'name~')
         search_opts['description~'] = getattr(args, 'description~')
         search_opts['description'] = getattr(args, 'description')
     elif (getattr(args, 'name~') or getattr(args, 'description~') or
@@ -5214,15 +5223,15 @@
     choices=['set', 'unset'],
     help="Actions: 'set' or 'unset'.")
 @cliutils.arg(
     'metadata',
     metavar='<key=value>',
     nargs='*',
     default=None,
-    help='Extra_specs to set or unset (key is only necessary on unset).')
+    help='Extra_specs to set or unset (only key is necessary to unset).')
 def do_type_key(cs, args):
     """Set or unset extra_spec for a share type (Admin only)."""
     stype = _find_share_type(cs, args.stype)
 
     if args.metadata is not None:
         keypair = _extract_metadata(args)
 
@@ -5451,15 +5460,15 @@
     choices=['set', 'unset'],
     help="Actions: 'set' or 'unset'.")
 @cliutils.arg(
     'group_specs',
     metavar='<key=value>',
     nargs='*',
     default=None,
-    help='Group specs to set or unset (key is only necessary on unset).')
+    help='Group specs to set or unset (only key is necessary to unset).')
 @cliutils.service_type('sharev2')
 def do_share_group_type_key(cs, args):
     """Set or unset group_spec for a share group type (Admin only)."""
     sg_type = _find_share_group_type(cs, args.share_group_type)
     if args.group_specs is not None:
         keypair = _extract_group_specs(args)
         if args.action == 'set':
@@ -6394,21 +6403,42 @@
                                       "replicas.")
 
 
 @cliutils.arg(
     'replica',
     metavar='<replica>',
     help='ID of the share replica.')
-@api_versions.wraps("2.11")
+@api_versions.wraps("2.11", "2.74")
 def do_share_replica_promote(cs, args):
     """Promote specified replica to 'active' replica_state."""
     replica = _find_share_replica(cs, args.replica)
     cs.share_replicas.promote(replica)
 
 
+@cliutils.arg(
+    'replica',
+    metavar='<replica>',
+    help='ID of the share replica.')
+@cliutils.arg(
+    '--quiesce-wait-time',
+    metavar='<quiesce-wait-time>',
+    default=None,
+    help='Quiesce wait time in seconds. Available for '
+         'microversion >= 2.75')
+@api_versions.wraps("2.75")  # noqa
+def do_share_replica_promote(cs, args):  # noqa
+    """Promote specified replica to 'active' replica_state."""
+    replica = _find_share_replica(cs, args.replica)
+
+    quiesce_wait_time = None
+    if args.quiesce_wait_time:
+        quiesce_wait_time = args.quiesce_wait_time
+    cs.share_replicas.promote(replica, quiesce_wait_time)
+
+
 @api_versions.wraps("2.47")
 @cliutils.arg(
     'replica',
     metavar='<replica>',
     help='ID of the share replica.')
 @cliutils.arg(
     '--columns',
@@ -6434,19 +6464,19 @@
     cliutils.print_list(export_locations, list_of_keys)
 
 
 @api_versions.wraps("2.47")
 @cliutils.arg(
     'replica',
     metavar='<replica>',
-    help='Name or ID of the share instance.')
+    help='Name or ID of the share replica.')
 @cliutils.arg(
     'export_location',
     metavar='<export_location>',
-    help='ID of the share instance export location.')
+    help='ID of the share replica export location.')
 def do_share_replica_export_location_show(cs, args):
     """Show details of a share replica's export location."""
     replica = _find_share_replica(cs, args.replica)
     export_location = cs.share_replica_export_locations.get(
         replica, args.export_location)
     view_data = export_location._info.copy()
     cliutils.print_dict(view_data)
```

### Comparing `python-manilaclient-4.2.0/python_manilaclient.egg-info/PKG-INFO` & `python-manilaclient-4.3.0/python_manilaclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-manilaclient
-Version: 4.2.0
+Version: 4.3.0
 Summary: Client library for OpenStack Manila API.
 Home-page: https://docs.openstack.org/python-manilaclient/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `python-manilaclient-4.2.0/python_manilaclient.egg-info/SOURCES.txt` & `python-manilaclient-4.3.0/python_manilaclient.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -273,22 +273,24 @@
 releasenotes/notes/add-export-location-filter-4cf3114doe40k598.yaml
 releasenotes/notes/add-ipv6-access-type-4dko90r1a9a1e0b8.yaml
 releasenotes/notes/add-like-filter-591572762357ef4b.yaml
 releasenotes/notes/add-message-list-and-delete-41b3323edd63d894.yaml
 releasenotes/notes/add-metadata-for-share-access-rule-11a6b36c0f4c87c2.yaml
 releasenotes/notes/add-per-share-gigabytes-quotas-40bc404bd3cbdd89.yaml
 releasenotes/notes/add-query-params-pools-list-api-12cf1s14ddf40kdd.yaml
+releasenotes/notes/add-quiesce-wait-time-for-replica-promote-30d9fa66afc854f2.yaml
 releasenotes/notes/add-quota-per-share-type-support-3b2708ea232e69bc.yaml
 releasenotes/notes/add-scheduler-hints-to-share-create-70d429cb0aaf8f11.yaml
 releasenotes/notes/add-scheduler-hints-to-share-replica-create-d152a3934e5ad3a7.yaml
 releasenotes/notes/add-share-group-quotas-support-b6563cec58209a1d.yaml
 releasenotes/notes/add-share-group-support-a3166f6ca4d06a81.yaml
 releasenotes/notes/add-share-network-sec-service-add-update-to-in-use-networks-ec7a60d07ebceaf4.yaml
 releasenotes/notes/add-share-replicas-and-replica-gigabytes-quotas-909436c2b2420f2c.yaml
 releasenotes/notes/add-snapshot-instances-admin-api-3cf3114doe40k598.yaml
+releasenotes/notes/add-snapshot-metadata-49b0288bf2f12bf0.yaml
 releasenotes/notes/add-support-filter-search-for-share-type-fdbaaa9510cc59dd.yaml
 releasenotes/notes/add-support-to-check-quota-usage-scfdg14dod40k71a.yaml
 releasenotes/notes/add_support_multiple_subnet_per_az-46145c3e90e097be.yaml
 releasenotes/notes/bp-export-locations-replica-az-commands-03aa32c08f59c42d.yaml
 releasenotes/notes/bp-integrate-os-profiler-4818066dc2fbf7b7.yaml
 releasenotes/notes/bp-ocata-migration-improvements-f63c5d233856fbee.yaml
 releasenotes/notes/bp-support-group-spec-search-share-group-type-api-d5d9a6096f084b91.yaml
@@ -330,14 +332,15 @@
 releasenotes/notes/bug-1920888-fix-error-in-cli-manila-list-with-sorting-key-availabilityzone-cea5a1f5d8a38fc3.yaml
 releasenotes/notes/bug-1925486-add-share-network-option-to-replica-create-api-7d2ff3628e93fc77.yaml
 releasenotes/notes/bug-1953670-fix-id-attr-for-share-group-type-access-repr-008338a53d7a6a50.yaml
 releasenotes/notes/bug-1959329-fix-server-listing-by-subnets-fa6447fd43093cae.yaml
 releasenotes/notes/bug-1960422-fix-no-default-share-type-d6191ea0aa1e57fa.yaml
 releasenotes/notes/bug-1975488-skip-force-kwarg-if-unspecified-f98c717df1d6e364.yaml
 releasenotes/notes/bug-1980985-dont-use-share-type-with-snapshot-ref-de0331c640afbbd3.yaml
+releasenotes/notes/bug-1999775-add-os-key-0cfc95c7b480df05.yaml
 releasenotes/notes/bug-share-access-list-3cf3114doe40k599.yaml
 releasenotes/notes/bug_1570085_fix-905786b797379309.yaml
 releasenotes/notes/bug_1603387_fix_env_variable_8ed5450aab41aa5f.yaml
 releasenotes/notes/bug_1606168_fix-54d3c3bb78389f01.yaml
 releasenotes/notes/bug_1715769_fix-3ec701b0fb9d7910.yaml
 releasenotes/notes/bug_1777849_1779935_fix-344cb8f09b7df502.yaml
 releasenotes/notes/bug_1782672-1954059b373f03de.yaml
```

### Comparing `python-manilaclient-4.2.0/python_manilaclient.egg-info/entry_points.txt` & `python-manilaclient-4.3.0/python_manilaclient.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/rally-jobs/rally-manila-no-ss.yaml` & `python-manilaclient-4.3.0/rally-jobs/rally-manila-no-ss.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/rally-jobs/rally-manila.yaml` & `python-manilaclient-4.3.0/rally-jobs/rally-manila.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/releasenotes/notes/add-share-network-sec-service-add-update-to-in-use-networks-ec7a60d07ebceaf4.yaml` & `python-manilaclient-4.3.0/releasenotes/notes/add-share-network-sec-service-add-update-to-in-use-networks-ec7a60d07ebceaf4.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/releasenotes/notes/deprecate-v1-a0cfa6fd723c2f46.yaml` & `python-manilaclient-4.3.0/releasenotes/notes/deprecate-v1-a0cfa6fd723c2f46.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/releasenotes/notes/manila-openstackclient-bf61ceb270d3afb7.yaml` & `python-manilaclient-4.3.0/releasenotes/notes/manila-openstackclient-bf61ceb270d3afb7.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/releasenotes/notes/newton-migration-improvements-166a03472948bdef.yaml` & `python-manilaclient-4.3.0/releasenotes/notes/newton-migration-improvements-166a03472948bdef.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/releasenotes/notes/remove-experimental-flag-from-share-groups-feature-dcf2b0b67fe4cac4.yaml` & `python-manilaclient-4.3.0/releasenotes/notes/remove-experimental-flag-from-share-groups-feature-dcf2b0b67fe4cac4.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/releasenotes/notes/share-network-multiple-subnets-732309abfbf5987c.yaml` & `python-manilaclient-4.3.0/releasenotes/notes/share-network-multiple-subnets-732309abfbf5987c.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/releasenotes/source/conf.py` & `python-manilaclient-4.3.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/requirements.txt` & `python-manilaclient-4.3.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/roles/populate-manilaclient-config/README.rst` & `python-manilaclient-4.3.0/roles/populate-manilaclient-config/README.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/roles/populate-manilaclient-config/tasks/main.yaml` & `python-manilaclient-4.3.0/roles/populate-manilaclient-config/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/run_tests.sh` & `python-manilaclient-4.3.0/run_tests.sh`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/setup.cfg` & `python-manilaclient-4.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/setup.py` & `python-manilaclient-4.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.2.0/tox.ini` & `python-manilaclient-4.3.0/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 [tox]
 distribute = False
 envlist = py3,pep8
 minversion = 3.18.0
-skipsdist = True
 # Automatic envs (pyXX) will only use the python version appropriate to that
 # env and ignore basepython inherited from [testenv] if we set
 # ignore_basepython_conflict.
 ignore_basepython_conflict = true
 
 [testenv]
 basepython = python3
@@ -29,25 +28,23 @@
 commands =
   flake8
 
 [testenv:venv]
 commands = {posargs}
 
 [testenv:docs]
-usedevelop = True
 deps =
        -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
        -r{toxinidir}/doc/requirements.txt
 allowlist_externals = rm
 commands =
   rm -rf doc/build
   sphinx-build -b html doc/source doc/build/html
 
 [testenv:pdf-docs]
-usedevelop = True
 deps = {[testenv:docs]deps}
 allowlist_externals =
   make
 commands =
   sphinx-build  -W -b latex doc/source doc/build/pdf
   make -C doc/build/pdf
```

### Comparing `python-manilaclient-4.2.0/zuul.d/python-manilaclient-jobs.yaml` & `python-manilaclient-4.3.0/zuul.d/python-manilaclient-jobs.yaml`

 * *Files identical despite different names*

