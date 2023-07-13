# Comparing `tmp/fabrictestbed-mflib-1.0.0.tar.gz` & `tmp/fabrictestbed-mflib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrictestbed-mflib-1.0.0.tar", last modified: Sun Apr 23 02:50:25 2023, max compression
+gzip compressed data, was "fabrictestbed-mflib-1.0.1.tar", last modified: Thu Jul 13 16:54:42 2023, max compression
```

## Comparing `fabrictestbed-mflib-1.0.0.tar` & `fabrictestbed-mflib-1.0.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      647 2023-02-01 16:43:59.704079 fabrictestbed-mflib-1.0.0/.gitignore
--rw-r--r--   0        0        0      575 2023-03-29 18:17:09.721091 fabrictestbed-mflib-1.0.0/.readthedocs.yaml
--rw-r--r--   0        0        0     1071 2023-02-01 16:43:59.704079 fabrictestbed-mflib-1.0.0/LICENSE
--rw-r--r--   0        0        0       24 2023-02-01 16:43:59.704079 fabrictestbed-mflib-1.0.0/MANIFEST.in
--rw-r--r--   0        0        0   667845 2023-04-23 02:15:54.442310 fabrictestbed-mflib-1.0.0/MFLib.pdf
--rw-r--r--   0        0        0     3974 2023-04-22 05:12:44.140491 fabrictestbed-mflib-1.0.0/README.md
--rwxr-xr-x   0        0        0      817 2023-04-17 18:32:21.683648 fabrictestbed-mflib-1.0.0/create_html_doc.sh
--rwxr-xr-x   0        0        0      687 2023-04-13 17:46:39.734392 fabrictestbed-mflib-1.0.0/create_pdf_doc.sh
--rwxr-xr-x   0        0        0      668 2023-04-13 17:46:39.734392 fabrictestbed-mflib-1.0.0/create_release.sh
--rw-r--r--   0        0        0      638 2023-02-01 16:43:59.708079 fabrictestbed-mflib-1.0.0/docs/Makefile
--rw-r--r--   0        0        0      804 2023-02-01 16:43:59.708079 fabrictestbed-mflib-1.0.0/docs/make.bat
--rw-r--r--   0        0        0       74 2023-04-23 02:13:59.649527 fabrictestbed-mflib-1.0.0/docs/requirements.txt
-lrwxr-xr-x   0        0        0        0 2023-02-01 16:43:59.708079 fabrictestbed-mflib-1.0.0/docs/source/README.md -> ../../README.md
--rw-r--r--   0        0        0       41 2023-02-01 16:43:59.708079 fabrictestbed-mflib-1.0.0/docs/source/_static/placeholder
--rw-r--r--   0        0        0       41 2023-02-01 16:43:59.708079 fabrictestbed-mflib-1.0.0/docs/source/_templates/placeholder
--rw-r--r--   0        0        0     1297 2023-04-23 02:12:57.745116 fabrictestbed-mflib-1.0.0/docs/source/conf.py
--rw-r--r--   0        0        0      204 2023-02-01 16:43:59.708079 fabrictestbed-mflib-1.0.0/docs/source/core.rst
--rw-r--r--   0        0        0    42620 2023-04-22 05:12:44.140491 fabrictestbed-mflib-1.0.0/docs/source/images/3nodes.png
--rw-r--r--   0        0        0    71388 2023-04-22 05:12:44.144491 fabrictestbed-mflib-1.0.0/docs/source/images/3nodes_add_meas.png
--rw-r--r--   0        0        0   100374 2023-04-22 05:12:44.144491 fabrictestbed-mflib-1.0.0/docs/source/images/3nodes_ini.png
--rw-r--r--   0        0        0    70104 2023-04-22 05:12:44.144491 fabrictestbed-mflib-1.0.0/docs/source/images/3nodes_inst.png
--rw-r--r--   0        0        0   204495 2023-04-22 05:12:44.144491 fabrictestbed-mflib-1.0.0/docs/source/images/keys.png
--rw-r--r--   0        0        0      310 2023-04-22 05:12:44.144491 fabrictestbed-mflib-1.0.0/docs/source/index.rst
--rw-r--r--   0        0        0       94 2023-04-22 05:12:44.144491 fabrictestbed-mflib-1.0.0/docs/source/mf_timestamp.rst
--rw-r--r--   0        0        0      215 2023-04-13 17:46:39.734392 fabrictestbed-mflib-1.0.0/docs/source/mflib.rst
--rw-r--r--   0        0        0     6230 2023-04-22 05:12:44.144491 fabrictestbed-mflib-1.0.0/docs/source/overview.md
--rw-r--r--   0        0        0       58 2023-04-22 05:12:44.144491 fabrictestbed-mflib-1.0.0/docs/source/owl.rst
--rw-r--r--   0        0        0       81 2023-04-22 05:12:44.144491 fabrictestbed-mflib-1.0.0/docs/source/owl_data.rst
--rw-r--r--   0        0        0     7308 2023-02-01 16:43:59.708079 fabrictestbed-mflib-1.0.0/mflib/README.md
--rw-r--r--   0        0        0      539 2023-04-23 02:15:39.926210 fabrictestbed-mflib-1.0.0/mflib/__init__.py
--rw-r--r--   0        0        0    47374 2023-04-22 17:59:18.127064 fabrictestbed-mflib-1.0.0/mflib/core.py
--rw-r--r--   0        0        0    17118 2023-04-22 05:12:44.144491 fabrictestbed-mflib-1.0.0/mflib/mf_timestamp.py
--rw-r--r--   0        0        0    32687 2023-04-22 17:59:18.127064 fabrictestbed-mflib-1.0.0/mflib/mflib.py
--rw-r--r--   0        0        0    27981 2023-04-22 17:59:18.127064 fabrictestbed-mflib-1.0.0/mflib/mfvis.py
--rw-r--r--   0        0        0    15650 2023-04-22 05:12:44.144491 fabrictestbed-mflib-1.0.0/mflib/owl.py
--rw-r--r--   0        0        0    11857 2023-04-22 17:59:18.127064 fabrictestbed-mflib-1.0.0/mflib/owl_data.py
--rw-r--r--   0        0        0      735 2023-04-22 05:12:44.144491 fabrictestbed-mflib-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       32 2023-04-23 02:13:38.561386 fabrictestbed-mflib-1.0.0/requirements.txt
--rw-r--r--   0        0        0     4482 1970-01-01 00:00:00.000000 fabrictestbed-mflib-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      647 2023-02-01 16:43:59.704079 fabrictestbed-mflib-1.0.1/.gitignore
+-rw-r--r--   0        0        0      575 2023-03-29 18:17:09.721091 fabrictestbed-mflib-1.0.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     1071 2023-02-01 16:43:59.704079 fabrictestbed-mflib-1.0.1/LICENSE
+-rw-r--r--   0        0        0       24 2023-02-01 16:43:59.704079 fabrictestbed-mflib-1.0.1/MANIFEST.in
+-rw-r--r--   0        0        0   675079 2023-07-13 16:18:35.327701 fabrictestbed-mflib-1.0.1/MFLib.pdf
+-rw-r--r--   0        0        0     3974 2023-04-22 05:12:44.140491 fabrictestbed-mflib-1.0.1/README.md
+-rwxr-xr-x   0        0        0      817 2023-04-17 18:32:21.683648 fabrictestbed-mflib-1.0.1/create_html_doc.sh
+-rwxr-xr-x   0        0        0      687 2023-04-13 17:46:39.734392 fabrictestbed-mflib-1.0.1/create_pdf_doc.sh
+-rwxr-xr-x   0        0        0      668 2023-04-13 17:46:39.734392 fabrictestbed-mflib-1.0.1/create_release.sh
+-rw-r--r--   0        0        0      638 2023-02-01 16:43:59.708079 fabrictestbed-mflib-1.0.1/docs/Makefile
+-rw-r--r--   0        0        0      804 2023-02-01 16:43:59.708079 fabrictestbed-mflib-1.0.1/docs/make.bat
+-rw-r--r--   0        0        0      159 2023-07-10 14:20:37.321779 fabrictestbed-mflib-1.0.1/docs/requirements.txt
+lrwxr-xr-x   0        0        0        0 2023-02-01 16:43:59.708079 fabrictestbed-mflib-1.0.1/docs/source/README.md -> ../../README.md
+-rw-r--r--   0        0        0       41 2023-02-01 16:43:59.708079 fabrictestbed-mflib-1.0.1/docs/source/_static/placeholder
+-rw-r--r--   0        0        0       41 2023-02-01 16:43:59.708079 fabrictestbed-mflib-1.0.1/docs/source/_templates/placeholder
+-rw-r--r--   0        0        0     1297 2023-04-23 02:12:57.745116 fabrictestbed-mflib-1.0.1/docs/source/conf.py
+-rw-r--r--   0        0        0      204 2023-02-01 16:43:59.708079 fabrictestbed-mflib-1.0.1/docs/source/core.rst
+-rw-r--r--   0        0        0    42620 2023-04-22 05:12:44.140491 fabrictestbed-mflib-1.0.1/docs/source/images/3nodes.png
+-rw-r--r--   0        0        0    71388 2023-04-22 05:12:44.144491 fabrictestbed-mflib-1.0.1/docs/source/images/3nodes_add_meas.png
+-rw-r--r--   0        0        0   100374 2023-04-22 05:12:44.144491 fabrictestbed-mflib-1.0.1/docs/source/images/3nodes_ini.png
+-rw-r--r--   0        0        0    70104 2023-04-22 05:12:44.144491 fabrictestbed-mflib-1.0.1/docs/source/images/3nodes_inst.png
+-rw-r--r--   0        0        0   204495 2023-04-22 05:12:44.144491 fabrictestbed-mflib-1.0.1/docs/source/images/keys.png
+-rw-r--r--   0        0        0      310 2023-04-25 19:08:01.544111 fabrictestbed-mflib-1.0.1/docs/source/index.rst
+-rw-r--r--   0        0        0      147 2023-07-10 14:20:37.321779 fabrictestbed-mflib-1.0.1/docs/source/mf_timestamp.rst
+-rw-r--r--   0        0        0      215 2023-04-13 17:46:39.734392 fabrictestbed-mflib-1.0.1/docs/source/mflib.rst
+-rw-r--r--   0        0        0     6230 2023-04-22 05:12:44.144491 fabrictestbed-mflib-1.0.1/docs/source/overview.md
+-rw-r--r--   0        0        0       58 2023-04-22 05:12:44.144491 fabrictestbed-mflib-1.0.1/docs/source/owl.rst
+-rw-r--r--   0        0        0       65 2023-07-10 14:20:37.321779 fabrictestbed-mflib-1.0.1/docs/source/owl_data.rst
+-rw-r--r--   0        0        0     7308 2023-02-01 16:43:59.708079 fabrictestbed-mflib-1.0.1/mflib/README.md
+-rw-r--r--   0        0        0      539 2023-07-13 16:18:05.603483 fabrictestbed-mflib-1.0.1/mflib/__init__.py
+-rw-r--r--   0        0        0    47373 2023-07-12 21:57:11.810083 fabrictestbed-mflib-1.0.1/mflib/core.py
+-rw-r--r--   0        0        0    17168 2023-07-10 14:20:37.321779 fabrictestbed-mflib-1.0.1/mflib/mf_timestamp.py
+-rw-r--r--   0        0        0    32686 2023-07-12 21:59:47.616104 fabrictestbed-mflib-1.0.1/mflib/mflib.py
+-rw-r--r--   0        0        0    27981 2023-04-22 17:59:18.127064 fabrictestbed-mflib-1.0.1/mflib/mfvis.py
+-rw-r--r--   0        0        0    15650 2023-04-22 05:12:44.144491 fabrictestbed-mflib-1.0.1/mflib/owl.py
+-rw-r--r--   0        0        0    11857 2023-04-22 17:59:18.127064 fabrictestbed-mflib-1.0.1/mflib/owl_data.py
+-rw-r--r--   0        0        0      735 2023-04-22 05:12:44.144491 fabrictestbed-mflib-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       32 2023-04-23 02:13:38.561386 fabrictestbed-mflib-1.0.1/requirements.txt
+-rw-r--r--   0        0        0     4482 1970-01-01 00:00:00.000000 fabrictestbed-mflib-1.0.1/PKG-INFO
```

### Comparing `fabrictestbed-mflib-1.0.0/.gitignore` & `fabrictestbed-mflib-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-1.0.0/.readthedocs.yaml` & `fabrictestbed-mflib-1.0.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-1.0.0/LICENSE` & `fabrictestbed-mflib-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-1.0.0/MFLib.pdf` & `fabrictestbed-mflib-1.0.1/MFLib.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 11% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,13 +1,13 @@
 MFLib
-Release 1.0.0
+Release 1.0.1
 
 Fabric UKY Team
 
-Apr 22, 2023
+Jul 13, 2023
 
 CONTENTS
 
 1
 
 Documentation Resources
 1.1 Example Jupyter Notebooks . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
@@ -57,43 +57,43 @@
 
 MFLib Core
 
 12
 
 7
 
-MF mf_timestamp
+MFLib mf_timestamp
 
 17
 
 8
 
 OWL
 
-18
+19
 
 9
 
 OWL Data
 
-21
+22
 
 Python Module Index
 
-22
+23
 
 Index
 
-23
+24
 
 i
 
-MFLib, Release 1.0.0
+MFLib, Release 1.0.1
 
-docs failing
+docs passing
 
 Welcome to the FABRIC Measurement Framework Library. MFLib makes it easy to install monitoring systems to a
 FABRIC experimenter’s slice. The monitoring system makes extensive use of industry standards such as Prometheus,
 Grafana, Elastic Search and Kibana while adding customized monitoring tools and dashboards for quick setup and
 visualization.
 
 CONTENTS
@@ -167,15 +167,15 @@
 
 Run the bash script to create the MFLIB.pdf documentation. MFLIB.pdf will be placed in the root directory of the
 repository.
 ./create_pdf_doc.sh
 
 4
 
-MFLib, Release 1.0.0
+MFLib, Release 1.0.1
 
 3.2 Distribution Package
 MFLib package is created using Flit Be sure to create and commit the PDF documentation to GitHub before building
 and publishing to PyPi. The MFLib.pdf is included in the distributition.
 To build python package for PyPi run
 ./create_release.sh
 
@@ -216,15 +216,15 @@
 MFLib().addMeasNode(slice) where slice is a fabric slice that has been specified but not yet submitted. This example
 has 3 ndoes and an experimental network.
 
 The MFLib().addMeasNode(slice) adds an extra node called the Measurement Node (meas_node) and an measure-
 
 6
 
-MFLib, Release 1.0.0
+MFLib, Release 1.0.1
 
 ment network.
 
 4.1.2 Init & Instrumentize
 MFlib works on an existing slice to which MFLib must first add some software and services.
 MFLib(slice_name) mf = MFLib(slice_name, local_storage_directory="/tmp/mflib") First you must
 create the MFLib object by passing the slice name to MFLib() . You can optionally pass a string for where you would
@@ -248,15 +248,15 @@
 – Prometheus & Grafana
 – ELK with Kibana
 
 4.1. MFLib Methods
 
 7
 
-MFLib, Release 1.0.0
+MFLib, Release 1.0.1
 
 4.1.3 Service Methods
 Measurement Framework has “services” which are installed on the measurement node. The MFLib.instrumentize()
 method installs Prometheus, Grafana, and ELK.. MFLib is built on top of MFLib.Core(). MFLib uses Core methods to
 interact with services using several basic methods: create, info, update, start, stop and remove. Each of these methods
 require the service name. Most can also take an optional dictionary and an optional list of files to be uploaded. All will
 return a json object with at least a “success” and “msg” values.
@@ -285,15 +285,15 @@
 mflib.download_common_hosts mf.download_common_hosts() retrieves an ansible hosts.ini file for the slice. The
 hosts file will contain 2 groups: Experiment_nodes and Measurement_node
 
 4.1. MFLib Methods
 
 8
 
-MFLib, Release 1.0.0
+MFLib, Release 1.0.1
 
 mflib.download_log_file mf.download_log_file(service, method) retrieves the log files for runs of the given
 service’s method: create, info, update. . . etc. This can be useful for debugging.
 
 4.1.4 Accessing Experiment Nodes via Bastion Host
 Many of the services set up by MFLib run web accessible user interfaces on the Measurement Node. Since experimental
 resources are secured by the FABRIC Bastion host, a tunnel must be created to access the web pages.
@@ -311,15 +311,15 @@
 MFLIB
 
 MFLib is the main class that is used to interact with the Measurement Framework set up in a user’s FABRIC Experiment.
 class mflib.mflib.MFLib(slice_name='', local_storage_directory='/tmp/mflib', mf_repo_branch='main',
 optimize_repos=False)
 Bases: Core
 MFLib allows for adding and controlling the MeasurementFramework in a Fabric experiementers slice.
-static addMeasNode(slice, cores=4, ram=16, disk=500, network_type='FABNetv4', site='NCSA',
+static addMeasNode(slice, cores=4, ram=16, disk=500, network_type='FABNetv4', site='EDC',
 image='default_ubuntu_20')
 Adds Measurement node and measurement network to an unsubmitted slice object.
 Parameters
 • slice (fablib.slice) – Slice object already set with experiment topology.
 • cores (int, optional) – Cores for measurement node. Defaults to 4 cores.
 • ram (int, optional) – _description_. Defaults to 16 GB ram.
 • disk (int, optional) – _description_. Defaults to 500 GB disk.
@@ -339,15 +339,15 @@
 Parameters
 slice_name (str) – The name of the slice to be monitored.
 Returns
 False if no Measure Node found or a init process fails. True otherwise.
 
 10
 
-MFLib, Release 1.0.0
+MFLib, Release 1.0.1
 
 Return type
 Bool
 instrumentize(services=['prometheus', 'elk'])
 Instrumentize the slice. This is a convenience method that sets up & starts the monitoring of the slice. Sets
 up Prometheus, ELK & Grafana.
 Parameters
@@ -420,15 +420,15 @@
 Parameters
 • service (String) – The name of the service.
 • data (JSON serializable object) –
 • files (List of Strings) – List of filepaths to be uploaded.
 
 12
 
-MFLib, Release 1.0.0
+MFLib, Release 1.0.1
 
 Returns
 Dictionary of creation results.
 Return type
 dict
 download_log_file(service, method)
 Download the log file for the given service and method. Downloaded file will be stored locally for future
@@ -468,15 +468,15 @@
 Return type
 String
 property grafana_tunnel_local_port
 If a tunnel is used for grafana, this value must be set for the port. :returns: port number :rtype: String
 
 13
 
-MFLib, Release 1.0.0
+MFLib, Release 1.0.1
 
 info(service, data=None)
 Gets inormation from an existing service. Strictly gets information, does not change how the service is
 running.
 Parameters
 • service (String) – The name of the service.
 • data (JSON Serializable Object) – Data to be passed to a JSON file place in the
@@ -514,15 +514,15 @@
 property log_directory
 The full path for the log directory.
 Returns
 The full path to the log directory.
 
 14
 
-MFLib, Release 1.0.0
+MFLib, Release 1.0.1
 
 Return type
 String
 property meas_node
 The fablib node object for the Measurement Node in the slice.
 Returns
 The fablib node object for the Measurement Node in the slice.
@@ -561,15 +561,15 @@
 start(services=[])
 Restarts a stopped service using existing configs on meas node.
 Parameters
 services (List of Strings) – The name of the services to be restarted.
 
 15
 
-MFLib, Release 1.0.0
+MFLib, Release 1.0.1
 
 Returns
 List of start result dictionaries.
 Return type
 List
 stop(services=[])
 Stops a service, does not remove the service, just stops it from using resources.
@@ -608,18 +608,94 @@
 
 16
 
 CHAPTER
 
 SEVEN
 
-MF MF_TIMESTAMP
+MFLIB MF_TIMESTAMP
+
+MFLib’s Timestamp functions are defined in this class.
+class mflib.mf_timestamp.mf_timestamp(slice_name, container_name)
+Creates precision timestamps.
+deploy_influxdb_dashboard(dashboard_file, influxdb_node_name, bind_mount_volume)
+Uploads a dashboard template file from Jupyterhub to influxdb and apply the template :param dashboard_file: path of the dashboard file on Jupyterhub :type dashboard_file: str :param influxdb_node_name:
+which fabric node is influxdb running on :type influxdb_node_name: str :param bind_mount_volume: bind
+mount volume of the influxdb docker container :type bind_mount_volume: str
+download_file_from_influxdb(data_node, data_type, influxdb_node_name, local_file)
+Downlaods the .csv data file from the influxdb container to juputerhub :param data_node: where the data
+comes from :type data_node: str :param data_type: packet_timestamp or event timestamp :type data_type:
+str :param influxdb_node_name: which fabric node is influxdb running on :type influxdb_node_name: str
+:param local_file: path on Jupyterhub for the downlaod .csv file :type local_file: str
+download_timestamp_file(node, data_type, local_file, bind_mount_volume)
+Downloads the collected timestamp file to Jupyterhub Use fablib node.download_file() to download the
+timestamp data file that can be accessed from the bind mount volume :param node: fabric node on which
+the timestamp docker container is running :type node: fablib.node :param data_type: packet_timestamp
+or event timestamp :type data_type: str :param local_file: path on Jupyterhub for the download file :type
+local_file: str :param bind_mount_volume: bind mount volume of the running timestamp docker container
+:type bind_mount_volume: str
+download_timestamp_from_influxdb(node, data_type, bucket, org, token, name, influxdb_ip=None)
+Downloads the timestamp data from influxdb :param node: fabric node on which the timestamp docker
+container is running :type node: fablib.node :param data_type: packet_timestamp or event timestamp :type
+data_type: str :param bucket: name of the influxdb bucket to dump data to :type bucket: str :param org:
+org of the bucket :type org: str :param token: token of the bucket :type token: str :param name: name of the
+timestamp experiment :type name: str :param influxdb_ip: the IP address of the node where the influxdb
+container is running :type influxdb_ip: str, optional
+generate_csv_on_influxdb_node(data_node, name, data_type, bucket, org, token, influxdb_node_name)
+Generates a .csv file in the influxdb container for the query data :param data_node: where the data comes
+from :type data_node: str :param name: name of the timestamp experiment :type name: str :param
+data_type: packet_timestamp or event timestamp :type data_type: str :param bucket: name of the influxdb
+bucket to dump data to :type bucket: str :param org: org of the bucket :type org: str :param token: token
+of the bucket :type token: str :param influxdb_node_name: which fabric node is influxdb running on :type
+influxdb_node_name: str
 
 17
 
+MFLib, Release 1.0.1
+
+get_event_timestamp(node, name, verbose=False)
+Prints the collected event timestamp by calling timestamptool.py in the timestamp docker container running
+on node It reads the local event timestamp file and prints the result :param node: fabric node on which the
+timestamp docker container is running :type node: fablib.node :param name: name of the event timestamp
+experiment :type name: str
+get_packet_timestamp(node, name, verbose=False)
+Prints the collected packet timestamp by calling timestamptool.py in the timestamp docker container running on the node It reads the local packet timestamp file and prints the result :param node: fabric node on
+which the timestamp docker container is running :type node: fablib.node :param name: name of the packet
+timestamp experiment :type name: str
+plot_event_timestamp(json_obj)
+Plots the count of events :param json_obj: list of json objects with timestamp info :type json_obj: list
+plot_packet_timestamp(json_obj)
+Plots the count of packets captured :param json_obj: list of json objects with timestamp info :type json_obj:
+list
+read_from_local_file(file)
+Reads and processes the downloaded timestamp data file :param file: file path on Jupyterhub for the final
+timestamp result :type file: str
+record_event_timestamp(node, name, event, description=None, verbose=False)
+Records event timestamp by calling timestamptool.py in the timestamp docker container running on the
+node :param node: fabric node on which the timestamp docker container is running :type node: fablib.node
+:param name: name of the event timestamp experiment :type name: str :param event: name of the event
+:type event: str :param description: description of the event :type description: str, optional
+record_packet_timestamp(node, name, interface, ipversion, protocol, duration, host=None, port=None,
+verbose=False)
+Records packet timestamp by calling timestamptool.py in the timestamp docker container running on the
+node :param node: fabric node on which the timestamp docker container is running :type node: fablib.node
+:param name: name of the packet timestamp experiment :type name: str :param interface: which interface
+tcpdump captures the packets :type interface: str :param ipversion: IPv4 or IPv6 :type ipversion: str :param
+protocol: tcp or udp :type protocol: str :param duration: seconds to run tcpdump :type duration: str :param
+host: host for tcpdump command :type host: str, optional :param port: port for tcpdump command :type
+port: str, optional
+upload_timestamp_to_influxdb(node, data_type, bucket, org, token, influxdb_ip=None)
+Uploads the timestamp data to influxdb :param node: fabric node on which the timestamp docker container
+is running :type node: fablib.node :param data_type: packet_timestamp or event timestamp :type data_type:
+str :param bucket: name of the influxdb bucket to dump data to :type bucket: str :param org: org of the
+bucket :type org: str :param token: token of the bucket :type token: str :param influxdb_ip: IP of the node
+where influxdb container is running :type influxdb_ip: str, optional
+
+18
+
 CHAPTER
 
 EIGHT
 
 OWL
 
 class mflib.owl.Owl(local_owl_dir, remote_out_dir, remote_conf_dir=None)
@@ -649,17 +725,17 @@
 • port (int) – port to be used by OWL
 • cap_mode (str) – capture mode for OWL. Currently only “save” is supported.
 • pcap_int (int) – time interval (sec) at which tcpdump will start a new pcap file.
 generate_local_links_file(links)
 Create a local copy of links.json file.
 Parameters
 links ([(str, str)]) – list of endpoint pairs [(‘src_ip’, ‘dst_ip’)]
-18
+19
 
-MFLib, Release 1.0.0
+MFLib, Release 1.0.1
 
 get_local_service_file_paths()
 Get paths for owl.conf and links.json files.
 Returns
 owl.conf path, links.json path
 Return type
 [str, str]
@@ -694,17 +770,17 @@
 Parameters
 node (fablib.Node) – remote node
 remove_owl_docker_image(node, name='fabric-owl')
 Remove container with the name given and OWL Docker image saved on the node.
 Parameters
 • node (fablib.Node) – remote node
 
-19
+20
 
-MFLib, Release 1.0.0
+MFLib, Release 1.0.1
 
 • name (str) – container name
 start_owl_receiver(dst_node, receiving_ip, name='fabric-owl', pcap_time_limit=360, duration=180)
 Start Docker container to run OWL receiver.
 Parameters
 • dst_node (fablib.Node) – OWL destination node
 • receiving_ip (str) – IPv4 address of dst node where OWL packets are expected.
@@ -727,156 +803,210 @@
 Parameters
 • node (fablib.Node) – remote node
 • name (str) – container name
 class mflib.owl.OwlMf(local_owl_dir)
 To be used when interacting with OWL on an MF slice with a measurement node. Initializes with the default
 MF paths for remote conf and out directories.
 
-20
+21
 
 CHAPTER
 
 NINE
 
 OWL DATA
 
-21
+mflib.owl_data.convert_pcap_to_csv(pcap_files, outfile='out.csv', append_csv=False, verbose=False)
+Extract data from the list of pcap files and write to one csv file.
+Parameters
+• pcap_files ([posix.Path ]) – list of pcap file paths
+• outfile (str) – name of csv file
+• append_csv (bool) – whether to append data to an existing csv file of that name
+• verbose (bool) – if True, prints each line as it is appended to csv
+mflib.owl_data.list_pcap_files(root_dir)
+Search recursively for pcap files under root_dir
+Parameters
+root_dir (str) – Directory that will be treated as root for this search
+Return files_list
+absolute paths for all the *.pcap files under the root_dir
+Return type
+[posix.Path]
+
+22
 
 PYTHON MODULE INDEX
 
 m
 mflib.core, 12
-mflib.mf_timestamp.mf_timestamp, 17
+mflib.mf_timestamp, 17
 mflib.mflib, 10
-mflib.owl, 18
-mflib.owl_data.OwlDataAnalyzer, 21
+mflib.owl, 19
+mflib.owl_data, 22
 
-22
+23
 
 INDEX
 
 A
 
-get_mfuser_private_key()
-(mflib.core.Core
-method),
-13
-add_mflib_log_handler()
+download_timestamp_from_influxdb()
+(mflib.mf_timestamp.mf_timestamp
 (mflib.mflib.MFLib
-get_owl_log() (mflib.owl.OwlDocker method), 19
+17
+
+add_mflib_log_handler()
 method), 10
-grafana_tunnel (mflib.core.Core property), 13
 addMeasNode() (mflib.mflib.MFLib static method), 10
-grafana_tunnel_local_port (mflib.core.Core property), 13
+
+method),
+
+G
+
 B
+
+generate_csv_on_influxdb_node()
+(mflib.mf_timestamp.mf_timestamp method),
 bootstrap_status_file (mflib.core.Core property),
+17
 12
-
+generate_local_config() (mflib.owl.Owl method),
+19
 C
+generate_local_links_file()
+(mflib.owl.Owl
 check_node_environment()
 (mflib.owl.OwlDocker
-static method), 19
+method), 19
+static method), 20
+get_bootstrap_status() (mflib.core.Core method),
 common_hosts_file (mflib.core.Core property), 12
+13
+convert_pcap_to_csv() (in module mflib.owl_data),
+get_event_timestamp()
+22
+(mflib.mf_timestamp.mf_timestamp method),
 Core (class in mflib.core), 12
+17
 core_class_version (mflib.core.Core attribute), 12
+get_local_service_file_paths() (mflib.owl.Owl
 create() (mflib.core.Core method), 12
+method), 20
 create_local_service_dirs()
 (mflib.owl.Owl
-method), 18
+get_mfuser_private_key()
+(mflib.core.Core
+method), 19
+method), 13
 create_remote_conf_dir() (mflib.owl.Owl method),
-18
+get_owl_log() (mflib.owl.OwlDocker method), 20
+19
+get_packet_timestamp()
 create_remote_out_dir() (mflib.owl.Owl method),
+(mflib.mf_timestamp.mf_timestamp method),
+19
 18
-
-I
-info() (mflib.core.Core method), 13
+grafana_tunnel
+(mflib.core.Core property), 13
+D
+grafana_tunnel_local_port (mflib.core.Core propdelete_remote_output() (mflib.owl.Owl method), 19
+erty), 13
+deploy_influxdb_dashboard()
+(mflib.mf_timestamp.mf_timestamp method), I
+17
+download_common_hosts()
+(mflib.mflib.MFLib info() (mflib.core.Core method), 13
 init() (mflib.mflib.MFLib method), 10
+method), 10
 instrumentize() (mflib.mflib.MFLib method), 11
-
+download_file_from_influxdb()
+(mflib.mf_timestamp.mf_timestamp method),
 K
+17
 kibana_tunnel (mflib.core.Core property), 14
-kibana_tunnel_local_port (mflib.core.Core property), 14
-
+download_log_file() (mflib.core.Core method), 13
+kibana_tunnel_local_port (mflib.core.Core propdownload_output() (mflib.owl.Owl method), 19
+erty), 14
+download_service_file() (mflib.core.Core method),
+13
 L
+download_timestamp_file()
+(mflib.mf_timestamp.mf_timestamp method), list_experiment_ip_addrs() (mflib.owl.Owl static
+17
+method), 20
+24
 
-list_experiment_ip_addrs() (mflib.owl.Owl static
-method), 19
-list_remote_output() (mflib.owl.Owl method), 19
+MFLib, Release 1.0.1
+
+list_pcap_files() (in module mflib.owl_data), 22
+list_remote_output() (mflib.owl.Owl method), 20
 local_mfuser_private_key_filename
 (mflib.core.Core property), 14
-D
 local_mfuser_public_key_filename
 (mflib.core.Core property), 14
-delete_remote_output() (mflib.owl.Owl method), 18
-local_slice_directory
-(mflib.core.Core property),
-download_common_hosts()
-(mflib.mflib.MFLib
+local_slice_directory (mflib.core.Core property),
 14
-method), 10
 log_directory (mflib.core.Core property), 14
-download_log_file() (mflib.core.Core method), 13
-download_output() (mflib.owl.Owl method), 18
-download_service_file() (mflib.core.Core method), M
-13
+
+M
 meas_node (mflib.core.Core property), 15
 meas_node_ip (mflib.core.Core property), 15
-G
+mf_timestamp (class in mflib.mf_timestamp), 17
 MFLib (class in mflib.mflib), 10
-generate_local_config() (mflib.owl.Owl method), mflib.core
+mflib.core
 module, 12
-18
-generate_local_links_file()
-(mflib.owl.Owl mflib.mf_timestamp.mf_timestamp
+mflib.mf_timestamp
 module, 17
-method), 18
-get_bootstrap_status() (mflib.core.Core method), mflib.mflib
+mflib.mflib
 module, 10
-13
-get_local_service_file_paths() (mflib.owl.Owl mflib.owl
-module, 18
-method), 19
-mflib.owl_data.OwlDataAnalyzer
-23
-
-MFLib, Release 1.0.0
-
-module, 21
+mflib.owl
+module, 19
+mflib.owl_data
+module, 22
 mflib_class_version (mflib.mflib.MFLib attribute),
 11
 module
 mflib.core, 12
-mflib.mf_timestamp.mf_timestamp, 17
+mflib.mf_timestamp, 17
 mflib.mflib, 10
-mflib.owl, 18
-mflib.owl_data.OwlDataAnalyzer, 21
-
-upload_service_files() (mflib.core.Core method),
-16
+mflib.owl, 19
+mflib.owl_data, 22
 
 O
-Owl (class in mflib.owl), 18
-OwlDocker (class in mflib.owl), 19
-OwlMf (class in mflib.owl), 20
+Owl (class in mflib.owl), 19
+OwlDocker (class in mflib.owl), 20
+OwlMf (class in mflib.owl), 21
 
 P
+plot_event_timestamp()
+(mflib.mf_timestamp.mf_timestamp method),
+18
+plot_packet_timestamp()
+(mflib.mf_timestamp.mf_timestamp method),
+18
 print_local_service_files()
 (mflib.owl.Owl
-method), 19
+method), 20
 pull_owl_docker_image()
 (mflib.owl.OwlDocker
-method), 19
+method), 20
 
-R
+(mflib.mf_timestamp.mf_timestamp method),
+18
+record_event_timestamp()
+(mflib.mf_timestamp.mf_timestamp method),
+18
+record_packet_timestamp()
+(mflib.mf_timestamp.mf_timestamp method),
+18
 remove() (mflib.core.Core method), 15
 remove_mflib_log_handler()
 (mflib.mflib.MFLib
 method), 11
 remove_owl_docker_image() (mflib.owl.OwlDocker
-method), 19
+method), 20
 restore_DNS() (mflib.mflib.MFLib method), 11
 restore_DNS_all_nodes()
 (mflib.mflib.MFLib
 method), 11
 
 S
 set_core_logger() (mflib.core.Core method), 15
@@ -884,26 +1014,35 @@
 set_DNS_all_nodes() (mflib.mflib.MFLib method), 11
 set_mflib_logger() (mflib.mflib.MFLib method), 11
 slice_name (mflib.core.Core property), 15
 slice_username (mflib.core.Core property), 15
 start() (mflib.core.Core method), 15
 start_owl_receiver()
 (mflib.owl.OwlDocker
-method), 20
+method), 21
 start_owl_sender() (mflib.owl.OwlDocker method),
-20
+21
 stop() (mflib.core.Core method), 16
-stop_owl_docker() (mflib.owl.OwlDocker method), 20
+stop_owl_docker() (mflib.owl.OwlDocker method), 21
 
 T
 tunnel_host (mflib.core.Core property), 16
 
 U
 update() (mflib.core.Core method), 16
 upload_service_directory()
 (mflib.core.Core
 method), 16
+upload_service_files() (mflib.core.Core method),
+16
+upload_timestamp_to_influxdb()
+(mflib.mf_timestamp.mf_timestamp method),
+18
+
+R
+read_from_local_file()
+
 Index
 
-24
+25
```

### Comparing `fabrictestbed-mflib-1.0.0/README.md` & `fabrictestbed-mflib-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-1.0.0/create_html_doc.sh` & `fabrictestbed-mflib-1.0.1/create_html_doc.sh`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-1.0.0/create_pdf_doc.sh` & `fabrictestbed-mflib-1.0.1/create_pdf_doc.sh`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-1.0.0/create_release.sh` & `fabrictestbed-mflib-1.0.1/create_release.sh`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-1.0.0/docs/Makefile` & `fabrictestbed-mflib-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-1.0.0/docs/make.bat` & `fabrictestbed-mflib-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-1.0.0/docs/source/conf.py` & `fabrictestbed-mflib-1.0.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-1.0.0/docs/source/images/3nodes.png` & `fabrictestbed-mflib-1.0.1/docs/source/images/3nodes.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-1.0.0/docs/source/images/3nodes_add_meas.png` & `fabrictestbed-mflib-1.0.1/docs/source/images/3nodes_add_meas.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-1.0.0/docs/source/images/3nodes_ini.png` & `fabrictestbed-mflib-1.0.1/docs/source/images/3nodes_ini.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-1.0.0/docs/source/images/3nodes_inst.png` & `fabrictestbed-mflib-1.0.1/docs/source/images/3nodes_inst.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-1.0.0/docs/source/images/keys.png` & `fabrictestbed-mflib-1.0.1/docs/source/images/keys.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-1.0.0/docs/source/overview.md` & `fabrictestbed-mflib-1.0.1/docs/source/overview.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-1.0.0/mflib/README.md` & `fabrictestbed-mflib-1.0.1/mflib/README.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-1.0.0/mflib/__init__.py` & `fabrictestbed-mflib-1.0.1/mflib/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 FABRIC Measurement Framework Python Client Library - Makes monitoring FABRIC Slice easy.
 """
 # release level is a alpha, b beta, rc candidate, dev development, post post,  or f final
 # (major, minor, micro, release level, release build)
-__version_info__ = [1, 0, 0, "f", 0]
+__version_info__ = [1, 0, 1, "f", 0]
 
 __version__ = f"{__version_info__[0]}.{__version_info__[1]}.{__version_info__[2]}"
 
 if __version_info__[3] != 'f':
     __version__ = f"{__version__}{__version_info__[3]}{__version_info__[4]}"
```

### Comparing `fabrictestbed-mflib-1.0.0/mflib/core.py` & `fabrictestbed-mflib-1.0.1/mflib/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -955,15 +955,15 @@
             force(Boolean): If downloaded file already exists locally, it will not be downloaded unless force is True. .
         Returns:
             Dictionary: Bootstrap dict if any type of bootstraping has occured, Empty dict otherwise.
         """
         if force or not os.path.exists(self.bootstrap_status_file):
             download_success, download_msg = self._download_bootstrap_status()
             if not download_success:
-                return {"msg", download_msg }
+                return {"msg":download_msg }
 
         if os.path.exists(self.bootstrap_status_file):
             if os.stat(self.bootstrap_status_file).st_size == 0:
                 return {}
                 # workaround download creating empty file if file not found
             with open(self.bootstrap_status_file) as bsf:
                 try:
```

### Comparing `fabrictestbed-mflib-1.0.0/mflib/mf_timestamp.py` & `fabrictestbed-mflib-1.0.1/mflib/mf_timestamp.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,17 @@
 from fabrictestbed_extensions.fablib.fablib import fablib
 from fabrictestbed_extensions.fablib.fablib import FablibManager as fablib_manager
 import matplotlib.pyplot as plt
 import pandas as pd
 import numpy as np
 
 class mf_timestamp():
+    """
+    Creates precision timestamps.
+    """
     
     def __init__(self, slice_name, container_name):
         """
         Constructor. Builds Manager for mf_timestamp object.
         """
         super().__init__()
         self.slice_name=slice_name
```

### Comparing `fabrictestbed-mflib-1.0.0/mflib/mflib.py` & `fabrictestbed-mflib-1.0.1/mflib/mflib.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     @staticmethod
     def addMeasNode(
         slice,
         cores=4,
         ram=16,
         disk=500,
         network_type="FABNetv4",
-        site="NCSA",
+        site="EDC",
         image="default_ubuntu_20",
     ):
         """
         Adds Measurement node and measurement network to an unsubmitted slice object.
 
         Args:
             slice (fablib.slice): Slice object already set with experiment topology.
```

### Comparing `fabrictestbed-mflib-1.0.0/mflib/mfvis.py` & `fabrictestbed-mflib-1.0.1/mflib/mfvis.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-1.0.0/mflib/owl.py` & `fabrictestbed-mflib-1.0.1/mflib/owl.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-1.0.0/mflib/owl_data.py` & `fabrictestbed-mflib-1.0.1/mflib/owl_data.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-1.0.0/pyproject.toml` & `fabrictestbed-mflib-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-1.0.0/PKG-INFO` & `fabrictestbed-mflib-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabrictestbed-mflib
-Version: 1.0.0
+Version: 1.0.1
 Summary: FABRIC Measurement Framework Python Client Library - Makes monitoring FABRIC Slice easy.
 Author: Song, Pinyi, Hussam
 Author-email: Carpenter <csacarp0@g.uky.edu>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

