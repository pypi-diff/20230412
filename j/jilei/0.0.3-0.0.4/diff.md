# Comparing `tmp/jilei-0.0.3-py3-none-any.whl.zip` & `tmp/jilei-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1699 bytes, number of entries: 6
+Zip file size: 1701 bytes, number of entries: 6
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-12 11:09 jilei/__init__.py
--rw-rw-rw-  2.0 fat      326 b- defN 23-Apr-12 11:33 jilei/wxwork.py
--rw-rw-rw-  2.0 fat      431 b- defN 23-Apr-12 11:35 jilei-0.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-12 11:35 jilei-0.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-12 11:35 jilei-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      430 b- defN 23-Apr-12 11:35 jilei-0.0.3.dist-info/RECORD
-6 files, 1285 bytes uncompressed, 917 bytes compressed:  28.6%
+-rw-rw-rw-  2.0 fat      322 b- defN 23-Apr-12 11:37 jilei/wxwork.py
+-rw-rw-rw-  2.0 fat      431 b- defN 23-Apr-12 11:38 jilei-0.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-12 11:38 jilei-0.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-12 11:38 jilei-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      430 b- defN 23-Apr-12 11:38 jilei-0.0.4.dist-info/RECORD
+6 files, 1281 bytes uncompressed, 919 bytes compressed:  28.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: jilei/__init__.py
 Comment: 
 
 Filename: jilei/wxwork.py
 Comment: 
 
-Filename: jilei-0.0.3.dist-info/METADATA
+Filename: jilei-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: jilei-0.0.3.dist-info/WHEEL
+Filename: jilei-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: jilei-0.0.3.dist-info/top_level.txt
+Filename: jilei-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: jilei-0.0.3.dist-info/RECORD
+Filename: jilei-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jilei/wxwork.py

```diff
@@ -1,13 +1,11 @@
-import requests
 import json
-
-
+import requests
 
 
 def group_notify(key, msg={"msgtype": "text", "text": { "content": "测试消息"}}):
     url = f'https://qyapi.weixin.qq.com/cgi-bin/webhook/send?key={key}'
     headers = {"Content-Type": "application/json"}
-    resp = requests.post(url, headers=headers, data=json.dumps(msg))
+    return requests.post(url, headers=headers, data=json.dumps(msg))
```

