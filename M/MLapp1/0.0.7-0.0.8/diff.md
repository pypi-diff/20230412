# Comparing `tmp/MLapp1-0.0.7.tar.gz` & `tmp/MLapp1-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MLapp1-0.0.7.tar", last modified: Wed Apr 12 16:13:18 2023, max compression
+gzip compressed data, was "MLapp1-0.0.8.tar", last modified: Wed Apr 12 16:26:56 2023, max compression
```

## Comparing `MLapp1-0.0.7.tar` & `MLapp1-0.0.8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 16:13:18.253991 MLapp1-0.0.7/
--rw-------   0 akshay     (503) staff       (20)    35823 2022-06-02 07:43:07.000000 MLapp1-0.0.7/LICENSE.toml
--rw-r--r--   0 akshay     (503) staff       (20)      480 2023-04-12 16:13:18.254119 MLapp1-0.0.7/PKG-INFO
--rw-------   0 akshay     (503) staff       (20)        8 2023-04-12 10:13:27.000000 MLapp1-0.0.7/README.md
--rw-------   0 akshay     (503) staff       (20)       88 2022-06-02 07:45:52.000000 MLapp1-0.0.7/pyproject.toml
--rw-------   0 akshay     (503) staff       (20)      857 2023-04-12 16:13:18.254641 MLapp1-0.0.7/setup.cfg
-drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 16:13:18.243433 MLapp1-0.0.7/src/
-drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 16:13:18.248601 MLapp1-0.0.7/src/MLapp/
--rw-------   0 akshay     (503) staff       (20)     1035 2022-09-12 15:07:15.000000 MLapp1-0.0.7/src/MLapp/README.txt
-drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 16:13:18.252404 MLapp1-0.0.7/src/MLapp/UI/
--rw-------   0 akshay     (503) staff       (20)      109 2022-05-23 13:37:19.000000 MLapp1-0.0.7/src/MLapp/UI/__init__.py
--rw-------   0 akshay     (503) staff       (20)    26860 2022-09-22 15:11:18.000000 MLapp1-0.0.7/src/MLapp/UI/autoML.py
--rw-------   0 akshay     (503) staff       (20)    61898 2022-08-29 10:14:56.000000 MLapp1-0.0.7/src/MLapp/UI/classifcationAlgo.py
--rw-------   0 akshay     (503) staff       (20)    34120 2022-07-29 11:43:58.000000 MLapp1-0.0.7/src/MLapp/UI/componentIDs.py
--rw-------   0 akshay     (503) staff       (20)    28664 2022-08-29 10:15:24.000000 MLapp1-0.0.7/src/MLapp/UI/dataSampling.py
--rw-------   0 akshay     (503) staff       (20)    21241 2022-08-29 10:16:09.000000 MLapp1-0.0.7/src/MLapp/UI/featureSelection.py
--rwxr-xr-x   0 akshay     (503) staff       (20)     4731 2022-07-19 11:00:49.000000 MLapp1-0.0.7/src/MLapp/UI/layouts.py
--rw-------   0 akshay     (503) staff       (20)    23237 2022-09-12 14:20:10.000000 MLapp1-0.0.7/src/MLapp/UI/modelEvaluation.py
--rw-------   0 akshay     (503) staff       (20)    25582 2023-04-12 08:17:24.000000 MLapp1-0.0.7/src/MLapp/UI/result.py
--rw-------   0 akshay     (503) staff       (20)    19093 2022-08-29 10:16:51.000000 MLapp1-0.0.7/src/MLapp/UI/scaling.py
--rw-------   0 akshay     (503) staff       (20)     5562 2022-08-30 12:21:10.000000 MLapp1-0.0.7/src/MLapp/UI/submit.py
--rwxr-xr-x   0 akshay     (503) staff       (20)    13625 2022-09-22 15:55:06.000000 MLapp1-0.0.7/src/MLapp/UI/uploadInput.py
--rw-r--r--   0 akshay     (503) staff       (20)      109 2022-05-23 13:37:19.000000 MLapp1-0.0.7/src/MLapp/__init__.py
--rwxr-xr-x   0 akshay     (503) staff       (20)      485 2023-04-12 08:49:57.000000 MLapp1-0.0.7/src/MLapp/app.py
--rw-------   0 akshay     (503) staff       (20)     2556 2022-07-11 09:48:49.000000 MLapp1-0.0.7/src/MLapp/generateScript.py
--rw-------   0 akshay     (503) staff       (20)    45926 2023-04-12 07:46:30.000000 MLapp1-0.0.7/src/MLapp/helperFunctions.py
--rw-------   0 akshay     (503) staff       (20)      319 2023-04-12 16:12:15.000000 MLapp1-0.0.7/src/MLapp/launcher.py
--rwxr-xr-x   0 akshay     (503) staff       (20)     3853 2023-04-12 08:51:43.000000 MLapp1-0.0.7/src/MLapp/main.py
--rw-------   0 akshay     (503) staff       (20)    13361 2022-09-13 11:45:53.000000 MLapp1-0.0.7/src/MLapp/scriptTemplate.py
--rw-------   0 akshay     (503) staff       (20)    12723 2022-09-22 10:44:47.000000 MLapp1-0.0.7/src/MLapp/subScript.py
-drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 16:13:18.253765 MLapp1-0.0.7/src/MLapp1.egg-info/
--rw-r--r--   0 akshay     (503) staff       (20)      480 2023-04-12 16:13:18.000000 MLapp1-0.0.7/src/MLapp1.egg-info/PKG-INFO
--rw-r--r--   0 akshay     (503) staff       (20)      751 2023-04-12 16:13:18.000000 MLapp1-0.0.7/src/MLapp1.egg-info/SOURCES.txt
--rw-r--r--   0 akshay     (503) staff       (20)        1 2023-04-12 16:13:18.000000 MLapp1-0.0.7/src/MLapp1.egg-info/dependency_links.txt
--rw-r--r--   0 akshay     (503) staff       (20)      188 2023-04-12 16:13:18.000000 MLapp1-0.0.7/src/MLapp1.egg-info/requires.txt
--rw-r--r--   0 akshay     (503) staff       (20)        6 2023-04-12 16:13:18.000000 MLapp1-0.0.7/src/MLapp1.egg-info/top_level.txt
+drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 16:26:56.168928 MLapp1-0.0.8/
+-rw-------   0 akshay     (503) staff       (20)    35823 2022-06-02 07:43:07.000000 MLapp1-0.0.8/LICENSE.toml
+-rw-r--r--   0 akshay     (503) staff       (20)      480 2023-04-12 16:26:56.169009 MLapp1-0.0.8/PKG-INFO
+-rw-------   0 akshay     (503) staff       (20)        8 2023-04-12 10:13:27.000000 MLapp1-0.0.8/README.md
+-rw-------   0 akshay     (503) staff       (20)       88 2022-06-02 07:45:52.000000 MLapp1-0.0.8/pyproject.toml
+-rw-------   0 akshay     (503) staff       (20)      857 2023-04-12 16:26:56.169455 MLapp1-0.0.8/setup.cfg
+drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 16:26:56.159786 MLapp1-0.0.8/src/
+drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 16:26:56.164239 MLapp1-0.0.8/src/MLapp/
+-rw-------   0 akshay     (503) staff       (20)     1035 2022-09-12 15:07:15.000000 MLapp1-0.0.8/src/MLapp/README.txt
+drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 16:26:56.167605 MLapp1-0.0.8/src/MLapp/UI/
+-rw-------   0 akshay     (503) staff       (20)      109 2022-05-23 13:37:19.000000 MLapp1-0.0.8/src/MLapp/UI/__init__.py
+-rw-------   0 akshay     (503) staff       (20)    26863 2023-04-12 16:23:12.000000 MLapp1-0.0.8/src/MLapp/UI/autoML.py
+-rw-------   0 akshay     (503) staff       (20)    61901 2023-04-12 16:24:56.000000 MLapp1-0.0.8/src/MLapp/UI/classifcationAlgo.py
+-rw-------   0 akshay     (503) staff       (20)    34120 2022-07-29 11:43:58.000000 MLapp1-0.0.8/src/MLapp/UI/componentIDs.py
+-rw-------   0 akshay     (503) staff       (20)    28666 2023-04-12 16:24:48.000000 MLapp1-0.0.8/src/MLapp/UI/dataSampling.py
+-rw-------   0 akshay     (503) staff       (20)    21244 2023-04-12 16:23:57.000000 MLapp1-0.0.8/src/MLapp/UI/featureSelection.py
+-rwxr-xr-x   0 akshay     (503) staff       (20)     4731 2022-07-19 11:00:49.000000 MLapp1-0.0.8/src/MLapp/UI/layouts.py
+-rw-------   0 akshay     (503) staff       (20)    23240 2023-04-12 16:23:20.000000 MLapp1-0.0.8/src/MLapp/UI/modelEvaluation.py
+-rw-------   0 akshay     (503) staff       (20)    25583 2023-04-12 16:22:45.000000 MLapp1-0.0.8/src/MLapp/UI/result.py
+-rw-------   0 akshay     (503) staff       (20)    19094 2023-04-12 16:23:48.000000 MLapp1-0.0.8/src/MLapp/UI/scaling.py
+-rw-------   0 akshay     (503) staff       (20)     5565 2023-04-12 16:23:39.000000 MLapp1-0.0.8/src/MLapp/UI/submit.py
+-rwxr-xr-x   0 akshay     (503) staff       (20)    13628 2023-04-12 16:23:03.000000 MLapp1-0.0.8/src/MLapp/UI/uploadInput.py
+-rw-r--r--   0 akshay     (503) staff       (20)      109 2022-05-23 13:37:19.000000 MLapp1-0.0.8/src/MLapp/__init__.py
+-rwxr-xr-x   0 akshay     (503) staff       (20)      485 2023-04-12 08:49:57.000000 MLapp1-0.0.8/src/MLapp/app.py
+-rw-------   0 akshay     (503) staff       (20)     2558 2023-04-12 16:16:15.000000 MLapp1-0.0.8/src/MLapp/generateScript.py
+-rw-------   0 akshay     (503) staff       (20)    45927 2023-04-12 16:25:43.000000 MLapp1-0.0.8/src/MLapp/helperFunctions.py
+-rw-------   0 akshay     (503) staff       (20)      319 2023-04-12 16:12:15.000000 MLapp1-0.0.8/src/MLapp/launcher.py
+-rwxr-xr-x   0 akshay     (503) staff       (20)     3861 2023-04-12 16:15:34.000000 MLapp1-0.0.8/src/MLapp/main.py
+-rw-------   0 akshay     (503) staff       (20)    13361 2022-09-13 11:45:53.000000 MLapp1-0.0.8/src/MLapp/scriptTemplate.py
+-rw-------   0 akshay     (503) staff       (20)    12723 2022-09-22 10:44:47.000000 MLapp1-0.0.8/src/MLapp/subScript.py
+drwxr-xr-x   0 akshay     (503) staff       (20)        0 2023-04-12 16:26:56.168766 MLapp1-0.0.8/src/MLapp1.egg-info/
+-rw-r--r--   0 akshay     (503) staff       (20)      480 2023-04-12 16:26:56.000000 MLapp1-0.0.8/src/MLapp1.egg-info/PKG-INFO
+-rw-r--r--   0 akshay     (503) staff       (20)      751 2023-04-12 16:26:56.000000 MLapp1-0.0.8/src/MLapp1.egg-info/SOURCES.txt
+-rw-r--r--   0 akshay     (503) staff       (20)        1 2023-04-12 16:26:56.000000 MLapp1-0.0.8/src/MLapp1.egg-info/dependency_links.txt
+-rw-r--r--   0 akshay     (503) staff       (20)      188 2023-04-12 16:26:56.000000 MLapp1-0.0.8/src/MLapp1.egg-info/requires.txt
+-rw-r--r--   0 akshay     (503) staff       (20)        6 2023-04-12 16:26:56.000000 MLapp1-0.0.8/src/MLapp1.egg-info/top_level.txt
```

### Comparing `MLapp1-0.0.7/LICENSE.toml` & `MLapp1-0.0.8/LICENSE.toml`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.7/setup.cfg` & `MLapp1-0.0.8/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = MLapp1
-version = 0.0.7
+version = 0.0.8
 author = Akshay
 author_email = akshaysuhag1996@gmail.com
 description = "MLapp"
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/FunctionalUrology/
 project_urls =
```

### Comparing `MLapp1-0.0.7/src/MLapp/README.txt` & `MLapp1-0.0.8/src/MLapp/README.txt`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.7/src/MLapp/UI/autoML.py` & `MLapp1-0.0.8/src/MLapp/UI/autoML.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 import datetime
 import io
 import pandas as pd
 import dash_bootstrap_components as dbc
 import dash_uploader as du
 from dash import dash_table,html,dcc
 import UI.result
-from helperFunctions import *
-from UI.scaling import genrateInfoCallback, genrateCollapseCallback
+from .helperFunctions import *
+from .UI.scaling import genrateInfoCallback, genrateCollapseCallback
 from subScript import runSubscript
 
 
 #!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!! 
 # =============================================================================
 # Upload data tab
 # 
@@ -436,15 +436,15 @@
         metrics=[{'label': i, 'value': i} for i in cols]
         return False,metrics
 
 
 #!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!  
 #update plots/tables as per user input
 from matplotlib.colors import is_color_like
-from helperFunctions import *
+from .helperFunctions import *
 
 @app.callback(Output("uploadResult_plots_autoML", "children"),
               [Input("plotOptions_autoML", "value"),
               #Input(component_id='hidden2', component_property='children'),
               Input({"type": "barPlotColor_autoML", "index": ALL}, "value"),
               Input( {"type": "barPlotText_autoML", "index": ALL} , "value"),
               Input({"type": "linePlotColor_autoML", "index": ALL} , "value"),
```

### Comparing `MLapp1-0.0.7/src/MLapp/UI/classifcationAlgo.py` & `MLapp1-0.0.8/src/MLapp/UI/classifcationAlgo.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 @author: akshay
 """
 
 
 import dash_bootstrap_components as dbc
 from dash import dcc,html
-from UI.scaling import genrateInfoCallback, genrateCollapseCallback,genrateAlertCallback,infoText
-from UI.dataSampling import get_neighbors_Para
+from .UI.scaling import genrateInfoCallback, genrateCollapseCallback,genrateAlertCallback,infoText
+from .UI.dataSampling import get_neighbors_Para
 from app import app
 from dash.dependencies import Input, Output,State
 
     #get the header of each card of sampling tab
 def getAlgoHeader(algo):
     return dbc.Row([
      dbc.Col(dbc.Checklist(options=[{"label": algo,"value": True}],
@@ -1012,15 +1012,15 @@
                 ],className="mt-3",color="dark", outline=True)
 
 
 
 #!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 
 #list of all parameters of classssification algo
-from UI.componentIDs import classification_Com_IDS
+from .UI.componentIDs import classification_Com_IDS
 classification_Com_IDS=classification_Com_IDS.split(",")
 classification_Com_IDS = [sub[1 : ] for sub in classification_Com_IDS]
 
 #get all the algo names
 global algoName
 algoName=[]
 for item in classification_Com_IDS:
```

### Comparing `MLapp1-0.0.7/src/MLapp/UI/componentIDs.py` & `MLapp1-0.0.8/src/MLapp/UI/componentIDs.py`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.7/src/MLapp/UI/dataSampling.py` & `MLapp1-0.0.8/src/MLapp/UI/dataSampling.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Created on Wed Oct  6 12:38:23 2021
 
 @author: akshay
 """
 
 import dash_bootstrap_components as dbc
 from dash import dcc,html
-from UI.scaling import genrateInfoCallback, genrateCollapseCallback,infoText
+from .UI.scaling import genrateInfoCallback, genrateCollapseCallback,infoText
 from app import app
 from dash.dependencies import Input, Output,State
 
 #define card for Oversampling tab
 #!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 
     #get the header of each card of sampling tab
@@ -502,15 +502,15 @@
 
 
 
 
 #!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 
 #list of all parameters of undersampling algo
-from UI.componentIDs import undersampling_Com_IDS
+from .UI.componentIDs import undersampling_Com_IDS
 undersampling_Com_IDS=undersampling_Com_IDS.split(",")
 undersampling_Com_IDS = [sub[1 : ] for sub in undersampling_Com_IDS]
 
 #get all the algo names
 global algoName
 algoName=[]
 for item in undersampling_Com_IDS:
```

### Comparing `MLapp1-0.0.7/src/MLapp/UI/featureSelection.py` & `MLapp1-0.0.8/src/MLapp/UI/featureSelection.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 @author: akshay
 """
 
 
 import dash_bootstrap_components as dbc
 from dash import dcc,html
-from UI.scaling import genrateInfoCallback, genrateCollapseCallback,genrateAlertCallback,infoText
-from UI.dataSampling import get_neighbors_Para
+from .UI.scaling import genrateInfoCallback, genrateCollapseCallback,genrateAlertCallback,infoText
+from .UI.dataSampling import get_neighbors_Para
 from app import app
 from dash.dependencies import Input, Output,State
 
 
 #get the header of each card of sampling tab
 def getAlgoHeader(algo):
     return dbc.Row([
@@ -346,15 +346,15 @@
 #                 ],className="mt-3",color="dark", outline=True)
 # =============================================================================
 
 
 #!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 
 #list of all parameters of feature sel algo
-from UI.componentIDs import featSel_Com_IDS
+from .UI.componentIDs import featSel_Com_IDS
 featSel_Com_IDS=featSel_Com_IDS.split(",")
 featSel_Com_IDS = [sub[1 : ] for sub in featSel_Com_IDS]
 
 #get all the algo names
 global algoName
 algoName=[]
 for item in featSel_Com_IDS:
```

### Comparing `MLapp1-0.0.7/src/MLapp/UI/layouts.py` & `MLapp1-0.0.8/src/MLapp/UI/layouts.py`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.7/src/MLapp/UI/modelEvaluation.py` & `MLapp1-0.0.8/src/MLapp/UI/modelEvaluation.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 from dash import dcc,html
 import dash_bootstrap_components as dbc
 from app import app
 from dash.dependencies import Input, Output,State
 import dash_bootstrap_components as dbc
 from dash import dcc,html
-from UI.scaling import genrateInfoCallback, genrateCollapseCallback,genrateAlertCallback,infoText
-from UI.dataSampling import get_neighbors_Para
+from .UI.scaling import genrateInfoCallback, genrateCollapseCallback,genrateAlertCallback,infoText
+from .UI.dataSampling import get_neighbors_Para
 from app import app
 from dash.dependencies import Input, Output,State
 
 #!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 #Metrices
 
 modelEval_metrics=dbc.FormGroup([
@@ -361,15 +361,15 @@
                  
 
                 ],className="mt-3",color="dark", outline=True)
 
 
 #!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 #list of all parameters of model eval method tabs
-from UI.componentIDs import modelEval_Com_IDS
+from .UI.componentIDs import modelEval_Com_IDS
 modelEval_Com_IDS=modelEval_Com_IDS.split(",")
 modelEval_Com_IDS = [sub[1 : ] for sub in modelEval_Com_IDS]
 
 #get all the algo names
 global algoName
 algoName=[]
 for item in modelEval_Com_IDS:
```

### Comparing `MLapp1-0.0.7/src/MLapp/UI/result.py` & `MLapp1-0.0.8/src/MLapp/UI/result.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 from dash import dcc,html,dash_table
 import dash_bootstrap_components as dbc
 from app import app
 from dash.dependencies import Input, Output,State
 import dash_uploader as du
 import pickle,dash
-from helperFunctions import *
+from .helperFunctions import *
 du.configure_upload(app, 'uploads')
 
 
 #!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!! 
 uploadResult=dbc.Card([dbc.CardBody([
                     html.Div(dbc.Label("Upload Results",style={"font-weight": "bold","font-size": "16px"})),
                     du.Upload(
```

### Comparing `MLapp1-0.0.7/src/MLapp/UI/scaling.py` & `MLapp1-0.0.8/src/MLapp/UI/scaling.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #global scalingAlgo
 scalingAlgo={k:[] for k in ["MaxAbs Scaler","MinMax Scaler","Normalizer","PowerTransformer",
              "QuantileTransformer","Robust Scaler","Standard Scaler"]}
 
 
 #get info text
 #!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
-from UI.componentIDs import allIds
+from .UI.componentIDs import allIds
 
 def infoText(id_):
     text=allIds[id_][0]
     link=allIds[id_][1]
     return html.Label([text,html.Br() ,html.Br() ," Please refer to the ",
                                html.A('scikit-learn user guide', href=link,target="_blank",style={"color": "black"}),
                                " for further details."],
```

### Comparing `MLapp1-0.0.7/src/MLapp/UI/submit.py` & `MLapp1-0.0.8/src/MLapp/UI/submit.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 import dash
 from dash import dcc
 from app import app
 import dash_bootstrap_components as dbc
 import dash_html_components as html
 from dash.dependencies import Input, Output,State,ALL
 from dash.exceptions import PreventUpdate
-from UI.layouts import preprocessing_content,modelEval_content
-from helperFunctions import saveUserInputData
-from UI.uploadInput import upload_data_content
+from .UI.layouts import preprocessing_content,modelEval_content
+from .helperFunctions import saveUserInputData
+from .UI.uploadInput import upload_data_content
 
 
 
 seed_core=[
     
     dbc.CardBody(
         [
```

### Comparing `MLapp1-0.0.7/src/MLapp/UI/uploadInput.py` & `MLapp1-0.0.8/src/MLapp/UI/uploadInput.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 import base64
 import datetime
 import io
 import pandas as pd
 import dash_bootstrap_components as dbc
 import dash_uploader as du
 from dash import dash_table,html,dcc
-import UI.result
-from helperFunctions import *
-from UI.scaling import genrateInfoCallback, genrateCollapseCallback
+import .UI.result
+from .helperFunctions import *
+from .UI.scaling import genrateInfoCallback, genrateCollapseCallback
 
 #!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!! 
 # =============================================================================
 # Upload data tab
 # 
 # =============================================================================
```

### Comparing `MLapp1-0.0.7/src/MLapp/generateScript.py` & `MLapp1-0.0.8/src/MLapp/generateScript.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 """
 Created on Wed Apr 27 11:19:43 2022
 
 @author: akshay
 """
 
 
-from UI.componentIDs import classification_Com_IDS,classification_models,\
+from .UI.componentIDs import classification_Com_IDS,classification_models,\
     undersampling_Com_IDS,underSamp_models,\
        overrsampling_Com_IDS, overSamp_models, \
            modelEval_Com_IDS,\
                scaling_Com_IDS,scaling_models, \
                    featSel_Com_IDS, featSel_models,featSel_est
 
-from helperFunctions import getAlgoNames,removeModelId,getActiveAlgo,getMoedlEvalActive,saveUserInputData,getActiveAlgoFeatSel
+from .helperFunctions import getAlgoNames,removeModelId,getActiveAlgo,getMoedlEvalActive,saveUserInputData,getActiveAlgoFeatSel
 import pickle
 
 #!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 
 # importing the module
 import ast
 with open('myfile.txt') as f:
```

### Comparing `MLapp1-0.0.7/src/MLapp/helperFunctions.py` & `MLapp1-0.0.8/src/MLapp/helperFunctions.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,15 +283,15 @@
 
                     
                 models_active[model_id]=model
             i+=1
     return models_active
 
 #!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
-from UI.componentIDs import classification_Com_IDS,classification_models,\
+from .UI.componentIDs import classification_Com_IDS,classification_models,\
     undersampling_Com_IDS,underSamp_models,\
        overrsampling_Com_IDS, overSamp_models, \
            modelEval_Com_IDS,\
                scaling_Com_IDS,scaling_models, \
                    featSel_Com_IDS, featSel_models,featSel_est
                    
 import pickle
```

### Comparing `MLapp1-0.0.7/src/MLapp/main.py` & `MLapp1-0.0.8/src/MLapp/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 """
 
 from dash import dcc,html
 from dash.dependencies import Input, Output,State
 import dash_bootstrap_components as dbc
 import dash_table
 
-from app import app
-from UI.layouts import preprocessing_content,modelEval_content
-from UI.scaling import scalingAlgo
-from UI.classifcationAlgo import classAlgo_content
-from UI.submit import submit_con
-from UI.result import uploadResult_content
-from UI.uploadInput import upload_data_content
-from UI.autoML import autoML_content
+from .app import app
+from .UI.layouts import preprocessing_content,modelEval_content
+from .UI.scaling import scalingAlgo
+from .UI.classifcationAlgo import classAlgo_content
+from .UI.submit import submit_con
+from .UI.result import uploadResult_content
+from .UI.uploadInput import upload_data_content
+from .UI.autoML import autoML_content
 
 
 
 
 app.css.config.serve_locally = False
```

### Comparing `MLapp1-0.0.7/src/MLapp/scriptTemplate.py` & `MLapp1-0.0.8/src/MLapp/scriptTemplate.py`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.7/src/MLapp/subScript.py` & `MLapp1-0.0.8/src/MLapp/subScript.py`

 * *Files identical despite different names*

### Comparing `MLapp1-0.0.7/src/MLapp1.egg-info/SOURCES.txt` & `MLapp1-0.0.8/src/MLapp1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

