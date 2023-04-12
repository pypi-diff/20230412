# Comparing `tmp/cnd_cr_obj_naming-0.2.3-py3-none-any.whl.zip` & `tmp/cnd_cr_obj_naming-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 3475 bytes, number of entries: 9
--rw-rw-rw-  2.0 unx        5 b- defN 23-Apr-11 21:16 cr_obj_naming/VERSION
--rw-r--r--  2.0 unx      187 b- defN 23-Apr-11 21:16 cr_obj_naming/__init__.py
--rw-r--r--  2.0 unx      122 b- defN 23-Apr-11 21:16 cr_obj_naming/__version__.py
--rw-r--r--  2.0 unx     1459 b- defN 23-Apr-11 21:16 cr_obj_naming/cnd_consul.py
--rw-r--r--  2.0 unx     1433 b- defN 23-Apr-11 21:16 cr_obj_naming/obj_naming.py
--rw-r--r--  2.0 unx      825 b- defN 23-Apr-11 21:17 cnd_cr_obj_naming-0.2.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 21:17 cnd_cr_obj_naming-0.2.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Apr-11 21:17 cnd_cr_obj_naming-0.2.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      745 b- defN 23-Apr-11 21:17 cnd_cr_obj_naming-0.2.3.dist-info/RECORD
-9 files, 4882 bytes uncompressed, 2177 bytes compressed:  55.4%
+Zip file size: 3462 bytes, number of entries: 9
+-rw-rw-rw-  2.0 unx        5 b- defN 23-Apr-12 00:26 cr_obj_naming/VERSION
+-rw-r--r--  2.0 unx      187 b- defN 23-Apr-12 00:26 cr_obj_naming/__init__.py
+-rw-r--r--  2.0 unx      122 b- defN 23-Apr-12 00:26 cr_obj_naming/__version__.py
+-rw-r--r--  2.0 unx     1454 b- defN 23-Apr-12 00:26 cr_obj_naming/cnd_consul.py
+-rw-r--r--  2.0 unx     1452 b- defN 23-Apr-12 00:26 cr_obj_naming/obj_naming.py
+-rw-r--r--  2.0 unx      825 b- defN 23-Apr-12 00:26 cnd_cr_obj_naming-1.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 00:26 cnd_cr_obj_naming-1.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Apr-12 00:26 cnd_cr_obj_naming-1.0.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      745 b- defN 23-Apr-12 00:26 cnd_cr_obj_naming-1.0.0.dist-info/RECORD
+9 files, 4896 bytes uncompressed, 2164 bytes compressed:  55.8%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: cr_obj_naming/cnd_consul.py
 Comment: 
 
 Filename: cr_obj_naming/obj_naming.py
 Comment: 
 
-Filename: cnd_cr_obj_naming-0.2.3.dist-info/METADATA
+Filename: cnd_cr_obj_naming-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: cnd_cr_obj_naming-0.2.3.dist-info/WHEEL
+Filename: cnd_cr_obj_naming-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: cnd_cr_obj_naming-0.2.3.dist-info/top_level.txt
+Filename: cnd_cr_obj_naming-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: cnd_cr_obj_naming-0.2.3.dist-info/RECORD
+Filename: cnd_cr_obj_naming-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cr_obj_naming/VERSION

```diff
@@ -1 +1 @@
-0.2.3
+1.0.0
```

## cr_obj_naming/cnd_consul.py

```diff
@@ -24,19 +24,19 @@
 		str = f'{self.consul_creds["path"]}/'
 		if deployment_id is not None:
 			str = f'{str}{deployment_id}'
 		self._print.trace_d(f'Path : {str}')
 		return str
 
 	def all(self):
-		index, paths = self.consul.kv.get(self.full_path(), recurse=True, keys=True)
+		index, paths = self.consul.kv.get(self.full_path(), recurse=True)
 		self._print.trace_d(f'Returned value : {paths}')
 		result = []
 		for path in paths:
-			result.append(path.split('/')[-1])
+			result.append(json.loads(path["Value"]))
 		self._print.trace_d(f'Item returned len : {len(result)}')
 		return result
 
 	def get(self, id=None):
 		index, my_data = self.consul.kv.get(self.full_path(id))
 		self._print.trace_d(f'Raw data : {my_data}')
 		return json.loads(my_data['Value'])
```

## cr_obj_naming/obj_naming.py

```diff
@@ -26,20 +26,21 @@
     @data.setter
     def data(self, my_data):
         self._data = my_data
         
     def save(self):
         self._data["name"] = self._value()
         self._print.trace_d(f'DeploymentId : {self._data["name"]}')
-        return self._cnd_consul.put(self._data["deployment_id"], self._data)
+        self._cnd_consul.put(self._data["deployment_id"], self._data)
+        return self._data["name"]
 
     def find_by_id(self, id):
         my_data = self._cnd_consul.get(id)
         self._print.trace_d(f'Raw data : {my_data}')
-        return my_data["name"]
+        return my_data
         
     def update(self):
         return self.save()
         
     def destroy(self):
         return self._cnd_consul.destroy(self._data["deployment_id"])
```

## Comparing `cnd_cr_obj_naming-0.2.3.dist-info/METADATA` & `cnd_cr_obj_naming-1.0.0.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnd-cr-obj-naming
-Version: 0.2.3
+Version: 1.0.0
 Summary: Base for vro Custom Resource Object Naming
 Home-page: https://gitlab.com/changendevops/cloudtools/cnd-cr-object.git
 Author: Denis FABIEN
 Author-email: denis.fabien@changendevops.com
 License: MIT/X11
 Project-URL: Documentation, https://changendevops.com
 Project-URL: Source, https://gitlab.com/changendevops/cloudtools/cnd-cr-object.git
```

## Comparing `cnd_cr_obj_naming-0.2.3.dist-info/RECORD` & `cnd_cr_obj_naming-1.0.0.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-cr_obj_naming/VERSION,sha256=XSSKc1S0uwOYYmkC_fs0xKSWJb5x9x3if9NA5sO4Xkw,5
+cr_obj_naming/VERSION,sha256=klIfw8vZZL3J9YSpkbif3apXVO0cyW1tQkRTOGacEwU,5
 cr_obj_naming/__init__.py,sha256=1uv3gz09BL1cmYDLPne0PkqXcvqxLP9jy2DjeeyDCrA,187
 cr_obj_naming/__version__.py,sha256=ikxlExFPaHGK8AzUG9pDnI7Sm8GtkjdM12d5iJMRgik,122
-cr_obj_naming/cnd_consul.py,sha256=BGjFqm0UO2TQf-VW_ZhpfyRw0zF6JGswis0XTmTh9Ok,1459
-cr_obj_naming/obj_naming.py,sha256=EFivRyeS8NsRD-QrIrWDAVnkC1BGkgvu0An9vB10m2A,1433
-cnd_cr_obj_naming-0.2.3.dist-info/METADATA,sha256=Fdi0D99PN_ZXnIXGQ1jy_VTgeYqZL0RE7ymGTK_ZHG4,825
-cnd_cr_obj_naming-0.2.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-cnd_cr_obj_naming-0.2.3.dist-info/top_level.txt,sha256=IxheoHqwoyK8b3XMzAfOoe8Owc9qJeKmqwl2BTPOmBU,14
-cnd_cr_obj_naming-0.2.3.dist-info/RECORD,,
+cr_obj_naming/cnd_consul.py,sha256=Y1651yLtYfWz6z-Cfz9hwXyplHkF8bS8fiOY7b_FaZ0,1454
+cr_obj_naming/obj_naming.py,sha256=uKdroR-S5w7qR9-0-4hAlVNkgivapouuoRGe5P1blBw,1452
+cnd_cr_obj_naming-1.0.0.dist-info/METADATA,sha256=4kGfg8pvh1plM_5uwvbyE2Ujbeqvv4tc0k2alF_hCv0,825
+cnd_cr_obj_naming-1.0.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+cnd_cr_obj_naming-1.0.0.dist-info/top_level.txt,sha256=IxheoHqwoyK8b3XMzAfOoe8Owc9qJeKmqwl2BTPOmBU,14
+cnd_cr_obj_naming-1.0.0.dist-info/RECORD,,
```

