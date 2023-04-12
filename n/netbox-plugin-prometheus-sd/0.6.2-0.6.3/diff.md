# Comparing `tmp/netbox_plugin_prometheus_sd-0.6.2.tar.gz` & `tmp/netbox_plugin_prometheus_sd-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_plugin_prometheus_sd-0.6.2.tar", max compression
+gzip compressed data, was "netbox_plugin_prometheus_sd-0.6.3.tar", max compression
```

## Comparing `netbox_plugin_prometheus_sd-0.6.2.tar` & `netbox_plugin_prometheus_sd-0.6.3.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     1069 2023-02-27 11:52:39.515967 netbox_plugin_prometheus_sd-0.6.2/LICENSE
--rw-r--r--   0        0        0     3724 2023-02-27 11:52:39.515967 netbox_plugin_prometheus_sd-0.6.2/README.md
--rw-r--r--   0        0        0      488 2023-02-27 11:52:39.519967 netbox_plugin_prometheus_sd-0.6.2/netbox_prometheus_sd/__init__.py
--rw-r--r--   0        0        0        0 2023-02-27 11:52:39.519967 netbox_plugin_prometheus_sd-0.6.2/netbox_prometheus_sd/api/__init__.py
--rw-r--r--   0        0        0     3851 2023-02-27 11:52:39.519967 netbox_plugin_prometheus_sd-0.6.2/netbox_prometheus_sd/api/serializers.py
--rw-r--r--   0        0        0      321 2023-02-27 11:52:39.519967 netbox_plugin_prometheus_sd-0.6.2/netbox_prometheus_sd/api/urls.py
--rw-r--r--   0        0        0     3858 2023-02-27 11:52:39.519967 netbox_plugin_prometheus_sd-0.6.2/netbox_prometheus_sd/api/utils.py
--rw-r--r--   0        0        0     2545 2023-02-27 11:52:39.519967 netbox_plugin_prometheus_sd-0.6.2/netbox_prometheus_sd/api/views.py
--rw-r--r--   0        0        0       50 2023-02-27 11:52:39.519967 netbox_plugin_prometheus_sd-0.6.2/netbox_prometheus_sd/tests/__init__.py
--rw-r--r--   0        0        0     2764 2023-02-27 11:52:39.519967 netbox_plugin_prometheus_sd-0.6.2/netbox_prometheus_sd/tests/test_api.py
--rw-r--r--   0        0        0     8737 2023-02-27 11:52:39.519967 netbox_plugin_prometheus_sd-0.6.2/netbox_prometheus_sd/tests/test_serializers.py
--rw-r--r--   0        0        0     3672 2023-02-27 11:52:39.519967 netbox_plugin_prometheus_sd-0.6.2/netbox_prometheus_sd/tests/utils.py
--rw-r--r--   0        0        0      617 2023-02-27 11:52:55.912505 netbox_plugin_prometheus_sd-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     4488 1970-01-01 00:00:00.000000 netbox_plugin_prometheus_sd-0.6.2/setup.py
--rw-r--r--   0        0        0     4329 1970-01-01 00:00:00.000000 netbox_plugin_prometheus_sd-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-12 09:59:26.361881 netbox_plugin_prometheus_sd-0.6.3/LICENSE
+-rw-r--r--   0        0        0     3918 2023-04-12 09:59:26.361881 netbox_plugin_prometheus_sd-0.6.3/README.md
+-rw-r--r--   0        0        0      488 2023-04-12 09:59:26.365882 netbox_plugin_prometheus_sd-0.6.3/netbox_prometheus_sd/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 09:59:26.365882 netbox_plugin_prometheus_sd-0.6.3/netbox_prometheus_sd/api/__init__.py
+-rw-r--r--   0        0        0     3891 2023-04-12 09:59:26.365882 netbox_plugin_prometheus_sd-0.6.3/netbox_prometheus_sd/api/serializers.py
+-rw-r--r--   0        0        0      321 2023-04-12 09:59:26.365882 netbox_plugin_prometheus_sd-0.6.3/netbox_prometheus_sd/api/urls.py
+-rw-r--r--   0        0        0     4005 2023-04-12 09:59:26.365882 netbox_plugin_prometheus_sd-0.6.3/netbox_prometheus_sd/api/utils.py
+-rw-r--r--   0        0        0     2545 2023-04-12 09:59:26.365882 netbox_plugin_prometheus_sd-0.6.3/netbox_prometheus_sd/api/views.py
+-rw-r--r--   0        0        0       50 2023-04-12 09:59:26.365882 netbox_plugin_prometheus_sd-0.6.3/netbox_prometheus_sd/tests/__init__.py
+-rw-r--r--   0        0        0     2764 2023-04-12 09:59:26.365882 netbox_plugin_prometheus_sd-0.6.3/netbox_prometheus_sd/tests/test_api.py
+-rwxr-xr-x   0        0        0     8825 2023-04-12 09:59:26.365882 netbox_plugin_prometheus_sd-0.6.3/netbox_prometheus_sd/tests/test_serializers.py
+-rw-r--r--   0        0        0     3817 2023-04-12 09:59:26.365882 netbox_plugin_prometheus_sd-0.6.3/netbox_prometheus_sd/tests/utils.py
+-rw-r--r--   0        0        0      617 2023-04-12 09:59:41.394267 netbox_plugin_prometheus_sd-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     4523 1970-01-01 00:00:00.000000 netbox_plugin_prometheus_sd-0.6.3/PKG-INFO
```

### Comparing `netbox_plugin_prometheus_sd-0.6.2/LICENSE` & `netbox_plugin_prometheus_sd-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_plugin_prometheus_sd-0.6.2/README.md` & `netbox_plugin_prometheus_sd-0.6.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -47,15 +47,23 @@
 
 ### Example
 
 A working example on how to use this plugin with Prometheus is located at the `example` folder. Netbox content is created by using Netbox docker initializers.
 
 The demo data doesn't make sense, but they are good enough for demonstrating how to configure Prometheus and get demo data to Prometheus service discovery.
 
-Go to the `example` folder and run `docker-compose up`. Prometheus should get available on `http://localhost:9090`. Netbox content should then be available in the service discovery tab.
+Go to the `example` folder and run `docker-compose up`. Prometheus should get available on `http://localhost:9090`.
+
+Push some example devices and objects to Netbox using the initializers:
+
+```
+docker-compose exec  netbox /opt/netbox/netbox/manage.py load_initializer_data --path /opt/netbox/initializers
+```
+
+Netbox content should then be available in the service discovery tab.
 
 ## Development
 
 We use Poetry for dependency management and invoke as task runner.
 As Netbox plugins cannot be tested standalone, we need invoke to start all code embedded in Netbox Docker containers.
 
 All code to run in docker is located under `development`.
```

### Comparing `netbox_plugin_prometheus_sd-0.6.2/netbox_prometheus_sd/api/serializers.py` & `netbox_plugin_prometheus_sd-0.6.3/netbox_prometheus_sd/api/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         utils.extract_primary_ip(obj, labels)
         utils.extracts_platform(obj, labels)
         utils.extract_tags(obj, labels)
         utils.extract_tenant(obj, labels)
         utils.extract_cluster(obj, labels)
         utils.extract_services(obj, labels)
         utils.extract_contacts(obj, labels)
+        utils.extract_rack(obj, labels)
         utils.extract_custom_fields(obj, labels)
 
         if hasattr(obj, "device_role") and obj.device_role is not None:
             labels["role"] = obj.device_role.name
             labels["role_slug"] = obj.device_role.slug
 
         if hasattr(obj, "device_type") and obj.device_type is not None:
```

### Comparing `netbox_plugin_prometheus_sd-0.6.2/netbox_prometheus_sd/api/utils.py` & `netbox_plugin_prometheus_sd-0.6.3/netbox_prometheus_sd/api/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,19 @@
             if contact.contact.email:
                 labels[f"contact_{contact.priority}_email"] = contact.contact.email
             if contact.contact.comments:
                 labels[f"contact_{contact.priority}_comments"] = contact.contact.comments
             if hasattr(contact, "role") and contact.role is not None:
                 labels[f"contact_{contact.priority}_role"] = contact.role.name
 
+def extract_rack(obj, labels: LabelDict):
+    """Extract rack"""
+    if hasattr(obj, "rack") and obj.rack:
+        labels["rack"] = obj.rack.name
+
 def extract_custom_fields(obj, labels: LabelDict):
     if hasattr(obj, "custom_field_data") and obj.custom_field_data is not None:
         for key, value in obj.custom_field_data.items():
             # Render primitive value as string representation
             if not hasattr(value, '__dict__'):
                 labels["custom_field_" + key.lower()] = str(value)
             # Complex types are rendered as json
```

### Comparing `netbox_plugin_prometheus_sd-0.6.2/netbox_prometheus_sd/api/views.py` & `netbox_plugin_prometheus_sd-0.6.3/netbox_prometheus_sd/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_prometheus_sd-0.6.2/netbox_prometheus_sd/tests/test_api.py` & `netbox_plugin_prometheus_sd-0.6.3/netbox_prometheus_sd/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_prometheus_sd-0.6.2/netbox_prometheus_sd/tests/test_serializers.py` & `netbox_plugin_prometheus_sd-0.6.3/netbox_prometheus_sd/tests/test_serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,14 +147,15 @@
         )
         self.assertDictContainsSubset(
             {"__meta_netbox_primary_ip4": "192.168.0.1"}, data["labels"]
         )
         self.assertDictContainsSubset(
             {"__meta_netbox_primary_ip6": "2001:db8:1701::2"}, data["labels"]
         )
+        self.assertDictContainsSubset({"__meta_netbox_rack": "R01B01"}, data["labels"])
         self.assertDictContainsSubset(
             {"__meta_netbox_tenant": "Acme Corp."}, data["labels"]
         )
         self.assertDictContainsSubset(
             {"__meta_netbox_tenant_slug": "acme"}, data["labels"]
         )
         self.assertDictContainsSubset(
```

### Comparing `netbox_plugin_prometheus_sd-0.6.2/netbox_prometheus_sd/tests/utils.py` & `netbox_plugin_prometheus_sd-0.6.3/netbox_prometheus_sd/tests/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dcim.models.devices import DeviceType, Manufacturer
 from dcim.models.sites import Site
-from dcim.models import Device, DeviceRole, Platform
+from dcim.models import Device, DeviceRole, Platform, Rack
 
 from ipam.models import IPAddress
 from tenancy.models import Tenant, TenantGroup
 
 from virtualization.models import (
     Cluster,
     ClusterGroup,
@@ -95,14 +95,17 @@
     device.tenant = build_tenant()
     device.custom_field_data = build_custom_fields()
     device.platform = Platform.objects.get_or_create(name="Junos", slug="junos")[0]
     device.primary_ip4 = IPAddress.objects.get_or_create(address="192.168.0.1/24")[0]
     device.primary_ip6 = IPAddress.objects.get_or_create(address="2001:db8:1701::2/64")[
         0
     ]
+    device.rack = Rack.objects.get_or_create(
+        name="R01B01", site=Site.objects.get_or_create(name="Site", slug="site")[0]
+    )[0]
     device.tags.add("Tag1")
     device.tags.add("Tag 2")
     return device
 
 
 def build_minimal_ip(address):
     return IPAddress.objects.get_or_create(address=address)[0]
```

### Comparing `netbox_plugin_prometheus_sd-0.6.2/pyproject.toml` & `netbox_plugin_prometheus_sd-0.6.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "netbox-plugin-prometheus-sd"
-version = "0.6.2" # placeholder
+version = "0.6.3" # placeholder
 description = "A Netbox plugin to provide Netbox entires to Prometheus HTTP service discovery"
 authors = ["Felix Peters <felix.peters@breuninger.de>"]
 license = "MIT"
 readme = "README.md"
 
 packages = [
     { include = "netbox_prometheus_sd" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 [tool.poetry.dev-dependencies]
-black = "^23.1"
+black = "^23.3"
 invoke = "^2.0.0"
-pylint = "^2.15.5"
+pylint = "^2.17.2"
 pylint-django = "^2.5.3"
-yamllint = "^1.28.0"
+yamllint = "^1.30.0"
 typed-ast = "^1.5.4"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `netbox_plugin_prometheus_sd-0.6.2/setup.py` & `netbox_plugin_prometheus_sd-0.6.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,113 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: netbox-plugin-prometheus-sd
+Version: 0.6.3
+Summary: A Netbox plugin to provide Netbox entires to Prometheus HTTP service discovery
+License: MIT
+Author: Felix Peters
+Author-email: felix.peters@breuninger.de
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
 
-packages = \
-['netbox_prometheus_sd',
- 'netbox_prometheus_sd.api',
- 'netbox_prometheus_sd.tests']
-
-package_data = \
-{'': ['*']}
-
-setup_kwargs = {
-    'name': 'netbox-plugin-prometheus-sd',
-    'version': '0.6.2',
-    'description': 'A Netbox plugin to provide Netbox entires to Prometheus HTTP service discovery',
-    'long_description': "# netbox-plugin-prometheus-sd\n\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n[![CI](https://github.com/FlxPeters/netbox-plugin-prometheus-sd/workflows/CI/badge.svg?event=push)](https://github.com/FlxPeters/netbox-plugin-prometheus-sd/actions?query=workflow%3ACI)\n[![PyPI](https://img.shields.io/pypi/v/netbox-plugin-prometheus-sd)](https://pypi.org/project/netbox-plugin-prometheus-sd/)\n\nProvide Prometheus http_sd compatible API Endpoint with data from Netbox.\n\nHTTP SD is a new feature in Prometheus 2.28.0 that allows hosts to be found via a URL instead of just files.\nThis plugin implements API endpoints in Netbox to make devices, IPs and virtual machines available to Prometheus.\n\n## Compatibility\n\nWe aim to support the latest major versions of Netbox. For now we Support Netbox `2.11`, `3.0`, `3.1`, `3.2` and `3.3` including bugfix versions.\nAll relevant target versions are tested in CI. Have a look at the Github Actions definition for the current build targets.\n\n## Installation\n\nThe plugin is available as a Python package in pypi and can be installed with pip\n\n    pip install netbox-plugin-prometheus-sd\n\nEnable the plugin in /opt/netbox/netbox/netbox/configuration.py:\n\n    PLUGINS = ['netbox_prometheus_sd']\n\nThe plugin has not further plugin configuration at the moment.\n\n## Usage\n\nThe plugin only provides a new API endpoint on the Netbox API. There is no further action required after installation.\n\n### API\n\nThe plugin reuses Netbox API view sets with new serializers for Prometheus.\nThis means that all filters that can be used on the Netbox api can also be used to filter Prometheus targets.\nPaging is disabled because Prometheus does not support paged results.\n\nThe plugin also reuses the Netbox authentication and permission model.\nDepending on the Netbox configuration, a token with valid object permissions must be passed to Netbox.\n\n```\nGET        /api/plugins/prometheus-sd/devices/              Get a list of devices in a prometheus compatible format\nGET        /api/plugins/prometheus-sd/virtual-machines/     Get a list of vms in a prometheus compatible format\nGET        /api/plugins/prometheus-sd/ip-addresses/         Get a list of ip in a prometheus compatible format\n```\n\n### Example\n\nA working example on how to use this plugin with Prometheus is located at the `example` folder. Netbox content is created by using Netbox docker initializers.\n\nThe demo data doesn't make sense, but they are good enough for demonstrating how to configure Prometheus and get demo data to Prometheus service discovery.\n\nGo to the `example` folder and run `docker-compose up`. Prometheus should get available on `http://localhost:9090`. Netbox content should then be available in the service discovery tab.\n\n## Development\n\nWe use Poetry for dependency management and invoke as task runner.\nAs Netbox plugins cannot be tested standalone, we need invoke to start all code embedded in Netbox Docker containers.\n\nAll code to run in docker is located under `development`.\nTo start a virtual env managed by poetry run `poetry shell`.\nAll following commands are started inside this environment.\n\nIn order to run tests invoke the test steps\n\n``` bash\n# Execute all tests\ninvoke tests\n\n# Execute unit tests only\ninvoke unittest\n```\n\nFeatures should be covered by a unit test, but some times it's easier to develop on an running system.\n\n``` bash\n# Start a local Netbox with docker\ninvoke start\n\n# Create an user named `admin`\ninvoke create-user\n```\n\nVisit http://localhost:8000 and log in with the new user.\nYou can now define Netbox entities and test around.\n\nAPI endpoints for testing can be found at http://localhost:8000/api/plugins/prometheus-sd/\n",
-    'author': 'Felix Peters',
-    'author_email': 'felix.peters@breuninger.de',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.8,<4.0',
-}
+# netbox-plugin-prometheus-sd
 
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![CI](https://github.com/FlxPeters/netbox-plugin-prometheus-sd/workflows/CI/badge.svg?event=push)](https://github.com/FlxPeters/netbox-plugin-prometheus-sd/actions?query=workflow%3ACI)
+[![PyPI](https://img.shields.io/pypi/v/netbox-plugin-prometheus-sd)](https://pypi.org/project/netbox-plugin-prometheus-sd/)
+
+Provide Prometheus http_sd compatible API Endpoint with data from Netbox.
+
+HTTP SD is a new feature in Prometheus 2.28.0 that allows hosts to be found via a URL instead of just files.
+This plugin implements API endpoints in Netbox to make devices, IPs and virtual machines available to Prometheus.
+
+## Compatibility
+
+We aim to support the latest major versions of Netbox. For now we Support Netbox `2.11`, `3.0`, `3.1`, `3.2` and `3.3` including bugfix versions.
+All relevant target versions are tested in CI. Have a look at the Github Actions definition for the current build targets.
+
+## Installation
+
+The plugin is available as a Python package in pypi and can be installed with pip
+
+    pip install netbox-plugin-prometheus-sd
+
+Enable the plugin in /opt/netbox/netbox/netbox/configuration.py:
+
+    PLUGINS = ['netbox_prometheus_sd']
+
+The plugin has not further plugin configuration at the moment.
+
+## Usage
+
+The plugin only provides a new API endpoint on the Netbox API. There is no further action required after installation.
+
+### API
+
+The plugin reuses Netbox API view sets with new serializers for Prometheus.
+This means that all filters that can be used on the Netbox api can also be used to filter Prometheus targets.
+Paging is disabled because Prometheus does not support paged results.
+
+The plugin also reuses the Netbox authentication and permission model.
+Depending on the Netbox configuration, a token with valid object permissions must be passed to Netbox.
+
+```
+GET        /api/plugins/prometheus-sd/devices/              Get a list of devices in a prometheus compatible format
+GET        /api/plugins/prometheus-sd/virtual-machines/     Get a list of vms in a prometheus compatible format
+GET        /api/plugins/prometheus-sd/ip-addresses/         Get a list of ip in a prometheus compatible format
+```
+
+### Example
+
+A working example on how to use this plugin with Prometheus is located at the `example` folder. Netbox content is created by using Netbox docker initializers.
+
+The demo data doesn't make sense, but they are good enough for demonstrating how to configure Prometheus and get demo data to Prometheus service discovery.
+
+Go to the `example` folder and run `docker-compose up`. Prometheus should get available on `http://localhost:9090`.
+
+Push some example devices and objects to Netbox using the initializers:
+
+```
+docker-compose exec  netbox /opt/netbox/netbox/manage.py load_initializer_data --path /opt/netbox/initializers
+```
+
+Netbox content should then be available in the service discovery tab.
+
+## Development
+
+We use Poetry for dependency management and invoke as task runner.
+As Netbox plugins cannot be tested standalone, we need invoke to start all code embedded in Netbox Docker containers.
+
+All code to run in docker is located under `development`.
+To start a virtual env managed by poetry run `poetry shell`.
+All following commands are started inside this environment.
+
+In order to run tests invoke the test steps
+
+``` bash
+# Execute all tests
+invoke tests
+
+# Execute unit tests only
+invoke unittest
+```
+
+Features should be covered by a unit test, but some times it's easier to develop on an running system.
+
+``` bash
+# Start a local Netbox with docker
+invoke start
+
+# Create an user named `admin`
+invoke create-user
+```
+
+Visit http://localhost:8000 and log in with the new user.
+You can now define Netbox entities and test around.
+
+API endpoints for testing can be found at http://localhost:8000/api/plugins/prometheus-sd/
 
-setup(**setup_kwargs)
```

