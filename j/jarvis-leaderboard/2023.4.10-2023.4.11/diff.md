# Comparing `tmp/jarvis_leaderboard-2023.4.10.tar.gz` & `tmp/jarvis_leaderboard-2023.4.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jarvis_leaderboard-2023.4.10.tar", last modified: Tue Apr 11 22:07:27 2023, max compression
+gzip compressed data, was "jarvis_leaderboard-2023.4.11.tar", last modified: Wed Apr 12 02:43:49 2023, max compression
```

## Comparing `jarvis_leaderboard-2023.4.10.tar` & `jarvis_leaderboard-2023.4.11.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-11 22:07:27.000000 jarvis_leaderboard-2023.4.10/
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-11 22:07:26.000000 jarvis_leaderboard-2023.4.10/jarvis_leaderboard/
--rw-r--r--   0 knc6     (54782) users      (100)       49 2023-04-11 22:06:36.000000 jarvis_leaderboard-2023.4.10/jarvis_leaderboard/__init__.py
--rw-r--r--   0 knc6     (54782) users      (100)      110 2023-04-11 22:06:36.000000 jarvis_leaderboard-2023.4.10/jarvis_leaderboard/jarvis_serve.py
--rw-r--r--   0 knc6     (54782) users      (100)     2895 2023-04-11 22:06:37.000000 jarvis_leaderboard-2023.4.10/jarvis_leaderboard/jarvis_upload.py
--rw-r--r--   0 knc6     (54782) users      (100)     3297 2023-04-11 22:05:58.000000 jarvis_leaderboard-2023.4.10/jarvis_leaderboard/populate_data.py
--rw-r--r--   0 knc6     (54782) users      (100)    29792 2023-04-11 22:06:37.000000 jarvis_leaderboard-2023.4.10/jarvis_leaderboard/rebuild.py
-drwxr-xr-x   0 knc6     (54782) users      (100)        0 2023-04-11 22:07:27.000000 jarvis_leaderboard-2023.4.10/jarvis_leaderboard.egg-info/
--rw-r--r--   0 knc6     (54782) users      (100)     7527 2023-04-11 22:07:21.000000 jarvis_leaderboard-2023.4.10/jarvis_leaderboard.egg-info/PKG-INFO
--rw-r--r--   0 knc6     (54782) users      (100)      395 2023-04-11 22:07:22.000000 jarvis_leaderboard-2023.4.10/jarvis_leaderboard.egg-info/SOURCES.txt
--rw-r--r--   0 knc6     (54782) users      (100)        1 2023-04-11 22:07:21.000000 jarvis_leaderboard-2023.4.10/jarvis_leaderboard.egg-info/dependency_links.txt
--rw-r--r--   0 knc6     (54782) users      (100)      142 2023-04-11 22:07:21.000000 jarvis_leaderboard-2023.4.10/jarvis_leaderboard.egg-info/requires.txt
--rw-r--r--   0 knc6     (54782) users      (100)       19 2023-04-11 22:07:21.000000 jarvis_leaderboard-2023.4.10/jarvis_leaderboard.egg-info/top_level.txt
--rw-r--r--   0 knc6     (54782) users      (100)     5978 2023-04-11 22:04:59.000000 jarvis_leaderboard-2023.4.10/README.md
--rw-r--r--   0 knc6     (54782) users      (100)     1249 2023-04-11 22:06:37.000000 jarvis_leaderboard-2023.4.10/setup.py
--rw-r--r--   0 knc6     (54782) users      (100)     7527 2023-04-11 22:07:27.000000 jarvis_leaderboard-2023.4.10/PKG-INFO
--rw-r--r--   0 knc6     (54782) users      (100)       38 2023-04-11 22:07:27.000000 jarvis_leaderboard-2023.4.10/setup.cfg
+drwxrwxrwx   0 kamalch   (1000) kamalch   (1000)        0 2023-04-12 02:43:51.033417 jarvis_leaderboard-2023.4.11/
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     1064 2023-02-25 21:44:25.000000 jarvis_leaderboard-2023.4.11/LICENSE
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     6421 2023-04-12 02:43:51.031426 jarvis_leaderboard-2023.4.11/PKG-INFO
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     5978 2023-04-11 22:13:11.000000 jarvis_leaderboard-2023.4.11/README.md
+drwxrwxrwx   0 kamalch   (1000) kamalch   (1000)        0 2023-04-12 02:43:50.972418 jarvis_leaderboard-2023.4.11/jarvis_leaderboard/
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)       49 2023-04-12 02:21:11.000000 jarvis_leaderboard-2023.4.11/jarvis_leaderboard/__init__.py
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     3297 2023-04-07 21:22:48.000000 jarvis_leaderboard-2023.4.11/jarvis_leaderboard/jarvis_populate_data.py
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)      112 2023-04-12 00:54:55.000000 jarvis_leaderboard-2023.4.11/jarvis_leaderboard/jarvis_serve.py
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     2918 2023-04-12 02:08:02.000000 jarvis_leaderboard-2023.4.11/jarvis_leaderboard/jarvis_upload.py
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)    29738 2023-04-12 02:35:25.000000 jarvis_leaderboard-2023.4.11/jarvis_leaderboard/rebuild.py
+drwxrwxrwx   0 kamalch   (1000) kamalch   (1000)        0 2023-04-12 02:43:51.020424 jarvis_leaderboard-2023.4.11/jarvis_leaderboard.egg-info/
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     6421 2023-04-12 02:43:50.000000 jarvis_leaderboard-2023.4.11/jarvis_leaderboard.egg-info/PKG-INFO
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)      410 2023-04-12 02:43:50.000000 jarvis_leaderboard-2023.4.11/jarvis_leaderboard.egg-info/SOURCES.txt
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)        1 2023-04-12 02:43:50.000000 jarvis_leaderboard-2023.4.11/jarvis_leaderboard.egg-info/dependency_links.txt
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)      142 2023-04-12 02:43:50.000000 jarvis_leaderboard-2023.4.11/jarvis_leaderboard.egg-info/requires.txt
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)       19 2023-04-12 02:43:50.000000 jarvis_leaderboard-2023.4.11/jarvis_leaderboard.egg-info/top_level.txt
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)       38 2023-04-12 02:43:51.034428 jarvis_leaderboard-2023.4.11/setup.cfg
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     1303 2023-04-12 02:21:03.000000 jarvis_leaderboard-2023.4.11/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `jarvis_leaderboard-2023.4.10/jarvis_leaderboard/jarvis_upload.py` & `jarvis_leaderboard-2023.4.11/jarvis_leaderboard/jarvis_upload.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     cmd = "ls ./" + add_dir
     print(cmd)
     os.system(cmd)
 
     cmd = "git add ./" + add_dir + "/*"
     print(cmd)
     os.system(cmd)
-    cmd = "git commit"
+    cmd = "git commit -m 'Adding benchmark.'"
     print(cmd)
     os.system(cmd)
     cmd = "git push"
     print(cmd)
     os.system(cmd)
 
     cmd = "python jarvis_leaderboard/rebuild.py"
```

### Comparing `jarvis_leaderboard-2023.4.10/jarvis_leaderboard/populate_data.py` & `jarvis_leaderboard-2023.4.11/jarvis_leaderboard/jarvis_populate_data.py`

 * *Files identical despite different names*

### Comparing `jarvis_leaderboard-2023.4.10/jarvis_leaderboard/rebuild.py` & `jarvis_leaderboard-2023.4.11/jarvis_leaderboard/rebuild.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from jarvis.db.jsonutils import loadjson
 from sklearn.metrics import mean_absolute_error, accuracy_score
 import pandas as pd
 import glob
 import zipfile
 import json
 from collections import defaultdict
-import collections
 import numpy as np
 
 # from mkdocs import utils
 
 # base_url = utils.get_relative_url('.','.')
 # print ('base_url',base_url)
 root_dir = os.path.dirname(os.path.abspath(__file__))
@@ -65,15 +64,14 @@
                 if "Number of benchmarks:" in i:
                     num = int(i.split("Number of benchmarks:")[1])
         return str(num)
 
     for i in methods:
         line += "<tr>" + "<td>" + i + "</td>"
         for j in tasks:
-            # <td><a href="./AI/SinglePropertyPrediction" target="_blank"><!-AI_SinglePropertyPrediction->120</a></td>
             num = get_num_benches(method=i, task=j)
             if num == "0":
                 line += "<td>" + "-" + "</td>"
             else:
                 line += (
                     '<td><a href="./'
                     + i
@@ -204,15 +202,14 @@
         if "qm9_std_jctc" in csv_path:
             # print('scaling[dataset][prop],',scaling[dataset][prop])
             res = round(
                 scaling[dataset][prop]
                 * mean_absolute_error(df["actual"], df["prediction"]),
                 3,
             )
-            # res = round(mean_absolute_error(df["actual"]*scaling[dataset][prop], df["prediction"]*scaling[dataset]), 3)
             results["res"] = res
             # print(csv_path)
             # print('mae1',mean_absolute_error(csv_data['target'],csv_data['prediction']))
             # print('res',res)
             # print(csv_data)
             # print(actual_df)
             # print()
@@ -255,15 +252,14 @@
         prop = temp[2]
         dataset = temp[3]
         method = temp[0]
         metric = temp[-1]
         # print ('metric',metric)
         # print ('dataset',dataset)
         team = i.split("/")[-2]
-        # md_filename = os.path.join("../docs",method,submod,prop) #"../docs/" + method + "/" +submod+"/"+ prop + ".md"
         md_filename = "../docs/" + method + "/" + submod + "/" + prop + ".md"
         # print ('md_filename',md_filename)
         md_path = os.path.join(root_dir, md_filename)
         # print(
         #    fname,
         #    data_split,
         #    prop,
@@ -475,14 +471,27 @@
                     + "-"
                     + i["result"]["dataset"]
                     + "-"
                     + i["result"]["method"]
                     + "-"
                     + i["result"]["metric"]
                 )
+                name2 = (
+                    i["result"]["method"]
+                    + "-"
+                    + i["result"]["submod"]
+                    + "-"
+                    + i["result"]["prop"]
+                    + "-"
+                    + i["result"]["dataset"]
+                    + "-"
+                    + i["result"]["data_split"]
+                    + "-"
+                    + i["result"]["metric"]
+                )
                 if name == name2:
                     temp = float(i["result"]["res"])
                     # if md_path!='docs/index.md':
                     # selected[name] = i["result"]
                     i["result"]["team"] = i["team"]
                     if name not in selected:
                         selected[name] = i["result"]
@@ -513,15 +522,16 @@
             + "<th>Score</th>"
             + "<th>Team</th>"
             + "<th>Dataset</th>"
             + "<th>Size</th>"
             + "</tr></thead>"
         )
         for i, j in selected.items():
-            if md_path == "docs/index.md":
+            if len(md_path.split("/")) == 2:
+                # if md_path == "docs/index.md":
                 temp = (
                     temp
                     + "<tr>"
                     + "<td>"
                     + '<a href="./'
                     + j["method"]
                     + '" target="_blank">'
@@ -754,15 +764,14 @@
                 temp2 = (
                     # "<!--number_of_methods--> - Number of methods: "
                     "<!--number_of_methods--> - Number of methods: "
                     + "["
                     + str(n_methods)
                     + "]"
                     + "(https://github.com/usnistgov/jarvis_leaderboard/tree/main/jarvis_leaderboard/benchmarks)"
-                    # "<!--number_of_methods--> - Number of methods: "+'<a href = "https://github.com/usnistgov/jarvis_leaderboard/tree/main/jarvis_leaderboard/benchmarks" target="_blank"> '+str(n_methods)+'</a>'
                     # + str(n_methods)
                     # + str(len(dat))
                     # + "\n"
                 )
                 content.append(temp2)
             elif "<!--number_of_benchmarks-->" in j:
                 temp2 = (
@@ -776,37 +785,37 @@
                 content.append(j)
         # filedata = filedata.replace('<!--table_content-->', temp)
 
         with open(md_path, "w") as file:
             file.write("\n".join(content))
 
     homepage = [
-        "SinglePropertyPrediction-test-formation_energy_peratom-dft_3d-AI-mae",
-        "SinglePropertyPrediction-test-optb88vdw_bandgap-dft_3d-AI-mae",
-        "SinglePropertyPrediction-test-optb88vdw_total_energy-dft_3d-AI-mae",
-        "SinglePropertyPrediction-test-bulk_modulus_kv-dft_3d-AI-mae",
-        "SinglePropertyClass-test-optb88vdw_bandgap-dft_3d-AI-acc",
-        "SinglePropertyPrediction-test-LUMO-qm9_std_jctc-AI-mae",
-        "SinglePropertyPrediction-test-max_co2_adsp-hmof-AI-mae",
-        "MLFF-test-energy-alignn_ff_db-AI-mae",
-        "ImageClass-test-bravais_class-stem_2d_image-AI-acc",
-        "TextClass-test-categories-arXiv-AI-acc",
-        "SinglePropertyPrediction-test-bulk_modulus_JVASP_816_Al-dft_3d-FF-mae",
-        "SinglePropertyPrediction-test-bulk_modulus_JVASP_816_Al-dft_3d-ES-mae",
-        "SinglePropertyPrediction-test-bulk_modulus-dft_3d-ES-mae",
-        "SinglePropertyPrediction-test-bulk_modulus_JVASP_1002_Si-dft_3d-ES-mae",
-        "SinglePropertyPrediction-test-bandgap-dft_3d-ES-mae",
-        "SinglePropertyPrediction-test-bandgap_JVASP_1002_Si-dft_3d-ES-mae",
-        "SinglePropertyPrediction-test-epsx-dft_3d-ES-mae",
-        "SinglePropertyPrediction-test-Tc_supercon_JVASP_1151_MgB2-dft_3d-ES-mae",
-        "SinglePropertyPrediction-test-Tc_supercon-dft_3d-ES-mae",
-        "SinglePropertyPrediction-test-slme-dft_3d-ES-mae",
-        "Spectra-test-dielectric_function-dft_3d-ES-multimae",
-        "EigenSolver-test-electron_bands_JVASP_816_Al_WTBH-dft_3d-QC-multimae",
-        "Spectra-test-XRD_JVASP_19821_MgB2-dft_3d-EXP-multimae",
+        "AI-SinglePropertyPrediction-formation_energy_peratom-dft_3d-test-mae",
+        "AI-SinglePropertyPrediction-optb88vdw_bandgap-dft_3d-test-mae",
+        "AI-SinglePropertyPrediction-optb88vdw_total_energy-dft_3d-test-mae",
+        "AI-SinglePropertyPrediction-bulk_modulus_kv-dft_3d-test-mae",
+        "AI-SinglePropertyClass-optb88vdw_bandgap-dft_3d-test-acc",
+        "AI-SinglePropertyPrediction-LUMO-qm9_std_jctc-test-mae",
+        "AI-SinglePropertyPrediction-max_co2_adsp-hmof-test-mae",
+        "AI-MLFF-energy-alignn_ff_db-test-mae",
+        "AI-ImageClass-bravais_class-stem_2d_image-test-acc",
+        "AI-TextClass-categories-arXiv-test-acc",
+        "FF-SinglePropertyPrediction-bulk_modulus_JVASP_816_Al-dft_3d-test-mae",
+        "ES-SinglePropertyPrediction-bulk_modulus_JVASP_816_Al-dft_3d-test-mae",
+        "ES-SinglePropertyPrediction-bulk_modulus-dft_3d-test-mae",
+        "ES-SinglePropertyPrediction-bulk_modulus_JVASP_1002_Si-dft_3d-test-mae",
+        "ES-SinglePropertyPrediction-bandgap-dft_3d-test-mae",
+        "ES-SinglePropertyPrediction-bandgap_JVASP_1002_Si-dft_3d-test-mae",
+        "ES-SinglePropertyPrediction-epsx-dft_3d-test-mae",
+        "ES-SinglePropertyPrediction-Tc_supercon_JVASP_1151_MgB2-dft_3d-test-mae",
+        "ES-SinglePropertyPrediction-Tc_supercon-dft_3d-test-mae",
+        "ES-SinglePropertyPrediction-slme-dft_3d-test-mae",
+        "ES-Spectra-dielectric_function-dft_3d-test-multimae",
+        "QC-EigenSolver-electron_bands_JVASP_816_Al_WTBH-dft_3d-test-multimae",
+        "EXP-Spectra-XRD_JVASP_19821_MgB2-dft_3d-test-multimae",
     ]
     x = []
     for i in glob.glob("jarvis_leaderboard/benchmarks/*/*.csv.zip"):
         x.append(i.split(".csv.zip")[0])
         # x.append(i.split('/')[-1].split('.csv.zip')[0])
     print(x, len(x))
     update_individual_index_md(md_path="docs/index.md", homepage=homepage)
@@ -860,7 +869,11 @@
         md_path="docs/AI/Spectra/index.md", key="AI", extra_key="Spectra"
     )
     make_summary_table()
     print("errors", errors)
     os.chdir(current_dir)
     return errors
     # print("dat", dat)
+
+
+if __name__ == "__main__":
+    rebuild_pages()
```

### Comparing `jarvis_leaderboard-2023.4.10/README.md` & `jarvis_leaderboard-2023.4.11/README.md`

 * *Files identical despite different names*

### Comparing `jarvis_leaderboard-2023.4.10/setup.py` & `jarvis_leaderboard-2023.4.11/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="jarvis_leaderboard",  # Replace with your own username
-    version="2023.04.10",
+    version="2023.04.11",
     author="Kamal Choudhary",
     author_email="kamal.choudhary@nist.gov",
     description="jarvis_leaderboard",
     install_requires=[
         "numpy>=1.19.5",
         "scipy>=1.6.3",
         "jarvis-tools>=2021.07.19",
@@ -20,17 +20,18 @@
         "pydantic>=1.8.1",
         "markdown==3.2.1",
         # "flake8>=3.9.1",
         # "pycodestyle>=2.7.0",
         # "pydocstyle>=6.0.0",
     ],
     scripts=[
+        "jarvis_leaderboard/jarvis_populate_data.py",
         "jarvis_leaderboard/jarvis_upload.py",
-        "jarvis_leaderboard/rebuild.py",
         "jarvis_leaderboard/jarvis_serve.py",
+        "jarvis_leaderboard/rebuild.py",
     ],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/knc6/jarvis_leaderboard",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

