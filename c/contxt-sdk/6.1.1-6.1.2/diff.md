# Comparing `tmp/contxt_sdk-6.1.1.tar.gz` & `tmp/contxt_sdk-6.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contxt_sdk-6.1.1.tar", max compression
+gzip compressed data, was "contxt_sdk-6.1.2.tar", max compression
```

## Comparing `contxt_sdk-6.1.1.tar` & `contxt_sdk-6.1.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0      738 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/LICENSE
--rw-r--r--   0        0        0      589 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/README.md
--rw-r--r--   0        0        0      193 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/contxt/__init__.py
--rw-r--r--   0        0        0       64 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/contxt/__main__.py
--rw-r--r--   0        0        0     2442 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/contxt/auth/__init__.py
--rw-r--r--   0        0        0    11776 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/contxt/auth/cli.py
--rw-r--r--   0        0        0     1790 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/contxt/auth/jwt.py
--rw-r--r--   0        0        0     1437 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/contxt/auth/machine.py
--rw-r--r--   0        0        0     1964 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/contxt/cli/clients.py
--rw-r--r--   0        0        0      611 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/contxt/cli/commands/auth.py
--rw-r--r--   0        0        0     3801 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/contxt/cli/commands/clusters.py
--rw-r--r--   0        0        0      740 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/contxt/cli/commands/edge_nodes.py
--rw-r--r--   0        0        0     5990 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/contxt/cli/commands/ems.py
--rw-r--r--   0        0        0     1348 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/contxt/cli/commands/facilities.py
--rw-r--r--   0        0        0    12886 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/contxt/cli/commands/iot.py
--rw-r--r--   0        0        0      832 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/contxt/cli/commands/metrics.py
--rw-r--r--   0        0        0      571 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/contxt/cli/commands/orgs.py
--rw-r--r--   0        0        0     3404 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/contxt/cli/commands/project_envs.py
--rw-r--r--   0        0        0     2422 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/contxt/cli/commands/projects.py
--rw-r--r--   0        0        0     2134 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/contxt/cli/commands/service_instances.py
--rw-r--r--   0        0        0     1770 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/contxt/cli/commands/services.py
--rw-r--r--   0        0        0     1333 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/contxt/cli/log.py
--rw-r--r--   0        0        0     1776 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/contxt/cli/main.py
--rw-r--r--   0        0        0     3200 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/contxt/cli/utils.py
--rw-r--r--   0        0        0     7066 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/contxt/models/__init__.py
--rw-r--r--   0        0        0     3918 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/contxt/models/bus.py
--rw-r--r--   0        0        0    11536 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/contxt/models/contxt.py
--rw-r--r--   0        0        0     8567 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/contxt/models/ems.py
--rw-r--r--   0        0        0     2751 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/contxt/models/etl.py
--rw-r--r--   0        0        0     4702 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/contxt/models/events.py
--rw-r--r--   0        0        0     2119 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/contxt/models/facilities.py
--rw-r--r--   0        0        0     7031 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/contxt/models/iot.py
--rw-r--r--   0        0        0     1461 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/contxt/models/sis.py
--rw-r--r--   0        0        0       63 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/contxt/py.typed
--rw-r--r--   0        0        0      361 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/contxt/services/__init__.py
--rw-r--r--   0        0        0     7563 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/contxt/services/api.py
--rw-r--r--   0        0        0     1614 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/contxt/services/auth.py
--rw-r--r--   0        0        0     2200 2023-04-11 14:35:22.825229 contxt_sdk-6.1.1/contxt/services/bus.py
--rw-r--r--   0        0        0     4662 2023-04-11 14:35:22.829228 contxt_sdk-6.1.1/contxt/services/contxt.py
--rw-r--r--   0        0        0     1435 2023-04-11 14:35:22.829228 contxt_sdk-6.1.1/contxt/services/contxt_deployments.py
--rw-r--r--   0        0        0     4711 2023-04-11 14:35:22.829228 contxt_sdk-6.1.1/contxt/services/ems.py
--rw-r--r--   0        0        0     4428 2023-04-11 14:35:22.829228 contxt_sdk-6.1.1/contxt/services/events.py
--rw-r--r--   0        0        0    17622 2023-04-11 14:35:22.829228 contxt_sdk-6.1.1/contxt/services/iot.py
--rw-r--r--   0        0        0     3968 2023-04-11 14:35:22.829228 contxt_sdk-6.1.1/contxt/services/ngest.py
--rw-r--r--   0        0        0     2190 2023-04-11 14:35:22.829228 contxt_sdk-6.1.1/contxt/services/nionic.py
--rw-r--r--   0        0        0     6318 2023-04-11 14:35:22.829228 contxt_sdk-6.1.1/contxt/services/pagination.py
--rw-r--r--   0        0        0     2151 2023-04-11 14:35:22.829228 contxt_sdk-6.1.1/contxt/utils/__init__.py
--rw-r--r--   0        0        0     4501 2023-04-11 14:35:22.829228 contxt_sdk-6.1.1/contxt/utils/object_mapper.py
--rw-r--r--   0        0        0      321 2023-04-11 14:35:22.829228 contxt_sdk-6.1.1/contxt/utils/orgs.py
--rw-r--r--   0        0        0     8000 2023-04-11 14:35:22.829228 contxt_sdk-6.1.1/contxt/utils/serializer.py
--rw-r--r--   0        0        0     1558 2023-04-11 14:35:22.829228 contxt_sdk-6.1.1/contxt/workers.py
--rw-r--r--   0        0        0     1535 2023-04-11 14:35:39.077350 contxt_sdk-6.1.1/pyproject.toml
--rw-r--r--   0        0        0     1573 1970-01-01 00:00:00.000000 contxt_sdk-6.1.1/PKG-INFO
+-rw-r--r--   0        0        0      738 2023-04-12 13:17:42.615770 contxt_sdk-6.1.2/LICENSE
+-rw-r--r--   0        0        0      589 2023-04-12 13:17:42.615770 contxt_sdk-6.1.2/README.md
+-rw-r--r--   0        0        0      193 2023-04-12 13:17:42.615770 contxt_sdk-6.1.2/contxt/__init__.py
+-rw-r--r--   0        0        0       64 2023-04-12 13:17:42.615770 contxt_sdk-6.1.2/contxt/__main__.py
+-rw-r--r--   0        0        0     2442 2023-04-12 13:17:42.615770 contxt_sdk-6.1.2/contxt/auth/__init__.py
+-rw-r--r--   0        0        0    11776 2023-04-12 13:17:42.615770 contxt_sdk-6.1.2/contxt/auth/cli.py
+-rw-r--r--   0        0        0     1790 2023-04-12 13:17:42.615770 contxt_sdk-6.1.2/contxt/auth/jwt.py
+-rw-r--r--   0        0        0     1437 2023-04-12 13:17:42.615770 contxt_sdk-6.1.2/contxt/auth/machine.py
+-rw-r--r--   0        0        0     1964 2023-04-12 13:17:42.615770 contxt_sdk-6.1.2/contxt/cli/clients.py
+-rw-r--r--   0        0        0      611 2023-04-12 13:17:42.615770 contxt_sdk-6.1.2/contxt/cli/commands/auth.py
+-rw-r--r--   0        0        0     3801 2023-04-12 13:17:42.615770 contxt_sdk-6.1.2/contxt/cli/commands/clusters.py
+-rw-r--r--   0        0        0      740 2023-04-12 13:17:42.615770 contxt_sdk-6.1.2/contxt/cli/commands/edge_nodes.py
+-rw-r--r--   0        0        0     5990 2023-04-12 13:17:42.615770 contxt_sdk-6.1.2/contxt/cli/commands/ems.py
+-rw-r--r--   0        0        0     1348 2023-04-12 13:17:42.615770 contxt_sdk-6.1.2/contxt/cli/commands/facilities.py
+-rw-r--r--   0        0        0    12886 2023-04-12 13:17:42.615770 contxt_sdk-6.1.2/contxt/cli/commands/iot.py
+-rw-r--r--   0        0        0      832 2023-04-12 13:17:42.615770 contxt_sdk-6.1.2/contxt/cli/commands/metrics.py
+-rw-r--r--   0        0        0      571 2023-04-12 13:17:42.615770 contxt_sdk-6.1.2/contxt/cli/commands/orgs.py
+-rw-r--r--   0        0        0     3404 2023-04-12 13:17:42.619773 contxt_sdk-6.1.2/contxt/cli/commands/project_envs.py
+-rw-r--r--   0        0        0     2422 2023-04-12 13:17:42.619773 contxt_sdk-6.1.2/contxt/cli/commands/projects.py
+-rw-r--r--   0        0        0     2134 2023-04-12 13:17:42.619773 contxt_sdk-6.1.2/contxt/cli/commands/service_instances.py
+-rw-r--r--   0        0        0     1770 2023-04-12 13:17:42.619773 contxt_sdk-6.1.2/contxt/cli/commands/services.py
+-rw-r--r--   0        0        0     1333 2023-04-12 13:17:42.619773 contxt_sdk-6.1.2/contxt/cli/log.py
+-rw-r--r--   0        0        0     1776 2023-04-12 13:17:42.619773 contxt_sdk-6.1.2/contxt/cli/main.py
+-rw-r--r--   0        0        0     3200 2023-04-12 13:17:42.619773 contxt_sdk-6.1.2/contxt/cli/utils.py
+-rw-r--r--   0        0        0     7066 2023-04-12 13:17:42.619773 contxt_sdk-6.1.2/contxt/models/__init__.py
+-rw-r--r--   0        0        0     3918 2023-04-12 13:17:42.619773 contxt_sdk-6.1.2/contxt/models/bus.py
+-rw-r--r--   0        0        0    11536 2023-04-12 13:17:42.619773 contxt_sdk-6.1.2/contxt/models/contxt.py
+-rw-r--r--   0        0        0     8567 2023-04-12 13:17:42.619773 contxt_sdk-6.1.2/contxt/models/ems.py
+-rw-r--r--   0        0        0     2751 2023-04-12 13:17:42.619773 contxt_sdk-6.1.2/contxt/models/etl.py
+-rw-r--r--   0        0        0     4702 2023-04-12 13:17:42.619773 contxt_sdk-6.1.2/contxt/models/events.py
+-rw-r--r--   0        0        0     2119 2023-04-12 13:17:42.619773 contxt_sdk-6.1.2/contxt/models/facilities.py
+-rw-r--r--   0        0        0     7031 2023-04-12 13:17:42.619773 contxt_sdk-6.1.2/contxt/models/iot.py
+-rw-r--r--   0        0        0     1461 2023-04-12 13:17:42.619773 contxt_sdk-6.1.2/contxt/models/sis.py
+-rw-r--r--   0        0        0       63 2023-04-12 13:17:42.619773 contxt_sdk-6.1.2/contxt/py.typed
+-rw-r--r--   0        0        0      361 2023-04-12 13:17:42.619773 contxt_sdk-6.1.2/contxt/services/__init__.py
+-rw-r--r--   0        0        0     7563 2023-04-12 13:17:42.619773 contxt_sdk-6.1.2/contxt/services/api.py
+-rw-r--r--   0        0        0     1614 2023-04-12 13:17:42.619773 contxt_sdk-6.1.2/contxt/services/auth.py
+-rw-r--r--   0        0        0     2200 2023-04-12 13:17:42.619773 contxt_sdk-6.1.2/contxt/services/bus.py
+-rw-r--r--   0        0        0     4662 2023-04-12 13:17:42.619773 contxt_sdk-6.1.2/contxt/services/contxt.py
+-rw-r--r--   0        0        0     1435 2023-04-12 13:17:42.619773 contxt_sdk-6.1.2/contxt/services/contxt_deployments.py
+-rw-r--r--   0        0        0     4711 2023-04-12 13:17:42.619773 contxt_sdk-6.1.2/contxt/services/ems.py
+-rw-r--r--   0        0        0     4428 2023-04-12 13:17:42.619773 contxt_sdk-6.1.2/contxt/services/events.py
+-rw-r--r--   0        0        0    17622 2023-04-12 13:17:42.619773 contxt_sdk-6.1.2/contxt/services/iot.py
+-rw-r--r--   0        0        0     3968 2023-04-12 13:17:42.619773 contxt_sdk-6.1.2/contxt/services/ngest.py
+-rw-r--r--   0        0        0     2190 2023-04-12 13:17:42.619773 contxt_sdk-6.1.2/contxt/services/nionic.py
+-rw-r--r--   0        0        0     6318 2023-04-12 13:17:42.619773 contxt_sdk-6.1.2/contxt/services/pagination.py
+-rw-r--r--   0        0        0     2151 2023-04-12 13:17:42.619773 contxt_sdk-6.1.2/contxt/utils/__init__.py
+-rw-r--r--   0        0        0     4501 2023-04-12 13:17:42.619773 contxt_sdk-6.1.2/contxt/utils/object_mapper.py
+-rw-r--r--   0        0        0      321 2023-04-12 13:17:42.619773 contxt_sdk-6.1.2/contxt/utils/orgs.py
+-rw-r--r--   0        0        0     8000 2023-04-12 13:17:42.619773 contxt_sdk-6.1.2/contxt/utils/serializer.py
+-rw-r--r--   0        0        0     1558 2023-04-12 13:17:42.619773 contxt_sdk-6.1.2/contxt/workers.py
+-rw-r--r--   0        0        0     1535 2023-04-12 13:17:59.544441 contxt_sdk-6.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1573 1970-01-01 00:00:00.000000 contxt_sdk-6.1.2/PKG-INFO
```

### Comparing `contxt_sdk-6.1.1/LICENSE` & `contxt_sdk-6.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/README.md` & `contxt_sdk-6.1.2/README.md`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/auth/__init__.py` & `contxt_sdk-6.1.2/contxt/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/auth/cli.py` & `contxt_sdk-6.1.2/contxt/auth/cli.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/auth/jwt.py` & `contxt_sdk-6.1.2/contxt/auth/jwt.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/auth/machine.py` & `contxt_sdk-6.1.2/contxt/auth/machine.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/cli/clients.py` & `contxt_sdk-6.1.2/contxt/cli/clients.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/cli/commands/auth.py` & `contxt_sdk-6.1.2/contxt/cli/commands/auth.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/cli/commands/clusters.py` & `contxt_sdk-6.1.2/contxt/cli/commands/clusters.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/cli/commands/edge_nodes.py` & `contxt_sdk-6.1.2/contxt/cli/commands/edge_nodes.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/cli/commands/ems.py` & `contxt_sdk-6.1.2/contxt/cli/commands/ems.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/cli/commands/facilities.py` & `contxt_sdk-6.1.2/contxt/cli/commands/facilities.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/cli/commands/iot.py` & `contxt_sdk-6.1.2/contxt/cli/commands/iot.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/cli/commands/metrics.py` & `contxt_sdk-6.1.2/contxt/cli/commands/metrics.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/cli/commands/orgs.py` & `contxt_sdk-6.1.2/contxt/cli/commands/orgs.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/cli/commands/project_envs.py` & `contxt_sdk-6.1.2/contxt/cli/commands/project_envs.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/cli/commands/projects.py` & `contxt_sdk-6.1.2/contxt/cli/commands/projects.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/cli/commands/service_instances.py` & `contxt_sdk-6.1.2/contxt/cli/commands/service_instances.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/cli/commands/services.py` & `contxt_sdk-6.1.2/contxt/cli/commands/services.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/cli/log.py` & `contxt_sdk-6.1.2/contxt/cli/log.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/cli/main.py` & `contxt_sdk-6.1.2/contxt/cli/main.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/cli/utils.py` & `contxt_sdk-6.1.2/contxt/cli/utils.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/models/__init__.py` & `contxt_sdk-6.1.2/contxt/models/__init__.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/models/bus.py` & `contxt_sdk-6.1.2/contxt/models/bus.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/models/contxt.py` & `contxt_sdk-6.1.2/contxt/models/contxt.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/models/ems.py` & `contxt_sdk-6.1.2/contxt/models/ems.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/models/etl.py` & `contxt_sdk-6.1.2/contxt/models/etl.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/models/events.py` & `contxt_sdk-6.1.2/contxt/models/events.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/models/facilities.py` & `contxt_sdk-6.1.2/contxt/models/facilities.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/models/iot.py` & `contxt_sdk-6.1.2/contxt/models/iot.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/models/sis.py` & `contxt_sdk-6.1.2/contxt/models/sis.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/services/api.py` & `contxt_sdk-6.1.2/contxt/services/api.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/services/auth.py` & `contxt_sdk-6.1.2/contxt/services/auth.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/services/bus.py` & `contxt_sdk-6.1.2/contxt/services/bus.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/services/contxt.py` & `contxt_sdk-6.1.2/contxt/services/contxt.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/services/contxt_deployments.py` & `contxt_sdk-6.1.2/contxt/services/contxt_deployments.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/services/ems.py` & `contxt_sdk-6.1.2/contxt/services/ems.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/services/events.py` & `contxt_sdk-6.1.2/contxt/services/events.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/services/iot.py` & `contxt_sdk-6.1.2/contxt/services/iot.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/services/ngest.py` & `contxt_sdk-6.1.2/contxt/services/ngest.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/services/nionic.py` & `contxt_sdk-6.1.2/contxt/services/nionic.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/services/pagination.py` & `contxt_sdk-6.1.2/contxt/services/pagination.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/utils/__init__.py` & `contxt_sdk-6.1.2/contxt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/utils/object_mapper.py` & `contxt_sdk-6.1.2/contxt/utils/object_mapper.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/utils/serializer.py` & `contxt_sdk-6.1.2/contxt/utils/serializer.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/contxt/workers.py` & `contxt_sdk-6.1.2/contxt/workers.py`

 * *Files identical despite different names*

### Comparing `contxt_sdk-6.1.1/pyproject.toml` & `contxt_sdk-6.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "contxt-sdk"
-version = "6.1.1"
+version = "6.1.2"
 description = "Contxt SDK from ndustrial"
 authors = ["ndustrial <dev@ndustrial.io>"]
 license = "ISC"
 readme = "README.md"
 repository = "https://github.com/ndustrialio/contxt-sdk-python"
 packages = [ { include = "contxt" } ]
```

### Comparing `contxt_sdk-6.1.1/PKG-INFO` & `contxt_sdk-6.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contxt-sdk
-Version: 6.1.1
+Version: 6.1.2
 Summary: Contxt SDK from ndustrial
 Home-page: https://github.com/ndustrialio/contxt-sdk-python
 License: ISC
 Author: ndustrial
 Author-email: dev@ndustrial.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved
```

