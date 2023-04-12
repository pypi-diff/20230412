# Comparing `tmp/aliyun-python-sdk-r-kvstore-2.8.0.tar.gz` & `tmp/aliyun-python-sdk-r-kvstore-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-r-kvstore-2.8.0.tar", last modified: Wed Oct 21 12:31:33 2020, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-r-kvstore-2.9.0.tar", last modified: Fri Nov 13 09:36:44 2020, max compression
```

## Comparing `aliyun-python-sdk-r-kvstore-2.8.0.tar` & `aliyun-python-sdk-r-kvstore-2.9.0.tar`

### file list

```diff
@@ -1,105 +1,110 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-21 12:31:33.000000 aliyun-python-sdk-r-kvstore-2.8.0/
--rw-r--r--   0 root         (0) root         (0)        0 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1567 2020-10-21 12:31:33.000000 aliyun-python-sdk-r-kvstore-2.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      539 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-21 12:31:33.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyun_python_sdk_r_kvstore.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1567 2020-10-21 12:31:33.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyun_python_sdk_r_kvstore.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6438 2020-10-21 12:31:33.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyun_python_sdk_r_kvstore.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-10-21 12:31:33.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyun_python_sdk_r_kvstore.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2020-10-21 12:31:33.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyun_python_sdk_r_kvstore.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2020-10-21 12:31:33.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyun_python_sdk_r_kvstore.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-21 12:31:33.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/
--rw-r--r--   0 root         (0) root         (0)       21 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3350 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-21 12:31:33.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/
--rw-r--r--   0 root         (0) root         (0)        0 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-21 12:31:33.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/
--rw-r--r--   0 root         (0) root         (0)     3259 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/AddShardingNodeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2779 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/AllocateDirectConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2831 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/AllocateInstancePublicConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     3399 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/CreateAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     2411 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/CreateBackupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2433 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/CreateCacheAnalysisTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     5049 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/CreateDedicatedInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     3937 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/CreateDedicatedUserClusterRequest.py
--rw-r--r--   0 root         (0) root         (0)     2483 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/CreateGlobalDistributeCacheRequest.py
--rw-r--r--   0 root         (0) root         (0)     7203 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/CreateInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     4213 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/CreateUserClusterHostRequest.py
--rw-r--r--   0 root         (0) root         (0)     2591 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DeleteAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     2747 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DeleteDedicatedInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2729 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DeleteDedicatedUserClusterRequest.py
--rw-r--r--   0 root         (0) root         (0)     2623 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DeleteInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2571 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DeleteShardingNodeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2867 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DeleteUserClusterHostRequest.py
--rw-r--r--   0 root         (0) root         (0)     2597 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeAccountsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3957 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeAuditRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3517 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeAvailableResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2427 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeBackupPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     3383 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeBackupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3071 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeCacheAnalysisReportListRequest.py
--rw-r--r--   0 root         (0) root         (0)     3247 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeCacheAnalysisReportRequest.py
--rw-r--r--   0 root         (0) root         (0)     2437 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeClusterMemberInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     2437 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeDBInstanceNetInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     3907 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeDedicatedClusterInstanceListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2419 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeDedicatedUserClusterRequest.py
--rw-r--r--   0 root         (0) root         (0)     2813 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeGlobalDistributeCacheRequest.py
--rw-r--r--   0 root         (0) root         (0)     3309 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeHistoryMonitorValuesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2437 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeInstanceAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2791 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeInstanceAutoRenewalAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2425 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeInstanceSSLRequest.py
--rw-r--r--   0 root         (0) root         (0)     5829 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2639 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeIntranetAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2445 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeLogicInstanceTopologyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2255 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeMonitorItemsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2583 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeParametersRequest.py
--rw-r--r--   0 root         (0) root         (0)     4601 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribePriceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2441 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeRegionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     4287 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeRunningLogRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2455 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeSecurityGroupConfigurationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2425 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeSecurityIpsRequest.py
--rw-r--r--   0 root         (0) root         (0)     4097 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeSlowLogRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3499 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeUserClusterHostInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     3109 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeUserClusterHostRequest.py
--rw-r--r--   0 root         (0) root         (0)     2437 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeZonesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2607 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/FlushExpireKeysRequest.py
--rw-r--r--   0 root         (0) root         (0)     2413 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/FlushInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2815 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/GrantAccountPrivilegeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2447 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/InitializeKvstorePermissionRequest.py
--rw-r--r--   0 root         (0) root         (0)     3097 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ListTagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2939 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/MigrateToOtherZoneRequest.py
--rw-r--r--   0 root         (0) root         (0)     2833 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyAccountDescriptionRequest.py
--rw-r--r--   0 root         (0) root         (0)     3047 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyAccountPasswordRequest.py
--rw-r--r--   0 root         (0) root         (0)     3089 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyBackupPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     3223 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyDBInstanceConnectionStringRequest.py
--rw-r--r--   0 root         (0) root         (0)     3319 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyDedicatedInstanceSpecRequest.py
--rw-r--r--   0 root         (0) root         (0)     4085 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyDedicatedUserClusterRequest.py
--rw-r--r--   0 root         (0) root         (0)     3057 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2793 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceAutoRenewalAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2575 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2855 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceMaintainTimeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2813 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceMajorVersionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2813 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceMinorVersionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2869 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceNetExpireTimeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2593 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceSSLRequest.py
--rw-r--r--   0 root         (0) root         (0)     4013 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceSpecRequest.py
--rw-r--r--   0 root         (0) root         (0)     2615 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceVpcAuthModeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2433 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyIntranetAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2615 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyResourceGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2665 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifySecurityGroupConfigurationRequest.py
--rw-r--r--   0 root         (0) root         (0)     3253 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifySecurityIpsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3075 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyUserClusterHostRequest.py
--rw-r--r--   0 root         (0) root         (0)     2433 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ReleaseDirectConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2699 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ReleaseInstancePublicConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     3563 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/RenewInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2869 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ReplaceUserClusterHostRequest.py
--rw-r--r--   0 root         (0) root         (0)     2807 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ResetAccountPasswordRequest.py
--rw-r--r--   0 root         (0) root         (0)     2833 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/RestartInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2577 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/RestoreInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     3345 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/SwitchNetworkRequest.py
--rw-r--r--   0 root         (0) root         (0)     2709 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/SyncDtsStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2923 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/TagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2725 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/TransformToPrePaidRequest.py
--rw-r--r--   0 root         (0) root         (0)     2915 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/UntagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/__init__.py
--rw-r--r--   0 root         (0) root         (0)       38 2020-10-21 12:31:33.000000 aliyun-python-sdk-r-kvstore-2.8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2482 2020-10-21 12:31:32.000000 aliyun-python-sdk-r-kvstore-2.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1567 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      539 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyun_python_sdk_r_kvstore.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1567 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyun_python_sdk_r_kvstore.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6780 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyun_python_sdk_r_kvstore.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyun_python_sdk_r_kvstore.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyun_python_sdk_r_kvstore.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyun_python_sdk_r_kvstore.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/
+-rw-r--r--   0 root         (0) root         (0)       21 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3350 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/
+-rw-r--r--   0 root         (0) root         (0)     3259 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/AddShardingNodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2779 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/AllocateDirectConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/AllocateInstancePublicConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3399 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/CreateAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2411 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/CreateBackupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2433 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/CreateCacheAnalysisTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     5049 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/CreateDedicatedInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3937 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/CreateDedicatedUserClusterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/CreateGlobalDistributeCacheRequest.py
+-rw-r--r--   0 root         (0) root         (0)     7203 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/CreateInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4213 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/CreateUserClusterHostRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2591 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DeleteAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2747 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DeleteDedicatedInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2729 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DeleteDedicatedUserClusterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2623 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DeleteInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2571 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DeleteShardingNodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2867 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DeleteUserClusterHostRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2597 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeAccountsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3957 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeAuditRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3517 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeAvailableResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2427 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeBackupPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3383 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeBackupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3071 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeCacheAnalysisReportListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3247 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeCacheAnalysisReportRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2437 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeClusterMemberInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2437 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeDBInstanceNetInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3907 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeDedicatedClusterInstanceListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2419 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeDedicatedUserClusterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2601 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeEngineVersionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2813 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeGlobalDistributeCacheRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3309 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeHistoryMonitorValuesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2437 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeInstanceAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2791 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeInstanceAutoRenewalAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2431 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeInstanceConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2425 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeInstanceSSLRequest.py
+-rw-r--r--   0 root         (0) root         (0)     5829 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2639 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeIntranetAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2445 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeLogicInstanceTopologyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2255 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeMonitorItemsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2795 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeParameterTemplatesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2583 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeParametersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4601 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribePriceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2441 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2925 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeRoleZoneInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4287 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeRunningLogRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2455 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeSecurityGroupConfigurationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2425 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeSecurityIpsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4097 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeSlowLogRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3213 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeTasksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3499 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeUserClusterHostInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3109 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeUserClusterHostRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2437 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeZonesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2607 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/FlushExpireKeysRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2413 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/FlushInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2815 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/GrantAccountPrivilegeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2269 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/InitializeKvstorePermissionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3097 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ListTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2939 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/MigrateToOtherZoneRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2833 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyAccountDescriptionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3047 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyAccountPasswordRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3089 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyBackupPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3223 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyDBInstanceConnectionStringRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3319 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyDedicatedInstanceSpecRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4085 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyDedicatedUserClusterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3057 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2793 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceAutoRenewalAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2575 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2855 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceMaintainTimeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2813 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceMajorVersionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2813 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceMinorVersionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2869 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceNetExpireTimeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2593 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceSSLRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4013 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceSpecRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2615 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceVpcAuthModeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2433 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyIntranetAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2615 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyResourceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2665 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifySecurityGroupConfigurationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3253 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifySecurityIpsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3075 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyUserClusterHostRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2433 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ReleaseDirectConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2699 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ReleaseInstancePublicConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3563 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/RenewInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2869 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ReplaceUserClusterHostRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2807 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ResetAccountPasswordRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2833 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/RestartInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2577 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/RestoreInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3345 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/SwitchNetworkRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2709 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/SyncDtsStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2923 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/TagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2725 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/TransformToPrePaidRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2915 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/UntagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       38 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2482 2020-11-13 09:36:44.000000 aliyun-python-sdk-r-kvstore-2.9.0/setup.py
```

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/PKG-INFO` & `aliyun-python-sdk-r-kvstore-2.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-r-kvstore
-Version: 2.8.0
+Version: 2.9.0
 Summary: The r-kvstore module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-r-kvstore
```

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/README.rst` & `aliyun-python-sdk-r-kvstore-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyun_python_sdk_r_kvstore.egg-info/PKG-INFO` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyun_python_sdk_r_kvstore.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-r-kvstore
-Version: 2.8.0
+Version: 2.9.0
 Summary: The r-kvstore module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-r-kvstore
```

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyun_python_sdk_r_kvstore.egg-info/SOURCES.txt` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyun_python_sdk_r_kvstore.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -33,30 +33,35 @@
 aliyunsdkr_kvstore/request/v20150101/DescribeBackupsRequest.py
 aliyunsdkr_kvstore/request/v20150101/DescribeCacheAnalysisReportListRequest.py
 aliyunsdkr_kvstore/request/v20150101/DescribeCacheAnalysisReportRequest.py
 aliyunsdkr_kvstore/request/v20150101/DescribeClusterMemberInfoRequest.py
 aliyunsdkr_kvstore/request/v20150101/DescribeDBInstanceNetInfoRequest.py
 aliyunsdkr_kvstore/request/v20150101/DescribeDedicatedClusterInstanceListRequest.py
 aliyunsdkr_kvstore/request/v20150101/DescribeDedicatedUserClusterRequest.py
+aliyunsdkr_kvstore/request/v20150101/DescribeEngineVersionRequest.py
 aliyunsdkr_kvstore/request/v20150101/DescribeGlobalDistributeCacheRequest.py
 aliyunsdkr_kvstore/request/v20150101/DescribeHistoryMonitorValuesRequest.py
 aliyunsdkr_kvstore/request/v20150101/DescribeInstanceAttributeRequest.py
 aliyunsdkr_kvstore/request/v20150101/DescribeInstanceAutoRenewalAttributeRequest.py
+aliyunsdkr_kvstore/request/v20150101/DescribeInstanceConfigRequest.py
 aliyunsdkr_kvstore/request/v20150101/DescribeInstanceSSLRequest.py
 aliyunsdkr_kvstore/request/v20150101/DescribeInstancesRequest.py
 aliyunsdkr_kvstore/request/v20150101/DescribeIntranetAttributeRequest.py
 aliyunsdkr_kvstore/request/v20150101/DescribeLogicInstanceTopologyRequest.py
 aliyunsdkr_kvstore/request/v20150101/DescribeMonitorItemsRequest.py
+aliyunsdkr_kvstore/request/v20150101/DescribeParameterTemplatesRequest.py
 aliyunsdkr_kvstore/request/v20150101/DescribeParametersRequest.py
 aliyunsdkr_kvstore/request/v20150101/DescribePriceRequest.py
 aliyunsdkr_kvstore/request/v20150101/DescribeRegionsRequest.py
+aliyunsdkr_kvstore/request/v20150101/DescribeRoleZoneInfoRequest.py
 aliyunsdkr_kvstore/request/v20150101/DescribeRunningLogRecordsRequest.py
 aliyunsdkr_kvstore/request/v20150101/DescribeSecurityGroupConfigurationRequest.py
 aliyunsdkr_kvstore/request/v20150101/DescribeSecurityIpsRequest.py
 aliyunsdkr_kvstore/request/v20150101/DescribeSlowLogRecordsRequest.py
+aliyunsdkr_kvstore/request/v20150101/DescribeTasksRequest.py
 aliyunsdkr_kvstore/request/v20150101/DescribeUserClusterHostInstanceRequest.py
 aliyunsdkr_kvstore/request/v20150101/DescribeUserClusterHostRequest.py
 aliyunsdkr_kvstore/request/v20150101/DescribeZonesRequest.py
 aliyunsdkr_kvstore/request/v20150101/FlushExpireKeysRequest.py
 aliyunsdkr_kvstore/request/v20150101/FlushInstanceRequest.py
 aliyunsdkr_kvstore/request/v20150101/GrantAccountPrivilegeRequest.py
 aliyunsdkr_kvstore/request/v20150101/InitializeKvstorePermissionRequest.py
```

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/endpoint.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/AddShardingNodeRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/AddShardingNodeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/AllocateDirectConnectionRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/AllocateDirectConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/AllocateInstancePublicConnectionRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/AllocateInstancePublicConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/CreateAccountRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/CreateAccountRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/CreateBackupRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/CreateBackupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/CreateCacheAnalysisTaskRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/CreateCacheAnalysisTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/CreateDedicatedInstanceRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/CreateDedicatedInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/CreateDedicatedUserClusterRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/CreateDedicatedUserClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/CreateGlobalDistributeCacheRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/CreateGlobalDistributeCacheRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/CreateInstanceRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/CreateInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/CreateUserClusterHostRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/CreateUserClusterHostRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DeleteAccountRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DeleteAccountRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DeleteDedicatedInstanceRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DeleteDedicatedInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DeleteDedicatedUserClusterRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DeleteDedicatedUserClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DeleteInstanceRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DeleteInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DeleteShardingNodeRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DeleteShardingNodeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DeleteUserClusterHostRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DeleteUserClusterHostRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeAccountsRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeAccountsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeAuditRecordsRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeAuditRecordsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeAvailableResourceRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeAvailableResourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeBackupPolicyRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeBackupPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeBackupsRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeBackupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeCacheAnalysisReportListRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeCacheAnalysisReportListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeCacheAnalysisReportRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeCacheAnalysisReportRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeClusterMemberInfoRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeClusterMemberInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeDBInstanceNetInfoRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeDBInstanceNetInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeDedicatedClusterInstanceListRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeDedicatedClusterInstanceListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeDedicatedUserClusterRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeDedicatedUserClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeGlobalDistributeCacheRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeGlobalDistributeCacheRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeHistoryMonitorValuesRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeHistoryMonitorValuesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeInstanceAttributeRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeInstanceAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeInstanceAutoRenewalAttributeRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeInstanceAutoRenewalAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeInstanceSSLRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeInstanceSSLRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeInstancesRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeIntranetAttributeRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeIntranetAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeLogicInstanceTopologyRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeLogicInstanceTopologyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeMonitorItemsRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeMonitorItemsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeParametersRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeParametersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribePriceRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribePriceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeRegionsRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeRegionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeRunningLogRecordsRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeRunningLogRecordsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeSecurityGroupConfigurationRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeSecurityGroupConfigurationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeSecurityIpsRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeSecurityIpsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeSlowLogRecordsRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeSlowLogRecordsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeUserClusterHostInstanceRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeUserClusterHostInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeUserClusterHostRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeUserClusterHostRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/DescribeZonesRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeZonesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/FlushExpireKeysRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/FlushExpireKeysRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/FlushInstanceRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/FlushInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/GrantAccountPrivilegeRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/GrantAccountPrivilegeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/InitializeKvstorePermissionRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/SyncDtsStatusRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkr_kvstore.endpoint import endpoint_data
 
-class InitializeKvstorePermissionRequest(RpcRequest):
+class SyncDtsStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'R-kvstore', '2015-01-01', 'InitializeKvstorePermission','redisa')
+		RpcRequest.__init__(self, 'R-kvstore', '2015-01-01', 'SyncDtsStatus','redisa')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
@@ -39,19 +39,19 @@
 
 	def get_SecurityToken(self):
 		return self.get_query_params().get('SecurityToken')
 
 	def set_SecurityToken(self,SecurityToken):
 		self.add_query_param('SecurityToken',SecurityToken)
 
-	def get_ServiceName(self):
-		return self.get_query_params().get('ServiceName')
+	def get_TaskId(self):
+		return self.get_query_params().get('TaskId')
 
-	def set_ServiceName(self,ServiceName):
-		self.add_query_param('ServiceName',ServiceName)
+	def set_TaskId(self,TaskId):
+		self.add_query_param('TaskId',TaskId)
 
 	def get_ResourceOwnerAccount(self):
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
 		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
 
@@ -61,8 +61,20 @@
 	def set_OwnerAccount(self,OwnerAccount):
 		self.add_query_param('OwnerAccount',OwnerAccount)
 
 	def get_OwnerId(self):
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
+		self.add_query_param('OwnerId',OwnerId)
+
+	def get_InstanceId(self):
+		return self.get_query_params().get('InstanceId')
+
+	def set_InstanceId(self,InstanceId):
+		self.add_query_param('InstanceId',InstanceId)
+
+	def get_Status(self):
+		return self.get_query_params().get('Status')
+
+	def set_Status(self,Status):
+		self.add_query_param('Status',Status)
```

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ListTagResourcesRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ListTagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/MigrateToOtherZoneRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/MigrateToOtherZoneRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyAccountDescriptionRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyAccountDescriptionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyAccountPasswordRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyAccountPasswordRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyBackupPolicyRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyBackupPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyDBInstanceConnectionStringRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyDBInstanceConnectionStringRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyDedicatedInstanceSpecRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyDedicatedInstanceSpecRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyDedicatedUserClusterRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyDedicatedUserClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceAttributeRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceAutoRenewalAttributeRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceAutoRenewalAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceConfigRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceMaintainTimeRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceMaintainTimeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceMajorVersionRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceMajorVersionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceMinorVersionRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceMinorVersionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceNetExpireTimeRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceNetExpireTimeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceSSLRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceSSLRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceSpecRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceSpecRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceVpcAuthModeRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyInstanceVpcAuthModeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyIntranetAttributeRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyIntranetAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyResourceGroupRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyResourceGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifySecurityGroupConfigurationRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifySecurityGroupConfigurationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifySecurityIpsRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifySecurityIpsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ModifyUserClusterHostRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ModifyUserClusterHostRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ReleaseDirectConnectionRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ReleaseDirectConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ReleaseInstancePublicConnectionRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ReleaseInstancePublicConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/RenewInstanceRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/RenewInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ReplaceUserClusterHostRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ReplaceUserClusterHostRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/ResetAccountPasswordRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/ResetAccountPasswordRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/RestartInstanceRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/RestartInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/RestoreInstanceRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/RestoreInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/SwitchNetworkRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/SwitchNetworkRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/SyncDtsStatusRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/TransformToPrePaidRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkr_kvstore.endpoint import endpoint_data
 
-class SyncDtsStatusRequest(RpcRequest):
+class TransformToPrePaidRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'R-kvstore', '2015-01-01', 'SyncDtsStatus','redisa')
+		RpcRequest.__init__(self, 'R-kvstore', '2015-01-01', 'TransformToPrePaid','redisa')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
@@ -39,19 +39,25 @@
 
 	def get_SecurityToken(self):
 		return self.get_query_params().get('SecurityToken')
 
 	def set_SecurityToken(self,SecurityToken):
 		self.add_query_param('SecurityToken',SecurityToken)
 
-	def get_TaskId(self):
-		return self.get_query_params().get('TaskId')
+	def get_Period(self):
+		return self.get_query_params().get('Period')
 
-	def set_TaskId(self,TaskId):
-		self.add_query_param('TaskId',TaskId)
+	def set_Period(self,Period):
+		self.add_query_param('Period',Period)
+
+	def get_AutoPay(self):
+		return self.get_query_params().get('AutoPay')
+
+	def set_AutoPay(self,AutoPay):
+		self.add_query_param('AutoPay',AutoPay)
 
 	def get_ResourceOwnerAccount(self):
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
 		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
 
@@ -67,14 +73,8 @@
 	def set_OwnerId(self,OwnerId):
 		self.add_query_param('OwnerId',OwnerId)
 
 	def get_InstanceId(self):
 		return self.get_query_params().get('InstanceId')
 
 	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_Status(self):
-		return self.get_query_params().get('Status')
-
-	def set_Status(self,Status):
-		self.add_query_param('Status',Status)
+		self.add_query_param('InstanceId',InstanceId)
```

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/TagResourcesRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/TagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/TransformToPrePaidRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/DescribeParameterTemplatesRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,48 +16,48 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkr_kvstore.endpoint import endpoint_data
 
-class TransformToPrePaidRequest(RpcRequest):
+class DescribeParameterTemplatesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'R-kvstore', '2015-01-01', 'TransformToPrePaid','redisa')
+		RpcRequest.__init__(self, 'R-kvstore', '2015-01-01', 'DescribeParameterTemplates','redisa')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
 
+	def get_EngineVersion(self):
+		return self.get_query_params().get('EngineVersion')
+
+	def set_EngineVersion(self,EngineVersion):
+		self.add_query_param('EngineVersion',EngineVersion)
+
 	def get_SecurityToken(self):
 		return self.get_query_params().get('SecurityToken')
 
 	def set_SecurityToken(self,SecurityToken):
 		self.add_query_param('SecurityToken',SecurityToken)
 
-	def get_Period(self):
-		return self.get_query_params().get('Period')
-
-	def set_Period(self,Period):
-		self.add_query_param('Period',Period)
-
-	def get_AutoPay(self):
-		return self.get_query_params().get('AutoPay')
+	def get_Engine(self):
+		return self.get_query_params().get('Engine')
 
-	def set_AutoPay(self,AutoPay):
-		self.add_query_param('AutoPay',AutoPay)
+	def set_Engine(self,Engine):
+		self.add_query_param('Engine',Engine)
 
 	def get_ResourceOwnerAccount(self):
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
 		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
 
@@ -69,12 +69,12 @@
 
 	def get_OwnerId(self):
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self,OwnerId):
 		self.add_query_param('OwnerId',OwnerId)
 
-	def get_InstanceId(self):
-		return self.get_query_params().get('InstanceId')
+	def get_CharacterType(self):
+		return self.get_query_params().get('CharacterType')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_CharacterType(self,CharacterType):
+		self.add_query_param('CharacterType',CharacterType)
```

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/aliyunsdkr_kvstore/request/v20150101/UntagResourcesRequest.py` & `aliyun-python-sdk-r-kvstore-2.9.0/aliyunsdkr_kvstore/request/v20150101/UntagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-r-kvstore-2.8.0/setup.py` & `aliyun-python-sdk-r-kvstore-2.9.0/setup.py`

 * *Files identical despite different names*

