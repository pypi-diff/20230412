# Comparing `tmp/tvault-0.3.3-py3-none-any.whl.zip` & `tmp/tvault-0.3.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 9979 bytes, number of entries: 11
--rw-r--r--  2.0 unx     2813 b- defN 23-Apr-11 08:19 tvault/__init__.py
+Zip file size: 10358 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     2977 b- defN 23-Apr-12 04:48 tvault/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-03 04:19 tvault/model_diff.py
 -rw-r--r--  2.0 unx     4789 b- defN 23-Apr-03 06:15 tvault/model_log.py
 -rw-r--r--  2.0 unx     8055 b- defN 23-Apr-11 08:27 tvault/parse_utils.py
--rw-r--r--  2.0 unx    12900 b- defN 23-Apr-11 08:01 tvault/torchvault.py
--rw-r--r--  2.0 unx     1067 b- defN 23-Apr-11 08:28 tvault-0.3.3.dist-info/LICENSE
--rw-r--r--  2.0 unx      380 b- defN 23-Apr-11 08:28 tvault-0.3.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 08:28 tvault-0.3.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 23-Apr-11 08:28 tvault-0.3.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-Apr-11 08:28 tvault-0.3.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      854 b- defN 23-Apr-11 08:28 tvault-0.3.3.dist-info/RECORD
-11 files, 31010 bytes uncompressed, 8539 bytes compressed:  72.5%
+-rw-r--r--  2.0 unx    14094 b- defN 23-Apr-12 04:43 tvault/torchvault.py
+-rw-r--r--  2.0 unx     1067 b- defN 23-Apr-12 04:48 tvault-0.3.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx      380 b- defN 23-Apr-12 04:48 tvault-0.3.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 04:48 tvault-0.3.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 23-Apr-12 04:48 tvault-0.3.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-12 04:48 tvault-0.3.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      854 b- defN 23-Apr-12 04:48 tvault-0.3.4.dist-info/RECORD
+11 files, 32368 bytes uncompressed, 8918 bytes compressed:  72.4%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: tvault/parse_utils.py
 Comment: 
 
 Filename: tvault/torchvault.py
 Comment: 
 
-Filename: tvault-0.3.3.dist-info/LICENSE
+Filename: tvault-0.3.4.dist-info/LICENSE
 Comment: 
 
-Filename: tvault-0.3.3.dist-info/METADATA
+Filename: tvault-0.3.4.dist-info/METADATA
 Comment: 
 
-Filename: tvault-0.3.3.dist-info/WHEEL
+Filename: tvault-0.3.4.dist-info/WHEEL
 Comment: 
 
-Filename: tvault-0.3.3.dist-info/entry_points.txt
+Filename: tvault-0.3.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: tvault-0.3.3.dist-info/top_level.txt
+Filename: tvault-0.3.4.dist-info/top_level.txt
 Comment: 
 
-Filename: tvault-0.3.3.dist-info/RECORD
+Filename: tvault-0.3.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tvault/__init__.py

```diff
@@ -23,31 +23,33 @@
 
 def diff(sha1="", index1=-1, sha2="", index2=-1, ask_gpt=False, log_dir="./model_log"):
     # def diff(self, sha1="", index1=-1, sha2="", index2=-1, out=False, ask_gpt=False)
     vault = TorchVault(log_dir)
     vault.diff(sha1, index1, sha2, index2, ask_gpt)
 
 
-def add_tag(tag="", sha="", log_dir="./model_log"):
+def add_tag(tag_type="", tag="", sha="", log_dir="./model_log"):
+    # def add_tag(self, sha="", tag_type="", tag="", idx=None)
     vault = TorchVault(log_dir)
-    vault.add_tag(sha, tag)
+    vault.add_tag(sha, tag_type, tag)
 
 
 def add_result(result=0, sha="", log_dir="./model_log"):
     vault = TorchVault(log_dir)
     vault.add_result(sha, result)
 
 
-def log_all(model, tag="", result=-1, optimizer=None, log_dir="./model_log", model_dir="./"):
+# tags should be a dictionary of key, value pairs
+def log_all(model, tags="", result=-1, optimizer=None, log_dir="./model_log", model_dir="./"):
     vault = TorchVault(log_dir, model_dir)
     vault.log_model(model)
     if optimizer is not None:
         vault.log_optimizer(optimizer)
-    if tag is not "":
-        vault.add_tag("", tag)
+    for tag_type, tag in tags.items():
+        vault.add_tag("", tag_type, tag)
     if result is not -1:
         vault.add_result("", result)
 
 
 """
 Other utils
 """
```

## tvault/torchvault.py

```diff
@@ -78,50 +78,48 @@
 
     """
     add tag to model log, commit sha may be from previous results.
     if idx is set to -1, all models in the commit hash are tagged.
     if idx is set to None, tag of most recent model is changed.
     """
 
-    def add_tag(self, sha="", tag="", idx=None):
+    def add_tag(self, sha="", tag_type="", tag="", idx=None):
         # if commit hash is not given, use current commit hash
         model_log = self.read_model_log(sha)
-        print(f"add tag: got model_log {model_log}")
         if len(model_log.keys()) == 0:
             print(f"tvault error: model log with commit hash {sha} does not exist.")
             raise TorchVaultError
 
         if idx == -1:
             target_idxs = list(range(len(model_log.keys())))
         elif idx == None:
             target_idxs = [len(model_log.keys()) - 1]
             print(f"add tags: {target_idxs}")
         else:
             target_idxs = [idx]
 
         for model_idx in target_idxs:
-            if "tag" in model_log[model_idx].keys():
+            if f"tag-{tag_type}" in model_log[model_idx].keys():
                 print(
-                    f"tvault: changing tag from {model_log[model_idx]['tag']} to {tag} for model {sha}"
+                    f"tvault: changing tag from {model_log[model_idx][f'tag-{tag_type}']} to {tag} for model {sha}"
                 )
             else:
                 print(f"tvault: setting tag {tag} for model {sha}")
-            model_log[model_idx]["tag"] = tag
+            model_log[model_idx][f"tag-{tag_type}"] = tag
         self.write_model_log(sha, model_log)
 
     """
     add result to model log, commit sha may be from previous results.
     if idx is set to -1, all models in the commit hash are tagged.
     if idx is set to None, tag of most recent model is changed.
     """
 
     def add_result(self, sha="", result=0, idx=None):
         # if commit hash is not given, use current commit hash
         model_log = self.read_model_log(sha)
-        print(f"add result: got model_log {model_log}")
         if len(model_log.keys()) == 0:
             print(f"tvault error: model log with commit hash {sha} does not exist.")
             raise TorchVaultError
 
         if idx == -1:
             target_idxs = list(range(len(model_log.keys())))
         elif idx == None:
@@ -189,14 +187,16 @@
     Basic diff calculator between two pytorch models.
     sha1: commit hash of previous model, must be set. (for now)
     index1: model index of model in commit hash sha1. If not set, use latest.
     sha2: commit hash of current model, must be set. (for now)
     index2: model index of model in commit hash sha2. If not set, use latest.
     out: if out flag is set, writes out
     ask_gpt: if ask_gpt is set, asks gpt for difference summary.
+
+    0412: Custom keys should not be considered when calculating diff.
     """
 
     def diff(self, sha1="", index1=-1, sha2="", index2=-1, ask_gpt=False):
         prev_model = self.read_model_log(sha1)
         cur_model = self.read_model_log(sha2)
         if len(prev_model.keys()) == 0:
             print(f"tvault error: sha1 argument must be provided.")
@@ -258,17 +258,20 @@
         print("=" * 40 + "ChatGPT Answer" + "=" * 40)
         print(answer)
         return
 
     """
     find models using either commit hash, tag, or result
     should find suitable models and return list of [hash, model index, tag, result].
+    Find models by that with custom keys, show result with such custom key
+
+    이거 refactoring: multi tag 가능하도록.
     """
 
-    def find(self, condition="hash", hash="", tag="", min=0, max=100):
+    def find(self, condition="hash", hash="", tag_type="", tag="", min=0, max=100):
         target_models = []
         if os.path.exists(self.log_dir):
             if len(os.listdir(self.log_dir)) == 0:
                 print(f"tvault error: log dir is empty")
                 raise TorchVaultError
             if condition == "hash":
                 if hash == "":
@@ -276,60 +279,92 @@
                     raise TorchVaultError
                 if os.path.exists(f"{self.log_dir}/model_{hash}"):
                     model_log = self.read_model_log(hash)
                     print(
                         f"tvault: model {hash} exists! - contains {len(model_log.keys())} experiments"
                     )
                     for model_idx, model in model_log.items():
-                        model_info = [hash, model_idx]
-                        if "tag" in model.keys():
-                            model_info.append(model["tag"])
-                        else:
-                            model_info.append("")
+                        model_info = {"HASH": hash, "MODEL-IDX": model_idx}
+                        for k, v in model.items():
+                            if "tag-" in k:
+                                model_info[k] = v
                         if "result" in model.keys():
-                            model_info.append(model["result"])
-                        else:
-                            model_info.append(-1)
+                            model_info["RESULT"] = model["result"]
+
                         target_models.append(model_info)
 
                 else:
                     print(f"tvault: model {hash} does not exist.")
             elif condition == "tag":
                 for model in os.listdir(self.log_dir):
                     with open(f"{self.log_dir}/{model}", "rb") as f:
                         model_log = pickle.load(f)
                     for model_idx, v in model_log.items():
-                        model_info = []
-                        if "tag" in v.keys() and v["tag"] == tag:
-                            model_info = [model, model_idx, v["tag"]]
+                        model_info = dict()
+
+                        if f"tag-{tag_type}" in v.keys() and v[f"tag-{tag_type}"] == tag:
+                            model_info = {
+                                "HASH": model,
+                                "MODEL-IDX": model_idx,
+                            }
                             if "result" in v.keys():
-                                model_info.append(v["result"])
-                            else:
-                                model_info.append(-1)
+                                model_info["RESULT"] = v["result"]
+
+                            # other tags
+                            for m_k, m_v in model.items():
+                                if "tag-" in m_k:
+                                    model_info[m_k] = m_v
                             target_models.append(model_info)
             elif condition == "result":
                 for model in os.listdir(self.log_dir):
                     with open(f"{self.log_dir}/{model}", "rb") as f:
                         model_log = pickle.load(f)
                     for model_idx, v in model_log.items():
-                        model_info = []
+                        model_info = dict()
+
                         if "result" in v.keys() and min <= v["result"] <= max:
-                            if "tag" in v.keys():
-                                model_info = [model, model_idx, v["tag"], v["result"]]
-                            else:
-                                model_info = [model, model_idx, "", v["result"]]
+                            model_info = {
+                                "HASH": model,
+                                "MODEL-IDX": model_idx,
+                                "RESULT": v["result"],
+                            }
+                            # other tags
+                            for m_k, m_v in model.items():
+                                if "tag-" in m_k:
+                                    model_info[m_k] = m_v
+
                             target_models.append(model_info)
             else:
                 print(f"tvault error:condition other than [hash, tag, result] is not supported.")
                 raise TorchVaultError
         return target_models
 
     def show_result(self, target_models):
         if len(target_models) == 0:
             print(f"tvault: no model satisfying the conditions")
             return
 
-        table = ["HASH", "MODEL-IDX", "TAG", "RESULT"]
-        tab = PrettyTable(table)
+        # find model log with most tags.
+        table = []
         for e in target_models:
+            if len(list(e.keys())) > len(table):
+                table = list(e.keys())
+
+        # table should be sorted here
+        sorted_table = ["HASH", "MODEL-IDX"]
+        for e in table:
+            if e.startswith("tag-"):
+                sorted_table.append(e.split("tag-")[1])
+        sorted_table.append("RESULT")
+
+        # table contains model_log keys with most tags
+        # should represent [hash, model idx, tag1, tag2, tag3, result] order.
+        tab = PrettyTable(sorted_table)
+        for e in target_models:
+            row = []
+            for k in sorted_table:
+                if k in e.keys():
+                    row.append(e[k])
+                else:
+                    row.append("")
             tab.add_row(e)
         print(tab)
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `tvault-0.3.3.dist-info/LICENSE` & `tvault-0.3.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tvault-0.3.3.dist-info/RECORD` & `tvault-0.3.4.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-tvault/__init__.py,sha256=oocr8VVcaYKVPGZXb41p0SLC55lKye9ZW_C96YRBvmI,2813
+tvault/__init__.py,sha256=Hg6qQlAM1KGMIDYrOSWD1zk_NwLhsVwf3jWYpwPGAAw,2977
 tvault/model_diff.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tvault/model_log.py,sha256=ZD1LeL1wBRKQEZaAfZEcjYP7w76yeD0eMRAnI-fBOiA,4789
 tvault/parse_utils.py,sha256=rxESYl0qdIlmi4xFQo7G7IPI4sofHOXBduYjibFb50o,8055
-tvault/torchvault.py,sha256=Vx33rt8ZRJHf_gobUyJQfxItbjxs-coXBYLfK-Y1mWM,12900
-tvault-0.3.3.dist-info/LICENSE,sha256=WMAFuHtOPuSTgn-WJtxM1LLEDLfqaKQes7X7VhOaaOU,1067
-tvault-0.3.3.dist-info/METADATA,sha256=CY_i36AlOvNltDTS0VvrQBJY-ydTGOPNjaX35kX8RTI,380
-tvault-0.3.3.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-tvault-0.3.3.dist-info/entry_points.txt,sha256=wdQKlmNgZH12ukkn44_90k6m4AgiW-MzRTo14Cf2RSc,53
-tvault-0.3.3.dist-info/top_level.txt,sha256=Z1ZnwpooKsyvyYmlAXuGVOIRK1hO7QkkDVaneY85JDI,7
-tvault-0.3.3.dist-info/RECORD,,
+tvault/torchvault.py,sha256=CNwxysUfHjnXxfjod63-ak6cC-MkZGp2XC6YOC5YYjc,14094
+tvault-0.3.4.dist-info/LICENSE,sha256=WMAFuHtOPuSTgn-WJtxM1LLEDLfqaKQes7X7VhOaaOU,1067
+tvault-0.3.4.dist-info/METADATA,sha256=8gptZCtR8WZSG-iHlumosOFqQiingEbRTe_g6Z-wAtE,380
+tvault-0.3.4.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+tvault-0.3.4.dist-info/entry_points.txt,sha256=wdQKlmNgZH12ukkn44_90k6m4AgiW-MzRTo14Cf2RSc,53
+tvault-0.3.4.dist-info/top_level.txt,sha256=Z1ZnwpooKsyvyYmlAXuGVOIRK1hO7QkkDVaneY85JDI,7
+tvault-0.3.4.dist-info/RECORD,,
```

