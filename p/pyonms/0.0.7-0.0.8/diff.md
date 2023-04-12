# Comparing `tmp/pyonms-0.0.7c.tar.gz` & `tmp/pyonms-0.0.8.tar.gz`

## Comparing `pyonms-0.0.7c.tar` & `pyonms-0.0.8.tar`

### file list

```diff
@@ -1,86 +1,86 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyonms-0.0.7/CHANGES.PY
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyonms-0.0.7/MANIFEST.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 pyonms-0.0.7/antora-playbook-local.yml
--rw-r--r--   0        0        0    27085 2020-02-02 00:00:00.000000 pyonms-0.0.7/external-functionapp-openapi.yaml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pyonms-0.0.7/old.env
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pyonms-0.0.7/requirements.txt
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pyonms-0.0.7/.github/python-version.txt
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 pyonms-0.0.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 pyonms-0.0.7/.github/workflows/codeql.yml
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 pyonms-0.0.7/.github/workflows/publish.yml
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 pyonms-0.0.7/docs/antora.yml
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 pyonms-0.0.7/docs/modules/ROOT/nav.adoc
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 pyonms-0.0.7/docs/modules/ROOT/pages/index.adoc
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 pyonms-0.0.7/docs/modules/ROOT/pages/introduction.adoc
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 pyonms-0.0.7/docs/modules/ROOT/pages/endpoints/alarms.adoc
--rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 pyonms-0.0.7/docs/modules/ROOT/pages/endpoints/business_services.adoc
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pyonms-0.0.7/docs/modules/ROOT/pages/endpoints/events.adoc
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 pyonms-0.0.7/docs/modules/ROOT/pages/endpoints/foreign_sources.adoc
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 pyonms-0.0.7/docs/modules/ROOT/pages/endpoints/nodes.adoc
--rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 pyonms-0.0.7/docs/modules/ROOT/pages/endpoints/requisitions.adoc
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 pyonms-0.0.7/docs/modules/ROOT/pages/portal/introduction.adoc
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 pyonms-0.0.7/docs/modules/ROOT/pages/using/connecting.adoc
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 pyonms-0.0.7/docs/modules/ROOT/pages/using/introduction.adoc
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 pyonms-0.0.7/docs/modules/ROOT/pages/using/support.adoc
--rw-r--r--   0        0        0     5179 2020-02-02 00:00:00.000000 pyonms-0.0.7/examples/example.py
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 pyonms-0.0.7/examples/portal.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyonms-0.0.7/pyonms/MANIFEST.in
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 pyonms-0.0.7/pyonms/__init__.py
--rw-r--r--   0        0        0     5895 2020-02-02 00:00:00.000000 pyonms-0.0.7/pyonms/dao/__init__.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 pyonms-0.0.7/pyonms/dao/alarms.py
--rw-r--r--   0        0        0     5982 2020-02-02 00:00:00.000000 pyonms-0.0.7/pyonms/dao/business_services.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 pyonms-0.0.7/pyonms/dao/events.py
--rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 pyonms-0.0.7/pyonms/dao/foreign_sources.py
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 pyonms-0.0.7/pyonms/dao/health.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 pyonms-0.0.7/pyonms/dao/info.py
--rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 pyonms-0.0.7/pyonms/dao/nodes.py
--rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 pyonms-0.0.7/pyonms/dao/requisitions.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pyonms-0.0.7/pyonms/models/__init__.py
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 pyonms-0.0.7/pyonms/models/alarm.py
--rw-r--r--   0        0        0    25294 2020-02-02 00:00:00.000000 pyonms-0.0.7/pyonms/models/business_service.py
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 pyonms-0.0.7/pyonms/models/event.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 pyonms-0.0.7/pyonms/models/exceptions.py
--rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 pyonms-0.0.7/pyonms/models/foreign_source.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 pyonms-0.0.7/pyonms/models/health.py
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 pyonms-0.0.7/pyonms/models/info.py
--rw-r--r--   0        0        0    12156 2020-02-02 00:00:00.000000 pyonms-0.0.7/pyonms/models/node.py
--rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 pyonms-0.0.7/pyonms/models/requisition.py
--rw-r--r--   0        0        0     7425 2020-02-02 00:00:00.000000 pyonms-0.0.7/pyonms/portal/__init__.py
--rw-r--r--   0        0        0     7674 2020-02-02 00:00:00.000000 pyonms-0.0.7/pyonms/portal/models.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 pyonms-0.0.7/pyonms/utils/__init__.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pyonms-0.0.7/test-mock/docker-compose.yaml
--rw-r--r--   0        0        0    26775 2020-02-02 00:00:00.000000 pyonms-0.0.7/test-mock/mocks/node_all.json
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pyonms-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 pyonms-0.0.7/tests/conftest.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 pyonms-0.0.7/tests/test_alarms.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 pyonms-0.0.7/tests/test_events.py
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 pyonms-0.0.7/tests/test_nodes.py
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 pyonms-0.0.7/tests/test_requisitions.py
--rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 pyonms-0.0.7/tests/cassettes/test_alarm_all.yaml
--rw-r--r--   0        0        0     7448 2020-02-02 00:00:00.000000 pyonms-0.0.7/tests/cassettes/test_alarm_batch.yaml
--rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 pyonms-0.0.7/tests/cassettes/test_alarm_one.yaml
--rw-r--r--   0        0        0    88993 2020-02-02 00:00:00.000000 pyonms-0.0.7/tests/cassettes/test_event_all.yaml
--rw-r--r--   0        0        0    11120 2020-02-02 00:00:00.000000 pyonms-0.0.7/tests/cassettes/test_event_batch.yaml
--rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 pyonms-0.0.7/tests/cassettes/test_event_one.yaml
--rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 pyonms-0.0.7/tests/cassettes/test_node_all.yaml
--rw-r--r--   0        0        0    11101 2020-02-02 00:00:00.000000 pyonms-0.0.7/tests/cassettes/test_node_batch.yaml
--rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 pyonms-0.0.7/tests/cassettes/test_node_ip.yaml
--rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 pyonms-0.0.7/tests/cassettes/test_node_ip_services.yaml
--rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 pyonms-0.0.7/tests/cassettes/test_node_metadata.yaml
--rw-r--r--   0        0        0    19618 2020-02-02 00:00:00.000000 pyonms-0.0.7/tests/cassettes/test_node_one.yaml
--rw-r--r--   0        0        0     7701 2020-02-02 00:00:00.000000 pyonms-0.0.7/tests/cassettes/test_node_snmp.yaml
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 pyonms-0.0.7/tests/cassettes/test_requisition_add_asset.yaml
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 pyonms-0.0.7/tests/cassettes/test_requisition_add_metadata.yaml
--rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 pyonms-0.0.7/tests/cassettes/test_requisition_all.yaml
--rw-r--r--   0        0        0     7150 2020-02-02 00:00:00.000000 pyonms-0.0.7/tests/cassettes/test_requisition_batch.yaml
--rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 pyonms-0.0.7/tests/cassettes/test_requisition_count_active.yaml
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 pyonms-0.0.7/tests/cassettes/test_requisition_count_deployed.yaml
--rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 pyonms-0.0.7/tests/cassettes/test_requisition_import.yaml
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 pyonms-0.0.7/tests/cassettes/test_requisition_one.yaml
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 pyonms-0.0.7/tests/cassettes/test_requisition_update_asset.yaml
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 pyonms-0.0.7/tests/cassettes/test_requisition_update_metadata.yaml
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 pyonms-0.0.7/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pyonms-0.0.7/LICENSE.txt
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 pyonms-0.0.7/README.md
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 pyonms-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 pyonms-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyonms-0.0.8/CHANGES.PY
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyonms-0.0.8/MANIFEST.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 pyonms-0.0.8/antora-playbook-local.yml
+-rw-r--r--   0        0        0    27085 2020-02-02 00:00:00.000000 pyonms-0.0.8/external-functionapp-openapi.yaml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pyonms-0.0.8/old.env
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pyonms-0.0.8/requirements.txt
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pyonms-0.0.8/.github/python-version.txt
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 pyonms-0.0.8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 pyonms-0.0.8/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 pyonms-0.0.8/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 pyonms-0.0.8/docs/antora.yml
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 pyonms-0.0.8/docs/modules/ROOT/nav.adoc
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 pyonms-0.0.8/docs/modules/ROOT/pages/index.adoc
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 pyonms-0.0.8/docs/modules/ROOT/pages/introduction.adoc
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 pyonms-0.0.8/docs/modules/ROOT/pages/endpoints/alarms.adoc
+-rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 pyonms-0.0.8/docs/modules/ROOT/pages/endpoints/business_services.adoc
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pyonms-0.0.8/docs/modules/ROOT/pages/endpoints/events.adoc
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 pyonms-0.0.8/docs/modules/ROOT/pages/endpoints/foreign_sources.adoc
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 pyonms-0.0.8/docs/modules/ROOT/pages/endpoints/nodes.adoc
+-rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 pyonms-0.0.8/docs/modules/ROOT/pages/endpoints/requisitions.adoc
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 pyonms-0.0.8/docs/modules/ROOT/pages/portal/introduction.adoc
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 pyonms-0.0.8/docs/modules/ROOT/pages/using/connecting.adoc
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 pyonms-0.0.8/docs/modules/ROOT/pages/using/introduction.adoc
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 pyonms-0.0.8/docs/modules/ROOT/pages/using/support.adoc
+-rw-r--r--   0        0        0     5179 2020-02-02 00:00:00.000000 pyonms-0.0.8/examples/example.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 pyonms-0.0.8/examples/portal.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/MANIFEST.in
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/__init__.py
+-rw-r--r--   0        0        0     5895 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/dao/__init__.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/dao/alarms.py
+-rw-r--r--   0        0        0     5982 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/dao/business_services.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/dao/events.py
+-rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/dao/foreign_sources.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/dao/health.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/dao/info.py
+-rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/dao/nodes.py
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/dao/requisitions.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/models/__init__.py
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/models/alarm.py
+-rw-r--r--   0        0        0    25294 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/models/business_service.py
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/models/event.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/models/exceptions.py
+-rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/models/foreign_source.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/models/health.py
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/models/info.py
+-rw-r--r--   0        0        0    12156 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/models/node.py
+-rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/models/requisition.py
+-rw-r--r--   0        0        0     7425 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/portal/__init__.py
+-rw-r--r--   0        0        0     7674 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/portal/models.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyonms/utils/__init__.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pyonms-0.0.8/test-mock/docker-compose.yaml
+-rw-r--r--   0        0        0    26775 2020-02-02 00:00:00.000000 pyonms-0.0.8/test-mock/mocks/node_all.json
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/conftest.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/test_alarms.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/test_events.py
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/test_nodes.py
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/test_requisitions.py
+-rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_alarm_all.yaml
+-rw-r--r--   0        0        0     7448 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_alarm_batch.yaml
+-rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_alarm_one.yaml
+-rw-r--r--   0        0        0    88993 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_event_all.yaml
+-rw-r--r--   0        0        0    11120 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_event_batch.yaml
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_event_one.yaml
+-rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_node_all.yaml
+-rw-r--r--   0        0        0    11101 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_node_batch.yaml
+-rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_node_ip.yaml
+-rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_node_ip_services.yaml
+-rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_node_metadata.yaml
+-rw-r--r--   0        0        0    19618 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_node_one.yaml
+-rw-r--r--   0        0        0     7701 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_node_snmp.yaml
+-rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_requisition_add_asset.yaml
+-rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_requisition_add_metadata.yaml
+-rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_requisition_all.yaml
+-rw-r--r--   0        0        0     7150 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_requisition_batch.yaml
+-rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_requisition_count_active.yaml
+-rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_requisition_count_deployed.yaml
+-rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_requisition_import.yaml
+-rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_requisition_one.yaml
+-rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_requisition_update_asset.yaml
+-rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 pyonms-0.0.8/tests/cassettes/test_requisition_update_metadata.yaml
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 pyonms-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pyonms-0.0.8/LICENSE.txt
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 pyonms-0.0.8/README.md
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 pyonms-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 pyonms-0.0.8/PKG-INFO
```

### Comparing `pyonms-0.0.7/antora-playbook-local.yml` & `pyonms-0.0.8/antora-playbook-local.yml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/external-functionapp-openapi.yaml` & `pyonms-0.0.8/external-functionapp-openapi.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/.github/ISSUE_TEMPLATE/bug_report.md` & `pyonms-0.0.8/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/.github/workflows/codeql.yml` & `pyonms-0.0.8/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/.github/workflows/publish.yml` & `pyonms-0.0.8/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/docs/modules/ROOT/pages/endpoints/alarms.adoc` & `pyonms-0.0.8/docs/modules/ROOT/pages/endpoints/alarms.adoc`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/docs/modules/ROOT/pages/endpoints/business_services.adoc` & `pyonms-0.0.8/docs/modules/ROOT/pages/endpoints/business_services.adoc`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/docs/modules/ROOT/pages/endpoints/events.adoc` & `pyonms-0.0.8/docs/modules/ROOT/pages/endpoints/events.adoc`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/docs/modules/ROOT/pages/endpoints/foreign_sources.adoc` & `pyonms-0.0.8/docs/modules/ROOT/pages/endpoints/foreign_sources.adoc`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/docs/modules/ROOT/pages/endpoints/nodes.adoc` & `pyonms-0.0.8/docs/modules/ROOT/pages/endpoints/nodes.adoc`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/docs/modules/ROOT/pages/endpoints/requisitions.adoc` & `pyonms-0.0.8/docs/modules/ROOT/pages/endpoints/requisitions.adoc`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/docs/modules/ROOT/pages/portal/introduction.adoc` & `pyonms-0.0.8/docs/modules/ROOT/pages/portal/introduction.adoc`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/docs/modules/ROOT/pages/using/connecting.adoc` & `pyonms-0.0.8/docs/modules/ROOT/pages/using/connecting.adoc`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/docs/modules/ROOT/pages/using/introduction.adoc` & `pyonms-0.0.8/docs/modules/ROOT/pages/using/introduction.adoc`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/examples/example.py` & `pyonms-0.0.8/examples/example.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/examples/portal.py` & `pyonms-0.0.8/examples/portal.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/pyonms/__init__.py` & `pyonms-0.0.8/pyonms/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # __init__.py
 
 """
 .. include:: ../README.md
 """
 
-__version__ = "0.0.7"
+__version__ = "0.0.8"
 
 from multiprocessing import current_process
 from urllib.parse import urlsplit
 
 import pyonms.dao.alarms
 import pyonms.dao.business_services
 import pyonms.dao.events
```

### Comparing `pyonms-0.0.7/pyonms/dao/__init__.py` & `pyonms-0.0.8/pyonms/dao/__init__.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/pyonms/dao/alarms.py` & `pyonms-0.0.8/pyonms/dao/alarms.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/pyonms/dao/business_services.py` & `pyonms-0.0.8/pyonms/dao/business_services.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/pyonms/dao/events.py` & `pyonms-0.0.8/pyonms/dao/events.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/pyonms/dao/foreign_sources.py` & `pyonms-0.0.8/pyonms/dao/foreign_sources.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/pyonms/dao/health.py` & `pyonms-0.0.8/pyonms/dao/health.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/pyonms/dao/info.py` & `pyonms-0.0.8/pyonms/dao/info.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/pyonms/dao/nodes.py` & `pyonms-0.0.8/pyonms/dao/nodes.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/pyonms/dao/requisitions.py` & `pyonms-0.0.8/pyonms/dao/requisitions.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/pyonms/models/alarm.py` & `pyonms-0.0.8/pyonms/models/alarm.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/pyonms/models/business_service.py` & `pyonms-0.0.8/pyonms/models/business_service.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/pyonms/models/event.py` & `pyonms-0.0.8/pyonms/models/event.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/pyonms/models/exceptions.py` & `pyonms-0.0.8/pyonms/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/pyonms/models/foreign_source.py` & `pyonms-0.0.8/pyonms/models/foreign_source.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/pyonms/models/health.py` & `pyonms-0.0.8/pyonms/models/health.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/pyonms/models/info.py` & `pyonms-0.0.8/pyonms/models/info.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/pyonms/models/node.py` & `pyonms-0.0.8/pyonms/models/node.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/pyonms/models/requisition.py` & `pyonms-0.0.8/pyonms/models/requisition.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/pyonms/portal/__init__.py` & `pyonms-0.0.8/pyonms/portal/__init__.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/pyonms/portal/models.py` & `pyonms-0.0.8/pyonms/portal/models.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/pyonms/utils/__init__.py` & `pyonms-0.0.8/pyonms/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/test-mock/mocks/node_all.json` & `pyonms-0.0.8/test-mock/mocks/node_all.json`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/tests/test_alarms.py` & `pyonms-0.0.8/tests/test_alarms.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/tests/test_events.py` & `pyonms-0.0.8/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/tests/test_nodes.py` & `pyonms-0.0.8/tests/test_nodes.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/tests/test_requisitions.py` & `pyonms-0.0.8/tests/test_requisitions.py`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/tests/cassettes/test_alarm_all.yaml` & `pyonms-0.0.8/tests/cassettes/test_alarm_all.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/tests/cassettes/test_alarm_batch.yaml` & `pyonms-0.0.8/tests/cassettes/test_alarm_batch.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/tests/cassettes/test_alarm_one.yaml` & `pyonms-0.0.8/tests/cassettes/test_alarm_one.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/tests/cassettes/test_event_all.yaml` & `pyonms-0.0.8/tests/cassettes/test_event_all.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/tests/cassettes/test_event_batch.yaml` & `pyonms-0.0.8/tests/cassettes/test_event_batch.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/tests/cassettes/test_event_one.yaml` & `pyonms-0.0.8/tests/cassettes/test_event_one.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/tests/cassettes/test_node_all.yaml` & `pyonms-0.0.8/tests/cassettes/test_node_all.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/tests/cassettes/test_node_batch.yaml` & `pyonms-0.0.8/tests/cassettes/test_node_batch.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/tests/cassettes/test_node_ip.yaml` & `pyonms-0.0.8/tests/cassettes/test_node_ip.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/tests/cassettes/test_node_ip_services.yaml` & `pyonms-0.0.8/tests/cassettes/test_node_ip_services.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/tests/cassettes/test_node_metadata.yaml` & `pyonms-0.0.8/tests/cassettes/test_node_metadata.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/tests/cassettes/test_node_one.yaml` & `pyonms-0.0.8/tests/cassettes/test_node_one.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/tests/cassettes/test_node_snmp.yaml` & `pyonms-0.0.8/tests/cassettes/test_node_snmp.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/tests/cassettes/test_requisition_add_asset.yaml` & `pyonms-0.0.8/tests/cassettes/test_requisition_add_asset.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/tests/cassettes/test_requisition_add_metadata.yaml` & `pyonms-0.0.8/tests/cassettes/test_requisition_add_metadata.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/tests/cassettes/test_requisition_all.yaml` & `pyonms-0.0.8/tests/cassettes/test_requisition_all.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/tests/cassettes/test_requisition_batch.yaml` & `pyonms-0.0.8/tests/cassettes/test_requisition_batch.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/tests/cassettes/test_requisition_count_active.yaml` & `pyonms-0.0.8/tests/cassettes/test_requisition_count_active.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/tests/cassettes/test_requisition_count_deployed.yaml` & `pyonms-0.0.8/tests/cassettes/test_requisition_count_deployed.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/tests/cassettes/test_requisition_import.yaml` & `pyonms-0.0.8/tests/cassettes/test_requisition_import.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/tests/cassettes/test_requisition_one.yaml` & `pyonms-0.0.8/tests/cassettes/test_requisition_one.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/tests/cassettes/test_requisition_update_asset.yaml` & `pyonms-0.0.8/tests/cassettes/test_requisition_update_asset.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/tests/cassettes/test_requisition_update_metadata.yaml` & `pyonms-0.0.8/tests/cassettes/test_requisition_update_metadata.yaml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/.gitignore` & `pyonms-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/LICENSE.txt` & `pyonms-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/README.md` & `pyonms-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/pyproject.toml` & `pyonms-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyonms-0.0.7/PKG-INFO` & `pyonms-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyonms
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Python library for accessing the OpenNMS REST API.
 Project-URL: Homepage, https://github.com/mmahacek/PyONMS
 Project-URL: Documentation, https://mmahacek.github.io/PyONMS/
 Author-email: Mark Mahacek <mmahacek@opennms.com>
 License-File: LICENSE.txt
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

