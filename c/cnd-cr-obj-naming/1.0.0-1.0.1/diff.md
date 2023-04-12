# Comparing `tmp/cnd_cr_obj_naming-1.0.0-py3-none-any.whl.zip` & `tmp/cnd_cr_obj_naming-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 3462 bytes, number of entries: 9
--rw-rw-rw-  2.0 unx        5 b- defN 23-Apr-12 00:26 cr_obj_naming/VERSION
--rw-r--r--  2.0 unx      187 b- defN 23-Apr-12 00:26 cr_obj_naming/__init__.py
--rw-r--r--  2.0 unx      122 b- defN 23-Apr-12 00:26 cr_obj_naming/__version__.py
--rw-r--r--  2.0 unx     1454 b- defN 23-Apr-12 00:26 cr_obj_naming/cnd_consul.py
--rw-r--r--  2.0 unx     1452 b- defN 23-Apr-12 00:26 cr_obj_naming/obj_naming.py
--rw-r--r--  2.0 unx      825 b- defN 23-Apr-12 00:26 cnd_cr_obj_naming-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 00:26 cnd_cr_obj_naming-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Apr-12 00:26 cnd_cr_obj_naming-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      745 b- defN 23-Apr-12 00:26 cnd_cr_obj_naming-1.0.0.dist-info/RECORD
-9 files, 4896 bytes uncompressed, 2164 bytes compressed:  55.8%
+Zip file size: 3465 bytes, number of entries: 9
+-rw-rw-rw-  2.0 unx        5 b- defN 23-Apr-12 13:13 cr_obj_naming/VERSION
+-rw-r--r--  2.0 unx      187 b- defN 23-Apr-12 13:13 cr_obj_naming/__init__.py
+-rw-r--r--  2.0 unx      122 b- defN 23-Apr-12 13:13 cr_obj_naming/__version__.py
+-rw-r--r--  2.0 unx     1454 b- defN 23-Apr-12 13:13 cr_obj_naming/cnd_consul.py
+-rw-r--r--  2.0 unx     1456 b- defN 23-Apr-12 13:13 cr_obj_naming/obj_naming.py
+-rw-r--r--  2.0 unx      825 b- defN 23-Apr-12 13:13 cnd_cr_obj_naming-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 13:13 cnd_cr_obj_naming-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Apr-12 13:13 cnd_cr_obj_naming-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      745 b- defN 23-Apr-12 13:13 cnd_cr_obj_naming-1.0.1.dist-info/RECORD
+9 files, 4900 bytes uncompressed, 2167 bytes compressed:  55.8%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: cr_obj_naming/cnd_consul.py
 Comment: 
 
 Filename: cr_obj_naming/obj_naming.py
 Comment: 
 
-Filename: cnd_cr_obj_naming-1.0.0.dist-info/METADATA
+Filename: cnd_cr_obj_naming-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: cnd_cr_obj_naming-1.0.0.dist-info/WHEEL
+Filename: cnd_cr_obj_naming-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: cnd_cr_obj_naming-1.0.0.dist-info/top_level.txt
+Filename: cnd_cr_obj_naming-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: cnd_cr_obj_naming-1.0.0.dist-info/RECORD
+Filename: cnd_cr_obj_naming-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cr_obj_naming/VERSION

```diff
@@ -1 +1 @@
-1.0.0
+1.0.1
```

## cr_obj_naming/obj_naming.py

```diff
@@ -8,15 +8,15 @@
     def __init__(self, data, cnd_consul, md5_length, _print):
         super().__init__(_print)
         self._data = data
         self._cnd_consul = cnd_consul
         self._md5_length = md5_length
 
     def _value(self):
-        base_string = f"{self._data['vra_id']}-{self._data['service_name']}-{self._data['env']}"
+        base_string = f"aria{self._data['vra_id']}-{self._data['service_name']}-{self._data['env']}"
         hash_val = hashlib.md5(f"{base_string}-{self._data['deployment_id']}".encode())
         return f"{base_string}-{hash_val.hexdigest()[0:self._md5_length]}"
 
     def all(self):
         return self._cnd_consul.all()
 
     @property
```

## Comparing `cnd_cr_obj_naming-1.0.0.dist-info/METADATA` & `cnd_cr_obj_naming-1.0.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnd-cr-obj-naming
-Version: 1.0.0
+Version: 1.0.1
 Summary: Base for vro Custom Resource Object Naming
 Home-page: https://gitlab.com/changendevops/cloudtools/cnd-cr-object.git
 Author: Denis FABIEN
 Author-email: denis.fabien@changendevops.com
 License: MIT/X11
 Project-URL: Documentation, https://changendevops.com
 Project-URL: Source, https://gitlab.com/changendevops/cloudtools/cnd-cr-object.git
```

## Comparing `cnd_cr_obj_naming-1.0.0.dist-info/RECORD` & `cnd_cr_obj_naming-1.0.1.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-cr_obj_naming/VERSION,sha256=klIfw8vZZL3J9YSpkbif3apXVO0cyW1tQkRTOGacEwU,5
+cr_obj_naming/VERSION,sha256=1R5uyUBYVUqEVYpbQC7m71_fVFXjXJAv7aYc2odSlDo,5
 cr_obj_naming/__init__.py,sha256=1uv3gz09BL1cmYDLPne0PkqXcvqxLP9jy2DjeeyDCrA,187
 cr_obj_naming/__version__.py,sha256=ikxlExFPaHGK8AzUG9pDnI7Sm8GtkjdM12d5iJMRgik,122
 cr_obj_naming/cnd_consul.py,sha256=Y1651yLtYfWz6z-Cfz9hwXyplHkF8bS8fiOY7b_FaZ0,1454
-cr_obj_naming/obj_naming.py,sha256=uKdroR-S5w7qR9-0-4hAlVNkgivapouuoRGe5P1blBw,1452
-cnd_cr_obj_naming-1.0.0.dist-info/METADATA,sha256=4kGfg8pvh1plM_5uwvbyE2Ujbeqvv4tc0k2alF_hCv0,825
-cnd_cr_obj_naming-1.0.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-cnd_cr_obj_naming-1.0.0.dist-info/top_level.txt,sha256=IxheoHqwoyK8b3XMzAfOoe8Owc9qJeKmqwl2BTPOmBU,14
-cnd_cr_obj_naming-1.0.0.dist-info/RECORD,,
+cr_obj_naming/obj_naming.py,sha256=-U-exAK7zbnDEKECyjWvhN5ErsmPBK47rybAlu4Qs_4,1456
+cnd_cr_obj_naming-1.0.1.dist-info/METADATA,sha256=TXCWtxbEQebIaHG5SqE-AQ68-L24fLBxmRKNpH2IEac,825
+cnd_cr_obj_naming-1.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+cnd_cr_obj_naming-1.0.1.dist-info/top_level.txt,sha256=IxheoHqwoyK8b3XMzAfOoe8Owc9qJeKmqwl2BTPOmBU,14
+cnd_cr_obj_naming-1.0.1.dist-info/RECORD,,
```

