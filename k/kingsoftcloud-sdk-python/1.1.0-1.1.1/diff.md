# Comparing `tmp/kingsoftcloud-sdk-python-1.1.0.tar.gz` & `tmp/kingsoftcloud-sdk-python-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kingsoftcloud-sdk-python-1.1.0.tar", last modified: Fri Jun 16 08:20:55 2023, max compression
+gzip compressed data, was "kingsoftcloud-sdk-python-1.1.1.tar", last modified: Thu Jul 13 02:23:00 2023, max compression
```

## Comparing `kingsoftcloud-sdk-python-1.1.0.tar` & `kingsoftcloud-sdk-python-1.1.1.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.897421 kingsoftcloud-sdk-python-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-16 08:20:55.897421 kingsoftcloud-sdk-python-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.881421 kingsoftcloud-sdk-python-1.1.0/kingsoftcloud_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-16 08:20:55.000000 kingsoftcloud-sdk-python-1.1.0/kingsoftcloud_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-06-16 08:20:55.000000 kingsoftcloud-sdk-python-1.1.0/kingsoftcloud_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 08:20:55.000000 kingsoftcloud-sdk-python-1.1.0/kingsoftcloud_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-16 08:20:55.000000 kingsoftcloud-sdk-python-1.1.0/kingsoftcloud_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 08:20:55.000000 kingsoftcloud-sdk-python-1.1.0/kingsoftcloud_sdk_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.881421 kingsoftcloud-sdk-python-1.1.0/ksyun/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.881421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.881421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/actiontrail/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/actiontrail/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.881421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/actiontrail/v20190401/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/actiontrail/v20190401/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/actiontrail/v20190401/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/actiontrail/v20190401/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.881421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.885421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill/v20180601/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill/v20180601/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill/v20180601/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill/v20180601/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.885421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill_union/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill_union/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.885421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill_union/v20200101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill_union/v20200101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill_union/v20200101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill_union/v20200101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.885421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill_union/v20211209/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill_union/v20211209/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill_union/v20211209/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill_union/v20211209/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.885421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.885421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bws/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bws/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bws/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bws/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.885421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/ebs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/ebs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.885421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/ebs/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/ebs/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16760 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/ebs/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21288 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/ebs/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.885421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/eip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/eip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.885421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/eip/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/eip/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/eip/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/eip/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.885421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/epc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/epc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.885421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/epc/v20151101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/epc/v20151101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47258 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/epc/v20151101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    57434 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/epc/v20151101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.885421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/iam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/iam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.889421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/iam/v20151101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/iam/v20151101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49208 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/iam/v20151101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    42904 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/iam/v20151101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.889421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/kad/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/kad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.889421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/kad/v20161122/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/kad/v20161122/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/kad/v20161122/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/kad/v20161122/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.889421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/kead/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/kead/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.889421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/kead/v20200101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/kead/v20200101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/kead/v20200101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/kead/v20200101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.889421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/kec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/kec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.889421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/kec/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/kec/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    85700 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/kec/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   122915 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/kec/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.889421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/mongodb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/mongodb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.889421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/mongodb/v20170101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/mongodb/v20170101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30975 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/mongodb/v20170101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    36775 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/mongodb/v20170101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.889421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/resourcemanager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/resourcemanager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.889421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/resourcemanager/v20210320/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/resourcemanager/v20210320/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/resourcemanager/v20210320/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/resourcemanager/v20210320/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.889421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/sks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/sks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.889421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/sks/v20151101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/sks/v20151101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/sks/v20151101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/sks/v20151101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.889421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/slb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/slb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.893421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/slb/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/slb/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43349 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/slb/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    59990 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/slb/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.893421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/slb/v20171210/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/slb/v20171210/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/slb/v20171210/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/slb/v20171210/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.893421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/sts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/sts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.893421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/sts/v20151101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/sts/v20151101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/sts/v20151101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/sts/v20151101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.893421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/tagv2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/tagv2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.893421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/tagv2/v20200901/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/tagv2/v20200901/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/tagv2/v20200901/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/tagv2/v20200901/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.893421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/trade/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/trade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.893421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/trade/v20200114/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/trade/v20200114/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/trade/v20200114/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/trade/v20200114/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.893421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/trade/v20200831/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/trade/v20200831/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/trade/v20200831/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/trade/v20200831/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.893421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/vpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/vpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.893421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/vpc/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/vpc/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68705 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/vpc/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    73360 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/vpc/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.897421 kingsoftcloud-sdk-python-1.1.0/ksyun/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/common/abstract_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/common/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/common/common_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/common/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.897421 kingsoftcloud-sdk-python-1.1.0/ksyun/common/exception/
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/common/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/common/exception/ksyun_sdk_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.897421 kingsoftcloud-sdk-python-1.1.0/ksyun/common/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/common/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/common/http/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.897421 kingsoftcloud-sdk-python-1.1.0/ksyun/common/profile/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/common/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/common/profile/client_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/common/profile/http_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/common/sign.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-16 08:20:55.897421 kingsoftcloud-sdk-python-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.249834 kingsoftcloud-sdk-python-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-13 02:23:00.249834 kingsoftcloud-sdk-python-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.233834 kingsoftcloud-sdk-python-1.1.1/kingsoftcloud_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-13 02:23:00.000000 kingsoftcloud-sdk-python-1.1.1/kingsoftcloud_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-07-13 02:23:00.000000 kingsoftcloud-sdk-python-1.1.1/kingsoftcloud_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 02:23:00.000000 kingsoftcloud-sdk-python-1.1.1/kingsoftcloud_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-13 02:23:00.000000 kingsoftcloud-sdk-python-1.1.1/kingsoftcloud_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-13 02:23:00.000000 kingsoftcloud-sdk-python-1.1.1/kingsoftcloud_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.233834 kingsoftcloud-sdk-python-1.1.1/ksyun/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.233834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.233834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/actiontrail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/actiontrail/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.233834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/actiontrail/v20190401/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/actiontrail/v20190401/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/actiontrail/v20190401/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/actiontrail/v20190401/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.233834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.233834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill/v20180601/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill/v20180601/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill/v20180601/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill/v20180601/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.233834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill_union/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill_union/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.237834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill_union/v20200101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill_union/v20200101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill_union/v20200101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill_union/v20200101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.237834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill_union/v20211209/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill_union/v20211209/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill_union/v20211209/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill_union/v20211209/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.237834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.237834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bws/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bws/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bws/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bws/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.237834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/ebs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/ebs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.237834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/ebs/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/ebs/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16760 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/ebs/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21288 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/ebs/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.237834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/eip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/eip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.237834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/eip/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/eip/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/eip/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/eip/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.241834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/epc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/epc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.241834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/epc/v20151101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/epc/v20151101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48112 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/epc/v20151101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58267 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/epc/v20151101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.241834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/iam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.241834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/iam/v20151101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/iam/v20151101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49208 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/iam/v20151101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42904 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/iam/v20151101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.241834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/kad/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/kad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.241834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/kad/v20161122/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/kad/v20161122/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/kad/v20161122/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/kad/v20161122/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.241834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/kead/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/kead/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.241834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/kead/v20200101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/kead/v20200101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/kead/v20200101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/kead/v20200101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.241834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/kec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/kec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.241834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/kec/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/kec/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85700 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/kec/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   122915 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/kec/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.245834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/mongodb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/mongodb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.245834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/mongodb/v20170101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/mongodb/v20170101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30975 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/mongodb/v20170101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36775 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/mongodb/v20170101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.245834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/resourcemanager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/resourcemanager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.245834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/resourcemanager/v20210320/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/resourcemanager/v20210320/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/resourcemanager/v20210320/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/resourcemanager/v20210320/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.245834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/sks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/sks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.245834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/sks/v20151101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/sks/v20151101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/sks/v20151101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/sks/v20151101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.245834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/slb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/slb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.245834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/slb/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/slb/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43349 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/slb/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59990 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/slb/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.245834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/slb/v20171210/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/slb/v20171210/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/slb/v20171210/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/slb/v20171210/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.245834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/sts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/sts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.245834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/sts/v20151101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/sts/v20151101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/sts/v20151101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/sts/v20151101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.245834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/tagv2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/tagv2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.249834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/tagv2/v20200901/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/tagv2/v20200901/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/tagv2/v20200901/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/tagv2/v20200901/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.249834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/trade/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/trade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.249834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/trade/v20200114/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/trade/v20200114/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/trade/v20200114/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/trade/v20200114/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.249834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/trade/v20200831/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/trade/v20200831/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/trade/v20200831/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/trade/v20200831/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.249834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/vpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/vpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.249834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/vpc/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/vpc/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72970 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/vpc/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76572 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/vpc/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.249834 kingsoftcloud-sdk-python-1.1.1/ksyun/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/common/abstract_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/common/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/common/common_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/common/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.249834 kingsoftcloud-sdk-python-1.1.1/ksyun/common/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/common/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/common/exception/ksyun_sdk_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.249834 kingsoftcloud-sdk-python-1.1.1/ksyun/common/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/common/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/common/http/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.249834 kingsoftcloud-sdk-python-1.1.1/ksyun/common/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/common/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/common/profile/client_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/common/profile/http_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/common/sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-13 02:23:00.253834 kingsoftcloud-sdk-python-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/setup.py
```

### Comparing `kingsoftcloud-sdk-python-1.1.0/LICENSE` & `kingsoftcloud-sdk-python-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/PKG-INFO` & `kingsoftcloud-sdk-python-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingsoftcloud-sdk-python
-Version: 1.1.0
+Version: 1.1.1
 Summary: Kingsoft Cloud SDK for Python
 Home-page: https://github.com/ksyun/ksyun-sdk-python
 Author: Kingsoft Cloud
 Maintainer-email: liuhuicheng1@kingsoft.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `kingsoftcloud-sdk-python-1.1.0/README.rst` & `kingsoftcloud-sdk-python-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/kingsoftcloud_sdk_python.egg-info/PKG-INFO` & `kingsoftcloud-sdk-python-1.1.1/kingsoftcloud_sdk_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingsoftcloud-sdk-python
-Version: 1.1.0
+Version: 1.1.1
 Summary: Kingsoft Cloud SDK for Python
 Home-page: https://github.com/ksyun/ksyun-sdk-python
 Author: Kingsoft Cloud
 Maintainer-email: liuhuicheng1@kingsoft.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `kingsoftcloud-sdk-python-1.1.0/kingsoftcloud_sdk_python.egg-info/SOURCES.txt` & `kingsoftcloud-sdk-python-1.1.1/kingsoftcloud_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/__init__.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '1.1.0'
+__version__ = '1.1.1'
```

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/actiontrail/v20190401/client.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/actiontrail/v20190401/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/actiontrail/v20190401/models.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/actiontrail/v20190401/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill/v20180601/client.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill/v20180601/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill/v20180601/models.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill/v20180601/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill_union/v20200101/client.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill_union/v20200101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill_union/v20200101/models.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill_union/v20200101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill_union/v20211209/client.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill_union/v20211209/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill_union/v20211209/models.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill_union/v20211209/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/bws/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/bws/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/bws/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/bws/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/ebs/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/ebs/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/ebs/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/ebs/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/eip/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/eip/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/eip/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/eip/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/epc/v20151101/client.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/epc/v20151101/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -648,14 +648,37 @@
         except Exception as e:
             if isinstance(e, KsyunSDKException):
                 raise
             else:
                 raise KsyunSDKException(e.message, e.message)
 
 
+    def ResetPassword(self, request):
+        """重置密码
+        :param request: Request instance for ResetPassword.
+        :type request: :class:`ksyun.client.epc.v20151101.models.ResetPasswordRequest`
+        """
+        try:
+            params = request._serialize()
+            body = self.call("ResetPassword", params)
+            response = json.loads(body)
+            if "Error" not in response:
+                return body
+            else:
+                code = response["Error"]["Code"]
+                message = response["Error"]["Message"]
+                req_id = response["RequestId"]
+                raise KsyunSDKException(code, message, req_id)
+        except Exception as e:
+            if isinstance(e, KsyunSDKException):
+                raise
+            else:
+                raise KsyunSDKException(e.message, e.message)
+
+
     def ModifyHyperThreading(self, request):
         """修改超线程
         :param request: Request instance for ModifyHyperThreading.
         :type request: :class:`ksyun.client.epc.v20151101.models.ModifyHyperThreadingRequest`
         """
         try:
             params = request._serialize()
```

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/epc/v20151101/models.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/epc/v20151101/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,14 +165,21 @@
         :type PathPrefix: String
         :param GpuImageDriverId: gpu版本
         :type PathPrefix: String
         :param SystemVolumeType: 云硬盘的系统盘类型
         :type PathPrefix: String
         :param SystemVolumeSize: 云硬盘系统盘大小
         :type PathPrefix: String
+        :param RoceNetwork: roce网络
+有效值： Open：开启  Close：关闭 
+
+
+
+
+        :type PathPrefix: String
         """
         self.HostType = None
         self.AvailabilityZone = None
         self.Raid = None
         self.RaidId = None
         self.ImageId = None
         self.NetworkInterfaceMode = None
@@ -214,14 +221,15 @@
         self.KesAgent = None
         self.KmrAgent = None
         self.ComputerName = None
         self.OverclockingAttribute = None
         self.GpuImageDriverId = None
         self.SystemVolumeType = None
         self.SystemVolumeSize = None
+        self.RoceNetwork = None
 
     def _deserialize(self, params):
         if params.get("HostType"):
             self.HostType = params.get("HostType")
         if params.get("AvailabilityZone"):
             self.AvailabilityZone = params.get("AvailabilityZone")
         if params.get("Raid"):
@@ -312,14 +320,16 @@
             self.OverclockingAttribute = params.get("OverclockingAttribute")
         if params.get("GpuImageDriverId"):
             self.GpuImageDriverId = params.get("GpuImageDriverId")
         if params.get("SystemVolumeType"):
             self.SystemVolumeType = params.get("SystemVolumeType")
         if params.get("SystemVolumeSize"):
             self.SystemVolumeSize = params.get("SystemVolumeSize")
+        if params.get("RoceNetwork"):
+            self.RoceNetwork = params.get("RoceNetwork")
 
 
 class StartEpcRequest(AbstractModel):
     """StartEpc请求参数结构体
     """
 
     def __init__(self):
@@ -1070,14 +1080,35 @@
         r"""DeleteRemoteManagement
         """
 
     def _deserialize(self, params):
         return
 
 
+class ResetPasswordRequest(AbstractModel):
+    """ResetPassword请求参数结构体
+    """
+
+    def __init__(self):
+        r"""重置密码
+        :param HostId: 裸金属服务器资源ID
+        :type PathPrefix: String
+        :param Password: 云物理主机的root密码
+        :type PathPrefix: String
+        """
+        self.HostId = None
+        self.Password = None
+
+    def _deserialize(self, params):
+        if params.get("HostId"):
+            self.HostId = params.get("HostId")
+        if params.get("Password"):
+            self.Password = params.get("Password")
+
+
 class ModifyHyperThreadingRequest(AbstractModel):
     """ModifyHyperThreading请求参数结构体
     """
 
     def __init__(self):
         r"""修改超线程
         :param HostId: 裸金属服务器资源ID
@@ -1496,15 +1527,15 @@
     """ModifyOverclockingAttribute请求参数结构体
     """
 
     def __init__(self):
         r"""修改超频
         :param HostId: 裸金属服务器资源ID
         :type PathPrefix: String
-        :param OverclockingAttribute: 超频属性，open|close
+        :param OverclockingAttribute: 超频属性，Open|Close
         :type PathPrefix: String
         """
         self.HostId = None
         self.OverclockingAttribute = None
 
     def _deserialize(self, params):
         if params.get("HostId"):
```

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/iam/v20151101/client.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/iam/v20151101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/iam/v20151101/models.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/iam/v20151101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/kad/v20161122/client.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/kad/v20161122/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/kad/v20161122/models.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/kad/v20161122/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/kead/v20200101/client.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/kead/v20200101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/kead/v20200101/models.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/kead/v20200101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/kec/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/kec/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/kec/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/kec/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/mongodb/v20170101/client.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/mongodb/v20170101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/mongodb/v20170101/models.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/mongodb/v20170101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/resourcemanager/v20210320/client.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/resourcemanager/v20210320/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/resourcemanager/v20210320/models.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/resourcemanager/v20210320/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/sks/v20151101/client.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/sks/v20151101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/sks/v20151101/models.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/sks/v20151101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/slb/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/slb/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/slb/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/slb/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/slb/v20171210/client.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/slb/v20171210/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/slb/v20171210/models.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/slb/v20171210/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/sts/v20151101/client.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/sts/v20151101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/sts/v20151101/models.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/sts/v20151101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/tagv2/v20200901/client.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/tagv2/v20200901/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/tagv2/v20200901/models.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/tagv2/v20200901/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/trade/v20200114/client.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/trade/v20200114/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/trade/v20200831/client.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/trade/v20200831/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/trade/v20200831/models.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/trade/v20200831/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/vpc/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/vpc/v20160304/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1591,14 +1591,129 @@
         except Exception as e:
             if isinstance(e, KsyunSDKException):
                 raise
             else:
                 raise KsyunSDKException(e.message, e.message)
 
 
+    def CreateHaVip(self, request):
+        """创建HaVip
+        :param request: Request instance for CreateHaVip.
+        :type request: :class:`ksyun.client.vpc.v20160304.models.CreateHaVipRequest`
+        """
+        try:
+            params = request._serialize()
+            body = self.call("CreateHaVip", params)
+            response = json.loads(body)
+            if "Error" not in response:
+                return body
+            else:
+                code = response["Error"]["Code"]
+                message = response["Error"]["Message"]
+                req_id = response["RequestId"]
+                raise KsyunSDKException(code, message, req_id)
+        except Exception as e:
+            if isinstance(e, KsyunSDKException):
+                raise
+            else:
+                raise KsyunSDKException(e.message, e.message)
+
+
+    def DeleteHaVip(self, request):
+        """删除HaVip
+        :param request: Request instance for DeleteHaVip.
+        :type request: :class:`ksyun.client.vpc.v20160304.models.DeleteHaVipRequest`
+        """
+        try:
+            params = request._serialize()
+            body = self.call("DeleteHaVip", params)
+            response = json.loads(body)
+            if "Error" not in response:
+                return body
+            else:
+                code = response["Error"]["Code"]
+                message = response["Error"]["Message"]
+                req_id = response["RequestId"]
+                raise KsyunSDKException(code, message, req_id)
+        except Exception as e:
+            if isinstance(e, KsyunSDKException):
+                raise
+            else:
+                raise KsyunSDKException(e.message, e.message)
+
+
+    def AssociateHaVip(self, request):
+        """绑定HaVip
+        :param request: Request instance for AssociateHaVip.
+        :type request: :class:`ksyun.client.vpc.v20160304.models.AssociateHaVipRequest`
+        """
+        try:
+            params = request._serialize()
+            body = self.call("AssociateHaVip", params)
+            response = json.loads(body)
+            if "Error" not in response:
+                return body
+            else:
+                code = response["Error"]["Code"]
+                message = response["Error"]["Message"]
+                req_id = response["RequestId"]
+                raise KsyunSDKException(code, message, req_id)
+        except Exception as e:
+            if isinstance(e, KsyunSDKException):
+                raise
+            else:
+                raise KsyunSDKException(e.message, e.message)
+
+
+    def UnAssociateHaVip(self, request):
+        """解绑HaVip
+        :param request: Request instance for UnAssociateHaVip.
+        :type request: :class:`ksyun.client.vpc.v20160304.models.UnAssociateHaVipRequest`
+        """
+        try:
+            params = request._serialize()
+            body = self.call("UnAssociateHaVip", params)
+            response = json.loads(body)
+            if "Error" not in response:
+                return body
+            else:
+                code = response["Error"]["Code"]
+                message = response["Error"]["Message"]
+                req_id = response["RequestId"]
+                raise KsyunSDKException(code, message, req_id)
+        except Exception as e:
+            if isinstance(e, KsyunSDKException):
+                raise
+            else:
+                raise KsyunSDKException(e.message, e.message)
+
+
+    def DescribeHaVip(self, request):
+        """查询HaVip
+        :param request: Request instance for DescribeHaVip.
+        :type request: :class:`ksyun.client.vpc.v20160304.models.DescribeHaVipRequest`
+        """
+        try:
+            params = request._serialize()
+            body = self.call("DescribeHaVip", params)
+            response = json.loads(body)
+            if "Error" not in response:
+                return body
+            else:
+                code = response["Error"]["Code"]
+                message = response["Error"]["Message"]
+                req_id = response["RequestId"]
+                raise KsyunSDKException(code, message, req_id)
+        except Exception as e:
+            if isinstance(e, KsyunSDKException):
+                raise
+            else:
+                raise KsyunSDKException(e.message, e.message)
+
+
     def DeleteDirectConnectGatewayRoute(self, request):
         """删除边界网关路由
         :param request: Request instance for DeleteDirectConnectGatewayRoute.
         :type request: :class:`ksyun.client.vpc.v20160304.models.DeleteDirectConnectGatewayRouteRequest`
         """
         try:
             params = request._serialize()
```

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/client/vpc/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/client/vpc/v20160304/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1976,14 +1976,124 @@
     def _deserialize(self, params):
         if params.get("NetworkInterfaceName"):
             self.NetworkInterfaceName = params.get("NetworkInterfaceName")
         if params.get("NetworkInterfaceId"):
             self.NetworkInterfaceId = params.get("NetworkInterfaceId")
 
 
+class CreateHaVipRequest(AbstractModel):
+    """CreateHaVip请求参数结构体
+    """
+
+    def __init__(self):
+        r"""创建HaVip
+        :param SubnetId: 子网的ID
+        :type PathPrefix: String
+        :param IpAddress: 高可用虚拟IP的IP地址
+        :type PathPrefix: String
+        """
+        self.SubnetId = None
+        self.IpAddress = None
+
+    def _deserialize(self, params):
+        if params.get("SubnetId"):
+            self.SubnetId = params.get("SubnetId")
+        if params.get("IpAddress"):
+            self.IpAddress = params.get("IpAddress")
+
+
+class DeleteHaVipRequest(AbstractModel):
+    """DeleteHaVip请求参数结构体
+    """
+
+    def __init__(self):
+        r"""删除HaVip
+        :param HaVipId: 高可用虚拟IP的ID
+        :type PathPrefix: String
+        """
+        self.HaVipId = None
+
+    def _deserialize(self, params):
+        if params.get("HaVipId"):
+            self.HaVipId = params.get("HaVipId")
+
+
+class AssociateHaVipRequest(AbstractModel):
+    """AssociateHaVip请求参数结构体
+    """
+
+    def __init__(self):
+        r"""绑定HaVip
+        :param NetworkInterfaceId: 网卡的ID
+        :type PathPrefix: String
+        :param HaVipId: 高可用虚拟IP的ID
+        :type PathPrefix: String
+        """
+        self.NetworkInterfaceId = None
+        self.HaVipId = None
+
+    def _deserialize(self, params):
+        if params.get("NetworkInterfaceId"):
+            self.NetworkInterfaceId = params.get("NetworkInterfaceId")
+        if params.get("HaVipId"):
+            self.HaVipId = params.get("HaVipId")
+
+
+class UnAssociateHaVipRequest(AbstractModel):
+    """UnAssociateHaVip请求参数结构体
+    """
+
+    def __init__(self):
+        r"""解绑HaVip
+        :param NetworkInterfaceId: 网卡的ID
+        :type PathPrefix: String
+        :param HaVipId: 高可用虚拟IP的ID
+        :type PathPrefix: String
+        """
+        self.NetworkInterfaceId = None
+        self.HaVipId = None
+
+    def _deserialize(self, params):
+        if params.get("NetworkInterfaceId"):
+            self.NetworkInterfaceId = params.get("NetworkInterfaceId")
+        if params.get("HaVipId"):
+            self.HaVipId = params.get("HaVipId")
+
+
+class DescribeHaVipRequest(AbstractModel):
+    """DescribeHaVip请求参数结构体
+    """
+
+    def __init__(self):
+        r"""查询HaVip
+        :param HaVipId: 多个高可用虚拟IP的ID
+        :type PathPrefix: Filter
+        :param Filter: 筛选Filter
+        :type PathPrefix: Filter
+        :param MaxResults: 单次调用可返回的最大条目数量
+        :type PathPrefix: Int
+        :param NextToken: 获取另一页返回结果的 token.
+        :type PathPrefix: String
+        """
+        self.HaVipId = None
+        self.Filter = None
+        self.MaxResults = None
+        self.NextToken = None
+
+    def _deserialize(self, params):
+        if params.get("HaVipId"):
+            self.HaVipId = params.get("HaVipId")
+        if params.get("Filter"):
+            self.Filter = params.get("Filter")
+        if params.get("MaxResults"):
+            self.MaxResults = params.get("MaxResults")
+        if params.get("NextToken"):
+            self.NextToken = params.get("NextToken")
+
+
 class DeleteDirectConnectGatewayRouteRequest(AbstractModel):
     """DeleteDirectConnectGatewayRoute请求参数结构体
     """
 
     def __init__(self):
         r"""删除边界网关路由
         :param DirectConnectGatewayRouteId: 边界网关路由ID
```

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/common/abstract_client.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/common/abstract_client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/common/abstract_model.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/common/abstract_model.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/common/common_client.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/common/common_client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/common/credential.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/common/credential.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/common/exception/__init__.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/common/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/common/exception/ksyun_sdk_exception.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/common/exception/ksyun_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/common/http/request.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/common/http/request.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/common/profile/client_profile.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/common/profile/client_profile.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/common/profile/http_profile.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/common/profile/http_profile.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/ksyun/common/sign.py` & `kingsoftcloud-sdk-python-1.1.1/ksyun/common/sign.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.0/setup.py` & `kingsoftcloud-sdk-python-1.1.1/setup.py`

 * *Files identical despite different names*

