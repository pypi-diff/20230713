# Comparing `tmp/aliyun-python-sdk-mse-3.0.6.tar.gz` & `tmp/aliyun-python-sdk-mse-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-mse-3.0.6.tar", last modified: Thu Feb 10 01:24:17 2022, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-mse-3.0.7.tar", last modified: Wed Feb 16 02:37:32 2022, max compression
```

## Comparing `aliyun-python-sdk-mse-3.0.6.tar` & `aliyun-python-sdk-mse-3.0.7.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/
--rw-r--r--   0 root         (0) root         (0)      575 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1537 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      527 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyun_python_sdk_mse.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1537 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyun_python_sdk_mse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6912 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyun_python_sdk_mse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyun_python_sdk_mse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyun_python_sdk_mse.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyun_python_sdk_mse.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/
--rw-r--r--   0 root         (0) root         (0)       21 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1088 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/
--rw-r--r--   0 root         (0) root         (0)     2195 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/AddAuthResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2579 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/AddBlackWhiteListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2440 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/AddGatewayDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     3313 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/AddGatewayRequest.py
--rw-r--r--   0 root         (0) root         (0)     2116 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/AddGatewayServiceVersionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2014 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/AddGatewaySlbRequest.py
--rw-r--r--   0 root         (0) root         (0)     3548 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/AddMockRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2081 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/AddSSLCertRequest.py
--rw-r--r--   0 root         (0) root         (0)     2354 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/AddServiceSourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2456 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/CloneNacosConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     3170 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/CreateAlarmRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2356 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/CreateApplicationRequest.py
--rw-r--r--   0 root         (0) root         (0)     4753 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/CreateClusterRequest.py
--rw-r--r--   0 root         (0) root         (0)     2384 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/CreateEngineNamespaceRequest.py
--rw-r--r--   0 root         (0) root         (0)     3185 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/CreateNacosConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     3463 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/CreateNacosInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2856 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/CreateNacosServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1968 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/CreateZnodeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1875 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/DeleteAlarmRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1846 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/DeleteAuthResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1668 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/DeleteClusterRequest.py
--rw-r--r--   0 root         (0) root         (0)     2012 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/DeleteEngineNamespaceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1852 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/DeleteGatewayDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     1884 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/DeleteGatewayRequest.py
--rw-r--r--   0 root         (0) root         (0)     2122 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/DeleteGatewayServiceVersionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2033 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/DeleteGatewaySlbRequest.py
--rw-r--r--   0 root         (0) root         (0)     2358 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/DeleteNacosConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2024 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/DeleteNacosConfigsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2257 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/DeleteNacosServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1884 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/DeleteServiceSourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2010 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/DeleteZnodeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2523 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ExportNacosConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2063 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/GetBlackWhiteListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2004 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/GetEngineNamepaceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1858 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/GetGatewayDomainDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     1885 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/GetGatewayOptionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1691 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/GetGatewayRequest.py
--rw-r--r--   0 root         (0) root         (0)     1898 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/GetGatewayServiceDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     2275 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/GetGovernanceKubernetesClusterListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1696 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/GetGovernanceKubernetesClusterRequest.py
--rw-r--r--   0 root         (0) root         (0)     1664 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/GetImageRequest.py
--rw-r--r--   0 root         (0) root         (0)     2068 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/GetImportFileUrlRequest.py
--rw-r--r--   0 root         (0) root         (0)     1709 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/GetKubernetesSourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1489 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/GetMseFeatureSwitchRequest.py
--rw-r--r--   0 root         (0) root         (0)     1695 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/GetMseSourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2352 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/GetNacosConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2358 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/GetNacosHistoryConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1809 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/GetOverviewRequest.py
--rw-r--r--   0 root         (0) root         (0)     2213 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ImportNacosConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2289 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ImportServicesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2047 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListAlarmContactGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2777 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListAlarmHistoriesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1675 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListAlarmItemsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2234 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListAlarmRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3187 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListAnsInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3199 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListAnsServiceClustersRequest.py
--rw-r--r--   0 root         (0) root         (0)     3179 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListAnsServicesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1503 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListClusterConnectionTypesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1483 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListClusterTypesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1686 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListClusterVersionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2254 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListClustersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1681 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListEngineNamespacesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2423 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListEurekaInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2224 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListEurekaServicesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1705 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListGatewayDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     2440 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListGatewayRequest.py
--rw-r--r--   0 root         (0) root         (0)     2454 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListGatewayServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1699 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListGatewaySlbRequest.py
--rw-r--r--   0 root         (0) root         (0)     2406 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListListenersByConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2213 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListListenersByIpRequest.py
--rw-r--r--   0 root         (0) root         (0)     3080 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListNacosConfigsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2766 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListNacosHistoryConfigsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1693 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListSSLCertRequest.py
--rw-r--r--   0 root         (0) root         (0)     1705 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListServiceSourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1824 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListZnodeChildrenRequest.py
--rw-r--r--   0 root         (0) root         (0)     1917 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ModifyGovernanceKubernetesClusterRequest.py
--rw-r--r--   0 root         (0) root         (0)     2065 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/PullServicesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1494 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/QueryBusinessLocationsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1851 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/QueryClusterDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     1706 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/QueryClusterDiskSpecificationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1501 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/QueryClusterSpecificationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2236 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/QueryConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1486 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/QueryGatewayRegionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1482 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/QueryGatewayTypeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2270 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/QueryGovernanceKubernetesClusterRequest.py
--rw-r--r--   0 root         (0) root         (0)     2560 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/QueryMonitorRequest.py
--rw-r--r--   0 root         (0) root         (0)     1474 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/QuerySlbSpecRequest.py
--rw-r--r--   0 root         (0) root         (0)     2019 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/QueryZnodeDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     2249 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/RestartClusterRequest.py
--rw-r--r--   0 root         (0) root         (0)     1863 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/RetryClusterRequest.py
--rw-r--r--   0 root         (0) root         (0)     2494 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ScalingClusterRequest.py
--rw-r--r--   0 root         (0) root         (0)     2013 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/SelectGatewaySlbRequest.py
--rw-r--r--   0 root         (0) root         (0)     1863 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/UpdateAclRequest.py
--rw-r--r--   0 root         (0) root         (0)     2549 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/UpdateBlackWhiteListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2092 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/UpdateClusterRequest.py
--rw-r--r--   0 root         (0) root         (0)     5451 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/UpdateConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2527 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/UpdateEngineNamespaceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2430 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/UpdateGatewayDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     1860 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/UpdateGatewayNameRequest.py
--rw-r--r--   0 root         (0) root         (0)     2124 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/UpdateGatewayOptionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2271 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/UpdateGatewayRouteHTTPRewriteRequest.py
--rw-r--r--   0 root         (0) root         (0)     2122 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/UpdateGatewayServiceVersionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1855 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/UpdateImageRequest.py
--rw-r--r--   0 root         (0) root         (0)     3121 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/UpdateNacosClusterRequest.py
--rw-r--r--   0 root         (0) root         (0)     3561 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/UpdateNacosConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     3463 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/UpdateNacosInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2669 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/UpdateNacosServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2087 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/UpdateSSLCertRequest.py
--rw-r--r--   0 root         (0) root         (0)     2165 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/UpdateZnodeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2082 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/UpgradeClusterRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2452 2022-02-10 01:24:17.000000 aliyun-python-sdk-mse-3.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-16 02:37:32.000000 aliyun-python-sdk-mse-3.0.7/
+-rw-r--r--   0 root         (0) root         (0)      575 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1537 2022-02-16 02:37:32.000000 aliyun-python-sdk-mse-3.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      527 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-16 02:37:32.000000 aliyun-python-sdk-mse-3.0.7/aliyun_python_sdk_mse.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1537 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyun_python_sdk_mse.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6912 2022-02-16 02:37:32.000000 aliyun-python-sdk-mse-3.0.7/aliyun_python_sdk_mse.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyun_python_sdk_mse.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyun_python_sdk_mse.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyun_python_sdk_mse.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-16 02:37:32.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-16 02:37:32.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-16 02:37:32.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/
+-rw-r--r--   0 root         (0) root         (0)     2195 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/AddAuthResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2579 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/AddBlackWhiteListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2440 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/AddGatewayDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3313 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/AddGatewayRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2116 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/AddGatewayServiceVersionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2014 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/AddGatewaySlbRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3548 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/AddMockRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2081 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/AddSSLCertRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2354 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/AddServiceSourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2456 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/CloneNacosConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3170 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/CreateAlarmRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2356 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/CreateApplicationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4753 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/CreateClusterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2384 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/CreateEngineNamespaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3185 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/CreateNacosConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3463 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/CreateNacosInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2856 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/CreateNacosServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1968 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/CreateZnodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1875 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/DeleteAlarmRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/DeleteAuthResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/DeleteClusterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2012 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/DeleteEngineNamespaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/DeleteGatewayDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1884 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/DeleteGatewayRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2122 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/DeleteGatewayServiceVersionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2033 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/DeleteGatewaySlbRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2358 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/DeleteNacosConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2024 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/DeleteNacosConfigsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2257 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/DeleteNacosServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1884 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/DeleteServiceSourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2010 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/DeleteZnodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2523 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ExportNacosConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2238 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/GetBlackWhiteListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/GetEngineNamepaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1858 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/GetGatewayDomainDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1885 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/GetGatewayOptionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1691 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/GetGatewayRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1898 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/GetGatewayServiceDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2275 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/GetGovernanceKubernetesClusterListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1696 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/GetGovernanceKubernetesClusterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/GetImageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2068 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/GetImportFileUrlRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/GetKubernetesSourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/GetMseFeatureSwitchRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/GetMseSourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2352 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/GetNacosConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2358 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/GetNacosHistoryConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1809 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/GetOverviewRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ImportNacosConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2289 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ImportServicesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2047 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListAlarmContactGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2777 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListAlarmHistoriesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1675 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListAlarmItemsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2234 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListAlarmRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3187 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListAnsInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3199 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListAnsServiceClustersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3179 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListAnsServicesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1503 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListClusterConnectionTypesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1680 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListClusterTypesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1686 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListClusterVersionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2254 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListClustersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1681 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListEngineNamespacesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2423 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListEurekaInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2224 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListEurekaServicesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1705 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListGatewayDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2440 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListGatewayRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2454 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListGatewayServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1699 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListGatewaySlbRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2406 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListListenersByConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListListenersByIpRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3080 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListNacosConfigsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2766 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListNacosHistoryConfigsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1693 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListSSLCertRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1705 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListServiceSourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1824 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListZnodeChildrenRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ModifyGovernanceKubernetesClusterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2065 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/PullServicesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1494 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/QueryBusinessLocationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1851 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/QueryClusterDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1706 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/QueryClusterDiskSpecificationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/QueryClusterSpecificationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2236 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/QueryConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1486 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/QueryGatewayRegionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1482 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/QueryGatewayTypeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2270 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/QueryGovernanceKubernetesClusterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2560 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/QueryMonitorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1474 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/QuerySlbSpecRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2019 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/QueryZnodeDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2249 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/RestartClusterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/RetryClusterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2494 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ScalingClusterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2013 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/SelectGatewaySlbRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/UpdateAclRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2724 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/UpdateBlackWhiteListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/UpdateClusterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     5451 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/UpdateConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2527 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/UpdateEngineNamespaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2430 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/UpdateGatewayDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1860 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/UpdateGatewayNameRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2124 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/UpdateGatewayOptionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2271 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/UpdateGatewayRouteHTTPRewriteRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2122 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/UpdateGatewayServiceVersionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1855 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/UpdateImageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3121 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/UpdateNacosClusterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3561 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/UpdateNacosConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3463 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/UpdateNacosInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2669 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/UpdateNacosServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2087 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/UpdateSSLCertRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2165 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/UpdateZnodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2082 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/UpgradeClusterRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2022-02-16 02:37:32.000000 aliyun-python-sdk-mse-3.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2452 2022-02-16 02:37:31.000000 aliyun-python-sdk-mse-3.0.7/setup.py
```

### Comparing `aliyun-python-sdk-mse-3.0.6/LICENSE` & `aliyun-python-sdk-mse-3.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/PKG-INFO` & `aliyun-python-sdk-mse-3.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-mse
-Version: 3.0.6
+Version: 3.0.7
 Summary: The mse module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-mse
```

### Comparing `aliyun-python-sdk-mse-3.0.6/README.rst` & `aliyun-python-sdk-mse-3.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyun_python_sdk_mse.egg-info/PKG-INFO` & `aliyun-python-sdk-mse-3.0.7/aliyun_python_sdk_mse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-mse
-Version: 3.0.6
+Version: 3.0.7
 Summary: The mse module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-mse
```

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyun_python_sdk_mse.egg-info/SOURCES.txt` & `aliyun-python-sdk-mse-3.0.7/aliyun_python_sdk_mse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/endpoint.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/AddAuthResourceRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/AddAuthResourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/AddBlackWhiteListRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/AddBlackWhiteListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/AddGatewayDomainRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/AddGatewayDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/AddGatewayRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/AddGatewayRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/AddGatewayServiceVersionRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/AddGatewayServiceVersionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/AddGatewaySlbRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/AddGatewaySlbRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/AddMockRuleRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/AddMockRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/AddSSLCertRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/AddSSLCertRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/AddServiceSourceRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/AddServiceSourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/CloneNacosConfigRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/CloneNacosConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/CreateAlarmRuleRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/CreateAlarmRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/CreateApplicationRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/CreateApplicationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/CreateClusterRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/CreateClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/CreateEngineNamespaceRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/CreateEngineNamespaceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/CreateNacosConfigRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/CreateNacosConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/CreateNacosInstanceRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/CreateNacosInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/CreateNacosServiceRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/CreateNacosServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/CreateZnodeRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/CreateZnodeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/DeleteAlarmRuleRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/DeleteAlarmRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/DeleteAuthResourceRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/DeleteAuthResourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/DeleteClusterRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/DeleteClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/DeleteEngineNamespaceRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/DeleteEngineNamespaceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/DeleteGatewayDomainRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/DeleteGatewayDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/DeleteGatewayRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/DeleteGatewayRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/DeleteGatewayServiceVersionRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/DeleteGatewayServiceVersionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/DeleteGatewaySlbRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/DeleteGatewaySlbRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/DeleteNacosConfigRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/DeleteNacosConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/DeleteNacosConfigsRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/DeleteNacosConfigsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/DeleteNacosServiceRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/DeleteNacosServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/DeleteServiceSourceRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/DeleteServiceSourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/DeleteZnodeRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/DeleteZnodeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ExportNacosConfigRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ExportNacosConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/GetBlackWhiteListRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/GetBlackWhiteListRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,12 +42,17 @@
 	def set_Type(self, Type):  # String
 		self.add_query_param('Type', Type)
 	def get_ResourceType(self): # String
 		return self.get_query_params().get('ResourceType')
 
 	def set_ResourceType(self, ResourceType):  # String
 		self.add_query_param('ResourceType', ResourceType)
+	def get_IsWhite(self): # Boolean
+		return self.get_query_params().get('IsWhite')
+
+	def set_IsWhite(self, IsWhite):  # Boolean
+		self.add_query_param('IsWhite', IsWhite)
 	def get_AcceptLanguage(self): # String
 		return self.get_query_params().get('AcceptLanguage')
 
 	def set_AcceptLanguage(self, AcceptLanguage):  # String
 		self.add_query_param('AcceptLanguage', AcceptLanguage)
```

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/GetEngineNamepaceRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/GetEngineNamepaceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/GetGatewayDomainDetailRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/GetGatewayDomainDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/GetGatewayOptionRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/GetGatewayOptionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/GetGatewayRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/GetGatewayRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/GetGatewayServiceDetailRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/GetGatewayServiceDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/GetGovernanceKubernetesClusterListRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/GetGovernanceKubernetesClusterListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/GetGovernanceKubernetesClusterRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/GetGovernanceKubernetesClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/GetImageRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/GetImageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/GetImportFileUrlRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/GetImportFileUrlRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/GetKubernetesSourceRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/GetKubernetesSourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/GetMseFeatureSwitchRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/GetMseFeatureSwitchRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/GetMseSourceRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/GetMseSourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/GetNacosConfigRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/GetNacosConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/GetNacosHistoryConfigRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/GetNacosHistoryConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/GetOverviewRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/GetOverviewRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ImportNacosConfigRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ImportNacosConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ImportServicesRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ImportServicesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListAlarmContactGroupsRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListAlarmContactGroupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListAlarmHistoriesRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListAlarmHistoriesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListAlarmItemsRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListAlarmItemsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListAlarmRulesRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListAlarmRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListAnsInstancesRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListAnsInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListAnsServiceClustersRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListAnsServiceClustersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListAnsServicesRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListAnsServicesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListClusterConnectionTypesRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListClusterConnectionTypesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListClusterTypesRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/QuerySlbSpecRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkmse.endpoint import endpoint_data
 
-class ListClusterTypesRequest(RpcRequest):
+class QuerySlbSpecRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'mse', '2019-05-31', 'ListClusterTypes')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'mse', '2019-05-31', 'QuerySlbSpec')
+		self.set_method('GET')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_AcceptLanguage(self): # String
```

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListClusterVersionsRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListClusterVersionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListClustersRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListClustersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListEngineNamespacesRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListEngineNamespacesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListEurekaInstancesRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListEurekaInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListEurekaServicesRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListEurekaServicesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListGatewayDomainRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListGatewayDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListGatewayRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListGatewayRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListGatewayServiceRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListGatewayServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListGatewaySlbRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListGatewaySlbRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListListenersByConfigRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListListenersByConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListListenersByIpRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListListenersByIpRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListNacosConfigsRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListNacosConfigsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListNacosHistoryConfigsRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListNacosHistoryConfigsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListSSLCertRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListSSLCertRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListServiceSourceRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListServiceSourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ListZnodeChildrenRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ListZnodeChildrenRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ModifyGovernanceKubernetesClusterRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ModifyGovernanceKubernetesClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/PullServicesRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/PullServicesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/QueryBusinessLocationsRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/QueryBusinessLocationsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/QueryClusterDetailRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/QueryClusterDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/QueryClusterDiskSpecificationRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/QueryClusterDiskSpecificationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/QueryClusterSpecificationRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/UpdateGatewayNameRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,23 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkmse.endpoint import endpoint_data
 
-class QueryClusterSpecificationRequest(RpcRequest):
+class UpdateGatewayNameRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'mse', '2019-05-31', 'QueryClusterSpecification')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'mse', '2019-05-31', 'UpdateGatewayName')
+		self.set_method('GET')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_GatewayUniqueId(self): # String
+		return self.get_query_params().get('GatewayUniqueId')
+
+	def set_GatewayUniqueId(self, GatewayUniqueId):  # String
+		self.add_query_param('GatewayUniqueId', GatewayUniqueId)
+	def get_Name(self): # String
+		return self.get_query_params().get('Name')
+
+	def set_Name(self, Name):  # String
+		self.add_query_param('Name', Name)
 	def get_AcceptLanguage(self): # String
 		return self.get_query_params().get('AcceptLanguage')
 
 	def set_AcceptLanguage(self, AcceptLanguage):  # String
 		self.add_query_param('AcceptLanguage', AcceptLanguage)
```

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/QueryConfigRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/QueryConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/QueryGatewayRegionRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/QueryGatewayRegionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/QueryGatewayTypeRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/QueryGatewayTypeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/QueryGovernanceKubernetesClusterRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/QueryGovernanceKubernetesClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/QueryMonitorRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/QueryMonitorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/QuerySlbSpecRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/QueryClusterSpecificationRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,23 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkmse.endpoint import endpoint_data
 
-class QuerySlbSpecRequest(RpcRequest):
+class QueryClusterSpecificationRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'mse', '2019-05-31', 'QuerySlbSpec')
-		self.set_method('GET')
+		RpcRequest.__init__(self, 'mse', '2019-05-31', 'QueryClusterSpecification')
+		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_ConnectType(self): # String
+		return self.get_query_params().get('ConnectType')
+
+	def set_ConnectType(self, ConnectType):  # String
+		self.add_query_param('ConnectType', ConnectType)
 	def get_AcceptLanguage(self): # String
 		return self.get_query_params().get('AcceptLanguage')
 
 	def set_AcceptLanguage(self, AcceptLanguage):  # String
 		self.add_query_param('AcceptLanguage', AcceptLanguage)
```

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/QueryZnodeDetailRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/QueryZnodeDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/RestartClusterRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/RestartClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/RetryClusterRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/RetryClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/ScalingClusterRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/ScalingClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/SelectGatewaySlbRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/SelectGatewaySlbRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/UpdateAclRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/UpdateAclRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/UpdateBlackWhiteListRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/UpdateBlackWhiteListRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,19 @@
 	def set_Type(self, Type):  # String
 		self.add_query_param('Type', Type)
 	def get_Content(self): # String
 		return self.get_query_params().get('Content')
 
 	def set_Content(self, Content):  # String
 		self.add_query_param('Content', Content)
+	def get_IsWhite(self): # Boolean
+		return self.get_query_params().get('IsWhite')
+
+	def set_IsWhite(self, IsWhite):  # Boolean
+		self.add_query_param('IsWhite', IsWhite)
 	def get_Id(self): # Long
 		return self.get_query_params().get('Id')
 
 	def set_Id(self, Id):  # Long
 		self.add_query_param('Id', Id)
 	def get_ResourceType(self): # String
 		return self.get_query_params().get('ResourceType')
```

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/UpdateClusterRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/UpdateClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/UpdateConfigRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/UpdateConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/UpdateEngineNamespaceRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/UpdateEngineNamespaceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/UpdateGatewayDomainRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/UpdateGatewayDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/UpdateGatewayNameRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/UpdateGatewayOptionRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,34 +15,40 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkmse.endpoint import endpoint_data
+import json
 
-class UpdateGatewayNameRequest(RpcRequest):
+class UpdateGatewayOptionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'mse', '2019-05-31', 'UpdateGatewayName')
-		self.set_method('GET')
+		RpcRequest.__init__(self, 'mse', '2019-05-31', 'UpdateGatewayOption')
+		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_GatewayUniqueId(self): # String
 		return self.get_query_params().get('GatewayUniqueId')
 
 	def set_GatewayUniqueId(self, GatewayUniqueId):  # String
 		self.add_query_param('GatewayUniqueId', GatewayUniqueId)
-	def get_Name(self): # String
-		return self.get_query_params().get('Name')
+	def get_GatewayOption(self): # Struct
+		return self.get_query_params().get('GatewayOption')
 
-	def set_Name(self, Name):  # String
-		self.add_query_param('Name', Name)
+	def set_GatewayOption(self, GatewayOption):  # Struct
+		self.add_query_param("GatewayOption", json.dumps(GatewayOption))
+	def get_GatewayId(self): # Long
+		return self.get_query_params().get('GatewayId')
+
+	def set_GatewayId(self, GatewayId):  # Long
+		self.add_query_param('GatewayId', GatewayId)
 	def get_AcceptLanguage(self): # String
 		return self.get_query_params().get('AcceptLanguage')
 
 	def set_AcceptLanguage(self, AcceptLanguage):  # String
 		self.add_query_param('AcceptLanguage', AcceptLanguage)
```

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/UpdateGatewayOptionRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/UpgradeClusterRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,40 +15,39 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkmse.endpoint import endpoint_data
-import json
 
-class UpdateGatewayOptionRequest(RpcRequest):
+class UpgradeClusterRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'mse', '2019-05-31', 'UpdateGatewayOption')
+		RpcRequest.__init__(self, 'mse', '2019-05-31', 'UpgradeCluster')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_GatewayUniqueId(self): # String
-		return self.get_query_params().get('GatewayUniqueId')
+	def get_UpgradeVersion(self): # String
+		return self.get_query_params().get('UpgradeVersion')
 
-	def set_GatewayUniqueId(self, GatewayUniqueId):  # String
-		self.add_query_param('GatewayUniqueId', GatewayUniqueId)
-	def get_GatewayOption(self): # Struct
-		return self.get_query_params().get('GatewayOption')
+	def set_UpgradeVersion(self, UpgradeVersion):  # String
+		self.add_query_param('UpgradeVersion', UpgradeVersion)
+	def get_InstanceId(self): # String
+		return self.get_query_params().get('InstanceId')
 
-	def set_GatewayOption(self, GatewayOption):  # Struct
-		self.add_query_param("GatewayOption", json.dumps(GatewayOption))
-	def get_GatewayId(self): # Long
-		return self.get_query_params().get('GatewayId')
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_RequestPars(self): # String
+		return self.get_query_params().get('RequestPars')
 
-	def set_GatewayId(self, GatewayId):  # Long
-		self.add_query_param('GatewayId', GatewayId)
+	def set_RequestPars(self, RequestPars):  # String
+		self.add_query_param('RequestPars', RequestPars)
 	def get_AcceptLanguage(self): # String
 		return self.get_query_params().get('AcceptLanguage')
 
 	def set_AcceptLanguage(self, AcceptLanguage):  # String
 		self.add_query_param('AcceptLanguage', AcceptLanguage)
```

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/UpdateGatewayRouteHTTPRewriteRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/UpdateGatewayRouteHTTPRewriteRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/UpdateGatewayServiceVersionRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/UpdateGatewayServiceVersionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/UpdateImageRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/UpdateImageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/UpdateNacosClusterRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/UpdateNacosClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/UpdateNacosConfigRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/UpdateNacosConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/UpdateNacosInstanceRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/UpdateNacosInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/UpdateNacosServiceRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/UpdateNacosServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/UpdateSSLCertRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/UpdateSSLCertRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/aliyunsdkmse/request/v20190531/UpdateZnodeRequest.py` & `aliyun-python-sdk-mse-3.0.7/aliyunsdkmse/request/v20190531/UpdateZnodeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-mse-3.0.6/setup.py` & `aliyun-python-sdk-mse-3.0.7/setup.py`

 * *Files identical despite different names*

