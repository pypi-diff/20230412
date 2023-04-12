# Comparing `tmp/snemail-1.1.13.tar.gz` & `tmp/snemail-1.1.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snemail-1.1.13.tar", last modified: Mon Apr 10 03:30:20 2023, max compression
+gzip compressed data, was "snemail-1.1.14.tar", last modified: Wed Apr 12 02:25:51 2023, max compression
```

## Comparing `snemail-1.1.13.tar` & `snemail-1.1.14.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 03:30:20.820922 snemail-1.1.13/
--rw-rw-rw-   0        0        0     1091 2023-04-10 02:22:39.000000 snemail-1.1.13/LICENSE
--rw-rw-rw-   0        0        0     4002 2023-04-10 03:30:20.820922 snemail-1.1.13/PKG-INFO
--rw-rw-rw-   0        0        0     3594 2023-04-10 02:22:39.000000 snemail-1.1.13/README.md
--rw-rw-rw-   0        0        0       42 2023-04-10 03:30:20.820922 snemail-1.1.13/setup.cfg
--rw-rw-rw-   0        0        0     1042 2023-04-10 03:29:57.000000 snemail-1.1.13/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 03:30:20.806920 snemail-1.1.13/snemail/
--rw-rw-rw-   0        0        0       22 2023-04-10 02:22:39.000000 snemail-1.1.13/snemail/__init__.py
--rw-rw-rw-   0        0        0     7663 2023-04-10 03:29:50.000000 snemail-1.1.13/snemail/package.py
-drwxrwxrwx   0        0        0        0 2023-04-10 03:30:20.818259 snemail-1.1.13/snemail.egg-info/
--rw-rw-rw-   0        0        0     4002 2023-04-10 03:30:20.000000 snemail-1.1.13/snemail.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-04-10 03:30:20.000000 snemail-1.1.13/snemail.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 03:30:20.000000 snemail-1.1.13/snemail.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-10 03:30:20.000000 snemail-1.1.13/snemail.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-10 03:30:20.819256 snemail-1.1.13/test/
--rw-rw-rw-   0        0        0      570 2023-04-10 02:27:22.000000 snemail-1.1.13/test/test_demp.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:25:51.088249 snemail-1.1.14/
+-rw-rw-rw-   0        0        0     1091 2023-04-10 02:22:39.000000 snemail-1.1.14/LICENSE
+-rw-rw-rw-   0        0        0     4002 2023-04-12 02:25:51.088249 snemail-1.1.14/PKG-INFO
+-rw-rw-rw-   0        0        0     3594 2023-04-10 02:22:39.000000 snemail-1.1.14/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-12 02:25:51.088249 snemail-1.1.14/setup.cfg
+-rw-rw-rw-   0        0        0     1042 2023-04-12 02:25:20.000000 snemail-1.1.14/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:25:51.073286 snemail-1.1.14/snemail/
+-rw-rw-rw-   0        0        0       22 2023-04-10 02:22:39.000000 snemail-1.1.14/snemail/__init__.py
+-rw-rw-rw-   0        0        0     7652 2023-04-12 02:25:15.000000 snemail-1.1.14/snemail/package.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:25:51.086255 snemail-1.1.14/snemail.egg-info/
+-rw-rw-rw-   0        0        0     4002 2023-04-12 02:25:50.000000 snemail-1.1.14/snemail.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2023-04-12 02:25:50.000000 snemail-1.1.14/snemail.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 02:25:50.000000 snemail-1.1.14/snemail.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-12 02:25:50.000000 snemail-1.1.14/snemail.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 02:25:51.087252 snemail-1.1.14/test/
+-rw-rw-rw-   0        0        0      573 2023-04-10 03:33:26.000000 snemail-1.1.14/test/test_demp.py
```

### Comparing `snemail-1.1.13/LICENSE` & `snemail-1.1.14/LICENSE`

 * *Files identical despite different names*

### Comparing `snemail-1.1.13/PKG-INFO` & `snemail-1.1.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snemail
-Version: 1.1.13
+Version: 1.1.14
 Summary: 发送邮件库
 Home-page: https://github.com/majormj/sendmail
 Author: manji
 Author-email: pnsm@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `snemail-1.1.13/README.md` & `snemail-1.1.14/README.md`

 * *Files identical despite different names*

### Comparing `snemail-1.1.13/setup.py` & `snemail-1.1.14/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="snemail",
-    version="1.1.13",
+    version="1.1.14",
     author="manji",
     author_email="pnsm@qq.com",                         # 作者邮箱
     description="发送邮件库",                            # 模块简介
     long_description=long_description,                  # 模块详细介绍
     long_description_content_type="text/markdown",      # 模块详细介绍格式
     url="https://github.com/majormj/sendmail",
     packages=setuptools.find_packages(),                # 自动找到项目中导入的模块
```

### Comparing `snemail-1.1.13/snemail/package.py` & `snemail-1.1.14/snemail/package.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
 
         if any([emailTo,emailCC]):
             self.msg['To']      = ";".join(emailTo)    # 显示的收件人 # ’收件人1；收件人2；收件人3....‘
             self.msg['cc']      = ";".join(emailCC)    # 显示的抄送人 用; 分割
         else:
             return '收件人或者抄送人必须有至少一个不为空'
         
-        emailToTure = ";".join(set(emailTo + emailCC ) - set(emailNoSend))  # 实际发送的邮件列表
+        emailToTure = set(emailTo + emailCC ) - set(emailNoSend) # 实际发送的邮件列表
         if not "@" in emailToTure  :
             return "不存在实际的邮件接收人，请检查。"
 
         # 发送邮件
         try:
             if self.loginStatus:
                 self.con.sendmail(self.emailCome,emailToTure,self.msg.as_string())
```

### Comparing `snemail-1.1.13/snemail.egg-info/PKG-INFO` & `snemail-1.1.14/snemail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snemail
-Version: 1.1.13
+Version: 1.1.14
 Summary: 发送邮件库
 Home-page: https://github.com/majormj/sendmail
 Author: manji
 Author-email: pnsm@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `snemail-1.1.13/test/test_demp.py` & `snemail-1.1.14/test/test_demp.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,11 +14,11 @@
     # 邮件正文图片
     sn.mail_image(image_path="")
 
     # 设置附件
     sn.mail_file([r"C:\Users\manji\Downloads\全量商品列表.xlsx"])
 
     # 登录邮箱
-    print(sn.login(user="",password=""))
+    print(sn.mail_login(user="",password=""))
 
     # 发送邮件
-    print(sn.mail_send(emailTo=['']))
+    print(sn.mail_send(emailTo=[]))
```

