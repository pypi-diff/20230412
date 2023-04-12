# Comparing `tmp/ga_vqc-0.0.53.tar.gz` & `tmp/ga_vqc-0.0.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ga_vqc-0.0.53.tar", last modified: Tue Apr 11 06:33:37 2023, max compression
+gzip compressed data, was "ga_vqc-0.0.54.tar", last modified: Wed Apr 12 07:18:46 2023, max compression
```

## Comparing `ga_vqc-0.0.53.tar` & `ga_vqc-0.0.54.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 tsievert   (502) staff       (20)        0 2023-04-11 06:33:37.255360 ga_vqc-0.0.53/
--rw-r--r--   0 tsievert   (502) staff       (20)     1076 2023-02-08 00:23:26.000000 ga_vqc-0.0.53/LICENSE
--rw-r--r--   0 tsievert   (502) staff       (20)     1260 2023-04-11 06:33:37.254998 ga_vqc-0.0.53/PKG-INFO
--rw-r--r--   0 tsievert   (502) staff       (20)      791 2023-04-01 20:47:43.000000 ga_vqc-0.0.53/README.md
-drwxr-xr-x   0 tsievert   (502) staff       (20)        0 2023-04-11 06:33:37.251944 ga_vqc-0.0.53/ga_vqc/
--rw-r--r--   0 tsievert   (502) staff       (20)     1916 2023-04-09 06:07:20.000000 ga_vqc-0.0.53/ga_vqc/Distance.py
--rw-r--r--   0 tsievert   (502) staff       (20)      495 2023-03-23 02:52:56.000000 ga_vqc-0.0.53/ga_vqc/GA_ABC.py
--rw-r--r--   0 tsievert   (502) staff       (20)      565 2023-04-07 18:02:50.000000 ga_vqc-0.0.53/ga_vqc/GA_Manager.py
--rw-r--r--   0 tsievert   (502) staff       (20)     1007 2023-04-09 08:12:19.000000 ga_vqc-0.0.53/ga_vqc/GA_Support.py
--rw-r--r--   0 tsievert   (502) staff       (20)     2598 2023-04-07 17:34:26.000000 ga_vqc-0.0.53/ga_vqc/Genes.py
--rw-r--r--   0 tsievert   (502) staff       (20)      430 2023-03-23 02:52:56.000000 ga_vqc-0.0.53/ga_vqc/VQC_ABC.py
--rw-r--r--   0 tsievert   (502) staff       (20)      159 2023-04-10 20:43:29.000000 ga_vqc-0.0.53/ga_vqc/__init__.py
--rw-r--r--   0 tsievert   (502) staff       (20)    11033 2023-04-10 20:42:42.000000 ga_vqc-0.0.53/ga_vqc/simple_Individual.py
--rw-r--r--   0 tsievert   (502) staff       (20)    17986 2023-04-11 06:32:50.000000 ga_vqc-0.0.53/ga_vqc/simple_Model.py
-drwxr-xr-x   0 tsievert   (502) staff       (20)        0 2023-04-11 06:33:37.254488 ga_vqc-0.0.53/ga_vqc.egg-info/
--rw-r--r--   0 tsievert   (502) staff       (20)     1260 2023-04-11 06:33:37.000000 ga_vqc-0.0.53/ga_vqc.egg-info/PKG-INFO
--rw-r--r--   0 tsievert   (502) staff       (20)      357 2023-04-11 06:33:37.000000 ga_vqc-0.0.53/ga_vqc.egg-info/SOURCES.txt
--rw-r--r--   0 tsievert   (502) staff       (20)        1 2023-04-11 06:33:37.000000 ga_vqc-0.0.53/ga_vqc.egg-info/dependency_links.txt
--rw-r--r--   0 tsievert   (502) staff       (20)      132 2023-04-11 06:33:37.000000 ga_vqc-0.0.53/ga_vqc.egg-info/requires.txt
--rw-r--r--   0 tsievert   (502) staff       (20)        7 2023-04-11 06:33:37.000000 ga_vqc-0.0.53/ga_vqc.egg-info/top_level.txt
--rw-r--r--   0 tsievert   (502) staff       (20)       38 2023-04-11 06:33:37.255473 ga_vqc-0.0.53/setup.cfg
--rw-r--r--   0 tsievert   (502) staff       (20)     1067 2023-04-11 04:45:04.000000 ga_vqc-0.0.53/setup.py
+drwxr-xr-x   0 tsievert   (502) staff       (20)        0 2023-04-12 07:18:46.584390 ga_vqc-0.0.54/
+-rw-r--r--   0 tsievert   (502) staff       (20)     1076 2023-02-08 00:23:26.000000 ga_vqc-0.0.54/LICENSE
+-rw-r--r--   0 tsievert   (502) staff       (20)     1260 2023-04-12 07:18:46.583837 ga_vqc-0.0.54/PKG-INFO
+-rw-r--r--   0 tsievert   (502) staff       (20)      791 2023-04-01 20:47:43.000000 ga_vqc-0.0.54/README.md
+drwxr-xr-x   0 tsievert   (502) staff       (20)        0 2023-04-12 07:18:46.580911 ga_vqc-0.0.54/ga_vqc/
+-rw-r--r--   0 tsievert   (502) staff       (20)     2961 2023-04-12 07:16:30.000000 ga_vqc-0.0.54/ga_vqc/Distance.py
+-rw-r--r--   0 tsievert   (502) staff       (20)      495 2023-03-23 02:52:56.000000 ga_vqc-0.0.54/ga_vqc/GA_ABC.py
+-rw-r--r--   0 tsievert   (502) staff       (20)      565 2023-04-07 18:02:50.000000 ga_vqc-0.0.54/ga_vqc/GA_Manager.py
+-rw-r--r--   0 tsievert   (502) staff       (20)     1007 2023-04-09 08:12:19.000000 ga_vqc-0.0.54/ga_vqc/GA_Support.py
+-rw-r--r--   0 tsievert   (502) staff       (20)     3628 2023-04-12 07:04:03.000000 ga_vqc-0.0.54/ga_vqc/Genes.py
+-rw-r--r--   0 tsievert   (502) staff       (20)      430 2023-03-23 02:52:56.000000 ga_vqc-0.0.54/ga_vqc/VQC_ABC.py
+-rw-r--r--   0 tsievert   (502) staff       (20)      159 2023-04-10 20:43:29.000000 ga_vqc-0.0.54/ga_vqc/__init__.py
+-rw-r--r--   0 tsievert   (502) staff       (20)    11033 2023-04-12 04:03:14.000000 ga_vqc-0.0.54/ga_vqc/simple_Individual.py
+-rw-r--r--   0 tsievert   (502) staff       (20)    17990 2023-04-12 06:36:08.000000 ga_vqc-0.0.54/ga_vqc/simple_Model.py
+drwxr-xr-x   0 tsievert   (502) staff       (20)        0 2023-04-12 07:18:46.583233 ga_vqc-0.0.54/ga_vqc.egg-info/
+-rw-r--r--   0 tsievert   (502) staff       (20)     1260 2023-04-12 07:18:46.000000 ga_vqc-0.0.54/ga_vqc.egg-info/PKG-INFO
+-rw-r--r--   0 tsievert   (502) staff       (20)      357 2023-04-12 07:18:46.000000 ga_vqc-0.0.54/ga_vqc.egg-info/SOURCES.txt
+-rw-r--r--   0 tsievert   (502) staff       (20)        1 2023-04-12 07:18:46.000000 ga_vqc-0.0.54/ga_vqc.egg-info/dependency_links.txt
+-rw-r--r--   0 tsievert   (502) staff       (20)      132 2023-04-12 07:18:46.000000 ga_vqc-0.0.54/ga_vqc.egg-info/requires.txt
+-rw-r--r--   0 tsievert   (502) staff       (20)        7 2023-04-12 07:18:46.000000 ga_vqc-0.0.54/ga_vqc.egg-info/top_level.txt
+-rw-r--r--   0 tsievert   (502) staff       (20)       38 2023-04-12 07:18:46.584529 ga_vqc-0.0.54/setup.cfg
+-rw-r--r--   0 tsievert   (502) staff       (20)     1067 2023-04-12 07:18:23.000000 ga_vqc-0.0.54/setup.py
```

### Comparing `ga_vqc-0.0.53/LICENSE` & `ga_vqc-0.0.54/LICENSE`

 * *Files identical despite different names*

### Comparing `ga_vqc-0.0.53/PKG-INFO` & `ga_vqc-0.0.54/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ga_vqc
-Version: 0.0.53
+Version: 0.0.54
 Summary: Genetic Algorithm for VQC ansatz search.
 Home-page: https://github.com/tcoulvert/GA_Ansatz_Search
 Author: Thomas Sievert
 Author-email: 63161166+tcoulvert@users.noreply.github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ga_vqc-0.0.53/README.md` & `ga_vqc-0.0.54/README.md`

 * *Files identical despite different names*

### Comparing `ga_vqc-0.0.53/ga_vqc/Distance.py` & `ga_vqc-0.0.54/ga_vqc/Distance.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import numpy as np
+from sklearn.decomposition import PCA
 from sklearn.manifold import TSNE
 
+
 def euclidean_distances(ansatz_comp, population, max_moments=None):
     vector_comp = create_vector(ansatz_comp, max_moments=max_moments)
     distances = []
     for ansatz in population:
         vector = create_vector(ansatz)
         distances.append(
             np.sum(
@@ -19,14 +21,18 @@
 
 def tsne(population, perplexity=2, rng_seed=None):
     vectors = []
     for ansatz in population:
         vectors.append(create_vector(ansatz))
     vectors = np.array(vectors)
     
+    if vectors.shape[1] > 100:
+        pca = PCA()
+        vectors = pca.fit_transform(vectors) 
+        
     t_sne = TSNE(
         n_components=2,
         perplexity=perplexity,
         init="random",
         n_iter=250,
         random_state=rng_seed,
     )
@@ -36,29 +42,50 @@
     return S_t_sne.T
 
 def create_vector(ansatz, max_moments=None):
     if max_moments is not None and ansatz.n_moments != max_moments:
         ansatz.add_moment('pad', num_pad=(max_moments - ansatz.n_moments))
 
     vector = []
+
     ### single-qubit gates ###
     for moment in range(ansatz.n_moments):
         for qubit in range(ansatz.n_qubits):
-            if ansatz[moment][qubit] == 'U3':
-                vector.append(1)
-            else:
-                vector.append(0)
+            one_qubit_states = []
+            for _ in range(
+                ansatz.genepool.n_gates(
+                    search_param={'n_qubits': 1}
+                )
+            ):
+                one_qubit_states.extend([0])
+            if ansatz.genepool.n_qubits(ansatz[moment][qubit]) != 1:
+                vector.extend([i for i in one_qubit_states])
+                continue
+            one_qubit_states[ansatz.genepool.index_of(ansatz[moment][qubit])] = 1 # Assumes 'I' always in index 0, and cannot NOT include 'I'
+            vector.extend([i for i in one_qubit_states])
 
-    ### 2-qubit gates (CNOT) ###
+    ### 2-qubit gates ###
     for moment in range(ansatz.n_moments):
-        # [(0,1), (0,2), (1,0), (1,2), (2,0), (2,1)]
-        two_qubit_pairs = [0, 0, 0, 0, 0, 0]
+        # [(0,1), (0,2), (1,0), (1,2), (2,0), (2,1), ('I', 'I')]
+        two_qubit_states = []
+        for _ in range(
+            ansatz.genepool.n_gates(
+                search_param={'n_qubits': 2}
+            )
+        ):
+            two_qubit_states.extend([0 for __ in range(np.math.factorial(ansatz.n_qubits) + 1)])
+            two_qubit_states[-1] = 1
+        
         for qubit in range(ansatz.n_qubits):
-            if ansatz[moment][qubit].find('_') > 0:
+            if ansatz[moment][qubit].find('_') > 0: # Doesn't work for passing more than 1 2-qubit gate, and only works for 'control'/'target' gates
+                two_qubit_states[-1] = 0
                 if ansatz[moment][qubit][-3] == 'C':
-                    two_qubit_pairs[2*qubit] = 1
+                    two_qubit_states[2*qubit] = 1
                 elif ansatz[moment][qubit][-3] == 'T':
-                    two_qubit_pairs[2*qubit + 1] = 1
+                    two_qubit_states[2*qubit + 1] = 1
                 break
-        vector.extend(two_qubit_pairs)
+        vector.extend(two_qubit_states)
+
+    ### 3+ qubit gates ###
+    # TO DO
 
     return np.array(vector)
```

### Comparing `ga_vqc-0.0.53/ga_vqc/GA_Manager.py` & `ga_vqc-0.0.54/ga_vqc/GA_Manager.py`

 * *Files identical despite different names*

### Comparing `ga_vqc-0.0.53/ga_vqc/GA_Support.py` & `ga_vqc-0.0.54/ga_vqc/GA_Support.py`

 * *Files identical despite different names*

### Comparing `ga_vqc-0.0.53/ga_vqc/Genes.py` & `ga_vqc-0.0.54/ga_vqc/Genes.py`

 * *Files 13% similar despite different names*

```diff
@@ -37,21 +37,51 @@
             if gate.name == gate_name:
                 return gate.n_params
 
         raise Exception("Gate asked for not in genepool.")
 
     def n_qubits(self, gate_name) -> int:
         if gate_name is None:
-            raise Exception("Cannot look for None-type gate.") 
+            raise Exception("Cannot look for None-type gate.")
+        if gate_name[0] == 'C': # properly check for non-name gates -> change ansatz_dicts to adjacency matrix
+            return 2 
         for gate in self.gates:
             if gate.name == gate_name:
                 return gate.n_qubits
 
         raise Exception("Gate asked for not in genepool.")
 
+    def n_gates(self, search_param={}):
+        """
+        Returns total number of gates unless given another parameter to search for.
+        """
+        for k, v in search_param.items():
+            count = 0
+            if k == 'n_params':
+                for gate in self.gates:
+                    if gate.n_params == v:
+                        count += 1
+                return count
+            elif k == 'n_qubits':
+                for gate in self.gates:
+                    if gate.n_qubits == v:
+                        count += 1
+                return count
+
+        return len(self.gates)
+
+    def index_of(self, gate_name):
+        if gate_name is None:
+            raise Exception("Cannot look for None-type gate.")
+        for i in range(len(self.gates)):
+            if self.gates[i].name == gate_name:
+                return i
+
+        raise Exception("Gate not in genepool.")
+
     def choice(self, size=1, replace=True, n_qubits=None, n_params=None):
         gates_copy = [gate for gate in self.gates]
         probs_copy = [prob for prob in self.probs]
         
         if n_qubits is not None:
             for i in range(len(gates_copy)):
                 if gates_copy[i].n_qubits != n_qubits:
```

### Comparing `ga_vqc-0.0.53/ga_vqc/simple_Individual.py` & `ga_vqc-0.0.54/ga_vqc/simple_Individual.py`

 * *Files identical despite different names*

### Comparing `ga_vqc-0.0.53/ga_vqc/simple_Model.py` & `ga_vqc-0.0.54/ga_vqc/simple_Model.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,16 +278,16 @@
             "fitness_stats": f"Avg fitness: {np.mean(self.fitness_arr)}, Std. Dev: {np.std(self.fitness_arr)}",
             "full_eval_metrics": self.metrics_arr,
             "eval_metrics_stats": [
                 f"Avg {k}: {np.mean([i[k] for i in self.metrics_arr])}, "
                 + f"Std. Dev: {np.std([i[k] for i in self.metrics_arr])}"
                 for k in self.metrics_arr[0].keys()
             ],
-            "full_distances": distances_from_best,
-            "distances_stats": f"Avg distance: {np.mean(distances_from_best)}, Std. Dev: {np.std(distances_from_best)}",
+            # "full_distances": distances_from_best,
+            # "distances_stats": f"Avg distance: {np.mean(distances_from_best)}, Std. Dev: {np.std(distances_from_best)}",
             "best_ansatz": self.best_perf["ansatz_dicts"],
             "best_drawn_ansatz": self.best_perf["ansatz_draw"],
             "best_fitness": self.best_perf["fitness"],
             "best_eval_metrics": self.best_perf["eval_metrics"],
             "best_fitness_gen": self.best_perf["generation"],
             "best_fitness_ix": self.best_perf["index"],
         }
```

### Comparing `ga_vqc-0.0.53/ga_vqc.egg-info/PKG-INFO` & `ga_vqc-0.0.54/ga_vqc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ga-vqc
-Version: 0.0.53
+Version: 0.0.54
 Summary: Genetic Algorithm for VQC ansatz search.
 Home-page: https://github.com/tcoulvert/GA_Ansatz_Search
 Author: Thomas Sievert
 Author-email: 63161166+tcoulvert@users.noreply.github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ga_vqc-0.0.53/setup.py` & `ga_vqc-0.0.54/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="ga_vqc",
-    version="0.0.53",
+    version="0.0.54",
     description="Genetic Algorithm for VQC ansatz search.",
     packages=find_packages(include=["ga_vqc"]),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

