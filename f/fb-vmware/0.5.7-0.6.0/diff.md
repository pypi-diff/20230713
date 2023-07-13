# Comparing `tmp/fb_vmware-0.5.7.tar.gz` & `tmp/fb_vmware-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fb_vmware-0.5.7.tar", last modified: Mon Jan  2 08:36:08 2023, max compression
+gzip compressed data, was "fb_vmware-0.6.0.tar", last modified: Thu Jul 13 15:56:10 2023, max compression
```

## Comparing `fb_vmware-0.5.7.tar` & `fb_vmware-0.6.0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 08:36:08.250125 fb_vmware-0.5.7/
--rw-r--r--   0 root         (0) root         (0)     7652 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       52 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1258 2023-01-02 08:36:08.250125 fb_vmware-0.5.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       93 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 08:36:08.242124 fb_vmware-0.5.7/bin/
--rwxr-xr-x   0 root         (0) root         (0)     1596 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/bin/get-vsphere-host-list
--rwxr-xr-x   0 root         (0) root         (0)     1580 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/bin/get-vsphere-vm-info
--rwxr-xr-x   0 root         (0) root         (0)     1588 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/bin/get-vsphere-vm-list
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 08:36:08.242124 fb_vmware-0.5.7/lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 08:36:08.246125 fb_vmware-0.5.7/lib/fb_vmware/
--rw-r--r--   0 root         (0) root         (0)     2790 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/lib/fb_vmware/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10932 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/lib/fb_vmware/about.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 08:36:08.246125 fb_vmware-0.5.7/lib/fb_vmware/app/
--rw-r--r--   0 root         (0) root         (0)     7653 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/lib/fb_vmware/app/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12389 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/lib/fb_vmware/app/get_host_list.py
--rw-r--r--   0 root         (0) root         (0)    10100 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/lib/fb_vmware/app/get_vm_info.py
--rw-r--r--   0 root         (0) root         (0)    17386 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/lib/fb_vmware/app/get_vm_list.py
--rw-r--r--   0 root         (0) root         (0)     7780 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/lib/fb_vmware/base.py
--rw-r--r--   0 root         (0) root         (0)    13270 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/lib/fb_vmware/cluster.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 08:36:08.246125 fb_vmware-0.5.7/lib/fb_vmware/config/
--rw-r--r--   0 root         (0) root         (0)    15942 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/lib/fb_vmware/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53902 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/lib/fb_vmware/connect.py
--rw-r--r--   0 root         (0) root         (0)    17452 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/lib/fb_vmware/controller.py
--rw-r--r--   0 root         (0) root         (0)    22287 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/lib/fb_vmware/datastore.py
--rw-r--r--   0 root         (0) root         (0)     8372 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/lib/fb_vmware/dc.py
--rw-r--r--   0 root         (0) root         (0)    19810 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/lib/fb_vmware/disk.py
--rw-r--r--   0 root         (0) root         (0)    15185 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/lib/fb_vmware/ds_cluster.py
--rw-r--r--   0 root         (0) root         (0)     8734 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/lib/fb_vmware/errors.py
--rw-r--r--   0 root         (0) root         (0)    24549 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/lib/fb_vmware/ether.py
--rw-r--r--   0 root         (0) root         (0)    30946 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/lib/fb_vmware/host.py
--rw-r--r--   0 root         (0) root         (0)    14668 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/lib/fb_vmware/host_port_group.py
--rw-r--r--   0 root         (0) root         (0)     5256 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/lib/fb_vmware/iface.py
--rw-r--r--   0 root         (0) root         (0)      459 2023-01-02 08:36:08.000000 fb_vmware-0.5.7/lib/fb_vmware/local_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 08:36:08.242124 fb_vmware-0.5.7/lib/fb_vmware/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 08:36:08.242124 fb_vmware-0.5.7/lib/fb_vmware/locale/de_DE/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 08:36:08.246125 fb_vmware-0.5.7/lib/fb_vmware/locale/de_DE/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)    27418 2023-01-02 08:36:06.000000 fb_vmware-0.5.7/lib/fb_vmware/locale/de_DE/LC_MESSAGES/fb_vmware.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 08:36:08.242124 fb_vmware-0.5.7/lib/fb_vmware/locale/en_US/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 08:36:08.246125 fb_vmware-0.5.7/lib/fb_vmware/locale/en_US/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     4398 2023-01-02 08:36:06.000000 fb_vmware-0.5.7/lib/fb_vmware/locale/en_US/LC_MESSAGES/fb_vmware.mo
--rw-r--r--   0 root         (0) root         (0)    16768 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/lib/fb_vmware/network.py
--rw-r--r--   0 root         (0) root         (0)     9511 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/lib/fb_vmware/obj.py
--rw-r--r--   0 root         (0) root         (0)     2575 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/lib/fb_vmware/spinner.py
--rw-r--r--   0 root         (0) root         (0)    28605 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/lib/fb_vmware/vm.py
--rw-r--r--   0 root         (0) root         (0)     3157 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/lib/fb_vmware/xlate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 08:36:08.246125 fb_vmware-0.5.7/lib/fb_vmware.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1258 2023-01-02 08:36:08.000000 fb_vmware-0.5.7/lib/fb_vmware.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1528 2023-01-02 08:36:08.000000 fb_vmware-0.5.7/lib/fb_vmware.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-02 08:36:08.000000 fb_vmware-0.5.7/lib/fb_vmware.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-01-02 08:36:08.000000 fb_vmware-0.5.7/lib/fb_vmware.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-01-02 08:36:08.000000 fb_vmware-0.5.7/lib/fb_vmware.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1246 2023-01-02 08:36:08.250125 fb_vmware-0.5.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6537 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 08:36:08.250125 fb_vmware-0.5.7/test/
--rw-r--r--   0 root         (0) root         (0)     3583 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/test/general.py
--rwxr-xr-x   0 root         (0) root         (0)     9433 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/test/test_00-errors.py
--rwxr-xr-x   0 root         (0) root         (0)     4172 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/test/test_10-base.py
--rwxr-xr-x   0 root         (0) root         (0)     2819 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/test/test_20-obj.py
--rwxr-xr-x   0 root         (0) root         (0)     4644 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/test/test_31_about_info.py
--rwxr-xr-x   0 root         (0) root         (0)     5139 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/test/test_32_cluster.py
--rwxr-xr-x   0 root         (0) root         (0)     4866 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/test/test_33_dc.py
--rwxr-xr-x   0 root         (0) root         (0)     2749 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/test/test_34_disk.py
--rwxr-xr-x   0 root         (0) root         (0)     3297 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/test/test_35_datastore.py
--rwxr-xr-x   0 root         (0) root         (0)     3372 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/test/test_36_ds_cluster.py
--rwxr-xr-x   0 root         (0) root         (0)     2767 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/test/test_37_ether.py
--rwxr-xr-x   0 root         (0) root         (0)     2817 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/test/test_38_iface.py
--rwxr-xr-x   0 root         (0) root         (0)     4523 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/test/test_39_network.py
--rwxr-xr-x   0 root         (0) root         (0)     2847 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/test/test_40_controller.py
--rwxr-xr-x   0 root         (0) root         (0)     2866 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/test/test_41_host_port_group.py
--rwxr-xr-x   0 root         (0) root         (0)     3097 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/test/test_50_host.py
--rwxr-xr-x   0 root         (0) root         (0)     3039 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/test/test_55_vm.py
--rwxr-xr-x   0 root         (0) root         (0)     3539 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/test/test_60_config.py
--rwxr-xr-x   0 root         (0) root         (0)     3211 2023-01-02 08:35:43.000000 fb_vmware-0.5.7/test/test_70_connect.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 15:56:10.707183 fb_vmware-0.6.0/
+-rw-r--r--   0 root         (0) root         (0)     7652 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       52 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1258 2023-07-13 15:56:10.707183 fb_vmware-0.6.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       93 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 15:56:10.699182 fb_vmware-0.6.0/bin/
+-rwxr-xr-x   0 root         (0) root         (0)     2012 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/bin/get-vsphere-host-list
+-rwxr-xr-x   0 root         (0) root         (0)     1981 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/bin/get-vsphere-vm-info
+-rwxr-xr-x   0 root         (0) root         (0)     1986 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/bin/get-vsphere-vm-list
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 15:56:10.699182 fb_vmware-0.6.0/lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 15:56:10.703183 fb_vmware-0.6.0/lib/fb_vmware/
+-rw-r--r--   0 root         (0) root         (0)     2146 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/lib/fb_vmware/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11253 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/lib/fb_vmware/about.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 15:56:10.703183 fb_vmware-0.6.0/lib/fb_vmware/app/
+-rw-r--r--   0 root         (0) root         (0)     7891 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/lib/fb_vmware/app/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12757 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/lib/fb_vmware/app/get_host_list.py
+-rw-r--r--   0 root         (0) root         (0)    10223 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/lib/fb_vmware/app/get_vm_info.py
+-rw-r--r--   0 root         (0) root         (0)    17673 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/lib/fb_vmware/app/get_vm_list.py
+-rw-r--r--   0 root         (0) root         (0)     8159 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/lib/fb_vmware/base.py
+-rw-r--r--   0 root         (0) root         (0)    13594 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/lib/fb_vmware/cluster.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 15:56:10.703183 fb_vmware-0.6.0/lib/fb_vmware/config/
+-rw-r--r--   0 root         (0) root         (0)    16498 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/lib/fb_vmware/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    55516 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/lib/fb_vmware/connect.py
+-rw-r--r--   0 root         (0) root         (0)    18764 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/lib/fb_vmware/controller.py
+-rw-r--r--   0 root         (0) root         (0)    24206 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/lib/fb_vmware/datastore.py
+-rw-r--r--   0 root         (0) root         (0)     8675 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/lib/fb_vmware/dc.py
+-rw-r--r--   0 root         (0) root         (0)    20969 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/lib/fb_vmware/disk.py
+-rw-r--r--   0 root         (0) root         (0)    17073 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/lib/fb_vmware/ds_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     9993 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/lib/fb_vmware/errors.py
+-rw-r--r--   0 root         (0) root         (0)    25970 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/lib/fb_vmware/ether.py
+-rw-r--r--   0 root         (0) root         (0)    32498 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/lib/fb_vmware/host.py
+-rw-r--r--   0 root         (0) root         (0)    15962 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/lib/fb_vmware/host_port_group.py
+-rw-r--r--   0 root         (0) root         (0)     5422 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/lib/fb_vmware/iface.py
+-rw-r--r--   0 root         (0) root         (0)      474 2023-07-13 15:56:10.000000 fb_vmware-0.6.0/lib/fb_vmware/local_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 15:56:10.699182 fb_vmware-0.6.0/lib/fb_vmware/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 15:56:10.699182 fb_vmware-0.6.0/lib/fb_vmware/locale/de_DE/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 15:56:10.703183 fb_vmware-0.6.0/lib/fb_vmware/locale/de_DE/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)    27481 2023-07-13 15:56:09.000000 fb_vmware-0.6.0/lib/fb_vmware/locale/de_DE/LC_MESSAGES/fb_vmware.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 15:56:10.699182 fb_vmware-0.6.0/lib/fb_vmware/locale/en_US/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 15:56:10.703183 fb_vmware-0.6.0/lib/fb_vmware/locale/en_US/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     4481 2023-07-13 15:56:09.000000 fb_vmware-0.6.0/lib/fb_vmware/locale/en_US/LC_MESSAGES/fb_vmware.mo
+-rw-r--r--   0 root         (0) root         (0)    18889 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/lib/fb_vmware/network.py
+-rw-r--r--   0 root         (0) root         (0)    10021 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/lib/fb_vmware/obj.py
+-rw-r--r--   0 root         (0) root         (0)     3726 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/lib/fb_vmware/spinner.py
+-rw-r--r--   0 root         (0) root         (0)    29777 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/lib/fb_vmware/vm.py
+-rw-r--r--   0 root         (0) root         (0)     3161 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/lib/fb_vmware/xlate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 15:56:10.703183 fb_vmware-0.6.0/lib/fb_vmware.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1258 2023-07-13 15:56:10.000000 fb_vmware-0.6.0/lib/fb_vmware.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1528 2023-07-13 15:56:10.000000 fb_vmware-0.6.0/lib/fb_vmware.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 15:56:10.000000 fb_vmware-0.6.0/lib/fb_vmware.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-07-13 15:56:10.000000 fb_vmware-0.6.0/lib/fb_vmware.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-13 15:56:10.000000 fb_vmware-0.6.0/lib/fb_vmware.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1251 2023-07-13 15:56:10.707183 fb_vmware-0.6.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     6975 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 15:56:10.707183 fb_vmware-0.6.0/test/
+-rw-r--r--   0 root         (0) root         (0)     3583 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/test/general.py
+-rwxr-xr-x   0 root         (0) root         (0)     9433 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/test/test_00-errors.py
+-rwxr-xr-x   0 root         (0) root         (0)     4172 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/test/test_10-base.py
+-rwxr-xr-x   0 root         (0) root         (0)     2819 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/test/test_20-obj.py
+-rwxr-xr-x   0 root         (0) root         (0)     4644 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/test/test_31_about_info.py
+-rwxr-xr-x   0 root         (0) root         (0)     5139 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/test/test_32_cluster.py
+-rwxr-xr-x   0 root         (0) root         (0)     4866 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/test/test_33_dc.py
+-rwxr-xr-x   0 root         (0) root         (0)     2749 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/test/test_34_disk.py
+-rwxr-xr-x   0 root         (0) root         (0)     3297 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/test/test_35_datastore.py
+-rwxr-xr-x   0 root         (0) root         (0)     3372 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/test/test_36_ds_cluster.py
+-rwxr-xr-x   0 root         (0) root         (0)     2767 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/test/test_37_ether.py
+-rwxr-xr-x   0 root         (0) root         (0)     2817 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/test/test_38_iface.py
+-rwxr-xr-x   0 root         (0) root         (0)     4523 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/test/test_39_network.py
+-rwxr-xr-x   0 root         (0) root         (0)     2847 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/test/test_40_controller.py
+-rwxr-xr-x   0 root         (0) root         (0)     2866 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/test/test_41_host_port_group.py
+-rwxr-xr-x   0 root         (0) root         (0)     3097 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/test/test_50_host.py
+-rwxr-xr-x   0 root         (0) root         (0)     3039 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/test/test_55_vm.py
+-rwxr-xr-x   0 root         (0) root         (0)     3539 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/test/test_60_config.py
+-rwxr-xr-x   0 root         (0) root         (0)     3211 2023-07-13 15:55:43.000000 fb_vmware-0.6.0/test/test_70_connect.py
```

### Comparing `fb_vmware-0.5.7/LICENSE` & `fb_vmware-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fb_vmware-0.5.7/PKG-INFO` & `fb_vmware-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fb_vmware
-Version: 0.5.7
+Version: 0.6.0
 Summary: A wrapper module around the pyvmomi module to simplify work and handling.
 Home-page: https://github.com/fbrehm/fb-vmware
 Author: Frank Brehm
 Author-email: frank@brehm-online.com
 License: LGPL3+
 Platform: posix
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `fb_vmware-0.5.7/bin/get-vsphere-host-list` & `fb_vmware-0.6.0/bin/get-vsphere-vm-info`

 * *Files 15% similar despite different names*

```diff
@@ -1,59 +1,71 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+"""
+@summary: Print information about a particular VM in VMWare VSphere.
+
+@author: Frank Brehm
+@contact: frank@brehm-online.com
+@copyright: © 2023 by Frank Brehm, Berlin
+"""
 
 from __future__ import print_function
 
+import locale
+import os
 import sys
 
-if sys.version_info[0] != 3:
-    print("This script is intended to use with Python3.", file=sys.stderr)
-    print("You are using Python: {0}.{1}.{2}-{3}-{4}.\n".format(
+MIN_PYTHON_MAJOR = 3
+MIN_PYTHON_MINOR = 6
+
+if sys.version_info[0] != MIN_PYTHON_MAJOR:
+    print(
+        'This script is intended to use with Python{}.'.format(MIN_PYTHON_MAJOR), file=sys.stderr)
+    print('You are using Python: {0}.{1}.{2}-{3}-{4}.\n'.format(
         *sys.version_info), file=sys.stderr)
     sys.exit(1)
 
-if sys.version_info[1] < 4:
-    print("A minimal Python version of 3.4 is necessary to execute this script.", file=sys.stderr)
-    print("You are using Python: {0}.{1}.{2}-{3}-{4}.\n".format(
+if sys.version_info[0] == MIN_PYTHON_MAJOR and sys.version_info[1] < MIN_PYTHON_MINOR:
+    print(
+        'A minimal Python version of {}.{} is necessary to execute this script.'.format(
+            MIN_PYTHON_MAJOR, MIN_PYTHON_MINOR), file=sys.stderr)
+    print('You are using Python: {0}.{1}.{2}-{3}-{4}.\n'.format(
         *sys.version_info), file=sys.stderr)
     sys.exit(1)
 
-import os
-import logging
-import locale
-
 # own modules:
 cur_dir = os.getcwd()
 base_dir = cur_dir
 
 if sys.argv[0] != '' and sys.argv[0] != '-c':
     bin_dir = os.path.dirname(os.path.realpath(sys.argv[0]))
 else:
     bin_dir = os.path.dirname(os.path.realpath(__file__))
 base_dir = os.path.abspath(os.path.join(bin_dir, '..'))
 lib_dir = os.path.join(base_dir, 'lib')
 module_dir = os.path.join(lib_dir, 'fb_vmware')
 if os.path.exists(module_dir):
     sys.path.insert(0, lib_dir)
 
-from fb_vmware.app.get_host_list import GetHostsListApplication
+from fb_vmware.app.get_vm_info import GetVmApplication
+from fb_vmware.xlate import XLATOR
 
-log = logging.getLogger(__name__)
+_ = XLATOR.gettext
 
 __author__ = 'Frank Brehm <frank@brehm-online.com>'
-__copyright__ = '(C) 2022 by Frank Brehm, Berlin'
+__copyright__ = '(C) 2023 by Frank Brehm, Berlin'
 
 appname = os.path.basename(sys.argv[0])
 
 locale.setlocale(locale.LC_ALL, '')
 
-app = GetHostsListApplication(appname=appname, base_dir=base_dir)
+app = GetVmApplication(appname=appname, base_dir=base_dir)
 app.initialized = True
 
 if app.verbose > 2:
-    print("{c}-Object:\n{a}".format(c=app.__class__.__name__, a=app))
+    print(_('{c}-Object:\n{a}').format(c=app.__class__.__name__, a=app))
 
 app()
 
 sys.exit(0)
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fb_vmware-0.5.7/bin/get-vsphere-vm-info` & `fb_vmware-0.6.0/bin/get-vsphere-vm-list`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,71 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+"""
+@summary: Print a list of all virtual machines in VMWare VSphere.
+
+@author: Frank Brehm
+@contact: frank@brehm-online.com
+@copyright: © 2023 by Frank Brehm, Berlin
+"""
 
 from __future__ import print_function
 
+import locale
+import os
 import sys
 
-if sys.version_info[0] != 3:
-    print("This script is intended to use with Python3.", file=sys.stderr)
-    print("You are using Python: {0}.{1}.{2}-{3}-{4}.\n".format(
+MIN_PYTHON_MAJOR = 3
+MIN_PYTHON_MINOR = 6
+
+if sys.version_info[0] != MIN_PYTHON_MAJOR:
+    print(
+        'This script is intended to use with Python{}.'.format(MIN_PYTHON_MAJOR), file=sys.stderr)
+    print('You are using Python: {0}.{1}.{2}-{3}-{4}.\n'.format(
         *sys.version_info), file=sys.stderr)
     sys.exit(1)
 
-if sys.version_info[1] < 4:
-    print("A minimal Python version of 3.4 is necessary to execute this script.", file=sys.stderr)
-    print("You are using Python: {0}.{1}.{2}-{3}-{4}.\n".format(
+if sys.version_info[0] == MIN_PYTHON_MAJOR and sys.version_info[1] < MIN_PYTHON_MINOR:
+    print(
+        'A minimal Python version of {}.{} is necessary to execute this script.'.format(
+            MIN_PYTHON_MAJOR, MIN_PYTHON_MINOR), file=sys.stderr)
+    print('You are using Python: {0}.{1}.{2}-{3}-{4}.\n'.format(
         *sys.version_info), file=sys.stderr)
     sys.exit(1)
 
-import os
-import logging
-import locale
-
 # own modules:
 cur_dir = os.getcwd()
 base_dir = cur_dir
 
 if sys.argv[0] != '' and sys.argv[0] != '-c':
     bin_dir = os.path.dirname(os.path.realpath(sys.argv[0]))
 else:
     bin_dir = os.path.dirname(os.path.realpath(__file__))
 base_dir = os.path.abspath(os.path.join(bin_dir, '..'))
 lib_dir = os.path.join(base_dir, 'lib')
 module_dir = os.path.join(lib_dir, 'fb_vmware')
 if os.path.exists(module_dir):
     sys.path.insert(0, lib_dir)
 
-from fb_vmware.app.get_vm_info import GetVmApplication
+from fb_vmware.app.get_vm_list import GetVmListApplication
+from fb_vmware.xlate import XLATOR
 
-log = logging.getLogger(__name__)
+_ = XLATOR.gettext
 
 __author__ = 'Frank Brehm <frank@brehm-online.com>'
-__copyright__ = '(C) 2022 by Frank Brehm, Berlin'
+__copyright__ = '(C) 2023 by Frank Brehm, Berlin'
 
 appname = os.path.basename(sys.argv[0])
 
 locale.setlocale(locale.LC_ALL, '')
 
-app = GetVmApplication(appname=appname, base_dir=base_dir)
+app = GetVmListApplication(appname=appname, base_dir=base_dir)
 app.initialized = True
 
 if app.verbose > 2:
-    print("{c}-Object:\n{a}".format(c=app.__class__.__name__, a=app))
+    print(_('{c}-Object:\n{a}').format(c=app.__class__.__name__, a=app))
 
 app()
 
 sys.exit(0)
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fb_vmware-0.5.7/bin/get-vsphere-vm-list` & `fb_vmware-0.6.0/bin/get-vsphere-host-list`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,71 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+"""
+@summary: An application to print a list of all physical hosts in a VMWare VSphere.
+
+@author: Frank Brehm
+@contact: frank@brehm-online.com
+@copyright: © 2023 by Frank Brehm, Berlin
+"""
 
 from __future__ import print_function
 
+import locale
+import os
 import sys
 
-if sys.version_info[0] != 3:
-    print("This script is intended to use with Python3.", file=sys.stderr)
-    print("You are using Python: {0}.{1}.{2}-{3}-{4}.\n".format(
+MIN_PYTHON_MAJOR = 3
+MIN_PYTHON_MINOR = 6
+
+if sys.version_info[0] != MIN_PYTHON_MAJOR:
+    print(
+        'This script is intended to use with Python{}.'.format(MIN_PYTHON_MAJOR), file=sys.stderr)
+    print('You are using Python: {0}.{1}.{2}-{3}-{4}.\n'.format(
         *sys.version_info), file=sys.stderr)
     sys.exit(1)
 
-if sys.version_info[1] < 4:
-    print("A minimal Python version of 3.4 is necessary to execute this script.", file=sys.stderr)
-    print("You are using Python: {0}.{1}.{2}-{3}-{4}.\n".format(
+if sys.version_info[0] == MIN_PYTHON_MAJOR and sys.version_info[1] < MIN_PYTHON_MINOR:
+    print(
+        'A minimal Python version of {}.{} is necessary to execute this script.'.format(
+            MIN_PYTHON_MAJOR, MIN_PYTHON_MINOR), file=sys.stderr)
+    print('You are using Python: {0}.{1}.{2}-{3}-{4}.\n'.format(
         *sys.version_info), file=sys.stderr)
     sys.exit(1)
 
-import os
-import logging
-import locale
-
 # own modules:
 cur_dir = os.getcwd()
 base_dir = cur_dir
 
 if sys.argv[0] != '' and sys.argv[0] != '-c':
     bin_dir = os.path.dirname(os.path.realpath(sys.argv[0]))
 else:
     bin_dir = os.path.dirname(os.path.realpath(__file__))
 base_dir = os.path.abspath(os.path.join(bin_dir, '..'))
 lib_dir = os.path.join(base_dir, 'lib')
 module_dir = os.path.join(lib_dir, 'fb_vmware')
 if os.path.exists(module_dir):
     sys.path.insert(0, lib_dir)
 
-from fb_vmware.app.get_vm_list import GetVmListApplication
+from fb_vmware.app.get_host_list import GetHostsListApplication
+from fb_vmware.xlate import XLATOR
 
-log = logging.getLogger(__name__)
+_ = XLATOR.gettext
 
 __author__ = 'Frank Brehm <frank@brehm-online.com>'
-__copyright__ = '(C) 2022 by Frank Brehm, Berlin'
+__copyright__ = '(C) 2023 by Frank Brehm, Berlin'
 
 appname = os.path.basename(sys.argv[0])
 
 locale.setlocale(locale.LC_ALL, '')
 
-app = GetVmListApplication(appname=appname, base_dir=base_dir)
+app = GetHostsListApplication(appname=appname, base_dir=base_dir)
 app.initialized = True
 
 if app.verbose > 2:
-    print("{c}-Object:\n{a}".format(c=app.__class__.__name__, a=app))
+    print(_('{c}-Object:\n{a}').format(c=app.__class__.__name__, a=app))
 
 app()
 
 sys.exit(0)
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fb_vmware-0.5.7/lib/fb_vmware/about.py` & `fb_vmware-0.6.0/lib/fb_vmware/about.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
+@summary: The module for capsulating a VSphere about info object.
+
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 by Frank Brehm, Berlin
-@summary: The module for capsulating a VSphere about info object.
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
 import logging
 import uuid
 
 
 # Third party modules
-from pyVmomi import vim
-
 from fb_tools.common import pp
 from fb_tools.obj import FbBaseObject
 from fb_tools.xlate import format_list
 
+from pyVmomi import vim
+
 # Own modules
 from .xlate import XLATOR
 
-__version__ = '0.3.3'
+__version__ = '0.3.4'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 
 
 # =============================================================================
 class VsphereAboutInfo(FbBaseObject):
+    """This is a wrapper for the about-information of a VMWare-VSphere center."""
 
     # -------------------------------------------------------------------------
     def __init__(
             self, appname=None, verbose=0, version=__version__, base_dir=None, initialized=None):
-
+        """Initialize the VsphereAboutInfo object."""
         self._api_type = None
         self._api_version = None
         self._name = None
         self._full_name = None
         self._vendor = None
         self._os_version = None
         self._os_type = None
@@ -236,23 +238,22 @@
             self._lic_prodversion = None
         else:
             self._lic_prodversion = v
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True):
         """
-        Transforms the elements of the object into a dict
+        Transform the elements of the object into a dict.
 
         @param short: don't include local properties in resulting dict.
         @type short: bool
 
         @return: structure as dict
         @rtype:  dict
         """
-
         res = super(VsphereAboutInfo, self).as_dict(short=short)
         res['api_type'] = self.api_type
         res['api_version'] = self.api_version
         res['name'] = self.name
         res['full_name'] = self.full_name
         res['vendor'] = self.vendor
         res['os_version'] = self.os_version
@@ -262,49 +263,49 @@
         res['lic_prodversion'] = self.lic_prodversion
 
         return res
 
     # -------------------------------------------------------------------------
     @classmethod
     def from_summary(cls, data, appname=None, verbose=0, base_dir=None, test_mode=False):
-
+        """Create a new VsphereAboutInfo object based on the data given from pyvmomi module."""
         if test_mode:
 
             necessary_fields = (
                 'apiType', 'apiVersion', 'name', 'fullName', 'vendor', 'version',
                 'osType', 'instanceUuid', 'licenseProductName', 'licenseProductVersion')
             failing_fields = []
 
             for field in necessary_fields:
                 if not hasattr(data, field):
                     failing_fields.append(field)
 
             if len(failing_fields):
                 msg = _(
-                    "The given parameter {p!r} on calling method {m}() has failing "
-                    "attributes").format(p='data', m='from_summary')
+                    'The given parameter {p!r} on calling method {m}() has failing '
+                    'attributes').format(p='data', m='from_summary')
                 msg += ': ' + format_list(failing_fields, do_repr=True)
                 raise AssertionError(msg)
 
         else:
             if not isinstance(data, vim.AboutInfo):
                 msg = _(
-                    "Parameter {t!r} must be a {e} object, a {v} object was given "
-                    "instead.").format(t='data', e='vim.AboutInfo', v=data.__class__.__qualname__)
+                    'Parameter {t!r} must be a {e} object, a {v} object was given '
+                    'instead.').format(t='data', e='vim.AboutInfo', v=data.__class__.__qualname__)
                 raise TypeError(msg)
 
         params = {
             'appname': appname,
             'verbose': verbose,
             'base_dir': base_dir,
             'initialized': False,
         }
 
         if verbose > 2:
-            LOG.debug(_("Creating {} object from:").format(cls.__name__) + '\n' + pp(params))
+            LOG.debug(_('Creating {} object from:').format(cls.__name__) + '\n' + pp(params))
         info = cls(**params)
 
 #        'about': (vim.AboutInfo) {
 #               dynamicType = <unset>,
 #               dynamicProperty = (vmodl.DynamicProperty) [],
 #               name = 'VMware vCenter Server',
 #               fullName = 'VMware vCenter Server 6.5.0 build-8024368',
@@ -332,21 +333,21 @@
         info.instance_uuid = data.instanceUuid
         info.lic_prodname = data.licenseProductName
         info.lic_prodversion = data.licenseProductVersion
 
         info.initialized = True
 
         if verbose > 2:
-            LOG.debug(_("Created {} object:").format(cls.__name__) + '\n' + pp(info.as_dict()))
+            LOG.debug(_('Created {} object:').format(cls.__name__) + '\n' + pp(info.as_dict()))
 
         return info
 
     # -------------------------------------------------------------------------
     def __copy__(self):
-
+        """Return a new VsphereAboutInfo object with data from current object copied in."""
         info = VsphereAboutInfo(
             appname=self.appname, verbose=self.verbose, base_dir=self.base_dir,
             initialized=False)
 
         info.api_type = self.api_type
         info.api_version = self.api_version
         info.name = self.name
@@ -360,14 +361,14 @@
 
         info.initialized = self.initialized
 
         return info
 
 
 # =============================================================================
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_vmware-0.5.7/lib/fb_vmware/app/__init__.py` & `fb_vmware-0.6.0/lib/fb_vmware/app/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,70 +1,66 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
+@summary: A base module for all VMWare/VSPhere application classes.
+
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 by Frank Brehm, Berlin
-@summary: A base module for all VMWare/VSPhere application classes
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import, print_function
 
 # Standard modules
-import logging
-import getpass
 import copy
+import getpass
+import logging
 
 # Third party modules
-import pytz
-
-from fb_tools.common import pp
 from fb_tools.cfg_app import FbConfigApplication
+from fb_tools.common import pp
 from fb_tools.errors import FbAppError
 from fb_tools.multi_config import DEFAULT_ENCODING
 
+import pytz
+
 # Own modules
 from .. import __version__ as GLOBAL_VERSION
-
-from ..xlate import XLATOR
-
 from ..config import VmwareConfiguration
-
 from ..connect import VsphereConnection
-
 from ..errors import VSphereExpectedError
+from ..xlate import XLATOR
 
-__version__ = '0.2.1'
+__version__ = '0.2.2'
 LOG = logging.getLogger(__name__)
 TZ = pytz.timezone('Europe/Berlin')
 
 _ = XLATOR.gettext
 ngettext = XLATOR.ngettext
 
 
 # =============================================================================
 class VmwareAppError(FbAppError):
-    """ Base exception class for all exceptions in all VMWare/VSPhere application classes."""
+    """Base exception class for all exceptions in all VMWare/VSPhere application classes."""
+
     pass
 
 
 # =============================================================================
 class BaseVmwareApplication(FbConfigApplication):
-    """
-    Base class for all VMWare/VSPhere application classes.
-    """
+    """Base class for all VMWare/VSPhere application classes."""
 
     # -------------------------------------------------------------------------
     def __init__(
         self, appname=None, verbose=0, version=GLOBAL_VERSION, base_dir=None,
             cfg_class=VmwareConfiguration, initialized=False, usage=None, description=None,
             argparse_epilog=None, argparse_prefix_chars='-', env_prefix=None,
             append_appname_to_stems=True, config_dir=None, additional_stems=None,
             additional_cfgdirs=None, cfg_encoding=DEFAULT_ENCODING,
             use_chardet=True):
-
+        """Initialize a BaseVmwareApplication object."""
         self.req_vspheres = None
         self.do_vspheres = []
 
         # Hash with all VSphere handler objects
         self.vsphere = {}
 
         super(BaseVmwareApplication, self).__init__(
@@ -73,54 +69,52 @@
             append_appname_to_stems=append_appname_to_stems, config_dir=config_dir,
             additional_stems=additional_stems, additional_cfgdirs=additional_cfgdirs,
             cfg_encoding=cfg_encoding, use_chardet=use_chardet, initialized=False,
         )
 
     # -------------------------------------------------------------------------
     def __del__(self):
-        """Cleaning up in emergency case."""
-
+        """Clean up in emergency case."""
         if self.vsphere.keys():
             self.cleaning_up()
 
     # -------------------------------------------------------------------------
     def post_init(self):
         """
-        Method to execute before calling run(). Here could be done some
-        finishing actions after reading in commandline parameters,
-        configuration a.s.o.
+        Execute some things before calling run().
+
+        Here could be done some finishing actions after reading in commandline
+        parameters, configuration a.s.o.
 
         This method could be overwritten by descendant classes, these
         methhods should allways include a call to post_init() of the
         parent class.
-
         """
-
         self.initialized = False
 
         super(BaseVmwareApplication, self).post_init()
 
         if self.verbose > 2:
-            LOG.debug(_("{what} of {app} ..").format(what='post_init()', app=self.appname))
+            LOG.debug(_('{what} of {app} ...').format(what='post_init()', app=self.appname))
 
         if not self.cfg.vsphere.keys():
-            msg = _("Did not found any configured Vsphere environments.")
+            msg = _('Did not found any configured Vsphere environments.')
             LOG.error(msg)
             self.exit(3)
 
         if self.args.req_vsphere:
             self.req_vspheres = []
             all_found = True
             for vs_name in self.args.req_vsphere:
-                LOG.debug(_("Checking for configured VSPhere instance {!r} ...").format(vs_name))
+                LOG.debug(_('Checking for configured VSPhere instance {!r} ...').format(vs_name))
                 vs = vs_name.strip().lower()
                 if vs not in self.cfg.vsphere.keys():
                     all_found = False
                     msg = _(
-                        "VSPhere {!r} not found in list of configured VSPhere instances.").format(
+                        'VSPhere {!r} not found in list of configured VSPhere instances.').format(
                             vs_name)
                     LOG.error(msg)
                 else:
                     if vs not in self.req_vspheres:
                         self.req_vspheres.append(vs)
             if not all_found:
                 self.exit(1)
@@ -139,79 +133,76 @@
                         n=vsphere_name, u=vsphere_data.user, h=vsphere_data.host)) + ' '
                 vsphere_data.password = getpass.getpass(prompt=prompt)
 
         self.init_vsphere_handlers()
 
     # -------------------------------------------------------------------------
     def init_arg_parser(self):
-        """
-        Public available method to initiate the argument parser.
-        """
-
+        """Initiate the argument parser."""
         super(BaseVmwareApplication, self).init_arg_parser()
 
         self.arg_parser.add_argument(
             '--vs', '--vsphere', dest='req_vsphere', nargs='*',
             help=_(
-                "The VSPhere names from configuration, in which the VMs should be searched.")
+                'The VSPhere names from configuration, in which the VMs should be searched.')
         )
 
     # -------------------------------------------------------------------------
     def perform_arg_parser(self):
-
+        """Evaluate the command line parameters. Maybe overridden."""
         if self.verbose > 2:
-            LOG.debug(_("Got command line arguments:") + '\n' + pp(self.args))
+            LOG.debug(_('Got command line arguments:') + '\n' + pp(self.args))
 
     # -------------------------------------------------------------------------
     def init_vsphere_handlers(self):
-
+        """Initialize all VSphere handlers."""
         if self.verbose > 1:
-            LOG.debug(_("Initializing VSphere handlers ..."))
+            LOG.debug(_('Initializing VSphere handlers ...'))
 
         try:
             for vsphere_name in self.do_vspheres:
                 self.init_vsphere_handler(vsphere_name)
         except VSphereExpectedError as e:
             LOG.error(str(e))
             self.exit(7)
 
     # -------------------------------------------------------------------------
     def init_vsphere_handler(self, vsphere_name):
-
+        """Initialize the given VSphere handler."""
         if self.verbose > 2:
-            LOG.debug(_("Initializing handler for VSPhere {!r} ...").format(vsphere_name))
+            LOG.debug(_('Initializing handler for VSPhere {!r} ...').format(vsphere_name))
 
         vsphere_data = self.cfg.vsphere[vsphere_name]
 
         vsphere = VsphereConnection(
             vsphere_data, auto_close=True, simulate=self.simulate, force=self.force,
             appname=self.appname, verbose=self.verbose, base_dir=self.base_dir,
             terminal_has_colors=self.terminal_has_colors, initialized=False)
 
         if vsphere:
             self.vsphere[vsphere_name] = vsphere
             vsphere.initialized = True
         else:
-            msg = _("Could not initialize {} object from:").format('VsphereConnection')
+            msg = _('Could not initialize {} object from:').format('VsphereConnection')
             msg += '\n' + str(vsphere_data)
             LOG.error(msg)
 
     # -------------------------------------------------------------------------
     def cleaning_up(self):
-
+        """Close all VSPhere connections and remove all VSphere handlers."""
         if self.verbose > 1:
-            LOG.debug(_("Cleaning up ..."))
+            LOG.debug(_('Cleaning up ...'))
 
         for vsphere_name in self.do_vspheres:
-            LOG.debug(_("Closing VSPhere object {!r} ...").format(vsphere_name))
+            LOG.debug(_('Closing VSPhere object {!r} ...').format(vsphere_name))
             self.vsphere[vsphere_name].disconnect()
             del self.vsphere[vsphere_name]
 
 
 # =============================================================================
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_vmware-0.5.7/lib/fb_vmware/app/get_host_list.py` & `fb_vmware-0.6.0/lib/fb_vmware/app/get_host_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,46 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
+@summary: The module for the application object of the get-vsphere-host-list application.
+
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 by Frank Brehm, Berlin
-@summary: The module for the application object of the get-vsphere-host-list application.
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import, print_function
 
 # Standard modules
 import logging
 import re
 import sys
-
 from operator import itemgetter
 
 # Third party modules
-
-from fb_tools.common import pp
 from fb_tools.argparse_actions import RegexOptionAction
+from fb_tools.common import pp
 from fb_tools.xlate import format_list
 
 # Own modules
+from . import BaseVmwareApplication, VmwareAppError
 from .. import __version__ as GLOBAL_VERSION
-
-from ..xlate import XLATOR
-
 from ..spinner import Spinner
+from ..xlate import XLATOR
 
-from . import BaseVmwareApplication, VmwareAppError
-
-__version__ = '0.3.2'
+__version__ = '0.3.3'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 ngettext = XLATOR.ngettext
 
 
 # =============================================================================
 class GetVmHostsAppError(VmwareAppError):
-    """ Base exception class for all exceptions in this application."""
+    """Base exception class for all exceptions in this application."""
+
     pass
 
 
 # =============================================================================
 class GetHostsListApplication(BaseVmwareApplication):
     """Class for the application object."""
 
@@ -52,18 +49,18 @@
     default_sort_keys = ['name', 'vsphere']
 
     # -------------------------------------------------------------------------
     def __init__(
         self, appname=None, verbose=0, version=GLOBAL_VERSION, base_dir=None,
             initialized=False, usage=None, description=None,
             argparse_epilog=None, argparse_prefix_chars='-', env_prefix=None):
-
+        """Initialize a GetHostsListApplication object."""
         desc = _(
-            "Tries to get a list of all physical hosts in "
-            "VMWare VSphere and print it out.")
+            'Tries to get a list of all physical hosts in '
+            'VMWare VSphere and print it out.')
 
         self._host_pattern = self.default_host_pattern
         self.sort_keys = self.default_sort_keys
 
         self.hosts = []
 
         super(GetHostsListApplication, self).__init__(
@@ -78,148 +75,144 @@
     def host_pattern(self):
         """The regex search pattern for filtering the host list."""
         return self._host_pattern
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True):
         """
-        Transforms the elements of the object into a dict
+        Transform the elements of the object into a dict.
 
         @param short: don't include local properties in resulting dict.
         @type short: bool
 
         @return: structure as dict
         @rtype:  dict
         """
-
         res = super(GetHostsListApplication, self).as_dict(short=short)
         res['host_pattern'] = self.host_pattern
         res['default_host_pattern'] = self.default_host_pattern
 
         return res
 
     # -------------------------------------------------------------------------
     def init_arg_parser(self):
-        """
-        Public available method to initiate the argument parser.
-        """
-
+        """Public available method to initiate the argument parser."""
         super(GetHostsListApplication, self).init_arg_parser()
 
         filter_group = self.arg_parser.add_argument_group(_('Filter options'))
 
         filter_group.add_argument(
             '-p', '--pattern', '--search-pattern',
             dest='host_pattern', metavar='REGEX', action=RegexOptionAction,
             topic=_('for names of hosts'), re_options=re.IGNORECASE,
             help=_(
-                "A regular expression to filter the output list of hosts by their name "
-                "(Default: {!r}).").format(self.default_host_pattern)
+                'A regular expression to filter the output list of hosts by their name '
+                '(Default: {!r}).').format(self.default_host_pattern)
         )
 
         online_filter = filter_group.add_mutually_exclusive_group()
         online_filter.add_argument(
-            '--on', '--online', action="store_true", dest="online",
-            help=_("Filter output for online hosts.")
+            '--on', '--online', action='store_true', dest='online',
+            help=_('Filter output for online hosts.')
         )
         online_filter.add_argument(
-            '--off', '--offline', action="store_true", dest="offline",
-            help=_("Filter output for offline hosts and templates.")
+            '--off', '--offline', action='store_true', dest='offline',
+            help=_('Filter output for offline hosts and templates.')
         )
 
         output_options = self.arg_parser.add_argument_group(_('Output options'))
 
         output_options.add_argument(
             '-S', '--sort', metavar='KEY', nargs='+', dest='sort_keys',
             choices=self.avail_sort_keys, help=_(
-                "The keys for sorting the output. Available keys are: {avail}. "
-                "The default sorting keys are: {default}.").format(
+                'The keys for sorting the output. Available keys are: {avail}. '
+                'The default sorting keys are: {default}.').format(
                 avail=format_list(self.avail_sort_keys, do_repr=True),
                 default=format_list(self.default_sort_keys, do_repr=True))
         )
 
     # -------------------------------------------------------------------------
     def perform_arg_parser(self):
-
+        """Evaluate command line parameters."""
         super(GetHostsListApplication, self).perform_arg_parser()
 
         if self.args.host_pattern:
             try:
                 re_name = re.compile(self.args.host_pattern, re.IGNORECASE)
-                LOG.debug(_("Regular expression for filtering: {!r}").format(re_name.pattern))
+                LOG.debug(_('Regular expression for filtering: {!r}').format(re_name.pattern))
                 self._host_pattern = self.args.host_pattern
             except Exception as e:
-                msg = _("Got a {c} for pattern {p!r}: {e}").format(
+                msg = _('Got a {c} for pattern {p!r}: {e}').format(
                     c=e.__class__.__name__, p=self.args.host_pattern, e=e)
                 LOG.error(msg)
 
         if self.args.sort_keys:
             self.sort_keys = self.args.sort_keys
 
     # -------------------------------------------------------------------------
     def _run(self):
 
-        LOG.debug(_("Starting {a!r}, version {v!r} ...").format(
+        LOG.debug(_('Starting {a!r}, version {v!r} ...').format(
             a=self.appname, v=self.version))
 
         ret = 0
         try:
             ret = self.get_all_hosts()
         finally:
             self.cleaning_up()
 
         self.exit(ret)
 
     # -------------------------------------------------------------------------
     def get_all_hosts(self):
-
+        """Collect all physical VMWare hosts."""
         ret = 0
         all_hosts = []
 
         if self.verbose:
             for vsphere_name in self.vsphere:
                 all_hosts += self.get_hosts(vsphere_name)
         elif not self.quiet:
-            spin_prompt = _("Getting all VSPhere hosts ...") + ' '
+            spin_prompt = _('Getting all VSPhere hosts ...') + ' '
             with Spinner(spin_prompt):
                 for vsphere_name in self.vsphere:
                     all_hosts += self.get_hosts(vsphere_name)
             sys.stdout.write(' ' * len(spin_prompt))
             sys.stdout.write('\r')
             sys.stdout.flush()
 
         first = True
         out_hosts = []
 
         for host in all_hosts:
             if self.verbose > 1 and first:
-                LOG.debug(_("First found host:") + '\n' + pp(host.as_dict()))
+                LOG.debug(_('First found host:') + '\n' + pp(host.as_dict()))
             first = False
             is_online = True
             if not host.connection_state or host.maintenance:
                 is_online = False
             if not host.online or host.quarantaine:
                 is_online = False
             if self.args.online:
                 if not is_online:
                     continue
             elif self.args.offline:
                 if is_online:
                     continue
             out_hosts.append(self.create_host_summary(host))
         if self.verbose > 1:
-            LOG.debug("All hosts:\n{}".format(pp(out_hosts)))
+            LOG.debug('All hosts:\n{}'.format(pp(out_hosts)))
 
         self.print_hosts(out_hosts)
 
         return ret
 
     # -------------------------------------------------------------------------
     def create_host_summary(self, host):
-
+        """Return a dict with host properties as a summary for the given host."""
         summary = {}
 
         summary['vsphere'] = host.vsphere
         summary['cluster'] = host.cluster_name
         summary['name'] = host.name
         summary['connection_state'] = host.connection_state
         cpu_cores = '-'
@@ -240,22 +233,22 @@
         summary['os_version'] = host.product.os_version
         summary['quarantaine'] = host.quarantaine
 
         return summary
 
     # -------------------------------------------------------------------------
     def print_hosts(self, hosts):
-
+        """Print on STDOUT all information about all hosts in a human readable format."""
         labels = {
             'vsphere': 'VSPhere',
             'cluster': 'Cluster',
             'name': 'Host',
-            'connection_state': _("Connect state"),
-            'cpus': _("CPU cores/threads"),
-            'memory_gb': _("Memory in GiB"),
+            'connection_state': _('Connect state'),
+            'cpus': _('CPU cores/threads'),
+            'memory_gb': _('Memory in GiB'),
             'vendor': _('Vendor'),
             'model': _('Model'),
             'maintenance': _('Maintenance'),
             'online': _('Online'),
             # 'no_portgroups': _('Portgroups'),
             'power_state': _('Power State'),
             'os_name': _('OS Name'),
@@ -282,40 +275,40 @@
                     host[label] = val
                 else:
                     if label == 'memory_gb':
                         val = '{:7.1f}'.format(val)
                         host[label] = val
                     elif label in ('connection_state', 'maintenance', 'online', 'quarantaine'):
                         if val:
-                            val = _("Yes")
+                            val = _('Yes')
                         else:
-                            val = _("No")
+                            val = _('No')
                         host[label] = val
                 if len(val) > str_lengths[label]:
                     str_lengths[label] = len(val)
 
         for label in labels.keys():
             if max_len:
                 max_len += 2
             max_len += str_lengths[label]
 
         if self.verbose > 1:
-            LOG.debug("Label length:\n" + pp(str_lengths))
-            LOG.debug("Max line length: {} chars".format(max_len))
+            LOG.debug('Label length:\n' + pp(str_lengths))
+            LOG.debug('Max line length: {} chars'.format(max_len))
 
         tpl = ''
         for label in label_list:
             if tpl != '':
                 tpl += '  '
             if label in ('memory_gb', 'cpus', 'no_portgroups'):
                 tpl += '{{{la}:>{le}}}'.format(la=label, le=str_lengths[label])
             else:
                 tpl += '{{{la}:<{le}}}'.format(la=label, le=str_lengths[label])
         if self.verbose > 1:
-            LOG.debug(_("Line template: {}").format(tpl))
+            LOG.debug(_('Line template: {}').format(tpl))
 
         if not self.quiet:
             print()
             print(tpl.format(**labels))
             print('-' * max_len)
 
         hosts.sort(key=itemgetter(*self.sort_keys))
@@ -323,25 +316,25 @@
         for host in hosts:
             count += 1
             print(tpl.format(**host))
 
         if not self.quiet:
             print()
             if count == 0:
-                msg = _("Found no VMWare hosts.")
+                msg = _('Found no VMWare hosts.')
             else:
                 msg = ngettext(
-                    "Found one VMWare host.",
-                    "Found {} VMWare hosts.", count).format(count)
+                    'Found one VMWare host.',
+                    'Found {} VMWare hosts.', count).format(count)
             print(msg)
             print()
 
     # -------------------------------------------------------------------------
     def get_hosts(self, vsphere_name):
-
+        """Get all host of all physical hosts in a VMWare VSPhere."""
         hosts = []
 
         vsphere = self.vsphere[vsphere_name]
         vsphere.get_datacenter()
 
         re_name = None
         if self.host_pattern is not None:
@@ -353,14 +346,14 @@
             host = vsphere.hosts[host_name]
             hosts.append(host)
 
         return hosts
 
 
 # =============================================================================
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_vmware-0.5.7/lib/fb_vmware/app/get_vm_info.py` & `fb_vmware-0.6.0/lib/fb_vmware/app/get_vm_info.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,113 +1,102 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
+@summary: The module for the application object of the get-vsphere-vm-info application.
+
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 by Frank Brehm, Berlin
-@summary: The module for the application object of the get-vsphere-vm-info application.
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import, print_function
 
 # Standard modules
 import logging
-
 from operator import attrgetter
 
-# Third party modules
-
 # Own modules
-from .. import __version__ as GLOBAL_VERSION
-
-from ..errors import VSphereExpectedError
-
-from ..xlate import XLATOR
-
 from . import BaseVmwareApplication, VmwareAppError
-
+from .. import __version__ as GLOBAL_VERSION
 from ..controller import VsphereDiskController
-
+from ..errors import VSphereExpectedError
 from ..ether import VsphereEthernetcard
+from ..xlate import XLATOR
 
-__version__ = '1.6.2'
+__version__ = '1.6.3'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 ngettext = XLATOR.ngettext
 
 
 # =============================================================================
 class GetVmAppError(VmwareAppError):
-    """ Base exception class for all exceptions in this application."""
+    """Base exception class for all exceptions in this application."""
+
     pass
 
 
 # =============================================================================
 class GetVmApplication(BaseVmwareApplication):
-    """
-    Class for the application objects.
-    """
+    """Class for the application objects."""
 
     # -------------------------------------------------------------------------
     def __init__(
         self, appname=None, verbose=0, version=GLOBAL_VERSION, base_dir=None,
             initialized=False, usage=None, description=None,
             argparse_epilog=None, argparse_prefix_chars='-', env_prefix=None):
-
+        """Initialize the GetVmApplication object."""
         desc = _(
-            "Tries to get information about the given virtual machines in "
-            "VMWare VSphere and print it out.")
+            'Tries to get information about the given virtual machines in '
+            'VMWare VSphere and print it out.')
 
         self.vms = []
 
         super(GetVmApplication, self).__init__(
             appname=appname, verbose=verbose, version=version, base_dir=base_dir,
             description=desc, initialized=False,
         )
 
         self.initialized = True
 
     # -------------------------------------------------------------------------
     def init_arg_parser(self):
-        """
-        Public available method to initiate the argument parser.
-        """
-
+        """Initiate the argument parser."""
         super(GetVmApplication, self).init_arg_parser()
 
         self.arg_parser.add_argument(
             'vms', metavar='VM', type=str, nargs='+',
             help=_('Names of the VM to get information.'),
         )
 
     # -------------------------------------------------------------------------
     def perform_arg_parser(self):
-
+        """Evaluate the command line parameters. Maybe overridden."""
         super(GetVmApplication, self).perform_arg_parser()
 
         for vm in self.args.vms:
             self.vms.append(vm)
 
     # -------------------------------------------------------------------------
     def _run(self):
 
-        LOG.debug(_("Starting {a!r}, version {v!r} ...").format(
+        LOG.debug(_('Starting {a!r}, version {v!r} ...').format(
             a=self.appname, v=self.version))
 
         ret = 99
         try:
             ret = self.show_vms()
         finally:
             self.cleaning_up()
 
         self.exit(ret)
 
     # -------------------------------------------------------------------------
     def show_vms(self):
-
+        """Show all virtual machines."""
         ret = 0
 
         try:
             for vsphere_name in self.vsphere:
                 vsphere = self.vsphere[vsphere_name]
                 vsphere.get_datacenter()
 
@@ -119,54 +108,54 @@
             if not self.show_vm(vm_name):
                 ret = 1
 
         return ret
 
     # -------------------------------------------------------------------------
     def show_vm(self, vm_name):
-
+        """Show a particular VM on STDOUT."""
         print('\n{}: '.format(vm_name), end='')
         if self.verbose:
             print()
 
         vm = self._get_vm_data(vm_name)
         if not vm:
-            print(self.colored(_("NOT FOUND"), 'RED'))
+            print(self.colored(_('NOT FOUND'), 'RED'))
             return False
 
         # print("{ok}\n{vm}".format(ok=self.colored("OK", 'GREEN'), vm=pp(vm.as_dict(bare=True))))
-        print("{ok}".format(ok=self.colored("OK", 'GREEN')))
+        print('{ok}'.format(ok=self.colored('OK', 'GREEN')))
         print()
-        print("    State:    {s:<13} Config version: {v}".format(
+        print('    State:    {s:<13} Config version: {v}'.format(
             s=vm.power_state, v=vm.config_version))
-        msg = "    VSPhere:  {vs:<10}    Cluster: {cl:<20}    Path: {p}".format(
+        msg = '    VSPhere:  {vs:<10}    Cluster: {cl:<20}    Path: {p}'.format(
             vs=vm.vsphere, cl=vm.cluster_name, p=vm.path)
         print(msg)
 
         no_cpu = '   -'
         if vm.num_cpu is not None:
             no_cpu = '{:4d}'.format(vm.num_cpu)
 
         ram = '        -'
         if vm.memory_gb is not None:
             ram = '{:5.1f} GiB'.format(vm.memory_gb)
 
-        msg = "    No. CPUs: {cp}          RAM: {m}                   Cfg-Path: {p}".format(
+        msg = '    No. CPUs: {cp}          RAM: {m}                   Cfg-Path: {p}'.format(
             cp=no_cpu, m=ram, p=vm.config_path)
         print(msg)
 
         os_id = '{:<43}'.format('-')
         if vm.guest_id is not None:
             os_id = '{:<43}'.format(vm.guest_id)
 
         os_name = _('Unknown')
         if vm.guest_fullname is not None:
             os_name = vm.guest_fullname
 
-        print("    OS:       {id}    {os}".format(id=os_id, os=os_name))
+        print('    OS:       {id}    {os}'.format(id=os_id, os=os_name))
 
         self._print_ctrlrs(vm)
         self._print_disks(vm)
         self._print_interfaces(vm)
         self._print_custom_data(vm)
 
         return True
@@ -184,28 +173,28 @@
             if first:
                 label = 'Controller:'
             first = False
             ctype = _('Unknown')
             nr_disks = len(ctrlr.devices)
             if ctrlr.ctrl_type in VsphereDiskController.type_names.keys():
                 ctype = VsphereDiskController.type_names[ctrlr.ctrl_type]
-            no_disk = ngettext("{nr:>2} disk ", "{nr:>2} disks", nr_disks).format(
+            no_disk = ngettext('{nr:>2} disk ", "{nr:>2} disks', nr_disks).format(
                 nr=nr_disks)
             # no_disk = _("{nr:>2} disks").format(nr=len(ctrlr.devices))
             # if len(ctrlr.devices) == 1:
             #     no_disk = _(" 1 disk ")
-            msg = "    {la:<15}  {nr:>2} - {di} - {ty}".format(
+            msg = '    {la:<15}  {nr:>2} - {di} - {ty}'.format(
                 la=label, nr=ctrlr.bus_nr, di=no_disk, ty=ctype)
             print(msg)
 
     # -------------------------------------------------------------------------
     def _print_disks(self, vm):
 
         if not vm.disks:
-            print("    Disks:       {}".format(_('None')))
+            print('    Disks:       {}'.format(_('None')))
             return
 
         total_gb = 0.0
         first = True
         for disk in vm.disks:
             total_gb += disk.size_gb
             label = ' ' * 15
@@ -213,51 +202,51 @@
                 label = (ngettext('Disk', 'Disks', len(vm.disks)) + ':').ljust(15)
             first = False
             ctrlr_nr = -1
             for ctrlr in vm.controllers:
                 if disk.key in ctrlr.devices:
                     ctrlr_nr = ctrlr.bus_nr
                     break
-            msg = "    {la}  {n:<15} - {s:7.1f} GiB - Controller {c:>2} - File {f}".format(
+            msg = '    {la}  {n:<15} - {s:7.1f} GiB - Controller {c:>2} - File {f}'.format(
                 la=label, n=disk.label, s=disk.size_gb, c=ctrlr_nr, f=disk.file_name)
             print(msg)
         if len(vm.disks) > 1:
             msg = (' ' * 21) + '{n:<15} - {s:7.1f} GiB'.format(n=_('Total'), s=total_gb)
             print(msg)
 
     # -------------------------------------------------------------------------
     def _print_interfaces(self, vm):
 
         if not vm.interfaces:
-            print("    Ethernet:    {}".format(_('None')))
+            print('    Ethernet:    {}'.format(_('None')))
             return
 
         first = True
         for dev in vm.interfaces:
             label = ' ' * 15
             if first:
                 label = 'Ethernet:'.ljust(15)
             first = False
             etype = _('Unknown')
             if dev.ether_type in VsphereEthernetcard.ether_types.keys():
                 etype = VsphereEthernetcard.ether_types[dev.ether_type]
-            msg = "    {la}  {n:<15} - Network {nw:<20} - Connection: {c:<4} - {t}".format(
+            msg = '    {la}  {n:<15} - Network {nw:<20} - Connection: {c:<4} - {t}'.format(
                 la=label, n=dev.label, nw=dev.backing_device, c=dev.connect_status, t=etype)
             print(msg)
 
     # -------------------------------------------------------------------------
     def _print_custom_data(self, vm):
 
         if not vm.custom_data:
             return
 
         no_vals = len(vm.custom_data)
 
         label = ngettext('Custom Value', 'Custom Values', no_vals)
-        print("    {}:".format(label))
+        print('    {}:'.format(label))
 
         max_key_len = 1
         for custom_data in vm.full_custom_data:
             for custom_name in custom_data.keys():
                 if len(custom_name) > max_key_len:
                     max_key_len = len(custom_name)
         max_key_len += 1
@@ -269,15 +258,15 @@
                     n=name, len=max_key_len, val=custom_value)
                 print(line.rstrip())
 
     # -------------------------------------------------------------------------
     def _get_vm_data(self, vm_name):
 
         if self.verbose > 1:
-            LOG.debug(_("Pulling full data of VM {!r} ...").format(vm_name))
+            LOG.debug(_('Pulling full data of VM {!r} ...').format(vm_name))
 
         vm = None
 
         for vsphere_name in self.vsphere:
             vsphere = self.vsphere[vsphere_name]
             vm = vsphere.get_vm(vm_name, vsphere_name=vsphere_name, no_error=True, as_obj=True)
             vm.full_custom_data = []
@@ -293,14 +282,14 @@
             if vm:
                 break
 
         return vm
 
 
 # =============================================================================
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_vmware-0.5.7/lib/fb_vmware/app/get_vm_list.py` & `fb_vmware-0.6.0/lib/fb_vmware/app/get_vm_list.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,72 +1,67 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
+@summary: The module for the application object of the get-vsphere-vm-list application.
+
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 by Frank Brehm, Berlin
-@summary: The module for the application object of the get-vsphere-vm-list application.
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import, print_function
 
 # Standard modules
 import logging
 import re
 import sys
-
-from operator import itemgetter, attrgetter
+from operator import attrgetter, itemgetter
 
 # Third party modules
-from fb_tools.common import pp, to_bool
 from fb_tools.argparse_actions import RegexOptionAction
+from fb_tools.common import pp, to_bool
 from fb_tools.xlate import format_list
 
 # Own modules
+from . import BaseVmwareApplication, VmwareAppError
 from .. import __version__ as GLOBAL_VERSION
-
-from ..xlate import XLATOR
-
 from ..spinner import Spinner
-
-from . import BaseVmwareApplication, VmwareAppError
-
 from ..vm import VsphereVm
+from ..xlate import XLATOR
 
-__version__ = '1.6.4'
+__version__ = '1.6.5'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 ngettext = XLATOR.ngettext
 
 
 # =============================================================================
 class GetVmListAppError(VmwareAppError):
-    """ Base exception class for all exceptions in this application."""
+    """Base exception class for all exceptions in this application."""
+
     pass
 
 
 # =============================================================================
 class GetVmListApplication(BaseVmwareApplication):
-    """
-    Class for the application objects.
-    """
+    """Class for the application objects."""
 
     default_vm_pattern = r'.*'
     avail_sort_keys = ('name', 'vsphere', 'cluster', 'path', 'type', 'onl_str', 'cfg_ver', 'os')
     default_sort_keys = ['name', 'vsphere']
 
     # -------------------------------------------------------------------------
     def __init__(
         self, appname=None, verbose=0, version=GLOBAL_VERSION, base_dir=None,
             initialized=False, usage=None, description=None,
             argparse_epilog=None, argparse_prefix_chars='-', env_prefix=None):
-
+        """Initialize a GetVmListApplication object."""
         desc = _(
-            "Tries to get a list of all virtual machines in "
-            "VMWare VSphere and print it out.")
+            'Tries to get a list of all virtual machines in '
+            'VMWare VSphere and print it out.')
 
         self._vm_pattern = self.default_vm_pattern
         self._details = False
 
         self.sort_keys = self.default_sort_keys
 
         self._re_hw = None
@@ -80,239 +75,230 @@
         )
 
         self.initialized = True
 
     # -------------------------------------------------------------------------
     @property
     def vm_pattern(self):
-        """The regex search pattern for filtering the VM list."""
+        """Return the regex search pattern for filtering the VM list."""
         return self._vm_pattern
 
     # -------------------------------------------------------------------------
     @property
     def details(self):
-        """Should the list be displyed with all details."""
+        """Return whther the list should be displyed with all details."""
         return self._details
 
     @details.setter
     def details(self, value):
         self._details = to_bool(value)
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True):
         """
-        Transforms the elements of the object into a dict
+        Transform the elements of the object into a dict.
 
         @param short: don't include local properties in resulting dict.
         @type short: bool
 
         @return: structure as dict
         @rtype:  dict
         """
-
         res = super(GetVmListApplication, self).as_dict(short=short)
         res['details'] = self.details
         res['vm_pattern'] = self.vm_pattern
         res['default_vm_pattern'] = self.default_vm_pattern
 
         return res
 
     # -------------------------------------------------------------------------
     def post_init(self):
         """
-        Method to execute before calling run(). Here could be done some
-        finishing actions after reading in commandline parameters,
-        configuration a.s.o.
-
-        This method could be overwritten by descendant classes, these
-        methhods should allways include a call to post_init() of the
-        parent class.
+        Execute some things before calling run().
 
+        Here could be done some finishing actions after reading in
+        commandline parameters, configuration a.s.o.
         """
-
         super(GetVmListApplication, self).post_init()
 
         self.initialized = True
 
     # -------------------------------------------------------------------------
     def init_arg_parser(self):
-        """
-        Public available method to initiate the argument parser.
-        """
-
+        """Initiate the argument parser."""
         super(GetVmListApplication, self).init_arg_parser()
 
         filter_group = self.arg_parser.add_argument_group(_('Filter options'))
 
         filter_group.add_argument(
             '-p', '--pattern', '--search-pattern',
             dest='vm_pattern', metavar='REGEX', action=RegexOptionAction,
             topic=_('for names of VMs'), re_options=re.IGNORECASE,
             help=_(
-                "A regular expression to filter the output list of VMs by their name "
-                "(Default: {!r}).").format(self.default_vm_pattern)
+                'A regular expression to filter the output list of VMs by their name '
+                '(Default: {!r}).').format(self.default_vm_pattern)
         )
 
         valid_vm_types = ('all', 'vm', 'template')
         filter_group.add_argument(
             '-T', '--type', metavar=_('TYPE'), dest='vm_type', choices=valid_vm_types,
             default='all', help=_(
-                "Filter output for the type of the VM. Valid values are {li} "
-                "(Default: {dflt!r}).").format(
+                'Filter output for the type of the VM. Valid values are {li} '
+                '(Default: {dflt!r}).').format(
                 dflt='all', li=format_list(valid_vm_types, do_repr=True))
         )
 
         online_filter = filter_group.add_mutually_exclusive_group()
         online_filter.add_argument(
-            '--on', '--online', action="store_true", dest="online",
-            help=_("Filter output for online VMs.")
+            '--on', '--online', action='store_true', dest='online',
+            help=_('Filter output for online VMs.')
         )
         online_filter.add_argument(
-            '--off', '--offline', action="store_true", dest="offline",
-            help=_("Filter output for offline VMs and templates.")
+            '--off', '--offline', action='store_true', dest='offline',
+            help=_('Filter output for offline VMs and templates.')
         )
 
         filter_group.add_argument(
             '-H', '--hw', '--hardware-config', metavar='REGEX', action=RegexOptionAction,
             dest='hw', topic=_('for VMWare hardware config version'), re_options=re.IGNORECASE,
             help=_(
-                "A regular expression to filter the output list of VMs by the VMWare hardware "
+                'A regular expression to filter the output list of VMs by the VMWare hardware '
                 "configuration version (e.g. '{}').").format(r'vmx-0\d$'),
         )
 
         filter_group.add_argument(
             '--os', metavar='REGEX', action=RegexOptionAction, dest='os',
             topic=_('for the Operating System version'), re_options=re.IGNORECASE,
             help=_(
-                "A regular expression to filter the output list of VMs by their Operating "
+                'A regular expression to filter the output list of VMs by their Operating '
                 "System version, e.g. '{}'.").format('oracleLinux.*(_64)?Guest')
         )
 
         output_options = self.arg_parser.add_argument_group(_('Output options'))
 
         output_options.add_argument(
-            '-D', '--details', dest='details', action="store_true",
-            help=_("Detailed output list (quering data needs some time longer).")
+            '-D', '--details', dest='details', action='store_true',
+            help=_('Detailed output list (quering data needs some time longer).')
         )
 
         output_options.add_argument(
             '-S', '--sort', metavar='KEY', nargs='+', dest='sort_keys',
             choices=self.avail_sort_keys, help=_(
-                "The keys for sorting the output. Available keys are: {avail}. "
-                "The default sorting keys are: {default}.").format(
+                'The keys for sorting the output. Available keys are: {avail}. '
+                'The default sorting keys are: {default}.').format(
                 avail=format_list(self.avail_sort_keys, do_repr=True),
                 default=format_list(self.default_sort_keys, do_repr=True))
         )
 
     # -------------------------------------------------------------------------
     def perform_arg_parser(self):
-
+        """Evaluate the command line parameters."""
         super(GetVmListApplication, self).perform_arg_parser()
 
         if self.args.details:
             self.details = self.args.details
 
         if self.args.vm_pattern:
             try:
                 re_name = re.compile(self.args.vm_pattern, re.IGNORECASE)
-                LOG.debug(_("Regular expression for filtering: {!r}").format(re_name.pattern))
+                LOG.debug(_('Regular expression for filtering: {!r}').format(re_name.pattern))
                 self._vm_pattern = self.args.vm_pattern
             except Exception as e:
-                msg = _("Got a {c} for pattern {p!r}: {e}").format(
+                msg = _('Got a {c} for pattern {p!r}: {e}').format(
                     c=e.__class__.__name__, p=self.args.vm_pattern, e=e)
                 LOG.error(msg)
 
         if not self.details:
             if self.args.online or self.args.offline or self.args.hw or self.args.os or \
                     self.args.vm_type != 'all':
-                LOG.info(_("Detailed output is required because of your given options."))
+                LOG.info(_('Detailed output is required because of your given options.'))
                 self.details = True
 
         if self.args.sort_keys:
             if self.details:
                 self.sort_keys = self.args.sort_keys
             else:
                 self.sort_keys = []
                 for key in self.args.sort_keys:
                     if key in ('name', 'vsphere', 'path'):
                         self.sort_keys.append(key)
                     else:
                         LOG.warn(_(
-                            "Sorting key {!r} not usable, if not detailed output "
-                            "was given.").format(key))
+                            'Sorting key {!r} not usable, if not detailed output '
+                            'was given.').format(key))
                 if not self.sort_keys:
                     LOG.warn(_(
-                        "No usable sorting keys found, using default sorting keys {}.").format(
+                        'No usable sorting keys found, using default sorting keys {}.').format(
                         format_list(self.default_sort_keys, do_repr=True)))
                     self.sort_keys = self.default_sort_keys
 
         if self.args.hw:
             self._re_hw = re.compile(self.args.hw, re.IGNORECASE)
         if self.args.os:
             self._re_os = re.compile(self.args.os, re.IGNORECASE)
 
     # -------------------------------------------------------------------------
     def _run(self):
 
-        LOG.debug(_("Starting {a!r}, version {v!r} ...").format(
+        LOG.debug(_('Starting {a!r}, version {v!r} ...').format(
             a=self.appname, v=self.version))
 
         ret = 0
         try:
             ret = self.get_all_vms()
         finally:
             self.cleaning_up()
 
         self.exit(ret)
 
     # -------------------------------------------------------------------------
     def get_all_vms(self):
-
+        """Get all VMs from VSphere, maybe filtered."""
         ret = 0
         all_vms = []
 
         re_name = re.compile(self.vm_pattern, re.IGNORECASE)
 
         if self.verbose:
             for vsphere_name in self.vsphere:
                 all_vms += self.get_vms(vsphere_name, re_name)
         elif not self.quiet:
-            spin_prompt = _("Getting all VSPhere VMs ...") + ' '
+            spin_prompt = _('Getting all VSPhere VMs ...') + ' '
             with Spinner(spin_prompt):
                 for vsphere_name in self.vsphere:
                     all_vms += self.get_vms(vsphere_name, re_name)
             sys.stdout.write(' ' * len(spin_prompt))
             sys.stdout.write('\r')
             sys.stdout.flush()
 
         if self.verbose > 1:
-            LOG.debug(_("Using sorting keys:") + ' ' + format_list(self.sort_keys, do_repr=True))
+            LOG.debug(_('Using sorting keys:') + ' ' + format_list(self.sort_keys, do_repr=True))
 
         if self.details:
             self.print_vms_detailed(all_vms)
         else:
             self.print_vms(all_vms)
 
         return ret
 
     # -------------------------------------------------------------------------
     def print_vms(self, all_vms):
-
+        """Print out on STDOUT the list of found VMs."""
         label_list = ('name', 'vsphere', 'path')
         labels = {
             'name': 'Host',
             'vsphere': 'VSphere',
             'path': 'Path',
         }
 
         self._print_vms(all_vms, label_list, labels)
 
     # -------------------------------------------------------------------------
     def print_vms_detailed(self, all_vms):
-
+        """Print out on STDOUT the list of found VMs in a detailled way."""
         label_list = self.avail_sort_keys
         labels = {
             'name': 'VM/Template',
             'vsphere': 'VSphere',
             'cluster': 'Cluster',
             'path': 'Path',
             'type': 'Type',
@@ -343,24 +329,24 @@
 
         for label in labels.keys():
             if max_len:
                 max_len += 2
             max_len += str_lengths[label]
 
         if self.verbose > 1:
-            LOG.debug("Label length:\n" + pp(str_lengths))
-            LOG.debug("Max line length: {} chars".format(max_len))
+            LOG.debug('Label length:\n' + pp(str_lengths))
+            LOG.debug('Max line length: {} chars'.format(max_len))
 
         tpl = ''
         for label in label_list:
             if tpl != '':
                 tpl += '  '
             tpl += '{{{la}:<{le}}}'.format(la=label, le=str_lengths[label])
         if self.verbose > 1:
-            LOG.debug(_("Line template: {}").format(tpl))
+            LOG.debug(_('Line template: {}').format(tpl))
 
         if not self.quiet:
             print()
             print(tpl.format(**labels))
             print('-' * max_len)
 
         all_vms.sort(key=itemgetter(*self.sort_keys))
@@ -369,25 +355,25 @@
             count += 1
 
             print(tpl.format(**cdata))
 
         if not self.quiet:
             print()
             if count == 0:
-                msg = _("Found no VMWare VMs.")
+                msg = _('Found no VMWare VMs.')
             else:
                 msg = ngettext(
-                    "Found one VMWare VM.",
-                    "Found {} VMWare VMs.", count).format(count)
+                    'Found one VMWare VM.',
+                    'Found {} VMWare VMs.', count).format(count)
             print(msg)
             print()
 
     # -------------------------------------------------------------------------
     def get_vms(self, vsphere_name, re_name=None):
-
+        """Get the filtered list of VMs from VSPhere."""
         vsphere = self.vsphere[vsphere_name]
         vsphere.get_datacenter()
 
         if re_name is None:
             re_name = re.compile(self.vm_pattern, re.IGNORECASE)
 
         if self.details:
@@ -397,66 +383,66 @@
             vm_list = vsphere.get_vms(re_name, vsphere_name=vsphere_name, name_only=True)
             vms = self.mangle_vmlist_no_details(vm_list, vsphere_name)
 
         return vms
 
     # -------------------------------------------------------------------------
     def mangle_vmlist_no_details(self, vm_list, vsphere_name):
-
+        """Prepare the non-detailled data about found VMs for output."""
         if self.verbose > 3:
-            LOG.debug("Mangling VM list:\n" + pp(vm_list))
+            LOG.debug('Mangling VM list:\n' + pp(vm_list))
 
         vms = []
         first = True
 
         for vm in sorted(vm_list, key=itemgetter(0, 1)):
 
             if self.verbose > 2 and first:
-                LOG.debug("VM:\n" + pp(vm))
+                LOG.debug('VM:\n' + pp(vm))
 
             cdata = {
                 'vsphere': vsphere_name,
                 'name': vm[0],
                 'path': vm[1],
             }
 
             if cdata['path']:
                 cdata['path'] = '/' + cdata['path']
             else:
                 cdata['path'] = '/'
 
             if self.verbose > 2 and first:
-                LOG.debug("Mangled VM:\n" + pp(cdata))
+                LOG.debug('Mangled VM:\n' + pp(cdata))
 
             first = False
 
             vms.append(cdata)
 
         return vms
 
     # -------------------------------------------------------------------------
     def mangle_vmlist_details(self, vm_list, vsphere_name):
-
+        """Prepare the detailled data about found VMs for output."""
         vms = []
 
         first = True
         for vm in sorted(vm_list, key=attrgetter('name', 'path')):
 
             if not isinstance(vm, VsphereVm):
-                msg = _("Found a {} object:").format(vm.__class__.__name__)
+                msg = _('Found a {} object:').format(vm.__class__.__name__)
                 msg += '\n' + pp(vm)
                 LOG.error(msg)
                 continue
 
             if self.verbose > 2 and first:
-                LOG.debug("VM:\n" + pp(vm.as_dict()))
+                LOG.debug('VM:\n' + pp(vm.as_dict()))
 
             cdata = self._mangle_vm_details(vm, vsphere_name)
             if self.verbose > 2 and first and cdata:
-                LOG.debug("Mangled VM:\n" + pp(cdata))
+                LOG.debug('Mangled VM:\n' + pp(cdata))
 
             first = False
 
             if not cdata:
                 continue
 
             vms.append(cdata)
@@ -520,14 +506,14 @@
         if vm.template:
             cdata['type'] = 'VMWare Template'
 
         return cdata
 
 
 # =============================================================================
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_vmware-0.5.7/lib/fb_vmware/base.py` & `fb_vmware-0.6.0/lib/fb_vmware/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,192 +1,191 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
+@summary: The module for a base VSphere handler object.
+
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 by Frank Brehm, Berlin
-@summary: The module for a base VSphere handler object.
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
 import logging
 import ssl
-
 from abc import ABCMeta, abstractmethod
 
 # Third party modules
-from six import add_metaclass
+from fb_tools.common import to_bool
+from fb_tools.handling_obj import HandlingObject
 
-import pytz
+from pyVim.connect import Disconnect
+from pyVim.connect import SmartConnect
 
-from pyVim.connect import SmartConnect, Disconnect
 from pyVmomi import vim
 
-from fb_tools.common import to_bool
-from fb_tools.handling_obj import HandlingObject
+import pytz
 
-# Own modules
-from .xlate import XLATOR
+from six import add_metaclass
 
+# Own modules
+from .config import DEFAULT_VSPHERE_CLUSTER
+from .config import VSPhereConfigInfo
 from .errors import BaseVSphereHandlerError
-from .errors import VSphereCannotConnectError, VSphereVimFault
-
-from .config import VSPhereConfigInfo, DEFAULT_VSPHERE_CLUSTER
+from .errors import VSphereCannotConnectError
+from .errors import VSphereVimFault
+from .xlate import XLATOR
 
-__version__ = '0.2.4'
+__version__ = '0.2.5'
 
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 
 DEFAULT_TZ_NAME = 'Europe/Berlin'
 DEFAULT_MAX_SEARCH_DEPTH = 10
 
 
 # =============================================================================
 @add_metaclass(ABCMeta)
 class BaseVsphereHandler(HandlingObject):
     """
     Base class for a VSphere handler object.
-    May not be instantiated.
+
+    Must not be instantiated.
     """
 
     max_search_depth = DEFAULT_MAX_SEARCH_DEPTH
 
     # -------------------------------------------------------------------------
     def __init__(
         self, connect_info, appname=None, verbose=0, version=__version__, base_dir=None,
             cluster=DEFAULT_VSPHERE_CLUSTER, auto_close=False, simulate=None,
             force=None, terminal_has_colors=False, initialized=False, tz=DEFAULT_TZ_NAME):
-
+        """Initialize a BaseVsphereHandler object."""
         self._cluster = cluster
         self._auto_close = False
         self._tz = pytz.timezone(DEFAULT_TZ_NAME)
 
         self.connect_info = None
         self.service_instance = None
 
         super(BaseVsphereHandler, self).__init__(
             appname=appname, verbose=verbose, version=version, base_dir=base_dir,
             simulate=simulate, force=force, terminal_has_colors=terminal_has_colors,
             initialized=False,
         )
 
         if not isinstance(connect_info, VSPhereConfigInfo):
-            msg = _("The given parameter {pc!r} ({pv!r}) is not a {o} object.").format(
+            msg = _('The given parameter {pc!r} ({pv!r}) is not a {o} object.').format(
                 pc='connect_info', pv=connect_info, o='VSPhereConfigInfo')
             raise BaseVSphereHandlerError(msg)
 
         if not connect_info.host:
-            msg = _("No VSPhere host name or address given in {w}.").format(w='connect_info')
+            msg = _('No VSPhere host name or address given in {w}.').format(w='connect_info')
             raise BaseVSphereHandlerError(msg)
 
         if not connect_info.initialized:
-            msg = _("The {c} object given as {w} is not initialized.").format(
+            msg = _('The {c} object given as {w} is not initialized.').format(
                 c='VSPhereConfigInfo', w='connect_info')
             raise BaseVSphereHandlerError(msg)
 
         self.connect_info = connect_info
 
         self.tz = tz
         self.auto_close = auto_close
 
         self.initialized = initialized
 
     # -----------------------------------------------------------
     @property
     def auto_close(self):
-        """Flage, whether an existing connection should be closed on
-            destroying the current object."""
+        """Should an existing connection be closed on destroying the current object."""
         return getattr(self, '_auto_close', False)
 
     @auto_close.setter
     def auto_close(self, value):
         self._auto_close = to_bool(value)
 
     # -----------------------------------------------------------
     @property
     def dc(self):
-        """The name of the VSphere datacenter to use."""
-
+        """Return the name of the VSphere datacenter to use."""
         connect_info = getattr(self, 'connect_info', None)
         if connect_info:
             return connect_info.dc
         return None
 
     # -----------------------------------------------------------
     @property
     def cluster(self):
-        """The name of the VSphere cluster to use."""
+        """Return the name of the VSphere cluster to use."""
         return self._cluster
 
     # -----------------------------------------------------------
     @property
     def tz(self):
-        """The current time zone."""
+        """Return the current time zone."""
         return self._tz
 
     @tz.setter
     def tz(self, value):
         if isinstance(value, pytz.tzinfo.BaseTzInfo):
             self._tz = value
         else:
             self._tz = pytz.timezone(value)
 
     # -------------------------------------------------------------------------
     @abstractmethod
     def __repr__(self):
         """Typecasting into a string for reproduction."""
-
-        out = "<%s()>" % (self.__class__.__name__)
+        out = '<%s()>' % (self.__class__.__name__)
         return out
 
     # -------------------------------------------------------------------------
     def _repr(self):
 
-        out = "<%s(" % (self.__class__.__name__)
+        out = '<%s(' % (self.__class__.__name__)
 
         fields = []
-        fields.append("connect_info={}".format(self.connect_info._repr()))
-        fields.append("cluster={!r}".format(self.cluster))
-        fields.append("auto_close={!r}".format(self.auto_close))
-        fields.append("simulate={!r}".format(self.simulate))
-        fields.append("force={!r}".format(self.force))
+        fields.append('connect_info={}'.format(self.connect_info._repr()))
+        fields.append('cluster={!r}'.format(self.cluster))
+        fields.append('auto_close={!r}'.format(self.auto_close))
+        fields.append('simulate={!r}'.format(self.simulate))
+        fields.append('force={!r}'.format(self.force))
 
-        out += ", ".join(fields) + ")>"
+        out += ', '.join(fields) + ')>'
         return out
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True):
         """
-        Transforms the elements of the object into a dict
+        Transform the elements of the object into a dict.
 
         @param short: don't include local properties in resulting dict.
         @type short: bool
 
         @return: structure as dict
         @rtype:  dict
         """
-
         res = super(BaseVsphereHandler, self).as_dict(short=short)
         res['dc'] = self.dc
         res['tz'] = None
         if self.tz:
             res['tz'] = self.tz.zone
         res['cluster'] = self.cluster
         res['auto_close'] = self.auto_close
         res['max_search_depth'] = self.max_search_depth
 
         return res
 
     # -------------------------------------------------------------------------
     def connect(self):
-
-        LOG.debug(_("Connecting to vSphere {!r} ...").format(self.connect_info.full_url))
+        """Connect to the the configured VSPhere instance."""
+        LOG.debug(_('Connecting to vSphere {!r} ...').format(self.connect_info.full_url))
 
         try:
             if self.connect_info.use_https:
 
                 ssl_context = None
                 if hasattr(ssl, '_create_unverified_context'):
                     ssl_context = ssl._create_unverified_context()
@@ -206,41 +205,42 @@
             raise VSphereVimFault(e, self.connect_info.full_url)
 
         if not self.service_instance:
             raise VSphereCannotConnectError(self.connect_info.url)
 
     # -------------------------------------------------------------------------
     def disconnect(self):
-
+        """Disconnect from the the configured VSPhere instance."""
         if self.service_instance:
-            LOG.debug(_("Disconnecting from VSPhere {!r}.").format(self.connect_info.url))
+            LOG.debug(_('Disconnecting from VSPhere {!r}.').format(self.connect_info.url))
             Disconnect(self.service_instance)
 
         self.service_instance = None
 
     # -------------------------------------------------------------------------
     def get_obj(self, content, vimtype, name):
-
+        """Get the appropriate pyvomomi object with the given criteria."""
         obj = None
         container = content.viewManager.CreateContainerView(content.rootFolder, vimtype, True)
         for c in container.view:
             if c.name == name:
                 obj = c
                 break
 
         return obj
 
     # -------------------------------------------------------------------------
     def __del__(self):
+        """Destroy the current Python object in this magic method."""
         if self.auto_close:
             self.disconnect()
 
 
 # =============================================================================
 
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_vmware-0.5.7/lib/fb_vmware/cluster.py` & `fb_vmware-0.6.0/lib/fb_vmware/cluster.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
+@summary: The module for capsulating a VSphere calculation cluster object.
+
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 by Frank Brehm, Berlin
-@summary: The module for capsulating a VSphere calculation cluster object.
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
 import logging
 
 # Third party modules
-from pyVmomi import vim
-
-from fb_tools.common import pp, to_bool, is_sequence
+from fb_tools.common import is_sequence, pp, to_bool
 from fb_tools.xlate import format_list
 
-# Own modules
-from .obj import VsphereObject, DEFAULT_OBJ_STATUS
+from pyVmomi import vim
 
+# Own modules
+from .obj import DEFAULT_OBJ_STATUS
+from .obj import VsphereObject
 from .xlate import XLATOR
 
-__version__ = '1.4.2'
+__version__ = '1.4.3'
 LOG = logging.getLogger(__name__)
 
 
 _ = XLATOR.gettext
 
 
 # =============================================================================
 class VsphereCluster(VsphereObject):
+    """An object for encapsulating a VSphere calculation cluster object."""
 
     # -------------------------------------------------------------------------
     def __init__(
         self, appname=None, verbose=0, version=__version__, base_dir=None, initialized=None,
             name=None, status=DEFAULT_OBJ_STATUS, cpu_cores=0, cpu_threads=0,
             config_status=DEFAULT_OBJ_STATUS, hosts_effective=0, hosts_total=0,
             mem_mb_effective=0, mem_total=0, standalone=False):
-
+        """Initialize a VsphereCluster object."""
         self.repr_fields = (
             'name', 'status', 'config_status', 'cpu_cores', 'cpu_threads', 'hosts_effective',
             'hosts_total', 'mem_mb_effective', 'mem_total', 'appname', 'verbose', 'version')
 
         self._status = None
         self._cpu_cores = None
         self._cpu_threads = None
@@ -52,15 +54,15 @@
         self._mem_total = None
         self._standalone = False
         self.networks = []
         self.datastores = []
         self.resource_pool = None
 
         super(VsphereCluster, self).__init__(
-            name=name, obj_type='vsphere_cluster', name_prefix="cluster", status=status,
+            name=name, obj_type='vsphere_cluster', name_prefix='cluster', status=status,
             config_status=config_status, appname=appname, verbose=verbose,
             version=version, base_dir=base_dir)
 
         self.cpu_cores = cpu_cores
         self.cpu_threads = cpu_threads
         self.hosts_effective = hosts_effective
         self.hosts_total = hosts_total
@@ -173,61 +175,57 @@
         if self.mem_total is None:
             return None
         return float(self.mem_total) / 1024.0 / 1024.0 / 1024.0
 
     # -----------------------------------------------------------
     @property
     def mem_mb_effective(self):
-        """The effective memory resources (in MB) available
-            to run virtual machines of the cluster."""
+        """The effective memory resources (in MB) available to run VMs of the cluster."""
         return self._mem_mb_effective
 
     @mem_mb_effective.setter
     def mem_mb_effective(self, value):
         if value is None:
             self._mem_mb_effective = 0
             return
 
         val = int(value)
         self._mem_mb_effective = val
 
     # -----------------------------------------------------------
     @property
     def mem_gb_effective(self):
-        """The effective memory resources (in GiBytes) available
-            to run virtual machines of the cluster."""
+        """The effective memory resources (in GiBytes) available to run VMs of the cluster."""
         if self.mem_mb_effective is None:
             return None
         return float(self.mem_mb_effective) / 1024.0
 
     # -----------------------------------------------------------
     @property
     def standalone(self):
-        "Is this a standalone host and not a computing cluster?"
-
+        """Return whether this a standalone host and not a computing cluster."""
         return self._standalone
 
     @standalone.setter
     def standalone(self, value):
-
         self._standalone = to_bool(value)
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True):
         """
-        Transforms the elements of the object into a dict
+        Transform the elements of the object into a dict.
 
         @param short: don't include local properties in resulting dict.
         @type short: bool
 
         @return: structure as dict
         @rtype:  dict
         """
-
         res = super(VsphereCluster, self).as_dict(short=short)
+
         res['resource_pool_name'] = self.resource_pool_name
         res['resource_pool_var'] = self.resource_pool_var
         res['cpu_cores'] = self.cpu_cores
         res['cpu_threads'] = self.cpu_threads
         res['hosts_effective'] = self.hosts_effective
         res['hosts_total'] = self.hosts_total
         res['mem_mb_effective'] = self.mem_mb_effective
@@ -244,47 +242,47 @@
                 res['resource_pool.summary'] = '{} object'.format(
                     self.resource_pool.summary.__class__.__name__)
 
         return res
 
     # -------------------------------------------------------------------------
     def __copy__(self):
-
+        """Magic method to return a deep copy of the current object."""
         return VsphereCluster(
             appname=self.appname, verbose=self.verbose, base_dir=self.base_dir,
             initialized=self.initialized, name=self.name, standalone=self.standalone,
             status=self.status, cpu_cores=self.cpu_cores, cpu_threads=self.cpu_threads,
             hosts_effective=self.hosts_effective, hosts_total=self.hosts_total,
             mem_mb_effective=self.mem_mb_effective, mem_total=self.mem_total)
 
     # -------------------------------------------------------------------------
     def __eq__(self, other):
-
+        """Use this magic method as the '=='-operator."""
         if self.verbose > 4:
-            LOG.debug(_("Comparing {} objects ...").format(self.__class__.__name__))
+            LOG.debug(_('Comparing {} objects ...').format(self.__class__.__name__))
 
         if not isinstance(other, VsphereCluster):
             return False
 
         if self.name != other.name:
             return False
 
         return True
 
     # -------------------------------------------------------------------------
     @classmethod
     def from_summary(cls, data, appname=None, verbose=0, base_dir=None, test_mode=False):
-
+        """Create a new VsphereCluster object based on the appropriate data from pyvomi."""
         if test_mode:
             cls._check_summary_data(data)
         else:
             if not isinstance(data, (vim.ClusterComputeResource, vim.ComputeResource)):
                 msg = _(
-                    "Parameter {t!r} must be a {e} object, a {v} object was given "
-                    "instead.").format(t='data', e='vim.AboutInfo', v=data.__class__.__qualname__)
+                    'Parameter {t!r} must be a {e} object, a {v} object was given '
+                    'instead.').format(t='data', e='vim.AboutInfo', v=data.__class__.__qualname__)
                 raise TypeError(msg)
 
         params = {
             'appname': appname,
             'verbose': verbose,
             'base_dir': base_dir,
             'initialized': True,
@@ -299,30 +297,30 @@
             'mem_total': data.summary.totalMemory,
             'standalone': False,
         }
         if isinstance(data, vim.ComputeResource):
             params['standalone'] = True
 
         if verbose > 2:
-            LOG.debug(_("Creating {} object from:").format(cls.__name__) + '\n' + pp(params))
+            LOG.debug(_('Creating {} object from:').format(cls.__name__) + '\n' + pp(params))
 
         cluster = cls(**params)
 
         for network in data.network:
             nname = network.name
             if nname not in cluster.networks:
                 if verbose > 2:
-                    LOG.debug(_("Cluster {c!r} has network {n!r}.").format(
+                    LOG.debug(_('Cluster {c!r} has network {n!r}.').format(
                         c=cluster.name, n=nname))
                 cluster.networks.append(nname)
 
         for ds in data.datastore:
             if ds.name not in cluster.datastores:
                 if verbose > 2:
-                    LOG.debug(_("Cluster {c!r} has datastore {d!r}.").format(
+                    LOG.debug(_('Cluster {c!r} has datastore {d!r}.').format(
                         c=cluster.name, d=ds.name))
                 cluster.datastores.append(ds.name)
 
         cluster.resource_pool = data.resourcePool
 
         return cluster
 
@@ -342,43 +340,43 @@
             if not hasattr(data, field):
                 failing_fields.append(field)
 
         if hasattr(data, 'summary'):
             summary = data.summary
             for field in summary_fields:
                 if not hasattr(summary, field):
-                    failing_fields.append("summary.{}".format(field))
+                    failing_fields.append('summary.{}'.format(field))
 
         if hasattr(data, 'datastore'):
             if not is_sequence(data.datastore):
                 msg = _(
-                    "The given parameter {p!r} on calling method {m}() is not a sequence "
-                    "type.").format(p='data.datastore', m='from_summary')
+                    'The given parameter {p!r} on calling method {m}() is not a sequence '
+                    'type.').format(p='data.datastore', m='from_summary')
                 raise AssertionError(msg)
 
         if hasattr(data, 'network'):
             if not is_sequence(data.network):
                 msg = _(
-                    "The given parameter {p!r} on calling method {m}() is not a sequence "
-                    "type.").format(p='data.network', m='from_summary')
+                    'The given parameter {p!r} on calling method {m}() is not a sequence '
+                    'type.').format(p='data.network', m='from_summary')
                 raise AssertionError(msg)
 
         if hasattr(data, 'resourcePool') and data.resourcePool:
             if not hasattr(data.resourcePool, 'summary'):
-                failing_fields.append("data.resourcePool.summary")
+                failing_fields.append('data.resourcePool.summary')
 
         if len(failing_fields):
             msg = _(
-                "The given parameter {p!r} on calling method {m}() has failing "
-                "attributes").format(p='data', m='from_summary')
+                'The given parameter {p!r} on calling method {m}() has failing '
+                'attributes').format(p='data', m='from_summary')
             msg += ': ' + format_list(failing_fields, do_repr=True)
             raise AssertionError(msg)
 
 
 # =============================================================================
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_vmware-0.5.7/lib/fb_vmware/config/__init__.py` & `fb_vmware-0.6.0/lib/fb_vmware/config/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
+@summary: A module for providing a configuration for VSPhere.
+
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 by Frank Brehm, Berlin
-@summary: A module for providing a configuration for VSPhere
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard module
-import logging
 import copy
+import logging
 
 # Third party modules
 
-from fb_tools.common import is_sequence, to_bool, pp
-from fb_tools.multi_config import MultiConfigError, BaseMultiConfig
+from fb_tools.common import is_sequence
+from fb_tools.common import pp
+from fb_tools.common import to_bool
+from fb_tools.multi_config import BaseMultiConfig
 from fb_tools.multi_config import DEFAULT_ENCODING
-from fb_tools.obj import FbGenericBaseObject, FbBaseObject
+from fb_tools.multi_config import MultiConfigError
+from fb_tools.obj import FbBaseObject
+from fb_tools.obj import FbGenericBaseObject
 
 # Own modules
-
-from ..errors import WrongPortTypeError, WrongPortValueError
-
+from ..errors import WrongPortTypeError
+from ..errors import WrongPortValueError
 from ..xlate import XLATOR
 
 __version__ = '0.5.6'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 
@@ -41,30 +45,29 @@
 DEFAULT_PORT_HTTPS = 443
 
 MAX_PORT_NUMBER = (2 ** 16) - 1
 
 
 # =============================================================================
 class VmwareConfigError(MultiConfigError):
-    """Base error class for all exceptions happened during
-    execution this configured application"""
+    """Base error class for all exceptions in this module."""
 
     pass
 
 
 # =============================================================================
 class VSPhereConfigInfo(FbBaseObject):
     """Encapsulating all necessary data to connect to a VSPhere server."""
 
     # -------------------------------------------------------------------------
     def __init__(
         self, appname=None, verbose=0, version=__version__, base_dir=None,
             host=None, use_https=True, port=DEFAULT_VSPHERE_PORT, dc=DEFAULT_VSPHERE_DC,
             user=DEFAULT_VSPHERE_USER, password=None, initialized=False):
-
+        """Initialize the VSPhereConfigInfo object."""
         self._host = None
         self._port = DEFAULT_VSPHERE_PORT
         self._use_https = True
         self._dc = DEFAULT_VSPHERE_DC
         self._user = DEFAULT_VSPHERE_USER
         self._password = None
 
@@ -81,23 +84,22 @@
 
         if initialized:
             self.initialized = True
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True):
         """
-        Transforms the elements of the object into a dict
+        Transform the elements of the object into a dict.
 
         @param short: don't include local properties in resulting dict.
         @type short: bool
 
         @return: structure as dict
         @rtype:  dict
         """
-
         res = super(VSPhereConfigInfo, self).as_dict(short=short)
 
         res['host'] = self.host
         res['use_https'] = self.use_https
         res['port'] = self.port
         res['dc'] = self.dc
         res['user'] = self.user
@@ -107,38 +109,38 @@
         res['full_url'] = self.full_url
 
         return res
 
     # -----------------------------------------------------------
     @property
     def host(self):
-        """The host name (or IP address) of the VSPhere server."""
+        """Return the host name (or IP address) of the VSPhere server."""
         return self._host
 
     @host.setter
     def host(self, value):
         if value is None or str(value).strip() == '':
             self._host = None
             return
         self._host = str(value).strip().lower()
 
     # -----------------------------------------------------------
     @property
     def use_https(self):
-        """Should there be used HTTPS for communicating with the VSPhere server?"""
+        """Return the need for HTTPS for communicating with the VSPhere server."""
         return self._use_https
 
     @use_https.setter
     def use_https(self, value):
         self._use_https = to_bool(value)
 
     # -----------------------------------------------------------
     @property
     def port(self):
-        "The TCP port number of the VSPhere server."
+        """Return the TCP port number of the VSPhere server."""
         return self._port
 
     @port.setter
     def port(self, value):
         try:
             val = int(value)
             if val <= 0 or val > MAX_PORT_NUMBER:
@@ -147,35 +149,35 @@
             raise WrongPortTypeError(val, str(e))
 
         self._port = val
 
     # -----------------------------------------------------------
     @property
     def dc(self):
-        """The name of the datacenter in VSPhere to use."""
+        """Return the name of the datacenter in VSPhere to use."""
         return self._dc
 
     @dc.setter
     def dc(self, value):
         if value is None or str(value).strip() == '':
-            msg = _("An empty name for a VSPhere datacenter is not allowed.")
+            msg = _('An empty name for a VSPhere datacenter is not allowed.')
             LOG.warn(msg)
             return
         self._dc = str(value).strip()
 
     # -----------------------------------------------------------
     @property
     def user(self):
         """The user name to use to connect to the VSPhere server."""
         return self._user
 
     @user.setter
     def user(self, value):
         if value is None or str(value).strip() == '':
-            msg = _("An empty user name for connecting to a VSPhere datacenter is not allowed.")
+            msg = _('An empty user name for connecting to a VSPhere datacenter is not allowed.')
             LOG.warn(msg)
             return
         self._user = str(value).strip()
 
     # -----------------------------------------------------------
     @property
     def password(self):
@@ -248,15 +250,15 @@
         return '{s}://{u}{pw}@{h}{p}'.format(
             s=self.schema, u=self.user, pw=pw, h=self.host, p=port)
 
     # -------------------------------------------------------------------------
     @classmethod
     def from_config(
             cls, section_name, vsphere_name, section, appname=None, verbose=0, base_dir=None):
-
+        """Create a new VSPhereConfigInfo object based on the data from config."""
         info = cls(appname=appname, verbose=verbose, base_dir=base_dir, initialized=False)
 
         try:
 
             for key in section.keys():
 
                 value = section[key]
@@ -277,75 +279,73 @@
                     info.user = value
                     continue
                 if key.lower() == 'password':
                     info.password = value
                     continue
 
                 msg = _(
-                    "Unknown key {k!r} with value {v!r} for VSphere {vs!r} in section "
-                    "{sec!r} found.").format(k=key, v=value, vs=vsphere_name, sec=section_name)
+                    'Unknown key {k!r} with value {v!r} for VSphere {vs!r} in section '
+                    '{sec!r} found.').format(k=key, v=value, vs=vsphere_name, sec=section_name)
                 LOG.warn(msg)
 
         except Exception as e:
-            msg = _("{e} in section {sn!r} for VSphere {vs!r}:").format(
+            msg = _('{e} in section {sn!r} for VSphere {vs!r}:').format(
                 e=e.__class__.__name__, sn=section_name, vs=vsphere_name)
             msg += ' ' + str(e)
             raise VmwareConfigError(msg)
 
         if not info.host:
             msg = _(
-                "There must be given at least the VSPhere hostname in section {sn!r} "
-                "for VSphere {vs!r}.").format(vs=vsphere_name, sec=section_name)
+                'There must be given at least the VSPhere hostname in section {sn!r} '
+                'for VSphere {vs!r}.').format(vs=vsphere_name, sec=section_name)
             raise VmwareConfigError(msg)
 
         info.initialized = True
 
         return info
 
     # -------------------------------------------------------------------------
     def __repr__(self):
         """Typecasting into a string for reproduction."""
-
-        out = "<%s(" % (self.__class__.__name__)
+        out = '<%s(' % (self.__class__.__name__)
 
         fields = []
-        fields.append("appname={!r}".format(self.appname))
-        fields.append("host={!r}".format(self.host))
-        fields.append("use_https={!r}".format(self.use_https))
-        fields.append("port={!r}".format(self.port))
-        fields.append("dc={!r}".format(self.dc))
-        fields.append("user={!r}".format(self.user))
-        fields.append("password={!r}".format(self.password))
-        fields.append("verbose={!r}".format(self.verbose))
-        fields.append("base_dir={!r}".format(self.base_dir))
-        fields.append("initialized={!r}".format(self.initialized))
+        fields.append('appname={!r}'.format(self.appname))
+        fields.append('host={!r}'.format(self.host))
+        fields.append('use_https={!r}'.format(self.use_https))
+        fields.append('port={!r}'.format(self.port))
+        fields.append('dc={!r}'.format(self.dc))
+        fields.append('user={!r}'.format(self.user))
+        fields.append('password={!r}'.format(self.password))
+        fields.append('verbose={!r}'.format(self.verbose))
+        fields.append('base_dir={!r}'.format(self.base_dir))
+        fields.append('initialized={!r}'.format(self.initialized))
 
-        out += ", ".join(fields) + ")>"
+        out += ', '.join(fields) + ')>'
         return out
 
     # -------------------------------------------------------------------------
     def _repr(self):
-        """A typecasting into a string for reproduction only with relevant information."""
-
-        out = "<%s(" % (self.__class__.__name__)
+        """Typecasting into a string for reproduction only with relevant information."""
+        out = '<%s(' % (self.__class__.__name__)
 
         fields = []
-        fields.append("host={!r}".format(self.host))
-        fields.append("use_https={!r}".format(self.use_https))
-        fields.append("port={!r}".format(self.port))
-        fields.append("dc={!r}".format(self.dc))
-        fields.append("user={!r}".format(self.user))
-        fields.append("password={!r}".format(self.show_password))
+        fields.append('host={!r}'.format(self.host))
+        fields.append('use_https={!r}'.format(self.use_https))
+        fields.append('port={!r}'.format(self.port))
+        fields.append('dc={!r}'.format(self.dc))
+        fields.append('user={!r}'.format(self.user))
+        fields.append('password={!r}'.format(self.show_password))
 
-        out += ", ".join(fields) + ")>"
+        out += ', '.join(fields) + ')>'
         return out
 
     # -------------------------------------------------------------------------
     def __copy__(self):
-
+        """Return a new VSPhereConfigInfo object with data from current object copied in."""
         new = self.__class__(
             appname=self.appname, verbose=self.verbose, base_dir=self.base_dir, host=self.host,
             use_https=self.use_https, port=self.port, dc=self.dc, user=self.user,
             password=self.password, initialized=self.initialized)
 
         return new
 
@@ -353,55 +353,55 @@
 # =============================================================================
 class VSPhereConfigInfoDict(dict, FbGenericBaseObject):
     """A dictionary containing VSPhereConfigInfo as values and their VSPhere names as keys."""
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True):
         """
-        Transforms the elements of the object into a dict
+        Transform the elements of the object into a dict.
 
         @param short: don't include local properties in resulting dict.
         @type short: bool
 
         @return: structure as dict
         @rtype:  dict
         """
-
         res = super(VSPhereConfigInfoDict, self).as_dict(short=short)
 
         for key in self.keys():
             res[key] = self[key].as_dict(short=short)
 
         return res
 
     # -------------------------------------------------------------------------
     def __copy__(self):
-
+        """Return a new VSPhereConfigInfoDict object with data from current object copied in."""
         new = self.__class__()
 
         for key in self.keys():
             new[key] = copy.copy(self[key])
 
         return new
 
 
 # =============================================================================
 class VmwareConfiguration(BaseMultiConfig):
     """
-    A class for providing a configuration for an arbitrary Vmware Application
-    and methods to read it from configuration files.
+    A class for providing a configuration for an arbitrary Vmware Application.
+
+    There are also methods to read it from configuration files.
     """
 
     # -------------------------------------------------------------------------
     def __init__(
         self, appname=None, verbose=0, version=__version__, base_dir=None,
             append_appname_to_stems=True, additional_stems=None, config_dir=DEFAULT_CONFIG_DIR,
             additional_config_file=None, additional_cfgdirs=None, encoding=DEFAULT_ENCODING,
             use_chardet=True, initialized=False):
-
+        """Initialize a VmwareConfiguration object."""
         add_stems = []
         if additional_stems:
             if is_sequence(additional_stems):
                 for stem in additional_stems:
                     add_stems.append(stem)
             else:
                 add_stems.append(additional_stems)
@@ -422,34 +422,34 @@
         )
 
         if initialized:
             self.initialized = True
 
     # -------------------------------------------------------------------------
     def eval_section(self, section_name):
-
+        """Evaluate a particular configuration section."""
         super(VmwareConfiguration, self).eval_section(section_name)
         sn = section_name.lower()
 
         if sn == 'vsphere' or sn.startswith('vsphere:'):
 
             section = self.cfg[section_name]
 
             if self.verbose > 2:
                 LOG.debug(
-                    _("Evaluating config section {!r}:").format(section_name) + '\n' + pp(section))
+                    _('Evaluating config section {!r}:').format(section_name) + '\n' + pp(section))
 
             if sn == 'vsphere':
                 return self._eval_bare_vsphere(section_name, section)
 
             if sn.startswith('vsphere:'):
                 vsphere_name = sn.replace('vsphere:', '').strip()
                 return self._eval_vsphere_instance(section_name, vsphere_name, section)
 
-            LOG.error(_("Empty VSphere name found."))
+            LOG.error(_('Empty VSphere name found.'))
 
     # -------------------------------------------------------------------------
     def _eval_bare_vsphere(self, section_name, section):
 
         for vsphere_name in section.keys():
             sub_section = section[vsphere_name]
             vs_name = vsphere_name.strip()
@@ -464,14 +464,14 @@
                 verbose=self.verbose, base_dir=self.base_dir)
             self.vsphere[vsphere_name] = vsphere_info
         except VmwareConfigError as e:
             LOG.error(str(e))
 
 
 # =============================================================================
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_vmware-0.5.7/lib/fb_vmware/connect.py` & `fb_vmware-0.6.0/lib/fb_vmware/connect.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,83 +1,73 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
+@summary: The module for a VSphere connection object.
+
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 by Frank Brehm, Berlin
-@summary: The module for a VSphere connection object.
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
+import datetime
 import logging
 import re
-import uuid
 import socket
 import time
-import datetime
-
-from numbers import Number
-
+import uuid
 try:
     from collections.abc import Sequence
 except ImportError:
     from collections import Sequence
+from numbers import Number
 
 # Third party modules
+from fb_tools.common import RE_TF_NAME, pp
+from fb_tools.errors import HandlerError
+
 from pyVmomi import vim, vmodl
+
 import requests
-import urllib3
 
-from fb_tools.common import pp, RE_TF_NAME
-from fb_tools.errors import HandlerError
+import urllib3
 
 # Own modules
-from .base import BaseVsphereHandler, DEFAULT_TZ_NAME
-
-from .config import DEFAULT_VSPHERE_CLUSTER
-
 from .about import VsphereAboutInfo
-
-from .dc import VsphereDatacenter
-
+from .base import BaseVsphereHandler, DEFAULT_TZ_NAME
 from .cluster import VsphereCluster
-
+from .config import DEFAULT_VSPHERE_CLUSTER
 from .datastore import VsphereDatastore, VsphereDatastoreDict
-
+from .dc import VsphereDatacenter
 from .ds_cluster import VsphereDsCluster, VsphereDsClusterDict
-
-from .network import VsphereNetwork, VsphereNetworkDict
-
-from .iface import VsphereVmInterface
-
+from .errors import TimeoutCreateVmError
+from .errors import VSphereDatacenterNotFoundError
+from .errors import VSphereExpectedError
+from .errors import VSphereNoDatastoresFoundError
+from .errors import VSphereVmNotFoundError
 from .host import VsphereHost
-
+from .iface import VsphereVmInterface
+from .network import VsphereNetwork, VsphereNetworkDict
 from .vm import VsphereVm, VsphereVmList
-
-from .errors import VSphereExpectedError, TimeoutCreateVmError, VSphereVmNotFoundError
-from .errors import VSphereDatacenterNotFoundError, VSphereNoDatastoresFoundError
-
 from .xlate import XLATOR
 
-__version__ = '1.9.3'
+__version__ = '1.9.4'
 LOG = logging.getLogger(__name__)
 
 DEFAULT_OS_VERSION = 'oracleLinux8_64Guest'
 DEFAULT_VM_CFG_VERSION = 'vmx-14'
 
 _ = XLATOR.gettext
 ngettext = XLATOR.ngettext
 
 
 # =============================================================================
 class VsphereConnection(BaseVsphereHandler):
-    """
-    Class for a VSphere connection handler object.
-    """
+    """Class for a VSphere connection handler object."""
 
     re_local_ds = re.compile(r'^local[_-]', re.IGNORECASE)
     vmw_api_version_to_hw_version = {
         '5.0': 8,
         '5.1': 9,
         '5.5': 10,
         '6.0': 11,
@@ -90,15 +80,15 @@
     }
 
     # -------------------------------------------------------------------------
     def __init__(
         self, connect_info, appname=None, verbose=0, version=__version__, base_dir=None,
             cluster=DEFAULT_VSPHERE_CLUSTER, auto_close=True, simulate=None,
             force=None, terminal_has_colors=False, tz=DEFAULT_TZ_NAME, initialized=False):
-
+        """Initialize a VsphereConnection object."""
         self.datastores = VsphereDatastoreDict()
         self.ds_clusters = VsphereDsClusterDict()
         self.networks = VsphereNetworkDict()
         self.about = None
         self.dc_obj = None
 
         self.ds_mapping = {}
@@ -117,20 +107,19 @@
         )
 
         self.initialized = initialized
 
     # -------------------------------------------------------------------------
     def __repr__(self):
         """Typecasting into a string for reproduction."""
-
         return self._repr()
 
     # -------------------------------------------------------------------------
     def get_about(self, disconnect=False):
-
+        """Get the 'about' information from VSphere as a VsphereAboutInfo object."""
         LOG.debug(_("Trying to get some 'about' information from VSphere."))
 
         try:
 
             if not self.service_instance:
                 self.connect()
 
@@ -148,49 +137,49 @@
             raise VSphereExpectedError(msg)
 
         finally:
             if disconnect:
                 self.disconnect()
 
         if self.verbose:
-            LOG.info(_("VSphere version: {!r}").format(self.about.os_version))
+            LOG.info(_('VSphere version: {!r}').format(self.about.os_version))
         if self.verbose > 1:
-            LOG.debug(_("Found VSphere about-information:") + '\n' + pp(self.about.as_dict()))
+            LOG.debug(_('Found VSphere about-information:') + '\n' + pp(self.about.as_dict()))
 
     # -------------------------------------------------------------------------
     def get_datacenter(self, disconnect=False):
-
-        LOG.debug(_("Trying to get datacenter from VSphere ..."))
+        """Get the datacenter from VSphere as a VsphereDatacenter object."""
+        LOG.debug(_('Trying to get datacenter from VSphere ...'))
 
         try:
 
             if not self.service_instance:
                 self.connect()
 
             content = self.service_instance.RetrieveContent()
             dc_obj = self.get_obj(content, [vim.Datacenter], self.dc)
             if not dc_obj:
                 raise VSphereDatacenterNotFoundError(self.dc)
 
             self.dc_obj = VsphereDatacenter.from_summary(
                 dc_obj, appname=self.appname, verbose=self.verbose, base_dir=self.base_dir)
-            LOG.debug(_("Found VSphere datacenter {!r}.").format(self.dc_obj.name))
+            LOG.debug(_('Found VSphere datacenter {!r}.').format(self.dc_obj.name))
             if self.verbose > 2:
-                LOG.debug(_("Info about datacenter:") + '\n' + str(self.dc_obj))
+                LOG.debug(_('Info about datacenter:') + '\n' + str(self.dc_obj))
 
         finally:
             if disconnect:
                 self.disconnect()
 
         return
 
     # -------------------------------------------------------------------------
     def get_clusters(self, disconnect=False):
-
-        LOG.debug(_("Trying to get all clusters from VSphere ..."))
+        """Get all clusters from VSphere as VsphereCluster objects."""
+        LOG.debug(_('Trying to get all clusters from VSphere ...'))
 
         self.clusters = []
 
         try:
 
             if not self.service_instance:
                 self.connect()
@@ -206,20 +195,20 @@
             if disconnect:
                 self.disconnect()
 
         if self.verbose > 2:
             out = []
             for cluster in self.clusters:
                 out.append(cluster.as_dict())
-            LOG.debug(_("Found clusters:") + '\n' + pp(out))
+            LOG.debug(_('Found clusters:') + '\n' + pp(out))
         elif self.verbose:
             out = []
             for cluster in self.clusters:
                 out.append(cluster.name)
-            LOG.debug(_("Found clusters:") + '\n' + pp(out))
+            LOG.debug(_('Found clusters:') + '\n' + pp(out))
 
     # -------------------------------------------------------------------------
     def _get_clusters(self, child, depth=1):
 
         if hasattr(child, 'childEntity'):
             if depth > self.max_search_depth:
                 return
@@ -236,37 +225,37 @@
                     obj_name = _('Found cluster')
                 host_label = ngettext('host', 'hosts', cluster.hosts_total)
                 cpus_label = ngettext('CPU', 'CPUs', cluster.cpu_cores)
                 thr_label = ngettext('thread', 'threads', cluster.cpu_threads)
                 nw_label = ngettext('network', 'networks', len(cluster.networks))
                 ds_label = ngettext('datastore', 'datastores', len(cluster.datastores))
                 LOG.debug(_(
-                    "{on} {cl!r}, {h} {h_l}, {cpu} {cpu_l}, {thr} {t_l}, "
-                    "{mem:0.1f} GiB Memory, {net} {nw_l} and {ds} {ds_l}.").format(
+                    '{on} {cl!r}, {h} {h_l}, {cpu} {cpu_l}, {thr} {t_l}, '
+                    '{mem:0.1f} GiB Memory, {net} {nw_l} and {ds} {ds_l}.').format(
                     on=obj_name, cl=cluster.name, h=cluster.hosts_total, h_l=host_label,
                     cpu=cluster.cpu_cores, cpu_l=cpus_label, thr=cluster.cpu_threads,
                     t_l=thr_label, mem=cluster.mem_gb_total, net=len(cluster.networks),
                     nw_l=nw_label, ds=len(cluster.datastores), ds_l=ds_label))
             self.clusters.append(cluster)
 
         return
 
     # -------------------------------------------------------------------------
     def get_cluster_by_name(self, cl_name):
-
+        """Return a VsphereCluster from cluster list by the given cluster name."""
         for cluster in self.clusters:
             if cluster.name.lower() == cl_name.lower():
                 return cluster
 
         return None
 
     # -------------------------------------------------------------------------
     def get_datastores(self, disconnect=False):
-
-        LOG.debug(_("Trying to get all datastores from VSphere ..."))
+        """Get all datastores from VSphere as VsphereDatastore objects."""
+        LOG.debug(_('Trying to get all datastores from VSphere ...'))
         self.datastores = VsphereDatastoreDict()
         self.ds_mapping = {}
 
         try:
 
             if not self.service_instance:
                 self.connect()
@@ -281,55 +270,55 @@
         finally:
             if disconnect:
                 self.disconnect()
 
         if self.datastores:
             if self.verbose > 1:
                 if self.verbose > 3:
-                    LOG.debug(_("Found datastores:") + '\n' + pp(self.datastores.as_list()))
+                    LOG.debug(_('Found datastores:') + '\n' + pp(self.datastores.as_list()))
                 else:
-                    LOG.debug(_("Found datastores:") + '\n' + pp(list(self.datastores.keys())))
+                    LOG.debug(_('Found datastores:') + '\n' + pp(list(self.datastores.keys())))
         else:
             raise VSphereNoDatastoresFoundError()
 
         for (ds_name, ds) in self.datastores.items():
             self.ds_mapping[ds_name] = ds.tf_name
 
         if self.verbose > 2:
-            LOG.debug(_("Datastore mappings:") + '\n' + pp(self.ds_mapping))
+            LOG.debug(_('Datastore mappings:') + '\n' + pp(self.ds_mapping))
 
     # -------------------------------------------------------------------------
     def _get_datastores(self, child, depth=1):
 
         if hasattr(child, 'childEntity'):
             if depth > self.max_search_depth:
                 return
             for sub_child in child.childEntity:
                 self._get_datastores(sub_child, depth + 1)
             return
 
         if isinstance(child, vim.Datastore):
             if self.re_local_ds.match(child.summary.name):
                 if self.verbose > 2:
-                    LOG.debug(_("Datastore {!r} seems to be local.").format(child.summary.name))
+                    LOG.debug(_('Datastore {!r} seems to be local.').format(child.summary.name))
                 return
             ds = VsphereDatastore.from_summary(
                 child, appname=self.appname, verbose=self.verbose, base_dir=self.base_dir)
             if self.verbose > 2:
                 LOG.debug(
-                    _("Found datastore {ds!r} of type {t!r}, capacity {c:0.1f} GByte.").format(
+                    _('Found datastore {ds!r} of type {t!r}, capacity {c:0.1f} GByte.').format(
                         ds=ds.name, t=ds.storage_type, c=ds.capacity_gb))
             self.datastores.append(ds)
 
         return
 
     # -------------------------------------------------------------------------
     def get_ds_clusters(self, disconnect=False):
-
-        LOG.debug(_("Trying to get all datastore clusters from VSphere ..."))
+        """Get all datastores clusters from VSphere as VsphereDsCluster objects."""
+        LOG.debug(_('Trying to get all datastore clusters from VSphere ...'))
         self.ds_clusters = VsphereDsClusterDict()
         self.ds_cluster_mapping = {}
 
         try:
 
             if not self.service_instance:
                 self.connect()
@@ -345,32 +334,32 @@
             if disconnect:
                 self.disconnect()
 
         if self.ds_clusters:
             if self.verbose > 1:
                 if self.verbose > 3:
                     LOG.debug(
-                        _("Found datastore clusters:") + '\n' + pp(self.ds_clusters.as_list()))
+                        _('Found datastore clusters:') + '\n' + pp(self.ds_clusters.as_list()))
                 else:
                     LOG.debug(
-                        _("Found datastore clusters:") + '\n' + pp(list(self.ds_clusters.keys())))
+                        _('Found datastore clusters:') + '\n' + pp(list(self.ds_clusters.keys())))
         else:
-            LOG.warning(_("No VSphere datastore clusters found."))
+            LOG.warning(_('No VSphere datastore clusters found.'))
 
         for (dsc_name, dsc) in self.ds_clusters.items():
             self.ds_cluster_mapping[dsc_name] = dsc.tf_name
 
         if self.verbose > 2:
-            LOG.debug(_("Datastore cluster mappings:") + '\n' + pp(self.ds_cluster_mapping))
+            LOG.debug(_('Datastore cluster mappings:') + '\n' + pp(self.ds_cluster_mapping))
 
     # -------------------------------------------------------------------------
     def _get_ds_clusters(self, child, depth=1):
 
         if self.verbose > 3:
-            LOG.debug(_("Found a {} child.").format(child.__class__.__name__))
+            LOG.debug(_('Found a {} child.').format(child.__class__.__name__))
 
         if hasattr(child, 'childEntity'):
             if depth > self.max_search_depth:
                 return
             for sub_child in child.childEntity:
                 self._get_ds_clusters(sub_child, depth + 1)
 
@@ -379,16 +368,16 @@
                 child, appname=self.appname, verbose=self.verbose, base_dir=self.base_dir)
             self.ds_clusters.append(ds)
 
         return
 
     # -------------------------------------------------------------------------
     def get_networks(self, disconnect=False):
-
-        LOG.debug(_("Trying to get all networks from VSphere ..."))
+        """Get all networks from VSphere as VsphereNetwork objects."""
+        LOG.debug(_('Trying to get all networks from VSphere ...'))
         self.networks = VsphereNetworkDict()
         self.network_mapping = {}
 
         try:
 
             if not self.service_instance:
                 self.connect()
@@ -402,35 +391,35 @@
 
         finally:
             if disconnect:
                 self.disconnect()
 
         if self.networks:
             msg = ngettext(
-                "Found one VSphere network.", "Found {n} VSphere networks.", len(self.networks))
+                'Found one VSphere network.', 'Found {n} VSphere networks.', len(self.networks))
             LOG.debug(msg.format(n=len(self.networks)))
             if self.verbose > 2:
                 if self.verbose > 3:
-                    LOG.debug(_("Found VSphere networks:") + '\n' + pp(self.networks.as_list()))
+                    LOG.debug(_('Found VSphere networks:') + '\n' + pp(self.networks.as_list()))
                 else:
-                    LOG.debug(_("Found VSphere networks:") + '\n' + pp(list(self.networks.keys())))
+                    LOG.debug(_('Found VSphere networks:') + '\n' + pp(list(self.networks.keys())))
         else:
-            LOG.error(_("No VSphere networks found."))
+            LOG.error(_('No VSphere networks found.'))
 
         for (net_name, net) in self.networks.items():
             self.network_mapping[net_name] = net.tf_name
 
         if self.verbose > 2:
-            LOG.debug(_("Network mappings:") + '\n' + pp(self.network_mapping))
+            LOG.debug(_('Network mappings:') + '\n' + pp(self.network_mapping))
 
     # -------------------------------------------------------------------------
     def _get_networks(self, child, depth=1):
 
         if self.verbose > 3:
-            LOG.debug(_("Found a {} child.").format(child.__class__.__name__))
+            LOG.debug(_('Found a {} child.').format(child.__class__.__name__))
 
         if hasattr(child, 'childEntity'):
             if depth > self.max_search_depth:
                 return
             for sub_child in child.childEntity:
                 self._get_networks(sub_child, depth + 1)
 
@@ -439,25 +428,25 @@
                 child, appname=self.appname, verbose=self.verbose, base_dir=self.base_dir)
             self.networks.append(ds)
 
         return
 
     # -------------------------------------------------------------------------
     def get_hosts(self, re_name=None, vsphere_name=None, disconnect=False):
-
+        """Get all physical hosts from VSphere as VsphereHost objects."""
         if re_name is not None:
             if not hasattr(re_name, 'match'):
-                msg = _("Parameter {p!r} => {r!r} seems not to be a regex object.").format(
+                msg = _('Parameter {p!r} => {r!r} seems not to be a regex object.').format(
                     p='re_name', r=re_name)
                 raise TypeError(msg)
             LOG.debug(_(
-                "Trying to get all host systems from VSphere with name pattern {!r} ...").format(
+                'Trying to get all host systems from VSphere with name pattern {!r} ...').format(
                 re_name.pattern))
         else:
-            LOG.debug(_("Trying to get all host systems from VSphere ..."))
+            LOG.debug(_('Trying to get all host systems from VSphere ...'))
 
         self.clusters = []
         self.hosts = {}
 
         try:
 
             if not self.service_instance:
@@ -476,26 +465,26 @@
                 self.disconnect()
 
         if self.verbose > 2:
             out = []
             for host_name in self.hosts.keys():
                 host = self.hosts[host_name]
                 out.append(host.as_dict())
-            LOG.debug(_("Found hosts:") + '\n' + pp(out))
+            LOG.debug(_('Found hosts:') + '\n' + pp(out))
         elif self.verbose:
             out = []
             for host_name in self.hosts.keys():
                 out.append(host_name)
-            LOG.debug(_("Found hosts:") + '\n' + pp(out))
+            LOG.debug(_('Found hosts:') + '\n' + pp(out))
 
     # -------------------------------------------------------------------------
     def _get_hosts(self, child, depth=1, re_name=None, vsphere_name=None, cluster_name=None):
 
         if self.verbose > 3:
-            LOG.debug(_("Checking {o}-object in cluster {c!r} ...").format(
+            LOG.debug(_('Checking {o}-object in cluster {c!r} ...').format(
                 o=child.__class__.__name__, c=cluster_name))
 
         if isinstance(child, (vim.ClusterComputeResource, vim.ComputeResource)):
             cluster = VsphereCluster.from_summary(
                 child, appname=self.appname, verbose=self.verbose, base_dir=self.base_dir)
             cluster_name = cluster.name
             if self.verbose > 1:
@@ -504,16 +493,16 @@
                     obj_name = _('Found cluster')
                 host_label = ngettext('host', 'hosts', cluster.hosts_total)
                 cpus_label = ngettext('CPU', 'CPUs', cluster.cpu_cores)
                 thr_label = ngettext('thread', 'threads', cluster.cpu_threads)
                 nw_label = ngettext('network', 'networks', len(cluster.networks))
                 ds_label = ngettext('datastore', 'datastores', len(cluster.datastores))
                 LOG.debug(_(
-                    "{on} {cl!r}, {h} {h_l}, {cpu} {cpu_l}, {thr} {t_l}, "
-                    "{mem:0.1f} GiB Memory, {net} {nw_l} and {ds} {ds_l}.").format(
+                    '{on} {cl!r}, {h} {h_l}, {cpu} {cpu_l}, {thr} {t_l}, '
+                    '{mem:0.1f} GiB Memory, {net} {nw_l} and {ds} {ds_l}.').format(
                     on=obj_name, cl=cluster.name, h=cluster.hosts_total, h_l=host_label,
                     cpu=cluster.cpu_cores, cpu_l=cpus_label, thr=cluster.cpu_threads,
                     t_l=thr_label, mem=cluster.mem_gb_total, net=len(cluster.networks),
                     nw_l=nw_label, ds=len(cluster.datastores), ds_l=ds_label))
 
             self.clusters.append(cluster)
 
@@ -521,51 +510,51 @@
 
                 hostname = host_def.summary.config.name
 
                 if re_name is not None:
                     if not re_name.search(hostname):
                         continue
 
-                LOG.debug(_("Found host {h!r} in cluster {c!r}.").format(
+                LOG.debug(_('Found host {h!r} in cluster {c!r}.').format(
                     h=hostname, c=cluster_name))
                 host = VsphereHost.from_summary(
                     host_def, vsphere=vsphere_name, cluster_name=cluster_name,
                     appname=self.appname, verbose=self.verbose, base_dir=self.base_dir)
                 self.hosts[host.name] = host
 
         return
 
     # -------------------------------------------------------------------------
     def get_vm(
             self, vm_name, vsphere_name=None, no_error=False, disconnect=False, as_vmw_obj=False,
             as_obj=False, name_only=False):
-
+        """Get a virtual machine from VSphere as VsphereVm object by its name."""
         pattern_name = r'^\s*' + re.escape(vm_name) + r'\s*$'
-        LOG.debug(_("Searching for VM {n!r} (pattern: {p!r}) in VSPhere {v!r} ...").format(
+        LOG.debug(_('Searching for VM {n!r} (pattern: {p!r}) in VSPhere {v!r} ...').format(
             n=vm_name, p=pattern_name, v=vsphere_name))
         re_name = re.compile(pattern_name, re.IGNORECASE)
         vmlist = self.get_vms(
             re_name, vsphere_name=vsphere_name, disconnect=disconnect, as_vmw_obj=as_vmw_obj,
             as_obj=as_obj, name_only=name_only, stop_at_found=True)
 
         if not vmlist:
-            msg = _("VSphere VM {!r} not found.").format(vm_name)
+            msg = _('VSphere VM {!r} not found.').format(vm_name)
             if no_error:
                 LOG.debug(msg)
             else:
                 LOG.error(msg)
             return None
 
         return vmlist[0]
 
     # -------------------------------------------------------------------------
     def _dict_from_vim_obj(self, vm, cur_path):
 
         if not isinstance(vm, vim.VirtualMachine):
-            msg = _("Parameter {t!r} must be a {e}, {v!r} was given.").format(
+            msg = _('Parameter {t!r} must be a {e}, {v!r} was given.').format(
                 t='vm', e='vim.VirtualMachine', v=vm)
             raise TypeError(msg)
 
         summary = vm.summary
         vm_config = summary.config
 
         vm_info = {}
@@ -644,25 +633,25 @@
             vm_info['interfaces'][unit_nr] = iface
         return vm_info
 
     # -------------------------------------------------------------------------
     def get_vms(
             self, re_name, vsphere_name=None, is_template=None, disconnect=False, as_vmw_obj=False,
             as_obj=False, name_only=False, stop_at_found=False):
-
+        """Get all virtual machines from VSphere as VsphereVm objects."""
         if not hasattr(re_name, 'match'):
-            msg = _("Parameter {p!r} => {r!r} seems not to be a regex object.").format(
+            msg = _('Parameter {p!r} => {r!r} seems not to be a regex object.').format(
                 p='re_name', r=re_name)
             raise TypeError(msg)
         if as_vmw_obj and as_obj:
-            msg = _("Parameter {p1!r} and {p2!r} may not be {w!r} at the same time.").format(
+            msg = _('Parameter {p1!r} and {p2!r} may not be {w!r} at the same time.').format(
                 p1='as_vmw_obj', p2='as_obj', w=True)
             raise ValueError(msg)
 
-        LOG.debug(_("Trying to get list of VMs with name pattern {!r} ...").format(
+        LOG.debug(_('Trying to get list of VMs with name pattern {!r} ...').format(
             re_name.pattern))
         vm_list = []
         if as_obj:
             vm_list = VsphereVmList(
                 appname=self.appname, verbose=self.verbose, base_dir=self.base_dir,
                 initialized=True)
 
@@ -674,28 +663,28 @@
             dc = self.get_obj(content, [vim.Datacenter], self.dc)
             if not dc:
                 raise VSphereDatacenterNotFoundError(self.dc)
 
             for child in dc.vmFolder.childEntity:
                 path = child.name
                 if self.verbose > 1:
-                    LOG.debug(_("Searching in path {!r} ...").format(path))
+                    LOG.debug(_('Searching in path {!r} ...').format(path))
                 vms = self._get_vms(
                     child, re_name, vsphere_name=vsphere_name, is_template=is_template,
                     as_vmw_obj=as_vmw_obj, as_obj=as_obj, name_only=name_only,
                     stop_at_found=stop_at_found)
                 if vms:
                     vm_list += vms
 
         finally:
             if disconnect:
                 self.disconnect()
 
         msg = ngettext(
-            "Found one VM with pattern {p!r}.", "Found {no} VMs with pattern {p!r}.", len(vm_list))
+            'Found one VM with pattern {p!r}.', 'Found {no} VMs with pattern {p!r}.', len(vm_list))
         LOG.debug(msg.format(no=len(vm_list), p=re_name.pattern))
 
         return vm_list
 
     # -------------------------------------------------------------------------
     def _get_vms(
             self, child, re_name, cur_path='', vsphere_name=None, is_template=None, depth=1,
@@ -722,31 +711,31 @@
         if isinstance(child, vim.VirtualMachine):
 
             summary = child.summary
             vm_config = summary.config
             vm_name = vm_config.name
 
             if self.verbose > 3:
-                LOG.debug(_("Checking VM {!r} ...").format(vm_name))
+                LOG.debug(_('Checking VM {!r} ...').format(vm_name))
             if is_template is not None:
                 if self.verbose > 3:
-                    msg = _("Checking VM {!r} for being a template ...")
+                    msg = _('Checking VM {!r} for being a template ...')
                     if not is_template:
-                        msg = _("Checking VM {!r} for being not a template ...")
+                        msg = _('Checking VM {!r} for being not a template ...')
                     LOG.debug(msg.format(vm_name))
                 if is_template and not vm_config.template:
                     return []
                 if not is_template and vm_config.template:
                     return []
 
             if self.verbose > 3:
-                LOG.debug(_("Checking VM {!r} for pattern.").format(vm_name))
+                LOG.debug(_('Checking VM {!r} for pattern.').format(vm_name))
             if re_name.search(vm_name):
                 if self.verbose > 2:
-                    LOG.debug(_("Found VM {!r}.").format(vm_name))
+                    LOG.debug(_('Found VM {!r}.').format(vm_name))
                 if name_only:
                     vm_list.append((vm_name, cur_path))
                 elif as_obj:
                     vm = VsphereVm.from_summary(
                         child, cur_path, vsphere=vsphere_name,
                         appname=self.appname, verbose=self.verbose, base_dir=self.base_dir)
                     vm_list.append(vm)
@@ -786,15 +775,15 @@
             if stop_at_found and vm_list:
                 break
 
         return vm_list
 
     # -------------------------------------------------------------------------
     def poweron_vm(self, vm, max_wait=20, disconnect=False):
-
+        """Power on the given virtual machine."""
         try:
 
             if not self.service_instance:
                 self.connect()
 
             if isinstance(vm, vim.VirtualMachine):
                 vm_obj = vm
@@ -802,30 +791,30 @@
             else:
                 vm_name = vm
                 vm_obj = self.get_vm(vm, as_vmw_obj=True)
                 if not vm_obj:
                     raise VSphereVmNotFoundError(vm)
 
             if vm_obj.runtime.powerState.lower() == 'poweredon':
-                LOG.info(_("VM {!r} is already powered on.").format(vm_name))
+                LOG.info(_('VM {!r} is already powered on.').format(vm_name))
                 return
 
-            LOG.info(_("Powering on VM {!r} ...").format(vm_name))
+            LOG.info(_('Powering on VM {!r} ...').format(vm_name))
 
             task = vm_obj.PowerOnVM_Task()
             self.wait_for_tasks([task], max_wait=max_wait)
-            LOG.debug(_("VM {!r} successful powered on.").format(vm_name))
+            LOG.debug(_('VM {!r} successful powered on.').format(vm_name))
 
         finally:
             if disconnect:
                 self.disconnect()
 
     # -------------------------------------------------------------------------
     def poweroff_vm(self, vm, max_wait=20, disconnect=False):
-
+        """Power off the given virtual machine."""
         try:
 
             if not self.service_instance:
                 self.connect()
 
             if isinstance(vm, vim.VirtualMachine):
                 vm_obj = vm
@@ -833,47 +822,48 @@
             else:
                 vm_name = vm
                 vm_obj = self.get_vm(vm, as_vmw_obj=True)
                 if not vm_obj:
                     raise VSphereVmNotFoundError(vm)
 
             if vm_obj.runtime.powerState.lower() == 'poweredoff':
-                LOG.info(_("VM {!r} is already powered off.").format(vm_name))
+                LOG.info(_('VM {!r} is already powered off.').format(vm_name))
                 return
 
-            LOG.info(_("Powering off VM {!r} ...").format(vm_name))
+            LOG.info(_('Powering off VM {!r} ...').format(vm_name))
 
             task = vm_obj.PowerOffVM_Task()
             self.wait_for_tasks([task], max_wait=max_wait)
-            LOG.debug(_("VM {!r} successful powered off.").format(vm_name))
+            LOG.debug(_('VM {!r} successful powered off.').format(vm_name))
 
         finally:
             if disconnect:
                 self.disconnect()
 
     # -------------------------------------------------------------------------
     def ensure_vm_folders(self, folders, disconnect=False):
-        LOG.debug(_("Ensuring existence of VSphere VM folders:") + '\n' + pp(folders))
+        """Ensure existence of the given VSphere VM folders."""
+        LOG.debug(_('Ensuring existence of VSphere VM folders:') + '\n' + pp(folders))
         try:
 
             if not self.service_instance:
                 self.connect()
 
             for folder in folders:
                 self.ensure_vm_folder(folder, disconnect=False)
 
         finally:
             if disconnect:
                 self.disconnect()
 
     # -------------------------------------------------------------------------
     def get_vm_folder(self, folder, disconnect=False):
-
+        """Get the given VSphere VM folder as a vim.Folder object."""
         if self.verbose > 1:
-            LOG.debug(_("Trying to get VM folder object for path {!r}.").format(folder))
+            LOG.debug(_('Trying to get VM folder object for path {!r}.').format(folder))
 
         paths = []
         parts = folder.split('/')
         for i in range(0, len(parts)):
             path = '/'.join(parts[0:i + 1])
             paths.append(path)
 
@@ -890,26 +880,26 @@
             folder_object = None
 
             index = 0
             last = False
             for part in parts:
                 abs_path = '/' + paths[index]
                 if self.verbose > 1:
-                    LOG.debug(_("Checking single VM folder {i}: {f!r}.").format(
+                    LOG.debug(_('Checking single VM folder {i}: {f!r}.').format(
                         i=index, f=abs_path))
                 if index == len(parts) - 1:
                     last = True
 
                 for child in parent_folder.childEntity:
                     if not isinstance(child, vim.Folder):
                         continue
                     if child.name != part:
                         continue
                     if self.verbose > 1:
-                        LOG.debug(_("Found VM folder {n}, parent: {p}").format(
+                        LOG.debug(_('Found VM folder {n}, parent: {p}').format(
                             n=child.name, p=parent_folder.name))
                     parent_folder = child
                     if last:
                         folder_object = child
                 index += 1
                 if last:
                     break
@@ -918,16 +908,16 @@
 
         finally:
             if disconnect:
                 self.disconnect()
 
     # -------------------------------------------------------------------------
     def ensure_vm_folder(self, folder, disconnect=False):
-
-        LOG.debug(_("Ensuring existence of VSphere VM folder {!r}.").format(folder))
+        """Ensure existence of the given VSphere VM folder."""
+        LOG.debug(_('Ensuring existence of VSphere VM folder {!r}.').format(folder))
 
         paths = []
         parts = folder.split('/')
         for i in range(0, len(parts)):
             path = '/'.join(parts[0:i + 1])
             paths.append(path)
 
@@ -944,17 +934,17 @@
 
             index = 0
             for part in parts:
 
                 abs_path = '/' + paths[index]
                 folder_object = self.get_vm_folder(paths[index], disconnect=False)
                 if folder_object:
-                    LOG.debug(_("VM Folder {!r} already exists.").format(abs_path))
+                    LOG.debug(_('VM Folder {!r} already exists.').format(abs_path))
                 else:
-                    LOG.info(_("Creating VM folder {!r} ...").format(abs_path))
+                    LOG.info(_('Creating VM folder {!r} ...').format(abs_path))
                     if self.simulate:
                         LOG.debug(_("Simulation mode, don't creating it."))
                         break
                     parent_folder = root_folder
                     if index != 0:
                         parent_folder = self.get_vm_folder(paths[index - 1], disconnect=False)
                     parent_folder.CreateFolder(part)
@@ -963,31 +953,31 @@
         finally:
             if disconnect:
                 self.disconnect()
 
     # -------------------------------------------------------------------------
     def wait_for_tasks(
             self, tasks, poll_time=0.1, disconnect=False, max_wait=None, start_time=None):
-
-        LOG.debug(_("Waiting for tasks to finish ..."))
+        """Wat for finishing the given VSPhere task."""
+        LOG.debug(_('Waiting for tasks to finish ...'))
         if not start_time:
             start_time = time.time()
 
         try:
 
             if not self.service_instance:
                 self.connect()
 
             property_collector = self.service_instance.content.propertyCollector
             task_list = [str(task) for task in tasks]
             if max_wait:
-                LOG.debug(_("Waiting at most {m} seconds for tasks {t} to finish ...").format(
+                LOG.debug(_('Waiting at most {m} seconds for tasks {t} to finish ...').format(
                     m=max_wait, t=task_list))
             else:
-                LOG.debug(_("Waiting for tasks {} to finish ...").format(task_list))
+                LOG.debug(_('Waiting for tasks {} to finish ...').format(task_list))
             # Create filter
             obj_specs = [vmodl.query.PropertyCollector.ObjectSpec(obj=task) for task in tasks]
             property_spec = vmodl.query.PropertyCollector.PropertySpec(
                 type=vim.Task, pathSet=[], all=True)
             filter_spec = vmodl.query.PropertyCollector.FilterSpec()
             filter_spec.objectSet = obj_specs
             filter_spec.propSet = [property_spec]
@@ -999,15 +989,15 @@
                     update = property_collector.WaitForUpdates(version)
                     for filter_set in update.filterSet:
                         if max_wait is not None and max_wait > 0:
                             time_diff = time.time() - start_time
                             if time_diff >= max_wait:
                                 return False
                         time.sleep(poll_time)
-                        LOG.debug(_("Waiting ..."))
+                        LOG.debug(_('Waiting ...'))
                         for obj_set in filter_set.objectSet:
                             task = obj_set.obj
                             for change in obj_set.changeSet:
                                 if change.name == 'info':
                                     state = change.val.state
                                 elif change.name == 'info.state':
                                     state = change.val
@@ -1032,19 +1022,19 @@
             if disconnect:
                 self.disconnect()
 
         return True
 
     # -------------------------------------------------------------------------
     def create_vm(self, name, vm_folder, vm_config_spec, pool, max_wait=5):
-
-        LOG.info(_("Creating VM {!r} ...").format(name))
+        """Create the VM with a given name, VM folder an specification."""
+        LOG.info(_('Creating VM {!r} ...').format(name))
 
         if self.simulate:
-            LOG.info(_("Simulation mode - VM {!r} will not be created.").format(name))
+            LOG.info(_('Simulation mode - VM {!r} will not be created.').format(name))
             return
 
         start_time = time.time()
 
         task = vm_folder.CreateVM_Task(config=vm_config_spec, pool=pool)
 
         if not self.wait_for_tasks(
@@ -1053,27 +1043,27 @@
             raise TimeoutCreateVmError(name, time_diff)
 
     # -------------------------------------------------------------------------
     def generate_vm_create_spec(
         self, name, datastore, disks=None, nw_interfaces=None, graphic_ram_mb=256,
             videao_ram_mb=32, boot_delay_secs=3, ram_mb=1024, num_cpus=1, ds_with_timestamp=False,
             os_version=DEFAULT_OS_VERSION, cfg_version=DEFAULT_VM_CFG_VERSION):
-
-        LOG.debug(_("Generating create spec for VM {!r} ...").format(name))
+        """Create a specification for creating a virtual machine."""
+        LOG.debug(_('Generating create spec for VM {!r} ...').format(name))
 
         # File definitions
         datastore_path = '[{ds}] {name}'.format(ds=datastore, name=name)
         if ds_with_timestamp:
             tstamp = datetime.datetime.now(tz=self.tz).strftime('%Y-%m-%d_%H-%M')
             datastore_path += '-' + tstamp
         datastore_path += '/'
-        LOG.debug(_("Datastore path: {!r}").format(datastore_path))
+        LOG.debug(_('Datastore path: {!r}').format(datastore_path))
 
         vm_path_name = datastore_path + name + '.vmx'
-        LOG.debug(_("VM path name: {!r}").format(vm_path_name))
+        LOG.debug(_('VM path name: {!r}').format(vm_path_name))
 
         vm_file_info = vim.vm.FileInfo(
             logDirectory=datastore_path, snapshotDirectory=datastore_path,
             suspendDirectory=datastore_path, vmPathName=vm_path_name)
 
         # Device definitions
         dev_changes = []
@@ -1115,54 +1105,54 @@
             name=name, deviceChange=dev_changes, flags=vm_flags, extraConfig=extra_opts,
             memoryMB=ram_mb, memoryHotAddEnabled=True, numCPUs=num_cpus,
             cpuHotAddEnabled=True, cpuHotRemoveEnabled=True, files=vm_file_info,
             guestId=os_version, version=cfg_version, bootOptions=boot_opts,
         )
 
         if self.verbose > 1:
-            LOG.debug(_("Generated VM config:") + '\n' + pp(config))
+            LOG.debug(_('Generated VM config:') + '\n' + pp(config))
 
         return config
 
     # -------------------------------------------------------------------------
     def generate_disk_spec(self, datastore_path, disks=None):
-
+        """Create a specification for creating a virtual disk."""
         disk_sizes2create = []
         if disks:
-            err_msg_tpl = _("Given disksize {!r} must be greater than zero.")
+            err_msg_tpl = _('Given disksize {!r} must be greater than zero.')
             if isinstance(disks, Number):
                 if disks <= 0:
                     raise ValueError(err_msg_tpl.format(disks))
                 disk_sizes2create.append(int(disks))
             elif isinstance(disks, Sequence):
                 if isinstance(disks, str):
                     size = int(disks)
                     if size <= 0:
                         raise ValueError(err_msg_tpl.format(disks))
                     disk_sizes2create.append(size)
                 else:
                     if len(disks) > 6:
-                        msg = _("There may be created at most 6 disks, but {} were given.").format(
+                        msg = _('There may be created at most 6 disks, but {} were given.').format(
                             len(disks))
                         raise HandlerError(msg)
                     for disk in disks:
                         size = int(disk)
                         if size <= 0:
                             raise ValueError(err_msg_tpl.format(disk))
                         disk_sizes2create.append(size)
 
         if self.verbose > 1:
             if disk_sizes2create:
                 msg = ngettext(
-                    "Generating spec for SCSI controller and one disk: {d}",
-                    "Generating spec for SCSI controller and {n} disks: {d}",
+                    'Generating spec for SCSI controller and one disk: {d}',
+                    'Generating spec for SCSI controller and {n} disks: {d}',
                     len(disk_sizes2create))
                 LOG.debug(msg.format(n=len(disk_sizes2create), d=pp(disk_sizes2create)))
             else:
-                LOG.debug(_("Generating spec for SCSI controller without disks."))
+                LOG.debug(_('Generating spec for SCSI controller without disks.'))
 
         dev_changes = []
 
         # Creating SCSI Controller
         scsi_ctr_spec = vim.vm.device.VirtualDeviceSpec()
         scsi_ctr_spec.operation = vim.vm.device.VirtualDeviceSpec.Operation.add
         scsi_ctr_spec.device = vim.vm.device.VirtualLsiLogicController()
@@ -1178,20 +1168,20 @@
         i = 0
         letter = 'a'
 
         for size in disk_sizes2create:
 
             size_kb = size * 1024 * 1024
             if self.verbose > 1:
-                dname = "sd{}".format(letter)
-                LOG.debug(_("Adding spec for disk {n!r} with {gb} GiB => {kb} KiByte.").format(
+                dname = 'sd{}'.format(letter)
+                LOG.debug(_('Adding spec for disk {n!r} with {gb} GiB => {kb} KiByte.').format(
                     n=dname, gb=size, kb=size_kb))
 
             disk_spec = vim.vm.device.VirtualDeviceSpec()
-            disk_spec.fileOperation = "create"
+            disk_spec.fileOperation = 'create'
             disk_spec.operation = vim.vm.device.VirtualDeviceSpec.Operation.add
             disk_spec.device = vim.vm.device.VirtualDisk()
             disk_spec.device.backing = vim.vm.device.VirtualDisk.FlatVer2BackingInfo()
             disk_spec.device.backing.diskMode = 'persistent'
             disk_spec.device.backing.fileName = '{p}template-sd{ltr}.vmdk'.format(
                 p=datastore_path, ltr=letter)
             disk_spec.device.unitNumber = i
@@ -1204,42 +1194,42 @@
             i += 1
             letter = chr(ord(letter) + 1)
 
         return dev_changes
 
     # -------------------------------------------------------------------------
     def generate_if_create_spec(self, nw_interfaces=None):
-
+        """Create a specification for creating a virtual interface."""
         if not nw_interfaces:
             return []
 
         ifaces = []
         if isinstance(nw_interfaces, VsphereVmInterface):
             ifaces.append(nw_interfaces)
         else:
             for iface in nw_interfaces:
                 if not isinstance(iface, VsphereVmInterface):
-                    msg = _("Invalid Interface description {!r} given.").format(iface)
+                    msg = _('Invalid Interface description {!r} given.').format(iface)
                     raise TypeError(msg)
                 ifaces.append(iface)
 
         dev_changes = []
-        dev_name = "eth{}"
+        dev_name = 'eth{}'
         i = 0
 
         for iface in ifaces:
 
             if self.verbose > 2:
-                LOG.debug(_("Defined interface:") + '\n' + pp(iface.as_dict()))
+                LOG.debug(_('Defined interface:') + '\n' + pp(iface.as_dict()))
 
             dname = dev_name.format(i)
             if self.verbose > 1:
                 LOG.debug(_(
-                    "Adding spec for network interface {d!r} (Network {n!r}, "
-                    "MAC: {m!r}, summary: {s!r}).").format(
+                    'Adding spec for network interface {d!r} (Network {n!r}, '
+                    'MAC: {m!r}, summary: {s!r}).').format(
                     d=dname, n=iface.network_name, m=iface.mac_address,
                     s=iface.summary))
 
             nic_spec = vim.vm.device.VirtualDeviceSpec()
             nic_spec.operation = vim.vm.device.VirtualDeviceSpec.Operation.add
             nic_spec.device = vim.vm.device.VirtualVmxnet3()
             nic_spec.device.deviceInfo = vim.Description()
@@ -1264,15 +1254,15 @@
 
             dev_changes.append(nic_spec)
 
         return dev_changes
 
     # -------------------------------------------------------------------------
     def purge_vm(self, vm, max_wait=20, disconnect=False):
-
+        """Purge a vitual machine completely from VSPhere."""
         try:
 
             if not self.service_instance:
                 self.connect()
 
             if isinstance(vm, vim.VirtualMachine):
                 vm_obj = vm
@@ -1281,27 +1271,27 @@
                 vm_name = vm
                 vm_obj = self.get_vm(vm, as_vmw_obj=True)
                 if not vm_obj:
                     raise VSphereVmNotFoundError(vm)
 
             self.poweroff_vm(vm_obj)
 
-            LOG.info(_("Purging VM {!r} ...").format(vm_name))
+            LOG.info(_('Purging VM {!r} ...').format(vm_name))
 
             task = vm_obj.Destroy_Task()
             self.wait_for_tasks([task], max_wait=max_wait)
-            LOG.debug(_("VM {!r} successful removed.").format(vm_name))
+            LOG.debug(_('VM {!r} successful removed.').format(vm_name))
 
         finally:
             if disconnect:
                 self.disconnect()
 
     # -------------------------------------------------------------------------
     def set_mac_of_nic(self, vm, new_mac, nic_nr=0):
-
+        """Set a virtual network interface to a new MAC address."""
         if not self.service_instance:
             self.connect()
 
         if isinstance(vm, vim.VirtualMachine):
             vm_obj = vm
             vm_name = vm.summary.config.name
         else:
@@ -1317,16 +1307,16 @@
                 if i == nic_nr:
                     virtual_nic_device = dev
                     break
                 i += 1
 
         if not virtual_nic_device:
             msg = _(
-                "Did not found virtual ethernet device No. {no} ("
-                "found {count} devices).").format(no=nic_nr, count=i)
+                'Did not found virtual ethernet device No. {no} ('
+                'found {count} devices).').format(no=nic_nr, count=i)
             raise HandlerError(msg)
 
         virtual_nic_spec = vim.vm.device.VirtualDeviceSpec()
         virtual_nic_spec.operation = vim.vm.device.VirtualDeviceSpec.Operation.edit
         virtual_nic_spec.device = virtual_nic_device
         virtual_nic_spec.device.macAddress = new_mac
         virtual_nic_spec.device.backing = virtual_nic_device.backing
@@ -1335,32 +1325,34 @@
 
         dev_changes = []
         dev_changes.append(virtual_nic_spec)
         spec = vim.vm.ConfigSpec()
         spec.deviceChange = dev_changes
 
         if self.verbose > 2:
-            LOG.debug(_("Changes of MAC address:") + '\n' + pp(spec))
+            LOG.debug(_('Changes of MAC address:') + '\n' + pp(spec))
 
         task = vm_obj.ReconfigVM_Task(spec=spec)
         self.wait_for_tasks([task])
-        LOG.debug(_("Successful changed MAC address of VM {v!r} to {m!r}.").format(
+        LOG.debug(_('Successful changed MAC address of VM {v!r} to {m!r}.').format(
             v=vm_name, m=new_mac))
 
     # -------------------------------------------------------------------------
     def custom_field_name(self, key_id):
-        """Tries to evaluate the verbose custom field name by the given key ID.
-           On the first attempt to get a lib/fb_vmware/ all available field
-           names are cached in the dict self.custom_fields from the customFieldsManager.
-           If the key could not be detected, None is returned."""
+        """
+        Try to evaluate the verbose custom field name by the given key ID.
 
+        On the first attempt to get a lib/fb_vmware/ all available field
+        names are cached in the dict self.custom_fields from the customFieldsManager.
+        If the key could not be detected, None is returned.
+        """
         if self.custom_fields is None:
 
             if self.verbose > 1:
-                msg = _("Trying to detect all field names of custom field definitions.")
+                msg = _('Trying to detect all field names of custom field definitions.')
 
             self.custom_fields = {}
 
             try:
                 if not self.service_instance:
                     self.connect()
                 content = self.service_instance.RetrieveContent()
@@ -1370,31 +1362,31 @@
                     self.custom_fields[custom_field.key] = custom_field.name
 
             except (
                     socket.timeout, urllib3.exceptions.ConnectTimeoutError,
                     urllib3.exceptions.MaxRetryError,
                     requests.exceptions.ConnectTimeout) as e:
                 msg = _(
-                    "Got a {c} on requesting custom field names from VSPhere {url}: {e}").format(
+                    'Got a {c} on requesting custom field names from VSPhere {url}: {e}').format(
                     c=e.__class__.__name__, url=self.connect_info.url, e=e)
                 raise VSphereExpectedError(msg)
 
             if self.verbose > 2:
-                msg = _("Got custom field names from VSPhere {}:").format(self.connect_info.url)
-                msg += "\n" + pp(self.custom_fields)
+                msg = _('Got custom field names from VSPhere {}:').format(self.connect_info.url)
+                msg += '\n' + pp(self.custom_fields)
                 LOG.debug(msg)
 
         if key_id in self.custom_fields:
             return self.custom_fields[key_id]
 
         return None
 
 
 # =============================================================================
 
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_vmware-0.5.7/lib/fb_vmware/controller.py` & `fb_vmware-0.6.0/lib/fb_vmware/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
+@summary: The module for a VSphere disk controller object.
+
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 by Frank Brehm, Berlin
-@summary: The module for a VSphere disk controller object.
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
-import logging
 import copy
-
+import logging
 try:
     from collections.abc import MutableSequence
 except ImportError:
     from collections import MutableSequence
 
 # Third party modules
-from pyVmomi import vim
-
 from fb_tools.common import pp, to_bool
 from fb_tools.obj import FbBaseObject
 from fb_tools.xlate import format_list
 
+from pyVmomi import vim
+
 # Own modules
 from .xlate import XLATOR
 
-__version__ = '0.3.1'
+__version__ = '0.3.2'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 
 
 # =============================================================================
 class VsphereDiskController(FbBaseObject):
+    """This is a wrapper for a vim.vm.device.VirtualController object."""
 
     ctrl_types = (
         (vim.vm.device.VirtualIDEController, 'ide'),
         (vim.vm.device.VirtualNVMEController, 'nvme'),
         (vim.vm.device.VirtualPCIController, 'pci'),
         (vim.vm.device.VirtualPS2Controller, 'ps2'),
         (vim.vm.device.VirtualAHCIController, 'ahci'),
@@ -72,15 +73,15 @@
     }
 
     # -------------------------------------------------------------------------
     def __init__(
         self, appname=None, verbose=0, version=__version__, base_dir=None, initialized=None,
             ctrl_type='unknown', bus_nr=None, devices=None, hot_add_remove=False,
             scsi_ctrl_nr=None, sharing=None):
-
+        """Initialize a VsphereDiskController object."""
         self._ctrl_type = 'unknown'
         self._bus_nr = None
         self.devices = []
         self._hot_add_remove = False
         self._scsi_ctrl_nr = None
         self._sharing = None
 
@@ -178,17 +179,17 @@
         if v == '':
             self._sharing = None
             return
         self._sharing = v
 
     # -------------------------------------------------------------------------
     def __eq__(self, other):
-
+        """Magic method for using it as the '=='-operator."""
         if self.verbose > 4:
-            LOG.debug(_("Comparing {} objects ...").format(self.__class__.__name__))
+            LOG.debug(_('Comparing {} objects ...').format(self.__class__.__name__))
 
         if not isinstance(other, VsphereDiskController):
             return False
 
         if self.ctrl_type != other.ctrl_type:
             return False
         if self.bus_nr != other.bus_nr:
@@ -199,25 +200,24 @@
             return False
 
         return True
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True, bare=False):
         """
-        Transforms the elements of the object into a dict
+        Transform the elements of the object into a dict.
 
         @param short: don't include local properties in resulting dict.
         @type short: bool
         @param bare: don't include generic fields in returning dict
         @type bare: bool
 
         @return: structure as dict
         @rtype:  dict
         """
-
         if bare:
             res = {
                 'ctrl_type': self.ctrl_type,
                 'ctrl_type_name': self.ctrl_type_name,
                 'bus_nr': self.bus_nr,
                 'hot_add_remove': self.hot_add_remove,
                 'scsi_ctrl_nr': self.scsi_ctrl_nr,
@@ -235,48 +235,48 @@
         res['sharing'] = self.sharing
         res['devices'] = copy.copy(self.devices),
 
         return res
 
     # -------------------------------------------------------------------------
     def __copy__(self):
-
+        """Return a new VsphereDiskController as a deep copy of the current object."""
         ctrl = VsphereDiskController(
             appname=self.appname, verbose=self.verbose, base_dir=self.base_dir,
             initialized=self.initialized, ctrl_type=self.ctrl_type, bus_nr=self.bus_nr,
             hot_add_remove=self.hot_add_remove, scsi_ctrl_nr=self.scsi_ctrl_nr,
             sharing=self.sharing, devices=self.devices)
 
         return ctrl
 
     # -------------------------------------------------------------------------
     @classmethod
     def from_summary(cls, data, appname=None, verbose=0, base_dir=None, test_mode=False):
-
+        """Create a new VsphereDiskController object based on the data given from pyvmomi."""
         if test_mode:
 
             necessary_fields = ('busNumber', 'disk')
 
             failing_fields = []
 
             for field in necessary_fields:
                 if not hasattr(data, field):
                     failing_fields.append(field)
 
             if len(failing_fields):
                 msg = _(
-                    "The given parameter {p!r} on calling method {m}() has failing "
-                    "attributes").format(p='data', m='from_summary')
+                    'The given parameter {p!r} on calling method {m}() has failing '
+                    'attributes').format(p='data', m='from_summary')
                 msg += ': ' + format_list(failing_fields, do_repr=True)
                 raise AssertionError(msg)
 
         else:
 
             if not isinstance(data, vim.vm.device.VirtualController):
-                msg = _("Parameter {t!r} must be a {e}, {v!r} ({vt}) was given.").format(
+                msg = _('Parameter {t!r} must be a {e}, {v!r} ({vt}) was given.').format(
                     t='data', e='vim.vm.device.VirtualController',
                     v=data, vt=data.__class__.__name__)
                 raise TypeError(msg)
 
         params = {
             'appname': appname,
             'verbose': verbose,
@@ -290,48 +290,46 @@
             params['devices'].append(disk_id)
         if isinstance(data, vim.vm.device.VirtualSCSIController):
             params['hot_add_remove'] = data.hotAddRemove
             params['scsi_ctrl_nr'] = data.scsiCtlrUnitNumber
             params['sharing'] = data.sharedBus
 
         if verbose > 2:
-            LOG.debug(_("Checking class of controller: {!r}").format(data.__class__.__name__))
+            LOG.debug(_('Checking class of controller: {!r}').format(data.__class__.__name__))
 
         try:
             for pair in cls.ctrl_types:
                 if isinstance(data, pair[0]):
                     params['ctrl_type'] = pair[1]
                     break
         except Exception:
             pass
 
         if verbose > 2:
-            LOG.debug(_("Creating {} object from:").format(cls.__name__) + '\n' + pp(params))
+            LOG.debug(_('Creating {} object from:').format(cls.__name__) + '\n' + pp(params))
 
         ctrl = cls(**params)
 
         if verbose > 2:
-            LOG.debug(_("Created {} object:").format(cls.__name__) + '\n' + pp(ctrl.as_dict()))
+            LOG.debug(_('Created {} object:').format(cls.__name__) + '\n' + pp(ctrl.as_dict()))
 
         return ctrl
 
 
 # =============================================================================
 class VsphereDiskControllerList(FbBaseObject, MutableSequence):
-    """
-    A list containing VsphereDiskController objects.
-    """
+    """A list containing VsphereDiskController objects."""
 
-    msg_no_controller = _("Invalid type {t!r} as an item of a {c}, only {o} objects are allowed.")
+    msg_no_controller = _('Invalid type {t!r} as an item of a {c}, only {o} objects are allowed.')
 
     # -------------------------------------------------------------------------
     def __init__(
         self, appname=None, verbose=0, version=__version__, base_dir=None,
             initialized=None, *ctrls):
-
+        """Initialize a VsphereDiskControllerList object."""
         self._list = []
 
         super(VsphereDiskControllerList, self).__init__(
             appname=appname, verbose=verbose, version=version, base_dir=base_dir,
             initialized=False)
 
         for ctrl in ctrls:
@@ -339,25 +337,24 @@
 
         if initialized is not None:
             self.initialized = initialized
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True, bare=False):
         """
-        Transforms the elements of the object into a dict
+        Transform the elements of the object into a dict.
 
         @param short: don't include local properties in resulting dict.
         @type short: bool
         @param bare: don't include generic fields in returning dict
         @type bare: bool
 
         @return: structure as dict or list
         @rtype:  dict or list
         """
-
         if bare:
             res = []
             for ctrl in self:
                 res.append(ctrl.as_dict(bare=True))
             return res
 
         res = super(VsphereDiskControllerList, self).as_dict(short=short)
@@ -366,34 +363,34 @@
         for ctrl in self:
             res['_list'].append(ctrl.as_dict(short=short))
 
         return res
 
     # -------------------------------------------------------------------------
     def __copy__(self):
-
+        """Return a new VsphereDiskControllerList as a deep copy of the current object."""
         new_list = VsphereDiskControllerList(
             appname=self.appname, verbose=self.verbose,
             base_dir=self.base_dir, initialized=False)
 
         for ctrl in self:
             new_list.append(ctrl)
 
         new_list.initialized = self.initialized
         return new_list
 
     # -------------------------------------------------------------------------
     def index(self, ctrl, *args):
-
+        """Return the numeric index of the given controller in current list."""
         i = None
         j = None
 
         if len(args) > 0:
             if len(args) > 2:
-                raise TypeError(_("{m} takes at most {max} arguments ({n} given).").format(
+                raise TypeError(_('{m} takes at most {max} arguments ({n} given).').format(
                     m='index()', max=3, n=len(args) + 1))
             i = int(args[0])
             if len(args) > 1:
                 j = int(args[1])
 
         index = 0
         start = 0
@@ -424,20 +421,20 @@
             for index in list(range(len(self._list))):
                 item = self._list[index]
                 if index >= end:
                     break
             if item == ctrl:
                 return index
 
-        msg = _("Controller is not in controller list.")
+        msg = _('Controller is not in controller list.')
         raise ValueError(msg)
 
     # -------------------------------------------------------------------------
     def __contains__(self, ctrl):
-
+        """Return whether the given controller is contained in current list."""
         if not isinstance(ctrl, VsphereDiskController):
             raise TypeError(self.msg_no_controller.format(
                 t=ctrl.__class__.__name__, c=self.__class__.__name__, o='VsphereDiskController'))
 
         if not self._list:
             return False
 
@@ -445,15 +442,15 @@
             if item == ctrl:
                 return True
 
         return False
 
     # -------------------------------------------------------------------------
     def count(self, ctrl):
-
+        """Return the number of controllers which are equal to the given one in current list."""
         if not isinstance(ctrl, VsphereDiskController):
             raise TypeError(self.msg_no_controller.format(
                 t=ctrl.__class__.__name__, c=self.__class__.__name__, o='VsphereDiskController'))
 
         if not self._list:
             return 0
 
@@ -461,71 +458,72 @@
         for item in self._list:
             if item == ctrl:
                 num += 1
         return num
 
     # -------------------------------------------------------------------------
     def __len__(self):
+        """Return the number of controllers in current list."""
         return len(self._list)
 
     # -------------------------------------------------------------------------
     def __iter__(self):
-
+        """Iterate through all controllers in current list."""
         for item in self._list:
             yield item
 
     # -------------------------------------------------------------------------
     def __getitem__(self, key):
+        """Get a controller from current list by the given numeric index."""
         return self._list.__getitem__(key)
 
     # -------------------------------------------------------------------------
     def __reversed__(self):
-
+        """Reverse the controllers in list in place."""
         return reversed(self._list)
 
     # -------------------------------------------------------------------------
     def __setitem__(self, key, ctrl):
-
+        """Replace the controller at the given numeric index by the given one."""
         if not isinstance(ctrl, VsphereDiskController):
             raise TypeError(self.msg_no_controller.format(
                 t=ctrl.__class__.__name__, c=self.__class__.__name__, o='VsphereDiskController'))
 
         self._list.__setitem__(key, ctrl)
 
     # -------------------------------------------------------------------------
     def __delitem__(self, key):
-
+        """Remove the controller at the given numeric index from list."""
         del self._list[key]
 
     # -------------------------------------------------------------------------
     def append(self, ctrl):
-
+        """Append the given controller to the current list."""
         if not isinstance(ctrl, VsphereDiskController):
             raise TypeError(self.msg_no_controller.format(
                 t=ctrl.__class__.__name__, c=self.__class__.__name__, o='VsphereDiskController'))
 
         self._list.append(ctrl)
 
     # -------------------------------------------------------------------------
     def insert(self, index, ctrl):
-
+        """Insert the given controller in current list at given index."""
         if not isinstance(ctrl, VsphereDiskController):
             raise TypeError(self.msg_no_controller.format(
                 t=ctrl.__class__.__name__, c=self.__class__.__name__, o='VsphereDiskController'))
 
         self._list.insert(index, ctrl)
 
     # -------------------------------------------------------------------------
     def clear(self):
-        "Remove all items from the VsphereDiskControllerList."
-
+        """Remove all items from the VsphereDiskControllerList."""
         self._list = []
 
 
 # =============================================================================
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_vmware-0.5.7/lib/fb_vmware/datastore.py` & `fb_vmware-0.6.0/lib/fb_vmware/datastore.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
+@summary: The module for a VSphere datastore object.
+
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 by Frank Brehm, Berlin
-@summary: The module for a VSphere datastore object.
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
 import logging
 import random
 import re
-
 try:
     from collections.abc import MutableMapping
 except ImportError:
     from collections import MutableMapping
 
 # Third party modules
-from pyVmomi import vim
-
 from fb_tools.common import pp, to_bool
 from fb_tools.obj import FbGenericBaseObject
 from fb_tools.xlate import format_list
 
-# Own modules
-from .xlate import XLATOR
+from pyVmomi import vim
 
+# Own modules
 from .obj import VsphereObject
+from .xlate import XLATOR
 
-__version__ = '1.4.2'
+__version__ = '1.4.3'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 
 
 # =============================================================================
 class VsphereDatastore(VsphereObject):
+    """Wrapper class for a VSphere datastore object."""
 
     re_is_nfs = re.compile(r'(?:share[_-]*nfs|nfs[_-]*share)', re.IGNORECASE)
     re_vmcb_fs = re.compile(r'vmcb-\d+-fc-\d+', re.IGNORECASE)
     re_local_ds = re.compile(r'^local_', re.IGNORECASE)
     re_k8s_ds = re.compile(r'[_-](?:k8s|kubernetes)[_-]', re.IGNORECASE)
 
     # -------------------------------------------------------------------------
     def __init__(
         self, appname=None, verbose=0, version=__version__, base_dir=None, initialized=None,
             name=None, status='gray', config_status='gray', accessible=True, capacity=None,
             free_space=None, maintenance_mode=None, multiple_host_access=True, fs_type=None,
             uncommitted=None, url=None, for_k8s=None):
-
+        """Initialize the VsphereDatastore object."""
         self.repr_fields = (
             'name', 'status', 'accessible', 'capacity', 'free_space', 'fs_type', 'storage_type',
             'appname', 'verbose', 'version')
 
         self._accessible = bool(accessible)
         self._capacity = int(capacity)
         self._free_space = int(free_space)
@@ -74,15 +74,15 @@
         self._for_k8s = False
 
         self._storage_type = 'unknown'
 
         self._calculated_usage = 0.0
 
         super(VsphereDatastore, self).__init__(
-            name=name, obj_type='vsphere_datastore', name_prefix="ds", status=status,
+            name=name, obj_type='vsphere_datastore', name_prefix='ds', status=status,
             config_status=config_status, appname=appname, verbose=verbose,
             version=version, base_dir=base_dir)
 
         st_type = self.storage_type_by_name(self.name)
         if st_type:
             self._storage_type = st_type
 
@@ -129,36 +129,41 @@
     def maintenance_mode(self):
         """The current maintenance mode state of the datastore."""
         return self._maintenance_mode
 
     # -----------------------------------------------------------
     @property
     def multiple_host_access(self):
-        """More than one host in the datacenter has been configured
-            with access to the datastore."""
+        """More than one host has been configured with access to the datastore."""
         return self._multiple_host_access
 
     # -----------------------------------------------------------
     @property
     def fs_type(self):
         """Type of file system volume, such as VMFS or NFS."""
         return self._fs_type
 
     # -----------------------------------------------------------
     @property
     def uncommitted(self):
-        """Total additional storage space, in bytes,
-            potentially used by all virtual machines on this datastore."""
+        """
+        Total additional storage space, in bytes.
+
+        This is potentially used by all virtual machines on this datastore.
+        """
         return self._uncommitted
 
     # -----------------------------------------------------------
     @property
     def uncommitted_gb(self):
-        """Total additional storage space, in GiBytes,
-            potentially used by all virtual machines on this datastore."""
+        """
+        Total additional storage space, in GiBytes.
+
+        This is potentially used by all virtual machines on this datastore.
+        """
         return float(self._uncommitted) / 1024.0 / 1024.0 / 1024.0
 
     # -----------------------------------------------------------
     @property
     def url(self):
         """The unique locator for the datastore."""
         return self._url
@@ -199,15 +204,15 @@
         if not self.calculated_usage:
             return self.free_space_gb
         return self.free_space_gb - self.calculated_usage
 
     # -------------------------------------------------------------------------
     @classmethod
     def from_summary(cls, data, appname=None, verbose=0, base_dir=None, test_mode=False):
-
+        """Create a new VsphereDatastore object based on the data given from pyvmomi module."""
         if test_mode:
 
             necessary_fields = ('summary', 'overallStatus', 'configStatus')
             summary_fields = ('capacity', 'freeSpace', 'name', 'type', 'url')
 
             failing_fields = []
 
@@ -219,23 +224,23 @@
                 summary = data.summary
                 for field in summary_fields:
                     if not hasattr(summary, field):
                         failing_fields.append('summary.' + field)
 
             if len(failing_fields):
                 msg = _(
-                    "The given parameter {p!r} on calling method {m}() has failing "
-                    "attributes").format(p='data', m='from_summary')
+                    'The given parameter {p!r} on calling method {m}() has failing '
+                    'attributes').format(p='data', m='from_summary')
                 msg += ': ' + format_list(failing_fields, do_repr=True)
                 raise AssertionError(msg)
 
         else:
 
             if not isinstance(data, vim.Datastore):
-                msg = _("Parameter {t!r} must be a {e}, {v!r} was given.").format(
+                msg = _('Parameter {t!r} must be a {e}, {v!r} was given.').format(
                     t='data', e='vim.Datastore', v=data)
                 raise TypeError(msg)
 
         params = {
             'appname': appname,
             'verbose': verbose,
             'base_dir': base_dir,
@@ -258,25 +263,23 @@
         if hasattr(data.summary, 'multipleHostAccess'):
             params['multiple_host_access'] = data.summary.multipleHostAccess
 
         if hasattr(data.summary, 'uncommitted'):
             params['uncommitted'] = data.summary.uncommitted
 
         if verbose > 2:
-            LOG.debug(_("Creating {} object from:").format(cls.__name__) + '\n' + pp(params))
+            LOG.debug(_('Creating {} object from:').format(cls.__name__) + '\n' + pp(params))
 
         ds = cls(**params)
         return ds
 
     # -------------------------------------------------------------------------
     @classmethod
     def storage_type_by_name(cls, name):
-        """Trying to guess the storage type by its name.
-            May be overridden in descentant classes."""
-
+        """Guess the storage type by its name. May be overridden in descentant classes."""
         if cls.re_is_nfs.search(name):
             return 'NFS'
 
         if '-sas-' in name.lower():
             return 'SAS'
 
         if '-ssd-' in name.lower():
@@ -292,33 +295,34 @@
             return 'LOCAL'
 
         return None
 
     # -------------------------------------------------------------------------
     @classmethod
     def detect_k8s(cls, name):
-        """Method for detecting from given name, whether the datastore
-            is intended to use as PV in Kubernetes or not."""
+        """
+        Is the datastore intended to use as PV in Kubernetes or not.
 
+        This detection is made on evaluating the datastore name.
+        """
         if cls.re_k8s_ds.search(name):
             return True
         return False
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True):
         """
-        Transforms the elements of the object into a dict
+        Transform the elements of the object into a dict.
 
         @param short: don't include local properties in resulting dict.
         @type short: bool
 
         @return: structure as dict
         @rtype:  dict
         """
-
         res = super(VsphereDatastore, self).as_dict(short=short)
         res['accessible'] = self.accessible
         res['capacity'] = self.capacity
         res['capacity_gb'] = self.capacity_gb
         res['free_space'] = self.free_space
         res['free_space_gb'] = self.free_space_gb
         res['maintenance_mode'] = self.maintenance_mode
@@ -332,56 +336,57 @@
         res['calculated_usage'] = self.calculated_usage
         res['avail_space_gb'] = self.avail_space_gb
 
         return res
 
     # -------------------------------------------------------------------------
     def __copy__(self):
-
+        """Return a new VsphereDatastore object with data from current object copied in."""
         return VsphereDatastore(
             appname=self.appname, verbose=self.verbose, base_dir=self.base_dir,
             initialized=self.initialized, name=self.name, accessible=self.accessible,
             capacity=self.capacity, free_space=self.free_space, for_k8s=self.for_k8s,
             maintenance_mode=self.maintenance_mode, multiple_host_access=self.multiple_host_access,
             fs_type=self.fs_type, uncommitted=self.uncommitted, url=self.url,
             status=self.status, config_status=self.config_status)
 
     # -------------------------------------------------------------------------
     def __eq__(self, other):
-
+        """Magic method for using it as the '=='-operator."""
         if self.verbose > 4:
-            LOG.debug(_("Comparing {} objects ...").format(self.__class__.__name__))
+            LOG.debug(_('Comparing {} objects ...').format(self.__class__.__name__))
 
         if not isinstance(other, VsphereDatastore):
             return False
 
         if self.name != other.name:
             return False
 
         return True
 
 
 # =============================================================================
 class VsphereDatastoreDict(MutableMapping, FbGenericBaseObject):
     """
     A dictionary containing VsphereDatastore objects.
+
     It works like a dict.
     """
 
-    msg_invalid_ds_type = _("Invalid item type {{!r}} to set, only {} allowed.").format(
+    msg_invalid_ds_type = _('Invalid item type {{!r}} to set, only {} allowed.').format(
         'VsphereDatastore')
-    msg_key_not_name = _("The key {k!r} must be equal to the datastore name {n!r}.")
-    msg_none_type_error = _("None type as key is not allowed.")
-    msg_empty_key_error = _("Empty key {!r} is not allowed.")
-    msg_no_ds_dict = _("Object {{!r}} is not a {} object.").format('VsphereDatastoreDict')
+    msg_key_not_name = _('The key {k!r} must be equal to the datastore name {n!r}.')
+    msg_none_type_error = _('None type as key is not allowed.')
+    msg_empty_key_error = _('Empty key {!r} is not allowed.')
+    msg_no_ds_dict = _('Object {{!r}} is not a {} object.').format('VsphereDatastoreDict')
 
     # -------------------------------------------------------------------------
     def __init__(self, *args, **kwargs):
-        '''Use the object dict'''
-        self._map = dict()
+        """Initialize a VsphereDatastoreDict object."""
+        self._map = {}
 
         for arg in args:
             self.append(arg)
 
     # -------------------------------------------------------------------------
     def _set_item(self, key, ds):
 
@@ -392,15 +397,15 @@
         if ds_name != key:
             raise KeyError(self.msg_key_not_name.format(k=key, n=ds_name))
 
         self._map[ds_name] = ds
 
     # -------------------------------------------------------------------------
     def append(self, ds):
-
+        """Set the given datastore in the current dict with its name as key."""
         if not isinstance(ds, VsphereDatastore):
             raise TypeError(self.msg_invalid_ds_type.format(ds.__class__.__name__))
         self._set_item(ds.name, ds)
 
     # -------------------------------------------------------------------------
     def _get_item(self, key):
 
@@ -411,14 +416,15 @@
         if ds_name == '':
             raise ValueError(self.msg_empty_key_error.format(key))
 
         return self._map[ds_name]
 
     # -------------------------------------------------------------------------
     def get(self, key):
+        """Get the datastore from dict by its name."""
         return self._get_item(key)
 
     # -------------------------------------------------------------------------
     def _del_item(self, key, strict=True):
 
         if key is None:
             raise TypeError(self.msg_none_type_error)
@@ -431,128 +437,138 @@
             return
 
         del self._map[ds_name]
 
     # -------------------------------------------------------------------------
     # The next five methods are requirements of the ABC.
     def __setitem__(self, key, value):
+        """Set the given datastore in the current dict by key."""
         self._set_item(key, value)
 
     # -------------------------------------------------------------------------
     def __getitem__(self, key):
+        """Get the datastore from dict by the key."""
         return self._get_item(key)
 
     # -------------------------------------------------------------------------
     def __delitem__(self, key):
+        """Remove the datastore from dict by the key."""
         self._del_item(key)
 
     # -------------------------------------------------------------------------
     def __iter__(self):
-
+        """Iterate through datastore names as keys."""
         for ds_name in self.keys():
             yield ds_name
 
     # -------------------------------------------------------------------------
     def __len__(self):
+        """Return the number of datastores in current dict."""
         return len(self._map)
 
     # -------------------------------------------------------------------------
     # The next methods aren't required, but nice for different purposes:
     def __str__(self):
-        '''returns simple dict representation of the mapping'''
+        """Return a simple dict representation of the mapping."""
         return str(self._map)
 
     # -------------------------------------------------------------------------
     def __repr__(self):
-        '''echoes class, id, & reproducible representation in the REPL'''
+        """Transform into a string for reproduction."""
         return '{}, {}({})'.format(
             super(VsphereDatastoreDict, self).__repr__(),
             self.__class__.__name__,
             self._map)
 
     # -------------------------------------------------------------------------
     def __contains__(self, key):
+        """Return whether the given datastore name is contained in current dict as a key."""
         if key is None:
             raise TypeError(self.msg_none_type_error)
 
         ds_name = str(key).strip()
         if ds_name == '':
             raise ValueError(self.msg_empty_key_error.format(key))
 
         return ds_name in self._map
 
     # -------------------------------------------------------------------------
     def keys(self):
-
+        """Return all datastore names of this dict in a sorted manner."""
         return sorted(self._map.keys(), key=str.lower)
 
     # -------------------------------------------------------------------------
     def items(self):
-
+        """Return tuples (datastore name + object as tuple) of this dict in a sorted manner."""
         item_list = []
 
         for ds_name in self.keys():
             item_list.append((ds_name, self._map[ds_name]))
 
         return item_list
 
     # -------------------------------------------------------------------------
     def values(self):
-
+        """Return all datastore objects of this dict."""
         value_list = []
         for ds_name in self.keys():
             value_list.append(self._map[ds_name])
         return value_list
 
     # -------------------------------------------------------------------------
     def __eq__(self, other):
-
+        """Magic method for using it as the '=='-operator."""
         if not isinstance(other, VsphereDatastoreDict):
             raise TypeError(self.msg_no_ds_dict.format(other))
 
         return self._map == other._map
 
     # -------------------------------------------------------------------------
     def __ne__(self, other):
-
+        """Magic method for using it as the '!='-operator."""
         if not isinstance(other, VsphereDatastoreDict):
             raise TypeError(self.msg_no_ds_dict.format(other))
 
         return self._map != other._map
 
     # -------------------------------------------------------------------------
     def pop(self, key, *args):
-
+        """Get the datastore by its name and remove it in dict."""
         if key is None:
             raise TypeError(self.msg_none_type_error)
 
         ds_name = str(key).strip()
         if ds_name == '':
             raise ValueError(self.msg_empty_key_error.format(key))
 
         return self._map.pop(ds_name, *args)
 
     # -------------------------------------------------------------------------
     def popitem(self):
-
+        """Remove and return a arbitrary (datastore name and object) pair from the dictionary."""
         if not len(self._map):
             return None
 
         ds_name = self.keys()[0]
         ds = self._map[ds_name]
         del self._map[ds_name]
         return (ds_name, ds)
 
     # -------------------------------------------------------------------------
     def clear(self):
-        self._map = dict()
+        """Remove all items from the dictionary."""
+        self._map = {}
 
     # -------------------------------------------------------------------------
     def setdefault(self, key, default):
+        """
+        Return the datastore, if the key is in dict.
 
+        If not, insert key with a value of default and return default.
+        """
         if key is None:
             raise TypeError(self.msg_none_type_error)
 
         ds_name = str(key).strip()
         if ds_name == '':
             raise ValueError(self.msg_empty_key_error.format(key))
 
@@ -563,66 +579,66 @@
             return self._map[ds_name]
 
         self._set_item(ds_name, default)
         return default
 
     # -------------------------------------------------------------------------
     def update(self, other):
-
+        """Update the dict with the key/value pairs from other, overwriting existing keys."""
         if isinstance(other, VsphereDatastoreDict) or isinstance(other, dict):
             for ds_name in other.keys():
                 self._set_item(ds_name, other[ds_name])
             return
 
         for tokens in other:
             key = tokens[0]
             value = tokens[1]
             self._set_item(key, value)
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True):
-
+        """Transform the elements of the object into a dict."""
         res = {}
         for ds_name in self._map:
             res[ds_name] = self._map[ds_name].as_dict(short)
         return res
 
     # -------------------------------------------------------------------------
     def as_list(self, short=True):
-
+        """Return a list with all datastores transformed to a dict."""
         res = []
         for ds_name in self.keys():
             res.append(self._map[ds_name].as_dict(short))
         return res
 
     # -------------------------------------------------------------------------
     def find_ds(self, needed_gb, ds_type='sata', reserve_space=True, use_ds=None, no_k8s=False):
-
+        """Find a datastore in dict with the given minimum free space and the given type."""
         search_chains = {
             'sata': ('sata', 'sas', 'ssd'),
             'sas': ('sas', 'sata', 'ssd'),
             'ssd': ('ssd', 'sas', 'sata'),
         }
 
         if ds_type not in search_chains:
-            raise ValueError(_("Could not handle datastore type {!r}.").format(ds_type))
+            raise ValueError(_('Could not handle datastore type {!r}.').format(ds_type))
         for dstp in search_chains[ds_type]:
             ds_name = self._find_ds(
                 needed_gb, dstp, reserve_space, use_ds=use_ds, no_k8s=no_k8s)
             if ds_name:
                 return ds_name
 
-        LOG.error(_("Could not found a datastore for {c:0.1f} GiB of type {t!r}.").format(
+        LOG.error(_('Could not found a datastore for {c:0.1f} GiB of type {t!r}.').format(
             c=needed_gb, t=ds_type))
         return None
 
     # -------------------------------------------------------------------------
     def _find_ds(self, needed_gb, ds_type, reserve_space=True, use_ds=None, no_k8s=False):
 
-        LOG.debug(_("Searching datastore for {c:0.1f} GiB of type {t!r}.").format(
+        LOG.debug(_('Searching datastore for {c:0.1f} GiB of type {t!r}.').format(
             c=needed_gb, t=ds_type))
 
         avail_ds_names = []
         for (ds_name, ds) in self.items():
             if use_ds:
                 if ds.name not in use_ds:
                     continue
@@ -641,14 +657,14 @@
             ds = self[ds_name]
             ds.calculated_usage += needed_gb
 
         return ds_name
 
 
 # =============================================================================
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_vmware-0.5.7/lib/fb_vmware/dc.py` & `fb_vmware-0.6.0/lib/fb_vmware/dc.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,69 +1,68 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
+@summary: The module for capsulating a VSphere datacenter object.
+
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 by Frank Brehm, Berlin
-@summary: The module for capsulating a VSphere datacenter object.
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
 import logging
 
 # Third party modules
-from pyVmomi import vim
-
 from fb_tools.common import pp
 from fb_tools.xlate import format_list
 
-# Own modules
-from .obj import VsphereObject, DEFAULT_OBJ_STATUS
+from pyVmomi import vim
 
+# Own modules
+from .obj import DEFAULT_OBJ_STATUS
+from .obj import VsphereObject
 from .xlate import XLATOR
 
-__version__ = '0.4.0'
+__version__ = '0.4.1'
 LOG = logging.getLogger(__name__)
 
 DEFAULT_HOST_FOLDER = 'host'
 DEFAULT_VM_FOLDER = 'vm'
 DEFAULT_DS_FOLDER = 'datastore'
 DEFAULT_NETWORK_FOLDER = 'network'
 
 _ = XLATOR.gettext
 
 
 # =============================================================================
 class VsphereDatacenter(VsphereObject):
-    """
-    Class for a VSphere Datacenter object.
-    """
+    """Encapsulation class for a VSphere Datacenter object."""
 
     # -------------------------------------------------------------------------
     def __init__(
         self, appname=None, verbose=0, version=__version__, base_dir=None, initialized=None,
             name=None, status=DEFAULT_OBJ_STATUS, config_status=DEFAULT_OBJ_STATUS,
             ds_folder=DEFAULT_DS_FOLDER, host_folder=DEFAULT_HOST_FOLDER,
             network_folder=DEFAULT_NETWORK_FOLDER, vm_folder=DEFAULT_VM_FOLDER,
             default_hw_version_key=None, max_hw_version_key=None):
-
+        """Initialize a VsphereDatacenter object."""
         self.repr_fields = (
             'name', 'obj_type', 'name_prefix', 'status', 'config_status',
             'appname', 'verbose', 'version')
 
         self._host_folder = DEFAULT_HOST_FOLDER
         self._vm_folder = DEFAULT_VM_FOLDER
         self._ds_folder = DEFAULT_DS_FOLDER
         self._network_folder = DEFAULT_NETWORK_FOLDER
         self._default_hw_version_key = None
         self._max_hw_version_key = None
 
         super(VsphereDatacenter, self).__init__(
-            name=name, obj_type='vsphere_datacenter', name_prefix="dc", status=status,
+            name=name, obj_type='vsphere_datacenter', name_prefix='dc', status=status,
             config_status=config_status, appname=appname, verbose=verbose,
             version=version, base_dir=base_dir)
 
         self._ds_folder = ds_folder
         self._host_folder = host_folder
         self._network_folder = network_folder
         self._vm_folder = vm_folder
@@ -108,63 +107,62 @@
     def max_hw_version_key(self):
         """Key for Maximum Hardware Version used on this datacenter."""
         return self._max_hw_version_key
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True):
         """
-        Transforms the elements of the object into a dict
+        Transform the elements of the object into a dict.
 
         @param short: don't include local properties in resulting dict.
         @type short: bool
 
         @return: structure as dict
         @rtype:  dict
         """
-
         res = super(VsphereDatacenter, self).as_dict(short=short)
         res['ds_folder'] = self.ds_folder
         res['host_folder'] = self.host_folder
         res['network_folder'] = self.network_folder
         res['vm_folder'] = self.vm_folder
         res['default_hw_version_key'] = self.default_hw_version_key
         res['max_hw_version_key'] = self.max_hw_version_key
 
         return res
 
     # -------------------------------------------------------------------------
     def __copy__(self):
-
+        """Return a new VsphereDatacenter as a deep copy of the current object."""
         return VsphereDatacenter(
             appname=self.appname, verbose=self.verbose, base_dir=self.base_dir,
             initialized=self.initialized, name=self.name,
             status=self.status, config_status=self.config_status,
             default_hw_version_key=self.default_hw_version_key,
             max_hw_version_key=self.max_hw_version_key)
 
     # -------------------------------------------------------------------------
     def __eq__(self, other):
-
+        """Magic method for using it as the '=='-operator."""
         if self.verbose > 4:
-            LOG.debug(_("Comparing {} objects ...").format(self.__class__.__name__))
+            LOG.debug(_('Comparing {} objects ...').format(self.__class__.__name__))
 
         if not isinstance(other, VsphereDatacenter):
             return False
 
         if self.name != other.name:
             return False
 
         return True
 
     # -------------------------------------------------------------------------
     @classmethod
     def from_summary(cls, data, appname=None, verbose=0, base_dir=None, test_mode=False):
-
+        """Create a new VsphereDatacenter object based on the data given from pyvmomi."""
         if verbose > 3:
-            LOG.debug("Creating {} object by data:".format(cls.__name__) + '\n' + pp(data))
+            LOG.debug('Creating {} object by data:'.format(cls.__name__) + '\n' + pp(data))
 
         if test_mode:
 
             necessary_fields = (
                 'name', 'overallStatus', 'configStatus', 'datastoreFolder', 'hostFolder',
                 'networkFolder', 'vmFolder')
             named_fields = ('datastoreFolder', 'hostFolder', 'networkFolder', 'vmFolder')
@@ -179,24 +177,24 @@
                 if hasattr(data, field):
                     attr = getattr(data, field)
                     if not hasattr(attr, 'name'):
                         failing_fields.append(field + '.name')
 
             if len(failing_fields):
                 msg = _(
-                    "The given parameter {p!r} on calling method {m}() has failing "
-                    "attributes").format(p='data', m='from_summary')
+                    'The given parameter {p!r} on calling method {m}() has failing '
+                    'attributes').format(p='data', m='from_summary')
                 msg += ': ' + format_list(failing_fields, do_repr=True)
                 raise AssertionError(msg)
 
         else:
             if not isinstance(data, vim.Datacenter):
                 msg = _(
-                    "Parameter {t!r} must be a {e} object, a {v} object was given "
-                    "instead.").format(t='data', e='vim.Datacenter', v=data.__class__.__qualname__)
+                    'Parameter {t!r} must be a {e} object, a {v} object was given '
+                    'instead.').format(t='data', e='vim.Datacenter', v=data.__class__.__qualname__)
                 raise TypeError(msg)
 
         params = {
             'appname': appname,
             'verbose': verbose,
             'base_dir': base_dir,
             'initialized': True,
@@ -214,23 +212,23 @@
         if hasattr(data, 'configuration'):
             if hasattr(data.configuration, 'defaultHardwareVersionKey'):
                 params['default_hw_version_key'] = data.configuration.defaultHardwareVersionKey
             if hasattr(data.configuration, 'maximumHardwareVersionKey'):
                 params['max_hw_version_key'] = data.configuration.maximumHardwareVersionKey
 
         if verbose > 2:
-            LOG.debug(_("Creating {} object from:").format(cls.__name__) + '\n' + pp(params))
+            LOG.debug(_('Creating {} object from:').format(cls.__name__) + '\n' + pp(params))
 
         dc = cls(**params)
 
         return dc
 
 
 # =============================================================================
 
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_vmware-0.5.7/lib/fb_vmware/disk.py` & `fb_vmware-0.6.0/lib/fb_vmware/disk.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,60 +1,59 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
+@summary: Mdule for capsulating a VSphere disk object, which can be assigned to a VM.
+
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 by Frank Brehm, Berlin
-@summary: The module for capsulating a VSphere disk object, which can be assigned
-          to a virtual machine..
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
 import logging
-import uuid
 import re
-
+import uuid
 try:
     from collections.abc import MutableSequence
 except ImportError:
     from collections import MutableSequence
 
 # Third party modules
-from pyVmomi import vim
-
 from fb_tools.common import pp
 from fb_tools.obj import FbBaseObject
 from fb_tools.xlate import format_list
 
+from pyVmomi import vim
+
 # Own modules
 from .xlate import XLATOR
 
-__version__ = '0.4.1'
+__version__ = '0.4.2'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 
 
 # =============================================================================
 class VsphereDisk(FbBaseObject):
+    """Encapsulation of a VSphere disk object, which can be assigned to a VM."""
 
     re_file_storage = re.compile(r'^\s*\[\s*([^\s\]]+)')
     re_file_rel = re.compile(r'^\s*\[[^\]]*]\s*(\S.*)\s*$')
 
     # -------------------------------------------------------------------------
     def __init__(
         self, appname=None, verbose=0, version=__version__, base_dir=None, initialized=None,
             uuid=None, file_name=None, unit_nr=None, label=None, key=None, controller_key=None,
             size=None, disk_id=None, summary=None):
-
+        """Initialize a VsphereDisk object."""
         # self.repr_fields = (
         #     'uuid', 'file_name', 'unit_nr', 'label', 'key', 'controller_key',
         #     'size', 'disk_id', 'appname', 'verbose')
-
         self._uuid = None
         self._file_name = None
         self._unit_nr = None
         self._label = None
         self._summary = None
         self._key = None
         self._controller_key = None
@@ -136,17 +135,20 @@
         if match:
             return match.group(1)
         return None
 
     # -----------------------------------------------------------
     @property
     def unit_nr(self):
-        """The unit number of this device on its controller.
-            This property is None if the controller property is None
-            (for example, when the device is not attached to a specific controller object)."""
+        """
+        The unit number of this device on its controller.
+
+        This property is None if the controller property is None
+        (for example, when the device is not attached to a specific controller object).
+        """
         return self._unit_nr
 
     @unit_nr.setter
     def unit_nr(self, value):
         if value is None:
             self._unit_nr = None
             return
@@ -185,16 +187,15 @@
             self._summary = None
             return
         self._summary = v
 
     # -----------------------------------------------------------
     @property
     def key(self):
-        """A unique key that distinguishes this device from other devices
-            in the same virtual machine."""
+        """A unique key that distinguishes this device from other devices in the same VM."""
         return self._key
 
     @key.setter
     def key(self, value):
         if value is None:
             self._key = None
             return
@@ -265,17 +266,17 @@
         if v == '':
             self._disk_id = None
             return
         self._disk_id = v
 
     # -------------------------------------------------------------------------
     def __eq__(self, other):
-
+        """Magic method for using it as the '=='-operator."""
         if self.verbose > 4:
-            LOG.debug(_("Comparing {} objects ...").format(self.__class__.__name__))
+            LOG.debug(_('Comparing {} objects ...').format(self.__class__.__name__))
 
         if not isinstance(other, VsphereDisk):
             return False
 
         if self.uuid != other.uuid:
             return False
         if self.file_name != other.file_name:
@@ -296,25 +297,24 @@
             return False
 
         return True
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True, bare=False):
         """
-        Transforms the elements of the object into a dict
+        Transform the elements of the object into a dict.
 
         @param short: don't include local properties in resulting dict.
         @type short: bool
         @param bare: don't include generic fields in returning dict
         @type bare: bool
 
         @return: structure as dict
         @rtype:  dict
         """
-
         if bare:
             res = {
                 'uuid': self.uuid,
                 'file_name': self.file_name,
                 'file_rel': self.file_rel,
                 'file_storage': self.file_storage,
                 'unit_nr': self.unit_nr,
@@ -346,27 +346,27 @@
         res['controller_key'] = self.controller_key
         res['disk_id'] = self.disk_id
 
         return res
 
     # -------------------------------------------------------------------------
     def __copy__(self):
-
+        """Return a new VsphereDisk as a deep copy of the current object."""
         disk = VsphereDisk(
             appname=self.appname, verbose=self.verbose, base_dir=self.base_dir,
             initialized=self.initialized, uuid=self.uuid, file_name=self.file_name,
             unit_nr=self.unit_nr, label=self.label, key=self.key, size=self.size,
             controller_key=self.controller_key, disk_id=self.disk_id, summary=self.summary)
 
         return disk
 
     # -------------------------------------------------------------------------
     @classmethod
     def from_summary(cls, data, appname=None, verbose=0, base_dir=None, test_mode=False):
-
+        """Create a new VsphereDisk object based on the data given from pyvmomi."""
         if test_mode:
 
             necessary_fields = (
                 'unitNumber', 'deviceInfo', 'capacityInBytes', 'key', 'backing',
                 'controllerKey', 'vDiskId')
 
             failing_fields = []
@@ -382,25 +382,25 @@
                         failing_fields.append('deviceInfo.' + field)
 
             if hasattr(data, 'backing') and not hasattr(data.backing, 'fileName'):
                 failing_fields.append('backing.fileName')
 
             if len(failing_fields):
                 msg = _(
-                    "The given parameter {p!r} on calling method {m}() has failing "
-                    "attributes").format(p='data', m='from_summary')
+                    'The given parameter {p!r} on calling method {m}() has failing '
+                    'attributes').format(p='data', m='from_summary')
                 msg += ': ' + format_list(failing_fields, do_repr=True)
                 raise AssertionError(msg)
 
         else:
 
             if not isinstance(data, vim.vm.device.VirtualDisk):
                 msg = _(
-                    "Parameter {t!r} must be a {e} object, a {v} object was given "
-                    "instead.").format(
+                    'Parameter {t!r} must be a {e} object, a {v} object was given '
+                    'instead.').format(
                         t='data', e='vim.vm.device.VirtualDisk', v=data.__class__.__qualname__)
                 raise TypeError(msg)
 
         params = {
             'appname': appname,
             'verbose': verbose,
             'base_dir': base_dir,
@@ -412,37 +412,35 @@
             'key': data.key,
             'file_name': data.backing.fileName,
             'controller_key': data.controllerKey,
             'disk_id': data.vDiskId,
         }
 
         if verbose > 2:
-            LOG.debug(_("Creating {} object from:").format(cls.__name__) + '\n' + pp(params))
+            LOG.debug(_('Creating {} object from:').format(cls.__name__) + '\n' + pp(params))
 
         disk = cls(**params)
 
         if verbose > 2:
-            LOG.debug(_("Created {} object:").format(cls.__name__) + '\n' + pp(disk.as_dict()))
+            LOG.debug(_('Created {} object:').format(cls.__name__) + '\n' + pp(disk.as_dict()))
 
         return disk
 
 
 # =============================================================================
 class VsphereDiskList(FbBaseObject, MutableSequence):
-    """
-    A list containing VsphereDisk objects.
-    """
+    """A list containing VsphereDisk objects."""
 
-    msg_no_disk = _("Invalid type {t!r} as an item of a {c}, only {o} objects are allowed.")
+    msg_no_disk = _('Invalid type {t!r} as an item of a {c}, only {o} objects are allowed.')
 
     # -------------------------------------------------------------------------
     def __init__(
         self, appname=None, verbose=0, version=__version__, base_dir=None,
             initialized=None, *disks):
-
+        """Initialize a VsphereDiskList object."""
         self._list = []
 
         super(VsphereDiskList, self).__init__(
             appname=appname, verbose=verbose, version=version, base_dir=base_dir,
             initialized=False)
 
         for disk in disks:
@@ -450,25 +448,24 @@
 
         if initialized is not None:
             self.initialized = initialized
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True, bare=False):
         """
-        Transforms the elements of the object into a dict
+        Transform the elements of the object into a dict.
 
         @param short: don't include local properties in resulting dict.
         @type short: bool
         @param bare: don't include generic fields in returning dict
         @type bare: bool
 
         @return: structure as dict or list
         @rtype:  dict or list
         """
-
         if bare:
             res = []
             for disk in self:
                 res.append(disk.as_dict(bare=True))
             return res
 
         res = super(VsphereDiskList, self).as_dict(short=short)
@@ -477,34 +474,34 @@
         for disk in self:
             res['_list'].append(disk.as_dict(short=short))
 
         return res
 
     # -------------------------------------------------------------------------
     def __copy__(self):
-
+        """Return a new VsphereDiskList as a deep copy of the current object."""
         new_list = self.__class__(
             appname=self.appname, verbose=self.verbose,
             base_dir=self.base_dir, initialized=False)
 
         for disk in self:
             new_list.append(disk)
 
         new_list.initialized = self.initialized
         return new_list
 
     # -------------------------------------------------------------------------
     def index(self, disk, *args):
-
+        """Return the numeric index of the given disk in current list."""
         i = None
         j = None
 
         if len(args) > 0:
             if len(args) > 2:
-                raise TypeError(_("{m} takes at most {max} arguments ({n} given).").format(
+                raise TypeError(_('{m} takes at most {max} arguments ({n} given).').format(
                     m='index()', max=3, n=len(args) + 1))
             i = int(args[0])
             if len(args) > 1:
                 j = int(args[1])
 
         index = 0
         start = 0
@@ -536,20 +533,20 @@
             for index in list(range(len(self._list))):
                 item = self._list[index]
                 if index >= end:
                     break
             if item == disk:
                 return index
 
-        msg = _("Disk is not in disk list.")
+        msg = _('Disk is not in disk list.')
         raise ValueError(msg)
 
     # -------------------------------------------------------------------------
     def __contains__(self, disk):
-
+        """Return whether the given disk is contained in current list."""
         if not isinstance(disk, VsphereDisk):
             raise TypeError(self.msg_no_disk.format(
                 t=disk.__class__.__name__, c=self.__class__.__name__, o='VsphereDisk'))
 
         if not self._list:
             return False
 
@@ -557,15 +554,15 @@
             if item == disk:
                 return True
 
         return False
 
     # -------------------------------------------------------------------------
     def count(self, disk):
-
+        """Return the number of disks which are equal to the given one in current list."""
         if not isinstance(disk, VsphereDisk):
             raise TypeError(self.msg_no_disk.format(
                 t=disk.__class__.__name__, c=self.__class__.__name__, o='VsphereDisk'))
 
         if not self._list:
             return 0
 
@@ -573,71 +570,72 @@
         for item in self._list:
             if item == disk:
                 num += 1
         return num
 
     # -------------------------------------------------------------------------
     def __len__(self):
+        """Return the number of disks in current list."""
         return len(self._list)
 
     # -------------------------------------------------------------------------
     def __iter__(self):
-
+        """Iterate through all disks in current list."""
         for item in self._list:
             yield item
 
     # -------------------------------------------------------------------------
     def __getitem__(self, key):
+        """Get a disk from current list by the given numeric index."""
         return self._list.__getitem__(key)
 
     # -------------------------------------------------------------------------
     def __reversed__(self):
-
+        """Reverse the disks in list in place."""
         return reversed(self._list)
 
     # -------------------------------------------------------------------------
     def __setitem__(self, key, disk):
-
+        """Replace the disk at the given numeric index by the given one."""
         if not isinstance(disk, VsphereDisk):
             raise TypeError(self.msg_no_disk.format(
                 t=disk.__class__.__name__, c=self.__class__.__name__, o='VsphereDisk'))
 
         self._list.__setitem__(key, disk)
 
     # -------------------------------------------------------------------------
     def __delitem__(self, key):
-
+        """Remove the disk at the given numeric index from list."""
         del self._list[key]
 
     # -------------------------------------------------------------------------
     def append(self, disk):
-
+        """Append the given disk to the current list."""
         if not isinstance(disk, VsphereDisk):
             raise TypeError(self.msg_no_disk.format(
                 t=disk.__class__.__name__, c=self.__class__.__name__, o='VsphereDisk'))
 
         self._list.append(disk)
 
     # -------------------------------------------------------------------------
     def insert(self, index, disk):
-
+        """Insert the given disk in current list at given index."""
         if not isinstance(disk, VsphereDisk):
             raise TypeError(self.msg_no_disk.format(
                 t=disk.__class__.__name__, c=self.__class__.__name__, o='VsphereDisk'))
 
         self._list.insert(index, disk)
 
     # -------------------------------------------------------------------------
     def clear(self):
-        "Remove all items from the VsphereDiskList."
-
+        """Remove all items from the VsphereDiskList."""
         self._list = []
 
 
 # =============================================================================
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_vmware-0.5.7/lib/fb_vmware/ds_cluster.py` & `fb_vmware-0.6.0/lib/fb_vmware/ds_cluster.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
+@summary: The module for a VSphere datastore cluster object.
+
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 by Frank Brehm, Berlin
-@summary: The module for a VSphere datastore cluster object.
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
 import logging
-
 try:
     from collections.abc import MutableMapping
 except ImportError:
     from collections import MutableMapping
 
 # Third party modules
-from pyVmomi import vim
-
 from fb_tools.common import pp
 from fb_tools.obj import FbGenericBaseObject
 from fb_tools.xlate import format_list
 
-# Own modules
-from .xlate import XLATOR
+from pyVmomi import vim
 
+# Own modules
 from .obj import VsphereObject
+from .xlate import XLATOR
 
-__version__ = '1.3.2'
+__version__ = '1.3.3'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 
 
 # =============================================================================
 class VsphereDsCluster(VsphereObject):
+    """A wrapper for a Datastore cluster (dsPod)."""
 
     # -------------------------------------------------------------------------
     def __init__(
         self, appname=None, verbose=0, version=__version__, base_dir=None, initialized=None,
             name=None, status='gray', config_status='gray', capacity=None, free_space=None):
-
+        """Initialize a VsphereDsCluster object."""
         self.repr_fields = (
             'name', 'status', 'config_status', 'capacity', 'free_space',
             'appname', 'verbose', 'version')
 
         self._capacity = int(capacity)
         self._free_space = int(free_space)
 
         self._calculated_usage = 0.0
 
         super(VsphereDsCluster, self).__init__(
-            name=name, obj_type='vsphere_datastore_cluster', name_prefix="dspod",
+            name=name, obj_type='vsphere_datastore_cluster', name_prefix='dspod',
             status=status, config_status=config_status,
             appname=appname, verbose=verbose, version=version, base_dir=base_dir)
 
         if initialized is not None:
             self.initialized = initialized
 
     # -----------------------------------------------------------
@@ -103,15 +103,15 @@
         if not self.calculated_usage:
             return self.free_space_gb
         return self.free_space_gb - self.calculated_usage
 
     # -------------------------------------------------------------------------
     @classmethod
     def from_summary(cls, data, appname=None, verbose=0, base_dir=None, test_mode=False):
-
+        """Create a new VsphereDsCluster object based on the data given from pyvmomi."""
         if test_mode:
 
             necessary_fields = ('summary', 'overallStatus', 'configStatus')
             summary_fields = ('capacity', 'freeSpace', 'name')
 
             failing_fields = []
 
@@ -123,23 +123,23 @@
                 summary = data.summary
                 for field in summary_fields:
                     if not hasattr(summary, field):
                         failing_fields.append('summary.' + field)
 
             if len(failing_fields):
                 msg = _(
-                    "The given parameter {p!r} on calling method {m}() has failing "
-                    "attributes").format(p='data', m='from_summary')
+                    'The given parameter {p!r} on calling method {m}() has failing '
+                    'attributes').format(p='data', m='from_summary')
                 msg += ': ' + format_list(failing_fields, do_repr=True)
                 raise AssertionError(msg)
 
         else:
 
             if not isinstance(data, vim.StoragePod):
-                msg = _("Parameter {t!r} must be a {e}, {v!r} was given.").format(
+                msg = _('Parameter {t!r} must be a {e}, {v!r} was given.').format(
                     t='data', e='vim.StoragePod', v=data)
                 raise TypeError(msg)
 
         params = {
             'appname': appname,
             'verbose': verbose,
             'base_dir': base_dir,
@@ -148,82 +148,82 @@
             'free_space': data.summary.freeSpace,
             'name': data.summary.name,
             'status': data.overallStatus,
             'config_status': data.configStatus,
         }
 
         if verbose > 2:
-            LOG.debug(_("Creating {} object from:").format(cls.__name__) + '\n' + pp(params))
+            LOG.debug(_('Creating {} object from:').format(cls.__name__) + '\n' + pp(params))
 
         cluster = cls(**params)
         return cluster
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True):
         """
-        Transforms the elements of the object into a dict
+        Transform the elements of the object into a dict.
 
         @param short: don't include local properties in resulting dict.
         @type short: bool
 
         @return: structure as dict
         @rtype:  dict
         """
-
         res = super(VsphereDsCluster, self).as_dict(short=short)
         res['capacity'] = self.capacity
         res['capacity_gb'] = self.capacity_gb
         res['free_space'] = self.free_space
         res['free_space_gb'] = self.free_space_gb
         res['calculated_usage'] = self.calculated_usage
         res['avail_space_gb'] = self.avail_space_gb
 
         return res
 
     # -------------------------------------------------------------------------
     def __copy__(self):
-
+        """Return a new VsphereDsCluster as a deep copy of the current object."""
         return VsphereDsCluster(
             appname=self.appname, verbose=self.verbose, base_dir=self.base_dir,
             initialized=self.initialized, name=self.name, status=self.status,
             config_status=self.config_status, capacity=self.capacity, free_space=self.free_space,)
 
     # -------------------------------------------------------------------------
     def __eq__(self, other):
-
+        """Magic method for using it as the '=='-operator."""
         if self.verbose > 4:
-            LOG.debug(_("Comparing {} objects ...").format(self.__class__.__name__))
+            LOG.debug(_('Comparing {} objects ...').format(self.__class__.__name__))
 
         if not isinstance(other, VsphereDsCluster):
             return False
 
         if self.name != other.name:
             return False
 
         return True
 
 
 # =============================================================================
 class VsphereDsClusterDict(MutableMapping, FbGenericBaseObject):
     """
     A dictionary containing VsphereDsCluster objects.
+
     It works like a dict.
     """
 
-    msg_invalid_cluster_type = _("Invalid item type {{!r}} to set, only {} allowed.").format(
+    msg_invalid_cluster_type = _('Invalid item type {{!r}} to set, only {} allowed.').format(
         'VsphereDsCluster')
-    msg_key_not_name = _("The key {k!r} must be equal to the datastore cluster name {n!r}.")
-    msg_none_type_error = _("None type as key is not allowed.")
-    msg_empty_key_error = _("Empty key {!r} is not allowed.")
-    msg_no_cluster_dict = _("Object {{!r}} is not a {} object.").format('VsphereDsClusterDict.')
+    msg_key_not_name = _('The key {k!r} must be equal to the datastore cluster name {n!r}.')
+    msg_none_type_error = _('None type as key is not allowed.')
+    msg_empty_key_error = _('Empty key {!r} is not allowed.')
+    msg_no_cluster_dict = _('Object {{!r}} is not a {} object.').format('VsphereDsClusterDict.')
 
     # -------------------------------------------------------------------------
     def __init__(self, *args, **kwargs):
-        '''Use the object dict'''
-        self._map = dict()
+        """Initialize a VsphereDsClusterDict object."""
+        self._map = {}
 
         for arg in args:
             self.append(arg)
 
     # -------------------------------------------------------------------------
     def _set_item(self, key, cluster):
 
@@ -234,15 +234,15 @@
         if cluster_name != key:
             raise KeyError(self.msg_key_not_name.format(k=key, n=cluster_name))
 
         self._map[cluster_name] = cluster
 
     # -------------------------------------------------------------------------
     def append(self, cluster):
-
+        """Set the given datastore cluster in the current dict with its name as key."""
         if not isinstance(cluster, VsphereDsCluster):
             raise TypeError(self.msg_invalid_cluster_type.format(cluster.__class__.__name__))
         self._set_item(cluster.name, cluster)
 
     # -------------------------------------------------------------------------
     def _get_item(self, key):
 
@@ -253,14 +253,15 @@
         if cluster_name == '':
             raise ValueError(self.msg_empty_key_error.format(key))
 
         return self._map[cluster_name]
 
     # -------------------------------------------------------------------------
     def get(self, key):
+        """Get the datastore cluster from dict by its name."""
         return self._get_item(key)
 
     # -------------------------------------------------------------------------
     def _del_item(self, key, strict=True):
 
         if key is None:
             raise TypeError(self.msg_none_type_error)
@@ -273,128 +274,138 @@
             return
 
         del self._map[cluster_name]
 
     # -------------------------------------------------------------------------
     # The next five methods are requirements of the ABC.
     def __setitem__(self, key, value):
+        """Set the given datastore cluster in the current dict by key."""
         self._set_item(key, value)
 
     # -------------------------------------------------------------------------
     def __getitem__(self, key):
+        """Get the datastore cluster from dict by the key."""
         return self._get_item(key)
 
     # -------------------------------------------------------------------------
     def __delitem__(self, key):
+        """Remove the datastore cluster from dict by the key."""
         self._del_item(key)
 
     # -------------------------------------------------------------------------
     def __iter__(self):
-
+        """Iterate through datastore cluster names as keys."""
         for cluster_name in self.keys():
             yield cluster_name
 
     # -------------------------------------------------------------------------
     def __len__(self):
+        """Return the number of datastore clusters in current dict."""
         return len(self._map)
 
     # -------------------------------------------------------------------------
     # The next methods aren't required, but nice for different purposes:
     def __str__(self):
-        '''returns simple dict representation of the mapping'''
+        """Return simple dict representation of the mapping."""
         return str(self._map)
 
     # -------------------------------------------------------------------------
     def __repr__(self):
-        '''echoes class, id, & reproducible representation in the REPL'''
+        """Transform into a string for reproduction."""
         return '{}, {}({})'.format(
             super(VsphereDsClusterDict, self).__repr__(),
             self.__class__.__name__,
             self._map)
 
     # -------------------------------------------------------------------------
     def __contains__(self, key):
+        """Return whether the given datastore cluster name is contained in this dict as a key."""
         if key is None:
             raise TypeError(self.msg_none_type_error)
 
         cluster_name = str(key).strip()
         if cluster_name == '':
             raise ValueError(self.msg_empty_key_error.format(key))
 
         return cluster_name in self._map
 
     # -------------------------------------------------------------------------
     def keys(self):
-
+        """Return all datastore cluster names of this dict in a sorted manner."""
         return sorted(self._map.keys(), key=str.lower)
 
     # -------------------------------------------------------------------------
     def items(self):
-
+        """Return tuples (ds cluster name + object as tuple) of this dict in a sorted manner."""
         item_list = []
 
         for cluster_name in self.keys():
             item_list.append((cluster_name, self._map[cluster_name]))
 
         return item_list
 
     # -------------------------------------------------------------------------
     def values(self):
-
+        """Return all datastore cluster objects of this dict."""
         value_list = []
         for cluster_name in self.keys():
             value_list.append(self._map[cluster_name])
         return value_list
 
     # -------------------------------------------------------------------------
     def __eq__(self, other):
-
+        """Magic method for using it as the '=='-operator."""
         if not isinstance(other, VsphereDsClusterDict):
             raise TypeError(self.msg_no_cluster_dict.format(other))
 
         return self._map == other._map
 
     # -------------------------------------------------------------------------
     def __ne__(self, other):
-
+        """Magic method for using it as the '!='-operator."""
         if not isinstance(other, VsphereDsClusterDict):
             raise TypeError(self.msg_no_cluster_dict.format(other))
 
         return self._map != other._map
 
     # -------------------------------------------------------------------------
     def pop(self, key, *args):
-
+        """Get the datastore cluster by its name and remove it in dict."""
         if key is None:
             raise TypeError(self.msg_none_type_error)
 
         cluster_name = str(key).strip()
         if cluster_name == '':
             raise ValueError(self.msg_empty_key_error.format(key))
 
         return self._map.pop(cluster_name, *args)
 
     # -------------------------------------------------------------------------
     def popitem(self):
-
+        """Remove and return a arbitrary (ds cluster name and object) pair from the dictionary."""
         if not len(self._map):
             return None
 
         cluster_name = self.keys()[0]
         cluster = self._map[cluster_name]
         del self._map[cluster_name]
         return (cluster_name, cluster)
 
     # -------------------------------------------------------------------------
     def clear(self):
-        self._map = dict()
+        """Remove all items from the dictionary."""
+        self._map = {}
 
     # -------------------------------------------------------------------------
     def setdefault(self, key, default):
+        """
+        Return the datastore cluster, if the key is in dict.
 
+        If not, insert key with a value of default and return default.
+        """
         if key is None:
             raise TypeError(self.msg_none_type_error)
 
         cluster_name = str(key).strip()
         if cluster_name == '':
             raise ValueError(self.msg_empty_key_error.format(key))
 
@@ -405,44 +416,44 @@
             return self._map[cluster_name]
 
         self._set_item(cluster_name, default)
         return default
 
     # -------------------------------------------------------------------------
     def update(self, other):
-
+        """Update the dict with the key/value pairs from other, overwriting existing keys."""
         if isinstance(other, VsphereDsClusterDict) or isinstance(other, dict):
             for cluster_name in other.keys():
                 self._set_item(cluster_name, other[cluster_name])
             return
 
         for tokens in other:
             key = tokens[0]
             value = tokens[1]
             self._set_item(key, value)
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True):
-
+        """Transform the elements of the object into a dict."""
         res = {}
         for cluster_name in self._map:
             res[cluster_name] = self._map[cluster_name].as_dict(short)
         return res
 
     # -------------------------------------------------------------------------
     def as_list(self, short=True):
-
+        """Return a list with all datastore clusters transformed to a dict."""
         res = []
         for cluster_name in self.keys():
             res.append(self._map[cluster_name].as_dict(short))
         return res
 
 
 # =============================================================================
 
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_vmware-0.5.7/lib/fb_vmware/errors.py` & `fb_vmware-0.6.0/lib/fb_vmware/errors.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,270 +1,279 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
+@summary: The module for special error classes on VSphere API operations.
+
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 by Frank Brehm, Berlin
-@summary: The module for special error classes on VSphere API operations.
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
 
 # Third party modules
 
 from fb_tools.errors import FbHandlerError
 
 # Own modules
 from .xlate import XLATOR
 
-__version__ = '0.3.3'
+__version__ = '0.3.4'
 
 _ = XLATOR.gettext
 
 
 # =============================================================================
 class FbVMWareError(FbHandlerError):
     """Base class for all exception belonging to VSphere/VMWare."""
+
     pass
 
 
 # =============================================================================
 class BaseVSphereHandlerError(FbVMWareError):
     """Base class for all exception belonging to VSphere."""
+
     pass
 
 
 # =============================================================================
 class VSphereHandlerError(BaseVSphereHandlerError):
     """Base class for all exception belonging to VSphere."""
+
     pass
 
 
 # =============================================================================
 class VSphereNoDatastoresFoundError(FbHandlerError):
+    """Special error class used, if no appropriate datastore could be found."""
 
     # -------------------------------------------------------------------------
     def __init__(self, msg=None):
-
+        """Initialize the VSphereNoDatastoresFoundError object."""
         if not msg:
-            msg = _("No VSphere datastores found.")
+            msg = _('No VSphere datastores found.')
         self.msg = msg
 
     # -------------------------------------------------------------------------
     def __str__(self):
-
+        """Typecast into a string."""
         return self.msg
 
 
 # =============================================================================
 class VSphereExpectedError(VSphereHandlerError):
-    """Base class for all errors, which could be expected in application object
-        and displayed without stack trace."""
+    """
+    Base class for all expected application errors.
+
+    These are exceptions raised in application objects, which are
+    displayed without stack trace.
+    """
+
     pass
 
 
 # =============================================================================
 class VSphereNameError(VSphereExpectedError):
     """Special error class for invalid Vsphere object names."""
 
     # -------------------------------------------------------------------------
     def __init__(self, name, obj_type=None):
-
+        """Initialize the VSphereNameError object."""
         self.name = name
         self.obj_type = obj_type
 
     # -------------------------------------------------------------------------
     def __str__(self):
-
+        """Typecast into a string."""
         if self.obj_type:
-            msg = _("Invalid name {n!r} for a {o} VSphere object.").format(
+            msg = _('Invalid name {n!r} for a {o} VSphere object.').format(
                 n=self.name, o=self.obj_type)
         else:
-            msg = _("Invalid name {!r} for a VSphere object.").format(self.name)
+            msg = _('Invalid name {!r} for a VSphere object.').format(self.name)
 
         return msg
 
 
 # =============================================================================
 class VSphereDatacenterNotFoundError(VSphereExpectedError):
-    """Special error class for the case, that the given datacenter
-         was not found in VSphere."""
+    """Error class, if the given datacenter was not found in VSphere."""
 
     # -------------------------------------------------------------------------
     def __init__(self, dc):
-
+        """Initialize the VSphereDatacenterNotFoundError object."""
         self.dc = dc
 
     # -------------------------------------------------------------------------
     def __str__(self):
-
-        msg = _("The VSphere datacenter {!r} is not existing.").format(self.dc)
+        """Typecast into a string."""
+        msg = _('The VSphere datacenter {!r} is not existing.').format(self.dc)
         return msg
 
 
 # =============================================================================
 class VSphereVmNotFoundError(VSphereExpectedError):
     """Special error class for the case, that the given VM was not found in VSphere."""
 
     # -------------------------------------------------------------------------
     def __init__(self, vm):
-
+        """Initialize the VSphereVmNotFoundError object."""
         self.vm = vm
 
     # -------------------------------------------------------------------------
     def __str__(self):
-
-        msg = _("The VSphere Virtual machine {!r} was not found.").format(self.vm)
+        """Typecast into a string."""
+        msg = _('The VSphere Virtual machine {!r} was not found.').format(self.vm)
         return msg
 
 
 # =============================================================================
 class VSphereNoDatastoreFoundError(VSphereExpectedError):
-    """Special error class for the case, that no SAN based data store was with
-        enogh free space was found."""
+    """Error class for the case, if no SAN based data store was with enogh free space was found."""
 
     # -------------------------------------------------------------------------
     def __init__(self, needed_bytes):
-
+        """Initialize the VSphereNoDatastoreFoundError object."""
         self.needed_bytes = int(needed_bytes)
 
     # -------------------------------------------------------------------------
     def __str__(self):
-
+        """Typecast into a string."""
         mb = float(self.needed_bytes) / 1024.0 / 1024.0
         gb = mb / 1024.0
 
         msg = _(
-            "No SAN based datastore found with at least {m:0.0f} MiB == {g:0.1f} GiB "
-            "available space found.").format(m=mb, g=gb)
+            'No SAN based datastore found with at least {m:0.0f} MiB == {g:0.1f} GiB '
+            'available space found.').format(m=mb, g=gb)
         return msg
 
 
 # =============================================================================
 class VSphereNetworkNotExistingError(VSphereExpectedError):
     """Special error class for the case, if the expected network is not existing."""
 
     # -------------------------------------------------------------------------
     def __init__(self, net_name):
-
+        """Initialize the VSphereNetworkNotExistingError object."""
         self.net_name = net_name
 
     # -------------------------------------------------------------------------
     def __str__(self):
-
-        msg = _("The network {!r} is not existing.").format(self.net_name)
+        """Typecast into a string."""
+        msg = _('The network {!r} is not existing.').format(self.net_name)
         return msg
 
 
 # =============================================================================
 class VSphereCannotConnectError(VSphereExpectedError):
-    """Special error class for the case, it cannot connect
-        to the given vSphere server."""
+    """Error class, if it cannot connect to the given vSphere server."""
 
     # -------------------------------------------------------------------------
     def __init__(self, url):
-
+        """Initialize the VSphereCannotConnectError object."""
         self.url = url
 
     # -------------------------------------------------------------------------
     def __str__(self):
-
-        msg = _("Could not connect to the vSphere {!r}.").format(self.url)
+        """Typecast into a string."""
+        msg = _('Could not connect to the vSphere {!r}.').format(self.url)
         return msg
 
 # =============================================================================
 class VSphereVimFault(VSphereExpectedError):
-    """Special error class for the case, it cannot connect
-        to the given vSphere server and gets a vim.fault.VimFault."""
+    """Error class, if it cannot connect to vSphere and gets a vim.fault.VimFault."""
 
     # -------------------------------------------------------------------------
     def __init__(self, fault, url):
-
+        """Initialize the VSphereVimFault object."""
         self.fault = fault
         self.url = url
 
     # -------------------------------------------------------------------------
     def __str__(self):
-
-        msg = _("Got a {c} on connecting to vSphere {url!r}:").format(
+        """Typecast into a string."""
+        msg = _('Got a {c} on connecting to vSphere {url!r}:').format(
             c=self.fault.__class__.__name__, url=self.url)
         msg += ' ' + self.fault.msg
         return msg
 
 
 # =============================================================================
 class TimeoutCreateVmError(VSphereExpectedError):
+    """Exception when a timeout on creating a VM was reached."""
 
     # -------------------------------------------------------------------------
     def __init__(self, vm, timeout=None):
-
+        """Initialize the TimeoutCreateVmError object."""
         t_o = None
         if timeout is not None:
             t_o = float(timeout)
         self.timeout = t_o
 
         self.vm = vm
 
     # -------------------------------------------------------------------------
     def __str__(self):
-
+        """Typecast into a string."""
         if self.timeout is not None:
-            msg = _("Timeout on creating VM {vm!r} after {to:0.1f} seconds.").format(
+            msg = _('Timeout on creating VM {vm!r} after {to:0.1f} seconds.').format(
                 vm=self.vm, to=self.timeout)
         else:
-            msg = _("Timeout on creating VM {!r}.").format(self.vm)
+            msg = _('Timeout on creating VM {!r}.').format(self.vm)
         return msg
 
 
 # =============================================================================
 class WrongPortTypeError(FbVMWareError, TypeError):
+    """Exception when wrong VSPhere server port was given."""
 
     # -------------------------------------------------------------------------
     def __init__(self, port, emesg=None):
-
+        """Initialize the WrongPortTypeError object."""
         self.port = port
         self.emesg = emesg
 
     # -------------------------------------------------------------------------
     def __str__(self):
-
-        msg = _("Invalid type of {!r} for a port of a VSPhere server").format(self.port)
+        """Typecast into a string."""
+        msg = _('Invalid type of {!r} for a port of a VSPhere server').format(self.port)
         if self.emesg:
             msg += ': ' + self.emesg
         else:
             msg += '.'
 
         return msg
 
 # =============================================================================
 class WrongPortValueError(FbVMWareError, ValueError):
+    """Exception when a wrong port number was given."""
 
     default_max_port = (2 ** 16) - 1
 
     # -------------------------------------------------------------------------
     def __init__(self, port, max_port=None):
-
+        """Initialize the WrongPortValueError object."""
         self.port = port
         self.max_port = max_port
         if self.max_port is None:
             self.max_port = self.default_max_port
 
     # -------------------------------------------------------------------------
     def __str__(self):
-
+        """Typecast into a string."""
         msg = _(
-            "Invalid port number {port!r} for the VSphere server, "
-            "PORT must be greater than zero and less or equal to {max}.").format(
+            'Invalid port number {port!r} for the VSphere server, '
+            'PORT must be greater than zero and less or equal to {max}.').format(
             port=self.port, max=self.max_port)
 
         return msg
 
 
 # =============================================================================
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_vmware-0.5.7/lib/fb_vmware/ether.py` & `fb_vmware-0.6.0/lib/fb_vmware/ether.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
+@summary: The module for a VSphere ethernet card object.
+
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 by Frank Brehm, Berlin
-@summary: The module for a VSphere ethernet card object.
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
-import logging
 import copy
-
+import logging
 try:
     from collections.abc import MutableSequence
 except ImportError:
     from collections import MutableSequence
 
 # Third party modules
-from pyVmomi import vim
-
 from fb_tools.common import pp, to_bool
 from fb_tools.obj import FbBaseObject
 from fb_tools.xlate import format_list
 
+from pyVmomi import vim
+
 # Own modules
 from .xlate import XLATOR
 
-__version__ = '0.3.2'
+__version__ = '0.3.3'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 
 
 # =============================================================================
 class VsphereEthernetcard(FbBaseObject):
+    """Wrapper class for a vim.vm.device.VirtualEthernetCard object and for its descendants."""
 
     ether_types = {
         'e1000e': 'Virtual E1000e Ethernet adapter',
         'e1000': 'Virtual E1000 Ethernet adapter',
         'pcnet32': 'Virtual AMD Lance PCNet32 Ethernet adapter',
         'sriov': 'Virtual SR-IOV enabled Ethernet adapter',
         'vmxnet2': 'Virtual Vmxnet2 Ethernet adapter',
@@ -50,15 +51,15 @@
     # -------------------------------------------------------------------------
     def __init__(
         self, appname=None, verbose=0, version=__version__, base_dir=None, initialized=None,
             unit_nr=None, key=None, address_type=None, external_id=None, mac_address=None,
             wake_on_lan=False, backing_device=None, backing_type=None, connected=False,
             connect_status=None, connect_on_start=False, allow_guest_control=False,
             ether_type=None, label=None):
-
+        """Initialize the VsphereEthernetcard object."""
         self._unit_nr = None
         self._key = None
         self._address_type = None
         self._external_id = None
         self._mac_address = None
         self._wake_on_lan = False
         self._backing_device = None
@@ -91,31 +92,37 @@
 
         if initialized is not None:
             self.initialized = initialized
 
     # -----------------------------------------------------------
     @property
     def unit_nr(self):
-        """The unit number of this device on its controller.
-            This property is None if the controller property is None
-            (for example, when the device is not attached to a specific controller object)."""
+        """
+        The unit number of this device on its controller.
+
+        This property is None if the controller property is None
+        (for example, when the device is not attached to a specific controller object).
+        """
         return self._unit_nr
 
     @unit_nr.setter
     def unit_nr(self, value):
         if value is None:
             self._unit_nr = None
             return
         self._unit_nr = int(value)
 
     # -----------------------------------------------------------
     @property
     def key(self):
-        """A unique key that distinguishes this device from other devices
-            in the same virtual machine."""
+        """
+        A unique numeric key of the network device.
+
+        It distinguishes this device from other devices in the same virtual machine.
+        """
         return self._key
 
     @key.setter
     def key(self, value):
         if value is None:
             self._key = None
             return
@@ -137,16 +144,19 @@
             self._address_type = None
             return
         self._address_type = v
 
     # -----------------------------------------------------------
     @property
     def external_id(self):
-        """An ID assigned to the virtual network adapter by external
-            management plane or controller."""
+        """
+        An external ID assigned to the virtual network adapter.
+
+        It is assigned by external management plane or controller.
+        """
         return self._external_id
 
     @external_id.setter
     def external_id(self, value):
         if value is None:
             self._external_id = None
             return
@@ -296,17 +306,17 @@
         if v == '':
             self._label = None
             return
         self._label = v
 
     # -------------------------------------------------------------------------
     def __eq__(self, other):
-
+        """Magic method for using it as the '=='-operator."""
         if self.verbose > 4:
-            LOG.debug(_("Comparing {} objects ...").format(self.__class__.__name__))
+            LOG.debug(_('Comparing {} objects ...').format(self.__class__.__name__))
 
         if not isinstance(other, VsphereEthernetcard):
             return False
 
         if self.unit_nr != other.unit_nr:
             return False
         if self.key != other.key:
@@ -337,25 +347,24 @@
             return False
 
         return True
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True, bare=False):
         """
-        Transforms the elements of the object into a dict
+        Transform the elements of the object into a dict.
 
         @param short: don't include local properties in resulting dict.
         @type short: bool
         @param bare: don't include generic fields in returning dict
         @type bare: bool
 
         @return: structure as dict
         @rtype:  dict
         """
-
         if bare:
             res = {
                 'unit_nr': self.unit_nr,
                 'key': self.key,
                 'address_type': self.address_type,
                 'external_id': self.external_id,
                 'mac_address': self.mac_address,
@@ -387,15 +396,15 @@
         res['ether_type'] = self.ether_type
         res['label'] = self.label
 
         return res
 
     # -------------------------------------------------------------------------
     def __copy__(self):
-
+        """Return a new VsphereEthernetcard as a deep copy of the current object."""
         card = VsphereEthernetcard(
             appname=self.appname, verbose=self.verbose, base_dir=self.base_dir,
             initialized=self.initialized, unit_nr=self.unit_nr, key=self.key,
             address_type=self.address_type, external_id=self.external_id,
             mac_address=self.mac_address, wake_on_lan=self.wake_on_lan,
             backing_device=self.backing_device, backing_type=self.backing_type,
             connected=self.connected, connect_status=self.connect_status,
@@ -403,20 +412,20 @@
             ether_type=self.ether_type, label=self.label)
 
         return card
 
     # -------------------------------------------------------------------------
     @classmethod
     def from_summary(cls, data, appname=None, verbose=0, base_dir=None, test_mode=False):
-
+        """Create a new VsphereEthernetcard object based on the data given from pyvmomi."""
         if test_mode:
             cls._check_summary_data(data)
         else:
             if not isinstance(data, vim.vm.device.VirtualEthernetCard):
-                msg = _("Parameter {t!r} must be a {e}, {v!r} ({vt}) was given.").format(
+                msg = _('Parameter {t!r} must be a {e}, {v!r} ({vt}) was given.').format(
                     t='data', e='vim.vm.device.VirtualEthernetCard',
                     v=data, vt=data.__class__.__name__)
                 raise TypeError(msg)
 
         params = {
             'appname': appname,
             'verbose': verbose,
@@ -436,15 +445,15 @@
             'allow_guest_control': data.connectable.allowGuestControl,
             'ether_type': 'unknown',
         }
         if data.deviceInfo:
             params['label'] = data.deviceInfo.label
 
         if verbose > 2:
-            LOG.debug(_("Checking class of ethernet card: {!r}").format(data.__class__.__name__))
+            LOG.debug(_('Checking class of ethernet card: {!r}').format(data.__class__.__name__))
 
         try:
             if isinstance(data, vim.vm.device.VirtualE1000e):
                 params['ether_type'] = 'e1000e'
             elif isinstance(data, vim.vm.device.VirtualE1000):
                 params['ether_type'] = 'e1000'
             elif isinstance(data, vim.vm.device.VirtualPCNet32):
@@ -459,20 +468,20 @@
                 params['ether_type'] = 'vmxnet3'
             elif isinstance(data, vim.vm.device.VirtualVmxnet):
                 params['ether_type'] = 'vmxnet'
         except Exception:
             pass
 
         if verbose > 2:
-            LOG.debug(_("Creating {} object from:").format(cls.__name__) + '\n' + pp(params))
+            LOG.debug(_('Creating {} object from:').format(cls.__name__) + '\n' + pp(params))
 
         card = cls(**params)
 
         if verbose > 2:
-            LOG.debug(_("Created {} object:").format(cls.__name__) + '\n' + pp(card.as_dict()))
+            LOG.debug(_('Created {} object:').format(cls.__name__) + '\n' + pp(card.as_dict()))
 
         return card
 
     # -------------------------------------------------------------------------
     @classmethod
     def _check_summary_data(cls, data):
 
@@ -495,33 +504,31 @@
             connectable = data.connectable
             for field in connectable_fields:
                 if not hasattr(connectable, field):
                     failing_fields.append('connectable.' + field)
 
         if len(failing_fields):
             msg = _(
-                "The given parameter {p!r} on calling method {m}() has failing "
-                "attributes").format(p='data', m='from_summary')
+                'The given parameter {p!r} on calling method {m}() has failing '
+                'attributes').format(p='data', m='from_summary')
             msg += ': ' + format_list(failing_fields, do_repr=True)
             raise AssertionError(msg)
 
 
 # =============================================================================
 class VsphereEthernetcardList(FbBaseObject, MutableSequence):
-    """
-    A list containing VsphereEthernetcard objects.
-    """
+    """A list containing VsphereEthernetcard objects."""
 
-    msg_no_ether_card = _("Invalid type {t!r} as an item of a {c}, only {o} objects are allowed.")
+    msg_no_ether_card = _('Invalid type {t!r} as an item of a {c}, only {o} objects are allowed.')
 
     # -------------------------------------------------------------------------
     def __init__(
         self, appname=None, verbose=0, version=__version__, base_dir=None,
             initialized=None, *cards):
-
+        """Initialize a VsphereEthernetcardList object."""
         self._list = []
 
         super(VsphereEthernetcardList, self).__init__(
             appname=appname, verbose=verbose, version=version, base_dir=base_dir,
             initialized=False)
 
         for card in cards:
@@ -529,25 +536,24 @@
 
         if initialized is not None:
             self.initialized = initialized
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True, bare=False):
         """
-        Transforms the elements of the object into a dict
+        Transform the elements of the object into a dict.
 
         @param short: don't include local properties in resulting dict.
         @type short: bool
         @param bare: don't include generic fields in returning dict
         @type bare: bool
 
         @return: structure as dict or list
         @rtype:  dict or list
         """
-
         if bare:
             res = []
             for card in self:
                 res.append(card.as_dict(bare=True))
             return res
 
         res = super(VsphereEthernetcardList, self).as_dict(short=short)
@@ -556,34 +562,34 @@
         for card in self:
             res['_list'].append(card.as_dict(short=short))
 
         return res
 
     # -------------------------------------------------------------------------
     def __copy__(self):
-
+        """Return a new VsphereEthernetcardList as a deep copy of the current object."""
         new_list = self.__class__(
             appname=self.appname, verbose=self.verbose,
             base_dir=self.base_dir, initialized=False)
 
         for card in self:
             new_list.append(copy.copy(card))
 
         new_list.initialized = self.initialized
         return new_list
 
     # -------------------------------------------------------------------------
     def index(self, card, *args):
-
+        """Return the numeric index of the given controller in current list."""
         i = None
         j = None
 
         if len(args) > 0:
             if len(args) > 2:
-                raise TypeError(_("{m} takes at most {max} arguments ({n} given).").format(
+                raise TypeError(_('{m} takes at most {max} arguments ({n} given).').format(
                     m='index()', max=3, n=len(args) + 1))
             i = int(args[0])
             if len(args) > 1:
                 j = int(args[1])
 
         index = 0
         start = 0
@@ -614,20 +620,20 @@
             for index in list(range(len(self._list))):
                 item = self._list[index]
                 if index >= end:
                     break
             if item == card:
                 return index
 
-        msg = _("card is not in card list.")
+        msg = _('card is not in card list.')
         raise ValueError(msg)
 
     # -------------------------------------------------------------------------
     def __contains__(self, card):
-
+        """Return whether the given controller is contained in current list."""
         if not isinstance(card, VsphereEthernetcard):
             raise TypeError(self.msg_no_ether_card.format(
                 t=card.__class__.__name__, c=self.__class__.__name__, o='VsphereEthernetcard'))
 
         if not self._list:
             return False
 
@@ -635,15 +641,15 @@
             if item == card:
                 return True
 
         return False
 
     # -------------------------------------------------------------------------
     def count(self, card):
-
+        """Return the number of controllers which are equal to the given one in current list."""
         if not isinstance(card, VsphereEthernetcard):
             raise TypeError(self.msg_no_ether_card.format(
                 t=card.__class__.__name__, c=self.__class__.__name__, o='VsphereEthernetcard'))
 
         if not self._list:
             return 0
 
@@ -651,79 +657,80 @@
         for item in self._list:
             if item == card:
                 num += 1
         return num
 
     # -------------------------------------------------------------------------
     def __len__(self):
+        """Return the number of controllers in current list."""
         return len(self._list)
 
     # -------------------------------------------------------------------------
     def __iter__(self):
-
+        """Iterate through all controllers in current list."""
         for item in self._list:
             yield item
 
     # -------------------------------------------------------------------------
     def __getitem__(self, key):
+        """Get a controller from current list by the given numeric index."""
         return self._list.__getitem__(key)
 
     # -------------------------------------------------------------------------
     def __reversed__(self):
-
+        """Reverse the controllers in list in place."""
         new_list = self.__class__(
             appname=self.appname, verbose=self.verbose,
             base_dir=self.base_dir, initialized=False)
 
         for card in reversed(self._list):
             new_list.append(copy.copy(card))
 
         new_list.initialized = self.initialized
         return new_list
 
     # -------------------------------------------------------------------------
     def __setitem__(self, key, card):
-
+        """Replace the controller at the given numeric index by the given one."""
         if not isinstance(card, VsphereEthernetcard):
             raise TypeError(self.msg_no_ether_card.format(
                 t=card.__class__.__name__, c=self.__class__.__name__, o='VsphereEthernetcard'))
 
         self._list.__setitem__(key, card)
 
     # -------------------------------------------------------------------------
     def __delitem__(self, key):
-
+        """Remove the controller at the given numeric index from list."""
         del self._list[key]
 
     # -------------------------------------------------------------------------
     def append(self, card):
-
+        """Append the given controller to the current list."""
         if not isinstance(card, VsphereEthernetcard):
             raise TypeError(self.msg_no_ether_card.format(
                 t=card.__class__.__name__, c=self.__class__.__name__, o='VsphereEthernetcard'))
 
         self._list.append(card)
 
     # -------------------------------------------------------------------------
     def insert(self, index, card):
-
+        """Insert the given controller in current list at given index."""
         if not isinstance(card, VsphereEthernetcard):
             raise TypeError(self.msg_no_ether_card.format(
                 t=card.__class__.__name__, c=self.__class__.__name__, o='VsphereEthernetcard'))
 
         self._list.insert(index, card)
 
     # -------------------------------------------------------------------------
     def clear(self):
-        "Remove all items from the VsphereEthernetcardList."
-
+        """Remove all items from the VsphereEthernetcardList."""
         self._list = []
 
 
 # =============================================================================
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_vmware-0.5.7/lib/fb_vmware/host.py` & `fb_vmware-0.6.0/lib/fb_vmware/host.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,62 +1,60 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
+@summary: The module for capsulating a VSphere host system object.
+
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 by Frank Brehm, Berlin
-@summary: The module for capsulating a VSphere host system object.
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
-import logging
+import copy
 import datetime
-import uuid
 import ipaddress
-import copy
-
+import logging
+import uuid
 try:
     from collections.abc import MutableSequence
 except ImportError:
     from collections import MutableSequence
 
 # Third party modules
-from pyVmomi import vim
-
 from fb_tools.common import pp, to_bool
 from fb_tools.obj import FbBaseObject
 from fb_tools.xlate import format_list
 
-# Own modules
-from .errors import VSphereHandlerError
-
-from .obj import VsphereObject, DEFAULT_OBJ_STATUS, OBJ_STATUS_GREEN
+from pyVmomi import vim
 
+# Own modules
 from .about import VsphereAboutInfo
-
+from .errors import VSphereHandlerError
 from .host_port_group import VsphereHostPortgroup, VsphereHostPortgroupList
-
+from .obj import DEFAULT_OBJ_STATUS, OBJ_STATUS_GREEN
+from .obj import VsphereObject
 from .xlate import XLATOR
 
-__version__ = '0.7.3'
+__version__ = '0.7.4'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 
 
 # =============================================================================
 class VsphereHostBiosInfo(FbBaseObject):
+    """Wrapper class for virtual BIOS informations."""
 
     # -------------------------------------------------------------------------
     def __init__(
         self, bios_version=None, fw_major=None, fw_minor=None, major=None, minor=None,
             release_date=None, vendor=None, appname=None, verbose=0, version=__version__,
             base_dir=None, initialized=None):
-
+        """Initialize a VsphereHostBiosInfo object."""
         self._bios_version = None
         self._fw_major = None
         self._fw_minor = None
         self._major = None
         self._minor = None
         self._release_date = None
         self._vendor = None
@@ -196,69 +194,69 @@
             self._vendor = None
         else:
             self._vendor = v
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True):
         """
-        Transforms the elements of the object into a dict
+        Transform the elements of the object into a dict.
 
         @param short: don't include local properties in resulting dict.
         @type short: bool
 
         @return: structure as dict
         @rtype:  dict
         """
-
         res = super(VsphereHostBiosInfo, self).as_dict(short=short)
+
         res['bios_version'] = self.bios_version
         res['fw_major'] = self.fw_major
         res['fw_minor'] = self.fw_minor
         res['major'] = self.major
         res['minor'] = self.minor
         res['release_date'] = self.release_date
         res['vendor'] = self.vendor
 
         return res
 
     # -------------------------------------------------------------------------
     def __copy__(self):
-
+        """Return a new VsphereHostBiosInfo as a deep copy of the current object."""
         info = VsphereHostBiosInfo(
             appname=self.appname, verbose=self.verbose, base_dir=self.base_dir,
             initialized=self.initialized, bios_version=self.bios_version,
             fw_major=self.fw_major, fw_minor=self.fw_minor, major=self.major, minor=self.minor,
             release_date=self.release_date, vendor=self.vendor)
 
         return info
 
     # -------------------------------------------------------------------------
     @classmethod
     def from_summary(cls, data, appname=None, verbose=0, base_dir=None, test_mode=False):
-
+        """Create a new VsphereDiskController object based on the data given from pyvmomi."""
         if test_mode:
 
             necessary_fields = ('biosVersion', 'releaseDate')
 
             failing_fields = []
 
             for field in necessary_fields:
                 if not hasattr(data, field):
                     failing_fields.append(field)
 
             if len(failing_fields):
                 msg = _(
-                    "The given parameter {p!r} on calling method {m}() has failing "
-                    "attributes").format(p='data', m='from_summary')
+                    'The given parameter {p!r} on calling method {m}() has failing '
+                    'attributes').format(p='data', m='from_summary')
                 msg += ': ' + format_list(failing_fields, do_repr=True)
                 raise AssertionError(msg)
 
         else:
             if not isinstance(data, vim.host.BIOSInfo):
-                msg = _("Parameter {t!r} must be a {e}, {v!r} ({vt}) was given.").format(
+                msg = _('Parameter {t!r} must be a {e}, {v!r} ({vt}) was given.').format(
                     t='data', e='vim.host.BIOSInfo', v=data, vt=data.__class__.__name__)
                 raise TypeError(msg)
 
         params = {
             'appname': appname,
             'verbose': verbose,
             'base_dir': base_dir,
@@ -274,30 +272,31 @@
             params['major'] = data.majorRelease
         if hasattr(data, 'minorRelease'):
             params['minor'] = data.minorRelease
         if hasattr(data, 'vendor'):
             params['vendor'] = data.vendor
 
         if verbose > 2:
-            LOG.debug(_("Creating {} object from:").format(cls.__name__) + '\n' + pp(params))
+            LOG.debug(_('Creating {} object from:').format(cls.__name__) + '\n' + pp(params))
 
         bios = cls(**params)
 
         return bios
 
 
 # =============================================================================
 class VsphereHost(VsphereObject):
+    """Wrapper class for a vim.HostSystem, which is the represtation of a physical ESX host."""
 
     # -------------------------------------------------------------------------
     def __init__(
         self, appname=None, verbose=0, version=__version__, base_dir=None, initialized=None,
             name=None, cluster_name=None, vsphere=None, status=DEFAULT_OBJ_STATUS,
             config_status=DEFAULT_OBJ_STATUS):
-
+        """Initialize a VsphereHost object."""
         self.repr_fields = ('name', 'vsphere')
         self._vsphere = None
         self._cluster_name = None
         self.bios = None
         self.cpu_speed = None
         self.cpu_cores = None
         self.cpu_pkgs = None
@@ -317,39 +316,38 @@
         self.ipv6_enabled = None
         self.atboot_ipv6_enabled = None
         self.portgroups = None
 
         self.product = None
 
         super(VsphereHost, self).__init__(
-            name=name, obj_type='vsphere_host', name_prefix="host", status=status,
+            name=name, obj_type='vsphere_host', name_prefix='host', status=status,
             config_status=config_status, appname=appname, verbose=verbose,
             version=version, base_dir=base_dir)
 
         if vsphere is not None:
             self.vsphere = vsphere
 
         self.cluster_name = cluster_name
 
     # -----------------------------------------------------------
     @property
     def vsphere(self):
-        """The name of the VSPhere from configuration, in which
-            the host should be existing."""
+        """The name of the VSPhere from configuration, of thr host."""
         return self._vsphere
 
     @vsphere.setter
     def vsphere(self, value):
         if value is None:
             self._vsphere = None
             return
 
         val = str(value).strip()
         if val == '':
-            msg = _("The name of the vsphere may not be empty.")
+            msg = _('The name of the vsphere may not be empty.')
             raise VSphereHandlerError(msg)
 
         self._vsphere = val
 
     # -----------------------------------------------------------
     @property
     def cluster_name(self):
@@ -387,51 +385,51 @@
             except Exception:
                 pass
             self._mgmt_ip = v
 
     # -----------------------------------------------------------
     @property
     def memory_mb(self):
-        "The RAM of the host in MiByte."
+        """The RAM of the host in MiByte."""
         if self.memory is None:
             return None
         return int(self.memory / 1024 / 1024)
 
     # -----------------------------------------------------------
     @property
     def memory_gb(self):
-        "The RAM of the host in GiByte."
+        """The RAM of the host in GiByte."""
         if self.memory is None:
             return None
         return float(self.memory) / 1024.0 / 1024.0 / 1024.0
 
     # -----------------------------------------------------------
     @property
     def maintenance(self):
-        "Is the host in maintenance mode."
+        """Is the host in maintenance mode."""
         return self._maintenance
 
     @maintenance.setter
     def maintenance(self, value):
         self._maintenance = to_bool(value)
 
     # -----------------------------------------------------------
     @property
     def quarantaine(self):
-        "Is the host in quarantaine mode."
+        """Is the host in quarantaine mode."""
         return self._quarantaine
 
     @quarantaine.setter
     def quarantaine(self, value):
         self._quarantaine = to_bool(value)
 
     # -----------------------------------------------------------
     @property
     def reboot_required(self):
-        "Does the host needs a reboot."
+        """Does the host needs a reboot."""
         return self._reboot_required
 
     @reboot_required.setter
     def reboot_required(self, value):
         self._reboot_required = to_bool(value)
 
     # -----------------------------------------------------------
@@ -463,24 +461,24 @@
             self._boot_time = None
         else:
             self._boot_time = v
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True):
         """
-        Transforms the elements of the object into a dict
+        Transform the elements of the object into a dict.
 
         @param short: don't include local properties in resulting dict.
         @type short: bool
 
         @return: structure as dict
         @rtype:  dict
         """
-
         res = super(VsphereHost, self).as_dict(short=short)
+
         res['vsphere'] = self.vsphere
         res['cluster_name'] = self.cluster_name
         res['memory_mb'] = self.memory_mb
         res['memory_gb'] = self.memory_gb
         res['boot_time'] = self.boot_time
         res['maintenance'] = self.maintenance
         res['quarantaine'] = self.quarantaine
@@ -493,31 +491,30 @@
         if self.bios is not None:
             res['bios'] = self.bios.as_dict(short=short)
 
         return res
 
     # -------------------------------------------------------------------------
     def __repr__(self):
-        """Typecasting into a string for reproduction."""
-
-        out = "<%s(" % (self.__class__.__name__)
+        """Typecast into a string for reproduction."""
+        out = '<%s(' % (self.__class__.__name__)
 
         fields = []
-        fields.append("appname={!r}".format(self.appname))
-        fields.append("verbose={!r}".format(self.verbose))
-        fields.append("name={!r}".format(self.name))
-        fields.append("cluster_name={!r}".format(self.cluster_name))
-        fields.append("initialized={!r}".format(self.initialized))
+        fields.append('appname={!r}'.format(self.appname))
+        fields.append('verbose={!r}'.format(self.verbose))
+        fields.append('name={!r}'.format(self.name))
+        fields.append('cluster_name={!r}'.format(self.cluster_name))
+        fields.append('initialized={!r}'.format(self.initialized))
 
-        out += ", ".join(fields) + ")>"
+        out += ', '.join(fields) + ')>'
         return out
 
     # -------------------------------------------------------------------------
     def __copy__(self):
-
+        """Return a new VsphereHost as a deep copy of the current object."""
         host = VsphereHost(
             appname=self.appname, verbose=self.verbose, base_dir=self.base_dir,
             initialized=self.initialized, vsphere=self.vsphere, name=self.name, status=self.status,
             config_status=self.config_status, cluster_name=self.cluster_name)
 
         if self.bios:
             host.bios = copy.copy(self.bios)
@@ -540,17 +537,17 @@
         host.product = copy.copy(self.product)
         host.portgroups = copy.copy(self.portgroups)
 
         return host
 
     # -------------------------------------------------------------------------
     def __eq__(self, other):
-
+        """Magic method for using it as the '=='-operator."""
         if self.verbose > 4:
-            LOG.debug(_("Comparing {} objects ...").format(self.__class__.__name__))
+            LOG.debug(_('Comparing {} objects ...').format(self.__class__.__name__))
 
         if not isinstance(other, VsphereHost):
             return False
 
         if self.vsphere != other.vsphere:
             return False
         if self.name != other.name:
@@ -559,40 +556,40 @@
         return True
 
     # -------------------------------------------------------------------------
     @classmethod
     def from_summary(
             cls, data, vsphere=None, appname=None, verbose=0, base_dir=None,
             cluster_name=None, test_mode=False):
-
+        """Create a new VsphereHost object based on the data given from pyvmomi."""
         if test_mode:
             cls._check_summary_data(data)
         else:
             if not isinstance(data, vim.HostSystem):
-                msg = _("Parameter {t!r} must be a {e}, {v!r} ({vt}) was given.").format(
+                msg = _('Parameter {t!r} must be a {e}, {v!r} ({vt}) was given.').format(
                     t='data', e='vim.HostSystem', v=data, vt=data.__class__.__name__)
                 raise TypeError(msg)
 
         if not data.config:
-            LOG.error(_("Host {!r} seems to be offline!").format(data.summary.config.name))
+            LOG.error(_('Host {!r} seems to be offline!').format(data.summary.config.name))
 
         params = {
             'vsphere': vsphere,
             'appname': appname,
             'verbose': verbose,
             'base_dir': base_dir,
             'initialized': True,
             'name': data.summary.config.name,
             'cluster_name': cluster_name,
             'status': DEFAULT_OBJ_STATUS,
             'config_status': OBJ_STATUS_GREEN,
         }
 
         if verbose > 2:
-            LOG.debug(_("Creating {} object from:").format(cls.__name__) + '\n' + pp(params))
+            LOG.debug(_('Creating {} object from:').format(cls.__name__) + '\n' + pp(params))
 
         host = cls(**params)
 
         host.bios = VsphereHostBiosInfo.from_summary(
             data.hardware.biosInfo, appname=appname, verbose=verbose, base_dir=base_dir,
             test_mode=test_mode)
 
@@ -655,89 +652,87 @@
 
         if hasattr(data, 'hardware'):
             failing_fields += cls._check_hardware_data(data.hardware)
 
         if hasattr(data, 'runtime'):
             for field in runtime_fields:
                 if not hasattr(data.runtime, field):
-                    failing_fields.append("runtime." + field)
+                    failing_fields.append('runtime.' + field)
 
         if hasattr(data, 'summary'):
             for field in summary_fields:
                 if not hasattr(data.summary, field):
-                    failing_fields.append("summary." + field)
+                    failing_fields.append('summary.' + field)
 
         if hasattr(data, 'config') and data.config:
             failing_fields += cls._check_config_data(data.config)
 
         if len(failing_fields):
             msg = _(
-                "The given parameter {p!r} on calling method {m}() has failing "
-                "attributes").format(p='data', m='from_summary')
+                'The given parameter {p!r} on calling method {m}() has failing '
+                'attributes').format(p='data', m='from_summary')
             msg += ': ' + format_list(failing_fields, do_repr=True)
             raise AssertionError(msg)
 
     # -------------------------------------------------------------------------
     @classmethod
     def _check_hardware_data(cls, hardware):
 
         hardware_fields = ('biosInfo', 'cpuInfo', 'memorySize', 'systemInfo')
         cpu_fields = ('hz', 'numCpuCores', 'numCpuPackages', 'numCpuThreads')
         failing_fields = []
 
         for field in hardware_fields:
             if not hasattr(hardware, field):
-                failing_fields.append("hardware." + field)
+                failing_fields.append('hardware.' + field)
 
         if hasattr(hardware, 'cpuInfo'):
             for field in cpu_fields:
                 if not hasattr(hardware.cpuInfo, field):
-                    failing_fields.append("hardware.cpuInfo." + field)
+                    failing_fields.append('hardware.cpuInfo.' + field)
 
         if hasattr(hardware, 'systemInfo'):
             if not hasattr(hardware.systemInfo, 'model'):
-                failing_fields.append("hardware.systemInfo.model")
+                failing_fields.append('hardware.systemInfo.model')
             if not hasattr(hardware.systemInfo, 'vendor'):
-                failing_fields.append("hardware.systemInfo.vendor")
+                failing_fields.append('hardware.systemInfo.vendor')
 
         return failing_fields
 
     # -------------------------------------------------------------------------
     @classmethod
     def _check_config_data(cls, config):
 
         failing_fields = []
 
         if not hasattr(config, 'product'):
-            failing_fields.append("config.product")
+            failing_fields.append('config.product')
         if not hasattr(config, 'network'):
-            failing_fields.append("config.network")
+            failing_fields.append('config.network')
         elif config.network:
             for field in ('ipV6Enabled', 'atBootIpV6Enabled', 'portgroup'):
                 if not hasattr(config.network, field):
-                    failing_fields.append("config.network." + field)
+                    failing_fields.append('config.network.' + field)
 
         return failing_fields
 
 
 # =============================================================================
 class VsphereHostList(FbBaseObject, MutableSequence):
-    """
-    A list containing VsphereHost objects.
-    """
+    """A list containing VsphereHost objects."""
 
     msg_no_host = _(
-        "Invalid type {{t!r}} as an item of a {{c}}, only {} objects are allowed.").format(
+        'Invalid type {{t!r}} as an item of a {{c}}, only {} objects are allowed.').format(
             'VsphereHost')
 
     # -------------------------------------------------------------------------
     def __init__(
         self, appname=None, verbose=0, version=__version__, base_dir=None,
             initialized=None, *hosts):
-
+        """Initialize a VsphereHostList object."""
         self._list = []
 
         super(VsphereHostList, self).__init__(
             appname=appname, verbose=verbose, version=version, base_dir=base_dir,
             initialized=False)
 
         for host in hosts:
@@ -745,25 +740,24 @@
 
         if initialized is not None:
             self.initialized = initialized
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True, bare=False):
         """
-        Transforms the elements of the object into a dict
+        Transform the elements of the object into a dict.
 
         @param short: don't include local properties in resulting dict.
         @type short: bool
         @param bare: don't include generic fields in returning dict
         @type bare: bool
 
         @return: structure as dict or list
         @rtype:  dict or list
         """
-
         if bare:
             res = []
             for host in self:
                 res.append(host.as_dict(short=True))
             return res
 
         res = super(VsphereHostList, self).as_dict(short=short)
@@ -772,34 +766,34 @@
         for host in self:
             res['_list'].append(host.as_dict(short=short))
 
         return res
 
     # -------------------------------------------------------------------------
     def __copy__(self):
-
+        """Return a new VsphereHostList as a deep copy of the current object."""
         new_list = self.__class__(
             appname=self.appname, verbose=self.verbose, base_dir=self.base_dir,
             initialized=False)
 
         for host in self:
             new_list.append(copy.copy(host))
 
         new_list.initialized = self.initialized
         return new_list
 
     # -------------------------------------------------------------------------
     def index(self, host, *args):
-
+        """Return the numeric index of the given host in current list."""
         i = None
         j = None
 
         if len(args) > 0:
             if len(args) > 2:
-                raise TypeError(_("{m} takes at most {max} arguments ({n} given).").format(
+                raise TypeError(_('{m} takes at most {max} arguments ({n} given).').format(
                     m='index()', max=3, n=len(args) + 1))
             i = int(args[0])
             if len(args) > 1:
                 j = int(args[1])
 
         index = 0
         start = 0
@@ -830,20 +824,20 @@
             for index in list(range(len(self._list))):
                 item = self._list[index]
                 if index >= end:
                     break
             if item == host:
                 return index
 
-        msg = _("host is not in host list.")
+        msg = _('host is not in host list.')
         raise ValueError(msg)
 
     # -------------------------------------------------------------------------
     def __contains__(self, host):
-
+        """Return whether the given host is contained in current list."""
         if not isinstance(host, VsphereHost):
             raise TypeError(self.msg_no_host.format(
                 t=host.__class__.__name__, c=self.__class__.__name__))
 
         if not self._list:
             return False
 
@@ -851,15 +845,15 @@
             if item == host:
                 return True
 
         return False
 
     # -------------------------------------------------------------------------
     def count(self, host):
-
+        """Return the number of hosts which are equal to the given one in current list."""
         if not isinstance(host, VsphereHost):
             raise TypeError(self.msg_no_host.format(
                 t=host.__class__.__name__, c=self.__class__.__name__))
 
         if not self._list:
             return 0
 
@@ -867,88 +861,89 @@
         for item in self._list:
             if item == host:
                 num += 1
         return num
 
     # -------------------------------------------------------------------------
     def __len__(self):
+        """Return the number of hosts in current list."""
         return len(self._list)
 
     # -------------------------------------------------------------------------
     def __iter__(self):
-
+        """Iterate through all hosts in current list."""
         for item in self._list:
             yield item
 
     # -------------------------------------------------------------------------
     def __getitem__(self, key):
+        """Get a host from current list by the given numeric index."""
         return self._list.__getitem__(key)
 
     # -------------------------------------------------------------------------
     def __reversed__(self):
-
+        """Reverse the hosts in list in place."""
         new_list = self.__class__(
             appname=self.appname, verbose=self.verbose,
             base_dir=self.base_dir, initialized=False)
 
         for host in reversed(self._list):
             new_list.append(copy.copy(host))
 
         new_list.initialized = self.initialized
         return new_list
 
     # -------------------------------------------------------------------------
     def __setitem__(self, key, host):
-
+        """Replace the host at the given numeric index by the given one."""
         if not isinstance(host, VsphereHost):
             raise TypeError(self.msg_no_host.format(
                 t=host.__class__.__name__, c=self.__class__.__name__))
 
         self._list.__setitem__(key, host)
 
     # -------------------------------------------------------------------------
     def __delitem__(self, key):
-
+        """Remove the host at the given numeric index from list."""
         del self._list[key]
 
     # -------------------------------------------------------------------------
     def append(self, host):
-
+        """Append the given host to the current list."""
         if not isinstance(host, VsphereHost):
             raise TypeError(self.msg_no_host.format(
                 t=host.__class__.__name__, c=self.__class__.__name__))
 
         self._list.append(host)
 
     # -------------------------------------------------------------------------
     def insert(self, index, host):
-
+        """Insert the given host in current list at given index."""
         if not isinstance(host, VsphereHost):
             raise TypeError(self.msg_no_host.format(
                 t=host.__class__.__name__, c=self.__class__.__name__))
 
         self._list.insert(index, host)
 
     # -------------------------------------------------------------------------
     def clear(self):
-        "Remove all items from the VsphereHostList."
-
+        """Remove all items from the VsphereHostList."""
         self._list = []
 
     # -------------------------------------------------------------------------
     def ordered(self):
-
+        """Iterate through the hosts in sorted order."""
         try:
             for host in sorted(self._list, key=lambda x: x.name.lower()):
                 yield host
         except StopIteration:
             pass
 
 
 # =============================================================================
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_vmware-0.5.7/lib/fb_vmware/host_port_group.py` & `fb_vmware-0.6.0/lib/fb_vmware/host_port_group.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
+@summary: The module for a VSphere host portgroup object.
+
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 by Frank Brehm, Berlin
-@summary: The module for a VSphere host portgroup object.
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
-import logging
 import copy
-
+import logging
 try:
     from collections.abc import MutableSequence
 except ImportError:
     from collections import MutableSequence
 
 # Third party modules
-from pyVmomi import vim
-
 from fb_tools.common import pp
 # from fb_tools.common import to_bool
 from fb_tools.obj import FbBaseObject
 from fb_tools.xlate import format_list
 
+from pyVmomi import vim
+
 # Own modules
 from .xlate import XLATOR
 
-__version__ = '0.2.3'
+__version__ = '0.2.4'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 
 
 # =============================================================================
 class VsphereHostPortgroup(FbBaseObject):
+    """This is a wrapeer for a vim.host.PortGroup object."""
 
     # -------------------------------------------------------------------------
     def __init__(
         self, appname=None, verbose=0, version=__version__, base_dir=None, initialized=None,
             name=None, vlan_id=None, vswitch_name=None, hostname=None):
-
+        """Initialize a VsphereHostPortgroup object."""
         self._name = None
         self._vlan_id = None
         self._vswitch_name = None
         self._hostname = None
 
         super(VsphereHostPortgroup, self).__init__(
             appname=appname, verbose=verbose, version=version,
@@ -122,25 +123,24 @@
             self._hostname = None
             return
         self._hostname = v
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True, bare=False):
         """
-        Transforms the elements of the object into a dict
+        Transform the elements of the object into a dict.
 
         @param short: don't include local properties in resulting dict.
         @type short: bool
         @param bare: don't include generic fields in returning dict
         @type bare: bool
 
         @return: structure as dict
         @rtype:  dict
         """
-
         if bare:
             res = {
                 'name': self.name,
                 'vlan_id': self.vlan_id,
                 'vswitch_name': self.vswitch_name,
                 'hostname': self.hostname,
             }
@@ -152,62 +152,62 @@
         res['vswitch_name'] = self.vswitch_name
         res['hostname'] = self.hostname
 
         return res
 
     # -------------------------------------------------------------------------
     def __eq__(self, other):
-
+        """Magic method for using it as the '=='-operator."""
         if self.verbose > 4:
-            LOG.debug(_("Comparing {} objects ...").format(self.__class__.__name__))
+            LOG.debug(_('Comparing {} objects ...').format(self.__class__.__name__))
 
         if not isinstance(other, VsphereHostPortgroup):
             return False
 
         if self.hostname != other.hostname:
             return False
         if self.name != other.name:
             return False
 
         return True
 
     # -------------------------------------------------------------------------
     def __copy__(self):
-
+        """Return a new VsphereHostPortgroup as a deep copy of the current object."""
         group = VsphereHostPortgroup(
             appname=self.appname, verbose=self.verbose, base_dir=self.base_dir,
             initialized=self.initialized, name=self.name, vlan_id=self.vlan_id,
             vswitch_name=self.vswitch_name, hostname=self.hostname)
 
         return group
 
     # -------------------------------------------------------------------------
     @classmethod
     def from_summary(
             cls, data, hostname=None, appname=None, verbose=0, base_dir=None, test_mode=False):
-
+        """Create a new VsphereHostPortgroup object based on the data given from pyvmomi."""
         if test_mode:
 
             failing_fields = []
             if not hasattr(data, 'spec'):
                 failing_fields.append('spec')
             else:
                 for field in ('name', 'vlanId', 'vswitchName'):
                     failing_fields.append('spec.' + field)
 
             if len(failing_fields):
                 msg = _(
-                    "The given parameter {p!r} on calling method {m}() has failing "
-                    "attributes").format(p='data', m='from_summary')
+                    'The given parameter {p!r} on calling method {m}() has failing '
+                    'attributes').format(p='data', m='from_summary')
                 msg += ': ' + format_list(failing_fields, do_repr=True)
                 raise AssertionError(msg)
 
         else:
             if not isinstance(data, vim.host.PortGroup):
-                msg = _("Parameter {t!r} must be a {e}, {v!r} ({vt}) was given.").format(
+                msg = _('Parameter {t!r} must be a {e}, {v!r} ({vt}) was given.').format(
                     t='data', e='vim.host.PortGroup', v=data, vt=data.__class__.__name__)
                 raise TypeError(msg)
 
         params = {
             'appname': appname,
             'verbose': verbose,
             'base_dir': base_dir,
@@ -215,37 +215,35 @@
             'name': data.spec.name,
             'vlan_id': data.spec.vlanId,
             'vswitch_name': data.spec.vswitchName,
             'hostname': hostname,
         }
 
         if verbose > 2:
-            LOG.debug(_("Creating {} object from:").format(cls.__name__) + '\n' + pp(params))
+            LOG.debug(_('Creating {} object from:').format(cls.__name__) + '\n' + pp(params))
 
         group = cls(**params)
 
         if verbose > 2:
-            LOG.debug(_("Created {} object:").format(cls.__name__) + '\n' + pp(group.as_dict()))
+            LOG.debug(_('Created {} object:').format(cls.__name__) + '\n' + pp(group.as_dict()))
 
         return group
 
 
 # =============================================================================
 class VsphereHostPortgroupList(FbBaseObject, MutableSequence):
-    """
-    A list containing VsphereHostPortgroup objects.
-    """
+    """A list containing VsphereHostPortgroup objects."""
 
-    msg_no_portgroup = _("Invalid type {t!r} as an item of a {c}, only {o} objects are allowed.")
+    msg_no_portgroup = _('Invalid type {t!r} as an item of a {c}, only {o} objects are allowed.')
 
     # -------------------------------------------------------------------------
     def __init__(
         self, appname=None, verbose=0, version=__version__, base_dir=None,
             initialized=None, hostname=None, *groups):
-
+        """Initialize a VsphereHostPortgroupList object."""
         self._list = []
         self._hostname = None
 
         super(VsphereHostPortgroupList, self).__init__(
             appname=appname, verbose=verbose, version=version, base_dir=base_dir,
             initialized=False)
 
@@ -273,25 +271,24 @@
             self._hostname = None
             return
         self._hostname = v
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True, bare=False):
         """
-        Transforms the elements of the object into a dict
+        Transform the elements of the object into a dict.
 
         @param short: don't include local properties in resulting dict.
         @type short: bool
         @param bare: don't include generic fields in returning dict
         @type bare: bool
 
         @return: structure as dict or list
         @rtype:  dict or list
         """
-
         if bare:
             res = []
             for group in self:
                 res.append(group.as_dict(bare=True))
             return res
 
         res = super(VsphereHostPortgroupList, self).as_dict(short=short)
@@ -301,34 +298,34 @@
         for group in self:
             res['_list'].append(group.as_dict(short=short))
 
         return res
 
     # -------------------------------------------------------------------------
     def __copy__(self):
-
+        """Return a new VsphereHostPortgroupList as a deep copy of the current object."""
         new_list = self.__class__(
             appname=self.appname, verbose=self.verbose, base_dir=self.base_dir,
             hostname=self.hostname, initialized=False)
 
         for group in self:
             new_list.append(copy.copy(group))
 
         new_list.initialized = self.initialized
         return new_list
 
     # -------------------------------------------------------------------------
     def index(self, group, *args):
-
+        """Return the numeric index of the given port group in current list."""
         i = None
         j = None
 
         if len(args) > 0:
             if len(args) > 2:
-                raise TypeError(_("{m} takes at most {max} arguments ({n} given).").format(
+                raise TypeError(_('{m} takes at most {max} arguments ({n} given).').format(
                     m='index()', max=3, n=len(args) + 1))
             i = int(args[0])
             if len(args) > 1:
                 j = int(args[1])
 
         index = 0
         start = 0
@@ -359,20 +356,20 @@
             for index in list(range(len(self._list))):
                 item = self._list[index]
                 if index >= end:
                     break
             if item == group:
                 return index
 
-        msg = _("group is not in group list.")
+        msg = _('group is not in group list.')
         raise ValueError(msg)
 
     # -------------------------------------------------------------------------
     def __contains__(self, group):
-
+        """Return whether the given port group is contained in current list."""
         if not isinstance(group, VsphereHostPortgroup):
             raise TypeError(self.msg_no_portgroup.format(
                 t=group.__class__.__name__, c=self.__class__.__name__, o='VsphereHostPortgroup'))
 
         if not self._list:
             return False
 
@@ -380,15 +377,15 @@
             if item == group:
                 return True
 
         return False
 
     # -------------------------------------------------------------------------
     def count(self, group):
-
+        """Return the number of port groups which are equal to the given one in current list."""
         if not isinstance(group, VsphereHostPortgroup):
             raise TypeError(self.msg_no_portgroup.format(
                 t=group.__class__.__name__, c=self.__class__.__name__, o='VsphereHostPortgroup'))
 
         if not self._list:
             return 0
 
@@ -396,82 +393,83 @@
         for item in self._list:
             if item == group:
                 num += 1
         return num
 
     # -------------------------------------------------------------------------
     def __len__(self):
+        """Return the number of port groups in current list."""
         return len(self._list)
 
     # -------------------------------------------------------------------------
     def __getitem__(self, key):
+        """Get a port group from current list by the given numeric index."""
         return self._list.__getitem__(key)
 
     # -------------------------------------------------------------------------
     def __reversed__(self):
-
+        """Reverse the port groups in list in place."""
         new_list = self.__class__(
             appname=self.appname, verbose=self.verbose,
             base_dir=self.base_dir, initialized=False)
 
         for group in reversed(self._list):
             new_list.append(copy.copy(group))
 
         new_list.initialized = self.initialized
         return new_list
 
     # -------------------------------------------------------------------------
     def __setitem__(self, key, group):
-
+        """Replace the port group at the given numeric index by the given one."""
         if not isinstance(group, VsphereHostPortgroup):
             raise TypeError(self.msg_no_portgroup.format(
                 t=group.__class__.__name__, c=self.__class__.__name__, o='VsphereHostPortgroup'))
 
         self._list.__setitem__(key, group)
 
     # -------------------------------------------------------------------------
     def __delitem__(self, key):
-
+        """Remove the port group at the given numeric index from list."""
         del self._list[key]
 
     # -------------------------------------------------------------------------
     def append(self, group):
-
+        """Append the given port group to the current list."""
         if not isinstance(group, VsphereHostPortgroup):
             raise TypeError(self.msg_no_portgroup.format(
                 t=group.__class__.__name__, c=self.__class__.__name__, o='VsphereHostPortgroup'))
 
         self._list.append(group)
 
     # -------------------------------------------------------------------------
     def insert(self, index, group):
-
+        """Insert the given port group in current list at given index."""
         if not isinstance(group, VsphereHostPortgroup):
             raise TypeError(self.msg_no_portgroup.format(
                 t=group.__class__.__name__, c=self.__class__.__name__, o='VsphereHostPortgroup'))
 
         self._list.insert(index, group)
 
     # -------------------------------------------------------------------------
     def clear(self):
-        "Remove all items from the VsphereHostPortgroupList."
-
+        """Remove all items from the VsphereHostPortgroupList."""
         self._list = []
 
     # -------------------------------------------------------------------------
     def ordered(self):
-
+        """Iterate through the port groups in sorted order."""
         try:
             for group in sorted(self._list, key=lambda x: x.name.lower()):
                 yield group
         except StopIteration:
             pass
 
 
 # =============================================================================
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_vmware-0.5.7/lib/fb_vmware/iface.py` & `fb_vmware-0.6.0/lib/fb_vmware/iface.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
+@summary: The module for a VSphere object for a network interface of a VM.
+
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 by Frank Brehm, Berlin
-@summary: The module for a VSphere network object.
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
 import logging
 
 # Third party modules
-from pyVmomi import vim
-
-from fb_tools.common import pp, RE_MAC_ADRESS
+from fb_tools.common import RE_MAC_ADRESS
+from fb_tools.common import pp
 from fb_tools.obj import FbBaseObject
 
+from pyVmomi import vim
+
 # Own modules
 from .errors import VSphereNameError
-
 from .xlate import XLATOR
 
 
-__version__ = '1.2.2'
+__version__ = '1.2.3'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 
 
 # =============================================================================
 class VsphereVmInterface(FbBaseObject):
+    """A wrapper class for a network interface of a VM (vim.Network)."""
 
     # -------------------------------------------------------------------------
     def __init__(
         self, appname=None, verbose=0, version=__version__, base_dir=None, initialized=None,
             name=None, network=None, network_name=None, mac_address=None, summary=None):
-
+        """Initialize a VsphereVmInterface object."""
         self.repr_fields = (
             'name', 'network_name', 'mac_address', 'summary', 'appname', 'verbose')
 
         self._name = None
         self.network = None
         self._network_name = None
         self._mac_address = None
@@ -50,15 +52,15 @@
             appname=appname, verbose=verbose, version=version, base_dir=base_dir)
 
         self.name = name
         self.mac_address = mac_address
 
         if network:
             if not isinstance(network, vim.Network):
-                msg = _("Parameter {t!r} must be a {e}, {v!r} was given.").format(
+                msg = _('Parameter {t!r} must be a {e}, {v!r} was given.').format(
                     t='network', e='vim.Network', v=network)
                 raise TypeError(msg)
             self._network = network
 
         self.network_name = network_name
         self.summary = summary
 
@@ -118,15 +120,15 @@
             self._mac_address = None
             return
         val = value.strip()
         if val == '':
             self._mac_address = None
             return
         if not RE_MAC_ADRESS.match(val):
-            msg = _("Invalid MAC address {!r} for interface given.").format(value)
+            msg = _('Invalid MAC address {!r} for interface given.').format(value)
             raise ValueError(msg)
 
         self._mac_address = val.lower()
 
     # -----------------------------------------------------------
     @property
     def summary(self):
@@ -143,47 +145,45 @@
             self._summary = None
             return
         self._summary = val
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True):
         """
-        Transforms the elements of the object into a dict
+        Transform the elements of the object into a dict.
 
         @param short: don't include local properties in resulting dict.
         @type short: bool
 
         @return: structure as dict
         @rtype:  dict
         """
-
         res = super(VsphereVmInterface, self).as_dict(short=short)
+
         res['name'] = self.name
         res['obj_type'] = self.obj_type
         res['network_name'] = self.network_name
         res['mac_address'] = self.mac_address
         res['summary'] = self.summary
 
         return res
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """
-        Typecasting function for translating object structure
-        into a string
+        Typecast function for translating object structure into a string.
 
         @return: structure as string
         @rtype:  str
         """
-
         return pp(self.as_dict(short=True))
 
 
 # =============================================================================
 
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_vmware-0.5.7/lib/fb_vmware/locale/de_DE/LC_MESSAGES/fb_vmware.mo` & `fb_vmware-0.6.0/lib/fb_vmware/locale/de_DE/LC_MESSAGES/fb_vmware.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,20 +1,20 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: fb_vmware 0.4.6\n"
+"Project-Id-Version: fb_vmware 0.5.7\n"
 "Report-Msgid-Bugs-To: frank@brehm-online.com\n"
-"PO-Revision-Date: 2022-06-09 17:45+0200\n"
+"PO-Revision-Date: 2023-07-13 17:20+0200\n"
 "Last-Translator: Frank Brehm <frank@brehm-online.com>\n"
 "Language: de_DE\n"
 "Language-Team: Frank Brehm <frank@brehm-online.com>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.1\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid ""
 "A regular expression to filter the output list of VMs by the VMWare hardware "
 "configuration version (e.g. '{}')."
 msgstr ""
 "Ein regulärer Ausdruck, um die Ausgabeliste der VMs nach ihrer VMWare-"
 "Hardwarekonfigurationsversion zu filtern (z.Bsp. '{}')."
@@ -538,14 +538,17 @@
 
 msgid "Powering off VM {!r} ..."
 msgstr "Schalte VM {!r} aus …"
 
 msgid "Powering on VM {!r} ..."
 msgstr "Schalte VM {!r} ein …"
 
+msgid "Pulling full data of VM {!r} ..."
+msgstr "Hole vollständige Daten der VM {!r} …"
+
 msgid "Purging VM {!r} ..."
 msgstr "Lösche VM {!r} vollständig …"
 
 msgid "Regular expression for filtering: {!r}"
 msgstr "Regulärer Ausdruck als Filter: {!r}"
 
 msgid "Searching VSphere network for address {} ..."
@@ -881,27 +884,29 @@
 msgstr[1] "Netzwerke"
 
 msgid "thread"
 msgid_plural "threads"
 msgstr[0] "Thread"
 msgstr[1] "Threads"
 
+msgid ""
+"{c}-Object:\n"
+"{a}"
+msgstr ""
+"{c}-Objekt:\n"
+"{a}"
+
 msgid "{e} in section {sn!r} for VSphere {vs!r}:"
 msgstr "{e} in Abschnitt {sn!r} für VSphere {vs!r}:"
 
 msgid "{m} takes at most {max} arguments ({n} given)."
 msgstr "{m} akzeptiert höchstens {max} Argumente ({n} wurden gegeben)."
 
-msgid "{nr:>2} disk "
-msgid_plural "{nr:>2} disks"
-msgstr[0] "{nr:>2} Platte "
-msgstr[1] "{nr:>2} Platten"
-
 msgid ""
 "{on} {cl!r}, {h} {h_l}, {cpu} {cpu_l}, {thr} {t_l}, {mem:0.1f} GiB Memory, "
 "{net} {nw_l} and {ds} {ds_l}."
 msgstr ""
 "{on} {cl!r}, {h} {h_l}, {cpu} {cpu_l}, {thr} {t_l}, {mem:0.1f} GiB "
 "Hauptspeicher, {net} {nw_l} und {ds} {ds_l}."
 
-msgid "{what} of {app} .."
+msgid "{what} of {app} ..."
 msgstr "{what} von {app} …"
```

### Comparing `fb_vmware-0.5.7/lib/fb_vmware/locale/en_US/LC_MESSAGES/fb_vmware.mo` & `fb_vmware-0.6.0/lib/fb_vmware/locale/en_US/LC_MESSAGES/fb_vmware.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,20 +1,20 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: fb_vmware 0.4.6\n"
+"Project-Id-Version: fb_vmware 0.5.7\n"
 "Report-Msgid-Bugs-To: frank@brehm-online.com\n"
-"PO-Revision-Date: 2022-06-09 16:20+0200\n"
+"PO-Revision-Date: 2022-07-13 17:21+0200\n"
 "Last-Translator: Frank Brehm <frank@brehm-online.com>\n"
 "Language: en_US\n"
 "Language-Team: Frank Brehm <frank@brehm-online.com>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.1\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Checking VM {!r} ..."
 msgstr "Checking VM {!r} …"
 
 msgid "Checking VM {!r} for being a template ..."
 msgstr "Checking VM {!r} for being a template …"
 
@@ -71,14 +71,17 @@
 
 msgid "Powering off VM {!r} ..."
 msgstr "Powering off VM {!r} …"
 
 msgid "Powering on VM {!r} ..."
 msgstr "Powering on VM {!r} …"
 
+msgid "Pulling full data of VM {!r} ..."
+msgstr "Pulling full data of VM {!r} …"
+
 msgid "Purging VM {!r} ..."
 msgstr "Purging VM {!r} …"
 
 msgid "Searching VSphere network for address {} ..."
 msgstr "Searching VSphere network for address {} …"
 
 msgid "Searching for VM {n!r} (pattern: {p!r}) in VSPhere {v!r} ..."
@@ -127,9 +130,9 @@
 
 msgid "Waiting for tasks to finish ..."
 msgstr "Waiting for tasks to finish …"
 
 msgid "Waiting for tasks {} to finish ..."
 msgstr "Waiting for tasks {} to finish …"
 
-msgid "{what} of {app} .."
+msgid "{what} of {app} ..."
 msgstr "{what} of {app} …"
```

### Comparing `fb_vmware-0.5.7/lib/fb_vmware/network.py` & `fb_vmware-0.6.0/lib/fb_vmware/network.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,94 +1,95 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
+@summary: The module for a VSphere network object.
+
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 by Frank Brehm, Berlin
-@summary: The module for a VSphere network object.
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
+import functools
+import ipaddress
 import logging
 import re
-import ipaddress
-import functools
-
 try:
     from collections.abc import MutableMapping
 except ImportError:
     from collections import MutableMapping
 
 # Third party modules
-from pyVmomi import vim
-
 from fb_tools.common import pp
 from fb_tools.obj import FbGenericBaseObject
 from fb_tools.xlate import format_list
 
-# Own modules
-from .obj import VsphereObject, DEFAULT_OBJ_STATUS
+from pyVmomi import vim
 
+# Own modules
+from .obj import DEFAULT_OBJ_STATUS
+from .obj import VsphereObject
 from .xlate import XLATOR
 
-__version__ = '1.3.3'
+__version__ = '1.3.4'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 
 
 # =============================================================================
 class VsphereNetwork(VsphereObject):
+    """Wrapper class for a Network definition in VSPhere (vim.Network)."""
 
     re_ipv4_name = re.compile(r'\s*((?:\d{1,3}\.){3}\d{1,3})_(\d+)\s*$')
     re_tf_name = re.compile(r'[^a-z0-9_]+', re.IGNORECASE)
 
     # -------------------------------------------------------------------------
     def __init__(
         self, appname=None, verbose=0, version=__version__, base_dir=None, initialized=None,
             name=None, status=DEFAULT_OBJ_STATUS, config_status=DEFAULT_OBJ_STATUS,
             accessible=True, ip_pool_id=None, ip_pool_name=None):
-
+        """Initialize a VsphereNetwork object."""
         self.repr_fields = (
             'name', 'obj_type', 'status', 'config_status', 'accessible',
             'ip_pool_id', 'ip_pool_name', 'appname', 'verbose')
 
         self._accessible = bool(accessible)
         self._ip_pool_id = ip_pool_id
         self._ip_pool_name = ip_pool_name
 
         self._network = None
 
         super(VsphereNetwork, self).__init__(
-            name=name, obj_type='vsphere_network', name_prefix="net", status=status,
+            name=name, obj_type='vsphere_network', name_prefix='net', status=status,
             config_status=config_status, appname=appname, verbose=verbose,
             version=version, base_dir=base_dir)
 
         match = self.re_ipv4_name.search(self.name)
         if match:
-            ip = "{a}/{m}".format(a=match.group(1), m=match.group(2))
+            ip = '{a}/{m}'.format(a=match.group(1), m=match.group(2))
             if self.verbose > 3:
-                LOG.debug(_("Trying to get IPv4 network {n!r} -> {i!r}.").format(
+                LOG.debug(_('Trying to get IPv4 network {n!r} -> {i!r}.').format(
                     n=self.name, i=ip))
 
             try:
                 net = ipaddress.ip_network(ip)
                 self._network = net
             except ValueError:
-                LOG.error(_("Could not get IP network from network name {!r}.").format(self.name))
+                LOG.error(_('Could not get IP network from network name {!r}.').format(self.name))
 
         if not self.network:
-            LOG.warning(_("Network {!r} has no IP network assigned.").format(self.name))
+            LOG.warning(_('Network {!r} has no IP network assigned.').format(self.name))
 
         if initialized is not None:
             self.initialized = initialized
 
         if self.verbose > 3:
-            LOG.debug(_("Initialized network object:") + '\n' + pp(self.as_dict()))
+            LOG.debug(_('Initialized network object:') + '\n' + pp(self.as_dict()))
 
     # -----------------------------------------------------------
     @property
     def accessible(self):
         """The connectivity status of this network."""
         return self._accessible
 
@@ -117,15 +118,15 @@
         if not self.network:
             return None
         return self.network.network_address + 1
 
     # -------------------------------------------------------------------------
     @classmethod
     def from_summary(cls, data, appname=None, verbose=0, base_dir=None, test_mode=False):
-
+        """Create a new VsphereNetwork object based on the data given from pyvmomi."""
         if test_mode:
 
             necessary_fields = ('summary', 'overallStatus', 'configStatus')
 
             failing_fields = []
 
             for field in necessary_fields:
@@ -134,22 +135,22 @@
 
             if hasattr(data, 'summary'):
                 if not hasattr(data.summary, 'name'):
                     failing_fields.append('summary.name')
 
             if len(failing_fields):
                 msg = _(
-                    "The given parameter {p!r} on calling method {m}() has failing "
-                    "attributes").format(p='data', m='from_summary')
+                    'The given parameter {p!r} on calling method {m}() has failing '
+                    'attributes').format(p='data', m='from_summary')
                 msg += ': ' + format_list(failing_fields, do_repr=True)
                 raise AssertionError(msg)
 
         else:
             if not isinstance(data, vim.Network):
-                msg = _("Parameter {t!r} must be a {e}, {v!r} was given.").format(
+                msg = _('Parameter {t!r} must be a {e}, {v!r} was given.').format(
                     t='data', e='vim.Network', v=data)
                 raise TypeError(msg)
 
         params = {
             'appname': appname,
             'verbose': verbose,
             'base_dir': base_dir,
@@ -165,101 +166,106 @@
         if hasattr(data.summary, 'ipPoolId'):
             params['ip_pool_id'] = data.summary.ipPoolId
 
         if hasattr(data.summary, 'ipPoolName'):
             params['ip_pool_name'] = data.summary.ipPoolName
 
         if verbose > 3:
-            LOG.debug(_("Creating {} object from:").format(cls.__name__) + '\n' + pp(params))
+            LOG.debug(_('Creating {} object from:').format(cls.__name__) + '\n' + pp(params))
 
         net = cls(**params)
         return net
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True):
         """
-        Transforms the elements of the object into a dict
+        Transform the elements of the object into a dict.
 
         @param short: don't include local properties in resulting dict.
         @type short: bool
 
         @return: structure as dict
         @rtype:  dict
         """
-
         res = super(VsphereNetwork, self).as_dict(short=short)
+
         res['accessible'] = self.accessible
         res['ip_pool_id'] = self.ip_pool_id
         res['ip_pool_name'] = self.ip_pool_name
         res['network'] = self.network
         res['gateway'] = self.gateway
 
         return res
 
     # -------------------------------------------------------------------------
     def __copy__(self):
-
+        """Return a new VsphereNetwork as a deep copy of the current object."""
         return VsphereNetwork(
             appname=self.appname, verbose=self.verbose, base_dir=self.base_dir,
             initialized=self.initialized, name=self.name, accessible=self.accessible,
             ip_pool_id=self.ip_pool_id, ip_pool_name=self.ip_pool_name,
             status=self.status, config_status=self.config_status)
 
     # -------------------------------------------------------------------------
     def __eq__(self, other):
-
+        """Magic method for using it as the '=='-operator."""
         if self.verbose > 4:
-            LOG.debug(_("Comparing {} objects ...").format(self.__class__.__name__))
+            LOG.debug(_('Comparing {} objects ...').format(self.__class__.__name__))
 
         if not isinstance(other, VsphereNetwork):
             return False
 
         if self.name != other.name:
             return False
 
         return True
 
 
 # =============================================================================
 class VsphereNetworkDict(MutableMapping, FbGenericBaseObject):
     """
     A dictionary containing VsphereNetwork objects.
+
     It works like a dict.
     """
 
-    msg_invalid_net_type = _("Invalid item type {{!r}} to set, only {} allowed.").format(
+    msg_invalid_net_type = _('Invalid item type {{!r}} to set, only {} allowed.').format(
         'VsphereNetwork')
-    msg_key_not_name = _("The key {k!r} must be equal to the network name {n!r}.")
-    msg_none_type_error = _("None type as key is not allowed.")
-    msg_empty_key_error = _("Empty key {!r} is not allowed.")
-    msg_no_net_dict = _("Object {{!r}} is not a {} object.").format('VsphereNetworkDict')
+    msg_key_not_name = _('The key {k!r} must be equal to the network name {n!r}.')
+    msg_none_type_error = _('None type as key is not allowed.')
+    msg_empty_key_error = _('Empty key {!r} is not allowed.')
+    msg_no_net_dict = _('Object {{!r}} is not a {} object.').format('VsphereNetworkDict')
 
     # -------------------------------------------------------------------------
     def __init__(self, *args, **kwargs):
-        '''Use the object dict'''
-        self._map = dict()
+        """Initialize a VsphereNetworkDict object."""
+        self._map = {}
 
         for arg in args:
             self.append(arg)
 
     # -------------------------------------------------------------------------
     def _set_item(self, key, net):
+        """
+        Set the given Network to the given key.
 
+        The key must be identic to the name of the network.
+        """
         if not isinstance(net, VsphereNetwork):
             raise TypeError(self.msg_invalid_net_type.format(net.__class__.__name__))
 
         net_name = net.name
         if net_name != key:
             raise KeyError(self.msg_key_not_name.format(k=key, n=net_name))
 
         self._map[net_name] = net
 
     # -------------------------------------------------------------------------
     def append(self, net):
-
+        """Set the given network in the current dict with its name as key."""
         if not isinstance(net, VsphereNetwork):
             raise TypeError(self.msg_invalid_net_type.format(net.__class__.__name__))
         self._set_item(net.name, net)
 
     # -------------------------------------------------------------------------
     def _get_item(self, key):
 
@@ -270,14 +276,15 @@
         if net_name == '':
             raise ValueError(self.msg_empty_key_error.format(key))
 
         return self._map[net_name]
 
     # -------------------------------------------------------------------------
     def get(self, key):
+        """Get the network from dict by its name."""
         return self._get_item(key)
 
     # -------------------------------------------------------------------------
     def _del_item(self, key, strict=True):
 
         if key is None:
             raise TypeError(self.msg_none_type_error)
@@ -290,62 +297,67 @@
             return
 
         del self._map[net_name]
 
     # -------------------------------------------------------------------------
     # The next five methods are requirements of the ABC.
     def __setitem__(self, key, value):
+        """Set the given network in the current dict by key."""
         self._set_item(key, value)
 
     # -------------------------------------------------------------------------
     def __getitem__(self, key):
+        """Get the network from dict by the key."""
         return self._get_item(key)
 
     # -------------------------------------------------------------------------
     def __delitem__(self, key):
+        """Remove the network from dict by the key."""
         self._del_item(key)
 
     # -------------------------------------------------------------------------
     def __iter__(self):
-
+        """Iterate through network names as keys."""
         for net_name in self.keys():
             yield net_name
 
     # -------------------------------------------------------------------------
     def __len__(self):
+        """Return the number of networks in current dict."""
         return len(self._map)
 
     # -------------------------------------------------------------------------
     # The next methods aren't required, but nice for different purposes:
     def __str__(self):
-        '''returns simple dict representation of the mapping'''
+        """Return simple dict representation of the mapping."""
         return str(self._map)
 
     # -------------------------------------------------------------------------
     def __repr__(self):
-        '''echoes class, id, & reproducible representation in the REPL'''
+        """Transform into a string for reproduction."""
         return '{}, {}({})'.format(
             super(VsphereNetworkDict, self).__repr__(),
             self.__class__.__name__,
             self._map)
 
     # -------------------------------------------------------------------------
     def __contains__(self, key):
+        """Return whether the given network name is contained in current dict as a key."""
         if key is None:
             raise TypeError(self.msg_none_type_error)
 
         net_name = str(key).strip()
         if net_name == '':
             raise ValueError(self.msg_empty_key_error.format(key))
 
         return net_name in self._map
 
     # -------------------------------------------------------------------------
     def keys(self):
-
+        """Return all network names of this dict in a sorted manner."""
         def netsort(x, y):
             net_x = self[x]
             net_y = self[y]
             if net_x.network is None and net_y.network is None:
                 return (
                     (net_x.name.lower() > net_y.name.lower()) - (
                         net_x.name.lower() < net_y.name.lower()))
@@ -359,76 +371,81 @@
                 return 1
             return 0
 
         return sorted(self._map.keys(), key=functools.cmp_to_key(netsort))
 
     # -------------------------------------------------------------------------
     def items(self):
-
+        """Return tuples (network name + object as tuple) of this dict in a sorted manner."""
         item_list = []
 
         for net_name in self.keys():
             item_list.append((net_name, self._map[net_name]))
 
         return item_list
 
     # -------------------------------------------------------------------------
     def values(self):
-
+        """Return all network objects of this dict."""
         value_list = []
         for net_name in self.keys():
             value_list.append(self._map[net_name])
         return value_list
 
     # -------------------------------------------------------------------------
     def __eq__(self, other):
-
+        """Magic method for using it as the '=='-operator."""
         if not isinstance(other, VsphereNetworkDict):
             raise TypeError(self.msg_no_net_dict.format(other))
 
         return self._map == other._map
 
     # -------------------------------------------------------------------------
     def __ne__(self, other):
-
+        """Magic method for using it as the '!='-operator."""
         if not isinstance(other, VsphereNetworkDict):
             raise TypeError(self.msg_no_net_dict.format(other))
 
         return self._map != other._map
 
     # -------------------------------------------------------------------------
     def pop(self, key, *args):
-
+        """Get the network by its name and remove it in dict."""
         if key is None:
             raise TypeError(self.msg_none_type_error)
 
         net_name = str(key).strip()
         if net_name == '':
             raise ValueError(self.msg_empty_key_error.format(key))
 
         return self._map.pop(net_name, *args)
 
     # -------------------------------------------------------------------------
     def popitem(self):
-
+        """Remove and return a arbitrary (network name and object) pair from the dictionary."""
         if not len(self._map):
             return None
 
         net_name = self.keys()[0]
         net = self._map[net_name]
         del self._map[net_name]
         return (net_name, net)
 
     # -------------------------------------------------------------------------
     def clear(self):
-        self._map = dict()
+        """Remove all items from the dictionary."""
+        self._map = {}
 
     # -------------------------------------------------------------------------
     def setdefault(self, key, default):
+        """
+        Return the network, if the key is in dict.
 
+        If not, insert key with a value of default and return default.
+        """
         if key is None:
             raise TypeError(self.msg_none_type_error)
 
         net_name = str(key).strip()
         if net_name == '':
             raise ValueError(self.msg_empty_key_error.format(key))
 
@@ -439,63 +456,68 @@
             return self._map[net_name]
 
         self._set_item(net_name, default)
         return default
 
     # -------------------------------------------------------------------------
     def update(self, other):
-
+        """Update the dict with the key/value pairs from other, overwriting existing keys."""
         if isinstance(other, VsphereNetworkDict) or isinstance(other, dict):
             for net_name in other.keys():
                 self._set_item(net_name, other[net_name])
             return
 
         for tokens in other:
             key = tokens[0]
             value = tokens[1]
             self._set_item(key, value)
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True):
-
+        """Transform the elements of the object into a dict."""
         res = {}
         for net_name in self._map:
             res[net_name] = self._map[net_name].as_dict(short)
         return res
 
     # -------------------------------------------------------------------------
     def as_list(self, short=True):
-
+        """Return a list with all networks transformed to a dict."""
         res = []
         for net_name in self.keys():
             res.append(self._map[net_name].as_dict(short))
         return res
 
     # -------------------------------------------------------------------------
     def get_network_for_ip(self, *ips):
+        """
+        Search a fitting network for the give IP addresses.
 
+        The name of the first matching network for the first IP address, which will
+        have a match, will be returned.
+        """
         for ip in ips:
             if not ip:
                 continue
-            LOG.debug(_("Searching VSphere network for address {} ...").format(ip))
+            LOG.debug(_('Searching VSphere network for address {} ...').format(ip))
             ipa = ipaddress.ip_address(ip)
 
             for net_name in self.keys():
                 net = self[net_name]
                 if net.network and ipa in net.network:
-                    LOG.debug(_("Found network {n!r} for IP {i}.").format(
+                    LOG.debug(_('Found network {n!r} for IP {i}.').format(
                         n=net_name, i=ip))
                     return net_name
 
-            LOG.debug(_("Could not find VSphere network for IP {}.").format(ip))
+            LOG.debug(_('Could not find VSphere network for IP {}.').format(ip))
 
-        ips_str = ', '.join(map(lambda x: str(x), list(filter(bool, ips))))
-        LOG.error(_("Could not find VSphere network for IP addresses {}.").format(ips_str))
+        ips_str = ', '.join((str(x) for x in list(filter(bool, ips))))
+        LOG.error(_('Could not find VSphere network for IP addresses {}.').format(ips_str))
         return None
 
 
 # =============================================================================
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_vmware-0.5.7/lib/fb_vmware/obj.py` & `fb_vmware-0.6.0/lib/fb_vmware/obj.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,56 +1,62 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
+@summary: The module for a base VSphere class.
+
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 by Frank Brehm, Berlin
-@summary: The base module module for a VSphere object.
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
-import re
-import logging
 import copy
+import logging
+import re
 
 # Third party modules
-from fb_tools.common import pp, RE_TF_NAME
+from fb_tools.common import RE_TF_NAME
+from fb_tools.common import pp
 from fb_tools.obj import FbBaseObject
 
 # Own modules
-from .xlate import XLATOR
-
 from .errors import VSphereNameError
+from .xlate import XLATOR
 
-__version__ = '1.3.2'
+__version__ = '1.3.3'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 
 DEFAULT_OBJ_STATUS = 'gray'
 OBJ_STATUS_GREEN = 'green'
 
 
 # =============================================================================
 class VsphereObject(FbBaseObject):
+    """
+    A base class for some other VSphere classes.
+
+    It is especially intended for classes mapping other classes from the pyVmomi package.
+    """
 
     re_ws = re.compile(r'\s+')
 
     repr_fields = (
         'name', 'obj_type', 'name_prefix', 'status', 'config_status',
         'appname', 'verbose', 'version')
     available_status_color = ['red', 'yellow', 'green', 'gray']
 
     # -------------------------------------------------------------------------
     def __init__(
-        self, name=None, obj_type=None, name_prefix="unknown", status=DEFAULT_OBJ_STATUS,
+        self, name=None, obj_type=None, name_prefix='unknown', status=DEFAULT_OBJ_STATUS,
             config_status=DEFAULT_OBJ_STATUS, appname=None, verbose=0, version=__version__,
             base_dir=None, initialized=None):
-
+        """Initialize a VsphereObject object."""
         self._name = None
         self._obj_type = None
         self._name_prefix = None
         self._status = None
         self._config_status = None
 
         super(VsphereObject, self).__init__(
@@ -71,20 +77,20 @@
         """The type of the VSphere object."""
         return self._obj_type
 
     @obj_type.setter
     def obj_type(self, value):
 
         if value is None:
-            msg = _("The type of a {} may not be None.").format('VsphereObject')
+            msg = _('The type of a {} may not be None.').format('VsphereObject')
             raise TypeError(msg)
 
         val = self.re_ws.sub('', str(value))
         if val == '':
-            msg = _("Invalid {w}.{p} {v!r}.").format(
+            msg = _('Invalid {w}.{p} {v!r}.').format(
                 w='VsphereObject', p='type', v=value)
             raise ValueError(msg)
 
         self._obj_type = val
 
     # -----------------------------------------------------------
     @property
@@ -99,15 +105,15 @@
             return
 
         val = str(value).strip().lower()
         if val == '':
             self._status = 'gray'
             return
         if val not in self.available_status_color:
-            msg = _("Invalid {w}.{p} {v!r}.").format(
+            msg = _('Invalid {w}.{p} {v!r}.').format(
                 w='VsphereObject', p='status', v=value)
             raise ValueError(msg)
 
         self._status = val
 
     # -----------------------------------------------------------
     @property
@@ -122,15 +128,15 @@
             return
 
         val = str(value).strip().lower()
         if val == '':
             self._config_status = 'gray'
             return
         if val not in self.available_status_color:
-            msg = _("Invalid {w}.{p} {v!r}.").format(
+            msg = _('Invalid {w}.{p} {v!r}.').format(
                 w='VsphereObject', p='config_status', v=value)
             raise ValueError(msg)
 
         self._config_status = val
 
     # -----------------------------------------------------------
     @property
@@ -138,19 +144,19 @@
         """The prefix for the terraform name."""
         return self._name_prefix
 
     @name_prefix.setter
     def name_prefix(self, value):
 
         if value is None:
-            raise TypeError(_("The name prefix of a {} may not be None.").format('VsphereObject'))
+            raise TypeError(_('The name prefix of a {} may not be None.').format('VsphereObject'))
 
         val = self.re_ws.sub('', str(value))
         if val == '':
-            msg = _("Invalid name prefix {p!r} for a {o}.").format(p=value, o='VsphereObject')
+            msg = _('Invalid name prefix {p!r} for a {o}.').format(p=value, o='VsphereObject')
             raise ValueError(msg)
 
         self._name_prefix = val
 
     # -----------------------------------------------------------
     @property
     def name(self):
@@ -169,15 +175,14 @@
 
         self._name = val
 
     # -----------------------------------------------------------
     @property
     def qual_name(self):
         """The qualified name of the object, including object_type and name."""
-
         if self.obj_type is None:
             if self.name is None:
                 return ''
             else:
                 return self.name.lower()
         if self.name is None:
             return self.obj_type.lower() + '.'
@@ -196,24 +201,24 @@
     def var_name(self):
         """The name of the variable used in terraform definitions."""
         return self.obj_type + '_' + RE_TF_NAME.sub('_', self.name.lower())
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True):
         """
-        Transforms the elements of the object into a dict
+        Transform the elements of the object into a dict.
 
         @param short: don't include local properties in resulting dict.
         @type short: bool
 
         @return: structure as dict
         @rtype:  dict
         """
-
         res = super(VsphereObject, self).as_dict(short=short)
+
         res['name'] = self.name
         res['qual_name'] = self.qual_name
         res['obj_type'] = self.obj_type
         res['name_prefix'] = self.name_prefix
         res['tf_name'] = self.tf_name
         res['var_name'] = self.var_name
         res['repr_fields'] = copy.copy(self.repr_fields)
@@ -221,93 +226,90 @@
         res['config_status'] = self.config_status
 
         return res
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """
-        Typecasting function for translating object structure
-        into a string
+        Typecast function for translating object structure into a string.
 
         @return: structure as string
         @rtype:  str
         """
-
         return pp(self.as_dict(short=True))
 
     # -------------------------------------------------------------------------
     def __repr__(self):
-        """Typecasting into a string for reproduction."""
-
-        out = "<%s(" % (self.__class__.__name__)
+        """Typecast into a string for reproduction."""
+        out = '<%s(' % (self.__class__.__name__)
 
         fields = []
         for field in self.repr_fields:
-            token = "{f}={v!r}".format(f=field, v=getattr(self, field))
+            token = '{f}={v!r}'.format(f=field, v=getattr(self, field))
             fields.append(token)
 
-        out += ", ".join(fields) + ")>"
+        out += ', '.join(fields) + ')>'
         return out
 
     # -------------------------------------------------------------------------
     def __lt__(self, other):
-
+        """Magic method for using it as the '<'-operator."""
         if not isinstance(other, VsphereObject):
-            msg = _("Object {{!r}} is not a {} object.").format('VsphereObject')
+            msg = _('Object {{!r}} is not a {} object.').format('VsphereObject')
             raise TypeError(msg.format(other))
 
         return self.qual_name < other.qual_name
 
     # -------------------------------------------------------------------------
     def __gt__(self, other):
-
+        """Magic method for using it as the '>'.operator."""
         if not isinstance(other, VsphereObject):
-            msg = _("Object {{!r}} is not a {} object.").format('VsphereObject')
+            msg = _('Object {{!r}} is not a {} object.').format('VsphereObject')
             raise TypeError(msg.format(other))
 
         return self.qual_name > other.qual_name
 
     # -------------------------------------------------------------------------
     def __eq__(self, other):
-
+        """Magic method for using it as the '=='-operator."""
         if self.verbose > 4:
-            LOG.debug(_("Comparing {} objects ...").format(self.__class__.__name__))
+            LOG.debug(_('Comparing {} objects ...').format(self.__class__.__name__))
 
         if not isinstance(other, VsphereObject):
             return False
 
         return self.qual_name == other.qual_name
 
     # -------------------------------------------------------------------------
     def __le__(self, other):
-
+        """Magic method for using it as the '<='-operator."""
         if not isinstance(other, VsphereObject):
-            msg = _("Object {{!r}} is not a {} object.").format('VsphereObject')
+            msg = _('Object {{!r}} is not a {} object.').format('VsphereObject')
             raise TypeError(msg.format(other))
 
         if self == other:
             return True
 
         return self.qual_name < other.qual_name
 
     # -------------------------------------------------------------------------
     def __ge__(self, other):
-
+        """Magic method for using it as the '>='-operator."""
         if not isinstance(other, VsphereObject):
-            msg = _("Object {{!r}} is not a {} object.").format('VsphereObject')
+            msg = _('Object {{!r}} is not a {} object.').format('VsphereObject')
             raise TypeError(msg.format(other))
 
         if self == other:
             return True
 
         return self.qual_name > other.qual_name
 
 
 # =============================================================================
 
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_vmware-0.5.7/lib/fb_vmware/vm.py` & `fb_vmware-0.6.0/lib/fb_vmware/vm.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
+@summary: The module for a VSphere virtual machine or template object.
+
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 by Frank Brehm, Berlin
-@summary: The module for a VSphere virtual machine or template object.
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
+import copy
 import logging
-import uuid
 import re
-import copy
-
+import uuid
 try:
     from collections.abc import MutableSequence
 except ImportError:
     from collections import MutableSequence
 
 # Third party modules
-from pyVmomi import vim
-
 from fb_tools.common import pp, to_bool
 from fb_tools.obj import FbBaseObject
 from fb_tools.xlate import format_list
 
-# Own modules
-from .errors import VSphereHandlerError
-
-from .obj import VsphereObject, DEFAULT_OBJ_STATUS, OBJ_STATUS_GREEN
+from pyVmomi import vim
 
+# Own modules
+from .controller import VsphereDiskController, VsphereDiskControllerList
 from .disk import VsphereDisk, VsphereDiskList
+from .errors import VSphereHandlerError
 from .ether import VsphereEthernetcard, VsphereEthernetcardList
-from .controller import VsphereDiskController, VsphereDiskControllerList
-
+from .obj import DEFAULT_OBJ_STATUS
+from .obj import OBJ_STATUS_GREEN
+from .obj import VsphereObject
 from .xlate import XLATOR
 
-__version__ = '0.6.3'
+__version__ = '0.6.4'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 
 
 # =============================================================================
 class VsphereVm(VsphereObject):
+    """This is a wrapper for a vim.VirtualMachine object."""
 
     re_vm_path_storage = re.compile(r'^\s*\[\s*([^\s\]]+)')
     re_vm_path_rel = re.compile(r'^\s*\[[^\]]*]\s*(\S.*)\s*$')
 
     # -------------------------------------------------------------------------
     def __init__(
         self, appname=None, verbose=0, version=__version__, base_dir=None, initialized=None,
             vsphere=None, name=None, status=DEFAULT_OBJ_STATUS, config_status=DEFAULT_OBJ_STATUS):
-
+        """Initialize a VsphereVm object."""
         self.repr_fields = ('name', 'vsphere')
         self._vsphere = None
         self._cluster_name = None
         self._path = None
         self._template = False
         self._memory_mb = None
         self._num_cpu = None
@@ -75,15 +75,15 @@
         self.interfaces = []
         self.controllers = []
         self.custom_data = []
 
         self.vm_tools = None
 
         super(VsphereVm, self).__init__(
-            name=name, obj_type='vsphere_vm', name_prefix="vm", status=status,
+            name=name, obj_type='vsphere_vm', name_prefix='vm', status=status,
             config_status=config_status, appname=appname, verbose=verbose,
             version=version, base_dir=base_dir)
 
         if vsphere is not None:
             self.vsphere = vsphere
 
         self.disks = VsphereDiskList(
@@ -92,27 +92,26 @@
             appname=appname, verbose=verbose, base_dir=base_dir, initialized=True)
         self.controllers = VsphereDiskControllerList(
             appname=appname, verbose=verbose, base_dir=base_dir, initialized=True)
 
     # -----------------------------------------------------------
     @property
     def vsphere(self):
-        """The name of the VSPhere from configuration, in which
-            the VM should be existing."""
+        """The name of the VSPhere from configuration, in which the VM should be existing."""
         return self._vsphere
 
     @vsphere.setter
     def vsphere(self, value):
         if value is None:
             self._vsphere = None
             return
 
         val = str(value).strip()
         if val == '':
-            msg = _("The name of the vsphere may not be empty.")
+            msg = _('The name of the vsphere may not be empty.')
             raise VSphereHandlerError(msg)
 
         self._vsphere = val
 
     # -----------------------------------------------------------
     @property
     def cluster_name(self):
@@ -163,15 +162,15 @@
             self._path = None
         else:
             self._path = v
 
     # -----------------------------------------------------------
     @property
     def template(self):
-        "Is this a VMWare template instead of a VM."
+        """Is this a VMWare template instead of a VM."""
         return self._template
 
     @template.setter
     def template(self, value):
         self._template = to_bool(value)
 
     # -----------------------------------------------------------
@@ -369,25 +368,24 @@
             self._config_version = None
         else:
             self._config_version = v
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True, bare=False):
         """
-        Transforms the elements of the object into a dict
+        Transform the elements of the object into a dict.
 
         @param short: don't include local properties in resulting dict.
         @type short: bool
         @param bare: don't include generic fields in returning dict
         @type bare: bool
 
         @return: structure as dict
         @rtype:  dict
         """
-
         if bare:
             res = {
                 'vsphere': self.vsphere,
                 'cluster_name': self.cluster_name,
                 'config_path': self.config_path,
                 'config_path_relative': self.config_path_relative,
                 'config_path_storage': self.config_path_storage,
@@ -433,15 +431,15 @@
         res['uuid'] = self.uuid
         res['instance_uuid'] = self.instance_uuid
 
         return res
 
     # -------------------------------------------------------------------------
     def __copy__(self):
-
+        """Return a new VsphereVm as a deep copy of the current object."""
         vm = VsphereVm(
             appname=self.appname, verbose=self.verbose, base_dir=self.base_dir,
             initialized=self.initialized, name=self.name, status=self.status,
             vsphere=self.vsphere, config_status=self.config_status)
 
         vm.cluster_name = self.cluster_name
         vm.config_path = self.config_path
@@ -462,17 +460,17 @@
         vm.interfaces = copy.copy(self.interfaces)
         vm.controllers = copy.copy(self.controllers)
 
         return vm
 
     # -------------------------------------------------------------------------
     def __eq__(self, other):
-
+        """Magic method for using it as the '=='-operator."""
         if self.verbose > 4:
-            LOG.debug(_("Comparing {} objects ...").format(self.__class__.__name__))
+            LOG.debug(_('Comparing {} objects ...').format(self.__class__.__name__))
 
         if not isinstance(other, VsphereVm):
             return False
 
         if self.vsphere != other.vsphere:
             return False
         if self.name != other.name:
@@ -483,20 +481,20 @@
         return True
 
     # -------------------------------------------------------------------------
     @classmethod
     def from_summary(
             cls, data, cur_path, vsphere=None, appname=None, verbose=0,
             base_dir=None, test_mode=False):
-
+        """Create a new VsphereVm object based on the data given from pyvmomi."""
         if test_mode:
             cls._check_summary_data(data)
         else:
             if not isinstance(data, vim.VirtualMachine):
-                msg = _("Parameter {t!r} must be a {e}, {v!r} ({vt}) was given.").format(
+                msg = _('Parameter {t!r} must be a {e}, {v!r} ({vt}) was given.').format(
                     t='data', e='vim.VirtualMachine', v=data, vt=data.__class__.__name__)
                 raise TypeError(msg)
 
         params = {
             'vsphere': vsphere,
             'appname': appname,
             'verbose': verbose,
@@ -504,15 +502,15 @@
             'initialized': True,
             'name': data.summary.config.name,
             'status': DEFAULT_OBJ_STATUS,
             'config_status': OBJ_STATUS_GREEN,
         }
 
         if verbose > 2:
-            LOG.debug(_("Creating {} object from:").format(cls.__name__) + '\n' + pp(params))
+            LOG.debug(_('Creating {} object from:').format(cls.__name__) + '\n' + pp(params))
 
         vm = cls(**params)
 
         vm.cluster_name = None
         if data.resourcePool:
             vm.cluster_name = data.resourcePool.owner.name
 
@@ -577,23 +575,23 @@
                         device, appname=appname, verbose=verbose, base_dir=base_dir)
                     vm.interfaces.append(iface)
                 elif isinstance(device, vim.vm.device.VirtualController):
                     ctrl = VsphereDiskController.from_summary(
                         device, appname=appname, verbose=verbose, base_dir=base_dir)
                     vm.controllers.append(ctrl)
                 elif verbose > 2:
-                    LOG.debug(_("Unknown hardware device of type {}.").format(
+                    LOG.debug(_('Unknown hardware device of type {}.').format(
                         device.__class__.__name__))
         else:
             LOG.error(_(
-                "There is something wrong wit VM {n!r} in cluster {c!r} and "
-                "path {p!r} ...").format(n=vm.name, c=vm.cluster_name, p=vm.path))
+                'There is something wrong wit VM {n!r} in cluster {c!r} and '
+                'path {p!r} ...').format(n=vm.name, c=vm.cluster_name, p=vm.path))
 
         if verbose > 2:
-            LOG.debug(_("Created {} object:").format(cls.__name__) + '\n' + pp(vm.as_dict()))
+            LOG.debug(_('Created {} object:').format(cls.__name__) + '\n' + pp(vm.as_dict()))
 
         return vm
 
     # -------------------------------------------------------------------------
     @classmethod
     def _check_summary_data(cls, data):
 
@@ -636,33 +634,31 @@
                     if not hasattr(data.config.hardware, 'device'):
                         failing_fields.append('config.hardware.device')
             else:
                 failing_fields.append('config.hardware')
 
         if len(failing_fields):
             msg = _(
-                "The given parameter {p!r} on calling method {m}() has failing "
-                "attributes").format(p='data', m='from_summary')
+                'The given parameter {p!r} on calling method {m}() has failing '
+                'attributes').format(p='data', m='from_summary')
             msg += ': ' + format_list(failing_fields, do_repr=True)
             raise AssertionError(msg)
 
 
 # =============================================================================
 class VsphereVmList(FbBaseObject, MutableSequence):
-    """
-    A list containing VsphereVm objects.
-    """
+    """A list containing VsphereVm objects."""
 
-    msg_no_vm = _("Invalid type {t!r} as an item of a {c}, only {o} objects are allowed.")
+    msg_no_vm = _('Invalid type {t!r} as an item of a {c}, only {o} objects are allowed.')
 
     # -------------------------------------------------------------------------
     def __init__(
         self, appname=None, verbose=0, version=__version__, base_dir=None,
             initialized=None, *vms):
-
+        """Initialize a VsphereVmList object."""
         self._list = []
 
         super(VsphereVmList, self).__init__(
             appname=appname, verbose=verbose, version=version, base_dir=base_dir,
             initialized=False)
 
         for vm in vms:
@@ -670,25 +666,24 @@
 
         if initialized is not None:
             self.initialized = initialized
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True, bare=False):
         """
-        Transforms the elements of the object into a dict
+        Transform the elements of the object into a dict.
 
         @param short: don't include local properties in resulting dict.
         @type short: bool
         @param bare: don't include generic fields in returning dict
         @type bare: bool
 
         @return: structure as dict or list
         @rtype:  dict or list
         """
-
         if bare:
             res = []
             for vm in self:
                 res.append(vm.as_dict(bare=True))
             return res
 
         res = super(VsphereVmList, self).as_dict(short=short)
@@ -697,34 +692,34 @@
         for vm in self:
             res['_list'].append(vm.as_dict(short=short))
 
         return res
 
     # -------------------------------------------------------------------------
     def __copy__(self):
-
+        """Return a new VsphereVmList as a deep copy of the current object."""
         new_list = self.__class__(
             appname=self.appname, verbose=self.verbose,
             base_dir=self.base_dir, initialized=False)
 
         for vm in self:
             new_list.append(copy.copy(vm))
 
         new_list.initialized = self.initialized
         return new_list
 
     # -------------------------------------------------------------------------
     def index(self, vm, *args):
-
+        """Return the numeric index of the given VM in current list."""
         i = None
         j = None
 
         if len(args) > 0:
             if len(args) > 2:
-                raise TypeError(_("{m} takes at most {max} arguments ({n} given).").format(
+                raise TypeError(_('{m} takes at most {max} arguments ({n} given).').format(
                     m='index()', max=3, n=len(args) + 1))
             i = int(args[0])
             if len(args) > 1:
                 j = int(args[1])
 
         index = 0
         start = 0
@@ -755,20 +750,20 @@
             for index in list(range(len(self._list))):
                 item = self._list[index]
                 if index >= end:
                     break
             if item == vm:
                 return index
 
-        msg = _("VM is not in VM list.")
+        msg = _('VM is not in VM list.')
         raise ValueError(msg)
 
     # -------------------------------------------------------------------------
     def __contains__(self, vm):
-
+        """Return whether the given VM is contained in current list."""
         if not isinstance(vm, VsphereVm):
             raise TypeError(self.msg_no_vm.format(
                 t=vm.__class__.__name__, c=self.__class__.__name__, o='VsphereVm'))
 
         if not self._list:
             return False
 
@@ -776,15 +771,15 @@
             if item == vm:
                 return True
 
         return False
 
     # -------------------------------------------------------------------------
     def count(self, vm):
-
+        """Return the number of VMs which are equal to the given one in current list."""
         if not isinstance(vm, VsphereVm):
             raise TypeError(self.msg_no_vm.format(
                 t=vm.__class__.__name__, c=self.__class__.__name__, o='VsphereVm'))
 
         if not self._list:
             return 0
 
@@ -792,79 +787,80 @@
         for item in self._list:
             if item == vm:
                 num += 1
         return num
 
     # -------------------------------------------------------------------------
     def __len__(self):
+        """Return the number of VMs in current list."""
         return len(self._list)
 
     # -------------------------------------------------------------------------
     def __iter__(self):
-
+        """Iterate through all VMs in current list."""
         for item in self._list:
             yield item
 
     # -------------------------------------------------------------------------
     def __getitem__(self, key):
+        """Get a VM from current list by the given numeric index."""
         return self._list.__getitem__(key)
 
     # -------------------------------------------------------------------------
     def __reversed__(self):
-
+        """Reverse the VMs in list in place."""
         new_list = self.__class__(
             appname=self.appname, verbose=self.verbose,
             base_dir=self.base_dir, initialized=False)
 
         for vm in reversed(self._list):
             new_list.append(copy.copy(vm))
 
         new_list.initialized = self.initialized
         return new_list
 
     # -------------------------------------------------------------------------
     def __setitem__(self, key, vm):
-
+        """Replace the VM at the given numeric index by the given one."""
         if not isinstance(vm, VsphereVm):
             raise TypeError(self.msg_no_vm.format(
                 t=vm.__class__.__name__, c=self.__class__.__name__, o='VsphereVm'))
 
         self._list.__setitem__(key, vm)
 
     # -------------------------------------------------------------------------
     def __delitem__(self, key):
-
+        """Remove the VM at the given numeric index from list."""
         del self._list[key]
 
     # -------------------------------------------------------------------------
     def append(self, vm):
-
+        """Append the given VM to the current list."""
         if not isinstance(vm, VsphereVm):
             raise TypeError(self.msg_no_vm.format(
                 t=vm.__class__.__name__, c=self.__class__.__name__, o='VsphereVm'))
 
         self._list.append(vm)
 
     # -------------------------------------------------------------------------
     def insert(self, index, vm):
-
+        """Insert the given VM in current list at given index."""
         if not isinstance(vm, VsphereVm):
             raise TypeError(self.msg_no_vm.format(
                 t=vm.__class__.__name__, c=self.__class__.__name__, o='VsphereVm'))
 
         self._list.insert(index, vm)
 
     # -------------------------------------------------------------------------
     def clear(self):
-        "Remove all items from the VsphereEthernetcardList."
-
+        """Remove all items from the VsphereEthernetcardList."""
         self._list = []
 
 
 # =============================================================================
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_vmware-0.5.7/lib/fb_vmware/xlate.py` & `fb_vmware-0.6.0/lib/fb_vmware/xlate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
-@author: Frank Brehm
-@contact: frank@brehm-online.com
-@copyright: © 2022 by Frank Brehm, Berlin
 @summary: The module for i18n.
-          It provides translation object, usable from all other
+
+          It provides a translation object, usable from all other
           modules in this package.
+
+@author: Frank Brehm
+@contact: frank@brehm-online.com
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import, print_function
 
 # Standard modules
-import logging
-import gettext
 import copy
-
+import gettext
+import logging
 try:
     from pathlib import Path
 except ImportError:
     from pathlib2 import Path
 
 # Third party modules
 import babel
@@ -30,15 +31,15 @@
 except ImportError:
     from distutils.version import LooseVersion as Version
 
 DOMAIN = 'fb_vmware'
 
 LOG = logging.getLogger(__name__)
 
-__version__ = '0.1.2'
+__version__ = '0.1.4'
 
 __me__ = Path(__file__).resolve()
 __module_dir__ = __me__.parent
 __lib_dir__ = __module_dir__.parent
 __base_dir__ = __lib_dir__.parent
 LOCALE_DIR = __base_dir__.joinpath('locale')
 if not LOCALE_DIR.is_dir():
@@ -72,14 +73,15 @@
 _ = XLATOR.gettext
 
 
 # =============================================================================
 def format_list(lst, do_repr=False, style='standard', locale=DEFAULT_LOCALE):
     """
     Format the items in `lst` as a list.
+
     :param lst: a sequence of items to format in to a list
     :param locale: the locale
     """
     if not lst:
         return ''
 
     my_list = copy.copy(lst)
@@ -91,29 +93,29 @@
     if CUR_BABEL_VERSION < NEWER_BABEL_VERSION:
         return babel.lists.format_list(my_list, locale=locale)
     return babel.lists.format_list(my_list, style=style, locale=locale)
 
 
 # =============================================================================
 
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     out_list = []
-    out_list.append([_("Module directory:"), str(__module_dir__)])
-    out_list.append([_("Base directory:"), str(__base_dir__)])
-    out_list.append([_("Locale directory:"), str(LOCALE_DIR)])
-    out_list.append([_("Locale domain:"), DOMAIN])
-    out_list.append([_("Found .mo-file:"), __mo_file__])
+    out_list.append([_('Module directory:'), str(__module_dir__)])
+    out_list.append([_('Base directory:'), str(__base_dir__)])
+    out_list.append([_('Locale directory:'), str(LOCALE_DIR)])
+    out_list.append([_('Locale domain:'), DOMAIN])
+    out_list.append([_('Found .mo-file:'), __mo_file__])
 
     max_len = 1
     for pair in out_list:
         if len(pair[0]) > max_len:
             max_len = len(pair[0])
 
-    template = "{{label:<{}}} {{val!r}}".format(max_len)
+    template = '{{label:<{}}} {{val!r}}'.format(max_len)
     for pair in out_list:
         print(template.format(label=pair[0], val=pair[1]))
 
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4
```

### Comparing `fb_vmware-0.5.7/lib/fb_vmware.egg-info/PKG-INFO` & `fb_vmware-0.6.0/lib/fb_vmware.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fb-vmware
-Version: 0.5.7
+Version: 0.6.0
 Summary: A wrapper module around the pyvmomi module to simplify work and handling.
 Home-page: https://github.com/fbrehm/fb-vmware
 Author: Frank Brehm
 Author-email: frank@brehm-online.com
 License: LGPL3+
 Platform: posix
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `fb_vmware-0.5.7/lib/fb_vmware.egg-info/SOURCES.txt` & `fb_vmware-0.6.0/lib/fb_vmware.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fb_vmware-0.5.7/setup.cfg` & `fb_vmware-0.6.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -52,13 +52,13 @@
 
 [pep8]
 max-line-length = 99
 
 [flake8]
 max-line-length = 99
 max-complexity = 20
-ignore = E226,E302,E41,E402
+ignore = E226,E302,E41,E402,B902
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `fb_vmware-0.5.7/setup.py` & `fb_vmware-0.6.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 """
+@summary: A wrapper module around the pyvmomi module to simplify work and handling.
+
 @author: Frank Brehm
 @contact: frank@brehm-online.com
 @license: LGPL3+
 @copyright: © 2022 Frank Brehm, Berlin
-@summary: A wrapper module around the pyvmomi module to simplify work and handling.
 """
 from __future__ import print_function
 
-import os
-import sys
-import re
-import pprint
 import datetime
-import textwrap
 import glob
+import os
 import pathlib
+import pprint
+import re
 import subprocess
-
-# Third party modules
-from setuptools import setup
+import sys
+import textwrap
 
 # own modules:
 __base_dir__ = os.path.abspath(os.path.dirname(__file__))
 __bin_dir__ = os.path.join(__base_dir__, 'bin')
 __lib_dir__ = os.path.join(__base_dir__, 'lib')
 __module_dir__ = os.path.join(__lib_dir__, 'fb_vmware')
 __init_py__ = os.path.join(__module_dir__, '__init__.py')
@@ -36,28 +34,32 @@
     '__lib_dir__': __lib_dir__,
     '__module_dir__': __module_dir__,
     '__init_py__': __init_py__,
 }
 
 # -----------------------------------
 def pp(obj):
+    """Human friendly output of data structures."""
     pprinter = pprint.PrettyPrinter(indent=4)
     return pprinter.pformat(obj)
 
 # print("Paths:\n{}".format(pp(PATHS)))
 
 
 if os.path.exists(__module_dir__) and os.path.isfile(__init_py__):
     sys.path.insert(0, os.path.abspath(__lib_dir__))
 
+# Third party modules
 import fb_vmware
 
+from setuptools import setup
+
 # from fb_tools.common import pp
 
-ENCODING = "utf-8"
+ENCODING = 'utf-8'
 
 __packet_version__ = fb_vmware.__version__
 
 __packet_name__ = 'fb_vmware'
 __debian_pkg_name__ = 'fb-vmware'
 
 __author__ = 'Frank Brehm'
@@ -69,43 +71,45 @@
 
 __open_args__ = {}
 if sys.version_info[0] < 3:
     __open_args__ = {'encoding': ENCODING, 'errors': 'surrogateescape'}
 
 # -----------------------------------
 def read(fname):
-
+    """Read the given file and return its content."""
     content = None
 
     if sys.version_info[0] < 3:
         with open(fname, 'r') as fh:
             content = fh.read()
     else:
         with open(fname, 'r', **__open_args__) as fh:
             content = fh.read()
 
     return content
 
 
 # -----------------------------------
 def is_python_file(filename):
+    """Return, whether the given file seems to be a Python source file."""
     if filename.endswith('.py'):
         return True
     else:
         return False
 
 
 # -----------------------------------
 __debian_dir__ = os.path.join(__base_dir__, 'debian')
 __changelog_file__ = os.path.join(__debian_dir__, 'changelog')
 __readme_file__ = os.path.join(__base_dir__, 'README.md')
 
 
 # -----------------------------------
 def get_debian_version():
+    """Return the latest package version fron Debian changelog file."""
     if not os.path.isfile(__changelog_file__):
         return None
     changelog = read(__changelog_file__)
     first_row = changelog.splitlines()[0].strip()
     if not first_row:
         return None
     pattern = r'^' + re.escape(__debian_pkg_name__) + r'\s+\(([^\)]+)\)'
@@ -118,24 +122,25 @@
 __debian_version__ = get_debian_version()
 
 if __debian_version__ is not None and __debian_version__ != '':
     __packet_version__ = __debian_version__
 
 # -----------------------------------
 def write_local_version():
-
+    """Write the local version file."""
     local_version_file = os.path.join(__module_dir__, 'local_version.py')
     local_version_file_content = textwrap.dedent('''\
         #!/usr/bin/python
         # -*- coding: utf-8 -*-
         """
+        @summary: A wrapper module around the pyvmomi module to simplify work and handling.
+
         @author: {author}
         @contact: {contact}
         @copyright: © {cur_year} by {author}, Berlin
-        @summary: Modules for common used objects, error classes and methods.
         """
 
         __author__ = '{author} <{contact}>'
         __copyright__ = '(C) {cur_year} by {author}, Berlin'
         __contact__ = {contact!r}
         __version__ = {version!r}
         __license__ = {license!r}
@@ -165,15 +170,15 @@
     'fb_tools',
     'argparse',
     'six'
 ]
 
 # -----------------------------------
 def read_requirements():
-
+    """Read the requiremments.txt file."""
     req_file = os.path.join(__base_dir__, 'requirements.txt')
     if not os.path.isfile(req_file):
         return
 
     f_content = read(req_file)
     if not f_content:
         return
@@ -198,15 +203,15 @@
 
 read_requirements()
 
 # -----------------------------------
 __scripts__ = []
 
 def get_scripts():
-
+    """Collect binary script files from bin/."""
     fpattern = os.path.join(__bin_dir__, '*')
     for fname in glob.glob(fpattern):
         script_name = os.path.relpath(fname, __base_dir__)
         if not os.path.isfile(fname):
             continue
         if not os.access(fname, os.X_OK):
             continue
@@ -220,14 +225,15 @@
 get_scripts()
 
 # -----------------------------------
 MO_FILES = 'locale/*/LC_MESSAGES/*.mo'
 PO_FILES = 'locale/*/LC_MESSAGES/*.po'
 
 def create_mo_files():
+    """Compile the translation files."""
     mo_files = []
     for po_path in glob.glob(PO_FILES):
         mo = pathlib.Path(po_path.replace('.po', '.mo'))
         if not mo.exists():
             subprocess.call(['msgfmt', '-o', str(mo), po_path])
         mo_files.append(str(mo))
```

### Comparing `fb_vmware-0.5.7/test/general.py` & `fb_vmware-0.6.0/test/general.py`

 * *Files identical despite different names*

### Comparing `fb_vmware-0.5.7/test/test_00-errors.py` & `fb_vmware-0.6.0/test/test_00-errors.py`

 * *Files identical despite different names*

### Comparing `fb_vmware-0.5.7/test/test_10-base.py` & `fb_vmware-0.6.0/test/test_10-base.py`

 * *Files identical despite different names*

### Comparing `fb_vmware-0.5.7/test/test_20-obj.py` & `fb_vmware-0.6.0/test/test_20-obj.py`

 * *Files identical despite different names*

### Comparing `fb_vmware-0.5.7/test/test_31_about_info.py` & `fb_vmware-0.6.0/test/test_31_about_info.py`

 * *Files identical despite different names*

### Comparing `fb_vmware-0.5.7/test/test_32_cluster.py` & `fb_vmware-0.6.0/test/test_32_cluster.py`

 * *Files identical despite different names*

### Comparing `fb_vmware-0.5.7/test/test_33_dc.py` & `fb_vmware-0.6.0/test/test_33_dc.py`

 * *Files identical despite different names*

### Comparing `fb_vmware-0.5.7/test/test_34_disk.py` & `fb_vmware-0.6.0/test/test_34_disk.py`

 * *Files identical despite different names*

### Comparing `fb_vmware-0.5.7/test/test_35_datastore.py` & `fb_vmware-0.6.0/test/test_35_datastore.py`

 * *Files identical despite different names*

### Comparing `fb_vmware-0.5.7/test/test_36_ds_cluster.py` & `fb_vmware-0.6.0/test/test_36_ds_cluster.py`

 * *Files identical despite different names*

### Comparing `fb_vmware-0.5.7/test/test_37_ether.py` & `fb_vmware-0.6.0/test/test_37_ether.py`

 * *Files identical despite different names*

### Comparing `fb_vmware-0.5.7/test/test_38_iface.py` & `fb_vmware-0.6.0/test/test_38_iface.py`

 * *Files identical despite different names*

### Comparing `fb_vmware-0.5.7/test/test_39_network.py` & `fb_vmware-0.6.0/test/test_39_network.py`

 * *Files identical despite different names*

### Comparing `fb_vmware-0.5.7/test/test_40_controller.py` & `fb_vmware-0.6.0/test/test_40_controller.py`

 * *Files identical despite different names*

### Comparing `fb_vmware-0.5.7/test/test_41_host_port_group.py` & `fb_vmware-0.6.0/test/test_41_host_port_group.py`

 * *Files identical despite different names*

### Comparing `fb_vmware-0.5.7/test/test_50_host.py` & `fb_vmware-0.6.0/test/test_50_host.py`

 * *Files identical despite different names*

### Comparing `fb_vmware-0.5.7/test/test_55_vm.py` & `fb_vmware-0.6.0/test/test_55_vm.py`

 * *Files identical despite different names*

### Comparing `fb_vmware-0.5.7/test/test_60_config.py` & `fb_vmware-0.6.0/test/test_60_config.py`

 * *Files identical despite different names*

### Comparing `fb_vmware-0.5.7/test/test_70_connect.py` & `fb_vmware-0.6.0/test/test_70_connect.py`

 * *Files identical despite different names*

