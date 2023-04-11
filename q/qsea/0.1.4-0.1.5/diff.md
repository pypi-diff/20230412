# Comparing `tmp/qsea-0.1.4.tar.gz` & `tmp/qsea-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\qsea-0.1.4.tar", last modified: Tue Apr 11 21:45:48 2023, max compression
+gzip compressed data, was "dist\qsea-0.1.5.tar", last modified: Tue Apr 11 22:28:14 2023, max compression
```

## Comparing `qsea-0.1.4.tar` & `qsea-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 21:45:48.614323 qsea-0.1.4/
--rw-rw-rw-   0        0        0     1061 2023-01-13 17:31:55.000000 qsea-0.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0      606 2023-04-11 21:45:48.612320 qsea-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-01-13 17:37:30.000000 qsea-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 21:45:48.606325 qsea-0.1.4/qsea/
--rw-rw-rw-   0        0        0    59908 2023-04-11 21:29:44.000000 qsea-0.1.4/qsea/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 21:45:48.611321 qsea-0.1.4/qsea.egg-info/
--rw-rw-rw-   0        0        0      606 2023-04-11 21:45:48.000000 qsea-0.1.4/qsea.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2023-04-11 21:45:48.000000 qsea-0.1.4/qsea.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 21:45:48.000000 qsea-0.1.4/qsea.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-11 21:45:48.000000 qsea-0.1.4/qsea.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-11 21:45:48.000000 qsea-0.1.4/qsea.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 21:45:48.614323 qsea-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      829 2023-04-11 21:45:39.000000 qsea-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 22:28:14.313572 qsea-0.1.5/
+-rw-rw-rw-   0        0        0     1061 2023-01-13 17:31:55.000000 qsea-0.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      606 2023-04-11 22:28:14.311491 qsea-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-01-13 17:37:30.000000 qsea-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 22:28:14.296498 qsea-0.1.5/qsea/
+-rw-rw-rw-   0        0        0    61127 2023-04-11 22:27:08.000000 qsea-0.1.5/qsea/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 22:28:14.310491 qsea-0.1.5/qsea.egg-info/
+-rw-rw-rw-   0        0        0      606 2023-04-11 22:28:13.000000 qsea-0.1.5/qsea.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2023-04-11 22:28:13.000000 qsea-0.1.5/qsea.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 22:28:13.000000 qsea-0.1.5/qsea.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-11 22:28:13.000000 qsea-0.1.5/qsea.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-11 22:28:13.000000 qsea-0.1.5/qsea.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 22:28:14.313572 qsea-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      829 2023-04-11 22:27:32.000000 qsea-0.1.5/setup.py
```

### Comparing `qsea-0.1.4/LICENSE.txt` & `qsea-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qsea-0.1.4/PKG-INFO` & `qsea-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsea
-Version: 0.1.4
+Version: 0.1.5
 Summary: Convenient way to work with Qlik Sense Engine API from Python
 Home-page: https://github.com/ncthuc/qsea
 Download-URL: https://pypi.org/project/qsea/
 Author: Lev Biriukov
 Author-email: lbiryukov@gmail.com
 License: MIT
 Keywords: QlikSense,Qlik
```

### Comparing `qsea-0.1.4/qsea/__init__.py` & `qsea-0.1.5/qsea/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,53 @@
 #!/usr/bin/env python
 # coding: utf-8
 
-# In[2]:
+# In[1]:
 
 
 # beta-версия к публикации
 
 import json
 import pandas as pd
 import datetime as dt
 import logging
 
 
-# In[5]:
+# In[47]:
+
+
+# version 0.1.12-04-23
+
+def OpenConnection(qlik_url, header_user, timeout = 10):
+    #to refine: review the overall config
+    ws = websocket.create_connection(qlik_url, sslopt={"cert_reqs": ssl.CERT_NONE},header=header_user, timeout = timeout)
+    result1 = ws.recv()
+    if 'severity' in json.loads(result1)['params']:
+        if json.loads(result1)['params']['severity'] == 'fatal':
+            print (json.loads(result1)['params']['message'])
+            print(False)
+            return ws
+    else: 
+        result2 = ws.recv()
+        if json.loads(result2)['params']['qSessionState'] in ['SESSION_ATTACHED', 'SESSION_CREATED']:
+            print (json.loads(result2)['params']['qSessionState'])
+            print(True)
+            return ws
+    return ws
+
+
+# In[3]:
 
 
 # version 0.1.22-07-11
 # just a shortcut to query Qlik Sense Engine Api; 
 # json_query - query text; 
 # attempts - maximum number of attempts;
 
-def Query(json_query, attempts = 1):
+def Query(ws, json_query, attempts = 1):
     ws.send(json.dumps(json_query))
     i = 1
     while i <= attempts:
         try: 
             result = ws.recv()
             return json.loads(result)
         except Exception as E:
@@ -38,161 +61,161 @@
 #         "method": "GetActiveDoc",
 #         "params": [],
 #         "outKey": -1,
 #         "id": 1
 #         })
 
 
-# In[6]:
+# In[4]:
 
 
 # version 0.1.22-07-11
 # returns App GUID by its name
 
-def GetAppID(AppName):
-    rawAppList = Query({
+def GetAppID(ws, AppName):
+    rawAppList = Query(ws, {
         "handle": -1,
         "method": "GetDocList",
         "params": [],
         "outKey": -1,
         "id": 1
         })
     
     for app in rawAppList['result']['qDocList']:
         if app['qDocName'] == AppName:
             return app['qDocId']
     
 # GetAppID('MyAppName')
 
 
-# In[7]:
+# In[5]:
 
 
 # version 0.1.22-07-11
 # opens the app (by name or ID) and returns its handle
 
-def OpenDoc(AppName = '', AppID = ''):
+def OpenDoc(ws, AppName = '', AppID = ''):
     if AppName == '' and AppID == '':
         logging.error('AppName or AppID not specified')
         return 0
     
     if AppName != '':
-        AppID = GetAppID(AppName)
+        AppID = GetAppID(ws, AppName)
 
-    zu = Query({
+    zu = Query(ws, {
     "handle": -1,
     "method": "OpenDoc",
     "params": [AppID],
     "outKey": -1,
     "id": 1
     })
 
     return zu['result']['qReturn']['qHandle']
     
 # AppHandle = OpenDoc('MyAppName')
 
 
-# In[8]:
+# In[6]:
 
 
 # version 0.1.22-07-08
 # Returns object properties by its handle; just a shortcut
 
-def GetProperties(handle):
-    return Query({
+def GetProperties(ws, handle):
+    return Query(ws, {
       "jsonrpc": "2.0",
       "id": 4,
       "method": "GetProperties",
       "handle": handle,
       "params": []
     })
 
 
-# In[9]:
+# In[7]:
 
 
 # version 0.1.22-07-08
 # Sets object properties by its handle and set query; just a shortcut
 
-def SetProperties(handle, query):
-    zu = Query({
+def SetProperties(ws, handle, query):
+    zu = Query(ws, {
               "jsonrpc": "2.0",
               "id": 4,
               "method": "SetProperties",
               "handle": handle,
               "params": [
                 query
                 ]
             })
     return zu
 
 
-# In[10]:
+# In[8]:
 
 
 # version 0.1.22-07-08
 # Returns object layout by its handle; just a shortcut
 
-def GetLayout(handle):
-    return Query({
+def GetLayout(ws, handle):
+    return Query(ws, {
       "jsonrpc": "2.0",
       "id": 4,
       "method": "GetLayout",
       "handle": handle,
       "params": []
     })
 
 
-# In[11]:
+# In[9]:
 
 
 # version 0.1.22-07-08
 # returns a handle of any object by its ID
 
-def GetObjectHandle(appHandle, ObjectId):
-    return Query({
+def GetObjectHandle(ws, appHandle, ObjectId):
+    return Query(ws, {
       "jsonrpc": "2.0",
       "id": 4,
       "method": "GetObject",
       "handle": appHandle,
       "params": [
         ObjectId
       ]
     })['result']['qReturn']['qHandle']
 
 
-# In[12]:
+# In[10]:
 
 
 # version 0.1.22-07-08
 # returns dataframe with all apps
 
-def GetAppList():
+def GetAppList(ws):
 
-    zu = Query({
+    zu = Query(ws, {
         "handle": -1,
         "method": "GetDocList",
         "params": [],
         "outKey": -1,
         "id": 1
         })
     
     df = pd.json_normalize(zu['result']['qDocList'])
     return df
 
 
-# In[13]:
+# In[70]:
 
 
 # version 0.1.22-07-08
 # returns dataframe with app variables
 
-def GetVarPandas(appHandle):
+def GetVarPandas(ws, appHandle):
     # get handle of VariableList
-    zu = Query({
+    zu = Query(ws, {
           "jsonrpc": "2.0",
           "id": 2,
           "method": "CreateSessionObject",
           "handle": appHandle,
           "params": [
             {
               "qInfo": {
@@ -203,28 +226,28 @@
                 "qType": "variable"
               }
             }
           ]
         }
     )
     listHandle = zu['result']['qReturn']['qHandle']
-    return pd.json_normalize(GetLayout(listHandle)['result']['qLayout']['qVariableList']['qItems'])
+    return pd.json_normalize(GetLayout(ws, listHandle)['result']['qLayout']['qVariableList']['qItems'])
 
 # zu = GetVarList(1)
 
 
-# In[14]:
+# In[71]:
 
 
 # version 0.1.22-07-08
 # returns dataframe with app master measures
 
-def GetMsPandas(appHandle):
+def GetMsPandas(ws, appHandle):
     # get handle of MeasureList
-    zu = Query({
+    zu = Query(ws, {
           "jsonrpc": "2.0",
           "id": 2,
           "method": "CreateSessionObject",
           "handle": appHandle,
           "params": [
             {
               "qInfo": {
@@ -240,28 +263,28 @@
                     }
               }
             }
           ]
         }
     )
     listHandle = zu['result']['qReturn']['qHandle']
-    return pd.json_normalize(GetLayout(listHandle)['result']['qLayout']['qMeasureList']['qItems'])
+    return pd.json_normalize(GetLayout(ws, listHandle)['result']['qLayout']['qMeasureList']['qItems'])
 
 # zu = GetMsList(1)
 
 
-# In[15]:
+# In[72]:
 
 
 # version 0.1.22-07-08
 # returns dataframe with app sheets
 
-def GetSheetPandas(appHandle):
+def GetSheetPandas(ws, appHandle):
     # get handle of SessionLists
-    zu = Query({
+    zu = Query(ws, {
       "jsonrpc": "2.0",
       "id": 2,
       "method": "CreateSessionObject",
       "handle": appHandle,
       "params": [
         {
           "qInfo": {
@@ -275,28 +298,28 @@
             }
           }
         }
       ]
     })
     
     listHandle = zu['result']['qReturn']['qHandle']
-    return pd.json_normalize(GetLayout(listHandle)['result']['qLayout']['qAppObjectList']['qItems'])
+    return pd.json_normalize(GetLayout(ws, listHandle)['result']['qLayout']['qAppObjectList']['qItems'])
 
 # zu = GetSheetList(1)
 
 
-# In[16]:
+# In[14]:
 
 
 # version 0.1.22-07-08
 # returns dataframe with app fields
 
-def GetFieldPandas(appHandle):
+def GetFieldPandas(ws, appHandle):
     # GetTablesAndKeys
-    zu = Query({
+    zu = Query(ws, {
       "jsonrpc": "2.0",
       "id": 1,
       "method": "GetTablesAndKeys",
       "handle": appHandle,
       "params": [
         {
           "qcx": 1000,
@@ -320,23 +343,23 @@
     pdf = df[cols].join(qFields)
     
     return pdf
 
 # zu = GetFieldList(1)
 
 
-# In[17]:
+# In[73]:
 
 
 # version 0.1.22-09-13
 # returns dataframe with app dimensions
 
-def GetDimPandas(appHandle):
+def GetDimPandas(ws, appHandle):
     # get handle of DimensionList
-    zu = Query({
+    zu = Query(ws, {
           "jsonrpc": "2.0",
           "id": 2,
           "method": "CreateSessionObject",
           "handle": 1,
           "params": [
             {
               "qInfo": {
@@ -353,98 +376,100 @@
               }
             }
           ]
         }
     )
 
     listHandle = zu['result']['qReturn']['qHandle']
-    return pd.json_normalize(GetLayout(listHandle)['result']['qLayout']['qDimensionList']['qItems'])
+    return pd.json_normalize(GetLayout(ws, listHandle)['result']['qLayout']['qDimensionList']['qItems'])
 
 # zu = GetDimPandas(1)
 
 
-# In[18]:
+# In[16]:
 
 
 # version 0.1.22-08-07
 # returns dataframe with objects on the sheet by its handle
 
-def GetSheetObjectsPandas(SheetHandle):
+def GetSheetObjectsPandas(ws, SheetHandle):
     # раскладка листа
-    SheetLayout = GetLayout(SheetHandle)
+    SheetLayout = GetLayout(ws, SheetHandle)
     odf = pd.json_normalize(GetLayout(SheetHandle)['result']['qLayout']['cells'])
     return odf
 
 
-# In[19]:
+# In[17]:
 
 
 # version 0.1.22-08-07
 # returns dataframe with measures used in object by its handle
 
-def GetObjectMeasuresPandas(ObjectHandle):
-    gl = Query({
+def GetObjectMeasuresPandas(ws, ObjectHandle):
+    gl = Query(ws, {
       "jsonrpc": "2.0",
       "id": 4,
       "method": "GetProperties",
       "handle": ObjectHandle,
       "params": []
     })
 
     odf = pd.json_normalize(gl['result']['qProp']['qHyperCubeDef']['qMeasures'])
     return odf
 
 
-# In[20]:
+# In[18]:
 
 
 # version 0.1.22-08-07
 # returns dataframe with dimensions used in object by its handle
 
-def GetObjectDimensionsPandas(ObjectHandle):
-    gl = Query({
+def GetObjectDimensionsPandas(ws, ObjectHandle):
+    gl = Query(ws, {
       "jsonrpc": "2.0",
       "id": 4,
       "method": "GetProperties",
       "handle": ObjectHandle,
       "params": []
     })
 
     odf = pd.json_normalize(gl['result']['qProp']['qHyperCubeDef']['qDimensions'])
     return odf
 
 
-# In[21]:
+# In[44]:
 
 
 # version 0.1.22-11-10
 # the class, representing the application
 
 class App:
     
-    def __init__(self, appName):
-        self.handle = OpenDoc(appName)
+    def __init__(self, ws, appName):
+        
+        self.handle = OpenDoc(ws, appName)
         self.name = appName
         self.variables = AppChildren(self, 'variables')
         self.measures = AppChildren(self, 'measures')
         self.sheets = AppChildren(self, 'sheets')
         self.fields = AppChildren(self, 'fields')
         self.dimensions = AppChildren(self, 'dimensions')
+        self.ws = ws
     
     def save(self):
-        Query({
+        Query(self.ws, {
             "jsonrpc": "2.0",
             "id": 6,
             "method": "DoSave",
             "handle": self.handle,
             "params": []
         })
 
 
-# In[22]:
+# In[64]:
 
 
 # version 0.1.22-11-10
 # the class, representing variables of the application
 # member of App.variables collection
 
 class Variable:
@@ -459,15 +484,15 @@
         self.description = ''
         self.createdDate = dt.datetime(year=1901, month=1, day=1)
         self.modifiedDate = dt.datetime(year=1901, month=1, day=1)
         self.scriptCreated = ''
         
         
     def getHandle(self):
-        self.handle = Query({
+        self.handle = Query(self.parent.ws, {
           "jsonrpc": "2.0",
           "id": 4,
           "method": "GetVariableById",
           "handle": self.appHandle,
           "params": [self.id]
         })['result']['qReturn']['qHandle']
         return self.handle
@@ -481,15 +506,15 @@
             else: definition = '"' + str(self.definition) + '"'
         else: definition = '"' + definition + '"'
         if description == '':
             if str(self.description) == 'nan': description = '""'
             else: description = '"' + str(self.description) + '"'
         else: description = '"' + description + '"'
         
-        zu = Query({
+        zu = Query(self.parent.ws, {
           "jsonrpc": "2.0",
           "id": 2,
           "method": "ApplyPatches",
           "handle": self.handle,
           "params": [
             [
               {
@@ -512,15 +537,15 @@
                 self.definition = definition
                 self.description = description
         except: 1
 
         return zu
     
     def delete(self):
-        zu = Query({
+        zu = Query(self.parent.ws, {
               "jsonrpc": "2.0",
               "id": 10,
               "method": "DestroyVariableById",
               "handle": self.appHandle,
               "params": [
                 self.id
               ]
@@ -542,15 +567,15 @@
         tdef = self.definition
         tdesc = self.description
         if str(tdesc) == 'nan': tdesc = ''
         parent.add(newName, tdef, tdesc)
         self.delete()
 
 
-# In[23]:
+# In[21]:
 
 
 # version 0.1.22-11-10
 # the class, representing fields of the application
 # member of App.fields collection
 
 class Field:
@@ -561,15 +586,15 @@
         
         self.tableName = ''
         self.informationDensity, self.nNonNulls, self.nRows, self.subsetRatio = 0, 0, 0, 0
         self.nTotalDistinctValues, self.nPresentDistinctValues = 0, 0
         self.keyType, self.tags = '', ''
 
 
-# In[24]:
+# In[22]:
 
 
 # version 0.1.22-11-10
 # the class, representing master measures of the application
 # member of App.measures collection
 
 class Measure:
@@ -581,15 +606,15 @@
         
         self.id, self.definition, self.description, self.label, self.labelExpression = '', '', '', '', ''
         self.formatType, self.formatNDec, self.formatUseThou, self.formatDec, self.formatThou = '', -1, -1, '', ''
         self.createdDate, self.modifiedDate = dt.datetime(year=1901, month=1, day=1), dt.datetime(year=1901, month=1, day=1)
         
         
     def getHandle(self):
-        self.handle = Query({
+        self.handle = Query(self.parent.ws, {
           "jsonrpc": "2.0",
           "id": 4,
           "method": "GetMeasure",
           "handle": self.appHandle,
           "params": [self.id]
         })['result']['qReturn']['qHandle']
         return self.handle
@@ -638,15 +663,15 @@
                     "qThou": formatThou
                   }
                 },
                 "qMetaDef": {'title': self.name}
             }
           ]
         }
-        zu = Query(t)
+        zu = Query(self.parent.ws, t)
         
         # прописать, что заменяем только в случае успеха
         try:
             if len(zu['change']) > 0:
                 self.definition = definition
                 self.label = label
                 self.labelExpression = labelExpression
@@ -656,15 +681,15 @@
                 self.formatDec = formatDec
                 self.formatThou = formatThou
         except: 1
         
         return zu
     
     def delete(self):
-        zu = Query({
+        zu = Query(self.parent.ws, {
               "jsonrpc": "2.0",
               "id": 10,
               "method": "DestroyMeasure",
               "handle": self.appHandle,
               "params": [
                 self.id
               ]
@@ -693,23 +718,23 @@
                 "qId": self.id,
                 "qType": "measure"
               },
                 "qMetaDef": {'title': name}
             }
           ]
         }
-        zu = Query(t)
+        zu = Query(self.parent.ws, t)
         
         # прописать, что заменяем только в случае успеха
         self.name = name
         
         return zu
 
 
-# In[25]:
+# In[23]:
 
 
 # version 0.1.22-11-10
 # the class, representing master dimensions of the application
 # member of App.dimensions collection
 
 class Dimension:
@@ -720,15 +745,15 @@
         self.parent = parent
         
         self.id, self.definition = '', ''
         self.createdDate, self.modifiedDate = dt.datetime(year=1901, month=1, day=1), dt.datetime(year=1901, month=1, day=1)
         
         
     def getHandle(self):
-        self.handle = Query({
+        self.handle = Query(self.parent.ws, {
           "jsonrpc": "2.0",
           "id": 4,
           "method": "GetDimension",
           "handle": self.appHandle,
           "params": [self.id]
         })['result']['qReturn']['qHandle']
         return self.handle
@@ -805,15 +830,15 @@
 #         self.formatUseThou = formatUseThou
 #         self.formatDec = formatDec
 #         self.formatThou = formatThou
         
 #         return zu
     
     def delete(self):
-        zu = Query({
+        zu = Query(self.parent.ws, {
               "jsonrpc": "2.0",
               "id": 10,
               "method": "DestroyDimension",
               "handle": self.appHandle,
               "params": [
                 self.id
               ]
@@ -850,15 +875,15 @@
         
 #         # прописать, что заменяем только в случае успеха
 #         self.name = name
         
 #         return zu
 
 
-# In[26]:
+# In[24]:
 
 
 # version 0.1.22-11-10
 
 class ChildrenIterator:
     def __init__(self, children):
         self.children = children.children
@@ -870,15 +895,15 @@
         if self._index < self._class_size:
             result = self.children[self._keys[self._index]]
             self._index +=1
             return result
         raise StopIteration
 
 
-# In[27]:
+# In[65]:
 
 
 # version 0.1.22-11-10
 # the class, representing different collections of app objects, like master measures or dimensions
 
 class AppChildren():
     def __init__(self, parent, _type):
@@ -887,15 +912,15 @@
         self.parent = parent
         self.appHandle = parent.handle
         self._type = _type
         
     def __getitem__(self, childName):
         if self._type == 'variables':
             if self.count == 0:
-                self.df = GetVarPandas(self.appHandle)
+                self.df = GetVarPandas(self.parent.ws, self.appHandle)
                 for varName in self.df['qName']:
                     var = Variable(self, varName)
                     var.appHandle = self.appHandle
                     
                     row = self.df[self.df['qName'] == varName].iloc[0]
                     var.id = row['qInfo.qId']
                     var.definition = row['qDefinition']
@@ -904,15 +929,15 @@
                     if str(var.scriptCreated) == 'nan': var.scriptCreated = False
 
                     self[varName] = var
                     self.count += 1
         
         if self._type == 'measures':
             if self.count == 0:
-                self.df = GetMsPandas(self.appHandle)
+                self.df = GetMsPandas(self.parent.ws, self.appHandle)
                 for msName in self.df['qMeta.title']:
                     ms = Measure(self, msName)
                     ms.appHandle = self.appHandle
 
                     row = self.df[self.df['qMeta.title'] == msName].iloc[0]
                     ms.id = row['qInfo.qId']
                     ms.definition = row['qData.measure.qDef']
@@ -928,15 +953,15 @@
                     ms.modifiedDate = dt.datetime.strptime(row['qMeta.modifiedDate'], '%Y-%m-%dT%H:%M:%S.%fZ')
 
                     self[msName] = ms
                     self.count += 1
                         
         if self._type == 'sheets':
             if self.count == 0:
-                self.df = GetSheetPandas(self.appHandle)
+                self.df = GetSheetPandas(self.parent.ws, self.appHandle)
                 for shName in self.df['qMeta.title']:
                     sh = Sheet(self, shName)
                     sh.appHandle = self.appHandle
                     
                     row = self.df[self.df['qMeta.title'] == shName].iloc[0]
                     sh.id = row['qInfo.qId']
                     sh.description = row['qMeta.description']
@@ -948,15 +973,15 @@
                     sh.ownerName = row['qMeta.owner.name']
 
                     self[shName] = sh
                     self.count += 1
                     
         if self._type == 'fields':
             if self.count == 0:
-                self.df = GetFieldPandas(self.appHandle)
+                self.df = GetFieldPandas(self.parent.ws, self.appHandle)
                 for fName in self.df['qFields.qName']:
                     f = Field(fName)
                     f.appHandle = self.appHandle
                     
                     row = self.df[self.df['qFields.qName'] == fName].iloc[0]
                     f.tableName = row['qName']
                     f.informationDensity = row['qFields.qInformationDensity']
@@ -969,15 +994,15 @@
                     f.tags = row['qFields.qTags']
 
                     self[fName] = f
                     self.count += 1
                     
         if self._type == 'dimensions':
             if self.count == 0:
-                self.df = GetDimPandas(self.appHandle)
+                self.df = GetDimPandas(self.parent.ws, self.appHandle)
                 for dimName in self.df['qMeta.title']:
                     dim = Dimension(self, dimName)
                     dim.appHandle = self.appHandle
 
                     row = self.df[self.df['qMeta.title'] == dimName].iloc[0]
                     dim.id = row['qInfo.qId']
                     #dim.definition = row['qData.measure.qDef']   добавить
@@ -1006,15 +1031,15 @@
     
     def load(self):
         try: zu = self['']
         except: 1
     
     def add(self, name, definition, description = '', label = '', labelExpression = '', formatType = 'U',                formatNDec = 10, formatUseThou = 0, formatDec = ',', formatThou = ''):
         if self._type == 'variables':
-            zu = Query({
+            zu = Query(self.parent.ws, {
                 "jsonrpc": "2.0",
                 "id": 4,
                 "method": "CreateVariableEx",
                 "handle": self.appHandle,
                 "params": [
                     {
                         "qInfo": {
@@ -1083,15 +1108,15 @@
                             "title": name,
                             "description": description
                                             }
                     }
                 }
             }
             logging.debug(t)
-            zu = Query(t)
+            zu = Query(self.parent.ws, t)
             
             try:
                 if zu['result']['qReturn']['qHandle'] > 0:
                     ms = Measure(self, name)
                     ms.appHandle = self.appHandle
 
                     # renew measures data from app
@@ -1114,15 +1139,15 @@
                     self.count += 1
                     logging.info('Measure created: %s', name)
                 else: logging.error('Failed to create measure: %s', name)
             except: logging.error('Failed to create measure: %s', name)
             return zu
 
 
-# In[28]:
+# In[26]:
 
 
 # version 0.1.22-11-10
 # the class, representing sheets of the application
 # member of App.sheets collection
 
 class Sheet:
@@ -1154,15 +1179,15 @@
               ]
             })['result']['qReturn']['qHandle']
         return self.handle
         
         
 
 
-# In[29]:
+# In[27]:
 
 
 # version 0.1.22-11-10
 # the class, representing collection of objects on the sheet
 
 class SheetChildren():
     def __init__(self, parent):
@@ -1215,15 +1240,15 @@
     
     def load(self):
         try: zu = self['']
         except: 1
     
 
 
-# In[30]:
+# In[28]:
 
 
 # version 0.1.22-11-10
 # the class, representing objects on the sheet, member of SheetChildren collection
 
 class Object:
     def __init__(self, parent, objName):
@@ -1249,15 +1274,15 @@
           "handle": self.appHandle,
           "params": [self.id]
         })['result']['qReturn']['qHandle']
         return self.handle
     
 
 
-# In[31]:
+# In[29]:
 
 
 # version 0.1.22-11-10
 # the class, representing dimensions, used in object on the sheet
 
 class ObjectDimension():
     def __init__(self, parent, dimName):
@@ -1360,15 +1385,15 @@
             logger.info('Dimension deleted: %s', self.name)
             del self.parent[self.name]
         else: logger.error('Failed to delete dimension: %s', self.name)
         
         return zu
 
 
-# In[32]:
+# In[30]:
 
 
 # version 0.1.22-11-10
 # the class, representing measures, used in object on the sheet
 
 class ObjectMeasure():
     def __init__(self, parent, msName):
@@ -1485,15 +1510,15 @@
             logger.info('Measure deleted: %s', self.name)
             del self.parent[self.name]
         else: logger.error('Failed to delete measure: %s', self.name)
         
         return zu
 
 
-# In[33]:
+# In[31]:
 
 
 # version 0.1.22-11-10
 # the class, representing different collections of sheet objects, like measures or dimensions
 
 class ObjectChildren():
     def __init__(self, parent, _type):
```

### Comparing `qsea-0.1.4/qsea.egg-info/PKG-INFO` & `qsea-0.1.5/qsea.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsea
-Version: 0.1.4
+Version: 0.1.5
 Summary: Convenient way to work with Qlik Sense Engine API from Python
 Home-page: https://github.com/ncthuc/qsea
 Download-URL: https://pypi.org/project/qsea/
 Author: Lev Biriukov
 Author-email: lbiryukov@gmail.com
 License: MIT
 Keywords: QlikSense,Qlik
```

### Comparing `qsea-0.1.4/setup.py` & `qsea-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     README = readme_file.read()
 
 with open('HISTORY.md') as history_file:
     HISTORY = history_file.read()
 
 setup_args = dict(
     name='qsea',
-    version='0.1.4',
+    version='0.1.5',
     description='Convenient way to work with Qlik Sense Engine API from Python',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY,
     license='MIT',
     packages=find_packages(),
     author='Lev Biriukov',
     author_email='lbiryukov@gmail.com',
```

