# Comparing `tmp/pastell-admin-0.1.15.tar.gz` & `tmp/pastell-admin-0.1.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pastell-admin-0.1.15.tar", last modified: Mon Mar 27 16:47:15 2023, max compression
+gzip compressed data, was "pastell-admin-0.1.16.tar", last modified: Wed Apr 12 14:49:28 2023, max compression
```

## Comparing `pastell-admin-0.1.15.tar` & `pastell-admin-0.1.16.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 16:47:15.526413 pastell-admin-0.1.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-27 16:47:06.000000 pastell-admin-0.1.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11405 2023-03-27 16:47:15.526413 pastell-admin-0.1.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-03-27 16:47:06.000000 pastell-admin-0.1.15/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-03-27 16:47:06.000000 pastell-admin-0.1.15/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 16:47:15.526413 pastell-admin-0.1.15/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 16:47:15.522413 pastell-admin-0.1.15/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 16:47:15.522413 pastell-admin-0.1.15/src/pastell_admin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11405 2023-03-27 16:47:15.000000 pastell-admin-0.1.15/src/pastell_admin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-03-27 16:47:15.000000 pastell-admin-0.1.15/src/pastell_admin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 16:47:15.000000 pastell-admin-0.1.15/src/pastell_admin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-03-27 16:47:15.000000 pastell-admin-0.1.15/src/pastell_admin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-27 16:47:15.000000 pastell-admin-0.1.15/src/pastell_admin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-27 16:47:15.000000 pastell-admin-0.1.15/src/pastell_admin.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 16:47:15.526413 pastell-admin-0.1.15/src/pastelladmin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 16:47:06.000000 pastell-admin-0.1.15/src/pastelladmin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 16:47:15.526413 pastell-admin-0.1.15/src/pastelladmin/api/
--rw-r--r--   0 runner    (1001) docker     (123)    19631 2023-03-27 16:47:06.000000 pastell-admin-0.1.15/src/pastelladmin/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-03-27 16:47:06.000000 pastell-admin-0.1.15/src/pastelladmin/delete_any.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2181 2023-03-27 16:47:06.000000 pastell-admin-0.1.15/src/pastelladmin/pastell_associations.py
--rw-r--r--   0 runner    (1001) docker     (123)    14568 2023-03-27 16:47:06.000000 pastell-admin-0.1.15/src/pastelladmin/pastell_connector.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1990 2023-03-27 16:47:06.000000 pastell-admin-0.1.15/src/pastelladmin/pastell_connector_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-03-27 16:47:06.000000 pastell-admin-0.1.15/src/pastelladmin/pastell_docs_delete_from_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-03-27 16:47:06.000000 pastell-admin-0.1.15/src/pastelladmin/pastell_find.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3213 2023-03-27 16:47:06.000000 pastell-admin-0.1.15/src/pastelladmin/pastell_matrice_roles.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2540 2023-03-27 16:47:06.000000 pastell-admin-0.1.15/src/pastelladmin/pastell_org.py
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-03-27 16:47:06.000000 pastell-admin-0.1.15/src/pastelladmin/pastell_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 16:47:15.526413 pastell-admin-0.1.15/src/pastelladmin/shared/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-03-27 16:47:06.000000 pastell-admin-0.1.15/src/pastelladmin/shared/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:49:28.608570 pastell-admin-0.1.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-12 14:49:14.000000 pastell-admin-0.1.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11405 2023-04-12 14:49:28.608570 pastell-admin-0.1.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-04-12 14:49:14.000000 pastell-admin-0.1.16/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-12 14:49:14.000000 pastell-admin-0.1.16/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 14:49:28.608570 pastell-admin-0.1.16/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:49:28.604570 pastell-admin-0.1.16/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:49:28.608570 pastell-admin-0.1.16/src/pastell_admin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11405 2023-04-12 14:49:28.000000 pastell-admin-0.1.16/src/pastell_admin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-12 14:49:28.000000 pastell-admin-0.1.16/src/pastell_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:49:28.000000 pastell-admin-0.1.16/src/pastell_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-12 14:49:28.000000 pastell-admin-0.1.16/src/pastell_admin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-12 14:49:28.000000 pastell-admin-0.1.16/src/pastell_admin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-12 14:49:28.000000 pastell-admin-0.1.16/src/pastell_admin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:49:28.608570 pastell-admin-0.1.16/src/pastelladmin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:49:14.000000 pastell-admin-0.1.16/src/pastelladmin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:49:28.608570 pastell-admin-0.1.16/src/pastelladmin/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    19924 2023-04-12 14:49:14.000000 pastell-admin-0.1.16/src/pastelladmin/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-12 14:49:14.000000 pastell-admin-0.1.16/src/pastelladmin/delete_any.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2181 2023-04-12 14:49:14.000000 pastell-admin-0.1.16/src/pastelladmin/pastell_associations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-04-12 14:49:14.000000 pastell-admin-0.1.16/src/pastelladmin/pastell_connector.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1990 2023-04-12 14:49:14.000000 pastell-admin-0.1.16/src/pastelladmin/pastell_connector_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-12 14:49:14.000000 pastell-admin-0.1.16/src/pastelladmin/pastell_docs_delete_from_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-04-12 14:49:14.000000 pastell-admin-0.1.16/src/pastelladmin/pastell_find.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3213 2023-04-12 14:49:14.000000 pastell-admin-0.1.16/src/pastelladmin/pastell_matrice_roles.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2540 2023-04-12 14:49:14.000000 pastell-admin-0.1.16/src/pastelladmin/pastell_org.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-04-12 14:49:14.000000 pastell-admin-0.1.16/src/pastelladmin/pastell_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:49:28.608570 pastell-admin-0.1.16/src/pastelladmin/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-12 14:49:14.000000 pastell-admin-0.1.16/src/pastelladmin/shared/configuration.py
```

### Comparing `pastell-admin-0.1.15/LICENSE` & `pastell-admin-0.1.16/LICENSE`

 * *Files identical despite different names*

### Comparing `pastell-admin-0.1.15/PKG-INFO` & `pastell-admin-0.1.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pastell-admin
-Version: 0.1.15
+Version: 0.1.16
 Author-email: Sebastien Pelhate <sebastien.pelhate@megalis.bretagne.bzh>, Yann Guenneugues <yann.guenneugues@sib.fr>
 Project-URL: Homepage, https://github.com/megalis-bretagne/scripts-pastell
 Project-URL: Bug Tracker, https://github.com/megalis-bretagne/scripts-pastell/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -17,22 +17,22 @@
 
 
 # Installation
 
 Pour la version stable :
 
 ```
-pip install pastell-admin==0.1.15
+pip install pastell-admin==0.1.16
 ```
 
 Pour la version de dev :
 
 ```
 pip install requests
-pip install -i https://test.pypi.org/simple/ pastell-admin==0.1.15
+pip install -i https://test.pypi.org/simple/ pastell-admin==0.1.16
 ```
 # Développement
 
 ```
 git clone git@github.com:megalis-bretagne/scripts-pastell.git
 cd scripts-pastell
 python3 -m venv .venv
```

### Comparing `pastell-admin-0.1.15/README.md` & `pastell-admin-0.1.16/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 
 # Installation
 
 Pour la version stable :
 
 ```
-pip install pastell-admin==0.1.15
+pip install pastell-admin==0.1.16
 ```
 
 Pour la version de dev :
 
 ```
 pip install requests
-pip install -i https://test.pypi.org/simple/ pastell-admin==0.1.15
+pip install -i https://test.pypi.org/simple/ pastell-admin==0.1.16
 ```
 # Développement
 
 ```
 git clone git@github.com:megalis-bretagne/scripts-pastell.git
 cd scripts-pastell
 python3 -m venv .venv
```

### Comparing `pastell-admin-0.1.15/pyproject.toml` & `pastell-admin-0.1.16/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pastell-admin"
-version = "0.1.15"
+version = "0.1.16"
 authors = [
   { name="Sebastien Pelhate", email="sebastien.pelhate@megalis.bretagne.bzh"}, {name ="Yann Guenneugues" ,email="yann.guenneugues@sib.fr"  }
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pastell-admin-0.1.15/src/pastell_admin.egg-info/PKG-INFO` & `pastell-admin-0.1.16/src/pastell_admin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pastell-admin
-Version: 0.1.15
+Version: 0.1.16
 Author-email: Sebastien Pelhate <sebastien.pelhate@megalis.bretagne.bzh>, Yann Guenneugues <yann.guenneugues@sib.fr>
 Project-URL: Homepage, https://github.com/megalis-bretagne/scripts-pastell
 Project-URL: Bug Tracker, https://github.com/megalis-bretagne/scripts-pastell/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -17,22 +17,22 @@
 
 
 # Installation
 
 Pour la version stable :
 
 ```
-pip install pastell-admin==0.1.15
+pip install pastell-admin==0.1.16
 ```
 
 Pour la version de dev :
 
 ```
 pip install requests
-pip install -i https://test.pypi.org/simple/ pastell-admin==0.1.15
+pip install -i https://test.pypi.org/simple/ pastell-admin==0.1.16
 ```
 # Développement
 
 ```
 git clone git@github.com:megalis-bretagne/scripts-pastell.git
 cd scripts-pastell
 python3 -m venv .venv
```

### Comparing `pastell-admin-0.1.15/src/pastell_admin.egg-info/SOURCES.txt` & `pastell-admin-0.1.16/src/pastell_admin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pastell-admin-0.1.15/src/pastelladmin/api/client.py` & `pastell-admin-0.1.16/src/pastelladmin/api/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python3
 from ast import Assert, Param
 from distutils.log import error
+from fcntl import F_DUPFD
 import requests, json
 from requests.auth import HTTPBasicAuth
 from urllib.parse import urlencode
 from datetime import datetime
 
 class Session():
     """
@@ -367,27 +368,32 @@
     def delete(self, id_e, id_ce):
         url = f"https://{self.server}/api/v2/entite/{id_e}/connecteur/{id_ce}"
         request = requests.delete(url, auth=self.auth)
         result = json.loads(request.text)
         if request.status_code == 200:
             print(f"info: Connecteur: {id_ce} supprimé avec succès")
 
-    def update(self, id_e, id_ce, parameters):
+    def update(self, id_e, id_ce, parameters, file=None):
         """_summary_
 
         Args:
             id_e (_type_): _description_
             id_ce (_type_): _description_
             parameters (_type_): _description_
 
         Returns:
             _type_: _description_
         """
-        urlConnecteur = f"https://{self.server}/api/v2/entite/{id_e}/connecteur/{id_ce}/content/"
-        responseConnecteur = requests.patch(urlConnecteur, data=parameters, auth=self.auth)
+        if file:
+            urlConnecteur = f"https://{self.server}/api/v2/entite/{id_e}/connecteur/{id_ce}/file/definition"
+            responseConnecteur = requests.post(urlConnecteur, data=parameters, files=file, auth=self.auth)
+        else:
+            urlConnecteur = f"https://{self.server}/api/v2/entite/{id_e}/connecteur/{id_ce}/content/"
+            responseConnecteur = requests.patch(urlConnecteur, data=parameters, auth=self.auth)
+
         success = False
         if responseConnecteur.ok:
             success = True
         else:
             print(f"error: Creation config connecteur {id_ce} KO erreur:{responseConnecteur.text}")
 
         return Result(success, None)
```

### Comparing `pastell-admin-0.1.15/src/pastelladmin/delete_any.py` & `pastell-admin-0.1.16/src/pastelladmin/delete_any.py`

 * *Files identical despite different names*

### Comparing `pastell-admin-0.1.15/src/pastelladmin/pastell_associations.py` & `pastell-admin-0.1.16/src/pastelladmin/pastell_associations.py`

 * *Files identical despite different names*

### Comparing `pastell-admin-0.1.15/src/pastelladmin/pastell_connector.py` & `pastell-admin-0.1.16/src/pastelladmin/pastell_connector.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 import  json, re
-import os
+import os, tempfile
 from datetime import datetime
 import argparse
 from .api.client import Session, Entity, Association, Connector
 from .shared.configuration import getConfiguration
 
 """
 Ce script permet de gérer des connecteurs pour une instance Pastell:
@@ -43,15 +43,15 @@
   result = o.copy()
   for key, val in o.items():
     variable = re.findall('{{(.*?)}}', val)
     if variable and os.getenv(variable[0]):
       result[key] = os.getenv(variable[0])
   return result
 
-def taskConnectorFor(session, scope, action, connector_template, delete_list, flux_associe, lib_connector, type_connector, id_connector, details, recursive, scheduler):
+def taskConnectorFor(session, scope, action, connector_template, delete_list, flux_associe, lib_connector, type_connector, id_connector, details, recursive, scheduler, file):
   global connector
   if scope == 'all':
     # Get all entities from Pastell API
     request = Entity(session).getAll()
     if request.success:
       entities = request.result
     else:
@@ -125,16 +125,19 @@
         # Its possible have many connectors with the same libelle
         if len(id_ce_list) > 1:
           print(f"warning : des doublons existent pour le connecteur {lib_connector} de l'entité {id_e}")
         # get only the first id_ce
         id_ce = id_ce_list[0]
         if action in ['append', 'update']:
           print(f"info : entité : {id_e} : mise à jour du connecteur : {id_ce}")
-          parameters = variables_substitution(connector_template["parameters"])
-          result = Connector(session).update(id_e, id_ce, parameters)
+          if type_connector == "transformation":
+            parameters = {'file_name': 'definition.json'}
+          else:
+            parameters = variables_substitution(connector_template["parameters"])
+          result = Connector(session).update(id_e, id_ce, parameters, file)
           if result and flux_associe:
             Association(session).create(id_e, flux_associe, id_ce, type_connector)
           if result.success and scheduler:
             Connector(session).action(id_e, id_ce, "purge-async")
 
         elif action == 'dissociate':
           #Dissociate only with the flux specified
@@ -144,15 +147,15 @@
         elif action == 'create':
           # Does not occurs because entities are filtered for this connector
           print(f"warning : le connecteur existe déjà : {id_ce} pour l'entité : {id_e}")
       else:
         if action in ['create', 'append']:
           #Only create connector if does not exists yet
           print(f"info : création du connecteur pour l'entité : {id_e}")
-          createConnecteur(session, id_e, connector_template, flux_associe, lib_connector, type_connector, scheduler)
+          createConnecteur(session, id_e, connector_template, flux_associe, lib_connector, type_connector, scheduler, file)
         elif action in ['delete', 'update']:
           # Does not occurs because entities are filtered for this connector
           print(f"warning: Aucun connecteur de type {type_connector}:{id_connector} et libellé {lib_connector} trouvé pour l'entité ({id_e})")
 
 
 def deleteConnector(session, id_e, id_ce):
   #delete associations for this connector
@@ -173,27 +176,30 @@
     if flux:
       print(f"info : désassociation du connecteur {id_ce} avec le flux {association['flux']}")
     else:
       print(f"info: désassociation du connecteur {id_ce} avec tous les flux")
     Association(session).delete(id_e, association["id_fe"])
 
 
-def createConnecteur(session, id_e, connector_template, flux_associe, lib_connector, type_connector, scheduler):
+def createConnecteur(session, id_e, connector_template, flux_associe, lib_connector, type_connector, scheduler, file):
   definition = variables_substitution(connector_template["definition"])
-  parameters = variables_substitution(connector_template["parameters"])
+  if type_connector == "transformation":
+    parameters = {'file_name': 'definition.json'}
+  else:
+    parameters = variables_substitution(connector_template["parameters"])
   #Etape 1 Creation du connecteur sans sa configuration pour l'IDE sélectionnée
   request = Connector(session).create(id_e, definition)
   if request.success:
     id_ce = request.result
   else:
     print(f"error : {request.result}")
 
   if id_ce:
     # ETAPE 2: configuration du connecteur précédemment créé avec injection des paramètres
-    request = Connector(session).update(id_e, id_ce, parameters)
+    request = Connector(session).update(id_e, id_ce, parameters, file)
     if request.success and flux_associe:
       Association(session).create(id_e, flux_associe, id_ce, type_connector)
     if request.success and scheduler:
       Connector(session).action(id_e, id_ce, "purge-async")
 
   else:
     print(f"error : Création du connecteur {lib_connector} KO erreur:{request.result}")
@@ -226,14 +232,15 @@
 
 def connector(env, action, org=None, flux_associe=None, source=None, type_connector=None, id_connector=None, lib_connector=None, details=None, recursive=None, scheduler=None):
   #Get parameters from config file ~/.pastell-admin
   config = getConfiguration()
 
   delete_list = None
   connector_template = None
+  file_transformation = None
 
   #Export var to OS environnement
   for var, value in config[env].items():
     if var not in ('server', 'login', 'password'):
       os.environ[var] = value
 
   #Check for mandatory parameters
@@ -247,14 +254,24 @@
     connector_template = json.load(f)
     # Récupération des propriétés du connecteur & substitution des variables
     assert all( key in connector_template.keys() for key in ["definition", "parameters"])
     assert all(key in connector_template["definition"].keys() for key in ["libelle", "id_connecteur", "type"])
     lib_connector = connector_template["definition"]["libelle"]
     id_connector = connector_template["definition"]["id_connecteur"]
     type_connector = connector_template["definition"]["type"]
+    if type_connector == "transformation":
+      parameters = connector_template["parameters"]
+      #Create temporary file from parameters
+      tmpfile = tempfile.NamedTemporaryFile()
+      with open(tmpfile.name, "w") as f:
+        f.write(json.dumps(parameters))
+      file_transformation = {'file_content': open(tmpfile.name, "rb")}
+
+
+
   #if delete
   elif action == 'delete':
     assert (lib_connector and type_connector and id_connector) or source
     if source:
       f = open(source)
       # returns JSON object as dictionary
       delete_list = json.load(f)
@@ -274,15 +291,16 @@
   #Check if session is valid
   if not session.valid:
     exit()
   if action in ['status', 'create', 'append', 'dissociate', 'delete', 'update']:
     scope = 'all'
     if org:
       scope = org
-    taskConnectorFor(session, scope, action, connector_template, delete_list, flux_associe, lib_connector, type_connector, id_connector, details, recursive, scheduler)
-
+    taskConnectorFor(session, scope, action, connector_template, delete_list, flux_associe, lib_connector, type_connector, id_connector, details, recursive, scheduler, file=file_transformation)
+    if file_transformation and tmpfile:
+      tmpfile.close()
 
 if __name__ == '__main__':
   script_wrapper()
```

### Comparing `pastell-admin-0.1.15/src/pastelladmin/pastell_connector_instances.py` & `pastell-admin-0.1.16/src/pastelladmin/pastell_connector_instances.py`

 * *Files identical despite different names*

### Comparing `pastell-admin-0.1.15/src/pastelladmin/pastell_docs_delete_from_list.py` & `pastell-admin-0.1.16/src/pastelladmin/pastell_docs_delete_from_list.py`

 * *Files identical despite different names*

### Comparing `pastell-admin-0.1.15/src/pastelladmin/pastell_find.py` & `pastell-admin-0.1.16/src/pastelladmin/pastell_find.py`

 * *Files identical despite different names*

### Comparing `pastell-admin-0.1.15/src/pastelladmin/pastell_matrice_roles.py` & `pastell-admin-0.1.16/src/pastelladmin/pastell_matrice_roles.py`

 * *Files identical despite different names*

### Comparing `pastell-admin-0.1.15/src/pastelladmin/pastell_org.py` & `pastell-admin-0.1.16/src/pastelladmin/pastell_org.py`

 * *Files identical despite different names*

### Comparing `pastell-admin-0.1.15/src/pastelladmin/pastell_stats.py` & `pastell-admin-0.1.16/src/pastelladmin/pastell_stats.py`

 * *Files identical despite different names*

