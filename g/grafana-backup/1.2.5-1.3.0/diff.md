# Comparing `tmp/grafana-backup-1.2.5.tar.gz` & `tmp/grafana-backup-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grafana-backup-1.2.5.tar", last modified: Tue Feb 21 07:53:03 2023, max compression
+gzip compressed data, was "grafana-backup-1.3.0.tar", last modified: Wed Apr 12 05:36:31 2023, max compression
```

## Comparing `grafana-backup-1.2.5.tar` & `grafana-backup-1.3.0.tar`

### file list

```diff
@@ -1,72 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:53:03.666027 grafana-backup-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-02-21 07:53:03.666027 grafana-backup-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9726 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:53:03.662027 grafana-backup-1.2.5/grafana_backup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/api_checks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1061 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/azure_storage_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/azure_storage_upload.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2644 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1398 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/commons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:53:03.662027 grafana-backup-1.2.5/grafana_backup/conf/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/conf/grafanaSettings.json
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/create_alert_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/create_annotation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1078 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/create_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/create_datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/create_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/create_library_element.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1225 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/create_org.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/create_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/create_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/create_team_member.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1631 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/create_user.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21066 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/dashboardApi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2343 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/delete_alert_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/delete_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/delete_dashboards.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/delete_datasources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/delete_folders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/delete_library_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/delete_snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/delete_team_members.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/delete_teams.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/gcs_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/gcs_upload.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8381 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/grafanaSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/influx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/make_users_viewers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1992 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/pause_alerts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6337 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/restore.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1188 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/restore_user_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/s3_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/s3_upload.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3557 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/save_alert_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/save_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/save_dashboards.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/save_datasources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/save_folders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/save_library_elements.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3408 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/save_orgs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/save_snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/save_team_members.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/save_teams.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3766 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/save_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/save_versions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1813 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/tools.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1379 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/unpause_alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/grafana_backup/update_folder_permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:53:03.662027 grafana-backup-1.2.5/grafana_backup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-02-21 07:53:03.000000 grafana-backup-1.2.5/grafana_backup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-02-21 07:53:03.000000 grafana-backup-1.2.5/grafana_backup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 07:53:03.000000 grafana-backup-1.2.5/grafana_backup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-02-21 07:53:03.000000 grafana-backup-1.2.5/grafana_backup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-02-21 07:53:03.000000 grafana-backup-1.2.5/grafana_backup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-21 07:53:03.000000 grafana-backup-1.2.5/grafana_backup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-21 07:53:03.666027 grafana-backup-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-02-21 07:52:45.000000 grafana-backup-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:36:31.173667 grafana-backup-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10140 2023-04-12 05:36:31.173667 grafana-backup-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:36:31.173667 grafana-backup-1.3.0/grafana_backup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/api_checks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1076 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/azure_storage_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/azure_storage_upload.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2656 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1398 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/commons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:36:31.173667 grafana-backup-1.3.0/grafana_backup/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/conf/grafanaSettings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/create_alert_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/create_alert_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/create_annotation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1078 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/create_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/create_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/create_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/create_library_element.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1225 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/create_org.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/create_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/create_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/create_team_member.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1631 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/create_user.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22704 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/dashboardApi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2343 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/delete_alert_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/delete_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/delete_dashboards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/delete_datasources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/delete_folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/delete_library_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/delete_snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/delete_team_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/delete_teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/gcs_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/gcs_upload.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8381 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/grafanaSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/influx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/make_users_viewers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1992 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/pause_alerts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6464 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/restore.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1188 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/restore_user_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/s3_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/s3_upload.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3688 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/save_alert_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/save_alert_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/save_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/save_dashboards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/save_datasources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/save_folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/save_library_elements.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3408 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/save_orgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/save_snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/save_team_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/save_teams.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3766 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/save_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/save_versions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1813 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/tools.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1379 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/unpause_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/grafana_backup/update_folder_permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:36:31.173667 grafana-backup-1.3.0/grafana_backup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10140 2023-04-12 05:36:31.000000 grafana-backup-1.3.0/grafana_backup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-12 05:36:31.000000 grafana-backup-1.3.0/grafana_backup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 05:36:31.000000 grafana-backup-1.3.0/grafana_backup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-12 05:36:31.000000 grafana-backup-1.3.0/grafana_backup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-12 05:36:31.000000 grafana-backup-1.3.0/grafana_backup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 05:36:31.000000 grafana-backup-1.3.0/grafana_backup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 05:36:31.173667 grafana-backup-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-12 05:36:13.000000 grafana-backup-1.3.0/setup.py
```

### Comparing `grafana-backup-1.2.5/LICENSE` & `grafana-backup-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/PKG-INFO` & `grafana-backup-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grafana-backup
-Version: 1.2.5
+Version: 1.3.0
 Summary: A Python-based application to backup Grafana settings using the Grafana API
 Home-page: https://github.com/ysde/grafana-backup-tool
 Author: author
 Author-email: ysde108@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -22,14 +22,15 @@
 ## Supported components
 * Folder
 * Folder Permissions
 * Library Elements (doesn't work with Grafana 8.0.0 but 8.4.3)
 * Dashboard (contains Alert)
 * Datasource
 * Alert Channel
+* Alert Rules (Supported in version 9.4.0 of grafana and up.)
 * Teams
 * Team Members (Needs Basic Authentication (username and password, see [grafana doc](https://grafana.com/docs/grafana/latest/http_api/org/#admin-organizations-api))
     * You need to set `Admin's account and password` in `grafanaSettings.json`, or set the base64 encoded `admin account and password` in ENV `GRAFANA_BASIC_AUTH`. E.g `export GRAFANA_BASIC_AUTH=YWRtaW46YWRtaW4=`
     * Or Sets this ENV of the Grafana server `GF_USERS_ALLOW_ORG_CREATE=true`. see [grafana doc](https://grafana.com/docs/grafana/latest/http_api/org/#create-organization)
 * Organization (Needs Basic Authentication (username and password, see [grafana doc](https://grafana.com/docs/grafana/latest/http_api/org/#admin-organizations-api))
     * You need to set `Admin's account and password` in `grafanaSettings.json`, or set the base64 encoded `admin account and password` in ENV `GRAFANA_BASIC_AUTH`. E.g `export GRAFANA_BASIC_AUTH=YWRtaW46YWRtaW4=`
     * Or Sets this ENV of the Grafana server `GF_USERS_ALLOW_ORG_CREATE=true`. see [grafana doc](https://grafana.com/docs/grafana/latest/http_api/org/#create-organization)
@@ -178,14 +179,15 @@
 		   -e AZURE_STORAGE_CONTAINER_NAME="azure-storage-container-name" \
 		   -e AZURE_STORAGE_CONNECTION_STRING="azure-storage-connection-string"
 ```
 
 ***GCS Example:*** Set GCS configurations in `-e` or `grafanaSettings.json`([example](https://github.com/ysde/grafana-backup-tool/blob/master/examples/grafana-backup.example.json))
 ```
 		   -e GCS_BUCKET_NAME="bucket-name" \
+		   -e GCLOUD_PROJECT="gcp-project-name" \
 		   -e GOOGLE_APPLICATION_CREDENTIALS="credential-file-path"
 ```
 
 
 ### Restore
 
 ```
```

### Comparing `grafana-backup-1.2.5/README.md` & `grafana-backup-1.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 ## Supported components
 * Folder
 * Folder Permissions
 * Library Elements (doesn't work with Grafana 8.0.0 but 8.4.3)
 * Dashboard (contains Alert)
 * Datasource
 * Alert Channel
+* Alert Rules (Supported in version 9.4.0 of grafana and up.)
 * Teams
 * Team Members (Needs Basic Authentication (username and password, see [grafana doc](https://grafana.com/docs/grafana/latest/http_api/org/#admin-organizations-api))
     * You need to set `Admin's account and password` in `grafanaSettings.json`, or set the base64 encoded `admin account and password` in ENV `GRAFANA_BASIC_AUTH`. E.g `export GRAFANA_BASIC_AUTH=YWRtaW46YWRtaW4=`
     * Or Sets this ENV of the Grafana server `GF_USERS_ALLOW_ORG_CREATE=true`. see [grafana doc](https://grafana.com/docs/grafana/latest/http_api/org/#create-organization)
 * Organization (Needs Basic Authentication (username and password, see [grafana doc](https://grafana.com/docs/grafana/latest/http_api/org/#admin-organizations-api))
     * You need to set `Admin's account and password` in `grafanaSettings.json`, or set the base64 encoded `admin account and password` in ENV `GRAFANA_BASIC_AUTH`. E.g `export GRAFANA_BASIC_AUTH=YWRtaW46YWRtaW4=`
     * Or Sets this ENV of the Grafana server `GF_USERS_ALLOW_ORG_CREATE=true`. see [grafana doc](https://grafana.com/docs/grafana/latest/http_api/org/#create-organization)
@@ -168,14 +169,15 @@
 		   -e AZURE_STORAGE_CONTAINER_NAME="azure-storage-container-name" \
 		   -e AZURE_STORAGE_CONNECTION_STRING="azure-storage-connection-string"
 ```
 
 ***GCS Example:*** Set GCS configurations in `-e` or `grafanaSettings.json`([example](https://github.com/ysde/grafana-backup-tool/blob/master/examples/grafana-backup.example.json))
 ```
 		   -e GCS_BUCKET_NAME="bucket-name" \
+		   -e GCLOUD_PROJECT="gcp-project-name" \
 		   -e GOOGLE_APPLICATION_CREDENTIALS="credential-file-path"
 ```
 
 
 ### Restore
 
 ```
```

### Comparing `grafana-backup-1.2.5/grafana_backup/api_checks.py` & `grafana-backup-1.3.0/grafana_backup/api_checks.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/archive.py` & `grafana-backup-1.3.0/grafana_backup/archive.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     backup_dir = settings.get('BACKUP_DIR')
     timestamp = settings.get('TIMESTAMP')
 
     archive_file = '{0}/{1}.tar.gz'.format(backup_dir, timestamp)
     backup_files = list()
 
     for folder_name in ['folders', 'datasources', 'dashboards', 'alert_channels', 'organizations', 'users', 'snapshots',
-                        'versions', 'annotations', 'library-elements', 'teams', 'team_members']:
+                        'versions', 'annotations', 'library-elements', 'teams', 'team_members', 'alert_rules']:
         backup_path = '{0}/{1}/{2}'.format(backup_dir, folder_name, timestamp)
 
         for file_path in glob(backup_path):
             print('backup {0} at: {1}'.format(folder_name, file_path))
             backup_files.append(file_path)
 
     if os.path.exists(archive_file):
```

### Comparing `grafana-backup-1.2.5/grafana_backup/azure_storage_download.py` & `grafana-backup-1.3.0/grafana_backup/azure_storage_download.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/azure_storage_upload.py` & `grafana-backup-1.3.0/grafana_backup/azure_storage_upload.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/cli.py` & `grafana-backup-1.3.0/grafana_backup/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     grafana-backup --version
 
 Options:
     -h --help                               Show this help message and exit
     --version                               Get version information and exit
     --config=<filename>                     Override default configuration path
     --components=<>                         Comma separated list of individual components to backup (all by default); versions can only be saved not restored.
-                                            <folders,folder_permissions,dashboards,datasources,alert-channels,organizations,users,snapshots,versions,annotations,library_elements,teams,team_members>
+                                            <folders,folder_permissions,dashboards,datasources,alert-channels,alert-rules,organizations,users,snapshots,versions,annotations,library_elements,teams,team_members>
 
     --no-archive                            Skip archive creation and do not delete unarchived files
                                             (used for troubleshooting purposes)
 """.format(PKG_NAME, PKG_VERSION)
 
 
 args = docopt(docstring, help=False,
```

### Comparing `grafana-backup-1.2.5/grafana_backup/commons.py` & `grafana-backup-1.3.0/grafana_backup/commons.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/create_alert_channel.py` & `grafana-backup-1.3.0/grafana_backup/create_alert_channel.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/create_annotation.py` & `grafana-backup-1.3.0/grafana_backup/create_annotation.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/create_dashboard.py` & `grafana-backup-1.3.0/grafana_backup/create_dashboard.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/create_datasource.py` & `grafana-backup-1.3.0/grafana_backup/create_datasource.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/create_folder.py` & `grafana-backup-1.3.0/grafana_backup/create_folder.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/create_library_element.py` & `grafana-backup-1.3.0/grafana_backup/create_library_element.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,13 +11,28 @@
 
     with open(file_path, 'r') as f:
         data = f.read()
 
     # Library Elements can only be created referencing a folder id. However, this folder id is not unique across Grafana
     # instances. Therefore, we need to first find the folder id by the given folder uid.
     library_element = json.loads(data)
-    folder_uid = library_element['meta']['folderUid']
-    folder_id = get_folder(folder_uid, grafana_url, http_post_headers, verify_ssl, client_cert, debug)[1]['id']
-    library_element['folderId'] = folder_id
-    result = create_library_element(json.dumps(library_element), grafana_url, http_post_headers, verify_ssl,
-                                    client_cert, debug)
-    print("create library_elements: {0}, status: {1}, msg: {2}".format(library_element['name'], result[0], result[1]))
+    folder_uid = library_element["meta"]["folderUid"]
+    folder_id_response = get_folder(
+        folder_uid, grafana_url, http_post_headers, verify_ssl, client_cert, debug
+    )[1]
+    if isinstance(folder_id_response, list):
+        library_element["folderUid"] = folder_id_response[0]['uid']
+    else:
+        library_element["folderUid"] = folder_id_response['uid']
+    result = create_library_element(
+        json.dumps(library_element),
+        grafana_url,
+        http_post_headers,
+        verify_ssl,
+        client_cert,
+        debug,
+    )
+    print(
+        "create library_elements: {0}, status: {1}, msg: {2}".format(
+            library_element["name"], result[0], result[1]
+        )
+    )
```

### Comparing `grafana-backup-1.2.5/grafana_backup/create_org.py` & `grafana-backup-1.3.0/grafana_backup/create_org.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/create_snapshot.py` & `grafana-backup-1.3.0/grafana_backup/create_snapshot.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/create_team.py` & `grafana-backup-1.3.0/grafana_backup/create_team.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/create_team_member.py` & `grafana-backup-1.3.0/grafana_backup/create_team_member.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/create_user.py` & `grafana-backup-1.3.0/grafana_backup/create_user.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/dashboardApi.py` & `grafana-backup-1.3.0/grafana_backup/dashboardApi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import re
 import json
 import requests
 import sys
 from grafana_backup.commons import log_response, to_python2_and_3_compatible_string
+from packaging import version
 
 
 def health_check(grafana_url, http_get_headers, verify_ssl, client_cert, debug):
     url = '{0}/api/health'.format(grafana_url)
     print("\n[Pre-Check] grafana health check: {0}".format(url))
     return send_grafana_get(url, http_get_headers, verify_ssl, client_cert, debug)
 
@@ -168,14 +169,40 @@
 
 
 def delete_annotation(id_, grafana_url, http_get_headers, verify_ssl, client_cert, debug):
     return send_grafana_delete('{0}/api/annotations/{1}'.format(grafana_url, id_), http_get_headers, verify_ssl,
                                client_cert, debug)
 
 
+def search_alert_rules(grafana_url, http_get_headers, verify_ssl, client_cert, debug):
+    url = '{0}/api/v1/provisioning/alert-rules'.format(grafana_url)
+    print("search alert rules in grafana: {0}".format(url))
+    return send_grafana_get(url, http_get_headers, verify_ssl, client_cert, debug)
+
+
+def get_alert_rule(uid, grafana_url, http_get_headers, verify_ssl, client_cert, debug):
+    url = '{0}/api/v1/provisioning/alert-rules/{1}'.format(grafana_url, uid)
+    return send_grafana_get(url, http_get_headers, verify_ssl, client_cert, debug)
+
+
+def create_alert_rule(alert, grafana_url, http_get_headers, verify_ssl, client_cert, debug):
+    url = '{0}/api/v1/provisioning/alert-rules'.format(grafana_url)
+    return send_grafana_post(url, alert, http_get_headers, verify_ssl, client_cert, debug)
+
+
+def delete_alert_rule(uid, grafana_url, http_get_headers, verify_ssl, client_cert, debug):
+    url = '{0}/api/v1/provisioning/alert-rules/{1}'.format(grafana_url, uid)
+    return send_grafana_delete(url, http_get_headers, verify_ssl, client_cert, debug)
+
+
+def update_alert_rule(uid, alert, grafana_url, http_get_headers, verify_ssl, client_cert, debug):
+    url = '{0}/api/v1/provisioning/alert-rules/{1}'.format(grafana_url, uid)
+    return send_grafana_put(url, alert, http_get_headers, verify_ssl, client_cert, debug)
+
+
 def search_alert_channels(grafana_url, http_get_headers, verify_ssl, client_cert, debug):
     url = '{0}/api/alert-notifications'.format(grafana_url)
     print("search alert channels in grafana: {0}".format(url))
     return send_grafana_get(url, http_get_headers, verify_ssl, client_cert, debug)
 
 
 def create_alert_channel(payload, grafana_url, http_post_headers, verify_ssl, client_cert, debug):
@@ -403,14 +430,20 @@
                              debug)
 
 
 def add_user_to_org(org_id, payload, grafana_url, http_post_headers, verify_ssl, client_cert, debug):
     return send_grafana_post('{0}/api/orgs/{1}/users'.format(grafana_url, org_id), payload, http_post_headers, verify_ssl, client_cert,
                              debug)
 
+def get_grafana_version(grafana_url):
+    r = requests.get('{0}/api/health'.format(grafana_url))
+    if r.status_code == 200:
+        return version.parse(r.json()['version'])
+    else:
+        raise Exception("Unable to get version, returned response: {0}".format(r.status_code))
 
 def send_grafana_get(url, http_get_headers, verify_ssl, client_cert, debug):
     r = requests.get(url, headers=http_get_headers, verify=verify_ssl, cert=client_cert)
     if debug:
         log_response(r)
     return (r.status_code, r.json())
```

### Comparing `grafana-backup-1.2.5/grafana_backup/delete.py` & `grafana-backup-1.3.0/grafana_backup/delete.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/delete_alert_channels.py` & `grafana-backup-1.3.0/grafana_backup/delete_alert_channels.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/delete_annotations.py` & `grafana-backup-1.3.0/grafana_backup/delete_annotations.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/delete_dashboards.py` & `grafana-backup-1.3.0/grafana_backup/delete_dashboards.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/delete_datasources.py` & `grafana-backup-1.3.0/grafana_backup/delete_datasources.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/delete_folders.py` & `grafana-backup-1.3.0/grafana_backup/delete_folders.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/delete_library_elements.py` & `grafana-backup-1.3.0/grafana_backup/delete_library_elements.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/delete_snapshots.py` & `grafana-backup-1.3.0/grafana_backup/delete_snapshots.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/delete_team_members.py` & `grafana-backup-1.3.0/grafana_backup/delete_team_members.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/delete_teams.py` & `grafana-backup-1.3.0/grafana_backup/delete_teams.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/gcs_download.py` & `grafana-backup-1.3.0/grafana_backup/gcs_download.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/gcs_upload.py` & `grafana-backup-1.3.0/grafana_backup/gcs_upload.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/grafanaSettings.py` & `grafana-backup-1.3.0/grafana_backup/grafanaSettings.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/influx.py` & `grafana-backup-1.3.0/grafana_backup/influx.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/make_users_viewers.py` & `grafana-backup-1.3.0/grafana_backup/make_users_viewers.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/pause_alerts.py` & `grafana-backup-1.3.0/grafana_backup/pause_alerts.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/restore.py` & `grafana-backup-1.3.0/grafana_backup/restore.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from grafana_backup.create_org import main as create_org
 from grafana_backup.api_checks import main as api_checks
 from grafana_backup.create_folder import main as create_folder
 from grafana_backup.update_folder_permissions import main as update_folder_permissions
 from grafana_backup.create_datasource import main as create_datasource
 from grafana_backup.create_dashboard import main as create_dashboard
 from grafana_backup.create_alert_channel import main as create_alert_channel
+from grafana_backup.create_alert_rule import main as create_alert_rule
 from grafana_backup.create_user import main as create_user
 from grafana_backup.create_snapshot import main as create_snapshot
 from grafana_backup.create_annotation import main as create_annotation
 from grafana_backup.create_team import main as create_team
 from grafana_backup.create_team_member import main as create_team_member
 from grafana_backup.create_library_element import main as create_library_element
 from grafana_backup.s3_download import main as s3_download
@@ -84,14 +85,15 @@
     restore_functions['organization'] = create_org
     restore_functions['user'] = create_user
     restore_functions['snapshot'] = create_snapshot
     restore_functions['annotation'] = create_annotation
     restore_functions['team'] = create_team
     restore_functions['team_member'] = create_team_member
     restore_functions['folder_permission'] = update_folder_permissions
+    restore_functions['alert_rule'] = create_alert_rule
 
     if sys.version_info >= (3,):
         with tempfile.TemporaryDirectory() as tmpdir:
             tar.extractall(tmpdir)
             tar.close()
             restore_components(args, settings, restore_functions, tmpdir)
     else:
```

### Comparing `grafana-backup-1.2.5/grafana_backup/restore_user_permissions.py` & `grafana-backup-1.3.0/grafana_backup/restore_user_permissions.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/s3_download.py` & `grafana-backup-1.3.0/grafana_backup/s3_download.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/s3_upload.py` & `grafana-backup-1.3.0/grafana_backup/s3_upload.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/save.py` & `grafana-backup-1.3.0/grafana_backup/save.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from grafana_backup.api_checks import main as api_checks
+from grafana_backup.save_alert_rules import main as save_alert_rules
 from grafana_backup.save_dashboards import main as save_dashboards
 from grafana_backup.save_datasources import main as save_datasources
 from grafana_backup.save_folders import main as save_folders
 from grafana_backup.save_alert_channels import main as save_alert_channels
 from grafana_backup.save_snapshots import main as save_snapshots
 from grafana_backup.save_versions import main as save_versions
 from grafana_backup.save_annotations import main as save_annotations
@@ -30,15 +31,16 @@
                         'organizations': save_orgs,
                         'users': save_users,
                         'snapshots': save_snapshots,
                         'versions': save_versions,
                         'annotations': save_annotations,
                         'library-elements': save_library_elements,
                         'teams': save_teams,
-                        'team-members': save_team_members}
+                        'team-members': save_team_members,
+                        'save-alert-rules': save_alert_rules}
 
     (status, json_resp, dashboard_uid_support, datasource_uid_support, paging_support) = api_checks(settings)
 
     # Do not continue if API is unavailable or token is not valid
     if not status == 200:
         print("server status is not ok: {0}".format(json_resp))
         sys.exit(1)
```

### Comparing `grafana-backup-1.2.5/grafana_backup/save_alert_channels.py` & `grafana-backup-1.3.0/grafana_backup/save_alert_channels.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/save_annotations.py` & `grafana-backup-1.3.0/grafana_backup/save_annotations.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/save_dashboards.py` & `grafana-backup-1.3.0/grafana_backup/save_dashboards.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/save_datasources.py` & `grafana-backup-1.3.0/grafana_backup/save_datasources.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/save_folders.py` & `grafana-backup-1.3.0/grafana_backup/save_folders.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/save_library_elements.py` & `grafana-backup-1.3.0/grafana_backup/save_library_elements.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/save_orgs.py` & `grafana-backup-1.3.0/grafana_backup/save_orgs.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/save_snapshots.py` & `grafana-backup-1.3.0/grafana_backup/save_snapshots.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/save_team_members.py` & `grafana-backup-1.3.0/grafana_backup/save_team_members.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/save_teams.py` & `grafana-backup-1.3.0/grafana_backup/save_teams.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/save_users.py` & `grafana-backup-1.3.0/grafana_backup/save_users.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/save_versions.py` & `grafana-backup-1.3.0/grafana_backup/save_versions.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/tools.py` & `grafana-backup-1.3.0/grafana_backup/tools.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/unpause_alerts.py` & `grafana-backup-1.3.0/grafana_backup/unpause_alerts.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup/update_folder_permissions.py` & `grafana-backup-1.3.0/grafana_backup/update_folder_permissions.py`

 * *Files identical despite different names*

### Comparing `grafana-backup-1.2.5/grafana_backup.egg-info/PKG-INFO` & `grafana-backup-1.3.0/grafana_backup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grafana-backup
-Version: 1.2.5
+Version: 1.3.0
 Summary: A Python-based application to backup Grafana settings using the Grafana API
 Home-page: https://github.com/ysde/grafana-backup-tool
 Author: author
 Author-email: ysde108@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -22,14 +22,15 @@
 ## Supported components
 * Folder
 * Folder Permissions
 * Library Elements (doesn't work with Grafana 8.0.0 but 8.4.3)
 * Dashboard (contains Alert)
 * Datasource
 * Alert Channel
+* Alert Rules (Supported in version 9.4.0 of grafana and up.)
 * Teams
 * Team Members (Needs Basic Authentication (username and password, see [grafana doc](https://grafana.com/docs/grafana/latest/http_api/org/#admin-organizations-api))
     * You need to set `Admin's account and password` in `grafanaSettings.json`, or set the base64 encoded `admin account and password` in ENV `GRAFANA_BASIC_AUTH`. E.g `export GRAFANA_BASIC_AUTH=YWRtaW46YWRtaW4=`
     * Or Sets this ENV of the Grafana server `GF_USERS_ALLOW_ORG_CREATE=true`. see [grafana doc](https://grafana.com/docs/grafana/latest/http_api/org/#create-organization)
 * Organization (Needs Basic Authentication (username and password, see [grafana doc](https://grafana.com/docs/grafana/latest/http_api/org/#admin-organizations-api))
     * You need to set `Admin's account and password` in `grafanaSettings.json`, or set the base64 encoded `admin account and password` in ENV `GRAFANA_BASIC_AUTH`. E.g `export GRAFANA_BASIC_AUTH=YWRtaW46YWRtaW4=`
     * Or Sets this ENV of the Grafana server `GF_USERS_ALLOW_ORG_CREATE=true`. see [grafana doc](https://grafana.com/docs/grafana/latest/http_api/org/#create-organization)
@@ -178,14 +179,15 @@
 		   -e AZURE_STORAGE_CONTAINER_NAME="azure-storage-container-name" \
 		   -e AZURE_STORAGE_CONNECTION_STRING="azure-storage-connection-string"
 ```
 
 ***GCS Example:*** Set GCS configurations in `-e` or `grafanaSettings.json`([example](https://github.com/ysde/grafana-backup-tool/blob/master/examples/grafana-backup.example.json))
 ```
 		   -e GCS_BUCKET_NAME="bucket-name" \
+		   -e GCLOUD_PROJECT="gcp-project-name" \
 		   -e GOOGLE_APPLICATION_CREDENTIALS="credential-file-path"
 ```
 
 
 ### Restore
 
 ```
```

### Comparing `grafana-backup-1.2.5/grafana_backup.egg-info/SOURCES.txt` & `grafana-backup-1.3.0/grafana_backup.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 grafana_backup/archive.py
 grafana_backup/azure_storage_download.py
 grafana_backup/azure_storage_upload.py
 grafana_backup/cli.py
 grafana_backup/commons.py
 grafana_backup/constants.py
 grafana_backup/create_alert_channel.py
+grafana_backup/create_alert_rule.py
 grafana_backup/create_annotation.py
 grafana_backup/create_dashboard.py
 grafana_backup/create_datasource.py
 grafana_backup/create_folder.py
 grafana_backup/create_library_element.py
 grafana_backup/create_org.py
 grafana_backup/create_snapshot.py
@@ -39,14 +40,15 @@
 grafana_backup/pause_alerts.py
 grafana_backup/restore.py
 grafana_backup/restore_user_permissions.py
 grafana_backup/s3_download.py
 grafana_backup/s3_upload.py
 grafana_backup/save.py
 grafana_backup/save_alert_channels.py
+grafana_backup/save_alert_rules.py
 grafana_backup/save_annotations.py
 grafana_backup/save_dashboards.py
 grafana_backup/save_datasources.py
 grafana_backup/save_folders.py
 grafana_backup/save_library_elements.py
 grafana_backup/save_orgs.py
 grafana_backup/save_snapshots.py
```

### Comparing `grafana-backup-1.2.5/setup.py` & `grafana-backup-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 version = PKG_VERSION
 requires = [
     'requests',
     'docopt',
     'boto3',
     'azure-storage-blob',
     'google-cloud-storage',
-    'influxdb'
+    'influxdb',
+    'packaging'
 ]
 
 setup(
     name=name,
     version=version,
     description='A Python-based application to backup Grafana settings using the Grafana API',
     long_description_content_type='text/markdown',
```

