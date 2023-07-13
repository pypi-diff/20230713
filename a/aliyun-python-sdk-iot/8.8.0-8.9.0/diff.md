# Comparing `tmp/aliyun-python-sdk-iot-8.8.0.tar.gz` & `tmp/aliyun-python-sdk-iot-8.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-iot-8.8.0.tar", last modified: Fri May 15 10:00:44 2020, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-iot-8.9.0.tar", last modified: Fri Jun 12 05:47:24 2020, max compression
```

## Comparing `aliyun-python-sdk-iot-8.8.0.tar` & `aliyun-python-sdk-iot-8.9.0.tar`

### file list

```diff
@@ -1,194 +1,220 @@
-drwxrwxr-x   0 admin     (1017) admin     (1017)        0 2020-05-15 10:00:44.000000 aliyun-python-sdk-iot-8.8.0/
--rw-rw-r--   0 admin     (1017) admin     (1017)        0 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/MANIFEST.in
-drwxrwxr-x   0 admin     (1017) admin     (1017)        0 2020-05-15 10:00:44.000000 aliyun-python-sdk-iot-8.8.0/aliyun_python_sdk_iot.egg-info/
--rw-rw-r--   0 admin     (1017) admin     (1017)        1 2020-05-15 10:00:44.000000 aliyun-python-sdk-iot-8.8.0/aliyun_python_sdk_iot.egg-info/dependency_links.txt
--rw-rw-r--   0 admin     (1017) admin     (1017)       13 2020-05-15 10:00:44.000000 aliyun-python-sdk-iot-8.8.0/aliyun_python_sdk_iot.egg-info/top_level.txt
--rw-rw-r--   0 admin     (1017) admin     (1017)       31 2020-05-15 10:00:44.000000 aliyun-python-sdk-iot-8.8.0/aliyun_python_sdk_iot.egg-info/requires.txt
--rw-rw-r--   0 admin     (1017) admin     (1017)    11206 2020-05-15 10:00:44.000000 aliyun-python-sdk-iot-8.8.0/aliyun_python_sdk_iot.egg-info/SOURCES.txt
--rw-rw-r--   0 admin     (1017) admin     (1017)     1537 2020-05-15 10:00:44.000000 aliyun-python-sdk-iot-8.8.0/aliyun_python_sdk_iot.egg-info/PKG-INFO
-drwxrwxr-x   0 admin     (1017) admin     (1017)        0 2020-05-15 10:00:44.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/
--rw-rw-r--   0 admin     (1017) admin     (1017)       21 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/__init__.py
-drwxrwxr-x   0 admin     (1017) admin     (1017)        0 2020-05-15 10:00:44.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/
--rw-rw-r--   0 admin     (1017) admin     (1017)        0 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/__init__.py
-drwxrwxr-x   0 admin     (1017) admin     (1017)        0 2020-05-15 10:00:44.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/
--rw-rw-r--   0 admin     (1017) admin     (1017)     1784 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/SetDeviceGroupTagsRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1614 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CancelOTAStrategyByJobRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2131 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateLoRaNodesTaskRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1933 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchCheckDeviceNamesRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1872 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateEdgeInstanceRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1824 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/DeleteEdgeDriverVersionRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2726 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/InvokeDataAPIServiceRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1780 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchRegisterDeviceRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2116 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/UpdateProductTopicRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2084 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/SaveDevicePropRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1948 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDeviceDetailRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1944 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/RemoveThingTopoRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2044 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/ReplaceEdgeInstanceGatewayRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2290 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/RRpcRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2176 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/NotifyAddThingTopoRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2344 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryEdgeDriverVersionRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2166 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/GetThingModelTslRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2130 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateProductTagsRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1925 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchUnbindDeviceFromEdgeInstanceRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2258 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/InvokeThingServiceRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1934 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/ResetThingRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1949 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/DeleteProductTagsRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2302 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateEdgeDriverRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2108 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchAddDeviceGroupRelationsRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1640 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryProductCertInfoRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2180 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchGetDeviceStateRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1666 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/ListThingTemplatesRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2257 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDeviceDesiredPropertyRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1923 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchGetEdgeInstanceDeviceDriverRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1820 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDeviceGroupByDeviceRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2226 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryProductListRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1936 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/EnableThingRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1856 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/UnbindApplicationFromEdgeInstanceRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1976 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDeviceListByDeviceGroupRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1630 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/GetEdgeInstanceRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1624 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QuerySuperDeviceGroupRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1476 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryLoRaJoinPermissionsRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2092 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDeviceFileRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1808 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/SetProductCertInfoRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2136 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BindGatewayToEdgeInstanceRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1622 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/GetDataAPIServiceDetailRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1468 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/GenerateOTAUploadURLRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2237 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/InvokeThingsServiceRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2865 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDevicePropertiesDataRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2952 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateEdgeDriverVersionRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1978 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/ListOTAJobByFirmwareRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1944 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/GetDeviceStatusRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2069 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/SetDevicesPropertyRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1978 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateDeviceGroupRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2105 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchGetEdgeInstanceChannelRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1944 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDevicePropRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2068 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BindApplicationToEdgeInstanceRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     3070 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryAppDeviceListRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2290 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDeviceFileListRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)        0 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/__init__.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1956 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/GetGatewayBySubDeviceRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1936 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryEdgeInstanceRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2893 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateOTADynamicUpgradeJobRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2104 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryEdgeDriverRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1626 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/DeleteProductRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1747 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchGetEdgeDriverRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2112 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/ListOTATaskByJobRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1592 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryOTAJobRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2246 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/GetThingTopoRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2906 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateRuleRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1964 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDevicePropertyStatusRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1935 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchQueryDeviceDetailRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2740 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDeviceServiceDataRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2328 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateEdgeOssPreSignedAddressRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1612 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/GetNodesAddingTaskRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1844 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/ListThingModelVersionRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     3378 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateOTAFirmwareRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2198 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/PublishThingModelRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1648 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryEdgeInstanceGatewayRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2742 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDevicePropertyDataRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2504 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDeviceByStatusRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2156 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDeviceGroupListRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2134 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateProductTopicRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2090 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/SetDevicePropertyRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1905 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateTopicRouteTableRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2122 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/PubRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2451 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchUpdateDeviceNicknameRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1826 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/ReleaseEdgeDriverVersionRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2296 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/ListProductByTagsRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1828 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateThingModelRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1998 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/UpdateDeviceShadowRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2152 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BindDriverToEdgeInstanceRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2262 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/RegisterDeviceRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2247 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CancelOTATaskByDeviceRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2146 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/ListOTAFirmwareRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1624 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryTopicReverseRouteTableRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1630 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/ListProductTagsRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2492 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CancelOTATaskByJobRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1984 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/ListRuleRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2010 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/PubBroadcastRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1960 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDeviceRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1608 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/GetLoraNodesTaskRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1654 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CloseEdgeInstanceDeploymentRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1634 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryProductTopicRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1622 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDeviceGroupInfoRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2130 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/UpdateProductTagsRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1938 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/DisableThingRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1814 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchRegisterDeviceWithApplyIdRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1606 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/ListRuleActionsRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1616 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/DeleteDeviceGroupRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1818 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/GetEdgeDriverVersionRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     3794 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateOTAStaticUpgradeJobRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1596 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/DeleteRuleRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2952 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/UpdateEdgeDriverVersionRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1618 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/DeleteProductTopicRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1634 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/DeleteOTAFirmwareRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1923 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchGetEdgeInstanceDeviceConfigRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1984 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryEdgeInstanceDriverRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1820 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/ClearEdgeInstanceDriverConfigsRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1614 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/GetRuleActionRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2136 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/ImportThingModelTslRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1610 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryTopicRouteTableRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1620 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/DeleteEdgeDriverRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1802 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDeviceCertRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2085 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchGetEdgeInstanceDeviceChannelRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1792 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateEdgeInstanceDeploymentRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1642 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDeviceStatisticsRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2126 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/UpdateProductFilterConfigRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2251 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchSetEdgeInstanceDeviceChannelRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1592 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/StopRuleRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2111 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchDeleteEdgeInstanceChannelRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2229 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDeviceGroupByTagsRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     3028 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchAddThingTopoRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2902 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDeviceEventDataRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2294 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CopyThingModelRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1632 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryOTAFirmwareRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2324 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryEdgeInstanceChannelRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2100 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/DeleteDevicePropRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2264 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/SetDeviceDesiredPropertyRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2114 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchDeleteDeviceGroupRelationsRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1814 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryBatchRegisterDeviceStatusRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2318 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/ListOTAJobByDeviceRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1938 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/DeleteDeviceRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     3934 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateProductRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2000 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/UpdateThingModelRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1834 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/GetEdgeInstanceDeploymentRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1905 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/DeleteTopicRouteTableRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2187 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchSetEdgeInstanceDeviceConfigRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2692 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/UpdateRuleRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2094 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/DeleteDeviceFileRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2016 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryThingModelRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2590 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateEdgeInstanceChannelRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1984 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryEdgeInstanceDeviceRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2355 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateOTAVerifyJobRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2867 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/DeleteThingModelRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1927 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchClearEdgeInstanceDeviceConfigRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1636 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/DeleteEdgeInstanceRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1620 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/DeleteRuleActionRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1802 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/GetDeviceShadowRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1782 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/UpdateDeviceGroupRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2328 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryEdgeInstanceHistoricDeploymentRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2219 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDeviceByTagsRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2418 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/SetEdgeInstanceDriverConfigsRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     4300 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateDataAPIServiceRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1816 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/UnbindDriverFromEdgeInstanceRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1840 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/GetThingTemplateRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2097 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchBindDeviceToEdgeInstanceWithDriverRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2756 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/UpdateEdgeInstanceChannelRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2326 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryEdgeInstanceDeviceByDriverRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2210 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/UpdateEdgeInstanceRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1624 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryProductRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1949 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchGetEdgeInstanceDriverConfigsRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1590 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/GetRuleRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1946 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/UpdateRuleActionRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1982 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/UpdateProductRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1735 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchGetDeviceBindStatusRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1628 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDeviceGroupTagListRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1624 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryCertUrlByApplyIdRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1956 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryPageByApplyIdRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1594 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/StartRuleRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2136 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateRuleActionRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     3289 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/endpoint.py
--rw-rw-r--   0 admin     (1017) admin     (1017)       38 2020-05-15 10:00:44.000000 aliyun-python-sdk-iot-8.8.0/setup.cfg
--rw-rw-r--   0 admin     (1017) admin     (1017)      527 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/README.rst
--rw-rw-r--   0 admin     (1017) admin     (1017)     1537 2020-05-15 10:00:44.000000 aliyun-python-sdk-iot-8.8.0/PKG-INFO
--rw-rw-r--   0 admin     (1017) admin     (1017)     2452 2020-05-15 10:00:43.000000 aliyun-python-sdk-iot-8.8.0/setup.py
+drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-06-12 05:47:24.000000 aliyun-python-sdk-iot-8.9.0/
+-rw-rw-r--   0 admin      (531) admin      (531)       38 2020-06-12 05:47:24.000000 aliyun-python-sdk-iot-8.9.0/setup.cfg
+drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-06-12 05:47:24.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/
+-rw-rw-r--   0 admin      (531) admin      (531)       21 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/__init__.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3289 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/endpoint.py
+drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-06-12 05:47:24.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/
+-rw-rw-r--   0 admin      (531) admin      (531)        0 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/__init__.py
+drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-06-12 05:47:24.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/
+-rw-rw-r--   0 admin      (531) admin      (531)     1594 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/StartRuleRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1933 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchCheckDeviceNamesRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2246 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/GetThingTopoRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1872 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateEdgeInstanceRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1780 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/TriggerSceneRuleRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)        0 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/__init__.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2257 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDeviceDesiredPropertyRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2069 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/SetDevicesPropertyRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1624 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QuerySuperDeviceGroupRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2085 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchGetEdgeInstanceDeviceChannelRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3070 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryAppDeviceListRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1735 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchGetDeviceBindStatusRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2097 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchBindDeviceToEdgeInstanceWithDriverRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1636 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DeleteEdgeInstanceRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1816 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/UnbindDriverFromEdgeInstanceRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2100 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DeleteDevicePropRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1935 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchQueryDeviceDetailRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1949 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchGetEdgeInstanceDriverConfigsRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1828 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateThingModelRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1624 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryTopicReverseRouteTableRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1982 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/UpdateProductRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2146 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/ListOTAFirmwareRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2434 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDetailSceneRuleLogRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2742 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDevicePropertyDataRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1934 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/ResetThingRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2000 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/UpdateThingModelRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1616 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DeleteDeviceGroupRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1976 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDeviceListByDeviceGroupRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1905 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DeleteTopicRouteTableRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1630 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryConsumerGroupStatusRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1874 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateConsumerGroupSubscribeRelationRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1624 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryProductRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1628 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDeviceGroupTagListRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1923 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchGetEdgeInstanceDeviceDriverRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1834 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/GetEdgeInstanceDeploymentRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1610 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryTopicRouteTableRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1782 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DeleteSubscribeRelationRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1808 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/SetProductCertInfoRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2156 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDeviceGroupListRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1938 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DeleteDeviceRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1824 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DeleteEdgeDriverVersionRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1592 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryOTAJobRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1964 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDevicePropertyStatusRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2126 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/UpdateProductFilterConfigRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3794 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateOTAStaticUpgradeJobRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1782 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/UpdateDeviceGroupRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2084 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/SaveDevicePropRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2740 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDeviceServiceDataRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1948 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDeviceDetailRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2906 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateRuleRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1592 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/StopRuleRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1634 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DeleteOTAFirmwareRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2130 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateProductTagsRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1614 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CancelOTAStrategyByJobRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1925 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchUnbindDeviceFromEdgeInstanceRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1476 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryLoRaJoinPermissionsRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1784 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/SetDeviceGroupTagsRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1792 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateEdgeInstanceDeploymentRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1620 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DeleteRuleActionRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1608 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/GetLoraNodesTaskRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1978 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/ListOTAJobByFirmwareRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2326 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryEdgeInstanceDeviceByDriverRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1630 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/GetEdgeInstanceRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2294 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CopyThingModelRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2090 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/SetDevicePropertyRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2262 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/RegisterDeviceRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2136 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateRuleActionRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2166 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/GetThingModelTslRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1818 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/GetEdgeDriverVersionRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1936 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/EnableThingRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1632 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryOTAFirmwareRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2893 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateOTADynamicUpgradeJobRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1856 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/UnbindApplicationFromEdgeInstanceRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3863 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateSubscribeRelationRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2504 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDeviceByStatusRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2344 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryEdgeDriverVersionRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2418 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/SetEdgeInstanceDriverConfigsRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2187 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchSetEdgeInstanceDeviceConfigRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2229 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDeviceGroupByTagsRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2131 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateLoRaNodesTaskRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1936 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryEdgeInstanceRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1802 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BindSceneRuleToEdgeInstanceRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1949 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DeleteProductTagsRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1944 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/RemoveThingTopoRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1618 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DeleteProductTopicRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1747 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchGetEdgeDriverRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1956 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryPageByApplyIdRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2104 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryEdgeDriverRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1642 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDeviceStatisticsRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1978 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateDeviceGroupRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1946 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/UpdateRuleActionRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2865 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDevicePropertiesDataRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1648 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryEdgeInstanceGatewayRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2328 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryEdgeInstanceHistoricDeploymentRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2112 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/ListOTATaskByJobRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1606 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DeleteSceneRuleRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1612 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/GetNodesAddingTaskRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1905 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateTopicRouteTableRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1636 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryConsumerGroupByGroupIdRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3112 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateEdgeDriverVersionRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2146 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/UpdateSceneRuleRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2237 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/InvokeThingsServiceRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2226 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryProductListRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1608 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DisableSceneRuleRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1874 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DeleteConsumerGroupSubscribeRelationRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2318 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/ListOTAJobByDeviceRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1956 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/GetGatewayBySubDeviceRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1780 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QuerySubscribeRelationRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2902 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDeviceEventDataRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2726 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/InvokeDataAPIServiceRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1984 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryEdgeInstanceDriverRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2492 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CancelOTATaskByJobRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1954 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QuerySceneRuleRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2134 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateProductTopicRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2219 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDeviceByTagsRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1468 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/GenerateOTAUploadURLRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2324 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryEdgeInstanceChannelRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1998 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateSceneRuleRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2118 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryConsumerGroupListRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2092 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDeviceFileRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3934 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateProductRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1600 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/GetSceneRuleRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1590 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/GetRuleRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2044 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/ReplaceEdgeInstanceGatewayRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1944 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDevicePropRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2176 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/NotifyAddThingTopoRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3028 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchAddThingTopoRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1802 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDeviceCertRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1840 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/GetThingTemplateRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1998 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/UpdateDeviceShadowRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2264 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/SetDeviceDesiredPropertyRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1666 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/ListThingTemplatesRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2136 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BindGatewayToEdgeInstanceRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2328 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateEdgeOssPreSignedAddressRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1984 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/ListRuleRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1596 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DeleteRuleRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1990 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryEdgeInstanceSceneRuleRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2016 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryThingModelRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1814 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryBatchRegisterDeviceStatusRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1654 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CloseEdgeInstanceDeploymentRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1804 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/UpdateConsumerGroupRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2108 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchAddDeviceGroupRelationsRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2355 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateOTAVerifyJobRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1640 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryProductCertInfoRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2130 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/UpdateProductTagsRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2247 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CancelOTATaskByDeviceRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2451 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchUpdateDeviceNicknameRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1630 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/ListProductTagsRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1622 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDeviceGroupInfoRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1614 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/GetRuleActionRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2114 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchDeleteDeviceGroupRelationsRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3112 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/UpdateEdgeDriverVersionRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1938 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DisableThingRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1632 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateConsumerGroupRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2180 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchGetDeviceStateRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1814 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchRegisterDeviceWithApplyIdRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2094 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DeleteDeviceFileRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1923 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchGetEdgeInstanceDeviceConfigRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2430 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QuerySummarySceneRuleLogRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2290 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/RRpcRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2692 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/UpdateRuleRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     4300 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateDataAPIServiceRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1606 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/ListRuleActionsRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1944 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/GetDeviceStatusRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1802 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/GetDeviceShadowRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1634 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/ResetConsumerGroupPositionRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2210 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/UpdateEdgeInstanceRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1606 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/EnableSceneRuleRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1810 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/UnbindSceneRuleFromEdgeInstanceRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1634 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryProductTopicRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2068 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BindApplicationToEdgeInstanceRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2251 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchSetEdgeInstanceDeviceChannelRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2198 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/PublishThingModelRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2116 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/UpdateProductTopicRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3863 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/UpdateSubscribeRelationRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2590 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateEdgeInstanceChannelRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1626 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DeleteProductRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2152 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BindDriverToEdgeInstanceRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2111 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchDeleteEdgeInstanceChannelRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2867 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DeleteThingModelRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1844 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/ListThingModelVersionRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2122 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/PubRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1826 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/ReleaseEdgeDriverVersionRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2105 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchGetEdgeInstanceChannelRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1620 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DeleteConsumerGroupRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1620 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DeleteEdgeDriverRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2296 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/ListProductByTagsRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2258 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/InvokeThingServiceRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2756 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/UpdateEdgeInstanceChannelRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1780 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchRegisterDeviceRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2302 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateEdgeDriverRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1960 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDeviceRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1984 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryEdgeInstanceDeviceRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1927 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchClearEdgeInstanceDeviceConfigRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2290 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDeviceFileListRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2010 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/PubBroadcastRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1820 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDeviceGroupByDeviceRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1820 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/ClearEdgeInstanceDriverConfigsRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1624 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryCertUrlByApplyIdRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3378 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateOTAFirmwareRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1622 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/GetDataAPIServiceDetailRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2136 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/ImportThingModelTslRequest.py
+drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-06-12 05:47:24.000000 aliyun-python-sdk-iot-8.9.0/aliyun_python_sdk_iot.egg-info/
+-rw-rw-r--   0 admin      (531) admin      (531)        1 2020-06-12 05:47:24.000000 aliyun-python-sdk-iot-8.9.0/aliyun_python_sdk_iot.egg-info/dependency_links.txt
+-rw-rw-r--   0 admin      (531) admin      (531)       31 2020-06-12 05:47:24.000000 aliyun-python-sdk-iot-8.9.0/aliyun_python_sdk_iot.egg-info/requires.txt
+-rw-rw-r--   0 admin      (531) admin      (531)    12866 2020-06-12 05:47:24.000000 aliyun-python-sdk-iot-8.9.0/aliyun_python_sdk_iot.egg-info/SOURCES.txt
+-rw-rw-r--   0 admin      (531) admin      (531)       13 2020-06-12 05:47:24.000000 aliyun-python-sdk-iot-8.9.0/aliyun_python_sdk_iot.egg-info/top_level.txt
+-rw-rw-r--   0 admin      (531) admin      (531)     1537 2020-06-12 05:47:24.000000 aliyun-python-sdk-iot-8.9.0/aliyun_python_sdk_iot.egg-info/PKG-INFO
+-rw-rw-r--   0 admin      (531) admin      (531)     2452 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/setup.py
+-rw-rw-r--   0 admin      (531) admin      (531)        0 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/MANIFEST.in
+-rw-rw-r--   0 admin      (531) admin      (531)      527 2020-06-12 05:47:23.000000 aliyun-python-sdk-iot-8.9.0/README.rst
+-rw-rw-r--   0 admin      (531) admin      (531)     1537 2020-06-12 05:47:24.000000 aliyun-python-sdk-iot-8.9.0/PKG-INFO
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyun_python_sdk_iot.egg-info/SOURCES.txt` & `aliyun-python-sdk-iot-8.9.0/aliyun_python_sdk_iot.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,20 +30,23 @@
 aliyunsdkiot/request/v20180120/BatchSetEdgeInstanceDeviceChannelRequest.py
 aliyunsdkiot/request/v20180120/BatchSetEdgeInstanceDeviceConfigRequest.py
 aliyunsdkiot/request/v20180120/BatchUnbindDeviceFromEdgeInstanceRequest.py
 aliyunsdkiot/request/v20180120/BatchUpdateDeviceNicknameRequest.py
 aliyunsdkiot/request/v20180120/BindApplicationToEdgeInstanceRequest.py
 aliyunsdkiot/request/v20180120/BindDriverToEdgeInstanceRequest.py
 aliyunsdkiot/request/v20180120/BindGatewayToEdgeInstanceRequest.py
+aliyunsdkiot/request/v20180120/BindSceneRuleToEdgeInstanceRequest.py
 aliyunsdkiot/request/v20180120/CancelOTAStrategyByJobRequest.py
 aliyunsdkiot/request/v20180120/CancelOTATaskByDeviceRequest.py
 aliyunsdkiot/request/v20180120/CancelOTATaskByJobRequest.py
 aliyunsdkiot/request/v20180120/ClearEdgeInstanceDriverConfigsRequest.py
 aliyunsdkiot/request/v20180120/CloseEdgeInstanceDeploymentRequest.py
 aliyunsdkiot/request/v20180120/CopyThingModelRequest.py
+aliyunsdkiot/request/v20180120/CreateConsumerGroupRequest.py
+aliyunsdkiot/request/v20180120/CreateConsumerGroupSubscribeRelationRequest.py
 aliyunsdkiot/request/v20180120/CreateDataAPIServiceRequest.py
 aliyunsdkiot/request/v20180120/CreateDeviceGroupRequest.py
 aliyunsdkiot/request/v20180120/CreateEdgeDriverRequest.py
 aliyunsdkiot/request/v20180120/CreateEdgeDriverVersionRequest.py
 aliyunsdkiot/request/v20180120/CreateEdgeInstanceChannelRequest.py
 aliyunsdkiot/request/v20180120/CreateEdgeInstanceDeploymentRequest.py
 aliyunsdkiot/request/v20180120/CreateEdgeInstanceRequest.py
@@ -54,45 +57,54 @@
 aliyunsdkiot/request/v20180120/CreateOTAStaticUpgradeJobRequest.py
 aliyunsdkiot/request/v20180120/CreateOTAVerifyJobRequest.py
 aliyunsdkiot/request/v20180120/CreateProductRequest.py
 aliyunsdkiot/request/v20180120/CreateProductTagsRequest.py
 aliyunsdkiot/request/v20180120/CreateProductTopicRequest.py
 aliyunsdkiot/request/v20180120/CreateRuleActionRequest.py
 aliyunsdkiot/request/v20180120/CreateRuleRequest.py
+aliyunsdkiot/request/v20180120/CreateSceneRuleRequest.py
+aliyunsdkiot/request/v20180120/CreateSubscribeRelationRequest.py
 aliyunsdkiot/request/v20180120/CreateThingModelRequest.py
 aliyunsdkiot/request/v20180120/CreateTopicRouteTableRequest.py
+aliyunsdkiot/request/v20180120/DeleteConsumerGroupRequest.py
+aliyunsdkiot/request/v20180120/DeleteConsumerGroupSubscribeRelationRequest.py
 aliyunsdkiot/request/v20180120/DeleteDeviceFileRequest.py
 aliyunsdkiot/request/v20180120/DeleteDeviceGroupRequest.py
 aliyunsdkiot/request/v20180120/DeleteDevicePropRequest.py
 aliyunsdkiot/request/v20180120/DeleteDeviceRequest.py
 aliyunsdkiot/request/v20180120/DeleteEdgeDriverRequest.py
 aliyunsdkiot/request/v20180120/DeleteEdgeDriverVersionRequest.py
 aliyunsdkiot/request/v20180120/DeleteEdgeInstanceRequest.py
 aliyunsdkiot/request/v20180120/DeleteOTAFirmwareRequest.py
 aliyunsdkiot/request/v20180120/DeleteProductRequest.py
 aliyunsdkiot/request/v20180120/DeleteProductTagsRequest.py
 aliyunsdkiot/request/v20180120/DeleteProductTopicRequest.py
 aliyunsdkiot/request/v20180120/DeleteRuleActionRequest.py
 aliyunsdkiot/request/v20180120/DeleteRuleRequest.py
+aliyunsdkiot/request/v20180120/DeleteSceneRuleRequest.py
+aliyunsdkiot/request/v20180120/DeleteSubscribeRelationRequest.py
 aliyunsdkiot/request/v20180120/DeleteThingModelRequest.py
 aliyunsdkiot/request/v20180120/DeleteTopicRouteTableRequest.py
+aliyunsdkiot/request/v20180120/DisableSceneRuleRequest.py
 aliyunsdkiot/request/v20180120/DisableThingRequest.py
+aliyunsdkiot/request/v20180120/EnableSceneRuleRequest.py
 aliyunsdkiot/request/v20180120/EnableThingRequest.py
 aliyunsdkiot/request/v20180120/GenerateOTAUploadURLRequest.py
 aliyunsdkiot/request/v20180120/GetDataAPIServiceDetailRequest.py
 aliyunsdkiot/request/v20180120/GetDeviceShadowRequest.py
 aliyunsdkiot/request/v20180120/GetDeviceStatusRequest.py
 aliyunsdkiot/request/v20180120/GetEdgeDriverVersionRequest.py
 aliyunsdkiot/request/v20180120/GetEdgeInstanceDeploymentRequest.py
 aliyunsdkiot/request/v20180120/GetEdgeInstanceRequest.py
 aliyunsdkiot/request/v20180120/GetGatewayBySubDeviceRequest.py
 aliyunsdkiot/request/v20180120/GetLoraNodesTaskRequest.py
 aliyunsdkiot/request/v20180120/GetNodesAddingTaskRequest.py
 aliyunsdkiot/request/v20180120/GetRuleActionRequest.py
 aliyunsdkiot/request/v20180120/GetRuleRequest.py
+aliyunsdkiot/request/v20180120/GetSceneRuleRequest.py
 aliyunsdkiot/request/v20180120/GetThingModelTslRequest.py
 aliyunsdkiot/request/v20180120/GetThingTemplateRequest.py
 aliyunsdkiot/request/v20180120/GetThingTopoRequest.py
 aliyunsdkiot/request/v20180120/ImportThingModelTslRequest.py
 aliyunsdkiot/request/v20180120/InvokeDataAPIServiceRequest.py
 aliyunsdkiot/request/v20180120/InvokeThingServiceRequest.py
 aliyunsdkiot/request/v20180120/InvokeThingsServiceRequest.py
@@ -109,14 +121,18 @@
 aliyunsdkiot/request/v20180120/NotifyAddThingTopoRequest.py
 aliyunsdkiot/request/v20180120/PubBroadcastRequest.py
 aliyunsdkiot/request/v20180120/PubRequest.py
 aliyunsdkiot/request/v20180120/PublishThingModelRequest.py
 aliyunsdkiot/request/v20180120/QueryAppDeviceListRequest.py
 aliyunsdkiot/request/v20180120/QueryBatchRegisterDeviceStatusRequest.py
 aliyunsdkiot/request/v20180120/QueryCertUrlByApplyIdRequest.py
+aliyunsdkiot/request/v20180120/QueryConsumerGroupByGroupIdRequest.py
+aliyunsdkiot/request/v20180120/QueryConsumerGroupListRequest.py
+aliyunsdkiot/request/v20180120/QueryConsumerGroupStatusRequest.py
+aliyunsdkiot/request/v20180120/QueryDetailSceneRuleLogRequest.py
 aliyunsdkiot/request/v20180120/QueryDeviceByStatusRequest.py
 aliyunsdkiot/request/v20180120/QueryDeviceByTagsRequest.py
 aliyunsdkiot/request/v20180120/QueryDeviceCertRequest.py
 aliyunsdkiot/request/v20180120/QueryDeviceDesiredPropertyRequest.py
 aliyunsdkiot/request/v20180120/QueryDeviceDetailRequest.py
 aliyunsdkiot/request/v20180120/QueryDeviceEventDataRequest.py
 aliyunsdkiot/request/v20180120/QueryDeviceFileListRequest.py
@@ -139,49 +155,59 @@
 aliyunsdkiot/request/v20180120/QueryEdgeInstanceChannelRequest.py
 aliyunsdkiot/request/v20180120/QueryEdgeInstanceDeviceByDriverRequest.py
 aliyunsdkiot/request/v20180120/QueryEdgeInstanceDeviceRequest.py
 aliyunsdkiot/request/v20180120/QueryEdgeInstanceDriverRequest.py
 aliyunsdkiot/request/v20180120/QueryEdgeInstanceGatewayRequest.py
 aliyunsdkiot/request/v20180120/QueryEdgeInstanceHistoricDeploymentRequest.py
 aliyunsdkiot/request/v20180120/QueryEdgeInstanceRequest.py
+aliyunsdkiot/request/v20180120/QueryEdgeInstanceSceneRuleRequest.py
 aliyunsdkiot/request/v20180120/QueryLoRaJoinPermissionsRequest.py
 aliyunsdkiot/request/v20180120/QueryOTAFirmwareRequest.py
 aliyunsdkiot/request/v20180120/QueryOTAJobRequest.py
 aliyunsdkiot/request/v20180120/QueryPageByApplyIdRequest.py
 aliyunsdkiot/request/v20180120/QueryProductCertInfoRequest.py
 aliyunsdkiot/request/v20180120/QueryProductListRequest.py
 aliyunsdkiot/request/v20180120/QueryProductRequest.py
 aliyunsdkiot/request/v20180120/QueryProductTopicRequest.py
+aliyunsdkiot/request/v20180120/QuerySceneRuleRequest.py
+aliyunsdkiot/request/v20180120/QuerySubscribeRelationRequest.py
+aliyunsdkiot/request/v20180120/QuerySummarySceneRuleLogRequest.py
 aliyunsdkiot/request/v20180120/QuerySuperDeviceGroupRequest.py
 aliyunsdkiot/request/v20180120/QueryThingModelRequest.py
 aliyunsdkiot/request/v20180120/QueryTopicReverseRouteTableRequest.py
 aliyunsdkiot/request/v20180120/QueryTopicRouteTableRequest.py
 aliyunsdkiot/request/v20180120/RRpcRequest.py
 aliyunsdkiot/request/v20180120/RegisterDeviceRequest.py
 aliyunsdkiot/request/v20180120/ReleaseEdgeDriverVersionRequest.py
 aliyunsdkiot/request/v20180120/RemoveThingTopoRequest.py
 aliyunsdkiot/request/v20180120/ReplaceEdgeInstanceGatewayRequest.py
+aliyunsdkiot/request/v20180120/ResetConsumerGroupPositionRequest.py
 aliyunsdkiot/request/v20180120/ResetThingRequest.py
 aliyunsdkiot/request/v20180120/SaveDevicePropRequest.py
 aliyunsdkiot/request/v20180120/SetDeviceDesiredPropertyRequest.py
 aliyunsdkiot/request/v20180120/SetDeviceGroupTagsRequest.py
 aliyunsdkiot/request/v20180120/SetDevicePropertyRequest.py
 aliyunsdkiot/request/v20180120/SetDevicesPropertyRequest.py
 aliyunsdkiot/request/v20180120/SetEdgeInstanceDriverConfigsRequest.py
 aliyunsdkiot/request/v20180120/SetProductCertInfoRequest.py
 aliyunsdkiot/request/v20180120/StartRuleRequest.py
 aliyunsdkiot/request/v20180120/StopRuleRequest.py
+aliyunsdkiot/request/v20180120/TriggerSceneRuleRequest.py
 aliyunsdkiot/request/v20180120/UnbindApplicationFromEdgeInstanceRequest.py
 aliyunsdkiot/request/v20180120/UnbindDriverFromEdgeInstanceRequest.py
+aliyunsdkiot/request/v20180120/UnbindSceneRuleFromEdgeInstanceRequest.py
+aliyunsdkiot/request/v20180120/UpdateConsumerGroupRequest.py
 aliyunsdkiot/request/v20180120/UpdateDeviceGroupRequest.py
 aliyunsdkiot/request/v20180120/UpdateDeviceShadowRequest.py
 aliyunsdkiot/request/v20180120/UpdateEdgeDriverVersionRequest.py
 aliyunsdkiot/request/v20180120/UpdateEdgeInstanceChannelRequest.py
 aliyunsdkiot/request/v20180120/UpdateEdgeInstanceRequest.py
 aliyunsdkiot/request/v20180120/UpdateProductFilterConfigRequest.py
 aliyunsdkiot/request/v20180120/UpdateProductRequest.py
 aliyunsdkiot/request/v20180120/UpdateProductTagsRequest.py
 aliyunsdkiot/request/v20180120/UpdateProductTopicRequest.py
 aliyunsdkiot/request/v20180120/UpdateRuleActionRequest.py
 aliyunsdkiot/request/v20180120/UpdateRuleRequest.py
+aliyunsdkiot/request/v20180120/UpdateSceneRuleRequest.py
+aliyunsdkiot/request/v20180120/UpdateSubscribeRelationRequest.py
 aliyunsdkiot/request/v20180120/UpdateThingModelRequest.py
 aliyunsdkiot/request/v20180120/__init__.py
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyun_python_sdk_iot.egg-info/PKG-INFO` & `aliyun-python-sdk-iot-8.9.0/aliyun_python_sdk_iot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-iot
-Version: 8.8.0
+Version: 8.9.0
 Summary: The iot module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-iot
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/SetDeviceGroupTagsRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/SetDeviceGroupTagsRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class SetDeviceGroupTagsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'SetDeviceGroupTags','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'SetDeviceGroupTags','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CancelOTAStrategyByJobRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CancelOTAStrategyByJobRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class CancelOTAStrategyByJobRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CancelOTAStrategyByJob','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CancelOTAStrategyByJob','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateLoRaNodesTaskRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateLoRaNodesTaskRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class CreateLoRaNodesTaskRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateLoRaNodesTask','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateLoRaNodesTask','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchCheckDeviceNamesRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchCheckDeviceNamesRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class BatchCheckDeviceNamesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchCheckDeviceNames','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchCheckDeviceNames','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateEdgeInstanceRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateEdgeInstanceRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class CreateEdgeInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateEdgeInstance','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateEdgeInstance','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/DeleteEdgeDriverVersionRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DeleteEdgeDriverVersionRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class DeleteEdgeDriverVersionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'DeleteEdgeDriverVersion','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'DeleteEdgeDriverVersion','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/InvokeDataAPIServiceRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/InvokeDataAPIServiceRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class InvokeDataAPIServiceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'InvokeDataAPIService','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'InvokeDataAPIService','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchRegisterDeviceRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchRegisterDeviceRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class BatchRegisterDeviceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchRegisterDevice','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchRegisterDevice','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/UpdateProductTopicRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/UpdateProductTopicRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class UpdateProductTopicRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'UpdateProductTopic','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'UpdateProductTopic','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/SaveDevicePropRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/SaveDevicePropRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class SaveDevicePropRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'SaveDeviceProp','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'SaveDeviceProp','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDeviceDetailRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDeviceDetailRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryDeviceDetailRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDeviceDetail','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDeviceDetail','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/RemoveThingTopoRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/RemoveThingTopoRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class RemoveThingTopoRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'RemoveThingTopo','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'RemoveThingTopo','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/ReplaceEdgeInstanceGatewayRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/ReplaceEdgeInstanceGatewayRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class ReplaceEdgeInstanceGatewayRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'ReplaceEdgeInstanceGateway','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'ReplaceEdgeInstanceGateway','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/RRpcRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/RRpcRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class RRpcRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'RRpc','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'RRpc','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/NotifyAddThingTopoRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/NotifyAddThingTopoRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class NotifyAddThingTopoRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'NotifyAddThingTopo','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'NotifyAddThingTopo','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryEdgeDriverVersionRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryEdgeDriverVersionRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryEdgeDriverVersionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryEdgeDriverVersion','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryEdgeDriverVersion','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/GetThingModelTslRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/GetThingModelTslRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class GetThingModelTslRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'GetThingModelTsl','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'GetThingModelTsl','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateProductTagsRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateProductTagsRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class CreateProductTagsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateProductTags','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateProductTags','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchUnbindDeviceFromEdgeInstanceRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchUnbindDeviceFromEdgeInstanceRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class BatchUnbindDeviceFromEdgeInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchUnbindDeviceFromEdgeInstance','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchUnbindDeviceFromEdgeInstance','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/InvokeThingServiceRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/InvokeThingServiceRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class InvokeThingServiceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'InvokeThingService','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'InvokeThingService','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/ResetThingRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/ResetThingRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class ResetThingRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'ResetThing','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'ResetThing','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/DeleteProductTagsRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DeleteProductTagsRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class DeleteProductTagsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'DeleteProductTags','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'DeleteProductTags','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateEdgeDriverRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateEdgeDriverRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class CreateEdgeDriverRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateEdgeDriver','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateEdgeDriver','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchAddDeviceGroupRelationsRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchAddDeviceGroupRelationsRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class BatchAddDeviceGroupRelationsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchAddDeviceGroupRelations','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchAddDeviceGroupRelations','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryProductCertInfoRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryProductCertInfoRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryProductCertInfoRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryProductCertInfo','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryProductCertInfo','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchGetDeviceStateRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchGetDeviceStateRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class BatchGetDeviceStateRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchGetDeviceState','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchGetDeviceState','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/ListThingTemplatesRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/ListThingTemplatesRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class ListThingTemplatesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'ListThingTemplates','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'ListThingTemplates','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDeviceDesiredPropertyRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDeviceDesiredPropertyRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryDeviceDesiredPropertyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDeviceDesiredProperty','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDeviceDesiredProperty','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchGetEdgeInstanceDeviceDriverRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchGetEdgeInstanceDeviceDriverRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class BatchGetEdgeInstanceDeviceDriverRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchGetEdgeInstanceDeviceDriver','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchGetEdgeInstanceDeviceDriver','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDeviceGroupByDeviceRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDeviceGroupByDeviceRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryDeviceGroupByDeviceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDeviceGroupByDevice','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDeviceGroupByDevice','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryProductListRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryProductListRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryProductListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryProductList','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryProductList','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/EnableThingRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/EnableThingRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class EnableThingRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'EnableThing','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'EnableThing','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/UnbindApplicationFromEdgeInstanceRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/UnbindApplicationFromEdgeInstanceRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class UnbindApplicationFromEdgeInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'UnbindApplicationFromEdgeInstance','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'UnbindApplicationFromEdgeInstance','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDeviceListByDeviceGroupRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDeviceListByDeviceGroupRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryDeviceListByDeviceGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDeviceListByDeviceGroup','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDeviceListByDeviceGroup','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/GetEdgeInstanceRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/GetEdgeInstanceRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class GetEdgeInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'GetEdgeInstance','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'GetEdgeInstance','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QuerySuperDeviceGroupRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QuerySuperDeviceGroupRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QuerySuperDeviceGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QuerySuperDeviceGroup','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QuerySuperDeviceGroup','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryLoRaJoinPermissionsRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryLoRaJoinPermissionsRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryLoRaJoinPermissionsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryLoRaJoinPermissions','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryLoRaJoinPermissions','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDeviceFileRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDeviceFileRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryDeviceFileRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDeviceFile','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDeviceFile','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/SetProductCertInfoRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/SetProductCertInfoRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class SetProductCertInfoRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'SetProductCertInfo','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'SetProductCertInfo','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BindGatewayToEdgeInstanceRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BindGatewayToEdgeInstanceRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class BindGatewayToEdgeInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BindGatewayToEdgeInstance','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BindGatewayToEdgeInstance','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/GetDataAPIServiceDetailRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/GetDataAPIServiceDetailRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class GetDataAPIServiceDetailRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'GetDataAPIServiceDetail','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'GetDataAPIServiceDetail','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/GenerateOTAUploadURLRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/GenerateOTAUploadURLRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class GenerateOTAUploadURLRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'GenerateOTAUploadURL','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'GenerateOTAUploadURL','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/InvokeThingsServiceRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/InvokeThingsServiceRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class InvokeThingsServiceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'InvokeThingsService','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'InvokeThingsService','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDevicePropertiesDataRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDevicePropertiesDataRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryDevicePropertiesDataRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDevicePropertiesData','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDevicePropertiesData','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateEdgeDriverVersionRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateEdgeDriverVersionRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,28 +19,34 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class CreateEdgeDriverVersionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateEdgeDriverVersion','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateEdgeDriverVersion','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ConfigCheckRule(self):
 		return self.get_query_params().get('ConfigCheckRule')
 
 	def set_ConfigCheckRule(self,ConfigCheckRule):
 		self.add_query_param('ConfigCheckRule',ConfigCheckRule)
 
+	def get_Argument(self):
+		return self.get_query_params().get('Argument')
+
+	def set_Argument(self,Argument):
+		self.add_query_param('Argument',Argument)
+
 	def get_EdgeVersion(self):
 		return self.get_query_params().get('EdgeVersion')
 
 	def set_EdgeVersion(self,EdgeVersion):
 		self.add_query_param('EdgeVersion',EdgeVersion)
 
 	def get_Description(self):
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/ListOTAJobByFirmwareRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/ListOTAJobByFirmwareRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class ListOTAJobByFirmwareRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'ListOTAJobByFirmware','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'ListOTAJobByFirmware','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/GetDeviceStatusRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DeleteDeviceFileRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
-class GetDeviceStatusRequest(RpcRequest):
+class DeleteDeviceFileRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'GetDeviceStatus','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'DeleteDeviceFile','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
@@ -39,14 +39,20 @@
 
 	def get_IotInstanceId(self):
 		return self.get_query_params().get('IotInstanceId')
 
 	def set_IotInstanceId(self,IotInstanceId):
 		self.add_query_param('IotInstanceId',IotInstanceId)
 
+	def get_FileId(self):
+		return self.get_query_params().get('FileId')
+
+	def set_FileId(self,FileId):
+		self.add_query_param('FileId',FileId)
+
 	def get_ProductKey(self):
 		return self.get_query_params().get('ProductKey')
 
 	def set_ProductKey(self,ProductKey):
 		self.add_query_param('ProductKey',ProductKey)
 
 	def get_DeviceName(self):
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/SetDevicesPropertyRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/SetDevicesPropertyRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class SetDevicesPropertyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'SetDevicesProperty','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'SetDevicesProperty','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateDeviceGroupRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateDeviceGroupRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class CreateDeviceGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateDeviceGroup','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateDeviceGroup','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchGetEdgeInstanceChannelRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchGetEdgeInstanceChannelRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class BatchGetEdgeInstanceChannelRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchGetEdgeInstanceChannel','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchGetEdgeInstanceChannel','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDevicePropRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDevicePropRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryDevicePropRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDeviceProp','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDeviceProp','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BindApplicationToEdgeInstanceRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BindApplicationToEdgeInstanceRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class BindApplicationToEdgeInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BindApplicationToEdgeInstance','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BindApplicationToEdgeInstance','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryAppDeviceListRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryAppDeviceListRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryAppDeviceListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryAppDeviceList','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryAppDeviceList','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDeviceFileListRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDeviceFileListRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryDeviceFileListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDeviceFileList','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDeviceFileList','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/GetGatewayBySubDeviceRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/GetGatewayBySubDeviceRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class GetGatewayBySubDeviceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'GetGatewayBySubDevice','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'GetGatewayBySubDevice','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryEdgeInstanceRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryEdgeInstanceRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryEdgeInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryEdgeInstance','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryEdgeInstance','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateOTADynamicUpgradeJobRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateOTADynamicUpgradeJobRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class CreateOTADynamicUpgradeJobRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateOTADynamicUpgradeJob','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateOTADynamicUpgradeJob','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryEdgeDriverRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryEdgeDriverRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryEdgeDriverRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryEdgeDriver','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryEdgeDriver','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/DeleteProductRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DeleteProductRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class DeleteProductRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'DeleteProduct','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'DeleteProduct','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchGetEdgeDriverRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchGetEdgeDriverRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class BatchGetEdgeDriverRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchGetEdgeDriver','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchGetEdgeDriver','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/ListOTATaskByJobRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/ListOTATaskByJobRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class ListOTATaskByJobRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'ListOTATaskByJob','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'ListOTATaskByJob','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryOTAJobRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryOTAJobRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryOTAJobRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryOTAJob','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryOTAJob','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/GetThingTopoRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/GetThingTopoRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class GetThingTopoRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'GetThingTopo','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'GetThingTopo','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateRuleRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateRuleRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class CreateRuleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateRule','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateRule','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDevicePropertyStatusRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDevicePropertyStatusRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryDevicePropertyStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDevicePropertyStatus','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDevicePropertyStatus','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchQueryDeviceDetailRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchQueryDeviceDetailRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class BatchQueryDeviceDetailRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchQueryDeviceDetail','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchQueryDeviceDetail','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDeviceServiceDataRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDeviceServiceDataRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryDeviceServiceDataRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDeviceServiceData','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDeviceServiceData','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateEdgeOssPreSignedAddressRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateEdgeOssPreSignedAddressRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class CreateEdgeOssPreSignedAddressRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateEdgeOssPreSignedAddress','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateEdgeOssPreSignedAddress','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/GetNodesAddingTaskRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/GetNodesAddingTaskRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class GetNodesAddingTaskRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'GetNodesAddingTask','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'GetNodesAddingTask','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/ListThingModelVersionRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/ListRuleRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
-class ListThingModelVersionRequest(RpcRequest):
+class ListRuleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'ListThingModelVersion','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'ListRule','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
@@ -39,12 +39,18 @@
 
 	def get_IotInstanceId(self):
 		return self.get_query_params().get('IotInstanceId')
 
 	def set_IotInstanceId(self,IotInstanceId):
 		self.add_query_param('IotInstanceId',IotInstanceId)
 
-	def get_ProductKey(self):
-		return self.get_query_params().get('ProductKey')
+	def get_PageSize(self):
+		return self.get_query_params().get('PageSize')
 
-	def set_ProductKey(self,ProductKey):
-		self.add_query_param('ProductKey',ProductKey)
+	def set_PageSize(self,PageSize):
+		self.add_query_param('PageSize',PageSize)
+
+	def get_CurrentPage(self):
+		return self.get_query_params().get('CurrentPage')
+
+	def set_CurrentPage(self,CurrentPage):
+		self.add_query_param('CurrentPage',CurrentPage)
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateOTAFirmwareRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateOTAFirmwareRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class CreateOTAFirmwareRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateOTAFirmware','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateOTAFirmware','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/PublishThingModelRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/PublishThingModelRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class PublishThingModelRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'PublishThingModel','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'PublishThingModel','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryEdgeInstanceGatewayRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryEdgeInstanceGatewayRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryEdgeInstanceGatewayRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryEdgeInstanceGateway','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryEdgeInstanceGateway','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDevicePropertyDataRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDevicePropertyDataRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryDevicePropertyDataRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDevicePropertyData','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDevicePropertyData','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDeviceByStatusRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDeviceByStatusRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryDeviceByStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDeviceByStatus','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDeviceByStatus','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDeviceGroupListRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDeviceGroupListRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryDeviceGroupListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDeviceGroupList','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDeviceGroupList','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateProductTopicRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateProductTopicRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class CreateProductTopicRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateProductTopic','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateProductTopic','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/SetDevicePropertyRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/SetDevicePropertyRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class SetDevicePropertyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'SetDeviceProperty','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'SetDeviceProperty','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateTopicRouteTableRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateTopicRouteTableRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class CreateTopicRouteTableRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateTopicRouteTable','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateTopicRouteTable','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/PubRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/PubRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class PubRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'Pub','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'Pub','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchUpdateDeviceNicknameRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchUpdateDeviceNicknameRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class BatchUpdateDeviceNicknameRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchUpdateDeviceNickname','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchUpdateDeviceNickname','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/ReleaseEdgeDriverVersionRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/ReleaseEdgeDriverVersionRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class ReleaseEdgeDriverVersionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'ReleaseEdgeDriverVersion','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'ReleaseEdgeDriverVersion','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/ListProductByTagsRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/ListProductByTagsRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class ListProductByTagsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'ListProductByTags','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'ListProductByTags','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateThingModelRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateThingModelRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class CreateThingModelRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateThingModel','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateThingModel','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/UpdateDeviceShadowRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/UpdateDeviceShadowRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class UpdateDeviceShadowRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'UpdateDeviceShadow','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'UpdateDeviceShadow','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BindDriverToEdgeInstanceRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BindDriverToEdgeInstanceRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class BindDriverToEdgeInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BindDriverToEdgeInstance','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BindDriverToEdgeInstance','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/RegisterDeviceRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/RegisterDeviceRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class RegisterDeviceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'RegisterDevice','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'RegisterDevice','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CancelOTATaskByDeviceRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CancelOTATaskByDeviceRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class CancelOTATaskByDeviceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CancelOTATaskByDevice','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CancelOTATaskByDevice','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/ListOTAFirmwareRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/ListOTAFirmwareRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class ListOTAFirmwareRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'ListOTAFirmware','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'ListOTAFirmware','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryTopicReverseRouteTableRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryTopicRouteTableRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
-class QueryTopicReverseRouteTableRequest(RpcRequest):
+class QueryTopicRouteTableRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryTopicReverseRouteTable','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryTopicRouteTable','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/ListProductTagsRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/ListProductTagsRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class ListProductTagsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'ListProductTags','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'ListProductTags','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CancelOTATaskByJobRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CancelOTATaskByJobRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class CancelOTATaskByJobRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CancelOTATaskByJob','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CancelOTATaskByJob','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/ListRuleRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QuerySceneRuleRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,30 +16,30 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
-class ListRuleRequest(RpcRequest):
+class QuerySceneRuleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'ListRule','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QuerySceneRule','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
-	def get_ResourceGroupId(self):
-		return self.get_query_params().get('ResourceGroupId')
+	def get_RuleName(self):
+		return self.get_query_params().get('RuleName')
 
-	def set_ResourceGroupId(self,ResourceGroupId):
-		self.add_query_param('ResourceGroupId',ResourceGroupId)
+	def set_RuleName(self,RuleName):
+		self.add_query_param('RuleName',RuleName)
 
 	def get_IotInstanceId(self):
 		return self.get_query_params().get('IotInstanceId')
 
 	def set_IotInstanceId(self,IotInstanceId):
 		self.add_query_param('IotInstanceId',IotInstanceId)
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/PubBroadcastRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/PubBroadcastRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class PubBroadcastRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'PubBroadcast','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'PubBroadcast','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDeviceRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDeviceRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryDeviceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDevice','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDevice','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/GetLoraNodesTaskRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/StartRuleRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,29 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
-class GetLoraNodesTaskRequest(RpcRequest):
+class StartRuleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'GetLoraNodesTask','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'StartRule','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_IotInstanceId(self):
 		return self.get_query_params().get('IotInstanceId')
 
 	def set_IotInstanceId(self,IotInstanceId):
 		self.add_query_param('IotInstanceId',IotInstanceId)
 
-	def get_TaskId(self):
-		return self.get_query_params().get('TaskId')
+	def get_RuleId(self):
+		return self.get_query_params().get('RuleId')
 
-	def set_TaskId(self,TaskId):
-		self.add_query_param('TaskId',TaskId)
+	def set_RuleId(self,RuleId):
+		self.add_query_param('RuleId',RuleId)
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CloseEdgeInstanceDeploymentRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/TriggerSceneRuleRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
-class CloseEdgeInstanceDeploymentRequest(RpcRequest):
+class TriggerSceneRuleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CloseEdgeInstanceDeployment','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'TriggerSceneRule','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
@@ -37,8 +37,14 @@
 	def set_IotInstanceId(self,IotInstanceId):
 		self.add_query_param('IotInstanceId',IotInstanceId)
 
 	def get_InstanceId(self):
 		return self.get_query_params().get('InstanceId')
 
 	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+		self.add_query_param('InstanceId',InstanceId)
+
+	def get_RuleId(self):
+		return self.get_query_params().get('RuleId')
+
+	def set_RuleId(self,RuleId):
+		self.add_query_param('RuleId',RuleId)
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryProductTopicRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryProductRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
-class QueryProductTopicRequest(RpcRequest):
+class QueryProductRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryProductTopic','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryProduct','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDeviceGroupInfoRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDeviceGroupInfoRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryDeviceGroupInfoRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDeviceGroupInfo','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDeviceGroupInfo','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/UpdateProductTagsRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/UpdateProductTagsRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class UpdateProductTagsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'UpdateProductTags','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'UpdateProductTags','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/DisableThingRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DisableThingRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class DisableThingRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'DisableThing','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'DisableThing','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchRegisterDeviceWithApplyIdRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchRegisterDeviceWithApplyIdRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class BatchRegisterDeviceWithApplyIdRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchRegisterDeviceWithApplyId','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchRegisterDeviceWithApplyId','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/ListRuleActionsRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/ListRuleActionsRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class ListRuleActionsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'ListRuleActions','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'ListRuleActions','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/DeleteDeviceGroupRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DeleteDeviceGroupRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class DeleteDeviceGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'DeleteDeviceGroup','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'DeleteDeviceGroup','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/GetEdgeDriverVersionRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/GetEdgeDriverVersionRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class GetEdgeDriverVersionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'GetEdgeDriverVersion','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'GetEdgeDriverVersion','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateOTAStaticUpgradeJobRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateOTAStaticUpgradeJobRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class CreateOTAStaticUpgradeJobRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateOTAStaticUpgradeJob','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateOTAStaticUpgradeJob','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/DeleteRuleRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DeleteRuleRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class DeleteRuleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'DeleteRule','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'DeleteRule','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/UpdateEdgeDriverVersionRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/UpdateEdgeDriverVersionRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,28 +19,34 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class UpdateEdgeDriverVersionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'UpdateEdgeDriverVersion','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'UpdateEdgeDriverVersion','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ConfigCheckRule(self):
 		return self.get_query_params().get('ConfigCheckRule')
 
 	def set_ConfigCheckRule(self,ConfigCheckRule):
 		self.add_query_param('ConfigCheckRule',ConfigCheckRule)
 
+	def get_Argument(self):
+		return self.get_query_params().get('Argument')
+
+	def set_Argument(self,Argument):
+		self.add_query_param('Argument',Argument)
+
 	def get_EdgeVersion(self):
 		return self.get_query_params().get('EdgeVersion')
 
 	def set_EdgeVersion(self,EdgeVersion):
 		self.add_query_param('EdgeVersion',EdgeVersion)
 
 	def get_Description(self):
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/DeleteProductTopicRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DeleteProductTopicRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class DeleteProductTopicRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'DeleteProductTopic','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'DeleteProductTopic','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/DeleteOTAFirmwareRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DeleteOTAFirmwareRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class DeleteOTAFirmwareRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'DeleteOTAFirmware','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'DeleteOTAFirmware','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchGetEdgeInstanceDeviceConfigRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchClearEdgeInstanceDeviceConfigRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
-class BatchGetEdgeInstanceDeviceConfigRequest(RpcRequest):
+class BatchClearEdgeInstanceDeviceConfigRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchGetEdgeInstanceDeviceConfig','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchClearEdgeInstanceDeviceConfig','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryEdgeInstanceDriverRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryEdgeInstanceDriverRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryEdgeInstanceDriverRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryEdgeInstanceDriver','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryEdgeInstanceDriver','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/ClearEdgeInstanceDriverConfigsRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/ClearEdgeInstanceDriverConfigsRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class ClearEdgeInstanceDriverConfigsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'ClearEdgeInstanceDriverConfigs','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'ClearEdgeInstanceDriverConfigs','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/GetRuleActionRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/GetRuleActionRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class GetRuleActionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'GetRuleAction','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'GetRuleAction','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/ImportThingModelTslRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/ImportThingModelTslRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class ImportThingModelTslRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'ImportThingModelTsl','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'ImportThingModelTsl','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryTopicRouteTableRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryTopicReverseRouteTableRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
-class QueryTopicRouteTableRequest(RpcRequest):
+class QueryTopicReverseRouteTableRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryTopicRouteTable','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryTopicReverseRouteTable','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/DeleteEdgeDriverRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DeleteEdgeDriverRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class DeleteEdgeDriverRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'DeleteEdgeDriver','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'DeleteEdgeDriver','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDeviceCertRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDeviceCertRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryDeviceCertRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDeviceCert','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDeviceCert','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchGetEdgeInstanceDeviceChannelRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchGetEdgeInstanceDeviceChannelRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class BatchGetEdgeInstanceDeviceChannelRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchGetEdgeInstanceDeviceChannel','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchGetEdgeInstanceDeviceChannel','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateEdgeInstanceDeploymentRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchGetEdgeInstanceDeviceConfigRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,30 +16,32 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
-class CreateEdgeInstanceDeploymentRequest(RpcRequest):
+class BatchGetEdgeInstanceDeviceConfigRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateEdgeInstanceDeployment','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchGetEdgeInstanceDeviceConfig','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
-	def get_Type(self):
-		return self.get_query_params().get('Type')
+	def get_IotIdss(self):
+		return self.get_query_params().get('IotIdss')
 
-	def set_Type(self,Type):
-		self.add_query_param('Type',Type)
+	def set_IotIdss(self, IotIdss):
+		for depth1 in range(len(IotIdss)):
+			if IotIdss[depth1] is not None:
+				self.add_query_param('IotIds.' + str(depth1 + 1) , IotIdss[depth1])
 
 	def get_IotInstanceId(self):
 		return self.get_query_params().get('IotInstanceId')
 
 	def set_IotInstanceId(self,IotInstanceId):
 		self.add_query_param('IotInstanceId',IotInstanceId)
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDeviceStatisticsRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDeviceStatisticsRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryDeviceStatisticsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDeviceStatistics','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDeviceStatistics','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/UpdateProductFilterConfigRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/UpdateProductFilterConfigRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class UpdateProductFilterConfigRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'UpdateProductFilterConfig','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'UpdateProductFilterConfig','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchSetEdgeInstanceDeviceChannelRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchSetEdgeInstanceDeviceChannelRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class BatchSetEdgeInstanceDeviceChannelRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchSetEdgeInstanceDeviceChannel','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchSetEdgeInstanceDeviceChannel','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/StopRuleRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/StopRuleRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class StopRuleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'StopRule','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'StopRule','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchDeleteEdgeInstanceChannelRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchDeleteEdgeInstanceChannelRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class BatchDeleteEdgeInstanceChannelRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchDeleteEdgeInstanceChannel','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchDeleteEdgeInstanceChannel','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDeviceGroupByTagsRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDeviceGroupByTagsRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryDeviceGroupByTagsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDeviceGroupByTags','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDeviceGroupByTags','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchAddThingTopoRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchAddThingTopoRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class BatchAddThingTopoRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchAddThingTopo','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchAddThingTopo','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDeviceEventDataRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDeviceEventDataRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryDeviceEventDataRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDeviceEventData','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDeviceEventData','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CopyThingModelRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CopyThingModelRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class CopyThingModelRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CopyThingModel','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CopyThingModel','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryOTAFirmwareRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryOTAFirmwareRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryOTAFirmwareRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryOTAFirmware','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryOTAFirmware','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryEdgeInstanceChannelRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryEdgeInstanceChannelRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryEdgeInstanceChannelRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryEdgeInstanceChannel','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryEdgeInstanceChannel','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/DeleteDevicePropRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DeleteDevicePropRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class DeleteDevicePropRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'DeleteDeviceProp','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'DeleteDeviceProp','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/SetDeviceDesiredPropertyRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/SetDeviceDesiredPropertyRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class SetDeviceDesiredPropertyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'SetDeviceDesiredProperty','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'SetDeviceDesiredProperty','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchDeleteDeviceGroupRelationsRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchDeleteDeviceGroupRelationsRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class BatchDeleteDeviceGroupRelationsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchDeleteDeviceGroupRelations','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchDeleteDeviceGroupRelations','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryBatchRegisterDeviceStatusRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryBatchRegisterDeviceStatusRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryBatchRegisterDeviceStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryBatchRegisterDeviceStatus','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryBatchRegisterDeviceStatus','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/ListOTAJobByDeviceRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/ListOTAJobByDeviceRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class ListOTAJobByDeviceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'ListOTAJobByDevice','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'ListOTAJobByDevice','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/DeleteDeviceRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DeleteDeviceRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class DeleteDeviceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'DeleteDevice','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'DeleteDevice','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateProductRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateProductRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class CreateProductRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateProduct','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateProduct','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/UpdateThingModelRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/UpdateThingModelRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class UpdateThingModelRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'UpdateThingModel','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'UpdateThingModel','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/GetEdgeInstanceDeploymentRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/GetEdgeInstanceDeploymentRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class GetEdgeInstanceDeploymentRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'GetEdgeInstanceDeployment','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'GetEdgeInstanceDeployment','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/DeleteTopicRouteTableRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DeleteTopicRouteTableRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class DeleteTopicRouteTableRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'DeleteTopicRouteTable','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'DeleteTopicRouteTable','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchSetEdgeInstanceDeviceConfigRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchSetEdgeInstanceDeviceConfigRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class BatchSetEdgeInstanceDeviceConfigRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchSetEdgeInstanceDeviceConfig','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchSetEdgeInstanceDeviceConfig','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/UpdateRuleRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/UpdateRuleRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class UpdateRuleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'UpdateRule','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'UpdateRule','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/DeleteDeviceFileRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/GetDeviceStatusRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
-class DeleteDeviceFileRequest(RpcRequest):
+class GetDeviceStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'DeleteDeviceFile','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'GetDeviceStatus','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
@@ -39,20 +39,14 @@
 
 	def get_IotInstanceId(self):
 		return self.get_query_params().get('IotInstanceId')
 
 	def set_IotInstanceId(self,IotInstanceId):
 		self.add_query_param('IotInstanceId',IotInstanceId)
 
-	def get_FileId(self):
-		return self.get_query_params().get('FileId')
-
-	def set_FileId(self,FileId):
-		self.add_query_param('FileId',FileId)
-
 	def get_ProductKey(self):
 		return self.get_query_params().get('ProductKey')
 
 	def set_ProductKey(self,ProductKey):
 		self.add_query_param('ProductKey',ProductKey)
 
 	def get_DeviceName(self):
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryThingModelRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryThingModelRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryThingModelRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryThingModel','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryThingModel','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateEdgeInstanceChannelRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateEdgeInstanceChannelRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class CreateEdgeInstanceChannelRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateEdgeInstanceChannel','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateEdgeInstanceChannel','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryEdgeInstanceDeviceRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryEdgeInstanceDeviceRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryEdgeInstanceDeviceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryEdgeInstanceDevice','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryEdgeInstanceDevice','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateOTAVerifyJobRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateOTAVerifyJobRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class CreateOTAVerifyJobRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateOTAVerifyJob','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateOTAVerifyJob','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/DeleteThingModelRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DeleteThingModelRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class DeleteThingModelRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'DeleteThingModel','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'DeleteThingModel','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchClearEdgeInstanceDeviceConfigRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/UnbindSceneRuleFromEdgeInstanceRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,37 +16,35 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
-class BatchClearEdgeInstanceDeviceConfigRequest(RpcRequest):
+class UnbindSceneRuleFromEdgeInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchClearEdgeInstanceDeviceConfig','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'UnbindSceneRuleFromEdgeInstance','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
-	def get_IotIdss(self):
-		return self.get_query_params().get('IotIdss')
-
-	def set_IotIdss(self, IotIdss):
-		for depth1 in range(len(IotIdss)):
-			if IotIdss[depth1] is not None:
-				self.add_query_param('IotIds.' + str(depth1 + 1) , IotIdss[depth1])
-
 	def get_IotInstanceId(self):
 		return self.get_query_params().get('IotInstanceId')
 
 	def set_IotInstanceId(self,IotInstanceId):
 		self.add_query_param('IotInstanceId',IotInstanceId)
 
 	def get_InstanceId(self):
 		return self.get_query_params().get('InstanceId')
 
 	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+		self.add_query_param('InstanceId',InstanceId)
+
+	def get_RuleId(self):
+		return self.get_query_params().get('RuleId')
+
+	def set_RuleId(self,RuleId):
+		self.add_query_param('RuleId',RuleId)
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/DeleteEdgeInstanceRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DeleteEdgeInstanceRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class DeleteEdgeInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'DeleteEdgeInstance','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'DeleteEdgeInstance','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/DeleteRuleActionRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/DeleteRuleActionRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class DeleteRuleActionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'DeleteRuleAction','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'DeleteRuleAction','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/GetDeviceShadowRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/GetDeviceShadowRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class GetDeviceShadowRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'GetDeviceShadow','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'GetDeviceShadow','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/UpdateDeviceGroupRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/UpdateDeviceGroupRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class UpdateDeviceGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'UpdateDeviceGroup','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'UpdateDeviceGroup','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryEdgeInstanceHistoricDeploymentRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryEdgeInstanceHistoricDeploymentRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryEdgeInstanceHistoricDeploymentRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryEdgeInstanceHistoricDeployment','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryEdgeInstanceHistoricDeployment','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDeviceByTagsRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDeviceByTagsRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryDeviceByTagsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDeviceByTags','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDeviceByTags','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/SetEdgeInstanceDriverConfigsRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/SetEdgeInstanceDriverConfigsRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class SetEdgeInstanceDriverConfigsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'SetEdgeInstanceDriverConfigs','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'SetEdgeInstanceDriverConfigs','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateDataAPIServiceRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateDataAPIServiceRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class CreateDataAPIServiceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateDataAPIService','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateDataAPIService','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/UnbindDriverFromEdgeInstanceRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/UnbindDriverFromEdgeInstanceRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class UnbindDriverFromEdgeInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'UnbindDriverFromEdgeInstance','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'UnbindDriverFromEdgeInstance','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/GetThingTemplateRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/GetThingTemplateRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class GetThingTemplateRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'GetThingTemplate','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'GetThingTemplate','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchBindDeviceToEdgeInstanceWithDriverRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchBindDeviceToEdgeInstanceWithDriverRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class BatchBindDeviceToEdgeInstanceWithDriverRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchBindDeviceToEdgeInstanceWithDriver','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchBindDeviceToEdgeInstanceWithDriver','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/UpdateEdgeInstanceChannelRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/UpdateEdgeInstanceChannelRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class UpdateEdgeInstanceChannelRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'UpdateEdgeInstanceChannel','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'UpdateEdgeInstanceChannel','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryEdgeInstanceDeviceByDriverRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryEdgeInstanceDeviceByDriverRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryEdgeInstanceDeviceByDriverRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryEdgeInstanceDeviceByDriver','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryEdgeInstanceDeviceByDriver','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/UpdateEdgeInstanceRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/UpdateEdgeInstanceRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class UpdateEdgeInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'UpdateEdgeInstance','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'UpdateEdgeInstance','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryProductRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryProductTopicRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
-class QueryProductRequest(RpcRequest):
+class QueryProductTopicRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryProduct','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryProductTopic','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchGetEdgeInstanceDriverConfigsRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchGetEdgeInstanceDriverConfigsRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class BatchGetEdgeInstanceDriverConfigsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchGetEdgeInstanceDriverConfigs','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchGetEdgeInstanceDriverConfigs','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/GetRuleRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/GetRuleRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class GetRuleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'GetRule','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'GetRule','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/UpdateRuleActionRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/UpdateRuleActionRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class UpdateRuleActionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'UpdateRuleAction','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'UpdateRuleAction','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/UpdateProductRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/UpdateProductRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class UpdateProductRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'UpdateProduct','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'UpdateProduct','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/BatchGetDeviceBindStatusRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/BatchGetDeviceBindStatusRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class BatchGetDeviceBindStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchGetDeviceBindStatus','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'BatchGetDeviceBindStatus','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryDeviceGroupTagListRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryDeviceGroupTagListRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryDeviceGroupTagListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDeviceGroupTagList','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryDeviceGroupTagList','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryCertUrlByApplyIdRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryCertUrlByApplyIdRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryCertUrlByApplyIdRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryCertUrlByApplyId','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryCertUrlByApplyId','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/QueryPageByApplyIdRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/QueryPageByApplyIdRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class QueryPageByApplyIdRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryPageByApplyId','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'QueryPageByApplyId','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/StartRuleRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/GetSceneRuleRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
-class StartRuleRequest(RpcRequest):
+class GetSceneRuleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'StartRule','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'GetSceneRule','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/request/v20180120/CreateRuleActionRequest.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/request/v20180120/CreateRuleActionRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkiot.endpoint import endpoint_data
 
 class CreateRuleActionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateRuleAction','Iot')
+		RpcRequest.__init__(self, 'Iot', '2018-01-20', 'CreateRuleAction','iot')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-iot-8.8.0/aliyunsdkiot/endpoint.py` & `aliyun-python-sdk-iot-8.9.0/aliyunsdkiot/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iot-8.8.0/README.rst` & `aliyun-python-sdk-iot-8.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iot-8.8.0/PKG-INFO` & `aliyun-python-sdk-iot-8.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-iot
-Version: 8.8.0
+Version: 8.9.0
 Summary: The iot module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-iot
```

### Comparing `aliyun-python-sdk-iot-8.8.0/setup.py` & `aliyun-python-sdk-iot-8.9.0/setup.py`

 * *Files identical despite different names*

