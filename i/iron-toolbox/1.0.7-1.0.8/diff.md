# Comparing `tmp/iron_toolbox-1.0.7.tar.gz` & `tmp/iron_toolbox-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iron_toolbox-1.0.7.tar", last modified: Wed Apr  5 12:41:25 2023, max compression
+gzip compressed data, was "iron_toolbox-1.0.8.tar", last modified: Wed Apr 12 18:15:46 2023, max compression
```

## Comparing `iron_toolbox-1.0.7.tar` & `iron_toolbox-1.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 12:41:25.887949 iron_toolbox-1.0.7/
--rw-rw-rw-   0        0        0     1092 2023-03-16 21:06:41.000000 iron_toolbox-1.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0      649 2023-04-05 12:41:25.887949 iron_toolbox-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       76 2023-03-17 14:20:36.000000 iron_toolbox-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-05 12:41:25.877434 iron_toolbox-1.0.7/iron_toolbox/
--rw-rw-rw-   0        0        0      105 2023-03-16 23:27:50.000000 iron_toolbox-1.0.7/iron_toolbox/__init__.py
--rw-rw-rw-   0        0        0    15272 2023-04-05 12:40:46.000000 iron_toolbox-1.0.7/iron_toolbox/aws_functions.py
--rw-rw-rw-   0        0        0     1757 2023-03-16 23:27:50.000000 iron_toolbox-1.0.7/iron_toolbox/domo_functions.py
--rw-rw-rw-   0        0        0    24103 2023-02-23 20:09:35.000000 iron_toolbox-1.0.7/iron_toolbox/iron_functions.py
--rw-rw-rw-   0        0        0    64808 2023-03-21 15:07:05.000000 iron_toolbox-1.0.7/iron_toolbox/mongo_functions.py
--rw-rw-rw-   0        0        0     4325 2023-02-01 20:27:50.000000 iron_toolbox-1.0.7/iron_toolbox/sftp_functions.py
-drwxrwxrwx   0        0        0        0 2023-04-05 12:41:25.885954 iron_toolbox-1.0.7/iron_toolbox.egg-info/
--rw-rw-rw-   0        0        0      649 2023-04-05 12:41:25.000000 iron_toolbox-1.0.7/iron_toolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      399 2023-04-05 12:41:25.000000 iron_toolbox-1.0.7/iron_toolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 12:41:25.000000 iron_toolbox-1.0.7/iron_toolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      222 2023-04-05 12:41:25.000000 iron_toolbox-1.0.7/iron_toolbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-05 12:41:25.000000 iron_toolbox-1.0.7/iron_toolbox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-05 12:41:25.889455 iron_toolbox-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1586 2023-04-05 12:40:46.000000 iron_toolbox-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:15:46.173829 iron_toolbox-1.0.8/
+-rw-rw-rw-   0        0        0     1092 2023-03-16 21:06:41.000000 iron_toolbox-1.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0      649 2023-04-12 18:15:46.173829 iron_toolbox-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       76 2023-03-17 14:20:36.000000 iron_toolbox-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 18:15:46.164742 iron_toolbox-1.0.8/iron_toolbox/
+-rw-rw-rw-   0        0        0      105 2023-03-16 23:27:50.000000 iron_toolbox-1.0.8/iron_toolbox/__init__.py
+-rw-rw-rw-   0        0        0    15272 2023-04-05 12:40:46.000000 iron_toolbox-1.0.8/iron_toolbox/aws_functions.py
+-rw-rw-rw-   0        0        0     1757 2023-03-16 23:27:50.000000 iron_toolbox-1.0.8/iron_toolbox/domo_functions.py
+-rw-rw-rw-   0        0        0    24103 2023-02-23 20:09:35.000000 iron_toolbox-1.0.8/iron_toolbox/iron_functions.py
+-rw-rw-rw-   0        0        0    64816 2023-04-12 18:15:15.000000 iron_toolbox-1.0.8/iron_toolbox/mongo_functions.py
+-rw-rw-rw-   0        0        0     4325 2023-02-01 20:27:50.000000 iron_toolbox-1.0.8/iron_toolbox/sftp_functions.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:15:46.171829 iron_toolbox-1.0.8/iron_toolbox.egg-info/
+-rw-rw-rw-   0        0        0      649 2023-04-12 18:15:45.000000 iron_toolbox-1.0.8/iron_toolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      399 2023-04-12 18:15:45.000000 iron_toolbox-1.0.8/iron_toolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 18:15:45.000000 iron_toolbox-1.0.8/iron_toolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      222 2023-04-12 18:15:45.000000 iron_toolbox-1.0.8/iron_toolbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-12 18:15:45.000000 iron_toolbox-1.0.8/iron_toolbox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-12 18:15:46.175829 iron_toolbox-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1586 2023-04-12 18:15:15.000000 iron_toolbox-1.0.8/setup.py
```

### Comparing `iron_toolbox-1.0.7/LICENSE.txt` & `iron_toolbox-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iron_toolbox-1.0.7/PKG-INFO` & `iron_toolbox-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iron_toolbox
-Version: 1.0.7
+Version: 1.0.8
 Summary: Functions to be used by Iron Data Analytics Team
 Home-page: https://github.com/IronTrainers/iron_data_toolbox
 Download-URL: https://github.com/IronTrainers/iron_data_toolbox/archive/refs/tags/iron_data_toolboox.tar.gz
 Author: Luciano Siqueira
 Author-email: lucianosiqueira@iron.fit
 License: MIT
 Project-URL: Bug Tracker, https://github.com/IronTrainers/iron_data_toolbox/issues
```

### Comparing `iron_toolbox-1.0.7/iron_toolbox/aws_functions.py` & `iron_toolbox-1.0.8/iron_toolbox/aws_functions.py`

 * *Files identical despite different names*

### Comparing `iron_toolbox-1.0.7/iron_toolbox/domo_functions.py` & `iron_toolbox-1.0.8/iron_toolbox/domo_functions.py`

 * *Files identical despite different names*

### Comparing `iron_toolbox-1.0.7/iron_toolbox/iron_functions.py` & `iron_toolbox-1.0.8/iron_toolbox/iron_functions.py`

 * *Files identical despite different names*

### Comparing `iron_toolbox-1.0.7/iron_toolbox/mongo_functions.py` & `iron_toolbox-1.0.8/iron_toolbox/mongo_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,18 +84,18 @@
                                                                   'description': 1,
                                                                   'cid10': 1,
                                                                   'ciap': 1}), desc="Total itens recebidos:"))
         print(f'Realizando tratamento do Dataset {mongodb_collection}!')
         dbsupport = dbsupport.replace({'_p_patient': r'^_User\$'}, {'_p_patient': ''}, regex=True)
         dbsupport = dbsupport.replace({'_p_activeStaff': r'^Staff\$'}, {'_p_activeStaff': ''}, regex=True)
         dbsupport = dbsupport.replace({'_p_support': r'^Support\$'}, {'_p_support': ''}, regex=True)
+        dbsupport = pd.concat([dbsupport, dbsupport_schema])
     else:
         dbsupport = pd.DataFrame(tqdm(db[mongodb_collection].find(filtro, colunas), desc="Total itens recebidos:"))
     # adicionar o tratamento fora do if com uma condicao de teste
-    dbsupport = pd.concat([dbsupport, dbsupport_schema])
     print(f'Dataset {mongodb_collection} Criado!')
     return dbsupport
 
 
 def gerar_tabela_corporation(filtro=None, colunas=None, mongodb_collection='Corporation'):
     contar_itens_collection(filtro, mongodb_collection)
     if colunas is None:
@@ -484,23 +484,23 @@
                                                           {'_p_scheduledAppointments': ''}, regex=True)
         dbusertelephonecall = dbusertelephonecall.replace({'_p_staff': r'^Staff\$'}, {'_p_staff': ''}, regex=True)
         dbusertelephonecall = dbusertelephonecall.replace({'_p_responsible': r'^Staff\$'}, {'_p_responsible': ''},
                                                           regex=True)
         dbusertelephonecall = dbusertelephonecall.replace({'_p_user': r'^_User\$'}, {'_p_user': ''}, regex=True)
         dbusertelephonecall = dbusertelephonecall.replace({'_p_corporation': r'^Corporation\$'},
                                                                   {'_p_corporation': ''}, regex=True)
-
+        dbusertelephonecall = pd.concat([dbusertelephonecall, dbusertelephonecall_schema])
     else:
         dbusertelephonecall = pd.DataFrame(tqdm(db[mongodb_collection].find(filtro, colunas),
                                                 desc="Total itens recebidos:"))
         dbusertelephonecall = dbusertelephonecall.replace({'_p_support': r'^Support\$'}, {'_p_support': ''}, regex=True)
         dbusertelephonecall = dbusertelephonecall.replace({'_p_staff': r'^Staff\$'}, {'_p_staff': ''}, regex=True)
         dbusertelephonecall = dbusertelephonecall.replace({'_p_user': r'^_User\$'}, {'_p_user': ''}, regex=True)
 
-    dbusertelephonecall = pd.concat([dbusertelephonecall, dbusertelephonecall_schema])
+
     print(f'Dataset {mongodb_collection} Criado!')
     return dbusertelephonecall
 
 
 def gerar_tabela_scheduled_appointments(filtro=None, colunas=None, mongodb_collection='ScheduledAppointments'):
     contar_itens_collection(filtro, mongodb_collection)
     if colunas is None:
```

### Comparing `iron_toolbox-1.0.7/iron_toolbox/sftp_functions.py` & `iron_toolbox-1.0.8/iron_toolbox/sftp_functions.py`

 * *Files identical despite different names*

### Comparing `iron_toolbox-1.0.7/iron_toolbox.egg-info/PKG-INFO` & `iron_toolbox-1.0.8/iron_toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iron-toolbox
-Version: 1.0.7
+Version: 1.0.8
 Summary: Functions to be used by Iron Data Analytics Team
 Home-page: https://github.com/IronTrainers/iron_data_toolbox
 Download-URL: https://github.com/IronTrainers/iron_data_toolbox/archive/refs/tags/iron_data_toolboox.tar.gz
 Author: Luciano Siqueira
 Author-email: lucianosiqueira@iron.fit
 License: MIT
 Project-URL: Bug Tracker, https://github.com/IronTrainers/iron_data_toolbox/issues
```

### Comparing `iron_toolbox-1.0.7/setup.py` & `iron_toolbox-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # with open('requirements.txt') as f:
 #     required = f.read().splitlines()
     
 setuptools.setup(
     name='iron_toolbox',
     packages=['iron_toolbox'],
-    version='1.0.7',
+    version='1.0.8',
     license='MIT',
     description='Functions to be used by Iron Data Analytics Team',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Luciano Siqueira',
     author_email='lucianosiqueira@iron.fit',
     url='https://github.com/IronTrainers/iron_data_toolbox',
```

