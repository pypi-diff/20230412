# Comparing `tmp/nso-oc-2.42.0.tar.gz` & `tmp/nso-oc-2.43.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nso-oc-2.42.0.tar", last modified: Tue Apr 11 19:37:55 2023, max compression
+gzip compressed data, was "nso-oc-2.43.0.tar", last modified: Wed Apr 12 13:06:38 2023, max compression
```

## Comparing `nso-oc-2.42.0.tar` & `nso-oc-2.43.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:37:55.442282 nso-oc-2.42.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-04-11 19:37:05.000000 nso-oc-2.42.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-11 19:37:05.000000 nso-oc-2.42.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-11 19:37:55.442282 nso-oc-2.42.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-11 19:37:05.000000 nso-oc-2.42.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:37:55.434282 nso-oc-2.42.0/nso_oc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-11 19:37:55.000000 nso-oc-2.42.0/nso_oc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-11 19:37:55.000000 nso-oc-2.42.0/nso_oc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 19:37:55.000000 nso-oc-2.42.0/nso_oc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-11 19:37:55.000000 nso-oc-2.42.0/nso_oc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 19:37:55.000000 nso-oc-2.42.0/nso_oc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-11 19:37:55.000000 nso-oc-2.42.0/nso_oc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:37:55.434282 nso-oc-2.42.0/package_nso_to_oc/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-11 19:37:05.000000 nso-oc-2.42.0/package_nso_to_oc/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-11 19:37:05.000000 nso-oc-2.42.0/package_nso_to_oc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-11 19:37:05.000000 nso-oc-2.42.0/package_nso_to_oc/common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3569 2023-04-11 19:37:05.000000 nso-oc-2.42.0/package_nso_to_oc/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:37:55.438282 nso-oc-2.42.0/package_nso_to_oc/xe/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-11 19:37:05.000000 nso-oc-2.42.0/package_nso_to_oc/xe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-04-11 19:37:05.000000 nso-oc-2.42.0/package_nso_to_oc/xe/common_xe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-11 19:37:05.000000 nso-oc-2.42.0/package_nso_to_oc/xe/main_xe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30054 2023-04-11 19:37:05.000000 nso-oc-2.42.0/package_nso_to_oc/xe/xe_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)    36678 2023-04-11 19:37:05.000000 nso-oc-2.42.0/package_nso_to_oc/xe/xe_bgp.py
--rw-r--r--   0 runner    (1001) docker     (123)    58208 2023-04-11 19:37:05.000000 nso-oc-2.42.0/package_nso_to_oc/xe/xe_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    41835 2023-04-11 19:37:05.000000 nso-oc-2.42.0/package_nso_to_oc/xe/xe_network_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)    38030 2023-04-11 19:37:05.000000 nso-oc-2.42.0/package_nso_to_oc/xe/xe_ospfv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    29011 2023-04-11 19:37:05.000000 nso-oc-2.42.0/package_nso_to_oc/xe/xe_routing_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-04-11 19:37:05.000000 nso-oc-2.42.0/package_nso_to_oc/xe/xe_static_route.py
--rw-r--r--   0 runner    (1001) docker     (123)    32957 2023-04-11 19:37:05.000000 nso-oc-2.42.0/package_nso_to_oc/xe/xe_stp.py
--rw-r--r--   0 runner    (1001) docker     (123)    90722 2023-04-11 19:37:05.000000 nso-oc-2.42.0/package_nso_to_oc/xe/xe_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-04-11 19:37:05.000000 nso-oc-2.42.0/package_nso_to_oc/xe/xe_vlans.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:37:55.442282 nso-oc-2.42.0/package_nso_to_oc/xr/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-11 19:37:05.000000 nso-oc-2.42.0/package_nso_to_oc/xr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-11 19:37:05.000000 nso-oc-2.42.0/package_nso_to_oc/xr/common_xr.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-11 19:37:05.000000 nso-oc-2.42.0/package_nso_to_oc/xr/main_xr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23665 2023-04-11 19:37:05.000000 nso-oc-2.42.0/package_nso_to_oc/xr/xr_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-04-11 19:37:05.000000 nso-oc-2.42.0/package_nso_to_oc/xr/xr_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-04-11 19:37:05.000000 nso-oc-2.42.0/package_nso_to_oc/xr/xr_system.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-11 19:37:05.000000 nso-oc-2.42.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-11 19:37:55.442282 nso-oc-2.42.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-11 19:37:05.000000 nso-oc-2.42.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:06:38.835225 nso-oc-2.43.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-04-12 13:06:03.000000 nso-oc-2.43.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-12 13:06:03.000000 nso-oc-2.43.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-12 13:06:38.835225 nso-oc-2.43.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-12 13:06:03.000000 nso-oc-2.43.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:06:38.831225 nso-oc-2.43.0/nso_oc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-12 13:06:38.000000 nso-oc-2.43.0/nso_oc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-12 13:06:38.000000 nso-oc-2.43.0/nso_oc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 13:06:38.000000 nso-oc-2.43.0/nso_oc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-12 13:06:38.000000 nso-oc-2.43.0/nso_oc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 13:06:38.000000 nso-oc-2.43.0/nso_oc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 13:06:38.000000 nso-oc-2.43.0/nso_oc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:06:38.831225 nso-oc-2.43.0/package_nso_to_oc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-12 13:06:03.000000 nso-oc-2.43.0/package_nso_to_oc/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-12 13:06:03.000000 nso-oc-2.43.0/package_nso_to_oc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-12 13:06:03.000000 nso-oc-2.43.0/package_nso_to_oc/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3569 2023-04-12 13:06:03.000000 nso-oc-2.43.0/package_nso_to_oc/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:06:38.835225 nso-oc-2.43.0/package_nso_to_oc/xe/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-12 13:06:03.000000 nso-oc-2.43.0/package_nso_to_oc/xe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-04-12 13:06:03.000000 nso-oc-2.43.0/package_nso_to_oc/xe/common_xe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-12 13:06:03.000000 nso-oc-2.43.0/package_nso_to_oc/xe/main_xe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30054 2023-04-12 13:06:03.000000 nso-oc-2.43.0/package_nso_to_oc/xe/xe_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36678 2023-04-12 13:06:03.000000 nso-oc-2.43.0/package_nso_to_oc/xe/xe_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58208 2023-04-12 13:06:03.000000 nso-oc-2.43.0/package_nso_to_oc/xe/xe_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41835 2023-04-12 13:06:03.000000 nso-oc-2.43.0/package_nso_to_oc/xe/xe_network_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38030 2023-04-12 13:06:03.000000 nso-oc-2.43.0/package_nso_to_oc/xe/xe_ospfv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29448 2023-04-12 13:06:03.000000 nso-oc-2.43.0/package_nso_to_oc/xe/xe_routing_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-04-12 13:06:03.000000 nso-oc-2.43.0/package_nso_to_oc/xe/xe_static_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32957 2023-04-12 13:06:03.000000 nso-oc-2.43.0/package_nso_to_oc/xe/xe_stp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90722 2023-04-12 13:06:03.000000 nso-oc-2.43.0/package_nso_to_oc/xe/xe_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-04-12 13:06:03.000000 nso-oc-2.43.0/package_nso_to_oc/xe/xe_vlans.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:06:38.835225 nso-oc-2.43.0/package_nso_to_oc/xr/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-12 13:06:03.000000 nso-oc-2.43.0/package_nso_to_oc/xr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-12 13:06:03.000000 nso-oc-2.43.0/package_nso_to_oc/xr/common_xr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-12 13:06:03.000000 nso-oc-2.43.0/package_nso_to_oc/xr/main_xr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23665 2023-04-12 13:06:03.000000 nso-oc-2.43.0/package_nso_to_oc/xr/xr_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-04-12 13:06:03.000000 nso-oc-2.43.0/package_nso_to_oc/xr/xr_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-04-12 13:06:03.000000 nso-oc-2.43.0/package_nso_to_oc/xr/xr_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-12 13:06:03.000000 nso-oc-2.43.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-12 13:06:38.835225 nso-oc-2.43.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-12 13:06:03.000000 nso-oc-2.43.0/setup.py
```

### Comparing `nso-oc-2.42.0/LICENSE` & `nso-oc-2.43.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nso-oc-2.42.0/PKG-INFO` & `nso-oc-2.43.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nso-oc
-Version: 2.42.0
+Version: 2.43.0
 Summary: Cisco NSO OpenConfig Tools
 Home-page: https://github.com/model-driven-devops/nso-oc-services
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NSO NED device configuration to OpenConfig
```

### Comparing `nso-oc-2.42.0/README.md` & `nso-oc-2.43.0/README.md`

 * *Files identical despite different names*

### Comparing `nso-oc-2.42.0/nso_oc.egg-info/PKG-INFO` & `nso-oc-2.43.0/nso_oc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nso-oc
-Version: 2.42.0
+Version: 2.43.0
 Summary: Cisco NSO OpenConfig Tools
 Home-page: https://github.com/model-driven-devops/nso-oc-services
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NSO NED device configuration to OpenConfig
```

### Comparing `nso-oc-2.42.0/nso_oc.egg-info/SOURCES.txt` & `nso-oc-2.43.0/nso_oc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nso-oc-2.42.0/package_nso_to_oc/README.md` & `nso-oc-2.43.0/package_nso_to_oc/README.md`

 * *Files identical despite different names*

### Comparing `nso-oc-2.42.0/package_nso_to_oc/common.py` & `nso-oc-2.43.0/package_nso_to_oc/common.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.42.0/package_nso_to_oc/main.py` & `nso-oc-2.43.0/package_nso_to_oc/main.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.42.0/package_nso_to_oc/xe/common_xe.py` & `nso-oc-2.43.0/package_nso_to_oc/xe/common_xe.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.42.0/package_nso_to_oc/xe/main_xe.py` & `nso-oc-2.43.0/package_nso_to_oc/xe/main_xe.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.42.0/package_nso_to_oc/xe/xe_acls.py` & `nso-oc-2.43.0/package_nso_to_oc/xe/xe_acls.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.42.0/package_nso_to_oc/xe/xe_bgp.py` & `nso-oc-2.43.0/package_nso_to_oc/xe/xe_bgp.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.42.0/package_nso_to_oc/xe/xe_interfaces.py` & `nso-oc-2.43.0/package_nso_to_oc/xe/xe_interfaces.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.42.0/package_nso_to_oc/xe/xe_network_instances.py` & `nso-oc-2.43.0/package_nso_to_oc/xe/xe_network_instances.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.42.0/package_nso_to_oc/xe/xe_ospfv2.py` & `nso-oc-2.43.0/package_nso_to_oc/xe/xe_ospfv2.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.42.0/package_nso_to_oc/xe/xe_routing_policy.py` & `nso-oc-2.43.0/package_nso_to_oc/xe/xe_routing_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,60 +75,62 @@
                 "openconfig-routing-policy:name": prefix.get("name"),
                 "openconfig-routing-policy:mode": "IPV4"
             },
             "openconfig-routing-policy:prefixes": {"openconfig-routing-policy:prefix": []}
         }
         prefixes = new_prefix_set["openconfig-routing-policy:prefixes"]["openconfig-routing-policy:prefix"]
         seq_list_after = common.get_index_or_default(xe_prefixes_after, prefix_index, {}).get("seq", [])
-        all_processed = True
 
         for seq_index, seq in enumerate(prefix.get("seq", [])):
             if "deny" in seq:
-                all_processed = False
-                routing_policy_notes.append(
-f"""
-Prefix Name: {prefix.get("name")}
-Sequence Number: {seq.get("no")}
-This sequence contains a deny operation, which is not supported in OpenConfig. Translation, of the entire list, to OC will be skipped.
-""")
-                continue
-            if not "permit" in seq:
-                continue
-
-            masklength = "exact" if not "le" in seq["permit"] else f'{seq["permit"].get("ge", 0)}..{seq["permit"]["le"]}'
-            new_prefix = {
-                "openconfig-routing-policy:ip-prefix": seq["permit"].get("ip"),
-                "openconfig-routing-policy:masklength-range": masklength,
-                "openconfig-routing-policy:config": {
+                masklength = "exact" if not "le" in seq["deny"] else f'{seq["deny"].get("ge", 0)}..{seq["deny"]["le"]}'
+                new_prefix = {
+                    "openconfig-routing-policy:ip-prefix": seq["deny"].get("ip"),
+                    "openconfig-routing-policy:masklength-range": masklength,
+                    "openconfig-routing-policy:config": {
+                        "openconfig-routing-policy:ip-prefix": seq["deny"].get("ip"),
+                        "openconfig-routing-policy:masklength-range": masklength,
+                        "openconfig-routing-policy-ext:seq": seq["no"],
+                        "openconfig-routing-policy-ext:policy_action": 'DENY_ROUTE'
+                    }
+                }
+            elif "permit" in seq:
+                masklength = "exact" if not "le" in seq["permit"] else f'{seq["permit"].get("ge", 0)}..{seq["permit"]["le"]}'
+                new_prefix = {
                     "openconfig-routing-policy:ip-prefix": seq["permit"].get("ip"),
                     "openconfig-routing-policy:masklength-range": masklength,
-                    "openconfig-routing-policy-ext:seq": seq["no"]
+                    "openconfig-routing-policy:config": {
+                        "openconfig-routing-policy:ip-prefix": seq["permit"].get("ip"),
+                        "openconfig-routing-policy:masklength-range": masklength,
+                        "openconfig-routing-policy-ext:seq": seq["no"],
+                        "openconfig-routing-policy-ext:policy_action": 'PERMIT_ROUTE'
+                    }
                 }
-            }
+
             prefixes.append(new_prefix)
 
-            # # Ensure the value we're nullifying does exist
-            # if common.get_index_or_default(seq_list_after, seq_index, None):
-            #     seq_list_after[seq_index] = None
-
-        if all_processed:
-            prefix_sets["openconfig-routing-policy:prefix-sets"]["openconfig-routing-policy:prefix-set"].append(new_prefix_set)
-            common.get_index_or_default(xe_prefixes_after, prefix_index, {})["name"] = None
-    
+            # Ensure the value we're nullifying does exist
+            if common.get_index_or_default(seq_list_after, seq_index, None):
+                seq_list_after[seq_index] = None
+
+        prefix_sets["openconfig-routing-policy:prefix-sets"]["openconfig-routing-policy:prefix-set"].append(new_prefix_set)
+        common.get_index_or_default(xe_prefixes_after, prefix_index, {})["name"] = None
+
     for prefix_item in config_after.get("tailf-ned-cisco-ios:ip", {}).get("prefix-list", {}).get("prefixes", []):
         if "name" in prefix_item and prefix_item["name"]:
             prefixes_list.append(prefix_item)
-    
+
     if len(prefixes_list) > 0:
         config_after["tailf-ned-cisco-ios:ip"]["prefix-list"]["prefixes"] = prefixes_list
     elif "prefixes" in config_after.get("tailf-ned-cisco-ios:ip", {}).get("prefix-list", {}):
         del config_after["tailf-ned-cisco-ios:ip"]["prefix-list"]["prefixes"]
 
     openconfig_routing_policies["openconfig-routing-policy:routing-policy"]["openconfig-routing-policy:defined-sets"].update(prefix_sets)
 
+
 def process_as_path_sets(config_before, config_after):
     as_path_sets = {"openconfig-bgp-policy:as-path-sets": {"openconfig-bgp-policy:as-path-set": []}}
     access_list = config_before.get("tailf-ned-cisco-ios:ip", {}).get("as-path", {}).get("access-list", [])
     access_list_after = config_after.get("tailf-ned-cisco-ios:ip", {}).get("as-path", {}).get("access-list", [])
     all_processed = True
     updated_access_list = []
```

### Comparing `nso-oc-2.42.0/package_nso_to_oc/xe/xe_static_route.py` & `nso-oc-2.43.0/package_nso_to_oc/xe/xe_static_route.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.42.0/package_nso_to_oc/xe/xe_stp.py` & `nso-oc-2.43.0/package_nso_to_oc/xe/xe_stp.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.42.0/package_nso_to_oc/xe/xe_system.py` & `nso-oc-2.43.0/package_nso_to_oc/xe/xe_system.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.42.0/package_nso_to_oc/xe/xe_vlans.py` & `nso-oc-2.43.0/package_nso_to_oc/xe/xe_vlans.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.42.0/package_nso_to_oc/xr/common_xr.py` & `nso-oc-2.43.0/package_nso_to_oc/xr/common_xr.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.42.0/package_nso_to_oc/xr/main_xr.py` & `nso-oc-2.43.0/package_nso_to_oc/xr/main_xr.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.42.0/package_nso_to_oc/xr/xr_acls.py` & `nso-oc-2.43.0/package_nso_to_oc/xr/xr_acls.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.42.0/package_nso_to_oc/xr/xr_interfaces.py` & `nso-oc-2.43.0/package_nso_to_oc/xr/xr_interfaces.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.42.0/package_nso_to_oc/xr/xr_system.py` & `nso-oc-2.43.0/package_nso_to_oc/xr/xr_system.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.42.0/setup.py` & `nso-oc-2.43.0/setup.py`

 * *Files identical despite different names*

