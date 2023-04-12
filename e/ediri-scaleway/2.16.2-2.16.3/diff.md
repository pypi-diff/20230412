# Comparing `tmp/ediri_scaleway-2.16.2.tar.gz` & `tmp/ediri_scaleway-2.16.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ediri_scaleway-2.16.2.tar", last modified: Sun Apr  9 18:36:49 2023, max compression
+gzip compressed data, was "ediri_scaleway-2.16.3.tar", last modified: Wed Apr 12 09:11:34 2023, max compression
```

## Comparing `ediri_scaleway-2.16.2.tar` & `ediri_scaleway-2.16.3.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:36:49.282122 ediri_scaleway-2.16.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-09 18:36:49.282122 ediri_scaleway-2.16.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:36:49.282122 ediri_scaleway-2.16.2/ediri_scaleway/
--rw-r--r--   0 runner    (1001) docker     (123)    18441 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   155818 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    12817 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/account_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    16591 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/account_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    18156 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/apple_silicon_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    50133 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/baremetal_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/cockpit.py
--rw-r--r--   0 runner    (1001) docker     (123)    12426 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/cockpit_grafana_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    13197 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/cockpit_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:36:49.282122 ediri_scaleway-2.16.2/ediri_scaleway/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    57754 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    15443 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/container_cron.py
--rw-r--r--   0 runner    (1001) docker     (123)    14192 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/container_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    25163 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/container_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)    16123 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/container_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    49237 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/domain_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    16997 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/domain_zone.py
--rw-r--r--   0 runner    (1001) docker     (123)    23692 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/flexible_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)    50956 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/function.py
--rw-r--r--   0 runner    (1001) docker     (123)    16513 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/function_cron.py
--rw-r--r--   0 runner    (1001) docker     (123)    13658 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/function_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    22652 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/function_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)    16221 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/function_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_account_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_account_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_baremetal_offer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_baremetal_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_baremetal_os.py
--rw-r--r--   0 runner    (1001) docker     (123)    12906 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_baremetal_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_cockpit.py
--rw-r--r--   0 runner    (1001) docker     (123)    17262 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     9371 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_container_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_domain_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_domain_zone.py
--rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_flexible_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_function_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_iam_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_iam_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_iam_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_iam_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    11595 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_instance_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_instance_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_instance_private_nic.py
--rw-r--r--   0 runner    (1001) docker     (123)    10840 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_instance_security_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    17259 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_instance_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     6516 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_instance_servers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_instance_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_instance_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_iot_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    10978 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_iot_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)    15618 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_k8s_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    15518 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_k8s_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_k8s_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_lb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_lb_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)    16819 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_lb_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_lb_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_lb_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_lb_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_lb_frontends.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_lb_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_lb_ips.py
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_lb_route.py
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_lb_routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_lbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_marketplace_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_object_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_rdb_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_rdb_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_rdb_database_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)    14520 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_rdb_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_rdb_privilege.py
--rw-r--r--   0 runner    (1001) docker     (123)    11070 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_redis_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_registry_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_registry_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_secret_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8769 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_tem_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_vpc_gateway_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_vpc_private_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     9542 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_vpc_public_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_vpc_public_gateway_dhcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9251 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_vpc_public_gateway_dhcp_reservation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_vpc_public_gateway_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_vpc_public_gateway_pat_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6058 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/get_web_host_offer.py
--rw-r--r--   0 runner    (1001) docker     (123)    23351 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/iam_api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    14010 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/iam_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    18177 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/iam_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    24564 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/iam_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    16556 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/iam_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    30002 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/instance_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/instance_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/instance_ip_reverse_dns.py
--rw-r--r--   0 runner    (1001) docker     (123)    21043 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/instance_placement_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    15355 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/instance_private_nic.py
--rw-r--r--   0 runner    (1001) docker     (123)    35854 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/instance_security_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    13285 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/instance_security_group_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    70543 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/instance_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    25939 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/instance_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)    12709 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/instance_user_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    24213 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/instance_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    27308 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/iot_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    32719 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/iot_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/iot_network.py
--rw-r--r--   0 runner    (1001) docker     (123)    17326 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/iot_route.py
--rw-r--r--   0 runner    (1001) docker     (123)    53788 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/k8s_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    53970 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/k8s_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    36315 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/lb.py
--rw-r--r--   0 runner    (1001) docker     (123)    67438 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/lb_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    20988 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/lb_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    23436 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/lb_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    14291 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/lb_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/lb_route.py
--rw-r--r--   0 runner    (1001) docker     (123)    16571 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/mnq_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)    16922 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/mnq_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)    36145 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/object_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    23973 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/object_bucket_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11954 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/object_bucket_lock_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    11764 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/object_bucket_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    24785 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/object_bucket_website_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    24069 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/object_item.py
--rw-r--r--   0 runner    (1001) docker     (123)   249319 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/rdb_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    13109 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/rdb_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    19284 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/rdb_database_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)    61205 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/rdb_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    16572 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/rdb_privilege.py
--rw-r--r--   0 runner    (1001) docker     (123)    16480 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/rdb_read_replica.py
--rw-r--r--   0 runner    (1001) docker     (123)    14226 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/rdb_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    43382 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/redis_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    16962 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/registry_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)    18659 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    17069 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/secret_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    23279 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/tem_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    27758 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/vpc_gateway_network.py
--rw-r--r--   0 runner    (1001) docker     (123)    16578 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/vpc_private_network.py
--rw-r--r--   0 runner    (1001) docker     (123)    28639 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/vpc_public_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    44997 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/vpc_public_gateway_dhcp.py
--rw-r--r--   0 runner    (1001) docker     (123)    22479 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/vpc_public_gateway_dhcp_reservation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17679 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/vpc_public_gateway_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)    11651 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/vpc_public_gateway_ip_reverse_dns.py
--rw-r--r--   0 runner    (1001) docker     (123)    21775 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/ediri_scaleway/vpc_public_gateway_pat_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:36:49.282122 ediri_scaleway-2.16.2/ediri_scaleway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-09 18:36:49.000000 ediri_scaleway-2.16.2/ediri_scaleway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-04-09 18:36:49.000000 ediri_scaleway-2.16.2/ediri_scaleway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 18:36:49.000000 ediri_scaleway-2.16.2/ediri_scaleway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 18:36:49.000000 ediri_scaleway-2.16.2/ediri_scaleway.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-09 18:36:49.000000 ediri_scaleway-2.16.2/ediri_scaleway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-09 18:36:49.000000 ediri_scaleway-2.16.2/ediri_scaleway.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 18:36:49.282122 ediri_scaleway-2.16.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-09 18:36:48.000000 ediri_scaleway-2.16.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:11:34.773323 ediri_scaleway-2.16.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-12 09:11:34.773323 ediri_scaleway-2.16.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:11:34.773323 ediri_scaleway-2.16.3/ediri_scaleway/
+-rw-r--r--   0 runner    (1001) docker     (123)    18441 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   155818 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12817 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/account_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16591 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/account_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18156 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/apple_silicon_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50133 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/baremetal_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/cockpit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12426 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/cockpit_grafana_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13197 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/cockpit_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:11:34.773323 ediri_scaleway-2.16.3/ediri_scaleway/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57754 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15443 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/container_cron.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14192 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/container_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25163 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/container_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16123 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/container_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49237 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16997 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/domain_zone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23692 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/flexible_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50956 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16513 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/function_cron.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13658 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/function_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22652 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/function_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16221 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/function_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_account_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_account_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_baremetal_offer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_baremetal_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_baremetal_os.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12906 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_baremetal_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_cockpit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17262 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9371 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_container_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_domain_zone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_flexible_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_function_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_iam_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_iam_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_iam_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_iam_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11595 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_instance_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_instance_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_instance_private_nic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10840 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_instance_security_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17259 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_instance_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6516 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_instance_servers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_instance_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_instance_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_iot_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10978 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_iot_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15618 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_k8s_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15518 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_k8s_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_k8s_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_lb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_lb_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16819 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_lb_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_lb_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_lb_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_lb_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_lb_frontends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_lb_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_lb_ips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_lb_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_lb_routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_lbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_marketplace_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_object_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_rdb_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_rdb_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_rdb_database_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14520 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_rdb_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_rdb_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11070 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_redis_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_registry_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_registry_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_secret_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8769 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_tem_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_vpc_gateway_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_vpc_private_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9542 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_vpc_public_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_vpc_public_gateway_dhcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9251 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_vpc_public_gateway_dhcp_reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_vpc_public_gateway_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_vpc_public_gateway_pat_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6058 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/get_web_host_offer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23351 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/iam_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14010 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/iam_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18177 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/iam_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24564 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/iam_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16556 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/iam_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30002 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/instance_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/instance_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/instance_ip_reverse_dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21043 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/instance_placement_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15355 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/instance_private_nic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35854 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/instance_security_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13285 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/instance_security_group_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70543 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/instance_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25939 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/instance_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12709 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/instance_user_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24213 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/instance_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27308 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/iot_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32719 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/iot_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/iot_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17326 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/iot_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53788 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/k8s_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53970 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/k8s_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36315 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/lb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67438 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/lb_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20988 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/lb_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23436 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/lb_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14291 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/lb_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/lb_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16571 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/mnq_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16922 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/mnq_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36145 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/object_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23973 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/object_bucket_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11954 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/object_bucket_lock_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11764 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/object_bucket_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24785 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/object_bucket_website_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24069 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/object_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)   249319 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/rdb_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13109 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/rdb_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19284 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/rdb_database_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61205 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/rdb_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16572 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/rdb_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16480 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/rdb_read_replica.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14226 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/rdb_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43382 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/redis_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16962 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/registry_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18659 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17069 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/secret_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23279 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/tem_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27758 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/vpc_gateway_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16578 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/vpc_private_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28639 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/vpc_public_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44997 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/vpc_public_gateway_dhcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22479 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/vpc_public_gateway_dhcp_reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17679 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/vpc_public_gateway_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11651 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/vpc_public_gateway_ip_reverse_dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21775 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway/vpc_public_gateway_pat_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:11:34.773323 ediri_scaleway-2.16.3/ediri_scaleway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/ediri_scaleway.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 09:11:34.773323 ediri_scaleway-2.16.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-12 09:11:34.000000 ediri_scaleway-2.16.3/setup.py
```

### Comparing `ediri_scaleway-2.16.2/PKG-INFO` & `ediri_scaleway-2.16.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ediri_scaleway
-Version: 2.16.2
+Version: 2.16.3
 Summary: A Pulumi package for creating and managing Scaleway resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/dirien/pulumi-scaleway
 Keywords: pulumi scaleway category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `ediri_scaleway-2.16.2/README.md` & `ediri_scaleway-2.16.3/README.md`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/__init__.py` & `ediri_scaleway-2.16.3/ediri_scaleway/__init__.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/_inputs.py` & `ediri_scaleway-2.16.3/ediri_scaleway/_inputs.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/_utilities.py` & `ediri_scaleway-2.16.3/ediri_scaleway/_utilities.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/account_project.py` & `ediri_scaleway-2.16.3/ediri_scaleway/account_project.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/account_ssh_key.py` & `ediri_scaleway-2.16.3/ediri_scaleway/account_ssh_key.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/apple_silicon_server.py` & `ediri_scaleway-2.16.3/ediri_scaleway/apple_silicon_server.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/baremetal_server.py` & `ediri_scaleway-2.16.3/ediri_scaleway/baremetal_server.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/cockpit.py` & `ediri_scaleway-2.16.3/ediri_scaleway/cockpit.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/cockpit_grafana_user.py` & `ediri_scaleway-2.16.3/ediri_scaleway/cockpit_grafana_user.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/cockpit_token.py` & `ediri_scaleway-2.16.3/ediri_scaleway/cockpit_token.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/config/vars.py` & `ediri_scaleway-2.16.3/ediri_scaleway/config/vars.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/container.py` & `ediri_scaleway-2.16.3/ediri_scaleway/container.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/container_cron.py` & `ediri_scaleway-2.16.3/ediri_scaleway/container_cron.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/container_domain.py` & `ediri_scaleway-2.16.3/ediri_scaleway/container_domain.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/container_namespace.py` & `ediri_scaleway-2.16.3/ediri_scaleway/container_namespace.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/container_token.py` & `ediri_scaleway-2.16.3/ediri_scaleway/container_token.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/domain_record.py` & `ediri_scaleway-2.16.3/ediri_scaleway/domain_record.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/domain_zone.py` & `ediri_scaleway-2.16.3/ediri_scaleway/domain_zone.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/flexible_ip.py` & `ediri_scaleway-2.16.3/ediri_scaleway/flexible_ip.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/function.py` & `ediri_scaleway-2.16.3/ediri_scaleway/function.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/function_cron.py` & `ediri_scaleway-2.16.3/ediri_scaleway/function_cron.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/function_domain.py` & `ediri_scaleway-2.16.3/ediri_scaleway/function_domain.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/function_namespace.py` & `ediri_scaleway-2.16.3/ediri_scaleway/function_namespace.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/function_token.py` & `ediri_scaleway-2.16.3/ediri_scaleway/function_token.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_account_project.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_account_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     @property
     @pulumi.getter(name="organizationId")
     def organization_id(self) -> Optional[str]:
         return pulumi.get(self, "organization_id")
 
     @property
     @pulumi.getter(name="projectId")
-    def project_id(self) -> Optional[str]:
+    def project_id(self) -> str:
         return pulumi.get(self, "project_id")
 
     @property
     @pulumi.getter(name="updatedAt")
     def updated_at(self) -> str:
         return pulumi.get(self, "updated_at")
```

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_account_ssh_key.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_account_ssh_key.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_baremetal_offer.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_baremetal_offer.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_baremetal_option.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_baremetal_option.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_baremetal_os.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_baremetal_os.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_baremetal_server.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_baremetal_server.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_cockpit.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_cockpit.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_container.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_container.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_container_namespace.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_container_namespace.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_domain_record.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_domain_record.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_domain_zone.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_domain_zone.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_flexible_ip.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_flexible_ip.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_function.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_function.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_function_namespace.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_function_namespace.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_iam_application.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_iam_application.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_iam_group.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_iam_group.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_iam_ssh_key.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_iam_ssh_key.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_iam_user.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_iam_user.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_instance_image.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_instance_image.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_instance_ip.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_instance_ip.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_instance_private_nic.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_instance_private_nic.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_instance_security_group.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_instance_security_group.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_instance_server.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_instance_server.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_instance_servers.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_instance_servers.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_instance_snapshot.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_instance_snapshot.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_instance_volume.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_instance_volume.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_iot_device.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_iot_device.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_iot_hub.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_iot_hub.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_k8s_cluster.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_k8s_cluster.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_k8s_pool.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_k8s_pool.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_k8s_version.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_k8s_version.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_lb.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_lb.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_lb_acls.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_lb_acls.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_lb_backend.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_lb_backend.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_lb_backends.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_lb_backends.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_lb_certificate.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_lb_certificate.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_lb_frontend.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_lb_frontend.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_lb_frontends.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_lb_frontends.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_lb_ip.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_lb_ip.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_lb_ips.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_lb_ips.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_lb_route.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_lb_route.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_lb_routes.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_lb_routes.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_lbs.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_lbs.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_marketplace_image.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_marketplace_image.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_object_bucket.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_object_bucket.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_rdb_acl.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_rdb_acl.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_rdb_database.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_rdb_database.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_rdb_database_backup.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_rdb_database_backup.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_rdb_instance.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_rdb_instance.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_rdb_privilege.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_rdb_privilege.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_redis_cluster.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_redis_cluster.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_registry_image.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_registry_image.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_registry_namespace.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_registry_namespace.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_secret.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_secret.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_secret_version.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_secret_version.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_tem_domain.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_tem_domain.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_vpc_gateway_network.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_vpc_gateway_network.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_vpc_private_network.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_vpc_private_network.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_vpc_public_gateway.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_vpc_public_gateway.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_vpc_public_gateway_dhcp.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_vpc_public_gateway_dhcp.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_vpc_public_gateway_dhcp_reservation.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_vpc_public_gateway_dhcp_reservation.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_vpc_public_gateway_ip.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_vpc_public_gateway_ip.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_vpc_public_gateway_pat_rule.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_vpc_public_gateway_pat_rule.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/get_web_host_offer.py` & `ediri_scaleway-2.16.3/ediri_scaleway/get_web_host_offer.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/iam_api_key.py` & `ediri_scaleway-2.16.3/ediri_scaleway/iam_api_key.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/iam_application.py` & `ediri_scaleway-2.16.3/ediri_scaleway/iam_application.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/iam_group.py` & `ediri_scaleway-2.16.3/ediri_scaleway/iam_group.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/iam_policy.py` & `ediri_scaleway-2.16.3/ediri_scaleway/iam_policy.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/iam_ssh_key.py` & `ediri_scaleway-2.16.3/ediri_scaleway/iam_ssh_key.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/instance_image.py` & `ediri_scaleway-2.16.3/ediri_scaleway/instance_image.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/instance_ip.py` & `ediri_scaleway-2.16.3/ediri_scaleway/instance_ip.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/instance_ip_reverse_dns.py` & `ediri_scaleway-2.16.3/ediri_scaleway/instance_ip_reverse_dns.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/instance_placement_group.py` & `ediri_scaleway-2.16.3/ediri_scaleway/instance_placement_group.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/instance_private_nic.py` & `ediri_scaleway-2.16.3/ediri_scaleway/instance_private_nic.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/instance_security_group.py` & `ediri_scaleway-2.16.3/ediri_scaleway/instance_security_group.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/instance_security_group_rules.py` & `ediri_scaleway-2.16.3/ediri_scaleway/instance_security_group_rules.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/instance_server.py` & `ediri_scaleway-2.16.3/ediri_scaleway/instance_server.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/instance_snapshot.py` & `ediri_scaleway-2.16.3/ediri_scaleway/instance_snapshot.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/instance_user_data.py` & `ediri_scaleway-2.16.3/ediri_scaleway/instance_user_data.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/instance_volume.py` & `ediri_scaleway-2.16.3/ediri_scaleway/instance_volume.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/iot_device.py` & `ediri_scaleway-2.16.3/ediri_scaleway/iot_device.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/iot_hub.py` & `ediri_scaleway-2.16.3/ediri_scaleway/iot_hub.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/iot_network.py` & `ediri_scaleway-2.16.3/ediri_scaleway/iot_network.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/iot_route.py` & `ediri_scaleway-2.16.3/ediri_scaleway/iot_route.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/k8s_cluster.py` & `ediri_scaleway-2.16.3/ediri_scaleway/k8s_cluster.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/k8s_pool.py` & `ediri_scaleway-2.16.3/ediri_scaleway/k8s_pool.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/lb.py` & `ediri_scaleway-2.16.3/ediri_scaleway/lb.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/lb_backend.py` & `ediri_scaleway-2.16.3/ediri_scaleway/lb_backend.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/lb_certificate.py` & `ediri_scaleway-2.16.3/ediri_scaleway/lb_certificate.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/lb_frontend.py` & `ediri_scaleway-2.16.3/ediri_scaleway/lb_frontend.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/lb_ip.py` & `ediri_scaleway-2.16.3/ediri_scaleway/lb_ip.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/lb_route.py` & `ediri_scaleway-2.16.3/ediri_scaleway/lb_route.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/mnq_credential.py` & `ediri_scaleway-2.16.3/ediri_scaleway/mnq_credential.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/mnq_namespace.py` & `ediri_scaleway-2.16.3/ediri_scaleway/mnq_namespace.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/object_bucket.py` & `ediri_scaleway-2.16.3/ediri_scaleway/object_bucket.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/object_bucket_acl.py` & `ediri_scaleway-2.16.3/ediri_scaleway/object_bucket_acl.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/object_bucket_lock_configuration.py` & `ediri_scaleway-2.16.3/ediri_scaleway/object_bucket_lock_configuration.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/object_bucket_policy.py` & `ediri_scaleway-2.16.3/ediri_scaleway/object_bucket_policy.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/object_bucket_website_configuration.py` & `ediri_scaleway-2.16.3/ediri_scaleway/object_bucket_website_configuration.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/object_item.py` & `ediri_scaleway-2.16.3/ediri_scaleway/object_item.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/outputs.py` & `ediri_scaleway-2.16.3/ediri_scaleway/outputs.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/provider.py` & `ediri_scaleway-2.16.3/ediri_scaleway/provider.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/rdb_acl.py` & `ediri_scaleway-2.16.3/ediri_scaleway/rdb_acl.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/rdb_database.py` & `ediri_scaleway-2.16.3/ediri_scaleway/rdb_database.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/rdb_database_backup.py` & `ediri_scaleway-2.16.3/ediri_scaleway/rdb_database_backup.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/rdb_instance.py` & `ediri_scaleway-2.16.3/ediri_scaleway/rdb_instance.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/rdb_privilege.py` & `ediri_scaleway-2.16.3/ediri_scaleway/rdb_privilege.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/rdb_read_replica.py` & `ediri_scaleway-2.16.3/ediri_scaleway/rdb_read_replica.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/rdb_user.py` & `ediri_scaleway-2.16.3/ediri_scaleway/rdb_user.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/redis_cluster.py` & `ediri_scaleway-2.16.3/ediri_scaleway/redis_cluster.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/registry_namespace.py` & `ediri_scaleway-2.16.3/ediri_scaleway/registry_namespace.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/secret.py` & `ediri_scaleway-2.16.3/ediri_scaleway/secret.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/secret_version.py` & `ediri_scaleway-2.16.3/ediri_scaleway/secret_version.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/tem_domain.py` & `ediri_scaleway-2.16.3/ediri_scaleway/tem_domain.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/vpc_gateway_network.py` & `ediri_scaleway-2.16.3/ediri_scaleway/vpc_gateway_network.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/vpc_private_network.py` & `ediri_scaleway-2.16.3/ediri_scaleway/vpc_private_network.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/vpc_public_gateway.py` & `ediri_scaleway-2.16.3/ediri_scaleway/vpc_public_gateway.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/vpc_public_gateway_dhcp.py` & `ediri_scaleway-2.16.3/ediri_scaleway/vpc_public_gateway_dhcp.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/vpc_public_gateway_dhcp_reservation.py` & `ediri_scaleway-2.16.3/ediri_scaleway/vpc_public_gateway_dhcp_reservation.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/vpc_public_gateway_ip.py` & `ediri_scaleway-2.16.3/ediri_scaleway/vpc_public_gateway_ip.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/vpc_public_gateway_ip_reverse_dns.py` & `ediri_scaleway-2.16.3/ediri_scaleway/vpc_public_gateway_ip_reverse_dns.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway/vpc_public_gateway_pat_rule.py` & `ediri_scaleway-2.16.3/ediri_scaleway/vpc_public_gateway_pat_rule.py`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway.egg-info/PKG-INFO` & `ediri_scaleway-2.16.3/ediri_scaleway.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ediri-scaleway
-Version: 2.16.2
+Version: 2.16.3
 Summary: A Pulumi package for creating and managing Scaleway resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/dirien/pulumi-scaleway
 Keywords: pulumi scaleway category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `ediri_scaleway-2.16.2/ediri_scaleway.egg-info/SOURCES.txt` & `ediri_scaleway-2.16.3/ediri_scaleway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ediri_scaleway-2.16.2/setup.py` & `ediri_scaleway-2.16.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "2.16.2"
-PLUGIN_VERSION = "2.16.2"
+VERSION = "2.16.3"
+PLUGIN_VERSION = "2.16.3"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'scaleway', PLUGIN_VERSION, '--server', 'github://api.github.com/dirien/pulumi-scaleway'])
         except OSError as error:
```

