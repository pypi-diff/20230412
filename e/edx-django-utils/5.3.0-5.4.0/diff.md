# Comparing `tmp/edx-django-utils-5.3.0.tar.gz` & `tmp/edx-django-utils-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-django-utils-5.3.0.tar", last modified: Fri Mar 17 20:50:39 2023, max compression
+gzip compressed data, was "edx-django-utils-5.4.0.tar", last modified: Wed Apr 12 14:25:41 2023, max compression
```

## Comparing `edx-django-utils-5.3.0.tar` & `edx-django-utils-5.4.0.tar`

### file list

```diff
@@ -1,117 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:39.615829 edx-django-utils-5.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)    12505 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    25567 2023-03-17 20:50:39.615829 edx-django-utils-5.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6841 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:39.607829 edx-django-utils-5.3.0/edx_django_utils/
--rw-r--r--   0 runner    (1001) docker     (122)      157 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:39.611829 edx-django-utils-5.3.0/edx_django_utils/admin/
--rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/admin/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:39.611829 edx-django-utils-5.3.0/edx_django_utils/admin/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/admin/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      225 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/admin/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     1430 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/admin/tests/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (122)      246 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:39.611829 edx-django-utils-5.3.0/edx_django_utils/cache/
--rw-r--r--   0 runner    (1001) docker     (122)      148 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1400 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/cache/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:39.611829 edx-django-utils-5.3.0/edx_django_utils/cache/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/cache/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3077 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/cache/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)    12463 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/cache/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10907 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/cache/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:39.611829 edx-django-utils-5.3.0/edx_django_utils/db/
--rw-r--r--   0 runner    (1001) docker     (122)      387 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1754 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/db/queryset_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     4834 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/db/read_replica.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:39.611829 edx-django-utils-5.3.0/edx_django_utils/db/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/db/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2152 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/db/tests/test_queryset_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3454 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/db/tests/test_read_replica.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:39.611829 edx-django-utils-5.3.0/edx_django_utils/ip/
--rw-r--r--   0 runner    (1001) docker     (122)     7936 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/ip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:39.611829 edx-django-utils-5.3.0/edx_django_utils/ip/internal/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/ip/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10730 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/ip/internal/ip.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:39.611829 edx-django-utils-5.3.0/edx_django_utils/ip/internal/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/ip/internal/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13591 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/ip/internal/tests/test_ip.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:39.611829 edx-django-utils-5.3.0/edx_django_utils/logging/
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:39.611829 edx-django-utils-5.3.0/edx_django_utils/logging/internal/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/logging/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      791 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/logging/internal/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     7961 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/logging/internal/log_sensitive.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:39.611829 edx-django-utils-5.3.0/edx_django_utils/logging/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/logging/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2875 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/logging/tests/test_log_sensitive.py
--rw-r--r--   0 runner    (1001) docker     (122)     1734 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/logging/tests/test_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:39.611829 edx-django-utils-5.3.0/edx_django_utils/monitoring/
--rw-r--r--   0 runner    (1001) docker     (122)      899 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/monitoring/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:39.611829 edx-django-utils-5.3.0/edx_django_utils/monitoring/internal/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/monitoring/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:39.611829 edx-django-utils-5.3.0/edx_django_utils/monitoring/internal/code_owner/
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/monitoring/internal/code_owner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5260 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/monitoring/internal/code_owner/middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)    10474 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/monitoring/internal/code_owner/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    21330 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/monitoring/internal/middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)     2621 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/monitoring/internal/transactions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3895 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/monitoring/internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2255 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/monitoring/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:39.611829 edx-django-utils-5.3.0/edx_django_utils/monitoring/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)    11530 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/monitoring/scripts/new_relic_nrql_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     8178 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/monitoring/scripts/process_cookie_monitoring_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:39.611829 edx-django-utils-5.3.0/edx_django_utils/monitoring/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/monitoring/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:39.615829 edx-django-utils-5.3.0/edx_django_utils/monitoring/tests/code_owner/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/monitoring/tests/code_owner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      272 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/monitoring/tests/code_owner/mock_views.py
--rw-r--r--   0 runner    (1001) docker     (122)    12959 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/monitoring/tests/code_owner/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)     6037 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/monitoring/tests/code_owner/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     6238 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/monitoring/tests/test_custom_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (122)    11923 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/monitoring/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)      759 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/monitoring/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3016 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/monitoring/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:39.615829 edx-django-utils-5.3.0/edx_django_utils/plugins/
--rw-r--r--   0 runner    (1001) docker     (122)      531 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/plugins/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     3200 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/plugins/pluggable_override.py
--rw-r--r--   0 runner    (1001) docker     (122)      794 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/plugins/plugin_apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     4082 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/plugins/plugin_contexts.py
--rw-r--r--   0 runner    (1001) docker     (122)     1682 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/plugins/plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/plugins/plugin_settings.py
--rw-r--r--   0 runner    (1001) docker     (122)     2824 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/plugins/plugin_signals.py
--rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/plugins/plugin_urls.py
--rw-r--r--   0 runner    (1001) docker     (122)      408 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/plugins/registry.py
--rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/plugins/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:39.615829 edx-django-utils-5.3.0/edx_django_utils/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1768 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/tests/test_pluggable_override.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:39.615829 edx-django-utils-5.3.0/edx_django_utils/user/
--rw-r--r--   0 runner    (1001) docker     (122)      556 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:39.615829 edx-django-utils-5.3.0/edx_django_utils/user/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/user/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:39.615829 edx-django-utils-5.3.0/edx_django_utils/user/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/user/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5165 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/user/management/commands/manage_group.py
--rw-r--r--   0 runner    (1001) docker     (122)     6487 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/user/management/commands/manage_user.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:39.615829 edx-django-utils-5.3.0/edx_django_utils/user/management/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/user/management/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7382 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/user/management/tests/test_manage_group.py
--rw-r--r--   0 runner    (1001) docker     (122)     7796 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/user/management/tests/test_manage_user.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:39.615829 edx-django-utils-5.3.0/edx_django_utils/user/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/user/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      902 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/edx_django_utils/user/tests/test_user.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:39.611829 edx-django-utils-5.3.0/edx_django_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    25567 2023-03-17 20:50:39.000000 edx-django-utils-5.3.0/edx_django_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3678 2023-03-17 20:50:39.000000 edx-django-utils-5.3.0/edx_django_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-17 20:50:39.000000 edx-django-utils-5.3.0/edx_django_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       87 2023-03-17 20:50:39.000000 edx-django-utils-5.3.0/edx_django_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-17 20:50:39.000000 edx-django-utils-5.3.0/edx_django_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-03-17 20:50:39.000000 edx-django-utils-5.3.0/edx_django_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-03-17 20:50:39.000000 edx-django-utils-5.3.0/edx_django_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 20:50:39.615829 edx-django-utils-5.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      738 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      882 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      126 2023-03-17 20:50:39.615829 edx-django-utils-5.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5451 2023-03-17 20:50:35.000000 edx-django-utils-5.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.183745 edx-django-utils-5.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    12775 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    26136 2023-04-12 14:25:41.183745 edx-django-utils-5.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6980 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.167745 edx-django-utils-5.4.0/edx_django_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.171745 edx-django-utils-5.4.0/edx_django_utils/admin/
+-rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/admin/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.171745 edx-django-utils-5.4.0/edx_django_utils/admin/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/admin/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      225 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/admin/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1430 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/admin/tests/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (122)      246 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.171745 edx-django-utils-5.4.0/edx_django_utils/cache/
+-rw-r--r--   0 runner    (1001) docker     (122)      148 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1400 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/cache/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.171745 edx-django-utils-5.4.0/edx_django_utils/cache/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/cache/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3077 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/cache/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12463 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/cache/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10907 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/cache/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.171745 edx-django-utils-5.4.0/edx_django_utils/db/
+-rw-r--r--   0 runner    (1001) docker     (122)      387 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1754 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/db/queryset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4834 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/db/read_replica.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.171745 edx-django-utils-5.4.0/edx_django_utils/db/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/db/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2152 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/db/tests/test_queryset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3454 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/db/tests/test_read_replica.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.171745 edx-django-utils-5.4.0/edx_django_utils/ip/
+-rw-r--r--   0 runner    (1001) docker     (122)     7936 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/ip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.171745 edx-django-utils-5.4.0/edx_django_utils/ip/internal/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/ip/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10730 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/ip/internal/ip.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.171745 edx-django-utils-5.4.0/edx_django_utils/ip/internal/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/ip/internal/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13591 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/ip/internal/tests/test_ip.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.171745 edx-django-utils-5.4.0/edx_django_utils/logging/
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.171745 edx-django-utils-5.4.0/edx_django_utils/logging/internal/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/logging/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      791 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/logging/internal/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7961 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/logging/internal/log_sensitive.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.171745 edx-django-utils-5.4.0/edx_django_utils/logging/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/logging/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2875 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/logging/tests/test_log_sensitive.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1734 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/logging/tests/test_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.171745 edx-django-utils-5.4.0/edx_django_utils/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (122)      899 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.175745 edx-django-utils-5.4.0/edx_django_utils/monitoring/internal/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.175745 edx-django-utils-5.4.0/edx_django_utils/monitoring/internal/code_owner/
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/internal/code_owner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5260 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/internal/code_owner/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10474 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/internal/code_owner/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21330 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/internal/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2621 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/internal/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3895 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2255 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.175745 edx-django-utils-5.4.0/edx_django_utils/monitoring/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)    11530 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/scripts/new_relic_nrql_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8178 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/scripts/process_cookie_monitoring_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.175745 edx-django-utils-5.4.0/edx_django_utils/monitoring/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.175745 edx-django-utils-5.4.0/edx_django_utils/monitoring/tests/code_owner/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/tests/code_owner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      272 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/tests/code_owner/mock_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12959 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/tests/code_owner/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6037 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/tests/code_owner/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6238 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/tests/test_custom_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11923 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)      759 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3016 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/monitoring/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.179745 edx-django-utils-5.4.0/edx_django_utils/plugins/
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/plugins/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3200 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/plugins/pluggable_override.py
+-rw-r--r--   0 runner    (1001) docker     (122)      794 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/plugins/plugin_apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4082 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/plugins/plugin_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1682 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/plugins/plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/plugins/plugin_settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2824 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/plugins/plugin_signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/plugins/plugin_urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      408 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/plugins/registry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/plugins/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.167745 edx-django-utils-5.4.0/edx_django_utils/security/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.179745 edx-django-utils-5.4.0/edx_django_utils/security/csp/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/security/csp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5753 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/security/csp/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.179745 edx-django-utils-5.4.0/edx_django_utils/security/csp/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     4974 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/security/csp/tests/test_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.179745 edx-django-utils-5.4.0/edx_django_utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1768 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/tests/test_pluggable_override.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.179745 edx-django-utils-5.4.0/edx_django_utils/user/
+-rw-r--r--   0 runner    (1001) docker     (122)      556 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.179745 edx-django-utils-5.4.0/edx_django_utils/user/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/user/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.179745 edx-django-utils-5.4.0/edx_django_utils/user/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/user/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5165 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/user/management/commands/manage_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6487 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/user/management/commands/manage_user.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.179745 edx-django-utils-5.4.0/edx_django_utils/user/management/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/user/management/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7382 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/user/management/tests/test_manage_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7796 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/user/management/tests/test_manage_user.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.179745 edx-django-utils-5.4.0/edx_django_utils/user/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/user/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      902 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/edx_django_utils/user/tests/test_user.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.167745 edx-django-utils-5.4.0/edx_django_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    26136 2023-04-12 14:25:41.000000 edx-django-utils-5.4.0/edx_django_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3819 2023-04-12 14:25:41.000000 edx-django-utils-5.4.0/edx_django_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 14:25:41.000000 edx-django-utils-5.4.0/edx_django_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       87 2023-04-12 14:25:41.000000 edx-django-utils-5.4.0/edx_django_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 14:25:41.000000 edx-django-utils-5.4.0/edx_django_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-04-12 14:25:41.000000 edx-django-utils-5.4.0/edx_django_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-12 14:25:41.000000 edx-django-utils-5.4.0/edx_django_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 14:25:41.183745 edx-django-utils-5.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      617 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      882 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-04-12 14:25:41.183745 edx-django-utils-5.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5451 2023-04-12 14:25:36.000000 edx-django-utils-5.4.0/setup.py
```

### Comparing `edx-django-utils-5.3.0/CHANGELOG.rst` & `edx-django-utils-5.4.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,30 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[5.4.0] - 2023-04-12
+--------------------
+
+Added
+~~~~~
+
+* Added Content-Security-Policy response header middleware under ``security/csp``
+
+[5.3.0] - 2023-03-17
+--------------------
+
+Fixed
+~~~~~
+
+* Report both specified and existing email when refusing to create a user
+
 [5.2.0] - 2022-10-06
 --------------------
 
 Added
 ~~~~~
 
 * Added a wrapper for background_task in monitoring.
```

### Comparing `edx-django-utils-5.3.0/LICENSE.txt` & `edx-django-utils-5.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/PKG-INFO` & `edx-django-utils-5.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: edx-django-utils
-Version: 5.3.0
+Version: 5.4.0
 Summary: EdX utilities for Django Application development.
 Home-page: https://github.com/openedx/edx-django-utils
 Author: edX
 Author-email: oscm@edx.org
 License: UNKNOWN
 Description: edx-django-utils
         ================
@@ -32,26 +32,30 @@
         * `Logging Utilities`_: Includes log filters and an encrypted logging helper.
         
         * `Monitoring Utilities`_: Includes Middleware and utilities for enhanced monitoring.
           At this time, supports NewRelic monitoring.
         
         * `Plugin Infrastructure`_: Enables enhanced Django Plugin capabilities.
         
+        * `Security Utilities`_: Includes a middleware to add CSP response headers.
+        
         .. _Cache Utilities: edx_django_utils/cache/README.rst
         
         .. _Django User and Group Utilities: edx_django_utils/user/README.rst
         
         .. _IP Address Utilities: edx_django_utils/ip/README.rst
         
         .. _Logging Utilities: edx_django_utils/logging/README.rst
         
         .. _Monitoring Utilities: edx_django_utils/monitoring/README.rst
         
         .. _Plugin Infrastructure: edx_django_utils/plugins/README.rst
         
+        .. _Security Utilities: edx_django_utils/security/README.rst
+        
         Documentation
         -------------
         
         The full documentation is in the docs directory, and is published to https://edx-django-utils.readthedocs.org.
         
         Getting Started
         ---------------
@@ -218,14 +222,30 @@
            This project adheres to Semantic Versioning (https://semver.org/).
         
         .. There should always be an "Unreleased" section for changes pending release.
         
         Unreleased
         ----------
         
+        [5.4.0] - 2023-04-12
+        --------------------
+        
+        Added
+        ~~~~~
+        
+        * Added Content-Security-Policy response header middleware under ``security/csp``
+        
+        [5.3.0] - 2023-03-17
+        --------------------
+        
+        Fixed
+        ~~~~~
+        
+        * Report both specified and existing email when refusing to create a user
+        
         [5.2.0] - 2022-10-06
         --------------------
         
         Added
         ~~~~~
         
         * Added a wrapper for background_task in monitoring.
```

### Comparing `edx-django-utils-5.3.0/README.rst` & `edx-django-utils-5.4.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -24,26 +24,30 @@
 * `Logging Utilities`_: Includes log filters and an encrypted logging helper.
 
 * `Monitoring Utilities`_: Includes Middleware and utilities for enhanced monitoring.
   At this time, supports NewRelic monitoring.
 
 * `Plugin Infrastructure`_: Enables enhanced Django Plugin capabilities.
 
+* `Security Utilities`_: Includes a middleware to add CSP response headers.
+
 .. _Cache Utilities: edx_django_utils/cache/README.rst
 
 .. _Django User and Group Utilities: edx_django_utils/user/README.rst
 
 .. _IP Address Utilities: edx_django_utils/ip/README.rst
 
 .. _Logging Utilities: edx_django_utils/logging/README.rst
 
 .. _Monitoring Utilities: edx_django_utils/monitoring/README.rst
 
 .. _Plugin Infrastructure: edx_django_utils/plugins/README.rst
 
+.. _Security Utilities: edx_django_utils/security/README.rst
+
 Documentation
 -------------
 
 The full documentation is in the docs directory, and is published to https://edx-django-utils.readthedocs.org.
 
 Getting Started
 ---------------
```

### Comparing `edx-django-utils-5.3.0/edx_django_utils/admin/mixins.py` & `edx-django-utils-5.4.0/edx_django_utils/admin/mixins.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/admin/tests/test_mixins.py` & `edx-django-utils-5.4.0/edx_django_utils/admin/tests/test_mixins.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/cache/middleware.py` & `edx-django-utils-5.4.0/edx_django_utils/cache/middleware.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/cache/tests/test_middleware.py` & `edx-django-utils-5.4.0/edx_django_utils/cache/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/cache/tests/test_utils.py` & `edx-django-utils-5.4.0/edx_django_utils/cache/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/cache/utils.py` & `edx-django-utils-5.4.0/edx_django_utils/cache/utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/db/queryset_utils.py` & `edx-django-utils-5.4.0/edx_django_utils/db/queryset_utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/db/read_replica.py` & `edx-django-utils-5.4.0/edx_django_utils/db/read_replica.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/db/tests/test_queryset_utils.py` & `edx-django-utils-5.4.0/edx_django_utils/db/tests/test_queryset_utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/db/tests/test_read_replica.py` & `edx-django-utils-5.4.0/edx_django_utils/db/tests/test_read_replica.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/ip/__init__.py` & `edx-django-utils-5.4.0/edx_django_utils/ip/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/ip/internal/ip.py` & `edx-django-utils-5.4.0/edx_django_utils/ip/internal/ip.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/ip/internal/tests/test_ip.py` & `edx-django-utils-5.4.0/edx_django_utils/ip/internal/tests/test_ip.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/logging/internal/filters.py` & `edx-django-utils-5.4.0/edx_django_utils/logging/internal/filters.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/logging/internal/log_sensitive.py` & `edx-django-utils-5.4.0/edx_django_utils/logging/internal/log_sensitive.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/logging/tests/test_log_sensitive.py` & `edx-django-utils-5.4.0/edx_django_utils/logging/tests/test_log_sensitive.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/logging/tests/test_logging.py` & `edx-django-utils-5.4.0/edx_django_utils/logging/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/monitoring/__init__.py` & `edx-django-utils-5.4.0/edx_django_utils/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/monitoring/internal/code_owner/middleware.py` & `edx-django-utils-5.4.0/edx_django_utils/monitoring/internal/code_owner/middleware.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/monitoring/internal/code_owner/utils.py` & `edx-django-utils-5.4.0/edx_django_utils/monitoring/internal/code_owner/utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/monitoring/internal/middleware.py` & `edx-django-utils-5.4.0/edx_django_utils/monitoring/internal/middleware.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/monitoring/internal/transactions.py` & `edx-django-utils-5.4.0/edx_django_utils/monitoring/internal/transactions.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/monitoring/internal/utils.py` & `edx-django-utils-5.4.0/edx_django_utils/monitoring/internal/utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/monitoring/middleware.py` & `edx-django-utils-5.4.0/edx_django_utils/monitoring/middleware.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/monitoring/scripts/new_relic_nrql_search.py` & `edx-django-utils-5.4.0/edx_django_utils/monitoring/scripts/new_relic_nrql_search.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/monitoring/scripts/process_cookie_monitoring_logs.py` & `edx-django-utils-5.4.0/edx_django_utils/monitoring/scripts/process_cookie_monitoring_logs.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/monitoring/tests/code_owner/test_middleware.py` & `edx-django-utils-5.4.0/edx_django_utils/monitoring/tests/code_owner/test_middleware.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/monitoring/tests/code_owner/test_utils.py` & `edx-django-utils-5.4.0/edx_django_utils/monitoring/tests/code_owner/test_utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/monitoring/tests/test_custom_monitoring.py` & `edx-django-utils-5.4.0/edx_django_utils/monitoring/tests/test_custom_monitoring.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/monitoring/tests/test_middleware.py` & `edx-django-utils-5.4.0/edx_django_utils/monitoring/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/monitoring/tests/test_utils.py` & `edx-django-utils-5.4.0/edx_django_utils/monitoring/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/monitoring/utils.py` & `edx-django-utils-5.4.0/edx_django_utils/monitoring/utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/plugins/__init__.py` & `edx-django-utils-5.4.0/edx_django_utils/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/plugins/constants.py` & `edx-django-utils-5.4.0/edx_django_utils/plugins/constants.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/plugins/pluggable_override.py` & `edx-django-utils-5.4.0/edx_django_utils/plugins/pluggable_override.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/plugins/plugin_apps.py` & `edx-django-utils-5.4.0/edx_django_utils/plugins/plugin_apps.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/plugins/plugin_contexts.py` & `edx-django-utils-5.4.0/edx_django_utils/plugins/plugin_contexts.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/plugins/plugin_manager.py` & `edx-django-utils-5.4.0/edx_django_utils/plugins/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/plugins/plugin_settings.py` & `edx-django-utils-5.4.0/edx_django_utils/plugins/plugin_settings.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/plugins/plugin_signals.py` & `edx-django-utils-5.4.0/edx_django_utils/plugins/plugin_signals.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/plugins/plugin_urls.py` & `edx-django-utils-5.4.0/edx_django_utils/plugins/plugin_urls.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/plugins/utils.py` & `edx-django-utils-5.4.0/edx_django_utils/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/tests/test_pluggable_override.py` & `edx-django-utils-5.4.0/edx_django_utils/tests/test_pluggable_override.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/user/__init__.py` & `edx-django-utils-5.4.0/edx_django_utils/user/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/user/management/commands/manage_group.py` & `edx-django-utils-5.4.0/edx_django_utils/user/management/commands/manage_group.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/user/management/commands/manage_user.py` & `edx-django-utils-5.4.0/edx_django_utils/user/management/commands/manage_user.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/user/management/tests/test_manage_group.py` & `edx-django-utils-5.4.0/edx_django_utils/user/management/tests/test_manage_group.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/user/management/tests/test_manage_user.py` & `edx-django-utils-5.4.0/edx_django_utils/user/management/tests/test_manage_user.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils/user/tests/test_user.py` & `edx-django-utils-5.4.0/edx_django_utils/user/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/edx_django_utils.egg-info/PKG-INFO` & `edx-django-utils-5.4.0/edx_django_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: edx-django-utils
-Version: 5.3.0
+Version: 5.4.0
 Summary: EdX utilities for Django Application development.
 Home-page: https://github.com/openedx/edx-django-utils
 Author: edX
 Author-email: oscm@edx.org
 License: UNKNOWN
 Description: edx-django-utils
         ================
@@ -32,26 +32,30 @@
         * `Logging Utilities`_: Includes log filters and an encrypted logging helper.
         
         * `Monitoring Utilities`_: Includes Middleware and utilities for enhanced monitoring.
           At this time, supports NewRelic monitoring.
         
         * `Plugin Infrastructure`_: Enables enhanced Django Plugin capabilities.
         
+        * `Security Utilities`_: Includes a middleware to add CSP response headers.
+        
         .. _Cache Utilities: edx_django_utils/cache/README.rst
         
         .. _Django User and Group Utilities: edx_django_utils/user/README.rst
         
         .. _IP Address Utilities: edx_django_utils/ip/README.rst
         
         .. _Logging Utilities: edx_django_utils/logging/README.rst
         
         .. _Monitoring Utilities: edx_django_utils/monitoring/README.rst
         
         .. _Plugin Infrastructure: edx_django_utils/plugins/README.rst
         
+        .. _Security Utilities: edx_django_utils/security/README.rst
+        
         Documentation
         -------------
         
         The full documentation is in the docs directory, and is published to https://edx-django-utils.readthedocs.org.
         
         Getting Started
         ---------------
@@ -218,14 +222,30 @@
            This project adheres to Semantic Versioning (https://semver.org/).
         
         .. There should always be an "Unreleased" section for changes pending release.
         
         Unreleased
         ----------
         
+        [5.4.0] - 2023-04-12
+        --------------------
+        
+        Added
+        ~~~~~
+        
+        * Added Content-Security-Policy response header middleware under ``security/csp``
+        
+        [5.3.0] - 2023-03-17
+        --------------------
+        
+        Fixed
+        ~~~~~
+        
+        * Report both specified and existing email when refusing to create a user
+        
         [5.2.0] - 2022-10-06
         --------------------
         
         Added
         ~~~~~
         
         * Added a wrapper for background_task in monitoring.
```

### Comparing `edx-django-utils-5.3.0/edx_django_utils.egg-info/SOURCES.txt` & `edx-django-utils-5.4.0/edx_django_utils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,17 @@
 edx_django_utils/plugins/plugin_contexts.py
 edx_django_utils/plugins/plugin_manager.py
 edx_django_utils/plugins/plugin_settings.py
 edx_django_utils/plugins/plugin_signals.py
 edx_django_utils/plugins/plugin_urls.py
 edx_django_utils/plugins/registry.py
 edx_django_utils/plugins/utils.py
+edx_django_utils/security/csp/__init__.py
+edx_django_utils/security/csp/middleware.py
+edx_django_utils/security/csp/tests/test_middleware.py
 edx_django_utils/tests/test_pluggable_override.py
 edx_django_utils/user/__init__.py
 edx_django_utils/user/management/__init__.py
 edx_django_utils/user/management/commands/__init__.py
 edx_django_utils/user/management/commands/manage_group.py
 edx_django_utils/user/management/commands/manage_user.py
 edx_django_utils/user/management/tests/__init__.py
```

### Comparing `edx-django-utils-5.3.0/requirements/base.in` & `edx-django-utils-5.4.0/requirements/base.in`

 * *Files 18% similar despite different names*

```diff
@@ -2,12 +2,11 @@
 
 -c constraints.txt
 
 Django                    # Web application framework
 django-waffle             # Allows for feature toggles in Django.
 newrelic                  # New Relic agent for performance monitoring
 psutil                    # Library for retrieving information on running processes and system utilization
-                          # NOTE: psutil pinned to match edx-platform version. Will need to be updated at the same time.
 stevedore                 # Used by plugins to make importing easier
 django-crum               # Used by logging filters
 PyNaCl                    # User-friendly cryptography (wrapper and bindings for libsodium)
 click                     # CLI tools
```

### Comparing `edx-django-utils-5.3.0/requirements/constraints.txt` & `edx-django-utils-5.4.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.3.0/setup.py` & `edx-django-utils-5.4.0/setup.py`

 * *Files identical despite different names*

