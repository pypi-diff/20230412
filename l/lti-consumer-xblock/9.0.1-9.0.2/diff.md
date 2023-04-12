# Comparing `tmp/lti-consumer-xblock-9.0.1.tar.gz` & `tmp/lti-consumer-xblock-9.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lti-consumer-xblock-9.0.1.tar", last modified: Tue Apr 11 14:25:01 2023, max compression
+gzip compressed data, was "lti-consumer-xblock-9.0.2.tar", last modified: Wed Apr 12 16:57:11 2023, max compression
```

## Comparing `lti-consumer-xblock-9.0.1.tar` & `lti-consumer-xblock-9.0.2.tar`

### file list

```diff
@@ -1,213 +1,213 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.502351 lti-consumer-xblock-9.0.1/
--rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (122)    14196 2023-04-11 14:25:01.502351 lti-consumer-xblock-9.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    13412 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.478351 lti-consumer-xblock-9.0.1/lti_consumer/
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)    11820 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      672 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     5845 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/data.py
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)      666 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.482351 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14958 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.482351 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/contrib/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5551 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/contrib/django.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.482351 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/contrib/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/contrib/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6923 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/contrib/tests/test_django.py
--rw-r--r--   0 runner    (1001) docker     (122)      143 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     5976 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/oauth.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.482351 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13817 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/tests/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3674 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/tests/test_oauth.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.482351 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/ags.py
--rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    32216 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/deep_linking.py
--rw-r--r--   0 runner    (1001) docker     (122)     1996 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.482351 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/extensions/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.482351 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/extensions/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/extensions/rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3499 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)      388 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/extensions/rest_framework/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      554 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py
--rw-r--r--   0 runner    (1001) docker     (122)     3298 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1759 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py
--rw-r--r--   0 runner    (1001) docker     (122)    14353 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)      775 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/extensions/rest_framework/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     7491 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/key_handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/nprs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.486351 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.486351 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/extensions/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.486351 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/extensions/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/extensions/rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4234 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)     9039 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/test_ags.py
--rw-r--r--   0 runner    (1001) docker     (122)    39510 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/test_deep_linking.py
--rw-r--r--   0 runner    (1001) docker     (122)     9305 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/test_key_handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/test_nrps.py
--rw-r--r--   0 runner    (1001) docker     (122)      226 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    69931 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/lti_xblock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.490351 lti-consumer-xblock-9.0.1/lti_consumer/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)      940 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/migrations/0002_ltiagslineitem.py
--rw-r--r--   0 runner    (1001) docker     (122)     1677 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/migrations/0003_ltiagsscore.py
--rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/migrations/0004_keyset_mgmt_to_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/migrations/0005_migrate_keyset_to_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py
--rw-r--r--   0 runner    (1001) docker     (122)     1105 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/migrations/0007_ltidlcontentitem.py
--rw-r--r--   0 runner    (1001) docker     (122)      924 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/migrations/0008_fix_uuid_backfill.py
--rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/migrations/0009_backfill-empty-string-config-id.py
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py
--rw-r--r--   0 runner    (1001) docker     (122)      496 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/migrations/0012_rename_courseeditltifieldsenabledflag_model.py
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/migrations/0013_auto_20210712_1352.py
--rw-r--r--   0 runner    (1001) docker     (122)      821 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/migrations/0014_adds_external_id.py
--rw-r--r--   0 runner    (1001) docker     (122)     3641 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/migrations/0015_add_additional_1p3_fields.py
--rw-r--r--   0 runner    (1001) docker     (122)      521 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py
--rw-r--r--   0 runner    (1001) docker     (122)      844 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    32021 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     8078 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/outcomes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.490351 lti-consumer-xblock-9.0.1/lti_consumer/plugin/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11681 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/plugin/compat.py
--rw-r--r--   0 runner    (1001) docker     (122)     2404 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/plugin/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)    35136 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/plugin/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.490351 lti-consumer-xblock-9.0.1/lti_consumer/signals/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3800 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/signals/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.474351 lti-consumer-xblock-9.0.1/lti_consumer/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.490351 lti-consumer-xblock-9.0.1/lti_consumer/static/css/
--rw-r--r--   0 runner    (1001) docker     (122)     4091 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/static/css/student.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.490351 lti-consumer-xblock-9.0.1/lti_consumer/static/js/
--rw-r--r--   0 runner    (1001) docker     (122)    10549 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/static/js/xblock_lti_consumer.js
--rw-r--r--   0 runner    (1001) docker     (122)     6043 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/static/js/xblock_studio_view.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.490351 lti-consumer-xblock-9.0.1/lti_consumer/static/sass/
--rw-r--r--   0 runner    (1001) docker     (122)     4751 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/static/sass/student.scss
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.474351 lti-consumer-xblock-9.0.1/lti_consumer/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.490351 lti-consumer-xblock-9.0.1/lti_consumer/templates/html/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.490351 lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti-dl/
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti-dl/dl_response_error.html
--rw-r--r--   0 runner    (1001) docker     (122)      434 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti-dl/dl_response_saved.html
--rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti-dl/render_dl_content.html
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti-dl/render_html.html
--rw-r--r--   0 runner    (1001) docker     (122)      890 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti-dl/render_image.html
--rw-r--r--   0 runner    (1001) docker     (122)      709 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti-dl/render_link.html
--rw-r--r--   0 runner    (1001) docker     (122)      355 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti-dl/render_lti_resource_link.html
--rw-r--r--   0 runner    (1001) docker     (122)      893 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti_1p3_launch.html
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti_1p3_permission_error.html
--rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti_1p3_studio.html
--rw-r--r--   0 runner    (1001) docker     (122)      364 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti_iframe.html
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti_launch.html
--rw-r--r--   0 runner    (1001) docker     (122)      429 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti_launch_error.html
--rw-r--r--   0 runner    (1001) docker     (122)      445 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti_proctoring_start_error.html
--rw-r--r--   0 runner    (1001) docker     (122)     3849 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templates/html/student.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.494351 lti-consumer-xblock-9.0.1/lti_consumer/templates/xml/
--rw-r--r--   0 runner    (1001) docker     (122)      798 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templates/xml/outcome_service_response.xml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.494351 lti-consumer-xblock-9.0.1/lti_consumer/templatetags/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      780 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templatetags/get_dl_lti_launch_url.py
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/templatetags/lti_sanitize.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.494351 lti-consumer-xblock-9.0.1/lti_consumer/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2807 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.494351 lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.494351 lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/plugin/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11288 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/plugin/test_proctoring.py
--rw-r--r--   0 runner    (1001) docker     (122)    25574 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/plugin/test_views.py
--rw-r--r--   0 runner    (1001) docker     (122)    38579 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/plugin/test_views_lti_ags.py
--rw-r--r--   0 runner    (1001) docker     (122)    26203 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py
--rw-r--r--   0 runner    (1001) docker     (122)    10559 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py
--rw-r--r--   0 runner    (1001) docker     (122)    26379 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     2866 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)    82946 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/test_lti_xblock.py
--rw-r--r--   0 runner    (1001) docker     (122)    24054 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)    16718 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/test_outcomes.py
--rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (122)     4743 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      366 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/track.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.494351 lti-consumer-xblock-9.0.1/lti_consumer/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.474351 lti-consumer-xblock-9.0.1/lti_consumer/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.494351 lti-consumer-xblock-9.0.1/lti_consumer/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    10720 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/ar/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    20385 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/ar/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.474351 lti-consumer-xblock-9.0.1/lti_consumer/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.498351 lti-consumer-xblock-9.0.1/lti_consumer/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      380 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/en/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    14641 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/en/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.474351 lti-consumer-xblock-9.0.1/lti_consumer/translations/es_419/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.498351 lti-consumer-xblock-9.0.1/lti_consumer/translations/es_419/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9197 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/es_419/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    24997 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/es_419/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.474351 lti-consumer-xblock-9.0.1/lti_consumer/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.498351 lti-consumer-xblock-9.0.1/lti_consumer/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1404 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/fr/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    24275 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/fr/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.474351 lti-consumer-xblock-9.0.1/lti_consumer/translations/fr_CA/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.498351 lti-consumer-xblock-9.0.1/lti_consumer/translations/fr_CA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9166 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10186 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.474351 lti-consumer-xblock-9.0.1/lti_consumer/translations/he/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.498351 lti-consumer-xblock-9.0.1/lti_consumer/translations/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    10080 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/he/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    19741 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/he/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.474351 lti-consumer-xblock-9.0.1/lti_consumer/translations/hi/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.498351 lti-consumer-xblock-9.0.1/lti_consumer/translations/hi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      461 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/hi/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    14649 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/hi/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.474351 lti-consumer-xblock-9.0.1/lti_consumer/translations/ja_JP/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.498351 lti-consumer-xblock-9.0.1/lti_consumer/translations/ja_JP/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9838 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10907 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.474351 lti-consumer-xblock-9.0.1/lti_consumer/translations/ko_KR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.498351 lti-consumer-xblock-9.0.1/lti_consumer/translations/ko_KR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      469 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/ko_KR/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    14719 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.474351 lti-consumer-xblock-9.0.1/lti_consumer/translations/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.498351 lti-consumer-xblock-9.0.1/lti_consumer/translations/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1349 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    15126 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.474351 lti-consumer-xblock-9.0.1/lti_consumer/translations/pt_PT/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.498351 lti-consumer-xblock-9.0.1/lti_consumer/translations/pt_PT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    10221 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    18852 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.478351 lti-consumer-xblock-9.0.1/lti_consumer/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.498351 lti-consumer-xblock-9.0.1/lti_consumer/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      601 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/ru/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    14789 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/ru/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.478351 lti-consumer-xblock-9.0.1/lti_consumer/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.498351 lti-consumer-xblock-9.0.1/lti_consumer/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      495 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/zh_CN/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    14700 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)    10931 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/lti_consumer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.502351 lti-consumer-xblock-9.0.1/lti_consumer_xblock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14196 2023-04-11 14:25:01.000000 lti-consumer-xblock-9.0.1/lti_consumer_xblock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6826 2023-04-11 14:25:01.000000 lti-consumer-xblock-9.0.1/lti_consumer_xblock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)      106 2023-04-11 14:25:01.000000 lti-consumer-xblock-9.0.1/lti_consumer_xblock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      199 2023-04-11 14:25:01.000000 lti-consumer-xblock-9.0.1/lti_consumer_xblock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      171 2023-04-11 14:25:01.000000 lti-consumer-xblock-9.0.1/lti_consumer_xblock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-11 14:25:01.000000 lti-consumer-xblock-9.0.1/lti_consumer_xblock.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 14:25:01.502351 lti-consumer-xblock-9.0.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      493 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-04-11 14:25:01.502351 lti-consumer-xblock-9.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5875 2023-04-11 14:24:58.000000 lti-consumer-xblock-9.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.896233 lti-consumer-xblock-9.0.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)    14196 2023-04-12 16:57:11.896233 lti-consumer-xblock-9.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    13412 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.840233 lti-consumer-xblock-9.0.2/lti_consumer/
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11820 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      672 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5845 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)      666 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.844233 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14958 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.844233 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/contrib/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5551 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/contrib/django.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.844233 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/contrib/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/contrib/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6923 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/contrib/tests/test_django.py
+-rw-r--r--   0 runner    (1001) docker     (122)      143 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5976 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/oauth.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.844233 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13817 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/tests/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3674 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/tests/test_oauth.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.848233 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/ags.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32216 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/deep_linking.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1996 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.848233 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/extensions/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.848233 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/extensions/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/extensions/rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3499 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)      388 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/extensions/rest_framework/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      554 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3298 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1759 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14353 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/extensions/rest_framework/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7491 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/key_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/nprs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.852233 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.852233 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/extensions/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.852233 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/extensions/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/extensions/rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4234 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9039 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/test_ags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39510 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/test_deep_linking.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9305 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/test_key_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/test_nrps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    69931 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_xblock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.864233 lti-consumer-xblock-9.0.2/lti_consumer/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)      940 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/migrations/0002_ltiagslineitem.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1677 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/migrations/0003_ltiagsscore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/migrations/0004_keyset_mgmt_to_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/migrations/0005_migrate_keyset_to_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1105 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/migrations/0007_ltidlcontentitem.py
+-rw-r--r--   0 runner    (1001) docker     (122)      924 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/migrations/0008_fix_uuid_backfill.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/migrations/0009_backfill-empty-string-config-id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py
+-rw-r--r--   0 runner    (1001) docker     (122)      496 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/migrations/0012_rename_courseeditltifieldsenabledflag_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/migrations/0013_auto_20210712_1352.py
+-rw-r--r--   0 runner    (1001) docker     (122)      821 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/migrations/0014_adds_external_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3641 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/migrations/0015_add_additional_1p3_fields.py
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py
+-rw-r--r--   0 runner    (1001) docker     (122)      844 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32021 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8078 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/outcomes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.864233 lti-consumer-xblock-9.0.2/lti_consumer/plugin/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11681 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/plugin/compat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2404 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/plugin/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35136 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/plugin/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.868233 lti-consumer-xblock-9.0.2/lti_consumer/signals/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3800 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/signals/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.832233 lti-consumer-xblock-9.0.2/lti_consumer/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.868233 lti-consumer-xblock-9.0.2/lti_consumer/static/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     4091 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/static/css/student.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.868233 lti-consumer-xblock-9.0.2/lti_consumer/static/js/
+-rw-r--r--   0 runner    (1001) docker     (122)    10596 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/static/js/xblock_lti_consumer.js
+-rw-r--r--   0 runner    (1001) docker     (122)     6043 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/static/js/xblock_studio_view.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.868233 lti-consumer-xblock-9.0.2/lti_consumer/static/sass/
+-rw-r--r--   0 runner    (1001) docker     (122)     4751 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/static/sass/student.scss
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.832233 lti-consumer-xblock-9.0.2/lti_consumer/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.868233 lti-consumer-xblock-9.0.2/lti_consumer/templates/html/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.876233 lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti-dl/
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti-dl/dl_response_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)      434 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti-dl/dl_response_saved.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti-dl/render_dl_content.html
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti-dl/render_html.html
+-rw-r--r--   0 runner    (1001) docker     (122)      890 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti-dl/render_image.html
+-rw-r--r--   0 runner    (1001) docker     (122)      709 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti-dl/render_link.html
+-rw-r--r--   0 runner    (1001) docker     (122)      355 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti-dl/render_lti_resource_link.html
+-rw-r--r--   0 runner    (1001) docker     (122)      893 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti_1p3_launch.html
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti_1p3_permission_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti_1p3_studio.html
+-rw-r--r--   0 runner    (1001) docker     (122)      364 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti_iframe.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti_launch.html
+-rw-r--r--   0 runner    (1001) docker     (122)      429 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti_launch_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)      445 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti_proctoring_start_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3849 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templates/html/student.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.876233 lti-consumer-xblock-9.0.2/lti_consumer/templates/xml/
+-rw-r--r--   0 runner    (1001) docker     (122)      798 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templates/xml/outcome_service_response.xml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.876233 lti-consumer-xblock-9.0.2/lti_consumer/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      780 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templatetags/get_dl_lti_launch_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templatetags/lti_sanitize.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.876233 lti-consumer-xblock-9.0.2/lti_consumer/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2807 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.880233 lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.880233 lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/plugin/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11288 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/plugin/test_proctoring.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25574 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/plugin/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38579 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/plugin/test_views_lti_ags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26203 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10559 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26379 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2866 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    82946 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/test_lti_xblock.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24054 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16718 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/test_outcomes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4743 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      366 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/track.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.880233 lti-consumer-xblock-9.0.2/lti_consumer/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.832233 lti-consumer-xblock-9.0.2/lti_consumer/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.880233 lti-consumer-xblock-9.0.2/lti_consumer/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    10720 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/ar/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    22143 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/ar/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.832233 lti-consumer-xblock-9.0.2/lti_consumer/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.880233 lti-consumer-xblock-9.0.2/lti_consumer/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      380 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/en/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16396 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/en/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.832233 lti-consumer-xblock-9.0.2/lti_consumer/translations/es_419/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.880233 lti-consumer-xblock-9.0.2/lti_consumer/translations/es_419/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     9197 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/es_419/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26467 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/es_419/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.832233 lti-consumer-xblock-9.0.2/lti_consumer/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.884233 lti-consumer-xblock-9.0.2/lti_consumer/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1404 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/fr/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    25340 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/fr/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.836233 lti-consumer-xblock-9.0.2/lti_consumer/translations/fr_CA/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.884233 lti-consumer-xblock-9.0.2/lti_consumer/translations/fr_CA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     9166 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10186 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.836233 lti-consumer-xblock-9.0.2/lti_consumer/translations/he/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.884233 lti-consumer-xblock-9.0.2/lti_consumer/translations/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    10080 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/he/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    21499 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/he/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.836233 lti-consumer-xblock-9.0.2/lti_consumer/translations/hi/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.884233 lti-consumer-xblock-9.0.2/lti_consumer/translations/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      461 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/hi/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16407 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/hi/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.836233 lti-consumer-xblock-9.0.2/lti_consumer/translations/ja_JP/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.888233 lti-consumer-xblock-9.0.2/lti_consumer/translations/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     9838 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10907 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.836233 lti-consumer-xblock-9.0.2/lti_consumer/translations/ko_KR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.888233 lti-consumer-xblock-9.0.2/lti_consumer/translations/ko_KR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      469 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/ko_KR/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16477 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.836233 lti-consumer-xblock-9.0.2/lti_consumer/translations/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.888233 lti-consumer-xblock-9.0.2/lti_consumer/translations/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1349 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16884 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.836233 lti-consumer-xblock-9.0.2/lti_consumer/translations/pt_PT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.888233 lti-consumer-xblock-9.0.2/lti_consumer/translations/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    10221 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18852 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.836233 lti-consumer-xblock-9.0.2/lti_consumer/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.892233 lti-consumer-xblock-9.0.2/lti_consumer/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      601 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/ru/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16547 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/ru/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.836233 lti-consumer-xblock-9.0.2/lti_consumer/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.892233 lti-consumer-xblock-9.0.2/lti_consumer/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      495 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/zh_CN/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16458 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)    10931 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.892233 lti-consumer-xblock-9.0.2/lti_consumer_xblock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14196 2023-04-12 16:57:11.000000 lti-consumer-xblock-9.0.2/lti_consumer_xblock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6826 2023-04-12 16:57:11.000000 lti-consumer-xblock-9.0.2/lti_consumer_xblock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-04-12 16:57:11.000000 lti-consumer-xblock-9.0.2/lti_consumer_xblock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      199 2023-04-12 16:57:11.000000 lti-consumer-xblock-9.0.2/lti_consumer_xblock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      171 2023-04-12 16:57:11.000000 lti-consumer-xblock-9.0.2/lti_consumer_xblock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-12 16:57:11.000000 lti-consumer-xblock-9.0.2/lti_consumer_xblock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.896233 lti-consumer-xblock-9.0.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-04-12 16:57:11.896233 lti-consumer-xblock-9.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5875 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/setup.py
```

### Comparing `lti-consumer-xblock-9.0.1/LICENSE` & `lti-consumer-xblock-9.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/NOTICE` & `lti-consumer-xblock-9.0.2/NOTICE`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/PKG-INFO` & `lti-consumer-xblock-9.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lti-consumer-xblock
-Version: 9.0.1
+Version: 9.0.2
 Summary: This XBlock implements the consumer side of the LTI specification.
 Home-page: https://github.com/openedx/xblock-lti-consumer
 Author: Open edX project
 Author-email: oscm@edx.org
 Keywords: lti consumer xblock
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
```

### Comparing `lti-consumer-xblock-9.0.1/README.rst` & `lti-consumer-xblock-9.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/admin.py` & `lti-consumer-xblock-9.0.2/lti_consumer/admin.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/api.py` & `lti-consumer-xblock-9.0.2/lti_consumer/api.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/apps.py` & `lti-consumer-xblock-9.0.2/lti_consumer/apps.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/data.py` & `lti-consumer-xblock-9.0.2/lti_consumer/data.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/filters.py` & `lti-consumer-xblock-9.0.2/lti_consumer/filters.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/forms.py` & `lti-consumer-xblock-9.0.2/lti_consumer/forms.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/consumer.py` & `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/consumer.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/contrib/django.py` & `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/contrib/django.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/contrib/tests/test_django.py` & `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/contrib/tests/test_django.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/oauth.py` & `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/oauth.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/tests/test_consumer.py` & `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p1/tests/test_oauth.py` & `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/tests/test_oauth.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/ags.py` & `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/ags.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/constants.py` & `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/constants.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/consumer.py` & `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/consumer.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/deep_linking.py` & `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/deep_linking.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/exceptions.py` & `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/exceptions.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py` & `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py` & `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py` & `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py` & `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py` & `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/extensions/rest_framework/utils.py` & `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/extensions/rest_framework/utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/key_handlers.py` & `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/key_handlers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/nprs.py` & `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/nprs.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py` & `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py` & `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/test_ags.py` & `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/test_ags.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/test_consumer.py` & `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/test_deep_linking.py` & `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/test_deep_linking.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/test_key_handlers.py` & `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/test_key_handlers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/lti_1p3/tests/test_nrps.py` & `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/test_nrps.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/lti_xblock.py` & `lti-consumer-xblock-9.0.2/lti_consumer/lti_xblock.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/migrations/0001_initial.py` & `lti-consumer-xblock-9.0.2/lti_consumer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/migrations/0002_ltiagslineitem.py` & `lti-consumer-xblock-9.0.2/lti_consumer/migrations/0002_ltiagslineitem.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/migrations/0003_ltiagsscore.py` & `lti-consumer-xblock-9.0.2/lti_consumer/migrations/0003_ltiagsscore.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/migrations/0004_keyset_mgmt_to_model.py` & `lti-consumer-xblock-9.0.2/lti_consumer/migrations/0004_keyset_mgmt_to_model.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/migrations/0005_migrate_keyset_to_model.py` & `lti-consumer-xblock-9.0.2/lti_consumer/migrations/0005_migrate_keyset_to_model.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py` & `lti-consumer-xblock-9.0.2/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/migrations/0007_ltidlcontentitem.py` & `lti-consumer-xblock-9.0.2/lti_consumer/migrations/0007_ltidlcontentitem.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/migrations/0008_fix_uuid_backfill.py` & `lti-consumer-xblock-9.0.2/lti_consumer/migrations/0008_fix_uuid_backfill.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/migrations/0009_backfill-empty-string-config-id.py` & `lti-consumer-xblock-9.0.2/lti_consumer/migrations/0009_backfill-empty-string-config-id.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py` & `lti-consumer-xblock-9.0.2/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py` & `lti-consumer-xblock-9.0.2/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/migrations/0013_auto_20210712_1352.py` & `lti-consumer-xblock-9.0.2/lti_consumer/migrations/0013_auto_20210712_1352.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/migrations/0014_adds_external_id.py` & `lti-consumer-xblock-9.0.2/lti_consumer/migrations/0014_adds_external_id.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/migrations/0015_add_additional_1p3_fields.py` & `lti-consumer-xblock-9.0.2/lti_consumer/migrations/0015_add_additional_1p3_fields.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py` & `lti-consumer-xblock-9.0.2/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py` & `lti-consumer-xblock-9.0.2/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/models.py` & `lti-consumer-xblock-9.0.2/lti_consumer/models.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/outcomes.py` & `lti-consumer-xblock-9.0.2/lti_consumer/outcomes.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/plugin/compat.py` & `lti-consumer-xblock-9.0.2/lti_consumer/plugin/compat.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/plugin/urls.py` & `lti-consumer-xblock-9.0.2/lti_consumer/plugin/urls.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/plugin/views.py` & `lti-consumer-xblock-9.0.2/lti_consumer/plugin/views.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/signals/signals.py` & `lti-consumer-xblock-9.0.2/lti_consumer/signals/signals.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/static/css/student.css` & `lti-consumer-xblock-9.0.2/lti_consumer/static/css/student.css`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/static/js/xblock_lti_consumer.js` & `lti-consumer-xblock-9.0.2/lti_consumer/static/js/xblock_lti_consumer.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -128,17 +128,17 @@
             $('<div id="' + dialog_container_id + '"></div>').insertAfter(triggerElement) // TODO: this will need some cute styling. It looks like trash but it works.
                 .append('<p>' + message + '</p>')
 
             var $dialog_container = $("#" + dialog_container_id);
 
             if (showCancelButton) {
                 $dialog_container
-                    .append('<button style="margin-right:1rem" id="cancel-button">Cancel</button>');
+                    .append('<button style="margin-right:1rem" id="cancel-button">' + gettext("Cancel") + '</button>');
             }
-            $dialog_container.append('<button id="confirm-button">OK</button>');
+            $dialog_container.append('<button id="confirm-button">' + gettext('OK') + '</button>');
 
             // When a learner clicks "OK" or "Cancel" in the consent dialog, remove the consent dialog, show the launch
             // button, and resolve the promise.
             $dialog_container.find('#confirm-button').click(function() {
                 // Show the button that triggered the event, i.e. the launch button.
                 triggerElement.show();
                 $dialog_container.remove()
@@ -159,29 +159,28 @@
         var $ltiContainer = $element.find('.lti-consumer-container');
         var askToSendUsername = $ltiContainer.data('ask-to-send-username') == 'True';
         var askToSendEmail = $ltiContainer.data('ask-to-send-email') == 'True';
         var ltiVersion = $ltiContainer.data('lti-version');
 
         function renderPIIConsentPromptIfRequired(onSuccess, showCancelButton = true) {
             if (askToSendUsername && askToSendEmail) {
-                msg = "Click OK to have your username and e-mail address sent to a 3rd party application.";
+                msg = gettext('Click OK to have your username and e-mail address sent to a 3rd party application.');
             } else if (askToSendUsername) {
-                msg = "Click OK to have your username sent to a 3rd party application.";
+                msg = gettext('Click OK to have your username sent to a 3rd party application.');
             } else if (askToSendEmail) {
-                msg = "Click OK to have your e-mail address sent to a 3rd party application.";
+                msg = gettext('Click OK to have your e-mail address sent to a 3rd party application.');
             } else {
-                onSuccess("OK");
+                onSuccess('OK');
                 return;
             }
 
             if (showCancelButton) {
-                msg += "\n\nClick Cancel to return to this page without sending your information.";
+                msg += '\n\n' + gettext('Click Cancel to return to this page without sending your information.');
             }
 
-            msg = gettext(msg);
             $.when(confirmDialog(msg, $(this), showCancelButton)).then(onSuccess);
         }
 
         // Render consent dialog for inline elements immediately.
         var $ltiIframeContainerElement = $element.find('#lti-iframe-container');
         $ltiIframeContainerElement.each(function() {
             var ltiIframeTarget = $ltiIframeContainerElement.data('target')
```

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/static/js/xblock_studio_view.js` & `lti-consumer-xblock-9.0.2/lti_consumer/static/js/xblock_studio_view.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/static/sass/student.scss` & `lti-consumer-xblock-9.0.2/lti_consumer/static/sass/student.scss`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti-dl/render_dl_content.html` & `lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti-dl/render_dl_content.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti-dl/render_image.html` & `lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti-dl/render_image.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti-dl/render_link.html` & `lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti-dl/render_link.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti_1p3_launch.html` & `lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti_1p3_launch.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti_1p3_studio.html` & `lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti_1p3_studio.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/templates/html/lti_launch.html` & `lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti_launch.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/templates/html/student.html` & `lti-consumer-xblock-9.0.2/lti_consumer/templates/html/student.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/templates/xml/outcome_service_response.xml` & `lti-consumer-xblock-9.0.2/lti_consumer/templates/xml/outcome_service_response.xml`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/templatetags/get_dl_lti_launch_url.py` & `lti-consumer-xblock-9.0.2/lti_consumer/templatetags/get_dl_lti_launch_url.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/templatetags/lti_sanitize.py` & `lti-consumer-xblock-9.0.2/lti_consumer/templatetags/lti_sanitize.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/tests/test_utils.py` & `lti-consumer-xblock-9.0.2/lti_consumer/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/plugin/test_proctoring.py` & `lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/plugin/test_proctoring.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/plugin/test_views.py` & `lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/plugin/test_views.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/plugin/test_views_lti_ags.py` & `lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/plugin/test_views_lti_ags.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py` & `lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py` & `lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/test_api.py` & `lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/test_filters.py` & `lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/test_filters.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/test_lti_xblock.py` & `lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/test_lti_xblock.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/test_models.py` & `lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/test_models.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/test_outcomes.py` & `lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/test_outcomes.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/test_signals.py` & `lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/test_signals.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/tests/unit/test_utils.py` & `lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/translations/ar/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.0.2/lti_consumer/translations/ar/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/translations/ar/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.2/lti_consumer/translations/ar/LC_MESSAGES/text.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,458 +4,520 @@
 # 
 # Translators:
 # shefaa abu jabel <shefaa.aj@gmail.com>, 2016
 msgid ""
 msgstr ""
 "Project-Id-Version: XBlocks\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-02-01 17:24-0300\n"
+"POT-Creation-Date: 2023-04-11 15:09-0400\n"
 "PO-Revision-Date: 2016-06-08 14:38+0000\n"
 "Last-Translator: shefaa abu jabel <shefaa.aj@gmail.com>, 2016\n"
 "Language-Team: Arabic (http://app.transifex.com/open-edx/xblocks/language/ar/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ar\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 && n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 
-#: lti_1p3/extensions/rest_framework/authentication.py:40
+#: lti_1p3/extensions/rest_framework/authentication.py:41
 msgid "Missing LTI 1.3 authentication token."
 msgstr ""
 
-#: lti_1p3/extensions/rest_framework/authentication.py:44
+#: lti_1p3/extensions/rest_framework/authentication.py:45
 msgid "Invalid token header. No credentials provided."
 msgstr ""
 
-#: lti_1p3/extensions/rest_framework/authentication.py:48
+#: lti_1p3/extensions/rest_framework/authentication.py:49
 msgid "Invalid token header. Token string should not contain spaces."
 msgstr ""
 
-#: lti_1p3/extensions/rest_framework/authentication.py:56
+#: lti_1p3/extensions/rest_framework/authentication.py:57
 msgid "LTI configuration not found."
 msgstr ""
 
-#: lti_1p3/extensions/rest_framework/authentication.py:65
+#: lti_1p3/extensions/rest_framework/authentication.py:66
 msgid "Invalid token signature."
 msgstr ""
 
-#: lti_xblock.py:127
+#: lti_xblock.py:126
 msgid "No valid user id found in endpoint URL"
 msgstr "لم يتم العثور على هوية صالحة للمستخدم في URL نقطة النهاية"
 
-#: lti_xblock.py:233
+#: lti_xblock.py:139
+msgid "Configuration on block"
+msgstr ""
+
+#: lti_xblock.py:143
+msgid "Database Configuration"
+msgstr ""
+
+#: lti_xblock.py:146
+msgid "Reusable Configuration"
+msgstr ""
+
+#: lti_xblock.py:253
 msgid "Display Name"
 msgstr "عرض الاسم"
 
-#: lti_xblock.py:235
+#: lti_xblock.py:255
 msgid ""
 "Enter the name that students see for this component. Analytics reports may "
 "also use the display name to identify this component."
 msgstr "أدخل الاسم الذي يراه الطلاب لهذا المكون. يمكن أن تستخدم تقارير التحليلات أيضاً الاسم المعروض من أجل تعريف هذا المكون."
 
-#: lti_xblock.py:239
+#: lti_xblock.py:259
 msgid "LTI Consumer"
 msgstr "مستخدم  LTI"
 
-#: lti_xblock.py:242
+#: lti_xblock.py:262
 msgid "LTI Application Information"
 msgstr "معلومات تطبيق LTI"
 
-#: lti_xblock.py:244
+#: lti_xblock.py:264
 msgid ""
 "Enter a description of the third party application. If requesting username "
 "and/or email, use this text box to inform users why their username and/or "
 "email will be forwarded to a third party application."
 msgstr "قم بإدخال وصف لتطبيق الطرف الثالث. إذا تم طلب اسم مستخدم و/أو بريد إلكتروني، استخدم مربع النص هذا لإبلاغ المستخدمين عن سبب تحويل اسم المستخدم و/أو البريد الإلكتروني الخاص بهم إلى تطبيق طرف ثالث."
 
-#: lti_xblock.py:254
+#: lti_xblock.py:272
+msgid "Configuration Type"
+msgstr ""
+
+#: lti_xblock.py:277
+msgid ""
+"Select 'Configuration on block' to configure a new LTI Tool. If the support "
+"staff provided you with a pre-configured LTI reusable Tool ID, "
+"select'Reusable Configuration' and enter it in the text field below."
+msgstr ""
+
+#: lti_xblock.py:284
 msgid "LTI Version"
 msgstr ""
 
-#: lti_xblock.py:262
+#: lti_xblock.py:292
 msgid ""
 "Select the LTI version that your tool supports.<br />The XBlock LTI Consumer"
 " fully supports LTI 1.1.1, LTI 1.3 and LTI Advantage features."
 msgstr ""
 
-#: lti_xblock.py:268
+#: lti_xblock.py:299
+msgid "LTI Reusable Configuration ID"
+msgstr ""
+
+#: lti_xblock.py:301
+msgid ""
+"Enter the reusable LTI external configuration ID provided by the support "
+"staff."
+msgstr ""
+
+#: lti_xblock.py:306
 msgid "Tool Launch URL"
 msgstr ""
 
-#: lti_xblock.py:272
+#: lti_xblock.py:310
 msgid ""
 "Enter the LTI 1.3 Tool Launch URL. <br />This is the URL the LMS will use to"
 " launch the LTI Tool."
 msgstr ""
 
-#: lti_xblock.py:277
+#: lti_xblock.py:315
 msgid "Tool Initiate Login URL"
 msgstr ""
 
-#: lti_xblock.py:281
+#: lti_xblock.py:319
 msgid ""
 "Enter the LTI 1.3 Tool OIDC Authorization url (can also be called login or "
 "login initiation URL).<br />This is the URL the LMS will use to start a LTI "
 "authorization prior to doing the launch request."
 msgstr ""
 
-#: lti_xblock.py:288
+#: lti_xblock.py:325
+msgid "Registered Redirect URIs"
+msgstr ""
+
+#: lti_xblock.py:327
+msgid ""
+"Valid urls the Tool may request us to redirect the id token to. The redirect"
+" uris are often the same as the launch url/deep linking url so if this field"
+" is empty, it will use them as the default. If you need to use different "
+"redirect uri's, enter them here. If you use this field you must enter all "
+"valid redirect uri's the tool may request."
+msgstr ""
+
+#: lti_xblock.py:337
 msgid "Tool Public Key Mode"
 msgstr ""
 
-#: lti_xblock.py:296
+#: lti_xblock.py:345
 msgid "Select how the tool's public key information will be specified."
 msgstr ""
 
-#: lti_xblock.py:300
+#: lti_xblock.py:349
 msgid "Tool Keyset URL"
 msgstr ""
 
-#: lti_xblock.py:304
+#: lti_xblock.py:353
 msgid ""
 "Enter the LTI 1.3 Tool's JWK keysets URL.<br />This link should retrieve a "
 "JSON file containing public keys and signature algorithm information, so "
 "that the LMS can check if the messages and launch requests received have the"
 " signature from the tool.<br /><b>This is not required when doing LTI 1.3 "
 "Launches without LTI Advantage nor Basic Outcomes requests.</b>"
 msgstr ""
 
-#: lti_xblock.py:314
+#: lti_xblock.py:363
 msgid "Tool Public Key"
 msgstr ""
 
-#: lti_xblock.py:319
+#: lti_xblock.py:368
 msgid ""
 "Enter the LTI 1.3 Tool's public key.<br />This is a string that starts with "
 "'-----BEGIN PUBLIC KEY-----' and is required so that the LMS can check if "
 "the messages and launch requests received have the signature from the "
 "tool.<br /><b>This is not required when doing LTI 1.3 Launches without LTI "
 "Advantage nor Basic Outcomes requests.</b>"
 msgstr ""
 
-#: lti_xblock.py:329
+#: lti_xblock.py:378
 msgid "Enable LTI NRPS"
 msgstr ""
 
-#: lti_xblock.py:330
+#: lti_xblock.py:379
 msgid "Enable LTI Names and Role Provisioning Services."
 msgstr ""
 
-#: lti_xblock.py:337
+#: lti_xblock.py:386
 msgid "LTI 1.3 Block Client ID - DEPRECATED"
 msgstr ""
 
-#: lti_xblock.py:340
+#: lti_xblock.py:389
 msgid "DEPRECATED - This is now stored in the LtiConfiguration model."
 msgstr ""
 
-#: lti_xblock.py:343
+#: lti_xblock.py:392
 msgid "LTI 1.3 Block Key - DEPRECATED"
 msgstr ""
 
-#: lti_xblock.py:350
+#: lti_xblock.py:399
 msgid "Deep linking"
 msgstr ""
 
-#: lti_xblock.py:351
+#: lti_xblock.py:400
 msgid "Select True if you want to enable LTI Advantage Deep Linking."
 msgstr ""
 
-#: lti_xblock.py:356
+#: lti_xblock.py:405
 msgid "Deep Linking Launch URL"
 msgstr ""
 
-#: lti_xblock.py:360
+#: lti_xblock.py:409
 msgid ""
 "Enter the LTI Advantage Deep Linking Launch URL. If the tool does not "
 "specify one, use the same value as 'Tool Launch URL'."
 msgstr ""
 
-#: lti_xblock.py:365
+#: lti_xblock.py:414
 msgid "LTI Assignment and Grades Service"
 msgstr ""
 
-#: lti_xblock.py:367
+#: lti_xblock.py:416
 msgid "Disabled"
 msgstr ""
 
-#: lti_xblock.py:368
+#: lti_xblock.py:417
 msgid "Allow tools to submit grades only (declarative)"
 msgstr ""
 
-#: lti_xblock.py:369
+#: lti_xblock.py:418
 msgid "Allow tools to manage and submit grade (programmatic)"
 msgstr ""
 
-#: lti_xblock.py:374
+#: lti_xblock.py:423
 msgid ""
 "Enable the LTI-AGS service and select the functionality enabled for LTI "
 "tools. The 'declarative' mode (default) will provide a tool with a LineItem "
 "created from the XBlock settings, while the 'programmatic' one will allow "
 "tools to manage, create and link the grades."
 msgstr ""
 
-#: lti_xblock.py:382
+#: lti_xblock.py:431
 msgid "LTI ID"
 msgstr "هوية LTI"
 
-#: lti_xblock.py:384
+#: lti_xblock.py:433
 #, python-brace-format
 msgid ""
 "Enter the LTI ID for the external LTI provider. This value must be the same "
 "LTI ID that you entered in the LTI Passports setting on the Advanced "
 "Settings page.<br />See the {docs_anchor_open}edX LTI "
 "documentation{anchor_close} for more details on this setting."
 msgstr "أدخل هوية LTI لمورد LTI الخارجي. يجب أن تكون هذه القيمة هي نفس قيمة هوية LTI التي أدخلتها في إعدادات جوازات مرور LTI في صفحة الإعدادات المتقدمة.<br />اطلع على مستندات {docs_anchor_open} edX LTI{anchor_close} للمزيد من التفاصيل عن هذا الإعداد."
 
-#: lti_xblock.py:396
+#: lti_xblock.py:445
 msgid "LTI URL"
 msgstr "LTI URL"
 
-#: lti_xblock.py:398
+#: lti_xblock.py:447
 #, python-brace-format
 msgid ""
 "Enter the URL of the external tool that this component launches. This "
 "setting is only used when Hide External Tool is set to False.<br />See the "
 "{docs_anchor_open}edX LTI documentation{anchor_close} for more details on "
 "this setting."
 msgstr "أدخل URL الأداة الخارجية التي يقوم هذا المكون بتشغيلها. يتم استخدام هذا الإعداد فقط عند تحديد إخفاء الأداة الخارجية  على خيار خاطئ.<br />اطلع على مستندات {docs_anchor_open} edX LTI{anchor_close} للمزيد من التفاصيل عن هذا الإعداد."
 
-#: lti_xblock.py:411
+#: lti_xblock.py:460
 msgid "Custom Parameters"
 msgstr "العوامل المخصصة"
 
-#: lti_xblock.py:413
+#: lti_xblock.py:462
 #, python-brace-format
 msgid ""
 "Add the key/value pair for any custom parameters, such as the page your "
 "e-book should open to or the background color for this component. Ex. "
 "[\"page=1\", \"color=white\"]<br />See the {docs_anchor_open}edX LTI "
 "documentation{anchor_close} for more details on this setting."
 msgstr "أضف زوج المفتاح/القيمة لأي عوامل مخصصة، مثل الصفحة التي يجب أن يفتحها كتابك الإلكتروني أو لون خلفية هذا المكون. مثال. Ex. [\"page=1\", \"color=white\"]<br />اطلع على مستندات {docs_anchor_open} edX LTI{anchor_close} للمزيد من التفاصيل عن هذا الإعداد."
 
-#: lti_xblock.py:423
+#: lti_xblock.py:472
 msgid "LTI Launch Target"
 msgstr "هدف تشغيل LTI"
 
-#: lti_xblock.py:425
+#: lti_xblock.py:474
 msgid ""
 "Select Inline if you want the LTI content to open in an IFrame in the "
 "current page. Select Modal if you want the LTI content to open in a modal "
 "window in the current page. Select New Window if you want the LTI content to"
 " open in a new browser window. This setting is only used when Hide External "
 "Tool is set to False."
 msgstr "قم بتحديد خط داخلي إذا كنت تريد أن يتم فتح محتويات LTI في إطار IFrame في الصفحة الحالية. حدد  الشكل إذا كنت تريد أن يتم فتح محتويات LTI في نافذة موضعية في الصفحة الحالية. اختر نافذة جديدة إذا كنت تريد أن يتم فتح محتويات LTI في نافذة متصفح جديد. ‏‫سيتم استخدام هذا الإعداد فقط عندما يتم ضبط إخفاء الأداة الخارجية على خاطىء ."
 
-#: lti_xblock.py:439
+#: lti_xblock.py:488
 msgid "Button Text"
 msgstr "نص الزر"
 
-#: lti_xblock.py:441
+#: lti_xblock.py:490
 msgid ""
 "Enter the text on the button used to launch the third party application. "
 "This setting is only used when Hide External Tool is set to False and LTI "
 "Launch Target is set to Modal or New Window."
 msgstr "أدخل النص على الزر المستخدم لبدء تشغيل تطبيق الطرف الثالث. لا يتم استخدام هذا الإعداد إلا عند ضبط إخفاء الأداة الخارجية على خاطئ، وضبط هدف بدء تشغيل LTI على نموذج  أو نافذة جديدة ."
 
-#: lti_xblock.py:449
+#: lti_xblock.py:498
 msgid "Inline Height"
 msgstr "ارتفاع ضمن الخطوط"
 
-#: lti_xblock.py:451
+#: lti_xblock.py:500
 msgid ""
 "Enter the desired pixel height of the iframe which will contain the LTI "
 "tool. This setting is only used when Hide External Tool is set to False and "
 "LTI Launch Target is set to Inline."
 msgstr "أدخل ارتفاع البيكسل المرغوب لإطار iframe الذي سوف يحتوي على أداة LTI. لا يتم استخدام هذا الإعداد إلا عند ضبط إخفاء الأداة الخارجية على خاطئ، وضبط هدف بدء تشغيل LTI ضمن الخطوط."
 
-#: lti_xblock.py:459
+#: lti_xblock.py:508
 msgid "Modal Height"
 msgstr "ارتفاع شكلي"
 
-#: lti_xblock.py:461
+#: lti_xblock.py:510
 msgid ""
 "Enter the desired viewport percentage height of the modal overlay which will"
 " contain the LTI tool. This setting is only used when Hide External Tool is "
 "set to False and LTI Launch Target is set to Modal."
 msgstr "أدخل الارتفاع المرغوب لمنفذ العرض بالنسبة المئوية للتداخل الشكلي الذي سوف يحتوي على أداة LTI. لا يتم استخدام هذا الإعداد إلا عند ضبط إخفاء الأداة الخارجية على خاطئ، وضبط هدف بدء تشغيل LTI على نموذج."
 
-#: lti_xblock.py:469
+#: lti_xblock.py:518
 msgid "Modal Width"
 msgstr "العرض الشكلي"
 
-#: lti_xblock.py:471
+#: lti_xblock.py:520
 msgid ""
 "Enter the desired viewport percentage width of the modal overlay which will "
 "contain the LTI tool. This setting is only used when Hide External Tool is "
 "set to False and LTI Launch Target is set to Modal."
 msgstr "أدخل العرض المرغوب لمنفذ العرض بالنسبة المئوية للتداخل الشكلي الذي سوف يحتوي على أداة LTI. لا يتم استخدام هذا الإعداد إلا عند ضبط إخفاء الأداة الخارجية على خاطئ، وضبط هدف بدء تشغيل LTI على نموذج."
 
-#: lti_xblock.py:479
+#: lti_xblock.py:528
 msgid "Scored"
 msgstr "النتيجة"
 
-#: lti_xblock.py:480
+#: lti_xblock.py:529
 msgid ""
 "Select True if this component will receive a numerical score from the "
 "external LTI system."
 msgstr "اختر صحيح إذا كان هذا المكون سيحصل على نتيجة رقمية من نظام LTI خارجي."
 
-#: lti_xblock.py:487
+#: lti_xblock.py:536
 msgid ""
 "Enter the number of points possible for this component.  The default value "
 "is 1.0.  This setting is only used when Scored is set to True."
 msgstr "أدخل عدد النقاط المتاحة لهذا المكون.  القيمة الافتراضية هي 1.0.  ‏‫يتم استخدام هذا الإعداد فقط عند تحديد النتيجة المنشورة صحيح."
 
-#: lti_xblock.py:496
+#: lti_xblock.py:545
 msgid ""
 "The score kept in the xblock KVS -- duplicate of the published score in "
 "django DB"
 msgstr "النتيجة المحفوظة في xblock KVS -- هي نسخة عن النتيجة المنشورة في django DB"
 
-#: lti_xblock.py:501
+#: lti_xblock.py:550
 msgid "Comment as returned from grader, LTI2.0 spec"
 msgstr "الملاحظات التي تم إرجاعها من مانح العلامة، مواصفات LTI2.0"
 
-#: lti_xblock.py:506
+#: lti_xblock.py:555
 msgid "Hide External Tool"
 msgstr "إخفاء الأداء الخارجية"
 
-#: lti_xblock.py:508
+#: lti_xblock.py:557
 msgid ""
 "Select True if you want to use this component as a placeholder for syncing "
 "with an external grading  system rather than launch an external tool.  This "
 "setting hides the Launch button and any IFrames for this component."
 msgstr "اختر صحيح إذا كنت ترغب في استخدام هذا المكون كحافظ للمكان للمزامنة مع نظام خارجي لوضع العلامات بدلاً نت استخدام أداة خارجية.  يقوم هذا الإعداد بإخفاء زر بدء التشغيل وأي IFrames لهذا المكون."
 
-#: lti_xblock.py:516
+#: lti_xblock.py:565
 msgid "Accept grades past deadline"
 msgstr "قبول العلامات بعد انقضاء الموعد المحدد"
 
-#: lti_xblock.py:517
+#: lti_xblock.py:566
 msgid ""
 "Select True to allow third party systems to post grades past the deadline."
 msgstr "اختر صحيح  للسماح لأنظمة الطرف الثالث بوضع علامات بعد انقضاء الموعد المحدد."
 
-#: lti_xblock.py:525
+#: lti_xblock.py:574
 msgid "Request user's username"
 msgstr "اطلب اسم المستخدم الخاص بالمستخدم"
 
 #. Translators: This is used to request the user's username for a third party
 #. service.
-#: lti_xblock.py:527
+#: lti_xblock.py:576
 msgid "Select True to request the user's username."
 msgstr "اختر ״ صحيح״  لطلب اسم مستخدم خاص بالمستخدم."
 
-#: lti_xblock.py:532
+#: lti_xblock.py:581
 msgid "Request user's email"
 msgstr "اطلب البريد الإلكتروني الخاص بالمستخدم"
 
 #. Translators: This is used to request the user's email for a third party
 #. service.
-#: lti_xblock.py:534
+#: lti_xblock.py:583
 msgid "Select True to request the user's email address."
 msgstr "اختر صحيح لطلب عنوان البريد الإلكتروني الخاص بالمستخدم."
 
-#: lti_xblock.py:539
+#: lti_xblock.py:588
 msgid "Send extra parameters"
 msgstr ""
 
-#: lti_xblock.py:540
+#: lti_xblock.py:589
 msgid ""
 "Select True to send the extra parameters, which might contain Personally "
 "Identifiable Information. The processors are site-wide, please consult the "
 "site administrator if you have any questions."
 msgstr ""
 
-#: lti_xblock.py:603
+#: lti_xblock.py:652
 msgid "Custom Parameters must be a list"
 msgstr ""
 
-#: lti_xblock.py:713
+#: lti_xblock.py:783 lti_xblock.py:1062
+msgid "Could not get user data for current request"
+msgstr ""
+
+#: lti_xblock.py:810
 msgid ""
 "Could not parse LTI passport: {lti_passport!r}. Should be \"id:key:secret\" "
 "string."
 msgstr ""
 
-#: lti_xblock.py:729 lti_xblock.py:745
+#: lti_xblock.py:828 lti_xblock.py:842 lti_xblock.py:858
 msgid "Could not get user id for current request"
 msgstr "تعذر الحصول على هوية مستخدم للطلب الحالي"
 
-#: lti_xblock.py:850
+#: lti_xblock.py:994
 msgid ""
 "Could not parse custom parameter: {custom_parameter!r}. Should be \"x=y\" "
 "string."
 msgstr ""
 
-#: lti_xblock.py:1310
+#: lti_xblock.py:1343
 msgid "[LTI]: Real user not found against anon_id: {}"
 msgstr "[LTI]: لم يتم العثور على مستخدم حقيقي مقابل هوية غير معرفة: {}"
 
-#: models.py:72
+#: models.py:79
 msgid "Configuration Stored on XBlock fields"
 msgstr ""
 
-#: models.py:73
+#: models.py:80
 msgid "Configuration Stored on this model"
 msgstr ""
 
-#: models.py:97
+#: models.py:81
+msgid "Configuration Stored on external service"
+msgstr ""
+
+#: models.py:113
 msgid "LTI configuration data."
 msgstr ""
 
-#: models.py:104
+#: models.py:120
 msgid "The URL of the external tool that initiates the launch."
 msgstr ""
 
-#: models.py:109
+#: models.py:125
 msgid "Client key provided by the LTI tool provider."
 msgstr ""
 
-#: models.py:115
+#: models.py:131
 msgid "Client secret provided by the LTI tool provider."
 msgstr ""
 
-#: models.py:121
+#: models.py:137
 msgid "Platform's generated Private key. Keep this value secret."
 msgstr ""
 
-#: models.py:127
+#: models.py:143
 msgid "Platform's generated Private key ID"
 msgstr ""
 
-#: models.py:132
+#: models.py:148
 msgid "Platform's generated JWK keyset."
 msgstr ""
 
-#: models.py:138
+#: models.py:154
 msgid "Client ID used by LTI tool"
 msgstr ""
 
-#: models.py:148
+#: models.py:250
 msgid "LTI Configuration stores on XBlock needs a block location set."
 msgstr ""
 
-#: models.py:155
-msgid "Invalid LTI configuration."
+#: models.py:256
+msgid ""
+"LTI Configuration stored on the model for LTI 1.3 must have a value for one "
+"of lti_1p3_tool_public_key or lti_1p3_tool_keyset_url."
+msgstr ""
+
+#: models.py:263
+msgid ""
+"CONFIG_ON_XBLOCK and CONFIG_EXTERNAL are not supported for LTI 1.3 "
+"Proctoring Services."
 msgstr ""
 
-#: models.py:165
-msgid "Block location not set, it's not possible to retrieve the block."
+#: models.py:271
+msgid "Invalid LTI configuration."
 msgstr ""
 
-#: plugin/views.py:246
+#: plugin/views.py:453
 msgid "The selected content type is not supported by Open edX."
 msgstr ""
 
-#: plugin/views.py:261
+#: plugin/views.py:468
 msgid "You don't have access to save LTI Content Items."
 msgstr ""
 
-#: plugin/views.py:262
+#: plugin/views.py:469
 msgid ""
 "Please check that you have course staff permissions and double check this "
 "block's LTI settings."
 msgstr ""
 
 #: templates/html/lti-dl/dl_response_error.html:6
 msgid "LTI Deep Linking failed."
@@ -469,23 +531,14 @@
 msgid "The LTI Deep Linking content was successfully saved in the LMS."
 msgstr ""
 
 #: templates/html/lti-dl/dl_response_saved.html:13
 msgid "You can safely close this page now."
 msgstr ""
 
-#: templates/html/lti_1p3_launch_error.html:10
-msgid "There was an error while launching the LTI 1.3 tool."
-msgstr ""
-
-#: templates/html/lti_1p3_launch_error.html:13
-msgid ""
-"If you're seeing this on a live course, please contact the course staff."
-msgstr ""
-
 #: templates/html/lti_1p3_permission_error.html:10
 msgid "Unauthorized."
 msgstr ""
 
 #: templates/html/lti_1p3_permission_error.html:13
 msgid ""
 "Students don't have permissions to perform LTI Deep Linking configuration "
@@ -546,27 +599,46 @@
 msgid "Deep Linking Launch - Configure tool"
 msgstr ""
 
 #: templates/html/lti_launch.html:27
 msgid "Press to Launch"
 msgstr ""
 
-#: static/js/xblock_lti_consumer.js:142
-msgid ""
-"Click OK to have your username and e-mail address sent to a 3rd party application.\n"
-"\n"
-"Click Cancel to return to this page without sending your information."
+#: templates/html/lti_launch_error.html:10
+msgid "There was an error while launching the LTI tool."
 msgstr ""
 
-#: static/js/xblock_lti_consumer.js:144
+#: templates/html/lti_launch_error.html:13
+#: templates/html/lti_proctoring_start_error.html:13
 msgid ""
-"Click OK to have your username sent to a 3rd party application.\n"
-"\n"
-"Click Cancel to return to this page without sending your information."
+"If you're seeing this on a live course, please contact the course staff."
+msgstr ""
+
+#: templates/html/lti_proctoring_start_error.html:10
+msgid "There was an error while starting your LTI proctored assessment."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:126
+msgid "Cancel"
 msgstr ""
 
-#: static/js/xblock_lti_consumer.js:146
+#: static/js/xblock_lti_consumer.js:128
+msgid "OK"
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:157
 msgid ""
-"Click OK to have your e-mail address sent to a 3rd party application.\n"
-"\n"
-"Click Cancel to return to this page without sending your information."
+"Click OK to have your username and e-mail address sent to a 3rd party "
+"application."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:159
+msgid "Click OK to have your username sent to a 3rd party application."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:161
+msgid "Click OK to have your e-mail address sent to a 3rd party application."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:168
+msgid "Click Cancel to return to this page without sending your information."
 msgstr ""
```

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/translations/en/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.2/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po`

 * *Files 7% similar despite different names*

```diff
@@ -1,459 +1,524 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-#
-#, fuzzy
+# 
+# Translators:
+# Renata Barboza, 2016
+# Simone Baldissera, 2021
 msgid ""
 msgstr ""
-"Project-Id-Version: PACKAGE VERSION\n"
+"Project-Id-Version: XBlocks\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-02-01 17:24-0300\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"POT-Creation-Date: 2023-04-11 15:09-0400\n"
+"PO-Revision-Date: 2016-06-08 14:38+0000\n"
+"Last-Translator: Simone Baldissera, 2021\n"
+"Language-Team: Portuguese (Brazil) (http://app.transifex.com/open-edx/xblocks/language/pt_BR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: pt_BR\n"
+"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
-#: lti_1p3/extensions/rest_framework/authentication.py:40
+#: lti_1p3/extensions/rest_framework/authentication.py:41
 msgid "Missing LTI 1.3 authentication token."
 msgstr ""
 
-#: lti_1p3/extensions/rest_framework/authentication.py:44
+#: lti_1p3/extensions/rest_framework/authentication.py:45
 msgid "Invalid token header. No credentials provided."
 msgstr ""
 
-#: lti_1p3/extensions/rest_framework/authentication.py:48
+#: lti_1p3/extensions/rest_framework/authentication.py:49
 msgid "Invalid token header. Token string should not contain spaces."
 msgstr ""
 
-#: lti_1p3/extensions/rest_framework/authentication.py:56
+#: lti_1p3/extensions/rest_framework/authentication.py:57
 msgid "LTI configuration not found."
 msgstr ""
 
-#: lti_1p3/extensions/rest_framework/authentication.py:65
+#: lti_1p3/extensions/rest_framework/authentication.py:66
 msgid "Invalid token signature."
 msgstr ""
 
-#: lti_xblock.py:127
+#: lti_xblock.py:126
 msgid "No valid user id found in endpoint URL"
+msgstr "Nenhuma ID de usuário válido encontrada no ponto de extremidade da URL"
+
+#: lti_xblock.py:139
+msgid "Configuration on block"
 msgstr ""
 
-#: lti_xblock.py:233
-msgid "Display Name"
+#: lti_xblock.py:143
+msgid "Database Configuration"
 msgstr ""
 
-#: lti_xblock.py:235
+#: lti_xblock.py:146
+msgid "Reusable Configuration"
+msgstr ""
+
+#: lti_xblock.py:253
+msgid "Display Name"
+msgstr "Nome de exibição"
+
+#: lti_xblock.py:255
 msgid ""
 "Enter the name that students see for this component. Analytics reports may "
 "also use the display name to identify this component."
-msgstr ""
+msgstr "Forneça o nome que os alunos verão para este componente. Os relatórios de análise também poderão usar o nome de exibição para identificar este componente. "
 
-#: lti_xblock.py:239
+#: lti_xblock.py:259
 msgid "LTI Consumer"
-msgstr ""
+msgstr "Consumidor de LTI"
 
-#: lti_xblock.py:242
+#: lti_xblock.py:262
 msgid "LTI Application Information"
-msgstr ""
+msgstr "Informações do aplicativo LTI"
 
-#: lti_xblock.py:244
+#: lti_xblock.py:264
 msgid ""
 "Enter a description of the third party application. If requesting username "
 "and/or email, use this text box to inform users why their username and/or "
 "email will be forwarded to a third party application."
 msgstr ""
 
-#: lti_xblock.py:254
+#: lti_xblock.py:272
+msgid "Configuration Type"
+msgstr ""
+
+#: lti_xblock.py:277
+msgid ""
+"Select 'Configuration on block' to configure a new LTI Tool. If the support "
+"staff provided you with a pre-configured LTI reusable Tool ID, "
+"select'Reusable Configuration' and enter it in the text field below."
+msgstr ""
+
+#: lti_xblock.py:284
 msgid "LTI Version"
 msgstr ""
 
-#: lti_xblock.py:262
+#: lti_xblock.py:292
+msgid ""
+"Select the LTI version that your tool supports.<br />The XBlock LTI Consumer"
+" fully supports LTI 1.1.1, LTI 1.3 and LTI Advantage features."
+msgstr ""
+
+#: lti_xblock.py:299
+msgid "LTI Reusable Configuration ID"
+msgstr ""
+
+#: lti_xblock.py:301
 msgid ""
-"Select the LTI version that your tool supports.<br />The XBlock LTI Consumer "
-"fully supports LTI 1.1.1, LTI 1.3 and LTI Advantage features."
+"Enter the reusable LTI external configuration ID provided by the support "
+"staff."
 msgstr ""
 
-#: lti_xblock.py:268
+#: lti_xblock.py:306
 msgid "Tool Launch URL"
 msgstr ""
 
-#: lti_xblock.py:272
+#: lti_xblock.py:310
 msgid ""
-"Enter the LTI 1.3 Tool Launch URL. <br />This is the URL the LMS will use to "
-"launch the LTI Tool."
+"Enter the LTI 1.3 Tool Launch URL. <br />This is the URL the LMS will use to"
+" launch the LTI Tool."
 msgstr ""
 
-#: lti_xblock.py:277
+#: lti_xblock.py:315
 msgid "Tool Initiate Login URL"
 msgstr ""
 
-#: lti_xblock.py:281
+#: lti_xblock.py:319
 msgid ""
 "Enter the LTI 1.3 Tool OIDC Authorization url (can also be called login or "
 "login initiation URL).<br />This is the URL the LMS will use to start a LTI "
 "authorization prior to doing the launch request."
 msgstr ""
 
-#: lti_xblock.py:288
+#: lti_xblock.py:325
+msgid "Registered Redirect URIs"
+msgstr ""
+
+#: lti_xblock.py:327
+msgid ""
+"Valid urls the Tool may request us to redirect the id token to. The redirect"
+" uris are often the same as the launch url/deep linking url so if this field"
+" is empty, it will use them as the default. If you need to use different "
+"redirect uri's, enter them here. If you use this field you must enter all "
+"valid redirect uri's the tool may request."
+msgstr ""
+
+#: lti_xblock.py:337
 msgid "Tool Public Key Mode"
 msgstr ""
 
-#: lti_xblock.py:296
+#: lti_xblock.py:345
 msgid "Select how the tool's public key information will be specified."
 msgstr ""
 
-#: lti_xblock.py:300
+#: lti_xblock.py:349
 msgid "Tool Keyset URL"
 msgstr ""
 
-#: lti_xblock.py:304
+#: lti_xblock.py:353
 msgid ""
 "Enter the LTI 1.3 Tool's JWK keysets URL.<br />This link should retrieve a "
 "JSON file containing public keys and signature algorithm information, so "
-"that the LMS can check if the messages and launch requests received have the "
-"signature from the tool.<br /><b>This is not required when doing LTI 1.3 "
+"that the LMS can check if the messages and launch requests received have the"
+" signature from the tool.<br /><b>This is not required when doing LTI 1.3 "
 "Launches without LTI Advantage nor Basic Outcomes requests.</b>"
 msgstr ""
 
-#: lti_xblock.py:314
+#: lti_xblock.py:363
 msgid "Tool Public Key"
 msgstr ""
 
-#: lti_xblock.py:319
+#: lti_xblock.py:368
 msgid ""
 "Enter the LTI 1.3 Tool's public key.<br />This is a string that starts with "
 "'-----BEGIN PUBLIC KEY-----' and is required so that the LMS can check if "
-"the messages and launch requests received have the signature from the tool."
-"<br /><b>This is not required when doing LTI 1.3 Launches without LTI "
+"the messages and launch requests received have the signature from the "
+"tool.<br /><b>This is not required when doing LTI 1.3 Launches without LTI "
 "Advantage nor Basic Outcomes requests.</b>"
 msgstr ""
 
-#: lti_xblock.py:329
+#: lti_xblock.py:378
 msgid "Enable LTI NRPS"
 msgstr ""
 
-#: lti_xblock.py:330
+#: lti_xblock.py:379
 msgid "Enable LTI Names and Role Provisioning Services."
 msgstr ""
 
-#: lti_xblock.py:337
+#: lti_xblock.py:386
 msgid "LTI 1.3 Block Client ID - DEPRECATED"
 msgstr ""
 
-#: lti_xblock.py:340
+#: lti_xblock.py:389
 msgid "DEPRECATED - This is now stored in the LtiConfiguration model."
 msgstr ""
 
-#: lti_xblock.py:343
+#: lti_xblock.py:392
 msgid "LTI 1.3 Block Key - DEPRECATED"
 msgstr ""
 
-#: lti_xblock.py:350
+#: lti_xblock.py:399
 msgid "Deep linking"
 msgstr ""
 
-#: lti_xblock.py:351
+#: lti_xblock.py:400
 msgid "Select True if you want to enable LTI Advantage Deep Linking."
 msgstr ""
 
-#: lti_xblock.py:356
+#: lti_xblock.py:405
 msgid "Deep Linking Launch URL"
 msgstr ""
 
-#: lti_xblock.py:360
+#: lti_xblock.py:409
 msgid ""
 "Enter the LTI Advantage Deep Linking Launch URL. If the tool does not "
 "specify one, use the same value as 'Tool Launch URL'."
 msgstr ""
 
-#: lti_xblock.py:365
+#: lti_xblock.py:414
 msgid "LTI Assignment and Grades Service"
 msgstr ""
 
-#: lti_xblock.py:367
+#: lti_xblock.py:416
 msgid "Disabled"
 msgstr ""
 
-#: lti_xblock.py:368
+#: lti_xblock.py:417
 msgid "Allow tools to submit grades only (declarative)"
 msgstr ""
 
-#: lti_xblock.py:369
+#: lti_xblock.py:418
 msgid "Allow tools to manage and submit grade (programmatic)"
 msgstr ""
 
-#: lti_xblock.py:374
+#: lti_xblock.py:423
 msgid ""
 "Enable the LTI-AGS service and select the functionality enabled for LTI "
 "tools. The 'declarative' mode (default) will provide a tool with a LineItem "
 "created from the XBlock settings, while the 'programmatic' one will allow "
 "tools to manage, create and link the grades."
 msgstr ""
 
-#: lti_xblock.py:382
+#: lti_xblock.py:431
 msgid "LTI ID"
-msgstr ""
+msgstr "ID do LTI"
 
-#: lti_xblock.py:384
+#: lti_xblock.py:433
 #, python-brace-format
 msgid ""
 "Enter the LTI ID for the external LTI provider. This value must be the same "
 "LTI ID that you entered in the LTI Passports setting on the Advanced "
 "Settings page.<br />See the {docs_anchor_open}edX LTI "
 "documentation{anchor_close} for more details on this setting."
 msgstr ""
 
-#: lti_xblock.py:396
+#: lti_xblock.py:445
 msgid "LTI URL"
 msgstr ""
 
-#: lti_xblock.py:398
+#: lti_xblock.py:447
 #, python-brace-format
 msgid ""
 "Enter the URL of the external tool that this component launches. This "
 "setting is only used when Hide External Tool is set to False.<br />See the "
 "{docs_anchor_open}edX LTI documentation{anchor_close} for more details on "
 "this setting."
 msgstr ""
 
-#: lti_xblock.py:411
+#: lti_xblock.py:460
 msgid "Custom Parameters"
 msgstr ""
 
-#: lti_xblock.py:413
+#: lti_xblock.py:462
 #, python-brace-format
 msgid ""
-"Add the key/value pair for any custom parameters, such as the page your e-"
-"book should open to or the background color for this component. Ex. "
+"Add the key/value pair for any custom parameters, such as the page your "
+"e-book should open to or the background color for this component. Ex. "
 "[\"page=1\", \"color=white\"]<br />See the {docs_anchor_open}edX LTI "
 "documentation{anchor_close} for more details on this setting."
 msgstr ""
 
-#: lti_xblock.py:423
+#: lti_xblock.py:472
 msgid "LTI Launch Target"
 msgstr ""
 
-#: lti_xblock.py:425
+#: lti_xblock.py:474
 msgid ""
 "Select Inline if you want the LTI content to open in an IFrame in the "
 "current page. Select Modal if you want the LTI content to open in a modal "
-"window in the current page. Select New Window if you want the LTI content to "
-"open in a new browser window. This setting is only used when Hide External "
+"window in the current page. Select New Window if you want the LTI content to"
+" open in a new browser window. This setting is only used when Hide External "
 "Tool is set to False."
 msgstr ""
 
-#: lti_xblock.py:439
+#: lti_xblock.py:488
 msgid "Button Text"
 msgstr ""
 
-#: lti_xblock.py:441
+#: lti_xblock.py:490
 msgid ""
 "Enter the text on the button used to launch the third party application. "
 "This setting is only used when Hide External Tool is set to False and LTI "
 "Launch Target is set to Modal or New Window."
 msgstr ""
 
-#: lti_xblock.py:449
+#: lti_xblock.py:498
 msgid "Inline Height"
-msgstr ""
+msgstr "Altura do embutido"
 
-#: lti_xblock.py:451
+#: lti_xblock.py:500
 msgid ""
 "Enter the desired pixel height of the iframe which will contain the LTI "
 "tool. This setting is only used when Hide External Tool is set to False and "
 "LTI Launch Target is set to Inline."
 msgstr ""
 
-#: lti_xblock.py:459
+#: lti_xblock.py:508
 msgid "Modal Height"
-msgstr ""
+msgstr "Altura do modal"
 
-#: lti_xblock.py:461
+#: lti_xblock.py:510
 msgid ""
-"Enter the desired viewport percentage height of the modal overlay which will "
-"contain the LTI tool. This setting is only used when Hide External Tool is "
+"Enter the desired viewport percentage height of the modal overlay which will"
+" contain the LTI tool. This setting is only used when Hide External Tool is "
 "set to False and LTI Launch Target is set to Modal."
 msgstr ""
 
-#: lti_xblock.py:469
+#: lti_xblock.py:518
 msgid "Modal Width"
-msgstr ""
+msgstr "Largura do modal"
 
-#: lti_xblock.py:471
+#: lti_xblock.py:520
 msgid ""
 "Enter the desired viewport percentage width of the modal overlay which will "
 "contain the LTI tool. This setting is only used when Hide External Tool is "
 "set to False and LTI Launch Target is set to Modal."
 msgstr ""
 
-#: lti_xblock.py:479
+#: lti_xblock.py:528
 msgid "Scored"
 msgstr ""
 
-#: lti_xblock.py:480
+#: lti_xblock.py:529
 msgid ""
 "Select True if this component will receive a numerical score from the "
 "external LTI system."
 msgstr ""
 
-#: lti_xblock.py:487
+#: lti_xblock.py:536
 msgid ""
 "Enter the number of points possible for this component.  The default value "
 "is 1.0.  This setting is only used when Scored is set to True."
 msgstr ""
 
-#: lti_xblock.py:496
+#: lti_xblock.py:545
 msgid ""
 "The score kept in the xblock KVS -- duplicate of the published score in "
 "django DB"
 msgstr ""
 
-#: lti_xblock.py:501
+#: lti_xblock.py:550
 msgid "Comment as returned from grader, LTI2.0 spec"
 msgstr ""
 
-#: lti_xblock.py:506
+#: lti_xblock.py:555
 msgid "Hide External Tool"
 msgstr ""
 
-#: lti_xblock.py:508
+#: lti_xblock.py:557
 msgid ""
 "Select True if you want to use this component as a placeholder for syncing "
 "with an external grading  system rather than launch an external tool.  This "
 "setting hides the Launch button and any IFrames for this component."
 msgstr ""
 
-#: lti_xblock.py:516
+#: lti_xblock.py:565
 msgid "Accept grades past deadline"
 msgstr ""
 
-#: lti_xblock.py:517
+#: lti_xblock.py:566
 msgid ""
 "Select True to allow third party systems to post grades past the deadline."
 msgstr ""
 
-#: lti_xblock.py:525
+#: lti_xblock.py:574
 msgid "Request user's username"
 msgstr ""
 
-#. Translators: This is used to request the user's username for a third party service.
-#: lti_xblock.py:527
+#. Translators: This is used to request the user's username for a third party
+#. service.
+#: lti_xblock.py:576
 msgid "Select True to request the user's username."
 msgstr ""
 
-#: lti_xblock.py:532
+#: lti_xblock.py:581
 msgid "Request user's email"
 msgstr ""
 
-#. Translators: This is used to request the user's email for a third party service.
-#: lti_xblock.py:534
+#. Translators: This is used to request the user's email for a third party
+#. service.
+#: lti_xblock.py:583
 msgid "Select True to request the user's email address."
 msgstr ""
 
-#: lti_xblock.py:539
+#: lti_xblock.py:588
 msgid "Send extra parameters"
 msgstr ""
 
-#: lti_xblock.py:540
+#: lti_xblock.py:589
 msgid ""
 "Select True to send the extra parameters, which might contain Personally "
 "Identifiable Information. The processors are site-wide, please consult the "
 "site administrator if you have any questions."
 msgstr ""
 
-#: lti_xblock.py:603
+#: lti_xblock.py:652
 msgid "Custom Parameters must be a list"
 msgstr ""
 
-#: lti_xblock.py:713
+#: lti_xblock.py:783 lti_xblock.py:1062
+msgid "Could not get user data for current request"
+msgstr ""
+
+#: lti_xblock.py:810
 msgid ""
 "Could not parse LTI passport: {lti_passport!r}. Should be \"id:key:secret\" "
 "string."
 msgstr ""
 
-#: lti_xblock.py:729 lti_xblock.py:745
+#: lti_xblock.py:828 lti_xblock.py:842 lti_xblock.py:858
 msgid "Could not get user id for current request"
 msgstr ""
 
-#: lti_xblock.py:850
+#: lti_xblock.py:994
 msgid ""
 "Could not parse custom parameter: {custom_parameter!r}. Should be \"x=y\" "
 "string."
 msgstr ""
 
-#: lti_xblock.py:1310
+#: lti_xblock.py:1343
 msgid "[LTI]: Real user not found against anon_id: {}"
 msgstr ""
 
-#: models.py:72
+#: models.py:79
 msgid "Configuration Stored on XBlock fields"
 msgstr ""
 
-#: models.py:73
+#: models.py:80
 msgid "Configuration Stored on this model"
 msgstr ""
 
-#: models.py:97
+#: models.py:81
+msgid "Configuration Stored on external service"
+msgstr ""
+
+#: models.py:113
 msgid "LTI configuration data."
 msgstr ""
 
-#: models.py:104
+#: models.py:120
 msgid "The URL of the external tool that initiates the launch."
 msgstr ""
 
-#: models.py:109
+#: models.py:125
 msgid "Client key provided by the LTI tool provider."
 msgstr ""
 
-#: models.py:115
+#: models.py:131
 msgid "Client secret provided by the LTI tool provider."
 msgstr ""
 
-#: models.py:121
+#: models.py:137
 msgid "Platform's generated Private key. Keep this value secret."
 msgstr ""
 
-#: models.py:127
+#: models.py:143
 msgid "Platform's generated Private key ID"
 msgstr ""
 
-#: models.py:132
+#: models.py:148
 msgid "Platform's generated JWK keyset."
 msgstr ""
 
-#: models.py:138
+#: models.py:154
 msgid "Client ID used by LTI tool"
 msgstr ""
 
-#: models.py:148
+#: models.py:250
 msgid "LTI Configuration stores on XBlock needs a block location set."
 msgstr ""
 
-#: models.py:155
-msgid "Invalid LTI configuration."
+#: models.py:256
+msgid ""
+"LTI Configuration stored on the model for LTI 1.3 must have a value for one "
+"of lti_1p3_tool_public_key or lti_1p3_tool_keyset_url."
+msgstr ""
+
+#: models.py:263
+msgid ""
+"CONFIG_ON_XBLOCK and CONFIG_EXTERNAL are not supported for LTI 1.3 "
+"Proctoring Services."
 msgstr ""
 
-#: models.py:165
-msgid "Block location not set, it's not possible to retrieve the block."
+#: models.py:271
+msgid "Invalid LTI configuration."
 msgstr ""
 
-#: plugin/views.py:246
+#: plugin/views.py:453
 msgid "The selected content type is not supported by Open edX."
 msgstr ""
 
-#: plugin/views.py:261
+#: plugin/views.py:468
 msgid "You don't have access to save LTI Content Items."
 msgstr ""
 
-#: plugin/views.py:262
+#: plugin/views.py:469
 msgid ""
 "Please check that you have course staff permissions and double check this "
 "block's LTI settings."
 msgstr ""
 
 #: templates/html/lti-dl/dl_response_error.html:6
 msgid "LTI Deep Linking failed."
@@ -467,23 +532,14 @@
 msgid "The LTI Deep Linking content was successfully saved in the LMS."
 msgstr ""
 
 #: templates/html/lti-dl/dl_response_saved.html:13
 msgid "You can safely close this page now."
 msgstr ""
 
-#: templates/html/lti_1p3_launch_error.html:10
-msgid "There was an error while launching the LTI 1.3 tool."
-msgstr ""
-
-#: templates/html/lti_1p3_launch_error.html:13
-msgid ""
-"If you're seeing this on a live course, please contact the course staff."
-msgstr ""
-
 #: templates/html/lti_1p3_permission_error.html:10
 msgid "Unauthorized."
 msgstr ""
 
 #: templates/html/lti_1p3_permission_error.html:13
 msgid ""
 "Students don't have permissions to perform LTI Deep Linking configuration "
@@ -492,16 +548,16 @@
 
 #: templates/html/lti_1p3_studio.html:3
 msgid "LTI 1.3 Launches can only be performed from the LMS."
 msgstr ""
 
 #: templates/html/lti_1p3_studio.html:7
 msgid ""
-"To set up the LTI integration, you need to register the LMS in the tool with "
-"the information provided below."
+"To set up the LTI integration, you need to register the LMS in the tool with"
+" the information provided below."
 msgstr ""
 
 #: templates/html/lti_1p3_studio.html:11
 msgid "Client ID: "
 msgstr ""
 
 #: templates/html/lti_1p3_studio.html:16
@@ -544,28 +600,46 @@
 msgid "Deep Linking Launch - Configure tool"
 msgstr ""
 
 #: templates/html/lti_launch.html:27
 msgid "Press to Launch"
 msgstr ""
 
-#: static/js/xblock_lti_consumer.js:142
-msgid ""
-"Click OK to have your username and e-mail address sent to a 3rd party "
-"application.\n"
-"\n"
-"Click Cancel to return to this page without sending your information."
+#: templates/html/lti_launch_error.html:10
+msgid "There was an error while launching the LTI tool."
 msgstr ""
 
-#: static/js/xblock_lti_consumer.js:144
+#: templates/html/lti_launch_error.html:13
+#: templates/html/lti_proctoring_start_error.html:13
 msgid ""
-"Click OK to have your username sent to a 3rd party application.\n"
-"\n"
-"Click Cancel to return to this page without sending your information."
+"If you're seeing this on a live course, please contact the course staff."
+msgstr ""
+
+#: templates/html/lti_proctoring_start_error.html:10
+msgid "There was an error while starting your LTI proctored assessment."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:126
+msgid "Cancel"
 msgstr ""
 
-#: static/js/xblock_lti_consumer.js:146
+#: static/js/xblock_lti_consumer.js:128
+msgid "OK"
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:157
 msgid ""
-"Click OK to have your e-mail address sent to a 3rd party application.\n"
-"\n"
-"Click Cancel to return to this page without sending your information."
+"Click OK to have your username and e-mail address sent to a 3rd party "
+"application."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:159
+msgid "Click OK to have your username sent to a 3rd party application."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:161
+msgid "Click OK to have your e-mail address sent to a 3rd party application."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:168
+msgid "Click Cancel to return to this page without sending your information."
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/translations/es_419/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.0.2/lti_consumer/translations/es_419/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/translations/es_419/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.2/lti_consumer/translations/es_419/LC_MESSAGES/text.po`

 * *Files 8% similar despite different names*

```diff
@@ -3,462 +3,525 @@
 # This file is distributed under the same license as the PACKAGE package.
 # 
 # Translators:
 # Albeiro Gonzalez <albeiro.gonzalez@edunext.co>, 2018
 # Ana Garcia, 2022
 # Juan Camilo Montoya Franco <juan.montoya@edunext.co>, 2017,2021
 # Laura Silva <lingison@edx.org>, 2016
+# Zach Hancock, 2023
 msgid ""
 msgstr ""
 "Project-Id-Version: XBlocks\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-02-01 17:24-0300\n"
+"POT-Creation-Date: 2023-04-11 15:09-0400\n"
 "PO-Revision-Date: 2016-06-08 14:38+0000\n"
-"Last-Translator: Ana Garcia, 2022\n"
+"Last-Translator: Zach Hancock, 2023\n"
 "Language-Team: Spanish (Latin America) (http://app.transifex.com/open-edx/xblocks/language/es_419/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: es_419\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
-#: lti_1p3/extensions/rest_framework/authentication.py:40
+#: lti_1p3/extensions/rest_framework/authentication.py:41
 msgid "Missing LTI 1.3 authentication token."
 msgstr "El token de autenticación de LTI 1.3 no se encuentra disponible."
 
-#: lti_1p3/extensions/rest_framework/authentication.py:44
+#: lti_1p3/extensions/rest_framework/authentication.py:45
 msgid "Invalid token header. No credentials provided."
 msgstr "Encabezado de token inválido. No se suministraron las credenciales."
 
-#: lti_1p3/extensions/rest_framework/authentication.py:48
+#: lti_1p3/extensions/rest_framework/authentication.py:49
 msgid "Invalid token header. Token string should not contain spaces."
 msgstr "Encabezado de token inválido. La cadena de caracteres del token no debe contener espacios."
 
-#: lti_1p3/extensions/rest_framework/authentication.py:56
+#: lti_1p3/extensions/rest_framework/authentication.py:57
 msgid "LTI configuration not found."
 msgstr "No se encontró la configuración LTI."
 
-#: lti_1p3/extensions/rest_framework/authentication.py:65
+#: lti_1p3/extensions/rest_framework/authentication.py:66
 msgid "Invalid token signature."
 msgstr "Firma de token inválida."
 
-#: lti_xblock.py:127
+#: lti_xblock.py:126
 msgid "No valid user id found in endpoint URL"
 msgstr "No se encontró un id de usuario válido en el URL del endpoint"
 
-#: lti_xblock.py:233
+#: lti_xblock.py:139
+msgid "Configuration on block"
+msgstr ""
+
+#: lti_xblock.py:143
+msgid "Database Configuration"
+msgstr ""
+
+#: lti_xblock.py:146
+msgid "Reusable Configuration"
+msgstr ""
+
+#: lti_xblock.py:253
 msgid "Display Name"
 msgstr "Nombre a mostrar"
 
-#: lti_xblock.py:235
+#: lti_xblock.py:255
 msgid ""
 "Enter the name that students see for this component. Analytics reports may "
 "also use the display name to identify this component."
 msgstr "Ingrese el nombre que los estudiantes verán para este componente. Los reportes de Analytics también pueden utilizar el nombre para mostrar para identificar este componente."
 
-#: lti_xblock.py:239
+#: lti_xblock.py:259
 msgid "LTI Consumer"
 msgstr "Consumidor LTI"
 
-#: lti_xblock.py:242
+#: lti_xblock.py:262
 msgid "LTI Application Information"
 msgstr "Información sobre la aplicación LTI"
 
-#: lti_xblock.py:244
+#: lti_xblock.py:264
 msgid ""
 "Enter a description of the third party application. If requesting username "
 "and/or email, use this text box to inform users why their username and/or "
 "email will be forwarded to a third party application."
 msgstr "Provea una descripción de la aplicación de un tercero. Si se solicita el nombre del usuario o su correo, use este cuadro de texto para informar al usuario que su nombre de usuario y su correo serán redireccionados a una aplicación de un tercero."
 
-#: lti_xblock.py:254
+#: lti_xblock.py:272
+msgid "Configuration Type"
+msgstr ""
+
+#: lti_xblock.py:277
+msgid ""
+"Select 'Configuration on block' to configure a new LTI Tool. If the support "
+"staff provided you with a pre-configured LTI reusable Tool ID, "
+"select'Reusable Configuration' and enter it in the text field below."
+msgstr ""
+
+#: lti_xblock.py:284
 msgid "LTI Version"
 msgstr "Versión LTI"
 
-#: lti_xblock.py:262
+#: lti_xblock.py:292
 msgid ""
 "Select the LTI version that your tool supports.<br />The XBlock LTI Consumer"
 " fully supports LTI 1.1.1, LTI 1.3 and LTI Advantage features."
 msgstr "Seleccione la versión de LTI que su herramienta soporta. <br />El Xblock LTI Consumer soporta completamente las características de LTI 1.1.1, LTI 1.3 y LTI Advantage."
 
-#: lti_xblock.py:268
+#: lti_xblock.py:299
+msgid "LTI Reusable Configuration ID"
+msgstr ""
+
+#: lti_xblock.py:301
+msgid ""
+"Enter the reusable LTI external configuration ID provided by the support "
+"staff."
+msgstr ""
+
+#: lti_xblock.py:306
 msgid "Tool Launch URL"
 msgstr "URL para lanzar la herramienta"
 
-#: lti_xblock.py:272
+#: lti_xblock.py:310
 msgid ""
 "Enter the LTI 1.3 Tool Launch URL. <br />This is the URL the LMS will use to"
 " launch the LTI Tool."
 msgstr "Ingrese la URL para lanzar la herramienta LTI 1.3. <br />Esta es la URL que el LMS usará para abrir la herramienta LTI."
 
-#: lti_xblock.py:277
+#: lti_xblock.py:315
 msgid "Tool Initiate Login URL"
 msgstr "URL para iniciar el login en la herramienta externa"
 
-#: lti_xblock.py:281
+#: lti_xblock.py:319
 msgid ""
 "Enter the LTI 1.3 Tool OIDC Authorization url (can also be called login or "
 "login initiation URL).<br />This is the URL the LMS will use to start a LTI "
 "authorization prior to doing the launch request."
 msgstr "Ingrese la URL de autorización OIDC de la herramienta LTI 1.3 (tambien llamada URL de login, o de inicio de sesión). <br />Esta es la URL que el LMS usará para iniciar la autorización con el componente LTI antes de comenzar."
 
-#: lti_xblock.py:288
+#: lti_xblock.py:325
+msgid "Registered Redirect URIs"
+msgstr ""
+
+#: lti_xblock.py:327
+msgid ""
+"Valid urls the Tool may request us to redirect the id token to. The redirect"
+" uris are often the same as the launch url/deep linking url so if this field"
+" is empty, it will use them as the default. If you need to use different "
+"redirect uri's, enter them here. If you use this field you must enter all "
+"valid redirect uri's the tool may request."
+msgstr ""
+
+#: lti_xblock.py:337
 msgid "Tool Public Key Mode"
 msgstr "Modo de clave pública de la herramienta"
 
-#: lti_xblock.py:296
+#: lti_xblock.py:345
 msgid "Select how the tool's public key information will be specified."
 msgstr "Seleccione cómo se especificará la información de la clave pública de la herramienta."
 
-#: lti_xblock.py:300
+#: lti_xblock.py:349
 msgid "Tool Keyset URL"
 msgstr "URL del conjunto de claves de la herramienta"
 
-#: lti_xblock.py:304
+#: lti_xblock.py:353
 msgid ""
 "Enter the LTI 1.3 Tool's JWK keysets URL.<br />This link should retrieve a "
 "JSON file containing public keys and signature algorithm information, so "
 "that the LMS can check if the messages and launch requests received have the"
 " signature from the tool.<br /><b>This is not required when doing LTI 1.3 "
 "Launches without LTI Advantage nor Basic Outcomes requests.</b>"
 msgstr "Ingrese la clave pública de la herramienta LTI 1.3.<br />Esta cadena de texto comienza con '-----BEGIN PUBLIC KEY-----' y es requerida por el LMS para verificar los mensajes recibidos desde la herramienta externa.<br /><b>No es requerida cuando se hace el lanzamiento de la herramienta sin LTI Advantage ni para peticiones sencillas.</b>"
 
-#: lti_xblock.py:314
+#: lti_xblock.py:363
 msgid "Tool Public Key"
 msgstr "Llave pública de la herramienta"
 
-#: lti_xblock.py:319
+#: lti_xblock.py:368
 msgid ""
 "Enter the LTI 1.3 Tool's public key.<br />This is a string that starts with "
 "'-----BEGIN PUBLIC KEY-----' and is required so that the LMS can check if "
 "the messages and launch requests received have the signature from the "
 "tool.<br /><b>This is not required when doing LTI 1.3 Launches without LTI "
 "Advantage nor Basic Outcomes requests.</b>"
 msgstr "Ingrese la llave pública de la herramienta LTI 1.3.<br />Esta cadena de texto comienza con '-----BEGIN PUBLIC KEY-----' y es requerida por el LMS para verificar los mensajes recibidos desde la herramienta externa.<br /><b>No es requerida cuando se hace el lanzamiento de la herramienta sin LTI Advantage ni para peticiones sencillas.</b>"
 
-#: lti_xblock.py:329
+#: lti_xblock.py:378
 msgid "Enable LTI NRPS"
 msgstr "Habilitar LTI NRPS"
 
-#: lti_xblock.py:330
+#: lti_xblock.py:379
 msgid "Enable LTI Names and Role Provisioning Services."
 msgstr "Habilitar los servicios de provisión de nombres y roles de LTI."
 
-#: lti_xblock.py:337
+#: lti_xblock.py:386
 msgid "LTI 1.3 Block Client ID - DEPRECATED"
 msgstr "LTI 1.3 Block Client ID - DEPRECADO"
 
-#: lti_xblock.py:340
+#: lti_xblock.py:389
 msgid "DEPRECATED - This is now stored in the LtiConfiguration model."
 msgstr "DEPRECADO - Esto ahora se almacena en el modelo LtiConfiguration."
 
-#: lti_xblock.py:343
+#: lti_xblock.py:392
 msgid "LTI 1.3 Block Key - DEPRECATED"
 msgstr "LTI 1.3 Block Key - DEPRECADO"
 
-#: lti_xblock.py:350
+#: lti_xblock.py:399
 msgid "Deep linking"
 msgstr "Deep linking"
 
-#: lti_xblock.py:351
+#: lti_xblock.py:400
 msgid "Select True if you want to enable LTI Advantage Deep Linking."
 msgstr "Seleccione True si desea habiliitar el Deep Linking de LTI Advantage."
 
-#: lti_xblock.py:356
+#: lti_xblock.py:405
 msgid "Deep Linking Launch URL"
 msgstr "URL de lanzamiento para Deep Linking"
 
-#: lti_xblock.py:360
+#: lti_xblock.py:409
 msgid ""
 "Enter the LTI Advantage Deep Linking Launch URL. If the tool does not "
 "specify one, use the same value as 'Tool Launch URL'."
 msgstr "Ingrese la URL de lanzamiento para LTI Advantage Deep Linking. Si la herramienta no especifica una dirección, use la misma dirección URL para lanzamiento de la herramienta."
 
-#: lti_xblock.py:365
+#: lti_xblock.py:414
 msgid "LTI Assignment and Grades Service"
 msgstr "Servicio de Tareas y Calificaciones de LTI"
 
-#: lti_xblock.py:367
+#: lti_xblock.py:416
 msgid "Disabled"
 msgstr "Invalidar"
 
-#: lti_xblock.py:368
+#: lti_xblock.py:417
 msgid "Allow tools to submit grades only (declarative)"
 msgstr "Permite que las herramientas envíen únicamente calificaciones (declarativo)"
 
-#: lti_xblock.py:369
+#: lti_xblock.py:418
 msgid "Allow tools to manage and submit grade (programmatic)"
 msgstr "Permite que las herramientas envíen calificaciones (programático)"
 
-#: lti_xblock.py:374
+#: lti_xblock.py:423
 msgid ""
 "Enable the LTI-AGS service and select the functionality enabled for LTI "
 "tools. The 'declarative' mode (default) will provide a tool with a LineItem "
 "created from the XBlock settings, while the 'programmatic' one will allow "
 "tools to manage, create and link the grades."
 msgstr "Habilite el servicio AGS de LTI y seleccione la funcionalidad habilitada para las herramientas LTI. El modo 'declarativo' (por defecto) le dará una herramienta con un LineItem creado a partir de las configuraciones del Xblock, mientras el modo 'programático' le permitirá a las herramientas administrar, crear y enlazar las calificaciones."
 
-#: lti_xblock.py:382
+#: lti_xblock.py:431
 msgid "LTI ID"
 msgstr "ID de LTI"
 
-#: lti_xblock.py:384
+#: lti_xblock.py:433
 #, python-brace-format
 msgid ""
 "Enter the LTI ID for the external LTI provider. This value must be the same "
 "LTI ID that you entered in the LTI Passports setting on the Advanced "
 "Settings page.<br />See the {docs_anchor_open}edX LTI "
 "documentation{anchor_close} for more details on this setting."
 msgstr "Introduzca el ID LTI para el proveedor LTI externo. Este valor debe ser el mismo ID LTI que ingresó en la configuración de Pasaportes LTI en la página Configuración avanzada.<br />Consulte la {docs_anchor_open} documentación de edX LTI {anchor_close} para obtener más detalles sobre esta configuración."
 
-#: lti_xblock.py:396
+#: lti_xblock.py:445
 msgid "LTI URL"
 msgstr "URL de LTI"
 
-#: lti_xblock.py:398
+#: lti_xblock.py:447
 #, python-brace-format
 msgid ""
 "Enter the URL of the external tool that this component launches. This "
 "setting is only used when Hide External Tool is set to False.<br />See the "
 "{docs_anchor_open}edX LTI documentation{anchor_close} for more details on "
 "this setting."
 msgstr "Ingrese la URL de la herramienta externa que este componente inicia. Esta configuración sólo se utiliza cuando Ocultar herramienta externa se establece en Falso.<br />Consulte la {docs_anchor_open} documentación de edX LTI {anchor_close} para obtener más detalles sobre esta configuración."
 
-#: lti_xblock.py:411
+#: lti_xblock.py:460
 msgid "Custom Parameters"
 msgstr "Parámetros personalizados"
 
-#: lti_xblock.py:413
+#: lti_xblock.py:462
 #, python-brace-format
 msgid ""
 "Add the key/value pair for any custom parameters, such as the page your "
 "e-book should open to or the background color for this component. Ex. "
 "[\"page=1\", \"color=white\"]<br />See the {docs_anchor_open}edX LTI "
 "documentation{anchor_close} for more details on this setting."
 msgstr "Agregue el par clave / valor para cualquier parámetro personalizado, como la página a la que su libro electrónico debe abrirse o el color de fondo para este componente. Ej. [\"page=1\", \"color=white\"]<br />Consulte la {docs_anchor_open} documentación de edX LTI {anchor_close} para obtener más detalles sobre esta configuración"
 
-#: lti_xblock.py:423
+#: lti_xblock.py:472
 msgid "LTI Launch Target"
 msgstr "Target para el LTI"
 
-#: lti_xblock.py:425
+#: lti_xblock.py:474
 msgid ""
 "Select Inline if you want the LTI content to open in an IFrame in the "
 "current page. Select Modal if you want the LTI content to open in a modal "
 "window in the current page. Select New Window if you want the LTI content to"
 " open in a new browser window. This setting is only used when Hide External "
 "Tool is set to False."
 msgstr "Seleccione Inline si desea que el contenido LTI se abra en un IFrame en la página actual. Seleccione Modal si desea que el contenido LTI se abra en una ventana modal en la página actual. Seleccione Nueva ventana si desea que el contenido LTI se abra en una nueva ventana del navegador. Esta configuración sólo se utiliza cuando Ocultar herramienta externa se establece en Falso."
 
-#: lti_xblock.py:439
+#: lti_xblock.py:488
 msgid "Button Text"
 msgstr "Texto para el botón"
 
-#: lti_xblock.py:441
+#: lti_xblock.py:490
 msgid ""
 "Enter the text on the button used to launch the third party application. "
 "This setting is only used when Hide External Tool is set to False and LTI "
 "Launch Target is set to Modal or New Window."
 msgstr "Ingrese el texto en el botón usado para iniciar la aplicación de terceros. Esta opción sólo se utiliza cuando Ocultar herramienta externa se establece en Falso y el Target para el LTI se establece en Modal o Nueva Ventana."
 
-#: lti_xblock.py:449
+#: lti_xblock.py:498
 msgid "Inline Height"
 msgstr "Altura Inline"
 
-#: lti_xblock.py:451
+#: lti_xblock.py:500
 msgid ""
 "Enter the desired pixel height of the iframe which will contain the LTI "
 "tool. This setting is only used when Hide External Tool is set to False and "
 "LTI Launch Target is set to Inline."
 msgstr "Introduzca la altura en píxeles deseada del iframe que contendrá la herramienta LTI. Esta opción sólo se utiliza cuando Ocultar herramienta externa se establece en False y Target para el LTI se establece en Inline."
 
-#: lti_xblock.py:459
+#: lti_xblock.py:508
 msgid "Modal Height"
 msgstr "Altura del modal"
 
-#: lti_xblock.py:461
+#: lti_xblock.py:510
 msgid ""
 "Enter the desired viewport percentage height of the modal overlay which will"
 " contain the LTI tool. This setting is only used when Hide External Tool is "
 "set to False and LTI Launch Target is set to Modal."
 msgstr "Ingrese la altura de porcentaje de visualización deseada de la superposición modal que contendrá la herramienta LTI. Esta opción sólo se utiliza cuando Ocultar herramienta externa se establece en False y Target para el LTI se establece en Modal."
 
-#: lti_xblock.py:469
+#: lti_xblock.py:518
 msgid "Modal Width"
 msgstr "Ancho del modal"
 
-#: lti_xblock.py:471
+#: lti_xblock.py:520
 msgid ""
 "Enter the desired viewport percentage width of the modal overlay which will "
 "contain the LTI tool. This setting is only used when Hide External Tool is "
 "set to False and LTI Launch Target is set to Modal."
 msgstr "Ingrese el ancho de porcentaje de la ventana de visualización de la superposición modal que contendrá la herramienta LTI. Esta opción sólo se utiliza cuando Ocultar herramienta externa se establece en False y Target para el LTI se establece en Modal."
 
-#: lti_xblock.py:479
+#: lti_xblock.py:528
 msgid "Scored"
 msgstr "Puntuado"
 
-#: lti_xblock.py:480
+#: lti_xblock.py:529
 msgid ""
 "Select True if this component will receive a numerical score from the "
 "external LTI system."
 msgstr "Seleccione True si este componente recibirá una puntuación numérica desde un sistema LTI externo."
 
-#: lti_xblock.py:487
+#: lti_xblock.py:536
 msgid ""
 "Enter the number of points possible for this component.  The default value "
 "is 1.0.  This setting is only used when Scored is set to True."
 msgstr "Ingrese el número de puntos posibles para este componente. El valor por defecto es 1.0. Este valor solo se utiliza cuando el parámetro de calificación está definido como True."
 
-#: lti_xblock.py:496
+#: lti_xblock.py:545
 msgid ""
 "The score kept in the xblock KVS -- duplicate of the published score in "
 "django DB"
 msgstr "La calificación almacenada en xblock KVS -- un duplicado de la calificación publicada en django DB"
 
-#: lti_xblock.py:501
+#: lti_xblock.py:550
 msgid "Comment as returned from grader, LTI2.0 spec"
 msgstr "El comentario tal y como fue enviado por el evaluador, LTI2.0 spec"
 
-#: lti_xblock.py:506
+#: lti_xblock.py:555
 msgid "Hide External Tool"
 msgstr "Ocultar la herramienta externa"
 
-#: lti_xblock.py:508
+#: lti_xblock.py:557
 msgid ""
 "Select True if you want to use this component as a placeholder for syncing "
 "with an external grading  system rather than launch an external tool.  This "
 "setting hides the Launch button and any IFrames for this component."
 msgstr "Seleccione True si desea usar este componente como marcador para sincronizarse con un servicio externo en lugar de lanzar una herramienta externa. Esta opción oculta el botón de Lanzar y cualquier iframe para este componente."
 
-#: lti_xblock.py:516
+#: lti_xblock.py:565
 msgid "Accept grades past deadline"
 msgstr "Aceptar notas después de la fecha límite"
 
-#: lti_xblock.py:517
+#: lti_xblock.py:566
 msgid ""
 "Select True to allow third party systems to post grades past the deadline."
 msgstr "Seleccione True para permitir que sistemas de terceros publiquen calificaciones después de la fecha límite."
 
-#: lti_xblock.py:525
+#: lti_xblock.py:574
 msgid "Request user's username"
 msgstr "Solicite el nombre público del usuario"
 
 #. Translators: This is used to request the user's username for a third party
 #. service.
-#: lti_xblock.py:527
+#: lti_xblock.py:576
 msgid "Select True to request the user's username."
 msgstr "Seleccione True para solicitar el nombre de usuario."
 
-#: lti_xblock.py:532
+#: lti_xblock.py:581
 msgid "Request user's email"
 msgstr "Solicitar la dirección de correo del usuario"
 
 #. Translators: This is used to request the user's email for a third party
 #. service.
-#: lti_xblock.py:534
+#: lti_xblock.py:583
 msgid "Select True to request the user's email address."
 msgstr "Seleccione True para solicitar el correo electrónico del usuario."
 
-#: lti_xblock.py:539
+#: lti_xblock.py:588
 msgid "Send extra parameters"
 msgstr "Enviar parámetros adicionales"
 
-#: lti_xblock.py:540
+#: lti_xblock.py:589
 msgid ""
 "Select True to send the extra parameters, which might contain Personally "
 "Identifiable Information. The processors are site-wide, please consult the "
 "site administrator if you have any questions."
 msgstr "Seleccione True praa enviar los parámetros adicionales, los cuales pueden contener información de identificación personal. Los procesadores son para todo el sitio, por favor consulte al administrador del sitio si tiene cualquier pregunta."
 
-#: lti_xblock.py:603
+#: lti_xblock.py:652
 msgid "Custom Parameters must be a list"
 msgstr "Los parámetros personalizados deben ser una lista"
 
-#: lti_xblock.py:713
+#: lti_xblock.py:783 lti_xblock.py:1062
+msgid "Could not get user data for current request"
+msgstr ""
+
+#: lti_xblock.py:810
 msgid ""
 "Could not parse LTI passport: {lti_passport!r}. Should be \"id:key:secret\" "
 "string."
 msgstr "No fué posible parsear el pasaporte LTI: {lti_passport!r}. Debería ser una cadena de tipo \"id:key:secret\"."
 
-#: lti_xblock.py:729 lti_xblock.py:745
+#: lti_xblock.py:828 lti_xblock.py:842 lti_xblock.py:858
 msgid "Could not get user id for current request"
 msgstr "No se pudo obtener el id de usuario para esta petición"
 
-#: lti_xblock.py:850
+#: lti_xblock.py:994
 msgid ""
 "Could not parse custom parameter: {custom_parameter!r}. Should be \"x=y\" "
 "string."
 msgstr "No fué posible parsear el parametro: {custom_parameter!r}. Debería ser una cadena tipo \"x=y\"."
 
-#: lti_xblock.py:1310
+#: lti_xblock.py:1343
 msgid "[LTI]: Real user not found against anon_id: {}"
 msgstr "[LTI]: No se encontró un usuario que coincidiera con anon_id: {}"
 
-#: models.py:72
+#: models.py:79
 msgid "Configuration Stored on XBlock fields"
 msgstr "Configuración almacenada en campos de XBlocks"
 
-#: models.py:73
+#: models.py:80
 msgid "Configuration Stored on this model"
 msgstr "Configuración almacenada en este modelo"
 
-#: models.py:97
+#: models.py:81
+msgid "Configuration Stored on external service"
+msgstr ""
+
+#: models.py:113
 msgid "LTI configuration data."
 msgstr "Datos de configuración de LTI"
 
-#: models.py:104
+#: models.py:120
 msgid "The URL of the external tool that initiates the launch."
 msgstr "URL de la herramienta externa que inicia el lanzamiento."
 
-#: models.py:109
+#: models.py:125
 msgid "Client key provided by the LTI tool provider."
 msgstr "Llave de cliente suministrada por el proveedor de la herramienta LTI."
 
-#: models.py:115
+#: models.py:131
 msgid "Client secret provided by the LTI tool provider."
 msgstr "Secreto de cliente suministrado por el proveedor de la herramienta LTI."
 
-#: models.py:121
+#: models.py:137
 msgid "Platform's generated Private key. Keep this value secret."
 msgstr "Llave privada generada para la plataforma. Mantenga este valor en secreto."
 
-#: models.py:127
+#: models.py:143
 msgid "Platform's generated Private key ID"
 msgstr "Llave privada generada para la plataforma."
 
-#: models.py:132
+#: models.py:148
 msgid "Platform's generated JWK keyset."
 msgstr "JWK keyset generado para la plataforma"
 
-#: models.py:138
+#: models.py:154
 msgid "Client ID used by LTI tool"
 msgstr "ID del cliente usado por la herramienta LTI"
 
-#: models.py:148
+#: models.py:250
 msgid "LTI Configuration stores on XBlock needs a block location set."
 msgstr "Las configuraciones LTI para XBlock necesitan una ubicación de bloque."
 
-#: models.py:155
+#: models.py:256
+msgid ""
+"LTI Configuration stored on the model for LTI 1.3 must have a value for one "
+"of lti_1p3_tool_public_key or lti_1p3_tool_keyset_url."
+msgstr ""
+
+#: models.py:263
+msgid ""
+"CONFIG_ON_XBLOCK and CONFIG_EXTERNAL are not supported for LTI 1.3 "
+"Proctoring Services."
+msgstr ""
+
+#: models.py:271
 msgid "Invalid LTI configuration."
 msgstr "Configuración LTI inválida"
 
-#: models.py:165
-msgid "Block location not set, it's not possible to retrieve the block."
-msgstr "No se definió la ubicación del bloque, por lo que no es posible encontrar el bloque"
-
-#: plugin/views.py:246
+#: plugin/views.py:453
 msgid "The selected content type is not supported by Open edX."
 msgstr "El tipo de contenido seleccionado no está soportado por Open edX."
 
-#: plugin/views.py:261
+#: plugin/views.py:468
 msgid "You don't have access to save LTI Content Items."
 msgstr "Usted no tiene acceso para guardar items de contenido LTI."
 
-#: plugin/views.py:262
+#: plugin/views.py:469
 msgid ""
 "Please check that you have course staff permissions and double check this "
 "block's LTI settings."
 msgstr "Por favor verifique que tiene permisos de staff en el curso y confirme las configuraciones de LTI para este bloque."
 
 #: templates/html/lti-dl/dl_response_error.html:6
 msgid "LTI Deep Linking failed."
@@ -472,23 +535,14 @@
 msgid "The LTI Deep Linking content was successfully saved in the LMS."
 msgstr "El contenido de Deep Linking de LTI fué guardado con exito en el LMS."
 
 #: templates/html/lti-dl/dl_response_saved.html:13
 msgid "You can safely close this page now."
 msgstr "Puede cerrar esta página ahora."
 
-#: templates/html/lti_1p3_launch_error.html:10
-msgid "There was an error while launching the LTI 1.3 tool."
-msgstr "Ocurrió un error al lanzar la herramienta LTI 1.3."
-
-#: templates/html/lti_1p3_launch_error.html:13
-msgid ""
-"If you're seeing this on a live course, please contact the course staff."
-msgstr "Si usted está viendo esto en un curso en vivo, por favor contacte al equipo del curso."
-
 #: templates/html/lti_1p3_permission_error.html:10
 msgid "Unauthorized."
 msgstr "No autorizado."
 
 #: templates/html/lti_1p3_permission_error.html:13
 msgid ""
 "Students don't have permissions to perform LTI Deep Linking configuration "
@@ -549,27 +603,46 @@
 msgid "Deep Linking Launch - Configure tool"
 msgstr "Herramienta de configuración para lanzamiento de Deep Linking"
 
 #: templates/html/lti_launch.html:27
 msgid "Press to Launch"
 msgstr "Pulsar para iniciar"
 
-#: static/js/xblock_lti_consumer.js:142
+#: templates/html/lti_launch_error.html:10
+msgid "There was an error while launching the LTI tool."
+msgstr ""
+
+#: templates/html/lti_launch_error.html:13
+#: templates/html/lti_proctoring_start_error.html:13
 msgid ""
-"Click OK to have your username and e-mail address sent to a 3rd party application.\n"
-"\n"
-"Click Cancel to return to this page without sending your information."
-msgstr "Haz Clic en ACEPTAR para que tu nombre de usuario y correo electrónico sean enviados a una aplicación de 3ros.\n\nHaz Clic en CANCELAR para volver a está página sin que se que envíe su información."
-
-#: static/js/xblock_lti_consumer.js:144
-msgid ""
-"Click OK to have your username sent to a 3rd party application.\n"
-"\n"
-"Click Cancel to return to this page without sending your information."
-msgstr "Haz Clic en ACEPTAR para que su nombre de usuario sea enviado a una aplicación de 3ros.\n\nHaz Clic en CANCELAR para volver a está página sin que se que envíe su información."
-
-#: static/js/xblock_lti_consumer.js:146
-msgid ""
-"Click OK to have your e-mail address sent to a 3rd party application.\n"
-"\n"
-"Click Cancel to return to this page without sending your information."
-msgstr "Haz Clic en ACEPTAR para que tu correo electrónico sea enviado a una aplicación de 3ros.\n\nHaz Clic en CANCELAR para volver a está página sin que se que envíe su información."
+"If you're seeing this on a live course, please contact the course staff."
+msgstr "Si usted está viendo esto en un curso en vivo, por favor contacte al equipo del curso."
+
+#: templates/html/lti_proctoring_start_error.html:10
+msgid "There was an error while starting your LTI proctored assessment."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:126
+msgid "Cancel"
+msgstr "Cancelar"
+
+#: static/js/xblock_lti_consumer.js:128
+msgid "OK"
+msgstr "Aceptar"
+
+#: static/js/xblock_lti_consumer.js:157
+msgid ""
+"Click OK to have your username and e-mail address sent to a 3rd party "
+"application."
+msgstr "Haz Clic en ACEPTAR para que tu nombre de usuario y correo electrónico sean enviados a una aplicación de 3ros."
+
+#: static/js/xblock_lti_consumer.js:159
+msgid "Click OK to have your username sent to a 3rd party application."
+msgstr "Haz Clic en ACEPTAR para que su nombre de usuario sea enviado a una aplicación de 3ros."
+
+#: static/js/xblock_lti_consumer.js:161
+msgid "Click OK to have your e-mail address sent to a 3rd party application."
+msgstr "Haz Clic en ACEPTAR para que tu correo electrónico sea enviado a una aplicación de 3ros."
+
+#: static/js/xblock_lti_consumer.js:168
+msgid "Click Cancel to return to this page without sending your information."
+msgstr "Clic en CANCELAR para volver a está página sin que se que envíe su información."
```

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/translations/fr/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.0.2/lti_consumer/translations/fr/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/translations/fr/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.2/lti_consumer/translations/fr/LC_MESSAGES/text.po`

 * *Files 8% similar despite different names*

```diff
@@ -6,458 +6,520 @@
 # Abdessamad Derraz <derraz.abdessamad@gmail.com>, 2021
 # Jorg722, 2022
 # willyedoo <willyedoo@gmail.com>, 2019
 msgid ""
 msgstr ""
 "Project-Id-Version: XBlocks\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-02-01 17:24-0300\n"
+"POT-Creation-Date: 2023-04-11 15:09-0400\n"
 "PO-Revision-Date: 2016-06-08 14:38+0000\n"
 "Last-Translator: Jorg722, 2022\n"
 "Language-Team: French (http://app.transifex.com/open-edx/xblocks/language/fr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: fr\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
-#: lti_1p3/extensions/rest_framework/authentication.py:40
+#: lti_1p3/extensions/rest_framework/authentication.py:41
 msgid "Missing LTI 1.3 authentication token."
 msgstr "Jeton d'authentification LTI 1.3 manquant."
 
-#: lti_1p3/extensions/rest_framework/authentication.py:44
+#: lti_1p3/extensions/rest_framework/authentication.py:45
 msgid "Invalid token header. No credentials provided."
 msgstr "En-tête de jeton non valide. Aucune information d'identification fournie."
 
-#: lti_1p3/extensions/rest_framework/authentication.py:48
+#: lti_1p3/extensions/rest_framework/authentication.py:49
 msgid "Invalid token header. Token string should not contain spaces."
 msgstr "En-tête de jeton non valide. La chaîne de jeton ne doit pas contenir d'espaces."
 
-#: lti_1p3/extensions/rest_framework/authentication.py:56
+#: lti_1p3/extensions/rest_framework/authentication.py:57
 msgid "LTI configuration not found."
 msgstr "Configuration LTI introuvable."
 
-#: lti_1p3/extensions/rest_framework/authentication.py:65
+#: lti_1p3/extensions/rest_framework/authentication.py:66
 msgid "Invalid token signature."
 msgstr "Signature de jeton non valide."
 
-#: lti_xblock.py:127
+#: lti_xblock.py:126
 msgid "No valid user id found in endpoint URL"
 msgstr "Aucun ID utilisateur valide trouvé dans l'URL cible"
 
-#: lti_xblock.py:233
+#: lti_xblock.py:139
+msgid "Configuration on block"
+msgstr ""
+
+#: lti_xblock.py:143
+msgid "Database Configuration"
+msgstr ""
+
+#: lti_xblock.py:146
+msgid "Reusable Configuration"
+msgstr ""
+
+#: lti_xblock.py:253
 msgid "Display Name"
 msgstr "Nom d'affichage"
 
-#: lti_xblock.py:235
+#: lti_xblock.py:255
 msgid ""
 "Enter the name that students see for this component. Analytics reports may "
 "also use the display name to identify this component."
 msgstr "Entrez le nom que les étudiants voient pour ce composant. Les rapports d'analyse peuvent également utiliser le nom d'affichage pour identifier ce composant."
 
-#: lti_xblock.py:239
+#: lti_xblock.py:259
 msgid "LTI Consumer"
 msgstr "Client LTI"
 
-#: lti_xblock.py:242
+#: lti_xblock.py:262
 msgid "LTI Application Information"
 msgstr "Information sur l'application LTI"
 
-#: lti_xblock.py:244
+#: lti_xblock.py:264
 msgid ""
 "Enter a description of the third party application. If requesting username "
 "and/or email, use this text box to inform users why their username and/or "
 "email will be forwarded to a third party application."
 msgstr "Saisir une description de l'application tierce. Si vous demandez le nom d'utilisateur et/ou le mail, utilisez cette zone de texte pour informer les utilisateurs que leur nom d'utilisateur et/ou le mail seront transmis à une application tierce."
 
-#: lti_xblock.py:254
+#: lti_xblock.py:272
+msgid "Configuration Type"
+msgstr ""
+
+#: lti_xblock.py:277
+msgid ""
+"Select 'Configuration on block' to configure a new LTI Tool. If the support "
+"staff provided you with a pre-configured LTI reusable Tool ID, "
+"select'Reusable Configuration' and enter it in the text field below."
+msgstr ""
+
+#: lti_xblock.py:284
 msgid "LTI Version"
 msgstr "Version LTI"
 
-#: lti_xblock.py:262
+#: lti_xblock.py:292
 msgid ""
 "Select the LTI version that your tool supports.<br />The XBlock LTI Consumer"
 " fully supports LTI 1.1.1, LTI 1.3 and LTI Advantage features."
 msgstr "Sélectionnez la version LTI prise en charge par votre outil.<br />Le consommateur XBlock LTI prend entièrement en charge les fonctionnalités LTI 1.1.1, LTI 1.3 et LTI Advantage."
 
-#: lti_xblock.py:268
+#: lti_xblock.py:299
+msgid "LTI Reusable Configuration ID"
+msgstr ""
+
+#: lti_xblock.py:301
+msgid ""
+"Enter the reusable LTI external configuration ID provided by the support "
+"staff."
+msgstr ""
+
+#: lti_xblock.py:306
 msgid "Tool Launch URL"
 msgstr "URL de lancement de l'outil"
 
-#: lti_xblock.py:272
+#: lti_xblock.py:310
 msgid ""
 "Enter the LTI 1.3 Tool Launch URL. <br />This is the URL the LMS will use to"
 " launch the LTI Tool."
 msgstr "Entrez l'URL de lancement de l'outil LTI 1.3. <br /> Il s'agit de l'URL que le LMS utilisera pour lancer l'outil LTI."
 
-#: lti_xblock.py:277
+#: lti_xblock.py:315
 msgid "Tool Initiate Login URL"
 msgstr "URL d'ouverture de session de l'outil"
 
-#: lti_xblock.py:281
+#: lti_xblock.py:319
 msgid ""
 "Enter the LTI 1.3 Tool OIDC Authorization url (can also be called login or "
 "login initiation URL).<br />This is the URL the LMS will use to start a LTI "
 "authorization prior to doing the launch request."
 msgstr "Entrez l'URL d'autorisation OIDC de l'outil LTI 1.3 (peut également être appelée URL de connexion ou URL d'initiation de connexion).<br /> Il s'agit de l'URL que le LMS utilisera pour démarrer une autorisation LTI avant de faire la demande de lancement."
 
-#: lti_xblock.py:288
+#: lti_xblock.py:325
+msgid "Registered Redirect URIs"
+msgstr ""
+
+#: lti_xblock.py:327
+msgid ""
+"Valid urls the Tool may request us to redirect the id token to. The redirect"
+" uris are often the same as the launch url/deep linking url so if this field"
+" is empty, it will use them as the default. If you need to use different "
+"redirect uri's, enter them here. If you use this field you must enter all "
+"valid redirect uri's the tool may request."
+msgstr ""
+
+#: lti_xblock.py:337
 msgid "Tool Public Key Mode"
 msgstr ""
 
-#: lti_xblock.py:296
+#: lti_xblock.py:345
 msgid "Select how the tool's public key information will be specified."
 msgstr ""
 
-#: lti_xblock.py:300
+#: lti_xblock.py:349
 msgid "Tool Keyset URL"
 msgstr ""
 
-#: lti_xblock.py:304
+#: lti_xblock.py:353
 msgid ""
 "Enter the LTI 1.3 Tool's JWK keysets URL.<br />This link should retrieve a "
 "JSON file containing public keys and signature algorithm information, so "
 "that the LMS can check if the messages and launch requests received have the"
 " signature from the tool.<br /><b>This is not required when doing LTI 1.3 "
 "Launches without LTI Advantage nor Basic Outcomes requests.</b>"
 msgstr ""
 
-#: lti_xblock.py:314
+#: lti_xblock.py:363
 msgid "Tool Public Key"
 msgstr "Clé publique de l'outil"
 
-#: lti_xblock.py:319
+#: lti_xblock.py:368
 msgid ""
 "Enter the LTI 1.3 Tool's public key.<br />This is a string that starts with "
 "'-----BEGIN PUBLIC KEY-----' and is required so that the LMS can check if "
 "the messages and launch requests received have the signature from the "
 "tool.<br /><b>This is not required when doing LTI 1.3 Launches without LTI "
 "Advantage nor Basic Outcomes requests.</b>"
 msgstr "Entrez la clé publique de l'outil LTI 1.3.<br />Ceci est une chaîne qui commence par '-----BEGIN PUBLIC KEY-----' et est nécessaire pour que le LMS puisse vérifier si les messages et demandes de lancement reçus ont la signature de l'outil.<br /><b>Cela n'est pas nécessaire lors des lancements LTI 1.3 sans LTI Advantage ni demandes Basic Outcomes.</b>"
 
-#: lti_xblock.py:329
+#: lti_xblock.py:378
 msgid "Enable LTI NRPS"
 msgstr "Activer LTI NRPS"
 
-#: lti_xblock.py:330
+#: lti_xblock.py:379
 msgid "Enable LTI Names and Role Provisioning Services."
 msgstr "Activez les LTI Names et les services de provisionnement de rôles."
 
-#: lti_xblock.py:337
+#: lti_xblock.py:386
 msgid "LTI 1.3 Block Client ID - DEPRECATED"
 msgstr "LTI 1.3 Block Client ID - OBSOLÈTE"
 
-#: lti_xblock.py:340
+#: lti_xblock.py:389
 msgid "DEPRECATED - This is now stored in the LtiConfiguration model."
 msgstr "OBSOLÈTE - Ceci est maintenant stocké dans le modèle LtiConfiguration."
 
-#: lti_xblock.py:343
+#: lti_xblock.py:392
 msgid "LTI 1.3 Block Key - DEPRECATED"
 msgstr "LTI 1.3 Block Key - OBSOLÈTE"
 
-#: lti_xblock.py:350
+#: lti_xblock.py:399
 msgid "Deep linking"
 msgstr "Deep linking"
 
-#: lti_xblock.py:351
+#: lti_xblock.py:400
 msgid "Select True if you want to enable LTI Advantage Deep Linking."
 msgstr "Sélectionnez Vrai si vous souhaitez activer LTI Advantage Deep Linking."
 
-#: lti_xblock.py:356
+#: lti_xblock.py:405
 msgid "Deep Linking Launch URL"
 msgstr "URL de lancement Deep Linking"
 
-#: lti_xblock.py:360
+#: lti_xblock.py:409
 msgid ""
 "Enter the LTI Advantage Deep Linking Launch URL. If the tool does not "
 "specify one, use the same value as 'Tool Launch URL'."
 msgstr "Saisissez l'URL de lancement LTI Advantage Deep Linking. Si l'outil n'en spécifie pas, utilisez la même valeur que « URL de lancement de l'outil »."
 
-#: lti_xblock.py:365
+#: lti_xblock.py:414
 msgid "LTI Assignment and Grades Service"
 msgstr "Service d'affectation et de notes LTI"
 
-#: lti_xblock.py:367
+#: lti_xblock.py:416
 msgid "Disabled"
 msgstr "Désactivé"
 
-#: lti_xblock.py:368
+#: lti_xblock.py:417
 msgid "Allow tools to submit grades only (declarative)"
 msgstr "Autoriser les outils à soumettre des notes uniquement (déclaratif)"
 
-#: lti_xblock.py:369
+#: lti_xblock.py:418
 msgid "Allow tools to manage and submit grade (programmatic)"
 msgstr "Autoriser les outils à gérer et soumettre la note (programmatique)"
 
-#: lti_xblock.py:374
+#: lti_xblock.py:423
 msgid ""
 "Enable the LTI-AGS service and select the functionality enabled for LTI "
 "tools. The 'declarative' mode (default) will provide a tool with a LineItem "
 "created from the XBlock settings, while the 'programmatic' one will allow "
 "tools to manage, create and link the grades."
 msgstr "Activez le service LTI-AGS et sélectionnez la fonctionnalité activée pour les outils LTI. Le mode \"déclaratif\" (par défaut) fournira un outil avec un élément de ligne créé à partir des paramètres XBlock, tandis que le mode \"programmatique\" permettra aux outils de gérer, créer et lier les notes."
 
-#: lti_xblock.py:382
+#: lti_xblock.py:431
 msgid "LTI ID"
 msgstr "identifiant LTI"
 
-#: lti_xblock.py:384
+#: lti_xblock.py:433
 #, python-brace-format
 msgid ""
 "Enter the LTI ID for the external LTI provider. This value must be the same "
 "LTI ID that you entered in the LTI Passports setting on the Advanced "
 "Settings page.<br />See the {docs_anchor_open}edX LTI "
 "documentation{anchor_close} for more details on this setting."
 msgstr "Entrez l'ID LTI du fournisseur LTI externe. Cette valeur doit être identique à l'ID LTI que vous avez entré dans le paramètre LTI Passports de la page des paramètres avancés.<br />Voir {docs_anchor_open}edX LTI documentation{anchor_close} pour plus de détails sur ce paramètre."
 
-#: lti_xblock.py:396
+#: lti_xblock.py:445
 msgid "LTI URL"
 msgstr "URL LTI"
 
-#: lti_xblock.py:398
+#: lti_xblock.py:447
 #, python-brace-format
 msgid ""
 "Enter the URL of the external tool that this component launches. This "
 "setting is only used when Hide External Tool is set to False.<br />See the "
 "{docs_anchor_open}edX LTI documentation{anchor_close} for more details on "
 "this setting."
 msgstr "Entrez l'URL de l'outil externe que ce composant lance. Ce paramètre est uniquement utilisé lorsque l'option Masquer l'outil externe est définie sur False.<br />Voir {docs_anchor_open}edX LTI documentation{anchor_close} pour plus de détails sur ce paramètre."
 
-#: lti_xblock.py:411
+#: lti_xblock.py:460
 msgid "Custom Parameters"
 msgstr "Paramètres personnalisés"
 
-#: lti_xblock.py:413
+#: lti_xblock.py:462
 #, python-brace-format
 msgid ""
 "Add the key/value pair for any custom parameters, such as the page your "
 "e-book should open to or the background color for this component. Ex. "
 "[\"page=1\", \"color=white\"]<br />See the {docs_anchor_open}edX LTI "
 "documentation{anchor_close} for more details on this setting."
 msgstr "Ajoutez la paire clé / valeur pour tous les paramètres personnalisés, tels que la page que votre livre électronique doit ouvrir ou la couleur d'arrière-plan de ce composant. Ex. [\"page=1\", \"color=white\"]<br />Voir {docs_anchor_open}edX LTI documentation{anchor_close} pour plus de détails sur ce paramètre."
 
-#: lti_xblock.py:423
+#: lti_xblock.py:472
 msgid "LTI Launch Target"
 msgstr "Lancer la cible LTI"
 
-#: lti_xblock.py:425
+#: lti_xblock.py:474
 msgid ""
 "Select Inline if you want the LTI content to open in an IFrame in the "
 "current page. Select Modal if you want the LTI content to open in a modal "
 "window in the current page. Select New Window if you want the LTI content to"
 " open in a new browser window. This setting is only used when Hide External "
 "Tool is set to False."
 msgstr "Sélectionnez Inline si vous souhaitez que le contenu LTI s'ouvre dans un IFrame de la page en cours. Sélectionnez Modal si vous souhaitez que le contenu LTI s'ouvre dans une fenêtre modale de la page en cours. Sélectionnez Nouvelle Fenêtre si vous souhaitez que le contenu LTI s'ouvre dans une nouvelle fenêtre du navigateur. Ce paramètre est uniquement utilisé lorsque l'option masquer l'outil externe est définie sur False."
 
-#: lti_xblock.py:439
+#: lti_xblock.py:488
 msgid "Button Text"
 msgstr "Texte du bouton"
 
-#: lti_xblock.py:441
+#: lti_xblock.py:490
 msgid ""
 "Enter the text on the button used to launch the third party application. "
 "This setting is only used when Hide External Tool is set to False and LTI "
 "Launch Target is set to Modal or New Window."
 msgstr "Entrez le texte du bouton qui sera utilisé pour lancer l'application tierce. Ce paramètre est utilisé uniquement lorsque masquer l'outil externe est défini sur False et que LTI Launch Target est défini sur Modal ou Nouvelle fenêtre."
 
-#: lti_xblock.py:449
+#: lti_xblock.py:498
 msgid "Inline Height"
 msgstr "Hauteur intégré"
 
-#: lti_xblock.py:451
+#: lti_xblock.py:500
 msgid ""
 "Enter the desired pixel height of the iframe which will contain the LTI "
 "tool. This setting is only used when Hide External Tool is set to False and "
 "LTI Launch Target is set to Inline."
 msgstr "Entrez la hauteur de pixel souhaitée de l'iframe qui contiendra l'outil LTI. Ce paramètre est uniquement utilisé lorsque masquer l'outil externe est défini sur False et que LTI Launch Target est défini sur Inline."
 
-#: lti_xblock.py:459
+#: lti_xblock.py:508
 msgid "Modal Height"
 msgstr "Hauteur modale"
 
-#: lti_xblock.py:461
+#: lti_xblock.py:510
 msgid ""
 "Enter the desired viewport percentage height of the modal overlay which will"
 " contain the LTI tool. This setting is only used when Hide External Tool is "
 "set to False and LTI Launch Target is set to Modal."
 msgstr "Entrez le pourcentage de hauteur de la fenêtre de visualisation de la superposition modale qui contiendra l’outil LTI. Ce paramètre est uniquement utilisé lorsque masquer l'outil externe est défini sur False et que LTI Launch Target est défini sur Modal."
 
-#: lti_xblock.py:469
+#: lti_xblock.py:518
 msgid "Modal Width"
 msgstr "Largeur modale"
 
-#: lti_xblock.py:471
+#: lti_xblock.py:520
 msgid ""
 "Enter the desired viewport percentage width of the modal overlay which will "
 "contain the LTI tool. This setting is only used when Hide External Tool is "
 "set to False and LTI Launch Target is set to Modal."
 msgstr "Entrez le pourcentage de largeur de la fenêtre de superposition modale qui contiendra l’outil LTI. Ce paramètre est uniquement utilisé lorsque masquer l'outil externe est défini sur False et que LTI Launch Target est défini sur Modal."
 
-#: lti_xblock.py:479
+#: lti_xblock.py:528
 msgid "Scored"
 msgstr "A obtenu"
 
-#: lti_xblock.py:480
+#: lti_xblock.py:529
 msgid ""
 "Select True if this component will receive a numerical score from the "
 "external LTI system."
 msgstr "Sélectionnez Vrai si ce composant doit recevoir un score numérique du système LTI externe."
 
-#: lti_xblock.py:487
+#: lti_xblock.py:536
 msgid ""
 "Enter the number of points possible for this component.  The default value "
 "is 1.0.  This setting is only used when Scored is set to True."
 msgstr "Entrez le nombre de points possible pour ce composant. La valeur par défaut est de 1,0. Ce paramètre est utilisé uniquement lorsque Noté est positionné sur Vrai."
 
-#: lti_xblock.py:496
+#: lti_xblock.py:545
 msgid ""
 "The score kept in the xblock KVS -- duplicate of the published score in "
 "django DB"
 msgstr "Le score conservé dans le xBlock KVS - duplicata du score publié dans django DB"
 
-#: lti_xblock.py:501
+#: lti_xblock.py:550
 msgid "Comment as returned from grader, LTI2.0 spec"
 msgstr "Commentaire sous la forme retourné par l'évaluateur, spécification LTI2.0"
 
-#: lti_xblock.py:506
+#: lti_xblock.py:555
 msgid "Hide External Tool"
 msgstr "Cacher l'outil externe"
 
-#: lti_xblock.py:508
+#: lti_xblock.py:557
 msgid ""
 "Select True if you want to use this component as a placeholder for syncing "
 "with an external grading  system rather than launch an external tool.  This "
 "setting hides the Launch button and any IFrames for this component."
 msgstr "Sélectionnez Vrai si vous voulez utiliser ce composant comme un espace réservé pour la synchronisation avec un système de notation externe plutôt que de lancer un outil externe. Ce paramètre masque le bouton de lancement ainsi que tous les IFrames pour ce composant."
 
-#: lti_xblock.py:516
+#: lti_xblock.py:565
 msgid "Accept grades past deadline"
 msgstr "Accepter les notes après la date limite"
 
-#: lti_xblock.py:517
+#: lti_xblock.py:566
 msgid ""
 "Select True to allow third party systems to post grades past the deadline."
 msgstr "Sélectionner vrai (true) pour permettre aux systèmes tierces de poster des notes après la date limite."
 
-#: lti_xblock.py:525
+#: lti_xblock.py:574
 msgid "Request user's username"
 msgstr "Demander le nom de l'utilisateur"
 
 #. Translators: This is used to request the user's username for a third party
 #. service.
-#: lti_xblock.py:527
+#: lti_xblock.py:576
 msgid "Select True to request the user's username."
 msgstr "Choisir vrai (true) afin de demander le nom d'utilisateur."
 
-#: lti_xblock.py:532
+#: lti_xblock.py:581
 msgid "Request user's email"
 msgstr "Demander l'e-mail de l'utilisateur"
 
 #. Translators: This is used to request the user's email for a third party
 #. service.
-#: lti_xblock.py:534
+#: lti_xblock.py:583
 msgid "Select True to request the user's email address."
 msgstr "Choisir vrai (true) afin de demander l'adresse e-mail de l'utilisateur."
 
-#: lti_xblock.py:539
+#: lti_xblock.py:588
 msgid "Send extra parameters"
 msgstr "Envoyer des paramètres supplémentaires"
 
-#: lti_xblock.py:540
+#: lti_xblock.py:589
 msgid ""
 "Select True to send the extra parameters, which might contain Personally "
 "Identifiable Information. The processors are site-wide, please consult the "
 "site administrator if you have any questions."
 msgstr "Sélectionnez Vrai pour envoyer les paramètres supplémentaires, qui peuvent contenir des informations personnellement identifiables. Les processeurs sont à l'échelle du site, veuillez consulter l'administrateur du site si vous avez des questions."
 
-#: lti_xblock.py:603
+#: lti_xblock.py:652
 msgid "Custom Parameters must be a list"
 msgstr "Les paramètres personnalisés doivent être une liste"
 
-#: lti_xblock.py:713
+#: lti_xblock.py:783 lti_xblock.py:1062
+msgid "Could not get user data for current request"
+msgstr ""
+
+#: lti_xblock.py:810
 msgid ""
 "Could not parse LTI passport: {lti_passport!r}. Should be \"id:key:secret\" "
 "string."
 msgstr "Impossible d'analyser le passeport LTI : {lti_passport!r}. Devrait être une chaîne \"id:key:secret\"."
 
-#: lti_xblock.py:729 lti_xblock.py:745
+#: lti_xblock.py:828 lti_xblock.py:842 lti_xblock.py:858
 msgid "Could not get user id for current request"
 msgstr "Impossible d'obtenir l'ID utilisateur pour la demande en cours"
 
-#: lti_xblock.py:850
+#: lti_xblock.py:994
 msgid ""
 "Could not parse custom parameter: {custom_parameter!r}. Should be \"x=y\" "
 "string."
 msgstr "Impossible d'analyser le paramètre personnalisé: {custom_parameter!r}. Doit être une chaîne \"x=y\"."
 
-#: lti_xblock.py:1310
+#: lti_xblock.py:1343
 msgid "[LTI]: Real user not found against anon_id: {}"
 msgstr "[LTI]: Utilisateur réel non trouvé pour anon_id: {}"
 
-#: models.py:72
+#: models.py:79
 msgid "Configuration Stored on XBlock fields"
 msgstr "Configuration stockée sur les champs du XBlock"
 
-#: models.py:73
+#: models.py:80
 msgid "Configuration Stored on this model"
 msgstr "Configuration stockée sur ce modèle"
 
-#: models.py:97
+#: models.py:81
+msgid "Configuration Stored on external service"
+msgstr ""
+
+#: models.py:113
 msgid "LTI configuration data."
 msgstr "Données de configuration LTI."
 
-#: models.py:104
+#: models.py:120
 msgid "The URL of the external tool that initiates the launch."
 msgstr "L'URL de l'outil externe qui initie le lancement."
 
-#: models.py:109
+#: models.py:125
 msgid "Client key provided by the LTI tool provider."
 msgstr "Clé client fournie par le fournisseur d'outils LTI."
 
-#: models.py:115
+#: models.py:131
 msgid "Client secret provided by the LTI tool provider."
 msgstr "Secret client fourni par le fournisseur d'outils LTI."
 
-#: models.py:121
+#: models.py:137
 msgid "Platform's generated Private key. Keep this value secret."
 msgstr "Clé privée générée par la plateforme. Gardez cette valeur secrète."
 
-#: models.py:127
+#: models.py:143
 msgid "Platform's generated Private key ID"
 msgstr "ID de clé privée généré par la plate-forme"
 
-#: models.py:132
+#: models.py:148
 msgid "Platform's generated JWK keyset."
 msgstr "Jeu de clés JWK généré par la plate-forme."
 
-#: models.py:138
+#: models.py:154
 msgid "Client ID used by LTI tool"
 msgstr "ID Client utilisé par l'outil LTI"
 
-#: models.py:148
+#: models.py:250
 msgid "LTI Configuration stores on XBlock needs a block location set."
 msgstr "Les configurations LTI sur stockées sur XBlock ont besoin d'un ensemble d'emplacement de bloc."
 
-#: models.py:155
+#: models.py:256
+msgid ""
+"LTI Configuration stored on the model for LTI 1.3 must have a value for one "
+"of lti_1p3_tool_public_key or lti_1p3_tool_keyset_url."
+msgstr ""
+
+#: models.py:263
+msgid ""
+"CONFIG_ON_XBLOCK and CONFIG_EXTERNAL are not supported for LTI 1.3 "
+"Proctoring Services."
+msgstr ""
+
+#: models.py:271
 msgid "Invalid LTI configuration."
 msgstr "Configuration LTI non valide."
 
-#: models.py:165
-msgid "Block location not set, it's not possible to retrieve the block."
-msgstr "Emplacement du bloc non défini, il n'est pas possible de récupérer le bloc."
-
-#: plugin/views.py:246
+#: plugin/views.py:453
 msgid "The selected content type is not supported by Open edX."
 msgstr "Le type de contenu sélectionné n'est pas pris en charge par Open edX."
 
-#: plugin/views.py:261
+#: plugin/views.py:468
 msgid "You don't have access to save LTI Content Items."
 msgstr "Vous n'avez pas accès pour enregistrer les éléments de contenu LTI."
 
-#: plugin/views.py:262
+#: plugin/views.py:469
 msgid ""
 "Please check that you have course staff permissions and double check this "
 "block's LTI settings."
 msgstr "Veuillez vérifier que vous disposez des autorisations du personnel de cours et revérifier les paramètres LTI de ce bloc."
 
 #: templates/html/lti-dl/dl_response_error.html:6
 msgid "LTI Deep Linking failed."
@@ -471,23 +533,14 @@
 msgid "The LTI Deep Linking content was successfully saved in the LMS."
 msgstr "Le contenu LTI Deep Linking a été enregistré avec succès dans le LMS."
 
 #: templates/html/lti-dl/dl_response_saved.html:13
 msgid "You can safely close this page now."
 msgstr "Vous pouvez maintenant fermer cette page en toute sécurité."
 
-#: templates/html/lti_1p3_launch_error.html:10
-msgid "There was an error while launching the LTI 1.3 tool."
-msgstr "Une erreur s'est produite lors du lancement de l'outil LTI 1.3."
-
-#: templates/html/lti_1p3_launch_error.html:13
-msgid ""
-"If you're seeing this on a live course, please contact the course staff."
-msgstr "Si vous voyez cela sur un cours actif veuillez contacter le personnel du cours."
-
 #: templates/html/lti_1p3_permission_error.html:10
 msgid "Unauthorized."
 msgstr "Non autorisé."
 
 #: templates/html/lti_1p3_permission_error.html:13
 msgid ""
 "Students don't have permissions to perform LTI Deep Linking configuration "
@@ -548,27 +601,46 @@
 msgid "Deep Linking Launch - Configure tool"
 msgstr "Lancement de Deep Linking - Configuration de l'outil"
 
 #: templates/html/lti_launch.html:27
 msgid "Press to Launch"
 msgstr ""
 
-#: static/js/xblock_lti_consumer.js:142
+#: templates/html/lti_launch_error.html:10
+msgid "There was an error while launching the LTI tool."
+msgstr ""
+
+#: templates/html/lti_launch_error.html:13
+#: templates/html/lti_proctoring_start_error.html:13
+msgid ""
+"If you're seeing this on a live course, please contact the course staff."
+msgstr "Si vous voyez cela sur un cours actif veuillez contacter le personnel du cours."
+
+#: templates/html/lti_proctoring_start_error.html:10
+msgid "There was an error while starting your LTI proctored assessment."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:126
+msgid "Cancel"
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:128
+msgid "OK"
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:157
 msgid ""
-"Click OK to have your username and e-mail address sent to a 3rd party application.\n"
-"\n"
-"Click Cancel to return to this page without sending your information."
-msgstr "Cliquez sur OK pour avoir votre nom d'utilisateur et votre adresse électronique transmis à une application tierce.\n\nCliquez sur Annuler pour retourner à la page précédente sans envoyer d'information."
-
-#: static/js/xblock_lti_consumer.js:144
-msgid ""
-"Click OK to have your username sent to a 3rd party application.\n"
-"\n"
-"Click Cancel to return to this page without sending your information."
-msgstr "Cliquez sur OK pour avoir votre nom d'utilisateur transmis à une application tierce.\n\nCliquez sur Annuler pour retourner à la page précédente sans envoyer d'information."
-
-#: static/js/xblock_lti_consumer.js:146
-msgid ""
-"Click OK to have your e-mail address sent to a 3rd party application.\n"
-"\n"
-"Click Cancel to return to this page without sending your information."
-msgstr "Cliquez sur OK pour avoir votre adresse mail transmise à une application tierce.\n\nCliquez sur Annuler pour retourner à la page précédente sans envoyer d'information."
+"Click OK to have your username and e-mail address sent to a 3rd party "
+"application."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:159
+msgid "Click OK to have your username sent to a 3rd party application."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:161
+msgid "Click OK to have your e-mail address sent to a 3rd party application."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:168
+msgid "Click Cancel to return to this page without sending your information."
+msgstr ""
```

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.0.2/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.2/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/translations/he/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.0.2/lti_consumer/translations/he/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/translations/he/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.2/lti_consumer/translations/he/LC_MESSAGES/text.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,458 +4,520 @@
 # 
 # Translators:
 # qualityalltext <quality@alltext.co.il>, 2016
 msgid ""
 msgstr ""
 "Project-Id-Version: XBlocks\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-02-01 17:24-0300\n"
+"POT-Creation-Date: 2023-04-11 15:09-0400\n"
 "PO-Revision-Date: 2016-06-08 14:38+0000\n"
 "Last-Translator: qualityalltext <quality@alltext.co.il>, 2016\n"
 "Language-Team: Hebrew (http://app.transifex.com/open-edx/xblocks/language/he/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: he\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n == 2 && n % 1 == 0) ? 1: (n % 10 == 0 && n % 1 == 0 && n > 10) ? 2 : 3;\n"
 
-#: lti_1p3/extensions/rest_framework/authentication.py:40
+#: lti_1p3/extensions/rest_framework/authentication.py:41
 msgid "Missing LTI 1.3 authentication token."
 msgstr ""
 
-#: lti_1p3/extensions/rest_framework/authentication.py:44
+#: lti_1p3/extensions/rest_framework/authentication.py:45
 msgid "Invalid token header. No credentials provided."
 msgstr ""
 
-#: lti_1p3/extensions/rest_framework/authentication.py:48
+#: lti_1p3/extensions/rest_framework/authentication.py:49
 msgid "Invalid token header. Token string should not contain spaces."
 msgstr ""
 
-#: lti_1p3/extensions/rest_framework/authentication.py:56
+#: lti_1p3/extensions/rest_framework/authentication.py:57
 msgid "LTI configuration not found."
 msgstr ""
 
-#: lti_1p3/extensions/rest_framework/authentication.py:65
+#: lti_1p3/extensions/rest_framework/authentication.py:66
 msgid "Invalid token signature."
 msgstr ""
 
-#: lti_xblock.py:127
+#: lti_xblock.py:126
 msgid "No valid user id found in endpoint URL"
 msgstr "לא נמצא מזהה משתמש תקף בכתובת ה-URL הסופית"
 
-#: lti_xblock.py:233
+#: lti_xblock.py:139
+msgid "Configuration on block"
+msgstr ""
+
+#: lti_xblock.py:143
+msgid "Database Configuration"
+msgstr ""
+
+#: lti_xblock.py:146
+msgid "Reusable Configuration"
+msgstr ""
+
+#: lti_xblock.py:253
 msgid "Display Name"
 msgstr "הצג שם"
 
-#: lti_xblock.py:235
+#: lti_xblock.py:255
 msgid ""
 "Enter the name that students see for this component. Analytics reports may "
 "also use the display name to identify this component."
 msgstr "יש להזין את שם המרכיב שרואים הלומדים. דוחות הניתוח יכולים להשתמש גם בשם התצוגה לזיהוי מרכיב זה."
 
-#: lti_xblock.py:239
+#: lti_xblock.py:259
 msgid "LTI Consumer"
 msgstr "צרכן LTI"
 
-#: lti_xblock.py:242
+#: lti_xblock.py:262
 msgid "LTI Application Information"
 msgstr "מידע אודות אפליקציית LTI"
 
-#: lti_xblock.py:244
+#: lti_xblock.py:264
 msgid ""
 "Enter a description of the third party application. If requesting username "
 "and/or email, use this text box to inform users why their username and/or "
 "email will be forwarded to a third party application."
 msgstr "יש להזין תיאור של יישום צד ג'. בבקשת שם משתמש ו/או כתובת דוא״ל, יש להשתמש בתיבת טקסט זו על מנת להודיע למשתמשים מדוע שם המשתמש ו/או כתובת הדוא״ ל שלהם תועבר ליישום של גורם צד ג'."
 
-#: lti_xblock.py:254
+#: lti_xblock.py:272
+msgid "Configuration Type"
+msgstr ""
+
+#: lti_xblock.py:277
+msgid ""
+"Select 'Configuration on block' to configure a new LTI Tool. If the support "
+"staff provided you with a pre-configured LTI reusable Tool ID, "
+"select'Reusable Configuration' and enter it in the text field below."
+msgstr ""
+
+#: lti_xblock.py:284
 msgid "LTI Version"
 msgstr ""
 
-#: lti_xblock.py:262
+#: lti_xblock.py:292
 msgid ""
 "Select the LTI version that your tool supports.<br />The XBlock LTI Consumer"
 " fully supports LTI 1.1.1, LTI 1.3 and LTI Advantage features."
 msgstr ""
 
-#: lti_xblock.py:268
+#: lti_xblock.py:299
+msgid "LTI Reusable Configuration ID"
+msgstr ""
+
+#: lti_xblock.py:301
+msgid ""
+"Enter the reusable LTI external configuration ID provided by the support "
+"staff."
+msgstr ""
+
+#: lti_xblock.py:306
 msgid "Tool Launch URL"
 msgstr ""
 
-#: lti_xblock.py:272
+#: lti_xblock.py:310
 msgid ""
 "Enter the LTI 1.3 Tool Launch URL. <br />This is the URL the LMS will use to"
 " launch the LTI Tool."
 msgstr ""
 
-#: lti_xblock.py:277
+#: lti_xblock.py:315
 msgid "Tool Initiate Login URL"
 msgstr ""
 
-#: lti_xblock.py:281
+#: lti_xblock.py:319
 msgid ""
 "Enter the LTI 1.3 Tool OIDC Authorization url (can also be called login or "
 "login initiation URL).<br />This is the URL the LMS will use to start a LTI "
 "authorization prior to doing the launch request."
 msgstr ""
 
-#: lti_xblock.py:288
+#: lti_xblock.py:325
+msgid "Registered Redirect URIs"
+msgstr ""
+
+#: lti_xblock.py:327
+msgid ""
+"Valid urls the Tool may request us to redirect the id token to. The redirect"
+" uris are often the same as the launch url/deep linking url so if this field"
+" is empty, it will use them as the default. If you need to use different "
+"redirect uri's, enter them here. If you use this field you must enter all "
+"valid redirect uri's the tool may request."
+msgstr ""
+
+#: lti_xblock.py:337
 msgid "Tool Public Key Mode"
 msgstr ""
 
-#: lti_xblock.py:296
+#: lti_xblock.py:345
 msgid "Select how the tool's public key information will be specified."
 msgstr ""
 
-#: lti_xblock.py:300
+#: lti_xblock.py:349
 msgid "Tool Keyset URL"
 msgstr ""
 
-#: lti_xblock.py:304
+#: lti_xblock.py:353
 msgid ""
 "Enter the LTI 1.3 Tool's JWK keysets URL.<br />This link should retrieve a "
 "JSON file containing public keys and signature algorithm information, so "
 "that the LMS can check if the messages and launch requests received have the"
 " signature from the tool.<br /><b>This is not required when doing LTI 1.3 "
 "Launches without LTI Advantage nor Basic Outcomes requests.</b>"
 msgstr ""
 
-#: lti_xblock.py:314
+#: lti_xblock.py:363
 msgid "Tool Public Key"
 msgstr ""
 
-#: lti_xblock.py:319
+#: lti_xblock.py:368
 msgid ""
 "Enter the LTI 1.3 Tool's public key.<br />This is a string that starts with "
 "'-----BEGIN PUBLIC KEY-----' and is required so that the LMS can check if "
 "the messages and launch requests received have the signature from the "
 "tool.<br /><b>This is not required when doing LTI 1.3 Launches without LTI "
 "Advantage nor Basic Outcomes requests.</b>"
 msgstr ""
 
-#: lti_xblock.py:329
+#: lti_xblock.py:378
 msgid "Enable LTI NRPS"
 msgstr ""
 
-#: lti_xblock.py:330
+#: lti_xblock.py:379
 msgid "Enable LTI Names and Role Provisioning Services."
 msgstr ""
 
-#: lti_xblock.py:337
+#: lti_xblock.py:386
 msgid "LTI 1.3 Block Client ID - DEPRECATED"
 msgstr ""
 
-#: lti_xblock.py:340
+#: lti_xblock.py:389
 msgid "DEPRECATED - This is now stored in the LtiConfiguration model."
 msgstr ""
 
-#: lti_xblock.py:343
+#: lti_xblock.py:392
 msgid "LTI 1.3 Block Key - DEPRECATED"
 msgstr ""
 
-#: lti_xblock.py:350
+#: lti_xblock.py:399
 msgid "Deep linking"
 msgstr ""
 
-#: lti_xblock.py:351
+#: lti_xblock.py:400
 msgid "Select True if you want to enable LTI Advantage Deep Linking."
 msgstr ""
 
-#: lti_xblock.py:356
+#: lti_xblock.py:405
 msgid "Deep Linking Launch URL"
 msgstr ""
 
-#: lti_xblock.py:360
+#: lti_xblock.py:409
 msgid ""
 "Enter the LTI Advantage Deep Linking Launch URL. If the tool does not "
 "specify one, use the same value as 'Tool Launch URL'."
 msgstr ""
 
-#: lti_xblock.py:365
+#: lti_xblock.py:414
 msgid "LTI Assignment and Grades Service"
 msgstr ""
 
-#: lti_xblock.py:367
+#: lti_xblock.py:416
 msgid "Disabled"
 msgstr ""
 
-#: lti_xblock.py:368
+#: lti_xblock.py:417
 msgid "Allow tools to submit grades only (declarative)"
 msgstr ""
 
-#: lti_xblock.py:369
+#: lti_xblock.py:418
 msgid "Allow tools to manage and submit grade (programmatic)"
 msgstr ""
 
-#: lti_xblock.py:374
+#: lti_xblock.py:423
 msgid ""
 "Enable the LTI-AGS service and select the functionality enabled for LTI "
 "tools. The 'declarative' mode (default) will provide a tool with a LineItem "
 "created from the XBlock settings, while the 'programmatic' one will allow "
 "tools to manage, create and link the grades."
 msgstr ""
 
-#: lti_xblock.py:382
+#: lti_xblock.py:431
 msgid "LTI ID"
 msgstr "מזהה LTI"
 
-#: lti_xblock.py:384
+#: lti_xblock.py:433
 #, python-brace-format
 msgid ""
 "Enter the LTI ID for the external LTI provider. This value must be the same "
 "LTI ID that you entered in the LTI Passports setting on the Advanced "
 "Settings page.<br />See the {docs_anchor_open}edX LTI "
 "documentation{anchor_close} for more details on this setting."
 msgstr "הזן את מזהה ה-LTI לספק ה-LTI החיצוני. ערך זה חייב להיות זהה למזהה LTI שהזנת בהגדרות LTI Passports הנמצא בעמוד ההגדרות המתקדמות.<br />לפרטים נוספים אודות הגדרה זו, ראה {docs_anchor_open}edX LTI תיעוד{anchor_close}."
 
-#: lti_xblock.py:396
+#: lti_xblock.py:445
 msgid "LTI URL"
 msgstr "כתובת ה-URL של LTI"
 
-#: lti_xblock.py:398
+#: lti_xblock.py:447
 #, python-brace-format
 msgid ""
 "Enter the URL of the external tool that this component launches. This "
 "setting is only used when Hide External Tool is set to False.<br />See the "
 "{docs_anchor_open}edX LTI documentation{anchor_close} for more details on "
 "this setting."
 msgstr "הזן את כתובת האתר של הכלי החיצוני שרכיב זה מפעיל. ניתן להשתמש בהגדרה זו אך ורק כאשר האפשרות 'הסתר כלי חיצוני' נמצאת במצב 'False'.<br />לפרטים נוספים אודות הגדרה זו, ראה {docs_anchor_open}edX LTI תיעוד{anchor_close}."
 
-#: lti_xblock.py:411
+#: lti_xblock.py:460
 msgid "Custom Parameters"
 msgstr "פרמטרים מותאמים אישית"
 
-#: lti_xblock.py:413
+#: lti_xblock.py:462
 #, python-brace-format
 msgid ""
 "Add the key/value pair for any custom parameters, such as the page your "
 "e-book should open to or the background color for this component. Ex. "
 "[\"page=1\", \"color=white\"]<br />See the {docs_anchor_open}edX LTI "
 "documentation{anchor_close} for more details on this setting."
 msgstr "הוסף את צמד מפתח/ערך לכל פרמטר בהתאמה אישית כמו הדף שבו הספר האלקטרוני צריך להיפתח או צבע הרקע של מרכיב זה. לדוגמה. [\"page=1\", \"color=white\"]<br />ראה את {docs_anchor_open}edX LTI תיעוד{anchor_close} לפרטים נוספים אודות הגדרה זו."
 
-#: lti_xblock.py:423
+#: lti_xblock.py:472
 msgid "LTI Launch Target"
 msgstr "יעד השקת LTI"
 
-#: lti_xblock.py:425
+#: lti_xblock.py:474
 msgid ""
 "Select Inline if you want the LTI content to open in an IFrame in the "
 "current page. Select Modal if you want the LTI content to open in a modal "
 "window in the current page. Select New Window if you want the LTI content to"
 " open in a new browser window. This setting is only used when Hide External "
 "Tool is set to False."
 msgstr "בחר את האפשרות Inline אם ברצונך שתוכן ה-LTI יפתח בעמוד הנוכחי ב- IFrame. בחר את האפשרות Modal אם ברצונך שתוכן ה-LTI יפתח בעמוד הנוכחי בחלון Modal. בחר את האפשרות New Window אם ברצונך שתוכן ה-LTI יפתח בחלון דפדפן חדש. ניתן להשתמש בהגדרה זו אך ורק כאשר האפשרות 'הסתר כלי חיצוני' נמצאת במצב 'לא נכון'."
 
-#: lti_xblock.py:439
+#: lti_xblock.py:488
 msgid "Button Text"
 msgstr "טקסט תחתי"
 
-#: lti_xblock.py:441
+#: lti_xblock.py:490
 msgid ""
 "Enter the text on the button used to launch the third party application. "
 "This setting is only used when Hide External Tool is set to False and LTI "
 "Launch Target is set to Modal or New Window."
 msgstr "הזן בתחתית את הטקסט המשמש להפעלת האפליקציה של צד שלישי. ניתן להשתמש בהגדרה זו אך ורק כאשר האפשרות 'הסתר כלי חיצוני' נמצאת במצב 'לא נכון' וכאשר LTI Launch Target מוגדר כ-Modal או חלון חדש."
 
-#: lti_xblock.py:449
+#: lti_xblock.py:498
 msgid "Inline Height"
 msgstr "גובה ה-inline"
 
-#: lti_xblock.py:451
+#: lti_xblock.py:500
 msgid ""
 "Enter the desired pixel height of the iframe which will contain the LTI "
 "tool. This setting is only used when Hide External Tool is set to False and "
 "LTI Launch Target is set to Inline."
 msgstr "הזן את גובה הפיקסלים המבוקש של ה-iframe שיכלול את כלי ה-LTI. ניתן להשתמש בהגדרה זו אך ורק כאשר האפשרות 'הסתר כלי חיצוני' נמצאת במצב 'לא נכון' וכאשר LTI Launch Target מוגדר כ-Inline."
 
-#: lti_xblock.py:459
+#: lti_xblock.py:508
 msgid "Modal Height"
 msgstr "גובה ה-Modal"
 
-#: lti_xblock.py:461
+#: lti_xblock.py:510
 msgid ""
 "Enter the desired viewport percentage height of the modal overlay which will"
 " contain the LTI tool. This setting is only used when Hide External Tool is "
 "set to False and LTI Launch Target is set to Modal."
 msgstr "הזן את אחוז גובה האשנב של כיסוי ה-modal שיכלול את כלי ה-LTI. ניתן להשתמש בהגדרה זו אך ורק כאשר האפשרות 'הסתר כלי חיצוני' נמצאת במצב 'לא נכון' וכאשר LTI Launch Target מוגדר כ-Modal."
 
-#: lti_xblock.py:469
+#: lti_xblock.py:518
 msgid "Modal Width"
 msgstr "רוחב ה-Modal"
 
-#: lti_xblock.py:471
+#: lti_xblock.py:520
 msgid ""
 "Enter the desired viewport percentage width of the modal overlay which will "
 "contain the LTI tool. This setting is only used when Hide External Tool is "
 "set to False and LTI Launch Target is set to Modal."
 msgstr "הזן את אחוז רוחב האשנב של כיסוי ה-modal שיכלול את כלי ה-LTI. ניתן להשתמש בהגדרה זו אך ורק כאשר האפשרות 'הסתר כלי חיצוני' נמצאת במצב 'לא נכון' וכאשר LTI Launch Target מוגדר כ-Modal."
 
-#: lti_xblock.py:479
+#: lti_xblock.py:528
 msgid "Scored"
 msgstr "קיבל ציון"
 
-#: lti_xblock.py:480
+#: lti_xblock.py:529
 msgid ""
 "Select True if this component will receive a numerical score from the "
 "external LTI system."
 msgstr "בחר באפשרות נכון אם מרכיב זה יקבל ציון מספרי ממערכת ה-LTI החיצונית."
 
-#: lti_xblock.py:487
+#: lti_xblock.py:536
 msgid ""
 "Enter the number of points possible for this component.  The default value "
 "is 1.0.  This setting is only used when Scored is set to True."
 msgstr "הזן את מספר הנקודות האפשריות למרכיב זה.  ברירת המחדל היא 1.0. ניתן להשתמש בהגדרה זו אך ורק כאשר 'קיבל ציון' מוגדר כ-נכון."
 
-#: lti_xblock.py:496
+#: lti_xblock.py:545
 msgid ""
 "The score kept in the xblock KVS -- duplicate of the published score in "
 "django DB"
 msgstr "הציון נשמר ב- xblock KVS – שכפול הציון המפורסם ב-django DB"
 
-#: lti_xblock.py:501
+#: lti_xblock.py:550
 msgid "Comment as returned from grader, LTI2.0 spec"
 msgstr "הערה חוזרת ממעניק הציון, LTI2.0 spec"
 
-#: lti_xblock.py:506
+#: lti_xblock.py:555
 msgid "Hide External Tool"
 msgstr "הסתר כלי חיצוני"
 
-#: lti_xblock.py:508
+#: lti_xblock.py:557
 msgid ""
 "Select True if you want to use this component as a placeholder for syncing "
 "with an external grading  system rather than launch an external tool.  This "
 "setting hides the Launch button and any IFrames for this component."
 msgstr "בחר באפשרות 'נכון' אם ברצונך להשתמש במרכיב זה כשומר מקום עבור סנכרון עם מערכת ציונים חיצונית במקום להפעיל כלי חיצוני.  הגדרה זו מסתירה את לחצן 'הפעל' וכל IFrames עבור מרכיב זה."
 
-#: lti_xblock.py:516
+#: lti_xblock.py:565
 msgid "Accept grades past deadline"
 msgstr "קבל ציונים לאחר המועד הסופי"
 
-#: lti_xblock.py:517
+#: lti_xblock.py:566
 msgid ""
 "Select True to allow third party systems to post grades past the deadline."
 msgstr "בחר באפשרות 'נכון' על מנת לאפשר למערכות צד שלישי לפרסם ציונים לאחר המועד הסופי."
 
-#: lti_xblock.py:525
+#: lti_xblock.py:574
 msgid "Request user's username"
 msgstr "בקש את שם המשתמש של המשתמש"
 
 #. Translators: This is used to request the user's username for a third party
 #. service.
-#: lti_xblock.py:527
+#: lti_xblock.py:576
 msgid "Select True to request the user's username."
 msgstr "בחר באפשרות 'נכון' על מנת לבקש את שם המשתמש של המשתמש."
 
-#: lti_xblock.py:532
+#: lti_xblock.py:581
 msgid "Request user's email"
 msgstr "בקש את כתובת הדוא״ל של המשתמש"
 
 #. Translators: This is used to request the user's email for a third party
 #. service.
-#: lti_xblock.py:534
+#: lti_xblock.py:583
 msgid "Select True to request the user's email address."
 msgstr "בחר באפשרות 'נכון' על מנת לבקש את כתובת דוא״ל המשתמש."
 
-#: lti_xblock.py:539
+#: lti_xblock.py:588
 msgid "Send extra parameters"
 msgstr ""
 
-#: lti_xblock.py:540
+#: lti_xblock.py:589
 msgid ""
 "Select True to send the extra parameters, which might contain Personally "
 "Identifiable Information. The processors are site-wide, please consult the "
 "site administrator if you have any questions."
 msgstr ""
 
-#: lti_xblock.py:603
+#: lti_xblock.py:652
 msgid "Custom Parameters must be a list"
 msgstr ""
 
-#: lti_xblock.py:713
+#: lti_xblock.py:783 lti_xblock.py:1062
+msgid "Could not get user data for current request"
+msgstr ""
+
+#: lti_xblock.py:810
 msgid ""
 "Could not parse LTI passport: {lti_passport!r}. Should be \"id:key:secret\" "
 "string."
 msgstr ""
 
-#: lti_xblock.py:729 lti_xblock.py:745
+#: lti_xblock.py:828 lti_xblock.py:842 lti_xblock.py:858
 msgid "Could not get user id for current request"
 msgstr "לא ניתן להשיג מזהה משתמש לבקשה הנוכחית"
 
-#: lti_xblock.py:850
+#: lti_xblock.py:994
 msgid ""
 "Could not parse custom parameter: {custom_parameter!r}. Should be \"x=y\" "
 "string."
 msgstr ""
 
-#: lti_xblock.py:1310
+#: lti_xblock.py:1343
 msgid "[LTI]: Real user not found against anon_id: {}"
 msgstr "[LTI]: לא נמצא משתמש אמיתי מול anon_id: {}"
 
-#: models.py:72
+#: models.py:79
 msgid "Configuration Stored on XBlock fields"
 msgstr ""
 
-#: models.py:73
+#: models.py:80
 msgid "Configuration Stored on this model"
 msgstr ""
 
-#: models.py:97
+#: models.py:81
+msgid "Configuration Stored on external service"
+msgstr ""
+
+#: models.py:113
 msgid "LTI configuration data."
 msgstr ""
 
-#: models.py:104
+#: models.py:120
 msgid "The URL of the external tool that initiates the launch."
 msgstr ""
 
-#: models.py:109
+#: models.py:125
 msgid "Client key provided by the LTI tool provider."
 msgstr ""
 
-#: models.py:115
+#: models.py:131
 msgid "Client secret provided by the LTI tool provider."
 msgstr ""
 
-#: models.py:121
+#: models.py:137
 msgid "Platform's generated Private key. Keep this value secret."
 msgstr ""
 
-#: models.py:127
+#: models.py:143
 msgid "Platform's generated Private key ID"
 msgstr ""
 
-#: models.py:132
+#: models.py:148
 msgid "Platform's generated JWK keyset."
 msgstr ""
 
-#: models.py:138
+#: models.py:154
 msgid "Client ID used by LTI tool"
 msgstr ""
 
-#: models.py:148
+#: models.py:250
 msgid "LTI Configuration stores on XBlock needs a block location set."
 msgstr ""
 
-#: models.py:155
-msgid "Invalid LTI configuration."
+#: models.py:256
+msgid ""
+"LTI Configuration stored on the model for LTI 1.3 must have a value for one "
+"of lti_1p3_tool_public_key or lti_1p3_tool_keyset_url."
+msgstr ""
+
+#: models.py:263
+msgid ""
+"CONFIG_ON_XBLOCK and CONFIG_EXTERNAL are not supported for LTI 1.3 "
+"Proctoring Services."
 msgstr ""
 
-#: models.py:165
-msgid "Block location not set, it's not possible to retrieve the block."
+#: models.py:271
+msgid "Invalid LTI configuration."
 msgstr ""
 
-#: plugin/views.py:246
+#: plugin/views.py:453
 msgid "The selected content type is not supported by Open edX."
 msgstr ""
 
-#: plugin/views.py:261
+#: plugin/views.py:468
 msgid "You don't have access to save LTI Content Items."
 msgstr ""
 
-#: plugin/views.py:262
+#: plugin/views.py:469
 msgid ""
 "Please check that you have course staff permissions and double check this "
 "block's LTI settings."
 msgstr ""
 
 #: templates/html/lti-dl/dl_response_error.html:6
 msgid "LTI Deep Linking failed."
@@ -469,23 +531,14 @@
 msgid "The LTI Deep Linking content was successfully saved in the LMS."
 msgstr ""
 
 #: templates/html/lti-dl/dl_response_saved.html:13
 msgid "You can safely close this page now."
 msgstr ""
 
-#: templates/html/lti_1p3_launch_error.html:10
-msgid "There was an error while launching the LTI 1.3 tool."
-msgstr ""
-
-#: templates/html/lti_1p3_launch_error.html:13
-msgid ""
-"If you're seeing this on a live course, please contact the course staff."
-msgstr ""
-
 #: templates/html/lti_1p3_permission_error.html:10
 msgid "Unauthorized."
 msgstr ""
 
 #: templates/html/lti_1p3_permission_error.html:13
 msgid ""
 "Students don't have permissions to perform LTI Deep Linking configuration "
@@ -546,27 +599,46 @@
 msgid "Deep Linking Launch - Configure tool"
 msgstr ""
 
 #: templates/html/lti_launch.html:27
 msgid "Press to Launch"
 msgstr ""
 
-#: static/js/xblock_lti_consumer.js:142
-msgid ""
-"Click OK to have your username and e-mail address sent to a 3rd party application.\n"
-"\n"
-"Click Cancel to return to this page without sending your information."
+#: templates/html/lti_launch_error.html:10
+msgid "There was an error while launching the LTI tool."
 msgstr ""
 
-#: static/js/xblock_lti_consumer.js:144
+#: templates/html/lti_launch_error.html:13
+#: templates/html/lti_proctoring_start_error.html:13
 msgid ""
-"Click OK to have your username sent to a 3rd party application.\n"
-"\n"
-"Click Cancel to return to this page without sending your information."
+"If you're seeing this on a live course, please contact the course staff."
+msgstr ""
+
+#: templates/html/lti_proctoring_start_error.html:10
+msgid "There was an error while starting your LTI proctored assessment."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:126
+msgid "Cancel"
 msgstr ""
 
-#: static/js/xblock_lti_consumer.js:146
+#: static/js/xblock_lti_consumer.js:128
+msgid "OK"
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:157
 msgid ""
-"Click OK to have your e-mail address sent to a 3rd party application.\n"
-"\n"
-"Click Cancel to return to this page without sending your information."
+"Click OK to have your username and e-mail address sent to a 3rd party "
+"application."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:159
+msgid "Click OK to have your username sent to a 3rd party application."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:161
+msgid "Click OK to have your e-mail address sent to a 3rd party application."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:168
+msgid "Click Cancel to return to this page without sending your information."
 msgstr ""
```

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/translations/hi/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.2/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po`

 * *Files 9% similar despite different names*

```diff
@@ -1,460 +1,523 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # 
 # Translators:
+# Iris Zeng <yz3535@nyu.edu>, 2016
 msgid ""
 msgstr ""
 "Project-Id-Version: XBlocks\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-02-01 17:24-0300\n"
+"POT-Creation-Date: 2023-04-11 15:09-0400\n"
 "PO-Revision-Date: 2016-06-08 14:38+0000\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: Hindi (http://app.transifex.com/open-edx/xblocks/language/hi/)\n"
+"Last-Translator: Iris Zeng <yz3535@nyu.edu>, 2016\n"
+"Language-Team: Chinese (China) (http://app.transifex.com/open-edx/xblocks/language/zh_CN/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: hi\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: zh_CN\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
-#: lti_1p3/extensions/rest_framework/authentication.py:40
+#: lti_1p3/extensions/rest_framework/authentication.py:41
 msgid "Missing LTI 1.3 authentication token."
 msgstr ""
 
-#: lti_1p3/extensions/rest_framework/authentication.py:44
+#: lti_1p3/extensions/rest_framework/authentication.py:45
 msgid "Invalid token header. No credentials provided."
 msgstr ""
 
-#: lti_1p3/extensions/rest_framework/authentication.py:48
+#: lti_1p3/extensions/rest_framework/authentication.py:49
 msgid "Invalid token header. Token string should not contain spaces."
 msgstr ""
 
-#: lti_1p3/extensions/rest_framework/authentication.py:56
+#: lti_1p3/extensions/rest_framework/authentication.py:57
 msgid "LTI configuration not found."
 msgstr ""
 
-#: lti_1p3/extensions/rest_framework/authentication.py:65
+#: lti_1p3/extensions/rest_framework/authentication.py:66
 msgid "Invalid token signature."
 msgstr ""
 
-#: lti_xblock.py:127
+#: lti_xblock.py:126
 msgid "No valid user id found in endpoint URL"
 msgstr ""
 
-#: lti_xblock.py:233
+#: lti_xblock.py:139
+msgid "Configuration on block"
+msgstr ""
+
+#: lti_xblock.py:143
+msgid "Database Configuration"
+msgstr ""
+
+#: lti_xblock.py:146
+msgid "Reusable Configuration"
+msgstr ""
+
+#: lti_xblock.py:253
 msgid "Display Name"
 msgstr ""
 
-#: lti_xblock.py:235
+#: lti_xblock.py:255
 msgid ""
 "Enter the name that students see for this component. Analytics reports may "
 "also use the display name to identify this component."
 msgstr ""
 
-#: lti_xblock.py:239
+#: lti_xblock.py:259
 msgid "LTI Consumer"
 msgstr ""
 
-#: lti_xblock.py:242
+#: lti_xblock.py:262
 msgid "LTI Application Information"
 msgstr ""
 
-#: lti_xblock.py:244
+#: lti_xblock.py:264
 msgid ""
 "Enter a description of the third party application. If requesting username "
 "and/or email, use this text box to inform users why their username and/or "
 "email will be forwarded to a third party application."
 msgstr ""
 
-#: lti_xblock.py:254
+#: lti_xblock.py:272
+msgid "Configuration Type"
+msgstr ""
+
+#: lti_xblock.py:277
+msgid ""
+"Select 'Configuration on block' to configure a new LTI Tool. If the support "
+"staff provided you with a pre-configured LTI reusable Tool ID, "
+"select'Reusable Configuration' and enter it in the text field below."
+msgstr ""
+
+#: lti_xblock.py:284
 msgid "LTI Version"
 msgstr ""
 
-#: lti_xblock.py:262
+#: lti_xblock.py:292
 msgid ""
 "Select the LTI version that your tool supports.<br />The XBlock LTI Consumer"
 " fully supports LTI 1.1.1, LTI 1.3 and LTI Advantage features."
 msgstr ""
 
-#: lti_xblock.py:268
+#: lti_xblock.py:299
+msgid "LTI Reusable Configuration ID"
+msgstr ""
+
+#: lti_xblock.py:301
+msgid ""
+"Enter the reusable LTI external configuration ID provided by the support "
+"staff."
+msgstr ""
+
+#: lti_xblock.py:306
 msgid "Tool Launch URL"
 msgstr ""
 
-#: lti_xblock.py:272
+#: lti_xblock.py:310
 msgid ""
 "Enter the LTI 1.3 Tool Launch URL. <br />This is the URL the LMS will use to"
 " launch the LTI Tool."
 msgstr ""
 
-#: lti_xblock.py:277
+#: lti_xblock.py:315
 msgid "Tool Initiate Login URL"
 msgstr ""
 
-#: lti_xblock.py:281
+#: lti_xblock.py:319
 msgid ""
 "Enter the LTI 1.3 Tool OIDC Authorization url (can also be called login or "
 "login initiation URL).<br />This is the URL the LMS will use to start a LTI "
 "authorization prior to doing the launch request."
 msgstr ""
 
-#: lti_xblock.py:288
+#: lti_xblock.py:325
+msgid "Registered Redirect URIs"
+msgstr ""
+
+#: lti_xblock.py:327
+msgid ""
+"Valid urls the Tool may request us to redirect the id token to. The redirect"
+" uris are often the same as the launch url/deep linking url so if this field"
+" is empty, it will use them as the default. If you need to use different "
+"redirect uri's, enter them here. If you use this field you must enter all "
+"valid redirect uri's the tool may request."
+msgstr ""
+
+#: lti_xblock.py:337
 msgid "Tool Public Key Mode"
 msgstr ""
 
-#: lti_xblock.py:296
+#: lti_xblock.py:345
 msgid "Select how the tool's public key information will be specified."
 msgstr ""
 
-#: lti_xblock.py:300
+#: lti_xblock.py:349
 msgid "Tool Keyset URL"
 msgstr ""
 
-#: lti_xblock.py:304
+#: lti_xblock.py:353
 msgid ""
 "Enter the LTI 1.3 Tool's JWK keysets URL.<br />This link should retrieve a "
 "JSON file containing public keys and signature algorithm information, so "
 "that the LMS can check if the messages and launch requests received have the"
 " signature from the tool.<br /><b>This is not required when doing LTI 1.3 "
 "Launches without LTI Advantage nor Basic Outcomes requests.</b>"
 msgstr ""
 
-#: lti_xblock.py:314
+#: lti_xblock.py:363
 msgid "Tool Public Key"
 msgstr ""
 
-#: lti_xblock.py:319
+#: lti_xblock.py:368
 msgid ""
 "Enter the LTI 1.3 Tool's public key.<br />This is a string that starts with "
 "'-----BEGIN PUBLIC KEY-----' and is required so that the LMS can check if "
 "the messages and launch requests received have the signature from the "
 "tool.<br /><b>This is not required when doing LTI 1.3 Launches without LTI "
 "Advantage nor Basic Outcomes requests.</b>"
 msgstr ""
 
-#: lti_xblock.py:329
+#: lti_xblock.py:378
 msgid "Enable LTI NRPS"
 msgstr ""
 
-#: lti_xblock.py:330
+#: lti_xblock.py:379
 msgid "Enable LTI Names and Role Provisioning Services."
 msgstr ""
 
-#: lti_xblock.py:337
+#: lti_xblock.py:386
 msgid "LTI 1.3 Block Client ID - DEPRECATED"
 msgstr ""
 
-#: lti_xblock.py:340
+#: lti_xblock.py:389
 msgid "DEPRECATED - This is now stored in the LtiConfiguration model."
 msgstr ""
 
-#: lti_xblock.py:343
+#: lti_xblock.py:392
 msgid "LTI 1.3 Block Key - DEPRECATED"
 msgstr ""
 
-#: lti_xblock.py:350
+#: lti_xblock.py:399
 msgid "Deep linking"
 msgstr ""
 
-#: lti_xblock.py:351
+#: lti_xblock.py:400
 msgid "Select True if you want to enable LTI Advantage Deep Linking."
 msgstr ""
 
-#: lti_xblock.py:356
+#: lti_xblock.py:405
 msgid "Deep Linking Launch URL"
 msgstr ""
 
-#: lti_xblock.py:360
+#: lti_xblock.py:409
 msgid ""
 "Enter the LTI Advantage Deep Linking Launch URL. If the tool does not "
 "specify one, use the same value as 'Tool Launch URL'."
 msgstr ""
 
-#: lti_xblock.py:365
+#: lti_xblock.py:414
 msgid "LTI Assignment and Grades Service"
 msgstr ""
 
-#: lti_xblock.py:367
+#: lti_xblock.py:416
 msgid "Disabled"
 msgstr ""
 
-#: lti_xblock.py:368
+#: lti_xblock.py:417
 msgid "Allow tools to submit grades only (declarative)"
 msgstr ""
 
-#: lti_xblock.py:369
+#: lti_xblock.py:418
 msgid "Allow tools to manage and submit grade (programmatic)"
 msgstr ""
 
-#: lti_xblock.py:374
+#: lti_xblock.py:423
 msgid ""
 "Enable the LTI-AGS service and select the functionality enabled for LTI "
 "tools. The 'declarative' mode (default) will provide a tool with a LineItem "
 "created from the XBlock settings, while the 'programmatic' one will allow "
 "tools to manage, create and link the grades."
 msgstr ""
 
-#: lti_xblock.py:382
+#: lti_xblock.py:431
 msgid "LTI ID"
 msgstr ""
 
-#: lti_xblock.py:384
+#: lti_xblock.py:433
 #, python-brace-format
 msgid ""
 "Enter the LTI ID for the external LTI provider. This value must be the same "
 "LTI ID that you entered in the LTI Passports setting on the Advanced "
 "Settings page.<br />See the {docs_anchor_open}edX LTI "
 "documentation{anchor_close} for more details on this setting."
 msgstr ""
 
-#: lti_xblock.py:396
+#: lti_xblock.py:445
 msgid "LTI URL"
 msgstr ""
 
-#: lti_xblock.py:398
+#: lti_xblock.py:447
 #, python-brace-format
 msgid ""
 "Enter the URL of the external tool that this component launches. This "
 "setting is only used when Hide External Tool is set to False.<br />See the "
 "{docs_anchor_open}edX LTI documentation{anchor_close} for more details on "
 "this setting."
 msgstr ""
 
-#: lti_xblock.py:411
+#: lti_xblock.py:460
 msgid "Custom Parameters"
 msgstr ""
 
-#: lti_xblock.py:413
+#: lti_xblock.py:462
 #, python-brace-format
 msgid ""
 "Add the key/value pair for any custom parameters, such as the page your "
 "e-book should open to or the background color for this component. Ex. "
 "[\"page=1\", \"color=white\"]<br />See the {docs_anchor_open}edX LTI "
 "documentation{anchor_close} for more details on this setting."
 msgstr ""
 
-#: lti_xblock.py:423
+#: lti_xblock.py:472
 msgid "LTI Launch Target"
 msgstr ""
 
-#: lti_xblock.py:425
+#: lti_xblock.py:474
 msgid ""
 "Select Inline if you want the LTI content to open in an IFrame in the "
 "current page. Select Modal if you want the LTI content to open in a modal "
 "window in the current page. Select New Window if you want the LTI content to"
 " open in a new browser window. This setting is only used when Hide External "
 "Tool is set to False."
 msgstr ""
 
-#: lti_xblock.py:439
+#: lti_xblock.py:488
 msgid "Button Text"
 msgstr ""
 
-#: lti_xblock.py:441
+#: lti_xblock.py:490
 msgid ""
 "Enter the text on the button used to launch the third party application. "
 "This setting is only used when Hide External Tool is set to False and LTI "
 "Launch Target is set to Modal or New Window."
 msgstr ""
 
-#: lti_xblock.py:449
+#: lti_xblock.py:498
 msgid "Inline Height"
 msgstr ""
 
-#: lti_xblock.py:451
+#: lti_xblock.py:500
 msgid ""
 "Enter the desired pixel height of the iframe which will contain the LTI "
 "tool. This setting is only used when Hide External Tool is set to False and "
 "LTI Launch Target is set to Inline."
 msgstr ""
 
-#: lti_xblock.py:459
+#: lti_xblock.py:508
 msgid "Modal Height"
 msgstr ""
 
-#: lti_xblock.py:461
+#: lti_xblock.py:510
 msgid ""
 "Enter the desired viewport percentage height of the modal overlay which will"
 " contain the LTI tool. This setting is only used when Hide External Tool is "
 "set to False and LTI Launch Target is set to Modal."
 msgstr ""
 
-#: lti_xblock.py:469
+#: lti_xblock.py:518
 msgid "Modal Width"
 msgstr ""
 
-#: lti_xblock.py:471
+#: lti_xblock.py:520
 msgid ""
 "Enter the desired viewport percentage width of the modal overlay which will "
 "contain the LTI tool. This setting is only used when Hide External Tool is "
 "set to False and LTI Launch Target is set to Modal."
 msgstr ""
 
-#: lti_xblock.py:479
+#: lti_xblock.py:528
 msgid "Scored"
 msgstr ""
 
-#: lti_xblock.py:480
+#: lti_xblock.py:529
 msgid ""
 "Select True if this component will receive a numerical score from the "
 "external LTI system."
 msgstr ""
 
-#: lti_xblock.py:487
+#: lti_xblock.py:536
 msgid ""
 "Enter the number of points possible for this component.  The default value "
 "is 1.0.  This setting is only used when Scored is set to True."
 msgstr ""
 
-#: lti_xblock.py:496
+#: lti_xblock.py:545
 msgid ""
 "The score kept in the xblock KVS -- duplicate of the published score in "
 "django DB"
 msgstr ""
 
-#: lti_xblock.py:501
+#: lti_xblock.py:550
 msgid "Comment as returned from grader, LTI2.0 spec"
 msgstr ""
 
-#: lti_xblock.py:506
+#: lti_xblock.py:555
 msgid "Hide External Tool"
 msgstr ""
 
-#: lti_xblock.py:508
+#: lti_xblock.py:557
 msgid ""
 "Select True if you want to use this component as a placeholder for syncing "
 "with an external grading  system rather than launch an external tool.  This "
 "setting hides the Launch button and any IFrames for this component."
 msgstr ""
 
-#: lti_xblock.py:516
+#: lti_xblock.py:565
 msgid "Accept grades past deadline"
 msgstr ""
 
-#: lti_xblock.py:517
+#: lti_xblock.py:566
 msgid ""
 "Select True to allow third party systems to post grades past the deadline."
 msgstr ""
 
-#: lti_xblock.py:525
+#: lti_xblock.py:574
 msgid "Request user's username"
 msgstr ""
 
 #. Translators: This is used to request the user's username for a third party
 #. service.
-#: lti_xblock.py:527
+#: lti_xblock.py:576
 msgid "Select True to request the user's username."
 msgstr ""
 
-#: lti_xblock.py:532
+#: lti_xblock.py:581
 msgid "Request user's email"
 msgstr ""
 
 #. Translators: This is used to request the user's email for a third party
 #. service.
-#: lti_xblock.py:534
+#: lti_xblock.py:583
 msgid "Select True to request the user's email address."
 msgstr ""
 
-#: lti_xblock.py:539
+#: lti_xblock.py:588
 msgid "Send extra parameters"
 msgstr ""
 
-#: lti_xblock.py:540
+#: lti_xblock.py:589
 msgid ""
 "Select True to send the extra parameters, which might contain Personally "
 "Identifiable Information. The processors are site-wide, please consult the "
 "site administrator if you have any questions."
 msgstr ""
 
-#: lti_xblock.py:603
+#: lti_xblock.py:652
 msgid "Custom Parameters must be a list"
 msgstr ""
 
-#: lti_xblock.py:713
+#: lti_xblock.py:783 lti_xblock.py:1062
+msgid "Could not get user data for current request"
+msgstr ""
+
+#: lti_xblock.py:810
 msgid ""
 "Could not parse LTI passport: {lti_passport!r}. Should be \"id:key:secret\" "
 "string."
 msgstr ""
 
-#: lti_xblock.py:729 lti_xblock.py:745
+#: lti_xblock.py:828 lti_xblock.py:842 lti_xblock.py:858
 msgid "Could not get user id for current request"
 msgstr ""
 
-#: lti_xblock.py:850
+#: lti_xblock.py:994
 msgid ""
 "Could not parse custom parameter: {custom_parameter!r}. Should be \"x=y\" "
 "string."
 msgstr ""
 
-#: lti_xblock.py:1310
+#: lti_xblock.py:1343
 msgid "[LTI]: Real user not found against anon_id: {}"
 msgstr ""
 
-#: models.py:72
+#: models.py:79
 msgid "Configuration Stored on XBlock fields"
 msgstr ""
 
-#: models.py:73
+#: models.py:80
 msgid "Configuration Stored on this model"
 msgstr ""
 
-#: models.py:97
+#: models.py:81
+msgid "Configuration Stored on external service"
+msgstr ""
+
+#: models.py:113
 msgid "LTI configuration data."
 msgstr ""
 
-#: models.py:104
+#: models.py:120
 msgid "The URL of the external tool that initiates the launch."
 msgstr ""
 
-#: models.py:109
+#: models.py:125
 msgid "Client key provided by the LTI tool provider."
 msgstr ""
 
-#: models.py:115
+#: models.py:131
 msgid "Client secret provided by the LTI tool provider."
 msgstr ""
 
-#: models.py:121
+#: models.py:137
 msgid "Platform's generated Private key. Keep this value secret."
 msgstr ""
 
-#: models.py:127
+#: models.py:143
 msgid "Platform's generated Private key ID"
 msgstr ""
 
-#: models.py:132
+#: models.py:148
 msgid "Platform's generated JWK keyset."
 msgstr ""
 
-#: models.py:138
+#: models.py:154
 msgid "Client ID used by LTI tool"
 msgstr ""
 
-#: models.py:148
+#: models.py:250
 msgid "LTI Configuration stores on XBlock needs a block location set."
 msgstr ""
 
-#: models.py:155
-msgid "Invalid LTI configuration."
+#: models.py:256
+msgid ""
+"LTI Configuration stored on the model for LTI 1.3 must have a value for one "
+"of lti_1p3_tool_public_key or lti_1p3_tool_keyset_url."
+msgstr ""
+
+#: models.py:263
+msgid ""
+"CONFIG_ON_XBLOCK and CONFIG_EXTERNAL are not supported for LTI 1.3 "
+"Proctoring Services."
 msgstr ""
 
-#: models.py:165
-msgid "Block location not set, it's not possible to retrieve the block."
+#: models.py:271
+msgid "Invalid LTI configuration."
 msgstr ""
 
-#: plugin/views.py:246
+#: plugin/views.py:453
 msgid "The selected content type is not supported by Open edX."
 msgstr ""
 
-#: plugin/views.py:261
+#: plugin/views.py:468
 msgid "You don't have access to save LTI Content Items."
 msgstr ""
 
-#: plugin/views.py:262
+#: plugin/views.py:469
 msgid ""
 "Please check that you have course staff permissions and double check this "
 "block's LTI settings."
 msgstr ""
 
 #: templates/html/lti-dl/dl_response_error.html:6
 msgid "LTI Deep Linking failed."
@@ -468,23 +531,14 @@
 msgid "The LTI Deep Linking content was successfully saved in the LMS."
 msgstr ""
 
 #: templates/html/lti-dl/dl_response_saved.html:13
 msgid "You can safely close this page now."
 msgstr ""
 
-#: templates/html/lti_1p3_launch_error.html:10
-msgid "There was an error while launching the LTI 1.3 tool."
-msgstr ""
-
-#: templates/html/lti_1p3_launch_error.html:13
-msgid ""
-"If you're seeing this on a live course, please contact the course staff."
-msgstr ""
-
 #: templates/html/lti_1p3_permission_error.html:10
 msgid "Unauthorized."
 msgstr ""
 
 #: templates/html/lti_1p3_permission_error.html:13
 msgid ""
 "Students don't have permissions to perform LTI Deep Linking configuration "
@@ -545,27 +599,46 @@
 msgid "Deep Linking Launch - Configure tool"
 msgstr ""
 
 #: templates/html/lti_launch.html:27
 msgid "Press to Launch"
 msgstr ""
 
-#: static/js/xblock_lti_consumer.js:142
-msgid ""
-"Click OK to have your username and e-mail address sent to a 3rd party application.\n"
-"\n"
-"Click Cancel to return to this page without sending your information."
+#: templates/html/lti_launch_error.html:10
+msgid "There was an error while launching the LTI tool."
 msgstr ""
 
-#: static/js/xblock_lti_consumer.js:144
+#: templates/html/lti_launch_error.html:13
+#: templates/html/lti_proctoring_start_error.html:13
 msgid ""
-"Click OK to have your username sent to a 3rd party application.\n"
-"\n"
-"Click Cancel to return to this page without sending your information."
+"If you're seeing this on a live course, please contact the course staff."
+msgstr ""
+
+#: templates/html/lti_proctoring_start_error.html:10
+msgid "There was an error while starting your LTI proctored assessment."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:126
+msgid "Cancel"
 msgstr ""
 
-#: static/js/xblock_lti_consumer.js:146
+#: static/js/xblock_lti_consumer.js:128
+msgid "OK"
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:157
 msgid ""
-"Click OK to have your e-mail address sent to a 3rd party application.\n"
-"\n"
-"Click Cancel to return to this page without sending your information."
+"Click OK to have your username and e-mail address sent to a 3rd party "
+"application."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:159
+msgid "Click OK to have your username sent to a 3rd party application."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:161
+msgid "Click OK to have your e-mail address sent to a 3rd party application."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:168
+msgid "Click Cancel to return to this page without sending your information."
 msgstr ""
```

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.0.2/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.2/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.2/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po`

 * *Files 9% similar despite different names*

```diff
@@ -4,458 +4,520 @@
 # 
 # Translators:
 # Wonjae Choi <juniorleo651@gmail.com>, 2021
 msgid ""
 msgstr ""
 "Project-Id-Version: XBlocks\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-02-01 17:24-0300\n"
+"POT-Creation-Date: 2023-04-11 15:09-0400\n"
 "PO-Revision-Date: 2016-06-08 14:38+0000\n"
 "Last-Translator: Wonjae Choi <juniorleo651@gmail.com>, 2021\n"
 "Language-Team: Korean (Korea) (http://app.transifex.com/open-edx/xblocks/language/ko_KR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ko_KR\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
-#: lti_1p3/extensions/rest_framework/authentication.py:40
+#: lti_1p3/extensions/rest_framework/authentication.py:41
 msgid "Missing LTI 1.3 authentication token."
 msgstr ""
 
-#: lti_1p3/extensions/rest_framework/authentication.py:44
+#: lti_1p3/extensions/rest_framework/authentication.py:45
 msgid "Invalid token header. No credentials provided."
 msgstr ""
 
-#: lti_1p3/extensions/rest_framework/authentication.py:48
+#: lti_1p3/extensions/rest_framework/authentication.py:49
 msgid "Invalid token header. Token string should not contain spaces."
 msgstr ""
 
-#: lti_1p3/extensions/rest_framework/authentication.py:56
+#: lti_1p3/extensions/rest_framework/authentication.py:57
 msgid "LTI configuration not found."
 msgstr ""
 
-#: lti_1p3/extensions/rest_framework/authentication.py:65
+#: lti_1p3/extensions/rest_framework/authentication.py:66
 msgid "Invalid token signature."
 msgstr ""
 
-#: lti_xblock.py:127
+#: lti_xblock.py:126
 msgid "No valid user id found in endpoint URL"
 msgstr ""
 
-#: lti_xblock.py:233
+#: lti_xblock.py:139
+msgid "Configuration on block"
+msgstr ""
+
+#: lti_xblock.py:143
+msgid "Database Configuration"
+msgstr ""
+
+#: lti_xblock.py:146
+msgid "Reusable Configuration"
+msgstr ""
+
+#: lti_xblock.py:253
 msgid "Display Name"
 msgstr ""
 
-#: lti_xblock.py:235
+#: lti_xblock.py:255
 msgid ""
 "Enter the name that students see for this component. Analytics reports may "
 "also use the display name to identify this component."
 msgstr ""
 
-#: lti_xblock.py:239
+#: lti_xblock.py:259
 msgid "LTI Consumer"
 msgstr ""
 
-#: lti_xblock.py:242
+#: lti_xblock.py:262
 msgid "LTI Application Information"
 msgstr ""
 
-#: lti_xblock.py:244
+#: lti_xblock.py:264
 msgid ""
 "Enter a description of the third party application. If requesting username "
 "and/or email, use this text box to inform users why their username and/or "
 "email will be forwarded to a third party application."
 msgstr ""
 
-#: lti_xblock.py:254
+#: lti_xblock.py:272
+msgid "Configuration Type"
+msgstr ""
+
+#: lti_xblock.py:277
+msgid ""
+"Select 'Configuration on block' to configure a new LTI Tool. If the support "
+"staff provided you with a pre-configured LTI reusable Tool ID, "
+"select'Reusable Configuration' and enter it in the text field below."
+msgstr ""
+
+#: lti_xblock.py:284
 msgid "LTI Version"
 msgstr ""
 
-#: lti_xblock.py:262
+#: lti_xblock.py:292
 msgid ""
 "Select the LTI version that your tool supports.<br />The XBlock LTI Consumer"
 " fully supports LTI 1.1.1, LTI 1.3 and LTI Advantage features."
 msgstr ""
 
-#: lti_xblock.py:268
+#: lti_xblock.py:299
+msgid "LTI Reusable Configuration ID"
+msgstr ""
+
+#: lti_xblock.py:301
+msgid ""
+"Enter the reusable LTI external configuration ID provided by the support "
+"staff."
+msgstr ""
+
+#: lti_xblock.py:306
 msgid "Tool Launch URL"
 msgstr ""
 
-#: lti_xblock.py:272
+#: lti_xblock.py:310
 msgid ""
 "Enter the LTI 1.3 Tool Launch URL. <br />This is the URL the LMS will use to"
 " launch the LTI Tool."
 msgstr ""
 
-#: lti_xblock.py:277
+#: lti_xblock.py:315
 msgid "Tool Initiate Login URL"
 msgstr ""
 
-#: lti_xblock.py:281
+#: lti_xblock.py:319
 msgid ""
 "Enter the LTI 1.3 Tool OIDC Authorization url (can also be called login or "
 "login initiation URL).<br />This is the URL the LMS will use to start a LTI "
 "authorization prior to doing the launch request."
 msgstr ""
 
-#: lti_xblock.py:288
+#: lti_xblock.py:325
+msgid "Registered Redirect URIs"
+msgstr ""
+
+#: lti_xblock.py:327
+msgid ""
+"Valid urls the Tool may request us to redirect the id token to. The redirect"
+" uris are often the same as the launch url/deep linking url so if this field"
+" is empty, it will use them as the default. If you need to use different "
+"redirect uri's, enter them here. If you use this field you must enter all "
+"valid redirect uri's the tool may request."
+msgstr ""
+
+#: lti_xblock.py:337
 msgid "Tool Public Key Mode"
 msgstr ""
 
-#: lti_xblock.py:296
+#: lti_xblock.py:345
 msgid "Select how the tool's public key information will be specified."
 msgstr ""
 
-#: lti_xblock.py:300
+#: lti_xblock.py:349
 msgid "Tool Keyset URL"
 msgstr ""
 
-#: lti_xblock.py:304
+#: lti_xblock.py:353
 msgid ""
 "Enter the LTI 1.3 Tool's JWK keysets URL.<br />This link should retrieve a "
 "JSON file containing public keys and signature algorithm information, so "
 "that the LMS can check if the messages and launch requests received have the"
 " signature from the tool.<br /><b>This is not required when doing LTI 1.3 "
 "Launches without LTI Advantage nor Basic Outcomes requests.</b>"
 msgstr ""
 
-#: lti_xblock.py:314
+#: lti_xblock.py:363
 msgid "Tool Public Key"
 msgstr ""
 
-#: lti_xblock.py:319
+#: lti_xblock.py:368
 msgid ""
 "Enter the LTI 1.3 Tool's public key.<br />This is a string that starts with "
 "'-----BEGIN PUBLIC KEY-----' and is required so that the LMS can check if "
 "the messages and launch requests received have the signature from the "
 "tool.<br /><b>This is not required when doing LTI 1.3 Launches without LTI "
 "Advantage nor Basic Outcomes requests.</b>"
 msgstr ""
 
-#: lti_xblock.py:329
+#: lti_xblock.py:378
 msgid "Enable LTI NRPS"
 msgstr ""
 
-#: lti_xblock.py:330
+#: lti_xblock.py:379
 msgid "Enable LTI Names and Role Provisioning Services."
 msgstr ""
 
-#: lti_xblock.py:337
+#: lti_xblock.py:386
 msgid "LTI 1.3 Block Client ID - DEPRECATED"
 msgstr ""
 
-#: lti_xblock.py:340
+#: lti_xblock.py:389
 msgid "DEPRECATED - This is now stored in the LtiConfiguration model."
 msgstr ""
 
-#: lti_xblock.py:343
+#: lti_xblock.py:392
 msgid "LTI 1.3 Block Key - DEPRECATED"
 msgstr ""
 
-#: lti_xblock.py:350
+#: lti_xblock.py:399
 msgid "Deep linking"
 msgstr ""
 
-#: lti_xblock.py:351
+#: lti_xblock.py:400
 msgid "Select True if you want to enable LTI Advantage Deep Linking."
 msgstr ""
 
-#: lti_xblock.py:356
+#: lti_xblock.py:405
 msgid "Deep Linking Launch URL"
 msgstr ""
 
-#: lti_xblock.py:360
+#: lti_xblock.py:409
 msgid ""
 "Enter the LTI Advantage Deep Linking Launch URL. If the tool does not "
 "specify one, use the same value as 'Tool Launch URL'."
 msgstr ""
 
-#: lti_xblock.py:365
+#: lti_xblock.py:414
 msgid "LTI Assignment and Grades Service"
 msgstr ""
 
-#: lti_xblock.py:367
+#: lti_xblock.py:416
 msgid "Disabled"
 msgstr ""
 
-#: lti_xblock.py:368
+#: lti_xblock.py:417
 msgid "Allow tools to submit grades only (declarative)"
 msgstr ""
 
-#: lti_xblock.py:369
+#: lti_xblock.py:418
 msgid "Allow tools to manage and submit grade (programmatic)"
 msgstr ""
 
-#: lti_xblock.py:374
+#: lti_xblock.py:423
 msgid ""
 "Enable the LTI-AGS service and select the functionality enabled for LTI "
 "tools. The 'declarative' mode (default) will provide a tool with a LineItem "
 "created from the XBlock settings, while the 'programmatic' one will allow "
 "tools to manage, create and link the grades."
 msgstr ""
 
-#: lti_xblock.py:382
+#: lti_xblock.py:431
 msgid "LTI ID"
 msgstr ""
 
-#: lti_xblock.py:384
+#: lti_xblock.py:433
 #, python-brace-format
 msgid ""
 "Enter the LTI ID for the external LTI provider. This value must be the same "
 "LTI ID that you entered in the LTI Passports setting on the Advanced "
 "Settings page.<br />See the {docs_anchor_open}edX LTI "
 "documentation{anchor_close} for more details on this setting."
 msgstr ""
 
-#: lti_xblock.py:396
+#: lti_xblock.py:445
 msgid "LTI URL"
 msgstr ""
 
-#: lti_xblock.py:398
+#: lti_xblock.py:447
 #, python-brace-format
 msgid ""
 "Enter the URL of the external tool that this component launches. This "
 "setting is only used when Hide External Tool is set to False.<br />See the "
 "{docs_anchor_open}edX LTI documentation{anchor_close} for more details on "
 "this setting."
 msgstr ""
 
-#: lti_xblock.py:411
+#: lti_xblock.py:460
 msgid "Custom Parameters"
 msgstr ""
 
-#: lti_xblock.py:413
+#: lti_xblock.py:462
 #, python-brace-format
 msgid ""
 "Add the key/value pair for any custom parameters, such as the page your "
 "e-book should open to or the background color for this component. Ex. "
 "[\"page=1\", \"color=white\"]<br />See the {docs_anchor_open}edX LTI "
 "documentation{anchor_close} for more details on this setting."
 msgstr ""
 
-#: lti_xblock.py:423
+#: lti_xblock.py:472
 msgid "LTI Launch Target"
 msgstr ""
 
-#: lti_xblock.py:425
+#: lti_xblock.py:474
 msgid ""
 "Select Inline if you want the LTI content to open in an IFrame in the "
 "current page. Select Modal if you want the LTI content to open in a modal "
 "window in the current page. Select New Window if you want the LTI content to"
 " open in a new browser window. This setting is only used when Hide External "
 "Tool is set to False."
 msgstr ""
 
-#: lti_xblock.py:439
+#: lti_xblock.py:488
 msgid "Button Text"
 msgstr ""
 
-#: lti_xblock.py:441
+#: lti_xblock.py:490
 msgid ""
 "Enter the text on the button used to launch the third party application. "
 "This setting is only used when Hide External Tool is set to False and LTI "
 "Launch Target is set to Modal or New Window."
 msgstr ""
 
-#: lti_xblock.py:449
+#: lti_xblock.py:498
 msgid "Inline Height"
 msgstr ""
 
-#: lti_xblock.py:451
+#: lti_xblock.py:500
 msgid ""
 "Enter the desired pixel height of the iframe which will contain the LTI "
 "tool. This setting is only used when Hide External Tool is set to False and "
 "LTI Launch Target is set to Inline."
 msgstr ""
 
-#: lti_xblock.py:459
+#: lti_xblock.py:508
 msgid "Modal Height"
 msgstr ""
 
-#: lti_xblock.py:461
+#: lti_xblock.py:510
 msgid ""
 "Enter the desired viewport percentage height of the modal overlay which will"
 " contain the LTI tool. This setting is only used when Hide External Tool is "
 "set to False and LTI Launch Target is set to Modal."
 msgstr ""
 
-#: lti_xblock.py:469
+#: lti_xblock.py:518
 msgid "Modal Width"
 msgstr ""
 
-#: lti_xblock.py:471
+#: lti_xblock.py:520
 msgid ""
 "Enter the desired viewport percentage width of the modal overlay which will "
 "contain the LTI tool. This setting is only used when Hide External Tool is "
 "set to False and LTI Launch Target is set to Modal."
 msgstr ""
 
-#: lti_xblock.py:479
+#: lti_xblock.py:528
 msgid "Scored"
 msgstr ""
 
-#: lti_xblock.py:480
+#: lti_xblock.py:529
 msgid ""
 "Select True if this component will receive a numerical score from the "
 "external LTI system."
 msgstr ""
 
-#: lti_xblock.py:487
+#: lti_xblock.py:536
 msgid ""
 "Enter the number of points possible for this component.  The default value "
 "is 1.0.  This setting is only used when Scored is set to True."
 msgstr ""
 
-#: lti_xblock.py:496
+#: lti_xblock.py:545
 msgid ""
 "The score kept in the xblock KVS -- duplicate of the published score in "
 "django DB"
 msgstr ""
 
-#: lti_xblock.py:501
+#: lti_xblock.py:550
 msgid "Comment as returned from grader, LTI2.0 spec"
 msgstr ""
 
-#: lti_xblock.py:506
+#: lti_xblock.py:555
 msgid "Hide External Tool"
 msgstr ""
 
-#: lti_xblock.py:508
+#: lti_xblock.py:557
 msgid ""
 "Select True if you want to use this component as a placeholder for syncing "
 "with an external grading  system rather than launch an external tool.  This "
 "setting hides the Launch button and any IFrames for this component."
 msgstr ""
 
-#: lti_xblock.py:516
+#: lti_xblock.py:565
 msgid "Accept grades past deadline"
 msgstr ""
 
-#: lti_xblock.py:517
+#: lti_xblock.py:566
 msgid ""
 "Select True to allow third party systems to post grades past the deadline."
 msgstr ""
 
-#: lti_xblock.py:525
+#: lti_xblock.py:574
 msgid "Request user's username"
 msgstr ""
 
 #. Translators: This is used to request the user's username for a third party
 #. service.
-#: lti_xblock.py:527
+#: lti_xblock.py:576
 msgid "Select True to request the user's username."
 msgstr ""
 
-#: lti_xblock.py:532
+#: lti_xblock.py:581
 msgid "Request user's email"
 msgstr ""
 
 #. Translators: This is used to request the user's email for a third party
 #. service.
-#: lti_xblock.py:534
+#: lti_xblock.py:583
 msgid "Select True to request the user's email address."
 msgstr ""
 
-#: lti_xblock.py:539
+#: lti_xblock.py:588
 msgid "Send extra parameters"
 msgstr ""
 
-#: lti_xblock.py:540
+#: lti_xblock.py:589
 msgid ""
 "Select True to send the extra parameters, which might contain Personally "
 "Identifiable Information. The processors are site-wide, please consult the "
 "site administrator if you have any questions."
 msgstr ""
 
-#: lti_xblock.py:603
+#: lti_xblock.py:652
 msgid "Custom Parameters must be a list"
 msgstr ""
 
-#: lti_xblock.py:713
+#: lti_xblock.py:783 lti_xblock.py:1062
+msgid "Could not get user data for current request"
+msgstr ""
+
+#: lti_xblock.py:810
 msgid ""
 "Could not parse LTI passport: {lti_passport!r}. Should be \"id:key:secret\" "
 "string."
 msgstr ""
 
-#: lti_xblock.py:729 lti_xblock.py:745
+#: lti_xblock.py:828 lti_xblock.py:842 lti_xblock.py:858
 msgid "Could not get user id for current request"
 msgstr ""
 
-#: lti_xblock.py:850
+#: lti_xblock.py:994
 msgid ""
 "Could not parse custom parameter: {custom_parameter!r}. Should be \"x=y\" "
 "string."
 msgstr ""
 
-#: lti_xblock.py:1310
+#: lti_xblock.py:1343
 msgid "[LTI]: Real user not found against anon_id: {}"
 msgstr ""
 
-#: models.py:72
+#: models.py:79
 msgid "Configuration Stored on XBlock fields"
 msgstr ""
 
-#: models.py:73
+#: models.py:80
 msgid "Configuration Stored on this model"
 msgstr ""
 
-#: models.py:97
+#: models.py:81
+msgid "Configuration Stored on external service"
+msgstr ""
+
+#: models.py:113
 msgid "LTI configuration data."
 msgstr ""
 
-#: models.py:104
+#: models.py:120
 msgid "The URL of the external tool that initiates the launch."
 msgstr ""
 
-#: models.py:109
+#: models.py:125
 msgid "Client key provided by the LTI tool provider."
 msgstr ""
 
-#: models.py:115
+#: models.py:131
 msgid "Client secret provided by the LTI tool provider."
 msgstr ""
 
-#: models.py:121
+#: models.py:137
 msgid "Platform's generated Private key. Keep this value secret."
 msgstr ""
 
-#: models.py:127
+#: models.py:143
 msgid "Platform's generated Private key ID"
 msgstr ""
 
-#: models.py:132
+#: models.py:148
 msgid "Platform's generated JWK keyset."
 msgstr ""
 
-#: models.py:138
+#: models.py:154
 msgid "Client ID used by LTI tool"
 msgstr ""
 
-#: models.py:148
+#: models.py:250
 msgid "LTI Configuration stores on XBlock needs a block location set."
 msgstr ""
 
-#: models.py:155
-msgid "Invalid LTI configuration."
+#: models.py:256
+msgid ""
+"LTI Configuration stored on the model for LTI 1.3 must have a value for one "
+"of lti_1p3_tool_public_key or lti_1p3_tool_keyset_url."
+msgstr ""
+
+#: models.py:263
+msgid ""
+"CONFIG_ON_XBLOCK and CONFIG_EXTERNAL are not supported for LTI 1.3 "
+"Proctoring Services."
 msgstr ""
 
-#: models.py:165
-msgid "Block location not set, it's not possible to retrieve the block."
+#: models.py:271
+msgid "Invalid LTI configuration."
 msgstr ""
 
-#: plugin/views.py:246
+#: plugin/views.py:453
 msgid "The selected content type is not supported by Open edX."
 msgstr ""
 
-#: plugin/views.py:261
+#: plugin/views.py:468
 msgid "You don't have access to save LTI Content Items."
 msgstr ""
 
-#: plugin/views.py:262
+#: plugin/views.py:469
 msgid ""
 "Please check that you have course staff permissions and double check this "
 "block's LTI settings."
 msgstr ""
 
 #: templates/html/lti-dl/dl_response_error.html:6
 msgid "LTI Deep Linking failed."
@@ -469,23 +531,14 @@
 msgid "The LTI Deep Linking content was successfully saved in the LMS."
 msgstr ""
 
 #: templates/html/lti-dl/dl_response_saved.html:13
 msgid "You can safely close this page now."
 msgstr ""
 
-#: templates/html/lti_1p3_launch_error.html:10
-msgid "There was an error while launching the LTI 1.3 tool."
-msgstr ""
-
-#: templates/html/lti_1p3_launch_error.html:13
-msgid ""
-"If you're seeing this on a live course, please contact the course staff."
-msgstr ""
-
 #: templates/html/lti_1p3_permission_error.html:10
 msgid "Unauthorized."
 msgstr ""
 
 #: templates/html/lti_1p3_permission_error.html:13
 msgid ""
 "Students don't have permissions to perform LTI Deep Linking configuration "
@@ -546,27 +599,46 @@
 msgid "Deep Linking Launch - Configure tool"
 msgstr ""
 
 #: templates/html/lti_launch.html:27
 msgid "Press to Launch"
 msgstr ""
 
-#: static/js/xblock_lti_consumer.js:142
-msgid ""
-"Click OK to have your username and e-mail address sent to a 3rd party application.\n"
-"\n"
-"Click Cancel to return to this page without sending your information."
+#: templates/html/lti_launch_error.html:10
+msgid "There was an error while launching the LTI tool."
 msgstr ""
 
-#: static/js/xblock_lti_consumer.js:144
+#: templates/html/lti_launch_error.html:13
+#: templates/html/lti_proctoring_start_error.html:13
 msgid ""
-"Click OK to have your username sent to a 3rd party application.\n"
-"\n"
-"Click Cancel to return to this page without sending your information."
+"If you're seeing this on a live course, please contact the course staff."
+msgstr ""
+
+#: templates/html/lti_proctoring_start_error.html:10
+msgid "There was an error while starting your LTI proctored assessment."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:126
+msgid "Cancel"
 msgstr ""
 
-#: static/js/xblock_lti_consumer.js:146
+#: static/js/xblock_lti_consumer.js:128
+msgid "OK"
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:157
 msgid ""
-"Click OK to have your e-mail address sent to a 3rd party application.\n"
-"\n"
-"Click Cancel to return to this page without sending your information."
+"Click OK to have your username and e-mail address sent to a 3rd party "
+"application."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:159
+msgid "Click OK to have your username sent to a 3rd party application."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:161
+msgid "Click OK to have your e-mail address sent to a 3rd party application."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:168
+msgid "Click Cancel to return to this page without sending your information."
 msgstr ""
```

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.0.2/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.2/lti_consumer/translations/ru/LC_MESSAGES/text.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,462 +1,522 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # 
 # Translators:
-# Renata Barboza, 2016
-# Simone Baldissera, 2021
 msgid ""
 msgstr ""
 "Project-Id-Version: XBlocks\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-02-01 17:24-0300\n"
+"POT-Creation-Date: 2023-04-11 15:09-0400\n"
 "PO-Revision-Date: 2016-06-08 14:38+0000\n"
-"Last-Translator: Simone Baldissera, 2021\n"
-"Language-Team: Portuguese (Brazil) (http://app.transifex.com/open-edx/xblocks/language/pt_BR/)\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: Russian (http://app.transifex.com/open-edx/xblocks/language/ru/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: pt_BR\n"
-"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
+"Language: ru\n"
+"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n%100>=11 && n%100<=14)? 2 : 3);\n"
 
-#: lti_1p3/extensions/rest_framework/authentication.py:40
+#: lti_1p3/extensions/rest_framework/authentication.py:41
 msgid "Missing LTI 1.3 authentication token."
 msgstr ""
 
-#: lti_1p3/extensions/rest_framework/authentication.py:44
+#: lti_1p3/extensions/rest_framework/authentication.py:45
 msgid "Invalid token header. No credentials provided."
 msgstr ""
 
-#: lti_1p3/extensions/rest_framework/authentication.py:48
+#: lti_1p3/extensions/rest_framework/authentication.py:49
 msgid "Invalid token header. Token string should not contain spaces."
 msgstr ""
 
-#: lti_1p3/extensions/rest_framework/authentication.py:56
+#: lti_1p3/extensions/rest_framework/authentication.py:57
 msgid "LTI configuration not found."
 msgstr ""
 
-#: lti_1p3/extensions/rest_framework/authentication.py:65
+#: lti_1p3/extensions/rest_framework/authentication.py:66
 msgid "Invalid token signature."
 msgstr ""
 
-#: lti_xblock.py:127
+#: lti_xblock.py:126
 msgid "No valid user id found in endpoint URL"
-msgstr "Nenhuma ID de usuário válido encontrada no ponto de extremidade da URL"
+msgstr ""
+
+#: lti_xblock.py:139
+msgid "Configuration on block"
+msgstr ""
+
+#: lti_xblock.py:143
+msgid "Database Configuration"
+msgstr ""
 
-#: lti_xblock.py:233
+#: lti_xblock.py:146
+msgid "Reusable Configuration"
+msgstr ""
+
+#: lti_xblock.py:253
 msgid "Display Name"
-msgstr "Nome de exibição"
+msgstr ""
 
-#: lti_xblock.py:235
+#: lti_xblock.py:255
 msgid ""
 "Enter the name that students see for this component. Analytics reports may "
 "also use the display name to identify this component."
-msgstr "Forneça o nome que os alunos verão para este componente. Os relatórios de análise também poderão usar o nome de exibição para identificar este componente. "
+msgstr ""
 
-#: lti_xblock.py:239
+#: lti_xblock.py:259
 msgid "LTI Consumer"
-msgstr "Consumidor de LTI"
+msgstr ""
 
-#: lti_xblock.py:242
+#: lti_xblock.py:262
 msgid "LTI Application Information"
-msgstr "Informações do aplicativo LTI"
+msgstr ""
 
-#: lti_xblock.py:244
+#: lti_xblock.py:264
 msgid ""
 "Enter a description of the third party application. If requesting username "
 "and/or email, use this text box to inform users why their username and/or "
 "email will be forwarded to a third party application."
 msgstr ""
 
-#: lti_xblock.py:254
+#: lti_xblock.py:272
+msgid "Configuration Type"
+msgstr ""
+
+#: lti_xblock.py:277
+msgid ""
+"Select 'Configuration on block' to configure a new LTI Tool. If the support "
+"staff provided you with a pre-configured LTI reusable Tool ID, "
+"select'Reusable Configuration' and enter it in the text field below."
+msgstr ""
+
+#: lti_xblock.py:284
 msgid "LTI Version"
 msgstr ""
 
-#: lti_xblock.py:262
+#: lti_xblock.py:292
 msgid ""
 "Select the LTI version that your tool supports.<br />The XBlock LTI Consumer"
 " fully supports LTI 1.1.1, LTI 1.3 and LTI Advantage features."
 msgstr ""
 
-#: lti_xblock.py:268
+#: lti_xblock.py:299
+msgid "LTI Reusable Configuration ID"
+msgstr ""
+
+#: lti_xblock.py:301
+msgid ""
+"Enter the reusable LTI external configuration ID provided by the support "
+"staff."
+msgstr ""
+
+#: lti_xblock.py:306
 msgid "Tool Launch URL"
 msgstr ""
 
-#: lti_xblock.py:272
+#: lti_xblock.py:310
 msgid ""
 "Enter the LTI 1.3 Tool Launch URL. <br />This is the URL the LMS will use to"
 " launch the LTI Tool."
 msgstr ""
 
-#: lti_xblock.py:277
+#: lti_xblock.py:315
 msgid "Tool Initiate Login URL"
 msgstr ""
 
-#: lti_xblock.py:281
+#: lti_xblock.py:319
 msgid ""
 "Enter the LTI 1.3 Tool OIDC Authorization url (can also be called login or "
 "login initiation URL).<br />This is the URL the LMS will use to start a LTI "
 "authorization prior to doing the launch request."
 msgstr ""
 
-#: lti_xblock.py:288
+#: lti_xblock.py:325
+msgid "Registered Redirect URIs"
+msgstr ""
+
+#: lti_xblock.py:327
+msgid ""
+"Valid urls the Tool may request us to redirect the id token to. The redirect"
+" uris are often the same as the launch url/deep linking url so if this field"
+" is empty, it will use them as the default. If you need to use different "
+"redirect uri's, enter them here. If you use this field you must enter all "
+"valid redirect uri's the tool may request."
+msgstr ""
+
+#: lti_xblock.py:337
 msgid "Tool Public Key Mode"
 msgstr ""
 
-#: lti_xblock.py:296
+#: lti_xblock.py:345
 msgid "Select how the tool's public key information will be specified."
 msgstr ""
 
-#: lti_xblock.py:300
+#: lti_xblock.py:349
 msgid "Tool Keyset URL"
 msgstr ""
 
-#: lti_xblock.py:304
+#: lti_xblock.py:353
 msgid ""
 "Enter the LTI 1.3 Tool's JWK keysets URL.<br />This link should retrieve a "
 "JSON file containing public keys and signature algorithm information, so "
 "that the LMS can check if the messages and launch requests received have the"
 " signature from the tool.<br /><b>This is not required when doing LTI 1.3 "
 "Launches without LTI Advantage nor Basic Outcomes requests.</b>"
 msgstr ""
 
-#: lti_xblock.py:314
+#: lti_xblock.py:363
 msgid "Tool Public Key"
 msgstr ""
 
-#: lti_xblock.py:319
+#: lti_xblock.py:368
 msgid ""
 "Enter the LTI 1.3 Tool's public key.<br />This is a string that starts with "
 "'-----BEGIN PUBLIC KEY-----' and is required so that the LMS can check if "
 "the messages and launch requests received have the signature from the "
 "tool.<br /><b>This is not required when doing LTI 1.3 Launches without LTI "
 "Advantage nor Basic Outcomes requests.</b>"
 msgstr ""
 
-#: lti_xblock.py:329
+#: lti_xblock.py:378
 msgid "Enable LTI NRPS"
 msgstr ""
 
-#: lti_xblock.py:330
+#: lti_xblock.py:379
 msgid "Enable LTI Names and Role Provisioning Services."
 msgstr ""
 
-#: lti_xblock.py:337
+#: lti_xblock.py:386
 msgid "LTI 1.3 Block Client ID - DEPRECATED"
 msgstr ""
 
-#: lti_xblock.py:340
+#: lti_xblock.py:389
 msgid "DEPRECATED - This is now stored in the LtiConfiguration model."
 msgstr ""
 
-#: lti_xblock.py:343
+#: lti_xblock.py:392
 msgid "LTI 1.3 Block Key - DEPRECATED"
 msgstr ""
 
-#: lti_xblock.py:350
+#: lti_xblock.py:399
 msgid "Deep linking"
 msgstr ""
 
-#: lti_xblock.py:351
+#: lti_xblock.py:400
 msgid "Select True if you want to enable LTI Advantage Deep Linking."
 msgstr ""
 
-#: lti_xblock.py:356
+#: lti_xblock.py:405
 msgid "Deep Linking Launch URL"
 msgstr ""
 
-#: lti_xblock.py:360
+#: lti_xblock.py:409
 msgid ""
 "Enter the LTI Advantage Deep Linking Launch URL. If the tool does not "
 "specify one, use the same value as 'Tool Launch URL'."
 msgstr ""
 
-#: lti_xblock.py:365
+#: lti_xblock.py:414
 msgid "LTI Assignment and Grades Service"
 msgstr ""
 
-#: lti_xblock.py:367
+#: lti_xblock.py:416
 msgid "Disabled"
 msgstr ""
 
-#: lti_xblock.py:368
+#: lti_xblock.py:417
 msgid "Allow tools to submit grades only (declarative)"
 msgstr ""
 
-#: lti_xblock.py:369
+#: lti_xblock.py:418
 msgid "Allow tools to manage and submit grade (programmatic)"
 msgstr ""
 
-#: lti_xblock.py:374
+#: lti_xblock.py:423
 msgid ""
 "Enable the LTI-AGS service and select the functionality enabled for LTI "
 "tools. The 'declarative' mode (default) will provide a tool with a LineItem "
 "created from the XBlock settings, while the 'programmatic' one will allow "
 "tools to manage, create and link the grades."
 msgstr ""
 
-#: lti_xblock.py:382
+#: lti_xblock.py:431
 msgid "LTI ID"
-msgstr "ID do LTI"
+msgstr ""
 
-#: lti_xblock.py:384
+#: lti_xblock.py:433
 #, python-brace-format
 msgid ""
 "Enter the LTI ID for the external LTI provider. This value must be the same "
 "LTI ID that you entered in the LTI Passports setting on the Advanced "
 "Settings page.<br />See the {docs_anchor_open}edX LTI "
 "documentation{anchor_close} for more details on this setting."
 msgstr ""
 
-#: lti_xblock.py:396
+#: lti_xblock.py:445
 msgid "LTI URL"
 msgstr ""
 
-#: lti_xblock.py:398
+#: lti_xblock.py:447
 #, python-brace-format
 msgid ""
 "Enter the URL of the external tool that this component launches. This "
 "setting is only used when Hide External Tool is set to False.<br />See the "
 "{docs_anchor_open}edX LTI documentation{anchor_close} for more details on "
 "this setting."
 msgstr ""
 
-#: lti_xblock.py:411
+#: lti_xblock.py:460
 msgid "Custom Parameters"
 msgstr ""
 
-#: lti_xblock.py:413
+#: lti_xblock.py:462
 #, python-brace-format
 msgid ""
 "Add the key/value pair for any custom parameters, such as the page your "
 "e-book should open to or the background color for this component. Ex. "
 "[\"page=1\", \"color=white\"]<br />See the {docs_anchor_open}edX LTI "
 "documentation{anchor_close} for more details on this setting."
 msgstr ""
 
-#: lti_xblock.py:423
+#: lti_xblock.py:472
 msgid "LTI Launch Target"
 msgstr ""
 
-#: lti_xblock.py:425
+#: lti_xblock.py:474
 msgid ""
 "Select Inline if you want the LTI content to open in an IFrame in the "
 "current page. Select Modal if you want the LTI content to open in a modal "
 "window in the current page. Select New Window if you want the LTI content to"
 " open in a new browser window. This setting is only used when Hide External "
 "Tool is set to False."
 msgstr ""
 
-#: lti_xblock.py:439
+#: lti_xblock.py:488
 msgid "Button Text"
 msgstr ""
 
-#: lti_xblock.py:441
+#: lti_xblock.py:490
 msgid ""
 "Enter the text on the button used to launch the third party application. "
 "This setting is only used when Hide External Tool is set to False and LTI "
 "Launch Target is set to Modal or New Window."
 msgstr ""
 
-#: lti_xblock.py:449
+#: lti_xblock.py:498
 msgid "Inline Height"
-msgstr "Altura do embutido"
+msgstr ""
 
-#: lti_xblock.py:451
+#: lti_xblock.py:500
 msgid ""
 "Enter the desired pixel height of the iframe which will contain the LTI "
 "tool. This setting is only used when Hide External Tool is set to False and "
 "LTI Launch Target is set to Inline."
 msgstr ""
 
-#: lti_xblock.py:459
+#: lti_xblock.py:508
 msgid "Modal Height"
-msgstr "Altura do modal"
+msgstr ""
 
-#: lti_xblock.py:461
+#: lti_xblock.py:510
 msgid ""
 "Enter the desired viewport percentage height of the modal overlay which will"
 " contain the LTI tool. This setting is only used when Hide External Tool is "
 "set to False and LTI Launch Target is set to Modal."
 msgstr ""
 
-#: lti_xblock.py:469
+#: lti_xblock.py:518
 msgid "Modal Width"
-msgstr "Largura do modal"
+msgstr ""
 
-#: lti_xblock.py:471
+#: lti_xblock.py:520
 msgid ""
 "Enter the desired viewport percentage width of the modal overlay which will "
 "contain the LTI tool. This setting is only used when Hide External Tool is "
 "set to False and LTI Launch Target is set to Modal."
 msgstr ""
 
-#: lti_xblock.py:479
+#: lti_xblock.py:528
 msgid "Scored"
 msgstr ""
 
-#: lti_xblock.py:480
+#: lti_xblock.py:529
 msgid ""
 "Select True if this component will receive a numerical score from the "
 "external LTI system."
 msgstr ""
 
-#: lti_xblock.py:487
+#: lti_xblock.py:536
 msgid ""
 "Enter the number of points possible for this component.  The default value "
 "is 1.0.  This setting is only used when Scored is set to True."
 msgstr ""
 
-#: lti_xblock.py:496
+#: lti_xblock.py:545
 msgid ""
 "The score kept in the xblock KVS -- duplicate of the published score in "
 "django DB"
 msgstr ""
 
-#: lti_xblock.py:501
+#: lti_xblock.py:550
 msgid "Comment as returned from grader, LTI2.0 spec"
 msgstr ""
 
-#: lti_xblock.py:506
+#: lti_xblock.py:555
 msgid "Hide External Tool"
 msgstr ""
 
-#: lti_xblock.py:508
+#: lti_xblock.py:557
 msgid ""
 "Select True if you want to use this component as a placeholder for syncing "
 "with an external grading  system rather than launch an external tool.  This "
 "setting hides the Launch button and any IFrames for this component."
 msgstr ""
 
-#: lti_xblock.py:516
+#: lti_xblock.py:565
 msgid "Accept grades past deadline"
 msgstr ""
 
-#: lti_xblock.py:517
+#: lti_xblock.py:566
 msgid ""
 "Select True to allow third party systems to post grades past the deadline."
 msgstr ""
 
-#: lti_xblock.py:525
+#: lti_xblock.py:574
 msgid "Request user's username"
 msgstr ""
 
 #. Translators: This is used to request the user's username for a third party
 #. service.
-#: lti_xblock.py:527
+#: lti_xblock.py:576
 msgid "Select True to request the user's username."
 msgstr ""
 
-#: lti_xblock.py:532
+#: lti_xblock.py:581
 msgid "Request user's email"
 msgstr ""
 
 #. Translators: This is used to request the user's email for a third party
 #. service.
-#: lti_xblock.py:534
+#: lti_xblock.py:583
 msgid "Select True to request the user's email address."
 msgstr ""
 
-#: lti_xblock.py:539
+#: lti_xblock.py:588
 msgid "Send extra parameters"
 msgstr ""
 
-#: lti_xblock.py:540
+#: lti_xblock.py:589
 msgid ""
 "Select True to send the extra parameters, which might contain Personally "
 "Identifiable Information. The processors are site-wide, please consult the "
 "site administrator if you have any questions."
 msgstr ""
 
-#: lti_xblock.py:603
+#: lti_xblock.py:652
 msgid "Custom Parameters must be a list"
 msgstr ""
 
-#: lti_xblock.py:713
+#: lti_xblock.py:783 lti_xblock.py:1062
+msgid "Could not get user data for current request"
+msgstr ""
+
+#: lti_xblock.py:810
 msgid ""
 "Could not parse LTI passport: {lti_passport!r}. Should be \"id:key:secret\" "
 "string."
 msgstr ""
 
-#: lti_xblock.py:729 lti_xblock.py:745
+#: lti_xblock.py:828 lti_xblock.py:842 lti_xblock.py:858
 msgid "Could not get user id for current request"
 msgstr ""
 
-#: lti_xblock.py:850
+#: lti_xblock.py:994
 msgid ""
 "Could not parse custom parameter: {custom_parameter!r}. Should be \"x=y\" "
 "string."
 msgstr ""
 
-#: lti_xblock.py:1310
+#: lti_xblock.py:1343
 msgid "[LTI]: Real user not found against anon_id: {}"
 msgstr ""
 
-#: models.py:72
+#: models.py:79
 msgid "Configuration Stored on XBlock fields"
 msgstr ""
 
-#: models.py:73
+#: models.py:80
 msgid "Configuration Stored on this model"
 msgstr ""
 
-#: models.py:97
+#: models.py:81
+msgid "Configuration Stored on external service"
+msgstr ""
+
+#: models.py:113
 msgid "LTI configuration data."
 msgstr ""
 
-#: models.py:104
+#: models.py:120
 msgid "The URL of the external tool that initiates the launch."
 msgstr ""
 
-#: models.py:109
+#: models.py:125
 msgid "Client key provided by the LTI tool provider."
 msgstr ""
 
-#: models.py:115
+#: models.py:131
 msgid "Client secret provided by the LTI tool provider."
 msgstr ""
 
-#: models.py:121
+#: models.py:137
 msgid "Platform's generated Private key. Keep this value secret."
 msgstr ""
 
-#: models.py:127
+#: models.py:143
 msgid "Platform's generated Private key ID"
 msgstr ""
 
-#: models.py:132
+#: models.py:148
 msgid "Platform's generated JWK keyset."
 msgstr ""
 
-#: models.py:138
+#: models.py:154
 msgid "Client ID used by LTI tool"
 msgstr ""
 
-#: models.py:148
+#: models.py:250
 msgid "LTI Configuration stores on XBlock needs a block location set."
 msgstr ""
 
-#: models.py:155
-msgid "Invalid LTI configuration."
+#: models.py:256
+msgid ""
+"LTI Configuration stored on the model for LTI 1.3 must have a value for one "
+"of lti_1p3_tool_public_key or lti_1p3_tool_keyset_url."
 msgstr ""
 
-#: models.py:165
-msgid "Block location not set, it's not possible to retrieve the block."
+#: models.py:263
+msgid ""
+"CONFIG_ON_XBLOCK and CONFIG_EXTERNAL are not supported for LTI 1.3 "
+"Proctoring Services."
 msgstr ""
 
-#: plugin/views.py:246
+#: models.py:271
+msgid "Invalid LTI configuration."
+msgstr ""
+
+#: plugin/views.py:453
 msgid "The selected content type is not supported by Open edX."
 msgstr ""
 
-#: plugin/views.py:261
+#: plugin/views.py:468
 msgid "You don't have access to save LTI Content Items."
 msgstr ""
 
-#: plugin/views.py:262
+#: plugin/views.py:469
 msgid ""
 "Please check that you have course staff permissions and double check this "
 "block's LTI settings."
 msgstr ""
 
 #: templates/html/lti-dl/dl_response_error.html:6
 msgid "LTI Deep Linking failed."
@@ -470,23 +530,14 @@
 msgid "The LTI Deep Linking content was successfully saved in the LMS."
 msgstr ""
 
 #: templates/html/lti-dl/dl_response_saved.html:13
 msgid "You can safely close this page now."
 msgstr ""
 
-#: templates/html/lti_1p3_launch_error.html:10
-msgid "There was an error while launching the LTI 1.3 tool."
-msgstr ""
-
-#: templates/html/lti_1p3_launch_error.html:13
-msgid ""
-"If you're seeing this on a live course, please contact the course staff."
-msgstr ""
-
 #: templates/html/lti_1p3_permission_error.html:10
 msgid "Unauthorized."
 msgstr ""
 
 #: templates/html/lti_1p3_permission_error.html:13
 msgid ""
 "Students don't have permissions to perform LTI Deep Linking configuration "
@@ -547,27 +598,46 @@
 msgid "Deep Linking Launch - Configure tool"
 msgstr ""
 
 #: templates/html/lti_launch.html:27
 msgid "Press to Launch"
 msgstr ""
 
-#: static/js/xblock_lti_consumer.js:142
-msgid ""
-"Click OK to have your username and e-mail address sent to a 3rd party application.\n"
-"\n"
-"Click Cancel to return to this page without sending your information."
+#: templates/html/lti_launch_error.html:10
+msgid "There was an error while launching the LTI tool."
 msgstr ""
 
-#: static/js/xblock_lti_consumer.js:144
+#: templates/html/lti_launch_error.html:13
+#: templates/html/lti_proctoring_start_error.html:13
 msgid ""
-"Click OK to have your username sent to a 3rd party application.\n"
-"\n"
-"Click Cancel to return to this page without sending your information."
+"If you're seeing this on a live course, please contact the course staff."
 msgstr ""
 
-#: static/js/xblock_lti_consumer.js:146
+#: templates/html/lti_proctoring_start_error.html:10
+msgid "There was an error while starting your LTI proctored assessment."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:126
+msgid "Cancel"
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:128
+msgid "OK"
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:157
 msgid ""
-"Click OK to have your e-mail address sent to a 3rd party application.\n"
-"\n"
-"Click Cancel to return to this page without sending your information."
+"Click OK to have your username and e-mail address sent to a 3rd party "
+"application."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:159
+msgid "Click OK to have your username sent to a 3rd party application."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:161
+msgid "Click OK to have your e-mail address sent to a 3rd party application."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:168
+msgid "Click Cancel to return to this page without sending your information."
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.0.2/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.2/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/translations/ru/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.0.2/lti_consumer/translations/ru/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/translations/ru/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.2/lti_consumer/translations/hi/LC_MESSAGES/text.po`

 * *Files 9% similar despite different names*

```diff
@@ -3,458 +3,520 @@
 # This file is distributed under the same license as the PACKAGE package.
 # 
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: XBlocks\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-02-01 17:24-0300\n"
+"POT-Creation-Date: 2023-04-11 15:09-0400\n"
 "PO-Revision-Date: 2016-06-08 14:38+0000\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: Russian (http://app.transifex.com/open-edx/xblocks/language/ru/)\n"
+"Language-Team: Hindi (http://app.transifex.com/open-edx/xblocks/language/hi/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: ru\n"
-"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n%100>=11 && n%100<=14)? 2 : 3);\n"
+"Language: hi\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: lti_1p3/extensions/rest_framework/authentication.py:40
+#: lti_1p3/extensions/rest_framework/authentication.py:41
 msgid "Missing LTI 1.3 authentication token."
 msgstr ""
 
-#: lti_1p3/extensions/rest_framework/authentication.py:44
+#: lti_1p3/extensions/rest_framework/authentication.py:45
 msgid "Invalid token header. No credentials provided."
 msgstr ""
 
-#: lti_1p3/extensions/rest_framework/authentication.py:48
+#: lti_1p3/extensions/rest_framework/authentication.py:49
 msgid "Invalid token header. Token string should not contain spaces."
 msgstr ""
 
-#: lti_1p3/extensions/rest_framework/authentication.py:56
+#: lti_1p3/extensions/rest_framework/authentication.py:57
 msgid "LTI configuration not found."
 msgstr ""
 
-#: lti_1p3/extensions/rest_framework/authentication.py:65
+#: lti_1p3/extensions/rest_framework/authentication.py:66
 msgid "Invalid token signature."
 msgstr ""
 
-#: lti_xblock.py:127
+#: lti_xblock.py:126
 msgid "No valid user id found in endpoint URL"
 msgstr ""
 
-#: lti_xblock.py:233
+#: lti_xblock.py:139
+msgid "Configuration on block"
+msgstr ""
+
+#: lti_xblock.py:143
+msgid "Database Configuration"
+msgstr ""
+
+#: lti_xblock.py:146
+msgid "Reusable Configuration"
+msgstr ""
+
+#: lti_xblock.py:253
 msgid "Display Name"
 msgstr ""
 
-#: lti_xblock.py:235
+#: lti_xblock.py:255
 msgid ""
 "Enter the name that students see for this component. Analytics reports may "
 "also use the display name to identify this component."
 msgstr ""
 
-#: lti_xblock.py:239
+#: lti_xblock.py:259
 msgid "LTI Consumer"
 msgstr ""
 
-#: lti_xblock.py:242
+#: lti_xblock.py:262
 msgid "LTI Application Information"
 msgstr ""
 
-#: lti_xblock.py:244
+#: lti_xblock.py:264
 msgid ""
 "Enter a description of the third party application. If requesting username "
 "and/or email, use this text box to inform users why their username and/or "
 "email will be forwarded to a third party application."
 msgstr ""
 
-#: lti_xblock.py:254
+#: lti_xblock.py:272
+msgid "Configuration Type"
+msgstr ""
+
+#: lti_xblock.py:277
+msgid ""
+"Select 'Configuration on block' to configure a new LTI Tool. If the support "
+"staff provided you with a pre-configured LTI reusable Tool ID, "
+"select'Reusable Configuration' and enter it in the text field below."
+msgstr ""
+
+#: lti_xblock.py:284
 msgid "LTI Version"
 msgstr ""
 
-#: lti_xblock.py:262
+#: lti_xblock.py:292
 msgid ""
 "Select the LTI version that your tool supports.<br />The XBlock LTI Consumer"
 " fully supports LTI 1.1.1, LTI 1.3 and LTI Advantage features."
 msgstr ""
 
-#: lti_xblock.py:268
+#: lti_xblock.py:299
+msgid "LTI Reusable Configuration ID"
+msgstr ""
+
+#: lti_xblock.py:301
+msgid ""
+"Enter the reusable LTI external configuration ID provided by the support "
+"staff."
+msgstr ""
+
+#: lti_xblock.py:306
 msgid "Tool Launch URL"
 msgstr ""
 
-#: lti_xblock.py:272
+#: lti_xblock.py:310
 msgid ""
 "Enter the LTI 1.3 Tool Launch URL. <br />This is the URL the LMS will use to"
 " launch the LTI Tool."
 msgstr ""
 
-#: lti_xblock.py:277
+#: lti_xblock.py:315
 msgid "Tool Initiate Login URL"
 msgstr ""
 
-#: lti_xblock.py:281
+#: lti_xblock.py:319
 msgid ""
 "Enter the LTI 1.3 Tool OIDC Authorization url (can also be called login or "
 "login initiation URL).<br />This is the URL the LMS will use to start a LTI "
 "authorization prior to doing the launch request."
 msgstr ""
 
-#: lti_xblock.py:288
+#: lti_xblock.py:325
+msgid "Registered Redirect URIs"
+msgstr ""
+
+#: lti_xblock.py:327
+msgid ""
+"Valid urls the Tool may request us to redirect the id token to. The redirect"
+" uris are often the same as the launch url/deep linking url so if this field"
+" is empty, it will use them as the default. If you need to use different "
+"redirect uri's, enter them here. If you use this field you must enter all "
+"valid redirect uri's the tool may request."
+msgstr ""
+
+#: lti_xblock.py:337
 msgid "Tool Public Key Mode"
 msgstr ""
 
-#: lti_xblock.py:296
+#: lti_xblock.py:345
 msgid "Select how the tool's public key information will be specified."
 msgstr ""
 
-#: lti_xblock.py:300
+#: lti_xblock.py:349
 msgid "Tool Keyset URL"
 msgstr ""
 
-#: lti_xblock.py:304
+#: lti_xblock.py:353
 msgid ""
 "Enter the LTI 1.3 Tool's JWK keysets URL.<br />This link should retrieve a "
 "JSON file containing public keys and signature algorithm information, so "
 "that the LMS can check if the messages and launch requests received have the"
 " signature from the tool.<br /><b>This is not required when doing LTI 1.3 "
 "Launches without LTI Advantage nor Basic Outcomes requests.</b>"
 msgstr ""
 
-#: lti_xblock.py:314
+#: lti_xblock.py:363
 msgid "Tool Public Key"
 msgstr ""
 
-#: lti_xblock.py:319
+#: lti_xblock.py:368
 msgid ""
 "Enter the LTI 1.3 Tool's public key.<br />This is a string that starts with "
 "'-----BEGIN PUBLIC KEY-----' and is required so that the LMS can check if "
 "the messages and launch requests received have the signature from the "
 "tool.<br /><b>This is not required when doing LTI 1.3 Launches without LTI "
 "Advantage nor Basic Outcomes requests.</b>"
 msgstr ""
 
-#: lti_xblock.py:329
+#: lti_xblock.py:378
 msgid "Enable LTI NRPS"
 msgstr ""
 
-#: lti_xblock.py:330
+#: lti_xblock.py:379
 msgid "Enable LTI Names and Role Provisioning Services."
 msgstr ""
 
-#: lti_xblock.py:337
+#: lti_xblock.py:386
 msgid "LTI 1.3 Block Client ID - DEPRECATED"
 msgstr ""
 
-#: lti_xblock.py:340
+#: lti_xblock.py:389
 msgid "DEPRECATED - This is now stored in the LtiConfiguration model."
 msgstr ""
 
-#: lti_xblock.py:343
+#: lti_xblock.py:392
 msgid "LTI 1.3 Block Key - DEPRECATED"
 msgstr ""
 
-#: lti_xblock.py:350
+#: lti_xblock.py:399
 msgid "Deep linking"
 msgstr ""
 
-#: lti_xblock.py:351
+#: lti_xblock.py:400
 msgid "Select True if you want to enable LTI Advantage Deep Linking."
 msgstr ""
 
-#: lti_xblock.py:356
+#: lti_xblock.py:405
 msgid "Deep Linking Launch URL"
 msgstr ""
 
-#: lti_xblock.py:360
+#: lti_xblock.py:409
 msgid ""
 "Enter the LTI Advantage Deep Linking Launch URL. If the tool does not "
 "specify one, use the same value as 'Tool Launch URL'."
 msgstr ""
 
-#: lti_xblock.py:365
+#: lti_xblock.py:414
 msgid "LTI Assignment and Grades Service"
 msgstr ""
 
-#: lti_xblock.py:367
+#: lti_xblock.py:416
 msgid "Disabled"
 msgstr ""
 
-#: lti_xblock.py:368
+#: lti_xblock.py:417
 msgid "Allow tools to submit grades only (declarative)"
 msgstr ""
 
-#: lti_xblock.py:369
+#: lti_xblock.py:418
 msgid "Allow tools to manage and submit grade (programmatic)"
 msgstr ""
 
-#: lti_xblock.py:374
+#: lti_xblock.py:423
 msgid ""
 "Enable the LTI-AGS service and select the functionality enabled for LTI "
 "tools. The 'declarative' mode (default) will provide a tool with a LineItem "
 "created from the XBlock settings, while the 'programmatic' one will allow "
 "tools to manage, create and link the grades."
 msgstr ""
 
-#: lti_xblock.py:382
+#: lti_xblock.py:431
 msgid "LTI ID"
 msgstr ""
 
-#: lti_xblock.py:384
+#: lti_xblock.py:433
 #, python-brace-format
 msgid ""
 "Enter the LTI ID for the external LTI provider. This value must be the same "
 "LTI ID that you entered in the LTI Passports setting on the Advanced "
 "Settings page.<br />See the {docs_anchor_open}edX LTI "
 "documentation{anchor_close} for more details on this setting."
 msgstr ""
 
-#: lti_xblock.py:396
+#: lti_xblock.py:445
 msgid "LTI URL"
 msgstr ""
 
-#: lti_xblock.py:398
+#: lti_xblock.py:447
 #, python-brace-format
 msgid ""
 "Enter the URL of the external tool that this component launches. This "
 "setting is only used when Hide External Tool is set to False.<br />See the "
 "{docs_anchor_open}edX LTI documentation{anchor_close} for more details on "
 "this setting."
 msgstr ""
 
-#: lti_xblock.py:411
+#: lti_xblock.py:460
 msgid "Custom Parameters"
 msgstr ""
 
-#: lti_xblock.py:413
+#: lti_xblock.py:462
 #, python-brace-format
 msgid ""
 "Add the key/value pair for any custom parameters, such as the page your "
 "e-book should open to or the background color for this component. Ex. "
 "[\"page=1\", \"color=white\"]<br />See the {docs_anchor_open}edX LTI "
 "documentation{anchor_close} for more details on this setting."
 msgstr ""
 
-#: lti_xblock.py:423
+#: lti_xblock.py:472
 msgid "LTI Launch Target"
 msgstr ""
 
-#: lti_xblock.py:425
+#: lti_xblock.py:474
 msgid ""
 "Select Inline if you want the LTI content to open in an IFrame in the "
 "current page. Select Modal if you want the LTI content to open in a modal "
 "window in the current page. Select New Window if you want the LTI content to"
 " open in a new browser window. This setting is only used when Hide External "
 "Tool is set to False."
 msgstr ""
 
-#: lti_xblock.py:439
+#: lti_xblock.py:488
 msgid "Button Text"
 msgstr ""
 
-#: lti_xblock.py:441
+#: lti_xblock.py:490
 msgid ""
 "Enter the text on the button used to launch the third party application. "
 "This setting is only used when Hide External Tool is set to False and LTI "
 "Launch Target is set to Modal or New Window."
 msgstr ""
 
-#: lti_xblock.py:449
+#: lti_xblock.py:498
 msgid "Inline Height"
 msgstr ""
 
-#: lti_xblock.py:451
+#: lti_xblock.py:500
 msgid ""
 "Enter the desired pixel height of the iframe which will contain the LTI "
 "tool. This setting is only used when Hide External Tool is set to False and "
 "LTI Launch Target is set to Inline."
 msgstr ""
 
-#: lti_xblock.py:459
+#: lti_xblock.py:508
 msgid "Modal Height"
 msgstr ""
 
-#: lti_xblock.py:461
+#: lti_xblock.py:510
 msgid ""
 "Enter the desired viewport percentage height of the modal overlay which will"
 " contain the LTI tool. This setting is only used when Hide External Tool is "
 "set to False and LTI Launch Target is set to Modal."
 msgstr ""
 
-#: lti_xblock.py:469
+#: lti_xblock.py:518
 msgid "Modal Width"
 msgstr ""
 
-#: lti_xblock.py:471
+#: lti_xblock.py:520
 msgid ""
 "Enter the desired viewport percentage width of the modal overlay which will "
 "contain the LTI tool. This setting is only used when Hide External Tool is "
 "set to False and LTI Launch Target is set to Modal."
 msgstr ""
 
-#: lti_xblock.py:479
+#: lti_xblock.py:528
 msgid "Scored"
 msgstr ""
 
-#: lti_xblock.py:480
+#: lti_xblock.py:529
 msgid ""
 "Select True if this component will receive a numerical score from the "
 "external LTI system."
 msgstr ""
 
-#: lti_xblock.py:487
+#: lti_xblock.py:536
 msgid ""
 "Enter the number of points possible for this component.  The default value "
 "is 1.0.  This setting is only used when Scored is set to True."
 msgstr ""
 
-#: lti_xblock.py:496
+#: lti_xblock.py:545
 msgid ""
 "The score kept in the xblock KVS -- duplicate of the published score in "
 "django DB"
 msgstr ""
 
-#: lti_xblock.py:501
+#: lti_xblock.py:550
 msgid "Comment as returned from grader, LTI2.0 spec"
 msgstr ""
 
-#: lti_xblock.py:506
+#: lti_xblock.py:555
 msgid "Hide External Tool"
 msgstr ""
 
-#: lti_xblock.py:508
+#: lti_xblock.py:557
 msgid ""
 "Select True if you want to use this component as a placeholder for syncing "
 "with an external grading  system rather than launch an external tool.  This "
 "setting hides the Launch button and any IFrames for this component."
 msgstr ""
 
-#: lti_xblock.py:516
+#: lti_xblock.py:565
 msgid "Accept grades past deadline"
 msgstr ""
 
-#: lti_xblock.py:517
+#: lti_xblock.py:566
 msgid ""
 "Select True to allow third party systems to post grades past the deadline."
 msgstr ""
 
-#: lti_xblock.py:525
+#: lti_xblock.py:574
 msgid "Request user's username"
 msgstr ""
 
 #. Translators: This is used to request the user's username for a third party
 #. service.
-#: lti_xblock.py:527
+#: lti_xblock.py:576
 msgid "Select True to request the user's username."
 msgstr ""
 
-#: lti_xblock.py:532
+#: lti_xblock.py:581
 msgid "Request user's email"
 msgstr ""
 
 #. Translators: This is used to request the user's email for a third party
 #. service.
-#: lti_xblock.py:534
+#: lti_xblock.py:583
 msgid "Select True to request the user's email address."
 msgstr ""
 
-#: lti_xblock.py:539
+#: lti_xblock.py:588
 msgid "Send extra parameters"
 msgstr ""
 
-#: lti_xblock.py:540
+#: lti_xblock.py:589
 msgid ""
 "Select True to send the extra parameters, which might contain Personally "
 "Identifiable Information. The processors are site-wide, please consult the "
 "site administrator if you have any questions."
 msgstr ""
 
-#: lti_xblock.py:603
+#: lti_xblock.py:652
 msgid "Custom Parameters must be a list"
 msgstr ""
 
-#: lti_xblock.py:713
+#: lti_xblock.py:783 lti_xblock.py:1062
+msgid "Could not get user data for current request"
+msgstr ""
+
+#: lti_xblock.py:810
 msgid ""
 "Could not parse LTI passport: {lti_passport!r}. Should be \"id:key:secret\" "
 "string."
 msgstr ""
 
-#: lti_xblock.py:729 lti_xblock.py:745
+#: lti_xblock.py:828 lti_xblock.py:842 lti_xblock.py:858
 msgid "Could not get user id for current request"
 msgstr ""
 
-#: lti_xblock.py:850
+#: lti_xblock.py:994
 msgid ""
 "Could not parse custom parameter: {custom_parameter!r}. Should be \"x=y\" "
 "string."
 msgstr ""
 
-#: lti_xblock.py:1310
+#: lti_xblock.py:1343
 msgid "[LTI]: Real user not found against anon_id: {}"
 msgstr ""
 
-#: models.py:72
+#: models.py:79
 msgid "Configuration Stored on XBlock fields"
 msgstr ""
 
-#: models.py:73
+#: models.py:80
 msgid "Configuration Stored on this model"
 msgstr ""
 
-#: models.py:97
+#: models.py:81
+msgid "Configuration Stored on external service"
+msgstr ""
+
+#: models.py:113
 msgid "LTI configuration data."
 msgstr ""
 
-#: models.py:104
+#: models.py:120
 msgid "The URL of the external tool that initiates the launch."
 msgstr ""
 
-#: models.py:109
+#: models.py:125
 msgid "Client key provided by the LTI tool provider."
 msgstr ""
 
-#: models.py:115
+#: models.py:131
 msgid "Client secret provided by the LTI tool provider."
 msgstr ""
 
-#: models.py:121
+#: models.py:137
 msgid "Platform's generated Private key. Keep this value secret."
 msgstr ""
 
-#: models.py:127
+#: models.py:143
 msgid "Platform's generated Private key ID"
 msgstr ""
 
-#: models.py:132
+#: models.py:148
 msgid "Platform's generated JWK keyset."
 msgstr ""
 
-#: models.py:138
+#: models.py:154
 msgid "Client ID used by LTI tool"
 msgstr ""
 
-#: models.py:148
+#: models.py:250
 msgid "LTI Configuration stores on XBlock needs a block location set."
 msgstr ""
 
-#: models.py:155
-msgid "Invalid LTI configuration."
+#: models.py:256
+msgid ""
+"LTI Configuration stored on the model for LTI 1.3 must have a value for one "
+"of lti_1p3_tool_public_key or lti_1p3_tool_keyset_url."
+msgstr ""
+
+#: models.py:263
+msgid ""
+"CONFIG_ON_XBLOCK and CONFIG_EXTERNAL are not supported for LTI 1.3 "
+"Proctoring Services."
 msgstr ""
 
-#: models.py:165
-msgid "Block location not set, it's not possible to retrieve the block."
+#: models.py:271
+msgid "Invalid LTI configuration."
 msgstr ""
 
-#: plugin/views.py:246
+#: plugin/views.py:453
 msgid "The selected content type is not supported by Open edX."
 msgstr ""
 
-#: plugin/views.py:261
+#: plugin/views.py:468
 msgid "You don't have access to save LTI Content Items."
 msgstr ""
 
-#: plugin/views.py:262
+#: plugin/views.py:469
 msgid ""
 "Please check that you have course staff permissions and double check this "
 "block's LTI settings."
 msgstr ""
 
 #: templates/html/lti-dl/dl_response_error.html:6
 msgid "LTI Deep Linking failed."
@@ -468,23 +530,14 @@
 msgid "The LTI Deep Linking content was successfully saved in the LMS."
 msgstr ""
 
 #: templates/html/lti-dl/dl_response_saved.html:13
 msgid "You can safely close this page now."
 msgstr ""
 
-#: templates/html/lti_1p3_launch_error.html:10
-msgid "There was an error while launching the LTI 1.3 tool."
-msgstr ""
-
-#: templates/html/lti_1p3_launch_error.html:13
-msgid ""
-"If you're seeing this on a live course, please contact the course staff."
-msgstr ""
-
 #: templates/html/lti_1p3_permission_error.html:10
 msgid "Unauthorized."
 msgstr ""
 
 #: templates/html/lti_1p3_permission_error.html:13
 msgid ""
 "Students don't have permissions to perform LTI Deep Linking configuration "
@@ -545,27 +598,46 @@
 msgid "Deep Linking Launch - Configure tool"
 msgstr ""
 
 #: templates/html/lti_launch.html:27
 msgid "Press to Launch"
 msgstr ""
 
-#: static/js/xblock_lti_consumer.js:142
-msgid ""
-"Click OK to have your username and e-mail address sent to a 3rd party application.\n"
-"\n"
-"Click Cancel to return to this page without sending your information."
+#: templates/html/lti_launch_error.html:10
+msgid "There was an error while launching the LTI tool."
 msgstr ""
 
-#: static/js/xblock_lti_consumer.js:144
+#: templates/html/lti_launch_error.html:13
+#: templates/html/lti_proctoring_start_error.html:13
 msgid ""
-"Click OK to have your username sent to a 3rd party application.\n"
-"\n"
-"Click Cancel to return to this page without sending your information."
+"If you're seeing this on a live course, please contact the course staff."
+msgstr ""
+
+#: templates/html/lti_proctoring_start_error.html:10
+msgid "There was an error while starting your LTI proctored assessment."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:126
+msgid "Cancel"
 msgstr ""
 
-#: static/js/xblock_lti_consumer.js:146
+#: static/js/xblock_lti_consumer.js:128
+msgid "OK"
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:157
 msgid ""
-"Click OK to have your e-mail address sent to a 3rd party application.\n"
-"\n"
-"Click Cancel to return to this page without sending your information."
+"Click OK to have your username and e-mail address sent to a 3rd party "
+"application."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:159
+msgid "Click OK to have your username sent to a 3rd party application."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:161
+msgid "Click OK to have your e-mail address sent to a 3rd party application."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:168
+msgid "Click Cancel to return to this page without sending your information."
 msgstr ""
```

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.2/lti_consumer/translations/en/LC_MESSAGES/text.po`

 * *Files 19% similar despite different names*

```diff
@@ -1,461 +1,521 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# 
-# Translators:
-# Iris Zeng <yz3535@nyu.edu>, 2016
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
+#, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: XBlocks\n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-02-01 17:24-0300\n"
-"PO-Revision-Date: 2016-06-08 14:38+0000\n"
-"Last-Translator: Iris Zeng <yz3535@nyu.edu>, 2016\n"
-"Language-Team: Chinese (China) (http://app.transifex.com/open-edx/xblocks/language/zh_CN/)\n"
+"POT-Creation-Date: 2023-04-11 15:09-0400\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: zh_CN\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: lti_1p3/extensions/rest_framework/authentication.py:40
+#: lti_1p3/extensions/rest_framework/authentication.py:41
 msgid "Missing LTI 1.3 authentication token."
 msgstr ""
 
-#: lti_1p3/extensions/rest_framework/authentication.py:44
+#: lti_1p3/extensions/rest_framework/authentication.py:45
 msgid "Invalid token header. No credentials provided."
 msgstr ""
 
-#: lti_1p3/extensions/rest_framework/authentication.py:48
+#: lti_1p3/extensions/rest_framework/authentication.py:49
 msgid "Invalid token header. Token string should not contain spaces."
 msgstr ""
 
-#: lti_1p3/extensions/rest_framework/authentication.py:56
+#: lti_1p3/extensions/rest_framework/authentication.py:57
 msgid "LTI configuration not found."
 msgstr ""
 
-#: lti_1p3/extensions/rest_framework/authentication.py:65
+#: lti_1p3/extensions/rest_framework/authentication.py:66
 msgid "Invalid token signature."
 msgstr ""
 
-#: lti_xblock.py:127
+#: lti_xblock.py:126
 msgid "No valid user id found in endpoint URL"
 msgstr ""
 
-#: lti_xblock.py:233
+#: lti_xblock.py:139
+msgid "Configuration on block"
+msgstr ""
+
+#: lti_xblock.py:143
+msgid "Database Configuration"
+msgstr ""
+
+#: lti_xblock.py:146
+msgid "Reusable Configuration"
+msgstr ""
+
+#: lti_xblock.py:253
 msgid "Display Name"
 msgstr ""
 
-#: lti_xblock.py:235
+#: lti_xblock.py:255
 msgid ""
 "Enter the name that students see for this component. Analytics reports may "
 "also use the display name to identify this component."
 msgstr ""
 
-#: lti_xblock.py:239
+#: lti_xblock.py:259
 msgid "LTI Consumer"
 msgstr ""
 
-#: lti_xblock.py:242
+#: lti_xblock.py:262
 msgid "LTI Application Information"
 msgstr ""
 
-#: lti_xblock.py:244
+#: lti_xblock.py:264
 msgid ""
 "Enter a description of the third party application. If requesting username "
 "and/or email, use this text box to inform users why their username and/or "
 "email will be forwarded to a third party application."
 msgstr ""
 
-#: lti_xblock.py:254
+#: lti_xblock.py:272
+msgid "Configuration Type"
+msgstr ""
+
+#: lti_xblock.py:277
+msgid ""
+"Select 'Configuration on block' to configure a new LTI Tool. If the support "
+"staff provided you with a pre-configured LTI reusable Tool ID, "
+"select'Reusable Configuration' and enter it in the text field below."
+msgstr ""
+
+#: lti_xblock.py:284
 msgid "LTI Version"
 msgstr ""
 
-#: lti_xblock.py:262
+#: lti_xblock.py:292
 msgid ""
-"Select the LTI version that your tool supports.<br />The XBlock LTI Consumer"
-" fully supports LTI 1.1.1, LTI 1.3 and LTI Advantage features."
+"Select the LTI version that your tool supports.<br />The XBlock LTI Consumer "
+"fully supports LTI 1.1.1, LTI 1.3 and LTI Advantage features."
+msgstr ""
+
+#: lti_xblock.py:299
+msgid "LTI Reusable Configuration ID"
 msgstr ""
 
-#: lti_xblock.py:268
+#: lti_xblock.py:301
+msgid ""
+"Enter the reusable LTI external configuration ID provided by the support "
+"staff."
+msgstr ""
+
+#: lti_xblock.py:306
 msgid "Tool Launch URL"
 msgstr ""
 
-#: lti_xblock.py:272
+#: lti_xblock.py:310
 msgid ""
-"Enter the LTI 1.3 Tool Launch URL. <br />This is the URL the LMS will use to"
-" launch the LTI Tool."
+"Enter the LTI 1.3 Tool Launch URL. <br />This is the URL the LMS will use to "
+"launch the LTI Tool."
 msgstr ""
 
-#: lti_xblock.py:277
+#: lti_xblock.py:315
 msgid "Tool Initiate Login URL"
 msgstr ""
 
-#: lti_xblock.py:281
+#: lti_xblock.py:319
 msgid ""
 "Enter the LTI 1.3 Tool OIDC Authorization url (can also be called login or "
 "login initiation URL).<br />This is the URL the LMS will use to start a LTI "
 "authorization prior to doing the launch request."
 msgstr ""
 
-#: lti_xblock.py:288
+#: lti_xblock.py:325
+msgid "Registered Redirect URIs"
+msgstr ""
+
+#: lti_xblock.py:327
+msgid ""
+"Valid urls the Tool may request us to redirect the id token to. The redirect "
+"uris are often the same as the launch url/deep linking url so if this field "
+"is empty, it will use them as the default. If you need to use different "
+"redirect uri's, enter them here. If you use this field you must enter all "
+"valid redirect uri's the tool may request."
+msgstr ""
+
+#: lti_xblock.py:337
 msgid "Tool Public Key Mode"
 msgstr ""
 
-#: lti_xblock.py:296
+#: lti_xblock.py:345
 msgid "Select how the tool's public key information will be specified."
 msgstr ""
 
-#: lti_xblock.py:300
+#: lti_xblock.py:349
 msgid "Tool Keyset URL"
 msgstr ""
 
-#: lti_xblock.py:304
+#: lti_xblock.py:353
 msgid ""
 "Enter the LTI 1.3 Tool's JWK keysets URL.<br />This link should retrieve a "
 "JSON file containing public keys and signature algorithm information, so "
-"that the LMS can check if the messages and launch requests received have the"
-" signature from the tool.<br /><b>This is not required when doing LTI 1.3 "
+"that the LMS can check if the messages and launch requests received have the "
+"signature from the tool.<br /><b>This is not required when doing LTI 1.3 "
 "Launches without LTI Advantage nor Basic Outcomes requests.</b>"
 msgstr ""
 
-#: lti_xblock.py:314
+#: lti_xblock.py:363
 msgid "Tool Public Key"
 msgstr ""
 
-#: lti_xblock.py:319
+#: lti_xblock.py:368
 msgid ""
 "Enter the LTI 1.3 Tool's public key.<br />This is a string that starts with "
 "'-----BEGIN PUBLIC KEY-----' and is required so that the LMS can check if "
-"the messages and launch requests received have the signature from the "
-"tool.<br /><b>This is not required when doing LTI 1.3 Launches without LTI "
+"the messages and launch requests received have the signature from the tool."
+"<br /><b>This is not required when doing LTI 1.3 Launches without LTI "
 "Advantage nor Basic Outcomes requests.</b>"
 msgstr ""
 
-#: lti_xblock.py:329
+#: lti_xblock.py:378
 msgid "Enable LTI NRPS"
 msgstr ""
 
-#: lti_xblock.py:330
+#: lti_xblock.py:379
 msgid "Enable LTI Names and Role Provisioning Services."
 msgstr ""
 
-#: lti_xblock.py:337
+#: lti_xblock.py:386
 msgid "LTI 1.3 Block Client ID - DEPRECATED"
 msgstr ""
 
-#: lti_xblock.py:340
+#: lti_xblock.py:389
 msgid "DEPRECATED - This is now stored in the LtiConfiguration model."
 msgstr ""
 
-#: lti_xblock.py:343
+#: lti_xblock.py:392
 msgid "LTI 1.3 Block Key - DEPRECATED"
 msgstr ""
 
-#: lti_xblock.py:350
+#: lti_xblock.py:399
 msgid "Deep linking"
 msgstr ""
 
-#: lti_xblock.py:351
+#: lti_xblock.py:400
 msgid "Select True if you want to enable LTI Advantage Deep Linking."
 msgstr ""
 
-#: lti_xblock.py:356
+#: lti_xblock.py:405
 msgid "Deep Linking Launch URL"
 msgstr ""
 
-#: lti_xblock.py:360
+#: lti_xblock.py:409
 msgid ""
 "Enter the LTI Advantage Deep Linking Launch URL. If the tool does not "
 "specify one, use the same value as 'Tool Launch URL'."
 msgstr ""
 
-#: lti_xblock.py:365
+#: lti_xblock.py:414
 msgid "LTI Assignment and Grades Service"
 msgstr ""
 
-#: lti_xblock.py:367
+#: lti_xblock.py:416
 msgid "Disabled"
 msgstr ""
 
-#: lti_xblock.py:368
+#: lti_xblock.py:417
 msgid "Allow tools to submit grades only (declarative)"
 msgstr ""
 
-#: lti_xblock.py:369
+#: lti_xblock.py:418
 msgid "Allow tools to manage and submit grade (programmatic)"
 msgstr ""
 
-#: lti_xblock.py:374
+#: lti_xblock.py:423
 msgid ""
 "Enable the LTI-AGS service and select the functionality enabled for LTI "
 "tools. The 'declarative' mode (default) will provide a tool with a LineItem "
 "created from the XBlock settings, while the 'programmatic' one will allow "
 "tools to manage, create and link the grades."
 msgstr ""
 
-#: lti_xblock.py:382
+#: lti_xblock.py:431
 msgid "LTI ID"
 msgstr ""
 
-#: lti_xblock.py:384
+#: lti_xblock.py:433
 #, python-brace-format
 msgid ""
 "Enter the LTI ID for the external LTI provider. This value must be the same "
 "LTI ID that you entered in the LTI Passports setting on the Advanced "
 "Settings page.<br />See the {docs_anchor_open}edX LTI "
 "documentation{anchor_close} for more details on this setting."
 msgstr ""
 
-#: lti_xblock.py:396
+#: lti_xblock.py:445
 msgid "LTI URL"
 msgstr ""
 
-#: lti_xblock.py:398
+#: lti_xblock.py:447
 #, python-brace-format
 msgid ""
 "Enter the URL of the external tool that this component launches. This "
 "setting is only used when Hide External Tool is set to False.<br />See the "
 "{docs_anchor_open}edX LTI documentation{anchor_close} for more details on "
 "this setting."
 msgstr ""
 
-#: lti_xblock.py:411
+#: lti_xblock.py:460
 msgid "Custom Parameters"
 msgstr ""
 
-#: lti_xblock.py:413
+#: lti_xblock.py:462
 #, python-brace-format
 msgid ""
-"Add the key/value pair for any custom parameters, such as the page your "
-"e-book should open to or the background color for this component. Ex. "
+"Add the key/value pair for any custom parameters, such as the page your e-"
+"book should open to or the background color for this component. Ex. "
 "[\"page=1\", \"color=white\"]<br />See the {docs_anchor_open}edX LTI "
 "documentation{anchor_close} for more details on this setting."
 msgstr ""
 
-#: lti_xblock.py:423
+#: lti_xblock.py:472
 msgid "LTI Launch Target"
 msgstr ""
 
-#: lti_xblock.py:425
+#: lti_xblock.py:474
 msgid ""
 "Select Inline if you want the LTI content to open in an IFrame in the "
 "current page. Select Modal if you want the LTI content to open in a modal "
-"window in the current page. Select New Window if you want the LTI content to"
-" open in a new browser window. This setting is only used when Hide External "
+"window in the current page. Select New Window if you want the LTI content to "
+"open in a new browser window. This setting is only used when Hide External "
 "Tool is set to False."
 msgstr ""
 
-#: lti_xblock.py:439
+#: lti_xblock.py:488
 msgid "Button Text"
 msgstr ""
 
-#: lti_xblock.py:441
+#: lti_xblock.py:490
 msgid ""
 "Enter the text on the button used to launch the third party application. "
 "This setting is only used when Hide External Tool is set to False and LTI "
 "Launch Target is set to Modal or New Window."
 msgstr ""
 
-#: lti_xblock.py:449
+#: lti_xblock.py:498
 msgid "Inline Height"
 msgstr ""
 
-#: lti_xblock.py:451
+#: lti_xblock.py:500
 msgid ""
 "Enter the desired pixel height of the iframe which will contain the LTI "
 "tool. This setting is only used when Hide External Tool is set to False and "
 "LTI Launch Target is set to Inline."
 msgstr ""
 
-#: lti_xblock.py:459
+#: lti_xblock.py:508
 msgid "Modal Height"
 msgstr ""
 
-#: lti_xblock.py:461
+#: lti_xblock.py:510
 msgid ""
-"Enter the desired viewport percentage height of the modal overlay which will"
-" contain the LTI tool. This setting is only used when Hide External Tool is "
+"Enter the desired viewport percentage height of the modal overlay which will "
+"contain the LTI tool. This setting is only used when Hide External Tool is "
 "set to False and LTI Launch Target is set to Modal."
 msgstr ""
 
-#: lti_xblock.py:469
+#: lti_xblock.py:518
 msgid "Modal Width"
 msgstr ""
 
-#: lti_xblock.py:471
+#: lti_xblock.py:520
 msgid ""
 "Enter the desired viewport percentage width of the modal overlay which will "
 "contain the LTI tool. This setting is only used when Hide External Tool is "
 "set to False and LTI Launch Target is set to Modal."
 msgstr ""
 
-#: lti_xblock.py:479
+#: lti_xblock.py:528
 msgid "Scored"
 msgstr ""
 
-#: lti_xblock.py:480
+#: lti_xblock.py:529
 msgid ""
 "Select True if this component will receive a numerical score from the "
 "external LTI system."
 msgstr ""
 
-#: lti_xblock.py:487
+#: lti_xblock.py:536
 msgid ""
 "Enter the number of points possible for this component.  The default value "
 "is 1.0.  This setting is only used when Scored is set to True."
 msgstr ""
 
-#: lti_xblock.py:496
+#: lti_xblock.py:545
 msgid ""
 "The score kept in the xblock KVS -- duplicate of the published score in "
 "django DB"
 msgstr ""
 
-#: lti_xblock.py:501
+#: lti_xblock.py:550
 msgid "Comment as returned from grader, LTI2.0 spec"
 msgstr ""
 
-#: lti_xblock.py:506
+#: lti_xblock.py:555
 msgid "Hide External Tool"
 msgstr ""
 
-#: lti_xblock.py:508
+#: lti_xblock.py:557
 msgid ""
 "Select True if you want to use this component as a placeholder for syncing "
 "with an external grading  system rather than launch an external tool.  This "
 "setting hides the Launch button and any IFrames for this component."
 msgstr ""
 
-#: lti_xblock.py:516
+#: lti_xblock.py:565
 msgid "Accept grades past deadline"
 msgstr ""
 
-#: lti_xblock.py:517
+#: lti_xblock.py:566
 msgid ""
 "Select True to allow third party systems to post grades past the deadline."
 msgstr ""
 
-#: lti_xblock.py:525
+#: lti_xblock.py:574
 msgid "Request user's username"
 msgstr ""
 
-#. Translators: This is used to request the user's username for a third party
-#. service.
-#: lti_xblock.py:527
+#. Translators: This is used to request the user's username for a third party service.
+#: lti_xblock.py:576
 msgid "Select True to request the user's username."
 msgstr ""
 
-#: lti_xblock.py:532
+#: lti_xblock.py:581
 msgid "Request user's email"
 msgstr ""
 
-#. Translators: This is used to request the user's email for a third party
-#. service.
-#: lti_xblock.py:534
+#. Translators: This is used to request the user's email for a third party service.
+#: lti_xblock.py:583
 msgid "Select True to request the user's email address."
 msgstr ""
 
-#: lti_xblock.py:539
+#: lti_xblock.py:588
 msgid "Send extra parameters"
 msgstr ""
 
-#: lti_xblock.py:540
+#: lti_xblock.py:589
 msgid ""
 "Select True to send the extra parameters, which might contain Personally "
 "Identifiable Information. The processors are site-wide, please consult the "
 "site administrator if you have any questions."
 msgstr ""
 
-#: lti_xblock.py:603
+#: lti_xblock.py:652
 msgid "Custom Parameters must be a list"
 msgstr ""
 
-#: lti_xblock.py:713
+#: lti_xblock.py:783 lti_xblock.py:1062
+msgid "Could not get user data for current request"
+msgstr ""
+
+#: lti_xblock.py:810
 msgid ""
 "Could not parse LTI passport: {lti_passport!r}. Should be \"id:key:secret\" "
 "string."
 msgstr ""
 
-#: lti_xblock.py:729 lti_xblock.py:745
+#: lti_xblock.py:828 lti_xblock.py:842 lti_xblock.py:858
 msgid "Could not get user id for current request"
 msgstr ""
 
-#: lti_xblock.py:850
+#: lti_xblock.py:994
 msgid ""
 "Could not parse custom parameter: {custom_parameter!r}. Should be \"x=y\" "
 "string."
 msgstr ""
 
-#: lti_xblock.py:1310
+#: lti_xblock.py:1343
 msgid "[LTI]: Real user not found against anon_id: {}"
 msgstr ""
 
-#: models.py:72
+#: models.py:79
 msgid "Configuration Stored on XBlock fields"
 msgstr ""
 
-#: models.py:73
+#: models.py:80
 msgid "Configuration Stored on this model"
 msgstr ""
 
-#: models.py:97
+#: models.py:81
+msgid "Configuration Stored on external service"
+msgstr ""
+
+#: models.py:113
 msgid "LTI configuration data."
 msgstr ""
 
-#: models.py:104
+#: models.py:120
 msgid "The URL of the external tool that initiates the launch."
 msgstr ""
 
-#: models.py:109
+#: models.py:125
 msgid "Client key provided by the LTI tool provider."
 msgstr ""
 
-#: models.py:115
+#: models.py:131
 msgid "Client secret provided by the LTI tool provider."
 msgstr ""
 
-#: models.py:121
+#: models.py:137
 msgid "Platform's generated Private key. Keep this value secret."
 msgstr ""
 
-#: models.py:127
+#: models.py:143
 msgid "Platform's generated Private key ID"
 msgstr ""
 
-#: models.py:132
+#: models.py:148
 msgid "Platform's generated JWK keyset."
 msgstr ""
 
-#: models.py:138
+#: models.py:154
 msgid "Client ID used by LTI tool"
 msgstr ""
 
-#: models.py:148
+#: models.py:250
 msgid "LTI Configuration stores on XBlock needs a block location set."
 msgstr ""
 
-#: models.py:155
-msgid "Invalid LTI configuration."
+#: models.py:256
+msgid ""
+"LTI Configuration stored on the model for LTI 1.3 must have a value for one "
+"of lti_1p3_tool_public_key or lti_1p3_tool_keyset_url."
 msgstr ""
 
-#: models.py:165
-msgid "Block location not set, it's not possible to retrieve the block."
+#: models.py:263
+msgid ""
+"CONFIG_ON_XBLOCK and CONFIG_EXTERNAL are not supported for LTI 1.3 "
+"Proctoring Services."
 msgstr ""
 
-#: plugin/views.py:246
+#: models.py:271
+msgid "Invalid LTI configuration."
+msgstr ""
+
+#: plugin/views.py:453
 msgid "The selected content type is not supported by Open edX."
 msgstr ""
 
-#: plugin/views.py:261
+#: plugin/views.py:468
 msgid "You don't have access to save LTI Content Items."
 msgstr ""
 
-#: plugin/views.py:262
+#: plugin/views.py:469
 msgid ""
 "Please check that you have course staff permissions and double check this "
 "block's LTI settings."
 msgstr ""
 
 #: templates/html/lti-dl/dl_response_error.html:6
 msgid "LTI Deep Linking failed."
@@ -469,23 +529,14 @@
 msgid "The LTI Deep Linking content was successfully saved in the LMS."
 msgstr ""
 
 #: templates/html/lti-dl/dl_response_saved.html:13
 msgid "You can safely close this page now."
 msgstr ""
 
-#: templates/html/lti_1p3_launch_error.html:10
-msgid "There was an error while launching the LTI 1.3 tool."
-msgstr ""
-
-#: templates/html/lti_1p3_launch_error.html:13
-msgid ""
-"If you're seeing this on a live course, please contact the course staff."
-msgstr ""
-
 #: templates/html/lti_1p3_permission_error.html:10
 msgid "Unauthorized."
 msgstr ""
 
 #: templates/html/lti_1p3_permission_error.html:13
 msgid ""
 "Students don't have permissions to perform LTI Deep Linking configuration "
@@ -494,16 +545,16 @@
 
 #: templates/html/lti_1p3_studio.html:3
 msgid "LTI 1.3 Launches can only be performed from the LMS."
 msgstr ""
 
 #: templates/html/lti_1p3_studio.html:7
 msgid ""
-"To set up the LTI integration, you need to register the LMS in the tool with"
-" the information provided below."
+"To set up the LTI integration, you need to register the LMS in the tool with "
+"the information provided below."
 msgstr ""
 
 #: templates/html/lti_1p3_studio.html:11
 msgid "Client ID: "
 msgstr ""
 
 #: templates/html/lti_1p3_studio.html:16
@@ -546,27 +597,46 @@
 msgid "Deep Linking Launch - Configure tool"
 msgstr ""
 
 #: templates/html/lti_launch.html:27
 msgid "Press to Launch"
 msgstr ""
 
-#: static/js/xblock_lti_consumer.js:142
-msgid ""
-"Click OK to have your username and e-mail address sent to a 3rd party application.\n"
-"\n"
-"Click Cancel to return to this page without sending your information."
+#: templates/html/lti_launch_error.html:10
+msgid "There was an error while launching the LTI tool."
 msgstr ""
 
-#: static/js/xblock_lti_consumer.js:144
+#: templates/html/lti_launch_error.html:13
+#: templates/html/lti_proctoring_start_error.html:13
 msgid ""
-"Click OK to have your username sent to a 3rd party application.\n"
-"\n"
-"Click Cancel to return to this page without sending your information."
+"If you're seeing this on a live course, please contact the course staff."
+msgstr ""
+
+#: templates/html/lti_proctoring_start_error.html:10
+msgid "There was an error while starting your LTI proctored assessment."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:126
+msgid "Cancel"
 msgstr ""
 
-#: static/js/xblock_lti_consumer.js:146
+#: static/js/xblock_lti_consumer.js:128
+msgid "OK"
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:157
 msgid ""
-"Click OK to have your e-mail address sent to a 3rd party application.\n"
-"\n"
-"Click Cancel to return to this page without sending your information."
+"Click OK to have your username and e-mail address sent to a 3rd party "
+"application."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:159
+msgid "Click OK to have your username sent to a 3rd party application."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:161
+msgid "Click OK to have your e-mail address sent to a 3rd party application."
+msgstr ""
+
+#: static/js/xblock_lti_consumer.js:168
+msgid "Click Cancel to return to this page without sending your information."
 msgstr ""
```

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer/utils.py` & `lti-consumer-xblock-9.0.2/lti_consumer/utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer_xblock.egg-info/PKG-INFO` & `lti-consumer-xblock-9.0.2/lti_consumer_xblock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lti-consumer-xblock
-Version: 9.0.1
+Version: 9.0.2
 Summary: This XBlock implements the consumer side of the LTI specification.
 Home-page: https://github.com/openedx/xblock-lti-consumer
 Author: Open edX project
 Author-email: oscm@edx.org
 Keywords: lti consumer xblock
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
```

### Comparing `lti-consumer-xblock-9.0.1/lti_consumer_xblock.egg-info/SOURCES.txt` & `lti-consumer-xblock-9.0.2/lti_consumer_xblock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.1/setup.py` & `lti-consumer-xblock-9.0.2/setup.py`

 * *Files identical despite different names*

