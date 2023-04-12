# Comparing `tmp/ddd-interface-0.0.8.tar.gz` & `tmp/ddd-interface-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddd-interface-0.0.8.tar", last modified: Fri Feb 17 10:43:45 2023, max compression
+gzip compressed data, was "ddd-interface-0.0.9.tar", last modified: Sun Feb 19 00:48:30 2023, max compression
```

## Comparing `ddd-interface-0.0.8.tar` & `ddd-interface-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 10:43:45.465674 ddd-interface-0.0.8/
--rw-rw-rw-   0 root         (0) root         (0)     1091 2023-02-17 10:41:54.000000 ddd-interface-0.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      295 2023-02-17 10:43:45.465674 ddd-interface-0.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      316 2023-02-17 10:41:54.000000 ddd-interface-0.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-17 10:43:45.465674 ddd-interface-0.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      625 2023-02-17 10:41:54.000000 ddd-interface-0.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 10:43:45.457674 ddd-interface-0.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 10:43:45.461674 ddd-interface-0.0.8/src/ddd_interface/
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-02-17 10:41:54.000000 ddd-interface-0.0.8/src/ddd_interface/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 10:43:45.461674 ddd-interface-0.0.8/src/ddd_interface/application/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-17 10:41:54.000000 ddd-interface-0.0.8/src/ddd_interface/application/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      575 2023-02-17 10:41:54.000000 ddd-interface-0.0.8/src/ddd_interface/application/assembler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 10:43:45.461674 ddd-interface-0.0.8/src/ddd_interface/domain/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-17 10:41:54.000000 ddd-interface-0.0.8/src/ddd_interface/domain/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-02-17 10:41:54.000000 ddd-interface-0.0.8/src/ddd_interface/domain/entity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 10:43:45.465674 ddd-interface-0.0.8/src/ddd_interface/infrastructure/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-17 10:41:54.000000 ddd-interface-0.0.8/src/ddd_interface/infrastructure/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-02-17 10:41:54.000000 ddd-interface-0.0.8/src/ddd_interface/infrastructure/converter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 10:43:45.465674 ddd-interface-0.0.8/src/ddd_interface/objects/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-17 10:41:54.000000 ddd-interface-0.0.8/src/ddd_interface/objects/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8045 2023-02-17 10:41:54.000000 ddd-interface-0.0.8/src/ddd_interface/objects/assembler.py
--rw-rw-rw-   0 root         (0) root         (0)     7950 2023-02-17 10:41:54.000000 ddd-interface-0.0.8/src/ddd_interface/objects/converter.py
--rw-rw-rw-   0 root         (0) root         (0)     1464 2023-02-17 10:41:54.000000 ddd-interface-0.0.8/src/ddd_interface/objects/do.py
--rw-rw-rw-   0 root         (0) root         (0)     1478 2023-02-17 10:41:54.000000 ddd-interface-0.0.8/src/ddd_interface/objects/dto.py
--rw-rw-rw-   0 root         (0) root         (0)     5079 2023-02-17 10:41:54.000000 ddd-interface-0.0.8/src/ddd_interface/objects/entity.py
--rw-rw-rw-   0 root         (0) root         (0)     1371 2023-02-17 10:41:54.000000 ddd-interface-0.0.8/src/ddd_interface/objects/value_obj.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-02-17 10:41:54.000000 ddd-interface-0.0.8/src/ddd_interface/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 10:43:45.461674 ddd-interface-0.0.8/src/ddd_interface.egg-info/
--rw-r--r--   0 root         (0) root         (0)      295 2023-02-17 10:43:45.000000 ddd-interface-0.0.8/src/ddd_interface.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      753 2023-02-17 10:43:45.000000 ddd-interface-0.0.8/src/ddd_interface.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-17 10:43:45.000000 ddd-interface-0.0.8/src/ddd_interface.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-02-17 10:43:45.000000 ddd-interface-0.0.8/src/ddd_interface.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-19 00:48:30.164723 ddd-interface-0.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2023-02-19 00:47:29.000000 ddd-interface-0.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      295 2023-02-19 00:48:30.164723 ddd-interface-0.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      316 2023-02-19 00:47:29.000000 ddd-interface-0.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-02-19 00:48:30.164723 ddd-interface-0.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      625 2023-02-19 00:47:29.000000 ddd-interface-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-19 00:48:30.156723 ddd-interface-0.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-19 00:48:30.160723 ddd-interface-0.0.9/src/ddd_interface/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-02-19 00:47:29.000000 ddd-interface-0.0.9/src/ddd_interface/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-19 00:48:30.160723 ddd-interface-0.0.9/src/ddd_interface/application/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-19 00:47:29.000000 ddd-interface-0.0.9/src/ddd_interface/application/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      575 2023-02-19 00:47:29.000000 ddd-interface-0.0.9/src/ddd_interface/application/assembler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-19 00:48:30.160723 ddd-interface-0.0.9/src/ddd_interface/domain/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-19 00:47:29.000000 ddd-interface-0.0.9/src/ddd_interface/domain/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-02-19 00:47:29.000000 ddd-interface-0.0.9/src/ddd_interface/domain/entity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-19 00:48:30.160723 ddd-interface-0.0.9/src/ddd_interface/infrastructure/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-19 00:47:29.000000 ddd-interface-0.0.9/src/ddd_interface/infrastructure/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-02-19 00:47:29.000000 ddd-interface-0.0.9/src/ddd_interface/infrastructure/converter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-19 00:48:30.164723 ddd-interface-0.0.9/src/ddd_interface/objects/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-19 00:47:29.000000 ddd-interface-0.0.9/src/ddd_interface/objects/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8045 2023-02-19 00:47:29.000000 ddd-interface-0.0.9/src/ddd_interface/objects/assembler.py
+-rw-rw-rw-   0 root         (0) root         (0)     7950 2023-02-19 00:47:29.000000 ddd-interface-0.0.9/src/ddd_interface/objects/converter.py
+-rw-rw-rw-   0 root         (0) root         (0)     1464 2023-02-19 00:47:29.000000 ddd-interface-0.0.9/src/ddd_interface/objects/do.py
+-rw-rw-rw-   0 root         (0) root         (0)     1478 2023-02-19 00:47:29.000000 ddd-interface-0.0.9/src/ddd_interface/objects/dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     5079 2023-02-19 00:47:29.000000 ddd-interface-0.0.9/src/ddd_interface/objects/entity.py
+-rw-rw-rw-   0 root         (0) root         (0)     1371 2023-02-19 00:47:29.000000 ddd-interface-0.0.9/src/ddd_interface/objects/value_obj.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-02-19 00:47:29.000000 ddd-interface-0.0.9/src/ddd_interface/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-19 00:48:30.160723 ddd-interface-0.0.9/src/ddd_interface.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      295 2023-02-19 00:48:30.000000 ddd-interface-0.0.9/src/ddd_interface.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      753 2023-02-19 00:48:30.000000 ddd-interface-0.0.9/src/ddd_interface.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-19 00:48:30.000000 ddd-interface-0.0.9/src/ddd_interface.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-02-19 00:48:30.000000 ddd-interface-0.0.9/src/ddd_interface.egg-info/top_level.txt
```

### Comparing `ddd-interface-0.0.8/LICENSE` & `ddd-interface-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ddd-interface-0.0.8/setup.py` & `ddd-interface-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `ddd-interface-0.0.8/src/ddd_interface/application/assembler.py` & `ddd-interface-0.0.9/src/ddd_interface/application/assembler.py`

 * *Files identical despite different names*

### Comparing `ddd-interface-0.0.8/src/ddd_interface/infrastructure/converter.py` & `ddd-interface-0.0.9/src/ddd_interface/infrastructure/converter.py`

 * *Files identical despite different names*

### Comparing `ddd-interface-0.0.8/src/ddd_interface/objects/assembler.py` & `ddd-interface-0.0.9/src/ddd_interface/objects/assembler.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -168,31 +168,31 @@
 
 
 
 class APIGatewayRequestAssembler(Assembler):
     def to_entity(self, dto: APIGatewayRequestDTO):
         return APIGatewayRequest(
             service_name = UStr(dto.service_name),
+            method = UStr(dto.method),
             ip = None if dto.ip is None else UStr(dto.ip),
             port = None if dto.port is None else UInt(dto.port),
             route = None if dto.route is None else UStr(dto.route),
             action = None if dto.action is None else UStr(dto.action),
             auth = None if dto.auth is None else UDict(dto.auth),
-            method = UStr(dto.method),
             data = None if dto.data is None else UDict(dto.data)
         )
     def to_dto(self, x:APIGatewayRequest):
         return APIGatewayRequestDTO(
             service_name = x.service_name.get_value(),
+            method = x.method.get_value(),
             ip = None if x.ip is None else x.ip.get_value(),
             port = None if x.port is None else x.port.get_value(),
             route = None if x.route is None else x.route.get_value(),
             action = None if x.action is None else x.action.get_value(),
             auth = None if x.auth is None else x.auth.get_value(),
-            method = x.method.get_value(),
             data = None if x.data is None else x.data.get_value()
         )
 api_gateway_request_assembler=APIGatewayRequestAssembler()
 
 
 
 class APIGatewayBlacklistItemAssembler(Assembler):
```

### Comparing `ddd-interface-0.0.8/src/ddd_interface/objects/converter.py` & `ddd-interface-0.0.9/src/ddd_interface/objects/converter.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -168,31 +168,31 @@
 
 
 
 class APIGatewayRequestConverter(Converter):
     def to_entity(self, do: APIGatewayRequestDO):
         return APIGatewayRequest(
             service_name = UStr(do.service_name),
+            method = UStr(do.method),
             ip = None if do.ip is None else UStr(do.ip),
             port = None if do.port is None else UInt(do.port),
             route = None if do.route is None else UStr(do.route),
             action = None if do.action is None else UStr(do.action),
             auth = None if do.auth is None else UDict(do.auth),
-            method = UStr(do.method),
             data = None if do.data is None else UDict(do.data)
         )
     def to_do(self, x:APIGatewayRequest):
         return APIGatewayRequestDO(
             service_name = x.service_name.get_value(),
+            method = x.method.get_value(),
             ip = None if x.ip is None else x.ip.get_value(),
             port = None if x.port is None else x.port.get_value(),
             route = None if x.route is None else x.route.get_value(),
             action = None if x.action is None else x.action.get_value(),
             auth = None if x.auth is None else x.auth.get_value(),
-            method = x.method.get_value(),
             data = None if x.data is None else x.data.get_value()
         )
 api_gateway_request_converter=APIGatewayRequestConverter()
 
 
 
 class APIGatewayBlacklistItemConverter(Converter):
```

### Comparing `ddd-interface-0.0.8/src/ddd_interface/objects/do.py` & `ddd-interface-0.0.9/src/ddd_interface/objects/do.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -57,20 +57,20 @@
     variables: List[str]
     paths: List[str]
 
 
 
 class APIGatewayRequestDO(BaseModel):
     service_name: str
+    method: str
     ip: Optional[str] = None
     port: Optional[int] = None
     route: Optional[str] = None
     action: Optional[str] = None
     auth: Optional[Dict] = None
-    method: str
     data: Optional[Dict] = None
 
 
 
 class APIGatewayBlacklistItemDO(BaseModel):
     ip: str
     creation_time: str
```

### Comparing `ddd-interface-0.0.8/src/ddd_interface/objects/dto.py` & `ddd-interface-0.0.9/src/ddd_interface/objects/dto.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -57,20 +57,20 @@
     variables: List[str]
     paths: List[str]
 
 
 
 class APIGatewayRequestDTO(BaseModel):
     service_name: str
+    method: str
     ip: Optional[str] = None
     port: Optional[int] = None
     route: Optional[str] = None
     action: Optional[str] = None
     auth: Optional[Dict] = None
-    method: str
     data: Optional[Dict] = None
 
 
 
 class APIGatewayBlacklistItemDTO(BaseModel):
     ip: str
     creation_time: str
```

### Comparing `ddd-interface-0.0.8/src/ddd_interface/objects/entity.py` & `ddd-interface-0.0.9/src/ddd_interface/objects/entity.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -161,35 +161,35 @@
 
 
 
 class APIGatewayRequest(Entity):
     def __init__(
         self,
         service_name: UStr,
+        method: UStr,
         ip: Optional[UStr] = None,
         port: Optional[UInt] = None,
         route: Optional[UStr] = None,
         action: Optional[UStr] = None,
         auth: Optional[UDict] = None,
-        method: UStr,
         data: Optional[UDict] = None,
         **kwargs
     ) -> None:
         all_args=locals()
         del all_args['self']
         del all_args['__class__']
         del all_args['kwargs']
         super().__init__(**all_args)
         self.service_name = service_name
+        self.method = method
         self.ip = ip
         self.port = port
         self.route = route
         self.action = action
         self.auth = auth
-        self.method = method
         self.data = data
 
 
 
 class APIGatewayBlacklistItem(Entity):
     def __init__(
         self,
```

### Comparing `ddd-interface-0.0.8/src/ddd_interface/objects/value_obj.py` & `ddd-interface-0.0.9/src/ddd_interface/objects/value_obj.py`

 * *Files identical despite different names*

### Comparing `ddd-interface-0.0.8/src/ddd_interface.egg-info/SOURCES.txt` & `ddd-interface-0.0.9/src/ddd_interface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

