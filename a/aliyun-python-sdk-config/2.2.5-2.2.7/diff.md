# Comparing `tmp/aliyun-python-sdk-config-2.2.5.tar.gz` & `tmp/aliyun-python-sdk-config-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-config-2.2.5.tar", last modified: Wed Apr 12 14:46:15 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-config-2.2.7.tar", last modified: Wed Apr 12 15:19:41 2023, max compression
```

## Comparing `aliyun-python-sdk-config-2.2.5.tar` & `aliyun-python-sdk-config-2.2.7.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/
--rw-r--r--   0 root         (0) root         (0)      575 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1552 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      533 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyun_python_sdk_config.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1552 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyun_python_sdk_config.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8291 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyun_python_sdk_config.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyun_python_sdk_config.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyun_python_sdk_config.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyun_python_sdk_config.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1202 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/
--rw-r--r--   0 root         (0) root         (0)     1706 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ActiveAggregateConfigRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1963 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/AttachAggregateConfigRuleToCompliancePackRequest.py
--rw-r--r--   0 root         (0) root         (0)     1742 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/AttachConfigRuleToCompliancePackRequest.py
--rw-r--r--   0 root         (0) root         (0)     1979 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/CopyCompliancePacksRequest.py
--rw-r--r--   0 root         (0) root         (0)     1947 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/CopyConfigRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     4162 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/CreateAggregateCompliancePackRequest.py
--rw-r--r--   0 root         (0) root         (0)     4362 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/CreateAggregateConfigDeliveryChannelRequest.py
--rw-r--r--   0 root         (0) root         (0)     5870 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/CreateAggregateConfigRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2916 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/CreateAggregateRemediationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2354 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/CreateAggregatorRequest.py
--rw-r--r--   0 root         (0) root         (0)     3942 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/CreateCompliancePackRequest.py
--rw-r--r--   0 root         (0) root         (0)     4141 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/CreateConfigDeliveryChannelRequest.py
--rw-r--r--   0 root         (0) root         (0)     4918 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/CreateConfigRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     4166 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/CreateDeliveryChannelRequest.py
--rw-r--r--   0 root         (0) root         (0)     2696 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/CreateRemediationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1710 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/DeactiveAggregateConfigRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1489 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/DeactiveConfigRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2124 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/DeleteAggregateCompliancePacksRequest.py
--rw-r--r--   0 root         (0) root         (0)     1750 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/DeleteAggregateConfigDeliveryChannelRequest.py
--rw-r--r--   0 root         (0) root         (0)     1706 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/DeleteAggregateConfigRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1712 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/DeleteAggregateRemediationsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1680 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/DeleteAggregatorsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1904 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/DeleteCompliancePacksRequest.py
--rw-r--r--   0 root         (0) root         (0)     1529 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/DeleteConfigDeliveryChannelRequest.py
--rw-r--r--   0 root         (0) root         (0)     1492 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/DeleteRemediationsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1963 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/DetachAggregateConfigRuleToCompliancePackRequest.py
--rw-r--r--   0 root         (0) root         (0)     1742 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/DetachConfigRuleToCompliancePackRequest.py
--rw-r--r--   0 root         (0) root         (0)     1782 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/EvaluatePreConfigRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1940 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GenerateAggregateCompliancePackReportRequest.py
--rw-r--r--   0 root         (0) root         (0)     1916 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GenerateAggregateConfigRulesReportRequest.py
--rw-r--r--   0 root         (0) root         (0)     1720 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GenerateCompliancePackReportRequest.py
--rw-r--r--   0 root         (0) root         (0)     1696 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GenerateConfigRulesReportRequest.py
--rw-r--r--   0 root         (0) root         (0)     1741 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetAggregateAccountComplianceByPackRequest.py
--rw-r--r--   0 root         (0) root         (0)     1735 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetAggregateCompliancePackReportRequest.py
--rw-r--r--   0 root         (0) root         (0)     1723 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetAggregateCompliancePackRequest.py
--rw-r--r--   0 root         (0) root         (0)     1744 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetAggregateConfigDeliveryChannelRequest.py
--rw-r--r--   0 root         (0) root         (0)     1747 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetAggregateConfigRuleComplianceByPackRequest.py
--rw-r--r--   0 root         (0) root         (0)     1692 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetAggregateConfigRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1524 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetAggregateConfigRuleSummaryByRiskLevelRequest.py
--rw-r--r--   0 root         (0) root         (0)     1682 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetAggregateConfigRulesReportRequest.py
--rw-r--r--   0 root         (0) root         (0)     2511 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetAggregateDiscoveredResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2176 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetAggregateResourceComplianceByConfigRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1743 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetAggregateResourceComplianceByPackRequest.py
--rw-r--r--   0 root         (0) root         (0)     1740 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetAggregateResourceComplianceGroupByRegionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1752 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetAggregateResourceComplianceGroupByResourceTypeRequest.py
--rw-r--r--   0 root         (0) root         (0)     3255 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetAggregateResourceComplianceTimelineRequest.py
--rw-r--r--   0 root         (0) root         (0)     3261 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetAggregateResourceConfigurationTimelineRequest.py
--rw-r--r--   0 root         (0) root         (0)     2351 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetAggregateResourceCountsGroupByRegionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2327 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetAggregateResourceCountsGroupByResourceTypeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1470 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetAggregatorRequest.py
--rw-r--r--   0 root         (0) root         (0)     1514 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetCompliancePackReportRequest.py
--rw-r--r--   0 root         (0) root         (0)     1502 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetCompliancePackRequest.py
--rw-r--r--   0 root         (0) root         (0)     1523 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetConfigDeliveryChannelRequest.py
--rw-r--r--   0 root         (0) root         (0)     1526 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetConfigRuleComplianceByPackRequest.py
--rw-r--r--   0 root         (0) root         (0)     1471 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetConfigRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1303 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetConfigRuleSummaryByRiskLevelRequest.py
--rw-r--r--   0 root         (0) root         (0)     1461 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetConfigRulesReportRequest.py
--rw-r--r--   0 root         (0) root         (0)     1525 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetDiscoveredResourceCountsGroupByRegionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1501 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetDiscoveredResourceCountsGroupByResourceTypeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1844 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetDiscoveredResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1490 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetIntegratedServiceStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1461 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetManagedRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1725 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetResourceComplianceByConfigRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1522 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetResourceComplianceByPackRequest.py
--rw-r--r--   0 root         (0) root         (0)     1519 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetResourceComplianceGroupByRegionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1531 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetResourceComplianceGroupByResourceTypeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2588 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetResourceComplianceTimelineRequest.py
--rw-r--r--   0 root         (0) root         (0)     2594 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetResourceConfigurationTimelineRequest.py
--rw-r--r--   0 root         (0) root         (0)     2272 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/IgnoreAggregateEvaluationResultsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2052 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/IgnoreEvaluationResultsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2042 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListAggregateCompliancePacksRequest.py
--rw-r--r--   0 root         (0) root         (0)     1754 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListAggregateConfigDeliveryChannelsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3603 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListAggregateConfigRuleEvaluationResultsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3087 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListAggregateConfigRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3129 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListAggregateDiscoveredResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1704 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListAggregateRemediationsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2675 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListAggregateResourceEvaluationResultsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1650 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListAggregatorsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2154 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListCompliancePackTemplatesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1821 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListCompliancePacksRequest.py
--rw-r--r--   0 root         (0) root         (0)     1533 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListConfigDeliveryChannelsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2935 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListConfigRuleEvaluationResultsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2866 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListConfigRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2462 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListDiscoveredResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2217 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListManagedRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1870 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListPreManagedRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1768 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListRemediationTemplatesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1483 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListRemediationsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2454 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListResourceEvaluationResultsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2077 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListTagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1916 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/RevertAggregateEvaluationResultsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1696 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/RevertEvaluationResultsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2172 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/StartAggregateConfigRuleEvaluationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1698 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/StartAggregateRemediationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1477 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/StartRemediationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1292 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/StopConfigurationRecorderRequest.py
--rw-r--r--   0 root         (0) root         (0)     1885 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/TagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2132 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/UntagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3904 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/UpdateAggregateCompliancePackRequest.py
--rw-r--r--   0 root         (0) root         (0)     4513 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/UpdateAggregateConfigDeliveryChannelRequest.py
--rw-r--r--   0 root         (0) root         (0)     5650 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/UpdateAggregateConfigRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2726 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/UpdateAggregateRemediationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2342 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/UpdateAggregatorRequest.py
--rw-r--r--   0 root         (0) root         (0)     3684 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/UpdateCompliancePackRequest.py
--rw-r--r--   0 root         (0) root         (0)     4292 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/UpdateConfigDeliveryChannelRequest.py
--rw-r--r--   0 root         (0) root         (0)     4698 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/UpdateConfigRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     4316 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/UpdateDeliveryChannelRequest.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/UpdateIntegratedServiceStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2702 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/UpdateRemediationRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2467 2023-04-12 14:46:15.000000 aliyun-python-sdk-config-2.2.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1552 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      533 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyun_python_sdk_config.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1552 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyun_python_sdk_config.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8291 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyun_python_sdk_config.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyun_python_sdk_config.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyun_python_sdk_config.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyun_python_sdk_config.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1202 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/
+-rw-r--r--   0 root         (0) root         (0)     1706 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ActiveAggregateConfigRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1963 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/AttachAggregateConfigRuleToCompliancePackRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1742 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/AttachConfigRuleToCompliancePackRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1979 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/CopyCompliancePacksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1947 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/CopyConfigRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4162 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/CreateAggregateCompliancePackRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4362 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/CreateAggregateConfigDeliveryChannelRequest.py
+-rw-r--r--   0 root         (0) root         (0)     5870 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/CreateAggregateConfigRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2916 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/CreateAggregateRemediationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/CreateAggregatorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3942 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/CreateCompliancePackRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4141 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/CreateConfigDeliveryChannelRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4918 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/CreateConfigRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4166 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/CreateDeliveryChannelRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2696 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/CreateRemediationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/DeactiveAggregateConfigRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/DeactiveConfigRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2124 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/DeleteAggregateCompliancePacksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1750 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/DeleteAggregateConfigDeliveryChannelRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1706 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/DeleteAggregateConfigRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1712 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/DeleteAggregateRemediationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1680 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/DeleteAggregatorsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1904 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/DeleteCompliancePacksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/DeleteConfigDeliveryChannelRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1492 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/DeleteRemediationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1963 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/DetachAggregateConfigRuleToCompliancePackRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1742 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/DetachConfigRuleToCompliancePackRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/EvaluatePreConfigRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1940 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GenerateAggregateCompliancePackReportRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1916 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GenerateAggregateConfigRulesReportRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1720 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GenerateCompliancePackReportRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1696 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GenerateConfigRulesReportRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetAggregateAccountComplianceByPackRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetAggregateCompliancePackReportRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1723 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetAggregateCompliancePackRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1744 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetAggregateConfigDeliveryChannelRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1747 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetAggregateConfigRuleComplianceByPackRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetAggregateConfigRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1524 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetAggregateConfigRuleSummaryByRiskLevelRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1682 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetAggregateConfigRulesReportRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetAggregateDiscoveredResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2393 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetAggregateResourceComplianceByConfigRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1743 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetAggregateResourceComplianceByPackRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetAggregateResourceComplianceGroupByRegionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1752 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetAggregateResourceComplianceGroupByResourceTypeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3255 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetAggregateResourceComplianceTimelineRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3261 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetAggregateResourceConfigurationTimelineRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2351 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetAggregateResourceCountsGroupByRegionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2327 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetAggregateResourceCountsGroupByResourceTypeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1470 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetAggregatorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1514 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetCompliancePackReportRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1502 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetCompliancePackRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1523 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetConfigDeliveryChannelRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1526 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetConfigRuleComplianceByPackRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1471 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetConfigRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1303 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetConfigRuleSummaryByRiskLevelRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetConfigRulesReportRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1525 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetDiscoveredResourceCountsGroupByRegionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1501 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetDiscoveredResourceCountsGroupByResourceTypeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1844 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetDiscoveredResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetIntegratedServiceStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetManagedRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1725 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetResourceComplianceByConfigRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1522 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetResourceComplianceByPackRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1519 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetResourceComplianceGroupByRegionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1531 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetResourceComplianceGroupByResourceTypeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2588 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetResourceComplianceTimelineRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2594 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetResourceConfigurationTimelineRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2272 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/IgnoreAggregateEvaluationResultsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2052 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/IgnoreEvaluationResultsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2042 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListAggregateCompliancePacksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1754 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListAggregateConfigDeliveryChannelsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3603 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListAggregateConfigRuleEvaluationResultsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3087 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListAggregateConfigRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3129 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListAggregateDiscoveredResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListAggregateRemediationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2675 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListAggregateResourceEvaluationResultsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListAggregatorsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2154 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListCompliancePackTemplatesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1821 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListCompliancePacksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListConfigDeliveryChannelsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2935 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListConfigRuleEvaluationResultsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2866 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListConfigRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListDiscoveredResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2217 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListManagedRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1870 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListPreManagedRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListRemediationTemplatesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1483 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListRemediationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2454 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListResourceEvaluationResultsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2077 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1916 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/RevertAggregateEvaluationResultsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1696 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/RevertEvaluationResultsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2172 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/StartAggregateConfigRuleEvaluationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/StartAggregateRemediationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1477 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/StartRemediationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1292 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/StopConfigurationRecorderRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1885 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/TagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2132 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/UntagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3904 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/UpdateAggregateCompliancePackRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4513 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/UpdateAggregateConfigDeliveryChannelRequest.py
+-rw-r--r--   0 root         (0) root         (0)     5650 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/UpdateAggregateConfigRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2726 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/UpdateAggregateRemediationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2342 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/UpdateAggregatorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3684 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/UpdateCompliancePackRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4292 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/UpdateConfigDeliveryChannelRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4698 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/UpdateConfigRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4316 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/UpdateDeliveryChannelRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/UpdateIntegratedServiceStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2702 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/UpdateRemediationRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2467 2023-04-12 15:19:41.000000 aliyun-python-sdk-config-2.2.7/setup.py
```

### Comparing `aliyun-python-sdk-config-2.2.5/LICENSE` & `aliyun-python-sdk-config-2.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/PKG-INFO` & `aliyun-python-sdk-config-2.2.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-config
-Version: 2.2.5
+Version: 2.2.7
 Summary: The config module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-config
```

### Comparing `aliyun-python-sdk-config-2.2.5/README.rst` & `aliyun-python-sdk-config-2.2.7/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyun_python_sdk_config.egg-info/PKG-INFO` & `aliyun-python-sdk-config-2.2.7/aliyun_python_sdk_config.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-config
-Version: 2.2.5
+Version: 2.2.7
 Summary: The config module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-config
```

### Comparing `aliyun-python-sdk-config-2.2.5/aliyun_python_sdk_config.egg-info/SOURCES.txt` & `aliyun-python-sdk-config-2.2.7/aliyun_python_sdk_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/endpoint.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ActiveAggregateConfigRulesRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ActiveAggregateConfigRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/AttachAggregateConfigRuleToCompliancePackRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/AttachAggregateConfigRuleToCompliancePackRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/AttachConfigRuleToCompliancePackRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/AttachConfigRuleToCompliancePackRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/CopyCompliancePacksRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/CopyCompliancePacksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/CopyConfigRulesRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/CopyConfigRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/CreateAggregateCompliancePackRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/CreateAggregateCompliancePackRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/CreateAggregateConfigDeliveryChannelRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/CreateAggregateConfigDeliveryChannelRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/CreateAggregateConfigRuleRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/CreateAggregateConfigRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/CreateAggregateRemediationRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/CreateAggregateRemediationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/CreateAggregatorRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/CreateAggregatorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/CreateCompliancePackRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/CreateCompliancePackRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/CreateConfigDeliveryChannelRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/CreateConfigDeliveryChannelRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/CreateConfigRuleRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/CreateConfigRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/CreateDeliveryChannelRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/CreateDeliveryChannelRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/CreateRemediationRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/CreateRemediationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/DeactiveAggregateConfigRulesRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/DeactiveAggregateConfigRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/DeactiveConfigRulesRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/DeactiveConfigRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/DeleteAggregateCompliancePacksRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/DeleteAggregateCompliancePacksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/DeleteAggregateConfigDeliveryChannelRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/DeleteAggregateConfigDeliveryChannelRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/DeleteAggregateConfigRulesRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/DeleteAggregateConfigRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/DeleteAggregateRemediationsRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/DeleteAggregateRemediationsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/DeleteAggregatorsRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/DeleteAggregatorsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/DeleteCompliancePacksRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/DeleteCompliancePacksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/DeleteConfigDeliveryChannelRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/DeleteConfigDeliveryChannelRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/DeleteRemediationsRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/DeleteRemediationsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/DetachAggregateConfigRuleToCompliancePackRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/DetachAggregateConfigRuleToCompliancePackRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/DetachConfigRuleToCompliancePackRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/DetachConfigRuleToCompliancePackRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/EvaluatePreConfigRulesRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/EvaluatePreConfigRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GenerateAggregateCompliancePackReportRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GenerateAggregateCompliancePackReportRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GenerateAggregateConfigRulesReportRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GenerateAggregateConfigRulesReportRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GenerateCompliancePackReportRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GenerateCompliancePackReportRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GenerateConfigRulesReportRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GenerateConfigRulesReportRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetAggregateAccountComplianceByPackRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetAggregateAccountComplianceByPackRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetAggregateCompliancePackReportRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetAggregateCompliancePackReportRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetAggregateCompliancePackRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetAggregateCompliancePackRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetAggregateConfigDeliveryChannelRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetAggregateConfigDeliveryChannelRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetAggregateConfigRuleComplianceByPackRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetAggregateConfigRuleComplianceByPackRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetAggregateConfigRuleRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetAggregateConfigRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetAggregateConfigRuleSummaryByRiskLevelRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetAggregateConfigRuleSummaryByRiskLevelRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetAggregateConfigRulesReportRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetAggregateConfigRulesReportRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetAggregateDiscoveredResourceRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetAggregateDiscoveredResourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetAggregateResourceComplianceByConfigRuleRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetAggregateResourceComplianceByConfigRuleRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,19 @@
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ConfigRuleId(self): # String
 		return self.get_query_params().get('ConfigRuleId')
 
 	def set_ConfigRuleId(self, ConfigRuleId):  # String
 		self.add_query_param('ConfigRuleId', ConfigRuleId)
+	def get_ResourceOwnerId(self): # Long
+		return self.get_query_params().get('ResourceOwnerId')
+
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
 	def get_AggregatorId(self): # String
 		return self.get_query_params().get('AggregatorId')
 
 	def set_AggregatorId(self, AggregatorId):  # String
 		self.add_query_param('AggregatorId', AggregatorId)
 	def get_ResourceAccountId(self): # Long
 		return self.get_query_params().get('ResourceAccountId')
```

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetAggregateResourceComplianceByPackRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetAggregateResourceComplianceByPackRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetAggregateResourceComplianceGroupByRegionRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetAggregateResourceComplianceGroupByRegionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetAggregateResourceComplianceGroupByResourceTypeRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetAggregateResourceComplianceGroupByResourceTypeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetAggregateResourceComplianceTimelineRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetAggregateResourceComplianceTimelineRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetAggregateResourceConfigurationTimelineRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetAggregateResourceConfigurationTimelineRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetAggregateResourceCountsGroupByRegionRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetAggregateResourceCountsGroupByRegionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetAggregateResourceCountsGroupByResourceTypeRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetAggregateResourceCountsGroupByResourceTypeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetAggregatorRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetAggregatorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetCompliancePackReportRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetCompliancePackReportRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetCompliancePackRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetCompliancePackRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetConfigDeliveryChannelRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetConfigDeliveryChannelRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetConfigRuleComplianceByPackRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetConfigRuleComplianceByPackRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetConfigRuleRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetConfigRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetConfigRuleSummaryByRiskLevelRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetConfigRuleSummaryByRiskLevelRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetConfigRulesReportRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetConfigRulesReportRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetDiscoveredResourceCountsGroupByRegionRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetDiscoveredResourceCountsGroupByRegionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetDiscoveredResourceCountsGroupByResourceTypeRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetDiscoveredResourceCountsGroupByResourceTypeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetDiscoveredResourceRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetDiscoveredResourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetIntegratedServiceStatusRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetIntegratedServiceStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetManagedRuleRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetManagedRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetResourceComplianceByConfigRuleRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetResourceComplianceByConfigRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetResourceComplianceByPackRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetResourceComplianceByPackRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetResourceComplianceGroupByRegionRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetResourceComplianceGroupByRegionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetResourceComplianceGroupByResourceTypeRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetResourceComplianceGroupByResourceTypeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetResourceComplianceTimelineRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetResourceComplianceTimelineRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/GetResourceConfigurationTimelineRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/GetResourceConfigurationTimelineRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/IgnoreAggregateEvaluationResultsRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/IgnoreAggregateEvaluationResultsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/IgnoreEvaluationResultsRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/IgnoreEvaluationResultsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListAggregateCompliancePacksRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListAggregateCompliancePacksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListAggregateConfigDeliveryChannelsRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListAggregateConfigDeliveryChannelsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListAggregateConfigRuleEvaluationResultsRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListAggregateConfigRuleEvaluationResultsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListAggregateConfigRulesRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListAggregateConfigRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListAggregateDiscoveredResourcesRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListAggregateDiscoveredResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListAggregateRemediationsRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListAggregateRemediationsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListAggregateResourceEvaluationResultsRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListAggregateResourceEvaluationResultsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListAggregatorsRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListAggregatorsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListCompliancePackTemplatesRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListCompliancePackTemplatesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListCompliancePacksRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListCompliancePacksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListConfigDeliveryChannelsRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListConfigDeliveryChannelsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListConfigRuleEvaluationResultsRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListConfigRuleEvaluationResultsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListConfigRulesRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListConfigRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListDiscoveredResourcesRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListDiscoveredResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListManagedRulesRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListManagedRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListPreManagedRulesRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListPreManagedRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListRemediationTemplatesRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListRemediationTemplatesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListRemediationsRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListRemediationsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListResourceEvaluationResultsRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListResourceEvaluationResultsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/ListTagResourcesRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/ListTagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/RevertAggregateEvaluationResultsRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/RevertAggregateEvaluationResultsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/RevertEvaluationResultsRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/RevertEvaluationResultsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/StartAggregateConfigRuleEvaluationRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/StartAggregateConfigRuleEvaluationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/StartAggregateRemediationRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/StartAggregateRemediationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/StartRemediationRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/StartRemediationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/StopConfigurationRecorderRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/StopConfigurationRecorderRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/TagResourcesRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/TagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/UntagResourcesRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/UntagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/UpdateAggregateCompliancePackRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/UpdateAggregateCompliancePackRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/UpdateAggregateConfigDeliveryChannelRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/UpdateAggregateConfigDeliveryChannelRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/UpdateAggregateConfigRuleRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/UpdateAggregateConfigRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/UpdateAggregateRemediationRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/UpdateAggregateRemediationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/UpdateAggregatorRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/UpdateAggregatorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/UpdateCompliancePackRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/UpdateCompliancePackRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/UpdateConfigDeliveryChannelRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/UpdateConfigDeliveryChannelRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/UpdateConfigRuleRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/UpdateConfigRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/UpdateDeliveryChannelRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/UpdateDeliveryChannelRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/UpdateIntegratedServiceStatusRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/UpdateIntegratedServiceStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/aliyunsdkconfig/request/v20200907/UpdateRemediationRequest.py` & `aliyun-python-sdk-config-2.2.7/aliyunsdkconfig/request/v20200907/UpdateRemediationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-config-2.2.5/setup.py` & `aliyun-python-sdk-config-2.2.7/setup.py`

 * *Files identical despite different names*

