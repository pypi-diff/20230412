# Comparing `tmp/etl_csm-0.1.0.tar.gz` & `tmp/etl_csm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etl_csm-0.1.0.tar", last modified: Wed Apr 12 15:49:18 2023, max compression
+gzip compressed data, was "etl_csm-0.1.1.tar", last modified: Wed Apr 12 17:58:44 2023, max compression
```

## Comparing `etl_csm-0.1.0.tar` & `etl_csm-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 15:49:18.052555 etl_csm-0.1.0/
-drwxrwxrwx   0        0        0        0 2023-04-12 15:49:18.047555 etl_csm-0.1.0/Etl/
--rw-rw-rw-   0        0        0     3383 2023-04-12 15:19:35.000000 etl_csm-0.1.0/Etl/Execute.py
--rw-rw-rw-   0        0        0     1547 2023-04-12 14:55:44.000000 etl_csm-0.1.0/Etl/Extrator.py
--rw-rw-rw-   0        0        0     1965 2023-04-12 15:20:08.000000 etl_csm-0.1.0/Etl/Helper.py
--rw-rw-rw-   0        0        0     1761 2023-04-12 15:13:14.000000 etl_csm-0.1.0/Etl/Loader.py
--rw-rw-rw-   0        0        0     4814 2023-04-12 14:17:43.000000 etl_csm-0.1.0/Etl/Treatment_extras.py
--rw-rw-rw-   0        0        0    11840 2023-04-12 13:29:28.000000 etl_csm-0.1.0/Etl/Treatment_tracking.py
--rw-rw-rw-   0        0        0      656 2023-04-12 14:27:31.000000 etl_csm-0.1.0/Etl/Treatment_tracking_pme.py
--rw-rw-rw-   0        0        0      616 2023-04-12 15:19:11.000000 etl_csm-0.1.0/Etl/__init__.py
--rw-rw-rw-   0        0        0     1091 2023-03-14 18:25:25.000000 etl_csm-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      526 2023-04-12 15:49:18.051555 etl_csm-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      901 2023-04-03 13:37:17.000000 etl_csm-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 15:49:18.051555 etl_csm-0.1.0/etl_csm.egg-info/
--rw-rw-rw-   0        0        0      526 2023-04-12 15:49:17.000000 etl_csm-0.1.0/etl_csm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2023-04-12 15:49:17.000000 etl_csm-0.1.0/etl_csm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 15:49:17.000000 etl_csm-0.1.0/etl_csm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-04-12 15:49:17.000000 etl_csm-0.1.0/etl_csm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-12 15:49:17.000000 etl_csm-0.1.0/etl_csm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 15:49:18.052555 etl_csm-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      904 2023-04-12 15:45:22.000000 etl_csm-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 17:58:44.639399 etl_csm-0.1.1/
+drwxrwxrwx   0        0        0        0 2023-04-12 17:58:44.635396 etl_csm-0.1.1/Etl/
+-rw-rw-rw-   0        0        0     3379 2023-04-12 17:56:57.000000 etl_csm-0.1.1/Etl/Execute.py
+-rw-rw-rw-   0        0        0     1543 2023-04-12 17:56:57.000000 etl_csm-0.1.1/Etl/Extrator.py
+-rw-rw-rw-   0        0        0     1965 2023-04-12 17:53:53.000000 etl_csm-0.1.1/Etl/Helper.py
+-rw-rw-rw-   0        0        0     1753 2023-04-12 17:56:57.000000 etl_csm-0.1.1/Etl/Loader.py
+-rw-rw-rw-   0        0        0     4814 2023-04-12 17:53:53.000000 etl_csm-0.1.1/Etl/Treatment_extras.py
+-rw-rw-rw-   0        0        0    12289 2023-04-12 17:56:57.000000 etl_csm-0.1.1/Etl/Treatment_tracking.py
+-rw-rw-rw-   0        0        0      656 2023-04-12 17:53:53.000000 etl_csm-0.1.1/Etl/Treatment_tracking_pme.py
+-rw-rw-rw-   0        0        0      616 2023-04-12 17:53:53.000000 etl_csm-0.1.1/Etl/__init__.py
+-rw-rw-rw-   0        0        0     1091 2023-03-14 18:25:25.000000 etl_csm-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      526 2023-04-12 17:58:44.638396 etl_csm-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      901 2023-04-03 13:37:17.000000 etl_csm-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 17:58:44.638396 etl_csm-0.1.1/etl_csm.egg-info/
+-rw-rw-rw-   0        0        0      526 2023-04-12 17:58:44.000000 etl_csm-0.1.1/etl_csm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2023-04-12 17:58:44.000000 etl_csm-0.1.1/etl_csm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 17:58:44.000000 etl_csm-0.1.1/etl_csm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-04-12 17:58:44.000000 etl_csm-0.1.1/etl_csm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-12 17:58:44.000000 etl_csm-0.1.1/etl_csm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 17:58:44.639399 etl_csm-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      904 2023-04-12 17:58:08.000000 etl_csm-0.1.1/setup.py
```

### Comparing `etl_csm-0.1.0/Etl/Execute.py` & `etl_csm-0.1.1/Etl/Execute.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def etl_df(self):
         """
             Funcao que roda ETL do dataframe tracking,
             nao arquiva em memoria o dataframe extras_df
         """ 
         df = form_df_tracking(self.query) #1
         df = fill_na_tracking(df) #2
-        # df = remove_test(df) #3 Não se pode remover testes no ambiente de teste porque senao você remove todo mundo
+        df = remove_test(df) #3 Não se pode remover testes no ambiente de teste porque senao você remove todo mundo
         flag_duplicated_tracks(df) #4
         df = dtype_tracking(df) #5
         df['steps'] = steps_residential(df['category']) #6
         df['errors'] = errors(df['category']) #7
         return df
 
     def etl_extras_df(self,df:Type) -> Type:
@@ -50,15 +50,15 @@
         extras_df = fill_na_extras(extras_df) #4 
         extras_df = dtype_extras(extras_df) #5
         return extras_df
 
     def etl_df_pme(self):
         df = form_df_tracking(self.query) #1
         df = fill_na_tracking(df) #2
-        # df = remove_test(df) #3 Não se pode remover testes no ambiente de teste porque senao você remove todo mundo
+        df = remove_test(df) #3 Não se pode remover testes no ambiente de teste porque senao você remove todo mundo
         flag_duplicated_tracks(df) #4
         df = dtype_tracking(df) #5
         df['steps'] = steps_pme(df['category']) #6
         df['errors'] = errors(df['category']) #7
         return df
 
     def etl_extras_df_pme(self,df:Type) -> Type:
```

### Comparing `etl_csm-0.1.0/Etl/Extrator.py` & `etl_csm-0.1.1/Etl/Extrator.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,16 +13,16 @@
         ARGS
         query = Query a ser feita
     """
     try:
         engine = psycopg2.connect(
             database = 'postgres',
             user = 'tracking',
-            password = environ['SQL_PET_PASSWORD'],
-            host = 'pet-avi-chatbot-tracking-db.clarobrasil.mobi',
+            password = environ['SQL_PASSWORD'],
+            host = 'prd-avi-chatbot-tracking-db.clarobrasil.mobi',
             port = '5432',
         )
     except (Exception,psycopg2.Error) as error:
         print(f'''
             Erro na conexão
             {error}
             ''',)
```

### Comparing `etl_csm-0.1.0/Etl/Helper.py` & `etl_csm-0.1.1/Etl/Helper.py`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.0/Etl/Loader.py` & `etl_csm-0.1.1/Etl/Loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 from .Helper import psql_insert_copy,timing
 
 @timing
 def load_cloud(df:Type,bot:str) -> None:
     """
     Ira fazer o processo de carregamento para o RDS depois de processado.
     """
-    engine_alchemy = create_engine(f"postgresql://tracking:{environ['SQL_PET_PASSWORD']}@pet-avi-chatbot-tracking-db.clarobrasil.mobi:5432/clean_data")
+    engine_alchemy = create_engine(f"postgresql://tracking:{environ['SQL_PASSWORD']}@prd-avi-chatbot-tracking-db.clarobrasil.mobi:5432/clean_data")
     tries = 10
     for _ in range(tries):
         try:
             df.to_sql(f'{bot}_tracking_treated',engine_alchemy,if_exists = 'append',method = psql_insert_copy,index = False,chunksize = 10000)
             break
         except (Exception,psycopg2.Error) as error:
             warning("Fazendo novo conexao com a clean data para adicionar coluna!")
             engine = psycopg2.connect(
                 database = 'clean_data',
                 user = 'tracking',
-                password = environ['SQL_PET_PASSWORD'],
-                host = 'pet-avi-chatbot-tracking-db.clarobrasil.mobi',
+                password = environ['SQL_PASSWORD'],
+                host = 'prd-avi-chatbot-tracking-db.clarobrasil.mobi',
                 port = '5432',
             )
             cursor = engine.cursor()
             column = findall('"(.*?)"',str(error))[0]
             warning(f"Tive que acrescentar mais uma coluna ao seu dataframe ja existente a coluna foi {column}")
             query = f"""
             ALTER TABLE {bot}_tracking_treated
```

### Comparing `etl_csm-0.1.0/Etl/Treatment_extras.py` & `etl_csm-0.1.1/Etl/Treatment_extras.py`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.0/Etl/Treatment_tracking.py` & `etl_csm-0.1.1/Etl/Treatment_tracking.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,44 +127,50 @@
     unstepped_trackings = []
     st = []
     for i in s:
         if 'onbo' in i:
             if 'start' in i:
                 st.append('1-Onboarding + Retorno')
             elif 'segment' in i:
-                st.append('Opcional-Onboarding escolha de bot')
+                st.append('1.1-Opcional-Onboarding escolha de bot')
             else:
                 st.append(nan)
-        elif 'product-selection' in i:
-            st.append('Opcional-Seleciona produto')
         elif 'product-availability' in i:
             if 'cpf-request' in i:
                 st.append('3-Informa localizacao e cpf')
             elif 'cpf-validation' in i:
                 st.append('3.1-CPF valido (V.2.0)')
+            elif 'health-api-orders-validation' in i:
+                st.append('3.2-Consulta orders (V.2.1.1)')
+            elif 'api-residential-customer-contracts-open-request-validation' in i:
+                st.append('3.3-Consulta customer contracts (V.2.1.2)')
             elif 'postalcode-request' in i:
-                st.append('3.2-Obtencao de CEP')
-            elif 'postalcode-validation options' in i:
-                st.append('3.3-CEP valido (V.2.2)')
+                st.append('3.4-Obtencao de CEP')
+            elif 'postalcode-validation' in i:
+                st.append('3.5-CEP valido (V.2.2)')
             elif 'postalcode-validation-true' in i:
-                st.append('3.4-Passa endereco')
+                st.append('3.6-Pegando complemento')
             elif 'health-api-address-validation' in i:
-                st.append('3.5-Endereco valida (V.2.3)')
+                st.append('3.7-Endereco sendo validado (V.2.3)')
+            elif 'empty-public-space-validation' in i:
+                st.append('3.8-Validacao de logradouro (V.2.4)')
+            elif 'empty-neighborhood-validation' in i:
+                st.append('3.9-Bairro sendo validado (V.2.3)')
             elif 'address-confirmation' in i:
-                st.append('3.6-Endereco resumido')
+                st.append('3.9.1-Endereco resumido')
             elif 'health-api-residential-customer-contracts-validation' in i:
-                st.append('3.7-Consulta de CPF na api de base(V.2.9)')
+                st.append('3.9.2-Consulta de CPF na api de base (V.2.9)')
             elif 'client-validation' in i:
-                st.append('3.8-Localizado na api de base (V.2.10)')
+                st.append('3.9.3-Localizado na api de base validacao (V.2.10)')
             elif 'product-availability-validation' in i:
-                st.append('3.9-Produto e disponibilizado na regiao (V.2.12)')
+                st.append('3.9.4-Produto e disponibilizado na regiao (V.2.11)')
             elif 'health-api-plan-availability-validation' in i:
-                st.append('3.9.1-Consulta na api de catalogos(V.2.13)')
+                st.append('3.9.5-Consulta na api de catalogos(V.2.13)')
             elif 'plans-available-catalog-validation' in i:
-                st.append('3.9.2-Plano disponivel no catalogo (V.2.14)')
+                st.append('3.9.6-Plano disponivel no catalogo (V.2.14)')
             else:
                 st.append(nan)
         elif 'plan-selection' in i:
             st.append('4-Escolhe plano (Todos produtos)')
         elif 'registration' in i:
             if 'full-name-request' in i:
                 st.append('5-Realiza cadastro')
```

### Comparing `etl_csm-0.1.0/Etl/Treatment_tracking_pme.py` & `etl_csm-0.1.1/Etl/Treatment_tracking_pme.py`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.0/Etl/__init__.py` & `etl_csm-0.1.1/Etl/__init__.py`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.0/LICENSE` & `etl_csm-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.0/PKG-INFO` & `etl_csm-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etl_csm
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pacote de ETL
 Home-page: https://gitdev.clarobrasil.mobi/vendas-claro/csm/etl
 Author: ingloriamori
 Author-email: francisco.froes@globalhitss.com.br
 License: MIT
 Keywords: python,etl
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `etl_csm-0.1.0/README.md` & `etl_csm-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.0/etl_csm.egg-info/PKG-INFO` & `etl_csm-0.1.1/etl_csm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etl-csm
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pacote de ETL
 Home-page: https://gitdev.clarobrasil.mobi/vendas-claro/csm/etl
 Author: ingloriamori
 Author-email: francisco.froes@globalhitss.com.br
 License: MIT
 Keywords: python,etl
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `etl_csm-0.1.0/setup.py` & `etl_csm-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = 'Pacote de ETL'
 
 # Setting up
 setup(
     name = "etl_csm",
     version = VERSION,
     author = "ingloriamori",
```

