# Comparing `tmp/janus-dtnaas-0.2.post8.tar.gz` & `tmp/janus-dtnaas-0.2.post9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "janus-dtnaas-0.2.post8.tar", last modified: Thu Feb  9 20:49:50 2023, max compression
+gzip compressed data, was "janus-dtnaas-0.2.post9.tar", last modified: Fri Apr  7 15:36:23 2023, max compression
```

## Comparing `janus-dtnaas-0.2.post8.tar` & `janus-dtnaas-0.2.post9.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2023-02-09 20:49:50.726116 janus-dtnaas-0.2.post8/
--rw-r--r--   0 ezra      (1000) ezra      (1000)     1513 2022-09-29 18:53:21.000000 janus-dtnaas-0.2.post8/LICENSE
--rw-r--r--   0 ezra      (1000) ezra      (1000)       41 2022-09-29 18:53:21.000000 janus-dtnaas-0.2.post8/MANIFEST.in
--rw-r--r--   0 ezra      (1000) ezra      (1000)      888 2023-02-09 20:49:50.726116 janus-dtnaas-0.2.post8/PKG-INFO
--rw-r--r--   0 ezra      (1000) ezra      (1000)      365 2022-09-29 18:53:21.000000 janus-dtnaas-0.2.post8/README.md
-drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2023-02-09 20:49:50.722115 janus-dtnaas-0.2.post8/janus/
--rw-r--r--   0 ezra      (1000) ezra      (1000)        0 2021-10-13 19:48:34.000000 janus-dtnaas-0.2.post8/janus/__init__.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)       24 2021-10-13 19:48:34.000000 janus-dtnaas-0.2.post8/janus/agent_settings.py
-drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2023-02-09 20:49:50.722115 janus-dtnaas-0.2.post8/janus/api/
--rw-r--r--   0 ezra      (1000) ezra      (1000)        0 2022-09-29 18:53:21.000000 janus-dtnaas-0.2.post8/janus/api/__init__.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)    10792 2022-09-29 18:53:25.000000 janus-dtnaas-0.2.post8/janus/api/agent.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)     3733 2022-11-28 18:12:35.000000 janus-dtnaas-0.2.post8/janus/api/ansible_job.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)    35515 2023-02-09 20:49:16.000000 janus-dtnaas-0.2.post8/janus/api/controller.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)     5865 2023-02-06 20:00:48.000000 janus-dtnaas-0.2.post8/janus/api/db.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)    33445 2022-10-11 19:47:32.000000 janus-dtnaas-0.2.post8/janus/api/endpoints_api.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)      722 2022-11-28 18:12:35.000000 janus-dtnaas-0.2.post8/janus/api/models.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)     9097 2023-02-06 20:00:48.000000 janus-dtnaas-0.2.post8/janus/api/portainer_docker.py
-drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2023-02-09 20:49:50.726116 janus-dtnaas-0.2.post8/janus/api/sys/
--rw-r--r--   0 ezra      (1000) ezra      (1000)        0 2021-10-13 19:48:34.000000 janus-dtnaas-0.2.post8/janus/api/sys/__init__.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)      206 2021-10-13 19:48:34.000000 janus-dtnaas-0.2.post8/janus/api/sys/cpu.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)      599 2021-10-13 19:48:34.000000 janus-dtnaas-0.2.post8/janus/api/sys/disk.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)      313 2021-10-13 19:48:34.000000 janus-dtnaas-0.2.post8/janus/api/sys/mem.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)     1668 2022-09-29 18:53:21.000000 janus-dtnaas-0.2.post8/janus/api/sys/net.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)      373 2021-10-13 19:48:34.000000 janus-dtnaas-0.2.post8/janus/api/sys/numa.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)     2411 2021-10-13 19:48:34.000000 janus-dtnaas-0.2.post8/janus/api/sys/sysctl.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)    11595 2022-09-29 18:53:25.000000 janus-dtnaas-0.2.post8/janus/api/sys/tc.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)    16522 2022-12-07 17:00:22.000000 janus-dtnaas-0.2.post8/janus/api/utils.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)     1906 2022-11-28 18:12:35.000000 janus-dtnaas-0.2.post8/janus/api/validator.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)     5098 2023-01-10 21:16:29.000000 janus-dtnaas-0.2.post8/janus/app.py
-drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2023-02-09 20:49:50.726116 janus-dtnaas-0.2.post8/janus/config/
--rw-r--r--   0 ezra      (1000) ezra      (1000)      122 2022-09-29 18:53:21.000000 janus-dtnaas-0.2.post8/janus/config/janus.conf.example
--rw-r--r--   0 ezra      (1000) ezra      (1000)      369 2022-09-29 18:53:21.000000 janus-dtnaas-0.2.post8/janus/config/logging.conf
-drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2023-02-09 20:49:50.726116 janus-dtnaas-0.2.post8/janus/config/profiles/
--rw-r--r--   0 ezra      (1000) ezra      (1000)      193 2022-11-28 18:12:35.000000 janus-dtnaas-0.2.post8/janus/config/profiles/ansible.yaml
--rw-r--r--   0 ezra      (1000) ezra      (1000)      217 2022-09-29 18:53:21.000000 janus-dtnaas-0.2.post8/janus/config/profiles/features.yaml
--rw-r--r--   0 ezra      (1000) ezra      (1000)      177 2022-09-29 18:53:21.000000 janus-dtnaas-0.2.post8/janus/config/profiles/profiles.yaml
--rw-r--r--   0 ezra      (1000) ezra      (1000)      133 2022-09-29 18:53:21.000000 janus-dtnaas-0.2.post8/janus/config/profiles/qos.yaml
--rw-r--r--   0 ezra      (1000) ezra      (1000)      943 2022-11-28 18:12:35.000000 janus-dtnaas-0.2.post8/janus/config/profiles/test-profile.yaml
--rw-r--r--   0 ezra      (1000) ezra      (1000)      374 2022-09-29 18:53:21.000000 janus-dtnaas-0.2.post8/janus/config/profiles/volumes.yaml
-drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2023-02-09 20:49:50.726116 janus-dtnaas-0.2.post8/janus/lib/
--rw-r--r--   0 ezra      (1000) ezra      (1000)       40 2021-10-13 19:48:34.000000 janus-dtnaas-0.2.post8/janus/lib/__init__.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)     3744 2023-02-06 20:00:48.000000 janus-dtnaas-0.2.post8/janus/lib/agent_monitor.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)     8970 2023-02-06 20:00:48.000000 janus-dtnaas-0.2.post8/janus/settings.py
-drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2023-02-09 20:49:50.726116 janus-dtnaas-0.2.post8/janus_dtnaas.egg-info/
--rw-r--r--   0 ezra      (1000) ezra      (1000)      888 2023-02-09 20:49:50.000000 janus-dtnaas-0.2.post8/janus_dtnaas.egg-info/PKG-INFO
--rw-r--r--   0 ezra      (1000) ezra      (1000)     1086 2023-02-09 20:49:50.000000 janus-dtnaas-0.2.post8/janus_dtnaas.egg-info/SOURCES.txt
--rw-r--r--   0 ezra      (1000) ezra      (1000)        1 2023-02-09 20:49:50.000000 janus-dtnaas-0.2.post8/janus_dtnaas.egg-info/dependency_links.txt
--rw-r--r--   0 ezra      (1000) ezra      (1000)       46 2023-02-09 20:49:50.000000 janus-dtnaas-0.2.post8/janus_dtnaas.egg-info/entry_points.txt
--rw-r--r--   0 ezra      (1000) ezra      (1000)      201 2023-02-09 20:49:50.000000 janus-dtnaas-0.2.post8/janus_dtnaas.egg-info/requires.txt
--rw-r--r--   0 ezra      (1000) ezra      (1000)        6 2023-02-09 20:49:50.000000 janus-dtnaas-0.2.post8/janus_dtnaas.egg-info/top_level.txt
--rw-r--r--   0 ezra      (1000) ezra      (1000)      201 2022-11-28 18:12:35.000000 janus-dtnaas-0.2.post8/requirements.txt
--rw-r--r--   0 ezra      (1000) ezra      (1000)       38 2023-02-09 20:49:50.726116 janus-dtnaas-0.2.post8/setup.cfg
--rw-r--r--   0 ezra      (1000) ezra      (1000)     2723 2023-02-09 20:49:26.000000 janus-dtnaas-0.2.post8/setup.py
-drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2023-02-09 20:49:50.726116 janus-dtnaas-0.2.post8/tests/
--rw-r--r--   0 ezra      (1000) ezra      (1000)      165 2022-03-01 15:51:48.000000 janus-dtnaas-0.2.post8/tests/test_api.py
+drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2023-04-07 15:36:23.300041 janus-dtnaas-0.2.post9/
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     1513 2022-09-29 18:53:21.000000 janus-dtnaas-0.2.post9/LICENSE
+-rw-r--r--   0 ezra      (1000) ezra      (1000)       41 2022-09-29 18:53:21.000000 janus-dtnaas-0.2.post9/MANIFEST.in
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      888 2023-04-07 15:36:23.300041 janus-dtnaas-0.2.post9/PKG-INFO
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      365 2022-09-29 18:53:21.000000 janus-dtnaas-0.2.post9/README.md
+drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2023-04-07 15:36:23.292041 janus-dtnaas-0.2.post9/janus/
+-rw-r--r--   0 ezra      (1000) ezra      (1000)        0 2021-10-13 19:48:34.000000 janus-dtnaas-0.2.post9/janus/__init__.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)       24 2021-10-13 19:48:34.000000 janus-dtnaas-0.2.post9/janus/agent_settings.py
+drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2023-04-07 15:36:23.296041 janus-dtnaas-0.2.post9/janus/api/
+-rw-r--r--   0 ezra      (1000) ezra      (1000)        0 2022-09-29 18:53:21.000000 janus-dtnaas-0.2.post9/janus/api/__init__.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)    10792 2022-09-29 18:53:25.000000 janus-dtnaas-0.2.post9/janus/api/agent.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     3733 2022-11-28 18:12:35.000000 janus-dtnaas-0.2.post9/janus/api/ansible_job.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)    35097 2023-04-07 15:30:08.000000 janus-dtnaas-0.2.post9/janus/api/controller.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     5971 2023-04-07 15:30:08.000000 janus-dtnaas-0.2.post9/janus/api/db.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)    33445 2022-10-11 19:47:32.000000 janus-dtnaas-0.2.post9/janus/api/endpoints_api.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      722 2022-11-28 18:12:35.000000 janus-dtnaas-0.2.post9/janus/api/models.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     9097 2023-02-06 20:00:48.000000 janus-dtnaas-0.2.post9/janus/api/portainer_docker.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      717 2023-04-07 15:30:08.000000 janus-dtnaas-0.2.post9/janus/api/query.py
+drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2023-04-07 15:36:23.296041 janus-dtnaas-0.2.post9/janus/api/sys/
+-rw-r--r--   0 ezra      (1000) ezra      (1000)        0 2021-10-13 19:48:34.000000 janus-dtnaas-0.2.post9/janus/api/sys/__init__.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      206 2021-10-13 19:48:34.000000 janus-dtnaas-0.2.post9/janus/api/sys/cpu.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      599 2021-10-13 19:48:34.000000 janus-dtnaas-0.2.post9/janus/api/sys/disk.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      313 2021-10-13 19:48:34.000000 janus-dtnaas-0.2.post9/janus/api/sys/mem.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     1668 2022-09-29 18:53:21.000000 janus-dtnaas-0.2.post9/janus/api/sys/net.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      373 2021-10-13 19:48:34.000000 janus-dtnaas-0.2.post9/janus/api/sys/numa.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     2411 2021-10-13 19:48:34.000000 janus-dtnaas-0.2.post9/janus/api/sys/sysctl.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)    11595 2022-09-29 18:53:25.000000 janus-dtnaas-0.2.post9/janus/api/sys/tc.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)    16522 2022-12-07 17:00:22.000000 janus-dtnaas-0.2.post9/janus/api/utils.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     1906 2022-11-28 18:12:35.000000 janus-dtnaas-0.2.post9/janus/api/validator.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     5098 2023-02-10 21:07:23.000000 janus-dtnaas-0.2.post9/janus/app.py
+drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2023-04-07 15:36:23.296041 janus-dtnaas-0.2.post9/janus/config/
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      122 2022-09-29 18:53:21.000000 janus-dtnaas-0.2.post9/janus/config/janus.conf.example
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      369 2023-02-10 21:10:31.000000 janus-dtnaas-0.2.post9/janus/config/logging.conf
+drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2023-04-07 15:36:23.300041 janus-dtnaas-0.2.post9/janus/config/profiles/
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      193 2022-11-28 18:12:35.000000 janus-dtnaas-0.2.post9/janus/config/profiles/ansible.yaml
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      217 2022-09-29 18:53:21.000000 janus-dtnaas-0.2.post9/janus/config/profiles/features.yaml
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      177 2022-09-29 18:53:21.000000 janus-dtnaas-0.2.post9/janus/config/profiles/profiles.yaml
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      133 2022-09-29 18:53:21.000000 janus-dtnaas-0.2.post9/janus/config/profiles/qos.yaml
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      943 2022-11-28 18:12:35.000000 janus-dtnaas-0.2.post9/janus/config/profiles/test-profile.yaml
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      374 2022-09-29 18:53:21.000000 janus-dtnaas-0.2.post9/janus/config/profiles/volumes.yaml
+drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2023-04-07 15:36:23.300041 janus-dtnaas-0.2.post9/janus/lib/
+-rw-r--r--   0 ezra      (1000) ezra      (1000)       40 2021-10-13 19:48:34.000000 janus-dtnaas-0.2.post9/janus/lib/__init__.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     3744 2023-02-06 20:00:48.000000 janus-dtnaas-0.2.post9/janus/lib/agent_monitor.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     8770 2023-04-07 15:30:08.000000 janus-dtnaas-0.2.post9/janus/settings.py
+drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2023-04-07 15:36:23.300041 janus-dtnaas-0.2.post9/janus_dtnaas.egg-info/
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      888 2023-04-07 15:36:23.000000 janus-dtnaas-0.2.post9/janus_dtnaas.egg-info/PKG-INFO
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     1105 2023-04-07 15:36:23.000000 janus-dtnaas-0.2.post9/janus_dtnaas.egg-info/SOURCES.txt
+-rw-r--r--   0 ezra      (1000) ezra      (1000)        1 2023-04-07 15:36:23.000000 janus-dtnaas-0.2.post9/janus_dtnaas.egg-info/dependency_links.txt
+-rw-r--r--   0 ezra      (1000) ezra      (1000)       46 2023-04-07 15:36:23.000000 janus-dtnaas-0.2.post9/janus_dtnaas.egg-info/entry_points.txt
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      201 2023-04-07 15:36:23.000000 janus-dtnaas-0.2.post9/janus_dtnaas.egg-info/requires.txt
+-rw-r--r--   0 ezra      (1000) ezra      (1000)        6 2023-04-07 15:36:23.000000 janus-dtnaas-0.2.post9/janus_dtnaas.egg-info/top_level.txt
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      201 2022-11-28 18:12:35.000000 janus-dtnaas-0.2.post9/requirements.txt
+-rw-r--r--   0 ezra      (1000) ezra      (1000)       38 2023-04-07 15:36:23.300041 janus-dtnaas-0.2.post9/setup.cfg
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     2723 2023-04-07 15:35:53.000000 janus-dtnaas-0.2.post9/setup.py
+drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2023-04-07 15:36:23.300041 janus-dtnaas-0.2.post9/tests/
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      165 2022-03-01 15:51:48.000000 janus-dtnaas-0.2.post9/tests/test_api.py
```

### Comparing `janus-dtnaas-0.2.post8/LICENSE` & `janus-dtnaas-0.2.post9/LICENSE`

 * *Files identical despite different names*

### Comparing `janus-dtnaas-0.2.post8/PKG-INFO` & `janus-dtnaas-0.2.post9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: janus-dtnaas
-Version: 0.2.post8
+Version: 0.2.post9
 Summary: Janus DTNaaS Controller
 Home-page: https://github.com/esnet/janus
 Author: Ezra Kissel
 Author-email: kissel@es.net
 Keywords: Janus Controller
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
```

### Comparing `janus-dtnaas-0.2.post8/janus/api/agent.py` & `janus-dtnaas-0.2.post9/janus/api/agent.py`

 * *Files identical despite different names*

### Comparing `janus-dtnaas-0.2.post8/janus/api/ansible_job.py` & `janus-dtnaas-0.2.post9/janus/api/ansible_job.py`

 * *Files identical despite different names*

### Comparing `janus-dtnaas-0.2.post8/janus/api/controller.py` & `janus-dtnaas-0.2.post9/janus/api/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,59 +16,44 @@
 from werkzeug.exceptions import BadRequest
 
 from pydantic import ValidationError
 from urllib.parse import urlsplit
 from janus import settings
 from janus.lib import AgentMonitor
 from janus.settings import cfg
-from .utils import create_service, commit_db, precommit_db, error_svc, handle_image, set_qos
-from .db import init_db
-from .validator import Profile as ProfileSchema
+from janus.api.utils import create_service, commit_db, precommit_db, error_svc, handle_image, set_qos
+from janus.api.db import init_db
+from janus.api.query import QueryUser
+from janus.api.validator import Profile as ProfileSchema
+from janus.api.ansible_job import AnsibleJob
 
 # XXX: Portainer will eventually go behind an ABC interface
 # so we can support other provisioning backends
 from portainer_api.configuration import Configuration as Config
 from portainer_api.api_client import ApiClient
 from portainer_api.api import AuthApi
 from portainer_api.models import AuthenticateUserRequest
 from portainer_api.rest import ApiException
-from .portainer_docker import PortainerDockerApi
-from .endpoints_api import EndpointsApi
-from .ansible_job import AnsibleJob
+from janus.api.portainer_docker import PortainerDockerApi
+from janus.api.endpoints_api import EndpointsApi
+
 
 class State(Enum):
     UNKNOWN = 0
     INITIALIZED = 1
     STARTED = 2
     STOPPED = 3
     MIXED = 4
 
 class EPType(Enum):
     UNKNOWN = 0,
     PORTAINER = 1
     KUBERNETES = 2
     DOCKER = 3
 
-class QueryUser:
-    def query_builder(self, user=None, group=None, qargs=dict()):
-        qs = list()
-        user = user.split(',') if user else None
-        group = group.split(',') if group else None
-        if user and group:
-            qs.append(where('users').any(user) | where('groups').any(group))
-        elif user:
-            qs.append(where('users').any(user))
-        elif group:
-            qs.append(where('groups').any(group))
-        for k,v in qargs.items():
-            if v:
-                qs.append(eq(where(k), v))
-        if len(qs):
-            return reduce(lambda a, b: a & b, qs)
-        return None
 
 # Basic auth
 httpauth = HTTPBasicAuth()
 
 log = logging.getLogger(__name__)
 
 ns = Namespace('janus/controller', description='Operations for Janus on-demand container provisioning')
@@ -496,14 +481,16 @@
                 if "node" in s:
                     del s['node']
 
         # complete accounting
         record['id'] = Id
         record['services'] = svcs
         record['request'] = req
+        record['users'] = user.split(",") if user else []
+        record['groups'] = group.split(",") if group else []
         if errs:
             precommit_db(Id, delete=True)
             return {Id: record}
         else:
             return commit_db(record, Id)
```

### Comparing `janus-dtnaas-0.2.post8/janus/api/db.py` & `janus-dtnaas-0.2.post9/janus/api/db.py`

 * *Files 6% similar despite different names*

```diff
@@ -115,19 +115,23 @@
     else:
         assert(nodes is not None)
 
     try:
         dapi = PortainerDockerApi(client)
         am   = AgentMonitor(client)
         futures = list()
-        with ThreadPoolExecutor(max_workers=8) as executor:
-            for k, v in nodes.items():
-                futures.append(executor.submit(_get_endpoint_info, v['id'], v['public_url'], k, nodes))
-        for future in concurrent.futures.as_completed(futures):
-            item = future.result()
+        tp = ThreadPoolExecutor(max_workers=8)
+        for k, v in nodes.items():
+            futures.append(tp.submit(_get_endpoint_info, v['id'], v['public_url'], k, nodes))
+        for future in futures:
+            try:
+                item = future.result(timeout=5)
+            except Exception as e:
+                log.error(f"Timeout waiting on endpoint query, continuing")
+                continue
             mutex.acquire()
             node_table.upsert(item, Node.name == item['name'])
             mutex.release()
     except Exception as e:
         import traceback
         traceback.print_exc()
         log.error("Backend error: {}".format(e))
```

### Comparing `janus-dtnaas-0.2.post8/janus/api/endpoints_api.py` & `janus-dtnaas-0.2.post9/janus/api/endpoints_api.py`

 * *Files identical despite different names*

### Comparing `janus-dtnaas-0.2.post8/janus/api/models.py` & `janus-dtnaas-0.2.post9/janus/api/models.py`

 * *Files identical despite different names*

### Comparing `janus-dtnaas-0.2.post8/janus/api/portainer_docker.py` & `janus-dtnaas-0.2.post9/janus/api/portainer_docker.py`

 * *Files identical despite different names*

### Comparing `janus-dtnaas-0.2.post8/janus/api/sys/disk.py` & `janus-dtnaas-0.2.post9/janus/api/sys/disk.py`

 * *Files identical despite different names*

### Comparing `janus-dtnaas-0.2.post8/janus/api/sys/net.py` & `janus-dtnaas-0.2.post9/janus/api/sys/net.py`

 * *Files identical despite different names*

### Comparing `janus-dtnaas-0.2.post8/janus/api/sys/sysctl.py` & `janus-dtnaas-0.2.post9/janus/api/sys/sysctl.py`

 * *Files identical despite different names*

### Comparing `janus-dtnaas-0.2.post8/janus/api/sys/tc.py` & `janus-dtnaas-0.2.post9/janus/api/sys/tc.py`

 * *Files identical despite different names*

### Comparing `janus-dtnaas-0.2.post8/janus/api/utils.py` & `janus-dtnaas-0.2.post9/janus/api/utils.py`

 * *Files identical despite different names*

### Comparing `janus-dtnaas-0.2.post8/janus/api/validator.py` & `janus-dtnaas-0.2.post9/janus/api/validator.py`

 * *Files identical despite different names*

### Comparing `janus-dtnaas-0.2.post8/janus/app.py` & `janus-dtnaas-0.2.post9/janus/app.py`

 * *Files identical despite different names*

### Comparing `janus-dtnaas-0.2.post8/janus/config/profiles/test-profile.yaml` & `janus-dtnaas-0.2.post9/janus/config/profiles/test-profile.yaml`

 * *Files identical despite different names*

### Comparing `janus-dtnaas-0.2.post8/janus/lib/agent_monitor.py` & `janus-dtnaas-0.2.post9/janus/lib/agent_monitor.py`

 * *Files identical despite different names*

### Comparing `janus-dtnaas-0.2.post8/janus/settings.py` & `janus-dtnaas-0.2.post9/janus/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import yaml
 import logging
 from tinydb import TinyDB, Query, where
 from operator import eq
 from functools import reduce
 from werkzeug.security import generate_password_hash
 from janus.api.validator import QoS_Controller, Profile
+from janus.api.query import QueryUser
+
 
 API_PREFIX = '/api'
 DEFAULT_CFG_PATH = "/etc/janus/janus.conf"
 DEFAULT_PROFILE_PATH = "/etc/janus/profiles"
 DEFAULT_DB_PATH = "/etc/janus/db.json"
 #LOG_CFG_PATH = "/etc/janus/logging.conf"
 IGNORE_EPS = []
@@ -137,25 +139,16 @@
     def get_dbpath(self):
         return self._dbpath
 
     def get_users(self):
         return self._users
 
     def get_profile_from_db(self, p=None, user=None, group=None):
-        qs = list()
-        if user:
-            qs.append(where('users').any(user))
-        if group:
-            qs.append(where('groups').any(group))
-        if p:
-            qs.append(eq(where('name'), p))
-        if len(qs):
-            query = reduce(lambda a, b: a & b, qs)
-        else:
-            query = None
+        q = QueryUser()
+        query = q.query_builder(user, group, {"name": p})
         profile_tbl = self.db.table('profiles')
         if query and p:
             return profile_tbl.get(query)
         elif query:
             return profile_tbl.search(query)
         else:
             return profile_tbl.all()
```

### Comparing `janus-dtnaas-0.2.post8/janus_dtnaas.egg-info/PKG-INFO` & `janus-dtnaas-0.2.post9/janus_dtnaas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: janus-dtnaas
-Version: 0.2.post8
+Version: 0.2.post9
 Summary: Janus DTNaaS Controller
 Home-page: https://github.com/esnet/janus
 Author: Ezra Kissel
 Author-email: kissel@es.net
 Keywords: Janus Controller
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
```

### Comparing `janus-dtnaas-0.2.post8/janus_dtnaas.egg-info/SOURCES.txt` & `janus-dtnaas-0.2.post9/janus_dtnaas.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 janus/api/agent.py
 janus/api/ansible_job.py
 janus/api/controller.py
 janus/api/db.py
 janus/api/endpoints_api.py
 janus/api/models.py
 janus/api/portainer_docker.py
+janus/api/query.py
 janus/api/utils.py
 janus/api/validator.py
 janus/api/sys/__init__.py
 janus/api/sys/cpu.py
 janus/api/sys/disk.py
 janus/api/sys/mem.py
 janus/api/sys/net.py
```

### Comparing `janus-dtnaas-0.2.post8/setup.py` & `janus-dtnaas-0.2.post9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fh:
     requirements = fh.read()
 
 setup(
     name='janus-dtnaas',
-    version='0.2.post8',
+    version='0.2.post9',
     description='Janus DTNaaS Controller',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/esnet/janus',
     author='Ezra Kissel',
     author_email="kissel@es.net",
     include_package_data=True,
```

