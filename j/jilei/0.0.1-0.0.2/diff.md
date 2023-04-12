# Comparing `tmp/jilei-0.0.1-py3-none-any.whl.zip` & `tmp/jilei-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1952 bytes, number of entries: 6
+Zip file size: 1652 bytes, number of entries: 6
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-12 11:09 jilei/__init__.py
--rw-rw-rw-  2.0 fat      958 b- defN 23-Apr-12 11:13 jilei/wxwork.py
--rw-rw-rw-  2.0 fat      390 b- defN 23-Apr-12 11:19 jilei-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-12 11:19 jilei-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-12 11:19 jilei-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      430 b- defN 23-Apr-12 11:19 jilei-0.0.1.dist-info/RECORD
-6 files, 1876 bytes uncompressed, 1170 bytes compressed:  37.6%
+-rw-rw-rw-  2.0 fat      279 b- defN 23-Apr-12 11:27 jilei/wxwork.py
+-rw-rw-rw-  2.0 fat      390 b- defN 23-Apr-12 11:27 jilei-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-12 11:27 jilei-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-12 11:27 jilei-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      430 b- defN 23-Apr-12 11:27 jilei-0.0.2.dist-info/RECORD
+6 files, 1197 bytes uncompressed, 870 bytes compressed:  27.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: jilei/__init__.py
 Comment: 
 
 Filename: jilei/wxwork.py
 Comment: 
 
-Filename: jilei-0.0.1.dist-info/METADATA
+Filename: jilei-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: jilei-0.0.1.dist-info/WHEEL
+Filename: jilei-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: jilei-0.0.1.dist-info/top_level.txt
+Filename: jilei-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: jilei-0.0.1.dist-info/RECORD
+Filename: jilei-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jilei/wxwork.py

```diff
@@ -1,33 +1,10 @@
 import requests
 import json
 
-group_robot_webhooks = {
-    "技术部": "https://qyapi.weixin.qq.com/cgi-bin/webhook/send?key=8a301828-8d89-4fb8-b9e5-3e6f8a6a8474",
-    "nnUNet-子炀PC": "https://qyapi.weixin.qq.com/cgi-bin/webhook/send?key=f66f9b7b-685d-42af-8a64-077278422015"
-}
-
-text_msg = {
-    "msgtype": "text",
-    "text": {
-        "content": "测试一下",
-        "mentioned_list": ["朱剑波", "@all"],
-        "mentioned_mobile_list": ["13850004174", "@all"]
-    }
-}
-
-markdown_msg = {
-    "msgtype": "markdown",
-    "markdown": {
-        "content": "<font color='red'>markdown</font>\n"
-                   "# 一级标题\n"
-                   "## 二级标题"
-    }
-}
-
 
 def group_notify(key, msg="测试数据"):
     url = f'https://qyapi.weixin.qq.com/cgi-bin/webhook/send?key={key}'
     headers = {"Content-Type": "application/json"}
     resp = requests.post(url, headers=headers, data=json.dumps(msg))
```

