# Comparing `tmp/netbox-secrets-1.7.5.tar.gz` & `tmp/netbox-secrets-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-secrets-1.7.5.tar", last modified: Tue Jan 31 08:47:52 2023, max compression
+gzip compressed data, was "netbox-secrets-1.7.6.tar", last modified: Wed Apr 12 16:45:23 2023, max compression
```

## Comparing `netbox-secrets-1.7.5.tar` & `netbox-secrets-1.7.6.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 08:47:52.225487 netbox-secrets-1.7.5/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-01-31 08:47:52.225487 netbox-secrets-1.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 08:47:52.221487 netbox-secrets-1.7.5/netbox_secrets/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 08:47:52.221487 netbox-secrets-1.7.5/netbox_secrets/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/api/nested_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/filtersets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 08:47:52.221487 netbox-secrets-1.7.5/netbox_secrets/forms/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/forms/secrets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 08:47:52.221487 netbox-secrets-1.7.5/netbox_secrets/graphql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/graphql/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/graphql/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/hashers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 08:47:52.221487 netbox-secrets-1.7.5/netbox_secrets/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/migrations/0002_populate_userkeys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/migrations/0003_populate_secretroles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/migrations/0004_populate_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/migrations/0005_alter_secret_custom_field_data_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/migrations/0006_alter_userkey_created_alter_userkey_last_updated.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 08:47:52.221487 netbox-secrets-1.7.5/netbox_secrets/models/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14959 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/models/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/querysets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 08:47:52.217487 netbox-secrets-1.7.5/netbox_secrets/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 08:47:52.221487 netbox-secrets-1.7.5/netbox_secrets/static/netbox_secrets/
--rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/static/netbox_secrets/secrets.js
--rw-r--r--   0 runner    (1001) docker     (123)    24792 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/static/netbox_secrets/secrets.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 08:47:52.217487 netbox-secrets-1.7.5/netbox_secrets/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 08:47:52.225487 netbox-secrets-1.7.5/netbox_secrets/templates/netbox_secrets/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/templates/netbox_secrets/activate_keys.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 08:47:52.225487 netbox-secrets-1.7.5/netbox_secrets/templates/netbox_secrets/inc/
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/templates/netbox_secrets/inc/private_key_modal.html
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/templates/netbox_secrets/inc/secret_actions.html
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/templates/netbox_secrets/inc/secrets_panel.html
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/templates/netbox_secrets/inc/view_tab.html
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/templates/netbox_secrets/secret.html
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/templates/netbox_secrets/secret_edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/templates/netbox_secrets/secretrole.html
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/templates/netbox_secrets/userkey.html
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/templates/netbox_secrets/userkey_edit.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 08:47:52.225487 netbox-secrets-1.7.5/netbox_secrets/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/tests/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/tests/test_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 08:47:52.225487 netbox-secrets-1.7.5/netbox_secrets/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/utils/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/utils/hashers.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12761 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/netbox_secrets/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 08:47:52.221487 netbox-secrets-1.7.5/netbox_secrets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-01-31 08:47:52.000000 netbox-secrets-1.7.5/netbox_secrets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-01-31 08:47:52.000000 netbox-secrets-1.7.5/netbox_secrets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 08:47:52.000000 netbox-secrets-1.7.5/netbox_secrets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 08:47:52.000000 netbox-secrets-1.7.5/netbox_secrets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-31 08:47:52.000000 netbox-secrets-1.7.5/netbox_secrets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-31 08:47:52.000000 netbox-secrets-1.7.5/netbox_secrets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 08:47:52.225487 netbox-secrets-1.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-01-31 08:47:39.000000 netbox-secrets-1.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:23.445818 netbox-secrets-1.7.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-12 16:45:23.445818 netbox-secrets-1.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:23.437818 netbox-secrets-1.7.6/netbox_secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:23.441818 netbox-secrets-1.7.6/netbox_secrets/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/api/nested_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/filtersets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:23.441818 netbox-secrets-1.7.6/netbox_secrets/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/forms/secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:23.441818 netbox-secrets-1.7.6/netbox_secrets/graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/graphql/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/graphql/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/hashers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:23.441818 netbox-secrets-1.7.6/netbox_secrets/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/migrations/0002_populate_userkeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/migrations/0003_populate_secretroles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/migrations/0004_populate_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/migrations/0005_alter_secret_custom_field_data_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/migrations/0006_alter_userkey_created_alter_userkey_last_updated.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:23.441818 netbox-secrets-1.7.6/netbox_secrets/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14959 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/models/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/querysets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:23.429818 netbox-secrets-1.7.6/netbox_secrets/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:23.441818 netbox-secrets-1.7.6/netbox_secrets/static/netbox_secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/static/netbox_secrets/secrets.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24792 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/static/netbox_secrets/secrets.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:23.433818 netbox-secrets-1.7.6/netbox_secrets/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:23.441818 netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/activate_keys.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:23.445818 netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/inc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/inc/private_key_modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/inc/secret_actions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/inc/secrets_panel.html
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/inc/view_tab.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/secret.html
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/secret_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/secretrole.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/userkey.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/userkey_edit.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:23.445818 netbox-secrets-1.7.6/netbox_secrets/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/tests/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/tests/test_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:23.445818 netbox-secrets-1.7.6/netbox_secrets/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/utils/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/utils/hashers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12761 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:23.437818 netbox-secrets-1.7.6/netbox_secrets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-12 16:45:23.000000 netbox-secrets-1.7.6/netbox_secrets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-12 16:45:23.000000 netbox-secrets-1.7.6/netbox_secrets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:45:23.000000 netbox-secrets-1.7.6/netbox_secrets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:45:23.000000 netbox-secrets-1.7.6/netbox_secrets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-12 16:45:23.000000 netbox-secrets-1.7.6/netbox_secrets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 16:45:23.000000 netbox-secrets-1.7.6/netbox_secrets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 16:45:23.445818 netbox-secrets-1.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/setup.py
```

### Comparing `netbox-secrets-1.7.5/LICENSE.md` & `netbox-secrets-1.7.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/README.md` & `netbox-secrets-1.7.6/README.md`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/__init__.py` & `netbox-secrets-1.7.6/netbox_secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/admin.py` & `netbox-secrets-1.7.6/netbox_secrets/admin.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/api/nested_serializers.py` & `netbox-secrets-1.7.6/netbox_secrets/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/api/serializers.py` & `netbox-secrets-1.7.6/netbox_secrets/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/api/urls.py` & `netbox-secrets-1.7.6/netbox_secrets/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/api/views.py` & `netbox-secrets-1.7.6/netbox_secrets/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/filtersets.py` & `netbox-secrets-1.7.6/netbox_secrets/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/forms/secrets.py` & `netbox-secrets-1.7.6/netbox_secrets/forms/secrets.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/migrations/0001_initial.py` & `netbox-secrets-1.7.6/netbox_secrets/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/migrations/0002_populate_userkeys.py` & `netbox-secrets-1.7.6/netbox_secrets/migrations/0002_populate_userkeys.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/migrations/0003_populate_secretroles.py` & `netbox-secrets-1.7.6/netbox_secrets/migrations/0003_populate_secretroles.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/migrations/0005_alter_secret_custom_field_data_and_more.py` & `netbox-secrets-1.7.6/netbox_secrets/migrations/0005_alter_secret_custom_field_data_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/migrations/0006_alter_userkey_created_alter_userkey_last_updated.py` & `netbox-secrets-1.7.6/netbox_secrets/migrations/0006_alter_userkey_created_alter_userkey_last_updated.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/models/secrets.py` & `netbox-secrets-1.7.6/netbox_secrets/models/secrets.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/navigation.py` & `netbox-secrets-1.7.6/netbox_secrets/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/static/netbox_secrets/secrets.js` & `netbox-secrets-1.7.6/netbox_secrets/static/netbox_secrets/secrets.js`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/static/netbox_secrets/secrets.js.map` & `netbox-secrets-1.7.6/netbox_secrets/static/netbox_secrets/secrets.js.map`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/tables.py` & `netbox-secrets-1.7.6/netbox_secrets/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/template_content.py` & `netbox-secrets-1.7.6/netbox_secrets/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/templates/netbox_secrets/inc/private_key_modal.html` & `netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/inc/private_key_modal.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/templates/netbox_secrets/inc/secret_actions.html` & `netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/inc/secret_actions.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/templates/netbox_secrets/inc/secrets_panel.html` & `netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/inc/secrets_panel.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/templates/netbox_secrets/inc/view_tab.html` & `netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/inc/view_tab.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/templates/netbox_secrets/secret.html` & `netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/secret.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/templates/netbox_secrets/secret_edit.html` & `netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/secret_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/templates/netbox_secrets/secretrole.html` & `netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/secretrole.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/templates/netbox_secrets/userkey.html` & `netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/userkey.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/templates/netbox_secrets/userkey_edit.html` & `netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/userkey_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/tests/constants.py` & `netbox-secrets-1.7.6/netbox_secrets/tests/constants.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/tests/test_api.py` & `netbox-secrets-1.7.6/netbox_secrets/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/tests/test_filters.py` & `netbox-secrets-1.7.6/netbox_secrets/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/tests/test_form.py` & `netbox-secrets-1.7.6/netbox_secrets/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/tests/test_models.py` & `netbox-secrets-1.7.6/netbox_secrets/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/tests/test_views.py` & `netbox-secrets-1.7.6/netbox_secrets/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/urls.py` & `netbox-secrets-1.7.6/netbox_secrets/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/utils/crypto.py` & `netbox-secrets-1.7.6/netbox_secrets/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets/views.py` & `netbox-secrets-1.7.6/netbox_secrets/views.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/netbox_secrets.egg-info/SOURCES.txt` & `netbox-secrets-1.7.6/netbox_secrets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.5/setup.py` & `netbox-secrets-1.7.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='netbox-secrets',
-    version='1.7.5',
+    version='1.7.6',
     description='Netbox Secrets',
     long_description='A Secret store for NetBox',
     url='https://github.com/Onemind-Services-LLC/netbox-secrets/',
     author='Daniel Sheppard',
     author_email='dans@dansheps.com',
     license='Apache 2.0',
     install_requires=[
```

