# Comparing `tmp/aliyun-python-sdk-cbn-1.0.8.tar.gz` & `tmp/aliyun-python-sdk-cbn-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-cbn-1.0.8.tar", last modified: Thu Apr 22 05:36:12 2021, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-cbn-1.0.9.tar", last modified: Wed Aug 11 03:10:53 2021, max compression
```

## Comparing `aliyun-python-sdk-cbn-1.0.8.tar` & `aliyun-python-sdk-cbn-1.0.9.tar`

### file list

```diff
@@ -1,73 +1,103 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-22 05:36:12.000000 aliyun-python-sdk-cbn-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      575 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1537 2021-04-22 05:36:12.000000 aliyun-python-sdk-cbn-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      527 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-22 05:36:12.000000 aliyun-python-sdk-cbn-1.0.8/aliyun_python_sdk_cbn.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1537 2021-04-22 05:36:12.000000 aliyun-python-sdk-cbn-1.0.8/aliyun_python_sdk_cbn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3924 2021-04-22 05:36:12.000000 aliyun-python-sdk-cbn-1.0.8/aliyun_python_sdk_cbn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-22 05:36:12.000000 aliyun-python-sdk-cbn-1.0.8/aliyun_python_sdk_cbn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2021-04-22 05:36:12.000000 aliyun-python-sdk-cbn-1.0.8/aliyun_python_sdk_cbn.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2021-04-22 05:36:12.000000 aliyun-python-sdk-cbn-1.0.8/aliyun_python_sdk_cbn.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-22 05:36:12.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/
--rw-r--r--   0 root         (0) root         (0)       21 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1087 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-22 05:36:12.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/
--rw-r--r--   0 root         (0) root         (0)        0 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-22 05:36:12.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/
--rw-r--r--   0 root         (0) root         (0)     2522 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/ActiveFlowLogRequest.py
--rw-r--r--   0 root         (0) root         (0)     2446 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/AssociateCenBandwidthPackageRequest.py
--rw-r--r--   0 root         (0) root         (0)     3082 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/AttachCenChildInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     4304 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/CreateCenBandwidthPackageRequest.py
--rw-r--r--   0 root         (0) root         (0)     3522 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/CreateCenChildInstanceRouteEntryToCenRequest.py
--rw-r--r--   0 root         (0) root         (0)     2722 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/CreateCenRequest.py
--rw-r--r--   0 root         (0) root         (0)     9526 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/CreateCenRouteMapRequest.py
--rw-r--r--   0 root         (0) root         (0)     3074 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/CreateFlowlogRequest.py
--rw-r--r--   0 root         (0) root         (0)     2526 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DeactiveFlowLogRequest.py
--rw-r--r--   0 root         (0) root         (0)     2298 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DeleteCenBandwidthPackageRequest.py
--rw-r--r--   0 root         (0) root         (0)     3522 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DeleteCenChildInstanceRouteEntryToCenRequest.py
--rw-r--r--   0 root         (0) root         (0)     2170 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DeleteCenRequest.py
--rw-r--r--   0 root         (0) root         (0)     2536 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DeleteCenRouteMapRequest.py
--rw-r--r--   0 root         (0) root         (0)     2522 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DeleteFlowlogRequest.py
--rw-r--r--   0 root         (0) root         (0)     2880 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DeleteRouteServiceInCenRequest.py
--rw-r--r--   0 root         (0) root         (0)     2888 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribeCenAttachedChildInstanceAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     3002 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribeCenAttachedChildInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3379 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribeCenBandwidthPackagesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3358 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribeCenChildInstanceRouteEntriesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3022 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribeCenGeographicSpanRemainingBandwidthRequest.py
--rw-r--r--   0 root         (0) root         (0)     2602 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribeCenGeographicSpansRequest.py
--rw-r--r--   0 root         (0) root         (0)     2558 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribeCenInterRegionBandwidthLimitsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2582 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribeCenPrivateZoneRoutesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2880 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribeCenRegionDomainRouteEntriesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3088 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribeCenRouteMapsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3170 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribeCenVbrHealthCheckRequest.py
--rw-r--r--   0 root         (0) root         (0)     3349 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribeCensRequest.py
--rw-r--r--   0 root         (0) root         (0)     2244 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribeChildInstanceRegionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3726 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribeFlowlogsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2630 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribeGeographicRegionMembershipRequest.py
--rw-r--r--   0 root         (0) root         (0)     2376 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribeGrantRulesToCenRequest.py
--rw-r--r--   0 root         (0) root         (0)     3352 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribePublishedRouteEntriesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3532 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribeRouteConflictRequest.py
--rw-r--r--   0 root         (0) root         (0)     3218 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribeRouteServicesInCenRequest.py
--rw-r--r--   0 root         (0) root         (0)     3254 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DetachCenChildInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2836 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DisableCenVbrHealthCheckRequest.py
--rw-r--r--   0 root         (0) root         (0)     3720 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/EnableCenVbrHealthCheckRequest.py
--rw-r--r--   0 root         (0) root         (0)     3242 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/ListTagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2704 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/ModifyCenAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2630 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/ModifyCenBandwidthPackageAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2472 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/ModifyCenBandwidthPackageSpecRequest.py
--rw-r--r--   0 root         (0) root         (0)     9484 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/ModifyCenRouteMapRequest.py
--rw-r--r--   0 root         (0) root         (0)     2896 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/ModifyFlowLogAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     3000 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/PublishRouteEntriesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3378 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/ResolveAndRouteServiceInCenRequest.py
--rw-r--r--   0 root         (0) root         (0)     2750 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/RoutePrivateZoneInCenToVpcRequest.py
--rw-r--r--   0 root         (0) root         (0)     2808 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/SetCenInterRegionBandwidthLimitRequest.py
--rw-r--r--   0 root         (0) root         (0)     2908 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/TagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2636 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/TempUpgradeCenBandwidthPackageSpecRequest.py
--rw-r--r--   0 root         (0) root         (0)     2450 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/UnassociateCenBandwidthPackageRequest.py
--rw-r--r--   0 root         (0) root         (0)     2404 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/UnroutePrivateZoneInCenToVpcRequest.py
--rw-r--r--   0 root         (0) root         (0)     2900 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/UntagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3020 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/WithdrawPublishedRouteEntriesRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-04-22 05:36:12.000000 aliyun-python-sdk-cbn-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2452 2021-04-22 05:36:11.000000 aliyun-python-sdk-cbn-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      575 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1537 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      527 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyun_python_sdk_cbn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1537 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyun_python_sdk_cbn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6169 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyun_python_sdk_cbn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyun_python_sdk_cbn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyun_python_sdk_cbn.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyun_python_sdk_cbn.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/
+-rw-r--r--   0 root         (0) root         (0)       21 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/
+-rw-r--r--   0 root         (0) root         (0)     2522 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/ActiveFlowLogRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2446 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/AssociateCenBandwidthPackageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2952 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/AssociateTransitRouterAttachmentWithRouteTableRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3082 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/AttachCenChildInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4304 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/CreateCenBandwidthPackageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3522 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/CreateCenChildInstanceRouteEntryToCenRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2722 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/CreateCenRequest.py
+-rw-r--r--   0 root         (0) root         (0)     9526 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/CreateCenRouteMapRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3074 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/CreateFlowlogRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4478 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/CreateTransitRouterPeerAttachmentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2986 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/CreateTransitRouterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4236 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/CreateTransitRouterRouteEntryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3186 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/CreateTransitRouterRouteTableRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3898 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/CreateTransitRouterVbrAttachmentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4340 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/CreateTransitRouterVpcAttachmentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2526 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DeactiveFlowLogRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2298 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DeleteCenBandwidthPackageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3522 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DeleteCenChildInstanceRouteEntryToCenRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2170 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DeleteCenRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2536 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DeleteCenRouteMapRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2522 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DeleteFlowlogRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2880 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DeleteRouteServiceInCenRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2664 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DeleteTransitRouterPeerAttachmentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3908 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DeleteTransitRouterRouteEntryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2656 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DeleteTransitRouterRouteTableRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2662 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DeleteTransitRouterVbrAttachmentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2662 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DeleteTransitRouterVpcAttachmentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2888 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribeCenAttachedChildInstanceAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3002 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribeCenAttachedChildInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3379 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribeCenBandwidthPackagesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3358 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribeCenChildInstanceRouteEntriesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3022 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribeCenGeographicSpanRemainingBandwidthRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2602 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribeCenGeographicSpansRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2558 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribeCenInterRegionBandwidthLimitsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2582 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribeCenPrivateZoneRoutesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2880 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribeCenRegionDomainRouteEntriesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3088 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribeCenRouteMapsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3170 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribeCenVbrHealthCheckRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3349 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribeCensRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2244 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribeChildInstanceRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3726 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribeFlowlogsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2630 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribeGeographicRegionMembershipRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2376 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribeGrantRulesToCenRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3352 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribePublishedRouteEntriesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3532 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribeRouteConflictRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3218 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribeRouteServicesInCenRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3254 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DetachCenChildInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2836 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DisableCenVbrHealthCheckRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2942 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DisableTransitRouterRouteTablePropagationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2954 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DissociateTransitRouterAttachmentFromRouteTableRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3720 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/EnableCenVbrHealthCheckRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2940 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/EnableTransitRouterRouteTablePropagationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/ListTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2078 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/ListTransitRouterAvailableResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3018 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/ListTransitRouterPeerAttachmentsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4176 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/ListTransitRouterRouteEntriesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2950 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/ListTransitRouterRouteTableAssociationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2950 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/ListTransitRouterRouteTablePropagationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4018 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/ListTransitRouterRouteTablesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3016 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/ListTransitRouterVbrAttachmentsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3016 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/ListTransitRouterVpcAttachmentsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2722 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/ListTransitRoutersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2704 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/ModifyCenAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2630 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/ModifyCenBandwidthPackageAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2472 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/ModifyCenBandwidthPackageSpecRequest.py
+-rw-r--r--   0 root         (0) root         (0)     9484 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/ModifyCenRouteMapRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2896 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/ModifyFlowLogAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3000 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/PublishRouteEntriesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3378 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/ResolveAndRouteServiceInCenRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2750 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/RoutePrivateZoneInCenToVpcRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2808 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/SetCenInterRegionBandwidthLimitRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2908 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/TagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2636 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/TempUpgradeCenBandwidthPackageSpecRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2450 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/UnassociateCenBandwidthPackageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2404 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/UnroutePrivateZoneInCenToVpcRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2900 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/UntagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3926 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/UpdateTransitRouterPeerAttachmentAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3046 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/UpdateTransitRouterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3246 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/UpdateTransitRouterRouteEntryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3246 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/UpdateTransitRouterRouteTableRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3270 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/UpdateTransitRouterVbrAttachmentAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3270 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/UpdateTransitRouterVpcAttachmentAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3020 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/WithdrawPublishedRouteEntriesRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2452 2021-08-11 03:10:53.000000 aliyun-python-sdk-cbn-1.0.9/setup.py
```

### Comparing `aliyun-python-sdk-cbn-1.0.8/LICENSE` & `aliyun-python-sdk-cbn-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/PKG-INFO` & `aliyun-python-sdk-cbn-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-cbn
-Version: 1.0.8
+Version: 1.0.9
 Summary: The cbn module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-cbn
```

### Comparing `aliyun-python-sdk-cbn-1.0.8/README.rst` & `aliyun-python-sdk-cbn-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyun_python_sdk_cbn.egg-info/PKG-INFO` & `aliyun-python-sdk-cbn-1.0.9/aliyun_python_sdk_cbn.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-cbn
-Version: 1.0.8
+Version: 1.0.9
 Summary: The cbn module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-cbn
```

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/endpoint.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/ActiveFlowLogRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/ActiveFlowLogRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/AssociateCenBandwidthPackageRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/AssociateCenBandwidthPackageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/AttachCenChildInstanceRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/AttachCenChildInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/CreateCenBandwidthPackageRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/CreateCenBandwidthPackageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/CreateCenChildInstanceRouteEntryToCenRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/CreateCenChildInstanceRouteEntryToCenRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/CreateCenRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/CreateCenRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/CreateCenRouteMapRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/CreateCenRouteMapRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/CreateFlowlogRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/CreateFlowlogRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DeactiveFlowLogRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DeactiveFlowLogRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DeleteCenBandwidthPackageRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DeleteCenBandwidthPackageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DeleteCenChildInstanceRouteEntryToCenRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DeleteCenChildInstanceRouteEntryToCenRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DeleteCenRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DeleteCenRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DeleteCenRouteMapRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DeleteCenRouteMapRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DeleteFlowlogRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DeleteFlowlogRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DeleteRouteServiceInCenRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DeleteRouteServiceInCenRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribeCenAttachedChildInstanceAttributeRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribeCenAttachedChildInstanceAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribeCenAttachedChildInstancesRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribeCenAttachedChildInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribeCenBandwidthPackagesRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribeCenBandwidthPackagesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribeCenChildInstanceRouteEntriesRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribeCenChildInstanceRouteEntriesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribeCenGeographicSpanRemainingBandwidthRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribeCenGeographicSpanRemainingBandwidthRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribeCenGeographicSpansRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribeCenGeographicSpansRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribeCenInterRegionBandwidthLimitsRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribeCenInterRegionBandwidthLimitsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribeCenPrivateZoneRoutesRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribeCenPrivateZoneRoutesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribeCenRegionDomainRouteEntriesRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribeCenRegionDomainRouteEntriesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribeCenRouteMapsRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribeCenRouteMapsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribeCenVbrHealthCheckRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribeCenVbrHealthCheckRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribeCensRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribeCensRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribeChildInstanceRegionsRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribeChildInstanceRegionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribeFlowlogsRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribeFlowlogsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribeGeographicRegionMembershipRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribeGeographicRegionMembershipRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribeGrantRulesToCenRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribeGrantRulesToCenRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribePublishedRouteEntriesRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribePublishedRouteEntriesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribeRouteConflictRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribeRouteConflictRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DescribeRouteServicesInCenRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DescribeRouteServicesInCenRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DetachCenChildInstanceRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DetachCenChildInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/DisableCenVbrHealthCheckRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/DisableCenVbrHealthCheckRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/EnableCenVbrHealthCheckRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/EnableCenVbrHealthCheckRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/ListTagResourcesRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/ListTagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/ModifyCenAttributeRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/ModifyCenAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/ModifyCenBandwidthPackageAttributeRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/ModifyCenBandwidthPackageAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/ModifyCenBandwidthPackageSpecRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/ModifyCenBandwidthPackageSpecRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/ModifyCenRouteMapRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/ModifyCenRouteMapRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/ModifyFlowLogAttributeRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/ModifyFlowLogAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/PublishRouteEntriesRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/PublishRouteEntriesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/ResolveAndRouteServiceInCenRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/ResolveAndRouteServiceInCenRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/RoutePrivateZoneInCenToVpcRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/RoutePrivateZoneInCenToVpcRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/SetCenInterRegionBandwidthLimitRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/SetCenInterRegionBandwidthLimitRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/TagResourcesRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/TagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/TempUpgradeCenBandwidthPackageSpecRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/TempUpgradeCenBandwidthPackageSpecRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/UnassociateCenBandwidthPackageRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/UnassociateCenBandwidthPackageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/UnroutePrivateZoneInCenToVpcRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/UnroutePrivateZoneInCenToVpcRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/UntagResourcesRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/UntagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/aliyunsdkcbn/request/v20170912/WithdrawPublishedRouteEntriesRequest.py` & `aliyun-python-sdk-cbn-1.0.9/aliyunsdkcbn/request/v20170912/WithdrawPublishedRouteEntriesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cbn-1.0.8/setup.py` & `aliyun-python-sdk-cbn-1.0.9/setup.py`

 * *Files identical despite different names*

