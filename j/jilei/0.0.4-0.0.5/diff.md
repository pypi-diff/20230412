# Comparing `tmp/jilei-0.0.4-py3-none-any.whl.zip` & `tmp/jilei-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1701 bytes, number of entries: 6
+Zip file size: 1992 bytes, number of entries: 6
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-12 11:09 jilei/__init__.py
--rw-rw-rw-  2.0 fat      322 b- defN 23-Apr-12 11:37 jilei/wxwork.py
--rw-rw-rw-  2.0 fat      431 b- defN 23-Apr-12 11:38 jilei-0.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-12 11:38 jilei-0.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-12 11:38 jilei-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      430 b- defN 23-Apr-12 11:38 jilei-0.0.4.dist-info/RECORD
-6 files, 1281 bytes uncompressed, 919 bytes compressed:  28.3%
+-rw-rw-rw-  2.0 fat     1107 b- defN 23-Apr-12 12:17 jilei/wxwork.py
+-rw-rw-rw-  2.0 fat      431 b- defN 23-Apr-12 12:17 jilei-0.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-12 12:17 jilei-0.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-12 12:17 jilei-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      431 b- defN 23-Apr-12 12:17 jilei-0.0.5.dist-info/RECORD
+6 files, 2067 bytes uncompressed, 1210 bytes compressed:  41.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: jilei/__init__.py
 Comment: 
 
 Filename: jilei/wxwork.py
 Comment: 
 
-Filename: jilei-0.0.4.dist-info/METADATA
+Filename: jilei-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: jilei-0.0.4.dist-info/WHEEL
+Filename: jilei-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: jilei-0.0.4.dist-info/top_level.txt
+Filename: jilei-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: jilei-0.0.4.dist-info/RECORD
+Filename: jilei-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jilei/wxwork.py

```diff
@@ -4,8 +4,26 @@
 
 def group_notify(key, msg={"msgtype": "text", "text": { "content": "测试消息"}}):
     url = f'https://qyapi.weixin.qq.com/cgi-bin/webhook/send?key={key}'
     headers = {"Content-Type": "application/json"}
     return requests.post(url, headers=headers, data=json.dumps(msg))
 
 
+def generate_nnunet_template(total_epoch, current_epoch, train_loss, val_loss, pseudo_dice, learning_rate, epoch_time, best_dice):
+    """ 使用Markdown风格发送
+    """
+    markdown = f"# <font color='red'>NEW BEST DICE: {best_dice}!</font>\n" if best_dice else ""
+    markdown = markdown + f"**Epoch No.{current_epoch}** / {total_epoch}\n"
+    markdown = markdown + f"**train_loss**:     {train_loss}\n"
+    markdown = markdown + f"**var_loss**:       {val_loss}\n"
+    markdown = markdown + f"**pseudo_dice**:    {pseudo_dice}\n"
+    markdown = markdown + f"**learning_rate**:  {learning_rate}\n"
+    markdown = markdown + f"{epoch_time}s"
+    return {
+        "msgtype": "markdown",
+        "markdown": {
+            "content": markdown
+            }
+    }
+
+
```

