# Comparing `tmp/car-connector-framework-3.0.2rc268.tar.gz` & `tmp/car-connector-framework-3.0.2rc269.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "car-connector-framework-3.0.2rc268.tar", last modified: Tue Apr 11 20:40:05 2023, max compression
+gzip compressed data, was "car-connector-framework-3.0.2rc269.tar", last modified: Wed Apr 12 17:29:26 2023, max compression
```

## Comparing `car-connector-framework-3.0.2rc268.tar` & `car-connector-framework-3.0.2rc269.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-11 20:40:05.351308 car-connector-framework-3.0.2rc268/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2023-04-11 20:39:50.000000 car-connector-framework-3.0.2rc268/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      553 2023-04-11 20:39:50.000000 car-connector-framework-3.0.2rc268/LICENSE.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     4180 2023-04-11 20:40:05.351308 car-connector-framework-3.0.2rc268/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3662 2023-04-11 20:39:50.000000 car-connector-framework-3.0.2rc268/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-11 20:40:05.347311 car-connector-framework-3.0.2rc268/car_connector_framework.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4180 2023-04-11 20:40:04.000000 car-connector-framework-3.0.2rc268/car_connector_framework.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      599 2023-04-11 20:40:05.000000 car-connector-framework-3.0.2rc268/car_connector_framework.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-11 20:40:04.000000 car-connector-framework-3.0.2rc268/car_connector_framework.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       73 2023-04-11 20:40:05.000000 car-connector-framework-3.0.2rc268/car_connector_framework.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2023-04-11 20:40:05.000000 car-connector-framework-3.0.2rc268/car_connector_framework.egg-info/top_level.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-11 20:40:05.351308 car-connector-framework-3.0.2rc268/car_framework/
--rw-rw-r--   0 travis    (2000) travis    (2000)       42 2023-04-11 20:39:50.000000 car-connector-framework-3.0.2rc268/car_framework/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7460 2023-04-11 20:39:50.000000 car-connector-framework-3.0.2rc268/car_framework/app.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1377 2023-04-11 20:39:50.000000 car-connector-framework-3.0.2rc268/car_framework/base_import.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14096 2023-04-11 20:39:50.000000 car-connector-framework-3.0.2rc268/car_framework/car_service.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4014 2023-04-11 20:39:50.000000 car-connector-framework-3.0.2rc268/car_framework/communicator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2516 2023-04-11 20:39:50.000000 car-connector-framework-3.0.2rc268/car_framework/context.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6797 2023-04-11 20:39:50.000000 car-connector-framework-3.0.2rc268/car_framework/data_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      694 2023-04-11 20:39:50.000000 car-connector-framework-3.0.2rc268/car_framework/extension.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1590 2023-04-11 20:39:50.000000 car-connector-framework-3.0.2rc268/car_framework/full_import.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1732 2023-04-11 20:39:50.000000 car-connector-framework-3.0.2rc268/car_framework/inc_import.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      182 2023-04-11 20:39:50.000000 car-connector-framework-3.0.2rc268/car_framework/server_access.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6003 2023-04-11 20:39:50.000000 car-connector-framework-3.0.2rc268/car_framework/util.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-04-11 20:40:05.351308 car-connector-framework-3.0.2rc268/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1387 2023-04-11 20:39:50.000000 car-connector-framework-3.0.2rc268/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-12 17:29:26.525720 car-connector-framework-3.0.2rc269/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2023-04-12 17:29:05.000000 car-connector-framework-3.0.2rc269/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      553 2023-04-12 17:29:05.000000 car-connector-framework-3.0.2rc269/LICENSE.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4180 2023-04-12 17:29:26.525720 car-connector-framework-3.0.2rc269/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3662 2023-04-12 17:29:05.000000 car-connector-framework-3.0.2rc269/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-12 17:29:26.497734 car-connector-framework-3.0.2rc269/car_connector_framework.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4180 2023-04-12 17:29:25.000000 car-connector-framework-3.0.2rc269/car_connector_framework.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      599 2023-04-12 17:29:26.000000 car-connector-framework-3.0.2rc269/car_connector_framework.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-12 17:29:25.000000 car-connector-framework-3.0.2rc269/car_connector_framework.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       73 2023-04-12 17:29:26.000000 car-connector-framework-3.0.2rc269/car_connector_framework.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       14 2023-04-12 17:29:26.000000 car-connector-framework-3.0.2rc269/car_connector_framework.egg-info/top_level.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-12 17:29:26.521722 car-connector-framework-3.0.2rc269/car_framework/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       42 2023-04-12 17:29:05.000000 car-connector-framework-3.0.2rc269/car_framework/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7597 2023-04-12 17:29:05.000000 car-connector-framework-3.0.2rc269/car_framework/app.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1377 2023-04-12 17:29:05.000000 car-connector-framework-3.0.2rc269/car_framework/base_import.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14141 2023-04-12 17:29:05.000000 car-connector-framework-3.0.2rc269/car_framework/car_service.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4043 2023-04-12 17:29:05.000000 car-connector-framework-3.0.2rc269/car_framework/communicator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2554 2023-04-12 17:29:05.000000 car-connector-framework-3.0.2rc269/car_framework/context.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6806 2023-04-12 17:29:05.000000 car-connector-framework-3.0.2rc269/car_framework/data_handler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      694 2023-04-12 17:29:05.000000 car-connector-framework-3.0.2rc269/car_framework/extension.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1590 2023-04-12 17:29:05.000000 car-connector-framework-3.0.2rc269/car_framework/full_import.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1732 2023-04-12 17:29:05.000000 car-connector-framework-3.0.2rc269/car_framework/inc_import.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      182 2023-04-12 17:29:05.000000 car-connector-framework-3.0.2rc269/car_framework/server_access.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6003 2023-04-12 17:29:05.000000 car-connector-framework-3.0.2rc269/car_framework/util.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-04-12 17:29:26.525720 car-connector-framework-3.0.2rc269/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1387 2023-04-12 17:29:05.000000 car-connector-framework-3.0.2rc269/setup.py
```

### Comparing `car-connector-framework-3.0.2rc268/LICENSE` & `car-connector-framework-3.0.2rc269/LICENSE`

 * *Files identical despite different names*

### Comparing `car-connector-framework-3.0.2rc268/LICENSE.txt` & `car-connector-framework-3.0.2rc269/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `car-connector-framework-3.0.2rc268/PKG-INFO` & `car-connector-framework-3.0.2rc269/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: car-connector-framework
-Version: 3.0.2rc268
+Version: 3.0.2rc269
 Summary: CAR service connector framework
 Home-page: https://github.com/IBM/cp4s-car-connector-framework
 Author: IBM
 Author-email: 
 License: Apache License 2.0
 Platform: Any
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `car-connector-framework-3.0.2rc268/README.md` & `car-connector-framework-3.0.2rc269/README.md`

 * *Files identical despite different names*

### Comparing `car-connector-framework-3.0.2rc268/car_connector_framework.egg-info/PKG-INFO` & `car-connector-framework-3.0.2rc269/car_connector_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: car-connector-framework
-Version: 3.0.2rc268
+Version: 3.0.2rc269
 Summary: CAR service connector framework
 Home-page: https://github.com/IBM/cp4s-car-connector-framework
 Author: IBM
 Author-email: 
 License: Apache License 2.0
 Platform: Any
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `car-connector-framework-3.0.2rc268/car_connector_framework.egg-info/SOURCES.txt` & `car-connector-framework-3.0.2rc269/car_connector_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `car-connector-framework-3.0.2rc268/car_framework/app.py` & `car-connector-framework-3.0.2rc269/car_framework/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,75 +3,75 @@
 from car_framework.context import Context, context
 from car_framework.util import ErrorCode, IncrementalImportNotPossible, RecoverableFailure, UnrecoverableFailure, DatasourceFailure, decrypt_secrets, objectview
 
 
 class BaseApp(object):
     def __init__(self, description):
         self.parser = argparse.ArgumentParser(description=description)
-        self.parser.add_argument('-car-service-url', dest='car_service_apikey_url', default=os.getenv('CAR_SERVICE_URL',None), type=str, required=False, help='URL of the CAR ingestion service if API key is used for authorization')
-        self.parser.add_argument('-car-service-key', dest='api_key', default=os.getenv('CAR_SERVICE_KEY',None), type=str, required=False, help='API key for CAR ingestion service')
-        self.parser.add_argument('-car-service-password', dest='api_password', default=os.getenv('CAR_SERVICE_PASSWORD',None), type=str, required=False, help='Password for CAR ingestion service')
+        self.parser.add_argument('-car-service-url', dest='CAR_SERVICE_URL', default=os.getenv('CAR_SERVICE_URL',None), type=str, required=False, help='URL of the CAR ingestion service if API key is used for authorization')
+        self.parser.add_argument('-car-service-key', dest='CAR_SERVICE_KEY', default=os.getenv('CAR_SERVICE_KEY',None), type=str, required=False, help='API key for CAR ingestion service')
+        self.parser.add_argument('-car-service-password', dest='CAR_SERVICE_PASSWORD', default=os.getenv('CAR_SERVICE_PASSWORD',None), type=str, required=False, help='Password for CAR ingestion service')
 
-        self.parser.add_argument('-car-service-url-for-token', dest='car_service_token_url', default=os.getenv('CAR_SERVICE_URL_FOR_AUTHTOKEN',None), type=str, required=False, help='URL of the CAR ingestion service if Auth token is used for authorization')
-        self.parser.add_argument('-car-service-token', dest='api_token', default=os.getenv('CAR_SERVICE_AUTHTOKEN',None), type=str, required=False, help='Auth token for CAR ingestion service')
+        self.parser.add_argument('-car-service-url-for-token', dest='CAR_SERVICE_URL_FOR_AUTHTOKEN', default=os.getenv('CAR_SERVICE_URL_FOR_AUTHTOKEN',None), type=str, required=False, help='URL of the CAR ingestion service if Auth token is used for authorization')
+        self.parser.add_argument('-car-service-token', dest='CAR_SERVICE_AUTHTOKEN', default=os.getenv('CAR_SERVICE_AUTHTOKEN',None), type=str, required=False, help='Auth token for CAR ingestion service')
 
         # source id to uniquely identify each data source
-        self.parser.add_argument('-source', dest='source', default=os.getenv('CONNECTION_NAME',None), type=str, required=False, help='Unique source id for the data source')
-        self.parser.add_argument('-name', dest='connector_name', default=os.getenv('CONNECTOR_NAME', None), type=str, required=False, help='Name of the connector')
-        self.parser.add_argument('-version', dest='version', default=os.getenv('CONNECTOR_VERSION', None), type=str, required=False, help='Connector version number')
+        self.parser.add_argument('-source', dest='CONNECTION_NAME', default=os.getenv('CONNECTION_NAME',None), type=str, required=False, help='Unique source id for the data source')
+        self.parser.add_argument('-name', dest='CONNECTOR_NAME', default=os.getenv('CONNECTOR_NAME', None), type=str, required=False, help='Name of the connector')
+        self.parser.add_argument('-version', dest='CONNECTOR_VERSION', default=os.getenv('CONNECTOR_VERSION', None), type=str, required=False, help='Connector version number')
 
         self.parser.add_argument('-d', dest='debug', action='store_true', default=os.getenv('DEBUG', False), help='Enables DEBUG level logging')
-        self.parser.add_argument('-connection-test', dest='connection_test', type=bool, default=os.getenv('DATASOURCE_CONNECTION_TEST', False), help='Only perform datasource connection test and exit, if this parameter is present with any value.')
+        self.parser.add_argument('-connection-test', dest='DATASOURCE_CONNECTION_TEST', type=bool, default=os.getenv('DATASOURCE_CONNECTION_TEST', False), help='Only perform datasource connection test and exit, if this parameter is present with any value.')
         self.parser.add_argument('-export-data-dir', dest='export_data_dir', default='/tmp/car_temp_export_data', help='Export data directory path, deafualt /tmp/car_temp_export_data')
         self.parser.add_argument('-keep-export-data-dir', dest='keep_export_data_dir', action='store_true', help='True for not removing export_data directory after complete, default false')
         self.parser.add_argument('-export-data-page-size', dest='export_data_page_size', type=int, default=2000, help='File export_data dump page size, default 2000')
 
 
     def setup(self):
 
         file_secrets = decrypt_secrets()
         args = vars(self.parser.parse_args())
         if(file_secrets):
             args.update(file_secrets)
         self.args = objectview(args)
 
-        if not self.args.api_token:
-            if not self.args.api_key or not self.args.api_password:
+        if not self.args.CAR_SERVICE_AUTHTOKEN:
+            if not self.args.CAR_SERVICE_KEY or not self.args.CAR_SERVICE_PASSWORD:
                 self.parser.print_usage(sys.stderr)
                 sys.stderr.write('Either -car-service-token or -car-service-key and -car-service-password arguments are required.')
                 sys.exit(ErrorCode.CONNECTOR_RUNTIME_INVALID_PARAMETER.value)
 
-        if not self.args.car_service_apikey_url and not self.args.car_service_token_url:
+        if not self.args.CAR_SERVICE_URL and not self.args.CAR_SERVICE_URL_FOR_AUTHTOKEN:
             self.parser.print_usage(sys.stderr)
             sys.stderr.write('Either -car-service-url or -car-service-url-for-token is required.')
             sys.exit(ErrorCode.CONNECTOR_RUNTIME_INVALID_PARAMETER.value)
 
-        if self.args.car_service_apikey_url:
-            if not self.args.api_key or not self.args.api_password:
+        if self.args.CAR_SERVICE_URL:
+            if not self.args.CAR_SERVICE_KEY or not self.args.CAR_SERVICE_PASSWORD:
                 self.parser.print_usage(sys.stderr)
                 sys.stderr.write('If -car-service-url is provided then -car-service-key and -car-service-password arguments are required.')
                 sys.exit(ErrorCode.CONNECTOR_RUNTIME_INVALID_PARAMETER.value)
 
-        if self.args.car_service_token_url:
-            if not self.args.api_token:
+        if self.args.CAR_SERVICE_URL_FOR_AUTHTOKEN:
+            if not self.args.CAR_SERVICE_AUTHTOKEN:
                 self.parser.print_usage(sys.stderr)
                 sys.stderr.write('If -car-service-url-for-token is provided then -car-service-token argument is required.')
                 sys.exit(ErrorCode.CONNECTOR_RUNTIME_INVALID_PARAMETER.value)
 
-        if not self.args.source:
+        if not self.args.CONNECTION_NAME:
             self.parser.print_usage(sys.stderr)
             sys.stderr.write('Missing required -source argument.')
             sys.exit(ErrorCode.CONNECTOR_RUNTIME_INVALID_PARAMETER.value)
 
         Context(self.args)
 
 
     def run(self):
         try:
-            if self.args.connection_test:
+            if self.args.DATASOURCE_CONNECTION_TEST:
                 if hasattr(context(), 'asset_server') and hasattr(context().asset_server, 'test_connection') :
                     context().logger.info('Testing the datasource connection ... ')
                     code = context().asset_server.test_connection()
                     if code == 0:
                         context().logger.info('Testing the datasource connection was successful.')
                     else:
                         context().logger.error('Testing the datasource connection failed with code ' + str(code))
```

### Comparing `car-connector-framework-3.0.2rc268/car_framework/base_import.py` & `car-connector-framework-3.0.2rc269/car_framework/base_import.py`

 * *Files identical despite different names*

### Comparing `car-connector-framework-3.0.2rc268/car_framework/car_service.py` & `car-connector-framework-3.0.2rc269/car_framework/car_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,25 +27,25 @@
 class CarService(object):
 
     def __init__(self, communicator):
         self.communicator = communicator
 
 
     def get_model_state_id(self):
-        url = 'source/%s' % (urllib.parse.quote_plus(context().args.source))
+        url = 'source/%s' % (urllib.parse.quote_plus(context().args.CONNECTION_NAME))
         resp = self.communicator.get(url)
         if resp.status_code != 200:
             return None
         json_data = resp.json()
         return json_data and json_data.get(MODEL_STATE_ID)
 
 
     def save_model_state_id(self, new_model_state_id):
         data = json.dumps({ MODEL_STATE_ID: new_model_state_id })
-        resp = self.communicator.patch(SOURCE_RESOURCE, data=data, params={ 'key': context().args.source })
+        resp = self.communicator.patch(SOURCE_RESOURCE, data=data, params={ 'key': context().args.CONNECTION_NAME })
         if resp.status_code != 200:
             raise Exception('Error when trying to save a save point: %d' % resp.status_code)
 
 
     def reset_model_state_id(self):
         self.save_model_state_id('')
 
@@ -142,15 +142,15 @@
             resource_key = 'keys'
         else:
             resource_key = 'external_ids'
 
         ids_list = self.compose_paginated_list(ids)
         for page in ids_list:
 
-            url = 'source/%s/%s?%s=%s' % (context().args.source, resource, resource_key, ','.join(ids_list[page]))
+            url = 'source/%s/%s?%s=%s' % (context().args.CONNECTION_NAME, resource, resource_key, ','.join(ids_list[page]))
             r = self.communicator.delete(url)
 
             if r.status_code == 200:
                 continue
             elif recoverable_failure_status_code(r.status_code):
                 raise RecoverableFailure('Getting the following status code when accessing ISC CAR service: %d' % r.status_code)
             else:
@@ -280,23 +280,23 @@
                 if status == 'ERROR':
                     return CarDbStatus.FAILURE
             else:
                 return CarDbStatus.FAILURE
 
 
     def enter_full_import_in_progress_state(self):
-        endpoint = 'source/%s%s' % (context().args.source, FULL_IMPORT_IN_PROGRESS_ENDPOINT)
+        endpoint = 'source/%s%s' % (context().args.CONNECTION_NAME, FULL_IMPORT_IN_PROGRESS_ENDPOINT)
         r = self.communicator.post(endpoint)
         job_id = self._get_job_id_from_response(r)
         self.wait_until_done(job_id)
         return r.status_code
 
 
     def exit_full_import_in_progress_state(self):
-        endpoint = 'source/%s%s' % (context().args.source, FULL_IMPORT_IN_PROGRESS_ENDPOINT)
+        endpoint = 'source/%s%s' % (context().args.CONNECTION_NAME, FULL_IMPORT_IN_PROGRESS_ENDPOINT)
         r = self.communicator.delete(endpoint)
         job_id = self._get_job_id_from_response(r)
         self.wait_until_done(job_id)
         return r.status_code
 
 
     def compose_paginated_list(self, ids):
```

### Comparing `car-connector-framework-3.0.2rc268/car_framework/communicator.py` & `car-connector-framework-3.0.2rc269/car_framework/communicator.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,22 +30,22 @@
         context().logger.info('Retry after %s sec invoked with url %s' % (backoff_time, url))
 
 
 class Communicator(object):
     def __init__(self):
         self.headers = {'Accept' : 'application/json', 'Content-Type' : 'application/json'}
 
-        auth_token = context().args.api_token
+        auth_token = context().args.CAR_SERVICE_AUTHTOKEN
         if auth_token:
             self.headers['Authorization'] = 'car-token ' + auth_token
-            self.base_url = context().args.car_service_token_url
+            self.base_url = context().args.CAR_SERVICE_URL_FOR_AUTHTOKEN
             self.basic_auth = None
         else:
-            self.basic_auth = HTTPBasicAuth(context().args.api_key, context().args.api_password)
-            self.base_url = context().args.car_service_apikey_url
+            self.basic_auth = HTTPBasicAuth(context().args.CAR_SERVICE_KEY, context().args.CAR_SERVICE_PASSWORD)
+            self.base_url = context().args.CAR_SERVICE_URL
 
         if not self.base_url.endswith('/'):
             self.base_url = self.base_url + '/'
 
         retry_strategy = CallbackRetry(
             total=3,
             backoff_factor=10,
```

### Comparing `car-connector-framework-3.0.2rc268/car_framework/context.py` & `car-connector-framework-3.0.2rc269/car_framework/context.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,22 +7,22 @@
         # use inherited constructor
         super(CustomJsonFormatter, self).add_fields(log_record, record, message_dict)
 
         if not log_record.get('ibm_datetime'):
             now = datetime.utcnow().strftime('%Y-%m-%dT%H:%M:%S.%fZ')
             log_record['ibm_datetime'] = now
         
-        if not log_record.get('connector') and context().args.connector_name:
-            log_record['connector'] = context().args.connector_name
+        if not log_record.get('connector') and context().args.CONNECTOR_NAME:
+            log_record['connector'] = context().args.CONNECTOR_NAME
         
-        if not log_record.get('source') and context().args.source:
-            log_record['source'] = context().args.source
+        if not log_record.get('source') and context().args.CONNECTION_NAME:
+            log_record['source'] = context().args.CONNECTION_NAME
         
-        if not log_record.get('version') and context().args.version:
-            log_record['version'] = context().args.version
+        if not log_record.get('version') and context().args.CONNECTOR_VERSION:
+            log_record['version'] = context().args.CONNECTOR_VERSION
 
         # assign values to log_record
         log_record['level'] = log_record['level'].lower() if log_record.get('level') else record.levelname
         log_record['message'] = log_record['message'] if log_record.get('log') else record.message
         log_record['label'] = log_record['label'] if log_record.get('type') else record.name
 
 def create_logger(debug = False):
@@ -39,28 +39,28 @@
 
 def read_config(file_path, args):
     import json 
 
     try:
         with open(file_path) as f:
             config_file = json.load(f)
-            args.connector_name = config_file.get('connection', {}).get('type', {}).get('displayName', {})
+            args.CONNECTOR_NAME = config_file.get('connection', {}).get('type', {}).get('displayName', {})
     except Exception:
-        args.connector_name = ""
+        args.CONNECTOR_NAME = ""
 
 
 class Context(object):
     def __init__(self, args):
         global global_context
         global_context = self
 
         from car_framework.car_service import CarService
         from car_framework.communicator import Communicator
         self.args = args
-        if not args.connector_name:
+        if not args.CONNECTOR_NAME:
             read_config('configurations/config.json', self.args)
         self.logger = create_logger(args.debug)
         self.car_service = CarService(Communicator())
         
 
 global_context = None
 def context():
```

### Comparing `car-connector-framework-3.0.2rc268/car_framework/data_handler.py` & `car-connector-framework-3.0.2rc269/car_framework/data_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         if not keys:
             keys = []
             self.edge_keys[name] = keys
 
         key = '#'.join(str(x) for x in object.values())
         if not key in self.edge_keys[name]:
             object['report'] = self.report['_key']
-            object['source'] = context().args.source
+            object['source'] = context().args.CONNECTION_NAME
             object['active'] = True
             object['timestamp'] = self.report['timestamp']
             objects.append(object)
             self.edge_keys[name].append(key)
 
         # dump edges to file to free memory
         if len(self.edges[name]) >= context().args.export_data_page_size:
```

### Comparing `car-connector-framework-3.0.2rc268/car_framework/extension.py` & `car-connector-framework-3.0.2rc269/car_framework/extension.py`

 * *Files identical despite different names*

### Comparing `car-connector-framework-3.0.2rc268/car_framework/full_import.py` & `car-connector-framework-3.0.2rc269/car_framework/full_import.py`

 * *Files identical despite different names*

### Comparing `car-connector-framework-3.0.2rc268/car_framework/inc_import.py` & `car-connector-framework-3.0.2rc269/car_framework/inc_import.py`

 * *Files identical despite different names*

### Comparing `car-connector-framework-3.0.2rc268/car_framework/util.py` & `car-connector-framework-3.0.2rc269/car_framework/util.py`

 * *Files identical despite different names*

### Comparing `car-connector-framework-3.0.2rc268/setup.py` & `car-connector-framework-3.0.2rc269/setup.py`

 * *Files identical despite different names*

