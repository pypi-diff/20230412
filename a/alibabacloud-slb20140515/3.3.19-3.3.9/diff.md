# Comparing `tmp/alibabacloud_slb20140515-3.3.19.tar.gz` & `tmp/alibabacloud_slb20140515-3.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_slb20140515-3.3.19.tar", last modified: Wed Apr 12 02:34:41 2023, max compression
+gzip compressed data, was "dist/alibabacloud_slb20140515-3.3.9.tar", last modified: Wed Dec 29 10:09:58 2021, max compression
```

## Comparing `alibabacloud_slb20140515-3.3.19.tar` & `alibabacloud_slb20140515-3.3.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 02:34:41.000000 alibabacloud_slb20140515-3.3.19/
--rw-r--r--   0 root         (0) root         (0)      810 2023-04-12 02:34:41.000000 alibabacloud_slb20140515-3.3.19/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-12 02:34:41.000000 alibabacloud_slb20140515-3.3.19/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-12 02:34:41.000000 alibabacloud_slb20140515-3.3.19/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2346 2023-04-12 02:34:41.000000 alibabacloud_slb20140515-3.3.19/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2023-04-12 02:34:41.000000 alibabacloud_slb20140515-3.3.19/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1107 2023-04-12 02:34:41.000000 alibabacloud_slb20140515-3.3.19/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 02:34:41.000000 alibabacloud_slb20140515-3.3.19/alibabacloud_slb20140515/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-12 02:34:41.000000 alibabacloud_slb20140515-3.3.19/alibabacloud_slb20140515/__init__.py
--rw-r--r--   0 root         (0) root         (0)   539318 2023-04-12 02:34:41.000000 alibabacloud_slb20140515-3.3.19/alibabacloud_slb20140515/client.py
--rw-r--r--   0 root         (0) root         (0)  1012707 2023-04-12 02:34:41.000000 alibabacloud_slb20140515-3.3.19/alibabacloud_slb20140515/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 02:34:41.000000 alibabacloud_slb20140515-3.3.19/alibabacloud_slb20140515.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2346 2023-04-12 02:34:41.000000 alibabacloud_slb20140515-3.3.19/alibabacloud_slb20140515.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2023-04-12 02:34:41.000000 alibabacloud_slb20140515-3.3.19/alibabacloud_slb20140515.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 02:34:41.000000 alibabacloud_slb20140515-3.3.19/alibabacloud_slb20140515.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-04-12 02:34:41.000000 alibabacloud_slb20140515-3.3.19/alibabacloud_slb20140515.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-04-12 02:34:41.000000 alibabacloud_slb20140515-3.3.19/alibabacloud_slb20140515.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-12 02:34:41.000000 alibabacloud_slb20140515-3.3.19/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2627 2023-04-12 02:34:41.000000 alibabacloud_slb20140515-3.3.19/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/
+-rw-r--r--   0 root         (0) root         (0)      305 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2345 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1107 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/alibabacloud_slb20140515/
+-rw-r--r--   0 root         (0) root         (0)       21 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/alibabacloud_slb20140515/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   431433 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/alibabacloud_slb20140515/client.py
+-rw-r--r--   0 root         (0) root         (0)   695669 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/alibabacloud_slb20140515/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/alibabacloud_slb20140515.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2345 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/alibabacloud_slb20140515.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/alibabacloud_slb20140515.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/alibabacloud_slb20140515.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/alibabacloud_slb20140515.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/alibabacloud_slb20140515.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2627 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/setup.py
```

### Comparing `alibabacloud_slb20140515-3.3.19/LICENSE` & `alibabacloud_slb20140515-3.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_slb20140515-3.3.19/PKG-INFO` & `alibabacloud_slb20140515-3.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_slb20140515
-Version: 3.3.19
+Version: 3.3.9
 Summary: Alibaba Cloud Server Load Balancer (20140515) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_slb20140515-3.3.19/README-CN.md` & `alibabacloud_slb20140515-3.3.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_slb20140515-3.3.19/README.md` & `alibabacloud_slb20140515-3.3.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_slb20140515-3.3.19/alibabacloud_slb20140515/client.py` & `alibabacloud_slb20140515-3.3.9/alibabacloud_slb20140515/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -26,20 +26,21 @@
             'cn-qingdao': 'slb.aliyuncs.com',
             'cn-beijing': 'slb.aliyuncs.com',
             'cn-hangzhou': 'slb.aliyuncs.com',
             'cn-shanghai': 'slb.aliyuncs.com',
             'cn-shenzhen': 'slb.aliyuncs.com',
             'cn-hongkong': 'slb.aliyuncs.com',
             'ap-southeast-1': 'slb.aliyuncs.com',
-            'us-east-1': 'slb.aliyuncs.com',
             'us-west-1': 'slb.aliyuncs.com',
+            'us-east-1': 'slb.aliyuncs.com',
             'cn-shanghai-finance-1': 'slb.aliyuncs.com',
             'cn-shenzhen-finance-1': 'slb.aliyuncs.com',
             'cn-north-2-gov-1': 'slb.aliyuncs.com',
             'ap-northeast-2-pop': 'slb.aliyuncs.com',
+            'cn-beijing-finance-1': 'slb.aliyuncs.com',
             'cn-beijing-finance-pop': 'slb.aliyuncs.com',
             'cn-beijing-gov-1': 'slb.aliyuncs.com',
             'cn-beijing-nu16-b01': 'slb.aliyuncs.com',
             'cn-edge-1': 'slb.aliyuncs.com',
             'cn-fujian': 'slb.aliyuncs.com',
             'cn-haidian-cm12-c01': 'slb.aliyuncs.com',
             'cn-hangzhou-bj-b01': 'slb.aliyuncs.com',
@@ -56,15 +57,14 @@
             'cn-shanghai-inner': 'slb.aliyuncs.com',
             'cn-shanghai-internal-test-1': 'slb.aliyuncs.com',
             'cn-shenzhen-inner': 'slb.aliyuncs.com',
             'cn-shenzhen-st4-d01': 'slb.aliyuncs.com',
             'cn-shenzhen-su18-b01': 'slb.aliyuncs.com',
             'cn-wuhan': 'slb.aliyuncs.com',
             'cn-yushanfang': 'slb.aliyuncs.com',
-            'cn-zhangbei': 'slb.aliyuncs.com',
             'cn-zhangbei-na61-b01': 'slb.aliyuncs.com',
             'cn-zhangjiakou-na62-a01': 'slb.aliyuncs.com',
             'cn-zhengzhou-nebula-1': 'slb.aliyuncs.com',
             'eu-west-1-oxs': 'slb.aliyuncs.com',
             'rus-west-1-pop': 'slb.aliyuncs.com'
         }
         self.check_config(config)
@@ -87,23 +87,14 @@
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
     def add_access_control_list_entry_with_options(
         self,
         request: slb_20140515_models.AddAccessControlListEntryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.AddAccessControlListEntryResponse:
-        """
-        Each network ACL can contain one or more IP addresses or CIDR blocks. Take note of the following limits on network ACLs:
-        *   The number of IP entries that can be added to a network ACL with each Alibaba Cloud account at a time: 50
-        *   The maximum number of IP entries that each network ACL can contain: 300
-        
-        @param request: AddAccessControlListEntryRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: AddAccessControlListEntryResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_entrys):
             query['AclEntrys'] = request.acl_entrys
         if not UtilClient.is_unset(request.acl_id):
             query['AclId'] = request.acl_id
         if not UtilClient.is_unset(request.owner_account):
@@ -136,23 +127,14 @@
         )
 
     async def add_access_control_list_entry_with_options_async(
         self,
         request: slb_20140515_models.AddAccessControlListEntryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.AddAccessControlListEntryResponse:
-        """
-        Each network ACL can contain one or more IP addresses or CIDR blocks. Take note of the following limits on network ACLs:
-        *   The number of IP entries that can be added to a network ACL with each Alibaba Cloud account at a time: 50
-        *   The maximum number of IP entries that each network ACL can contain: 300
-        
-        @param request: AddAccessControlListEntryRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: AddAccessControlListEntryResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_entrys):
             query['AclEntrys'] = request.acl_entrys
         if not UtilClient.is_unset(request.acl_id):
             query['AclId'] = request.acl_id
         if not UtilClient.is_unset(request.owner_account):
@@ -184,52 +166,29 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def add_access_control_list_entry(
         self,
         request: slb_20140515_models.AddAccessControlListEntryRequest,
     ) -> slb_20140515_models.AddAccessControlListEntryResponse:
-        """
-        Each network ACL can contain one or more IP addresses or CIDR blocks. Take note of the following limits on network ACLs:
-        *   The number of IP entries that can be added to a network ACL with each Alibaba Cloud account at a time: 50
-        *   The maximum number of IP entries that each network ACL can contain: 300
-        
-        @param request: AddAccessControlListEntryRequest
-        @return: AddAccessControlListEntryResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.add_access_control_list_entry_with_options(request, runtime)
 
     async def add_access_control_list_entry_async(
         self,
         request: slb_20140515_models.AddAccessControlListEntryRequest,
     ) -> slb_20140515_models.AddAccessControlListEntryResponse:
-        """
-        Each network ACL can contain one or more IP addresses or CIDR blocks. Take note of the following limits on network ACLs:
-        *   The number of IP entries that can be added to a network ACL with each Alibaba Cloud account at a time: 50
-        *   The maximum number of IP entries that each network ACL can contain: 300
-        
-        @param request: AddAccessControlListEntryRequest
-        @return: AddAccessControlListEntryResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.add_access_control_list_entry_with_options_async(request, runtime)
 
     def add_backend_servers_with_options(
         self,
         request: slb_20140515_models.AddBackendServersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.AddBackendServersResponse:
-        """
-        >  If multiple identical Elastic Compute Service (ECS) instances are specified in a request, only the first ECS instance is added. The other ECS instances are ignored. If the backend server that you add is the same as one of the existing backend servers that are already associated with the listener, an error message is returned.
-        
-        @param request: AddBackendServersRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: AddBackendServersResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.backend_servers):
             query['BackendServers'] = request.backend_servers
         if not UtilClient.is_unset(request.load_balancer_id):
             query['LoadBalancerId'] = request.load_balancer_id
         if not UtilClient.is_unset(request.owner_account):
@@ -262,21 +221,14 @@
         )
 
     async def add_backend_servers_with_options_async(
         self,
         request: slb_20140515_models.AddBackendServersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.AddBackendServersResponse:
-        """
-        >  If multiple identical Elastic Compute Service (ECS) instances are specified in a request, only the first ECS instance is added. The other ECS instances are ignored. If the backend server that you add is the same as one of the existing backend servers that are already associated with the listener, an error message is returned.
-        
-        @param request: AddBackendServersRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: AddBackendServersResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.backend_servers):
             query['BackendServers'] = request.backend_servers
         if not UtilClient.is_unset(request.load_balancer_id):
             query['LoadBalancerId'] = request.load_balancer_id
         if not UtilClient.is_unset(request.owner_account):
@@ -308,33 +260,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def add_backend_servers(
         self,
         request: slb_20140515_models.AddBackendServersRequest,
     ) -> slb_20140515_models.AddBackendServersResponse:
-        """
-        >  If multiple identical Elastic Compute Service (ECS) instances are specified in a request, only the first ECS instance is added. The other ECS instances are ignored. If the backend server that you add is the same as one of the existing backend servers that are already associated with the listener, an error message is returned.
-        
-        @param request: AddBackendServersRequest
-        @return: AddBackendServersResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.add_backend_servers_with_options(request, runtime)
 
     async def add_backend_servers_async(
         self,
         request: slb_20140515_models.AddBackendServersRequest,
     ) -> slb_20140515_models.AddBackendServersResponse:
-        """
-        >  If multiple identical Elastic Compute Service (ECS) instances are specified in a request, only the first ECS instance is added. The other ECS instances are ignored. If the backend server that you add is the same as one of the existing backend servers that are already associated with the listener, an error message is returned.
-        
-        @param request: AddBackendServersRequest
-        @return: AddBackendServersResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.add_backend_servers_with_options_async(request, runtime)
 
     def add_listener_white_list_item_with_options(
         self,
         request: slb_20140515_models.AddListenerWhiteListItemRequest,
         runtime: util_models.RuntimeOptions,
@@ -437,26 +377,14 @@
         return await self.add_listener_white_list_item_with_options_async(request, runtime)
 
     def add_tags_with_options(
         self,
         request: slb_20140515_models.AddTagsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.AddTagsResponse:
-        """
-        # Limits
-        Before you call this API, note the following limits:
-        *   You can add up to 10 tags to each SLB instance.
-        *   You can add up to five pairs of tags at a time.
-        *   All the tags and keys added to an SLB instance must be unique.
-        *   If you add a tag of which the key is the same as that of an existing tag, but the value is different, the new tag overwrites the existing one.
-        
-        @param request: AddTagsRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: AddTagsResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.load_balancer_id):
             query['LoadBalancerId'] = request.load_balancer_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -489,26 +417,14 @@
         )
 
     async def add_tags_with_options_async(
         self,
         request: slb_20140515_models.AddTagsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.AddTagsResponse:
-        """
-        # Limits
-        Before you call this API, note the following limits:
-        *   You can add up to 10 tags to each SLB instance.
-        *   You can add up to five pairs of tags at a time.
-        *   All the tags and keys added to an SLB instance must be unique.
-        *   If you add a tag of which the key is the same as that of an existing tag, but the value is different, the new tag overwrites the existing one.
-        
-        @param request: AddTagsRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: AddTagsResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.load_balancer_id):
             query['LoadBalancerId'] = request.load_balancer_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -540,43 +456,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def add_tags(
         self,
         request: slb_20140515_models.AddTagsRequest,
     ) -> slb_20140515_models.AddTagsResponse:
-        """
-        # Limits
-        Before you call this API, note the following limits:
-        *   You can add up to 10 tags to each SLB instance.
-        *   You can add up to five pairs of tags at a time.
-        *   All the tags and keys added to an SLB instance must be unique.
-        *   If you add a tag of which the key is the same as that of an existing tag, but the value is different, the new tag overwrites the existing one.
-        
-        @param request: AddTagsRequest
-        @return: AddTagsResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.add_tags_with_options(request, runtime)
 
     async def add_tags_async(
         self,
         request: slb_20140515_models.AddTagsRequest,
     ) -> slb_20140515_models.AddTagsResponse:
-        """
-        # Limits
-        Before you call this API, note the following limits:
-        *   You can add up to 10 tags to each SLB instance.
-        *   You can add up to five pairs of tags at a time.
-        *   All the tags and keys added to an SLB instance must be unique.
-        *   If you add a tag of which the key is the same as that of an existing tag, but the value is different, the new tag overwrites the existing one.
-        
-        @param request: AddTagsRequest
-        @return: AddTagsResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.add_tags_with_options_async(request, runtime)
 
     def add_vserver_group_backend_servers_with_options(
         self,
         request: slb_20140515_models.AddVServerGroupBackendServersRequest,
         runtime: util_models.RuntimeOptions,
@@ -671,24 +565,14 @@
         return await self.add_vserver_group_backend_servers_with_options_async(request, runtime)
 
     def create_access_control_list_with_options(
         self,
         request: slb_20140515_models.CreateAccessControlListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.CreateAccessControlListResponse:
-        """
-        You can create multiple ACLs. Each ACL can contain one or more IP addresses or CIDR blocks. Before you create an ACL, take note of the following limits:
-        *   An account can have a maximum of 50 ACLs in each region.
-        *   You can add a maximum of 50 IP addresses or CIDR blocks at a time within an account.
-        *   Each ACL can contain a maximum of 300 IP addresses or CIDR blocks.
-        
-        @param request: CreateAccessControlListRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: CreateAccessControlListResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_name):
             query['AclName'] = request.acl_name
         if not UtilClient.is_unset(request.address_ipversion):
             query['AddressIPVersion'] = request.address_ipversion
         if not UtilClient.is_unset(request.owner_account):
@@ -723,24 +607,14 @@
         )
 
     async def create_access_control_list_with_options_async(
         self,
         request: slb_20140515_models.CreateAccessControlListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.CreateAccessControlListResponse:
-        """
-        You can create multiple ACLs. Each ACL can contain one or more IP addresses or CIDR blocks. Before you create an ACL, take note of the following limits:
-        *   An account can have a maximum of 50 ACLs in each region.
-        *   You can add a maximum of 50 IP addresses or CIDR blocks at a time within an account.
-        *   Each ACL can contain a maximum of 300 IP addresses or CIDR blocks.
-        
-        @param request: CreateAccessControlListRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: CreateAccessControlListResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_name):
             query['AclName'] = request.acl_name
         if not UtilClient.is_unset(request.address_ipversion):
             query['AddressIPVersion'] = request.address_ipversion
         if not UtilClient.is_unset(request.owner_account):
@@ -774,39 +648,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_access_control_list(
         self,
         request: slb_20140515_models.CreateAccessControlListRequest,
     ) -> slb_20140515_models.CreateAccessControlListResponse:
-        """
-        You can create multiple ACLs. Each ACL can contain one or more IP addresses or CIDR blocks. Before you create an ACL, take note of the following limits:
-        *   An account can have a maximum of 50 ACLs in each region.
-        *   You can add a maximum of 50 IP addresses or CIDR blocks at a time within an account.
-        *   Each ACL can contain a maximum of 300 IP addresses or CIDR blocks.
-        
-        @param request: CreateAccessControlListRequest
-        @return: CreateAccessControlListResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.create_access_control_list_with_options(request, runtime)
 
     async def create_access_control_list_async(
         self,
         request: slb_20140515_models.CreateAccessControlListRequest,
     ) -> slb_20140515_models.CreateAccessControlListResponse:
-        """
-        You can create multiple ACLs. Each ACL can contain one or more IP addresses or CIDR blocks. Before you create an ACL, take note of the following limits:
-        *   An account can have a maximum of 50 ACLs in each region.
-        *   You can add a maximum of 50 IP addresses or CIDR blocks at a time within an account.
-        *   Each ACL can contain a maximum of 300 IP addresses or CIDR blocks.
-        
-        @param request: CreateAccessControlListRequest
-        @return: CreateAccessControlListResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.create_access_control_list_with_options_async(request, runtime)
 
     def create_domain_extension_with_options(
         self,
         request: slb_20140515_models.CreateDomainExtensionRequest,
         runtime: util_models.RuntimeOptions,
@@ -909,24 +765,14 @@
         return await self.create_domain_extension_with_options_async(request, runtime)
 
     def create_load_balancer_with_options(
         self,
         request: slb_20140515_models.CreateLoadBalancerRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.CreateLoadBalancerResponse:
-        """
-        ##
-        *   Before you create a CLB instance, call the [DescribeAvailableResource](~~117645~~) operation to query the resources that are available for purchase in the region where you want to create the CLB instance.
-        *   After a CLB instance is created, you are charged when you use the CLB instance.
-        *   The pay-as-you-go billing method supports the pay-by-specification and pay-by-LCU metering methods.
-        
-        @param request: CreateLoadBalancerRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: CreateLoadBalancerResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.address):
             query['Address'] = request.address
         if not UtilClient.is_unset(request.address_ipversion):
             query['AddressIPVersion'] = request.address_ipversion
         if not UtilClient.is_unset(request.address_type):
@@ -937,16 +783,14 @@
             query['Bandwidth'] = request.bandwidth
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.delete_protection):
             query['DeleteProtection'] = request.delete_protection
         if not UtilClient.is_unset(request.duration):
             query['Duration'] = request.duration
-        if not UtilClient.is_unset(request.instance_charge_type):
-            query['InstanceChargeType'] = request.instance_charge_type
         if not UtilClient.is_unset(request.internet_charge_type):
             query['InternetChargeType'] = request.internet_charge_type
         if not UtilClient.is_unset(request.load_balancer_name):
             query['LoadBalancerName'] = request.load_balancer_name
         if not UtilClient.is_unset(request.load_balancer_spec):
             query['LoadBalancerSpec'] = request.load_balancer_spec
         if not UtilClient.is_unset(request.master_zone_id):
@@ -997,24 +841,14 @@
         )
 
     async def create_load_balancer_with_options_async(
         self,
         request: slb_20140515_models.CreateLoadBalancerRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.CreateLoadBalancerResponse:
-        """
-        ##
-        *   Before you create a CLB instance, call the [DescribeAvailableResource](~~117645~~) operation to query the resources that are available for purchase in the region where you want to create the CLB instance.
-        *   After a CLB instance is created, you are charged when you use the CLB instance.
-        *   The pay-as-you-go billing method supports the pay-by-specification and pay-by-LCU metering methods.
-        
-        @param request: CreateLoadBalancerRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: CreateLoadBalancerResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.address):
             query['Address'] = request.address
         if not UtilClient.is_unset(request.address_ipversion):
             query['AddressIPVersion'] = request.address_ipversion
         if not UtilClient.is_unset(request.address_type):
@@ -1025,16 +859,14 @@
             query['Bandwidth'] = request.bandwidth
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.delete_protection):
             query['DeleteProtection'] = request.delete_protection
         if not UtilClient.is_unset(request.duration):
             query['Duration'] = request.duration
-        if not UtilClient.is_unset(request.instance_charge_type):
-            query['InstanceChargeType'] = request.instance_charge_type
         if not UtilClient.is_unset(request.internet_charge_type):
             query['InternetChargeType'] = request.internet_charge_type
         if not UtilClient.is_unset(request.load_balancer_name):
             query['LoadBalancerName'] = request.load_balancer_name
         if not UtilClient.is_unset(request.load_balancer_spec):
             query['LoadBalancerSpec'] = request.load_balancer_spec
         if not UtilClient.is_unset(request.master_zone_id):
@@ -1084,57 +916,29 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_load_balancer(
         self,
         request: slb_20140515_models.CreateLoadBalancerRequest,
     ) -> slb_20140515_models.CreateLoadBalancerResponse:
-        """
-        ##
-        *   Before you create a CLB instance, call the [DescribeAvailableResource](~~117645~~) operation to query the resources that are available for purchase in the region where you want to create the CLB instance.
-        *   After a CLB instance is created, you are charged when you use the CLB instance.
-        *   The pay-as-you-go billing method supports the pay-by-specification and pay-by-LCU metering methods.
-        
-        @param request: CreateLoadBalancerRequest
-        @return: CreateLoadBalancerResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.create_load_balancer_with_options(request, runtime)
 
     async def create_load_balancer_async(
         self,
         request: slb_20140515_models.CreateLoadBalancerRequest,
     ) -> slb_20140515_models.CreateLoadBalancerResponse:
-        """
-        ##
-        *   Before you create a CLB instance, call the [DescribeAvailableResource](~~117645~~) operation to query the resources that are available for purchase in the region where you want to create the CLB instance.
-        *   After a CLB instance is created, you are charged when you use the CLB instance.
-        *   The pay-as-you-go billing method supports the pay-by-specification and pay-by-LCU metering methods.
-        
-        @param request: CreateLoadBalancerRequest
-        @return: CreateLoadBalancerResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.create_load_balancer_with_options_async(request, runtime)
 
     def create_load_balancer_httplistener_with_options(
         self,
         request: slb_20140515_models.CreateLoadBalancerHTTPListenerRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.CreateLoadBalancerHTTPListenerResponse:
-        """
-        ## Precautions
-        A newly created listener is in the **stopped** state. After a listener is created, you can call the [StartLoadBalancerListener](~~27597~~) operation to start the listener. After the listener is started, the listener can forward traffic to backend servers.
-        ## Prerequisites
-        A Classic Load Balancer (CLB) instance is created. For more information, see [CreateLoadBalancer](https://www.alibabacloud.com/help/en/server-load-balancer/latest/createloadbalancer-2).
-        
-        @param request: CreateLoadBalancerHTTPListenerRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: CreateLoadBalancerHTTPListenerResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_id):
             query['AclId'] = request.acl_id
         if not UtilClient.is_unset(request.acl_status):
             query['AclStatus'] = request.acl_status
         if not UtilClient.is_unset(request.acl_type):
@@ -1229,24 +1033,14 @@
         )
 
     async def create_load_balancer_httplistener_with_options_async(
         self,
         request: slb_20140515_models.CreateLoadBalancerHTTPListenerRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.CreateLoadBalancerHTTPListenerResponse:
-        """
-        ## Precautions
-        A newly created listener is in the **stopped** state. After a listener is created, you can call the [StartLoadBalancerListener](~~27597~~) operation to start the listener. After the listener is started, the listener can forward traffic to backend servers.
-        ## Prerequisites
-        A Classic Load Balancer (CLB) instance is created. For more information, see [CreateLoadBalancer](https://www.alibabacloud.com/help/en/server-load-balancer/latest/createloadbalancer-2).
-        
-        @param request: CreateLoadBalancerHTTPListenerRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: CreateLoadBalancerHTTPListenerResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_id):
             query['AclId'] = request.acl_id
         if not UtilClient.is_unset(request.acl_status):
             query['AclStatus'] = request.acl_status
         if not UtilClient.is_unset(request.acl_type):
@@ -1340,57 +1134,29 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_load_balancer_httplistener(
         self,
         request: slb_20140515_models.CreateLoadBalancerHTTPListenerRequest,
     ) -> slb_20140515_models.CreateLoadBalancerHTTPListenerResponse:
-        """
-        ## Precautions
-        A newly created listener is in the **stopped** state. After a listener is created, you can call the [StartLoadBalancerListener](~~27597~~) operation to start the listener. After the listener is started, the listener can forward traffic to backend servers.
-        ## Prerequisites
-        A Classic Load Balancer (CLB) instance is created. For more information, see [CreateLoadBalancer](https://www.alibabacloud.com/help/en/server-load-balancer/latest/createloadbalancer-2).
-        
-        @param request: CreateLoadBalancerHTTPListenerRequest
-        @return: CreateLoadBalancerHTTPListenerResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.create_load_balancer_httplistener_with_options(request, runtime)
 
     async def create_load_balancer_httplistener_async(
         self,
         request: slb_20140515_models.CreateLoadBalancerHTTPListenerRequest,
     ) -> slb_20140515_models.CreateLoadBalancerHTTPListenerResponse:
-        """
-        ## Precautions
-        A newly created listener is in the **stopped** state. After a listener is created, you can call the [StartLoadBalancerListener](~~27597~~) operation to start the listener. After the listener is started, the listener can forward traffic to backend servers.
-        ## Prerequisites
-        A Classic Load Balancer (CLB) instance is created. For more information, see [CreateLoadBalancer](https://www.alibabacloud.com/help/en/server-load-balancer/latest/createloadbalancer-2).
-        
-        @param request: CreateLoadBalancerHTTPListenerRequest
-        @return: CreateLoadBalancerHTTPListenerResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.create_load_balancer_httplistener_with_options_async(request, runtime)
 
     def create_load_balancer_httpslistener_with_options(
         self,
         request: slb_20140515_models.CreateLoadBalancerHTTPSListenerRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.CreateLoadBalancerHTTPSListenerResponse:
-        """
-        ## Precautions
-        A newly created listener is in the **stopped** state. After a listener is created, you can call the [StartLoadBalancerListener](~~27597~~) operation to start the listener. After the listener is started, the listener can forward traffic to backend servers.
-        ## Prerequisites
-        A Classic Load Balancer (CLB) instance is created. For more information, see [CreateLoadBalancer](https://www.alibabacloud.com/help/en/server-load-balancer/latest/createloadbalancer-2).
-        
-        @param request: CreateLoadBalancerHTTPSListenerRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: CreateLoadBalancerHTTPSListenerResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_id):
             query['AclId'] = request.acl_id
         if not UtilClient.is_unset(request.acl_status):
             query['AclStatus'] = request.acl_status
         if not UtilClient.is_unset(request.acl_type):
@@ -1489,24 +1255,14 @@
         )
 
     async def create_load_balancer_httpslistener_with_options_async(
         self,
         request: slb_20140515_models.CreateLoadBalancerHTTPSListenerRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.CreateLoadBalancerHTTPSListenerResponse:
-        """
-        ## Precautions
-        A newly created listener is in the **stopped** state. After a listener is created, you can call the [StartLoadBalancerListener](~~27597~~) operation to start the listener. After the listener is started, the listener can forward traffic to backend servers.
-        ## Prerequisites
-        A Classic Load Balancer (CLB) instance is created. For more information, see [CreateLoadBalancer](https://www.alibabacloud.com/help/en/server-load-balancer/latest/createloadbalancer-2).
-        
-        @param request: CreateLoadBalancerHTTPSListenerRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: CreateLoadBalancerHTTPSListenerResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_id):
             query['AclId'] = request.acl_id
         if not UtilClient.is_unset(request.acl_status):
             query['AclStatus'] = request.acl_status
         if not UtilClient.is_unset(request.acl_type):
@@ -1604,54 +1360,29 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_load_balancer_httpslistener(
         self,
         request: slb_20140515_models.CreateLoadBalancerHTTPSListenerRequest,
     ) -> slb_20140515_models.CreateLoadBalancerHTTPSListenerResponse:
-        """
-        ## Precautions
-        A newly created listener is in the **stopped** state. After a listener is created, you can call the [StartLoadBalancerListener](~~27597~~) operation to start the listener. After the listener is started, the listener can forward traffic to backend servers.
-        ## Prerequisites
-        A Classic Load Balancer (CLB) instance is created. For more information, see [CreateLoadBalancer](https://www.alibabacloud.com/help/en/server-load-balancer/latest/createloadbalancer-2).
-        
-        @param request: CreateLoadBalancerHTTPSListenerRequest
-        @return: CreateLoadBalancerHTTPSListenerResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.create_load_balancer_httpslistener_with_options(request, runtime)
 
     async def create_load_balancer_httpslistener_async(
         self,
         request: slb_20140515_models.CreateLoadBalancerHTTPSListenerRequest,
     ) -> slb_20140515_models.CreateLoadBalancerHTTPSListenerResponse:
-        """
-        ## Precautions
-        A newly created listener is in the **stopped** state. After a listener is created, you can call the [StartLoadBalancerListener](~~27597~~) operation to start the listener. After the listener is started, the listener can forward traffic to backend servers.
-        ## Prerequisites
-        A Classic Load Balancer (CLB) instance is created. For more information, see [CreateLoadBalancer](https://www.alibabacloud.com/help/en/server-load-balancer/latest/createloadbalancer-2).
-        
-        @param request: CreateLoadBalancerHTTPSListenerRequest
-        @return: CreateLoadBalancerHTTPSListenerResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.create_load_balancer_httpslistener_with_options_async(request, runtime)
 
     def create_load_balancer_tcplistener_with_options(
         self,
         request: slb_20140515_models.CreateLoadBalancerTCPListenerRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.CreateLoadBalancerTCPListenerResponse:
-        """
-        >  A newly created listener is in the *stopped** state. After a listener is created, you can call the [StartLoadBalancerListener](~~27597~~) operation to enable the listener to forward traffic to backend servers.
-        
-        @param request: CreateLoadBalancerTCPListenerRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: CreateLoadBalancerTCPListenerResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_id):
             query['AclId'] = request.acl_id
         if not UtilClient.is_unset(request.acl_status):
             query['AclStatus'] = request.acl_status
         if not UtilClient.is_unset(request.acl_type):
@@ -1672,16 +1403,14 @@
             query['HealthCheckConnectPort'] = request.health_check_connect_port
         if not UtilClient.is_unset(request.health_check_connect_timeout):
             query['HealthCheckConnectTimeout'] = request.health_check_connect_timeout
         if not UtilClient.is_unset(request.health_check_domain):
             query['HealthCheckDomain'] = request.health_check_domain
         if not UtilClient.is_unset(request.health_check_http_code):
             query['HealthCheckHttpCode'] = request.health_check_http_code
-        if not UtilClient.is_unset(request.health_check_switch):
-            query['HealthCheckSwitch'] = request.health_check_switch
         if not UtilClient.is_unset(request.health_check_type):
             query['HealthCheckType'] = request.health_check_type
         if not UtilClient.is_unset(request.health_check_uri):
             query['HealthCheckURI'] = request.health_check_uri
         if not UtilClient.is_unset(request.healthy_threshold):
             query['HealthyThreshold'] = request.healthy_threshold
         if not UtilClient.is_unset(request.listener_port):
@@ -1692,16 +1421,14 @@
             query['MasterSlaveServerGroupId'] = request.master_slave_server_group_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.persistence_timeout):
             query['PersistenceTimeout'] = request.persistence_timeout
-        if not UtilClient.is_unset(request.proxy_protocol_v2enabled):
-            query['ProxyProtocolV2Enabled'] = request.proxy_protocol_v2enabled
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
             query['ResourceOwnerId'] = request.resource_owner_id
         if not UtilClient.is_unset(request.scheduler):
@@ -1732,21 +1459,14 @@
         )
 
     async def create_load_balancer_tcplistener_with_options_async(
         self,
         request: slb_20140515_models.CreateLoadBalancerTCPListenerRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.CreateLoadBalancerTCPListenerResponse:
-        """
-        >  A newly created listener is in the *stopped** state. After a listener is created, you can call the [StartLoadBalancerListener](~~27597~~) operation to enable the listener to forward traffic to backend servers.
-        
-        @param request: CreateLoadBalancerTCPListenerRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: CreateLoadBalancerTCPListenerResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_id):
             query['AclId'] = request.acl_id
         if not UtilClient.is_unset(request.acl_status):
             query['AclStatus'] = request.acl_status
         if not UtilClient.is_unset(request.acl_type):
@@ -1767,16 +1487,14 @@
             query['HealthCheckConnectPort'] = request.health_check_connect_port
         if not UtilClient.is_unset(request.health_check_connect_timeout):
             query['HealthCheckConnectTimeout'] = request.health_check_connect_timeout
         if not UtilClient.is_unset(request.health_check_domain):
             query['HealthCheckDomain'] = request.health_check_domain
         if not UtilClient.is_unset(request.health_check_http_code):
             query['HealthCheckHttpCode'] = request.health_check_http_code
-        if not UtilClient.is_unset(request.health_check_switch):
-            query['HealthCheckSwitch'] = request.health_check_switch
         if not UtilClient.is_unset(request.health_check_type):
             query['HealthCheckType'] = request.health_check_type
         if not UtilClient.is_unset(request.health_check_uri):
             query['HealthCheckURI'] = request.health_check_uri
         if not UtilClient.is_unset(request.healthy_threshold):
             query['HealthyThreshold'] = request.healthy_threshold
         if not UtilClient.is_unset(request.listener_port):
@@ -1787,16 +1505,14 @@
             query['MasterSlaveServerGroupId'] = request.master_slave_server_group_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.persistence_timeout):
             query['PersistenceTimeout'] = request.persistence_timeout
-        if not UtilClient.is_unset(request.proxy_protocol_v2enabled):
-            query['ProxyProtocolV2Enabled'] = request.proxy_protocol_v2enabled
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
             query['ResourceOwnerId'] = request.resource_owner_id
         if not UtilClient.is_unset(request.scheduler):
@@ -1826,49 +1542,29 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_load_balancer_tcplistener(
         self,
         request: slb_20140515_models.CreateLoadBalancerTCPListenerRequest,
     ) -> slb_20140515_models.CreateLoadBalancerTCPListenerResponse:
-        """
-        >  A newly created listener is in the *stopped** state. After a listener is created, you can call the [StartLoadBalancerListener](~~27597~~) operation to enable the listener to forward traffic to backend servers.
-        
-        @param request: CreateLoadBalancerTCPListenerRequest
-        @return: CreateLoadBalancerTCPListenerResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.create_load_balancer_tcplistener_with_options(request, runtime)
 
     async def create_load_balancer_tcplistener_async(
         self,
         request: slb_20140515_models.CreateLoadBalancerTCPListenerRequest,
     ) -> slb_20140515_models.CreateLoadBalancerTCPListenerResponse:
-        """
-        >  A newly created listener is in the *stopped** state. After a listener is created, you can call the [StartLoadBalancerListener](~~27597~~) operation to enable the listener to forward traffic to backend servers.
-        
-        @param request: CreateLoadBalancerTCPListenerRequest
-        @return: CreateLoadBalancerTCPListenerResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.create_load_balancer_tcplistener_with_options_async(request, runtime)
 
     def create_load_balancer_udplistener_with_options(
         self,
         request: slb_20140515_models.CreateLoadBalancerUDPListenerRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.CreateLoadBalancerUDPListenerResponse:
-        """
-        UDP listeners of Classic Load Balancer (CLB) instances in a classic network cannot pass client IP addresses to backend servers.
-        >  A newly created listener is in the **stopped** state. After a listener is created, you can call the [StartLoadBalancerListener](~~27597~~) operation to enable the listener to forward traffic to backend servers.
-        
-        @param request: CreateLoadBalancerUDPListenerRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: CreateLoadBalancerUDPListenerResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_id):
             query['AclId'] = request.acl_id
         if not UtilClient.is_unset(request.acl_status):
             query['AclStatus'] = request.acl_status
         if not UtilClient.is_unset(request.acl_type):
@@ -1879,30 +1575,26 @@
             query['Bandwidth'] = request.bandwidth
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.health_check_connect_port):
             query['HealthCheckConnectPort'] = request.health_check_connect_port
         if not UtilClient.is_unset(request.health_check_connect_timeout):
             query['HealthCheckConnectTimeout'] = request.health_check_connect_timeout
-        if not UtilClient.is_unset(request.health_check_switch):
-            query['HealthCheckSwitch'] = request.health_check_switch
         if not UtilClient.is_unset(request.healthy_threshold):
             query['HealthyThreshold'] = request.healthy_threshold
         if not UtilClient.is_unset(request.listener_port):
             query['ListenerPort'] = request.listener_port
         if not UtilClient.is_unset(request.load_balancer_id):
             query['LoadBalancerId'] = request.load_balancer_id
         if not UtilClient.is_unset(request.master_slave_server_group_id):
             query['MasterSlaveServerGroupId'] = request.master_slave_server_group_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
-        if not UtilClient.is_unset(request.proxy_protocol_v2enabled):
-            query['ProxyProtocolV2Enabled'] = request.proxy_protocol_v2enabled
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
             query['ResourceOwnerId'] = request.resource_owner_id
         if not UtilClient.is_unset(request.scheduler):
@@ -1937,22 +1629,14 @@
         )
 
     async def create_load_balancer_udplistener_with_options_async(
         self,
         request: slb_20140515_models.CreateLoadBalancerUDPListenerRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.CreateLoadBalancerUDPListenerResponse:
-        """
-        UDP listeners of Classic Load Balancer (CLB) instances in a classic network cannot pass client IP addresses to backend servers.
-        >  A newly created listener is in the **stopped** state. After a listener is created, you can call the [StartLoadBalancerListener](~~27597~~) operation to enable the listener to forward traffic to backend servers.
-        
-        @param request: CreateLoadBalancerUDPListenerRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: CreateLoadBalancerUDPListenerResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_id):
             query['AclId'] = request.acl_id
         if not UtilClient.is_unset(request.acl_status):
             query['AclStatus'] = request.acl_status
         if not UtilClient.is_unset(request.acl_type):
@@ -1963,30 +1647,26 @@
             query['Bandwidth'] = request.bandwidth
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.health_check_connect_port):
             query['HealthCheckConnectPort'] = request.health_check_connect_port
         if not UtilClient.is_unset(request.health_check_connect_timeout):
             query['HealthCheckConnectTimeout'] = request.health_check_connect_timeout
-        if not UtilClient.is_unset(request.health_check_switch):
-            query['HealthCheckSwitch'] = request.health_check_switch
         if not UtilClient.is_unset(request.healthy_threshold):
             query['HealthyThreshold'] = request.healthy_threshold
         if not UtilClient.is_unset(request.listener_port):
             query['ListenerPort'] = request.listener_port
         if not UtilClient.is_unset(request.load_balancer_id):
             query['LoadBalancerId'] = request.load_balancer_id
         if not UtilClient.is_unset(request.master_slave_server_group_id):
             query['MasterSlaveServerGroupId'] = request.master_slave_server_group_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
-        if not UtilClient.is_unset(request.proxy_protocol_v2enabled):
-            query['ProxyProtocolV2Enabled'] = request.proxy_protocol_v2enabled
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
             query['ResourceOwnerId'] = request.resource_owner_id
         if not UtilClient.is_unset(request.scheduler):
@@ -2020,35 +1700,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_load_balancer_udplistener(
         self,
         request: slb_20140515_models.CreateLoadBalancerUDPListenerRequest,
     ) -> slb_20140515_models.CreateLoadBalancerUDPListenerResponse:
-        """
-        UDP listeners of Classic Load Balancer (CLB) instances in a classic network cannot pass client IP addresses to backend servers.
-        >  A newly created listener is in the **stopped** state. After a listener is created, you can call the [StartLoadBalancerListener](~~27597~~) operation to enable the listener to forward traffic to backend servers.
-        
-        @param request: CreateLoadBalancerUDPListenerRequest
-        @return: CreateLoadBalancerUDPListenerResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.create_load_balancer_udplistener_with_options(request, runtime)
 
     async def create_load_balancer_udplistener_async(
         self,
         request: slb_20140515_models.CreateLoadBalancerUDPListenerRequest,
     ) -> slb_20140515_models.CreateLoadBalancerUDPListenerResponse:
-        """
-        UDP listeners of Classic Load Balancer (CLB) instances in a classic network cannot pass client IP addresses to backend servers.
-        >  A newly created listener is in the **stopped** state. After a listener is created, you can call the [StartLoadBalancerListener](~~27597~~) operation to enable the listener to forward traffic to backend servers.
-        
-        @param request: CreateLoadBalancerUDPListenerRequest
-        @return: CreateLoadBalancerUDPListenerResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.create_load_balancer_udplistener_with_options_async(request, runtime)
 
     def create_master_slave_server_group_with_options(
         self,
         request: slb_20140515_models.CreateMasterSlaveServerGroupRequest,
         runtime: util_models.RuntimeOptions,
@@ -2267,14 +1933,16 @@
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
             query['ResourceOwnerId'] = request.resource_owner_id
         if not UtilClient.is_unset(request.tlsversions):
             query['TLSVersions'] = request.tlsversions
+        if not UtilClient.is_unset(request.access_key_id):
+            query['access_key_id'] = request.access_key_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreateTLSCipherPolicy',
             version='2014-05-15',
             protocol='HTTPS',
@@ -2309,14 +1977,16 @@
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
             query['ResourceOwnerId'] = request.resource_owner_id
         if not UtilClient.is_unset(request.tlsversions):
             query['TLSVersions'] = request.tlsversions
+        if not UtilClient.is_unset(request.access_key_id):
+            query['access_key_id'] = request.access_key_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreateTLSCipherPolicy',
             version='2014-05-15',
             protocol='HTTPS',
@@ -2445,21 +2115,14 @@
         return await self.create_vserver_group_with_options_async(request, runtime)
 
     def delete_access_control_list_with_options(
         self,
         request: slb_20140515_models.DeleteAccessControlListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.DeleteAccessControlListResponse:
-        """
-        >  An access control list can be deleted only after it is disassociated from a listener.
-        
-        @param request: DeleteAccessControlListRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DeleteAccessControlListResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_id):
             query['AclId'] = request.acl_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -2490,21 +2153,14 @@
         )
 
     async def delete_access_control_list_with_options_async(
         self,
         request: slb_20140515_models.DeleteAccessControlListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.DeleteAccessControlListResponse:
-        """
-        >  An access control list can be deleted only after it is disassociated from a listener.
-        
-        @param request: DeleteAccessControlListRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DeleteAccessControlListResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_id):
             query['AclId'] = request.acl_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -2534,146 +2190,29 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_access_control_list(
         self,
         request: slb_20140515_models.DeleteAccessControlListRequest,
     ) -> slb_20140515_models.DeleteAccessControlListResponse:
-        """
-        >  An access control list can be deleted only after it is disassociated from a listener.
-        
-        @param request: DeleteAccessControlListRequest
-        @return: DeleteAccessControlListResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.delete_access_control_list_with_options(request, runtime)
 
     async def delete_access_control_list_async(
         self,
         request: slb_20140515_models.DeleteAccessControlListRequest,
     ) -> slb_20140515_models.DeleteAccessControlListResponse:
-        """
-        >  An access control list can be deleted only after it is disassociated from a listener.
-        
-        @param request: DeleteAccessControlListRequest
-        @return: DeleteAccessControlListResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_access_control_list_with_options_async(request, runtime)
 
-    def delete_access_logs_download_attribute_with_options(
-        self,
-        request: slb_20140515_models.DeleteAccessLogsDownloadAttributeRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> slb_20140515_models.DeleteAccessLogsDownloadAttributeResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.load_balancer_id):
-            query['LoadBalancerId'] = request.load_balancer_id
-        if not UtilClient.is_unset(request.logs_download_attributes):
-            query['LogsDownloadAttributes'] = request.logs_download_attributes
-        if not UtilClient.is_unset(request.owner_account):
-            query['OwnerAccount'] = request.owner_account
-        if not UtilClient.is_unset(request.owner_id):
-            query['OwnerId'] = request.owner_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.resource_owner_account):
-            query['ResourceOwnerAccount'] = request.resource_owner_account
-        if not UtilClient.is_unset(request.resource_owner_id):
-            query['ResourceOwnerId'] = request.resource_owner_id
-        if not UtilClient.is_unset(request.tags):
-            query['Tags'] = request.tags
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DeleteAccessLogsDownloadAttribute',
-            version='2014-05-15',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            slb_20140515_models.DeleteAccessLogsDownloadAttributeResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def delete_access_logs_download_attribute_with_options_async(
-        self,
-        request: slb_20140515_models.DeleteAccessLogsDownloadAttributeRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> slb_20140515_models.DeleteAccessLogsDownloadAttributeResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.load_balancer_id):
-            query['LoadBalancerId'] = request.load_balancer_id
-        if not UtilClient.is_unset(request.logs_download_attributes):
-            query['LogsDownloadAttributes'] = request.logs_download_attributes
-        if not UtilClient.is_unset(request.owner_account):
-            query['OwnerAccount'] = request.owner_account
-        if not UtilClient.is_unset(request.owner_id):
-            query['OwnerId'] = request.owner_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.resource_owner_account):
-            query['ResourceOwnerAccount'] = request.resource_owner_account
-        if not UtilClient.is_unset(request.resource_owner_id):
-            query['ResourceOwnerId'] = request.resource_owner_id
-        if not UtilClient.is_unset(request.tags):
-            query['Tags'] = request.tags
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DeleteAccessLogsDownloadAttribute',
-            version='2014-05-15',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            slb_20140515_models.DeleteAccessLogsDownloadAttributeResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def delete_access_logs_download_attribute(
-        self,
-        request: slb_20140515_models.DeleteAccessLogsDownloadAttributeRequest,
-    ) -> slb_20140515_models.DeleteAccessLogsDownloadAttributeResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.delete_access_logs_download_attribute_with_options(request, runtime)
-
-    async def delete_access_logs_download_attribute_async(
-        self,
-        request: slb_20140515_models.DeleteAccessLogsDownloadAttributeRequest,
-    ) -> slb_20140515_models.DeleteAccessLogsDownloadAttributeResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.delete_access_logs_download_attribute_with_options_async(request, runtime)
-
     def delete_cacertificate_with_options(
         self,
         request: slb_20140515_models.DeleteCACertificateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.DeleteCACertificateResponse:
-        """
-        >  CA certificates in use cannot be deleted.
-        
-        @param request: DeleteCACertificateRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DeleteCACertificateResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.cacertificate_id):
             query['CACertificateId'] = request.cacertificate_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -2704,21 +2243,14 @@
         )
 
     async def delete_cacertificate_with_options_async(
         self,
         request: slb_20140515_models.DeleteCACertificateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.DeleteCACertificateResponse:
-        """
-        >  CA certificates in use cannot be deleted.
-        
-        @param request: DeleteCACertificateRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DeleteCACertificateResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.cacertificate_id):
             query['CACertificateId'] = request.cacertificate_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -2748,33 +2280,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_cacertificate(
         self,
         request: slb_20140515_models.DeleteCACertificateRequest,
     ) -> slb_20140515_models.DeleteCACertificateResponse:
-        """
-        >  CA certificates in use cannot be deleted.
-        
-        @param request: DeleteCACertificateRequest
-        @return: DeleteCACertificateResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.delete_cacertificate_with_options(request, runtime)
 
     async def delete_cacertificate_async(
         self,
         request: slb_20140515_models.DeleteCACertificateRequest,
     ) -> slb_20140515_models.DeleteCACertificateResponse:
-        """
-        >  CA certificates in use cannot be deleted.
-        
-        @param request: DeleteCACertificateRequest
-        @return: DeleteCACertificateResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_cacertificate_with_options_async(request, runtime)
 
     def delete_domain_extension_with_options(
         self,
         request: slb_20140515_models.DeleteDomainExtensionRequest,
         runtime: util_models.RuntimeOptions,
@@ -2865,21 +2385,14 @@
         return await self.delete_domain_extension_with_options_async(request, runtime)
 
     def delete_load_balancer_with_options(
         self,
         request: slb_20140515_models.DeleteLoadBalancerRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.DeleteLoadBalancerResponse:
-        """
-        >  After you delete an SLB instance, the listeners and tags added to the SLB instance are deleted.
-        
-        @param request: DeleteLoadBalancerRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DeleteLoadBalancerResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.load_balancer_id):
             query['LoadBalancerId'] = request.load_balancer_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -2910,21 +2423,14 @@
         )
 
     async def delete_load_balancer_with_options_async(
         self,
         request: slb_20140515_models.DeleteLoadBalancerRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.DeleteLoadBalancerResponse:
-        """
-        >  After you delete an SLB instance, the listeners and tags added to the SLB instance are deleted.
-        
-        @param request: DeleteLoadBalancerRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DeleteLoadBalancerResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.load_balancer_id):
             query['LoadBalancerId'] = request.load_balancer_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -2954,48 +2460,29 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_load_balancer(
         self,
         request: slb_20140515_models.DeleteLoadBalancerRequest,
     ) -> slb_20140515_models.DeleteLoadBalancerResponse:
-        """
-        >  After you delete an SLB instance, the listeners and tags added to the SLB instance are deleted.
-        
-        @param request: DeleteLoadBalancerRequest
-        @return: DeleteLoadBalancerResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.delete_load_balancer_with_options(request, runtime)
 
     async def delete_load_balancer_async(
         self,
         request: slb_20140515_models.DeleteLoadBalancerRequest,
     ) -> slb_20140515_models.DeleteLoadBalancerResponse:
-        """
-        >  After you delete an SLB instance, the listeners and tags added to the SLB instance are deleted.
-        
-        @param request: DeleteLoadBalancerRequest
-        @return: DeleteLoadBalancerResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_load_balancer_with_options_async(request, runtime)
 
     def delete_load_balancer_listener_with_options(
         self,
         request: slb_20140515_models.DeleteLoadBalancerListenerRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.DeleteLoadBalancerListenerResponse:
-        """
-        >  A listener can be deleted only when it is in the *stopped** or **running** state.
-        
-        @param request: DeleteLoadBalancerListenerRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DeleteLoadBalancerListenerResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.listener_port):
             query['ListenerPort'] = request.listener_port
         if not UtilClient.is_unset(request.listener_protocol):
             query['ListenerProtocol'] = request.listener_protocol
         if not UtilClient.is_unset(request.load_balancer_id):
@@ -3030,21 +2517,14 @@
         )
 
     async def delete_load_balancer_listener_with_options_async(
         self,
         request: slb_20140515_models.DeleteLoadBalancerListenerRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.DeleteLoadBalancerListenerResponse:
-        """
-        >  A listener can be deleted only when it is in the *stopped** or **running** state.
-        
-        @param request: DeleteLoadBalancerListenerRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DeleteLoadBalancerListenerResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.listener_port):
             query['ListenerPort'] = request.listener_port
         if not UtilClient.is_unset(request.listener_protocol):
             query['ListenerProtocol'] = request.listener_protocol
         if not UtilClient.is_unset(request.load_balancer_id):
@@ -3078,33 +2558,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_load_balancer_listener(
         self,
         request: slb_20140515_models.DeleteLoadBalancerListenerRequest,
     ) -> slb_20140515_models.DeleteLoadBalancerListenerResponse:
-        """
-        >  A listener can be deleted only when it is in the *stopped** or **running** state.
-        
-        @param request: DeleteLoadBalancerListenerRequest
-        @return: DeleteLoadBalancerListenerResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.delete_load_balancer_listener_with_options(request, runtime)
 
     async def delete_load_balancer_listener_async(
         self,
         request: slb_20140515_models.DeleteLoadBalancerListenerRequest,
     ) -> slb_20140515_models.DeleteLoadBalancerListenerResponse:
-        """
-        >  A listener can be deleted only when it is in the *stopped** or **running** state.
-        
-        @param request: DeleteLoadBalancerListenerRequest
-        @return: DeleteLoadBalancerListenerResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_load_balancer_listener_with_options_async(request, runtime)
 
     def delete_master_slave_server_group_with_options(
         self,
         request: slb_20140515_models.DeleteMasterSlaveServerGroupRequest,
         runtime: util_models.RuntimeOptions,
@@ -3195,22 +2663,14 @@
         return await self.delete_master_slave_server_group_with_options_async(request, runtime)
 
     def delete_rules_with_options(
         self,
         request: slb_20140515_models.DeleteRulesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.DeleteRulesResponse:
-        """
-        ## Limits
-        The RuleIds parameter is required. You can specify up to 10 forwarding rules in each request.
-        
-        @param request: DeleteRulesRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DeleteRulesResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.region_id):
@@ -3241,22 +2701,14 @@
         )
 
     async def delete_rules_with_options_async(
         self,
         request: slb_20140515_models.DeleteRulesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.DeleteRulesResponse:
-        """
-        ## Limits
-        The RuleIds parameter is required. You can specify up to 10 forwarding rules in each request.
-        
-        @param request: DeleteRulesRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DeleteRulesResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.region_id):
@@ -3286,50 +2738,29 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_rules(
         self,
         request: slb_20140515_models.DeleteRulesRequest,
     ) -> slb_20140515_models.DeleteRulesResponse:
-        """
-        ## Limits
-        The RuleIds parameter is required. You can specify up to 10 forwarding rules in each request.
-        
-        @param request: DeleteRulesRequest
-        @return: DeleteRulesResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.delete_rules_with_options(request, runtime)
 
     async def delete_rules_async(
         self,
         request: slb_20140515_models.DeleteRulesRequest,
     ) -> slb_20140515_models.DeleteRulesResponse:
-        """
-        ## Limits
-        The RuleIds parameter is required. You can specify up to 10 forwarding rules in each request.
-        
-        @param request: DeleteRulesRequest
-        @return: DeleteRulesResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_rules_with_options_async(request, runtime)
 
     def delete_server_certificate_with_options(
         self,
         request: slb_20140515_models.DeleteServerCertificateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.DeleteServerCertificateResponse:
-        """
-        >  You cannot delete server certificates that are in use.
-        
-        @param request: DeleteServerCertificateRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DeleteServerCertificateResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.region_id):
@@ -3360,21 +2791,14 @@
         )
 
     async def delete_server_certificate_with_options_async(
         self,
         request: slb_20140515_models.DeleteServerCertificateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.DeleteServerCertificateResponse:
-        """
-        >  You cannot delete server certificates that are in use.
-        
-        @param request: DeleteServerCertificateRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DeleteServerCertificateResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.region_id):
@@ -3404,33 +2828,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_server_certificate(
         self,
         request: slb_20140515_models.DeleteServerCertificateRequest,
     ) -> slb_20140515_models.DeleteServerCertificateResponse:
-        """
-        >  You cannot delete server certificates that are in use.
-        
-        @param request: DeleteServerCertificateRequest
-        @return: DeleteServerCertificateResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.delete_server_certificate_with_options(request, runtime)
 
     async def delete_server_certificate_async(
         self,
         request: slb_20140515_models.DeleteServerCertificateRequest,
     ) -> slb_20140515_models.DeleteServerCertificateResponse:
-        """
-        >  You cannot delete server certificates that are in use.
-        
-        @param request: DeleteServerCertificateRequest
-        @return: DeleteServerCertificateResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_server_certificate_with_options_async(request, runtime)
 
     def delete_tlscipher_policy_with_options(
         self,
         request: slb_20140515_models.DeleteTLSCipherPolicyRequest,
         runtime: util_models.RuntimeOptions,
@@ -3445,14 +2857,16 @@
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
             query['ResourceOwnerId'] = request.resource_owner_id
         if not UtilClient.is_unset(request.tlscipher_policy_id):
             query['TLSCipherPolicyId'] = request.tlscipher_policy_id
+        if not UtilClient.is_unset(request.access_key_id):
+            query['access_key_id'] = request.access_key_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DeleteTLSCipherPolicy',
             version='2014-05-15',
             protocol='HTTPS',
@@ -3483,14 +2897,16 @@
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
             query['ResourceOwnerId'] = request.resource_owner_id
         if not UtilClient.is_unset(request.tlscipher_policy_id):
             query['TLSCipherPolicyId'] = request.tlscipher_policy_id
+        if not UtilClient.is_unset(request.access_key_id):
+            query['access_key_id'] = request.access_key_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DeleteTLSCipherPolicy',
             version='2014-05-15',
             protocol='HTTPS',
@@ -3621,18 +3037,14 @@
             query['AclEntryComment'] = request.acl_entry_comment
         if not UtilClient.is_unset(request.acl_id):
             query['AclId'] = request.acl_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
-        if not UtilClient.is_unset(request.page):
-            query['Page'] = request.page
-        if not UtilClient.is_unset(request.page_size):
-            query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
             query['ResourceOwnerId'] = request.resource_owner_id
         req = open_api_models.OpenApiRequest(
@@ -3665,18 +3077,14 @@
             query['AclEntryComment'] = request.acl_entry_comment
         if not UtilClient.is_unset(request.acl_id):
             query['AclId'] = request.acl_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
-        if not UtilClient.is_unset(request.page):
-            query['Page'] = request.page
-        if not UtilClient.is_unset(request.page_size):
-            query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
             query['ResourceOwnerId'] = request.resource_owner_id
         req = open_api_models.OpenApiRequest(
@@ -3814,132 +3222,19 @@
     async def describe_access_control_lists_async(
         self,
         request: slb_20140515_models.DescribeAccessControlListsRequest,
     ) -> slb_20140515_models.DescribeAccessControlListsResponse:
         runtime = util_models.RuntimeOptions()
         return await self.describe_access_control_lists_with_options_async(request, runtime)
 
-    def describe_access_logs_download_attribute_with_options(
-        self,
-        request: slb_20140515_models.DescribeAccessLogsDownloadAttributeRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> slb_20140515_models.DescribeAccessLogsDownloadAttributeResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.load_balancer_id):
-            query['LoadBalancerId'] = request.load_balancer_id
-        if not UtilClient.is_unset(request.log_type):
-            query['LogType'] = request.log_type
-        if not UtilClient.is_unset(request.owner_account):
-            query['OwnerAccount'] = request.owner_account
-        if not UtilClient.is_unset(request.owner_id):
-            query['OwnerId'] = request.owner_id
-        if not UtilClient.is_unset(request.page_number):
-            query['PageNumber'] = request.page_number
-        if not UtilClient.is_unset(request.page_size):
-            query['PageSize'] = request.page_size
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.resource_owner_account):
-            query['ResourceOwnerAccount'] = request.resource_owner_account
-        if not UtilClient.is_unset(request.resource_owner_id):
-            query['ResourceOwnerId'] = request.resource_owner_id
-        if not UtilClient.is_unset(request.tags):
-            query['Tags'] = request.tags
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DescribeAccessLogsDownloadAttribute',
-            version='2014-05-15',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            slb_20140515_models.DescribeAccessLogsDownloadAttributeResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def describe_access_logs_download_attribute_with_options_async(
-        self,
-        request: slb_20140515_models.DescribeAccessLogsDownloadAttributeRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> slb_20140515_models.DescribeAccessLogsDownloadAttributeResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.load_balancer_id):
-            query['LoadBalancerId'] = request.load_balancer_id
-        if not UtilClient.is_unset(request.log_type):
-            query['LogType'] = request.log_type
-        if not UtilClient.is_unset(request.owner_account):
-            query['OwnerAccount'] = request.owner_account
-        if not UtilClient.is_unset(request.owner_id):
-            query['OwnerId'] = request.owner_id
-        if not UtilClient.is_unset(request.page_number):
-            query['PageNumber'] = request.page_number
-        if not UtilClient.is_unset(request.page_size):
-            query['PageSize'] = request.page_size
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.resource_owner_account):
-            query['ResourceOwnerAccount'] = request.resource_owner_account
-        if not UtilClient.is_unset(request.resource_owner_id):
-            query['ResourceOwnerId'] = request.resource_owner_id
-        if not UtilClient.is_unset(request.tags):
-            query['Tags'] = request.tags
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DescribeAccessLogsDownloadAttribute',
-            version='2014-05-15',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            slb_20140515_models.DescribeAccessLogsDownloadAttributeResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def describe_access_logs_download_attribute(
-        self,
-        request: slb_20140515_models.DescribeAccessLogsDownloadAttributeRequest,
-    ) -> slb_20140515_models.DescribeAccessLogsDownloadAttributeResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.describe_access_logs_download_attribute_with_options(request, runtime)
-
-    async def describe_access_logs_download_attribute_async(
-        self,
-        request: slb_20140515_models.DescribeAccessLogsDownloadAttributeRequest,
-    ) -> slb_20140515_models.DescribeAccessLogsDownloadAttributeResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.describe_access_logs_download_attribute_with_options_async(request, runtime)
-
     def describe_available_resource_with_options(
         self,
         request: slb_20140515_models.DescribeAvailableResourceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.DescribeAvailableResourceResponse:
-        """
-        >  Only resources that are available for purchase and the corresponding zones are returned.
-        
-        @param request: DescribeAvailableResourceRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DescribeAvailableResourceResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.address_ipversion):
             query['AddressIPVersion'] = request.address_ipversion
         if not UtilClient.is_unset(request.address_type):
             query['AddressType'] = request.address_type
         if not UtilClient.is_unset(request.owner_account):
@@ -3972,21 +3267,14 @@
         )
 
     async def describe_available_resource_with_options_async(
         self,
         request: slb_20140515_models.DescribeAvailableResourceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.DescribeAvailableResourceResponse:
-        """
-        >  Only resources that are available for purchase and the corresponding zones are returned.
-        
-        @param request: DescribeAvailableResourceRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DescribeAvailableResourceResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.address_ipversion):
             query['AddressIPVersion'] = request.address_ipversion
         if not UtilClient.is_unset(request.address_type):
             query['AddressType'] = request.address_type
         if not UtilClient.is_unset(request.owner_account):
@@ -4018,48 +3306,29 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_available_resource(
         self,
         request: slb_20140515_models.DescribeAvailableResourceRequest,
     ) -> slb_20140515_models.DescribeAvailableResourceResponse:
-        """
-        >  Only resources that are available for purchase and the corresponding zones are returned.
-        
-        @param request: DescribeAvailableResourceRequest
-        @return: DescribeAvailableResourceResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.describe_available_resource_with_options(request, runtime)
 
     async def describe_available_resource_async(
         self,
         request: slb_20140515_models.DescribeAvailableResourceRequest,
     ) -> slb_20140515_models.DescribeAvailableResourceResponse:
-        """
-        >  Only resources that are available for purchase and the corresponding zones are returned.
-        
-        @param request: DescribeAvailableResourceRequest
-        @return: DescribeAvailableResourceResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_available_resource_with_options_async(request, runtime)
 
     def describe_cacertificates_with_options(
         self,
         request: slb_20140515_models.DescribeCACertificatesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.DescribeCACertificatesResponse:
-        """
-        >  For security reasons, only fingerprints and names of the CA certificates are returned, the content of the CA certificates is not returned.
-        
-        @param request: DescribeCACertificatesRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DescribeCACertificatesResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.cacertificate_id):
             query['CACertificateId'] = request.cacertificate_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -4092,21 +3361,14 @@
         )
 
     async def describe_cacertificates_with_options_async(
         self,
         request: slb_20140515_models.DescribeCACertificatesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.DescribeCACertificatesResponse:
-        """
-        >  For security reasons, only fingerprints and names of the CA certificates are returned, the content of the CA certificates is not returned.
-        
-        @param request: DescribeCACertificatesRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DescribeCACertificatesResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.cacertificate_id):
             query['CACertificateId'] = request.cacertificate_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -4138,33 +3400,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_cacertificates(
         self,
         request: slb_20140515_models.DescribeCACertificatesRequest,
     ) -> slb_20140515_models.DescribeCACertificatesResponse:
-        """
-        >  For security reasons, only fingerprints and names of the CA certificates are returned, the content of the CA certificates is not returned.
-        
-        @param request: DescribeCACertificatesRequest
-        @return: DescribeCACertificatesResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.describe_cacertificates_with_options(request, runtime)
 
     async def describe_cacertificates_async(
         self,
         request: slb_20140515_models.DescribeCACertificatesRequest,
     ) -> slb_20140515_models.DescribeCACertificatesResponse:
-        """
-        >  For security reasons, only fingerprints and names of the CA certificates are returned, the content of the CA certificates is not returned.
-        
-        @param request: DescribeCACertificatesRequest
-        @return: DescribeCACertificatesResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_cacertificates_with_options_async(request, runtime)
 
     def describe_domain_extension_attribute_with_options(
         self,
         request: slb_20140515_models.DescribeDomainExtensionAttributeRequest,
         runtime: util_models.RuntimeOptions,
@@ -4446,104 +3696,14 @@
     async def describe_health_status_async(
         self,
         request: slb_20140515_models.DescribeHealthStatusRequest,
     ) -> slb_20140515_models.DescribeHealthStatusResponse:
         runtime = util_models.RuntimeOptions()
         return await self.describe_health_status_with_options_async(request, runtime)
 
-    def describe_high_defination_monitor_with_options(
-        self,
-        request: slb_20140515_models.DescribeHighDefinationMonitorRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> slb_20140515_models.DescribeHighDefinationMonitorResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.owner_account):
-            query['OwnerAccount'] = request.owner_account
-        if not UtilClient.is_unset(request.owner_id):
-            query['OwnerId'] = request.owner_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.resource_owner_account):
-            query['ResourceOwnerAccount'] = request.resource_owner_account
-        if not UtilClient.is_unset(request.resource_owner_id):
-            query['ResourceOwnerId'] = request.resource_owner_id
-        if not UtilClient.is_unset(request.tags):
-            query['Tags'] = request.tags
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DescribeHighDefinationMonitor',
-            version='2014-05-15',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            slb_20140515_models.DescribeHighDefinationMonitorResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def describe_high_defination_monitor_with_options_async(
-        self,
-        request: slb_20140515_models.DescribeHighDefinationMonitorRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> slb_20140515_models.DescribeHighDefinationMonitorResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.owner_account):
-            query['OwnerAccount'] = request.owner_account
-        if not UtilClient.is_unset(request.owner_id):
-            query['OwnerId'] = request.owner_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.resource_owner_account):
-            query['ResourceOwnerAccount'] = request.resource_owner_account
-        if not UtilClient.is_unset(request.resource_owner_id):
-            query['ResourceOwnerId'] = request.resource_owner_id
-        if not UtilClient.is_unset(request.tags):
-            query['Tags'] = request.tags
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DescribeHighDefinationMonitor',
-            version='2014-05-15',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            slb_20140515_models.DescribeHighDefinationMonitorResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def describe_high_defination_monitor(
-        self,
-        request: slb_20140515_models.DescribeHighDefinationMonitorRequest,
-    ) -> slb_20140515_models.DescribeHighDefinationMonitorResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.describe_high_defination_monitor_with_options(request, runtime)
-
-    async def describe_high_defination_monitor_async(
-        self,
-        request: slb_20140515_models.DescribeHighDefinationMonitorRequest,
-    ) -> slb_20140515_models.DescribeHighDefinationMonitorResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.describe_high_defination_monitor_with_options_async(request, runtime)
-
     def describe_listener_access_control_attribute_with_options(
         self,
         request: slb_20140515_models.DescribeListenerAccessControlAttributeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.DescribeListenerAccessControlAttributeResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -4639,21 +3799,14 @@
         return await self.describe_listener_access_control_attribute_with_options_async(request, runtime)
 
     def describe_load_balancer_attribute_with_options(
         self,
         request: slb_20140515_models.DescribeLoadBalancerAttributeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.DescribeLoadBalancerAttributeResponse:
-        """
-        > If the backend servers are deployed in a vServer group, you can call the [DescribeVServerGroupAttribute](~~35224~~) operation to query the backend servers.
-        
-        @param request: DescribeLoadBalancerAttributeRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DescribeLoadBalancerAttributeResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.load_balancer_id):
             query['LoadBalancerId'] = request.load_balancer_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -4684,21 +3837,14 @@
         )
 
     async def describe_load_balancer_attribute_with_options_async(
         self,
         request: slb_20140515_models.DescribeLoadBalancerAttributeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.DescribeLoadBalancerAttributeResponse:
-        """
-        > If the backend servers are deployed in a vServer group, you can call the [DescribeVServerGroupAttribute](~~35224~~) operation to query the backend servers.
-        
-        @param request: DescribeLoadBalancerAttributeRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DescribeLoadBalancerAttributeResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.load_balancer_id):
             query['LoadBalancerId'] = request.load_balancer_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -4728,50 +3874,29 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_load_balancer_attribute(
         self,
         request: slb_20140515_models.DescribeLoadBalancerAttributeRequest,
     ) -> slb_20140515_models.DescribeLoadBalancerAttributeResponse:
-        """
-        > If the backend servers are deployed in a vServer group, you can call the [DescribeVServerGroupAttribute](~~35224~~) operation to query the backend servers.
-        
-        @param request: DescribeLoadBalancerAttributeRequest
-        @return: DescribeLoadBalancerAttributeResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.describe_load_balancer_attribute_with_options(request, runtime)
 
     async def describe_load_balancer_attribute_async(
         self,
         request: slb_20140515_models.DescribeLoadBalancerAttributeRequest,
     ) -> slb_20140515_models.DescribeLoadBalancerAttributeResponse:
-        """
-        > If the backend servers are deployed in a vServer group, you can call the [DescribeVServerGroupAttribute](~~35224~~) operation to query the backend servers.
-        
-        @param request: DescribeLoadBalancerAttributeRequest
-        @return: DescribeLoadBalancerAttributeResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_load_balancer_attribute_with_options_async(request, runtime)
 
     def describe_load_balancer_httplistener_attribute_with_options(
         self,
         request: slb_20140515_models.DescribeLoadBalancerHTTPListenerAttributeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.DescribeLoadBalancerHTTPListenerAttributeResponse:
-        """
-        ## Prerequisites
-        *   A CLB instance is created. For more information, see [CreateLoadBalancer](~~27577~~).
-        *   An HTTP listener is created. For more information about how to create an HTTP listener, see [CreateLoadBalancerHTTPListener](~~27592~~).
-        
-        @param request: DescribeLoadBalancerHTTPListenerAttributeRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DescribeLoadBalancerHTTPListenerAttributeResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.listener_port):
             query['ListenerPort'] = request.listener_port
         if not UtilClient.is_unset(request.load_balancer_id):
             query['LoadBalancerId'] = request.load_balancer_id
         if not UtilClient.is_unset(request.owner_account):
@@ -4804,23 +3929,14 @@
         )
 
     async def describe_load_balancer_httplistener_attribute_with_options_async(
         self,
         request: slb_20140515_models.DescribeLoadBalancerHTTPListenerAttributeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.DescribeLoadBalancerHTTPListenerAttributeResponse:
-        """
-        ## Prerequisites
-        *   A CLB instance is created. For more information, see [CreateLoadBalancer](~~27577~~).
-        *   An HTTP listener is created. For more information about how to create an HTTP listener, see [CreateLoadBalancerHTTPListener](~~27592~~).
-        
-        @param request: DescribeLoadBalancerHTTPListenerAttributeRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DescribeLoadBalancerHTTPListenerAttributeResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.listener_port):
             query['ListenerPort'] = request.listener_port
         if not UtilClient.is_unset(request.load_balancer_id):
             query['LoadBalancerId'] = request.load_balancer_id
         if not UtilClient.is_unset(request.owner_account):
@@ -4852,54 +3968,29 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_load_balancer_httplistener_attribute(
         self,
         request: slb_20140515_models.DescribeLoadBalancerHTTPListenerAttributeRequest,
     ) -> slb_20140515_models.DescribeLoadBalancerHTTPListenerAttributeResponse:
-        """
-        ## Prerequisites
-        *   A CLB instance is created. For more information, see [CreateLoadBalancer](~~27577~~).
-        *   An HTTP listener is created. For more information about how to create an HTTP listener, see [CreateLoadBalancerHTTPListener](~~27592~~).
-        
-        @param request: DescribeLoadBalancerHTTPListenerAttributeRequest
-        @return: DescribeLoadBalancerHTTPListenerAttributeResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.describe_load_balancer_httplistener_attribute_with_options(request, runtime)
 
     async def describe_load_balancer_httplistener_attribute_async(
         self,
         request: slb_20140515_models.DescribeLoadBalancerHTTPListenerAttributeRequest,
     ) -> slb_20140515_models.DescribeLoadBalancerHTTPListenerAttributeResponse:
-        """
-        ## Prerequisites
-        *   A CLB instance is created. For more information, see [CreateLoadBalancer](~~27577~~).
-        *   An HTTP listener is created. For more information about how to create an HTTP listener, see [CreateLoadBalancerHTTPListener](~~27592~~).
-        
-        @param request: DescribeLoadBalancerHTTPListenerAttributeRequest
-        @return: DescribeLoadBalancerHTTPListenerAttributeResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_load_balancer_httplistener_attribute_with_options_async(request, runtime)
 
     def describe_load_balancer_httpslistener_attribute_with_options(
         self,
         request: slb_20140515_models.DescribeLoadBalancerHTTPSListenerAttributeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.DescribeLoadBalancerHTTPSListenerAttributeResponse:
-        """
-        ## Prerequisites
-        *   A CLB instance is created. For more information, see [CreateLoadBalancer](~~27577~~).
-        *   An HTTPS listener is created. For more information about how to create an HTTPS listener, see [CreateLoadBalancerHTTPSListener](~~27593~~).
-        
-        @param request: DescribeLoadBalancerHTTPSListenerAttributeRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DescribeLoadBalancerHTTPSListenerAttributeResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.listener_port):
             query['ListenerPort'] = request.listener_port
         if not UtilClient.is_unset(request.load_balancer_id):
             query['LoadBalancerId'] = request.load_balancer_id
         if not UtilClient.is_unset(request.owner_account):
@@ -4932,23 +4023,14 @@
         )
 
     async def describe_load_balancer_httpslistener_attribute_with_options_async(
         self,
         request: slb_20140515_models.DescribeLoadBalancerHTTPSListenerAttributeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.DescribeLoadBalancerHTTPSListenerAttributeResponse:
-        """
-        ## Prerequisites
-        *   A CLB instance is created. For more information, see [CreateLoadBalancer](~~27577~~).
-        *   An HTTPS listener is created. For more information about how to create an HTTPS listener, see [CreateLoadBalancerHTTPSListener](~~27593~~).
-        
-        @param request: DescribeLoadBalancerHTTPSListenerAttributeRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DescribeLoadBalancerHTTPSListenerAttributeResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.listener_port):
             query['ListenerPort'] = request.listener_port
         if not UtilClient.is_unset(request.load_balancer_id):
             query['LoadBalancerId'] = request.load_balancer_id
         if not UtilClient.is_unset(request.owner_account):
@@ -4980,58 +4062,29 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_load_balancer_httpslistener_attribute(
         self,
         request: slb_20140515_models.DescribeLoadBalancerHTTPSListenerAttributeRequest,
     ) -> slb_20140515_models.DescribeLoadBalancerHTTPSListenerAttributeResponse:
-        """
-        ## Prerequisites
-        *   A CLB instance is created. For more information, see [CreateLoadBalancer](~~27577~~).
-        *   An HTTPS listener is created. For more information about how to create an HTTPS listener, see [CreateLoadBalancerHTTPSListener](~~27593~~).
-        
-        @param request: DescribeLoadBalancerHTTPSListenerAttributeRequest
-        @return: DescribeLoadBalancerHTTPSListenerAttributeResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.describe_load_balancer_httpslistener_attribute_with_options(request, runtime)
 
     async def describe_load_balancer_httpslistener_attribute_async(
         self,
         request: slb_20140515_models.DescribeLoadBalancerHTTPSListenerAttributeRequest,
     ) -> slb_20140515_models.DescribeLoadBalancerHTTPSListenerAttributeResponse:
-        """
-        ## Prerequisites
-        *   A CLB instance is created. For more information, see [CreateLoadBalancer](~~27577~~).
-        *   An HTTPS listener is created. For more information about how to create an HTTPS listener, see [CreateLoadBalancerHTTPSListener](~~27593~~).
-        
-        @param request: DescribeLoadBalancerHTTPSListenerAttributeRequest
-        @return: DescribeLoadBalancerHTTPSListenerAttributeResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_load_balancer_httpslistener_attribute_with_options_async(request, runtime)
 
     def describe_load_balancer_listeners_with_options(
         self,
         request: slb_20140515_models.DescribeLoadBalancerListenersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.DescribeLoadBalancerListenersResponse:
-        """
-        ## Prerequisites
-        *   A CLB instance is created. For more information, see [CreateLoadBalancer](~~27577~~).
-        *   One or more listeners are added to the CLB instance. For more information, see the following topics:
-        *   [CreateLoadBalancerUDPListener](~~27595~~)
-        *   [CreateLoadBalancerTCPListener](~~27594~~)
-        *   [CreateLoadBalancerHTTPListener](~~27592~~)
-        *   [CreateLoadBalancerHTTPSListener](~~27593~~)
-        
-        @param request: DescribeLoadBalancerListenersRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DescribeLoadBalancerListenersResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.listener_protocol):
             query['ListenerProtocol'] = request.listener_protocol
         if not UtilClient.is_unset(request.load_balancer_id):
             query['LoadBalancerId'] = request.load_balancer_id
         if not UtilClient.is_unset(request.max_results):
@@ -5068,27 +4121,14 @@
         )
 
     async def describe_load_balancer_listeners_with_options_async(
         self,
         request: slb_20140515_models.DescribeLoadBalancerListenersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.DescribeLoadBalancerListenersResponse:
-        """
-        ## Prerequisites
-        *   A CLB instance is created. For more information, see [CreateLoadBalancer](~~27577~~).
-        *   One or more listeners are added to the CLB instance. For more information, see the following topics:
-        *   [CreateLoadBalancerUDPListener](~~27595~~)
-        *   [CreateLoadBalancerTCPListener](~~27594~~)
-        *   [CreateLoadBalancerHTTPListener](~~27592~~)
-        *   [CreateLoadBalancerHTTPSListener](~~27593~~)
-        
-        @param request: DescribeLoadBalancerListenersRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DescribeLoadBalancerListenersResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.listener_protocol):
             query['ListenerProtocol'] = request.listener_protocol
         if not UtilClient.is_unset(request.load_balancer_id):
             query['LoadBalancerId'] = request.load_balancer_id
         if not UtilClient.is_unset(request.max_results):
@@ -5124,45 +4164,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_load_balancer_listeners(
         self,
         request: slb_20140515_models.DescribeLoadBalancerListenersRequest,
     ) -> slb_20140515_models.DescribeLoadBalancerListenersResponse:
-        """
-        ## Prerequisites
-        *   A CLB instance is created. For more information, see [CreateLoadBalancer](~~27577~~).
-        *   One or more listeners are added to the CLB instance. For more information, see the following topics:
-        *   [CreateLoadBalancerUDPListener](~~27595~~)
-        *   [CreateLoadBalancerTCPListener](~~27594~~)
-        *   [CreateLoadBalancerHTTPListener](~~27592~~)
-        *   [CreateLoadBalancerHTTPSListener](~~27593~~)
-        
-        @param request: DescribeLoadBalancerListenersRequest
-        @return: DescribeLoadBalancerListenersResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.describe_load_balancer_listeners_with_options(request, runtime)
 
     async def describe_load_balancer_listeners_async(
         self,
         request: slb_20140515_models.DescribeLoadBalancerListenersRequest,
     ) -> slb_20140515_models.DescribeLoadBalancerListenersResponse:
-        """
-        ## Prerequisites
-        *   A CLB instance is created. For more information, see [CreateLoadBalancer](~~27577~~).
-        *   One or more listeners are added to the CLB instance. For more information, see the following topics:
-        *   [CreateLoadBalancerUDPListener](~~27595~~)
-        *   [CreateLoadBalancerTCPListener](~~27594~~)
-        *   [CreateLoadBalancerHTTPListener](~~27592~~)
-        *   [CreateLoadBalancerHTTPSListener](~~27593~~)
-        
-        @param request: DescribeLoadBalancerListenersRequest
-        @return: DescribeLoadBalancerListenersResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_load_balancer_listeners_with_options_async(request, runtime)
 
     def describe_load_balancer_tcplistener_attribute_with_options(
         self,
         request: slb_20140515_models.DescribeLoadBalancerTCPListenerAttributeRequest,
         runtime: util_models.RuntimeOptions,
@@ -5975,21 +4991,14 @@
         return await self.describe_rules_with_options_async(request, runtime)
 
     def describe_server_certificates_with_options(
         self,
         request: slb_20140515_models.DescribeServerCertificatesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.DescribeServerCertificatesResponse:
-        """
-        >  For security reasons, only fingerprints and names of the server certificates are returned. The content of the server certificates and private keys is not returned.
-        
-        @param request: DescribeServerCertificatesRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DescribeServerCertificatesResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.region_id):
@@ -6022,21 +5031,14 @@
         )
 
     async def describe_server_certificates_with_options_async(
         self,
         request: slb_20140515_models.DescribeServerCertificatesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.DescribeServerCertificatesResponse:
-        """
-        >  For security reasons, only fingerprints and names of the server certificates are returned. The content of the server certificates and private keys is not returned.
-        
-        @param request: DescribeServerCertificatesRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DescribeServerCertificatesResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.region_id):
@@ -6068,53 +5070,29 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_server_certificates(
         self,
         request: slb_20140515_models.DescribeServerCertificatesRequest,
     ) -> slb_20140515_models.DescribeServerCertificatesResponse:
-        """
-        >  For security reasons, only fingerprints and names of the server certificates are returned. The content of the server certificates and private keys is not returned.
-        
-        @param request: DescribeServerCertificatesRequest
-        @return: DescribeServerCertificatesResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.describe_server_certificates_with_options(request, runtime)
 
     async def describe_server_certificates_async(
         self,
         request: slb_20140515_models.DescribeServerCertificatesRequest,
     ) -> slb_20140515_models.DescribeServerCertificatesResponse:
-        """
-        >  For security reasons, only fingerprints and names of the server certificates are returned. The content of the server certificates and private keys is not returned.
-        
-        @param request: DescribeServerCertificatesRequest
-        @return: DescribeServerCertificatesResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_server_certificates_with_options_async(request, runtime)
 
     def describe_tags_with_options(
         self,
         request: slb_20140515_models.DescribeTagsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.DescribeTagsResponse:
-        """
-        When you call this operation, take note of the following items:
-        *   You can query tags by instance ID, tag key, and tag value. If the operation is successful, the system returns all tags that match the specified conditions.
-        *   The logical relationship among the specified conditions is AND. Only tags that match all the specified conditions are returned.
-        *   If the Tagkey parameter is set and the Tagvalue parameter is not set, all tags that contain the specified tag key are returned.
-        *   If you set the Tagvalue parameter in a request, you must also set the Tagkey parameter in the request.
-        *   If you set both the Tagkey and Tagvalue parameters, only tags that contain the specified keys and values are returned.
-        
-        @param request: DescribeTagsRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DescribeTagsResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.distinct_key):
             query['DistinctKey'] = request.distinct_key
         if not UtilClient.is_unset(request.load_balancer_id):
             query['LoadBalancerId'] = request.load_balancer_id
         if not UtilClient.is_unset(request.owner_account):
@@ -6153,26 +5131,14 @@
         )
 
     async def describe_tags_with_options_async(
         self,
         request: slb_20140515_models.DescribeTagsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.DescribeTagsResponse:
-        """
-        When you call this operation, take note of the following items:
-        *   You can query tags by instance ID, tag key, and tag value. If the operation is successful, the system returns all tags that match the specified conditions.
-        *   The logical relationship among the specified conditions is AND. Only tags that match all the specified conditions are returned.
-        *   If the Tagkey parameter is set and the Tagvalue parameter is not set, all tags that contain the specified tag key are returned.
-        *   If you set the Tagvalue parameter in a request, you must also set the Tagkey parameter in the request.
-        *   If you set both the Tagkey and Tagvalue parameters, only tags that contain the specified keys and values are returned.
-        
-        @param request: DescribeTagsRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DescribeTagsResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.distinct_key):
             query['DistinctKey'] = request.distinct_key
         if not UtilClient.is_unset(request.load_balancer_id):
             query['LoadBalancerId'] = request.load_balancer_id
         if not UtilClient.is_unset(request.owner_account):
@@ -6210,43 +5176,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_tags(
         self,
         request: slb_20140515_models.DescribeTagsRequest,
     ) -> slb_20140515_models.DescribeTagsResponse:
-        """
-        When you call this operation, take note of the following items:
-        *   You can query tags by instance ID, tag key, and tag value. If the operation is successful, the system returns all tags that match the specified conditions.
-        *   The logical relationship among the specified conditions is AND. Only tags that match all the specified conditions are returned.
-        *   If the Tagkey parameter is set and the Tagvalue parameter is not set, all tags that contain the specified tag key are returned.
-        *   If you set the Tagvalue parameter in a request, you must also set the Tagkey parameter in the request.
-        *   If you set both the Tagkey and Tagvalue parameters, only tags that contain the specified keys and values are returned.
-        
-        @param request: DescribeTagsRequest
-        @return: DescribeTagsResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.describe_tags_with_options(request, runtime)
 
     async def describe_tags_async(
         self,
         request: slb_20140515_models.DescribeTagsRequest,
     ) -> slb_20140515_models.DescribeTagsResponse:
-        """
-        When you call this operation, take note of the following items:
-        *   You can query tags by instance ID, tag key, and tag value. If the operation is successful, the system returns all tags that match the specified conditions.
-        *   The logical relationship among the specified conditions is AND. Only tags that match all the specified conditions are returned.
-        *   If the Tagkey parameter is set and the Tagvalue parameter is not set, all tags that contain the specified tag key are returned.
-        *   If you set the Tagvalue parameter in a request, you must also set the Tagkey parameter in the request.
-        *   If you set both the Tagkey and Tagvalue parameters, only tags that contain the specified keys and values are returned.
-        
-        @param request: DescribeTagsRequest
-        @return: DescribeTagsResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_tags_with_options_async(request, runtime)
 
     def describe_vserver_group_attribute_with_options(
         self,
         request: slb_20140515_models.DescribeVServerGroupAttributeRequest,
         runtime: util_models.RuntimeOptions,
@@ -6516,112 +5460,14 @@
     async def describe_zones_async(
         self,
         request: slb_20140515_models.DescribeZonesRequest,
     ) -> slb_20140515_models.DescribeZonesResponse:
         runtime = util_models.RuntimeOptions()
         return await self.describe_zones_with_options_async(request, runtime)
 
-    def enable_high_defination_monitor_with_options(
-        self,
-        request: slb_20140515_models.EnableHighDefinationMonitorRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> slb_20140515_models.EnableHighDefinationMonitorResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.log_project):
-            query['LogProject'] = request.log_project
-        if not UtilClient.is_unset(request.log_store):
-            query['LogStore'] = request.log_store
-        if not UtilClient.is_unset(request.owner_account):
-            query['OwnerAccount'] = request.owner_account
-        if not UtilClient.is_unset(request.owner_id):
-            query['OwnerId'] = request.owner_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.resource_owner_account):
-            query['ResourceOwnerAccount'] = request.resource_owner_account
-        if not UtilClient.is_unset(request.resource_owner_id):
-            query['ResourceOwnerId'] = request.resource_owner_id
-        if not UtilClient.is_unset(request.tags):
-            query['Tags'] = request.tags
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='EnableHighDefinationMonitor',
-            version='2014-05-15',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            slb_20140515_models.EnableHighDefinationMonitorResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def enable_high_defination_monitor_with_options_async(
-        self,
-        request: slb_20140515_models.EnableHighDefinationMonitorRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> slb_20140515_models.EnableHighDefinationMonitorResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.log_project):
-            query['LogProject'] = request.log_project
-        if not UtilClient.is_unset(request.log_store):
-            query['LogStore'] = request.log_store
-        if not UtilClient.is_unset(request.owner_account):
-            query['OwnerAccount'] = request.owner_account
-        if not UtilClient.is_unset(request.owner_id):
-            query['OwnerId'] = request.owner_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.resource_owner_account):
-            query['ResourceOwnerAccount'] = request.resource_owner_account
-        if not UtilClient.is_unset(request.resource_owner_id):
-            query['ResourceOwnerId'] = request.resource_owner_id
-        if not UtilClient.is_unset(request.tags):
-            query['Tags'] = request.tags
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='EnableHighDefinationMonitor',
-            version='2014-05-15',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            slb_20140515_models.EnableHighDefinationMonitorResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def enable_high_defination_monitor(
-        self,
-        request: slb_20140515_models.EnableHighDefinationMonitorRequest,
-    ) -> slb_20140515_models.EnableHighDefinationMonitorResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.enable_high_defination_monitor_with_options(request, runtime)
-
-    async def enable_high_defination_monitor_async(
-        self,
-        request: slb_20140515_models.EnableHighDefinationMonitorRequest,
-    ) -> slb_20140515_models.EnableHighDefinationMonitorResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.enable_high_defination_monitor_with_options_async(request, runtime)
-
     def list_tlscipher_policies_with_options(
         self,
         request: slb_20140515_models.ListTLSCipherPoliciesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.ListTLSCipherPoliciesResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -6641,14 +5487,16 @@
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
             query['ResourceOwnerId'] = request.resource_owner_id
         if not UtilClient.is_unset(request.tlscipher_policy_id):
             query['TLSCipherPolicyId'] = request.tlscipher_policy_id
+        if not UtilClient.is_unset(request.access_key_id):
+            query['access_key_id'] = request.access_key_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListTLSCipherPolicies',
             version='2014-05-15',
             protocol='HTTPS',
@@ -6687,14 +5535,16 @@
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
             query['ResourceOwnerId'] = request.resource_owner_id
         if not UtilClient.is_unset(request.tlscipher_policy_id):
             query['TLSCipherPolicyId'] = request.tlscipher_policy_id
+        if not UtilClient.is_unset(request.access_key_id):
+            query['access_key_id'] = request.access_key_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListTLSCipherPolicies',
             version='2014-05-15',
             protocol='HTTPS',
@@ -6725,24 +5575,14 @@
         return await self.list_tlscipher_policies_with_options_async(request, runtime)
 
     def list_tag_resources_with_options(
         self,
         request: slb_20140515_models.ListTagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.ListTagResourcesResponse:
-        """
-        Set **ResourceId.N** or **Tag.N** that consists of **Tag.N.Key** and **Tag.N.Value** in the request to specify the object to be queried.
-        *   **Tag.N** is a resource tag that consists of a key-value pair. If you set only **Tag.N.Key**, all tag values that are associated with the specified tag key are returned. If you set only **Tag.N.Value**, an error message is returned.
-        *   If you set **Tag.N** and **ResourceId.N** to filter tags, **ResourceId.N** must match all specified key-value pairs.
-        *   If you specify multiple key-value pairs, resources that contain these key-value pairs are returned.
-        
-        @param request: ListTagResourcesRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ListTagResourcesResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -6779,24 +5619,14 @@
         )
 
     async def list_tag_resources_with_options_async(
         self,
         request: slb_20140515_models.ListTagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.ListTagResourcesResponse:
-        """
-        Set **ResourceId.N** or **Tag.N** that consists of **Tag.N.Key** and **Tag.N.Value** in the request to specify the object to be queried.
-        *   **Tag.N** is a resource tag that consists of a key-value pair. If you set only **Tag.N.Key**, all tag values that are associated with the specified tag key are returned. If you set only **Tag.N.Value**, an error message is returned.
-        *   If you set **Tag.N** and **ResourceId.N** to filter tags, **ResourceId.N** must match all specified key-value pairs.
-        *   If you specify multiple key-value pairs, resources that contain these key-value pairs are returned.
-        
-        @param request: ListTagResourcesRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ListTagResourcesResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -6832,276 +5662,24 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_tag_resources(
         self,
         request: slb_20140515_models.ListTagResourcesRequest,
     ) -> slb_20140515_models.ListTagResourcesResponse:
-        """
-        Set **ResourceId.N** or **Tag.N** that consists of **Tag.N.Key** and **Tag.N.Value** in the request to specify the object to be queried.
-        *   **Tag.N** is a resource tag that consists of a key-value pair. If you set only **Tag.N.Key**, all tag values that are associated with the specified tag key are returned. If you set only **Tag.N.Value**, an error message is returned.
-        *   If you set **Tag.N** and **ResourceId.N** to filter tags, **ResourceId.N** must match all specified key-value pairs.
-        *   If you specify multiple key-value pairs, resources that contain these key-value pairs are returned.
-        
-        @param request: ListTagResourcesRequest
-        @return: ListTagResourcesResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.list_tag_resources_with_options(request, runtime)
 
     async def list_tag_resources_async(
         self,
         request: slb_20140515_models.ListTagResourcesRequest,
     ) -> slb_20140515_models.ListTagResourcesResponse:
-        """
-        Set **ResourceId.N** or **Tag.N** that consists of **Tag.N.Key** and **Tag.N.Value** in the request to specify the object to be queried.
-        *   **Tag.N** is a resource tag that consists of a key-value pair. If you set only **Tag.N.Key**, all tag values that are associated with the specified tag key are returned. If you set only **Tag.N.Value**, an error message is returned.
-        *   If you set **Tag.N** and **ResourceId.N** to filter tags, **ResourceId.N** must match all specified key-value pairs.
-        *   If you specify multiple key-value pairs, resources that contain these key-value pairs are returned.
-        
-        @param request: ListTagResourcesRequest
-        @return: ListTagResourcesResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.list_tag_resources_with_options_async(request, runtime)
 
-    def modify_high_defination_monitor_with_options(
-        self,
-        request: slb_20140515_models.ModifyHighDefinationMonitorRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> slb_20140515_models.ModifyHighDefinationMonitorResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.log_project):
-            query['LogProject'] = request.log_project
-        if not UtilClient.is_unset(request.log_store):
-            query['LogStore'] = request.log_store
-        if not UtilClient.is_unset(request.owner_account):
-            query['OwnerAccount'] = request.owner_account
-        if not UtilClient.is_unset(request.owner_id):
-            query['OwnerId'] = request.owner_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.resource_owner_account):
-            query['ResourceOwnerAccount'] = request.resource_owner_account
-        if not UtilClient.is_unset(request.resource_owner_id):
-            query['ResourceOwnerId'] = request.resource_owner_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='ModifyHighDefinationMonitor',
-            version='2014-05-15',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            slb_20140515_models.ModifyHighDefinationMonitorResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def modify_high_defination_monitor_with_options_async(
-        self,
-        request: slb_20140515_models.ModifyHighDefinationMonitorRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> slb_20140515_models.ModifyHighDefinationMonitorResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.log_project):
-            query['LogProject'] = request.log_project
-        if not UtilClient.is_unset(request.log_store):
-            query['LogStore'] = request.log_store
-        if not UtilClient.is_unset(request.owner_account):
-            query['OwnerAccount'] = request.owner_account
-        if not UtilClient.is_unset(request.owner_id):
-            query['OwnerId'] = request.owner_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.resource_owner_account):
-            query['ResourceOwnerAccount'] = request.resource_owner_account
-        if not UtilClient.is_unset(request.resource_owner_id):
-            query['ResourceOwnerId'] = request.resource_owner_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='ModifyHighDefinationMonitor',
-            version='2014-05-15',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            slb_20140515_models.ModifyHighDefinationMonitorResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def modify_high_defination_monitor(
-        self,
-        request: slb_20140515_models.ModifyHighDefinationMonitorRequest,
-    ) -> slb_20140515_models.ModifyHighDefinationMonitorResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.modify_high_defination_monitor_with_options(request, runtime)
-
-    async def modify_high_defination_monitor_async(
-        self,
-        request: slb_20140515_models.ModifyHighDefinationMonitorRequest,
-    ) -> slb_20140515_models.ModifyHighDefinationMonitorResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.modify_high_defination_monitor_with_options_async(request, runtime)
-
-    def modify_load_balancer_instance_charge_type_with_options(
-        self,
-        request: slb_20140515_models.ModifyLoadBalancerInstanceChargeTypeRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> slb_20140515_models.ModifyLoadBalancerInstanceChargeTypeResponse:
-        """
-        >
-        *   For pay-as-you-go CLB instances, you can only change the metering method from pay-by-specification to pay-by-LCU. You cannot change the metering method from pay-by-LCU to pay-by-specification.
-        *   This operation can change the metering method of only one instance at a time.
-        
-        @param request: ModifyLoadBalancerInstanceChargeTypeRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ModifyLoadBalancerInstanceChargeTypeResponse
-        """
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.bandwidth):
-            query['Bandwidth'] = request.bandwidth
-        if not UtilClient.is_unset(request.instance_charge_type):
-            query['InstanceChargeType'] = request.instance_charge_type
-        if not UtilClient.is_unset(request.internet_charge_type):
-            query['InternetChargeType'] = request.internet_charge_type
-        if not UtilClient.is_unset(request.load_balancer_id):
-            query['LoadBalancerId'] = request.load_balancer_id
-        if not UtilClient.is_unset(request.load_balancer_spec):
-            query['LoadBalancerSpec'] = request.load_balancer_spec
-        if not UtilClient.is_unset(request.owner_account):
-            query['OwnerAccount'] = request.owner_account
-        if not UtilClient.is_unset(request.owner_id):
-            query['OwnerId'] = request.owner_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.resource_owner_account):
-            query['ResourceOwnerAccount'] = request.resource_owner_account
-        if not UtilClient.is_unset(request.resource_owner_id):
-            query['ResourceOwnerId'] = request.resource_owner_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='ModifyLoadBalancerInstanceChargeType',
-            version='2014-05-15',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            slb_20140515_models.ModifyLoadBalancerInstanceChargeTypeResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def modify_load_balancer_instance_charge_type_with_options_async(
-        self,
-        request: slb_20140515_models.ModifyLoadBalancerInstanceChargeTypeRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> slb_20140515_models.ModifyLoadBalancerInstanceChargeTypeResponse:
-        """
-        >
-        *   For pay-as-you-go CLB instances, you can only change the metering method from pay-by-specification to pay-by-LCU. You cannot change the metering method from pay-by-LCU to pay-by-specification.
-        *   This operation can change the metering method of only one instance at a time.
-        
-        @param request: ModifyLoadBalancerInstanceChargeTypeRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ModifyLoadBalancerInstanceChargeTypeResponse
-        """
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.bandwidth):
-            query['Bandwidth'] = request.bandwidth
-        if not UtilClient.is_unset(request.instance_charge_type):
-            query['InstanceChargeType'] = request.instance_charge_type
-        if not UtilClient.is_unset(request.internet_charge_type):
-            query['InternetChargeType'] = request.internet_charge_type
-        if not UtilClient.is_unset(request.load_balancer_id):
-            query['LoadBalancerId'] = request.load_balancer_id
-        if not UtilClient.is_unset(request.load_balancer_spec):
-            query['LoadBalancerSpec'] = request.load_balancer_spec
-        if not UtilClient.is_unset(request.owner_account):
-            query['OwnerAccount'] = request.owner_account
-        if not UtilClient.is_unset(request.owner_id):
-            query['OwnerId'] = request.owner_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.resource_owner_account):
-            query['ResourceOwnerAccount'] = request.resource_owner_account
-        if not UtilClient.is_unset(request.resource_owner_id):
-            query['ResourceOwnerId'] = request.resource_owner_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='ModifyLoadBalancerInstanceChargeType',
-            version='2014-05-15',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            slb_20140515_models.ModifyLoadBalancerInstanceChargeTypeResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def modify_load_balancer_instance_charge_type(
-        self,
-        request: slb_20140515_models.ModifyLoadBalancerInstanceChargeTypeRequest,
-    ) -> slb_20140515_models.ModifyLoadBalancerInstanceChargeTypeResponse:
-        """
-        >
-        *   For pay-as-you-go CLB instances, you can only change the metering method from pay-by-specification to pay-by-LCU. You cannot change the metering method from pay-by-LCU to pay-by-specification.
-        *   This operation can change the metering method of only one instance at a time.
-        
-        @param request: ModifyLoadBalancerInstanceChargeTypeRequest
-        @return: ModifyLoadBalancerInstanceChargeTypeResponse
-        """
-        runtime = util_models.RuntimeOptions()
-        return self.modify_load_balancer_instance_charge_type_with_options(request, runtime)
-
-    async def modify_load_balancer_instance_charge_type_async(
-        self,
-        request: slb_20140515_models.ModifyLoadBalancerInstanceChargeTypeRequest,
-    ) -> slb_20140515_models.ModifyLoadBalancerInstanceChargeTypeResponse:
-        """
-        >
-        *   For pay-as-you-go CLB instances, you can only change the metering method from pay-by-specification to pay-by-LCU. You cannot change the metering method from pay-by-LCU to pay-by-specification.
-        *   This operation can change the metering method of only one instance at a time.
-        
-        @param request: ModifyLoadBalancerInstanceChargeTypeRequest
-        @return: ModifyLoadBalancerInstanceChargeTypeResponse
-        """
-        runtime = util_models.RuntimeOptions()
-        return await self.modify_load_balancer_instance_charge_type_with_options_async(request, runtime)
-
     def modify_load_balancer_instance_spec_with_options(
         self,
         request: slb_20140515_models.ModifyLoadBalancerInstanceSpecRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.ModifyLoadBalancerInstanceSpecResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -7197,23 +5775,14 @@
         return await self.modify_load_balancer_instance_spec_with_options_async(request, runtime)
 
     def modify_load_balancer_internet_spec_with_options(
         self,
         request: slb_20140515_models.ModifyLoadBalancerInternetSpecRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.ModifyLoadBalancerInternetSpecResponse:
-        """
-        ## Description
-        *   If you modify only the maximum bandwidth of a pay-by-bandwidth CLB instance, the new bandwidth immediately takes effect.
-        *   If you modify the metering method (for example, switch from pay-by-bandwidth to pay-by-data-transfer), the new metering method and the other changes specified in the operation take effect at 00:00:00 the next day.
-        
-        @param request: ModifyLoadBalancerInternetSpecRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ModifyLoadBalancerInternetSpecResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.auto_pay):
             query['AutoPay'] = request.auto_pay
         if not UtilClient.is_unset(request.bandwidth):
             query['Bandwidth'] = request.bandwidth
         if not UtilClient.is_unset(request.internet_charge_type):
@@ -7250,23 +5819,14 @@
         )
 
     async def modify_load_balancer_internet_spec_with_options_async(
         self,
         request: slb_20140515_models.ModifyLoadBalancerInternetSpecRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.ModifyLoadBalancerInternetSpecResponse:
-        """
-        ## Description
-        *   If you modify only the maximum bandwidth of a pay-by-bandwidth CLB instance, the new bandwidth immediately takes effect.
-        *   If you modify the metering method (for example, switch from pay-by-bandwidth to pay-by-data-transfer), the new metering method and the other changes specified in the operation take effect at 00:00:00 the next day.
-        
-        @param request: ModifyLoadBalancerInternetSpecRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ModifyLoadBalancerInternetSpecResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.auto_pay):
             query['AutoPay'] = request.auto_pay
         if not UtilClient.is_unset(request.bandwidth):
             query['Bandwidth'] = request.bandwidth
         if not UtilClient.is_unset(request.internet_charge_type):
@@ -7302,37 +5862,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_load_balancer_internet_spec(
         self,
         request: slb_20140515_models.ModifyLoadBalancerInternetSpecRequest,
     ) -> slb_20140515_models.ModifyLoadBalancerInternetSpecResponse:
-        """
-        ## Description
-        *   If you modify only the maximum bandwidth of a pay-by-bandwidth CLB instance, the new bandwidth immediately takes effect.
-        *   If you modify the metering method (for example, switch from pay-by-bandwidth to pay-by-data-transfer), the new metering method and the other changes specified in the operation take effect at 00:00:00 the next day.
-        
-        @param request: ModifyLoadBalancerInternetSpecRequest
-        @return: ModifyLoadBalancerInternetSpecResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.modify_load_balancer_internet_spec_with_options(request, runtime)
 
     async def modify_load_balancer_internet_spec_async(
         self,
         request: slb_20140515_models.ModifyLoadBalancerInternetSpecRequest,
     ) -> slb_20140515_models.ModifyLoadBalancerInternetSpecResponse:
-        """
-        ## Description
-        *   If you modify only the maximum bandwidth of a pay-by-bandwidth CLB instance, the new bandwidth immediately takes effect.
-        *   If you modify the metering method (for example, switch from pay-by-bandwidth to pay-by-data-transfer), the new metering method and the other changes specified in the operation take effect at 00:00:00 the next day.
-        
-        @param request: ModifyLoadBalancerInternetSpecRequest
-        @return: ModifyLoadBalancerInternetSpecResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_load_balancer_internet_spec_with_options_async(request, runtime)
 
     def modify_load_balancer_pay_type_with_options(
         self,
         request: slb_20140515_models.ModifyLoadBalancerPayTypeRequest,
         runtime: util_models.RuntimeOptions,
@@ -7439,21 +5983,14 @@
         return await self.modify_load_balancer_pay_type_with_options_async(request, runtime)
 
     def modify_vserver_group_backend_servers_with_options(
         self,
         request: slb_20140515_models.ModifyVServerGroupBackendServersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.ModifyVServerGroupBackendServersResponse:
-        """
-        You can call this operation to replace the backend servers in a specified vServer group. To modify the configurations of the backend servers, such as their weights, you can call the [SetVServerGroupAttribute](~~35217~~) operation.
-        
-        @param request: ModifyVServerGroupBackendServersRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ModifyVServerGroupBackendServersResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.new_backend_servers):
             query['NewBackendServers'] = request.new_backend_servers
         if not UtilClient.is_unset(request.old_backend_servers):
             query['OldBackendServers'] = request.old_backend_servers
         if not UtilClient.is_unset(request.owner_account):
@@ -7488,21 +6025,14 @@
         )
 
     async def modify_vserver_group_backend_servers_with_options_async(
         self,
         request: slb_20140515_models.ModifyVServerGroupBackendServersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.ModifyVServerGroupBackendServersResponse:
-        """
-        You can call this operation to replace the backend servers in a specified vServer group. To modify the configurations of the backend servers, such as their weights, you can call the [SetVServerGroupAttribute](~~35217~~) operation.
-        
-        @param request: ModifyVServerGroupBackendServersRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ModifyVServerGroupBackendServersResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.new_backend_servers):
             query['NewBackendServers'] = request.new_backend_servers
         if not UtilClient.is_unset(request.old_backend_servers):
             query['OldBackendServers'] = request.old_backend_servers
         if not UtilClient.is_unset(request.owner_account):
@@ -7536,33 +6066,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_vserver_group_backend_servers(
         self,
         request: slb_20140515_models.ModifyVServerGroupBackendServersRequest,
     ) -> slb_20140515_models.ModifyVServerGroupBackendServersResponse:
-        """
-        You can call this operation to replace the backend servers in a specified vServer group. To modify the configurations of the backend servers, such as their weights, you can call the [SetVServerGroupAttribute](~~35217~~) operation.
-        
-        @param request: ModifyVServerGroupBackendServersRequest
-        @return: ModifyVServerGroupBackendServersResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.modify_vserver_group_backend_servers_with_options(request, runtime)
 
     async def modify_vserver_group_backend_servers_async(
         self,
         request: slb_20140515_models.ModifyVServerGroupBackendServersRequest,
     ) -> slb_20140515_models.ModifyVServerGroupBackendServersResponse:
-        """
-        You can call this operation to replace the backend servers in a specified vServer group. To modify the configurations of the backend servers, such as their weights, you can call the [SetVServerGroupAttribute](~~35217~~) operation.
-        
-        @param request: ModifyVServerGroupBackendServersRequest
-        @return: ModifyVServerGroupBackendServersResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_vserver_group_backend_servers_with_options_async(request, runtime)
 
     def remove_access_control_list_entry_with_options(
         self,
         request: slb_20140515_models.RemoveAccessControlListEntryRequest,
         runtime: util_models.RuntimeOptions,
@@ -7657,21 +6175,14 @@
         return await self.remove_access_control_list_entry_with_options_async(request, runtime)
 
     def remove_backend_servers_with_options(
         self,
         request: slb_20140515_models.RemoveBackendServersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.RemoveBackendServersResponse:
-        """
-        >  If the backend servers that you want to remove are not in the server list of the Classic Load Balancer (CLB) instance, the request fails. However, the system does not report an error.
-        
-        @param request: RemoveBackendServersRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: RemoveBackendServersResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.backend_servers):
             query['BackendServers'] = request.backend_servers
         if not UtilClient.is_unset(request.load_balancer_id):
             query['LoadBalancerId'] = request.load_balancer_id
         if not UtilClient.is_unset(request.owner_account):
@@ -7704,21 +6215,14 @@
         )
 
     async def remove_backend_servers_with_options_async(
         self,
         request: slb_20140515_models.RemoveBackendServersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.RemoveBackendServersResponse:
-        """
-        >  If the backend servers that you want to remove are not in the server list of the Classic Load Balancer (CLB) instance, the request fails. However, the system does not report an error.
-        
-        @param request: RemoveBackendServersRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: RemoveBackendServersResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.backend_servers):
             query['BackendServers'] = request.backend_servers
         if not UtilClient.is_unset(request.load_balancer_id):
             query['LoadBalancerId'] = request.load_balancer_id
         if not UtilClient.is_unset(request.owner_account):
@@ -7750,33 +6254,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def remove_backend_servers(
         self,
         request: slb_20140515_models.RemoveBackendServersRequest,
     ) -> slb_20140515_models.RemoveBackendServersResponse:
-        """
-        >  If the backend servers that you want to remove are not in the server list of the Classic Load Balancer (CLB) instance, the request fails. However, the system does not report an error.
-        
-        @param request: RemoveBackendServersRequest
-        @return: RemoveBackendServersResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.remove_backend_servers_with_options(request, runtime)
 
     async def remove_backend_servers_async(
         self,
         request: slb_20140515_models.RemoveBackendServersRequest,
     ) -> slb_20140515_models.RemoveBackendServersResponse:
-        """
-        >  If the backend servers that you want to remove are not in the server list of the Classic Load Balancer (CLB) instance, the request fails. However, the system does not report an error.
-        
-        @param request: RemoveBackendServersRequest
-        @return: RemoveBackendServersResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.remove_backend_servers_with_options_async(request, runtime)
 
     def remove_listener_white_list_item_with_options(
         self,
         request: slb_20140515_models.RemoveListenerWhiteListItemRequest,
         runtime: util_models.RuntimeOptions,
@@ -7973,21 +6465,14 @@
         return await self.remove_tags_with_options_async(request, runtime)
 
     def remove_vserver_group_backend_servers_with_options(
         self,
         request: slb_20140515_models.RemoveVServerGroupBackendServersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.RemoveVServerGroupBackendServersResponse:
-        """
-        >  If one or more backend servers specified by the *BackendServers** parameter do not exist in the specified vServer group, these backend servers are ignored and no error message is returned.
-        
-        @param request: RemoveVServerGroupBackendServersRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: RemoveVServerGroupBackendServersResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.backend_servers):
             query['BackendServers'] = request.backend_servers
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -8020,21 +6505,14 @@
         )
 
     async def remove_vserver_group_backend_servers_with_options_async(
         self,
         request: slb_20140515_models.RemoveVServerGroupBackendServersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.RemoveVServerGroupBackendServersResponse:
-        """
-        >  If one or more backend servers specified by the *BackendServers** parameter do not exist in the specified vServer group, these backend servers are ignored and no error message is returned.
-        
-        @param request: RemoveVServerGroupBackendServersRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: RemoveVServerGroupBackendServersResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.backend_servers):
             query['BackendServers'] = request.backend_servers
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -8066,33 +6544,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def remove_vserver_group_backend_servers(
         self,
         request: slb_20140515_models.RemoveVServerGroupBackendServersRequest,
     ) -> slb_20140515_models.RemoveVServerGroupBackendServersResponse:
-        """
-        >  If one or more backend servers specified by the *BackendServers** parameter do not exist in the specified vServer group, these backend servers are ignored and no error message is returned.
-        
-        @param request: RemoveVServerGroupBackendServersRequest
-        @return: RemoveVServerGroupBackendServersResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.remove_vserver_group_backend_servers_with_options(request, runtime)
 
     async def remove_vserver_group_backend_servers_async(
         self,
         request: slb_20140515_models.RemoveVServerGroupBackendServersRequest,
     ) -> slb_20140515_models.RemoveVServerGroupBackendServersResponse:
-        """
-        >  If one or more backend servers specified by the *BackendServers** parameter do not exist in the specified vServer group, these backend servers are ignored and no error message is returned.
-        
-        @param request: RemoveVServerGroupBackendServersRequest
-        @return: RemoveVServerGroupBackendServersResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.remove_vserver_group_backend_servers_with_options_async(request, runtime)
 
     def set_access_control_list_attribute_with_options(
         self,
         request: slb_20140515_models.SetAccessControlListAttributeRequest,
         runtime: util_models.RuntimeOptions,
@@ -8182,112 +6648,14 @@
     async def set_access_control_list_attribute_async(
         self,
         request: slb_20140515_models.SetAccessControlListAttributeRequest,
     ) -> slb_20140515_models.SetAccessControlListAttributeResponse:
         runtime = util_models.RuntimeOptions()
         return await self.set_access_control_list_attribute_with_options_async(request, runtime)
 
-    def set_access_logs_download_attribute_with_options(
-        self,
-        request: slb_20140515_models.SetAccessLogsDownloadAttributeRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> slb_20140515_models.SetAccessLogsDownloadAttributeResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.load_balancer_id):
-            query['LoadBalancerId'] = request.load_balancer_id
-        if not UtilClient.is_unset(request.logs_download_attributes):
-            query['LogsDownloadAttributes'] = request.logs_download_attributes
-        if not UtilClient.is_unset(request.owner_account):
-            query['OwnerAccount'] = request.owner_account
-        if not UtilClient.is_unset(request.owner_id):
-            query['OwnerId'] = request.owner_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.resource_owner_account):
-            query['ResourceOwnerAccount'] = request.resource_owner_account
-        if not UtilClient.is_unset(request.resource_owner_id):
-            query['ResourceOwnerId'] = request.resource_owner_id
-        if not UtilClient.is_unset(request.tags):
-            query['Tags'] = request.tags
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='SetAccessLogsDownloadAttribute',
-            version='2014-05-15',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            slb_20140515_models.SetAccessLogsDownloadAttributeResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def set_access_logs_download_attribute_with_options_async(
-        self,
-        request: slb_20140515_models.SetAccessLogsDownloadAttributeRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> slb_20140515_models.SetAccessLogsDownloadAttributeResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.load_balancer_id):
-            query['LoadBalancerId'] = request.load_balancer_id
-        if not UtilClient.is_unset(request.logs_download_attributes):
-            query['LogsDownloadAttributes'] = request.logs_download_attributes
-        if not UtilClient.is_unset(request.owner_account):
-            query['OwnerAccount'] = request.owner_account
-        if not UtilClient.is_unset(request.owner_id):
-            query['OwnerId'] = request.owner_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.resource_owner_account):
-            query['ResourceOwnerAccount'] = request.resource_owner_account
-        if not UtilClient.is_unset(request.resource_owner_id):
-            query['ResourceOwnerId'] = request.resource_owner_id
-        if not UtilClient.is_unset(request.tags):
-            query['Tags'] = request.tags
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='SetAccessLogsDownloadAttribute',
-            version='2014-05-15',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            slb_20140515_models.SetAccessLogsDownloadAttributeResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def set_access_logs_download_attribute(
-        self,
-        request: slb_20140515_models.SetAccessLogsDownloadAttributeRequest,
-    ) -> slb_20140515_models.SetAccessLogsDownloadAttributeResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.set_access_logs_download_attribute_with_options(request, runtime)
-
-    async def set_access_logs_download_attribute_async(
-        self,
-        request: slb_20140515_models.SetAccessLogsDownloadAttributeRequest,
-    ) -> slb_20140515_models.SetAccessLogsDownloadAttributeResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.set_access_logs_download_attribute_with_options_async(request, runtime)
-
     def set_backend_servers_with_options(
         self,
         request: slb_20140515_models.SetBackendServersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.SetBackendServersResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -8473,21 +6841,14 @@
         return await self.set_cacertificate_name_with_options_async(request, runtime)
 
     def set_domain_extension_attribute_with_options(
         self,
         request: slb_20140515_models.SetDomainExtensionAttributeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.SetDomainExtensionAttributeResponse:
-        """
-        >  You cannot replace an additional certificate for a listener that is added to a shared-resource Server Load Balancer (SLB) instance.
-        
-        @param request: SetDomainExtensionAttributeRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: SetDomainExtensionAttributeResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain_extension_id):
             query['DomainExtensionId'] = request.domain_extension_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -8520,21 +6881,14 @@
         )
 
     async def set_domain_extension_attribute_with_options_async(
         self,
         request: slb_20140515_models.SetDomainExtensionAttributeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.SetDomainExtensionAttributeResponse:
-        """
-        >  You cannot replace an additional certificate for a listener that is added to a shared-resource Server Load Balancer (SLB) instance.
-        
-        @param request: SetDomainExtensionAttributeRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: SetDomainExtensionAttributeResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain_extension_id):
             query['DomainExtensionId'] = request.domain_extension_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -8566,33 +6920,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def set_domain_extension_attribute(
         self,
         request: slb_20140515_models.SetDomainExtensionAttributeRequest,
     ) -> slb_20140515_models.SetDomainExtensionAttributeResponse:
-        """
-        >  You cannot replace an additional certificate for a listener that is added to a shared-resource Server Load Balancer (SLB) instance.
-        
-        @param request: SetDomainExtensionAttributeRequest
-        @return: SetDomainExtensionAttributeResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.set_domain_extension_attribute_with_options(request, runtime)
 
     async def set_domain_extension_attribute_async(
         self,
         request: slb_20140515_models.SetDomainExtensionAttributeRequest,
     ) -> slb_20140515_models.SetDomainExtensionAttributeResponse:
-        """
-        >  You cannot replace an additional certificate for a listener that is added to a shared-resource Server Load Balancer (SLB) instance.
-        
-        @param request: SetDomainExtensionAttributeRequest
-        @return: SetDomainExtensionAttributeResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.set_domain_extension_attribute_with_options_async(request, runtime)
 
     def set_listener_access_control_status_with_options(
         self,
         request: slb_20140515_models.SetListenerAccessControlStatusRequest,
         runtime: util_models.RuntimeOptions,
@@ -8789,23 +7131,14 @@
         return await self.set_load_balancer_delete_protection_with_options_async(request, runtime)
 
     def set_load_balancer_httplistener_attribute_with_options(
         self,
         request: slb_20140515_models.SetLoadBalancerHTTPListenerAttributeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.SetLoadBalancerHTTPListenerAttributeResponse:
-        """
-        ## Prerequisites
-        *   A Classic Load Balancer (CLB) instance is created. For more information, see [CreateLoadBalancer](~~27577~~).
-        *   An HTTP listener is created. For more information about how to create an HTTP listener, see [CreateLoadBalancerHTTPListener](~~27592~~).
-        
-        @param request: SetLoadBalancerHTTPListenerAttributeRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: SetLoadBalancerHTTPListenerAttributeResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_id):
             query['AclId'] = request.acl_id
         if not UtilClient.is_unset(request.acl_status):
             query['AclStatus'] = request.acl_status
         if not UtilClient.is_unset(request.acl_type):
@@ -8896,23 +7229,14 @@
         )
 
     async def set_load_balancer_httplistener_attribute_with_options_async(
         self,
         request: slb_20140515_models.SetLoadBalancerHTTPListenerAttributeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.SetLoadBalancerHTTPListenerAttributeResponse:
-        """
-        ## Prerequisites
-        *   A Classic Load Balancer (CLB) instance is created. For more information, see [CreateLoadBalancer](~~27577~~).
-        *   An HTTP listener is created. For more information about how to create an HTTP listener, see [CreateLoadBalancerHTTPListener](~~27592~~).
-        
-        @param request: SetLoadBalancerHTTPListenerAttributeRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: SetLoadBalancerHTTPListenerAttributeResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_id):
             query['AclId'] = request.acl_id
         if not UtilClient.is_unset(request.acl_status):
             query['AclStatus'] = request.acl_status
         if not UtilClient.is_unset(request.acl_type):
@@ -9002,54 +7326,29 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def set_load_balancer_httplistener_attribute(
         self,
         request: slb_20140515_models.SetLoadBalancerHTTPListenerAttributeRequest,
     ) -> slb_20140515_models.SetLoadBalancerHTTPListenerAttributeResponse:
-        """
-        ## Prerequisites
-        *   A Classic Load Balancer (CLB) instance is created. For more information, see [CreateLoadBalancer](~~27577~~).
-        *   An HTTP listener is created. For more information about how to create an HTTP listener, see [CreateLoadBalancerHTTPListener](~~27592~~).
-        
-        @param request: SetLoadBalancerHTTPListenerAttributeRequest
-        @return: SetLoadBalancerHTTPListenerAttributeResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.set_load_balancer_httplistener_attribute_with_options(request, runtime)
 
     async def set_load_balancer_httplistener_attribute_async(
         self,
         request: slb_20140515_models.SetLoadBalancerHTTPListenerAttributeRequest,
     ) -> slb_20140515_models.SetLoadBalancerHTTPListenerAttributeResponse:
-        """
-        ## Prerequisites
-        *   A Classic Load Balancer (CLB) instance is created. For more information, see [CreateLoadBalancer](~~27577~~).
-        *   An HTTP listener is created. For more information about how to create an HTTP listener, see [CreateLoadBalancerHTTPListener](~~27592~~).
-        
-        @param request: SetLoadBalancerHTTPListenerAttributeRequest
-        @return: SetLoadBalancerHTTPListenerAttributeResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.set_load_balancer_httplistener_attribute_with_options_async(request, runtime)
 
     def set_load_balancer_httpslistener_attribute_with_options(
         self,
         request: slb_20140515_models.SetLoadBalancerHTTPSListenerAttributeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.SetLoadBalancerHTTPSListenerAttributeResponse:
-        """
-        ## Prerequisites
-        *   A Classic Load Balancer (CLB) instance is created. For more information, see [CreateLoadBalancer](~~27577~~).
-        *   An HTTPS listener is created. For more information about how to create an HTTPS listener, see [CreateLoadBalancerHTTPSListener](~~27593~~).
-        
-        @param request: SetLoadBalancerHTTPSListenerAttributeRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: SetLoadBalancerHTTPSListenerAttributeResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_id):
             query['AclId'] = request.acl_id
         if not UtilClient.is_unset(request.acl_status):
             query['AclStatus'] = request.acl_status
         if not UtilClient.is_unset(request.acl_type):
@@ -9148,23 +7447,14 @@
         )
 
     async def set_load_balancer_httpslistener_attribute_with_options_async(
         self,
         request: slb_20140515_models.SetLoadBalancerHTTPSListenerAttributeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.SetLoadBalancerHTTPSListenerAttributeResponse:
-        """
-        ## Prerequisites
-        *   A Classic Load Balancer (CLB) instance is created. For more information, see [CreateLoadBalancer](~~27577~~).
-        *   An HTTPS listener is created. For more information about how to create an HTTPS listener, see [CreateLoadBalancerHTTPSListener](~~27593~~).
-        
-        @param request: SetLoadBalancerHTTPSListenerAttributeRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: SetLoadBalancerHTTPSListenerAttributeResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_id):
             query['AclId'] = request.acl_id
         if not UtilClient.is_unset(request.acl_status):
             query['AclStatus'] = request.acl_status
         if not UtilClient.is_unset(request.acl_type):
@@ -9262,37 +7552,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def set_load_balancer_httpslistener_attribute(
         self,
         request: slb_20140515_models.SetLoadBalancerHTTPSListenerAttributeRequest,
     ) -> slb_20140515_models.SetLoadBalancerHTTPSListenerAttributeResponse:
-        """
-        ## Prerequisites
-        *   A Classic Load Balancer (CLB) instance is created. For more information, see [CreateLoadBalancer](~~27577~~).
-        *   An HTTPS listener is created. For more information about how to create an HTTPS listener, see [CreateLoadBalancerHTTPSListener](~~27593~~).
-        
-        @param request: SetLoadBalancerHTTPSListenerAttributeRequest
-        @return: SetLoadBalancerHTTPSListenerAttributeResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.set_load_balancer_httpslistener_attribute_with_options(request, runtime)
 
     async def set_load_balancer_httpslistener_attribute_async(
         self,
         request: slb_20140515_models.SetLoadBalancerHTTPSListenerAttributeRequest,
     ) -> slb_20140515_models.SetLoadBalancerHTTPSListenerAttributeResponse:
-        """
-        ## Prerequisites
-        *   A Classic Load Balancer (CLB) instance is created. For more information, see [CreateLoadBalancer](~~27577~~).
-        *   An HTTPS listener is created. For more information about how to create an HTTPS listener, see [CreateLoadBalancerHTTPSListener](~~27593~~).
-        
-        @param request: SetLoadBalancerHTTPSListenerAttributeRequest
-        @return: SetLoadBalancerHTTPSListenerAttributeResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.set_load_balancer_httpslistener_attribute_with_options_async(request, runtime)
 
     def set_load_balancer_modification_protection_with_options(
         self,
         request: slb_20140515_models.SetLoadBalancerModificationProtectionRequest,
         runtime: util_models.RuntimeOptions,
@@ -9579,23 +7853,14 @@
         return await self.set_load_balancer_status_with_options_async(request, runtime)
 
     def set_load_balancer_tcplistener_attribute_with_options(
         self,
         request: slb_20140515_models.SetLoadBalancerTCPListenerAttributeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.SetLoadBalancerTCPListenerAttributeResponse:
-        """
-        ## Prerequisites
-        *   A CLB instance is created. For more information, see [CreateLoadBalancer](~~27577~~).
-        *   A TCP listener is created. For more information, see [CreateLoadBalancerTCPListener](~~27594~~).
-        
-        @param request: SetLoadBalancerTCPListenerAttributeRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: SetLoadBalancerTCPListenerAttributeResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_id):
             query['AclId'] = request.acl_id
         if not UtilClient.is_unset(request.acl_status):
             query['AclStatus'] = request.acl_status
         if not UtilClient.is_unset(request.acl_type):
@@ -9616,16 +7881,14 @@
             query['HealthCheckConnectTimeout'] = request.health_check_connect_timeout
         if not UtilClient.is_unset(request.health_check_domain):
             query['HealthCheckDomain'] = request.health_check_domain
         if not UtilClient.is_unset(request.health_check_http_code):
             query['HealthCheckHttpCode'] = request.health_check_http_code
         if not UtilClient.is_unset(request.health_check_interval):
             query['HealthCheckInterval'] = request.health_check_interval
-        if not UtilClient.is_unset(request.health_check_switch):
-            query['HealthCheckSwitch'] = request.health_check_switch
         if not UtilClient.is_unset(request.health_check_type):
             query['HealthCheckType'] = request.health_check_type
         if not UtilClient.is_unset(request.health_check_uri):
             query['HealthCheckURI'] = request.health_check_uri
         if not UtilClient.is_unset(request.healthy_threshold):
             query['HealthyThreshold'] = request.healthy_threshold
         if not UtilClient.is_unset(request.listener_port):
@@ -9638,16 +7901,14 @@
             query['MasterSlaveServerGroupId'] = request.master_slave_server_group_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.persistence_timeout):
             query['PersistenceTimeout'] = request.persistence_timeout
-        if not UtilClient.is_unset(request.proxy_protocol_v2enabled):
-            query['ProxyProtocolV2Enabled'] = request.proxy_protocol_v2enabled
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
             query['ResourceOwnerId'] = request.resource_owner_id
         if not UtilClient.is_unset(request.scheduler):
@@ -9680,23 +7941,14 @@
         )
 
     async def set_load_balancer_tcplistener_attribute_with_options_async(
         self,
         request: slb_20140515_models.SetLoadBalancerTCPListenerAttributeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.SetLoadBalancerTCPListenerAttributeResponse:
-        """
-        ## Prerequisites
-        *   A CLB instance is created. For more information, see [CreateLoadBalancer](~~27577~~).
-        *   A TCP listener is created. For more information, see [CreateLoadBalancerTCPListener](~~27594~~).
-        
-        @param request: SetLoadBalancerTCPListenerAttributeRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: SetLoadBalancerTCPListenerAttributeResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_id):
             query['AclId'] = request.acl_id
         if not UtilClient.is_unset(request.acl_status):
             query['AclStatus'] = request.acl_status
         if not UtilClient.is_unset(request.acl_type):
@@ -9717,16 +7969,14 @@
             query['HealthCheckConnectTimeout'] = request.health_check_connect_timeout
         if not UtilClient.is_unset(request.health_check_domain):
             query['HealthCheckDomain'] = request.health_check_domain
         if not UtilClient.is_unset(request.health_check_http_code):
             query['HealthCheckHttpCode'] = request.health_check_http_code
         if not UtilClient.is_unset(request.health_check_interval):
             query['HealthCheckInterval'] = request.health_check_interval
-        if not UtilClient.is_unset(request.health_check_switch):
-            query['HealthCheckSwitch'] = request.health_check_switch
         if not UtilClient.is_unset(request.health_check_type):
             query['HealthCheckType'] = request.health_check_type
         if not UtilClient.is_unset(request.health_check_uri):
             query['HealthCheckURI'] = request.health_check_uri
         if not UtilClient.is_unset(request.healthy_threshold):
             query['HealthyThreshold'] = request.healthy_threshold
         if not UtilClient.is_unset(request.listener_port):
@@ -9739,16 +7989,14 @@
             query['MasterSlaveServerGroupId'] = request.master_slave_server_group_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.persistence_timeout):
             query['PersistenceTimeout'] = request.persistence_timeout
-        if not UtilClient.is_unset(request.proxy_protocol_v2enabled):
-            query['ProxyProtocolV2Enabled'] = request.proxy_protocol_v2enabled
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
             query['ResourceOwnerId'] = request.resource_owner_id
         if not UtilClient.is_unset(request.scheduler):
@@ -9780,54 +8028,29 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def set_load_balancer_tcplistener_attribute(
         self,
         request: slb_20140515_models.SetLoadBalancerTCPListenerAttributeRequest,
     ) -> slb_20140515_models.SetLoadBalancerTCPListenerAttributeResponse:
-        """
-        ## Prerequisites
-        *   A CLB instance is created. For more information, see [CreateLoadBalancer](~~27577~~).
-        *   A TCP listener is created. For more information, see [CreateLoadBalancerTCPListener](~~27594~~).
-        
-        @param request: SetLoadBalancerTCPListenerAttributeRequest
-        @return: SetLoadBalancerTCPListenerAttributeResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.set_load_balancer_tcplistener_attribute_with_options(request, runtime)
 
     async def set_load_balancer_tcplistener_attribute_async(
         self,
         request: slb_20140515_models.SetLoadBalancerTCPListenerAttributeRequest,
     ) -> slb_20140515_models.SetLoadBalancerTCPListenerAttributeResponse:
-        """
-        ## Prerequisites
-        *   A CLB instance is created. For more information, see [CreateLoadBalancer](~~27577~~).
-        *   A TCP listener is created. For more information, see [CreateLoadBalancerTCPListener](~~27594~~).
-        
-        @param request: SetLoadBalancerTCPListenerAttributeRequest
-        @return: SetLoadBalancerTCPListenerAttributeResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.set_load_balancer_tcplistener_attribute_with_options_async(request, runtime)
 
     def set_load_balancer_udplistener_attribute_with_options(
         self,
         request: slb_20140515_models.SetLoadBalancerUDPListenerAttributeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.SetLoadBalancerUDPListenerAttributeResponse:
-        """
-        ## Prerequisites
-        *   A Classic Load Balancer (CLB) instance is created. For more information, see [CreateLoadBalancer](~~27577~~).
-        *   A UDP listener is created. For more information, see [CreateLoadBalancerUDPListener](~~27595~~).
-        
-        @param request: SetLoadBalancerUDPListenerAttributeRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: SetLoadBalancerUDPListenerAttributeResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_id):
             query['AclId'] = request.acl_id
         if not UtilClient.is_unset(request.acl_status):
             query['AclStatus'] = request.acl_status
         if not UtilClient.is_unset(request.acl_type):
@@ -9838,32 +8061,28 @@
             query['Description'] = request.description
         if not UtilClient.is_unset(request.health_check_connect_port):
             query['HealthCheckConnectPort'] = request.health_check_connect_port
         if not UtilClient.is_unset(request.health_check_connect_timeout):
             query['HealthCheckConnectTimeout'] = request.health_check_connect_timeout
         if not UtilClient.is_unset(request.health_check_interval):
             query['HealthCheckInterval'] = request.health_check_interval
-        if not UtilClient.is_unset(request.health_check_switch):
-            query['HealthCheckSwitch'] = request.health_check_switch
         if not UtilClient.is_unset(request.healthy_threshold):
             query['HealthyThreshold'] = request.healthy_threshold
         if not UtilClient.is_unset(request.listener_port):
             query['ListenerPort'] = request.listener_port
         if not UtilClient.is_unset(request.load_balancer_id):
             query['LoadBalancerId'] = request.load_balancer_id
         if not UtilClient.is_unset(request.master_slave_server_group):
             query['MasterSlaveServerGroup'] = request.master_slave_server_group
         if not UtilClient.is_unset(request.master_slave_server_group_id):
             query['MasterSlaveServerGroupId'] = request.master_slave_server_group_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
-        if not UtilClient.is_unset(request.proxy_protocol_v2enabled):
-            query['ProxyProtocolV2Enabled'] = request.proxy_protocol_v2enabled
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
             query['ResourceOwnerId'] = request.resource_owner_id
         if not UtilClient.is_unset(request.scheduler):
@@ -9898,23 +8117,14 @@
         )
 
     async def set_load_balancer_udplistener_attribute_with_options_async(
         self,
         request: slb_20140515_models.SetLoadBalancerUDPListenerAttributeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.SetLoadBalancerUDPListenerAttributeResponse:
-        """
-        ## Prerequisites
-        *   A Classic Load Balancer (CLB) instance is created. For more information, see [CreateLoadBalancer](~~27577~~).
-        *   A UDP listener is created. For more information, see [CreateLoadBalancerUDPListener](~~27595~~).
-        
-        @param request: SetLoadBalancerUDPListenerAttributeRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: SetLoadBalancerUDPListenerAttributeResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_id):
             query['AclId'] = request.acl_id
         if not UtilClient.is_unset(request.acl_status):
             query['AclStatus'] = request.acl_status
         if not UtilClient.is_unset(request.acl_type):
@@ -9925,32 +8135,28 @@
             query['Description'] = request.description
         if not UtilClient.is_unset(request.health_check_connect_port):
             query['HealthCheckConnectPort'] = request.health_check_connect_port
         if not UtilClient.is_unset(request.health_check_connect_timeout):
             query['HealthCheckConnectTimeout'] = request.health_check_connect_timeout
         if not UtilClient.is_unset(request.health_check_interval):
             query['HealthCheckInterval'] = request.health_check_interval
-        if not UtilClient.is_unset(request.health_check_switch):
-            query['HealthCheckSwitch'] = request.health_check_switch
         if not UtilClient.is_unset(request.healthy_threshold):
             query['HealthyThreshold'] = request.healthy_threshold
         if not UtilClient.is_unset(request.listener_port):
             query['ListenerPort'] = request.listener_port
         if not UtilClient.is_unset(request.load_balancer_id):
             query['LoadBalancerId'] = request.load_balancer_id
         if not UtilClient.is_unset(request.master_slave_server_group):
             query['MasterSlaveServerGroup'] = request.master_slave_server_group
         if not UtilClient.is_unset(request.master_slave_server_group_id):
             query['MasterSlaveServerGroupId'] = request.master_slave_server_group_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
-        if not UtilClient.is_unset(request.proxy_protocol_v2enabled):
-            query['ProxyProtocolV2Enabled'] = request.proxy_protocol_v2enabled
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
             query['ResourceOwnerId'] = request.resource_owner_id
         if not UtilClient.is_unset(request.scheduler):
@@ -9984,37 +8190,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def set_load_balancer_udplistener_attribute(
         self,
         request: slb_20140515_models.SetLoadBalancerUDPListenerAttributeRequest,
     ) -> slb_20140515_models.SetLoadBalancerUDPListenerAttributeResponse:
-        """
-        ## Prerequisites
-        *   A Classic Load Balancer (CLB) instance is created. For more information, see [CreateLoadBalancer](~~27577~~).
-        *   A UDP listener is created. For more information, see [CreateLoadBalancerUDPListener](~~27595~~).
-        
-        @param request: SetLoadBalancerUDPListenerAttributeRequest
-        @return: SetLoadBalancerUDPListenerAttributeResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.set_load_balancer_udplistener_attribute_with_options(request, runtime)
 
     async def set_load_balancer_udplistener_attribute_async(
         self,
         request: slb_20140515_models.SetLoadBalancerUDPListenerAttributeRequest,
     ) -> slb_20140515_models.SetLoadBalancerUDPListenerAttributeResponse:
-        """
-        ## Prerequisites
-        *   A Classic Load Balancer (CLB) instance is created. For more information, see [CreateLoadBalancer](~~27577~~).
-        *   A UDP listener is created. For more information, see [CreateLoadBalancerUDPListener](~~27595~~).
-        
-        @param request: SetLoadBalancerUDPListenerAttributeRequest
-        @return: SetLoadBalancerUDPListenerAttributeResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.set_load_balancer_udplistener_attribute_with_options_async(request, runtime)
 
     def set_rule_with_options(
         self,
         request: slb_20140515_models.SetRuleRequest,
         runtime: util_models.RuntimeOptions,
@@ -10287,14 +8477,16 @@
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
             query['ResourceOwnerId'] = request.resource_owner_id
         if not UtilClient.is_unset(request.tlscipher_policy_id):
             query['TLSCipherPolicyId'] = request.tlscipher_policy_id
         if not UtilClient.is_unset(request.tlsversions):
             query['TLSVersions'] = request.tlsversions
+        if not UtilClient.is_unset(request.access_key_id):
+            query['access_key_id'] = request.access_key_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='SetTLSCipherPolicyAttribute',
             version='2014-05-15',
             protocol='HTTPS',
@@ -10331,14 +8523,16 @@
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
             query['ResourceOwnerId'] = request.resource_owner_id
         if not UtilClient.is_unset(request.tlscipher_policy_id):
             query['TLSCipherPolicyId'] = request.tlscipher_policy_id
         if not UtilClient.is_unset(request.tlsversions):
             query['TLSVersions'] = request.tlsversions
+        if not UtilClient.is_unset(request.access_key_id):
+            query['access_key_id'] = request.access_key_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='SetTLSCipherPolicyAttribute',
             version='2014-05-15',
             protocol='HTTPS',
@@ -10369,23 +8563,14 @@
         return await self.set_tlscipher_policy_attribute_with_options_async(request, runtime)
 
     def set_vserver_group_attribute_with_options(
         self,
         request: slb_20140515_models.SetVServerGroupAttributeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.SetVServerGroupAttributeResponse:
-        """
-        This operation allows you to modify only the name of a vServer group and the weights of the backend servers in the vServer group.
-        *   If you want to modify backend servers in a specified vServer group, call the [ModifyVServerGroupBackendServers](~~35220~~) operation.
-        *   If you want to add backend servers to a specified vServer group, call the [AddVServerGroupBackendServers](~~35218~~) operation.
-        
-        @param request: SetVServerGroupAttributeRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: SetVServerGroupAttributeResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.backend_servers):
             query['BackendServers'] = request.backend_servers
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -10420,23 +8605,14 @@
         )
 
     async def set_vserver_group_attribute_with_options_async(
         self,
         request: slb_20140515_models.SetVServerGroupAttributeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.SetVServerGroupAttributeResponse:
-        """
-        This operation allows you to modify only the name of a vServer group and the weights of the backend servers in the vServer group.
-        *   If you want to modify backend servers in a specified vServer group, call the [ModifyVServerGroupBackendServers](~~35220~~) operation.
-        *   If you want to add backend servers to a specified vServer group, call the [AddVServerGroupBackendServers](~~35218~~) operation.
-        
-        @param request: SetVServerGroupAttributeRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: SetVServerGroupAttributeResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.backend_servers):
             query['BackendServers'] = request.backend_servers
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -10470,55 +8646,29 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def set_vserver_group_attribute(
         self,
         request: slb_20140515_models.SetVServerGroupAttributeRequest,
     ) -> slb_20140515_models.SetVServerGroupAttributeResponse:
-        """
-        This operation allows you to modify only the name of a vServer group and the weights of the backend servers in the vServer group.
-        *   If you want to modify backend servers in a specified vServer group, call the [ModifyVServerGroupBackendServers](~~35220~~) operation.
-        *   If you want to add backend servers to a specified vServer group, call the [AddVServerGroupBackendServers](~~35218~~) operation.
-        
-        @param request: SetVServerGroupAttributeRequest
-        @return: SetVServerGroupAttributeResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.set_vserver_group_attribute_with_options(request, runtime)
 
     async def set_vserver_group_attribute_async(
         self,
         request: slb_20140515_models.SetVServerGroupAttributeRequest,
     ) -> slb_20140515_models.SetVServerGroupAttributeResponse:
-        """
-        This operation allows you to modify only the name of a vServer group and the weights of the backend servers in the vServer group.
-        *   If you want to modify backend servers in a specified vServer group, call the [ModifyVServerGroupBackendServers](~~35220~~) operation.
-        *   If you want to add backend servers to a specified vServer group, call the [AddVServerGroupBackendServers](~~35218~~) operation.
-        
-        @param request: SetVServerGroupAttributeRequest
-        @return: SetVServerGroupAttributeResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.set_vserver_group_attribute_with_options_async(request, runtime)
 
     def start_load_balancer_listener_with_options(
         self,
         request: slb_20140515_models.StartLoadBalancerListenerRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.StartLoadBalancerListenerResponse:
-        """
-        When you call this operation, note the following items:
-        *   You can call the operation only when the listener is in the Stopped state.
-        *   After the operation is called, the status of the listener changes to Starting.
-        *   You cannot call this operation when the SLB instance to which the listener is bound is in the Locked state.
-        
-        @param request: StartLoadBalancerListenerRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: StartLoadBalancerListenerResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.listener_port):
             query['ListenerPort'] = request.listener_port
         if not UtilClient.is_unset(request.listener_protocol):
             query['ListenerProtocol'] = request.listener_protocol
         if not UtilClient.is_unset(request.load_balancer_id):
@@ -10553,24 +8703,14 @@
         )
 
     async def start_load_balancer_listener_with_options_async(
         self,
         request: slb_20140515_models.StartLoadBalancerListenerRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.StartLoadBalancerListenerResponse:
-        """
-        When you call this operation, note the following items:
-        *   You can call the operation only when the listener is in the Stopped state.
-        *   After the operation is called, the status of the listener changes to Starting.
-        *   You cannot call this operation when the SLB instance to which the listener is bound is in the Locked state.
-        
-        @param request: StartLoadBalancerListenerRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: StartLoadBalancerListenerResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.listener_port):
             query['ListenerPort'] = request.listener_port
         if not UtilClient.is_unset(request.listener_protocol):
             query['ListenerProtocol'] = request.listener_protocol
         if not UtilClient.is_unset(request.load_balancer_id):
@@ -10604,57 +8744,29 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def start_load_balancer_listener(
         self,
         request: slb_20140515_models.StartLoadBalancerListenerRequest,
     ) -> slb_20140515_models.StartLoadBalancerListenerResponse:
-        """
-        When you call this operation, note the following items:
-        *   You can call the operation only when the listener is in the Stopped state.
-        *   After the operation is called, the status of the listener changes to Starting.
-        *   You cannot call this operation when the SLB instance to which the listener is bound is in the Locked state.
-        
-        @param request: StartLoadBalancerListenerRequest
-        @return: StartLoadBalancerListenerResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.start_load_balancer_listener_with_options(request, runtime)
 
     async def start_load_balancer_listener_async(
         self,
         request: slb_20140515_models.StartLoadBalancerListenerRequest,
     ) -> slb_20140515_models.StartLoadBalancerListenerResponse:
-        """
-        When you call this operation, note the following items:
-        *   You can call the operation only when the listener is in the Stopped state.
-        *   After the operation is called, the status of the listener changes to Starting.
-        *   You cannot call this operation when the SLB instance to which the listener is bound is in the Locked state.
-        
-        @param request: StartLoadBalancerListenerRequest
-        @return: StartLoadBalancerListenerResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.start_load_balancer_listener_with_options_async(request, runtime)
 
     def stop_load_balancer_listener_with_options(
         self,
         request: slb_20140515_models.StopLoadBalancerListenerRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.StopLoadBalancerListenerResponse:
-        """
-        Before you make this API call, note the following:
-        *   After the API call is successfully made, the listener enters the stopped state.
-        *   If the Server Load Balancer (SLB) instance to which the listener to be stopped belongs is in the locked state, this API call cannot be made.
-        >  If you stop the listener, your services will be disrupted. Exercise caution when you perform this action.
-        
-        @param request: StopLoadBalancerListenerRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: StopLoadBalancerListenerResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.listener_port):
             query['ListenerPort'] = request.listener_port
         if not UtilClient.is_unset(request.listener_protocol):
             query['ListenerProtocol'] = request.listener_protocol
         if not UtilClient.is_unset(request.load_balancer_id):
@@ -10689,24 +8801,14 @@
         )
 
     async def stop_load_balancer_listener_with_options_async(
         self,
         request: slb_20140515_models.StopLoadBalancerListenerRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.StopLoadBalancerListenerResponse:
-        """
-        Before you make this API call, note the following:
-        *   After the API call is successfully made, the listener enters the stopped state.
-        *   If the Server Load Balancer (SLB) instance to which the listener to be stopped belongs is in the locked state, this API call cannot be made.
-        >  If you stop the listener, your services will be disrupted. Exercise caution when you perform this action.
-        
-        @param request: StopLoadBalancerListenerRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: StopLoadBalancerListenerResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.listener_port):
             query['ListenerPort'] = request.listener_port
         if not UtilClient.is_unset(request.listener_protocol):
             query['ListenerProtocol'] = request.listener_protocol
         if not UtilClient.is_unset(request.load_balancer_id):
@@ -10740,54 +8842,29 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def stop_load_balancer_listener(
         self,
         request: slb_20140515_models.StopLoadBalancerListenerRequest,
     ) -> slb_20140515_models.StopLoadBalancerListenerResponse:
-        """
-        Before you make this API call, note the following:
-        *   After the API call is successfully made, the listener enters the stopped state.
-        *   If the Server Load Balancer (SLB) instance to which the listener to be stopped belongs is in the locked state, this API call cannot be made.
-        >  If you stop the listener, your services will be disrupted. Exercise caution when you perform this action.
-        
-        @param request: StopLoadBalancerListenerRequest
-        @return: StopLoadBalancerListenerResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.stop_load_balancer_listener_with_options(request, runtime)
 
     async def stop_load_balancer_listener_async(
         self,
         request: slb_20140515_models.StopLoadBalancerListenerRequest,
     ) -> slb_20140515_models.StopLoadBalancerListenerResponse:
-        """
-        Before you make this API call, note the following:
-        *   After the API call is successfully made, the listener enters the stopped state.
-        *   If the Server Load Balancer (SLB) instance to which the listener to be stopped belongs is in the locked state, this API call cannot be made.
-        >  If you stop the listener, your services will be disrupted. Exercise caution when you perform this action.
-        
-        @param request: StopLoadBalancerListenerRequest
-        @return: StopLoadBalancerListenerResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.stop_load_balancer_listener_with_options_async(request, runtime)
 
     def tag_resources_with_options(
         self,
         request: slb_20140515_models.TagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.TagResourcesResponse:
-        """
-        >  You can add at most 20 tags to each instance. Before you add tags to a resource, Alibaba Cloud checks the number of existing tags of the resource. If the maximum number is reached, an error message is returned.
-        
-        @param request: TagResourcesRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: TagResourcesResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.region_id):
@@ -10822,21 +8899,14 @@
         )
 
     async def tag_resources_with_options_async(
         self,
         request: slb_20140515_models.TagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.TagResourcesResponse:
-        """
-        >  You can add at most 20 tags to each instance. Before you add tags to a resource, Alibaba Cloud checks the number of existing tags of the resource. If the maximum number is reached, an error message is returned.
-        
-        @param request: TagResourcesRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: TagResourcesResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.region_id):
@@ -10870,33 +8940,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def tag_resources(
         self,
         request: slb_20140515_models.TagResourcesRequest,
     ) -> slb_20140515_models.TagResourcesResponse:
-        """
-        >  You can add at most 20 tags to each instance. Before you add tags to a resource, Alibaba Cloud checks the number of existing tags of the resource. If the maximum number is reached, an error message is returned.
-        
-        @param request: TagResourcesRequest
-        @return: TagResourcesResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.tag_resources_with_options(request, runtime)
 
     async def tag_resources_async(
         self,
         request: slb_20140515_models.TagResourcesRequest,
     ) -> slb_20140515_models.TagResourcesResponse:
-        """
-        >  You can add at most 20 tags to each instance. Before you add tags to a resource, Alibaba Cloud checks the number of existing tags of the resource. If the maximum number is reached, an error message is returned.
-        
-        @param request: TagResourcesRequest
-        @return: TagResourcesResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.tag_resources_with_options_async(request, runtime)
 
     def untag_resources_with_options(
         self,
         request: slb_20140515_models.UntagResourcesRequest,
         runtime: util_models.RuntimeOptions,
@@ -10999,21 +9057,14 @@
         return await self.untag_resources_with_options_async(request, runtime)
 
     def upload_cacertificate_with_options(
         self,
         request: slb_20140515_models.UploadCACertificateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.UploadCACertificateResponse:
-        """
-        You can upload only one CA certificate at a time. After a CA certificate is uploaded, the certificate ID, name, and fingerprint are returned.
-        
-        @param request: UploadCACertificateRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: UploadCACertificateResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.cacertificate):
             query['CACertificate'] = request.cacertificate
         if not UtilClient.is_unset(request.cacertificate_name):
             query['CACertificateName'] = request.cacertificate_name
         if not UtilClient.is_unset(request.owner_account):
@@ -11048,21 +9099,14 @@
         )
 
     async def upload_cacertificate_with_options_async(
         self,
         request: slb_20140515_models.UploadCACertificateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.UploadCACertificateResponse:
-        """
-        You can upload only one CA certificate at a time. After a CA certificate is uploaded, the certificate ID, name, and fingerprint are returned.
-        
-        @param request: UploadCACertificateRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: UploadCACertificateResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.cacertificate):
             query['CACertificate'] = request.cacertificate
         if not UtilClient.is_unset(request.cacertificate_name):
             query['CACertificateName'] = request.cacertificate_name
         if not UtilClient.is_unset(request.owner_account):
@@ -11096,50 +9140,29 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def upload_cacertificate(
         self,
         request: slb_20140515_models.UploadCACertificateRequest,
     ) -> slb_20140515_models.UploadCACertificateResponse:
-        """
-        You can upload only one CA certificate at a time. After a CA certificate is uploaded, the certificate ID, name, and fingerprint are returned.
-        
-        @param request: UploadCACertificateRequest
-        @return: UploadCACertificateResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.upload_cacertificate_with_options(request, runtime)
 
     async def upload_cacertificate_async(
         self,
         request: slb_20140515_models.UploadCACertificateRequest,
     ) -> slb_20140515_models.UploadCACertificateResponse:
-        """
-        You can upload only one CA certificate at a time. After a CA certificate is uploaded, the certificate ID, name, and fingerprint are returned.
-        
-        @param request: UploadCACertificateRequest
-        @return: UploadCACertificateResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.upload_cacertificate_with_options_async(request, runtime)
 
     def upload_server_certificate_with_options(
         self,
         request: slb_20140515_models.UploadServerCertificateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.UploadServerCertificateResponse:
-        """
-        ## Description
-        *   You can upload only one server certificate and its private key in each request.
-        *   After a server certificate and its private key are uploaded, the fingerprints of all server certificates that belong to your account are returned.
-        
-        @param request: UploadServerCertificateRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: UploadServerCertificateResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.ali_cloud_certificate_id):
             query['AliCloudCertificateId'] = request.ali_cloud_certificate_id
         if not UtilClient.is_unset(request.ali_cloud_certificate_name):
             query['AliCloudCertificateName'] = request.ali_cloud_certificate_name
         if not UtilClient.is_unset(request.ali_cloud_certificate_region_id):
@@ -11182,23 +9205,14 @@
         )
 
     async def upload_server_certificate_with_options_async(
         self,
         request: slb_20140515_models.UploadServerCertificateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> slb_20140515_models.UploadServerCertificateResponse:
-        """
-        ## Description
-        *   You can upload only one server certificate and its private key in each request.
-        *   After a server certificate and its private key are uploaded, the fingerprints of all server certificates that belong to your account are returned.
-        
-        @param request: UploadServerCertificateRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: UploadServerCertificateResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.ali_cloud_certificate_id):
             query['AliCloudCertificateId'] = request.ali_cloud_certificate_id
         if not UtilClient.is_unset(request.ali_cloud_certificate_name):
             query['AliCloudCertificateName'] = request.ali_cloud_certificate_name
         if not UtilClient.is_unset(request.ali_cloud_certificate_region_id):
@@ -11240,32 +9254,16 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def upload_server_certificate(
         self,
         request: slb_20140515_models.UploadServerCertificateRequest,
     ) -> slb_20140515_models.UploadServerCertificateResponse:
-        """
-        ## Description
-        *   You can upload only one server certificate and its private key in each request.
-        *   After a server certificate and its private key are uploaded, the fingerprints of all server certificates that belong to your account are returned.
-        
-        @param request: UploadServerCertificateRequest
-        @return: UploadServerCertificateResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.upload_server_certificate_with_options(request, runtime)
 
     async def upload_server_certificate_async(
         self,
         request: slb_20140515_models.UploadServerCertificateRequest,
     ) -> slb_20140515_models.UploadServerCertificateResponse:
-        """
-        ## Description
-        *   You can upload only one server certificate and its private key in each request.
-        *   After a server certificate and its private key are uploaded, the fingerprints of all server certificates that belong to your account are returned.
-        
-        @param request: UploadServerCertificateRequest
-        @return: UploadServerCertificateResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.upload_server_certificate_with_options_async(request, runtime)
```

### Comparing `alibabacloud_slb20140515-3.3.19/alibabacloud_slb20140515.egg-info/PKG-INFO` & `alibabacloud_slb20140515-3.3.9/alibabacloud_slb20140515.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-slb20140515
-Version: 3.3.19
+Version: 3.3.9
 Summary: Alibaba Cloud Server Load Balancer (20140515) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_slb20140515-3.3.19/setup.py` & `alibabacloud_slb20140515-3.3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_slb20140515.
 
-Created on 12/04/2023
+Created on 29/12/2021
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_slb20140515"
 NAME = "alibabacloud_slb20140515" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Server Load Balancer (20140515) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.8, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
-    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
+    "alibabacloud_tea_util>=0.3.5, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.1, <1.0.0",
+    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

