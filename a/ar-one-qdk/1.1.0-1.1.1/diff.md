# Comparing `tmp/ar_one_qdk-1.1.0-py3-none-any.whl.zip` & `tmp/ar_one_qdk-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5006 bytes, number of entries: 9
+Zip file size: 5029 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Oct-13 06:51 ar_qdk/__init__.py
--rw-rw-rw-  2.0 fat     8724 b- defN 23-Apr-10 08:18 ar_qdk/main.py
+-rw-rw-rw-  2.0 fat     8871 b- defN 23-Apr-12 12:11 ar_qdk/main.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Oct-13 08:32 ar_qdk/tests/__init__.py
 -rw-rw-rw-  2.0 fat     1007 b- defN 22-Mar-17 06:07 ar_qdk/tests/main_test.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-10 08:19 ar_one_qdk-1.1.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      229 b- defN 23-Apr-10 08:19 ar_one_qdk-1.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-10 08:19 ar_one_qdk-1.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-10 08:19 ar_one_qdk-1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      702 b- defN 23-Apr-10 08:19 ar_one_qdk-1.1.0.dist-info/RECORD
-9 files, 11852 bytes uncompressed, 3790 bytes compressed:  68.0%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-12 12:12 ar_one_qdk-1.1.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      229 b- defN 23-Apr-12 12:12 ar_one_qdk-1.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-12 12:12 ar_one_qdk-1.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-12 12:12 ar_one_qdk-1.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      702 b- defN 23-Apr-12 12:12 ar_one_qdk-1.1.1.dist-info/RECORD
+9 files, 11999 bytes uncompressed, 3813 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: ar_qdk/tests/__init__.py
 Comment: 
 
 Filename: ar_qdk/tests/main_test.py
 Comment: 
 
-Filename: ar_one_qdk-1.1.0.dist-info/LICENSE
+Filename: ar_one_qdk-1.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: ar_one_qdk-1.1.0.dist-info/METADATA
+Filename: ar_one_qdk-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: ar_one_qdk-1.1.0.dist-info/WHEEL
+Filename: ar_one_qdk-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: ar_one_qdk-1.1.0.dist-info/top_level.txt
+Filename: ar_one_qdk-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: ar_one_qdk-1.1.0.dist-info/RECORD
+Filename: ar_one_qdk-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ar_qdk/main.py

```diff
@@ -34,25 +34,27 @@
         :param comment: Комментарий.
         :return:
         """
         return self.execute_method('add_comment', record_id=record_id,
                                    comment=comment)
 
     def operate_gate_manual_control(self, operation, gate_name,
-                                    auto_close=False, **kwargs):
+                                    auto_close=False,  smart_auto_close=False,
+                                    *args, **kwargs):
         """
         Работа со шлагбаумами.
 
         :param operation: Название операции (close|open):
         :param gate_name: Имя шлагбаума (entry/exit)
         :return:
         """
         return self.execute_method('operate_gate_manual_control',
+                                   smart_auto_close=smart_auto_close,
                                    operation=operation, gate_name=gate_name,
-                                   auto_close=auto_close, **kwargs)
+                                   auto_close=auto_close, *args, **kwargs)
 
     def change_opened_record(self, record_id, auto_id, car_number, carrier,
                              trash_cat_id, trash_type_id, comment, pol_object,
                              client=None, polygon=None):
         """
         Изменить открытую запись.
```

## Comparing `ar_one_qdk-1.1.0.dist-info/LICENSE` & `ar_one_qdk-1.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

