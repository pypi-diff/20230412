# Comparing `tmp/stathub-0.1.3-py3-none-any.whl.zip` & `tmp/stathub-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1907 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     1120 b- defN 23-Apr-12 04:16 stathub/stathub.py
--rw-rw-rw-  2.0 fat      667 b- defN 23-Apr-12 06:53 stathub-0.1.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-12 06:53 stathub-0.1.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-12 06:53 stathub-0.1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      371 b- defN 23-Apr-12 06:53 stathub-0.1.3.dist-info/RECORD
-5 files, 2258 bytes uncompressed, 1213 bytes compressed:  46.3%
+Zip file size: 2042 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     1536 b- defN 23-Apr-12 08:33 stathub/stathub.py
+-rw-rw-rw-  2.0 fat      673 b- defN 23-Apr-12 08:39 stathub-0.1.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-12 08:39 stathub-0.1.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-12 08:39 stathub-0.1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      371 b- defN 23-Apr-12 08:39 stathub-0.1.4.dist-info/RECORD
+5 files, 2680 bytes uncompressed, 1348 bytes compressed:  49.7%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: stathub/stathub.py
 Comment: 
 
-Filename: stathub-0.1.3.dist-info/METADATA
+Filename: stathub-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: stathub-0.1.3.dist-info/WHEEL
+Filename: stathub-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: stathub-0.1.3.dist-info/top_level.txt
+Filename: stathub-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: stathub-0.1.3.dist-info/RECORD
+Filename: stathub-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## stathub/stathub.py

```diff
@@ -1,15 +1,20 @@
 def getdata(dataflow,version="1.0",start="",end="",language="th",label='name'):
     import requests
     import io
     import pandas as pd
     if (end != ""):
         end = "&endPeriod="+str(end)
+    if (label == "name"):
+        nlabel = "both"
+    else:
+        nlabel = label
+        
     r=requests.get("https://ns1-stathub.nso.go.th/rest/data/TNSO,"+dataflow+","+version+"/?startPeriod="+str(start)+end+"&dimensionAtObservation=AllDimensions",
-                   headers={"Accept":"application/vnd.sdmx.data+csv;file=true;labels="+label,"Accept-Language" : language}).content
+                   headers={"Accept":"application/vnd.sdmx.data+csv;file=true;labels="+nlabel,"Accept-Language" : language}).content
     rawData = pd.read_csv(io.StringIO(r.decode('utf-8')))
     if(label=="name"):
         nrow = rawData.shape[0]
         ncol = rawData.shape[1]
         for i in range(0,nrow):
             for j in range(0,ncol):
                 element = str(rawData.iat[i,j]).split(": ")
@@ -19,7 +24,15 @@
         for i in range(0,len(names)):
             element = str(names[i]).split(": ")
             if (len(element)>1):
                 names[i] = element[1]
         rawData.columns = names
     return rawData
 
+def dataexport(data,path="",exporttype='csv'):
+    import pandas as pd
+    if (exporttype=='csv'):
+        out = path+"output.csv"
+        data.to_csv(out, index=False, header=True, mode='a')
+    elif (exporttype=='excel'):
+        out = path+"output.xlsx"
+        data.to_excel(out, index=False, header=True)
```

## Comparing `stathub-0.1.3.dist-info/METADATA` & `stathub-0.1.4.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: stathub
-Version: 0.1.3
-Summary: A python package used for getting data from Statistics Sharing Hub
+Version: 0.1.4
+Summary: A python package used for getting data from Statistics Sharing Hub.
 Home-page: https://pypi.org/project/stathub
 Author: Government Strategic Information Center​
 Author-email: sdmx.tnso@gmail.com
 Requires-Python: >=3.8
 Requires-Dist: pandas
 Requires-Dist: requests
-
-## Project Description
+Requires-Dist: openpyxl
 
 This python package can be used for accessing and getting datasets from Statistics Sharing Hub (stathub.nso.go.th) maintained by Government Strategic Information Center​, National Statistical Office of Thailand.
 
-## Prerequisite Packages
-
+# Prerequisite Packages
 - pandas
 - requests
+- openpyxl
 
-## Contact
-
+# Contact
 sdmx.tnso@gmail.com
```

