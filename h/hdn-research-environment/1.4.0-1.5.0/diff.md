# Comparing `tmp/hdn-research-environment-1.4.0.tar.gz` & `tmp/hdn-research-environment-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hdn-research-environment-1.4.0.tar", last modified: Wed Feb 22 22:00:27 2023, max compression
+gzip compressed data, was "dist/hdn-research-environment-1.5.0.tar", last modified: Wed Apr 12 08:04:18 2023, max compression
```

## Comparing `hdn-research-environment-1.4.0.tar` & `hdn-research-environment-1.5.0.tar`

### file list

```diff
@@ -1,85 +1,84 @@
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-02-22 22:00:27.000000 hdn-research-environment-1.4.0/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1551 2022-03-29 08:15:30.000000 hdn-research-environment-1.4.0/LICENSE
--rw-r--r--   0 karolszuster   (501) staff       (20)      115 2022-03-29 08:32:41.000000 hdn-research-environment-1.4.0/MANIFEST.in
--rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-02-22 22:00:27.000000 hdn-research-environment-1.4.0/PKG-INFO
--rw-r--r--   0 karolszuster   (501) staff       (20)       90 2022-03-29 07:59:09.000000 hdn-research-environment-1.4.0/README.md
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-02-22 22:00:27.000000 hdn-research-environment-1.4.0/environment/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-1.4.0/environment/__init__.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-02-22 22:00:27.000000 hdn-research-environment-1.4.0/environment/api/
--rw-r--r--   0 karolszuster   (501) staff       (20)     2898 2023-02-22 22:00:03.000000 hdn-research-environment-1.4.0/environment/api/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      749 2023-02-11 18:26:19.000000 hdn-research-environment-1.4.0/environment/api/auth.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      663 2023-02-11 18:26:19.000000 hdn-research-environment-1.4.0/environment/api/decorators.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-02-22 22:00:27.000000 hdn-research-environment-1.4.0/environment/api/tests/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-1.4.0/environment/api/tests/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1392 2023-02-22 21:44:17.000000 hdn-research-environment-1.4.0/environment/api/tests/test_auth.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1543 2023-02-22 21:44:17.000000 hdn-research-environment-1.4.0/environment/api/tests/test_decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      154 2022-03-29 08:08:24.000000 hdn-research-environment-1.4.0/environment/apps.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2467 2023-02-22 22:00:03.000000 hdn-research-environment-1.4.0/environment/constants.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1298 2022-03-29 08:08:24.000000 hdn-research-environment-1.4.0/environment/decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1619 2022-03-29 08:08:24.000000 hdn-research-environment-1.4.0/environment/deserializers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2830 2023-02-22 22:00:03.000000 hdn-research-environment-1.4.0/environment/entities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      547 2022-03-29 08:08:24.000000 hdn-research-environment-1.4.0/environment/exceptions.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1727 2023-02-22 22:00:03.000000 hdn-research-environment-1.4.0/environment/forms.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      155 2022-03-29 08:08:24.000000 hdn-research-environment-1.4.0/environment/managers.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-02-22 22:00:27.000000 hdn-research-environment-1.4.0/environment/migrations/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1444 2022-03-29 08:08:24.000000 hdn-research-environment-1.4.0/environment/migrations/0001_initial.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1580 2022-03-29 08:08:24.000000 hdn-research-environment-1.4.0/environment/migrations/0002_billingsetup.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      404 2022-03-29 08:08:24.000000 hdn-research-environment-1.4.0/environment/migrations/0003_cloudidentity_is_workspace_done.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      421 2022-03-29 08:08:24.000000 hdn-research-environment-1.4.0/environment/migrations/0004_auto_20220309_0330.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2184 2022-03-29 15:52:24.000000 hdn-research-environment-1.4.0/environment/migrations/0005_workflow.py
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-1.4.0/environment/migrations/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1821 2023-01-20 14:18:52.000000 hdn-research-environment-1.4.0/environment/models.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    14521 2023-02-22 22:00:03.000000 hdn-research-environment-1.4.0/environment/services.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2556 2023-01-20 14:18:52.000000 hdn-research-environment-1.4.0/environment/signals.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-02-22 22:00:27.000000 hdn-research-environment-1.4.0/environment/static/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-02-22 22:00:27.000000 hdn-research-environment-1.4.0/environment/static/environment/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-02-22 22:00:27.000000 hdn-research-environment-1.4.0/environment/static/environment/css/
--rw-r--r--   0 karolszuster   (501) staff       (20)      342 2023-02-22 22:00:03.000000 hdn-research-environment-1.4.0/environment/static/environment/css/create_research_environment.css
--rw-r--r--   0 karolszuster   (501) staff       (20)     6583 2022-03-29 08:08:24.000000 hdn-research-environment-1.4.0/environment/static/environment/css/environment-base.css
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-02-22 22:00:27.000000 hdn-research-environment-1.4.0/environment/static/environment/js/
--rw-r--r--   0 karolszuster   (501) staff       (20)      564 2022-03-30 12:50:58.000000 hdn-research-environment-1.4.0/environment/static/environment/js/cookie.js
--rw-r--r--   0 karolszuster   (501) staff       (20)      367 2023-02-22 21:40:18.000000 hdn-research-environment-1.4.0/environment/static/environment/js/gpu_acceleration_disabling.js
--rw-r--r--   0 karolszuster   (501) staff       (20)      275 2023-02-22 15:25:18.000000 hdn-research-environment-1.4.0/environment/static/environment/js/pricing_change.js
--rw-r--r--   0 karolszuster   (501) staff       (20)     1658 2022-03-29 08:08:24.000000 hdn-research-environment-1.4.0/environment/tasks.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-02-22 22:00:27.000000 hdn-research-environment-1.4.0/environment/templates/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-02-22 22:00:27.000000 hdn-research-environment-1.4.0/environment/templates/environment/
--rw-r--r--   0 karolszuster   (501) staff       (20)     4511 2023-01-20 14:18:52.000000 hdn-research-environment-1.4.0/environment/templates/environment/_available_environments_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1423 2022-03-29 08:08:24.000000 hdn-research-environment-1.4.0/environment/templates/environment/_available_projects_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)      400 2022-03-29 08:08:24.000000 hdn-research-environment-1.4.0/environment/templates/environment/_cloud_identity_info.html
--rw-r--r--   0 karolszuster   (501) staff       (20)      801 2022-03-30 12:51:12.000000 hdn-research-environment-1.4.0/environment/templates/environment/base_environment_home.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     2193 2022-03-29 08:08:24.000000 hdn-research-environment-1.4.0/environment/templates/environment/billing_setup.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     2970 2023-02-22 22:00:03.000000 hdn-research-environment-1.4.0/environment/templates/environment/create_research_environment.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-02-22 22:00:27.000000 hdn-research-environment-1.4.0/environment/templates/environment/email/
--rw-r--r--   0 karolszuster   (501) staff       (20)      416 2022-03-29 08:08:24.000000 hdn-research-environment-1.4.0/environment/templates/environment/email/environment_access_expired.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1416 2022-03-29 08:08:24.000000 hdn-research-environment-1.4.0/environment/templates/environment/identity_provisioning.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     3866 2022-03-29 08:08:24.000000 hdn-research-environment-1.4.0/environment/templates/environment/research_environments.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1018 2022-03-29 08:08:24.000000 hdn-research-environment-1.4.0/environment/templates/environment/workspace_being_provisioned.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-02-22 22:00:27.000000 hdn-research-environment-1.4.0/environment/templates/tag/
--rw-r--r--   0 karolszuster   (501) staff       (20)      241 2022-03-29 08:08:24.000000 hdn-research-environment-1.4.0/environment/templates/tag/environment_action_button.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1422 2022-03-29 08:08:24.000000 hdn-research-environment-1.4.0/environment/templates/tag/environment_modal_button.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-02-22 22:00:27.000000 hdn-research-environment-1.4.0/environment/templatetags/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-1.4.0/environment/templatetags/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3460 2023-02-22 22:00:03.000000 hdn-research-environment-1.4.0/environment/templatetags/action_buttons.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-02-22 22:00:27.000000 hdn-research-environment-1.4.0/environment/tests/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-1.4.0/environment/tests/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      974 2022-03-29 08:08:24.000000 hdn-research-environment-1.4.0/environment/tests/helpers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    12256 2022-03-29 08:08:24.000000 hdn-research-environment-1.4.0/environment/tests/mocks.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3977 2023-02-22 21:44:22.000000 hdn-research-environment-1.4.0/environment/tests/test_decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    11233 2023-02-22 21:44:22.000000 hdn-research-environment-1.4.0/environment/tests/test_services.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     6444 2023-02-22 21:44:22.000000 hdn-research-environment-1.4.0/environment/tests/test_signals.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3847 2023-02-22 21:44:22.000000 hdn-research-environment-1.4.0/environment/tests/test_utilities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      629 2023-02-22 21:44:22.000000 hdn-research-environment-1.4.0/environment/tests/test_validators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     7755 2023-02-22 21:44:22.000000 hdn-research-environment-1.4.0/environment/tests/test_views.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1474 2022-03-29 08:08:24.000000 hdn-research-environment-1.4.0/environment/urls.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1305 2022-03-29 08:50:55.000000 hdn-research-environment-1.4.0/environment/utilities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      236 2022-03-29 08:08:24.000000 hdn-research-environment-1.4.0/environment/validators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     9871 2023-02-22 22:00:03.000000 hdn-research-environment-1.4.0/environment/views.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-02-22 22:00:27.000000 hdn-research-environment-1.4.0/hdn_research_environment.egg-info/
--rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-02-22 22:00:26.000000 hdn-research-environment-1.4.0/hdn_research_environment.egg-info/PKG-INFO
--rw-r--r--   0 karolszuster   (501) staff       (20)     2573 2023-02-22 22:00:26.000000 hdn-research-environment-1.4.0/hdn_research_environment.egg-info/SOURCES.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)        1 2023-02-22 22:00:26.000000 hdn-research-environment-1.4.0/hdn_research_environment.egg-info/dependency_links.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)       84 2023-02-22 22:00:26.000000 hdn-research-environment-1.4.0/hdn_research_environment.egg-info/requires.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)       12 2023-02-22 22:00:26.000000 hdn-research-environment-1.4.0/hdn_research_environment.egg-info/top_level.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)      109 2022-03-29 08:03:11.000000 hdn-research-environment-1.4.0/pyproject.toml
--rw-r--r--   0 karolszuster   (501) staff       (20)     1056 2023-02-22 22:00:27.000000 hdn-research-environment-1.4.0/setup.cfg
--rw-r--r--   0 karolszuster   (501) staff       (20)       38 2022-03-29 08:03:11.000000 hdn-research-environment-1.4.0/setup.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-12 08:04:18.000000 hdn-research-environment-1.5.0/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1551 2022-03-29 08:15:30.000000 hdn-research-environment-1.5.0/LICENSE
+-rw-r--r--   0 karolszuster   (501) staff       (20)      115 2022-03-29 08:32:41.000000 hdn-research-environment-1.5.0/MANIFEST.in
+-rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-04-12 08:04:18.000000 hdn-research-environment-1.5.0/PKG-INFO
+-rw-r--r--   0 karolszuster   (501) staff       (20)       90 2022-03-29 07:59:09.000000 hdn-research-environment-1.5.0/README.md
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-12 08:04:18.000000 hdn-research-environment-1.5.0/environment/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.0/environment/__init__.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-12 08:04:18.000000 hdn-research-environment-1.5.0/environment/api/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2906 2023-04-12 08:02:22.000000 hdn-research-environment-1.5.0/environment/api/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      749 2023-02-11 18:26:19.000000 hdn-research-environment-1.5.0/environment/api/auth.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      663 2023-02-11 18:26:19.000000 hdn-research-environment-1.5.0/environment/api/decorators.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-12 08:04:18.000000 hdn-research-environment-1.5.0/environment/api/tests/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.0/environment/api/tests/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1403 2023-04-12 08:02:22.000000 hdn-research-environment-1.5.0/environment/api/tests/test_auth.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1554 2023-04-12 08:02:22.000000 hdn-research-environment-1.5.0/environment/api/tests/test_decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      154 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.0/environment/apps.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3050 2023-04-12 08:02:22.000000 hdn-research-environment-1.5.0/environment/constants.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1298 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.0/environment/decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1619 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.0/environment/deserializers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2904 2023-04-12 08:02:22.000000 hdn-research-environment-1.5.0/environment/entities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      547 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.0/environment/exceptions.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2183 2023-04-12 08:02:22.000000 hdn-research-environment-1.5.0/environment/forms.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      155 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.0/environment/managers.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-12 08:04:18.000000 hdn-research-environment-1.5.0/environment/migrations/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1444 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.0/environment/migrations/0001_initial.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1580 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.0/environment/migrations/0002_billingsetup.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      404 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.0/environment/migrations/0003_cloudidentity_is_workspace_done.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      421 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.0/environment/migrations/0004_auto_20220309_0330.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2184 2022-03-29 15:52:24.000000 hdn-research-environment-1.5.0/environment/migrations/0005_workflow.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.0/environment/migrations/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1821 2023-01-20 14:18:52.000000 hdn-research-environment-1.5.0/environment/models.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    14537 2023-04-12 08:02:22.000000 hdn-research-environment-1.5.0/environment/services.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2556 2023-01-20 14:18:52.000000 hdn-research-environment-1.5.0/environment/signals.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-12 08:04:18.000000 hdn-research-environment-1.5.0/environment/static/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-12 08:04:18.000000 hdn-research-environment-1.5.0/environment/static/environment/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-12 08:04:18.000000 hdn-research-environment-1.5.0/environment/static/environment/css/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      342 2023-02-22 22:00:03.000000 hdn-research-environment-1.5.0/environment/static/environment/css/create_research_environment.css
+-rw-r--r--   0 karolszuster   (501) staff       (20)     6583 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.0/environment/static/environment/css/environment-base.css
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-12 08:04:18.000000 hdn-research-environment-1.5.0/environment/static/environment/js/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      564 2022-03-30 12:50:58.000000 hdn-research-environment-1.5.0/environment/static/environment/js/cookie.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3058 2023-04-12 08:02:23.000000 hdn-research-environment-1.5.0/environment/static/environment/js/pricing_change.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1658 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.0/environment/tasks.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-12 08:04:18.000000 hdn-research-environment-1.5.0/environment/templates/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-12 08:04:18.000000 hdn-research-environment-1.5.0/environment/templates/environment/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     4511 2023-01-20 14:18:52.000000 hdn-research-environment-1.5.0/environment/templates/environment/_available_environments_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1423 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.0/environment/templates/environment/_available_projects_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)      400 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.0/environment/templates/environment/_cloud_identity_info.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)      801 2022-03-30 12:51:12.000000 hdn-research-environment-1.5.0/environment/templates/environment/base_environment_home.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2193 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.0/environment/templates/environment/billing_setup.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     4256 2023-04-12 08:02:23.000000 hdn-research-environment-1.5.0/environment/templates/environment/create_research_environment.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-12 08:04:18.000000 hdn-research-environment-1.5.0/environment/templates/environment/email/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      416 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.0/environment/templates/environment/email/environment_access_expired.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1416 2023-04-12 08:02:23.000000 hdn-research-environment-1.5.0/environment/templates/environment/identity_provisioning.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3866 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.0/environment/templates/environment/research_environments.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1018 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.0/environment/templates/environment/workspace_being_provisioned.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-12 08:04:18.000000 hdn-research-environment-1.5.0/environment/templates/tag/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      241 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.0/environment/templates/tag/environment_action_button.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1422 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.0/environment/templates/tag/environment_modal_button.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-12 08:04:18.000000 hdn-research-environment-1.5.0/environment/templatetags/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.0/environment/templatetags/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3460 2023-02-22 22:00:03.000000 hdn-research-environment-1.5.0/environment/templatetags/action_buttons.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-12 08:04:18.000000 hdn-research-environment-1.5.0/environment/tests/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.0/environment/tests/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      974 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.0/environment/tests/helpers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    12256 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.0/environment/tests/mocks.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     4021 2023-04-12 08:02:23.000000 hdn-research-environment-1.5.0/environment/tests/test_decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    11332 2023-04-12 08:02:23.000000 hdn-research-environment-1.5.0/environment/tests/test_services.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     6477 2023-04-12 08:02:23.000000 hdn-research-environment-1.5.0/environment/tests/test_signals.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3891 2023-04-12 08:02:23.000000 hdn-research-environment-1.5.0/environment/tests/test_utilities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-04-12 08:02:23.000000 hdn-research-environment-1.5.0/environment/tests/test_validators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     7799 2023-04-12 08:02:23.000000 hdn-research-environment-1.5.0/environment/tests/test_views.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1474 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.0/environment/urls.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1305 2022-03-29 08:50:55.000000 hdn-research-environment-1.5.0/environment/utilities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      236 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.0/environment/validators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    10196 2023-04-12 08:02:23.000000 hdn-research-environment-1.5.0/environment/views.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-12 08:04:18.000000 hdn-research-environment-1.5.0/hdn_research_environment.egg-info/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-04-12 08:04:18.000000 hdn-research-environment-1.5.0/hdn_research_environment.egg-info/PKG-INFO
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2509 2023-04-12 08:04:18.000000 hdn-research-environment-1.5.0/hdn_research_environment.egg-info/SOURCES.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)        1 2023-04-12 08:04:18.000000 hdn-research-environment-1.5.0/hdn_research_environment.egg-info/dependency_links.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)       84 2023-04-12 08:04:18.000000 hdn-research-environment-1.5.0/hdn_research_environment.egg-info/requires.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)       12 2023-04-12 08:04:18.000000 hdn-research-environment-1.5.0/hdn_research_environment.egg-info/top_level.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)      109 2022-03-29 08:03:11.000000 hdn-research-environment-1.5.0/pyproject.toml
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1056 2023-04-12 08:04:18.000000 hdn-research-environment-1.5.0/setup.cfg
+-rw-r--r--   0 karolszuster   (501) staff       (20)       38 2022-03-29 08:03:11.000000 hdn-research-environment-1.5.0/setup.py
```

### Comparing `hdn-research-environment-1.4.0/LICENSE` & `hdn-research-environment-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.4.0/PKG-INFO` & `hdn-research-environment-1.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: hdn-research-environment
-Version: 1.4.0
+Version: 1.5.0
 Summary: A Django app for supporting cloud-native research environments
 Home-page: https://www.healthdatanexus.ai/
 Author: Your Name
 Author-email: yourname@example.com
 License: BSD-3-Clause  # Example license
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `hdn-research-environment-1.4.0/environment/api/__init__.py` & `hdn-research-environment-1.5.0/environment/api/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -71,24 +71,24 @@
     region: str,
     environment_type: str,
     instance_type: str,
     group_granting_data_access: str,
     persistent_disk: str,
     bucket_name: str,
     vm_image: Optional[str] = None,
-    gpu_accelerated: bool = False,
+    gpu_accelerator: Optional[str] = None,
 ):
     json = {
         "userid": gcp_user_id,
         "region": region,
         "type": environment_type,
         "machinetype": instance_type,
         "group_granting_data_access": group_granting_data_access,
         "bucketname": bucket_name,
         "persistentdisk": persistent_disk,
         "vmimage": vm_image,
-        "gpu_accelerated": gpu_accelerated,
+        "gpu_accelerator": gpu_accelerator,
     }
     json_without_empty_values = {
         key: val for key, val in json.items() if val is not None
     }
     return Request("POST", url="/workbench", json=json_without_empty_values)
```

### Comparing `hdn-research-environment-1.4.0/environment/api/auth.py` & `hdn-research-environment-1.5.0/environment/api/auth.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.4.0/environment/api/decorators.py` & `hdn-research-environment-1.5.0/environment/api/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.4.0/environment/api/tests/test_auth.py` & `hdn-research-environment-1.5.0/environment/api/tests/test_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 from requests import Request
 from google.auth.credentials import Credentials
 from django.test import TestCase
 from django.conf import settings
 from environment.api.auth import apply_api_credentials
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class AuthTestCase(TestCase):
     def test_apply_api_credentials_inserting_correct_headers(self):
         request = Request()
         apply_api_credentials(request)
 
         self.assertIn("authorization", request.headers)
         self.assertRegexpMatches(request.headers["authorization"], r"\ABearer")
```

### Comparing `hdn-research-environment-1.4.0/environment/api/tests/test_decorators.py` & `hdn-research-environment-1.5.0/environment/api/tests/test_decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,18 @@
 
 SAMPLE_BASE_URL = "http://example.com"
 
 
 SAMPLE_ENDPOINT = "/some_path"
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 @override_settings(CLOUD_RESEARCH_ENVIRONMENTS_API_URL=SAMPLE_BASE_URL)
 class DecoratorsTestCase(TestCase):
     def setUp(self):
         session_send_patcher = patch.object(Session, "send")
         self.session_send_mock = session_send_patcher.start()
         self.session_send_mock.return_value = Mock()
```

### Comparing `hdn-research-environment-1.4.0/environment/constants.py` & `hdn-research-environment-1.5.0/environment/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,68 +1,92 @@
 from environment.entities import (
     InstanceType,
     Region,
+    GPUAcceleratorType,
 )
 from collections import namedtuple
 
 MAX_RUNNING_ENVIRONMENTS = 4
 
 MAX_CPU_USAGE = 32
 
 PERSISTENT_DATA_DISK_NAME = "Persistent data disk 1GB"
-PERSISTENT_DATA_DISK_TIME_UNIT = "per Month"
 
-T4_TESLA_GPU_NAME = "NVIDIA T4 Tesla"
-
-ProjectedWorkbenchCost = namedtuple(
-    "ProjectedWorkbenchCost", "resource cost time_unit", defaults=["per Hour"]
-)
-PROJECTED_COSTS = {
+ProjectedWorkbenchCost = namedtuple("ProjectedWorkbenchCost", "resource cost")
+INSTANCE_PROJECTED_COSTS = {
     Region.US_CENTRAL: [
         ProjectedWorkbenchCost(*parameters)
         for parameters in [
             [InstanceType.N1_STANDARD_1.value, 0.05],
             [InstanceType.N1_STANDARD_2.value, 0.09],
             [InstanceType.N1_STANDARD_4.value, 0.19],
             [InstanceType.N1_STANDARD_8.value, 0.38],
             [InstanceType.N1_STANDARD_16.value, 0.76],
-            [T4_TESLA_GPU_NAME, 0.35],
-            [PERSISTENT_DATA_DISK_NAME, 0.05, PERSISTENT_DATA_DISK_TIME_UNIT],
         ]
     ],
     Region.NORTHAMERICA_NORTHEAST: [
         ProjectedWorkbenchCost(*parameters)
         for parameters in [
             [InstanceType.N1_STANDARD_1.value, 0.05],
             [InstanceType.N1_STANDARD_2.value, 0.11],
             [InstanceType.N1_STANDARD_4.value, 0.21],
             [InstanceType.N1_STANDARD_8.value, 0.42],
             [InstanceType.N1_STANDARD_16.value, 0.84],
-            [T4_TESLA_GPU_NAME, 0.35],
-            [PERSISTENT_DATA_DISK_NAME, 0.05, PERSISTENT_DATA_DISK_TIME_UNIT],
         ]
     ],
     Region.EUROPE_WEST: [
         ProjectedWorkbenchCost(*parameters)
         for parameters in [
             [InstanceType.N1_STANDARD_1.value, 0.06],
             [InstanceType.N1_STANDARD_2.value, 0.12],
             [InstanceType.N1_STANDARD_4.value, 0.24],
             [InstanceType.N1_STANDARD_8.value, 0.49],
             [InstanceType.N1_STANDARD_16.value, 0.98],
-            [T4_TESLA_GPU_NAME, 0.41],
-            [PERSISTENT_DATA_DISK_NAME, 0.05, PERSISTENT_DATA_DISK_TIME_UNIT],
         ]
     ],
     Region.AUSTRALIA_SOUTHEAST: [
         ProjectedWorkbenchCost(*parameters)
         for parameters in [
             [InstanceType.N1_STANDARD_1.value, 0.07],
             [InstanceType.N1_STANDARD_2.value, 0.13],
             [InstanceType.N1_STANDARD_4.value, 0.27],
             [InstanceType.N1_STANDARD_8.value, 0.35],
             [InstanceType.N1_STANDARD_16.value, 1.07],
-            [T4_TESLA_GPU_NAME, 0.44],
-            [PERSISTENT_DATA_DISK_NAME, 0.05, PERSISTENT_DATA_DISK_TIME_UNIT],
         ]
     ],
 }
+
+GPU_PROJECTED_COSTS = {
+    Region.US_CENTRAL: [
+        ProjectedWorkbenchCost(*parameters)
+        for parameters in [
+            [GPUAcceleratorType.NVIDIA_TESLA_T4.value, 0.35],
+        ]
+    ],
+    Region.NORTHAMERICA_NORTHEAST: [
+        ProjectedWorkbenchCost(*parameters)
+        for parameters in [
+            [GPUAcceleratorType.NVIDIA_TESLA_T4.value, 0.35],
+        ]
+    ],
+    Region.EUROPE_WEST: [
+        ProjectedWorkbenchCost(*parameters)
+        for parameters in [
+            [GPUAcceleratorType.NVIDIA_TESLA_T4.value, 0.41],
+        ]
+    ],
+    Region.AUSTRALIA_SOUTHEAST: [
+        ProjectedWorkbenchCost(*parameters)
+        for parameters in [
+            [GPUAcceleratorType.NVIDIA_TESLA_T4.value, 0.44],
+        ]
+    ],
+}
+
+DATA_STORAGE_PROJECTED_COSTS = {
+    Region.US_CENTRAL: ProjectedWorkbenchCost(PERSISTENT_DATA_DISK_NAME, 0.05),
+    Region.NORTHAMERICA_NORTHEAST: ProjectedWorkbenchCost(
+        PERSISTENT_DATA_DISK_NAME, 0.05
+    ),
+    Region.EUROPE_WEST: ProjectedWorkbenchCost(PERSISTENT_DATA_DISK_NAME, 0.05),
+    Region.AUSTRALIA_SOUTHEAST: ProjectedWorkbenchCost(PERSISTENT_DATA_DISK_NAME, 0.05),
+}
```

### Comparing `hdn-research-environment-1.4.0/environment/decorators.py` & `hdn-research-environment-1.5.0/environment/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.4.0/environment/deserializers.py` & `hdn-research-environment-1.5.0/environment/deserializers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.4.0/environment/entities.py` & `hdn-research-environment-1.5.0/environment/entities.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,18 @@
             InstanceType.N1_STANDARD_8: 8,
             InstanceType.N1_STANDARD_16: 16,
         }
 
         return INSTANCE_TO_CPU_MAP[self]
 
 
+class GPUAcceleratorType(Enum):
+    NVIDIA_TESLA_T4 = "NVIDIA_TESLA_T4"
+
+
 class EnvironmentStatus(Enum):
     PROVISIONING = "inprogress"
     PROVISIONING_FAILED = "workbench-setup-failed"
 
     RUNNING = "running"
     STARTING = "running-inprogress"
```

### Comparing `hdn-research-environment-1.4.0/environment/exceptions.py` & `hdn-research-environment-1.5.0/environment/exceptions.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.4.0/environment/migrations/0001_initial.py` & `hdn-research-environment-1.5.0/environment/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.4.0/environment/migrations/0002_billingsetup.py` & `hdn-research-environment-1.5.0/environment/migrations/0002_billingsetup.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.4.0/environment/migrations/0005_workflow.py` & `hdn-research-environment-1.5.0/environment/migrations/0005_workflow.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.4.0/environment/models.py` & `hdn-research-environment-1.5.0/environment/models.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.4.0/environment/services.py` & `hdn-research-environment-1.5.0/environment/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 def _create_workbench_kwargs(
     user: User,
     project: PublishedProject,
     region: str,
     instance_type: str,
     environment_type: str,
     persistent_disk: int,
-    gpu_accelerated: bool = False,
+    gpu_accelerator: Optional[str] = None,
 ) -> dict:
     gcp_user_id = user.cloud_identity.gcp_user_id
 
     common = {
         "gcp_user_id": gcp_user_id,
         "region": region,
         "environment_type": environment_type,
@@ -129,43 +129,43 @@
         "group_granting_data_access": _project_data_group(project),
         "persistent_disk": str(persistent_disk),
         "bucket_name": project.project_file_root(),
     }
     if environment_type == "jupyter":
         vm_image = (
             "common-cu110-notebooks"
-            if gpu_accelerated
+            if gpu_accelerator
             else "r-4-2-cpu-experimental-notebooks"
         )
         jupyter_kwargs = {
             "vm_image": vm_image,
-            "gpu_accelerated": gpu_accelerated,
+            "gpu_accelerator": gpu_accelerator,
         }
         return {**common, **jupyter_kwargs}
     else:
         return common
 
 
 def create_research_environment(
     user: User,
     project: PublishedProject,
     region: str,
     instance_type: str,
     environment_type: str,
     persistent_disk: int,
-    gpu_accelerated: bool = False,
+    gpu_accelerator: Optional[str] = None,
 ) -> str:
     kwargs = _create_workbench_kwargs(
         user,
         project,
         region,
         instance_type,
         environment_type,
         persistent_disk,
-        gpu_accelerated,
+        gpu_accelerator,
     )
     response = api.create_workbench(**kwargs)
     if not response.ok:
         error_message = response.json()[
             "error"
         ]  # TODO: Check all uses of "error"/"message"
         raise EnvironmentCreationFailed(error_message)
```

### Comparing `hdn-research-environment-1.4.0/environment/signals.py` & `hdn-research-environment-1.5.0/environment/signals.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.4.0/environment/static/environment/css/environment-base.css` & `hdn-research-environment-1.5.0/environment/static/environment/css/environment-base.css`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.4.0/environment/static/environment/js/cookie.js` & `hdn-research-environment-1.5.0/environment/static/environment/js/cookie.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.4.0/environment/tasks.py` & `hdn-research-environment-1.5.0/environment/tasks.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.4.0/environment/templates/environment/_available_environments_list.html` & `hdn-research-environment-1.5.0/environment/templates/environment/_available_environments_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.4.0/environment/templates/environment/_available_projects_list.html` & `hdn-research-environment-1.5.0/environment/templates/environment/_available_projects_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.4.0/environment/templates/environment/base_environment_home.html` & `hdn-research-environment-1.5.0/environment/templates/environment/base_environment_home.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.4.0/environment/templates/environment/billing_setup.html` & `hdn-research-environment-1.5.0/environment/templates/environment/billing_setup.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.4.0/environment/templates/environment/identity_provisioning.html` & `hdn-research-environment-1.5.0/environment/templates/environment/identity_provisioning.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.4.0/environment/templates/environment/research_environments.html` & `hdn-research-environment-1.5.0/environment/templates/environment/research_environments.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.4.0/environment/templates/environment/workspace_being_provisioned.html` & `hdn-research-environment-1.5.0/environment/templates/environment/workspace_being_provisioned.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.4.0/environment/templates/tag/environment_modal_button.html` & `hdn-research-environment-1.5.0/environment/templates/tag/environment_modal_button.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.4.0/environment/templatetags/action_buttons.py` & `hdn-research-environment-1.5.0/environment/templatetags/action_buttons.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.4.0/environment/tests/helpers.py` & `hdn-research-environment-1.5.0/environment/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.4.0/environment/tests/mocks.py` & `hdn-research-environment-1.5.0/environment/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.4.0/environment/tests/test_decorators.py` & `hdn-research-environment-1.5.0/environment/tests/test_decorators.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,18 @@
     cloud_identity_required,
     billing_setup_required,
     require_PATCH,
     require_DELETE,
 )
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class CloudIdentityRequiredTestCase(TestCase):
     def test_redirects_user_without_cloud_identity_to_identity_provisioning(self):
         request_with_user_without_cloud_identity = Mock(
             user=Mock(spec=[]),
         )
         view = Mock()
         decorated_view = cloud_identity_required(view)
@@ -33,15 +36,18 @@
         )
         view = Mock()
         decorated_view = cloud_identity_required(view)
         decorated_view(request_with_user_without_cloud_identity)
         view.assert_called()
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class BillingSetupRequiredTestCase(TestCase):
     def test_redirects_user_without_billing_account_to_billing_setup(self):
         request_with_user_without_billing_account = Mock(
             user=Mock(spec=[]),
         )
         view = Mock()
         decorated_view = billing_setup_required(view)
@@ -57,15 +63,18 @@
         )
         view = Mock()
         decorated_view = billing_setup_required(view)
         decorated_view(request_with_user_without_billing_account)
         view.assert_called()
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class RequirePatchTestCase(TestCase):
     def test_returns_405_for_non_patch_requests(self):
         methods = [
             "DELETE",
             "GET",
             "POST",
             "HEAD",
@@ -86,15 +95,18 @@
         request = Mock(method="PATCH")
         view = Mock()
         decorated_view = require_PATCH(view)
         decorated_view(request)
         view.assert_called()
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class RequireDeleteTestCase(TestCase):
     def test_returns_405_for_non_delete_requests(self):
         methods = ["PATCH", "GET", "POST", "HEAD", "PUT", "CONNECT", "OPTIONS", "TRACE"]
         responses = []
         for method in methods:
             request = Mock(method=method)
             view = Mock()
```

### Comparing `hdn-research-environment-1.4.0/environment/tests/test_services.py` & `hdn-research-environment-1.5.0/environment/tests/test_services.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,18 @@
 
 PublishedProject = apps.get_model("project", "PublishedProject")
 
 
 User = get_user_model()
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class CreateCloudIdentityTestCase(TestCase):
     def setUp(self):
         self.user = create_user_without_cloud_identity()
 
     @patch("environment.api.create_cloud_identity")
     def test_raises_if_request_fails(self, mock_create_cloud_identity):
         mock_create_cloud_identity.return_value.ok = False
@@ -76,27 +79,33 @@
         otp, identity = create_cloud_identity(self.user)
         self.assertEqual(otp, mock_otp)
         self.assertEqual(identity.gcp_user_id, f"researcher_{self.user.username}")
         self.assertEqual(identity.email, mock_email)
         self.assertEqual(self.user.cloud_identity, identity)
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class CreateBillingSetupTestCase(TestCase):
     def setUp(self):
         self.user = create_user_with_cloud_identity()
 
     def test_creates_billing_setup_for_specified_user(self):
         mock_billing_account = "XXXXXX-XXXXXX-XXXXXX"
         billing_setup = create_billing_setup(self.user, mock_billing_account)
         self.assertEqual(self.user.cloud_identity.billing_setup, billing_setup)
         self.assertEqual(billing_setup.billing_account_id, mock_billing_account)
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class CreateResearchEnvironmentTestCase(TestCase):
     def setUp(self):
         self.project = MagicMock()
         self.project.slug = "slug"
         self.project.get_project_file_root.return_value = "bucket"
         self.user = create_user_with_billing_setup()
 
@@ -124,15 +133,18 @@
             "n1-standard-1",
             "enviornment_type",
             "100",
         )
         self.assertEqual(result, mock_create_workbench.return_value)
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class StopRunningEnvironmentTestCase(TestCase):
     def setUp(self):
         self.user = create_user_with_billing_setup()
 
     @patch("environment.api.stop_workbench")
     def test_raises_if_request_fails(self, mock_stop_workbench):
         mock_stop_workbench.return_value.ok = False
@@ -149,15 +161,18 @@
         mock_stop_workbench.return_value.ok = True
         result = stop_running_environment(
             self.user, "workbench_id", Region.AUSTRALIA_SOUTHEAST
         )
         self.assertEqual(result, mock_stop_workbench.return_value)
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class StartStoppedEnvironmentTestCase(TestCase):
     def setUp(self):
         self.user = create_user_with_billing_setup()
 
     @patch("environment.api.start_workbench")
     def test_raises_if_request_fails(self, mock_start_workbench):
         mock_start_workbench.return_value.ok = False
@@ -174,15 +189,18 @@
         mock_stop_workbench.return_value.ok = True
         result = start_stopped_environment(
             self.user, "workbench_id", Region.AUSTRALIA_SOUTHEAST
         )
         self.assertEqual(result, mock_stop_workbench.return_value)
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class ChangeEnvironmentInstanceTypeTestCase(TestCase):
     def setUp(self):
         self.user = create_user_with_billing_setup()
 
     @patch("environment.api.change_workbench_instance_type")
     def test_raises_if_request_fails(self, mock_change_workbench_instance_type):
         mock_change_workbench_instance_type.return_value.ok = False
@@ -203,15 +221,18 @@
             "workbench_id",
             Region.AUSTRALIA_SOUTHEAST,
             InstanceType.N1_STANDARD_1,
         )
         self.assertEqual(result, mock_change_workbench_instance_type.return_value)
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class DeleteEnvironmentTestCase(TestCase):
     def setUp(self):
         self.user = create_user_with_billing_setup()
 
     @patch("environment.api.delete_workbench")
     def test_raises_if_request_fails(self, mock_delete_workbench):
         mock_delete_workbench.return_value.ok = False
@@ -228,15 +249,18 @@
         mock_delete_workbench.return_value.ok = True
         result = delete_environment(
             self.user, "workbench_id", Region.AUSTRALIA_SOUTHEAST
         )
         self.assertEqual(result, mock_delete_workbench.return_value)
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class VerifyBillingAndCreateWorkspaceTestCase(TestCase):
     def setUp(self):
         self.user = create_user_with_cloud_identity()
         self.some_billing_id = "XXXXXX-XXXXXX-XXXXXX"
 
     @patch("environment.api.create_workspace")
     def test_raises_if_request_fails(self, mock_create_workspace):
@@ -250,15 +274,18 @@
 
     @patch("environment.api.create_workspace")
     def test_not_raises_if_request_succeeds(self, mock_create_workspace):
         mock_create_workspace.return_value.ok = True
         verify_billing_and_create_workspace(self.user, self.some_billing_id)
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class GetAvailableEnvironmentsWithProjectsTestCase(TestCase):
     def setUp(self):
         self.user = create_user_with_cloud_identity()
 
     @patch("environment.api.get_workspace_list")
     def test_fetches_environments_and_parses_to_entity(self, mock_get_workspace_list):
         mock_get_workspace_list.return_value.json.return_value = get_workspace_list_json
```

### Comparing `hdn-research-environment-1.4.0/environment/tests/test_signals.py` & `hdn-research-environment-1.5.0/environment/tests/test_signals.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,18 @@
 from django.test import TestCase
 from django.conf import settings
 from django.utils import timezone
 
 from environment.signals import User, DataAccessRequest, Training
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class UserSignalsTestCase(TestCase):
     def test_memoizes_original_credentialing_on_init(self):
         new_user = User()
         self.assertEqual(new_user._original_is_credentialed, new_user.is_credentialed)
 
     @patch("environment.signals.stop_environments_with_expired_access")
     def test_does_not_schedule_task_on_save_if_user_has_no_billing_setup(
@@ -32,15 +35,18 @@
         mock_user_has_billing_setup.return_value = True
         new_user = User(is_credentialed=True)
         new_user.is_credentialed = False
         new_user.save()
         mock_stop_environments_with_expired_access.assert_called()
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class TrainingSignalsTestCase(TestCase):
     def test_memoizes_original_validity_on_init(self):
         new_user = User()
         new_user.save()
         new_training = Training(user=new_user, training_type_id=1)
         self.assertEqual(new_training._original_is_valid, new_training.is_valid())
 
@@ -67,15 +73,18 @@
         )
         new_training._original_is_valid = False
         new_training.is_valid = lambda: True
         new_training.save()
         mock_stop_environments_with_expired_access.assert_called()
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class DataAccessRequestSignalsTestCase(TestCase):
     def test_memoizes_original_is_accepted_on_init(self):
         new_access_request = DataAccessRequest()
         self.assertEqual(
             new_access_request._original_is_accepted, new_access_request.is_accepted()
         )
```

### Comparing `hdn-research-environment-1.4.0/environment/tests/test_utilities.py` & `hdn-research-environment-1.5.0/environment/tests/test_utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,30 +12,36 @@
     user_has_cloud_identity,
     user_has_billing_setup,
     left_join_iterators,
     inner_join_iterators,
 )
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class UserHasCloudIdentityTestCase(TestCase):
     def setUp(self):
         self.user_without_cloud_identity = create_user_without_cloud_identity()
         self.user_with_cloud_identity = create_user_with_cloud_identity(
             "laa", "loo", "lee"
         )
 
     def test_returns_false_for_user_without_cloud_identity(self):
         self.assertFalse(user_has_cloud_identity(self.user_without_cloud_identity))
 
     def test_returns_true_for_user_with_cloud_identity(self):
         self.assertTrue(user_has_cloud_identity(self.user_with_cloud_identity))
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class UserHasBillingSetupTestCase(TestCase):
     def setUp(self):
         self.user_without_cloud_identity = create_user_without_cloud_identity()
         self.user_with_cloud_identity = create_user_with_cloud_identity(
             "laa", "loo", "lee"
         )
         self.user_with_billing_setup = create_user_with_billing_setup(
@@ -48,15 +54,18 @@
     def test_returns_false_for_user_without_billing_setup(self):
         self.assertFalse(user_has_billing_setup(self.user_with_cloud_identity))
 
     def test_returns_true_for_user_with_billing_setup(self):
         self.assertTrue(user_has_billing_setup(self.user_with_billing_setup))
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class InnerJoinIteratorsTestCase(TestCase):
     def test_returns_lists_left_joined_on_keys(self):
         list1 = [
             {"id": 1, "data": "anything1"},
             {"id": 2, "data": "anything2"},
             {"id": 3, "data": "anything3"},
             {"id": 4, "data": "anything3"},
@@ -72,15 +81,18 @@
         expected_output = [
             (list1[1], list2[1]),
             (list1[2], list2[0]),
         ]
         self.assertEqual(inner_joined, expected_output)
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class LeftJoinIteratorsTestCase(TestCase):
     def test_returns_lists_left_joined_on_keys(self):
         list1 = [
             {"id": 1, "data": "anything1"},
             {"id": 2, "data": "anything2"},
             {"id": 3, "data": "anything3"},
             {"id": 4, "data": "anything3"},
```

### Comparing `hdn-research-environment-1.4.0/environment/tests/test_validators.py` & `hdn-research-environment-1.5.0/environment/tests/test_validators.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 from django.forms import ValidationError
 from django.test import TestCase
 from django.conf import settings
 
 from environment.validators import gcp_billing_account_id_validator
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class BillingAccountValidatorTestCase(TestCase):
     def test_fails_for_invalid_regex(self):
         self.assertRaises(
             ValidationError, gcp_billing_account_id_validator, "some value"
         )
 
     def test_succeeds_for_billing_account_regex(self):
```

### Comparing `hdn-research-environment-1.4.0/environment/tests/test_views.py` & `hdn-research-environment-1.5.0/environment/tests/test_views.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,18 @@
     create_user_without_cloud_identity,
     create_user_with_cloud_identity,
     create_user_with_billing_setup,
 )
 from environment.exceptions import BillingVerificationFailed
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class IdentityProvisioningTestCase(TestCase):
     url = reverse("identity_provisioning")
 
     def test_redirects_to_login_if_not_logged_in(self):
         response = self.client.get(self.url)
         redirect_url = f"{reverse('login')}?next={self.url}"
         self.assertRedirects(response, redirect_url)
@@ -50,15 +53,18 @@
         user = create_user_without_cloud_identity()
         self.client.force_login(user=user)
 
         self.client.post(self.url)
         self.assertEqual(self.client.session["cloud_identity_otp"], otp)
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class BillingSetupTestCase(TestCase):
     url = reverse("billing_setup")
 
     def test_redirects_to_login_if_not_logged_in(self):
         response = self.client.get(self.url)
         redirect_url = f"{reverse('login')}?next={self.url}"
         self.assertRedirects(response, redirect_url)
@@ -123,15 +129,18 @@
         mock_create_billing_setup.assert_called()
         mock_verify_billing_and_create_workspace.assert_called()
         self.assertRedirects(
             response, reverse("research_environments"), fetch_redirect_response=False
         )
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class ResearchEnvironmentsTestCase(TestCase):
     url = reverse("research_environments")
 
     def test_redirects_to_login_if_not_logged_in(self):
         response = self.client.get(self.url)
         redirect_url = f"{reverse('login')}?next={self.url}"
         self.assertRedirects(response, redirect_url)
@@ -162,15 +171,18 @@
 
         response = self.client.get(self.url)
         mock_get_environments_with_projects.assert_called()
         mock_get_available_projects_with_environments.assert_called()
         self.assertEqual(response.status_code, 200)
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class CreateResearchEnvironmentTestCase(TestCase):
     url = reverse(
         "create_research_environment",
         kwargs={"project_slug": "some_slug", "project_version": "some_version"},
     )
 
     def test_redirects_to_login_if_not_logged_in(self):
```

### Comparing `hdn-research-environment-1.4.0/environment/urls.py` & `hdn-research-environment-1.5.0/environment/urls.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.4.0/environment/utilities.py` & `hdn-research-environment-1.5.0/environment/utilities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.4.0/environment/views.py` & `hdn-research-environment-1.5.0/environment/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,17 +71,21 @@
                 return redirect("research_environments")
             except BillingVerificationFailed as err:
                 form.add_error("billing_account_id", err)
     else:
         form = BillingAccountIdForm()
 
     cloud_identity = request.user.cloud_identity
+    session_otp = request.session.get("cloud_identity_otp")
+    one_time_password = session_otp or services.get_user_info(
+        cloud_identity.gcp_user_id
+    ).get("one-time-password")
     context = {
         "email": cloud_identity.email,
-        "otp": request.session.get("cloud_identity_otp"),
+        "otp": one_time_password,
         "form": form,
     }
     return render(request, "environment/billing_setup.html", context)
 
 
 @require_GET
 @login_required
@@ -187,15 +191,15 @@
                 services.create_research_environment(
                     user=request.user,
                     project=project,
                     region=form.cleaned_data["region"],
                     instance_type=form.cleaned_data["instance_type"],
                     environment_type=form.cleaned_data["environment_type"],
                     persistent_disk=form.cleaned_data.get("persistent_disk"),
-                    gpu_accelerated=form.cleaned_data.get("gpu_accelerated"),
+                    gpu_accelerator=form.cleaned_data.get("gpu_accelerator"),
                 )
                 return redirect("research_environments")
             else:
                 messages.error(
                     request,
                     f"Quota exceeded - the specified configuration would use {cpu_usage} out of {constants.MAX_CPU_USAGE} CPUs",
                 )
@@ -203,15 +207,17 @@
         form = CreateResearchEnvironmentForm()
 
     exceeded_quotas = services.exceeded_quotas(request.user)
     context = {
         "form": form,
         "project": project,
         "exceeded_quotas": exceeded_quotas,
-        "projected_costs": constants.PROJECTED_COSTS,
+        "instance_projected_costs": constants.INSTANCE_PROJECTED_COSTS,
+        "gpu_projected_costs": constants.GPU_PROJECTED_COSTS,
+        "data_storage_projected_costs": constants.DATA_STORAGE_PROJECTED_COSTS,
     }
     return render(request, "environment/create_research_environment.html", context)
 
 
 @require_PATCH
 @login_required
 @cloud_identity_required
```

### Comparing `hdn-research-environment-1.4.0/hdn_research_environment.egg-info/PKG-INFO` & `hdn-research-environment-1.5.0/hdn_research_environment.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: hdn-research-environment
-Version: 1.4.0
+Version: 1.5.0
 Summary: A Django app for supporting cloud-native research environments
 Home-page: https://www.healthdatanexus.ai/
 Author: Your Name
 Author-email: yourname@example.com
 License: BSD-3-Clause  # Example license
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `hdn-research-environment-1.4.0/hdn_research_environment.egg-info/SOURCES.txt` & `hdn-research-environment-1.5.0/hdn_research_environment.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 environment/migrations/0003_cloudidentity_is_workspace_done.py
 environment/migrations/0004_auto_20220309_0330.py
 environment/migrations/0005_workflow.py
 environment/migrations/__init__.py
 environment/static/environment/css/create_research_environment.css
 environment/static/environment/css/environment-base.css
 environment/static/environment/js/cookie.js
-environment/static/environment/js/gpu_acceleration_disabling.js
 environment/static/environment/js/pricing_change.js
 environment/templates/environment/_available_environments_list.html
 environment/templates/environment/_available_projects_list.html
 environment/templates/environment/_cloud_identity_info.html
 environment/templates/environment/base_environment_home.html
 environment/templates/environment/billing_setup.html
 environment/templates/environment/create_research_environment.html
```

### Comparing `hdn-research-environment-1.4.0/setup.cfg` & `hdn-research-environment-1.5.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hdn-research-environment
-version = 1.4.0
+version = 1.5.0
 description = A Django app for supporting cloud-native research environments
 long_description = file: README.rst
 url = https://www.healthdatanexus.ai/
 author = Your Name
 author_email = yourname@example.com
 license = BSD-3-Clause  # Example license
 classifiers =
```

