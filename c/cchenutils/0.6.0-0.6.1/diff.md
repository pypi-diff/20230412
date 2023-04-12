# Comparing `tmp/cchenutils-0.6.0-py3-none-any.whl.zip` & `tmp/cchenutils-0.6.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 125300 bytes, number of entries: 107
--rw-rw-rw-  2.0 fat      274 b- defN 23-Apr-12 04:08 cchenutils/__init__.py
--rw-rw-rw-  2.0 fat      394 b- defN 23-Apr-12 06:23 cchenutils/__setup__.py
+Zip file size: 125313 bytes, number of entries: 107
+-rw-rw-rw-  2.0 fat      322 b- defN 23-Apr-12 06:24 cchenutils/__init__.py
+-rw-rw-rw-  2.0 fat      394 b- defN 23-Apr-12 06:24 cchenutils/__setup__.py
 -rw-rw-rw-  2.0 fat     1162 b- defN 23-Apr-11 07:30 cchenutils/_monitor.py
 -rw-rw-rw-  2.0 fat       84 b- defN 23-Apr-11 21:08 cchenutils/call.py
 -rw-rw-rw-  2.0 fat      634 b- defN 23-Apr-12 04:15 cchenutils/dict.py
 -rw-rw-rw-  2.0 fat     1789 b- defN 23-Apr-12 06:21 cchenutils/driver.py
 -rw-rw-rw-  2.0 fat     1064 b- defN 23-Apr-11 07:18 cchenutils/gmail.py
 -rw-rw-rw-  2.0 fat     3542 b- defN 23-Apr-12 05:36 cchenutils/session.py
 -rw-rw-rw-  2.0 fat     3184 b- defN 23-Apr-12 02:06 cchenutils/timer.py
@@ -97,13 +97,13 @@
 -rw-rw-rw-  2.0 fat     3312 b- defN 20-Mar-24 00:35 wanghong/video/prep/wav_split.py
 -rw-rw-rw-  2.0 fat      152 b- defN 20-Mar-26 19:39 wanghong/webscraping/__init__.py
 -rw-rw-rw-  2.0 fat      152 b- defN 20-Mar-26 19:39 wanghong/webscraping/taobao/__init__.py
 -rw-rw-rw-  2.0 fat     4548 b- defN 20-Apr-05 03:47 wanghong/webscraping/taobao/items_cover.py
 -rw-rw-rw-  2.0 fat     4874 b- defN 20-Mar-27 20:44 wanghong/webscraping/taobao/taobao_shopinfo_manual.py
 -rw-rw-rw-  2.0 fat      152 b- defN 20-Mar-26 19:39 wanghong/webscraping/yizhibo/__init__.py
 -rw-rw-rw-  2.0 fat     8389 b- defN 20-Mar-26 19:40 wanghong/webscraping/yizhibo/ts_downbind.py
--rw-rw-rw-  2.0 fat      195 b- defN 23-Apr-12 06:23 cchenutils-0.6.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-12 06:23 cchenutils-0.6.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 23-Apr-12 06:23 cchenutils-0.6.0.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-Apr-12 06:23 cchenutils-0.6.0.dist-info/zip-safe
--rw-rw-r--  2.0 fat     9423 b- defN 23-Apr-12 06:23 cchenutils-0.6.0.dist-info/RECORD
-107 files, 355736 bytes uncompressed, 110318 bytes compressed:  69.0%
+-rw-rw-rw-  2.0 fat      195 b- defN 23-Apr-12 06:24 cchenutils-0.6.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-12 06:24 cchenutils-0.6.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 23-Apr-12 06:24 cchenutils-0.6.1.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Apr-12 06:24 cchenutils-0.6.1.dist-info/zip-safe
+-rw-rw-r--  2.0 fat     9423 b- defN 23-Apr-12 06:24 cchenutils-0.6.1.dist-info/RECORD
+107 files, 355784 bytes uncompressed, 110331 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -300,23 +300,23 @@
 
 Filename: wanghong/webscraping/yizhibo/__init__.py
 Comment: 
 
 Filename: wanghong/webscraping/yizhibo/ts_downbind.py
 Comment: 
 
-Filename: cchenutils-0.6.0.dist-info/METADATA
+Filename: cchenutils-0.6.1.dist-info/METADATA
 Comment: 
 
-Filename: cchenutils-0.6.0.dist-info/WHEEL
+Filename: cchenutils-0.6.1.dist-info/WHEEL
 Comment: 
 
-Filename: cchenutils-0.6.0.dist-info/top_level.txt
+Filename: cchenutils-0.6.1.dist-info/top_level.txt
 Comment: 
 
-Filename: cchenutils-0.6.0.dist-info/zip-safe
+Filename: cchenutils-0.6.1.dist-info/zip-safe
 Comment: 
 
-Filename: cchenutils-0.6.0.dist-info/RECORD
+Filename: cchenutils-0.6.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cchenutils/__init__.py

```diff
@@ -1,11 +1,13 @@
 from .call import call
 from .dict import dict
 from .gmail import Gmail
 from .session import Session
 from .timer import Time, Timer, TimeController
+from .driver import Chrome
 
 __all__ = ['dict',
            'Session',
            'Gmail',
            'Time', 'Timer', 'TimeController',
-           'call']
+           'call',
+           'Chrome']
```

## cchenutils/__setup__.py

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cchenutils',
-    version='0.6.0',
+    version='0.6.1',
     keywords=('utils'),
     description='cc personal use',
     license='MIT License',
     install_requires=[],
     include_package_data=True,
     zip_safe=True,
```

## Comparing `cchenutils-0.6.0.dist-info/RECORD` & `cchenutils-0.6.1.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-cchenutils/__init__.py,sha256=vqBw4WV3EywVUKoyrCaDLobQ6co3g9FGoETzpM8ro-s,274
-cchenutils/__setup__.py,sha256=uynfRIiXnUCIjLKMTD0M6AVTjay3x4DCOVlpbpjvKck,394
+cchenutils/__init__.py,sha256=xodRBp2yEoofqeXf-3zdEtd2UCMQgcHJjPpZ4U9L_wc,322
+cchenutils/__setup__.py,sha256=eJI-Eh_CSd81YEIxcPrFekEVCTkI6EQAVx9l_dbAn7o,394
 cchenutils/_monitor.py,sha256=drOt6YBZGcbb2ZqMqGEslQlZWcCJW3GeN6T-XpHJ5R0,1162
 cchenutils/call.py,sha256=1y6rVCa7EqAxB1tfTLXG1KsTP25nTBYiixlepp5WNrI,84
 cchenutils/dict.py,sha256=qQ8dR1aV9KTCE3WFcJaDy5ihsRbhi-owKDAZupf6O30,634
 cchenutils/driver.py,sha256=sPjrF6A11iFNc51s3EE89X2q8EBNMQAxBmKSu6YPpHI,1789
 cchenutils/gmail.py,sha256=5VIF9-OyzpjWbB0waR1hogtbT66ZqXwFeaCPdrIcMko,1064
 cchenutils/session.py,sha256=8oJsgpF-OqrVdp8qKiTozPq_IH4drW7vdF8klqfRK4E,3542
 cchenutils/timer.py,sha256=ECPgVj_-8YNVeUUfScDkdwMUNJqONdWsopFT_UfRLt0,3184
@@ -96,12 +96,12 @@
 wanghong/video/prep/wav_split.py,sha256=UJ6iKDszpjRtpxGfE_-h_GAa_uT1dXd0ll_7zJ_2Icc,3312
 wanghong/webscraping/__init__.py,sha256=Zx53GK5f04rgk2G04neuZcLGRhYHCNKBWtimzB1dwIQ,152
 wanghong/webscraping/taobao/__init__.py,sha256=Zx53GK5f04rgk2G04neuZcLGRhYHCNKBWtimzB1dwIQ,152
 wanghong/webscraping/taobao/items_cover.py,sha256=xt1swF6RCnpR0eLJMsuhEkyLqw9M9GGa4BZfoPI-Egs,4548
 wanghong/webscraping/taobao/taobao_shopinfo_manual.py,sha256=wYjqTHCW4NcU8Qy8eLIi-ZpNgsXsNYeXeP7-eyMtVTw,4874
 wanghong/webscraping/yizhibo/__init__.py,sha256=Zx53GK5f04rgk2G04neuZcLGRhYHCNKBWtimzB1dwIQ,152
 wanghong/webscraping/yizhibo/ts_downbind.py,sha256=u-VOJl_EAsoA4Ep81XdF0GXeSc3Vr1QkmXnLDBca79o,8389
-cchenutils-0.6.0.dist-info/METADATA,sha256=zhbWOeNV0JGjO6i38XxnbX3-VsjblzS090a_ldpdAIU,195
-cchenutils-0.6.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-cchenutils-0.6.0.dist-info/top_level.txt,sha256=xLXRttimPVQEG1OBK3Vhwo65HZYG6DovfViIUG2CNRw,20
-cchenutils-0.6.0.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-cchenutils-0.6.0.dist-info/RECORD,,
+cchenutils-0.6.1.dist-info/METADATA,sha256=06fc55IDYIR-jeUmH2DuzdaJ6VPviF8-t_jBHULoUw0,195
+cchenutils-0.6.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+cchenutils-0.6.1.dist-info/top_level.txt,sha256=xLXRttimPVQEG1OBK3Vhwo65HZYG6DovfViIUG2CNRw,20
+cchenutils-0.6.1.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+cchenutils-0.6.1.dist-info/RECORD,,
```

