# Comparing `tmp/etl_csm-0.0.9.tar.gz` & `tmp/etl_csm-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etl_csm-0.0.9.tar", last modified: Mon Apr  3 14:03:56 2023, max compression
+gzip compressed data, was "etl_csm-0.1.0.tar", last modified: Wed Apr 12 15:49:18 2023, max compression
```

## Comparing `etl_csm-0.0.9.tar` & `etl_csm-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 14:03:56.823678 etl_csm-0.0.9/
-drwxrwxrwx   0        0        0        0 2023-04-03 14:03:56.818679 etl_csm-0.0.9/Etl/
--rw-rw-rw-   0        0        0     2512 2023-04-03 13:37:17.000000 etl_csm-0.0.9/Etl/Execute.py
--rw-rw-rw-   0        0        0     2116 2023-04-03 13:51:19.000000 etl_csm-0.0.9/Etl/Extrator.py
--rw-rw-rw-   0        0        0     1666 2023-04-03 13:37:17.000000 etl_csm-0.0.9/Etl/Helper.py
--rw-rw-rw-   0        0        0      574 2023-04-03 13:47:25.000000 etl_csm-0.0.9/Etl/Loader.py
--rw-rw-rw-   0        0        0     6195 2023-04-03 13:37:17.000000 etl_csm-0.0.9/Etl/Treatment_extras.py
--rw-rw-rw-   0        0        0    12413 2023-04-03 13:37:17.000000 etl_csm-0.0.9/Etl/Treatment_tracking.py
--rw-rw-rw-   0        0        0      564 2023-04-03 13:37:17.000000 etl_csm-0.0.9/Etl/__init__.py
--rw-rw-rw-   0        0        0     1091 2023-03-14 18:25:25.000000 etl_csm-0.0.9/LICENSE
--rw-rw-rw-   0        0        0      526 2023-04-03 14:03:56.822678 etl_csm-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      901 2023-04-03 13:37:17.000000 etl_csm-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-03 14:03:56.822678 etl_csm-0.0.9/etl_csm.egg-info/
--rw-rw-rw-   0        0        0      526 2023-04-03 14:03:56.000000 etl_csm-0.0.9/etl_csm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2023-04-03 14:03:56.000000 etl_csm-0.0.9/etl_csm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 14:03:56.000000 etl_csm-0.0.9/etl_csm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-04-03 14:03:56.000000 etl_csm-0.0.9/etl_csm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-03 14:03:56.000000 etl_csm-0.0.9/etl_csm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-03 14:03:56.823678 etl_csm-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      904 2023-04-03 14:03:53.000000 etl_csm-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:49:18.052555 etl_csm-0.1.0/
+drwxrwxrwx   0        0        0        0 2023-04-12 15:49:18.047555 etl_csm-0.1.0/Etl/
+-rw-rw-rw-   0        0        0     3383 2023-04-12 15:19:35.000000 etl_csm-0.1.0/Etl/Execute.py
+-rw-rw-rw-   0        0        0     1547 2023-04-12 14:55:44.000000 etl_csm-0.1.0/Etl/Extrator.py
+-rw-rw-rw-   0        0        0     1965 2023-04-12 15:20:08.000000 etl_csm-0.1.0/Etl/Helper.py
+-rw-rw-rw-   0        0        0     1761 2023-04-12 15:13:14.000000 etl_csm-0.1.0/Etl/Loader.py
+-rw-rw-rw-   0        0        0     4814 2023-04-12 14:17:43.000000 etl_csm-0.1.0/Etl/Treatment_extras.py
+-rw-rw-rw-   0        0        0    11840 2023-04-12 13:29:28.000000 etl_csm-0.1.0/Etl/Treatment_tracking.py
+-rw-rw-rw-   0        0        0      656 2023-04-12 14:27:31.000000 etl_csm-0.1.0/Etl/Treatment_tracking_pme.py
+-rw-rw-rw-   0        0        0      616 2023-04-12 15:19:11.000000 etl_csm-0.1.0/Etl/__init__.py
+-rw-rw-rw-   0        0        0     1091 2023-03-14 18:25:25.000000 etl_csm-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      526 2023-04-12 15:49:18.051555 etl_csm-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      901 2023-04-03 13:37:17.000000 etl_csm-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 15:49:18.051555 etl_csm-0.1.0/etl_csm.egg-info/
+-rw-rw-rw-   0        0        0      526 2023-04-12 15:49:17.000000 etl_csm-0.1.0/etl_csm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2023-04-12 15:49:17.000000 etl_csm-0.1.0/etl_csm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 15:49:17.000000 etl_csm-0.1.0/etl_csm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-04-12 15:49:17.000000 etl_csm-0.1.0/etl_csm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-12 15:49:17.000000 etl_csm-0.1.0/etl_csm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 15:49:18.052555 etl_csm-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      904 2023-04-12 15:45:22.000000 etl_csm-0.1.0/setup.py
```

### Comparing `etl_csm-0.0.9/Etl/Execute.py` & `etl_csm-0.1.0/Etl/Execute.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,78 +1,83 @@
-from logging import basicConfig,INFO
 from typing import Type
 from pandas import concat
+from logging import basicConfig,INFO
+from .Extrator import form_df_tracking,form_df_extras
+from .Treatment_tracking import fill_na_tracking,dtype_tracking,remove_test
+from .Treatment_tracking import steps_residential,errors,flag_duplicated_tracks
+from .Treatment_extras import patternizing_columns,ensure_nan_extras,dtype_extras,fill_na_extras
+from .Treatment_tracking_pme import steps_pme
 from .Helper import timing
-from .Extrator import Connection,form_df_extras
-from .Treatment_tracking import ensure_dtypes,dtype_tracking,remove_test,steps,errors,flag_duplicated_tracks
-from .Treatment_extras import patternizing_columns,ensure_nan_extras,dtype_extras
-from .Treatment_extras import fill_na_extras,patternizing_origins,form_extras_plan
 from .Loader import load_cloud
 
+
 class Runner:
     """
-    Classe de execucao geral, faz tudo o puxada de dados o tratamento deles e carrega eles
-    forma de evitar arquivos salvos em memoria local.
+        Runner é a classe que executa todo o conjunto de funcoes de tratamento.
+        Ele tambem inicializa o processo de logs
+        ARGS:
+        query = String que representa um SQL query valido  
     """
-    def __init__(self,query:str) -> Type:
-        """
-        Executor dessa funcao
-        query = string sql de extracao do RDS
-        """
-        self.query = query
-        basicConfig(filename='etl.log',filemode='a',level=INFO, format='%(levelname)s: %(message)s',)
-        # Configurando logs
+    def __init__(self,query:str,bot:str) -> Type:
+        if bot:
+            self.bot = bot
+            self.query = query
+            basicConfig(filename='etl.log',filemode='a',level=INFO, format='%(levelname)s: %(message)s')
+        else:
+            raise Exception("Para poder rodar essa classe repasse um bot, corparate/residential")
 
     def etl_df(self):
         """
-        Funcao que roda ETL do dataframe tracking,
-        nao arquiva em memoria o dataframe extras_df
-        """
-        #1
-        connection = Connection()
-        #2
-        df = connection.form_df_tracking(self.query)
-        #3
-        df = ensure_dtypes(df)
-        #4
-        # df = remove_test(df)
-        #  Não se pode remover testes no ambiente de teste porque senao você remove todo mundo
-        #5
-        flag_duplicated_tracks(df)
-        #6
-        df = dtype_tracking(df)
-        #7
-        df['steps'] = steps(df['category'])
-        #8
-        df['errors'] = errors(df['category'])
+            Funcao que roda ETL do dataframe tracking,
+            nao arquiva em memoria o dataframe extras_df
+        """ 
+        df = form_df_tracking(self.query) #1
+        df = fill_na_tracking(df) #2
+        # df = remove_test(df) #3 Não se pode remover testes no ambiente de teste porque senao você remove todo mundo
+        flag_duplicated_tracks(df) #4
+        df = dtype_tracking(df) #5
+        df['steps'] = steps_residential(df['category']) #6
+        df['errors'] = errors(df['category']) #7
         return df
-        # Sim esses objetos sao acessiveis se voce quiser
 
     def etl_extras_df(self,df:Type) -> Type:
         """
-        Funcao que roda ETL do dataframe extras
+            Funcao que forma o dataframe de extras
+            e os trata
         """
-        #1
-        extras_df = form_df_extras(df)
-        #2
-        extras_df = patternizing_columns(extras_df)
-        #3
-        extras_df = ensure_nan_extras(extras_df)
-        #4
-        extras_df = fill_na_extras(extras_df)
-        #5
-        extras_df = dtype_extras(extras_df)
-        #6
-        extras_df = patternizing_origins(extras_df)
-        #7
-        extras_df = form_extras_plan(extras_df)
+        extras_df = form_df_extras(df) #1
+        extras_df = patternizing_columns(extras_df) #2
+        extras_df = ensure_nan_extras(extras_df) #3
+        extras_df = fill_na_extras(extras_df) #4 
+        extras_df = dtype_extras(extras_df) #5
         return extras_df
-    
+
+    def etl_df_pme(self):
+        df = form_df_tracking(self.query) #1
+        df = fill_na_tracking(df) #2
+        # df = remove_test(df) #3 Não se pode remover testes no ambiente de teste porque senao você remove todo mundo
+        flag_duplicated_tracks(df) #4
+        df = dtype_tracking(df) #5
+        df['steps'] = steps_pme(df['category']) #6
+        df['errors'] = errors(df['category']) #7
+        return df
+
+    def etl_extras_df_pme(self,df:Type) -> Type:
+        extras_df = form_df_extras(df) #1
+        extras_df = patternizing_columns(extras_df) #2
+        # extras_df = ensure_nan_extras(extras_df) #3 Deixar para avaliacao
+        # extras_df = fill_na_extras(extras_df) #4 Deixar para avaliacao
+        # extras_df = dtype_extras(extras_df) #5 Deixar para avaliacao
+        return extras_df
+
     def run(self) -> None:
-        """
-        Funcao que roda tudo
-        """
-        df = self.etl_df()
-        extras_df = self.etl_extras_df(df)
-        df = concat([df,extras_df],axis = 1)
+        if self.bot == 'residential':
+            df = self.etl_df()
+            extras_df = self.etl_extras_df(df)
+            df = concat([df,extras_df],axis = 1)
+            load_cloud(df,self.bot)
+        if self.bot == 'corporate':
+            df = self.etl_df_pme()
+            extras_df = self.etl_extras_df_pme(df)
+            df = concat([df,extras_df],axis = 1)
+            load_cloud(df,self.bot)
 
-        load_cloud(df)
```

### Comparing `etl_csm-0.0.9/Etl/Helper.py` & `etl_csm-0.1.0/Etl/Helper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Type
 from functools import wraps
 from time import time
 from logging import info
 from io import StringIO
 from csv import writer
+from numpy import nan
 
 def timing(f):
     # Decorator simples para medir tempo de excecucao de funcao
     @wraps(f)
     def wrap(*args, **kw):
         ts = time()
         result = f(*args, **kw)
@@ -23,30 +24,40 @@
     for col in cursor.description:
         cols.append(col[0])
     return cols
 
 def psql_insert_copy(table, conn, keys, data_iter):
     """
     Executa sql query unico para por dados de maneira eficiente em postgresql
-
-    Parametros
-    ----------
-    table : pandas.io.sql.SQLTable - Tabela
-    conn : sqlalchemy.engine.Engine ou sqlalchemy.engine.Connection
-    keys : lista de strings com nomes das colunas, nao precisa passar
-    data_iter : Iterador que vai fazer o trampo todo
+    ARGS
+    table = pandas.io.sql.SQLTable - Tabela
+    conn = sqlalchemy.engine.Engine ou sqlalchemy.engine.Connection
+    keys = lista de strings com nomes das colunas, nao precisa passar
+    data_iter = Iterador que vai fazer o trampo todo
     """
     dbapi_conn = conn.connection
     with dbapi_conn.cursor() as cur:
         s_buf = StringIO()
         writer_obj = writer(s_buf)
         writer_obj.writerows(data_iter)
         s_buf.seek(0)
-
         columns = ', '.join(['"{}"'.format(k) for k in keys])
         if table.schema:
             table_name = '{}.{}'.format(table.schema, table.name)
         else:
             table_name = table.name
         sql = 'COPY {} ({}) FROM STDIN WITH CSV'.format(
             table_name, columns)
         cur.copy_expert(sql=sql, file=s_buf)
+
+def map_substring(s, dict_map):
+    """
+    Funcao helper mapeia as sub strings com facilidade
+    ARGS
+    s = pd.Series a ser interada por
+    dict_map = mapa se substrings
+    
+    """
+    for key in dict_map.keys():
+        if key in s: 
+            return dict_map[key]
+    return nan
```

### Comparing `etl_csm-0.0.9/Etl/Treatment_extras.py` & `etl_csm-0.1.0/Etl/Treatment_extras.py`

 * *Files 18% similar despite different names*

```diff
@@ -100,47 +100,12 @@
                 }
     dtypes = {}
     # Mapa dos dtypes do dataframe atual
     for k in list(extras_df.columns):
         try:
             dtypes[k] = general_map[k]
         except KeyError as error:
-            if k not in ['plan_value','plan_name','plan_offer']:
-                warning(f'O general map de datatypes precisa ser atualizado com a seguinte extra {k}')
+            warning(f'O general map de datatypes precisa ser atualizado com a seguinte extra {k}')
     extras_df = extras_df.astype(dtype = dtypes)
     return extras_df
 
-@timing
-def patternizing_origins(extras_df:Type) -> Type:
-    """
-    Tratamento unico para o extra global campaign_source, redefine os valores
-    a serem alterado e alinha eles
-    """
-    invalid_origins = {'Site':'site',
-    'Attendance Bot':'attendance bot',
-    'Carrinho abandonado e-commerce/SMS':'carrinho-abandonado-ecommerce-sms'}
 
-    extras_df['campaign_source'] = extras_df['campaign_source'].replace(invalid_origins).reset_index(drop = True)
-
-    return extras_df
-
-@timing
-def form_extras_plan(extras_df:Type) -> Type:
-    """
-    Formula coluna de extras globais de planos e deixa em formato json
-    """
-    def common_lambda(x):
-        try:
-            if isinstance(x, str):
-                return loads(x)
-            else:
-                return nan
-        except JSONDecodeError as error:
-            warning(f"Devido ao extra {x} tivemos erro na passagem para json")
-            return str(x)
-    try:
-        extras_df['plan_offer'] = extras_df.plan_offer.apply(common_lambda)
-        extras_df['plan_value'] = extras_df.plan_value.apply(common_lambda)
-        extras_df['plan_name'] = extras_df.plan_name.apply(common_lambda)
-    except AttributeError as error:
-        warning('Nenhum dos users passou por trackings de planos!')
-    return extras_df
```

### Comparing `etl_csm-0.0.9/Etl/Treatment_tracking.py` & `etl_csm-0.1.0/Etl/Treatment_tracking.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from logging import warning,info
 from typing import Type
 from numpy import nan,where
 from pandas import Timedelta
 from .Helper import timing
 
 @timing
-def ensure_dtypes(df:Type)-> Type:
+def fill_na_tracking(df:Type)-> Type:
     """
     Funcao feita para garantir que as colunas que são supostas 
     serem númericas realmente estarem em formato númerico. Tambem verifica se tem valores nulos.
     """
     df['user_phone'] = df.user_phone.str.replace('\D*','',regex = True).replace('',nan)
     df['original_user_id'] = df.original_user_id.replace('',nan)
     if df['user_phone'].isna().any():
@@ -115,62 +115,56 @@
 
     if flagger.fillna(False).any():
         warning('Temos trackings duplicado passar amostra para dev!')
         warning(f'Segue evidencias:{temp_df.loc[flagger.fillna(False)].head().to_dict()}')
         
 
 @timing
-def steps(s:Type) -> Type:
+def steps_residential(s:Type) -> Type:
     """
     Formula coluna steps de acordo com a coluna suffix
     s =  suffix series
     """
     unstepped_trackings = []
     st = []
     for i in s:
         if 'onbo' in i:
             if 'start' in i:
                 st.append('1-Onboarding + Retorno')
             elif 'segment' in i:
-                st.append('1.1-Opcional-Onboarding escolha de bot')
+                st.append('Opcional-Onboarding escolha de bot')
             else:
                 st.append(nan)
+        elif 'product-selection' in i:
+            st.append('Opcional-Seleciona produto')
         elif 'product-availability' in i:
             if 'cpf-request' in i:
                 st.append('3-Informa localizacao e cpf')
             elif 'cpf-validation' in i:
                 st.append('3.1-CPF valido (V.2.0)')
-            elif 'health-api-orders-validation' in i:
-                st.append('3.2-Consulta orders (V.2.1.1)')
-            elif 'api-residential-customer-contracts-open-request-validation' in i:
-                st.append('3.3-Consulta customer contracts (V.2.1.2)')
             elif 'postalcode-request' in i:
-                st.append('3.4-Obtencao de CEP')
-            elif 'postalcode-validation' in i:
-                st.append('3.5-CEP valido (V.2.2)')
+                st.append('3.2-Obtencao de CEP')
+            elif 'postalcode-validation options' in i:
+                st.append('3.3-CEP valido (V.2.2)')
             elif 'postalcode-validation-true' in i:
-                st.append('3.6-Pegando complemento')
+                st.append('3.4-Passa endereco')
             elif 'health-api-address-validation' in i:
-                st.append('3.7-Endereco sendo validado (V.2.3)')
-            elif 'empty-public-space-validation' in i:
-                st.append('3.8-Validacao de logradouro (V.2.4)')
-            elif 'empty-neighborhood-validation' in i:
-                st.append('3.9-Bairro sendo validado (V.2.3)')
+                st.append('3.5-Endereco valida (V.2.3)')
             elif 'address-confirmation' in i:
-                st.append('3.9.1-Endereco resumido')
+                st.append('3.6-Endereco resumido')
             elif 'health-api-residential-customer-contracts-validation' in i:
-                st.append('3.9.2-Consulta de CPF na api de base (V.2.9)')
+                st.append('3.7-Consulta de CPF na api de base(V.2.9)')
             elif 'client-validation' in i:
-                st.append('3.9.3-Localizado na api de base validacao (V.2.10)')
+                st.append('3.8-Localizado na api de base (V.2.10)')
             elif 'product-availability-validation' in i:
-                st.append('3.9.4-Produto e disponibilizado na regiao (V.2.11)')
+                st.append('3.9-Produto e disponibilizado na regiao (V.2.12)')
             elif 'health-api-plan-availability-validation' in i:
-                st.append('3.9.5-Consulta na api de catalogos(V.2.13)')
+                st.append('3.9.1-Consulta na api de catalogos(V.2.13)')
             elif 'plans-available-catalog-validation' in i:
-                st.append('3.9.6-Plano disponivel no catalogo (V.2.14)')
+                st.append('3.9.2-Plano disponivel no catalogo (V.2.14)')
             else:
                 st.append(nan)
         elif 'plan-selection' in i:
             st.append('4-Escolhe plano (Todos produtos)')
         elif 'registration' in i:
             if 'full-name-request' in i:
                 st.append('5-Realiza cadastro')
@@ -271,14 +265,8 @@
                 e.append(nan)
         else:
             e.append(nan)
     if any([i is not nan for i in e]):
         info('Aviso: Tivemos erros no bot :(')
     return e
 
-# Migrar para outro lambda
-def get_rid_of_undefined(df:Type) -> Type:
-    """
-    Ver com vini, capacidade extracao
-    """
-    pass
```

### Comparing `etl_csm-0.0.9/Etl/__init__.py` & `etl_csm-0.1.0/Etl/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from Etl.Execute import Runner
 from Etl.Extrator import (
-    Connection,
+    form_df_tracking,
     form_df_extras
 )
 from Etl.Helper import (
     timing,
     helper_columns,
     psql_insert_copy,
-
+    map_substring
 )
 from Etl.Treatment_extras import (
     patternizing_columns,
     ensure_nan_extras,
     fill_na_extras,
     dtype_extras,
-    patternizing_origins,
-    form_extras_plan,
 )
 from Etl.Treatment_tracking import (
-    ensure_dtypes,
+    fill_na_tracking,
     dtype_tracking,
     remove_test,
-    steps,
+    steps_residential,
     errors,
     flag_duplicated_tracks
 )
+
+from Etl.Treatment_tracking_pme import (
+    steps_pme
+)
+
 from Etl.Loader import (
     load_cloud
 )
```

### Comparing `etl_csm-0.0.9/LICENSE` & `etl_csm-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `etl_csm-0.0.9/PKG-INFO` & `etl_csm-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etl_csm
-Version: 0.0.9
+Version: 0.1.0
 Summary: Pacote de ETL
 Home-page: https://gitdev.clarobrasil.mobi/vendas-claro/csm/etl
 Author: ingloriamori
 Author-email: francisco.froes@globalhitss.com.br
 License: MIT
 Keywords: python,etl
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `etl_csm-0.0.9/README.md` & `etl_csm-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `etl_csm-0.0.9/etl_csm.egg-info/PKG-INFO` & `etl_csm-0.1.0/etl_csm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etl-csm
-Version: 0.0.9
+Version: 0.1.0
 Summary: Pacote de ETL
 Home-page: https://gitdev.clarobrasil.mobi/vendas-claro/csm/etl
 Author: ingloriamori
 Author-email: francisco.froes@globalhitss.com.br
 License: MIT
 Keywords: python,etl
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `etl_csm-0.0.9/setup.py` & `etl_csm-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.9'
+VERSION = '0.1.0'
 DESCRIPTION = 'Pacote de ETL'
 
 # Setting up
 setup(
     name = "etl_csm",
     version = VERSION,
     author = "ingloriamori",
```

