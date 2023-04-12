# Comparing `tmp/hitrustai_lab-1.0.8.tar.gz` & `tmp/hitrustai_lab-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hitrustai_lab-1.0.8.tar", last modified: Fri Sep 16 06:34:21 2022, max compression
+gzip compressed data, was "hitrustai_lab-1.0.9.tar", last modified: Fri Sep 16 06:40:05 2022, max compression
```

## Comparing `hitrustai_lab-1.0.8.tar` & `hitrustai_lab-1.0.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 06:34:21.364001 hitrustai_lab-1.0.8/
--rw-r--r--   0 root         (0) root         (0)     1077 2022-08-24 02:15:26.000000 hitrustai_lab-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      210 2022-09-16 06:34:21.364001 hitrustai_lab-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11066 2022-08-23 05:30:57.000000 hitrustai_lab-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 06:34:21.364001 hitrustai_lab-1.0.8/hitrustai_lab/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 06:34:21.364001 hitrustai_lab-1.0.8/hitrustai_lab/algorithm/
--rw-r--r--   0 root         (0) root         (0)     3683 2022-07-27 09:32:46.000000 hitrustai_lab-1.0.8/hitrustai_lab/algorithm/ahp.py
--rw-r--r--   0 root         (0) root         (0)     1794 2022-08-23 05:18:59.000000 hitrustai_lab-1.0.8/hitrustai_lab/algorithm/score_translate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 06:34:21.364001 hitrustai_lab-1.0.8/hitrustai_lab/elk/
--rw-r--r--   0 root         (0) root         (0)    14036 2022-09-16 03:47:14.000000 hitrustai_lab-1.0.8/hitrustai_lab/elk/modual_core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 06:34:21.364001 hitrustai_lab-1.0.8/hitrustai_lab/knoweloge_base/
--rw-r--r--   0 root         (0) root         (0)     2367 2022-08-03 02:41:49.000000 hitrustai_lab-1.0.8/hitrustai_lab/knoweloge_base/call_useranent_so.py
--rw-r--r--   0 root         (0) root         (0)      285 2022-08-03 02:41:49.000000 hitrustai_lab-1.0.8/hitrustai_lab/knoweloge_base/geoip.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 06:34:21.364001 hitrustai_lab-1.0.8/hitrustai_lab/matrix/
--rw-r--r--   0 root         (0) root         (0)     2219 2022-07-27 09:55:11.000000 hitrustai_lab-1.0.8/hitrustai_lab/matrix/model_matrix.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 06:34:21.364001 hitrustai_lab-1.0.8/hitrustai_lab/model_train/
--rw-r--r--   0 root         (0) root         (0)     9874 2022-08-18 07:51:16.000000 hitrustai_lab-1.0.8/hitrustai_lab/model_train/ai_module_train.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 06:34:21.364001 hitrustai_lab-1.0.8/hitrustai_lab/model_train/core/
--rw-r--r--   0 root         (0) root         (0)     2138 2022-08-17 06:03:24.000000 hitrustai_lab-1.0.8/hitrustai_lab/model_train/core/message.py
--rw-r--r--   0 root         (0) root         (0)     2654 2022-08-23 02:28:34.000000 hitrustai_lab-1.0.8/hitrustai_lab/model_train/core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 06:34:21.364001 hitrustai_lab-1.0.8/hitrustai_lab/mysql/
--rw-r--r--   0 root         (0) root         (0)      354 2022-07-27 03:22:50.000000 hitrustai_lab-1.0.8/hitrustai_lab/mysql/connenction_db.py
--rw-r--r--   0 root         (0) root         (0)     2462 2022-08-03 02:41:49.000000 hitrustai_lab-1.0.8/hitrustai_lab/mysql/get_db_to_csv_batch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 06:34:21.364001 hitrustai_lab-1.0.8/hitrustai_lab/orm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 06:34:21.364001 hitrustai_lab-1.0.8/hitrustai_lab/orm/Tables/
--rw-r--r--   0 root         (0) root         (0)    25586 2022-08-03 02:41:49.000000 hitrustai_lab-1.0.8/hitrustai_lab/orm/Tables/TB3DS.py
--rw-r--r--   0 root         (0) root         (0)     9500 2022-08-03 02:41:49.000000 hitrustai_lab-1.0.8/hitrustai_lab/orm/Tables/TBDiiA.py
--rw-r--r--   0 root         (0) root         (0)     2535 2022-09-16 02:34:56.000000 hitrustai_lab-1.0.8/hitrustai_lab/orm/Tables/TBMarchant.py
--rw-r--r--   0 root         (0) root         (0)     2241 2022-08-03 02:41:49.000000 hitrustai_lab-1.0.8/hitrustai_lab/orm/Tables/TBreport.py
--rw-r--r--   0 root         (0) root         (0)     6021 2022-08-03 02:41:49.000000 hitrustai_lab-1.0.8/hitrustai_lab/orm/Tables/TBtransaction.py
--rw-r--r--   0 root         (0) root         (0)     6434 2022-09-16 06:33:50.000000 hitrustai_lab-1.0.8/hitrustai_lab/orm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 06:34:21.364001 hitrustai_lab-1.0.8/hitrustai_lab.egg-info/
--rw-r--r--   0 root         (0) root         (0)      210 2022-09-16 06:34:21.000000 hitrustai_lab-1.0.8/hitrustai_lab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      831 2022-09-16 06:34:21.000000 hitrustai_lab-1.0.8/hitrustai_lab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-16 06:34:21.000000 hitrustai_lab-1.0.8/hitrustai_lab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      233 2022-09-16 06:34:21.000000 hitrustai_lab-1.0.8/hitrustai_lab.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-09-16 06:34:21.364001 hitrustai_lab-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      937 2022-09-16 06:34:18.000000 hitrustai_lab-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 06:40:05.765481 hitrustai_lab-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)     1077 2022-08-24 02:15:26.000000 hitrustai_lab-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      210 2022-09-16 06:40:05.765481 hitrustai_lab-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11066 2022-08-23 05:30:57.000000 hitrustai_lab-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 06:40:05.761482 hitrustai_lab-1.0.9/hitrustai_lab/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 06:40:05.765481 hitrustai_lab-1.0.9/hitrustai_lab/algorithm/
+-rw-r--r--   0 root         (0) root         (0)     3683 2022-07-27 09:32:46.000000 hitrustai_lab-1.0.9/hitrustai_lab/algorithm/ahp.py
+-rw-r--r--   0 root         (0) root         (0)     1794 2022-08-23 05:18:59.000000 hitrustai_lab-1.0.9/hitrustai_lab/algorithm/score_translate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 06:40:05.765481 hitrustai_lab-1.0.9/hitrustai_lab/elk/
+-rw-r--r--   0 root         (0) root         (0)    14032 2022-09-16 06:39:35.000000 hitrustai_lab-1.0.9/hitrustai_lab/elk/modual_core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 06:40:05.765481 hitrustai_lab-1.0.9/hitrustai_lab/knoweloge_base/
+-rw-r--r--   0 root         (0) root         (0)     2367 2022-08-03 02:41:49.000000 hitrustai_lab-1.0.9/hitrustai_lab/knoweloge_base/call_useranent_so.py
+-rw-r--r--   0 root         (0) root         (0)      285 2022-08-03 02:41:49.000000 hitrustai_lab-1.0.9/hitrustai_lab/knoweloge_base/geoip.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 06:40:05.765481 hitrustai_lab-1.0.9/hitrustai_lab/matrix/
+-rw-r--r--   0 root         (0) root         (0)     2219 2022-07-27 09:55:11.000000 hitrustai_lab-1.0.9/hitrustai_lab/matrix/model_matrix.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 06:40:05.765481 hitrustai_lab-1.0.9/hitrustai_lab/model_train/
+-rw-r--r--   0 root         (0) root         (0)     9874 2022-08-18 07:51:16.000000 hitrustai_lab-1.0.9/hitrustai_lab/model_train/ai_module_train.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 06:40:05.765481 hitrustai_lab-1.0.9/hitrustai_lab/model_train/core/
+-rw-r--r--   0 root         (0) root         (0)     2138 2022-08-17 06:03:24.000000 hitrustai_lab-1.0.9/hitrustai_lab/model_train/core/message.py
+-rw-r--r--   0 root         (0) root         (0)     2654 2022-08-23 02:28:34.000000 hitrustai_lab-1.0.9/hitrustai_lab/model_train/core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 06:40:05.765481 hitrustai_lab-1.0.9/hitrustai_lab/mysql/
+-rw-r--r--   0 root         (0) root         (0)      354 2022-07-27 03:22:50.000000 hitrustai_lab-1.0.9/hitrustai_lab/mysql/connenction_db.py
+-rw-r--r--   0 root         (0) root         (0)     2462 2022-08-03 02:41:49.000000 hitrustai_lab-1.0.9/hitrustai_lab/mysql/get_db_to_csv_batch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 06:40:05.765481 hitrustai_lab-1.0.9/hitrustai_lab/orm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 06:40:05.765481 hitrustai_lab-1.0.9/hitrustai_lab/orm/Tables/
+-rw-r--r--   0 root         (0) root         (0)    25586 2022-08-03 02:41:49.000000 hitrustai_lab-1.0.9/hitrustai_lab/orm/Tables/TB3DS.py
+-rw-r--r--   0 root         (0) root         (0)     9500 2022-08-03 02:41:49.000000 hitrustai_lab-1.0.9/hitrustai_lab/orm/Tables/TBDiiA.py
+-rw-r--r--   0 root         (0) root         (0)     2535 2022-09-16 02:34:56.000000 hitrustai_lab-1.0.9/hitrustai_lab/orm/Tables/TBMarchant.py
+-rw-r--r--   0 root         (0) root         (0)     2241 2022-08-03 02:41:49.000000 hitrustai_lab-1.0.9/hitrustai_lab/orm/Tables/TBreport.py
+-rw-r--r--   0 root         (0) root         (0)     6021 2022-08-03 02:41:49.000000 hitrustai_lab-1.0.9/hitrustai_lab/orm/Tables/TBtransaction.py
+-rw-r--r--   0 root         (0) root         (0)     6434 2022-09-16 06:33:50.000000 hitrustai_lab-1.0.9/hitrustai_lab/orm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 06:40:05.765481 hitrustai_lab-1.0.9/hitrustai_lab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      210 2022-09-16 06:40:05.000000 hitrustai_lab-1.0.9/hitrustai_lab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      831 2022-09-16 06:40:05.000000 hitrustai_lab-1.0.9/hitrustai_lab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-16 06:40:05.000000 hitrustai_lab-1.0.9/hitrustai_lab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      233 2022-09-16 06:40:05.000000 hitrustai_lab-1.0.9/hitrustai_lab.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-16 06:40:05.765481 hitrustai_lab-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      937 2022-09-16 06:40:03.000000 hitrustai_lab-1.0.9/setup.py
```

### Comparing `hitrustai_lab-1.0.8/LICENSE` & `hitrustai_lab-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hitrustai_lab-1.0.8/README.md` & `hitrustai_lab-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `hitrustai_lab-1.0.8/hitrustai_lab/algorithm/ahp.py` & `hitrustai_lab-1.0.9/hitrustai_lab/algorithm/ahp.py`

 * *Files identical despite different names*

### Comparing `hitrustai_lab-1.0.8/hitrustai_lab/algorithm/score_translate.py` & `hitrustai_lab-1.0.9/hitrustai_lab/algorithm/score_translate.py`

 * *Files identical despite different names*

### Comparing `hitrustai_lab-1.0.8/hitrustai_lab/elk/modual_core.py` & `hitrustai_lab-1.0.9/hitrustai_lab/elk/modual_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             ))
 
     def get_update_data(self):
         info_start_point = self.ELK.get_start_time(self.INDEX_NAME['info'], date_col='pk_id')
         result_start_point = self.ELK.get_start_time(self.INDEX_NAME['result'], date_col='pk_id')
 
         if info_start_point is None:
-            info_data = self.orm.elk_elk_query_filter(self.dict_arg["orm_predict_info"], self.n_rows)
+            info_data = self.orm.elk_query_filter(self.dict_arg["orm_predict_info"], self.n_rows)
             result_data = self.orm.elk_query_filter(self.dict_arg["orm_predict_result"], self.n_rows)
         else:
             info_data = self.orm.elk_query_filter(self.dict_arg["orm_predict_info"], self.n_rows, (self.dict_arg["orm_predict_info"].pk_id > info_start_point))
             result_data = self.orm.elk_query_filter(self.dict_arg["orm_predict_result"], self.n_rows, (self.dict_arg["orm_predict_result"].pk_id > result_start_point))
 
         if info_data.shape[0] == 0 and result_data.shape[0] == 0:
             print(self.dict_arg["modual_name"] + ' Upload Complete ! ')
```

### Comparing `hitrustai_lab-1.0.8/hitrustai_lab/knoweloge_base/call_useranent_so.py` & `hitrustai_lab-1.0.9/hitrustai_lab/knoweloge_base/call_useranent_so.py`

 * *Files identical despite different names*

### Comparing `hitrustai_lab-1.0.8/hitrustai_lab/matrix/model_matrix.py` & `hitrustai_lab-1.0.9/hitrustai_lab/matrix/model_matrix.py`

 * *Files identical despite different names*

### Comparing `hitrustai_lab-1.0.8/hitrustai_lab/model_train/ai_module_train.py` & `hitrustai_lab-1.0.9/hitrustai_lab/model_train/ai_module_train.py`

 * *Files identical despite different names*

### Comparing `hitrustai_lab-1.0.8/hitrustai_lab/model_train/core/message.py` & `hitrustai_lab-1.0.9/hitrustai_lab/model_train/core/message.py`

 * *Files identical despite different names*

### Comparing `hitrustai_lab-1.0.8/hitrustai_lab/model_train/core/utils.py` & `hitrustai_lab-1.0.9/hitrustai_lab/model_train/core/utils.py`

 * *Files identical despite different names*

### Comparing `hitrustai_lab-1.0.8/hitrustai_lab/mysql/get_db_to_csv_batch.py` & `hitrustai_lab-1.0.9/hitrustai_lab/mysql/get_db_to_csv_batch.py`

 * *Files identical despite different names*

### Comparing `hitrustai_lab-1.0.8/hitrustai_lab/orm/Tables/TB3DS.py` & `hitrustai_lab-1.0.9/hitrustai_lab/orm/Tables/TB3DS.py`

 * *Files identical despite different names*

### Comparing `hitrustai_lab-1.0.8/hitrustai_lab/orm/Tables/TBDiiA.py` & `hitrustai_lab-1.0.9/hitrustai_lab/orm/Tables/TBDiiA.py`

 * *Files identical despite different names*

### Comparing `hitrustai_lab-1.0.8/hitrustai_lab/orm/Tables/TBMarchant.py` & `hitrustai_lab-1.0.9/hitrustai_lab/orm/Tables/TBMarchant.py`

 * *Files identical despite different names*

### Comparing `hitrustai_lab-1.0.8/hitrustai_lab/orm/Tables/TBreport.py` & `hitrustai_lab-1.0.9/hitrustai_lab/orm/Tables/TBreport.py`

 * *Files identical despite different names*

### Comparing `hitrustai_lab-1.0.8/hitrustai_lab/orm/Tables/TBtransaction.py` & `hitrustai_lab-1.0.9/hitrustai_lab/orm/Tables/TBtransaction.py`

 * *Files identical despite different names*

### Comparing `hitrustai_lab-1.0.8/hitrustai_lab/orm/__init__.py` & `hitrustai_lab-1.0.9/hitrustai_lab/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `hitrustai_lab-1.0.8/hitrustai_lab.egg-info/SOURCES.txt` & `hitrustai_lab-1.0.9/hitrustai_lab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hitrustai_lab-1.0.8/setup.py` & `hitrustai_lab-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,14 @@
     list_r = get_all_dir(i)
     if len(list_r) > 0:
         for ii in list_r:
             list_file.append(ii)
 
 setup(
     name='hitrustai_lab',
-    version='1.0.8',
+    version='1.0.9',
 
     url='https://gitlab.hitrustai.com/bruce60108010204/hitrustai-lab',
     author='Bruce Tsai',
     author_email='brcue60108010204@gmail.com',
     packages=list_file,
 )
```

