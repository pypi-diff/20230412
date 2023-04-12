# Comparing `tmp/supex-2023.2.9.tar.gz` & `tmp/supex-2023.4.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/supex-2023.2.9.tar", last modified: Fri Feb 10 02:28:15 2023, max compression
+gzip compressed data, was "dist/supex-2023.4.12.tar", last modified: Wed Apr 12 11:22:15 2023, max compression
```

## Comparing `supex-2023.2.9.tar` & `supex-2023.4.12.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-10 02:28:15.000000 supex-2023.2.9/
--rw-r--r--   0 runner    (1001) docker     (116)     1090 2023-02-10 02:28:10.000000 supex-2023.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      669 2023-02-10 02:28:10.000000 supex-2023.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-10 02:28:15.000000 supex-2023.2.9/supex/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-10 02:28:15.000000 supex-2023.2.9/supex/utils/
--rw-r--r--   0 runner    (1001) docker     (116)       13 2023-02-10 02:28:10.000000 supex-2023.2.9/supex/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       39 2023-02-10 02:28:10.000000 supex-2023.2.9/supex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-10 02:28:15.000000 supex-2023.2.9/supex/models/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-10 02:28:15.000000 supex-2023.2.9/supex/models/reco/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-10 02:28:15.000000 supex-2023.2.9/supex/models/reco/sequential/
--rw-r--r--   0 runner    (1001) docker     (116)     5770 2023-02-10 02:28:10.000000 supex-2023.2.9/supex/models/reco/sequential/big_recbole_model.py
--rw-r--r--   0 runner    (1001) docker     (116)       91 2023-02-10 02:28:10.000000 supex-2023.2.9/supex/models/reco/sequential/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       13 2023-02-10 02:28:10.000000 supex-2023.2.9/supex/models/reco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       13 2023-02-10 02:28:10.000000 supex-2023.2.9/supex/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1133 2023-02-10 02:28:15.000000 supex-2023.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1049 2023-02-10 02:28:10.000000 supex-2023.2.9/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-02-10 02:28:15.000000 supex-2023.2.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-10 02:28:15.000000 supex-2023.2.9/supex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)        6 2023-02-10 02:28:15.000000 supex-2023.2.9/supex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1133 2023-02-10 02:28:15.000000 supex-2023.2.9/supex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)       26 2023-02-10 02:28:15.000000 supex-2023.2.9/supex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)      358 2023-02-10 02:28:15.000000 supex-2023.2.9/supex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-02-10 02:28:15.000000 supex-2023.2.9/supex.egg-info/dependency_links.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 11:22:15.000000 supex-2023.4.12/
+-rw-r--r--   0 runner    (1001) docker     (122)     1134 2023-04-12 11:22:15.000000 supex-2023.4.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-12 11:22:08.000000 supex-2023.4.12/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-12 11:22:15.000000 supex-2023.4.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-04-12 11:22:08.000000 supex-2023.4.12/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 11:22:15.000000 supex-2023.4.12/supex/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 11:22:15.000000 supex-2023.4.12/supex/models/
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-12 11:22:08.000000 supex-2023.4.12/supex/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 11:22:15.000000 supex-2023.4.12/supex/models/reco/
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-12 11:22:08.000000 supex-2023.4.12/supex/models/reco/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 11:22:15.000000 supex-2023.4.12/supex/models/reco/sequential/
+-rw-r--r--   0 runner    (1001) docker     (122)       91 2023-04-12 11:22:08.000000 supex-2023.4.12/supex/models/reco/sequential/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6676 2023-04-12 11:22:08.000000 supex-2023.4.12/supex/models/reco/sequential/big_recbole_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-04-12 11:22:08.000000 supex-2023.4.12/supex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 11:22:15.000000 supex-2023.4.12/supex/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-04-12 11:22:08.000000 supex-2023.4.12/supex/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11978 2023-04-12 11:22:08.000000 supex-2023.4.12/supex/utils/skt_hash.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 11:22:15.000000 supex-2023.4.12/supex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1134 2023-04-12 11:22:15.000000 supex-2023.4.12/supex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-04-12 11:22:15.000000 supex-2023.4.12/supex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      382 2023-04-12 11:22:15.000000 supex-2023.4.12/supex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-04-12 11:22:15.000000 supex-2023.4.12/supex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 11:22:15.000000 supex-2023.4.12/supex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1049 2023-04-12 11:22:08.000000 supex-2023.4.12/setup.py
```

### Comparing `supex-2023.2.9/LICENSE` & `supex-2023.4.12/LICENSE`

 * *Files identical despite different names*

### Comparing `supex-2023.2.9/README.md` & `supex-2023.4.12/README.md`

 * *Files identical despite different names*

### Comparing `supex-2023.2.9/supex/models/reco/sequential/big_recbole_model.py` & `supex-2023.4.12/supex/models/reco/sequential/big_recbole_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     """
 
     def __init__(
         self,
         model_name: str,
         model_version: str,
         data: pd.DataFrame,
+        data_type,
         user_id: str,
         item_id: str,
         timestamp: str,
         parameter_dict: dict = {},
         data_dir: str = None,
     ) -> None:
 
@@ -51,15 +52,14 @@
         else:
             os.makedirs(f"{data_dir}/{name}/")
 
         self.data_dir = data_dir
         self.user_id = user_id
         self.item_id = item_id
         self.timestamp = timestamp
-        self.data = data
         self.model_name = model_name
         self.name = name
 
         if parameter_dict:
             pass
         else:
             parameter_dict = {
@@ -70,38 +70,53 @@
                     "sample_num": 1,
                     "alpha": 1.0,
                     "dynamic": False,
                     "candidate_num": 0,
                 },
                 "MAX_ITEM_LIST_LENGTH": 20,
                 "eval_args": {
-                    "split": {"RS": [0.8, 0.1, 0.1]},
-                    "order": "RO",
+                    "split": {"LS": 'valid_and_test'},
+                    "order": "TO",
                     "group_by": "user",
-                    "mode": "full",
+                    "mode": "uni100",
                 },
             }
 
         parameter_dict.update(
             {
                 "data_path": f"{self.data_dir}",
                 "USER_ID_FIELD": f"{self.user_id}",
                 "ITEM_ID_FIELD": f"{self.item_id}",
                 "TIME_FIELD": f"{self.timestamp}",
-                "load_col": {"inter": [self.user_id, self.item_id, self.timestamp]},
+#                 "load_col": {"inter": [self.user_id, self.item_id, self.timestamp]},
             }
         )
         self.parameter_dict = parameter_dict
 
-        data_rename = data.rename(
-            columns={user_id: "user_id:token", item_id: "item_id:token", timestamp: "timestamp:float"}
-        )
-        data_rename[["user_id:token", "item_id:token", "timestamp:float"]].to_csv(
-            f"{data_dir}/{name}/{name}.inter", index=False, sep="\t"
-        )
+        if data_type:
+            re_col = {}
+            for i in data_type:
+                for j in data_type[i]:
+                    re_col[j] = f"{j}:{i}"
+
+            for key, value in data.items():
+                data[key] = value.rename(columns=re_col)
+                cols = [i for i in data[key].columns if i in list(re_col.values())]
+                data[key][cols].to_csv(f"{data_dir}/{name}/{name}.{key}", index=False, sep="\t")
+        else:
+            for key, value in data.items():
+                data[key] = value.rename(
+                    columns={user_id: "user_id:token", item_id: "item_id:token", timestamp: "timestamp:float"}
+                )
+                data[key][["user_id:token", "item_id:token", "timestamp:float"]].to_csv(
+                    f"{data_dir}/{name}/{name}.{key}", index=False, sep="\t"
+                )
+
+        self.data = data
+        self.re_col = re_col
 
     def _preprocessing(self):
         config = Config(model=self.model_name, dataset=self.name, config_dict=self.parameter_dict)
 
         # init random seed
         init_seed(config["seed"], config["reproducibility"])
 
@@ -123,24 +138,25 @@
 
         self.config = config
         return train_data, valid_data, test_data
 
     def _fit(
         self,
         train_data,
+        valid_data,
     ):
         # model loading and initialization
         seq_reco = getattr(sequential_model, self.model_name)
         self.model = seq_reco(self.config, train_data.dataset).to(self.config["device"])
 
         # trainer loading and initialization
         self.trainer = Trainer(self.config, self.model)
 
         # model training
-        best_valid_score, best_valid_result = self.trainer.fit(train_data)
+        best_valid_score, best_valid_result = self.trainer.fit(train_data, valid_data)
         return best_valid_score
 
     def _predict(
         self,
         test_data,
         nums=10,
         topk=10,
@@ -164,10 +180,17 @@
         return result
 
     def fit_predict(
         self,
         nums=10,
         topk=10,
     ):
-        train_data, valid_data, test_data = self._preprocessing()
-        self._fit(train_data)
-        return self._predict(test_data, nums, topk)
+        self.train_data, self.valid_data, self.test_data = self._preprocessing()
+        self._fit(self.train_data, self.valid_data)
+        return self._predict(self.test_data, nums, topk)
+
+    def get_evaluation(
+        self,
+    ):
+        self.train_data, self.valid_data, self.test_data = self._preprocessing()
+        self._fit(self.train_data, self.valid_data)
+        return self.trainer.evaluate(self.test_data)
```

### Comparing `supex-2023.2.9/PKG-INFO` & `supex-2023.4.12/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supex
-Version: 2023.2.9
+Version: 2023.4.12
 Summary: skt_ca_team library
 Home-page: https://github.com/sktaiflow/advanced_analytics
 Author: skt_ca_team
 Author-email: rbska56455@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `supex-2023.2.9/setup.py` & `supex-2023.4.12/setup.py`

 * *Files identical despite different names*

### Comparing `supex-2023.2.9/supex.egg-info/PKG-INFO` & `supex-2023.4.12/supex.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supex
-Version: 2023.2.9
+Version: 2023.4.12
 Summary: skt_ca_team library
 Home-page: https://github.com/sktaiflow/advanced_analytics
 Author: skt_ca_team
 Author-email: rbska56455@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

