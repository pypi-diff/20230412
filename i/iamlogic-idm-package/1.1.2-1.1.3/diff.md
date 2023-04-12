# Comparing `tmp/iamlogic_idm_package-1.1.2.tar.gz` & `tmp/iamlogic_idm_package-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamlogic_idm_package-1.1.2.tar", last modified: Wed Apr  5 19:44:16 2023, max compression
+gzip compressed data, was "iamlogic_idm_package-1.1.3.tar", last modified: Wed Apr 12 17:32:05 2023, max compression
```

## Comparing `iamlogic_idm_package-1.1.2.tar` & `iamlogic_idm_package-1.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 19:44:16.691003 iamlogic_idm_package-1.1.2/
--rw-rw-rw-   0        0        0      453 2023-04-05 19:44:16.687999 iamlogic_idm_package-1.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-05 19:44:16.661244 iamlogic_idm_package-1.1.2/iamlogic_idm_package.egg-info/
--rw-rw-rw-   0        0        0      453 2023-04-05 19:44:16.000000 iamlogic_idm_package-1.1.2/iamlogic_idm_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-04-05 19:44:16.000000 iamlogic_idm_package-1.1.2/iamlogic_idm_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 19:44:16.000000 iamlogic_idm_package-1.1.2/iamlogic_idm_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-05 19:44:16.000000 iamlogic_idm_package-1.1.2/iamlogic_idm_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-05 19:44:16.000000 iamlogic_idm_package-1.1.2/iamlogic_idm_package.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-05 19:44:16.686000 iamlogic_idm_package-1.1.2/idm_operation/
--rw-rw-rw-   0        0        0     8837 2023-04-05 19:42:58.000000 iamlogic_idm_package-1.1.2/idm_operation/IDM_Operation.py
--rw-rw-rw-   0        0        0        0 2023-03-31 04:53:08.000000 iamlogic_idm_package-1.1.2/idm_operation/__init__.py
--rw-rw-rw-   0        0        0       42 2023-04-05 19:44:16.691003 iamlogic_idm_package-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      666 2023-04-05 19:43:06.000000 iamlogic_idm_package-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 17:32:05.719197 iamlogic_idm_package-1.1.3/
+-rw-rw-rw-   0        0        0      444 2023-04-12 17:32:05.717200 iamlogic_idm_package-1.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-12 17:32:05.688810 iamlogic_idm_package-1.1.3/iamlogic_idm_package.egg-info/
+-rw-rw-rw-   0        0        0      444 2023-04-12 17:32:05.000000 iamlogic_idm_package-1.1.3/iamlogic_idm_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-04-12 17:32:05.000000 iamlogic_idm_package-1.1.3/iamlogic_idm_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 17:32:05.000000 iamlogic_idm_package-1.1.3/iamlogic_idm_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-12 17:32:05.000000 iamlogic_idm_package-1.1.3/iamlogic_idm_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-12 17:32:05.000000 iamlogic_idm_package-1.1.3/iamlogic_idm_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 17:32:05.714572 iamlogic_idm_package-1.1.3/idm_operation/
+-rw-rw-rw-   0        0        0     9494 2023-04-12 17:31:38.000000 iamlogic_idm_package-1.1.3/idm_operation/IDM_Operation.py
+-rw-rw-rw-   0        0        0        0 2023-03-31 04:53:08.000000 iamlogic_idm_package-1.1.3/idm_operation/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-04-12 17:32:05.720198 iamlogic_idm_package-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      654 2023-04-12 17:31:28.000000 iamlogic_idm_package-1.1.3/setup.py
```

### Comparing `iamlogic_idm_package-1.1.2/idm_operation/IDM_Operation.py` & `iamlogic_idm_package-1.1.3/idm_operation/IDM_Operation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from IDMConnector import ConnectorClass
-import time, json, logging, mysql.connector
+import time, json, logging, mysql.connector, traceback
 from datetime import timedelta
 
 logger = logging.getLogger()
 
 #######################
 #  Initialize_IDM_DB  #
 #######################
@@ -82,15 +82,15 @@
             except Exception as e:
                 if attempt < max_attempt:
                     time.sleep(delay)
                     logger.info(f"retry_attempt() func: exception attempt-{i}")
                     logger.error(str(e))
         return None
 
-    # sync method used to perform create, update, delete operations.
+    # sync method used to perform create, update, delete, ignore operations.
     # Update success/exception for each reconcilation.
     # When the connection is disconnected from the server side during mid-operation, retry the connection.
     # Calculating the reconcilation time is how long it takes to complete all the tasks.
     # Finally return the reconcilation total duration and sync status.    
     def sync(self, mappingid, config_data, log_level, db_config, secret_key) -> dict:                
         logger.setLevel(log_level)
         logger.debug("inside:ConnectorClass() , sync() func:")
@@ -123,37 +123,44 @@
                         with Initialize_IDM_DB(db_config) as dbObj:
                             dbObj.update_reconciliation_statistics(mappingid, json_update_data, obj['actions'], msg)
                     elif(obj['actions'] == "delete"):
                         json_delete_data = obj['reconcile_data']
                         logger.debug("inside:ConnectorClass() , sync() func elif delete try:")
                         deleteOp_response = self.idm_operation_obj.delete(json.loads(obj['reconcile_data']))
                         with Initialize_IDM_DB(db_config) as dbObj:
-                            dbObj.update_reconciliation_statistics(mappingid, json_delete_data, obj['actions'], msg)
+                            dbObj.update_reconciliation_statistics(mappingid, json_delete_data, obj['actions'], msg)                  
+                    elif(obj['actions'] == "ignore"):
+                        json_ignore_data = obj['reconcile_data']
+                        logger.debug("inside:ConnectorClass() , sync() func elif ignore try:")
+                        ignore_msg = "No operation can be performed which is ignored by behaviour" 
+                        with Initialize_IDM_DB(db_config) as dbObj:
+                            dbObj.update_reconciliation_statistics(mappingid, json_ignore_data, obj['actions'], ignore_msg)
                     processed_operation.add(obj['id'])
                     current_obj_id += 1
                 except Exception as e:
                     logger.debug("inside:ConnectorClass() , sync() except Exception:")
-                    logger.warning(str(e))
+                    _exception = traceback.format_exc()
+                    logger.warning(_exception)
                     with Initialize_IDM_DB(db_config) as dbObj:
-                        dbObj.update_reconciliation_statistics(mappingid, obj['reconcile_data'], obj['actions'], str(e))
+                        dbObj.update_reconciliation_statistics(mappingid, obj['reconcile_data'], obj['actions'], _exception)
                     try:
                         # Check the connection if any exception occurs
                         conn_test_res = self.idm_operation_obj.testConfig(config_data)
                         if conn_test_res["status"]:
                             logger.debug(f"connection is available,try response_obj_operation:{obj['id']}")
                             self.idm_operation_obj.__init__(config_data)
                             current_obj_id += 1
                     except Exception as e:
-                        # if testConfig() is false try again
+                        # if testConfig() is false try again                        
                         logger.info(f"Re-attempt before check, response_obj_operation:{obj['id']}")
                         conn_attempt_resp = self.retry_attempt(config_param=config_data, max_attempt=int(config_data['retry']))
                         if(conn_attempt_resp and conn_attempt_resp is not None):
                             logger.info(f"Re-attempt if conn true, response_obj_operation:{obj['id']}")
                             current_obj_id -= 1
                         else:
                             logger.info(f"Many re-attempt connectivity failed, response_obj_operation:{obj['id']}")
                             return {"error": "Please check the target application server connectivity. Many attempt could not connected!."}
 
         end_time = time.time()
         duration = end_time - start_time
         duration_str = str(timedelta(seconds=duration))
-        return {"total_duration":duration_str, "status": "sync done!"}
+        return {"total_duration":duration_str, "status": "Reconcilation Sync Completed!"}
```

### Comparing `iamlogic_idm_package-1.1.2/setup.py` & `iamlogic_idm_package-1.1.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='iamlogic_idm_package',
-    version='1.1.2',
-    description='IDM package',
-    author='Prabhu S',
+    version='1.1.3',
+    description='IAMLOGIC IDM package',   
     author_email='prabhu@iamlogic.com',
     packages=find_packages(),
     install_requires=[
         'requests',
         'cryptography',
         'sqlalchemy',
         'mysql-connector-python',
```

