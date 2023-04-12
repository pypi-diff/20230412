# Comparing `tmp/codeflare_sdk-0.4.2.tar.gz` & `tmp/codeflare_sdk-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeflare_sdk-0.4.2.tar", max compression
+gzip compressed data, was "codeflare_sdk-0.4.3.tar", max compression
```

## Comparing `codeflare_sdk-0.4.2.tar` & `codeflare_sdk-0.4.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11357 2022-11-22 00:48:43.906021 codeflare_sdk-0.4.2/LICENSE
--rw-r--r--   0        0        0     1852 2023-04-11 19:26:34.779878 codeflare_sdk-0.4.2/README.md
--rw-r--r--   0        0        0      728 2023-04-11 19:27:21.780203 codeflare_sdk-0.4.2/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-16 18:31:44.974735 codeflare_sdk-0.4.2/src/codeflare_sdk/__init__.py
--rw-r--r--   0        0        0        0 2022-11-16 19:42:48.730723 codeflare_sdk-0.4.2/src/codeflare_sdk/cluster/__init__.py
--rw-r--r--   0        0        0     4434 2023-04-11 19:26:34.787878 codeflare_sdk-0.4.2/src/codeflare_sdk/cluster/auth.py
--rw-r--r--   0        0        0    17834 2023-04-11 19:26:34.788878 codeflare_sdk-0.4.2/src/codeflare_sdk/cluster/cluster.py
--rw-r--r--   0        0        0     1706 2023-04-11 19:26:34.788878 codeflare_sdk-0.4.2/src/codeflare_sdk/cluster/config.py
--rw-r--r--   0        0        0     2141 2023-03-06 15:15:54.772713 codeflare_sdk-0.4.2/src/codeflare_sdk/cluster/model.py
--rw-r--r--   0        0        0        0 2023-03-27 14:54:38.071640 codeflare_sdk-0.4.2/src/codeflare_sdk/job/__init__.py
--rw-r--r--   0        0        0     6618 2023-04-11 19:26:34.788878 codeflare_sdk-0.4.2/src/codeflare_sdk/job/jobs.py
--rw-r--r--   0        0        0    10292 2022-11-16 18:31:44.978735 codeflare_sdk-0.4.2/src/codeflare_sdk/templates/aw-kuberay.yaml
--rw-r--r--   0        0        0     7782 2023-04-11 19:26:34.788878 codeflare_sdk-0.4.2/src/codeflare_sdk/templates/base-template.yaml
--rw-r--r--   0        0        0     9910 2023-04-11 19:26:34.788878 codeflare_sdk-0.4.2/src/codeflare_sdk/templates/new-template.yaml
--rw-r--r--   0        0        0        0 2022-11-16 19:42:58.205776 codeflare_sdk-0.4.2/src/codeflare_sdk/utils/__init__.py
--rwxr-xr-x   0        0        0    10830 2023-02-02 16:52:21.915294 codeflare_sdk-0.4.2/src/codeflare_sdk/utils/generate_yaml.py
--rw-r--r--   0        0        0     6778 2023-03-27 14:54:38.071640 codeflare_sdk-0.4.2/src/codeflare_sdk/utils/pretty_print.py
--rw-r--r--   0        0        0     2850 1970-01-01 00:00:00.000000 codeflare_sdk-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-11-22 00:48:43.906021 codeflare_sdk-0.4.3/LICENSE
+-rw-r--r--   0        0        0     1852 2023-04-11 19:26:34.779878 codeflare_sdk-0.4.3/README.md
+-rw-r--r--   0        0        0      728 2023-04-12 21:05:15.628402 codeflare_sdk-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-16 18:31:44.974735 codeflare_sdk-0.4.3/src/codeflare_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-16 19:42:48.730723 codeflare_sdk-0.4.3/src/codeflare_sdk/cluster/__init__.py
+-rw-r--r--   0        0        0     4434 2023-04-11 19:26:34.787878 codeflare_sdk-0.4.3/src/codeflare_sdk/cluster/auth.py
+-rw-r--r--   0        0        0    17834 2023-04-11 19:26:34.788878 codeflare_sdk-0.4.3/src/codeflare_sdk/cluster/cluster.py
+-rw-r--r--   0        0        0     1706 2023-04-11 19:26:34.788878 codeflare_sdk-0.4.3/src/codeflare_sdk/cluster/config.py
+-rw-r--r--   0        0        0     2141 2023-03-06 15:15:54.772713 codeflare_sdk-0.4.3/src/codeflare_sdk/cluster/model.py
+-rw-r--r--   0        0        0        0 2023-03-27 14:54:38.071640 codeflare_sdk-0.4.3/src/codeflare_sdk/job/__init__.py
+-rw-r--r--   0        0        0     6618 2023-04-11 19:26:34.788878 codeflare_sdk-0.4.3/src/codeflare_sdk/job/jobs.py
+-rw-r--r--   0        0        0    10292 2022-11-16 18:31:44.978735 codeflare_sdk-0.4.3/src/codeflare_sdk/templates/aw-kuberay.yaml
+-rw-r--r--   0        0        0     7782 2023-04-11 19:26:34.788878 codeflare_sdk-0.4.3/src/codeflare_sdk/templates/base-template.yaml
+-rw-r--r--   0        0        0    10080 2023-04-12 21:01:30.412216 codeflare_sdk-0.4.3/src/codeflare_sdk/templates/new-template.yaml
+-rw-r--r--   0        0        0        0 2022-11-16 19:42:58.205776 codeflare_sdk-0.4.3/src/codeflare_sdk/utils/__init__.py
+-rwxr-xr-x   0        0        0    10830 2023-02-02 16:52:21.915294 codeflare_sdk-0.4.3/src/codeflare_sdk/utils/generate_yaml.py
+-rw-r--r--   0        0        0     6778 2023-03-27 14:54:38.071640 codeflare_sdk-0.4.3/src/codeflare_sdk/utils/pretty_print.py
+-rw-r--r--   0        0        0     2850 1970-01-01 00:00:00.000000 codeflare_sdk-0.4.3/PKG-INFO
```

### Comparing `codeflare_sdk-0.4.2/LICENSE` & `codeflare_sdk-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.4.2/README.md` & `codeflare_sdk-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.4.2/pyproject.toml` & `codeflare_sdk-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "codeflare-sdk"
-version = "0.4.2"
+version = "0.4.3"
 description = "Python SDK for codeflare client"
 
 license = "Apache-2.0"
 
 authors = [
     "Michael Clifford <mcliffor@redhat.com>",
     "Mustafa Eyceoz <meyceoz@redhat.com>",
```

### Comparing `codeflare_sdk-0.4.2/src/codeflare_sdk/cluster/auth.py` & `codeflare_sdk-0.4.3/src/codeflare_sdk/cluster/auth.py`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.4.2/src/codeflare_sdk/cluster/cluster.py` & `codeflare_sdk-0.4.3/src/codeflare_sdk/cluster/cluster.py`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.4.2/src/codeflare_sdk/cluster/config.py` & `codeflare_sdk-0.4.3/src/codeflare_sdk/cluster/config.py`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.4.2/src/codeflare_sdk/cluster/model.py` & `codeflare_sdk-0.4.3/src/codeflare_sdk/cluster/model.py`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.4.2/src/codeflare_sdk/job/jobs.py` & `codeflare_sdk-0.4.3/src/codeflare_sdk/job/jobs.py`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.4.2/src/codeflare_sdk/templates/aw-kuberay.yaml` & `codeflare_sdk-0.4.3/src/codeflare_sdk/templates/aw-kuberay.yaml`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.4.2/src/codeflare_sdk/templates/base-template.yaml` & `codeflare_sdk-0.4.3/src/codeflare_sdk/templates/base-template.yaml`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.4.2/src/codeflare_sdk/templates/new-template.yaml` & `codeflare_sdk-0.4.3/src/codeflare_sdk/templates/new-template.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,20 @@
                       - matchExpressions:
                         - key: aw-kuberay
                           operator: In
                           values:
                           - "aw-kuberay"
                 containers:
                 # The Ray head pod
-                - name: ray-head
+                - env:
+                  - name: MY_POD_IP
+                    valueFrom:
+                      fieldRef:
+                        fieldPath: status.podIP
+                  name: ray-head
                   image: rayproject/ray:latest
                   imagePullPolicy: Always
                   ports:
                   - containerPort: 6379
                     name: gcs
                   - containerPort: 8265
                     name: dashboard
```

### Comparing `codeflare_sdk-0.4.2/src/codeflare_sdk/utils/generate_yaml.py` & `codeflare_sdk-0.4.3/src/codeflare_sdk/utils/generate_yaml.py`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.4.2/src/codeflare_sdk/utils/pretty_print.py` & `codeflare_sdk-0.4.3/src/codeflare_sdk/utils/pretty_print.py`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.4.2/PKG-INFO` & `codeflare_sdk-0.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeflare-sdk
-Version: 0.4.2
+Version: 0.4.3
 Summary: Python SDK for codeflare client
 Home-page: https://github.com/project-codeflare/codeflare-sdk
 License: Apache-2.0
 Keywords: codeflare,python,sdk,client,batch,scale
 Author: Michael Clifford
 Author-email: mcliffor@redhat.com
 Requires-Python: >=3.7,<4.0
```

