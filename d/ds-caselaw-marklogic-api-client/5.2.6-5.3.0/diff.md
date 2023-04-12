# Comparing `tmp/ds-caselaw-marklogic-api-client-5.2.6.tar.gz` & `tmp/ds_caselaw_marklogic_api_client-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ds-caselaw-marklogic-api-client-5.2.6.tar", last modified: Thu Apr  6 10:07:09 2023, max compression
+gzip compressed data, was "ds_caselaw_marklogic_api_client-5.3.0.tar", max compression
```

## Comparing `ds-caselaw-marklogic-api-client-5.2.6.tar` & `ds_caselaw_marklogic_api_client-5.3.0.tar`

### file list

```diff
@@ -1,52 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:07:09.894854 ds-caselaw-marklogic-api-client-5.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-04-06 10:07:09.894854 ds-caselaw-marklogic-api-client-5.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-06 10:07:09.894854 ds-caselaw-marklogic-api-client-5.2.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:07:09.886854 ds-caselaw-marklogic-api-client-5.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:07:09.890854 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/
--rw-r--r--   0 runner    (1001) docker     (123)    25434 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/Client.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/content_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xml_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:07:09.890854 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/break_judgment_checkout.xqy
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/checkin_judgment.xqy
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/checkout_judgment.xqy
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/copy_judgment.xqy
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/delete_judgment.xqy
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/get_judgment.xqy
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/get_judgment_checkout_status.xqy
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/get_judgment_version.xqy
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/get_last_modified.xqy
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/get_metadata_citation.xqy
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/get_metadata_court.xqy
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/get_metadata_name.xqy
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/get_metadata_work_date.xqy
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/get_properties_for_search_results.xqy
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/get_property.xqy
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/insert_judgment.xqy
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/list_judgment_versions.xqy
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/set_boolean_property.xqy
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/set_metadata_citation.xqy
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/set_metadata_court.xqy
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/set_metadata_name.xqy
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/set_metadata_this_uri.xqy
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/set_metadata_work_expression_date.xqy
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/set_property.xqy
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/update_judgment.xqy
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/update_locked_judgment.xqy
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/user_has_privilege.xqy
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/user_has_role.xqy
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/validate_all_documents.xqy
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/xslt.xqy
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-06 10:06:57.000000 ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/xslt_transform.xqy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:07:09.894854 ds-caselaw-marklogic-api-client-5.2.6/src/ds_caselaw_marklogic_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-04-06 10:07:09.000000 ds-caselaw-marklogic-api-client-5.2.6/src/ds_caselaw_marklogic_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-06 10:07:09.000000 ds-caselaw-marklogic-api-client-5.2.6/src/ds_caselaw_marklogic_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 10:07:09.000000 ds-caselaw-marklogic-api-client-5.2.6/src/ds_caselaw_marklogic_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 10:07:09.000000 ds-caselaw-marklogic-api-client-5.2.6/src/ds_caselaw_marklogic_api_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-06 10:07:09.000000 ds-caselaw-marklogic-api-client-5.2.6/src/ds_caselaw_marklogic_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-06 10:07:09.000000 ds-caselaw-marklogic-api-client-5.2.6/src/ds_caselaw_marklogic_api_client.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1108 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/LICENSE.md
+-rw-r--r--   0        0        0     3139 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/README.md
+-rw-r--r--   0        0        0      843 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/pyproject.toml
+-rw-r--r--   0        0        0    25434 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/Client.py
+-rw-r--r--   0        0        0        0 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/__init__.py
+-rw-r--r--   0        0        0     1954 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/content_hash.py
+-rw-r--r--   0        0        0     2318 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/errors.py
+-rw-r--r--   0        0        0        0 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/models/__init__.py
+-rw-r--r--   0        0        0     5272 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/models/judgments.py
+-rw-r--r--   0        0        0     1128 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/models/utilities/__init__.py
+-rw-r--r--   0        0        0     3453 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/models/utilities/aws.py
+-rw-r--r--   0        0        0        0 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/py.typed
+-rw-r--r--   0        0        0     3580 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xml_tools.py
+-rw-r--r--   0        0        0      220 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/break_judgment_checkout.xqy
+-rw-r--r--   0        0        0      197 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/checkin_judgment.xqy
+-rw-r--r--   0        0        0      385 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/checkout_judgment.xqy
+-rw-r--r--   0        0        0      318 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/copy_judgment.xqy
+-rw-r--r--   0        0        0      302 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/delete_judgment.xqy
+-rw-r--r--   0        0        0      715 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/get_judgment.xqy
+-rw-r--r--   0        0        0      193 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/get_judgment_checkout_status.xqy
+-rw-r--r--   0        0        0      292 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/get_judgment_version.xqy
+-rw-r--r--   0        0        0      172 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/get_last_modified.xqy
+-rw-r--r--   0        0        0      338 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/get_metadata_citation.xqy
+-rw-r--r--   0        0        0      339 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/get_metadata_court.xqy
+-rw-r--r--   0        0        0      221 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/get_metadata_name.xqy
+-rw-r--r--   0        0        0      358 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/get_metadata_work_date.xqy
+-rw-r--r--   0        0        0      594 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/get_properties_for_search_results.xqy
+-rw-r--r--   0        0        0      209 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/get_property.xqy
+-rw-r--r--   0        0        0      326 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/insert_judgment.xqy
+-rw-r--r--   0        0        0      190 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/list_judgment_versions.xqy
+-rw-r--r--   0        0        0      355 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/set_boolean_property.xqy
+-rw-r--r--   0        0        0      659 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/set_metadata_citation.xqy
+-rw-r--r--   0        0        0     1013 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/set_metadata_court.xqy
+-rw-r--r--   0        0        0      756 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/set_metadata_name.xqy
+-rw-r--r--   0        0        0     1762 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/set_metadata_this_uri.xqy
+-rw-r--r--   0        0        0      939 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/set_metadata_work_expression_date.xqy
+-rw-r--r--   0        0        0      343 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/set_property.xqy
+-rw-r--r--   0        0        0      420 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/update_judgment.xqy
+-rw-r--r--   0        0        0      556 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/update_locked_judgment.xqy
+-rw-r--r--   0        0        0      371 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/user_has_privilege.xqy
+-rw-r--r--   0        0        0      246 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/user_has_role.xqy
+-rw-r--r--   0        0        0      156 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/validate_all_documents.xqy
+-rw-r--r--   0        0        0      199 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/xslt.xqy
+-rw-r--r--   0        0        0     1381 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/xslt_transform.xqy
+-rw-r--r--   0        0        0     4128 1970-01-01 00:00:00.000000 ds_caselaw_marklogic_api_client-5.3.0/PKG-INFO
```

### Comparing `ds-caselaw-marklogic-api-client-5.2.6/LICENSE.md` & `ds_caselaw_marklogic_api_client-5.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ds-caselaw-marklogic-api-client-5.2.6/PKG-INFO` & `ds_caselaw_marklogic_api_client-5.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,31 @@
 Metadata-Version: 2.1
 Name: ds-caselaw-marklogic-api-client
-Version: 5.2.6
-Summary: An API client for interacting with the Caselaw Marklogic instance
+Version: 5.3.0
+Summary: An API client for interacting with the underlying data in Find Caselaw.
 Home-page: https://github.com/nationalarchives/ds-caselaw-custom-api-client
+Keywords: national archives,caselaw
 Author: The National Archives
-Project-URL: Bug Tracker, https://github.com/nationalarchives/ds-caselaw-custom-api-client/issues
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: boto3 (>=1.26.107,<2.0.0)
+Requires-Dist: certifi (==2022.12.7)
+Requires-Dist: charset-normalizer (==2.1.1)
+Requires-Dist: django-environ (==0.10.0)
+Requires-Dist: ds-caselaw-utils (>=0.5.0,<0.6.0)
+Requires-Dist: idna (==3.4)
+Requires-Dist: lxml (==4.9.2)
+Requires-Dist: memoization (==0.4.0)
+Requires-Dist: requests (==2.28.2)
+Requires-Dist: requests-toolbelt (==0.10.1)
+Requires-Dist: urllib3 (==1.26.15)
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
 
 # The National Archives: Find Case Law
 
 This repository is part of the [Find Case Law](https://caselaw.nationalarchives.gov.uk/) project at [The National Archives](https://www.nationalarchives.gov.uk/). For more information on the project, check [the documentation](https://github.com/nationalarchives/ds-find-caselaw-docs).
 
 # MarkLogic API Client
 
@@ -118,7 +129,8 @@
 0. Commit and push
 0. Open a PR from that branch to main
 0. Get approval on the PR
 0. Merge the PR to main and push
 0. Tag the merge commit on `main` with `v{major}.{minor}.{patch}` and push the tag
 0. Create a release in [Github releases](https://github.com/nationalarchives/ds-caselaw-custom-api-client/releases)
 using the created tag
+
```

### Comparing `ds-caselaw-marklogic-api-client-5.2.6/README.md` & `ds_caselaw_marklogic_api_client-5.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/Client.py` & `ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/Client.py`

 * *Files identical despite different names*

### Comparing `ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/content_hash.py` & `ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/content_hash.py`

 * *Files identical despite different names*

### Comparing `ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/errors.py` & `ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/errors.py`

 * *Files identical despite different names*

### Comparing `ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xml_tools.py` & `ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xml_tools.py`

 * *Files identical despite different names*

### Comparing `ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/get_judgment.xqy` & `ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/get_judgment.xqy`

 * *Files identical despite different names*

### Comparing `ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/get_properties_for_search_results.xqy` & `ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/get_properties_for_search_results.xqy`

 * *Files identical despite different names*

### Comparing `ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/set_metadata_citation.xqy` & `ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/set_metadata_citation.xqy`

 * *Files identical despite different names*

### Comparing `ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/set_metadata_court.xqy` & `ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/set_metadata_court.xqy`

 * *Files identical despite different names*

### Comparing `ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/set_metadata_name.xqy` & `ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/set_metadata_name.xqy`

 * *Files identical despite different names*

### Comparing `ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/set_metadata_this_uri.xqy` & `ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/set_metadata_this_uri.xqy`

 * *Files identical despite different names*

### Comparing `ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/set_metadata_work_expression_date.xqy` & `ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/set_metadata_work_expression_date.xqy`

 * *Files identical despite different names*

### Comparing `ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/update_locked_judgment.xqy` & `ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/update_locked_judgment.xqy`

 * *Files identical despite different names*

### Comparing `ds-caselaw-marklogic-api-client-5.2.6/src/caselawclient/xquery/xslt_transform.xqy` & `ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/xslt_transform.xqy`

 * *Files identical despite different names*

