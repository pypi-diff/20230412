# Comparing `tmp/krkn_lib_kubernetes_draft-0.1.7.tar.gz` & `tmp/krkn_lib_kubernetes_draft-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krkn_lib_kubernetes_draft-0.1.7.tar", max compression
+gzip compressed data, was "krkn_lib_kubernetes_draft-0.1.8.tar", max compression
```

## Comparing `krkn_lib_kubernetes_draft-0.1.7.tar` & `krkn_lib_kubernetes_draft-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    10173 2023-04-06 15:46:32.348308 krkn_lib_kubernetes_draft-0.1.7/LICENSE
--rw-r--r--   0        0        0       22 2023-04-06 15:46:32.348308 krkn_lib_kubernetes_draft-0.1.7/README.md
--rw-r--r--   0        0        0      539 2023-04-06 15:46:32.412308 krkn_lib_kubernetes_draft-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       63 2023-04-06 15:46:32.348308 krkn_lib_kubernetes_draft-0.1.7/src/krkn_lib_kubernetes_draft/__init__.py
--rw-r--r--   0        0        0    39745 2023-04-06 15:46:44.396272 krkn_lib_kubernetes_draft-0.1.7/src/krkn_lib_kubernetes_draft/client.py
--rw-r--r--   0        0        0     1690 2023-04-06 15:46:32.348308 krkn_lib_kubernetes_draft-0.1.7/src/krkn_lib_kubernetes_draft/resources.py
--rw-r--r--   0        0        0      732 1970-01-01 00:00:00.000000 krkn_lib_kubernetes_draft-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    10173 2023-04-12 08:14:10.838229 krkn_lib_kubernetes_draft-0.1.8/LICENSE
+-rw-r--r--   0        0        0       22 2023-04-12 08:14:10.838229 krkn_lib_kubernetes_draft-0.1.8/README.md
+-rw-r--r--   0        0        0      539 2023-04-12 08:14:10.906230 krkn_lib_kubernetes_draft-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0       63 2023-04-12 08:14:10.838229 krkn_lib_kubernetes_draft-0.1.8/src/krkn_lib_kubernetes_draft/__init__.py
+-rw-r--r--   0        0        0    39728 2023-04-12 08:14:22.166372 krkn_lib_kubernetes_draft-0.1.8/src/krkn_lib_kubernetes_draft/client.py
+-rw-r--r--   0        0        0     1690 2023-04-12 08:14:10.838229 krkn_lib_kubernetes_draft-0.1.8/src/krkn_lib_kubernetes_draft/resources.py
+-rw-r--r--   0        0        0      732 1970-01-01 00:00:00.000000 krkn_lib_kubernetes_draft-0.1.8/PKG-INFO
```

### Comparing `krkn_lib_kubernetes_draft-0.1.7/LICENSE` & `krkn_lib_kubernetes_draft-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `krkn_lib_kubernetes_draft-0.1.7/pyproject.toml` & `krkn_lib_kubernetes_draft-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "krkn-lib-kubernetes-draft"
-version = "v0.1.7"
+version = "v0.1.8"
 description = "Kubernetes library for Kraken"
 authors = ["Red Hat Chaos Engineering Team"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/redhat-chaos/krkn"
 #packages = [{include= "src/krkn_lib_kubernetes_draft"}]
```

### Comparing `krkn_lib_kubernetes_draft-0.1.7/src/krkn_lib_kubernetes_draft/client.py` & `krkn_lib_kubernetes_draft-0.1.8/src/krkn_lib_kubernetes_draft/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,20 +57,20 @@
         if kubeconfig_string is not None and kubeconfig_path is None:
             raise Exception(
                 "please use either a kubeconfig path "
                 "or a valid kubeconfig string"
             )
 
         if kubeconfig_string is not None:
-            self.initialize_clients_from_kconfig_string(kubeconfig_string)
+            self.__initialize_clients_from_kconfig_string(kubeconfig_string)
         else:
-            self.initialize_clients(self.initialize_clients(kubeconfig_path))
+            self.__initialize_clients(kubeconfig_path)
 
     # Load kubeconfig and initialize kubernetes python client
-    def initialize_clients(self, kubeconfig_path: str = None):
+    def __initialize_clients(self, kubeconfig_path: str = None):
         """
         Initialize all clients from kubeconfig path
 
         :param kubeconfig_path: kubeconfig path,
                (optional default KUBE_CONFIG_DEFAULT_LOCATION)
         """
         if kubeconfig_path is None:
@@ -86,15 +86,15 @@
 
         except OSError:
             raise Exception(
                 f"Invalid kube-config file: {kubeconfig_path}. "
                 "No configuration found."
             )
 
-    def initialize_clients_from_kconfig_string(
+    def __initialize_clients_from_kconfig_string(
         self,
         kubeconfig_str: str,
     ):
         """
         Initialize all clients from kubeconfig yaml string
 
         :param kubeconfig_str: kubeconfig in string format
```

### Comparing `krkn_lib_kubernetes_draft-0.1.7/src/krkn_lib_kubernetes_draft/resources.py` & `krkn_lib_kubernetes_draft-0.1.8/src/krkn_lib_kubernetes_draft/resources.py`

 * *Files identical despite different names*

### Comparing `krkn_lib_kubernetes_draft-0.1.7/PKG-INFO` & `krkn_lib_kubernetes_draft-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krkn-lib-kubernetes-draft
-Version: 0.1.7
+Version: 0.1.8
 Summary: Kubernetes library for Kraken
 Home-page: https://github.com/redhat-chaos/krkn
 License: Apache-2.0
 Author: Red Hat Chaos Engineering Team
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

