# Comparing `tmp/alibabacloud_config20200907-2.2.3.tar.gz` & `tmp/alibabacloud_config20200907-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_config20200907-2.2.3.tar", last modified: Tue Dec 27 03:00:57 2022, max compression
+gzip compressed data, was "dist/alibabacloud_config20200907-2.2.7.tar", last modified: Wed Apr 12 15:13:45 2023, max compression
```

## Comparing `alibabacloud_config20200907-2.2.3.tar` & `alibabacloud_config20200907-2.2.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 03:00:57.000000 alibabacloud_config20200907-2.2.3/
--rw-r--r--   0 root         (0) root         (0)      939 2022-12-27 03:00:57.000000 alibabacloud_config20200907-2.2.3/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-12-27 03:00:57.000000 alibabacloud_config20200907-2.2.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-12-27 03:00:57.000000 alibabacloud_config20200907-2.2.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2351 2022-12-27 03:00:57.000000 alibabacloud_config20200907-2.2.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1031 2022-12-27 03:00:57.000000 alibabacloud_config20200907-2.2.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2022-12-27 03:00:57.000000 alibabacloud_config20200907-2.2.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 03:00:57.000000 alibabacloud_config20200907-2.2.3/alibabacloud_config20200907/
--rw-r--r--   0 root         (0) root         (0)       21 2022-12-27 03:00:57.000000 alibabacloud_config20200907-2.2.3/alibabacloud_config20200907/__init__.py
--rw-r--r--   0 root         (0) root         (0)   398387 2022-12-27 03:00:57.000000 alibabacloud_config20200907-2.2.3/alibabacloud_config20200907/client.py
--rw-r--r--   0 root         (0) root         (0)   861977 2022-12-27 03:00:57.000000 alibabacloud_config20200907-2.2.3/alibabacloud_config20200907/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 03:00:57.000000 alibabacloud_config20200907-2.2.3/alibabacloud_config20200907.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2351 2022-12-27 03:00:57.000000 alibabacloud_config20200907-2.2.3/alibabacloud_config20200907.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      444 2022-12-27 03:00:57.000000 alibabacloud_config20200907-2.2.3/alibabacloud_config20200907.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-27 03:00:57.000000 alibabacloud_config20200907-2.2.3/alibabacloud_config20200907.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-12-27 03:00:57.000000 alibabacloud_config20200907-2.2.3/alibabacloud_config20200907.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2022-12-27 03:00:57.000000 alibabacloud_config20200907-2.2.3/alibabacloud_config20200907.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-12-27 03:00:57.000000 alibabacloud_config20200907-2.2.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2630 2022-12-27 03:00:57.000000 alibabacloud_config20200907-2.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/
+-rw-r--r--   0 root         (0) root         (0)      989 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2351 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/alibabacloud_config20200907/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/alibabacloud_config20200907/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   575945 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/alibabacloud_config20200907/client.py
+-rw-r--r--   0 root         (0) root         (0)  1139150 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/alibabacloud_config20200907/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/alibabacloud_config20200907.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2351 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/alibabacloud_config20200907.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      444 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/alibabacloud_config20200907.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/alibabacloud_config20200907.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/alibabacloud_config20200907.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/alibabacloud_config20200907.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2630 2023-04-12 15:13:45.000000 alibabacloud_config20200907-2.2.7/setup.py
```

### Comparing `alibabacloud_config20200907-2.2.3/ChangeLog.md` & `alibabacloud_config20200907-2.2.7/ChangeLog.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2022-12-27 Version: 2.2.3
+- Open Integrated Api.
+
 2022-11-29 Version: 2.2.2
 - Support ListRemediationExecutions.
 
 2022-11-02 Version: 2.2.1
 - Fix ListManagedRules bugs.
 
 2022-08-12 Version: 2.1.9
```

### Comparing `alibabacloud_config20200907-2.2.3/LICENSE` & `alibabacloud_config20200907-2.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_config20200907-2.2.3/PKG-INFO` & `alibabacloud_config20200907-2.2.7/alibabacloud_config20200907.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_config20200907
-Version: 2.2.3
+Name: alibabacloud-config20200907
+Version: 2.2.7
 Summary: Alibaba Cloud CloudConfig (20200907) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_config20200907-2.2.3/README-CN.md` & `alibabacloud_config20200907-2.2.7/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_config20200907-2.2.3/README.md` & `alibabacloud_config20200907-2.2.7/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_config20200907-2.2.3/alibabacloud_config20200907/client.py` & `alibabacloud_config20200907-2.2.7/alibabacloud_config20200907/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -46,14 +46,21 @@
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
     def active_aggregate_config_rules_with_options(
         self,
         request: config_20200907_models.ActiveAggregateConfigRulesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ActiveAggregateConfigRulesResponse:
+        """
+        The sample request in this topic shows you how to enable the `cr-5772ba41209e007b***` rule in the `ca-a4e5626622af0079****` account group.
+        
+        @param request: ActiveAggregateConfigRulesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ActiveAggregateConfigRulesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.config_rule_ids):
             query['ConfigRuleIds'] = request.config_rule_ids
         req = open_api_models.OpenApiRequest(
@@ -76,14 +83,21 @@
         )
 
     async def active_aggregate_config_rules_with_options_async(
         self,
         request: config_20200907_models.ActiveAggregateConfigRulesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ActiveAggregateConfigRulesResponse:
+        """
+        The sample request in this topic shows you how to enable the `cr-5772ba41209e007b***` rule in the `ca-a4e5626622af0079****` account group.
+        
+        @param request: ActiveAggregateConfigRulesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ActiveAggregateConfigRulesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.config_rule_ids):
             query['ConfigRuleIds'] = request.config_rule_ids
         req = open_api_models.OpenApiRequest(
@@ -105,29 +119,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def active_aggregate_config_rules(
         self,
         request: config_20200907_models.ActiveAggregateConfigRulesRequest,
     ) -> config_20200907_models.ActiveAggregateConfigRulesResponse:
+        """
+        The sample request in this topic shows you how to enable the `cr-5772ba41209e007b***` rule in the `ca-a4e5626622af0079****` account group.
+        
+        @param request: ActiveAggregateConfigRulesRequest
+        @return: ActiveAggregateConfigRulesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.active_aggregate_config_rules_with_options(request, runtime)
 
     async def active_aggregate_config_rules_async(
         self,
         request: config_20200907_models.ActiveAggregateConfigRulesRequest,
     ) -> config_20200907_models.ActiveAggregateConfigRulesResponse:
+        """
+        The sample request in this topic shows you how to enable the `cr-5772ba41209e007b***` rule in the `ca-a4e5626622af0079****` account group.
+        
+        @param request: ActiveAggregateConfigRulesRequest
+        @return: ActiveAggregateConfigRulesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.active_aggregate_config_rules_with_options_async(request, runtime)
 
     def attach_aggregate_config_rule_to_compliance_pack_with_options(
         self,
         request: config_20200907_models.AttachAggregateConfigRuleToCompliancePackRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.AttachAggregateConfigRuleToCompliancePackResponse:
+        """
+        The sample request in this topic shows you how to add the `cr-6cc4626622af00e7***` rule in the `ca-75b4626622af00c3****` account group to the `cp-5bb1626622af00bd****` compliance package.
+        
+        @param request: AttachAggregateConfigRuleToCompliancePackRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: AttachAggregateConfigRuleToCompliancePackResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.compliance_pack_id):
             query['CompliancePackId'] = request.compliance_pack_id
         if not UtilClient.is_unset(request.config_rule_ids):
@@ -152,14 +185,21 @@
         )
 
     async def attach_aggregate_config_rule_to_compliance_pack_with_options_async(
         self,
         request: config_20200907_models.AttachAggregateConfigRuleToCompliancePackRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.AttachAggregateConfigRuleToCompliancePackResponse:
+        """
+        The sample request in this topic shows you how to add the `cr-6cc4626622af00e7***` rule in the `ca-75b4626622af00c3****` account group to the `cp-5bb1626622af00bd****` compliance package.
+        
+        @param request: AttachAggregateConfigRuleToCompliancePackRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: AttachAggregateConfigRuleToCompliancePackResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.compliance_pack_id):
             query['CompliancePackId'] = request.compliance_pack_id
         if not UtilClient.is_unset(request.config_rule_ids):
@@ -183,29 +223,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def attach_aggregate_config_rule_to_compliance_pack(
         self,
         request: config_20200907_models.AttachAggregateConfigRuleToCompliancePackRequest,
     ) -> config_20200907_models.AttachAggregateConfigRuleToCompliancePackResponse:
+        """
+        The sample request in this topic shows you how to add the `cr-6cc4626622af00e7***` rule in the `ca-75b4626622af00c3****` account group to the `cp-5bb1626622af00bd****` compliance package.
+        
+        @param request: AttachAggregateConfigRuleToCompliancePackRequest
+        @return: AttachAggregateConfigRuleToCompliancePackResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.attach_aggregate_config_rule_to_compliance_pack_with_options(request, runtime)
 
     async def attach_aggregate_config_rule_to_compliance_pack_async(
         self,
         request: config_20200907_models.AttachAggregateConfigRuleToCompliancePackRequest,
     ) -> config_20200907_models.AttachAggregateConfigRuleToCompliancePackResponse:
+        """
+        The sample request in this topic shows you how to add the `cr-6cc4626622af00e7***` rule in the `ca-75b4626622af00c3****` account group to the `cp-5bb1626622af00bd****` compliance package.
+        
+        @param request: AttachAggregateConfigRuleToCompliancePackRequest
+        @return: AttachAggregateConfigRuleToCompliancePackResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.attach_aggregate_config_rule_to_compliance_pack_with_options_async(request, runtime)
 
     def attach_config_rule_to_compliance_pack_with_options(
         self,
         request: config_20200907_models.AttachConfigRuleToCompliancePackRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.AttachConfigRuleToCompliancePackResponse:
+        """
+        The sample request in this topic shows you how to add the `cr-6cc4626622af00e7***` rule to the `cp-5bb1626622af00bd****` compliance package.
+        
+        @param request: AttachConfigRuleToCompliancePackRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: AttachConfigRuleToCompliancePackResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.compliance_pack_id):
             query['CompliancePackId'] = request.compliance_pack_id
         if not UtilClient.is_unset(request.config_rule_ids):
             query['ConfigRuleIds'] = request.config_rule_ids
         req = open_api_models.OpenApiRequest(
@@ -228,14 +287,21 @@
         )
 
     async def attach_config_rule_to_compliance_pack_with_options_async(
         self,
         request: config_20200907_models.AttachConfigRuleToCompliancePackRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.AttachConfigRuleToCompliancePackResponse:
+        """
+        The sample request in this topic shows you how to add the `cr-6cc4626622af00e7***` rule to the `cp-5bb1626622af00bd****` compliance package.
+        
+        @param request: AttachConfigRuleToCompliancePackRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: AttachConfigRuleToCompliancePackResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.compliance_pack_id):
             query['CompliancePackId'] = request.compliance_pack_id
         if not UtilClient.is_unset(request.config_rule_ids):
             query['ConfigRuleIds'] = request.config_rule_ids
         req = open_api_models.OpenApiRequest(
@@ -257,21 +323,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def attach_config_rule_to_compliance_pack(
         self,
         request: config_20200907_models.AttachConfigRuleToCompliancePackRequest,
     ) -> config_20200907_models.AttachConfigRuleToCompliancePackResponse:
+        """
+        The sample request in this topic shows you how to add the `cr-6cc4626622af00e7***` rule to the `cp-5bb1626622af00bd****` compliance package.
+        
+        @param request: AttachConfigRuleToCompliancePackRequest
+        @return: AttachConfigRuleToCompliancePackResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.attach_config_rule_to_compliance_pack_with_options(request, runtime)
 
     async def attach_config_rule_to_compliance_pack_async(
         self,
         request: config_20200907_models.AttachConfigRuleToCompliancePackRequest,
     ) -> config_20200907_models.AttachConfigRuleToCompliancePackResponse:
+        """
+        The sample request in this topic shows you how to add the `cr-6cc4626622af00e7***` rule to the `cp-5bb1626622af00bd****` compliance package.
+        
+        @param request: AttachConfigRuleToCompliancePackRequest
+        @return: AttachConfigRuleToCompliancePackResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.attach_config_rule_to_compliance_pack_with_options_async(request, runtime)
 
     def copy_compliance_packs_with_options(
         self,
         request: config_20200907_models.CopyCompliancePacksRequest,
         runtime: util_models.RuntimeOptions,
@@ -428,14 +506,22 @@
         return await self.copy_config_rules_with_options_async(request, runtime)
 
     def create_aggregate_compliance_pack_with_options(
         self,
         tmp_req: config_20200907_models.CreateAggregateCompliancePackRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.CreateAggregateCompliancePackResponse:
+        """
+        You can use your management account to create up to five compliance packages for each account group.
+        This topic provides an example on how to create a compliance package named ClassifiedProtectionPreCheck for the `ca-f632626622af0079****` account group. The compliance package contains the `eip-bandwidth-limit` managed rule.
+        
+        @param tmp_req: CreateAggregateCompliancePackRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateAggregateCompliancePackResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = config_20200907_models.CreateAggregateCompliancePackShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.config_rules):
             request.config_rules_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.config_rules, 'ConfigRules', 'json')
         body = {}
         if not UtilClient.is_unset(request.aggregator_id):
@@ -484,14 +570,22 @@
         )
 
     async def create_aggregate_compliance_pack_with_options_async(
         self,
         tmp_req: config_20200907_models.CreateAggregateCompliancePackRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.CreateAggregateCompliancePackResponse:
+        """
+        You can use your management account to create up to five compliance packages for each account group.
+        This topic provides an example on how to create a compliance package named ClassifiedProtectionPreCheck for the `ca-f632626622af0079****` account group. The compliance package contains the `eip-bandwidth-limit` managed rule.
+        
+        @param tmp_req: CreateAggregateCompliancePackRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateAggregateCompliancePackResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = config_20200907_models.CreateAggregateCompliancePackShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.config_rules):
             request.config_rules_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.config_rules, 'ConfigRules', 'json')
         body = {}
         if not UtilClient.is_unset(request.aggregator_id):
@@ -539,29 +633,50 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_aggregate_compliance_pack(
         self,
         request: config_20200907_models.CreateAggregateCompliancePackRequest,
     ) -> config_20200907_models.CreateAggregateCompliancePackResponse:
+        """
+        You can use your management account to create up to five compliance packages for each account group.
+        This topic provides an example on how to create a compliance package named ClassifiedProtectionPreCheck for the `ca-f632626622af0079****` account group. The compliance package contains the `eip-bandwidth-limit` managed rule.
+        
+        @param request: CreateAggregateCompliancePackRequest
+        @return: CreateAggregateCompliancePackResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_aggregate_compliance_pack_with_options(request, runtime)
 
     async def create_aggregate_compliance_pack_async(
         self,
         request: config_20200907_models.CreateAggregateCompliancePackRequest,
     ) -> config_20200907_models.CreateAggregateCompliancePackResponse:
+        """
+        You can use your management account to create up to five compliance packages for each account group.
+        This topic provides an example on how to create a compliance package named ClassifiedProtectionPreCheck for the `ca-f632626622af0079****` account group. The compliance package contains the `eip-bandwidth-limit` managed rule.
+        
+        @param request: CreateAggregateCompliancePackRequest
+        @return: CreateAggregateCompliancePackResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_aggregate_compliance_pack_with_options_async(request, runtime)
 
     def create_aggregate_config_delivery_channel_with_options(
         self,
         request: config_20200907_models.CreateAggregateConfigDeliveryChannelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.CreateAggregateConfigDeliveryChannelResponse:
+        """
+        In this example, a delivery channel is created for an account group. The ID of the account group is `ca-a4e5626622af0079***`. The type of the delivery channel is `OSS` and the Alibaba Cloud Resource Name (ARN) of the delivery destination is `acs:oss:cn-shanghai:100931896542****:new-bucket`. The result indicates that the delivery channel is created. The ID of the delivery channel is `cdc-8e45ff4e06a3a8****`.
+        
+        @param request: CreateAggregateConfigDeliveryChannelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateAggregateConfigDeliveryChannelResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.configuration_item_change_notification):
@@ -604,14 +719,21 @@
         )
 
     async def create_aggregate_config_delivery_channel_with_options_async(
         self,
         request: config_20200907_models.CreateAggregateConfigDeliveryChannelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.CreateAggregateConfigDeliveryChannelResponse:
+        """
+        In this example, a delivery channel is created for an account group. The ID of the account group is `ca-a4e5626622af0079***`. The type of the delivery channel is `OSS` and the Alibaba Cloud Resource Name (ARN) of the delivery destination is `acs:oss:cn-shanghai:100931896542****:new-bucket`. The result indicates that the delivery channel is created. The ID of the delivery channel is `cdc-8e45ff4e06a3a8****`.
+        
+        @param request: CreateAggregateConfigDeliveryChannelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateAggregateConfigDeliveryChannelResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.configuration_item_change_notification):
@@ -653,29 +775,50 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_aggregate_config_delivery_channel(
         self,
         request: config_20200907_models.CreateAggregateConfigDeliveryChannelRequest,
     ) -> config_20200907_models.CreateAggregateConfigDeliveryChannelResponse:
+        """
+        In this example, a delivery channel is created for an account group. The ID of the account group is `ca-a4e5626622af0079***`. The type of the delivery channel is `OSS` and the Alibaba Cloud Resource Name (ARN) of the delivery destination is `acs:oss:cn-shanghai:100931896542****:new-bucket`. The result indicates that the delivery channel is created. The ID of the delivery channel is `cdc-8e45ff4e06a3a8****`.
+        
+        @param request: CreateAggregateConfigDeliveryChannelRequest
+        @return: CreateAggregateConfigDeliveryChannelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_aggregate_config_delivery_channel_with_options(request, runtime)
 
     async def create_aggregate_config_delivery_channel_async(
         self,
         request: config_20200907_models.CreateAggregateConfigDeliveryChannelRequest,
     ) -> config_20200907_models.CreateAggregateConfigDeliveryChannelResponse:
+        """
+        In this example, a delivery channel is created for an account group. The ID of the account group is `ca-a4e5626622af0079***`. The type of the delivery channel is `OSS` and the Alibaba Cloud Resource Name (ARN) of the delivery destination is `acs:oss:cn-shanghai:100931896542****:new-bucket`. The result indicates that the delivery channel is created. The ID of the delivery channel is `cdc-8e45ff4e06a3a8****`.
+        
+        @param request: CreateAggregateConfigDeliveryChannelRequest
+        @return: CreateAggregateConfigDeliveryChannelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_aggregate_config_delivery_channel_with_options_async(request, runtime)
 
     def create_aggregate_config_rule_with_options(
         self,
         tmp_req: config_20200907_models.CreateAggregateConfigRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.CreateAggregateConfigRuleResponse:
+        """
+        The sample request in this topic shows you how to create a rule based on the required-tags managed rule in the `ca-a4e5626622af0079***` account group. The return result shows that the rule is created and its ID is `cr-4e3d626622af0080****`.
+        ## Limits
+        A management account can contain up to 200 rules.
+        
+        @param tmp_req: CreateAggregateConfigRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateAggregateConfigRuleResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = config_20200907_models.CreateAggregateConfigRuleShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.input_parameters):
             request.input_parameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.input_parameters, 'InputParameters', 'json')
         if not UtilClient.is_unset(tmp_req.resource_types_scope):
             request.resource_types_scope_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.resource_types_scope, 'ResourceTypesScope', 'simple')
@@ -740,14 +883,23 @@
         )
 
     async def create_aggregate_config_rule_with_options_async(
         self,
         tmp_req: config_20200907_models.CreateAggregateConfigRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.CreateAggregateConfigRuleResponse:
+        """
+        The sample request in this topic shows you how to create a rule based on the required-tags managed rule in the `ca-a4e5626622af0079***` account group. The return result shows that the rule is created and its ID is `cr-4e3d626622af0080****`.
+        ## Limits
+        A management account can contain up to 200 rules.
+        
+        @param tmp_req: CreateAggregateConfigRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateAggregateConfigRuleResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = config_20200907_models.CreateAggregateConfigRuleShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.input_parameters):
             request.input_parameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.input_parameters, 'InputParameters', 'json')
         if not UtilClient.is_unset(tmp_req.resource_types_scope):
             request.resource_types_scope_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.resource_types_scope, 'ResourceTypesScope', 'simple')
@@ -811,29 +963,52 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_aggregate_config_rule(
         self,
         request: config_20200907_models.CreateAggregateConfigRuleRequest,
     ) -> config_20200907_models.CreateAggregateConfigRuleResponse:
+        """
+        The sample request in this topic shows you how to create a rule based on the required-tags managed rule in the `ca-a4e5626622af0079***` account group. The return result shows that the rule is created and its ID is `cr-4e3d626622af0080****`.
+        ## Limits
+        A management account can contain up to 200 rules.
+        
+        @param request: CreateAggregateConfigRuleRequest
+        @return: CreateAggregateConfigRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_aggregate_config_rule_with_options(request, runtime)
 
     async def create_aggregate_config_rule_async(
         self,
         request: config_20200907_models.CreateAggregateConfigRuleRequest,
     ) -> config_20200907_models.CreateAggregateConfigRuleResponse:
+        """
+        The sample request in this topic shows you how to create a rule based on the required-tags managed rule in the `ca-a4e5626622af0079***` account group. The return result shows that the rule is created and its ID is `cr-4e3d626622af0080****`.
+        ## Limits
+        A management account can contain up to 200 rules.
+        
+        @param request: CreateAggregateConfigRuleRequest
+        @return: CreateAggregateConfigRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_aggregate_config_rule_with_options_async(request, runtime)
 
     def create_aggregate_remediation_with_options(
         self,
         request: config_20200907_models.CreateAggregateRemediationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.CreateAggregateRemediationResponse:
+        """
+        The sample request in this topic shows you how to configure a remediation template for the rule whose ID is `cr-6b7c626622af00b4***` in the account group whose ID is `ca-6b4a626622af0012****`. The return result shows that a remediation template is configured and the ID of the remediation setting is `crr-909ba2d4716700eb****`.
+        
+        @param request: CreateAggregateRemediationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateAggregateRemediationResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.aggregator_id):
             body['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.config_rule_id):
@@ -868,14 +1043,21 @@
         )
 
     async def create_aggregate_remediation_with_options_async(
         self,
         request: config_20200907_models.CreateAggregateRemediationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.CreateAggregateRemediationResponse:
+        """
+        The sample request in this topic shows you how to configure a remediation template for the rule whose ID is `cr-6b7c626622af00b4***` in the account group whose ID is `ca-6b4a626622af0012****`. The return result shows that a remediation template is configured and the ID of the remediation setting is `crr-909ba2d4716700eb****`.
+        
+        @param request: CreateAggregateRemediationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateAggregateRemediationResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.aggregator_id):
             body['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.config_rule_id):
@@ -909,29 +1091,54 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_aggregate_remediation(
         self,
         request: config_20200907_models.CreateAggregateRemediationRequest,
     ) -> config_20200907_models.CreateAggregateRemediationResponse:
+        """
+        The sample request in this topic shows you how to configure a remediation template for the rule whose ID is `cr-6b7c626622af00b4***` in the account group whose ID is `ca-6b4a626622af0012****`. The return result shows that a remediation template is configured and the ID of the remediation setting is `crr-909ba2d4716700eb****`.
+        
+        @param request: CreateAggregateRemediationRequest
+        @return: CreateAggregateRemediationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_aggregate_remediation_with_options(request, runtime)
 
     async def create_aggregate_remediation_async(
         self,
         request: config_20200907_models.CreateAggregateRemediationRequest,
     ) -> config_20200907_models.CreateAggregateRemediationResponse:
+        """
+        The sample request in this topic shows you how to configure a remediation template for the rule whose ID is `cr-6b7c626622af00b4***` in the account group whose ID is `ca-6b4a626622af0012****`. The return result shows that a remediation template is configured and the ID of the remediation setting is `crr-909ba2d4716700eb****`.
+        
+        @param request: CreateAggregateRemediationRequest
+        @return: CreateAggregateRemediationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_aggregate_remediation_with_options_async(request, runtime)
 
     def create_aggregator_with_options(
         self,
         tmp_req: config_20200907_models.CreateAggregatorRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.CreateAggregatorResponse:
+        """
+        Each management account can create a maximum of five account groups. Each account group can contain a maximum of 200 member accounts.
+        Cloud Config supports the following types of account groups:
+        *   Global account group: The global account group contains all the member accounts that are added to the resource directory. A management account can create only one global account group.
+        *   Custom account group: If you create a custom account group, you must manually add all or specific member accounts from the resource directory to the custom account group.
+        In the example of this topic, a request is sent to create an account group of the `CUSTOM` type. The custom account group is named `Test_Group`, and its description is `Test account group`. The custom account group contains the following two member accounts:
+        *   Member account ID: `171322098523****`. Member account name: `Alice`.
+        *   Member account ID: `100532098349****`. Member account name: `Tom`.
+        
+        @param tmp_req: CreateAggregatorRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateAggregatorResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = config_20200907_models.CreateAggregatorShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.aggregator_accounts):
             request.aggregator_accounts_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.aggregator_accounts, 'AggregatorAccounts', 'json')
         body = {}
         if not UtilClient.is_unset(request.aggregator_accounts_shrink):
@@ -964,14 +1171,27 @@
         )
 
     async def create_aggregator_with_options_async(
         self,
         tmp_req: config_20200907_models.CreateAggregatorRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.CreateAggregatorResponse:
+        """
+        Each management account can create a maximum of five account groups. Each account group can contain a maximum of 200 member accounts.
+        Cloud Config supports the following types of account groups:
+        *   Global account group: The global account group contains all the member accounts that are added to the resource directory. A management account can create only one global account group.
+        *   Custom account group: If you create a custom account group, you must manually add all or specific member accounts from the resource directory to the custom account group.
+        In the example of this topic, a request is sent to create an account group of the `CUSTOM` type. The custom account group is named `Test_Group`, and its description is `Test account group`. The custom account group contains the following two member accounts:
+        *   Member account ID: `171322098523****`. Member account name: `Alice`.
+        *   Member account ID: `100532098349****`. Member account name: `Tom`.
+        
+        @param tmp_req: CreateAggregatorRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateAggregatorResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = config_20200907_models.CreateAggregatorShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.aggregator_accounts):
             request.aggregator_accounts_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.aggregator_accounts, 'AggregatorAccounts', 'json')
         body = {}
         if not UtilClient.is_unset(request.aggregator_accounts_shrink):
@@ -1003,29 +1223,61 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_aggregator(
         self,
         request: config_20200907_models.CreateAggregatorRequest,
     ) -> config_20200907_models.CreateAggregatorResponse:
+        """
+        Each management account can create a maximum of five account groups. Each account group can contain a maximum of 200 member accounts.
+        Cloud Config supports the following types of account groups:
+        *   Global account group: The global account group contains all the member accounts that are added to the resource directory. A management account can create only one global account group.
+        *   Custom account group: If you create a custom account group, you must manually add all or specific member accounts from the resource directory to the custom account group.
+        In the example of this topic, a request is sent to create an account group of the `CUSTOM` type. The custom account group is named `Test_Group`, and its description is `Test account group`. The custom account group contains the following two member accounts:
+        *   Member account ID: `171322098523****`. Member account name: `Alice`.
+        *   Member account ID: `100532098349****`. Member account name: `Tom`.
+        
+        @param request: CreateAggregatorRequest
+        @return: CreateAggregatorResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_aggregator_with_options(request, runtime)
 
     async def create_aggregator_async(
         self,
         request: config_20200907_models.CreateAggregatorRequest,
     ) -> config_20200907_models.CreateAggregatorResponse:
+        """
+        Each management account can create a maximum of five account groups. Each account group can contain a maximum of 200 member accounts.
+        Cloud Config supports the following types of account groups:
+        *   Global account group: The global account group contains all the member accounts that are added to the resource directory. A management account can create only one global account group.
+        *   Custom account group: If you create a custom account group, you must manually add all or specific member accounts from the resource directory to the custom account group.
+        In the example of this topic, a request is sent to create an account group of the `CUSTOM` type. The custom account group is named `Test_Group`, and its description is `Test account group`. The custom account group contains the following two member accounts:
+        *   Member account ID: `171322098523****`. Member account name: `Alice`.
+        *   Member account ID: `100532098349****`. Member account name: `Tom`.
+        
+        @param request: CreateAggregatorRequest
+        @return: CreateAggregatorResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_aggregator_with_options_async(request, runtime)
 
     def create_compliance_pack_with_options(
         self,
         tmp_req: config_20200907_models.CreateCompliancePackRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.CreateCompliancePackResponse:
+        """
+        Each ordinary account can create up to five compliance packages.
+        This topic provides an example on how to create a compliance package named ClassifiedProtectionPreCheck. The compliance package contains a managed rule named `eip-bandwidth-limit`.
+        
+        @param tmp_req: CreateCompliancePackRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateCompliancePackResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = config_20200907_models.CreateCompliancePackShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.config_rules):
             request.config_rules_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.config_rules, 'ConfigRules', 'json')
         body = {}
         if not UtilClient.is_unset(request.client_token):
@@ -1072,14 +1324,22 @@
         )
 
     async def create_compliance_pack_with_options_async(
         self,
         tmp_req: config_20200907_models.CreateCompliancePackRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.CreateCompliancePackResponse:
+        """
+        Each ordinary account can create up to five compliance packages.
+        This topic provides an example on how to create a compliance package named ClassifiedProtectionPreCheck. The compliance package contains a managed rule named `eip-bandwidth-limit`.
+        
+        @param tmp_req: CreateCompliancePackRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateCompliancePackResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = config_20200907_models.CreateCompliancePackShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.config_rules):
             request.config_rules_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.config_rules, 'ConfigRules', 'json')
         body = {}
         if not UtilClient.is_unset(request.client_token):
@@ -1125,29 +1385,50 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_compliance_pack(
         self,
         request: config_20200907_models.CreateCompliancePackRequest,
     ) -> config_20200907_models.CreateCompliancePackResponse:
+        """
+        Each ordinary account can create up to five compliance packages.
+        This topic provides an example on how to create a compliance package named ClassifiedProtectionPreCheck. The compliance package contains a managed rule named `eip-bandwidth-limit`.
+        
+        @param request: CreateCompliancePackRequest
+        @return: CreateCompliancePackResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_compliance_pack_with_options(request, runtime)
 
     async def create_compliance_pack_async(
         self,
         request: config_20200907_models.CreateCompliancePackRequest,
     ) -> config_20200907_models.CreateCompliancePackResponse:
+        """
+        Each ordinary account can create up to five compliance packages.
+        This topic provides an example on how to create a compliance package named ClassifiedProtectionPreCheck. The compliance package contains a managed rule named `eip-bandwidth-limit`.
+        
+        @param request: CreateCompliancePackRequest
+        @return: CreateCompliancePackResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_compliance_pack_with_options_async(request, runtime)
 
     def create_config_delivery_channel_with_options(
         self,
         request: config_20200907_models.CreateConfigDeliveryChannelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.CreateConfigDeliveryChannelResponse:
+        """
+        In this example, a delivery channel is created. The type of the delivery channel is `OSS` and the Alibaba Cloud Resource Name (ARN) of the delivery destination is `acs:oss:cn-shanghai:100931896542***:new-bucket`. The result indicates that the delivery channel is created, and the ID of the delivery channel is `cdc-8e45ff4e06a3a8****`.
+        
+        @param request: CreateConfigDeliveryChannelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateConfigDeliveryChannelResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.configuration_item_change_notification):
             query['ConfigurationItemChangeNotification'] = request.configuration_item_change_notification
         if not UtilClient.is_unset(request.configuration_snapshot):
@@ -1188,14 +1469,21 @@
         )
 
     async def create_config_delivery_channel_with_options_async(
         self,
         request: config_20200907_models.CreateConfigDeliveryChannelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.CreateConfigDeliveryChannelResponse:
+        """
+        In this example, a delivery channel is created. The type of the delivery channel is `OSS` and the Alibaba Cloud Resource Name (ARN) of the delivery destination is `acs:oss:cn-shanghai:100931896542***:new-bucket`. The result indicates that the delivery channel is created, and the ID of the delivery channel is `cdc-8e45ff4e06a3a8****`.
+        
+        @param request: CreateConfigDeliveryChannelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateConfigDeliveryChannelResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.configuration_item_change_notification):
             query['ConfigurationItemChangeNotification'] = request.configuration_item_change_notification
         if not UtilClient.is_unset(request.configuration_snapshot):
@@ -1235,29 +1523,50 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_config_delivery_channel(
         self,
         request: config_20200907_models.CreateConfigDeliveryChannelRequest,
     ) -> config_20200907_models.CreateConfigDeliveryChannelResponse:
+        """
+        In this example, a delivery channel is created. The type of the delivery channel is `OSS` and the Alibaba Cloud Resource Name (ARN) of the delivery destination is `acs:oss:cn-shanghai:100931896542***:new-bucket`. The result indicates that the delivery channel is created, and the ID of the delivery channel is `cdc-8e45ff4e06a3a8****`.
+        
+        @param request: CreateConfigDeliveryChannelRequest
+        @return: CreateConfigDeliveryChannelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_config_delivery_channel_with_options(request, runtime)
 
     async def create_config_delivery_channel_async(
         self,
         request: config_20200907_models.CreateConfigDeliveryChannelRequest,
     ) -> config_20200907_models.CreateConfigDeliveryChannelResponse:
+        """
+        In this example, a delivery channel is created. The type of the delivery channel is `OSS` and the Alibaba Cloud Resource Name (ARN) of the delivery destination is `acs:oss:cn-shanghai:100931896542***:new-bucket`. The result indicates that the delivery channel is created, and the ID of the delivery channel is `cdc-8e45ff4e06a3a8****`.
+        
+        @param request: CreateConfigDeliveryChannelRequest
+        @return: CreateConfigDeliveryChannelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_config_delivery_channel_with_options_async(request, runtime)
 
     def create_config_rule_with_options(
         self,
         tmp_req: config_20200907_models.CreateConfigRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.CreateConfigRuleResponse:
+        """
+        This topic provides an example on how to create a managed rule named required-tags. The returned result indicates that the rule is created and the ID of the rule is `cr-5772ba41209e007b***`.
+        ## Limits
+        You can use a common account to create up to 200 rules.
+        
+        @param tmp_req: CreateConfigRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateConfigRuleResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = config_20200907_models.CreateConfigRuleShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.input_parameters):
             request.input_parameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.input_parameters, 'InputParameters', 'json')
         if not UtilClient.is_unset(tmp_req.resource_types_scope):
             request.resource_types_scope_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.resource_types_scope, 'ResourceTypesScope', 'simple')
@@ -1314,14 +1623,23 @@
         )
 
     async def create_config_rule_with_options_async(
         self,
         tmp_req: config_20200907_models.CreateConfigRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.CreateConfigRuleResponse:
+        """
+        This topic provides an example on how to create a managed rule named required-tags. The returned result indicates that the rule is created and the ID of the rule is `cr-5772ba41209e007b***`.
+        ## Limits
+        You can use a common account to create up to 200 rules.
+        
+        @param tmp_req: CreateConfigRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateConfigRuleResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = config_20200907_models.CreateConfigRuleShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.input_parameters):
             request.input_parameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.input_parameters, 'InputParameters', 'json')
         if not UtilClient.is_unset(tmp_req.resource_types_scope):
             request.resource_types_scope_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.resource_types_scope, 'ResourceTypesScope', 'simple')
@@ -1377,29 +1695,54 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_config_rule(
         self,
         request: config_20200907_models.CreateConfigRuleRequest,
     ) -> config_20200907_models.CreateConfigRuleResponse:
+        """
+        This topic provides an example on how to create a managed rule named required-tags. The returned result indicates that the rule is created and the ID of the rule is `cr-5772ba41209e007b***`.
+        ## Limits
+        You can use a common account to create up to 200 rules.
+        
+        @param request: CreateConfigRuleRequest
+        @return: CreateConfigRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_config_rule_with_options(request, runtime)
 
     async def create_config_rule_async(
         self,
         request: config_20200907_models.CreateConfigRuleRequest,
     ) -> config_20200907_models.CreateConfigRuleResponse:
+        """
+        This topic provides an example on how to create a managed rule named required-tags. The returned result indicates that the rule is created and the ID of the rule is `cr-5772ba41209e007b***`.
+        ## Limits
+        You can use a common account to create up to 200 rules.
+        
+        @param request: CreateConfigRuleRequest
+        @return: CreateConfigRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_config_rule_with_options_async(request, runtime)
 
     def create_delivery_channel_with_options(
         self,
         request: config_20200907_models.CreateDeliveryChannelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.CreateDeliveryChannelResponse:
+        """
+        @deprecated : CreateDeliveryChannel is deprecated, please use Config::2020-09-07::CreateConfigDeliveryChannel,Config::2020-09-07::CreateAggregateConfigDeliveryChannel instead.
+        In this example, a delivery channel is created. The type of the delivery channle is `OSS`, the Alibaba Cloud Resource Name (ARN) of the delivery destination is `acs:oss:cn-shanghai:100931896542****:new-bucket`, and the ARN of the role that is assigned to the delivery channel is `acs:ram::100931896542****:role/aliyunserviceroleforconfig`. The response shows that the delivery channel is created, and the ID of the delivery channel is `cdc-8e45ff4e06a3a8****`.
+        
+        @param request: CreateDeliveryChannelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateDeliveryChannelResponse
+        Deprecated
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.configuration_item_change_notification):
             body['ConfigurationItemChangeNotification'] = request.configuration_item_change_notification
         if not UtilClient.is_unset(request.configuration_snapshot):
@@ -1440,14 +1783,23 @@
         )
 
     async def create_delivery_channel_with_options_async(
         self,
         request: config_20200907_models.CreateDeliveryChannelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.CreateDeliveryChannelResponse:
+        """
+        @deprecated : CreateDeliveryChannel is deprecated, please use Config::2020-09-07::CreateConfigDeliveryChannel,Config::2020-09-07::CreateAggregateConfigDeliveryChannel instead.
+        In this example, a delivery channel is created. The type of the delivery channle is `OSS`, the Alibaba Cloud Resource Name (ARN) of the delivery destination is `acs:oss:cn-shanghai:100931896542****:new-bucket`, and the ARN of the role that is assigned to the delivery channel is `acs:ram::100931896542****:role/aliyunserviceroleforconfig`. The response shows that the delivery channel is created, and the ID of the delivery channel is `cdc-8e45ff4e06a3a8****`.
+        
+        @param request: CreateDeliveryChannelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateDeliveryChannelResponse
+        Deprecated
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.configuration_item_change_notification):
             body['ConfigurationItemChangeNotification'] = request.configuration_item_change_notification
         if not UtilClient.is_unset(request.configuration_snapshot):
@@ -1487,29 +1839,52 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_delivery_channel(
         self,
         request: config_20200907_models.CreateDeliveryChannelRequest,
     ) -> config_20200907_models.CreateDeliveryChannelResponse:
+        """
+        @deprecated : CreateDeliveryChannel is deprecated, please use Config::2020-09-07::CreateConfigDeliveryChannel,Config::2020-09-07::CreateAggregateConfigDeliveryChannel instead.
+        In this example, a delivery channel is created. The type of the delivery channle is `OSS`, the Alibaba Cloud Resource Name (ARN) of the delivery destination is `acs:oss:cn-shanghai:100931896542****:new-bucket`, and the ARN of the role that is assigned to the delivery channel is `acs:ram::100931896542****:role/aliyunserviceroleforconfig`. The response shows that the delivery channel is created, and the ID of the delivery channel is `cdc-8e45ff4e06a3a8****`.
+        
+        @param request: CreateDeliveryChannelRequest
+        @return: CreateDeliveryChannelResponse
+        Deprecated
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_delivery_channel_with_options(request, runtime)
 
     async def create_delivery_channel_async(
         self,
         request: config_20200907_models.CreateDeliveryChannelRequest,
     ) -> config_20200907_models.CreateDeliveryChannelResponse:
+        """
+        @deprecated : CreateDeliveryChannel is deprecated, please use Config::2020-09-07::CreateConfigDeliveryChannel,Config::2020-09-07::CreateAggregateConfigDeliveryChannel instead.
+        In this example, a delivery channel is created. The type of the delivery channle is `OSS`, the Alibaba Cloud Resource Name (ARN) of the delivery destination is `acs:oss:cn-shanghai:100931896542****:new-bucket`, and the ARN of the role that is assigned to the delivery channel is `acs:ram::100931896542****:role/aliyunserviceroleforconfig`. The response shows that the delivery channel is created, and the ID of the delivery channel is `cdc-8e45ff4e06a3a8****`.
+        
+        @param request: CreateDeliveryChannelRequest
+        @return: CreateDeliveryChannelResponse
+        Deprecated
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_delivery_channel_with_options_async(request, runtime)
 
     def create_remediation_with_options(
         self,
         request: config_20200907_models.CreateRemediationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.CreateRemediationResponse:
+        """
+        In this topic, the rule whose ID is `cr-8a973ac2e2be00a2***` is used as an example. The return result shows that a remediation template is configured and the ID of the remediation setting is `crr-909ba2d4716700eb****`.
+        
+        @param request: CreateRemediationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateRemediationResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.config_rule_id):
             body['ConfigRuleId'] = request.config_rule_id
         if not UtilClient.is_unset(request.invoke_type):
@@ -1542,14 +1917,21 @@
         )
 
     async def create_remediation_with_options_async(
         self,
         request: config_20200907_models.CreateRemediationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.CreateRemediationResponse:
+        """
+        In this topic, the rule whose ID is `cr-8a973ac2e2be00a2***` is used as an example. The return result shows that a remediation template is configured and the ID of the remediation setting is `crr-909ba2d4716700eb****`.
+        
+        @param request: CreateRemediationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateRemediationResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.config_rule_id):
             body['ConfigRuleId'] = request.config_rule_id
         if not UtilClient.is_unset(request.invoke_type):
@@ -1581,29 +1963,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_remediation(
         self,
         request: config_20200907_models.CreateRemediationRequest,
     ) -> config_20200907_models.CreateRemediationResponse:
+        """
+        In this topic, the rule whose ID is `cr-8a973ac2e2be00a2***` is used as an example. The return result shows that a remediation template is configured and the ID of the remediation setting is `crr-909ba2d4716700eb****`.
+        
+        @param request: CreateRemediationRequest
+        @return: CreateRemediationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_remediation_with_options(request, runtime)
 
     async def create_remediation_async(
         self,
         request: config_20200907_models.CreateRemediationRequest,
     ) -> config_20200907_models.CreateRemediationResponse:
+        """
+        In this topic, the rule whose ID is `cr-8a973ac2e2be00a2***` is used as an example. The return result shows that a remediation template is configured and the ID of the remediation setting is `crr-909ba2d4716700eb****`.
+        
+        @param request: CreateRemediationRequest
+        @return: CreateRemediationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_remediation_with_options_async(request, runtime)
 
     def deactive_aggregate_config_rules_with_options(
         self,
         request: config_20200907_models.DeactiveAggregateConfigRulesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.DeactiveAggregateConfigRulesResponse:
+        """
+        The sample request in this topic shows you how to disable the `cr-5772ba41209e007b***` rule in the `ca-04b3fd170e340007****` account group.
+        
+        @param request: DeactiveAggregateConfigRulesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeactiveAggregateConfigRulesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.config_rule_ids):
             query['ConfigRuleIds'] = request.config_rule_ids
         req = open_api_models.OpenApiRequest(
@@ -1626,14 +2027,21 @@
         )
 
     async def deactive_aggregate_config_rules_with_options_async(
         self,
         request: config_20200907_models.DeactiveAggregateConfigRulesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.DeactiveAggregateConfigRulesResponse:
+        """
+        The sample request in this topic shows you how to disable the `cr-5772ba41209e007b***` rule in the `ca-04b3fd170e340007****` account group.
+        
+        @param request: DeactiveAggregateConfigRulesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeactiveAggregateConfigRulesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.config_rule_ids):
             query['ConfigRuleIds'] = request.config_rule_ids
         req = open_api_models.OpenApiRequest(
@@ -1655,29 +2063,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def deactive_aggregate_config_rules(
         self,
         request: config_20200907_models.DeactiveAggregateConfigRulesRequest,
     ) -> config_20200907_models.DeactiveAggregateConfigRulesResponse:
+        """
+        The sample request in this topic shows you how to disable the `cr-5772ba41209e007b***` rule in the `ca-04b3fd170e340007****` account group.
+        
+        @param request: DeactiveAggregateConfigRulesRequest
+        @return: DeactiveAggregateConfigRulesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.deactive_aggregate_config_rules_with_options(request, runtime)
 
     async def deactive_aggregate_config_rules_async(
         self,
         request: config_20200907_models.DeactiveAggregateConfigRulesRequest,
     ) -> config_20200907_models.DeactiveAggregateConfigRulesResponse:
+        """
+        The sample request in this topic shows you how to disable the `cr-5772ba41209e007b***` rule in the `ca-04b3fd170e340007****` account group.
+        
+        @param request: DeactiveAggregateConfigRulesRequest
+        @return: DeactiveAggregateConfigRulesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.deactive_aggregate_config_rules_with_options_async(request, runtime)
 
     def deactive_config_rules_with_options(
         self,
         request: config_20200907_models.DeactiveConfigRulesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.DeactiveConfigRulesResponse:
+        """
+        In this example, the `cr-19a56457e0d90058***` rule is used.
+        
+        @param request: DeactiveConfigRulesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeactiveConfigRulesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.config_rule_ids):
             query['ConfigRuleIds'] = request.config_rule_ids
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -1698,14 +2125,21 @@
         )
 
     async def deactive_config_rules_with_options_async(
         self,
         request: config_20200907_models.DeactiveConfigRulesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.DeactiveConfigRulesResponse:
+        """
+        In this example, the `cr-19a56457e0d90058***` rule is used.
+        
+        @param request: DeactiveConfigRulesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeactiveConfigRulesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.config_rule_ids):
             query['ConfigRuleIds'] = request.config_rule_ids
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -1725,29 +2159,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def deactive_config_rules(
         self,
         request: config_20200907_models.DeactiveConfigRulesRequest,
     ) -> config_20200907_models.DeactiveConfigRulesResponse:
+        """
+        In this example, the `cr-19a56457e0d90058***` rule is used.
+        
+        @param request: DeactiveConfigRulesRequest
+        @return: DeactiveConfigRulesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.deactive_config_rules_with_options(request, runtime)
 
     async def deactive_config_rules_async(
         self,
         request: config_20200907_models.DeactiveConfigRulesRequest,
     ) -> config_20200907_models.DeactiveConfigRulesResponse:
+        """
+        In this example, the `cr-19a56457e0d90058***` rule is used.
+        
+        @param request: DeactiveConfigRulesRequest
+        @return: DeactiveConfigRulesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.deactive_config_rules_with_options_async(request, runtime)
 
     def delete_aggregate_compliance_packs_with_options(
         self,
         request: config_20200907_models.DeleteAggregateCompliancePacksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.DeleteAggregateCompliancePacksResponse:
+        """
+        The sample request in this topic shows you how to delete the `cp-541e626622af0087***` compliance package from the `ca-04b3fd170e340007****` account group.
+        
+        @param request: DeleteAggregateCompliancePacksRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteAggregateCompliancePacksResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.aggregator_id):
             body['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.compliance_pack_ids):
@@ -1774,14 +2227,21 @@
         )
 
     async def delete_aggregate_compliance_packs_with_options_async(
         self,
         request: config_20200907_models.DeleteAggregateCompliancePacksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.DeleteAggregateCompliancePacksResponse:
+        """
+        The sample request in this topic shows you how to delete the `cp-541e626622af0087***` compliance package from the `ca-04b3fd170e340007****` account group.
+        
+        @param request: DeleteAggregateCompliancePacksRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteAggregateCompliancePacksResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.aggregator_id):
             body['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.compliance_pack_ids):
@@ -1807,29 +2267,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_aggregate_compliance_packs(
         self,
         request: config_20200907_models.DeleteAggregateCompliancePacksRequest,
     ) -> config_20200907_models.DeleteAggregateCompliancePacksResponse:
+        """
+        The sample request in this topic shows you how to delete the `cp-541e626622af0087***` compliance package from the `ca-04b3fd170e340007****` account group.
+        
+        @param request: DeleteAggregateCompliancePacksRequest
+        @return: DeleteAggregateCompliancePacksResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_aggregate_compliance_packs_with_options(request, runtime)
 
     async def delete_aggregate_compliance_packs_async(
         self,
         request: config_20200907_models.DeleteAggregateCompliancePacksRequest,
     ) -> config_20200907_models.DeleteAggregateCompliancePacksResponse:
+        """
+        The sample request in this topic shows you how to delete the `cp-541e626622af0087***` compliance package from the `ca-04b3fd170e340007****` account group.
+        
+        @param request: DeleteAggregateCompliancePacksRequest
+        @return: DeleteAggregateCompliancePacksResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_aggregate_compliance_packs_with_options_async(request, runtime)
 
     def delete_aggregate_config_delivery_channel_with_options(
         self,
         request: config_20200907_models.DeleteAggregateConfigDeliveryChannelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.DeleteAggregateConfigDeliveryChannelResponse:
+        """
+        This example shows how to delete the `cdc-38c3013b46c9002c***` delivery channel from the `ca-23c6626622af0041****` account group. The response shows that the `cdc-38c3013b46c9002c****` delivery channel is deleted.
+        
+        @param request: DeleteAggregateConfigDeliveryChannelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteAggregateConfigDeliveryChannelResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.delivery_channel_id):
             query['DeliveryChannelId'] = request.delivery_channel_id
         req = open_api_models.OpenApiRequest(
@@ -1852,14 +2331,21 @@
         )
 
     async def delete_aggregate_config_delivery_channel_with_options_async(
         self,
         request: config_20200907_models.DeleteAggregateConfigDeliveryChannelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.DeleteAggregateConfigDeliveryChannelResponse:
+        """
+        This example shows how to delete the `cdc-38c3013b46c9002c***` delivery channel from the `ca-23c6626622af0041****` account group. The response shows that the `cdc-38c3013b46c9002c****` delivery channel is deleted.
+        
+        @param request: DeleteAggregateConfigDeliveryChannelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteAggregateConfigDeliveryChannelResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.delivery_channel_id):
             query['DeliveryChannelId'] = request.delivery_channel_id
         req = open_api_models.OpenApiRequest(
@@ -1881,29 +2367,50 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_aggregate_config_delivery_channel(
         self,
         request: config_20200907_models.DeleteAggregateConfigDeliveryChannelRequest,
     ) -> config_20200907_models.DeleteAggregateConfigDeliveryChannelResponse:
+        """
+        This example shows how to delete the `cdc-38c3013b46c9002c***` delivery channel from the `ca-23c6626622af0041****` account group. The response shows that the `cdc-38c3013b46c9002c****` delivery channel is deleted.
+        
+        @param request: DeleteAggregateConfigDeliveryChannelRequest
+        @return: DeleteAggregateConfigDeliveryChannelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_aggregate_config_delivery_channel_with_options(request, runtime)
 
     async def delete_aggregate_config_delivery_channel_async(
         self,
         request: config_20200907_models.DeleteAggregateConfigDeliveryChannelRequest,
     ) -> config_20200907_models.DeleteAggregateConfigDeliveryChannelResponse:
+        """
+        This example shows how to delete the `cdc-38c3013b46c9002c***` delivery channel from the `ca-23c6626622af0041****` account group. The response shows that the `cdc-38c3013b46c9002c****` delivery channel is deleted.
+        
+        @param request: DeleteAggregateConfigDeliveryChannelRequest
+        @return: DeleteAggregateConfigDeliveryChannelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_aggregate_config_delivery_channel_with_options_async(request, runtime)
 
     def delete_aggregate_config_rules_with_options(
         self,
         request: config_20200907_models.DeleteAggregateConfigRulesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.DeleteAggregateConfigRulesResponse:
+        """
+        In this example, a rule named `cr-4e3d626622af0080***` is deleted from the `ca-a4e5626622af0079****` account group.
+        ## Background information
+        You can delete a rule in the Cloud Config console. After you delete the rule, the configurations of the rule are deleted.
+        
+        @param request: DeleteAggregateConfigRulesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteAggregateConfigRulesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.config_rule_ids):
             query['ConfigRuleIds'] = request.config_rule_ids
         req = open_api_models.OpenApiRequest(
@@ -1926,14 +2433,23 @@
         )
 
     async def delete_aggregate_config_rules_with_options_async(
         self,
         request: config_20200907_models.DeleteAggregateConfigRulesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.DeleteAggregateConfigRulesResponse:
+        """
+        In this example, a rule named `cr-4e3d626622af0080***` is deleted from the `ca-a4e5626622af0079****` account group.
+        ## Background information
+        You can delete a rule in the Cloud Config console. After you delete the rule, the configurations of the rule are deleted.
+        
+        @param request: DeleteAggregateConfigRulesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteAggregateConfigRulesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.config_rule_ids):
             query['ConfigRuleIds'] = request.config_rule_ids
         req = open_api_models.OpenApiRequest(
@@ -1955,29 +2471,52 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_aggregate_config_rules(
         self,
         request: config_20200907_models.DeleteAggregateConfigRulesRequest,
     ) -> config_20200907_models.DeleteAggregateConfigRulesResponse:
+        """
+        In this example, a rule named `cr-4e3d626622af0080***` is deleted from the `ca-a4e5626622af0079****` account group.
+        ## Background information
+        You can delete a rule in the Cloud Config console. After you delete the rule, the configurations of the rule are deleted.
+        
+        @param request: DeleteAggregateConfigRulesRequest
+        @return: DeleteAggregateConfigRulesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_aggregate_config_rules_with_options(request, runtime)
 
     async def delete_aggregate_config_rules_async(
         self,
         request: config_20200907_models.DeleteAggregateConfigRulesRequest,
     ) -> config_20200907_models.DeleteAggregateConfigRulesResponse:
+        """
+        In this example, a rule named `cr-4e3d626622af0080***` is deleted from the `ca-a4e5626622af0079****` account group.
+        ## Background information
+        You can delete a rule in the Cloud Config console. After you delete the rule, the configurations of the rule are deleted.
+        
+        @param request: DeleteAggregateConfigRulesRequest
+        @return: DeleteAggregateConfigRulesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_aggregate_config_rules_with_options_async(request, runtime)
 
     def delete_aggregate_remediations_with_options(
         self,
         request: config_20200907_models.DeleteAggregateRemediationsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.DeleteAggregateRemediationsResponse:
+        """
+        The sample request in this topic shows you how to delete the remediation setting whose ID is `crr-909ba2d4716700eb***` from the account group whose ID is `ca-6b4a626622af0012****`. The return result shows that the remediation setting whose ID is `crr-909ba2d4716700eb****` is deleted.
+        
+        @param request: DeleteAggregateRemediationsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteAggregateRemediationsResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.aggregator_id):
             body['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.remediation_ids):
             body['RemediationIds'] = request.remediation_ids
         req = open_api_models.OpenApiRequest(
@@ -2000,14 +2539,21 @@
         )
 
     async def delete_aggregate_remediations_with_options_async(
         self,
         request: config_20200907_models.DeleteAggregateRemediationsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.DeleteAggregateRemediationsResponse:
+        """
+        The sample request in this topic shows you how to delete the remediation setting whose ID is `crr-909ba2d4716700eb***` from the account group whose ID is `ca-6b4a626622af0012****`. The return result shows that the remediation setting whose ID is `crr-909ba2d4716700eb****` is deleted.
+        
+        @param request: DeleteAggregateRemediationsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteAggregateRemediationsResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.aggregator_id):
             body['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.remediation_ids):
             body['RemediationIds'] = request.remediation_ids
         req = open_api_models.OpenApiRequest(
@@ -2029,29 +2575,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_aggregate_remediations(
         self,
         request: config_20200907_models.DeleteAggregateRemediationsRequest,
     ) -> config_20200907_models.DeleteAggregateRemediationsResponse:
+        """
+        The sample request in this topic shows you how to delete the remediation setting whose ID is `crr-909ba2d4716700eb***` from the account group whose ID is `ca-6b4a626622af0012****`. The return result shows that the remediation setting whose ID is `crr-909ba2d4716700eb****` is deleted.
+        
+        @param request: DeleteAggregateRemediationsRequest
+        @return: DeleteAggregateRemediationsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_aggregate_remediations_with_options(request, runtime)
 
     async def delete_aggregate_remediations_async(
         self,
         request: config_20200907_models.DeleteAggregateRemediationsRequest,
     ) -> config_20200907_models.DeleteAggregateRemediationsResponse:
+        """
+        The sample request in this topic shows you how to delete the remediation setting whose ID is `crr-909ba2d4716700eb***` from the account group whose ID is `ca-6b4a626622af0012****`. The return result shows that the remediation setting whose ID is `crr-909ba2d4716700eb****` is deleted.
+        
+        @param request: DeleteAggregateRemediationsRequest
+        @return: DeleteAggregateRemediationsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_aggregate_remediations_with_options_async(request, runtime)
 
     def delete_aggregators_with_options(
         self,
         request: config_20200907_models.DeleteAggregatorsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.DeleteAggregatorsResponse:
+        """
+        In the example of this topic, a request is sent to delete the account group whose ID is `ca-9190626622af00a9***`.
+        
+        @param request: DeleteAggregatorsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteAggregatorsResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.aggregator_ids):
             body['AggregatorIds'] = request.aggregator_ids
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         req = open_api_models.OpenApiRequest(
@@ -2074,14 +2639,21 @@
         )
 
     async def delete_aggregators_with_options_async(
         self,
         request: config_20200907_models.DeleteAggregatorsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.DeleteAggregatorsResponse:
+        """
+        In the example of this topic, a request is sent to delete the account group whose ID is `ca-9190626622af00a9***`.
+        
+        @param request: DeleteAggregatorsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteAggregatorsResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.aggregator_ids):
             body['AggregatorIds'] = request.aggregator_ids
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         req = open_api_models.OpenApiRequest(
@@ -2103,29 +2675,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_aggregators(
         self,
         request: config_20200907_models.DeleteAggregatorsRequest,
     ) -> config_20200907_models.DeleteAggregatorsResponse:
+        """
+        In the example of this topic, a request is sent to delete the account group whose ID is `ca-9190626622af00a9***`.
+        
+        @param request: DeleteAggregatorsRequest
+        @return: DeleteAggregatorsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_aggregators_with_options(request, runtime)
 
     async def delete_aggregators_async(
         self,
         request: config_20200907_models.DeleteAggregatorsRequest,
     ) -> config_20200907_models.DeleteAggregatorsResponse:
+        """
+        In the example of this topic, a request is sent to delete the account group whose ID is `ca-9190626622af00a9***`.
+        
+        @param request: DeleteAggregatorsRequest
+        @return: DeleteAggregatorsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_aggregators_with_options_async(request, runtime)
 
     def delete_compliance_packs_with_options(
         self,
         request: config_20200907_models.DeleteCompliancePacksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.DeleteCompliancePacksResponse:
+        """
+        In this topic, the `cp-541e626622af0087***` compliance package is used as an example.
+        
+        @param request: DeleteCompliancePacksRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteCompliancePacksResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.compliance_pack_ids):
             body['CompliancePackIds'] = request.compliance_pack_ids
         if not UtilClient.is_unset(request.delete_rule):
@@ -2150,14 +2741,21 @@
         )
 
     async def delete_compliance_packs_with_options_async(
         self,
         request: config_20200907_models.DeleteCompliancePacksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.DeleteCompliancePacksResponse:
+        """
+        In this topic, the `cp-541e626622af0087***` compliance package is used as an example.
+        
+        @param request: DeleteCompliancePacksRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteCompliancePacksResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.compliance_pack_ids):
             body['CompliancePackIds'] = request.compliance_pack_ids
         if not UtilClient.is_unset(request.delete_rule):
@@ -2181,29 +2779,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_compliance_packs(
         self,
         request: config_20200907_models.DeleteCompliancePacksRequest,
     ) -> config_20200907_models.DeleteCompliancePacksResponse:
+        """
+        In this topic, the `cp-541e626622af0087***` compliance package is used as an example.
+        
+        @param request: DeleteCompliancePacksRequest
+        @return: DeleteCompliancePacksResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_compliance_packs_with_options(request, runtime)
 
     async def delete_compliance_packs_async(
         self,
         request: config_20200907_models.DeleteCompliancePacksRequest,
     ) -> config_20200907_models.DeleteCompliancePacksResponse:
+        """
+        In this topic, the `cp-541e626622af0087***` compliance package is used as an example.
+        
+        @param request: DeleteCompliancePacksRequest
+        @return: DeleteCompliancePacksResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_compliance_packs_with_options_async(request, runtime)
 
     def delete_config_delivery_channel_with_options(
         self,
         request: config_20200907_models.DeleteConfigDeliveryChannelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.DeleteConfigDeliveryChannelResponse:
+        """
+        This example shows how to delete the `cdc-38c3013b46c9002c***` delivery channel. The response shows that the `cdc-38c3013b46c9002c****` delivery channel is deleted.
+        
+        @param request: DeleteConfigDeliveryChannelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteConfigDeliveryChannelResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.delivery_channel_id):
             query['DeliveryChannelId'] = request.delivery_channel_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -2224,14 +2841,21 @@
         )
 
     async def delete_config_delivery_channel_with_options_async(
         self,
         request: config_20200907_models.DeleteConfigDeliveryChannelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.DeleteConfigDeliveryChannelResponse:
+        """
+        This example shows how to delete the `cdc-38c3013b46c9002c***` delivery channel. The response shows that the `cdc-38c3013b46c9002c****` delivery channel is deleted.
+        
+        @param request: DeleteConfigDeliveryChannelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteConfigDeliveryChannelResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.delivery_channel_id):
             query['DeliveryChannelId'] = request.delivery_channel_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -2251,29 +2875,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_config_delivery_channel(
         self,
         request: config_20200907_models.DeleteConfigDeliveryChannelRequest,
     ) -> config_20200907_models.DeleteConfigDeliveryChannelResponse:
+        """
+        This example shows how to delete the `cdc-38c3013b46c9002c***` delivery channel. The response shows that the `cdc-38c3013b46c9002c****` delivery channel is deleted.
+        
+        @param request: DeleteConfigDeliveryChannelRequest
+        @return: DeleteConfigDeliveryChannelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_config_delivery_channel_with_options(request, runtime)
 
     async def delete_config_delivery_channel_async(
         self,
         request: config_20200907_models.DeleteConfigDeliveryChannelRequest,
     ) -> config_20200907_models.DeleteConfigDeliveryChannelResponse:
+        """
+        This example shows how to delete the `cdc-38c3013b46c9002c***` delivery channel. The response shows that the `cdc-38c3013b46c9002c****` delivery channel is deleted.
+        
+        @param request: DeleteConfigDeliveryChannelRequest
+        @return: DeleteConfigDeliveryChannelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_config_delivery_channel_with_options_async(request, runtime)
 
     def delete_remediations_with_options(
         self,
         request: config_20200907_models.DeleteRemediationsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.DeleteRemediationsResponse:
+        """
+        In this topic, the remediation setting whose ID is `crr-909ba2d4716700eb***` is used as an example. The return result shows that the remediation setting whose ID is `crr-909ba2d4716700eb****` is deleted.
+        
+        @param request: DeleteRemediationsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteRemediationsResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.remediation_ids):
             body['RemediationIds'] = request.remediation_ids
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
@@ -2294,14 +2937,21 @@
         )
 
     async def delete_remediations_with_options_async(
         self,
         request: config_20200907_models.DeleteRemediationsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.DeleteRemediationsResponse:
+        """
+        In this topic, the remediation setting whose ID is `crr-909ba2d4716700eb***` is used as an example. The return result shows that the remediation setting whose ID is `crr-909ba2d4716700eb****` is deleted.
+        
+        @param request: DeleteRemediationsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteRemediationsResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.remediation_ids):
             body['RemediationIds'] = request.remediation_ids
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
@@ -2321,29 +2971,50 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_remediations(
         self,
         request: config_20200907_models.DeleteRemediationsRequest,
     ) -> config_20200907_models.DeleteRemediationsResponse:
+        """
+        In this topic, the remediation setting whose ID is `crr-909ba2d4716700eb***` is used as an example. The return result shows that the remediation setting whose ID is `crr-909ba2d4716700eb****` is deleted.
+        
+        @param request: DeleteRemediationsRequest
+        @return: DeleteRemediationsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_remediations_with_options(request, runtime)
 
     async def delete_remediations_async(
         self,
         request: config_20200907_models.DeleteRemediationsRequest,
     ) -> config_20200907_models.DeleteRemediationsResponse:
+        """
+        In this topic, the remediation setting whose ID is `crr-909ba2d4716700eb***` is used as an example. The return result shows that the remediation setting whose ID is `crr-909ba2d4716700eb****` is deleted.
+        
+        @param request: DeleteRemediationsRequest
+        @return: DeleteRemediationsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_remediations_with_options_async(request, runtime)
 
     def detach_aggregate_config_rule_to_compliance_pack_with_options(
         self,
         request: config_20200907_models.DetachAggregateConfigRuleToCompliancePackRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.DetachAggregateConfigRuleToCompliancePackResponse:
+        """
+        The sample request in this topic shows you how to remove the `cr-6cc4626622af00e7***` rule in the `ca-75b4626622af00c3****` account group from the `cp-5bb1626622af00bd****` compliance package.
+        ## Prerequisites
+        One or more rules in an account group are added to a compliance package.
+        
+        @param request: DetachAggregateConfigRuleToCompliancePackRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DetachAggregateConfigRuleToCompliancePackResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.compliance_pack_id):
             query['CompliancePackId'] = request.compliance_pack_id
         if not UtilClient.is_unset(request.config_rule_ids):
@@ -2368,14 +3039,23 @@
         )
 
     async def detach_aggregate_config_rule_to_compliance_pack_with_options_async(
         self,
         request: config_20200907_models.DetachAggregateConfigRuleToCompliancePackRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.DetachAggregateConfigRuleToCompliancePackResponse:
+        """
+        The sample request in this topic shows you how to remove the `cr-6cc4626622af00e7***` rule in the `ca-75b4626622af00c3****` account group from the `cp-5bb1626622af00bd****` compliance package.
+        ## Prerequisites
+        One or more rules in an account group are added to a compliance package.
+        
+        @param request: DetachAggregateConfigRuleToCompliancePackRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DetachAggregateConfigRuleToCompliancePackResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.compliance_pack_id):
             query['CompliancePackId'] = request.compliance_pack_id
         if not UtilClient.is_unset(request.config_rule_ids):
@@ -2399,29 +3079,54 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def detach_aggregate_config_rule_to_compliance_pack(
         self,
         request: config_20200907_models.DetachAggregateConfigRuleToCompliancePackRequest,
     ) -> config_20200907_models.DetachAggregateConfigRuleToCompliancePackResponse:
+        """
+        The sample request in this topic shows you how to remove the `cr-6cc4626622af00e7***` rule in the `ca-75b4626622af00c3****` account group from the `cp-5bb1626622af00bd****` compliance package.
+        ## Prerequisites
+        One or more rules in an account group are added to a compliance package.
+        
+        @param request: DetachAggregateConfigRuleToCompliancePackRequest
+        @return: DetachAggregateConfigRuleToCompliancePackResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.detach_aggregate_config_rule_to_compliance_pack_with_options(request, runtime)
 
     async def detach_aggregate_config_rule_to_compliance_pack_async(
         self,
         request: config_20200907_models.DetachAggregateConfigRuleToCompliancePackRequest,
     ) -> config_20200907_models.DetachAggregateConfigRuleToCompliancePackResponse:
+        """
+        The sample request in this topic shows you how to remove the `cr-6cc4626622af00e7***` rule in the `ca-75b4626622af00c3****` account group from the `cp-5bb1626622af00bd****` compliance package.
+        ## Prerequisites
+        One or more rules in an account group are added to a compliance package.
+        
+        @param request: DetachAggregateConfigRuleToCompliancePackRequest
+        @return: DetachAggregateConfigRuleToCompliancePackResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.detach_aggregate_config_rule_to_compliance_pack_with_options_async(request, runtime)
 
     def detach_config_rule_to_compliance_pack_with_options(
         self,
         request: config_20200907_models.DetachConfigRuleToCompliancePackRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.DetachConfigRuleToCompliancePackResponse:
+        """
+        The sample request in this topic shows you how to remove the `cr-6cc4626622af00e7***` rule from the `cp-5bb1626622af00bd****` compliance package.
+        ## Prerequisites
+        One or more rules are added to a compliance package.
+        
+        @param request: DetachConfigRuleToCompliancePackRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DetachConfigRuleToCompliancePackResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.compliance_pack_id):
             query['CompliancePackId'] = request.compliance_pack_id
         if not UtilClient.is_unset(request.config_rule_ids):
             query['ConfigRuleIds'] = request.config_rule_ids
         req = open_api_models.OpenApiRequest(
@@ -2444,14 +3149,23 @@
         )
 
     async def detach_config_rule_to_compliance_pack_with_options_async(
         self,
         request: config_20200907_models.DetachConfigRuleToCompliancePackRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.DetachConfigRuleToCompliancePackResponse:
+        """
+        The sample request in this topic shows you how to remove the `cr-6cc4626622af00e7***` rule from the `cp-5bb1626622af00bd****` compliance package.
+        ## Prerequisites
+        One or more rules are added to a compliance package.
+        
+        @param request: DetachConfigRuleToCompliancePackRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DetachConfigRuleToCompliancePackResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.compliance_pack_id):
             query['CompliancePackId'] = request.compliance_pack_id
         if not UtilClient.is_unset(request.config_rule_ids):
             query['ConfigRuleIds'] = request.config_rule_ids
         req = open_api_models.OpenApiRequest(
@@ -2473,21 +3187,37 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def detach_config_rule_to_compliance_pack(
         self,
         request: config_20200907_models.DetachConfigRuleToCompliancePackRequest,
     ) -> config_20200907_models.DetachConfigRuleToCompliancePackResponse:
+        """
+        The sample request in this topic shows you how to remove the `cr-6cc4626622af00e7***` rule from the `cp-5bb1626622af00bd****` compliance package.
+        ## Prerequisites
+        One or more rules are added to a compliance package.
+        
+        @param request: DetachConfigRuleToCompliancePackRequest
+        @return: DetachConfigRuleToCompliancePackResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.detach_config_rule_to_compliance_pack_with_options(request, runtime)
 
     async def detach_config_rule_to_compliance_pack_async(
         self,
         request: config_20200907_models.DetachConfigRuleToCompliancePackRequest,
     ) -> config_20200907_models.DetachConfigRuleToCompliancePackResponse:
+        """
+        The sample request in this topic shows you how to remove the `cr-6cc4626622af00e7***` rule from the `cp-5bb1626622af00bd****` compliance package.
+        ## Prerequisites
+        One or more rules are added to a compliance package.
+        
+        @param request: DetachConfigRuleToCompliancePackRequest
+        @return: DetachConfigRuleToCompliancePackResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.detach_config_rule_to_compliance_pack_with_options_async(request, runtime)
 
     def evaluate_pre_config_rules_with_options(
         self,
         tmp_req: config_20200907_models.EvaluatePreConfigRulesRequest,
         runtime: util_models.RuntimeOptions,
@@ -2570,14 +3300,22 @@
         return await self.evaluate_pre_config_rules_with_options_async(request, runtime)
 
     def generate_aggregate_compliance_pack_report_with_options(
         self,
         request: config_20200907_models.GenerateAggregateCompliancePackReportRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GenerateAggregateCompliancePackReportResponse:
+        """
+        >  You can call this operation to generate the latest compliance evaluation report. To download the report, call the GetAggregateConfigRulesReport operation. For more information, see [GetAggregateCompliancePackReport](~~262699~~).
+        The sample request in this topic shows you how to generate a compliance evaluation report based on the `cp-fdc8626622af00f9****` compliance package in the `ca-f632626622af0079****` account group.
+        
+        @param request: GenerateAggregateCompliancePackReportRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GenerateAggregateCompliancePackReportResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.aggregator_id):
             body['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.compliance_pack_id):
@@ -2602,14 +3340,22 @@
         )
 
     async def generate_aggregate_compliance_pack_report_with_options_async(
         self,
         request: config_20200907_models.GenerateAggregateCompliancePackReportRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GenerateAggregateCompliancePackReportResponse:
+        """
+        >  You can call this operation to generate the latest compliance evaluation report. To download the report, call the GetAggregateConfigRulesReport operation. For more information, see [GetAggregateCompliancePackReport](~~262699~~).
+        The sample request in this topic shows you how to generate a compliance evaluation report based on the `cp-fdc8626622af00f9****` compliance package in the `ca-f632626622af0079****` account group.
+        
+        @param request: GenerateAggregateCompliancePackReportRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GenerateAggregateCompliancePackReportResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.aggregator_id):
             body['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.compliance_pack_id):
@@ -2633,29 +3379,51 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def generate_aggregate_compliance_pack_report(
         self,
         request: config_20200907_models.GenerateAggregateCompliancePackReportRequest,
     ) -> config_20200907_models.GenerateAggregateCompliancePackReportResponse:
+        """
+        >  You can call this operation to generate the latest compliance evaluation report. To download the report, call the GetAggregateConfigRulesReport operation. For more information, see [GetAggregateCompliancePackReport](~~262699~~).
+        The sample request in this topic shows you how to generate a compliance evaluation report based on the `cp-fdc8626622af00f9****` compliance package in the `ca-f632626622af0079****` account group.
+        
+        @param request: GenerateAggregateCompliancePackReportRequest
+        @return: GenerateAggregateCompliancePackReportResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.generate_aggregate_compliance_pack_report_with_options(request, runtime)
 
     async def generate_aggregate_compliance_pack_report_async(
         self,
         request: config_20200907_models.GenerateAggregateCompliancePackReportRequest,
     ) -> config_20200907_models.GenerateAggregateCompliancePackReportResponse:
+        """
+        >  You can call this operation to generate the latest compliance evaluation report. To download the report, call the GetAggregateConfigRulesReport operation. For more information, see [GetAggregateCompliancePackReport](~~262699~~).
+        The sample request in this topic shows you how to generate a compliance evaluation report based on the `cp-fdc8626622af00f9****` compliance package in the `ca-f632626622af0079****` account group.
+        
+        @param request: GenerateAggregateCompliancePackReportRequest
+        @return: GenerateAggregateCompliancePackReportResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.generate_aggregate_compliance_pack_report_with_options_async(request, runtime)
 
     def generate_aggregate_config_rules_report_with_options(
         self,
         request: config_20200907_models.GenerateAggregateConfigRulesReportRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GenerateAggregateConfigRulesReportResponse:
+        """
+        >  You can call this operation to generate the latest compliance evaluation report. To download the report, call the GetAggregateConfigRulesReport operation. For more information, see [GetAggregateConfigRulesReport](~~262706~~).
+        The sample request in this topic shows you how to generate a compliance evaluation report based on all rules in the `ca-f632626622af0079****` account group.
+        
+        @param request: GenerateAggregateConfigRulesReportRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GenerateAggregateConfigRulesReportResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.aggregator_id):
             body['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.config_rule_ids):
@@ -2680,14 +3448,22 @@
         )
 
     async def generate_aggregate_config_rules_report_with_options_async(
         self,
         request: config_20200907_models.GenerateAggregateConfigRulesReportRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GenerateAggregateConfigRulesReportResponse:
+        """
+        >  You can call this operation to generate the latest compliance evaluation report. To download the report, call the GetAggregateConfigRulesReport operation. For more information, see [GetAggregateConfigRulesReport](~~262706~~).
+        The sample request in this topic shows you how to generate a compliance evaluation report based on all rules in the `ca-f632626622af0079****` account group.
+        
+        @param request: GenerateAggregateConfigRulesReportRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GenerateAggregateConfigRulesReportResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.aggregator_id):
             body['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.config_rule_ids):
@@ -2711,29 +3487,51 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def generate_aggregate_config_rules_report(
         self,
         request: config_20200907_models.GenerateAggregateConfigRulesReportRequest,
     ) -> config_20200907_models.GenerateAggregateConfigRulesReportResponse:
+        """
+        >  You can call this operation to generate the latest compliance evaluation report. To download the report, call the GetAggregateConfigRulesReport operation. For more information, see [GetAggregateConfigRulesReport](~~262706~~).
+        The sample request in this topic shows you how to generate a compliance evaluation report based on all rules in the `ca-f632626622af0079****` account group.
+        
+        @param request: GenerateAggregateConfigRulesReportRequest
+        @return: GenerateAggregateConfigRulesReportResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.generate_aggregate_config_rules_report_with_options(request, runtime)
 
     async def generate_aggregate_config_rules_report_async(
         self,
         request: config_20200907_models.GenerateAggregateConfigRulesReportRequest,
     ) -> config_20200907_models.GenerateAggregateConfigRulesReportResponse:
+        """
+        >  You can call this operation to generate the latest compliance evaluation report. To download the report, call the GetAggregateConfigRulesReport operation. For more information, see [GetAggregateConfigRulesReport](~~262706~~).
+        The sample request in this topic shows you how to generate a compliance evaluation report based on all rules in the `ca-f632626622af0079****` account group.
+        
+        @param request: GenerateAggregateConfigRulesReportRequest
+        @return: GenerateAggregateConfigRulesReportResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.generate_aggregate_config_rules_report_with_options_async(request, runtime)
 
     def generate_compliance_pack_report_with_options(
         self,
         request: config_20200907_models.GenerateCompliancePackReportRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GenerateCompliancePackReportResponse:
+        """
+        >  You can call this operation to generate the latest compliance evaluation report. To download the report, call the GetCompliancePackReport operation. For more information, see [GetCompliancePackReport](~~263347~~).
+        In this topic, the `cp-a8a8626622af0082****` compliance package is used as an example.
+        
+        @param request: GenerateCompliancePackReportRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GenerateCompliancePackReportResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.compliance_pack_id):
             body['CompliancePackId'] = request.compliance_pack_id
         req = open_api_models.OpenApiRequest(
@@ -2756,14 +3554,22 @@
         )
 
     async def generate_compliance_pack_report_with_options_async(
         self,
         request: config_20200907_models.GenerateCompliancePackReportRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GenerateCompliancePackReportResponse:
+        """
+        >  You can call this operation to generate the latest compliance evaluation report. To download the report, call the GetCompliancePackReport operation. For more information, see [GetCompliancePackReport](~~263347~~).
+        In this topic, the `cp-a8a8626622af0082****` compliance package is used as an example.
+        
+        @param request: GenerateCompliancePackReportRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GenerateCompliancePackReportResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.compliance_pack_id):
             body['CompliancePackId'] = request.compliance_pack_id
         req = open_api_models.OpenApiRequest(
@@ -2785,29 +3591,51 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def generate_compliance_pack_report(
         self,
         request: config_20200907_models.GenerateCompliancePackReportRequest,
     ) -> config_20200907_models.GenerateCompliancePackReportResponse:
+        """
+        >  You can call this operation to generate the latest compliance evaluation report. To download the report, call the GetCompliancePackReport operation. For more information, see [GetCompliancePackReport](~~263347~~).
+        In this topic, the `cp-a8a8626622af0082****` compliance package is used as an example.
+        
+        @param request: GenerateCompliancePackReportRequest
+        @return: GenerateCompliancePackReportResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.generate_compliance_pack_report_with_options(request, runtime)
 
     async def generate_compliance_pack_report_async(
         self,
         request: config_20200907_models.GenerateCompliancePackReportRequest,
     ) -> config_20200907_models.GenerateCompliancePackReportResponse:
+        """
+        >  You can call this operation to generate the latest compliance evaluation report. To download the report, call the GetCompliancePackReport operation. For more information, see [GetCompliancePackReport](~~263347~~).
+        In this topic, the `cp-a8a8626622af0082****` compliance package is used as an example.
+        
+        @param request: GenerateCompliancePackReportRequest
+        @return: GenerateCompliancePackReportResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.generate_compliance_pack_report_with_options_async(request, runtime)
 
     def generate_config_rules_report_with_options(
         self,
         request: config_20200907_models.GenerateConfigRulesReportRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GenerateConfigRulesReportResponse:
+        """
+        >  You can call this operation to generate the latest compliance evaluation report. To download the report, call the GetConfigRulesReport operation. For more information, see [GetConfigRulesReport](~~263608~~).
+        This topic provides an example of how to generate a compliance evaluation report based on all existing rules.
+        
+        @param request: GenerateConfigRulesReportRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GenerateConfigRulesReportResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.config_rule_ids):
             body['ConfigRuleIds'] = request.config_rule_ids
         req = open_api_models.OpenApiRequest(
@@ -2830,14 +3658,22 @@
         )
 
     async def generate_config_rules_report_with_options_async(
         self,
         request: config_20200907_models.GenerateConfigRulesReportRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GenerateConfigRulesReportResponse:
+        """
+        >  You can call this operation to generate the latest compliance evaluation report. To download the report, call the GetConfigRulesReport operation. For more information, see [GetConfigRulesReport](~~263608~~).
+        This topic provides an example of how to generate a compliance evaluation report based on all existing rules.
+        
+        @param request: GenerateConfigRulesReportRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GenerateConfigRulesReportResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.config_rule_ids):
             body['ConfigRuleIds'] = request.config_rule_ids
         req = open_api_models.OpenApiRequest(
@@ -2859,29 +3695,50 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def generate_config_rules_report(
         self,
         request: config_20200907_models.GenerateConfigRulesReportRequest,
     ) -> config_20200907_models.GenerateConfigRulesReportResponse:
+        """
+        >  You can call this operation to generate the latest compliance evaluation report. To download the report, call the GetConfigRulesReport operation. For more information, see [GetConfigRulesReport](~~263608~~).
+        This topic provides an example of how to generate a compliance evaluation report based on all existing rules.
+        
+        @param request: GenerateConfigRulesReportRequest
+        @return: GenerateConfigRulesReportResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.generate_config_rules_report_with_options(request, runtime)
 
     async def generate_config_rules_report_async(
         self,
         request: config_20200907_models.GenerateConfigRulesReportRequest,
     ) -> config_20200907_models.GenerateConfigRulesReportResponse:
+        """
+        >  You can call this operation to generate the latest compliance evaluation report. To download the report, call the GetConfigRulesReport operation. For more information, see [GetConfigRulesReport](~~263608~~).
+        This topic provides an example of how to generate a compliance evaluation report based on all existing rules.
+        
+        @param request: GenerateConfigRulesReportRequest
+        @return: GenerateConfigRulesReportResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.generate_config_rules_report_with_options_async(request, runtime)
 
     def get_aggregate_account_compliance_by_pack_with_options(
         self,
         request: config_20200907_models.GetAggregateAccountComplianceByPackRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateAccountComplianceByPackResponse:
+        """
+        The sample request in this topic shows you how to query the compliance evaluation results of member accounts monitored by the `cp-541e626622af0087***` compliance package in the `ca-04b3fd170e340007****` account group. The return result shows that two member accounts are monitored by the compliance package and they are both evaluated as compliant.
+        
+        @param request: GetAggregateAccountComplianceByPackRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAggregateAccountComplianceByPackResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetAggregateAccountComplianceByPack',
@@ -2900,14 +3757,21 @@
         )
 
     async def get_aggregate_account_compliance_by_pack_with_options_async(
         self,
         request: config_20200907_models.GetAggregateAccountComplianceByPackRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateAccountComplianceByPackResponse:
+        """
+        The sample request in this topic shows you how to query the compliance evaluation results of member accounts monitored by the `cp-541e626622af0087***` compliance package in the `ca-04b3fd170e340007****` account group. The return result shows that two member accounts are monitored by the compliance package and they are both evaluated as compliant.
+        
+        @param request: GetAggregateAccountComplianceByPackRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAggregateAccountComplianceByPackResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetAggregateAccountComplianceByPack',
@@ -2925,29 +3789,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_aggregate_account_compliance_by_pack(
         self,
         request: config_20200907_models.GetAggregateAccountComplianceByPackRequest,
     ) -> config_20200907_models.GetAggregateAccountComplianceByPackResponse:
+        """
+        The sample request in this topic shows you how to query the compliance evaluation results of member accounts monitored by the `cp-541e626622af0087***` compliance package in the `ca-04b3fd170e340007****` account group. The return result shows that two member accounts are monitored by the compliance package and they are both evaluated as compliant.
+        
+        @param request: GetAggregateAccountComplianceByPackRequest
+        @return: GetAggregateAccountComplianceByPackResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_aggregate_account_compliance_by_pack_with_options(request, runtime)
 
     async def get_aggregate_account_compliance_by_pack_async(
         self,
         request: config_20200907_models.GetAggregateAccountComplianceByPackRequest,
     ) -> config_20200907_models.GetAggregateAccountComplianceByPackResponse:
+        """
+        The sample request in this topic shows you how to query the compliance evaluation results of member accounts monitored by the `cp-541e626622af0087***` compliance package in the `ca-04b3fd170e340007****` account group. The return result shows that two member accounts are monitored by the compliance package and they are both evaluated as compliant.
+        
+        @param request: GetAggregateAccountComplianceByPackRequest
+        @return: GetAggregateAccountComplianceByPackResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_aggregate_account_compliance_by_pack_with_options_async(request, runtime)
 
     def get_aggregate_compliance_pack_with_options(
         self,
         request: config_20200907_models.GetAggregateCompliancePackRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateCompliancePackResponse:
+        """
+        The topic provides an example on how to query the details of a compliance package whose ID is `cp-fdc8626622af00f9***` in an account group whose ID is `ca-f632626622af0079****`.
+        
+        @param request: GetAggregateCompliancePackRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAggregateCompliancePackResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetAggregateCompliancePack',
@@ -2966,14 +3849,21 @@
         )
 
     async def get_aggregate_compliance_pack_with_options_async(
         self,
         request: config_20200907_models.GetAggregateCompliancePackRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateCompliancePackResponse:
+        """
+        The topic provides an example on how to query the details of a compliance package whose ID is `cp-fdc8626622af00f9***` in an account group whose ID is `ca-f632626622af0079****`.
+        
+        @param request: GetAggregateCompliancePackRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAggregateCompliancePackResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetAggregateCompliancePack',
@@ -2991,29 +3881,49 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_aggregate_compliance_pack(
         self,
         request: config_20200907_models.GetAggregateCompliancePackRequest,
     ) -> config_20200907_models.GetAggregateCompliancePackResponse:
+        """
+        The topic provides an example on how to query the details of a compliance package whose ID is `cp-fdc8626622af00f9***` in an account group whose ID is `ca-f632626622af0079****`.
+        
+        @param request: GetAggregateCompliancePackRequest
+        @return: GetAggregateCompliancePackResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_aggregate_compliance_pack_with_options(request, runtime)
 
     async def get_aggregate_compliance_pack_async(
         self,
         request: config_20200907_models.GetAggregateCompliancePackRequest,
     ) -> config_20200907_models.GetAggregateCompliancePackResponse:
+        """
+        The topic provides an example on how to query the details of a compliance package whose ID is `cp-fdc8626622af00f9***` in an account group whose ID is `ca-f632626622af0079****`.
+        
+        @param request: GetAggregateCompliancePackRequest
+        @return: GetAggregateCompliancePackResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_aggregate_compliance_pack_with_options_async(request, runtime)
 
     def get_aggregate_compliance_pack_report_with_options(
         self,
         request: config_20200907_models.GetAggregateCompliancePackReportRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateCompliancePackReportResponse:
+        """
+        >  Before you call this operation, you must call the GenerateAggregateCompliancePackReport operation to generate the latest compliance evaluation report based on a compliance package as required. For more information, see [GenerateAggregateCompliancePackReport](~~262687~~).
+        The sample request in this topic shows you how to query the compliance evaluation report that is generated based on the `cp-fdc8626622af00f9****` compliance package in the `ca-f632626622af0079****` account group.
+        
+        @param request: GetAggregateCompliancePackReportRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAggregateCompliancePackReportResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetAggregateCompliancePackReport',
@@ -3032,14 +3942,22 @@
         )
 
     async def get_aggregate_compliance_pack_report_with_options_async(
         self,
         request: config_20200907_models.GetAggregateCompliancePackReportRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateCompliancePackReportResponse:
+        """
+        >  Before you call this operation, you must call the GenerateAggregateCompliancePackReport operation to generate the latest compliance evaluation report based on a compliance package as required. For more information, see [GenerateAggregateCompliancePackReport](~~262687~~).
+        The sample request in this topic shows you how to query the compliance evaluation report that is generated based on the `cp-fdc8626622af00f9****` compliance package in the `ca-f632626622af0079****` account group.
+        
+        @param request: GetAggregateCompliancePackReportRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAggregateCompliancePackReportResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetAggregateCompliancePackReport',
@@ -3057,21 +3975,35 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_aggregate_compliance_pack_report(
         self,
         request: config_20200907_models.GetAggregateCompliancePackReportRequest,
     ) -> config_20200907_models.GetAggregateCompliancePackReportResponse:
+        """
+        >  Before you call this operation, you must call the GenerateAggregateCompliancePackReport operation to generate the latest compliance evaluation report based on a compliance package as required. For more information, see [GenerateAggregateCompliancePackReport](~~262687~~).
+        The sample request in this topic shows you how to query the compliance evaluation report that is generated based on the `cp-fdc8626622af00f9****` compliance package in the `ca-f632626622af0079****` account group.
+        
+        @param request: GetAggregateCompliancePackReportRequest
+        @return: GetAggregateCompliancePackReportResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_aggregate_compliance_pack_report_with_options(request, runtime)
 
     async def get_aggregate_compliance_pack_report_async(
         self,
         request: config_20200907_models.GetAggregateCompliancePackReportRequest,
     ) -> config_20200907_models.GetAggregateCompliancePackReportResponse:
+        """
+        >  Before you call this operation, you must call the GenerateAggregateCompliancePackReport operation to generate the latest compliance evaluation report based on a compliance package as required. For more information, see [GenerateAggregateCompliancePackReport](~~262687~~).
+        The sample request in this topic shows you how to query the compliance evaluation report that is generated based on the `cp-fdc8626622af00f9****` compliance package in the `ca-f632626622af0079****` account group.
+        
+        @param request: GetAggregateCompliancePackReportRequest
+        @return: GetAggregateCompliancePackReportResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_aggregate_compliance_pack_report_with_options_async(request, runtime)
 
     def get_aggregate_config_delivery_channel_with_options(
         self,
         request: config_20200907_models.GetAggregateConfigDeliveryChannelRequest,
         runtime: util_models.RuntimeOptions,
@@ -3146,14 +4078,21 @@
         return await self.get_aggregate_config_delivery_channel_with_options_async(request, runtime)
 
     def get_aggregate_config_rule_with_options(
         self,
         request: config_20200907_models.GetAggregateConfigRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateConfigRuleResponse:
+        """
+        This example shows how to query the details of the `cr-7f7d626622af0041***` rule in the `ca-7f00626622af0041****` account group.
+        
+        @param request: GetAggregateConfigRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAggregateConfigRuleResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.config_rule_id):
             query['ConfigRuleId'] = request.config_rule_id
         req = open_api_models.OpenApiRequest(
@@ -3176,14 +4115,21 @@
         )
 
     async def get_aggregate_config_rule_with_options_async(
         self,
         request: config_20200907_models.GetAggregateConfigRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateConfigRuleResponse:
+        """
+        This example shows how to query the details of the `cr-7f7d626622af0041***` rule in the `ca-7f00626622af0041****` account group.
+        
+        @param request: GetAggregateConfigRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAggregateConfigRuleResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.config_rule_id):
             query['ConfigRuleId'] = request.config_rule_id
         req = open_api_models.OpenApiRequest(
@@ -3205,29 +4151,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_aggregate_config_rule(
         self,
         request: config_20200907_models.GetAggregateConfigRuleRequest,
     ) -> config_20200907_models.GetAggregateConfigRuleResponse:
+        """
+        This example shows how to query the details of the `cr-7f7d626622af0041***` rule in the `ca-7f00626622af0041****` account group.
+        
+        @param request: GetAggregateConfigRuleRequest
+        @return: GetAggregateConfigRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_aggregate_config_rule_with_options(request, runtime)
 
     async def get_aggregate_config_rule_async(
         self,
         request: config_20200907_models.GetAggregateConfigRuleRequest,
     ) -> config_20200907_models.GetAggregateConfigRuleResponse:
+        """
+        This example shows how to query the details of the `cr-7f7d626622af0041***` rule in the `ca-7f00626622af0041****` account group.
+        
+        @param request: GetAggregateConfigRuleRequest
+        @return: GetAggregateConfigRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_aggregate_config_rule_with_options_async(request, runtime)
 
     def get_aggregate_config_rule_compliance_by_pack_with_options(
         self,
         request: config_20200907_models.GetAggregateConfigRuleComplianceByPackRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateConfigRuleComplianceByPackResponse:
+        """
+        The sample request in this topic shows you how to query the compliance evaluation results based on rules in the `cp-541e626622af0087***` compliance package that is created for the `ca-04b3fd170e340007****` account group. The return result shows a total of `one` rule. `No resources` are evaluated as non-compliant based on the rule.
+        
+        @param request: GetAggregateConfigRuleComplianceByPackRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAggregateConfigRuleComplianceByPackResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetAggregateConfigRuleComplianceByPack',
@@ -3246,14 +4211,21 @@
         )
 
     async def get_aggregate_config_rule_compliance_by_pack_with_options_async(
         self,
         request: config_20200907_models.GetAggregateConfigRuleComplianceByPackRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateConfigRuleComplianceByPackResponse:
+        """
+        The sample request in this topic shows you how to query the compliance evaluation results based on rules in the `cp-541e626622af0087***` compliance package that is created for the `ca-04b3fd170e340007****` account group. The return result shows a total of `one` rule. `No resources` are evaluated as non-compliant based on the rule.
+        
+        @param request: GetAggregateConfigRuleComplianceByPackRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAggregateConfigRuleComplianceByPackResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetAggregateConfigRuleComplianceByPack',
@@ -3271,29 +4243,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_aggregate_config_rule_compliance_by_pack(
         self,
         request: config_20200907_models.GetAggregateConfigRuleComplianceByPackRequest,
     ) -> config_20200907_models.GetAggregateConfigRuleComplianceByPackResponse:
+        """
+        The sample request in this topic shows you how to query the compliance evaluation results based on rules in the `cp-541e626622af0087***` compliance package that is created for the `ca-04b3fd170e340007****` account group. The return result shows a total of `one` rule. `No resources` are evaluated as non-compliant based on the rule.
+        
+        @param request: GetAggregateConfigRuleComplianceByPackRequest
+        @return: GetAggregateConfigRuleComplianceByPackResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_aggregate_config_rule_compliance_by_pack_with_options(request, runtime)
 
     async def get_aggregate_config_rule_compliance_by_pack_async(
         self,
         request: config_20200907_models.GetAggregateConfigRuleComplianceByPackRequest,
     ) -> config_20200907_models.GetAggregateConfigRuleComplianceByPackResponse:
+        """
+        The sample request in this topic shows you how to query the compliance evaluation results based on rules in the `cp-541e626622af0087***` compliance package that is created for the `ca-04b3fd170e340007****` account group. The return result shows a total of `one` rule. `No resources` are evaluated as non-compliant based on the rule.
+        
+        @param request: GetAggregateConfigRuleComplianceByPackRequest
+        @return: GetAggregateConfigRuleComplianceByPackResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_aggregate_config_rule_compliance_by_pack_with_options_async(request, runtime)
 
     def get_aggregate_config_rule_summary_by_risk_level_with_options(
         self,
         request: config_20200907_models.GetAggregateConfigRuleSummaryByRiskLevelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateConfigRuleSummaryByRiskLevelResponse:
+        """
+        In this topic, the `ca-3a58626622af0005***` account group is used as an example. The return result shows four rules that are specified with the high risk level. One of them detects non-compliant resources, and the resources evaluated by the remaining three are all compliant.
+        
+        @param request: GetAggregateConfigRuleSummaryByRiskLevelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAggregateConfigRuleSummaryByRiskLevelResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetAggregateConfigRuleSummaryByRiskLevel',
@@ -3312,14 +4303,21 @@
         )
 
     async def get_aggregate_config_rule_summary_by_risk_level_with_options_async(
         self,
         request: config_20200907_models.GetAggregateConfigRuleSummaryByRiskLevelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateConfigRuleSummaryByRiskLevelResponse:
+        """
+        In this topic, the `ca-3a58626622af0005***` account group is used as an example. The return result shows four rules that are specified with the high risk level. One of them detects non-compliant resources, and the resources evaluated by the remaining three are all compliant.
+        
+        @param request: GetAggregateConfigRuleSummaryByRiskLevelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAggregateConfigRuleSummaryByRiskLevelResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetAggregateConfigRuleSummaryByRiskLevel',
@@ -3337,29 +4335,49 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_aggregate_config_rule_summary_by_risk_level(
         self,
         request: config_20200907_models.GetAggregateConfigRuleSummaryByRiskLevelRequest,
     ) -> config_20200907_models.GetAggregateConfigRuleSummaryByRiskLevelResponse:
+        """
+        In this topic, the `ca-3a58626622af0005***` account group is used as an example. The return result shows four rules that are specified with the high risk level. One of them detects non-compliant resources, and the resources evaluated by the remaining three are all compliant.
+        
+        @param request: GetAggregateConfigRuleSummaryByRiskLevelRequest
+        @return: GetAggregateConfigRuleSummaryByRiskLevelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_aggregate_config_rule_summary_by_risk_level_with_options(request, runtime)
 
     async def get_aggregate_config_rule_summary_by_risk_level_async(
         self,
         request: config_20200907_models.GetAggregateConfigRuleSummaryByRiskLevelRequest,
     ) -> config_20200907_models.GetAggregateConfigRuleSummaryByRiskLevelResponse:
+        """
+        In this topic, the `ca-3a58626622af0005***` account group is used as an example. The return result shows four rules that are specified with the high risk level. One of them detects non-compliant resources, and the resources evaluated by the remaining three are all compliant.
+        
+        @param request: GetAggregateConfigRuleSummaryByRiskLevelRequest
+        @return: GetAggregateConfigRuleSummaryByRiskLevelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_aggregate_config_rule_summary_by_risk_level_with_options_async(request, runtime)
 
     def get_aggregate_config_rules_report_with_options(
         self,
         request: config_20200907_models.GetAggregateConfigRulesReportRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateConfigRulesReportResponse:
+        """
+        >  Before you call this operation, you must call the GenerateAggregateConfigRulesReport operation to generate the latest compliance evaluation report based on all rules in an account group as required. For more information, see [GenerateAggregateConfigRulesReport](~~262701~~).
+        The sample request in this topic shows you how to query the compliance evaluation report that is generated based on all rules in the `ca-f632626622af0079****` account group.
+        
+        @param request: GetAggregateConfigRulesReportRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAggregateConfigRulesReportResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.report_id):
             query['ReportId'] = request.report_id
         req = open_api_models.OpenApiRequest(
@@ -3382,14 +4400,22 @@
         )
 
     async def get_aggregate_config_rules_report_with_options_async(
         self,
         request: config_20200907_models.GetAggregateConfigRulesReportRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateConfigRulesReportResponse:
+        """
+        >  Before you call this operation, you must call the GenerateAggregateConfigRulesReport operation to generate the latest compliance evaluation report based on all rules in an account group as required. For more information, see [GenerateAggregateConfigRulesReport](~~262701~~).
+        The sample request in this topic shows you how to query the compliance evaluation report that is generated based on all rules in the `ca-f632626622af0079****` account group.
+        
+        @param request: GetAggregateConfigRulesReportRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAggregateConfigRulesReportResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.report_id):
             query['ReportId'] = request.report_id
         req = open_api_models.OpenApiRequest(
@@ -3411,29 +4437,50 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_aggregate_config_rules_report(
         self,
         request: config_20200907_models.GetAggregateConfigRulesReportRequest,
     ) -> config_20200907_models.GetAggregateConfigRulesReportResponse:
+        """
+        >  Before you call this operation, you must call the GenerateAggregateConfigRulesReport operation to generate the latest compliance evaluation report based on all rules in an account group as required. For more information, see [GenerateAggregateConfigRulesReport](~~262701~~).
+        The sample request in this topic shows you how to query the compliance evaluation report that is generated based on all rules in the `ca-f632626622af0079****` account group.
+        
+        @param request: GetAggregateConfigRulesReportRequest
+        @return: GetAggregateConfigRulesReportResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_aggregate_config_rules_report_with_options(request, runtime)
 
     async def get_aggregate_config_rules_report_async(
         self,
         request: config_20200907_models.GetAggregateConfigRulesReportRequest,
     ) -> config_20200907_models.GetAggregateConfigRulesReportResponse:
+        """
+        >  Before you call this operation, you must call the GenerateAggregateConfigRulesReport operation to generate the latest compliance evaluation report based on all rules in an account group as required. For more information, see [GenerateAggregateConfigRulesReport](~~262701~~).
+        The sample request in this topic shows you how to query the compliance evaluation report that is generated based on all rules in the `ca-f632626622af0079****` account group.
+        
+        @param request: GetAggregateConfigRulesReportRequest
+        @return: GetAggregateConfigRulesReportResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_aggregate_config_rules_report_with_options_async(request, runtime)
 
     def get_aggregate_discovered_resource_with_options(
         self,
         request: config_20200907_models.GetAggregateDiscoveredResourceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateDiscoveredResourceResponse:
+        """
+        The sample request in this topic shows you how to query the `new-bucket` resource in the `ca-5885626622af0008***` account group.
+        
+        @param request: GetAggregateDiscoveredResourceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAggregateDiscoveredResourceResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetAggregateDiscoveredResource',
@@ -3452,14 +4499,21 @@
         )
 
     async def get_aggregate_discovered_resource_with_options_async(
         self,
         request: config_20200907_models.GetAggregateDiscoveredResourceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateDiscoveredResourceResponse:
+        """
+        The sample request in this topic shows you how to query the `new-bucket` resource in the `ca-5885626622af0008***` account group.
+        
+        @param request: GetAggregateDiscoveredResourceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAggregateDiscoveredResourceResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetAggregateDiscoveredResource',
@@ -3477,37 +4531,58 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_aggregate_discovered_resource(
         self,
         request: config_20200907_models.GetAggregateDiscoveredResourceRequest,
     ) -> config_20200907_models.GetAggregateDiscoveredResourceResponse:
+        """
+        The sample request in this topic shows you how to query the `new-bucket` resource in the `ca-5885626622af0008***` account group.
+        
+        @param request: GetAggregateDiscoveredResourceRequest
+        @return: GetAggregateDiscoveredResourceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_aggregate_discovered_resource_with_options(request, runtime)
 
     async def get_aggregate_discovered_resource_async(
         self,
         request: config_20200907_models.GetAggregateDiscoveredResourceRequest,
     ) -> config_20200907_models.GetAggregateDiscoveredResourceResponse:
+        """
+        The sample request in this topic shows you how to query the `new-bucket` resource in the `ca-5885626622af0008***` account group.
+        
+        @param request: GetAggregateDiscoveredResourceRequest
+        @return: GetAggregateDiscoveredResourceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_aggregate_discovered_resource_with_options_async(request, runtime)
 
     def get_aggregate_resource_compliance_by_config_rule_with_options(
         self,
         request: config_20200907_models.GetAggregateResourceComplianceByConfigRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateResourceComplianceByConfigRuleResponse:
+        """
+        The sample request in this topic shows you how to query the compliance evaluation results based on the `cr-d369626622af008e***` rule in the `ca-a4e5626622af0079****` account group. The return result shows that a total of 10 resources are evaluated by the rule and five of them are evaluated as compliant.
+        
+        @param request: GetAggregateResourceComplianceByConfigRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAggregateResourceComplianceByConfigRuleResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.compliance_type):
             query['ComplianceType'] = request.compliance_type
         if not UtilClient.is_unset(request.config_rule_id):
             query['ConfigRuleId'] = request.config_rule_id
+        if not UtilClient.is_unset(request.resource_account_id):
+            query['ResourceAccountId'] = request.resource_account_id
         if not UtilClient.is_unset(request.resource_owner_id):
             query['ResourceOwnerId'] = request.resource_owner_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetAggregateResourceComplianceByConfigRule',
@@ -3526,22 +4601,31 @@
         )
 
     async def get_aggregate_resource_compliance_by_config_rule_with_options_async(
         self,
         request: config_20200907_models.GetAggregateResourceComplianceByConfigRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateResourceComplianceByConfigRuleResponse:
+        """
+        The sample request in this topic shows you how to query the compliance evaluation results based on the `cr-d369626622af008e***` rule in the `ca-a4e5626622af0079****` account group. The return result shows that a total of 10 resources are evaluated by the rule and five of them are evaluated as compliant.
+        
+        @param request: GetAggregateResourceComplianceByConfigRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAggregateResourceComplianceByConfigRuleResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.compliance_type):
             query['ComplianceType'] = request.compliance_type
         if not UtilClient.is_unset(request.config_rule_id):
             query['ConfigRuleId'] = request.config_rule_id
+        if not UtilClient.is_unset(request.resource_account_id):
+            query['ResourceAccountId'] = request.resource_account_id
         if not UtilClient.is_unset(request.resource_owner_id):
             query['ResourceOwnerId'] = request.resource_owner_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetAggregateResourceComplianceByConfigRule',
@@ -3559,29 +4643,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_aggregate_resource_compliance_by_config_rule(
         self,
         request: config_20200907_models.GetAggregateResourceComplianceByConfigRuleRequest,
     ) -> config_20200907_models.GetAggregateResourceComplianceByConfigRuleResponse:
+        """
+        The sample request in this topic shows you how to query the compliance evaluation results based on the `cr-d369626622af008e***` rule in the `ca-a4e5626622af0079****` account group. The return result shows that a total of 10 resources are evaluated by the rule and five of them are evaluated as compliant.
+        
+        @param request: GetAggregateResourceComplianceByConfigRuleRequest
+        @return: GetAggregateResourceComplianceByConfigRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_aggregate_resource_compliance_by_config_rule_with_options(request, runtime)
 
     async def get_aggregate_resource_compliance_by_config_rule_async(
         self,
         request: config_20200907_models.GetAggregateResourceComplianceByConfigRuleRequest,
     ) -> config_20200907_models.GetAggregateResourceComplianceByConfigRuleResponse:
+        """
+        The sample request in this topic shows you how to query the compliance evaluation results based on the `cr-d369626622af008e***` rule in the `ca-a4e5626622af0079****` account group. The return result shows that a total of 10 resources are evaluated by the rule and five of them are evaluated as compliant.
+        
+        @param request: GetAggregateResourceComplianceByConfigRuleRequest
+        @return: GetAggregateResourceComplianceByConfigRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_aggregate_resource_compliance_by_config_rule_with_options_async(request, runtime)
 
     def get_aggregate_resource_compliance_by_pack_with_options(
         self,
         request: config_20200907_models.GetAggregateResourceComplianceByPackRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateResourceComplianceByPackResponse:
+        """
+        The sample request in this topic shows you how to query the compliance evaluation results of resources monitored by the `cp-fdc8626622af00f9***` compliance package in the `ca-f632626622af0079****`account group. The return result shows that the total number of monitored resources is `10` and the number of non-compliant resources is `7`.
+        
+        @param request: GetAggregateResourceComplianceByPackRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAggregateResourceComplianceByPackResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetAggregateResourceComplianceByPack',
@@ -3600,14 +4703,21 @@
         )
 
     async def get_aggregate_resource_compliance_by_pack_with_options_async(
         self,
         request: config_20200907_models.GetAggregateResourceComplianceByPackRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateResourceComplianceByPackResponse:
+        """
+        The sample request in this topic shows you how to query the compliance evaluation results of resources monitored by the `cp-fdc8626622af00f9***` compliance package in the `ca-f632626622af0079****`account group. The return result shows that the total number of monitored resources is `10` and the number of non-compliant resources is `7`.
+        
+        @param request: GetAggregateResourceComplianceByPackRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAggregateResourceComplianceByPackResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetAggregateResourceComplianceByPack',
@@ -3625,21 +4735,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_aggregate_resource_compliance_by_pack(
         self,
         request: config_20200907_models.GetAggregateResourceComplianceByPackRequest,
     ) -> config_20200907_models.GetAggregateResourceComplianceByPackResponse:
+        """
+        The sample request in this topic shows you how to query the compliance evaluation results of resources monitored by the `cp-fdc8626622af00f9***` compliance package in the `ca-f632626622af0079****`account group. The return result shows that the total number of monitored resources is `10` and the number of non-compliant resources is `7`.
+        
+        @param request: GetAggregateResourceComplianceByPackRequest
+        @return: GetAggregateResourceComplianceByPackResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_aggregate_resource_compliance_by_pack_with_options(request, runtime)
 
     async def get_aggregate_resource_compliance_by_pack_async(
         self,
         request: config_20200907_models.GetAggregateResourceComplianceByPackRequest,
     ) -> config_20200907_models.GetAggregateResourceComplianceByPackResponse:
+        """
+        The sample request in this topic shows you how to query the compliance evaluation results of resources monitored by the `cp-fdc8626622af00f9***` compliance package in the `ca-f632626622af0079****`account group. The return result shows that the total number of monitored resources is `10` and the number of non-compliant resources is `7`.
+        
+        @param request: GetAggregateResourceComplianceByPackRequest
+        @return: GetAggregateResourceComplianceByPackResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_aggregate_resource_compliance_by_pack_with_options_async(request, runtime)
 
     def get_aggregate_resource_compliance_group_by_region_with_options(
         self,
         request: config_20200907_models.GetAggregateResourceComplianceGroupByRegionRequest,
         runtime: util_models.RuntimeOptions,
@@ -3788,14 +4910,21 @@
         return await self.get_aggregate_resource_compliance_group_by_resource_type_with_options_async(request, runtime)
 
     def get_aggregate_resource_compliance_timeline_with_options(
         self,
         request: config_20200907_models.GetAggregateResourceComplianceTimelineRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateResourceComplianceTimelineResponse:
+        """
+        The sample request in this topic shows you how to query the compliance timeline of the `new-bucket` resource that resides in the `cn-hangzhou` region within the `100931896542***` member account of the `ca-5885626622af0008****` account group. The new-bucket resource is an Object Storage Service (OSS) bucket. The return result shows the following two timestamps on the compliance timeline: `1625200295276` and `1625200228510`. The first timestamp indicates 12:31:35 on July 2, 2021 (UTC+8), and the second timestamp indicates 12:30:28 on July 2, 2021 (UTC+8).
+        
+        @param request: GetAggregateResourceComplianceTimelineRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAggregateResourceComplianceTimelineResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetAggregateResourceComplianceTimeline',
@@ -3814,14 +4943,21 @@
         )
 
     async def get_aggregate_resource_compliance_timeline_with_options_async(
         self,
         request: config_20200907_models.GetAggregateResourceComplianceTimelineRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateResourceComplianceTimelineResponse:
+        """
+        The sample request in this topic shows you how to query the compliance timeline of the `new-bucket` resource that resides in the `cn-hangzhou` region within the `100931896542***` member account of the `ca-5885626622af0008****` account group. The new-bucket resource is an Object Storage Service (OSS) bucket. The return result shows the following two timestamps on the compliance timeline: `1625200295276` and `1625200228510`. The first timestamp indicates 12:31:35 on July 2, 2021 (UTC+8), and the second timestamp indicates 12:30:28 on July 2, 2021 (UTC+8).
+        
+        @param request: GetAggregateResourceComplianceTimelineRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAggregateResourceComplianceTimelineResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetAggregateResourceComplianceTimeline',
@@ -3839,29 +4975,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_aggregate_resource_compliance_timeline(
         self,
         request: config_20200907_models.GetAggregateResourceComplianceTimelineRequest,
     ) -> config_20200907_models.GetAggregateResourceComplianceTimelineResponse:
+        """
+        The sample request in this topic shows you how to query the compliance timeline of the `new-bucket` resource that resides in the `cn-hangzhou` region within the `100931896542***` member account of the `ca-5885626622af0008****` account group. The new-bucket resource is an Object Storage Service (OSS) bucket. The return result shows the following two timestamps on the compliance timeline: `1625200295276` and `1625200228510`. The first timestamp indicates 12:31:35 on July 2, 2021 (UTC+8), and the second timestamp indicates 12:30:28 on July 2, 2021 (UTC+8).
+        
+        @param request: GetAggregateResourceComplianceTimelineRequest
+        @return: GetAggregateResourceComplianceTimelineResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_aggregate_resource_compliance_timeline_with_options(request, runtime)
 
     async def get_aggregate_resource_compliance_timeline_async(
         self,
         request: config_20200907_models.GetAggregateResourceComplianceTimelineRequest,
     ) -> config_20200907_models.GetAggregateResourceComplianceTimelineResponse:
+        """
+        The sample request in this topic shows you how to query the compliance timeline of the `new-bucket` resource that resides in the `cn-hangzhou` region within the `100931896542***` member account of the `ca-5885626622af0008****` account group. The new-bucket resource is an Object Storage Service (OSS) bucket. The return result shows the following two timestamps on the compliance timeline: `1625200295276` and `1625200228510`. The first timestamp indicates 12:31:35 on July 2, 2021 (UTC+8), and the second timestamp indicates 12:30:28 on July 2, 2021 (UTC+8).
+        
+        @param request: GetAggregateResourceComplianceTimelineRequest
+        @return: GetAggregateResourceComplianceTimelineResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_aggregate_resource_compliance_timeline_with_options_async(request, runtime)
 
     def get_aggregate_resource_configuration_timeline_with_options(
         self,
         request: config_20200907_models.GetAggregateResourceConfigurationTimelineRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateResourceConfigurationTimelineResponse:
+        """
+        The sample request in this topic shows you how to query the configuration timeline of the `new-bucket` resource that resides in the `cn-hangzhou` region within the `100931896542***` member account of the `ca-5885626622af0008****` account group. The new-bucket resource is an Object Storage Service (OSS) bucket. The return result shows that the timestamp when the resource configuration changes is `1624961112000`. The timestamp indicates 18:05:12 on June 29, 2021 (UTC+8).
+        
+        @param request: GetAggregateResourceConfigurationTimelineRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAggregateResourceConfigurationTimelineResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetAggregateResourceConfigurationTimeline',
@@ -3880,14 +5035,21 @@
         )
 
     async def get_aggregate_resource_configuration_timeline_with_options_async(
         self,
         request: config_20200907_models.GetAggregateResourceConfigurationTimelineRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateResourceConfigurationTimelineResponse:
+        """
+        The sample request in this topic shows you how to query the configuration timeline of the `new-bucket` resource that resides in the `cn-hangzhou` region within the `100931896542***` member account of the `ca-5885626622af0008****` account group. The new-bucket resource is an Object Storage Service (OSS) bucket. The return result shows that the timestamp when the resource configuration changes is `1624961112000`. The timestamp indicates 18:05:12 on June 29, 2021 (UTC+8).
+        
+        @param request: GetAggregateResourceConfigurationTimelineRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAggregateResourceConfigurationTimelineResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetAggregateResourceConfigurationTimeline',
@@ -3905,35 +5067,56 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_aggregate_resource_configuration_timeline(
         self,
         request: config_20200907_models.GetAggregateResourceConfigurationTimelineRequest,
     ) -> config_20200907_models.GetAggregateResourceConfigurationTimelineResponse:
+        """
+        The sample request in this topic shows you how to query the configuration timeline of the `new-bucket` resource that resides in the `cn-hangzhou` region within the `100931896542***` member account of the `ca-5885626622af0008****` account group. The new-bucket resource is an Object Storage Service (OSS) bucket. The return result shows that the timestamp when the resource configuration changes is `1624961112000`. The timestamp indicates 18:05:12 on June 29, 2021 (UTC+8).
+        
+        @param request: GetAggregateResourceConfigurationTimelineRequest
+        @return: GetAggregateResourceConfigurationTimelineResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_aggregate_resource_configuration_timeline_with_options(request, runtime)
 
     async def get_aggregate_resource_configuration_timeline_async(
         self,
         request: config_20200907_models.GetAggregateResourceConfigurationTimelineRequest,
     ) -> config_20200907_models.GetAggregateResourceConfigurationTimelineResponse:
+        """
+        The sample request in this topic shows you how to query the configuration timeline of the `new-bucket` resource that resides in the `cn-hangzhou` region within the `100931896542***` member account of the `ca-5885626622af0008****` account group. The new-bucket resource is an Object Storage Service (OSS) bucket. The return result shows that the timestamp when the resource configuration changes is `1624961112000`. The timestamp indicates 18:05:12 on June 29, 2021 (UTC+8).
+        
+        @param request: GetAggregateResourceConfigurationTimelineRequest
+        @return: GetAggregateResourceConfigurationTimelineResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_aggregate_resource_configuration_timeline_with_options_async(request, runtime)
 
     def get_aggregate_resource_counts_group_by_region_with_options(
         self,
         request: config_20200907_models.GetAggregateResourceCountsGroupByRegionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateResourceCountsGroupByRegionResponse:
+        """
+        This topic provides an example on how to query the statistics on the resources in an account group named `ca-a260626622af0005***` by region. The returned result shows that a total of `10` resources exist in the `cn-hangzhou` region.
+        
+        @param request: GetAggregateResourceCountsGroupByRegionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAggregateResourceCountsGroupByRegionResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.folder_id):
             query['FolderId'] = request.folder_id
+        if not UtilClient.is_unset(request.resource_account_id):
+            query['ResourceAccountId'] = request.resource_account_id
         if not UtilClient.is_unset(request.resource_owner_id):
             query['ResourceOwnerId'] = request.resource_owner_id
         if not UtilClient.is_unset(request.resource_type):
             query['ResourceType'] = request.resource_type
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -3954,20 +5137,29 @@
         )
 
     async def get_aggregate_resource_counts_group_by_region_with_options_async(
         self,
         request: config_20200907_models.GetAggregateResourceCountsGroupByRegionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateResourceCountsGroupByRegionResponse:
+        """
+        This topic provides an example on how to query the statistics on the resources in an account group named `ca-a260626622af0005***` by region. The returned result shows that a total of `10` resources exist in the `cn-hangzhou` region.
+        
+        @param request: GetAggregateResourceCountsGroupByRegionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAggregateResourceCountsGroupByRegionResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.folder_id):
             query['FolderId'] = request.folder_id
+        if not UtilClient.is_unset(request.resource_account_id):
+            query['ResourceAccountId'] = request.resource_account_id
         if not UtilClient.is_unset(request.resource_owner_id):
             query['ResourceOwnerId'] = request.resource_owner_id
         if not UtilClient.is_unset(request.resource_type):
             query['ResourceType'] = request.resource_type
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -3987,37 +5179,58 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_aggregate_resource_counts_group_by_region(
         self,
         request: config_20200907_models.GetAggregateResourceCountsGroupByRegionRequest,
     ) -> config_20200907_models.GetAggregateResourceCountsGroupByRegionResponse:
+        """
+        This topic provides an example on how to query the statistics on the resources in an account group named `ca-a260626622af0005***` by region. The returned result shows that a total of `10` resources exist in the `cn-hangzhou` region.
+        
+        @param request: GetAggregateResourceCountsGroupByRegionRequest
+        @return: GetAggregateResourceCountsGroupByRegionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_aggregate_resource_counts_group_by_region_with_options(request, runtime)
 
     async def get_aggregate_resource_counts_group_by_region_async(
         self,
         request: config_20200907_models.GetAggregateResourceCountsGroupByRegionRequest,
     ) -> config_20200907_models.GetAggregateResourceCountsGroupByRegionResponse:
+        """
+        This topic provides an example on how to query the statistics on the resources in an account group named `ca-a260626622af0005***` by region. The returned result shows that a total of `10` resources exist in the `cn-hangzhou` region.
+        
+        @param request: GetAggregateResourceCountsGroupByRegionRequest
+        @return: GetAggregateResourceCountsGroupByRegionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_aggregate_resource_counts_group_by_region_with_options_async(request, runtime)
 
     def get_aggregate_resource_counts_group_by_resource_type_with_options(
         self,
         request: config_20200907_models.GetAggregateResourceCountsGroupByResourceTypeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateResourceCountsGroupByResourceTypeResponse:
+        """
+        This topic provides an example on how to query the statistics on the resources in an account group whose ID is `ca-a260626622af0005***` by resource type. The returned result shows that a total of `seven` resources of the `ACS::RAM::Role` resource type exist.
+        
+        @param request: GetAggregateResourceCountsGroupByResourceTypeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAggregateResourceCountsGroupByResourceTypeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.folder_id):
             query['FolderId'] = request.folder_id
         if not UtilClient.is_unset(request.region):
             query['Region'] = request.region
+        if not UtilClient.is_unset(request.resource_account_id):
+            query['ResourceAccountId'] = request.resource_account_id
         if not UtilClient.is_unset(request.resource_owner_id):
             query['ResourceOwnerId'] = request.resource_owner_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetAggregateResourceCountsGroupByResourceType',
@@ -4036,22 +5249,31 @@
         )
 
     async def get_aggregate_resource_counts_group_by_resource_type_with_options_async(
         self,
         request: config_20200907_models.GetAggregateResourceCountsGroupByResourceTypeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregateResourceCountsGroupByResourceTypeResponse:
+        """
+        This topic provides an example on how to query the statistics on the resources in an account group whose ID is `ca-a260626622af0005***` by resource type. The returned result shows that a total of `seven` resources of the `ACS::RAM::Role` resource type exist.
+        
+        @param request: GetAggregateResourceCountsGroupByResourceTypeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAggregateResourceCountsGroupByResourceTypeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.folder_id):
             query['FolderId'] = request.folder_id
         if not UtilClient.is_unset(request.region):
             query['Region'] = request.region
+        if not UtilClient.is_unset(request.resource_account_id):
+            query['ResourceAccountId'] = request.resource_account_id
         if not UtilClient.is_unset(request.resource_owner_id):
             query['ResourceOwnerId'] = request.resource_owner_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetAggregateResourceCountsGroupByResourceType',
@@ -4069,29 +5291,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_aggregate_resource_counts_group_by_resource_type(
         self,
         request: config_20200907_models.GetAggregateResourceCountsGroupByResourceTypeRequest,
     ) -> config_20200907_models.GetAggregateResourceCountsGroupByResourceTypeResponse:
+        """
+        This topic provides an example on how to query the statistics on the resources in an account group whose ID is `ca-a260626622af0005***` by resource type. The returned result shows that a total of `seven` resources of the `ACS::RAM::Role` resource type exist.
+        
+        @param request: GetAggregateResourceCountsGroupByResourceTypeRequest
+        @return: GetAggregateResourceCountsGroupByResourceTypeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_aggregate_resource_counts_group_by_resource_type_with_options(request, runtime)
 
     async def get_aggregate_resource_counts_group_by_resource_type_async(
         self,
         request: config_20200907_models.GetAggregateResourceCountsGroupByResourceTypeRequest,
     ) -> config_20200907_models.GetAggregateResourceCountsGroupByResourceTypeResponse:
+        """
+        This topic provides an example on how to query the statistics on the resources in an account group whose ID is `ca-a260626622af0005***` by resource type. The returned result shows that a total of `seven` resources of the `ACS::RAM::Role` resource type exist.
+        
+        @param request: GetAggregateResourceCountsGroupByResourceTypeRequest
+        @return: GetAggregateResourceCountsGroupByResourceTypeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_aggregate_resource_counts_group_by_resource_type_with_options_async(request, runtime)
 
     def get_aggregator_with_options(
         self,
         request: config_20200907_models.GetAggregatorRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregatorResponse:
+        """
+        The sample request in this topic shows you how to query the details of the `ca-88ea626622af0055***` account group. The return result shows that the account group is named `Test_Group`, its description is `Test account group`, and it is of the `CUSTOM` type. The account group is in the `1` state, which indicates that it is created.
+        
+        @param request: GetAggregatorRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAggregatorResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetAggregator',
@@ -4110,14 +5351,21 @@
         )
 
     async def get_aggregator_with_options_async(
         self,
         request: config_20200907_models.GetAggregatorRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetAggregatorResponse:
+        """
+        The sample request in this topic shows you how to query the details of the `ca-88ea626622af0055***` account group. The return result shows that the account group is named `Test_Group`, its description is `Test account group`, and it is of the `CUSTOM` type. The account group is in the `1` state, which indicates that it is created.
+        
+        @param request: GetAggregatorRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAggregatorResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetAggregator',
@@ -4135,29 +5383,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_aggregator(
         self,
         request: config_20200907_models.GetAggregatorRequest,
     ) -> config_20200907_models.GetAggregatorResponse:
+        """
+        The sample request in this topic shows you how to query the details of the `ca-88ea626622af0055***` account group. The return result shows that the account group is named `Test_Group`, its description is `Test account group`, and it is of the `CUSTOM` type. The account group is in the `1` state, which indicates that it is created.
+        
+        @param request: GetAggregatorRequest
+        @return: GetAggregatorResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_aggregator_with_options(request, runtime)
 
     async def get_aggregator_async(
         self,
         request: config_20200907_models.GetAggregatorRequest,
     ) -> config_20200907_models.GetAggregatorResponse:
+        """
+        The sample request in this topic shows you how to query the details of the `ca-88ea626622af0055***` account group. The return result shows that the account group is named `Test_Group`, its description is `Test account group`, and it is of the `CUSTOM` type. The account group is in the `1` state, which indicates that it is created.
+        
+        @param request: GetAggregatorRequest
+        @return: GetAggregatorResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_aggregator_with_options_async(request, runtime)
 
     def get_compliance_pack_with_options(
         self,
         request: config_20200907_models.GetCompliancePackRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetCompliancePackResponse:
+        """
+        This topic provides an example on how to query the details of a compliance package whose ID is `cp-fdc8626622af00f9***`. The returned result shows that the name of the compliance package is `ClassifiedProtectionPreCheck`, the compliance package is in the `ACTIVE` state, and the risk level of the rules in the compliance package is `1`, which indicates high risk level.
+        
+        @param request: GetCompliancePackRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetCompliancePackResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetCompliancePack',
@@ -4176,14 +5443,21 @@
         )
 
     async def get_compliance_pack_with_options_async(
         self,
         request: config_20200907_models.GetCompliancePackRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetCompliancePackResponse:
+        """
+        This topic provides an example on how to query the details of a compliance package whose ID is `cp-fdc8626622af00f9***`. The returned result shows that the name of the compliance package is `ClassifiedProtectionPreCheck`, the compliance package is in the `ACTIVE` state, and the risk level of the rules in the compliance package is `1`, which indicates high risk level.
+        
+        @param request: GetCompliancePackRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetCompliancePackResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetCompliancePack',
@@ -4201,29 +5475,49 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_compliance_pack(
         self,
         request: config_20200907_models.GetCompliancePackRequest,
     ) -> config_20200907_models.GetCompliancePackResponse:
+        """
+        This topic provides an example on how to query the details of a compliance package whose ID is `cp-fdc8626622af00f9***`. The returned result shows that the name of the compliance package is `ClassifiedProtectionPreCheck`, the compliance package is in the `ACTIVE` state, and the risk level of the rules in the compliance package is `1`, which indicates high risk level.
+        
+        @param request: GetCompliancePackRequest
+        @return: GetCompliancePackResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_compliance_pack_with_options(request, runtime)
 
     async def get_compliance_pack_async(
         self,
         request: config_20200907_models.GetCompliancePackRequest,
     ) -> config_20200907_models.GetCompliancePackResponse:
+        """
+        This topic provides an example on how to query the details of a compliance package whose ID is `cp-fdc8626622af00f9***`. The returned result shows that the name of the compliance package is `ClassifiedProtectionPreCheck`, the compliance package is in the `ACTIVE` state, and the risk level of the rules in the compliance package is `1`, which indicates high risk level.
+        
+        @param request: GetCompliancePackRequest
+        @return: GetCompliancePackResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_compliance_pack_with_options_async(request, runtime)
 
     def get_compliance_pack_report_with_options(
         self,
         request: config_20200907_models.GetCompliancePackReportRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetCompliancePackReportResponse:
+        """
+        >  Before you call this operation, you must call the GenerateCompliancePackReport operation to generate the latest compliance evaluation report based on a compliance package as required. For more information, see [GenerateCompliancePackReport](~~263525~~).
+        In this topic, the `cp-fdc8626622af00f9****` compliance package is used as an example.
+        
+        @param request: GetCompliancePackReportRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetCompliancePackReportResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetCompliancePackReport',
@@ -4242,14 +5536,22 @@
         )
 
     async def get_compliance_pack_report_with_options_async(
         self,
         request: config_20200907_models.GetCompliancePackReportRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetCompliancePackReportResponse:
+        """
+        >  Before you call this operation, you must call the GenerateCompliancePackReport operation to generate the latest compliance evaluation report based on a compliance package as required. For more information, see [GenerateCompliancePackReport](~~263525~~).
+        In this topic, the `cp-fdc8626622af00f9****` compliance package is used as an example.
+        
+        @param request: GetCompliancePackReportRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetCompliancePackReportResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetCompliancePackReport',
@@ -4267,21 +5569,35 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_compliance_pack_report(
         self,
         request: config_20200907_models.GetCompliancePackReportRequest,
     ) -> config_20200907_models.GetCompliancePackReportResponse:
+        """
+        >  Before you call this operation, you must call the GenerateCompliancePackReport operation to generate the latest compliance evaluation report based on a compliance package as required. For more information, see [GenerateCompliancePackReport](~~263525~~).
+        In this topic, the `cp-fdc8626622af00f9****` compliance package is used as an example.
+        
+        @param request: GetCompliancePackReportRequest
+        @return: GetCompliancePackReportResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_compliance_pack_report_with_options(request, runtime)
 
     async def get_compliance_pack_report_async(
         self,
         request: config_20200907_models.GetCompliancePackReportRequest,
     ) -> config_20200907_models.GetCompliancePackReportResponse:
+        """
+        >  Before you call this operation, you must call the GenerateCompliancePackReport operation to generate the latest compliance evaluation report based on a compliance package as required. For more information, see [GenerateCompliancePackReport](~~263525~~).
+        In this topic, the `cp-fdc8626622af00f9****` compliance package is used as an example.
+        
+        @param request: GetCompliancePackReportRequest
+        @return: GetCompliancePackReportResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_compliance_pack_report_with_options_async(request, runtime)
 
     def get_config_delivery_channel_with_options(
         self,
         request: config_20200907_models.GetConfigDeliveryChannelRequest,
         runtime: util_models.RuntimeOptions,
@@ -4352,14 +5668,21 @@
         return await self.get_config_delivery_channel_with_options_async(request, runtime)
 
     def get_config_rule_with_options(
         self,
         request: config_20200907_models.GetConfigRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetConfigRuleResponse:
+        """
+        This example shows how to query the details of the `cr-7f7d626622af0041***` rule.
+        
+        @param request: GetConfigRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetConfigRuleResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.config_rule_id):
             query['ConfigRuleId'] = request.config_rule_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -4380,14 +5703,21 @@
         )
 
     async def get_config_rule_with_options_async(
         self,
         request: config_20200907_models.GetConfigRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetConfigRuleResponse:
+        """
+        This example shows how to query the details of the `cr-7f7d626622af0041***` rule.
+        
+        @param request: GetConfigRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetConfigRuleResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.config_rule_id):
             query['ConfigRuleId'] = request.config_rule_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -4407,29 +5737,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_config_rule(
         self,
         request: config_20200907_models.GetConfigRuleRequest,
     ) -> config_20200907_models.GetConfigRuleResponse:
+        """
+        This example shows how to query the details of the `cr-7f7d626622af0041***` rule.
+        
+        @param request: GetConfigRuleRequest
+        @return: GetConfigRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_config_rule_with_options(request, runtime)
 
     async def get_config_rule_async(
         self,
         request: config_20200907_models.GetConfigRuleRequest,
     ) -> config_20200907_models.GetConfigRuleResponse:
+        """
+        This example shows how to query the details of the `cr-7f7d626622af0041***` rule.
+        
+        @param request: GetConfigRuleRequest
+        @return: GetConfigRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_config_rule_with_options_async(request, runtime)
 
     def get_config_rule_compliance_by_pack_with_options(
         self,
         request: config_20200907_models.GetConfigRuleComplianceByPackRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetConfigRuleComplianceByPackResponse:
+        """
+        In this topic, the `cp-541e626622af0087***` compliance package is used as an example. The return result shows a total of one rule against which specific resources are evaluated as compliant.
+        
+        @param request: GetConfigRuleComplianceByPackRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetConfigRuleComplianceByPackResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetConfigRuleComplianceByPack',
@@ -4448,14 +5797,21 @@
         )
 
     async def get_config_rule_compliance_by_pack_with_options_async(
         self,
         request: config_20200907_models.GetConfigRuleComplianceByPackRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetConfigRuleComplianceByPackResponse:
+        """
+        In this topic, the `cp-541e626622af0087***` compliance package is used as an example. The return result shows a total of one rule against which specific resources are evaluated as compliant.
+        
+        @param request: GetConfigRuleComplianceByPackRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetConfigRuleComplianceByPackResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetConfigRuleComplianceByPack',
@@ -4473,28 +5829,47 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_config_rule_compliance_by_pack(
         self,
         request: config_20200907_models.GetConfigRuleComplianceByPackRequest,
     ) -> config_20200907_models.GetConfigRuleComplianceByPackResponse:
+        """
+        In this topic, the `cp-541e626622af0087***` compliance package is used as an example. The return result shows a total of one rule against which specific resources are evaluated as compliant.
+        
+        @param request: GetConfigRuleComplianceByPackRequest
+        @return: GetConfigRuleComplianceByPackResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_config_rule_compliance_by_pack_with_options(request, runtime)
 
     async def get_config_rule_compliance_by_pack_async(
         self,
         request: config_20200907_models.GetConfigRuleComplianceByPackRequest,
     ) -> config_20200907_models.GetConfigRuleComplianceByPackResponse:
+        """
+        In this topic, the `cp-541e626622af0087***` compliance package is used as an example. The return result shows a total of one rule against which specific resources are evaluated as compliant.
+        
+        @param request: GetConfigRuleComplianceByPackRequest
+        @return: GetConfigRuleComplianceByPackResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_config_rule_compliance_by_pack_with_options_async(request, runtime)
 
     def get_config_rule_summary_by_risk_level_with_options(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetConfigRuleSummaryByRiskLevelResponse:
+        """
+        This topic provides an example of how to query the summary of compliance evaluation results by rule risk level. The return result shows four rules that are specified with the high risk level. One of them detects non-compliant resources, and the resources evaluated by the remaining three are all compliant.
+        
+        @param request: GetConfigRuleSummaryByRiskLevelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetConfigRuleSummaryByRiskLevelResponse
+        """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
             action='GetConfigRuleSummaryByRiskLevel',
             version='2020-09-07',
             protocol='HTTPS',
             pathname='/',
             method='GET',
@@ -4508,14 +5883,21 @@
             self.call_api(params, req, runtime)
         )
 
     async def get_config_rule_summary_by_risk_level_with_options_async(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetConfigRuleSummaryByRiskLevelResponse:
+        """
+        This topic provides an example of how to query the summary of compliance evaluation results by rule risk level. The return result shows four rules that are specified with the high risk level. One of them detects non-compliant resources, and the resources evaluated by the remaining three are all compliant.
+        
+        @param request: GetConfigRuleSummaryByRiskLevelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetConfigRuleSummaryByRiskLevelResponse
+        """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
             action='GetConfigRuleSummaryByRiskLevel',
             version='2020-09-07',
             protocol='HTTPS',
             pathname='/',
             method='GET',
@@ -4526,26 +5908,44 @@
         )
         return TeaCore.from_map(
             config_20200907_models.GetConfigRuleSummaryByRiskLevelResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def get_config_rule_summary_by_risk_level(self) -> config_20200907_models.GetConfigRuleSummaryByRiskLevelResponse:
+        """
+        This topic provides an example of how to query the summary of compliance evaluation results by rule risk level. The return result shows four rules that are specified with the high risk level. One of them detects non-compliant resources, and the resources evaluated by the remaining three are all compliant.
+        
+        @return: GetConfigRuleSummaryByRiskLevelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_config_rule_summary_by_risk_level_with_options(runtime)
 
     async def get_config_rule_summary_by_risk_level_async(self) -> config_20200907_models.GetConfigRuleSummaryByRiskLevelResponse:
+        """
+        This topic provides an example of how to query the summary of compliance evaluation results by rule risk level. The return result shows four rules that are specified with the high risk level. One of them detects non-compliant resources, and the resources evaluated by the remaining three are all compliant.
+        
+        @return: GetConfigRuleSummaryByRiskLevelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_config_rule_summary_by_risk_level_with_options_async(runtime)
 
     def get_config_rules_report_with_options(
         self,
         request: config_20200907_models.GetConfigRulesReportRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetConfigRulesReportResponse:
+        """
+        >  Before you call this operation, you must call the GenerateConfigRulesReport operation to generate the latest compliance evaluation report based on all existing rules. For more information, see [GenerateConfigRulesReport](~~263601~~).
+        This topic provides an example of how to query the compliance evaluation report that is generated based on all existing rules.
+        
+        @param request: GetConfigRulesReportRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetConfigRulesReportResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.report_id):
             query['ReportId'] = request.report_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -4566,14 +5966,22 @@
         )
 
     async def get_config_rules_report_with_options_async(
         self,
         request: config_20200907_models.GetConfigRulesReportRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetConfigRulesReportResponse:
+        """
+        >  Before you call this operation, you must call the GenerateConfigRulesReport operation to generate the latest compliance evaluation report based on all existing rules. For more information, see [GenerateConfigRulesReport](~~263601~~).
+        This topic provides an example of how to query the compliance evaluation report that is generated based on all existing rules.
+        
+        @param request: GetConfigRulesReportRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetConfigRulesReportResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.report_id):
             query['ReportId'] = request.report_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -4593,29 +6001,50 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_config_rules_report(
         self,
         request: config_20200907_models.GetConfigRulesReportRequest,
     ) -> config_20200907_models.GetConfigRulesReportResponse:
+        """
+        >  Before you call this operation, you must call the GenerateConfigRulesReport operation to generate the latest compliance evaluation report based on all existing rules. For more information, see [GenerateConfigRulesReport](~~263601~~).
+        This topic provides an example of how to query the compliance evaluation report that is generated based on all existing rules.
+        
+        @param request: GetConfigRulesReportRequest
+        @return: GetConfigRulesReportResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_config_rules_report_with_options(request, runtime)
 
     async def get_config_rules_report_async(
         self,
         request: config_20200907_models.GetConfigRulesReportRequest,
     ) -> config_20200907_models.GetConfigRulesReportResponse:
+        """
+        >  Before you call this operation, you must call the GenerateConfigRulesReport operation to generate the latest compliance evaluation report based on all existing rules. For more information, see [GenerateConfigRulesReport](~~263601~~).
+        This topic provides an example of how to query the compliance evaluation report that is generated based on all existing rules.
+        
+        @param request: GetConfigRulesReportRequest
+        @return: GetConfigRulesReportResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_config_rules_report_with_options_async(request, runtime)
 
     def get_discovered_resource_with_options(
         self,
         request: config_20200907_models.GetDiscoveredResourceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetDiscoveredResourceResponse:
+        """
+        The sample request in this topic shows you how to query the details of the `new-bucket` resource.
+        
+        @param request: GetDiscoveredResourceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetDiscoveredResourceResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetDiscoveredResource',
@@ -4634,14 +6063,21 @@
         )
 
     async def get_discovered_resource_with_options_async(
         self,
         request: config_20200907_models.GetDiscoveredResourceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetDiscoveredResourceResponse:
+        """
+        The sample request in this topic shows you how to query the details of the `new-bucket` resource.
+        
+        @param request: GetDiscoveredResourceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetDiscoveredResourceResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetDiscoveredResource',
@@ -4659,29 +6095,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_discovered_resource(
         self,
         request: config_20200907_models.GetDiscoveredResourceRequest,
     ) -> config_20200907_models.GetDiscoveredResourceResponse:
+        """
+        The sample request in this topic shows you how to query the details of the `new-bucket` resource.
+        
+        @param request: GetDiscoveredResourceRequest
+        @return: GetDiscoveredResourceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_discovered_resource_with_options(request, runtime)
 
     async def get_discovered_resource_async(
         self,
         request: config_20200907_models.GetDiscoveredResourceRequest,
     ) -> config_20200907_models.GetDiscoveredResourceResponse:
+        """
+        The sample request in this topic shows you how to query the details of the `new-bucket` resource.
+        
+        @param request: GetDiscoveredResourceRequest
+        @return: GetDiscoveredResourceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_discovered_resource_with_options_async(request, runtime)
 
     def get_discovered_resource_counts_group_by_region_with_options(
         self,
         request: config_20200907_models.GetDiscoveredResourceCountsGroupByRegionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetDiscoveredResourceCountsGroupByRegionResponse:
+        """
+        This topic provides an example of how to query the statistics on resources by region. The returned result shows that a total of 10 resources exist in the `cn-hangzhou` region.
+        
+        @param request: GetDiscoveredResourceCountsGroupByRegionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetDiscoveredResourceCountsGroupByRegionResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.resource_type):
             query['ResourceType'] = request.resource_type
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -4702,14 +6157,21 @@
         )
 
     async def get_discovered_resource_counts_group_by_region_with_options_async(
         self,
         request: config_20200907_models.GetDiscoveredResourceCountsGroupByRegionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetDiscoveredResourceCountsGroupByRegionResponse:
+        """
+        This topic provides an example of how to query the statistics on resources by region. The returned result shows that a total of 10 resources exist in the `cn-hangzhou` region.
+        
+        @param request: GetDiscoveredResourceCountsGroupByRegionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetDiscoveredResourceCountsGroupByRegionResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.resource_type):
             query['ResourceType'] = request.resource_type
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -4729,29 +6191,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_discovered_resource_counts_group_by_region(
         self,
         request: config_20200907_models.GetDiscoveredResourceCountsGroupByRegionRequest,
     ) -> config_20200907_models.GetDiscoveredResourceCountsGroupByRegionResponse:
+        """
+        This topic provides an example of how to query the statistics on resources by region. The returned result shows that a total of 10 resources exist in the `cn-hangzhou` region.
+        
+        @param request: GetDiscoveredResourceCountsGroupByRegionRequest
+        @return: GetDiscoveredResourceCountsGroupByRegionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_discovered_resource_counts_group_by_region_with_options(request, runtime)
 
     async def get_discovered_resource_counts_group_by_region_async(
         self,
         request: config_20200907_models.GetDiscoveredResourceCountsGroupByRegionRequest,
     ) -> config_20200907_models.GetDiscoveredResourceCountsGroupByRegionResponse:
+        """
+        This topic provides an example of how to query the statistics on resources by region. The returned result shows that a total of 10 resources exist in the `cn-hangzhou` region.
+        
+        @param request: GetDiscoveredResourceCountsGroupByRegionRequest
+        @return: GetDiscoveredResourceCountsGroupByRegionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_discovered_resource_counts_group_by_region_with_options_async(request, runtime)
 
     def get_discovered_resource_counts_group_by_resource_type_with_options(
         self,
         request: config_20200907_models.GetDiscoveredResourceCountsGroupByResourceTypeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetDiscoveredResourceCountsGroupByResourceTypeResponse:
+        """
+        This topic describes how to query the statistics on resources by resource type. The returned result shows that a total of 10 resources of the `ACS::ECS::Instance` resource type exist.
+        
+        @param request: GetDiscoveredResourceCountsGroupByResourceTypeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetDiscoveredResourceCountsGroupByResourceTypeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.region):
             query['Region'] = request.region
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -4772,14 +6253,21 @@
         )
 
     async def get_discovered_resource_counts_group_by_resource_type_with_options_async(
         self,
         request: config_20200907_models.GetDiscoveredResourceCountsGroupByResourceTypeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetDiscoveredResourceCountsGroupByResourceTypeResponse:
+        """
+        This topic describes how to query the statistics on resources by resource type. The returned result shows that a total of 10 resources of the `ACS::ECS::Instance` resource type exist.
+        
+        @param request: GetDiscoveredResourceCountsGroupByResourceTypeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetDiscoveredResourceCountsGroupByResourceTypeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.region):
             query['Region'] = request.region
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -4799,21 +6287,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_discovered_resource_counts_group_by_resource_type(
         self,
         request: config_20200907_models.GetDiscoveredResourceCountsGroupByResourceTypeRequest,
     ) -> config_20200907_models.GetDiscoveredResourceCountsGroupByResourceTypeResponse:
+        """
+        This topic describes how to query the statistics on resources by resource type. The returned result shows that a total of 10 resources of the `ACS::ECS::Instance` resource type exist.
+        
+        @param request: GetDiscoveredResourceCountsGroupByResourceTypeRequest
+        @return: GetDiscoveredResourceCountsGroupByResourceTypeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_discovered_resource_counts_group_by_resource_type_with_options(request, runtime)
 
     async def get_discovered_resource_counts_group_by_resource_type_async(
         self,
         request: config_20200907_models.GetDiscoveredResourceCountsGroupByResourceTypeRequest,
     ) -> config_20200907_models.GetDiscoveredResourceCountsGroupByResourceTypeResponse:
+        """
+        This topic describes how to query the statistics on resources by resource type. The returned result shows that a total of 10 resources of the `ACS::ECS::Instance` resource type exist.
+        
+        @param request: GetDiscoveredResourceCountsGroupByResourceTypeRequest
+        @return: GetDiscoveredResourceCountsGroupByResourceTypeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_discovered_resource_counts_group_by_resource_type_with_options_async(request, runtime)
 
     def get_integrated_service_status_with_options(
         self,
         request: config_20200907_models.GetIntegratedServiceStatusRequest,
         runtime: util_models.RuntimeOptions,
@@ -4884,14 +6384,21 @@
         return await self.get_integrated_service_status_with_options_async(request, runtime)
 
     def get_managed_rule_with_options(
         self,
         request: config_20200907_models.GetManagedRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetManagedRuleResponse:
+        """
+        In this topic, the `cdn-domain-https-enabled` managed rule is used as an example.
+        
+        @param request: GetManagedRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetManagedRuleResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.identifier):
             query['Identifier'] = request.identifier
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -4912,14 +6419,21 @@
         )
 
     async def get_managed_rule_with_options_async(
         self,
         request: config_20200907_models.GetManagedRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetManagedRuleResponse:
+        """
+        In this topic, the `cdn-domain-https-enabled` managed rule is used as an example.
+        
+        @param request: GetManagedRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetManagedRuleResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.identifier):
             query['Identifier'] = request.identifier
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -4939,29 +6453,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_managed_rule(
         self,
         request: config_20200907_models.GetManagedRuleRequest,
     ) -> config_20200907_models.GetManagedRuleResponse:
+        """
+        In this topic, the `cdn-domain-https-enabled` managed rule is used as an example.
+        
+        @param request: GetManagedRuleRequest
+        @return: GetManagedRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_managed_rule_with_options(request, runtime)
 
     async def get_managed_rule_async(
         self,
         request: config_20200907_models.GetManagedRuleRequest,
     ) -> config_20200907_models.GetManagedRuleResponse:
+        """
+        In this topic, the `cdn-domain-https-enabled` managed rule is used as an example.
+        
+        @param request: GetManagedRuleRequest
+        @return: GetManagedRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_managed_rule_with_options_async(request, runtime)
 
     def get_resource_compliance_by_config_rule_with_options(
         self,
         request: config_20200907_models.GetResourceComplianceByConfigRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetResourceComplianceByConfigRuleResponse:
+        """
+        In this topic, the `cr-d369626622af008e***` rule is used as an example. The return result shows that a total of 10 resources are evaluated by the rule and `five` of them are evaluated as compliant.
+        
+        @param request: GetResourceComplianceByConfigRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetResourceComplianceByConfigRuleResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetResourceComplianceByConfigRule',
@@ -4980,14 +6513,21 @@
         )
 
     async def get_resource_compliance_by_config_rule_with_options_async(
         self,
         request: config_20200907_models.GetResourceComplianceByConfigRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetResourceComplianceByConfigRuleResponse:
+        """
+        In this topic, the `cr-d369626622af008e***` rule is used as an example. The return result shows that a total of 10 resources are evaluated by the rule and `five` of them are evaluated as compliant.
+        
+        @param request: GetResourceComplianceByConfigRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetResourceComplianceByConfigRuleResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetResourceComplianceByConfigRule',
@@ -5005,29 +6545,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_resource_compliance_by_config_rule(
         self,
         request: config_20200907_models.GetResourceComplianceByConfigRuleRequest,
     ) -> config_20200907_models.GetResourceComplianceByConfigRuleResponse:
+        """
+        In this topic, the `cr-d369626622af008e***` rule is used as an example. The return result shows that a total of 10 resources are evaluated by the rule and `five` of them are evaluated as compliant.
+        
+        @param request: GetResourceComplianceByConfigRuleRequest
+        @return: GetResourceComplianceByConfigRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_resource_compliance_by_config_rule_with_options(request, runtime)
 
     async def get_resource_compliance_by_config_rule_async(
         self,
         request: config_20200907_models.GetResourceComplianceByConfigRuleRequest,
     ) -> config_20200907_models.GetResourceComplianceByConfigRuleResponse:
+        """
+        In this topic, the `cr-d369626622af008e***` rule is used as an example. The return result shows that a total of 10 resources are evaluated by the rule and `five` of them are evaluated as compliant.
+        
+        @param request: GetResourceComplianceByConfigRuleRequest
+        @return: GetResourceComplianceByConfigRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_resource_compliance_by_config_rule_with_options_async(request, runtime)
 
     def get_resource_compliance_by_pack_with_options(
         self,
         request: config_20200907_models.GetResourceComplianceByPackRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetResourceComplianceByPackResponse:
+        """
+        In this topic, the `cp-541e626622af0087***` compliance package is used as an example. The return result shows a total of 10 resources and seven of them are evaluated as non-compliant.
+        
+        @param request: GetResourceComplianceByPackRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetResourceComplianceByPackResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetResourceComplianceByPack',
@@ -5046,14 +6605,21 @@
         )
 
     async def get_resource_compliance_by_pack_with_options_async(
         self,
         request: config_20200907_models.GetResourceComplianceByPackRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetResourceComplianceByPackResponse:
+        """
+        In this topic, the `cp-541e626622af0087***` compliance package is used as an example. The return result shows a total of 10 resources and seven of them are evaluated as non-compliant.
+        
+        @param request: GetResourceComplianceByPackRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetResourceComplianceByPackResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetResourceComplianceByPack',
@@ -5071,21 +6637,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_resource_compliance_by_pack(
         self,
         request: config_20200907_models.GetResourceComplianceByPackRequest,
     ) -> config_20200907_models.GetResourceComplianceByPackResponse:
+        """
+        In this topic, the `cp-541e626622af0087***` compliance package is used as an example. The return result shows a total of 10 resources and seven of them are evaluated as non-compliant.
+        
+        @param request: GetResourceComplianceByPackRequest
+        @return: GetResourceComplianceByPackResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_resource_compliance_by_pack_with_options(request, runtime)
 
     async def get_resource_compliance_by_pack_async(
         self,
         request: config_20200907_models.GetResourceComplianceByPackRequest,
     ) -> config_20200907_models.GetResourceComplianceByPackResponse:
+        """
+        In this topic, the `cp-541e626622af0087***` compliance package is used as an example. The return result shows a total of 10 resources and seven of them are evaluated as non-compliant.
+        
+        @param request: GetResourceComplianceByPackRequest
+        @return: GetResourceComplianceByPackResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_resource_compliance_by_pack_with_options_async(request, runtime)
 
     def get_resource_compliance_group_by_region_with_options(
         self,
         request: config_20200907_models.GetResourceComplianceGroupByRegionRequest,
         runtime: util_models.RuntimeOptions,
@@ -5226,14 +6804,21 @@
         return await self.get_resource_compliance_group_by_resource_type_with_options_async(request, runtime)
 
     def get_resource_compliance_timeline_with_options(
         self,
         request: config_20200907_models.GetResourceComplianceTimelineRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetResourceComplianceTimelineResponse:
+        """
+        The sample request in this topic shows you how to query the compliance timeline of the `new-bucket` resource that resides in the `cn-hangzhou` region. The resource is an Object Storage Service (OSS) bucket. The return result shows the following two timestamps on the compliance timeline: `1625200295276` and `1625200228510`. The first timestamp indicates 12:31:35 on July 2, 2021 (UTC+8) and the second timestamp indicates 12:30:28 on July 2, 2021 (UTC+8).
+        
+        @param request: GetResourceComplianceTimelineRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetResourceComplianceTimelineResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetResourceComplianceTimeline',
@@ -5252,14 +6837,21 @@
         )
 
     async def get_resource_compliance_timeline_with_options_async(
         self,
         request: config_20200907_models.GetResourceComplianceTimelineRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetResourceComplianceTimelineResponse:
+        """
+        The sample request in this topic shows you how to query the compliance timeline of the `new-bucket` resource that resides in the `cn-hangzhou` region. The resource is an Object Storage Service (OSS) bucket. The return result shows the following two timestamps on the compliance timeline: `1625200295276` and `1625200228510`. The first timestamp indicates 12:31:35 on July 2, 2021 (UTC+8) and the second timestamp indicates 12:30:28 on July 2, 2021 (UTC+8).
+        
+        @param request: GetResourceComplianceTimelineRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetResourceComplianceTimelineResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetResourceComplianceTimeline',
@@ -5277,29 +6869,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_resource_compliance_timeline(
         self,
         request: config_20200907_models.GetResourceComplianceTimelineRequest,
     ) -> config_20200907_models.GetResourceComplianceTimelineResponse:
+        """
+        The sample request in this topic shows you how to query the compliance timeline of the `new-bucket` resource that resides in the `cn-hangzhou` region. The resource is an Object Storage Service (OSS) bucket. The return result shows the following two timestamps on the compliance timeline: `1625200295276` and `1625200228510`. The first timestamp indicates 12:31:35 on July 2, 2021 (UTC+8) and the second timestamp indicates 12:30:28 on July 2, 2021 (UTC+8).
+        
+        @param request: GetResourceComplianceTimelineRequest
+        @return: GetResourceComplianceTimelineResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_resource_compliance_timeline_with_options(request, runtime)
 
     async def get_resource_compliance_timeline_async(
         self,
         request: config_20200907_models.GetResourceComplianceTimelineRequest,
     ) -> config_20200907_models.GetResourceComplianceTimelineResponse:
+        """
+        The sample request in this topic shows you how to query the compliance timeline of the `new-bucket` resource that resides in the `cn-hangzhou` region. The resource is an Object Storage Service (OSS) bucket. The return result shows the following two timestamps on the compliance timeline: `1625200295276` and `1625200228510`. The first timestamp indicates 12:31:35 on July 2, 2021 (UTC+8) and the second timestamp indicates 12:30:28 on July 2, 2021 (UTC+8).
+        
+        @param request: GetResourceComplianceTimelineRequest
+        @return: GetResourceComplianceTimelineResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_resource_compliance_timeline_with_options_async(request, runtime)
 
     def get_resource_configuration_timeline_with_options(
         self,
         request: config_20200907_models.GetResourceConfigurationTimelineRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetResourceConfigurationTimelineResponse:
+        """
+        The sample request in this topic shows you how to query the configuration timeline of the `new-bucket` resource that resides in the `cn-hangzhou` region. The new-bucket resource is an Object Storage Service (OSS) bucket. The return result shows that the timestamp when the resource configuration changes is `1624961112000`. The timestamp indicates 18:05:12 on June 29, 2021 (UTC+8).
+        
+        @param request: GetResourceConfigurationTimelineRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetResourceConfigurationTimelineResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetResourceConfigurationTimeline',
@@ -5318,14 +6929,21 @@
         )
 
     async def get_resource_configuration_timeline_with_options_async(
         self,
         request: config_20200907_models.GetResourceConfigurationTimelineRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.GetResourceConfigurationTimelineResponse:
+        """
+        The sample request in this topic shows you how to query the configuration timeline of the `new-bucket` resource that resides in the `cn-hangzhou` region. The new-bucket resource is an Object Storage Service (OSS) bucket. The return result shows that the timestamp when the resource configuration changes is `1624961112000`. The timestamp indicates 18:05:12 on June 29, 2021 (UTC+8).
+        
+        @param request: GetResourceConfigurationTimelineRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetResourceConfigurationTimelineResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetResourceConfigurationTimeline',
@@ -5343,29 +6961,49 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_resource_configuration_timeline(
         self,
         request: config_20200907_models.GetResourceConfigurationTimelineRequest,
     ) -> config_20200907_models.GetResourceConfigurationTimelineResponse:
+        """
+        The sample request in this topic shows you how to query the configuration timeline of the `new-bucket` resource that resides in the `cn-hangzhou` region. The new-bucket resource is an Object Storage Service (OSS) bucket. The return result shows that the timestamp when the resource configuration changes is `1624961112000`. The timestamp indicates 18:05:12 on June 29, 2021 (UTC+8).
+        
+        @param request: GetResourceConfigurationTimelineRequest
+        @return: GetResourceConfigurationTimelineResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_resource_configuration_timeline_with_options(request, runtime)
 
     async def get_resource_configuration_timeline_async(
         self,
         request: config_20200907_models.GetResourceConfigurationTimelineRequest,
     ) -> config_20200907_models.GetResourceConfigurationTimelineResponse:
+        """
+        The sample request in this topic shows you how to query the configuration timeline of the `new-bucket` resource that resides in the `cn-hangzhou` region. The new-bucket resource is an Object Storage Service (OSS) bucket. The return result shows that the timestamp when the resource configuration changes is `1624961112000`. The timestamp indicates 18:05:12 on June 29, 2021 (UTC+8).
+        
+        @param request: GetResourceConfigurationTimelineRequest
+        @return: GetResourceConfigurationTimelineResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_resource_configuration_timeline_with_options_async(request, runtime)
 
     def ignore_aggregate_evaluation_results_with_options(
         self,
         tmp_req: config_20200907_models.IgnoreAggregateEvaluationResultsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.IgnoreAggregateEvaluationResultsResponse:
+        """
+        After you ignore a resource that is evaluated as incompliant by using a rule, the resource is still evaluated by using the rule, but the compliance result is Ignored.
+        This example shows how to ignore the `lb-hp3a3b4ztyfm2plgm****` incompliant resource that is evaluated by using the `cr-7e72626622af0051***` rule in the `120886317861****` member account of the `ca-5b6c626622af008f****` account group. The ID of the region where the resource resides is `cn-beijing`, and the type of the resource is `ACS::SLB::LoadBalancer`.
+        
+        @param tmp_req: IgnoreAggregateEvaluationResultsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: IgnoreAggregateEvaluationResultsResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = config_20200907_models.IgnoreAggregateEvaluationResultsShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.resources):
             request.resources_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.resources, 'Resources', 'json')
         body = {}
         if not UtilClient.is_unset(request.aggregator_id):
@@ -5398,14 +7036,22 @@
         )
 
     async def ignore_aggregate_evaluation_results_with_options_async(
         self,
         tmp_req: config_20200907_models.IgnoreAggregateEvaluationResultsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.IgnoreAggregateEvaluationResultsResponse:
+        """
+        After you ignore a resource that is evaluated as incompliant by using a rule, the resource is still evaluated by using the rule, but the compliance result is Ignored.
+        This example shows how to ignore the `lb-hp3a3b4ztyfm2plgm****` incompliant resource that is evaluated by using the `cr-7e72626622af0051***` rule in the `120886317861****` member account of the `ca-5b6c626622af008f****` account group. The ID of the region where the resource resides is `cn-beijing`, and the type of the resource is `ACS::SLB::LoadBalancer`.
+        
+        @param tmp_req: IgnoreAggregateEvaluationResultsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: IgnoreAggregateEvaluationResultsResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = config_20200907_models.IgnoreAggregateEvaluationResultsShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.resources):
             request.resources_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.resources, 'Resources', 'json')
         body = {}
         if not UtilClient.is_unset(request.aggregator_id):
@@ -5437,29 +7083,51 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def ignore_aggregate_evaluation_results(
         self,
         request: config_20200907_models.IgnoreAggregateEvaluationResultsRequest,
     ) -> config_20200907_models.IgnoreAggregateEvaluationResultsResponse:
+        """
+        After you ignore a resource that is evaluated as incompliant by using a rule, the resource is still evaluated by using the rule, but the compliance result is Ignored.
+        This example shows how to ignore the `lb-hp3a3b4ztyfm2plgm****` incompliant resource that is evaluated by using the `cr-7e72626622af0051***` rule in the `120886317861****` member account of the `ca-5b6c626622af008f****` account group. The ID of the region where the resource resides is `cn-beijing`, and the type of the resource is `ACS::SLB::LoadBalancer`.
+        
+        @param request: IgnoreAggregateEvaluationResultsRequest
+        @return: IgnoreAggregateEvaluationResultsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.ignore_aggregate_evaluation_results_with_options(request, runtime)
 
     async def ignore_aggregate_evaluation_results_async(
         self,
         request: config_20200907_models.IgnoreAggregateEvaluationResultsRequest,
     ) -> config_20200907_models.IgnoreAggregateEvaluationResultsResponse:
+        """
+        After you ignore a resource that is evaluated as incompliant by using a rule, the resource is still evaluated by using the rule, but the compliance result is Ignored.
+        This example shows how to ignore the `lb-hp3a3b4ztyfm2plgm****` incompliant resource that is evaluated by using the `cr-7e72626622af0051***` rule in the `120886317861****` member account of the `ca-5b6c626622af008f****` account group. The ID of the region where the resource resides is `cn-beijing`, and the type of the resource is `ACS::SLB::LoadBalancer`.
+        
+        @param request: IgnoreAggregateEvaluationResultsRequest
+        @return: IgnoreAggregateEvaluationResultsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.ignore_aggregate_evaluation_results_with_options_async(request, runtime)
 
     def ignore_evaluation_results_with_options(
         self,
         tmp_req: config_20200907_models.IgnoreEvaluationResultsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.IgnoreEvaluationResultsResponse:
+        """
+        After you ignore a resource that is evaluated as incompliant by using a rule, the resource is still evaluated by using the rule, but the compliance result is Ignored.
+        This example shows how to ignore the `lb-hp3a3b4ztyfm2plgm****` resource that is evaluated as incompliant by using the `cr-7e72626622af0051****` rule in the `100931896542****` account. The ID of the region in which the resource resides is `cn-beijing`, and the type of the resource is `ACS::SLB::LoadBalancer`.
+        
+        @param tmp_req: IgnoreEvaluationResultsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: IgnoreEvaluationResultsResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = config_20200907_models.IgnoreEvaluationResultsShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.resources):
             request.resources_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.resources, 'Resources', 'json')
         body = {}
         if not UtilClient.is_unset(request.config_rule_id):
@@ -5490,14 +7158,22 @@
         )
 
     async def ignore_evaluation_results_with_options_async(
         self,
         tmp_req: config_20200907_models.IgnoreEvaluationResultsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.IgnoreEvaluationResultsResponse:
+        """
+        After you ignore a resource that is evaluated as incompliant by using a rule, the resource is still evaluated by using the rule, but the compliance result is Ignored.
+        This example shows how to ignore the `lb-hp3a3b4ztyfm2plgm****` resource that is evaluated as incompliant by using the `cr-7e72626622af0051****` rule in the `100931896542****` account. The ID of the region in which the resource resides is `cn-beijing`, and the type of the resource is `ACS::SLB::LoadBalancer`.
+        
+        @param tmp_req: IgnoreEvaluationResultsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: IgnoreEvaluationResultsResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = config_20200907_models.IgnoreEvaluationResultsShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.resources):
             request.resources_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.resources, 'Resources', 'json')
         body = {}
         if not UtilClient.is_unset(request.config_rule_id):
@@ -5527,29 +7203,50 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def ignore_evaluation_results(
         self,
         request: config_20200907_models.IgnoreEvaluationResultsRequest,
     ) -> config_20200907_models.IgnoreEvaluationResultsResponse:
+        """
+        After you ignore a resource that is evaluated as incompliant by using a rule, the resource is still evaluated by using the rule, but the compliance result is Ignored.
+        This example shows how to ignore the `lb-hp3a3b4ztyfm2plgm****` resource that is evaluated as incompliant by using the `cr-7e72626622af0051****` rule in the `100931896542****` account. The ID of the region in which the resource resides is `cn-beijing`, and the type of the resource is `ACS::SLB::LoadBalancer`.
+        
+        @param request: IgnoreEvaluationResultsRequest
+        @return: IgnoreEvaluationResultsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.ignore_evaluation_results_with_options(request, runtime)
 
     async def ignore_evaluation_results_async(
         self,
         request: config_20200907_models.IgnoreEvaluationResultsRequest,
     ) -> config_20200907_models.IgnoreEvaluationResultsResponse:
+        """
+        After you ignore a resource that is evaluated as incompliant by using a rule, the resource is still evaluated by using the rule, but the compliance result is Ignored.
+        This example shows how to ignore the `lb-hp3a3b4ztyfm2plgm****` resource that is evaluated as incompliant by using the `cr-7e72626622af0051****` rule in the `100931896542****` account. The ID of the region in which the resource resides is `cn-beijing`, and the type of the resource is `ACS::SLB::LoadBalancer`.
+        
+        @param request: IgnoreEvaluationResultsRequest
+        @return: IgnoreEvaluationResultsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.ignore_evaluation_results_with_options_async(request, runtime)
 
     def list_aggregate_compliance_packs_with_options(
         self,
         request: config_20200907_models.ListAggregateCompliancePacksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ListAggregateCompliancePacksResponse:
+        """
+        In this topic, the `ca-f632626622af0079***` account group is used as an example. The return result shows one compliance package whose ID is `cp-fdc8626622af00f9****`.
+        
+        @param request: ListAggregateCompliancePacksRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListAggregateCompliancePacksResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
@@ -5576,14 +7273,21 @@
         )
 
     async def list_aggregate_compliance_packs_with_options_async(
         self,
         request: config_20200907_models.ListAggregateCompliancePacksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ListAggregateCompliancePacksResponse:
+        """
+        In this topic, the `ca-f632626622af0079***` account group is used as an example. The return result shows one compliance package whose ID is `cp-fdc8626622af00f9****`.
+        
+        @param request: ListAggregateCompliancePacksRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListAggregateCompliancePacksResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
@@ -5609,21 +7313,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_aggregate_compliance_packs(
         self,
         request: config_20200907_models.ListAggregateCompliancePacksRequest,
     ) -> config_20200907_models.ListAggregateCompliancePacksResponse:
+        """
+        In this topic, the `ca-f632626622af0079***` account group is used as an example. The return result shows one compliance package whose ID is `cp-fdc8626622af00f9****`.
+        
+        @param request: ListAggregateCompliancePacksRequest
+        @return: ListAggregateCompliancePacksResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_aggregate_compliance_packs_with_options(request, runtime)
 
     async def list_aggregate_compliance_packs_async(
         self,
         request: config_20200907_models.ListAggregateCompliancePacksRequest,
     ) -> config_20200907_models.ListAggregateCompliancePacksResponse:
+        """
+        In this topic, the `ca-f632626622af0079***` account group is used as an example. The return result shows one compliance package whose ID is `cp-fdc8626622af00f9****`.
+        
+        @param request: ListAggregateCompliancePacksRequest
+        @return: ListAggregateCompliancePacksResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_aggregate_compliance_packs_with_options_async(request, runtime)
 
     def list_aggregate_config_delivery_channels_with_options(
         self,
         request: config_20200907_models.ListAggregateConfigDeliveryChannelsRequest,
         runtime: util_models.RuntimeOptions,
@@ -5698,14 +7414,21 @@
         return await self.list_aggregate_config_delivery_channels_with_options_async(request, runtime)
 
     def list_aggregate_config_rule_evaluation_results_with_options(
         self,
         request: config_20200907_models.ListAggregateConfigRuleEvaluationResultsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ListAggregateConfigRuleEvaluationResultsResponse:
+        """
+        This topic provides an example on how to query the compliance evaluation results of resources based on the `cr-888f626622af00ae***` rule in the `ca-d1e3326622af00cb****` account group. The returned result indicates that the `Bucket-test` resource is evaluated as `NON_COMPLIANT` by using the rule. The resource is an Object Storage Service (OSS) bucket.
+        
+        @param request: ListAggregateConfigRuleEvaluationResultsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListAggregateConfigRuleEvaluationResultsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.compliance_pack_id):
             query['CompliancePackId'] = request.compliance_pack_id
         if not UtilClient.is_unset(request.compliance_type):
@@ -5714,14 +7437,16 @@
             query['ConfigRuleId'] = request.config_rule_id
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.regions):
             query['Regions'] = request.regions
+        if not UtilClient.is_unset(request.resource_account_id):
+            query['ResourceAccountId'] = request.resource_account_id
         if not UtilClient.is_unset(request.resource_group_ids):
             query['ResourceGroupIds'] = request.resource_group_ids
         if not UtilClient.is_unset(request.resource_owner_id):
             query['ResourceOwnerId'] = request.resource_owner_id
         if not UtilClient.is_unset(request.resource_types):
             query['ResourceTypes'] = request.resource_types
         req = open_api_models.OpenApiRequest(
@@ -5744,14 +7469,21 @@
         )
 
     async def list_aggregate_config_rule_evaluation_results_with_options_async(
         self,
         request: config_20200907_models.ListAggregateConfigRuleEvaluationResultsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ListAggregateConfigRuleEvaluationResultsResponse:
+        """
+        This topic provides an example on how to query the compliance evaluation results of resources based on the `cr-888f626622af00ae***` rule in the `ca-d1e3326622af00cb****` account group. The returned result indicates that the `Bucket-test` resource is evaluated as `NON_COMPLIANT` by using the rule. The resource is an Object Storage Service (OSS) bucket.
+        
+        @param request: ListAggregateConfigRuleEvaluationResultsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListAggregateConfigRuleEvaluationResultsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.compliance_pack_id):
             query['CompliancePackId'] = request.compliance_pack_id
         if not UtilClient.is_unset(request.compliance_type):
@@ -5760,14 +7492,16 @@
             query['ConfigRuleId'] = request.config_rule_id
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.regions):
             query['Regions'] = request.regions
+        if not UtilClient.is_unset(request.resource_account_id):
+            query['ResourceAccountId'] = request.resource_account_id
         if not UtilClient.is_unset(request.resource_group_ids):
             query['ResourceGroupIds'] = request.resource_group_ids
         if not UtilClient.is_unset(request.resource_owner_id):
             query['ResourceOwnerId'] = request.resource_owner_id
         if not UtilClient.is_unset(request.resource_types):
             query['ResourceTypes'] = request.resource_types
         req = open_api_models.OpenApiRequest(
@@ -5789,29 +7523,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_aggregate_config_rule_evaluation_results(
         self,
         request: config_20200907_models.ListAggregateConfigRuleEvaluationResultsRequest,
     ) -> config_20200907_models.ListAggregateConfigRuleEvaluationResultsResponse:
+        """
+        This topic provides an example on how to query the compliance evaluation results of resources based on the `cr-888f626622af00ae***` rule in the `ca-d1e3326622af00cb****` account group. The returned result indicates that the `Bucket-test` resource is evaluated as `NON_COMPLIANT` by using the rule. The resource is an Object Storage Service (OSS) bucket.
+        
+        @param request: ListAggregateConfigRuleEvaluationResultsRequest
+        @return: ListAggregateConfigRuleEvaluationResultsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_aggregate_config_rule_evaluation_results_with_options(request, runtime)
 
     async def list_aggregate_config_rule_evaluation_results_async(
         self,
         request: config_20200907_models.ListAggregateConfigRuleEvaluationResultsRequest,
     ) -> config_20200907_models.ListAggregateConfigRuleEvaluationResultsResponse:
+        """
+        This topic provides an example on how to query the compliance evaluation results of resources based on the `cr-888f626622af00ae***` rule in the `ca-d1e3326622af00cb****` account group. The returned result indicates that the `Bucket-test` resource is evaluated as `NON_COMPLIANT` by using the rule. The resource is an Object Storage Service (OSS) bucket.
+        
+        @param request: ListAggregateConfigRuleEvaluationResultsRequest
+        @return: ListAggregateConfigRuleEvaluationResultsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_aggregate_config_rule_evaluation_results_with_options_async(request, runtime)
 
     def list_aggregate_config_rules_with_options(
         self,
         request: config_20200907_models.ListAggregateConfigRulesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ListAggregateConfigRulesResponse:
+        """
+        This topic provides an example on how to query the rules in an account group whose ID is `ca-f632626622af0079***`. The return result shows a total of one rule and two evaluated resources. The resources are both evaluated as `COMPLIANT`.
+        
+        @param request: ListAggregateConfigRulesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListAggregateConfigRulesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.compliance_type):
             query['ComplianceType'] = request.compliance_type
         if not UtilClient.is_unset(request.config_rule_name):
@@ -5820,14 +7573,16 @@
             query['ConfigRuleState'] = request.config_rule_state
         if not UtilClient.is_unset(request.keyword):
             query['Keyword'] = request.keyword
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.resource_types):
+            query['ResourceTypes'] = request.resource_types
         if not UtilClient.is_unset(request.risk_level):
             query['RiskLevel'] = request.risk_level
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListAggregateConfigRules',
@@ -5846,14 +7601,21 @@
         )
 
     async def list_aggregate_config_rules_with_options_async(
         self,
         request: config_20200907_models.ListAggregateConfigRulesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ListAggregateConfigRulesResponse:
+        """
+        This topic provides an example on how to query the rules in an account group whose ID is `ca-f632626622af0079***`. The return result shows a total of one rule and two evaluated resources. The resources are both evaluated as `COMPLIANT`.
+        
+        @param request: ListAggregateConfigRulesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListAggregateConfigRulesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.compliance_type):
             query['ComplianceType'] = request.compliance_type
         if not UtilClient.is_unset(request.config_rule_name):
@@ -5862,14 +7624,16 @@
             query['ConfigRuleState'] = request.config_rule_state
         if not UtilClient.is_unset(request.keyword):
             query['Keyword'] = request.keyword
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.resource_types):
+            query['ResourceTypes'] = request.resource_types
         if not UtilClient.is_unset(request.risk_level):
             query['RiskLevel'] = request.risk_level
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListAggregateConfigRules',
@@ -5887,39 +7651,60 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_aggregate_config_rules(
         self,
         request: config_20200907_models.ListAggregateConfigRulesRequest,
     ) -> config_20200907_models.ListAggregateConfigRulesResponse:
+        """
+        This topic provides an example on how to query the rules in an account group whose ID is `ca-f632626622af0079***`. The return result shows a total of one rule and two evaluated resources. The resources are both evaluated as `COMPLIANT`.
+        
+        @param request: ListAggregateConfigRulesRequest
+        @return: ListAggregateConfigRulesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_aggregate_config_rules_with_options(request, runtime)
 
     async def list_aggregate_config_rules_async(
         self,
         request: config_20200907_models.ListAggregateConfigRulesRequest,
     ) -> config_20200907_models.ListAggregateConfigRulesResponse:
+        """
+        This topic provides an example on how to query the rules in an account group whose ID is `ca-f632626622af0079***`. The return result shows a total of one rule and two evaluated resources. The resources are both evaluated as `COMPLIANT`.
+        
+        @param request: ListAggregateConfigRulesRequest
+        @return: ListAggregateConfigRulesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_aggregate_config_rules_with_options_async(request, runtime)
 
     def list_aggregate_discovered_resources_with_options(
         self,
         request: config_20200907_models.ListAggregateDiscoveredResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ListAggregateDiscoveredResourcesResponse:
+        """
+        This example shows how to query the resources in the `ca-c560626622af0005***` account group. The response shows that the account group contains eight resources.
+        
+        @param request: ListAggregateDiscoveredResourcesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListAggregateDiscoveredResourcesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.regions):
             query['Regions'] = request.regions
+        if not UtilClient.is_unset(request.resource_account_id):
+            query['ResourceAccountId'] = request.resource_account_id
         if not UtilClient.is_unset(request.resource_deleted):
             query['ResourceDeleted'] = request.resource_deleted
         if not UtilClient.is_unset(request.resource_id):
             query['ResourceId'] = request.resource_id
         if not UtilClient.is_unset(request.resource_owner_id):
             query['ResourceOwnerId'] = request.resource_owner_id
         if not UtilClient.is_unset(request.resource_types):
@@ -5944,24 +7729,33 @@
         )
 
     async def list_aggregate_discovered_resources_with_options_async(
         self,
         request: config_20200907_models.ListAggregateDiscoveredResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ListAggregateDiscoveredResourcesResponse:
+        """
+        This example shows how to query the resources in the `ca-c560626622af0005***` account group. The response shows that the account group contains eight resources.
+        
+        @param request: ListAggregateDiscoveredResourcesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListAggregateDiscoveredResourcesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.regions):
             query['Regions'] = request.regions
+        if not UtilClient.is_unset(request.resource_account_id):
+            query['ResourceAccountId'] = request.resource_account_id
         if not UtilClient.is_unset(request.resource_deleted):
             query['ResourceDeleted'] = request.resource_deleted
         if not UtilClient.is_unset(request.resource_id):
             query['ResourceId'] = request.resource_id
         if not UtilClient.is_unset(request.resource_owner_id):
             query['ResourceOwnerId'] = request.resource_owner_id
         if not UtilClient.is_unset(request.resource_types):
@@ -5985,29 +7779,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_aggregate_discovered_resources(
         self,
         request: config_20200907_models.ListAggregateDiscoveredResourcesRequest,
     ) -> config_20200907_models.ListAggregateDiscoveredResourcesResponse:
+        """
+        This example shows how to query the resources in the `ca-c560626622af0005***` account group. The response shows that the account group contains eight resources.
+        
+        @param request: ListAggregateDiscoveredResourcesRequest
+        @return: ListAggregateDiscoveredResourcesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_aggregate_discovered_resources_with_options(request, runtime)
 
     async def list_aggregate_discovered_resources_async(
         self,
         request: config_20200907_models.ListAggregateDiscoveredResourcesRequest,
     ) -> config_20200907_models.ListAggregateDiscoveredResourcesResponse:
+        """
+        This example shows how to query the resources in the `ca-c560626622af0005***` account group. The response shows that the account group contains eight resources.
+        
+        @param request: ListAggregateDiscoveredResourcesRequest
+        @return: ListAggregateDiscoveredResourcesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_aggregate_discovered_resources_with_options_async(request, runtime)
 
     def list_aggregate_remediations_with_options(
         self,
         request: config_20200907_models.ListAggregateRemediationsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ListAggregateRemediationsResponse:
+        """
+        The sample request in this topic shows you how to query the remediation setting of the rule whose ID is `cr-6b7c626622af00b4***` in the account group whose ID is `ca-6b4a626622af0012****`.
+        
+        @param request: ListAggregateRemediationsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListAggregateRemediationsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.config_rule_ids):
             query['ConfigRuleIds'] = request.config_rule_ids
         req = open_api_models.OpenApiRequest(
@@ -6030,14 +7843,21 @@
         )
 
     async def list_aggregate_remediations_with_options_async(
         self,
         request: config_20200907_models.ListAggregateRemediationsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ListAggregateRemediationsResponse:
+        """
+        The sample request in this topic shows you how to query the remediation setting of the rule whose ID is `cr-6b7c626622af00b4***` in the account group whose ID is `ca-6b4a626622af0012****`.
+        
+        @param request: ListAggregateRemediationsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListAggregateRemediationsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.config_rule_ids):
             query['ConfigRuleIds'] = request.config_rule_ids
         req = open_api_models.OpenApiRequest(
@@ -6059,29 +7879,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_aggregate_remediations(
         self,
         request: config_20200907_models.ListAggregateRemediationsRequest,
     ) -> config_20200907_models.ListAggregateRemediationsResponse:
+        """
+        The sample request in this topic shows you how to query the remediation setting of the rule whose ID is `cr-6b7c626622af00b4***` in the account group whose ID is `ca-6b4a626622af0012****`.
+        
+        @param request: ListAggregateRemediationsRequest
+        @return: ListAggregateRemediationsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_aggregate_remediations_with_options(request, runtime)
 
     async def list_aggregate_remediations_async(
         self,
         request: config_20200907_models.ListAggregateRemediationsRequest,
     ) -> config_20200907_models.ListAggregateRemediationsResponse:
+        """
+        The sample request in this topic shows you how to query the remediation setting of the rule whose ID is `cr-6b7c626622af00b4***` in the account group whose ID is `ca-6b4a626622af0012****`.
+        
+        @param request: ListAggregateRemediationsRequest
+        @return: ListAggregateRemediationsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_aggregate_remediations_with_options_async(request, runtime)
 
     def list_aggregate_resource_evaluation_results_with_options(
         self,
         request: config_20200907_models.ListAggregateResourceEvaluationResultsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ListAggregateResourceEvaluationResultsResponse:
+        """
+        This example shows how to query the compliance evaluation result of the `23642660635396***` resource in the `ca-7f00626622af0041****` account group. The resource is a RAM user. The returned result indicates that the resource is evaluated as `NON_COMPLIANT` by using the `cr-7f7d626622af0041****` rule.
+        
+        @param request: ListAggregateResourceEvaluationResultsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListAggregateResourceEvaluationResultsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.compliance_type):
             query['ComplianceType'] = request.compliance_type
         if not UtilClient.is_unset(request.max_results):
@@ -6114,14 +7953,21 @@
         )
 
     async def list_aggregate_resource_evaluation_results_with_options_async(
         self,
         request: config_20200907_models.ListAggregateResourceEvaluationResultsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ListAggregateResourceEvaluationResultsResponse:
+        """
+        This example shows how to query the compliance evaluation result of the `23642660635396***` resource in the `ca-7f00626622af0041****` account group. The resource is a RAM user. The returned result indicates that the resource is evaluated as `NON_COMPLIANT` by using the `cr-7f7d626622af0041****` rule.
+        
+        @param request: ListAggregateResourceEvaluationResultsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListAggregateResourceEvaluationResultsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.compliance_type):
             query['ComplianceType'] = request.compliance_type
         if not UtilClient.is_unset(request.max_results):
@@ -6153,29 +7999,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_aggregate_resource_evaluation_results(
         self,
         request: config_20200907_models.ListAggregateResourceEvaluationResultsRequest,
     ) -> config_20200907_models.ListAggregateResourceEvaluationResultsResponse:
+        """
+        This example shows how to query the compliance evaluation result of the `23642660635396***` resource in the `ca-7f00626622af0041****` account group. The resource is a RAM user. The returned result indicates that the resource is evaluated as `NON_COMPLIANT` by using the `cr-7f7d626622af0041****` rule.
+        
+        @param request: ListAggregateResourceEvaluationResultsRequest
+        @return: ListAggregateResourceEvaluationResultsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_aggregate_resource_evaluation_results_with_options(request, runtime)
 
     async def list_aggregate_resource_evaluation_results_async(
         self,
         request: config_20200907_models.ListAggregateResourceEvaluationResultsRequest,
     ) -> config_20200907_models.ListAggregateResourceEvaluationResultsResponse:
+        """
+        This example shows how to query the compliance evaluation result of the `23642660635396***` resource in the `ca-7f00626622af0041****` account group. The resource is a RAM user. The returned result indicates that the resource is evaluated as `NON_COMPLIANT` by using the `cr-7f7d626622af0041****` rule.
+        
+        @param request: ListAggregateResourceEvaluationResultsRequest
+        @return: ListAggregateResourceEvaluationResultsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_aggregate_resource_evaluation_results_with_options_async(request, runtime)
 
     def list_aggregators_with_options(
         self,
         request: config_20200907_models.ListAggregatorsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ListAggregatorsResponse:
+        """
+        The sample request in this topic shows you how to query account groups. A maximum of 10 entries can be returned for the request. As shown in the responses, the account group returned is named as `Test_Group`, its description is `Test account group`, and it is of the `CUSTOM` type, which indicates a custom account group. The account group contains two member accounts.
+        
+        @param request: ListAggregatorsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListAggregatorsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         req = open_api_models.OpenApiRequest(
@@ -6198,14 +8063,21 @@
         )
 
     async def list_aggregators_with_options_async(
         self,
         request: config_20200907_models.ListAggregatorsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ListAggregatorsResponse:
+        """
+        The sample request in this topic shows you how to query account groups. A maximum of 10 entries can be returned for the request. As shown in the responses, the account group returned is named as `Test_Group`, its description is `Test account group`, and it is of the `CUSTOM` type, which indicates a custom account group. The account group contains two member accounts.
+        
+        @param request: ListAggregatorsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListAggregatorsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         req = open_api_models.OpenApiRequest(
@@ -6227,37 +8099,58 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_aggregators(
         self,
         request: config_20200907_models.ListAggregatorsRequest,
     ) -> config_20200907_models.ListAggregatorsResponse:
+        """
+        The sample request in this topic shows you how to query account groups. A maximum of 10 entries can be returned for the request. As shown in the responses, the account group returned is named as `Test_Group`, its description is `Test account group`, and it is of the `CUSTOM` type, which indicates a custom account group. The account group contains two member accounts.
+        
+        @param request: ListAggregatorsRequest
+        @return: ListAggregatorsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_aggregators_with_options(request, runtime)
 
     async def list_aggregators_async(
         self,
         request: config_20200907_models.ListAggregatorsRequest,
     ) -> config_20200907_models.ListAggregatorsResponse:
+        """
+        The sample request in this topic shows you how to query account groups. A maximum of 10 entries can be returned for the request. As shown in the responses, the account group returned is named as `Test_Group`, its description is `Test account group`, and it is of the `CUSTOM` type, which indicates a custom account group. The account group contains two member accounts.
+        
+        @param request: ListAggregatorsRequest
+        @return: ListAggregatorsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_aggregators_with_options_async(request, runtime)
 
     def list_compliance_pack_templates_with_options(
         self,
         request: config_20200907_models.ListCompliancePackTemplatesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ListCompliancePackTemplatesResponse:
+        """
+        This topic provides an example on how to query the details of a compliance package template whose ID is `ct-d254ff4e06a300cf***`. The returned result indicates that the template name is `BestPracticesForNetwork`, the template ID is `ct-d254ff4e06a300cf****`, and the ID of the managed rule of the template is `slb-servercertificate-expired-check`.
+        
+        @param request: ListCompliancePackTemplatesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListCompliancePackTemplatesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.compliance_pack_template_id):
             query['CompliancePackTemplateId'] = request.compliance_pack_template_id
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.resource_types):
+            query['ResourceTypes'] = request.resource_types
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListCompliancePackTemplates',
             version='2020-09-07',
             protocol='HTTPS',
@@ -6274,22 +8167,31 @@
         )
 
     async def list_compliance_pack_templates_with_options_async(
         self,
         request: config_20200907_models.ListCompliancePackTemplatesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ListCompliancePackTemplatesResponse:
+        """
+        This topic provides an example on how to query the details of a compliance package template whose ID is `ct-d254ff4e06a300cf***`. The returned result indicates that the template name is `BestPracticesForNetwork`, the template ID is `ct-d254ff4e06a300cf****`, and the ID of the managed rule of the template is `slb-servercertificate-expired-check`.
+        
+        @param request: ListCompliancePackTemplatesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListCompliancePackTemplatesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.compliance_pack_template_id):
             query['CompliancePackTemplateId'] = request.compliance_pack_template_id
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.resource_types):
+            query['ResourceTypes'] = request.resource_types
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListCompliancePackTemplates',
             version='2020-09-07',
             protocol='HTTPS',
@@ -6305,29 +8207,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_compliance_pack_templates(
         self,
         request: config_20200907_models.ListCompliancePackTemplatesRequest,
     ) -> config_20200907_models.ListCompliancePackTemplatesResponse:
+        """
+        This topic provides an example on how to query the details of a compliance package template whose ID is `ct-d254ff4e06a300cf***`. The returned result indicates that the template name is `BestPracticesForNetwork`, the template ID is `ct-d254ff4e06a300cf****`, and the ID of the managed rule of the template is `slb-servercertificate-expired-check`.
+        
+        @param request: ListCompliancePackTemplatesRequest
+        @return: ListCompliancePackTemplatesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_compliance_pack_templates_with_options(request, runtime)
 
     async def list_compliance_pack_templates_async(
         self,
         request: config_20200907_models.ListCompliancePackTemplatesRequest,
     ) -> config_20200907_models.ListCompliancePackTemplatesResponse:
+        """
+        This topic provides an example on how to query the details of a compliance package template whose ID is `ct-d254ff4e06a300cf***`. The returned result indicates that the template name is `BestPracticesForNetwork`, the template ID is `ct-d254ff4e06a300cf****`, and the ID of the managed rule of the template is `slb-servercertificate-expired-check`.
+        
+        @param request: ListCompliancePackTemplatesRequest
+        @return: ListCompliancePackTemplatesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_compliance_pack_templates_with_options_async(request, runtime)
 
     def list_compliance_packs_with_options(
         self,
         request: config_20200907_models.ListCompliancePacksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ListCompliancePacksResponse:
+        """
+        This topic provides an example of how to query compliance packages. The return result shows the details of the `cp-fdc8626622af00f9***` compliance package.
+        
+        @param request: ListCompliancePacksRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListCompliancePacksResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.status):
@@ -6352,14 +8273,21 @@
         )
 
     async def list_compliance_packs_with_options_async(
         self,
         request: config_20200907_models.ListCompliancePacksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ListCompliancePacksResponse:
+        """
+        This topic provides an example of how to query compliance packages. The return result shows the details of the `cp-fdc8626622af00f9***` compliance package.
+        
+        @param request: ListCompliancePacksRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListCompliancePacksResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.status):
@@ -6383,21 +8311,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_compliance_packs(
         self,
         request: config_20200907_models.ListCompliancePacksRequest,
     ) -> config_20200907_models.ListCompliancePacksResponse:
+        """
+        This topic provides an example of how to query compliance packages. The return result shows the details of the `cp-fdc8626622af00f9***` compliance package.
+        
+        @param request: ListCompliancePacksRequest
+        @return: ListCompliancePacksResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_compliance_packs_with_options(request, runtime)
 
     async def list_compliance_packs_async(
         self,
         request: config_20200907_models.ListCompliancePacksRequest,
     ) -> config_20200907_models.ListCompliancePacksResponse:
+        """
+        This topic provides an example of how to query compliance packages. The return result shows the details of the `cp-fdc8626622af00f9***` compliance package.
+        
+        @param request: ListCompliancePacksRequest
+        @return: ListCompliancePacksResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_compliance_packs_with_options_async(request, runtime)
 
     def list_config_delivery_channels_with_options(
         self,
         request: config_20200907_models.ListConfigDeliveryChannelsRequest,
         runtime: util_models.RuntimeOptions,
@@ -6468,14 +8408,21 @@
         return await self.list_config_delivery_channels_with_options_async(request, runtime)
 
     def list_config_rule_evaluation_results_with_options(
         self,
         request: config_20200907_models.ListConfigRuleEvaluationResultsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ListConfigRuleEvaluationResultsResponse:
+        """
+        This topic provides an example on how to query the compliance evaluation result of resources based on a rule whose ID is `cr-cac56457e0d900d3***`. The returned result indicates that the `i-hp3e4kvhzqn2s11t****` resource is evaluated as `NON_COMPLIANT` by using the rule. The resource is an Elastic Compute Service (ECS) instance.
+        
+        @param request: ListConfigRuleEvaluationResultsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListConfigRuleEvaluationResultsResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListConfigRuleEvaluationResults',
@@ -6494,14 +8441,21 @@
         )
 
     async def list_config_rule_evaluation_results_with_options_async(
         self,
         request: config_20200907_models.ListConfigRuleEvaluationResultsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ListConfigRuleEvaluationResultsResponse:
+        """
+        This topic provides an example on how to query the compliance evaluation result of resources based on a rule whose ID is `cr-cac56457e0d900d3***`. The returned result indicates that the `i-hp3e4kvhzqn2s11t****` resource is evaluated as `NON_COMPLIANT` by using the rule. The resource is an Elastic Compute Service (ECS) instance.
+        
+        @param request: ListConfigRuleEvaluationResultsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListConfigRuleEvaluationResultsResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListConfigRuleEvaluationResults',
@@ -6519,29 +8473,146 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_config_rule_evaluation_results(
         self,
         request: config_20200907_models.ListConfigRuleEvaluationResultsRequest,
     ) -> config_20200907_models.ListConfigRuleEvaluationResultsResponse:
+        """
+        This topic provides an example on how to query the compliance evaluation result of resources based on a rule whose ID is `cr-cac56457e0d900d3***`. The returned result indicates that the `i-hp3e4kvhzqn2s11t****` resource is evaluated as `NON_COMPLIANT` by using the rule. The resource is an Elastic Compute Service (ECS) instance.
+        
+        @param request: ListConfigRuleEvaluationResultsRequest
+        @return: ListConfigRuleEvaluationResultsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_config_rule_evaluation_results_with_options(request, runtime)
 
     async def list_config_rule_evaluation_results_async(
         self,
         request: config_20200907_models.ListConfigRuleEvaluationResultsRequest,
     ) -> config_20200907_models.ListConfigRuleEvaluationResultsResponse:
+        """
+        This topic provides an example on how to query the compliance evaluation result of resources based on a rule whose ID is `cr-cac56457e0d900d3***`. The returned result indicates that the `i-hp3e4kvhzqn2s11t****` resource is evaluated as `NON_COMPLIANT` by using the rule. The resource is an Elastic Compute Service (ECS) instance.
+        
+        @param request: ListConfigRuleEvaluationResultsRequest
+        @return: ListConfigRuleEvaluationResultsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_config_rule_evaluation_results_with_options_async(request, runtime)
 
+    def list_config_rules_with_options(
+        self,
+        request: config_20200907_models.ListConfigRulesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> config_20200907_models.ListConfigRulesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.compliance_type):
+            query['ComplianceType'] = request.compliance_type
+        if not UtilClient.is_unset(request.config_rule_name):
+            query['ConfigRuleName'] = request.config_rule_name
+        if not UtilClient.is_unset(request.config_rule_state):
+            query['ConfigRuleState'] = request.config_rule_state
+        if not UtilClient.is_unset(request.keyword):
+            query['Keyword'] = request.keyword
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.resource_types):
+            query['ResourceTypes'] = request.resource_types
+        if not UtilClient.is_unset(request.risk_level):
+            query['RiskLevel'] = request.risk_level
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListConfigRules',
+            version='2020-09-07',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            config_20200907_models.ListConfigRulesResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_config_rules_with_options_async(
+        self,
+        request: config_20200907_models.ListConfigRulesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> config_20200907_models.ListConfigRulesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.compliance_type):
+            query['ComplianceType'] = request.compliance_type
+        if not UtilClient.is_unset(request.config_rule_name):
+            query['ConfigRuleName'] = request.config_rule_name
+        if not UtilClient.is_unset(request.config_rule_state):
+            query['ConfigRuleState'] = request.config_rule_state
+        if not UtilClient.is_unset(request.keyword):
+            query['Keyword'] = request.keyword
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.resource_types):
+            query['ResourceTypes'] = request.resource_types
+        if not UtilClient.is_unset(request.risk_level):
+            query['RiskLevel'] = request.risk_level
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListConfigRules',
+            version='2020-09-07',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            config_20200907_models.ListConfigRulesResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_config_rules(
+        self,
+        request: config_20200907_models.ListConfigRulesRequest,
+    ) -> config_20200907_models.ListConfigRulesResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_config_rules_with_options(request, runtime)
+
+    async def list_config_rules_async(
+        self,
+        request: config_20200907_models.ListConfigRulesRequest,
+    ) -> config_20200907_models.ListConfigRulesResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_config_rules_with_options_async(request, runtime)
+
     def list_discovered_resources_with_options(
         self,
         request: config_20200907_models.ListDiscoveredResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ListDiscoveredResourcesResponse:
+        """
+        This topic provides an example on how to call the ListDiscoveredResources operation to query the resources in the current Alibaba Cloud account. The returned result indicates that a total of eight resources exist in the account.
+        
+        @param request: ListDiscoveredResourcesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListDiscoveredResourcesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.regions):
@@ -6572,14 +8643,21 @@
         )
 
     async def list_discovered_resources_with_options_async(
         self,
         request: config_20200907_models.ListDiscoveredResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ListDiscoveredResourcesResponse:
+        """
+        This topic provides an example on how to call the ListDiscoveredResources operation to query the resources in the current Alibaba Cloud account. The returned result indicates that a total of eight resources exist in the account.
+        
+        @param request: ListDiscoveredResourcesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListDiscoveredResourcesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.regions):
@@ -6609,37 +8687,58 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_discovered_resources(
         self,
         request: config_20200907_models.ListDiscoveredResourcesRequest,
     ) -> config_20200907_models.ListDiscoveredResourcesResponse:
+        """
+        This topic provides an example on how to call the ListDiscoveredResources operation to query the resources in the current Alibaba Cloud account. The returned result indicates that a total of eight resources exist in the account.
+        
+        @param request: ListDiscoveredResourcesRequest
+        @return: ListDiscoveredResourcesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_discovered_resources_with_options(request, runtime)
 
     async def list_discovered_resources_async(
         self,
         request: config_20200907_models.ListDiscoveredResourcesRequest,
     ) -> config_20200907_models.ListDiscoveredResourcesResponse:
+        """
+        This topic provides an example on how to call the ListDiscoveredResources operation to query the resources in the current Alibaba Cloud account. The returned result indicates that a total of eight resources exist in the account.
+        
+        @param request: ListDiscoveredResourcesRequest
+        @return: ListDiscoveredResourcesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_discovered_resources_with_options_async(request, runtime)
 
     def list_managed_rules_with_options(
         self,
         request: config_20200907_models.ListManagedRulesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ListManagedRulesResponse:
+        """
+        This topic describes how to query the managed rules of Alibaba Cloud CDN by using the `CDN` keyword. The returned result shows that only one managed rule exists. You can view the rule details in the result.
+        
+        @param request: ListManagedRulesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListManagedRulesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.keyword):
             query['Keyword'] = request.keyword
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.resource_types):
+            query['ResourceTypes'] = request.resource_types
         if not UtilClient.is_unset(request.risk_level):
             query['RiskLevel'] = request.risk_level
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListManagedRules',
@@ -6658,22 +8757,31 @@
         )
 
     async def list_managed_rules_with_options_async(
         self,
         request: config_20200907_models.ListManagedRulesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ListManagedRulesResponse:
+        """
+        This topic describes how to query the managed rules of Alibaba Cloud CDN by using the `CDN` keyword. The returned result shows that only one managed rule exists. You can view the rule details in the result.
+        
+        @param request: ListManagedRulesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListManagedRulesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.keyword):
             query['Keyword'] = request.keyword
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.resource_types):
+            query['ResourceTypes'] = request.resource_types
         if not UtilClient.is_unset(request.risk_level):
             query['RiskLevel'] = request.risk_level
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListManagedRules',
@@ -6691,21 +8799,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_managed_rules(
         self,
         request: config_20200907_models.ListManagedRulesRequest,
     ) -> config_20200907_models.ListManagedRulesResponse:
+        """
+        This topic describes how to query the managed rules of Alibaba Cloud CDN by using the `CDN` keyword. The returned result shows that only one managed rule exists. You can view the rule details in the result.
+        
+        @param request: ListManagedRulesRequest
+        @return: ListManagedRulesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_managed_rules_with_options(request, runtime)
 
     async def list_managed_rules_async(
         self,
         request: config_20200907_models.ListManagedRulesRequest,
     ) -> config_20200907_models.ListManagedRulesResponse:
+        """
+        This topic describes how to query the managed rules of Alibaba Cloud CDN by using the `CDN` keyword. The returned result shows that only one managed rule exists. You can view the rule details in the result.
+        
+        @param request: ListManagedRulesRequest
+        @return: ListManagedRulesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_managed_rules_with_options_async(request, runtime)
 
     def list_pre_managed_rules_with_options(
         self,
         tmp_req: config_20200907_models.ListPreManagedRulesRequest,
         runtime: util_models.RuntimeOptions,
@@ -6792,14 +8912,21 @@
         return await self.list_pre_managed_rules_with_options_async(request, runtime)
 
     def list_remediation_templates_with_options(
         self,
         request: config_20200907_models.ListRemediationTemplatesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ListRemediationTemplatesResponse:
+        """
+        In this topic, the `oss-bucket-public-write-prohibited` managed rule is used as an example. The return result shows the details of the remediation template of the `OOS` type for the managed rule. OOS represents Operation Orchestration Service.
+        
+        @param request: ListRemediationTemplatesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListRemediationTemplatesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.managed_rule_identifier):
             query['ManagedRuleIdentifier'] = request.managed_rule_identifier
         if not UtilClient.is_unset(request.remediation_type):
             query['RemediationType'] = request.remediation_type
         req = open_api_models.OpenApiRequest(
@@ -6822,14 +8949,21 @@
         )
 
     async def list_remediation_templates_with_options_async(
         self,
         request: config_20200907_models.ListRemediationTemplatesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ListRemediationTemplatesResponse:
+        """
+        In this topic, the `oss-bucket-public-write-prohibited` managed rule is used as an example. The return result shows the details of the remediation template of the `OOS` type for the managed rule. OOS represents Operation Orchestration Service.
+        
+        @param request: ListRemediationTemplatesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListRemediationTemplatesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.managed_rule_identifier):
             query['ManagedRuleIdentifier'] = request.managed_rule_identifier
         if not UtilClient.is_unset(request.remediation_type):
             query['RemediationType'] = request.remediation_type
         req = open_api_models.OpenApiRequest(
@@ -6851,29 +8985,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_remediation_templates(
         self,
         request: config_20200907_models.ListRemediationTemplatesRequest,
     ) -> config_20200907_models.ListRemediationTemplatesResponse:
+        """
+        In this topic, the `oss-bucket-public-write-prohibited` managed rule is used as an example. The return result shows the details of the remediation template of the `OOS` type for the managed rule. OOS represents Operation Orchestration Service.
+        
+        @param request: ListRemediationTemplatesRequest
+        @return: ListRemediationTemplatesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_remediation_templates_with_options(request, runtime)
 
     async def list_remediation_templates_async(
         self,
         request: config_20200907_models.ListRemediationTemplatesRequest,
     ) -> config_20200907_models.ListRemediationTemplatesResponse:
+        """
+        In this topic, the `oss-bucket-public-write-prohibited` managed rule is used as an example. The return result shows the details of the remediation template of the `OOS` type for the managed rule. OOS represents Operation Orchestration Service.
+        
+        @param request: ListRemediationTemplatesRequest
+        @return: ListRemediationTemplatesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_remediation_templates_with_options_async(request, runtime)
 
     def list_remediations_with_options(
         self,
         request: config_20200907_models.ListRemediationsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ListRemediationsResponse:
+        """
+        In this topic, the rule whose ID is `cr-6b7c626622af00b4***` is used as an example.
+        
+        @param request: ListRemediationsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListRemediationsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.config_rule_ids):
             query['ConfigRuleIds'] = request.config_rule_ids
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -6894,14 +9047,21 @@
         )
 
     async def list_remediations_with_options_async(
         self,
         request: config_20200907_models.ListRemediationsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ListRemediationsResponse:
+        """
+        In this topic, the rule whose ID is `cr-6b7c626622af00b4***` is used as an example.
+        
+        @param request: ListRemediationsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListRemediationsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.config_rule_ids):
             query['ConfigRuleIds'] = request.config_rule_ids
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -6921,29 +9081,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_remediations(
         self,
         request: config_20200907_models.ListRemediationsRequest,
     ) -> config_20200907_models.ListRemediationsResponse:
+        """
+        In this topic, the rule whose ID is `cr-6b7c626622af00b4***` is used as an example.
+        
+        @param request: ListRemediationsRequest
+        @return: ListRemediationsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_remediations_with_options(request, runtime)
 
     async def list_remediations_async(
         self,
         request: config_20200907_models.ListRemediationsRequest,
     ) -> config_20200907_models.ListRemediationsResponse:
+        """
+        In this topic, the rule whose ID is `cr-6b7c626622af00b4***` is used as an example.
+        
+        @param request: ListRemediationsRequest
+        @return: ListRemediationsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_remediations_with_options_async(request, runtime)
 
     def list_resource_evaluation_results_with_options(
         self,
         request: config_20200907_models.ListResourceEvaluationResultsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ListResourceEvaluationResultsResponse:
+        """
+        In this example, the compliance evaluation result of the `23642660635396***` resource is queried and the resource is a RAM user. The returned result indicates that the resource is evaluated as `NON_COMPLIANT` by using the `cr-7f7d626622af0041****` rule.
+        
+        @param request: ListResourceEvaluationResultsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListResourceEvaluationResultsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.compliance_type):
             query['ComplianceType'] = request.compliance_type
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
@@ -6974,14 +9153,21 @@
         )
 
     async def list_resource_evaluation_results_with_options_async(
         self,
         request: config_20200907_models.ListResourceEvaluationResultsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.ListResourceEvaluationResultsResponse:
+        """
+        In this example, the compliance evaluation result of the `23642660635396***` resource is queried and the resource is a RAM user. The returned result indicates that the resource is evaluated as `NON_COMPLIANT` by using the `cr-7f7d626622af0041****` rule.
+        
+        @param request: ListResourceEvaluationResultsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListResourceEvaluationResultsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.compliance_type):
             query['ComplianceType'] = request.compliance_type
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
@@ -7011,21 +9197,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_resource_evaluation_results(
         self,
         request: config_20200907_models.ListResourceEvaluationResultsRequest,
     ) -> config_20200907_models.ListResourceEvaluationResultsResponse:
+        """
+        In this example, the compliance evaluation result of the `23642660635396***` resource is queried and the resource is a RAM user. The returned result indicates that the resource is evaluated as `NON_COMPLIANT` by using the `cr-7f7d626622af0041****` rule.
+        
+        @param request: ListResourceEvaluationResultsRequest
+        @return: ListResourceEvaluationResultsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_resource_evaluation_results_with_options(request, runtime)
 
     async def list_resource_evaluation_results_async(
         self,
         request: config_20200907_models.ListResourceEvaluationResultsRequest,
     ) -> config_20200907_models.ListResourceEvaluationResultsResponse:
+        """
+        In this example, the compliance evaluation result of the `23642660635396***` resource is queried and the resource is a RAM user. The returned result indicates that the resource is evaluated as `NON_COMPLIANT` by using the `cr-7f7d626622af0041****` rule.
+        
+        @param request: ListResourceEvaluationResultsRequest
+        @return: ListResourceEvaluationResultsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_resource_evaluation_results_with_options_async(request, runtime)
 
     def list_tag_resources_with_options(
         self,
         tmp_req: config_20200907_models.ListTagResourcesRequest,
         runtime: util_models.RuntimeOptions,
@@ -7120,14 +9318,23 @@
         return await self.list_tag_resources_with_options_async(request, runtime)
 
     def revert_aggregate_evaluation_results_with_options(
         self,
         tmp_req: config_20200907_models.RevertAggregateEvaluationResultsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.RevertAggregateEvaluationResultsResponse:
+        """
+        The sample request in this topic shows you how to reevaluate the `lb-hp3a3b4ztyfm2plgm***` non-compliant resource that is evaluated by the `cr-7e72626622af0051***` rule in the `120886317861****` member account of the `ca-5b6c626622af008f****` account group. The ID of the region in which the resource resides is `cn-beijing`, and the type of the resource is `ACS::SLB::LoadBalancer`.
+        ## Prerequisites
+        One or more non-compliant resources that are evaluated by a rule in an account group are ignored.
+        
+        @param tmp_req: RevertAggregateEvaluationResultsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RevertAggregateEvaluationResultsResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = config_20200907_models.RevertAggregateEvaluationResultsShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.resources):
             request.resources_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.resources, 'Resources', 'json')
         body = {}
         if not UtilClient.is_unset(request.aggregator_id):
@@ -7156,14 +9363,23 @@
         )
 
     async def revert_aggregate_evaluation_results_with_options_async(
         self,
         tmp_req: config_20200907_models.RevertAggregateEvaluationResultsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.RevertAggregateEvaluationResultsResponse:
+        """
+        The sample request in this topic shows you how to reevaluate the `lb-hp3a3b4ztyfm2plgm***` non-compliant resource that is evaluated by the `cr-7e72626622af0051***` rule in the `120886317861****` member account of the `ca-5b6c626622af008f****` account group. The ID of the region in which the resource resides is `cn-beijing`, and the type of the resource is `ACS::SLB::LoadBalancer`.
+        ## Prerequisites
+        One or more non-compliant resources that are evaluated by a rule in an account group are ignored.
+        
+        @param tmp_req: RevertAggregateEvaluationResultsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RevertAggregateEvaluationResultsResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = config_20200907_models.RevertAggregateEvaluationResultsShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.resources):
             request.resources_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.resources, 'Resources', 'json')
         body = {}
         if not UtilClient.is_unset(request.aggregator_id):
@@ -7191,29 +9407,54 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def revert_aggregate_evaluation_results(
         self,
         request: config_20200907_models.RevertAggregateEvaluationResultsRequest,
     ) -> config_20200907_models.RevertAggregateEvaluationResultsResponse:
+        """
+        The sample request in this topic shows you how to reevaluate the `lb-hp3a3b4ztyfm2plgm***` non-compliant resource that is evaluated by the `cr-7e72626622af0051***` rule in the `120886317861****` member account of the `ca-5b6c626622af008f****` account group. The ID of the region in which the resource resides is `cn-beijing`, and the type of the resource is `ACS::SLB::LoadBalancer`.
+        ## Prerequisites
+        One or more non-compliant resources that are evaluated by a rule in an account group are ignored.
+        
+        @param request: RevertAggregateEvaluationResultsRequest
+        @return: RevertAggregateEvaluationResultsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.revert_aggregate_evaluation_results_with_options(request, runtime)
 
     async def revert_aggregate_evaluation_results_async(
         self,
         request: config_20200907_models.RevertAggregateEvaluationResultsRequest,
     ) -> config_20200907_models.RevertAggregateEvaluationResultsResponse:
+        """
+        The sample request in this topic shows you how to reevaluate the `lb-hp3a3b4ztyfm2plgm***` non-compliant resource that is evaluated by the `cr-7e72626622af0051***` rule in the `120886317861****` member account of the `ca-5b6c626622af008f****` account group. The ID of the region in which the resource resides is `cn-beijing`, and the type of the resource is `ACS::SLB::LoadBalancer`.
+        ## Prerequisites
+        One or more non-compliant resources that are evaluated by a rule in an account group are ignored.
+        
+        @param request: RevertAggregateEvaluationResultsRequest
+        @return: RevertAggregateEvaluationResultsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.revert_aggregate_evaluation_results_with_options_async(request, runtime)
 
     def revert_evaluation_results_with_options(
         self,
         tmp_req: config_20200907_models.RevertEvaluationResultsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.RevertEvaluationResultsResponse:
+        """
+        The sample request in this topic shows you how to reevaluate the `lb-hp3a3b4ztyfm2plgm***` non-compliant resource that is evaluated by the `cr-7e72626622af0051****` rule. The ID of the region in which the resource resides is `cn-beijing`, and the type of the resource is `ACS::SLB::LoadBalancer`.
+        ## Prerequisites
+        One or more non-compliant resources that are evaluated by a rule are ignored.
+        
+        @param tmp_req: RevertEvaluationResultsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RevertEvaluationResultsResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = config_20200907_models.RevertEvaluationResultsShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.resources):
             request.resources_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.resources, 'Resources', 'json')
         body = {}
         if not UtilClient.is_unset(request.config_rule_id):
@@ -7240,14 +9481,23 @@
         )
 
     async def revert_evaluation_results_with_options_async(
         self,
         tmp_req: config_20200907_models.RevertEvaluationResultsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.RevertEvaluationResultsResponse:
+        """
+        The sample request in this topic shows you how to reevaluate the `lb-hp3a3b4ztyfm2plgm***` non-compliant resource that is evaluated by the `cr-7e72626622af0051****` rule. The ID of the region in which the resource resides is `cn-beijing`, and the type of the resource is `ACS::SLB::LoadBalancer`.
+        ## Prerequisites
+        One or more non-compliant resources that are evaluated by a rule are ignored.
+        
+        @param tmp_req: RevertEvaluationResultsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RevertEvaluationResultsResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = config_20200907_models.RevertEvaluationResultsShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.resources):
             request.resources_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.resources, 'Resources', 'json')
         body = {}
         if not UtilClient.is_unset(request.config_rule_id):
@@ -7273,29 +9523,53 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def revert_evaluation_results(
         self,
         request: config_20200907_models.RevertEvaluationResultsRequest,
     ) -> config_20200907_models.RevertEvaluationResultsResponse:
+        """
+        The sample request in this topic shows you how to reevaluate the `lb-hp3a3b4ztyfm2plgm***` non-compliant resource that is evaluated by the `cr-7e72626622af0051****` rule. The ID of the region in which the resource resides is `cn-beijing`, and the type of the resource is `ACS::SLB::LoadBalancer`.
+        ## Prerequisites
+        One or more non-compliant resources that are evaluated by a rule are ignored.
+        
+        @param request: RevertEvaluationResultsRequest
+        @return: RevertEvaluationResultsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.revert_evaluation_results_with_options(request, runtime)
 
     async def revert_evaluation_results_async(
         self,
         request: config_20200907_models.RevertEvaluationResultsRequest,
     ) -> config_20200907_models.RevertEvaluationResultsResponse:
+        """
+        The sample request in this topic shows you how to reevaluate the `lb-hp3a3b4ztyfm2plgm***` non-compliant resource that is evaluated by the `cr-7e72626622af0051****` rule. The ID of the region in which the resource resides is `cn-beijing`, and the type of the resource is `ACS::SLB::LoadBalancer`.
+        ## Prerequisites
+        One or more non-compliant resources that are evaluated by a rule are ignored.
+        
+        @param request: RevertEvaluationResultsRequest
+        @return: RevertEvaluationResultsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.revert_evaluation_results_with_options_async(request, runtime)
 
     def start_aggregate_config_rule_evaluation_with_options(
         self,
         request: config_20200907_models.StartAggregateConfigRuleEvaluationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.StartAggregateConfigRuleEvaluationResponse:
+        """
+        >  After you call this operation, the compliance evaluation is performed only once. To query the compliance evaluation results returned by the rule, call the ListAggregateConfigRuleEvaluationResults operation. For more information, see [ListAggregateConfigRuleEvaluationResults](~~265979~~).
+        The sample request in this topic shows you how to use the `cr-c169626622af009f****` rule in the `ca-3a58626622af0005****` account group to evaluate resources.
+        
+        @param request: StartAggregateConfigRuleEvaluationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StartAggregateConfigRuleEvaluationResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.compliance_pack_id):
             query['CompliancePackId'] = request.compliance_pack_id
         if not UtilClient.is_unset(request.config_rule_id):
@@ -7322,14 +9596,22 @@
         )
 
     async def start_aggregate_config_rule_evaluation_with_options_async(
         self,
         request: config_20200907_models.StartAggregateConfigRuleEvaluationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.StartAggregateConfigRuleEvaluationResponse:
+        """
+        >  After you call this operation, the compliance evaluation is performed only once. To query the compliance evaluation results returned by the rule, call the ListAggregateConfigRuleEvaluationResults operation. For more information, see [ListAggregateConfigRuleEvaluationResults](~~265979~~).
+        The sample request in this topic shows you how to use the `cr-c169626622af009f****` rule in the `ca-3a58626622af0005****` account group to evaluate resources.
+        
+        @param request: StartAggregateConfigRuleEvaluationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StartAggregateConfigRuleEvaluationResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.compliance_pack_id):
             query['CompliancePackId'] = request.compliance_pack_id
         if not UtilClient.is_unset(request.config_rule_id):
@@ -7355,29 +9637,50 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def start_aggregate_config_rule_evaluation(
         self,
         request: config_20200907_models.StartAggregateConfigRuleEvaluationRequest,
     ) -> config_20200907_models.StartAggregateConfigRuleEvaluationResponse:
+        """
+        >  After you call this operation, the compliance evaluation is performed only once. To query the compliance evaluation results returned by the rule, call the ListAggregateConfigRuleEvaluationResults operation. For more information, see [ListAggregateConfigRuleEvaluationResults](~~265979~~).
+        The sample request in this topic shows you how to use the `cr-c169626622af009f****` rule in the `ca-3a58626622af0005****` account group to evaluate resources.
+        
+        @param request: StartAggregateConfigRuleEvaluationRequest
+        @return: StartAggregateConfigRuleEvaluationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.start_aggregate_config_rule_evaluation_with_options(request, runtime)
 
     async def start_aggregate_config_rule_evaluation_async(
         self,
         request: config_20200907_models.StartAggregateConfigRuleEvaluationRequest,
     ) -> config_20200907_models.StartAggregateConfigRuleEvaluationResponse:
+        """
+        >  After you call this operation, the compliance evaluation is performed only once. To query the compliance evaluation results returned by the rule, call the ListAggregateConfigRuleEvaluationResults operation. For more information, see [ListAggregateConfigRuleEvaluationResults](~~265979~~).
+        The sample request in this topic shows you how to use the `cr-c169626622af009f****` rule in the `ca-3a58626622af0005****` account group to evaluate resources.
+        
+        @param request: StartAggregateConfigRuleEvaluationRequest
+        @return: StartAggregateConfigRuleEvaluationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.start_aggregate_config_rule_evaluation_with_options_async(request, runtime)
 
     def start_aggregate_remediation_with_options(
         self,
         request: config_20200907_models.StartAggregateRemediationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.StartAggregateRemediationResponse:
+        """
+        The sample request in this topic shows you how to manually execute the remediation template configured for the rule whose ID is `cr-6b7c626622af00b4***` in the account group whose ID is `ca-6b4a626622af0012****`. The return result shows that the manual execution is successful.
+        
+        @param request: StartAggregateRemediationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StartAggregateRemediationResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.config_rule_id):
             query['ConfigRuleId'] = request.config_rule_id
         req = open_api_models.OpenApiRequest(
@@ -7400,14 +9703,21 @@
         )
 
     async def start_aggregate_remediation_with_options_async(
         self,
         request: config_20200907_models.StartAggregateRemediationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.StartAggregateRemediationResponse:
+        """
+        The sample request in this topic shows you how to manually execute the remediation template configured for the rule whose ID is `cr-6b7c626622af00b4***` in the account group whose ID is `ca-6b4a626622af0012****`. The return result shows that the manual execution is successful.
+        
+        @param request: StartAggregateRemediationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StartAggregateRemediationResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.config_rule_id):
             query['ConfigRuleId'] = request.config_rule_id
         req = open_api_models.OpenApiRequest(
@@ -7429,29 +9739,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def start_aggregate_remediation(
         self,
         request: config_20200907_models.StartAggregateRemediationRequest,
     ) -> config_20200907_models.StartAggregateRemediationResponse:
+        """
+        The sample request in this topic shows you how to manually execute the remediation template configured for the rule whose ID is `cr-6b7c626622af00b4***` in the account group whose ID is `ca-6b4a626622af0012****`. The return result shows that the manual execution is successful.
+        
+        @param request: StartAggregateRemediationRequest
+        @return: StartAggregateRemediationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.start_aggregate_remediation_with_options(request, runtime)
 
     async def start_aggregate_remediation_async(
         self,
         request: config_20200907_models.StartAggregateRemediationRequest,
     ) -> config_20200907_models.StartAggregateRemediationResponse:
+        """
+        The sample request in this topic shows you how to manually execute the remediation template configured for the rule whose ID is `cr-6b7c626622af00b4***` in the account group whose ID is `ca-6b4a626622af0012****`. The return result shows that the manual execution is successful.
+        
+        @param request: StartAggregateRemediationRequest
+        @return: StartAggregateRemediationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.start_aggregate_remediation_with_options_async(request, runtime)
 
     def start_remediation_with_options(
         self,
         request: config_20200907_models.StartRemediationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.StartRemediationResponse:
+        """
+        In this topic, the rule whose ID is `cr-8a973ac2e2be00a2***` is used as an example. The return result shows that the manual execution is successful.
+        
+        @param request: StartRemediationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StartRemediationResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.config_rule_id):
             query['ConfigRuleId'] = request.config_rule_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -7472,14 +9801,21 @@
         )
 
     async def start_remediation_with_options_async(
         self,
         request: config_20200907_models.StartRemediationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.StartRemediationResponse:
+        """
+        In this topic, the rule whose ID is `cr-8a973ac2e2be00a2***` is used as an example. The return result shows that the manual execution is successful.
+        
+        @param request: StartRemediationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StartRemediationResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.config_rule_id):
             query['ConfigRuleId'] = request.config_rule_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -7499,21 +9835,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def start_remediation(
         self,
         request: config_20200907_models.StartRemediationRequest,
     ) -> config_20200907_models.StartRemediationResponse:
+        """
+        In this topic, the rule whose ID is `cr-8a973ac2e2be00a2***` is used as an example. The return result shows that the manual execution is successful.
+        
+        @param request: StartRemediationRequest
+        @return: StartRemediationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.start_remediation_with_options(request, runtime)
 
     async def start_remediation_async(
         self,
         request: config_20200907_models.StartRemediationRequest,
     ) -> config_20200907_models.StartRemediationResponse:
+        """
+        In this topic, the rule whose ID is `cr-8a973ac2e2be00a2***` is used as an example. The return result shows that the manual execution is successful.
+        
+        @param request: StartRemediationRequest
+        @return: StartRemediationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.start_remediation_with_options_async(request, runtime)
 
     def stop_configuration_recorder_with_options(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.StopConfigurationRecorderResponse:
@@ -7740,14 +10088,21 @@
         return await self.untag_resources_with_options_async(request, runtime)
 
     def update_aggregate_compliance_pack_with_options(
         self,
         tmp_req: config_20200907_models.UpdateAggregateCompliancePackRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.UpdateAggregateCompliancePackResponse:
+        """
+        This topic provides an example on how to change the value of a parameter for a managed rule whose ID is `eip-bandwidth-limit` to `20`. The managed rule is included in the `cp-fdc8626622af00f9***` compliance package in the `ca-f632626622af0079****` account group.
+        
+        @param tmp_req: UpdateAggregateCompliancePackRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateAggregateCompliancePackResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = config_20200907_models.UpdateAggregateCompliancePackShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.config_rules):
             request.config_rules_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.config_rules, 'ConfigRules', 'json')
         body = {}
         if not UtilClient.is_unset(request.aggregator_id):
@@ -7794,14 +10149,21 @@
         )
 
     async def update_aggregate_compliance_pack_with_options_async(
         self,
         tmp_req: config_20200907_models.UpdateAggregateCompliancePackRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.UpdateAggregateCompliancePackResponse:
+        """
+        This topic provides an example on how to change the value of a parameter for a managed rule whose ID is `eip-bandwidth-limit` to `20`. The managed rule is included in the `cp-fdc8626622af00f9***` compliance package in the `ca-f632626622af0079****` account group.
+        
+        @param tmp_req: UpdateAggregateCompliancePackRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateAggregateCompliancePackResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = config_20200907_models.UpdateAggregateCompliancePackShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.config_rules):
             request.config_rules_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.config_rules, 'ConfigRules', 'json')
         body = {}
         if not UtilClient.is_unset(request.aggregator_id):
@@ -7847,29 +10209,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_aggregate_compliance_pack(
         self,
         request: config_20200907_models.UpdateAggregateCompliancePackRequest,
     ) -> config_20200907_models.UpdateAggregateCompliancePackResponse:
+        """
+        This topic provides an example on how to change the value of a parameter for a managed rule whose ID is `eip-bandwidth-limit` to `20`. The managed rule is included in the `cp-fdc8626622af00f9***` compliance package in the `ca-f632626622af0079****` account group.
+        
+        @param request: UpdateAggregateCompliancePackRequest
+        @return: UpdateAggregateCompliancePackResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_aggregate_compliance_pack_with_options(request, runtime)
 
     async def update_aggregate_compliance_pack_async(
         self,
         request: config_20200907_models.UpdateAggregateCompliancePackRequest,
     ) -> config_20200907_models.UpdateAggregateCompliancePackResponse:
+        """
+        This topic provides an example on how to change the value of a parameter for a managed rule whose ID is `eip-bandwidth-limit` to `20`. The managed rule is included in the `cp-fdc8626622af00f9***` compliance package in the `ca-f632626622af0079****` account group.
+        
+        @param request: UpdateAggregateCompliancePackRequest
+        @return: UpdateAggregateCompliancePackResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_aggregate_compliance_pack_with_options_async(request, runtime)
 
     def update_aggregate_config_delivery_channel_with_options(
         self,
         request: config_20200907_models.UpdateAggregateConfigDeliveryChannelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.UpdateAggregateConfigDeliveryChannelResponse:
+        """
+        In this example, a delivery channel in an account group is disabled. The ID of the account group is `ca-a4e5626622af0079***`, and the ID of the delivery channel is `cdc-8e45ff4e06a3a8****```. The Status parameter is set to 0. After the delivery channel is disabled, Cloud Config retains the most recent delivery configuration and stops resource data delivery.
+        
+        @param request: UpdateAggregateConfigDeliveryChannelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateAggregateConfigDeliveryChannelResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.configuration_item_change_notification):
@@ -7914,14 +10295,21 @@
         )
 
     async def update_aggregate_config_delivery_channel_with_options_async(
         self,
         request: config_20200907_models.UpdateAggregateConfigDeliveryChannelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.UpdateAggregateConfigDeliveryChannelResponse:
+        """
+        In this example, a delivery channel in an account group is disabled. The ID of the account group is `ca-a4e5626622af0079***`, and the ID of the delivery channel is `cdc-8e45ff4e06a3a8****```. The Status parameter is set to 0. After the delivery channel is disabled, Cloud Config retains the most recent delivery configuration and stops resource data delivery.
+        
+        @param request: UpdateAggregateConfigDeliveryChannelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateAggregateConfigDeliveryChannelResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aggregator_id):
             query['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.configuration_item_change_notification):
@@ -7965,29 +10353,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_aggregate_config_delivery_channel(
         self,
         request: config_20200907_models.UpdateAggregateConfigDeliveryChannelRequest,
     ) -> config_20200907_models.UpdateAggregateConfigDeliveryChannelResponse:
+        """
+        In this example, a delivery channel in an account group is disabled. The ID of the account group is `ca-a4e5626622af0079***`, and the ID of the delivery channel is `cdc-8e45ff4e06a3a8****```. The Status parameter is set to 0. After the delivery channel is disabled, Cloud Config retains the most recent delivery configuration and stops resource data delivery.
+        
+        @param request: UpdateAggregateConfigDeliveryChannelRequest
+        @return: UpdateAggregateConfigDeliveryChannelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_aggregate_config_delivery_channel_with_options(request, runtime)
 
     async def update_aggregate_config_delivery_channel_async(
         self,
         request: config_20200907_models.UpdateAggregateConfigDeliveryChannelRequest,
     ) -> config_20200907_models.UpdateAggregateConfigDeliveryChannelResponse:
+        """
+        In this example, a delivery channel in an account group is disabled. The ID of the account group is `ca-a4e5626622af0079***`, and the ID of the delivery channel is `cdc-8e45ff4e06a3a8****```. The Status parameter is set to 0. After the delivery channel is disabled, Cloud Config retains the most recent delivery configuration and stops resource data delivery.
+        
+        @param request: UpdateAggregateConfigDeliveryChannelRequest
+        @return: UpdateAggregateConfigDeliveryChannelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_aggregate_config_delivery_channel_with_options_async(request, runtime)
 
     def update_aggregate_config_rule_with_options(
         self,
         tmp_req: config_20200907_models.UpdateAggregateConfigRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.UpdateAggregateConfigRuleResponse:
+        """
+        The sample request in this topic shows you how to change the risk level specified for the `cr-4e3d626622af0080***` managed rule to `3`, which indicates low risk level, in the `ca-a4e5626622af0079****` account group.
+        
+        @param tmp_req: UpdateAggregateConfigRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateAggregateConfigRuleResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = config_20200907_models.UpdateAggregateConfigRuleShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.input_parameters):
             request.input_parameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.input_parameters, 'InputParameters', 'json')
         if not UtilClient.is_unset(tmp_req.resource_types_scope):
             request.resource_types_scope_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.resource_types_scope, 'ResourceTypesScope', 'simple')
@@ -8050,14 +10457,21 @@
         )
 
     async def update_aggregate_config_rule_with_options_async(
         self,
         tmp_req: config_20200907_models.UpdateAggregateConfigRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.UpdateAggregateConfigRuleResponse:
+        """
+        The sample request in this topic shows you how to change the risk level specified for the `cr-4e3d626622af0080***` managed rule to `3`, which indicates low risk level, in the `ca-a4e5626622af0079****` account group.
+        
+        @param tmp_req: UpdateAggregateConfigRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateAggregateConfigRuleResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = config_20200907_models.UpdateAggregateConfigRuleShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.input_parameters):
             request.input_parameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.input_parameters, 'InputParameters', 'json')
         if not UtilClient.is_unset(tmp_req.resource_types_scope):
             request.resource_types_scope_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.resource_types_scope, 'ResourceTypesScope', 'simple')
@@ -8119,29 +10533,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_aggregate_config_rule(
         self,
         request: config_20200907_models.UpdateAggregateConfigRuleRequest,
     ) -> config_20200907_models.UpdateAggregateConfigRuleResponse:
+        """
+        The sample request in this topic shows you how to change the risk level specified for the `cr-4e3d626622af0080***` managed rule to `3`, which indicates low risk level, in the `ca-a4e5626622af0079****` account group.
+        
+        @param request: UpdateAggregateConfigRuleRequest
+        @return: UpdateAggregateConfigRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_aggregate_config_rule_with_options(request, runtime)
 
     async def update_aggregate_config_rule_async(
         self,
         request: config_20200907_models.UpdateAggregateConfigRuleRequest,
     ) -> config_20200907_models.UpdateAggregateConfigRuleResponse:
+        """
+        The sample request in this topic shows you how to change the risk level specified for the `cr-4e3d626622af0080***` managed rule to `3`, which indicates low risk level, in the `ca-a4e5626622af0079****` account group.
+        
+        @param request: UpdateAggregateConfigRuleRequest
+        @return: UpdateAggregateConfigRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_aggregate_config_rule_with_options_async(request, runtime)
 
     def update_aggregate_remediation_with_options(
         self,
         request: config_20200907_models.UpdateAggregateRemediationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.UpdateAggregateRemediationResponse:
+        """
+        This topic describes how to change the execution mode of the `crr-909ba2d4716700eb***` remediation setting for a rule in the `ca-6b4a626622af0012****` account group to `AUTO_EXECUTION`, which specifies automatic remediation. This topic also provides a sample request.
+        
+        @param request: UpdateAggregateRemediationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateAggregateRemediationResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.aggregator_id):
             body['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.invoke_type):
             body['InvokeType'] = request.invoke_type
         if not UtilClient.is_unset(request.params):
@@ -8174,14 +10607,21 @@
         )
 
     async def update_aggregate_remediation_with_options_async(
         self,
         request: config_20200907_models.UpdateAggregateRemediationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.UpdateAggregateRemediationResponse:
+        """
+        This topic describes how to change the execution mode of the `crr-909ba2d4716700eb***` remediation setting for a rule in the `ca-6b4a626622af0012****` account group to `AUTO_EXECUTION`, which specifies automatic remediation. This topic also provides a sample request.
+        
+        @param request: UpdateAggregateRemediationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateAggregateRemediationResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.aggregator_id):
             body['AggregatorId'] = request.aggregator_id
         if not UtilClient.is_unset(request.invoke_type):
             body['InvokeType'] = request.invoke_type
         if not UtilClient.is_unset(request.params):
@@ -8213,29 +10653,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_aggregate_remediation(
         self,
         request: config_20200907_models.UpdateAggregateRemediationRequest,
     ) -> config_20200907_models.UpdateAggregateRemediationResponse:
+        """
+        This topic describes how to change the execution mode of the `crr-909ba2d4716700eb***` remediation setting for a rule in the `ca-6b4a626622af0012****` account group to `AUTO_EXECUTION`, which specifies automatic remediation. This topic also provides a sample request.
+        
+        @param request: UpdateAggregateRemediationRequest
+        @return: UpdateAggregateRemediationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_aggregate_remediation_with_options(request, runtime)
 
     async def update_aggregate_remediation_async(
         self,
         request: config_20200907_models.UpdateAggregateRemediationRequest,
     ) -> config_20200907_models.UpdateAggregateRemediationResponse:
+        """
+        This topic describes how to change the execution mode of the `crr-909ba2d4716700eb***` remediation setting for a rule in the `ca-6b4a626622af0012****` account group to `AUTO_EXECUTION`, which specifies automatic remediation. This topic also provides a sample request.
+        
+        @param request: UpdateAggregateRemediationRequest
+        @return: UpdateAggregateRemediationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_aggregate_remediation_with_options_async(request, runtime)
 
     def update_aggregator_with_options(
         self,
         tmp_req: config_20200907_models.UpdateAggregatorRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.UpdateAggregatorResponse:
+        """
+        The sample request in this topic shows you how to add a member account to the account group whose ID is `ca-dacf86d8314e00eb***`. The member account ID is `173808452267****` and the member account name is `Tony`. The member account belongs to `ResourceDirectory`.
+        
+        @param tmp_req: UpdateAggregatorRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateAggregatorResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = config_20200907_models.UpdateAggregatorShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.aggregator_accounts):
             request.aggregator_accounts_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.aggregator_accounts, 'AggregatorAccounts', 'json')
         body = {}
         if not UtilClient.is_unset(request.aggregator_accounts_shrink):
@@ -8268,14 +10727,21 @@
         )
 
     async def update_aggregator_with_options_async(
         self,
         tmp_req: config_20200907_models.UpdateAggregatorRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.UpdateAggregatorResponse:
+        """
+        The sample request in this topic shows you how to add a member account to the account group whose ID is `ca-dacf86d8314e00eb***`. The member account ID is `173808452267****` and the member account name is `Tony`. The member account belongs to `ResourceDirectory`.
+        
+        @param tmp_req: UpdateAggregatorRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateAggregatorResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = config_20200907_models.UpdateAggregatorShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.aggregator_accounts):
             request.aggregator_accounts_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.aggregator_accounts, 'AggregatorAccounts', 'json')
         body = {}
         if not UtilClient.is_unset(request.aggregator_accounts_shrink):
@@ -8307,29 +10773,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_aggregator(
         self,
         request: config_20200907_models.UpdateAggregatorRequest,
     ) -> config_20200907_models.UpdateAggregatorResponse:
+        """
+        The sample request in this topic shows you how to add a member account to the account group whose ID is `ca-dacf86d8314e00eb***`. The member account ID is `173808452267****` and the member account name is `Tony`. The member account belongs to `ResourceDirectory`.
+        
+        @param request: UpdateAggregatorRequest
+        @return: UpdateAggregatorResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_aggregator_with_options(request, runtime)
 
     async def update_aggregator_async(
         self,
         request: config_20200907_models.UpdateAggregatorRequest,
     ) -> config_20200907_models.UpdateAggregatorResponse:
+        """
+        The sample request in this topic shows you how to add a member account to the account group whose ID is `ca-dacf86d8314e00eb***`. The member account ID is `173808452267****` and the member account name is `Tony`. The member account belongs to `ResourceDirectory`.
+        
+        @param request: UpdateAggregatorRequest
+        @return: UpdateAggregatorResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_aggregator_with_options_async(request, runtime)
 
     def update_compliance_pack_with_options(
         self,
         tmp_req: config_20200907_models.UpdateCompliancePackRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.UpdateCompliancePackResponse:
+        """
+        This topic provides an example on how to change the value of a parameter for a managed rule whose ID is `eip-bandwidth-limit` to `20`. The managed rule is included in the `cp-a8a8626622af0082***` compliance package.
+        
+        @param tmp_req: UpdateCompliancePackRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateCompliancePackResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = config_20200907_models.UpdateCompliancePackShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.config_rules):
             request.config_rules_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.config_rules, 'ConfigRules', 'json')
         body = {}
         if not UtilClient.is_unset(request.client_token):
@@ -8374,14 +10859,21 @@
         )
 
     async def update_compliance_pack_with_options_async(
         self,
         tmp_req: config_20200907_models.UpdateCompliancePackRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.UpdateCompliancePackResponse:
+        """
+        This topic provides an example on how to change the value of a parameter for a managed rule whose ID is `eip-bandwidth-limit` to `20`. The managed rule is included in the `cp-a8a8626622af0082***` compliance package.
+        
+        @param tmp_req: UpdateCompliancePackRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateCompliancePackResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = config_20200907_models.UpdateCompliancePackShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.config_rules):
             request.config_rules_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.config_rules, 'ConfigRules', 'json')
         body = {}
         if not UtilClient.is_unset(request.client_token):
@@ -8425,29 +10917,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_compliance_pack(
         self,
         request: config_20200907_models.UpdateCompliancePackRequest,
     ) -> config_20200907_models.UpdateCompliancePackResponse:
+        """
+        This topic provides an example on how to change the value of a parameter for a managed rule whose ID is `eip-bandwidth-limit` to `20`. The managed rule is included in the `cp-a8a8626622af0082***` compliance package.
+        
+        @param request: UpdateCompliancePackRequest
+        @return: UpdateCompliancePackResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_compliance_pack_with_options(request, runtime)
 
     async def update_compliance_pack_async(
         self,
         request: config_20200907_models.UpdateCompliancePackRequest,
     ) -> config_20200907_models.UpdateCompliancePackResponse:
+        """
+        This topic provides an example on how to change the value of a parameter for a managed rule whose ID is `eip-bandwidth-limit` to `20`. The managed rule is included in the `cp-a8a8626622af0082***` compliance package.
+        
+        @param request: UpdateCompliancePackRequest
+        @return: UpdateCompliancePackResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_compliance_pack_with_options_async(request, runtime)
 
     def update_config_delivery_channel_with_options(
         self,
         request: config_20200907_models.UpdateConfigDeliveryChannelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.UpdateConfigDeliveryChannelResponse:
+        """
+        In this example, a delivery channel is disabled. The ID of the delivery channel is `cdc-8e45ff4e06a3a8***```. The Status parameter is set to 0. After the delivery channel is disabled, Cloud Config retains the most recent delivery configuration and stops the delivery of resource data.
+        
+        @param request: UpdateConfigDeliveryChannelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateConfigDeliveryChannelResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.configuration_item_change_notification):
             query['ConfigurationItemChangeNotification'] = request.configuration_item_change_notification
         if not UtilClient.is_unset(request.configuration_snapshot):
@@ -8490,14 +11001,21 @@
         )
 
     async def update_config_delivery_channel_with_options_async(
         self,
         request: config_20200907_models.UpdateConfigDeliveryChannelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.UpdateConfigDeliveryChannelResponse:
+        """
+        In this example, a delivery channel is disabled. The ID of the delivery channel is `cdc-8e45ff4e06a3a8***```. The Status parameter is set to 0. After the delivery channel is disabled, Cloud Config retains the most recent delivery configuration and stops the delivery of resource data.
+        
+        @param request: UpdateConfigDeliveryChannelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateConfigDeliveryChannelResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.configuration_item_change_notification):
             query['ConfigurationItemChangeNotification'] = request.configuration_item_change_notification
         if not UtilClient.is_unset(request.configuration_snapshot):
@@ -8539,29 +11057,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_config_delivery_channel(
         self,
         request: config_20200907_models.UpdateConfigDeliveryChannelRequest,
     ) -> config_20200907_models.UpdateConfigDeliveryChannelResponse:
+        """
+        In this example, a delivery channel is disabled. The ID of the delivery channel is `cdc-8e45ff4e06a3a8***```. The Status parameter is set to 0. After the delivery channel is disabled, Cloud Config retains the most recent delivery configuration and stops the delivery of resource data.
+        
+        @param request: UpdateConfigDeliveryChannelRequest
+        @return: UpdateConfigDeliveryChannelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_config_delivery_channel_with_options(request, runtime)
 
     async def update_config_delivery_channel_async(
         self,
         request: config_20200907_models.UpdateConfigDeliveryChannelRequest,
     ) -> config_20200907_models.UpdateConfigDeliveryChannelResponse:
+        """
+        In this example, a delivery channel is disabled. The ID of the delivery channel is `cdc-8e45ff4e06a3a8***```. The Status parameter is set to 0. After the delivery channel is disabled, Cloud Config retains the most recent delivery configuration and stops the delivery of resource data.
+        
+        @param request: UpdateConfigDeliveryChannelRequest
+        @return: UpdateConfigDeliveryChannelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_config_delivery_channel_with_options_async(request, runtime)
 
     def update_config_rule_with_options(
         self,
         tmp_req: config_20200907_models.UpdateConfigRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.UpdateConfigRuleResponse:
+        """
+        This topic provides an example on how to change the risk level of a managed rule whose ID is `cr-a260626622af0005***` to `3` (low risk level).
+        
+        @param tmp_req: UpdateConfigRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateConfigRuleResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = config_20200907_models.UpdateConfigRuleShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.input_parameters):
             request.input_parameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.input_parameters, 'InputParameters', 'json')
         if not UtilClient.is_unset(tmp_req.resource_types_scope):
             request.resource_types_scope_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.resource_types_scope, 'ResourceTypesScope', 'simple')
@@ -8616,14 +11153,21 @@
         )
 
     async def update_config_rule_with_options_async(
         self,
         tmp_req: config_20200907_models.UpdateConfigRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.UpdateConfigRuleResponse:
+        """
+        This topic provides an example on how to change the risk level of a managed rule whose ID is `cr-a260626622af0005***` to `3` (low risk level).
+        
+        @param tmp_req: UpdateConfigRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateConfigRuleResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = config_20200907_models.UpdateConfigRuleShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.input_parameters):
             request.input_parameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.input_parameters, 'InputParameters', 'json')
         if not UtilClient.is_unset(tmp_req.resource_types_scope):
             request.resource_types_scope_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.resource_types_scope, 'ResourceTypesScope', 'simple')
@@ -8677,29 +11221,50 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_config_rule(
         self,
         request: config_20200907_models.UpdateConfigRuleRequest,
     ) -> config_20200907_models.UpdateConfigRuleResponse:
+        """
+        This topic provides an example on how to change the risk level of a managed rule whose ID is `cr-a260626622af0005***` to `3` (low risk level).
+        
+        @param request: UpdateConfigRuleRequest
+        @return: UpdateConfigRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_config_rule_with_options(request, runtime)
 
     async def update_config_rule_async(
         self,
         request: config_20200907_models.UpdateConfigRuleRequest,
     ) -> config_20200907_models.UpdateConfigRuleResponse:
+        """
+        This topic provides an example on how to change the risk level of a managed rule whose ID is `cr-a260626622af0005***` to `3` (low risk level).
+        
+        @param request: UpdateConfigRuleRequest
+        @return: UpdateConfigRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_config_rule_with_options_async(request, runtime)
 
     def update_delivery_channel_with_options(
         self,
         request: config_20200907_models.UpdateDeliveryChannelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.UpdateDeliveryChannelResponse:
+        """
+        @deprecated : UpdateDeliveryChannel is deprecated, please use Config::2020-09-07::UpdateConfigDeliveryChannel,Config::2020-09-07::UpdateAggregateConfigDeliveryChannel instead.
+        In this example, the status of the delivery channel whose ID is `cdc-8e45ff4e06a3a8****` is changed to 0, which indicates that the delivery channel is disabled. After the delivery channel is disabled, Cloud Config retains the last delivery configuration and stops resource data delivery.
+        
+        @param request: UpdateDeliveryChannelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateDeliveryChannelResponse
+        Deprecated
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.configuration_item_change_notification):
             body['ConfigurationItemChangeNotification'] = request.configuration_item_change_notification
         if not UtilClient.is_unset(request.configuration_snapshot):
@@ -8742,14 +11307,23 @@
         )
 
     async def update_delivery_channel_with_options_async(
         self,
         request: config_20200907_models.UpdateDeliveryChannelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.UpdateDeliveryChannelResponse:
+        """
+        @deprecated : UpdateDeliveryChannel is deprecated, please use Config::2020-09-07::UpdateConfigDeliveryChannel,Config::2020-09-07::UpdateAggregateConfigDeliveryChannel instead.
+        In this example, the status of the delivery channel whose ID is `cdc-8e45ff4e06a3a8****` is changed to 0, which indicates that the delivery channel is disabled. After the delivery channel is disabled, Cloud Config retains the last delivery configuration and stops resource data delivery.
+        
+        @param request: UpdateDeliveryChannelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateDeliveryChannelResponse
+        Deprecated
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.configuration_item_change_notification):
             body['ConfigurationItemChangeNotification'] = request.configuration_item_change_notification
         if not UtilClient.is_unset(request.configuration_snapshot):
@@ -8791,21 +11365,37 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_delivery_channel(
         self,
         request: config_20200907_models.UpdateDeliveryChannelRequest,
     ) -> config_20200907_models.UpdateDeliveryChannelResponse:
+        """
+        @deprecated : UpdateDeliveryChannel is deprecated, please use Config::2020-09-07::UpdateConfigDeliveryChannel,Config::2020-09-07::UpdateAggregateConfigDeliveryChannel instead.
+        In this example, the status of the delivery channel whose ID is `cdc-8e45ff4e06a3a8****` is changed to 0, which indicates that the delivery channel is disabled. After the delivery channel is disabled, Cloud Config retains the last delivery configuration and stops resource data delivery.
+        
+        @param request: UpdateDeliveryChannelRequest
+        @return: UpdateDeliveryChannelResponse
+        Deprecated
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_delivery_channel_with_options(request, runtime)
 
     async def update_delivery_channel_async(
         self,
         request: config_20200907_models.UpdateDeliveryChannelRequest,
     ) -> config_20200907_models.UpdateDeliveryChannelResponse:
+        """
+        @deprecated : UpdateDeliveryChannel is deprecated, please use Config::2020-09-07::UpdateConfigDeliveryChannel,Config::2020-09-07::UpdateAggregateConfigDeliveryChannel instead.
+        In this example, the status of the delivery channel whose ID is `cdc-8e45ff4e06a3a8****` is changed to 0, which indicates that the delivery channel is disabled. After the delivery channel is disabled, Cloud Config retains the last delivery configuration and stops resource data delivery.
+        
+        @param request: UpdateDeliveryChannelRequest
+        @return: UpdateDeliveryChannelResponse
+        Deprecated
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_delivery_channel_with_options_async(request, runtime)
 
     def update_integrated_service_status_with_options(
         self,
         request: config_20200907_models.UpdateIntegratedServiceStatusRequest,
         runtime: util_models.RuntimeOptions,
@@ -8880,14 +11470,21 @@
         return await self.update_integrated_service_status_with_options_async(request, runtime)
 
     def update_remediation_with_options(
         self,
         request: config_20200907_models.UpdateRemediationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.UpdateRemediationResponse:
+        """
+        This topic describes how to change the execution mode of the `crr-909ba2d4716700eb***` remediation setting to `AUTO_EXECUTION`, which specifies automatic remediation. This topic also provides a sample request.
+        
+        @param request: UpdateRemediationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateRemediationResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.invoke_type):
             body['InvokeType'] = request.invoke_type
         if not UtilClient.is_unset(request.params):
@@ -8920,14 +11517,21 @@
         )
 
     async def update_remediation_with_options_async(
         self,
         request: config_20200907_models.UpdateRemediationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> config_20200907_models.UpdateRemediationResponse:
+        """
+        This topic describes how to change the execution mode of the `crr-909ba2d4716700eb***` remediation setting to `AUTO_EXECUTION`, which specifies automatic remediation. This topic also provides a sample request.
+        
+        @param request: UpdateRemediationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateRemediationResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_token):
             body['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.invoke_type):
             body['InvokeType'] = request.invoke_type
         if not UtilClient.is_unset(request.params):
@@ -8959,16 +11563,28 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_remediation(
         self,
         request: config_20200907_models.UpdateRemediationRequest,
     ) -> config_20200907_models.UpdateRemediationResponse:
+        """
+        This topic describes how to change the execution mode of the `crr-909ba2d4716700eb***` remediation setting to `AUTO_EXECUTION`, which specifies automatic remediation. This topic also provides a sample request.
+        
+        @param request: UpdateRemediationRequest
+        @return: UpdateRemediationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_remediation_with_options(request, runtime)
 
     async def update_remediation_async(
         self,
         request: config_20200907_models.UpdateRemediationRequest,
     ) -> config_20200907_models.UpdateRemediationResponse:
+        """
+        This topic describes how to change the execution mode of the `crr-909ba2d4716700eb***` remediation setting to `AUTO_EXECUTION`, which specifies automatic remediation. This topic also provides a sample request.
+        
+        @param request: UpdateRemediationRequest
+        @return: UpdateRemediationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_remediation_with_options_async(request, runtime)
```

### Comparing `alibabacloud_config20200907-2.2.3/alibabacloud_config20200907.egg-info/PKG-INFO` & `alibabacloud_config20200907-2.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-config20200907
-Version: 2.2.3
+Name: alibabacloud_config20200907
+Version: 2.2.7
 Summary: Alibaba Cloud CloudConfig (20200907) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_config20200907-2.2.3/setup.py` & `alibabacloud_config20200907-2.2.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_config20200907.
 
-Created on 27/12/2022
+Created on 12/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_config20200907"
 NAME = "alibabacloud_config20200907" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud CloudConfig (20200907) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util>=0.3.8, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
-    "alibabacloud_openapi_util>=0.2.0, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

