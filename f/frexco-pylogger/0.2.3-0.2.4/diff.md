# Comparing `tmp/frexco_pylogger-0.2.3.tar.gz` & `tmp/frexco_pylogger-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frexco_pylogger-0.2.3.tar", last modified: Wed Feb  1 21:19:55 2023, max compression
+gzip compressed data, was "frexco_pylogger-0.2.4.tar", last modified: Wed Apr 12 15:21:17 2023, max compression
```

## Comparing `frexco_pylogger-0.2.3.tar` & `frexco_pylogger-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 victor    (1000) wheel      (998)        0 2023-02-01 21:19:55.611421 frexco_pylogger-0.2.3/
--rw-r--r--   0 victor    (1000) wheel      (998)     3052 2023-02-01 21:19:55.611421 frexco_pylogger-0.2.3/PKG-INFO
--rw-r--r--   0 victor    (1000) wheel      (998)     2612 2023-02-01 17:10:05.000000 frexco_pylogger-0.2.3/README.md
-drwxr-xr-x   0 victor    (1000) wheel      (998)        0 2023-02-01 21:19:55.608421 frexco_pylogger-0.2.3/frexco_pylogger/
--rw-r--r--   0 victor    (1000) wheel      (998)        0 2022-12-23 15:30:37.000000 frexco_pylogger-0.2.3/frexco_pylogger/__init__.py
--rw-r--r--   0 victor    (1000) wheel      (998)     6674 2023-02-01 21:19:16.000000 frexco_pylogger-0.2.3/frexco_pylogger/functions.py
-drwxr-xr-x   0 victor    (1000) wheel      (998)        0 2023-02-01 21:19:55.611421 frexco_pylogger-0.2.3/frexco_pylogger.egg-info/
--rw-r--r--   0 victor    (1000) wheel      (998)     3052 2023-02-01 21:19:55.000000 frexco_pylogger-0.2.3/frexco_pylogger.egg-info/PKG-INFO
--rw-r--r--   0 victor    (1000) wheel      (998)      269 2023-02-01 21:19:55.000000 frexco_pylogger-0.2.3/frexco_pylogger.egg-info/SOURCES.txt
--rw-r--r--   0 victor    (1000) wheel      (998)        1 2023-02-01 21:19:55.000000 frexco_pylogger-0.2.3/frexco_pylogger.egg-info/dependency_links.txt
--rw-r--r--   0 victor    (1000) wheel      (998)        9 2023-02-01 21:19:55.000000 frexco_pylogger-0.2.3/frexco_pylogger.egg-info/requires.txt
--rw-r--r--   0 victor    (1000) wheel      (998)       16 2023-02-01 21:19:55.000000 frexco_pylogger-0.2.3/frexco_pylogger.egg-info/top_level.txt
--rw-r--r--   0 victor    (1000) wheel      (998)       38 2023-02-01 21:19:55.611421 frexco_pylogger-0.2.3/setup.cfg
--rw-r--r--   0 victor    (1000) wheel      (998)      707 2023-02-01 21:19:52.000000 frexco_pylogger-0.2.3/setup.py
+drwxr-xr-x   0 victor    (1000) wheel      (998)        0 2023-04-12 15:21:17.370006 frexco_pylogger-0.2.4/
+-rw-r--r--   0 victor    (1000) wheel      (998)     3015 2023-04-12 15:21:17.370006 frexco_pylogger-0.2.4/PKG-INFO
+-rw-r--r--   0 victor    (1000) wheel      (998)     2612 2023-04-12 02:13:59.000000 frexco_pylogger-0.2.4/README.md
+drwxr-xr-x   0 victor    (1000) wheel      (998)        0 2023-04-12 15:21:17.369006 frexco_pylogger-0.2.4/frexco_pylogger/
+-rw-r--r--   0 victor    (1000) wheel      (998)        0 2023-04-12 02:13:59.000000 frexco_pylogger-0.2.4/frexco_pylogger/__init__.py
+-rw-r--r--   0 victor    (1000) wheel      (998)     6747 2023-04-12 02:14:49.000000 frexco_pylogger-0.2.4/frexco_pylogger/functions.py
+drwxr-xr-x   0 victor    (1000) wheel      (998)        0 2023-04-12 15:21:17.370006 frexco_pylogger-0.2.4/frexco_pylogger.egg-info/
+-rw-r--r--   0 victor    (1000) wheel      (998)     3015 2023-04-12 15:21:17.000000 frexco_pylogger-0.2.4/frexco_pylogger.egg-info/PKG-INFO
+-rw-r--r--   0 victor    (1000) wheel      (998)      269 2023-04-12 15:21:17.000000 frexco_pylogger-0.2.4/frexco_pylogger.egg-info/SOURCES.txt
+-rw-r--r--   0 victor    (1000) wheel      (998)        1 2023-04-12 15:21:17.000000 frexco_pylogger-0.2.4/frexco_pylogger.egg-info/dependency_links.txt
+-rw-r--r--   0 victor    (1000) wheel      (998)        9 2023-04-12 15:21:17.000000 frexco_pylogger-0.2.4/frexco_pylogger.egg-info/requires.txt
+-rw-r--r--   0 victor    (1000) wheel      (998)       16 2023-04-12 15:21:17.000000 frexco_pylogger-0.2.4/frexco_pylogger.egg-info/top_level.txt
+-rw-r--r--   0 victor    (1000) wheel      (998)       38 2023-04-12 15:21:17.370006 frexco_pylogger-0.2.4/setup.cfg
+-rw-r--r--   0 victor    (1000) wheel      (998)      707 2023-04-12 15:19:47.000000 frexco_pylogger-0.2.4/setup.py
```

### Comparing `frexco_pylogger-0.2.3/PKG-INFO` & `frexco_pylogger-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: frexco_pylogger
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python library for logging with colors and http status code.
 Home-page: https://github.com/frexco-digital/frexco-pylogger.git
-License: UNKNOWN
 Keywords: logs logging logger
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 
 # **Frexco PyLogger**
 
@@ -107,9 +105,7 @@
 
 logger.error(message="Uma messagem de error qualquer",
             status_code=500, data={"name": "Um error"}) # Enviar alerta
 
 logger.error(message="Uma messagem de error qualquer repetida",
             status_code=500, data={"name": "Um error"}, alert=False) # Não enviar alerta
 ```
-
-
```

### Comparing `frexco_pylogger-0.2.3/README.md` & `frexco_pylogger-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `frexco_pylogger-0.2.3/frexco_pylogger/functions.py` & `frexco_pylogger-0.2.4/frexco_pylogger/functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -135,47 +135,48 @@
         if args:
             self.logger.http(message, args) # type: ignore
         else:
             self.logger.http(message) # type: ignore
 
     def vault(self):
         vault_host = os.environ.get("VAULT_HOST")
+        vault_host = vault_host if vault_host.endswith("/") else vault_host + "/" # type: ignore
         vault_token = os.environ.get("VAULT_TOKEN")
         headers = {"X-Vault-Token": vault_token}
 
         try:
-            response = requests.get(url=f"{vault_host}/v1/prd/data/alert-logger", headers=headers) # type: ignore
+            response = requests.get(url=f"{vault_host}v1/prd/data/alert-logger", headers=headers) # type: ignore
             response = response.json()["data"]["data"]
             self.credentials = response
             self.alertmanager_host = response["alertmanager_host"]
         except Exception as error:
             self.warning(message="Vault Error.", data=error)
 
     def send_alert(self, message: str, status_code: Optional[int] = None, data=None):
         if self.alertmanager_host == "": return
 
         args = self.check_params(status_code, data)
         url = self.alertmanager_host
-        group = self.group.lower()
+
         now = datetime.now(timezone.utc)
         startsAt = datetime.now().strftime("%Y-%m-%dT%H:%M:%S.%fZ")
         diff = timedelta(minutes=5)
         endsAt = (now + diff).strftime("%Y-%m-%dT%H:%M:%S.%fZ")
 
         status = args.get("status") if args.get("status") else ""
         error = json.dumps(args.get('data')) if "data" in args else ""
-        dashboard_link = self.credentials[group] if group in self.credentials else "" # type: ignore
+        dashboard_link = self.credentials[self.group] if self.group in self.credentials else "" # type: ignore
         app_name = self.appname.replace("_"," ").replace("-", " ")
 
         data = [{
                 "startsAt": startsAt,
                 "endsAt": endsAt,
                 "labels": {
                     "alertname": app_name,
-                    "logs": group,
+                    "logs": "test",
                     "status": "error_log",
                     "url": dashboard_link,
                     "message": message,
                     "error": error,
                     "status_code": str(status),
                 },
             }]
```

### Comparing `frexco_pylogger-0.2.3/frexco_pylogger.egg-info/PKG-INFO` & `frexco_pylogger-0.2.4/frexco_pylogger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: frexco-pylogger
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python library for logging with colors and http status code.
 Home-page: https://github.com/frexco-digital/frexco-pylogger.git
-License: UNKNOWN
 Keywords: logs logging logger
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 
 # **Frexco PyLogger**
 
@@ -107,9 +105,7 @@
 
 logger.error(message="Uma messagem de error qualquer",
             status_code=500, data={"name": "Um error"}) # Enviar alerta
 
 logger.error(message="Uma messagem de error qualquer repetida",
             status_code=500, data={"name": "Um error"}, alert=False) # Não enviar alerta
 ```
-
-
```

### Comparing `frexco_pylogger-0.2.3/setup.py` & `frexco_pylogger-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='frexco_pylogger',
     packages=find_packages(include=['frexco_pylogger']),
-    version='0.2.3',
+    version='0.2.4',
     description='Python library for logging with colors and http status code.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/frexco-digital/frexco-pylogger.git',
     install_requires=["requests"],
     classifiers=CLASSIFIERS,
     keywords='logs logging logger',
```

