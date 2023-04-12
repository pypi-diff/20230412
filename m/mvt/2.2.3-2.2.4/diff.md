# Comparing `tmp/mvt-2.2.3.tar.gz` & `tmp/mvt-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mvt-2.2.3.tar", last modified: Wed Mar 29 12:49:21 2023, max compression
+gzip compressed data, was "mvt-2.2.4.tar", last modified: Wed Apr 12 10:58:12 2023, max compression
```

## Comparing `mvt-2.2.3.tar` & `mvt-2.2.4.tar`

### file list

```diff
@@ -1,187 +1,190 @@
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-29 12:49:21.880778 mvt-2.2.3/
--rw-r--r--   0 etienne   (1000) etienne   (1000)    17791 2021-07-26 21:43:37.000000 mvt-2.2.3/LICENSE
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3040 2023-03-29 12:49:21.880778 mvt-2.2.3/PKG-INFO
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2509 2022-06-17 08:45:47.000000 mvt-2.2.3/README.md
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-29 12:49:21.832778 mvt-2.2.3/mvt/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/__init__.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-29 12:49:21.840778 mvt-2.2.3/mvt/android/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      214 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/android/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)    10608 2023-03-01 21:38:00.000000 mvt-2.2.3/mvt/android/cli.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      973 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/android/cmd_check_adb.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1083 2023-02-21 19:16:49.000000 mvt-2.2.3/mvt/android/cmd_check_androidqf.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3798 2023-03-01 21:38:00.000000 mvt-2.2.3/mvt/android/cmd_check_backup.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2589 2023-03-01 21:38:00.000000 mvt-2.2.3/mvt/android/cmd_check_bugreport.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     6078 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/android/cmd_download_apks.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-29 12:49:21.840778 mvt-2.2.3/mvt/android/modules/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/android/modules/__init__.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-29 12:49:21.848778 mvt-2.2.3/mvt/android/modules/adb/
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1271 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/android/modules/adb/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)    12263 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/android/modules/adb/base.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3211 2023-03-24 17:45:57.000000 mvt-2.2.3/mvt/android/modules/adb/chrome_history.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1772 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/android/modules/adb/dumpsys_accessibility.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1755 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/android/modules/adb/dumpsys_activities.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2622 2023-03-24 17:25:12.000000 mvt-2.2.3/mvt/android/modules/adb/dumpsys_appops.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1975 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/android/modules/adb/dumpsys_battery_daily.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1633 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/android/modules/adb/dumpsys_battery_history.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1720 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/android/modules/adb/dumpsys_dbinfo.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1329 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/android/modules/adb/dumpsys_full.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3080 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/android/modules/adb/dumpsys_receivers.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     5130 2023-03-24 17:36:10.000000 mvt-2.2.3/mvt/android/modules/adb/files.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2173 2023-03-29 12:05:03.000000 mvt-2.2.3/mvt/android/modules/adb/getprop.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1905 2023-03-01 21:33:36.000000 mvt-2.2.3/mvt/android/modules/adb/logcat.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)    12138 2023-03-01 21:38:00.000000 mvt-2.2.3/mvt/android/modules/adb/packages.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2685 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/android/modules/adb/processes.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1755 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/android/modules/adb/root_binaries.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1367 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/android/modules/adb/selinux_status.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3543 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/android/modules/adb/settings.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     5745 2023-03-24 14:23:54.000000 mvt-2.2.3/mvt/android/modules/adb/sms.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3474 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/android/modules/adb/whatsapp.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-29 12:49:21.852778 mvt-2.2.3/mvt/android/modules/androidqf/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      739 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/android/modules/androidqf/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1291 2023-03-01 21:38:00.000000 mvt-2.2.3/mvt/android/modules/androidqf/base.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2330 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/android/modules/androidqf/dumpsys_accessibility.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2285 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/android/modules/androidqf/dumpsys_activities.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3045 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/android/modules/androidqf/dumpsys_appops.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3865 2023-03-01 21:38:00.000000 mvt-2.2.3/mvt/android/modules/androidqf/dumpsys_packages.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3567 2023-03-01 21:38:00.000000 mvt-2.2.3/mvt/android/modules/androidqf/dumpsys_receivers.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2687 2023-03-29 12:05:03.000000 mvt-2.2.3/mvt/android/modules/androidqf/getprop.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2918 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/android/modules/androidqf/processes.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2115 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/android/modules/androidqf/settings.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2935 2023-03-01 21:41:19.000000 mvt-2.2.3/mvt/android/modules/androidqf/sms.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-29 12:49:21.856778 mvt-2.2.3/mvt/android/modules/backup/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      238 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/android/modules/backup/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2031 2023-03-01 21:38:00.000000 mvt-2.2.3/mvt/android/modules/backup/base.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1987 2023-03-24 14:23:54.000000 mvt-2.2.3/mvt/android/modules/backup/sms.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-29 12:49:21.860778 mvt-2.2.3/mvt/android/modules/bugreport/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      646 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/android/modules/bugreport/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2396 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/android/modules/bugreport/accessibility.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2362 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/android/modules/bugreport/activities.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3202 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/android/modules/bugreport/appops.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2911 2023-03-01 21:38:00.000000 mvt-2.2.3/mvt/android/modules/bugreport/base.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2687 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/android/modules/bugreport/battery_daily.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2146 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/android/modules/bugreport/battery_history.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2315 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/android/modules/bugreport/dbinfo.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2341 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/android/modules/bugreport/getprop.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     4205 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/android/modules/bugreport/packages.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3772 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/android/modules/bugreport/receivers.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-29 12:49:21.860778 mvt-2.2.3/mvt/android/parsers/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      549 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/android/parsers/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     7568 2023-03-24 14:23:54.000000 mvt-2.2.3/mvt/android/parsers/backup.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)    15778 2023-03-01 21:38:01.000000 mvt-2.2.3/mvt/android/parsers/dumpsys.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      723 2023-03-29 12:05:03.000000 mvt-2.2.3/mvt/android/parsers/getprop.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-29 12:49:21.864778 mvt-2.2.3/mvt/common/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/common/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2425 2023-03-24 17:47:13.000000 mvt-2.2.3/mvt/common/cmd_check_iocs.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     6435 2023-03-15 09:02:05.000000 mvt-2.2.3/mvt/common/command.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      765 2023-02-21 19:16:49.000000 mvt-2.2.3/mvt/common/help.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)    20791 2023-03-29 12:05:03.000000 mvt-2.2.3/mvt/common/indicators.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2132 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/common/logo.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     7861 2023-03-24 18:01:23.000000 mvt-2.2.3/mvt/common/module.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1242 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/common/options.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     7797 2023-03-24 17:57:36.000000 mvt-2.2.3/mvt/common/updates.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     5787 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/common/url.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     5860 2023-03-24 17:57:45.000000 mvt-2.2.3/mvt/common/utils.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      215 2023-03-29 12:34:16.000000 mvt-2.2.3/mvt/common/version.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1365 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/common/virustotal.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-29 12:49:21.868778 mvt-2.2.3/mvt/ios/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      214 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)    10530 2023-03-01 21:38:00.000000 mvt-2.2.3/mvt/ios/cli.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1189 2023-02-21 19:16:49.000000 mvt-2.2.3/mvt/ios/cmd_check_backup.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1170 2023-02-21 19:16:49.000000 mvt-2.2.3/mvt/ios/cmd_check_fs.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     8970 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/decrypt.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-29 12:49:21.868778 mvt-2.2.3/mvt/ios/modules/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/__init__.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-29 12:49:21.868778 mvt-2.2.3/mvt/ios/modules/backup/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      439 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/backup/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2450 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/backup/backup_info.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     6222 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/backup/configuration_profiles.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     6614 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/backup/manifest.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3829 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/backup/profile_events.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     7259 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/base.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-29 12:49:21.872778 mvt-2.2.3/mvt/ios/modules/fs/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      894 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/fs/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     4565 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/fs/analytics.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2669 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/fs/analytics_ios_versions.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2887 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/fs/cache_files.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3016 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/fs/filesystem.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1651 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/fs/net_netusage.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3734 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/fs/safari_favicon.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3735 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/fs/shutdownlog.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2140 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/fs/version_history.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1369 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/fs/webkit_base.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1692 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/fs/webkit_indexeddb.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1702 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/fs/webkit_localstorage.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1425 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/fs/webkit_safariviewservice.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-29 12:49:21.876778 mvt-2.2.3/mvt/ios/modules/mixed/
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1395 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/mixed/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2349 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/mixed/calls.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3354 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/mixed/chrome_favicon.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3185 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/mixed/chrome_history.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2148 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/mixed/contacts.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3215 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/mixed/firefox_favicon.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2906 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/mixed/firefox_history.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     4377 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/mixed/idstatuscache.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     8046 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/mixed/interactionc.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     5163 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/mixed/locationd.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1442 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/mixed/net_datausage.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2869 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/mixed/osanalytics_addaily.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     6075 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/mixed/safari_browserstate.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     5912 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/mixed/safari_history.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     5364 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/mixed/shortcuts.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     5166 2023-03-24 14:23:54.000000 mvt-2.2.3/mvt/ios/modules/mixed/sms.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     4227 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/mixed/sms_attachments.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     6842 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/mixed/tcc.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     4269 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/mixed/webkit_resource_load_statistics.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     6438 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/mixed/webkit_session_resource_log.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     4684 2023-03-24 14:23:54.000000 mvt-2.2.3/mvt/ios/modules/mixed/whatsapp.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)    10455 2023-02-21 19:11:24.000000 mvt-2.2.3/mvt/ios/modules/net_base.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)    14149 2023-03-27 21:10:01.000000 mvt-2.2.3/mvt/ios/versions.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-29 12:49:21.836778 mvt-2.2.3/mvt.egg-info/
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3040 2023-03-29 12:49:21.000000 mvt-2.2.3/mvt.egg-info/PKG-INFO
--rw-r--r--   0 etienne   (1000) etienne   (1000)     5984 2023-03-29 12:49:21.000000 mvt-2.2.3/mvt.egg-info/SOURCES.txt
--rw-r--r--   0 etienne   (1000) etienne   (1000)        1 2023-03-29 12:49:21.000000 mvt-2.2.3/mvt.egg-info/dependency_links.txt
--rw-r--r--   0 etienne   (1000) etienne   (1000)       70 2023-03-29 12:49:21.000000 mvt-2.2.3/mvt.egg-info/entry_points.txt
--rw-r--r--   0 etienne   (1000) etienne   (1000)      189 2023-03-29 12:49:21.000000 mvt-2.2.3/mvt.egg-info/requires.txt
--rw-r--r--   0 etienne   (1000) etienne   (1000)       10 2023-03-29 12:49:21.000000 mvt-2.2.3/mvt.egg-info/top_level.txt
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1638 2023-03-29 12:49:21.880778 mvt-2.2.3/setup.cfg
--rwxr-xr-x   0 etienne   (1000) etienne   (1000)      231 2023-02-21 19:11:24.000000 mvt-2.2.3/setup.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-29 12:49:21.876778 mvt-2.2.3/tests/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:24.000000 mvt-2.2.3/tests/__init__.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-29 12:49:21.876778 mvt-2.2.3/tests/android/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:24.000000 mvt-2.2.3/tests/android/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2720 2023-02-21 19:11:24.000000 mvt-2.2.3/tests/android/test_backup_module.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2061 2023-02-21 19:11:24.000000 mvt-2.2.3/tests/android/test_backup_parser.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1585 2023-02-21 19:11:24.000000 mvt-2.2.3/tests/android/test_bugreport.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2372 2023-02-21 19:11:24.000000 mvt-2.2.3/tests/android/test_dumpsys_parser.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-29 12:49:21.880778 mvt-2.2.3/tests/android_androidqf/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:24.000000 mvt-2.2.3/tests/android_androidqf/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      629 2023-03-01 21:41:05.000000 mvt-2.2.3/tests/android_androidqf/test_dumpsysaccessbility.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      633 2023-03-01 21:39:38.000000 mvt-2.2.3/tests/android_androidqf/test_dumpsysappops.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1353 2023-03-29 10:50:24.000000 mvt-2.2.3/tests/android_androidqf/test_dumpsyspackages.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      607 2023-03-01 21:41:53.000000 mvt-2.2.3/tests/android_androidqf/test_dumpsysreceivers.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1342 2023-03-29 12:05:03.000000 mvt-2.2.3/tests/android_androidqf/test_getprop.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      670 2023-02-21 19:11:25.000000 mvt-2.2.3/tests/android_androidqf/test_processes.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      618 2023-03-01 21:40:12.000000 mvt-2.2.3/tests/android_androidqf/test_settings.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      639 2023-02-21 19:11:25.000000 mvt-2.2.3/tests/android_androidqf/test_sms.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-29 12:49:21.880778 mvt-2.2.3/tests/common/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:25.000000 mvt-2.2.3/tests/common/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1638 2023-03-29 12:05:03.000000 mvt-2.2.3/tests/common/test_indicators.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2290 2023-03-01 21:38:00.000000 mvt-2.2.3/tests/common/test_utils.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      725 2023-02-21 19:11:25.000000 mvt-2.2.3/tests/conftest.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-29 12:49:21.880778 mvt-2.2.3/tests/ios_backup/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:25.000000 mvt-2.2.3/tests/ios_backup/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      571 2023-02-21 19:11:25.000000 mvt-2.2.3/tests/ios_backup/test_backup_info.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1125 2023-02-21 19:11:25.000000 mvt-2.2.3/tests/ios_backup/test_datausage.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1008 2023-02-21 19:11:25.000000 mvt-2.2.3/tests/ios_backup/test_manifest.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1258 2023-02-21 19:11:25.000000 mvt-2.2.3/tests/ios_backup/test_safari_browserstate.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1010 2023-02-21 19:11:25.000000 mvt-2.2.3/tests/ios_backup/test_sms.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1266 2023-02-21 19:11:25.000000 mvt-2.2.3/tests/ios_backup/test_tcc.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      688 2023-03-01 21:42:08.000000 mvt-2.2.3/tests/ios_backup/test_webkit_resource_load_statistics.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-29 12:49:21.880778 mvt-2.2.3/tests/ios_fs/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:25.000000 mvt-2.2.3/tests/ios_fs/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1139 2023-02-21 19:11:25.000000 mvt-2.2.3/tests/ios_fs/test_filesystem.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      573 2023-02-21 19:11:25.000000 mvt-2.2.3/tests/test_check_android_androidqf.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      587 2023-02-21 19:11:25.000000 mvt-2.2.3/tests/test_check_android_bugreport.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      526 2023-02-21 19:11:25.000000 mvt-2.2.3/tests/test_check_ios_backup.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      484 2023-02-21 19:11:25.000000 mvt-2.2.3/tests/test_ios_versions.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      928 2023-02-21 19:11:25.000000 mvt-2.2.3/tests/utils.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-12 10:58:12.588795 mvt-2.2.4/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)    17791 2021-07-26 21:43:37.000000 mvt-2.2.4/LICENSE
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3040 2023-04-12 10:58:12.588795 mvt-2.2.4/PKG-INFO
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2509 2022-06-17 08:45:47.000000 mvt-2.2.4/README.md
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-12 10:58:12.564795 mvt-2.2.4/mvt/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/__init__.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-12 10:58:12.568795 mvt-2.2.4/mvt/android/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      214 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/android/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)    10608 2023-03-01 21:38:00.000000 mvt-2.2.4/mvt/android/cli.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      973 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/android/cmd_check_adb.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1083 2023-02-21 19:16:49.000000 mvt-2.2.4/mvt/android/cmd_check_androidqf.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3798 2023-04-07 13:03:23.000000 mvt-2.2.4/mvt/android/cmd_check_backup.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2589 2023-03-01 21:38:00.000000 mvt-2.2.4/mvt/android/cmd_check_bugreport.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     6078 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/android/cmd_download_apks.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-12 10:58:12.568795 mvt-2.2.4/mvt/android/modules/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/android/modules/__init__.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-12 10:58:12.568795 mvt-2.2.4/mvt/android/modules/adb/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1271 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/android/modules/adb/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)    12263 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/android/modules/adb/base.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3211 2023-03-24 17:45:57.000000 mvt-2.2.4/mvt/android/modules/adb/chrome_history.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1772 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/android/modules/adb/dumpsys_accessibility.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1755 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/android/modules/adb/dumpsys_activities.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2622 2023-03-24 17:25:12.000000 mvt-2.2.4/mvt/android/modules/adb/dumpsys_appops.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1975 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/android/modules/adb/dumpsys_battery_daily.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1633 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/android/modules/adb/dumpsys_battery_history.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1720 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/android/modules/adb/dumpsys_dbinfo.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1329 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/android/modules/adb/dumpsys_full.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3080 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/android/modules/adb/dumpsys_receivers.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     5130 2023-03-24 17:36:10.000000 mvt-2.2.4/mvt/android/modules/adb/files.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2173 2023-03-29 12:05:03.000000 mvt-2.2.4/mvt/android/modules/adb/getprop.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1905 2023-03-01 21:33:36.000000 mvt-2.2.4/mvt/android/modules/adb/logcat.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)    12138 2023-03-01 21:38:00.000000 mvt-2.2.4/mvt/android/modules/adb/packages.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2685 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/android/modules/adb/processes.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1755 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/android/modules/adb/root_binaries.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1367 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/android/modules/adb/selinux_status.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3543 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/android/modules/adb/settings.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     5656 2023-04-12 10:39:42.000000 mvt-2.2.4/mvt/android/modules/adb/sms.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3474 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/android/modules/adb/whatsapp.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-12 10:58:12.572795 mvt-2.2.4/mvt/android/modules/androidqf/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      739 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/android/modules/androidqf/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1291 2023-03-01 21:38:00.000000 mvt-2.2.4/mvt/android/modules/androidqf/base.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2330 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/android/modules/androidqf/dumpsys_accessibility.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2285 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/android/modules/androidqf/dumpsys_activities.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3045 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/android/modules/androidqf/dumpsys_appops.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3865 2023-03-01 21:38:00.000000 mvt-2.2.4/mvt/android/modules/androidqf/dumpsys_packages.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3567 2023-03-01 21:38:00.000000 mvt-2.2.4/mvt/android/modules/androidqf/dumpsys_receivers.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2687 2023-03-29 12:05:03.000000 mvt-2.2.4/mvt/android/modules/androidqf/getprop.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2918 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/android/modules/androidqf/processes.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2115 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/android/modules/androidqf/settings.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2935 2023-03-01 21:41:19.000000 mvt-2.2.4/mvt/android/modules/androidqf/sms.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-12 10:58:12.572795 mvt-2.2.4/mvt/android/modules/backup/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      238 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/android/modules/backup/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2031 2023-03-01 21:38:00.000000 mvt-2.2.4/mvt/android/modules/backup/base.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2175 2023-04-12 10:39:42.000000 mvt-2.2.4/mvt/android/modules/backup/sms.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-12 10:58:12.572795 mvt-2.2.4/mvt/android/modules/bugreport/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      646 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/android/modules/bugreport/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2396 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/android/modules/bugreport/accessibility.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2362 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/android/modules/bugreport/activities.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3202 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/android/modules/bugreport/appops.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2911 2023-03-01 21:38:00.000000 mvt-2.2.4/mvt/android/modules/bugreport/base.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2687 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/android/modules/bugreport/battery_daily.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2146 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/android/modules/bugreport/battery_history.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2315 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/android/modules/bugreport/dbinfo.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2341 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/android/modules/bugreport/getprop.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     4205 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/android/modules/bugreport/packages.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3772 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/android/modules/bugreport/receivers.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-12 10:58:12.572795 mvt-2.2.4/mvt/android/parsers/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      549 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/android/parsers/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     7503 2023-04-12 10:39:42.000000 mvt-2.2.4/mvt/android/parsers/backup.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)    15778 2023-03-01 21:38:01.000000 mvt-2.2.4/mvt/android/parsers/dumpsys.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      723 2023-03-29 12:05:03.000000 mvt-2.2.4/mvt/android/parsers/getprop.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-12 10:58:12.576795 mvt-2.2.4/mvt/common/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/common/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2425 2023-03-24 17:47:13.000000 mvt-2.2.4/mvt/common/cmd_check_iocs.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     6435 2023-03-15 09:02:05.000000 mvt-2.2.4/mvt/common/command.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      765 2023-02-21 19:16:49.000000 mvt-2.2.4/mvt/common/help.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)    20857 2023-04-07 13:06:52.000000 mvt-2.2.4/mvt/common/indicators.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2132 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/common/logo.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     8046 2023-04-07 10:26:00.000000 mvt-2.2.4/mvt/common/module.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1242 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/common/options.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     7797 2023-03-24 17:57:36.000000 mvt-2.2.4/mvt/common/updates.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     5787 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/common/url.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     5919 2023-04-07 12:48:42.000000 mvt-2.2.4/mvt/common/utils.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      215 2023-04-12 10:52:41.000000 mvt-2.2.4/mvt/common/version.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1365 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/common/virustotal.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-12 10:58:12.576795 mvt-2.2.4/mvt/ios/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      214 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/ios/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)    10530 2023-03-01 21:38:00.000000 mvt-2.2.4/mvt/ios/cli.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1189 2023-02-21 19:16:49.000000 mvt-2.2.4/mvt/ios/cmd_check_backup.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1170 2023-02-21 19:16:49.000000 mvt-2.2.4/mvt/ios/cmd_check_fs.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     8970 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/ios/decrypt.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-12 10:58:12.576795 mvt-2.2.4/mvt/ios/modules/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/ios/modules/__init__.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-12 10:58:12.576795 mvt-2.2.4/mvt/ios/modules/backup/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      439 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/ios/modules/backup/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2450 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/ios/modules/backup/backup_info.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     6222 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/ios/modules/backup/configuration_profiles.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     6614 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/ios/modules/backup/manifest.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3829 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/ios/modules/backup/profile_events.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     7223 2023-04-07 10:26:00.000000 mvt-2.2.4/mvt/ios/modules/base.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-12 10:58:12.580795 mvt-2.2.4/mvt/ios/modules/fs/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      894 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/ios/modules/fs/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     4691 2023-04-12 08:16:00.000000 mvt-2.2.4/mvt/ios/modules/fs/analytics.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2669 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/ios/modules/fs/analytics_ios_versions.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2887 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/ios/modules/fs/cache_files.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3014 2023-04-11 19:15:22.000000 mvt-2.2.4/mvt/ios/modules/fs/filesystem.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1651 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/ios/modules/fs/net_netusage.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3734 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/ios/modules/fs/safari_favicon.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3735 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/ios/modules/fs/shutdownlog.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2140 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/ios/modules/fs/version_history.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1369 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/ios/modules/fs/webkit_base.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1692 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/ios/modules/fs/webkit_indexeddb.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1702 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/ios/modules/fs/webkit_localstorage.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1425 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/ios/modules/fs/webkit_safariviewservice.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-12 10:58:12.584795 mvt-2.2.4/mvt/ios/modules/mixed/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1506 2023-04-11 18:44:24.000000 mvt-2.2.4/mvt/ios/modules/mixed/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     4947 2023-04-12 08:16:00.000000 mvt-2.2.4/mvt/ios/modules/mixed/applications.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     5052 2023-04-11 19:21:34.000000 mvt-2.2.4/mvt/ios/modules/mixed/calendar.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2349 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/ios/modules/mixed/calls.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3354 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/ios/modules/mixed/chrome_favicon.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3185 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/ios/modules/mixed/chrome_history.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2148 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/ios/modules/mixed/contacts.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3215 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/ios/modules/mixed/firefox_favicon.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2906 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/ios/modules/mixed/firefox_history.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     4377 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/ios/modules/mixed/idstatuscache.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)    14449 2023-04-07 10:26:00.000000 mvt-2.2.4/mvt/ios/modules/mixed/interactionc.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     5163 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/ios/modules/mixed/locationd.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1442 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/ios/modules/mixed/net_datausage.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2869 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/ios/modules/mixed/osanalytics_addaily.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     6075 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/ios/modules/mixed/safari_browserstate.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     5912 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/ios/modules/mixed/safari_history.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     5364 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/ios/modules/mixed/shortcuts.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     5094 2023-04-12 10:39:42.000000 mvt-2.2.4/mvt/ios/modules/mixed/sms.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     4227 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/ios/modules/mixed/sms_attachments.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     6842 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/ios/modules/mixed/tcc.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     4525 2023-04-07 12:42:40.000000 mvt-2.2.4/mvt/ios/modules/mixed/webkit_resource_load_statistics.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     6438 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/ios/modules/mixed/webkit_session_resource_log.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     4593 2023-04-12 10:39:42.000000 mvt-2.2.4/mvt/ios/modules/mixed/whatsapp.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)    10455 2023-02-21 19:11:24.000000 mvt-2.2.4/mvt/ios/modules/net_base.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)    14195 2023-04-07 20:22:15.000000 mvt-2.2.4/mvt/ios/versions.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-12 10:58:12.564795 mvt-2.2.4/mvt.egg-info/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3040 2023-04-12 10:58:11.000000 mvt-2.2.4/mvt.egg-info/PKG-INFO
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     6096 2023-04-12 10:58:12.000000 mvt-2.2.4/mvt.egg-info/SOURCES.txt
+-rw-r--r--   0 etienne   (1000) etienne   (1000)        1 2023-04-12 10:58:11.000000 mvt-2.2.4/mvt.egg-info/dependency_links.txt
+-rw-r--r--   0 etienne   (1000) etienne   (1000)       70 2023-04-12 10:58:11.000000 mvt-2.2.4/mvt.egg-info/entry_points.txt
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      189 2023-04-12 10:58:11.000000 mvt-2.2.4/mvt.egg-info/requires.txt
+-rw-r--r--   0 etienne   (1000) etienne   (1000)       10 2023-04-12 10:58:11.000000 mvt-2.2.4/mvt.egg-info/top_level.txt
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1638 2023-04-12 10:58:12.588795 mvt-2.2.4/setup.cfg
+-rwxr-xr-x   0 etienne   (1000) etienne   (1000)      231 2023-02-21 19:11:24.000000 mvt-2.2.4/setup.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-12 10:58:12.584795 mvt-2.2.4/tests/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:24.000000 mvt-2.2.4/tests/__init__.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-12 10:58:12.584795 mvt-2.2.4/tests/android/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:24.000000 mvt-2.2.4/tests/android/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2720 2023-02-21 19:11:24.000000 mvt-2.2.4/tests/android/test_backup_module.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2061 2023-02-21 19:11:24.000000 mvt-2.2.4/tests/android/test_backup_parser.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1585 2023-02-21 19:11:24.000000 mvt-2.2.4/tests/android/test_bugreport.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2372 2023-02-21 19:11:24.000000 mvt-2.2.4/tests/android/test_dumpsys_parser.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-12 10:58:12.584795 mvt-2.2.4/tests/android_androidqf/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:24.000000 mvt-2.2.4/tests/android_androidqf/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      629 2023-03-01 21:41:05.000000 mvt-2.2.4/tests/android_androidqf/test_dumpsysaccessbility.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      633 2023-03-01 21:39:38.000000 mvt-2.2.4/tests/android_androidqf/test_dumpsysappops.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1353 2023-03-29 10:50:24.000000 mvt-2.2.4/tests/android_androidqf/test_dumpsyspackages.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      607 2023-03-01 21:41:53.000000 mvt-2.2.4/tests/android_androidqf/test_dumpsysreceivers.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1342 2023-03-29 12:05:03.000000 mvt-2.2.4/tests/android_androidqf/test_getprop.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      670 2023-02-21 19:11:25.000000 mvt-2.2.4/tests/android_androidqf/test_processes.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      618 2023-03-01 21:40:12.000000 mvt-2.2.4/tests/android_androidqf/test_settings.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      639 2023-02-21 19:11:25.000000 mvt-2.2.4/tests/android_androidqf/test_sms.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-12 10:58:12.584795 mvt-2.2.4/tests/common/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:25.000000 mvt-2.2.4/tests/common/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1744 2023-04-07 12:35:45.000000 mvt-2.2.4/tests/common/test_indicators.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2290 2023-03-01 21:38:00.000000 mvt-2.2.4/tests/common/test_utils.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      725 2023-02-21 19:11:25.000000 mvt-2.2.4/tests/conftest.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-12 10:58:12.588795 mvt-2.2.4/tests/ios_backup/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:25.000000 mvt-2.2.4/tests/ios_backup/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      571 2023-02-21 19:11:25.000000 mvt-2.2.4/tests/ios_backup/test_backup_info.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1133 2023-04-11 19:12:42.000000 mvt-2.2.4/tests/ios_backup/test_calendar.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1125 2023-02-21 19:11:25.000000 mvt-2.2.4/tests/ios_backup/test_datausage.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1008 2023-02-21 19:11:25.000000 mvt-2.2.4/tests/ios_backup/test_manifest.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1258 2023-02-21 19:11:25.000000 mvt-2.2.4/tests/ios_backup/test_safari_browserstate.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1010 2023-02-21 19:11:25.000000 mvt-2.2.4/tests/ios_backup/test_sms.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1266 2023-02-21 19:11:25.000000 mvt-2.2.4/tests/ios_backup/test_tcc.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      688 2023-03-01 21:42:08.000000 mvt-2.2.4/tests/ios_backup/test_webkit_resource_load_statistics.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-12 10:58:12.588795 mvt-2.2.4/tests/ios_fs/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:25.000000 mvt-2.2.4/tests/ios_fs/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1139 2023-04-11 19:15:26.000000 mvt-2.2.4/tests/ios_fs/test_filesystem.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      573 2023-02-21 19:11:25.000000 mvt-2.2.4/tests/test_check_android_androidqf.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      587 2023-02-21 19:11:25.000000 mvt-2.2.4/tests/test_check_android_bugreport.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      526 2023-02-21 19:11:25.000000 mvt-2.2.4/tests/test_check_ios_backup.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      484 2023-02-21 19:11:25.000000 mvt-2.2.4/tests/test_ios_versions.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      928 2023-02-21 19:11:25.000000 mvt-2.2.4/tests/utils.py
```

### Comparing `mvt-2.2.3/LICENSE` & `mvt-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/PKG-INFO` & `mvt-2.2.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvt
-Version: 2.2.3
+Version: 2.2.4
 Summary: Mobile Verification Toolkit
 Home-page: https://github.com/mvt-project/mvt
 Author: Claudio Guarnieri
 Author-email: nex@nex.sx
 License: MVT v1.1
 Keywords: security,mobile,forensics,malware
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mvt-2.2.3/README.md` & `mvt-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/cli.py` & `mvt-2.2.4/mvt/android/cli.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/cmd_check_adb.py` & `mvt-2.2.4/mvt/android/cmd_check_adb.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/cmd_check_androidqf.py` & `mvt-2.2.4/mvt/android/cmd_check_androidqf.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/cmd_check_backup.py` & `mvt-2.2.4/mvt/android/cmd_check_backup.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/cmd_check_bugreport.py` & `mvt-2.2.4/mvt/android/cmd_check_bugreport.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/cmd_download_apks.py` & `mvt-2.2.4/mvt/android/cmd_download_apks.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/adb/__init__.py` & `mvt-2.2.4/mvt/android/modules/adb/__init__.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/adb/base.py` & `mvt-2.2.4/mvt/android/modules/adb/base.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/adb/chrome_history.py` & `mvt-2.2.4/mvt/android/modules/adb/chrome_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/adb/dumpsys_accessibility.py` & `mvt-2.2.4/mvt/android/modules/adb/dumpsys_accessibility.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/adb/dumpsys_activities.py` & `mvt-2.2.4/mvt/android/modules/adb/dumpsys_activities.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/adb/dumpsys_appops.py` & `mvt-2.2.4/mvt/android/modules/adb/dumpsys_appops.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/adb/dumpsys_battery_daily.py` & `mvt-2.2.4/mvt/android/modules/adb/dumpsys_battery_daily.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/adb/dumpsys_battery_history.py` & `mvt-2.2.4/mvt/android/modules/adb/dumpsys_battery_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/adb/dumpsys_dbinfo.py` & `mvt-2.2.4/mvt/android/modules/adb/dumpsys_dbinfo.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/adb/dumpsys_full.py` & `mvt-2.2.4/mvt/android/modules/adb/dumpsys_full.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/adb/dumpsys_receivers.py` & `mvt-2.2.4/mvt/android/modules/adb/dumpsys_receivers.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/adb/files.py` & `mvt-2.2.4/mvt/android/modules/adb/files.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/adb/getprop.py` & `mvt-2.2.4/mvt/android/modules/adb/getprop.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/adb/logcat.py` & `mvt-2.2.4/mvt/android/modules/adb/logcat.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/adb/packages.py` & `mvt-2.2.4/mvt/android/modules/adb/packages.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/adb/processes.py` & `mvt-2.2.4/mvt/android/modules/adb/processes.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/adb/root_binaries.py` & `mvt-2.2.4/mvt/android/modules/adb/root_binaries.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/adb/selinux_status.py` & `mvt-2.2.4/mvt/android/modules/adb/selinux_status.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/adb/settings.py` & `mvt-2.2.4/mvt/android/modules/adb/settings.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/adb/sms.py` & `mvt-2.2.4/mvt/android/modules/adb/sms.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     type as incoming,
     body AS body
 FROM sms;
 """
 
 
 class SMS(AndroidExtraction):
-    """This module extracts all SMS messages containing links."""
+    """This module extracts all SMS messages."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
         fast_mode: Optional[bool] = False,
@@ -73,16 +73,18 @@
         if not self.indicators:
             return
 
         for message in self.results:
             if "body" not in message:
                 continue
 
-            # TODO: check links exported from the body previously.
-            message_links = check_for_links(message["body"])
+            message_links = message.get("links", [])
+            if message_links == []:
+                message_links = check_for_links(message["body"])
+
             if self.indicators.check_domains(message_links):
                 self.detected.append(message)
 
     def _parse_db(self, db_path: str) -> None:
         """Parse an Android bugle_db SMS database file.
 
         :param db_path: Path to the Android SMS database file to process
@@ -102,23 +104,24 @@
             message = {}
             for index, value in enumerate(item):
                 message[names[index]] = value
 
             message["direction"] = ("received" if message["incoming"] == 1 else "sent")
             message["isodate"] = convert_unix_to_iso(message["timestamp"])
 
-            # If we find links in the messages or if they are empty we add
-            # them to the list of results.
-            if check_for_links(message["body"]) or message["body"].strip() == "":
-                self.results.append(message)
+            # Extract links in the message body
+            links = check_for_links(message["body"])
+            message["links"] = links
+
+            self.results.append(message)
 
         cur.close()
         conn.close()
 
-        self.log.info("Extracted a total of %d SMS messages containing links",
+        self.log.info("Extracted a total of %d SMS messages",
                       len(self.results))
 
     def _extract_sms_adb(self) -> None:
         """Use the Android backup command to extract SMS data from the native
         SMS app.
 
         It is crucial to use the under-documented "-nocompress" flag to disable
@@ -133,15 +136,15 @@
             self.results = parse_tar_for_sms(backup_tar)
         except AndroidBackupParsingError:
             self.log.info("Impossible to read SMS from the Android Backup, "
                           "please extract the SMS and try extracting it with "
                           "Android Backup Extractor")
             return
 
-        self.log.info("Extracted a total of %d SMS messages containing links",
+        self.log.info("Extracted a total of %d SMS messages",
                       len(self.results))
 
     def run(self) -> None:
         self._adb_connect()
 
         try:
             if self._adb_check_file_exists(os.path.join("/", SMS_BUGLE_PATH)):
```

### Comparing `mvt-2.2.3/mvt/android/modules/adb/whatsapp.py` & `mvt-2.2.4/mvt/android/modules/adb/whatsapp.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/androidqf/__init__.py` & `mvt-2.2.4/mvt/android/modules/androidqf/__init__.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/androidqf/base.py` & `mvt-2.2.4/mvt/android/modules/androidqf/base.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/androidqf/dumpsys_accessibility.py` & `mvt-2.2.4/mvt/android/modules/androidqf/dumpsys_accessibility.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/androidqf/dumpsys_activities.py` & `mvt-2.2.4/mvt/android/modules/androidqf/dumpsys_activities.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/androidqf/dumpsys_appops.py` & `mvt-2.2.4/mvt/android/modules/androidqf/dumpsys_appops.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/androidqf/dumpsys_packages.py` & `mvt-2.2.4/mvt/android/modules/androidqf/dumpsys_packages.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/androidqf/dumpsys_receivers.py` & `mvt-2.2.4/mvt/android/modules/androidqf/dumpsys_receivers.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/androidqf/getprop.py` & `mvt-2.2.4/mvt/android/modules/androidqf/getprop.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/androidqf/processes.py` & `mvt-2.2.4/mvt/android/modules/androidqf/processes.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/androidqf/settings.py` & `mvt-2.2.4/mvt/android/modules/androidqf/settings.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/androidqf/sms.py` & `mvt-2.2.4/mvt/android/modules/androidqf/sms.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/backup/base.py` & `mvt-2.2.4/mvt/android/modules/backup/base.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/backup/sms.py` & `mvt-2.2.4/mvt/android/modules/backup/sms.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 #   https://license.mvt.re/1.1/
 
 import logging
 from typing import Optional
 
 from mvt.android.modules.backup.base import BackupExtraction
 from mvt.android.parsers.backup import parse_sms_file
+from mvt.common.utils import check_for_links
 
 
 class SMS(BackupExtraction):
 
     def __init__(
         self,
         file_path: Optional[str] = None,
@@ -30,15 +31,19 @@
         if not self.indicators:
             return
 
         for message in self.results:
             if "body" not in message:
                 continue
 
-            if self.indicators.check_domains(message["links"]):
+            message_links = message.get("links", [])
+            if message_links == []:
+                message_links = check_for_links(message.get("text", ""))
+
+            if self.indicators.check_domains(message_links):
                 self.detected.append(message)
 
     def run(self) -> None:
         sms_path = "apps/com.android.providers.telephony/d_f/*_sms_backup"
         for file in self._get_files_by_pattern(sms_path):
             self.log.info("Processing SMS backup file at %s", file)
             data = self._get_file_content(file)
@@ -46,9 +51,9 @@
 
         mms_path = "apps/com.android.providers.telephony/d_f/*_mms_backup"
         for file in self._get_files_by_pattern(mms_path):
             self.log.info("Processing MMS backup file at %s", file)
             data = self._get_file_content(file)
             self.results.extend(parse_sms_file(data))
 
-        self.log.info("Extracted a total of %d SMS & MMS messages containing links",
+        self.log.info("Extracted a total of %d SMS & MMS messages",
                       len(self.results))
```

### Comparing `mvt-2.2.3/mvt/android/modules/bugreport/__init__.py` & `mvt-2.2.4/mvt/android/modules/bugreport/__init__.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/bugreport/accessibility.py` & `mvt-2.2.4/mvt/android/modules/bugreport/accessibility.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/bugreport/activities.py` & `mvt-2.2.4/mvt/android/modules/bugreport/activities.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/bugreport/appops.py` & `mvt-2.2.4/mvt/android/modules/bugreport/appops.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/bugreport/base.py` & `mvt-2.2.4/mvt/android/modules/bugreport/base.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/bugreport/battery_daily.py` & `mvt-2.2.4/mvt/android/modules/bugreport/battery_daily.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/bugreport/battery_history.py` & `mvt-2.2.4/mvt/android/modules/bugreport/battery_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/bugreport/dbinfo.py` & `mvt-2.2.4/mvt/android/modules/bugreport/dbinfo.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/bugreport/getprop.py` & `mvt-2.2.4/mvt/android/modules/bugreport/getprop.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/bugreport/packages.py` & `mvt-2.2.4/mvt/android/modules/bugreport/packages.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/modules/bugreport/receivers.py` & `mvt-2.2.4/mvt/android/modules/bugreport/receivers.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/parsers/__init__.py` & `mvt-2.2.4/mvt/android/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/parsers/backup.py` & `mvt-2.2.4/mvt/android/parsers/backup.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,14 +214,13 @@
             entry.pop("mms_body")
 
         message_links = check_for_links(entry["body"])
 
         entry["isodate"] = convert_unix_to_iso(int(entry["date"]) / 1000)
         entry["direction"] = ("sent" if int(entry["date_sent"]) else "received")
 
-        # If we find links in the messages or if they are empty we add them to
-        # the list.
+        # Extract links from the body
         if message_links or entry["body"].strip() == "":
             entry["links"] = message_links
-            res.append(entry)
+        res.append(entry)
 
     return res
```

### Comparing `mvt-2.2.3/mvt/android/parsers/dumpsys.py` & `mvt-2.2.4/mvt/android/parsers/dumpsys.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/android/parsers/getprop.py` & `mvt-2.2.4/mvt/android/parsers/getprop.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/common/cmd_check_iocs.py` & `mvt-2.2.4/mvt/common/cmd_check_iocs.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/common/command.py` & `mvt-2.2.4/mvt/common/command.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/common/help.py` & `mvt-2.2.4/mvt/common/help.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/common/indicators.py` & `mvt-2.2.4/mvt/common/indicators.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,21 +11,23 @@
 from appdirs import user_data_dir
 
 from .url import URL
 
 MVT_DATA_FOLDER = user_data_dir("mvt")
 MVT_INDICATORS_FOLDER = os.path.join(MVT_DATA_FOLDER, "indicators")
 
+logger = logging.getLogger(__name__)
+
 
 class Indicators:
     """This class is used to parse indicators from a STIX2 file and provide
     functions to compare extracted artifacts to the indicators.
     """
 
-    def __init__(self, log=logging.Logger) -> None:
+    def __init__(self, log=logger) -> None:
         self.log = log
         self.ioc_collections: List[Dict[str, Any]] = []
         self.total_ioc_count = 0
 
     def _load_downloaded_indicators(self) -> None:
         if not os.path.isdir(MVT_INDICATORS_FOLDER):
             return
@@ -211,15 +213,15 @@
         if load_default:
             self._load_downloaded_indicators()
 
         self._check_stix2_env_variable()
         self.log.info("Loaded a total of %d unique indicators",
                       self.total_ioc_count)
 
-    def get_iocs(self, ioc_type: str) -> Union[Iterator[Dict[str, Any]], None]:
+    def get_iocs(self, ioc_type: str) -> Iterator[Dict[str, Any]]:
         for ioc_collection in self.ioc_collections:
             for ioc in ioc_collection.get(ioc_type, []):
                 yield {
                     "value": ioc,
                     "type": ioc_type,
                     "name": ioc_collection["name"],
                     "stix2_file_name": ioc_collection["stix2_file_name"],
@@ -229,37 +231,39 @@
         """Check if a given URL matches any of the provided domain indicators.
 
         :param url: URL to match against domain indicators
         :type url: str
         :returns: Indicator details if matched, otherwise None
 
         """
-        # TODO: If the IOC domain contains a subdomain, it is not currently
-        #       being matched.
         if not url:
             return None
+        if not isinstance(url, str):
+            return None
 
         try:
             # First we use the provided URL.
             orig_url = URL(url)
 
             if orig_url.check_if_shortened():
                 # If it is, we try to retrieve the actual URL making an
                 # HTTP HEAD request.
                 unshortened = orig_url.unshorten()
 
-                # self.log.info("Found a shortened URL %s -> %s",
-                #               url, unshortened)
+                self.log.debug("Found a shortened URL %s -> %s",
+                               url, unshortened)
+                if unshortened is None:
+                    return None
 
                 # Now we check for any nested URL shorteners.
                 dest_url = URL(unshortened)
                 if dest_url.check_if_shortened():
-                    # self.log.info("Original URL %s appears to shorten another "
-                    #               "shortened URL %s ... checking!",
-                    #               orig_url.url, dest_url.url)
+                    self.log.debug("Original URL %s appears to shorten another "
+                                   "shortened URL %s ... checking!",
+                                   orig_url.url, dest_url.url)
                     return self.check_domain(dest_url.url)
 
                 final_url = dest_url
             else:
                 # If it's not shortened, we just use the original URL object.
                 final_url = orig_url
         except Exception:
@@ -438,15 +442,15 @@
                 self.log.warning("Found a known suspicious file path \"%s\" "
                                  "matching indicators form \"%s\"",
                                  file_path, ioc["name"])
                 return ioc
 
         return None
 
-    def check_file_path_process(self, file_path: str) -> Union[dict, None]:
+    def check_file_path_process(self, file_path: str) -> Optional[Dict[str, Any]]:
         """Check the provided file path contains a process name from the
         list of indicators
 
         :param file_path: File path or file name to check against file
         indicators
         :type file_path: str
         :returns: Indicator details if matched, otherwise None
@@ -459,14 +463,16 @@
             parts = file_path.split("/")
             if ioc["value"] in parts:
                 self.log.warning("Found known suspicious process name mentioned in file at "
                                   "path \"%s\" matching indicators from \"%s\"",
                                   file_path, ioc["name"])
                 return ioc
 
+        return None
+
     def check_profile(self, profile_uuid: str) -> Union[dict, None]:
         """Check the provided configuration profile UUID against the list of
         indicators.
 
         :param profile_uuid: Profile UUID to check against configuration profile
                              indicators
         :type profile_uuid: str
```

### Comparing `mvt-2.2.3/mvt/common/logo.py` & `mvt-2.2.4/mvt/common/logo.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/common/module.py` & `mvt-2.2.4/mvt/common/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,14 +181,18 @@
                              module.__class__.__name__, exc)
     else:
         try:
             module.check_indicators()
         except NotImplementedError:
             module.log.info("The %s module does not support checking for indicators",
                             module.__class__.__name__)
+        except Exception as exc:
+            module.log.exception("Error when checking indicators from module %s: %s",
+                                 module.__class__.__name__, exc)
+
         else:
             if module.indicators and not module.detected:
                 module.log.info("The %s module produced no detections!",
                                 module.__class__.__name__)
 
         try:
             module.to_timeline()
```

### Comparing `mvt-2.2.3/mvt/common/options.py` & `mvt-2.2.4/mvt/common/options.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/common/updates.py` & `mvt-2.2.4/mvt/common/updates.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/common/url.py` & `mvt-2.2.4/mvt/common/url.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/common/utils.py` & `mvt-2.2.4/mvt/common/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,17 +157,20 @@
     """Calculate the SHA256 hash of a file from a file path.
 
     :param file_path: Path to the file to hash
     :returns: The SHA256 hash string
 
     """
     sha256_hash = hashlib.sha256()
-    with open(file_path, "rb") as handle:
-        for byte_block in iter(lambda: handle.read(4096), b""):
-            sha256_hash.update(byte_block)
+    try:
+        with open(file_path, "rb") as handle:
+            for byte_block in iter(lambda: handle.read(4096), b""):
+                sha256_hash.update(byte_block)
+    except OSError:
+        return ""
 
     return sha256_hash.hexdigest()
 
 
 def generate_hashes_from_path(path: str, log) -> Iterator[dict]:
     """
     Generates hashes of all files at the given path.
```

### Comparing `mvt-2.2.3/mvt/common/virustotal.py` & `mvt-2.2.4/mvt/common/virustotal.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/cli.py` & `mvt-2.2.4/mvt/ios/cli.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/cmd_check_backup.py` & `mvt-2.2.4/mvt/ios/cmd_check_backup.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/cmd_check_fs.py` & `mvt-2.2.4/mvt/ios/cmd_check_fs.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/decrypt.py` & `mvt-2.2.4/mvt/ios/decrypt.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/modules/backup/backup_info.py` & `mvt-2.2.4/mvt/ios/modules/backup/backup_info.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/modules/backup/configuration_profiles.py` & `mvt-2.2.4/mvt/ios/modules/backup/configuration_profiles.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/modules/backup/manifest.py` & `mvt-2.2.4/mvt/ios/modules/backup/manifest.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/modules/backup/profile_events.py` & `mvt-2.2.4/mvt/ios/modules/backup/profile_events.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/modules/base.py` & `mvt-2.2.4/mvt/ios/modules/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     ) -> None:
         super().__init__(file_path=file_path, target_path=target_path,
                          results_path=results_path, fast_mode=fast_mode,
                          log=log, results=results)
 
         self.is_backup = False
         self.is_fs_dump = False
-        self.is_sysdiagnose = False
 
     def _recover_sqlite_db_if_needed(self, file_path: str,
                                      forced: Optional[bool] = False) -> None:
         """Tries to recover a malformed database by running a .clone command.
 
         :param file_path: Path to the malformed database file.
```

### Comparing `mvt-2.2.3/mvt/ios/modules/fs/__init__.py` & `mvt-2.2.4/mvt/ios/modules/fs/__init__.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/modules/fs/analytics.py` & `mvt-2.2.4/mvt/ios/modules/fs/analytics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
+import copy
 import logging
 import plistlib
 import sqlite3
 from typing import Optional, Union
 
 from mvt.common.utils import convert_mactime_to_iso
 
@@ -51,26 +52,28 @@
                 if not isinstance(value, str):
                     continue
 
                 ioc = self.indicators.check_process(value)
                 if ioc:
                     self.log.warning("Found mention of a malicious process \"%s\" in %s file at %s",
                                      value, result["artifact"],
-                                     result["timestamp"])
-                    result["matched_indicator"] = ioc
-                    self.detected.append(result)
+                                     result["isodate"])
+                    new_result = copy.copy(result)
+                    new_result["matched_indicator"] = ioc
+                    self.detected.append(new_result)
                     continue
 
                 ioc = self.indicators.check_domain(value)
                 if ioc:
                     self.log.warning("Found mention of a malicious domain \"%s\" in %s file at %s",
                                      value, result["artifact"],
-                                     result["timestamp"])
-                    result["matched_indicator"] = ioc
-                    self.detected.append(result)
+                                     result["isodate"])
+                    new_result = copy.copy(result)
+                    new_result["matched_indicator"] = ioc
+                    self.detected.append(new_result)
 
     def _extract_analytics_data(self):
         artifact = self.file_path.split("/")[-1]
 
         conn = sqlite3.connect(self.file_path)
         cur = conn.cursor()
```

### Comparing `mvt-2.2.3/mvt/ios/modules/fs/analytics_ios_versions.py` & `mvt-2.2.4/mvt/ios/modules/fs/analytics_ios_versions.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/modules/fs/cache_files.py` & `mvt-2.2.4/mvt/ios/modules/fs/cache_files.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/modules/fs/filesystem.py` & `mvt-2.2.4/mvt/ios/modules/fs/filesystem.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 
 from ..base import IOSExtraction
 
 
 class Filesystem(IOSExtraction):
     """This module extracts creation and modification date of files from a
     full file-system dump.
-
-
     """
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
```

### Comparing `mvt-2.2.3/mvt/ios/modules/fs/net_netusage.py` & `mvt-2.2.4/mvt/ios/modules/fs/net_netusage.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/modules/fs/safari_favicon.py` & `mvt-2.2.4/mvt/ios/modules/fs/safari_favicon.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/modules/fs/shutdownlog.py` & `mvt-2.2.4/mvt/ios/modules/fs/shutdownlog.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/modules/fs/version_history.py` & `mvt-2.2.4/mvt/ios/modules/fs/version_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/modules/fs/webkit_base.py` & `mvt-2.2.4/mvt/ios/modules/fs/webkit_base.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/modules/fs/webkit_indexeddb.py` & `mvt-2.2.4/mvt/ios/modules/fs/webkit_indexeddb.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/modules/fs/webkit_localstorage.py` & `mvt-2.2.4/mvt/ios/modules/fs/webkit_localstorage.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/modules/fs/webkit_safariviewservice.py` & `mvt-2.2.4/mvt/ios/modules/fs/webkit_safariviewservice.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/modules/mixed/__init__.py` & `mvt-2.2.4/mvt/ios/modules/mixed/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
+from .applications import Applications
+from .calendar import Calendar
 from .calls import Calls
 from .chrome_favicon import ChromeFavicon
 from .chrome_history import ChromeHistory
 from .contacts import Contacts
 from .firefox_favicon import FirefoxFavicon
 from .firefox_history import FirefoxHistory
 from .idstatuscache import IDStatusCache
@@ -24,8 +26,9 @@
 from .webkit_session_resource_log import WebkitSessionResourceLog
 from .whatsapp import Whatsapp
 
 MIXED_MODULES = [Calls, ChromeFavicon, ChromeHistory, Contacts, FirefoxFavicon,
                  FirefoxHistory, IDStatusCache, InteractionC, LocationdClients,
                  OSAnalyticsADDaily, Datausage, SafariBrowserState, SafariHistory,
                  TCC, SMS, SMSAttachments, WebkitResourceLoadStatistics,
-                 WebkitSessionResourceLog, Whatsapp, Shortcuts]
+                 WebkitSessionResourceLog, Whatsapp, Shortcuts, Applications,
+                 Calendar]
```

### Comparing `mvt-2.2.3/mvt/ios/modules/mixed/calls.py` & `mvt-2.2.4/mvt/ios/modules/mixed/calls.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/modules/mixed/chrome_favicon.py` & `mvt-2.2.4/mvt/ios/modules/mixed/chrome_favicon.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/modules/mixed/chrome_history.py` & `mvt-2.2.4/mvt/ios/modules/mixed/chrome_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/modules/mixed/contacts.py` & `mvt-2.2.4/mvt/ios/modules/mixed/contacts.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/modules/mixed/firefox_favicon.py` & `mvt-2.2.4/mvt/ios/modules/mixed/firefox_favicon.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/modules/mixed/firefox_history.py` & `mvt-2.2.4/mvt/ios/modules/mixed/firefox_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/modules/mixed/idstatuscache.py` & `mvt-2.2.4/mvt/ios/modules/mixed/idstatuscache.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/modules/mixed/locationd.py` & `mvt-2.2.4/mvt/ios/modules/mixed/locationd.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/modules/mixed/net_datausage.py` & `mvt-2.2.4/mvt/ios/modules/mixed/net_datausage.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/modules/mixed/osanalytics_addaily.py` & `mvt-2.2.4/mvt/ios/modules/mixed/osanalytics_addaily.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/modules/mixed/safari_browserstate.py` & `mvt-2.2.4/mvt/ios/modules/mixed/safari_browserstate.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/modules/mixed/safari_history.py` & `mvt-2.2.4/mvt/ios/modules/mixed/safari_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/modules/mixed/shortcuts.py` & `mvt-2.2.4/mvt/ios/modules/mixed/shortcuts.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/modules/mixed/sms.py` & `mvt-2.2.4/mvt/ios/modules/mixed/sms.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,15 +47,18 @@
         }
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for result in self.results:
-            message_links = check_for_links(result.get("text", ""))
+            message_links = result.get("links", [])
+            # Making sure not link was ignored
+            if message_links == []:
+                message_links = check_for_links(result.get("text", ""))
             ioc = self.indicators.check_domains(message_links)
             if ioc:
                 result["matched_indicator"] = ioc
                 self.detected.append(result)
 
     def run(self) -> None:
         self._find_ios_database(backup_ids=SMS_BACKUP_IDS,
@@ -114,22 +117,19 @@
             if not message.get("text", None):
                 message["text"] = ""
 
             alert = "ALERT: State-sponsored attackers may be targeting your iPhone"
             if message.get("text", "").startswith(alert):
                 self.log.warning("Apple warning about state-sponsored attack received on the %s",
                                  message["isodate"])
-                self.results.append(message)
             else:
                 # Extract links from the SMS message.
                 message_links = check_for_links(message.get("text", ""))
+                message["links"] = message_links
 
-                # If we find links in the messages or if they are empty we add
-                # them to the list.
-                if message_links or message.get("text", "").strip() == "":
-                    self.results.append(message)
+            self.results.append(message)
 
         cur.close()
         conn.close()
 
-        self.log.info("Extracted a total of %d SMS messages containing links",
+        self.log.info("Extracted a total of %d SMS messages",
                       len(self.results))
```

### Comparing `mvt-2.2.3/mvt/ios/modules/mixed/sms_attachments.py` & `mvt-2.2.4/mvt/ios/modules/mixed/sms_attachments.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/modules/mixed/tcc.py` & `mvt-2.2.4/mvt/ios/modules/mixed/tcc.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/modules/mixed/webkit_resource_load_statistics.py` & `mvt-2.2.4/mvt/ios/modules/mixed/webkit_resource_load_statistics.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,15 +66,23 @@
 
         self._recover_sqlite_db_if_needed(db_path)
 
         conn = sqlite3.connect(db_path)
         cur = conn.cursor()
 
         try:
-            cur.execute("SELECT * from ObservedDomains;")
+            # FIXME: table contains extra fields with timestamp here
+            cur.execute("""
+                SELECT
+                    domainID,
+                    registrableDomain,
+                    lastSeen,
+                    hadUserInteraction
+                from ObservedDomains;
+            """)
         except sqlite3.OperationalError:
             return
 
         for row in cur:
             self.results.append({
                 "domain_id": row[0],
                 "registrable_domain": row[1],
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mvt-2.2.3/mvt/ios/modules/mixed/webkit_session_resource_log.py` & `mvt-2.2.4/mvt/ios/modules/mixed/webkit_session_resource_log.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/modules/mixed/whatsapp.py` & `mvt-2.2.4/mvt/ios/modules/mixed/whatsapp.py`

 * *Files 10% similar despite different names*

```diff
@@ -108,18 +108,17 @@
             # Remove WhatsApp internal media URLs.
             filtered_links = []
             for link in message_links:
                 if not (link.startswith("https://mmg-fna.whatsapp.net/")
                         or link.startswith("https://mmg.whatsapp.net/")):
                     filtered_links.append(link)
 
-            # If we find messages with links, or if there's an empty message
-            # we add it to the results list.
+            # Add all the links found to the record
             if filtered_links or (message.get("ZTEXT") or "").strip() == "":
                 message["links"] = list(set(filtered_links))
-                self.results.append(message)
+            self.results.append(message)
 
         cur.close()
         conn.close()
 
-        self.log.info("Extracted a total of %d WhatsApp messages containing links",
+        self.log.info("Extracted a total of %d WhatsApp messages",
                       len(self.results))
```

### Comparing `mvt-2.2.3/mvt/ios/modules/net_base.py` & `mvt-2.2.4/mvt/ios/modules/net_base.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/mvt/ios/versions.py` & `mvt-2.2.4/mvt/ios/versions.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,15 +268,16 @@
     {"build": "20A392", "version": "16.0.3"},
     {"build": "20B82", "version": "16.1"},
     {"build": "20B101", "version": "16.1.1"},
     {"build": "20B110", "version": "16.1.2"},
     {"build": "20C65", "version": "16.2"},
     {"build": "20D47", "version": "16.3"},
     {"build": "20D67", "version": "16.3.1"},
-    {"build": "20E247", "version": "16.4"}
+    {"build": "20E247", "version": "16.4"},
+    {"build": "20E252", "version": "16.4.1"}
 ]
 
 
 def get_device_desc_from_id(identifier: str,
                             devices_list: list = IPHONE_MODELS) -> str:
     for model in devices_list:
         if identifier == model["identifier"]:
```

### Comparing `mvt-2.2.3/mvt.egg-info/PKG-INFO` & `mvt-2.2.4/mvt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvt
-Version: 2.2.3
+Version: 2.2.4
 Summary: Mobile Verification Toolkit
 Home-page: https://github.com/mvt-project/mvt
 Author: Claudio Guarnieri
 Author-email: nex@nex.sx
 License: MVT v1.1
 Keywords: security,mobile,forensics,malware
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mvt-2.2.3/mvt.egg-info/SOURCES.txt` & `mvt-2.2.4/mvt.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -104,14 +104,16 @@
 ./mvt/ios/modules/fs/shutdownlog.py
 ./mvt/ios/modules/fs/version_history.py
 ./mvt/ios/modules/fs/webkit_base.py
 ./mvt/ios/modules/fs/webkit_indexeddb.py
 ./mvt/ios/modules/fs/webkit_localstorage.py
 ./mvt/ios/modules/fs/webkit_safariviewservice.py
 ./mvt/ios/modules/mixed/__init__.py
+./mvt/ios/modules/mixed/applications.py
+./mvt/ios/modules/mixed/calendar.py
 ./mvt/ios/modules/mixed/calls.py
 ./mvt/ios/modules/mixed/chrome_favicon.py
 ./mvt/ios/modules/mixed/chrome_history.py
 ./mvt/ios/modules/mixed/contacts.py
 ./mvt/ios/modules/mixed/firefox_favicon.py
 ./mvt/ios/modules/mixed/firefox_history.py
 ./mvt/ios/modules/mixed/idstatuscache.py
@@ -150,14 +152,15 @@
 ./tests/android_androidqf/test_settings.py
 ./tests/android_androidqf/test_sms.py
 ./tests/common/__init__.py
 ./tests/common/test_indicators.py
 ./tests/common/test_utils.py
 ./tests/ios_backup/__init__.py
 ./tests/ios_backup/test_backup_info.py
+./tests/ios_backup/test_calendar.py
 ./tests/ios_backup/test_datausage.py
 ./tests/ios_backup/test_manifest.py
 ./tests/ios_backup/test_safari_browserstate.py
 ./tests/ios_backup/test_sms.py
 ./tests/ios_backup/test_tcc.py
 ./tests/ios_backup/test_webkit_resource_load_statistics.py
 ./tests/ios_fs/__init__.py
```

### Comparing `mvt-2.2.3/setup.cfg` & `mvt-2.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/tests/android/test_backup_module.py` & `mvt-2.2.4/tests/android/test_backup_module.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/tests/android/test_backup_parser.py` & `mvt-2.2.4/tests/android/test_backup_parser.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/tests/android/test_bugreport.py` & `mvt-2.2.4/tests/android/test_bugreport.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/tests/android/test_dumpsys_parser.py` & `mvt-2.2.4/tests/android/test_dumpsys_parser.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/tests/android_androidqf/test_dumpsysaccessbility.py` & `mvt-2.2.4/tests/android_androidqf/test_dumpsysaccessbility.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/tests/android_androidqf/test_dumpsysappops.py` & `mvt-2.2.4/tests/android_androidqf/test_dumpsysappops.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/tests/android_androidqf/test_dumpsyspackages.py` & `mvt-2.2.4/tests/android_androidqf/test_dumpsyspackages.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/tests/android_androidqf/test_dumpsysreceivers.py` & `mvt-2.2.4/tests/android_androidqf/test_dumpsysreceivers.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/tests/android_androidqf/test_getprop.py` & `mvt-2.2.4/tests/android_androidqf/test_getprop.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/tests/android_androidqf/test_processes.py` & `mvt-2.2.4/tests/android_androidqf/test_processes.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/tests/android_androidqf/test_settings.py` & `mvt-2.2.4/tests/android_androidqf/test_settings.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/tests/android_androidqf/test_sms.py` & `mvt-2.2.4/tests/android_androidqf/test_sms.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/tests/common/test_indicators.py` & `mvt-2.2.4/tests/common/test_indicators.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,16 +20,18 @@
         assert len(ind.ioc_collections[0]["file_names"]) == 1
         assert len(ind.ioc_collections[0]["processes"]) == 1
         assert len(ind.ioc_collections[0]["android_property_names"]) == 1
 
     def test_check_domain(self, indicator_file):
         ind = Indicators(log=logging)
         ind.load_indicators_files([indicator_file], load_default=False)
+        assert ind.check_domain(42) is None
         assert ind.check_domain("https://www.example.org/foobar")
         assert ind.check_domain("http://example.org:8080/toto")
+        assert ind.check_domain("https://github.com") is None
 
     def test_check_android_property(self, indicator_file):
         ind = Indicators(log=logging)
         ind.load_indicators_files([indicator_file], load_default=False)
         assert ind.check_android_property_name("sys.foobar")
         assert ind.check_android_property_name("sys.soundsokay") is None
```

### Comparing `mvt-2.2.3/tests/common/test_utils.py` & `mvt-2.2.4/tests/common/test_utils.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/tests/conftest.py` & `mvt-2.2.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/tests/ios_backup/test_backup_info.py` & `mvt-2.2.4/tests/ios_backup/test_backup_info.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/tests/ios_backup/test_datausage.py` & `mvt-2.2.4/tests/ios_backup/test_datausage.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/tests/ios_backup/test_manifest.py` & `mvt-2.2.4/tests/ios_backup/test_manifest.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/tests/ios_backup/test_safari_browserstate.py` & `mvt-2.2.4/tests/ios_backup/test_safari_browserstate.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/tests/ios_backup/test_sms.py` & `mvt-2.2.4/tests/ios_backup/test_sms.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/tests/ios_backup/test_tcc.py` & `mvt-2.2.4/tests/ios_backup/test_tcc.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/tests/ios_backup/test_webkit_resource_load_statistics.py` & `mvt-2.2.4/tests/ios_backup/test_webkit_resource_load_statistics.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/tests/ios_fs/test_filesystem.py` & `mvt-2.2.4/tests/ios_fs/test_filesystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 
 
 class TestFilesystem:
 
     def test_filesystem(self):
         m = Filesystem(target_path=get_ios_backup_folder())
         run_module(m)
-        assert len(m.results) == 12
-        assert len(m.timeline) == 12
+        assert len(m.results) == 14
+        assert len(m.timeline) == 14
         assert len(m.detected) == 0
 
     def test_detection(self, indicator_file):
         m = Filesystem(target_path=get_ios_backup_folder())
         ind = Indicators(log=logging.getLogger())
         ind.parse_stix2(indicator_file)
         # Adds a filename that exist in the folder
         ind.ioc_collections[0]["processes"].append("64d0019cb3d46bfc8cce545a8ba54b93e7ea9347")
         m.indicators = ind
         run_module(m)
-        assert len(m.results) == 12
-        assert len(m.timeline) == 12
+        assert len(m.results) == 14
+        assert len(m.timeline) == 14
         assert len(m.detected) == 1
```

### Comparing `mvt-2.2.3/tests/test_check_android_androidqf.py` & `mvt-2.2.4/tests/test_check_android_androidqf.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/tests/test_check_android_bugreport.py` & `mvt-2.2.4/tests/test_check_android_bugreport.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/tests/test_check_ios_backup.py` & `mvt-2.2.4/tests/test_check_ios_backup.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.3/tests/utils.py` & `mvt-2.2.4/tests/utils.py`

 * *Files identical despite different names*

