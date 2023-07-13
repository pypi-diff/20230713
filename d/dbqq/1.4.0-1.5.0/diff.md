# Comparing `tmp/dbqq-1.4.0.tar.gz` & `tmp/dbqq-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbqq-1.4.0.tar", last modified: Tue May 16 11:49:03 2023, max compression
+gzip compressed data, was "dbqq-1.5.0.tar", max compression
```

## Comparing `dbqq-1.4.0.tar` & `dbqq-1.5.0.tar`

### file list

```diff
@@ -1,46 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 11:49:03.358244 dbqq-1.4.0/
--rw-rw-rw-   0        0        0    14130 2023-05-16 11:49:03.357244 dbqq-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0    13400 2023-05-16 11:02:12.000000 dbqq-1.4.0/README.md
--rw-rw-rw-   0        0        0     1083 2023-05-16 11:02:12.000000 dbqq-1.4.0/license.md
--rw-rw-rw-   0        0        0     1302 2023-05-16 11:46:52.000000 dbqq-1.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-16 11:49:03.358244 dbqq-1.4.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-16 11:49:03.243243 dbqq-1.4.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-16 11:49:03.268242 dbqq-1.4.0/src/dbqq/
--rw-rw-rw-   0        0        0      127 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:49:03.299242 dbqq-1.4.0/src/dbqq/cli/
--rw-rw-rw-   0        0        0        0 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/cli/__init__.py
--rw-rw-rw-   0        0        0      968 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/cli/clean_connections.py
--rw-rw-rw-   0        0        0      713 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/cli/initialize_connections.py
--rw-rw-rw-   0        0        0     1295 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/cli/run_query.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:49:03.317243 dbqq-1.4.0/src/dbqq/connectors/
--rw-rw-rw-   0        0        0     1013 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/connectors/__init__.py
--rw-rw-rw-   0        0        0     7349 2023-05-16 11:46:45.000000 dbqq-1.4.0/src/dbqq/connectors/_base.py
--rw-rw-rw-   0        0        0     1778 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/connectors/_polar_connector.py
--rw-rw-rw-   0        0        0     5791 2023-05-16 11:46:33.000000 dbqq-1.4.0/src/dbqq/connectors/databricks.py
--rw-rw-rw-   0        0        0     2906 2023-05-16 11:46:33.000000 dbqq-1.4.0/src/dbqq/connectors/mssql.py
--rw-rw-rw-   0        0        0     4747 2023-05-16 11:46:35.000000 dbqq-1.4.0/src/dbqq/connectors/oracle.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:49:03.319241 dbqq-1.4.0/src/dbqq/data/
--rw-rw-rw-   0        0        0       46 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:49:03.326251 dbqq-1.4.0/src/dbqq/data/parsed/
--rw-rw-rw-   0        0        0       40 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/data/parsed/__init__.py
--rw-rw-rw-   0        0        0      822 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/data/parsed/sql.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:49:03.331256 dbqq-1.4.0/src/dbqq/security/
--rw-rw-rw-   0        0        0       86 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/security/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:49:03.343243 dbqq-1.4.0/src/dbqq/security/cli/
--rw-rw-rw-   0        0        0        0 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/security/cli/__init__.py
--rw-rw-rw-   0        0        0     1091 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/security/cli/decrypt_yaml.py
--rw-rw-rw-   0        0        0     1036 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/security/cli/encrypt_yaml.py
--rw-rw-rw-   0        0        0     1707 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/security/cli/write_keys.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:49:03.353245 dbqq-1.4.0/src/dbqq/security/functions/
--rw-rw-rw-   0        0        0      119 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/security/functions/__init__.py
--rw-rw-rw-   0        0        0     1006 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/security/functions/_functions.py
--rw-rw-rw-   0        0        0     4166 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/security/functions/_yaml.py
--rw-rw-rw-   0        0        0     2332 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/security/helpers.py
--rw-rw-rw-   0        0        0     5315 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:49:03.287244 dbqq-1.4.0/src/dbqq.egg-info/
--rw-rw-rw-   0        0        0    14130 2023-05-16 11:49:03.000000 dbqq-1.4.0/src/dbqq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      997 2023-05-16 11:49:03.000000 dbqq-1.4.0/src/dbqq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 11:49:03.000000 dbqq-1.4.0/src/dbqq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      339 2023-05-16 11:49:03.000000 dbqq-1.4.0/src/dbqq.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       96 2023-05-16 11:49:03.000000 dbqq-1.4.0/src/dbqq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-16 11:49:03.000000 dbqq-1.4.0/src/dbqq.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1083 2023-07-13 11:44:16.039818 dbqq-1.5.0/license.md
+-rw-r--r--   0        0        0     1213 2023-07-13 14:55:56.756230 dbqq-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0    13700 2023-07-13 14:41:32.795246 dbqq-1.5.0/README.md
+-rw-r--r--   0        0        0      145 2023-07-13 14:55:56.762231 dbqq-1.5.0/src/dbqq/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 11:44:16.047834 dbqq-1.5.0/src/dbqq/cli/__init__.py
+-rw-r--r--   0        0        0      968 2023-07-13 11:44:16.047834 dbqq-1.5.0/src/dbqq/cli/clean_connections.py
+-rw-r--r--   0        0        0      713 2023-07-13 11:44:16.048865 dbqq-1.5.0/src/dbqq/cli/initialize_connections.py
+-rw-r--r--   0        0        0     1295 2023-07-13 11:44:16.049831 dbqq-1.5.0/src/dbqq/cli/run_query.py
+-rw-r--r--   0        0        0     1013 2023-07-13 11:44:16.052887 dbqq-1.5.0/src/dbqq/connectors/__init__.py
+-rw-r--r--   0        0        0     7349 2023-07-13 11:44:16.053825 dbqq-1.5.0/src/dbqq/connectors/_base.py
+-rw-r--r--   0        0        0     1778 2023-07-13 11:44:16.054824 dbqq-1.5.0/src/dbqq/connectors/_polar_connector.py
+-rw-r--r--   0        0        0     5791 2023-07-13 14:28:07.131900 dbqq-1.5.0/src/dbqq/connectors/databricks.py
+-rw-r--r--   0        0        0     2906 2023-07-13 14:28:07.132901 dbqq-1.5.0/src/dbqq/connectors/mssql.py
+-rw-r--r--   0        0        0     4747 2023-07-13 14:26:02.251424 dbqq-1.5.0/src/dbqq/connectors/oracle.py
+-rw-r--r--   0        0        0       46 2023-07-13 11:44:16.059816 dbqq-1.5.0/src/dbqq/data/__init__.py
+-rw-r--r--   0        0        0       40 2023-07-13 11:44:16.062811 dbqq-1.5.0/src/dbqq/data/parsed/__init__.py
+-rw-r--r--   0        0        0      822 2023-07-13 11:44:16.063810 dbqq-1.5.0/src/dbqq/data/parsed/sql.py
+-rw-r--r--   0        0        0       86 2023-07-13 11:44:16.065807 dbqq-1.5.0/src/dbqq/security/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 11:44:16.068802 dbqq-1.5.0/src/dbqq/security/cli/__init__.py
+-rw-r--r--   0        0        0     1091 2023-07-13 11:44:16.069803 dbqq-1.5.0/src/dbqq/security/cli/decrypt_yaml.py
+-rw-r--r--   0        0        0     1036 2023-07-13 11:44:16.070776 dbqq-1.5.0/src/dbqq/security/cli/encrypt_yaml.py
+-rw-r--r--   0        0        0     1707 2023-07-13 13:10:23.334614 dbqq-1.5.0/src/dbqq/security/cli/write_keys.py
+-rw-r--r--   0        0        0      119 2023-07-13 11:44:16.074791 dbqq-1.5.0/src/dbqq/security/functions/__init__.py
+-rw-r--r--   0        0        0     1006 2023-07-13 11:44:16.074791 dbqq-1.5.0/src/dbqq/security/functions/_functions.py
+-rw-r--r--   0        0        0     4166 2023-07-13 11:44:16.075789 dbqq-1.5.0/src/dbqq/security/functions/_yaml.py
+-rw-r--r--   0        0        0     2332 2023-07-13 11:44:16.076784 dbqq-1.5.0/src/dbqq/security/helpers.py
+-rw-r--r--   0        0        0     6047 2023-07-13 14:15:24.340060 dbqq-1.5.0/src/dbqq/utils.py
+-rw-r--r--   0        0        0    14131 1970-01-01 00:00:00.000000 dbqq-1.5.0/PKG-INFO
```

### Comparing `dbqq-1.4.0/PKG-INFO` & `dbqq-1.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,14 @@
-Metadata-Version: 2.1
-Name: dbqq
-Version: 1.4.0
-Summary: quickly connect to and query databases
-Author-email: Chris Mamon <chrisam1993@live.com>
-Project-URL: Homepage, https://github.com/Chr1sC0de/database-quick-query
-Project-URL: Bug Tracker, https://github.com/Chr1sC0de/database-quick-query/issues
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: license.md
-
 # Database Quick Query
 
 - [Database Quick Query](#database-quick-query)
   - [Environment Variables](#environment-variables)
   - [Initialization](#initialization)
   - [Connection Configuration](#connection-configuration)
+    - [Parameter Stores](#parameter-stores)
   - [Encrypting Configs](#encrypting-configs)
     - [Creating Private and Public Keys](#creating-private-and-public-keys)
     - [Encrypting The Configuration File](#encrypting-the-configuration-file)
   - [Connectors](#connectors)
     - [Caching](#caching)
     - [Getting Basic Table Metadata](#getting-basic-table-metadata)
     - [Running Queries from a File](#running-queries-from-a-file)
@@ -50,14 +34,16 @@
 Example environment variable setup
 
 ```powershell
 # path to private key
 $env:DBQQ_PRIVATE_KEY = ".\private_key.pem" or ".\private_key.der" or "none"
 # path to connections, supports encrypted or flat yaml files
 $env:DBQQ_CONNECTORS = ".\connections.dbqq" or ".\connections.yaml"
+# if we have aws parameter store configuration
+$env:DBQQ_SSM_NAME= "name of parameter"
 ```
 
 ## Initialization
 
 Connections are loaded dynamically, and are initially blank within the
 connection files
 
@@ -157,18 +143,26 @@
     hostname: "*******"
     password: "*******"
     port: "*******"
     role: "*******"
     username: "*******"
 ```
 
-> [!todo]
->
-> add an option to allow users to access private keys from key vault
-> this way no private keys are stored locally only an api key
+### Parameter Stores
+
+Parameters can be extracted from the AWS Parameter Store, which overrides local
+configs. To retrieve the parameters, set the `name` and the `region`. By default,
+the region is set to `ap-southeast-2``.
+
+
+
+```powershell
+$env:DBQQ_SSM_NAME="name"
+$env:DBQQ_SSM_REGION="region"
+```
 
 ## Encrypting Configs
 
 It is probably not the best idea to store passwords as a flat file on your local
 computer. We have added the ability to encrypt configuration files via the
 `dbqq-encrypt-yaml.exe`.
```

### Comparing `dbqq-1.4.0/README.md` & `dbqq-1.5.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,531 +1,570 @@
-# Database Quick Query
-
-- [Database Quick Query](#database-quick-query)
-  - [Environment Variables](#environment-variables)
-  - [Initialization](#initialization)
-  - [Connection Configuration](#connection-configuration)
-  - [Encrypting Configs](#encrypting-configs)
-    - [Creating Private and Public Keys](#creating-private-and-public-keys)
-    - [Encrypting The Configuration File](#encrypting-the-configuration-file)
-  - [Connectors](#connectors)
-    - [Caching](#caching)
-    - [Getting Basic Table Metadata](#getting-basic-table-metadata)
-    - [Running Queries from a File](#running-queries-from-a-file)
-      - [Extracting queries and connections from a file](#extracting-queries-and-connections-from-a-file)
-        - [Basic Connection No Cache](#basic-connection-no-cache)
-        - [Connection With Cache](#connection-with-cache)
-        - [Connection With Cache and Date Lower Bound](#connection-with-cache-and-date-lower-bound)
-    - [Parsing Files](#parsing-files)
-    - [Jinja Templates](#jinja-templates)
-  - [Common Table Expressions](#common-table-expressions)
-    - [Rollback](#rollback)
-  - [Databricks Development](#databricks-development)
-  - [CLI Tools](#cli-tools)
-    - [dbqq-clean-connections](#dbqq-clean-connections)
-    - [dbqq-run-sql](#dbqq-run-sql)
-
-A wrapper over various database connector libraries for quickly performing
-queries for analysis. The package leverages [polars](https://www.pola.rs/) and
-[connectorx](https://github.com/sfu-db/connector-x) for their speed when handling Big data.
-
-## Environment Variables
-
-Example environment variable setup
-
-```powershell
-# path to private key
-$env:DBQQ_PRIVATE_KEY = ".\private_key.pem" or ".\private_key.der" or "none"
-# path to connections, supports encrypted or flat yaml files
-$env:DBQQ_CONNECTORS = ".\connections.dbqq" or ".\connections.yaml"
-```
-
-## Initialization
-
-Connections are loaded dynamically, and are initially blank within the
-connection files
-
-```python
-# dbqq/connectors/databricks.py etc.
-
-#! begin inject regex
-
-#! end inject regex
-```
-
-To initialize connections, simply install the package and run the command
-
-```powershell
-dbqq-initialize-connectors
-```
-
-As an example, after importing the package the configured connections should now
-be visible within the connection files. The following will be the result of an
-initialization given the configs in the `Connection Configuration` section.
-
-```python
-# dbqq/connectors/databricks.py
-
-#! begin inject regex
-
-class preprod(_general_connector):
-    source: str = 'preprod'
-
-class prod(_general_connector):
-    source: str = 'prod'
-
-class test(_general_connector):
-    source: str = 'test'
-
-class dev(_general_connector):
-    source: str = 'dev'
-
-#! end inject regex
-```
-
-## Connection Configuration
-
-To configure login details for various databases fill out the following required
-details into a `.yaml` (optionally now encrypt the file and delete the yaml)
-and set the environment variable `DBQQ_PRIVATE_KEY` to the location of the file.
-
-```yaml
-databricks:
-  dev:
-    access_token: "*******"
-    http_path: "*******"
-    server_hostname: "*******"
-  test:
-    access_token: "*******"
-    http_path: "*******"
-    server_hostname: "*******"
-  preprod:
-    access_token: "*******"
-    http_path: "*******"
-    server_hostname: "*******"
-  prod:
-    access_token: "*******"
-    http_path: "*******"
-    server_hostname: "*******"
-mssql:
-  conn1:
-    authentication_type: "*******"
-    database: "*******"
-    driver: "*******"
-    hostname: "*******"
-    password: "*******"
-    port: "*******"
-    username: "*******"
-  conn2:
-    authentication_type: "*******"
-    database: "*******"
-    driver: "*******"
-    hostname: "*******"
-    password: "*******"
-    port: "*******"
-    username: "*******"
-oracle:
-  conn1:
-    authentication_type: "*******"
-    connection_type: "*******"
-    database: "*******"
-    hostname: "*******"
-    password: "*******"
-    port: "*******"
-    role: "*******"
-    username: "*******"
-  conn2:
-    authentication_type: "*******"
-    connection_type: "*******"
-    database: "*******"
-    hostname: "*******"
-    password: "*******"
-    port: "*******"
-    role: "*******"
-    username: "*******"
-```
-
-> [!todo]
->
-> add an option to allow users to access private keys from key vault
-> this way no private keys are stored locally only an api key
-
-## Encrypting Configs
-
-It is probably not the best idea to store passwords as a flat file on your local
-computer. We have added the ability to encrypt configuration files via the
-`dbqq-encrypt-yaml.exe`.
-
-### Creating Private and Public Keys
-
-Before we can encrypt our configuration file we need to create both private and
-public keys. For our example let's say we have a working directory
-with the following configuration file
-
-```powershell
-C:\devops> ls
-
-Mode                 LastWriteTime         Length Name
-----                 -------------         ------ ----
--a----                                            config.yaml
-
-```
-
-create a folder called keys
-
-```powershell
-C:\devops> mkdir keys
-```
-
-we can use the `dbqq-write-keys.exe` method to generate the private and public
-keys
-
-```powershell
-C:\devops> dbqq-write-keys -l './keys' -k 1024 # supports der or pem call -h for help
-C:\devops> ls keys
-Mode                 LastWriteTime         Length Name
-----                 -------------         ------ ----
--a----                                            private_key.der
--a----                                            public_key.der
-```
-
-### Encrypting The Configuration File
-
-Apply `dbqq-encrypt-yaml` on the config file with the generated private key
-
-```powershell
-
-C:\devops> dbqq-encrypt-yaml 'config.yaml' './keys/private_key.der'
-C:\devops> ls keys
-Mode                 LastWriteTime         Length Name
-----                 -------------         ------ ----
--a----                                            config.dbqq
-
-```
-
-Finally secure the private key
-
-## Connectors
-
-The connectors module reads from the configuration files, categorizing the
-details into (currently) either an `oracle`, `mssql` or `databricks` connection.
-
-Given our example configuration file we can create an `oracle` to db `conn1` by
-calling:
-
-```python
-import polars as pl
-from dbqq import connectors
-
-connection = connectors.oracle.db1()
-
-```
-
-to run a query simply call the connection
-
-```python
-df: pl.LazyFrame = connection("select * from some.table")
-```
-
-connection calls always return a polars
-[LazyFrame](https://pola-rs.github.io/polars/py-polars/html/reference/lazyframe/index.html).
-This is because LazyFrames allow for whole-query optimisation in addition to
-parallelism, making them the preferred (and highest-performance) mode of
-operation for polars.
-
-Run `collect` to work with a DataFrame or `fetch` to partially collect
-
-```python
-df: pl.Dataframe = df.collect()
-```
-
-### Caching
-
-During the analysis, we may want to cache queries for iteration. This can be
-performed simply by calling the cache method:
-
-```python
-connection.cache()("select * from schema.table")
-```
-
-the data will be saved as a `.parquet` file with a corresponding `.yaml` file.
-The cached files will be stored in the `.temp` folder with a unique identifier
-unless specified.
-
-To set the location and name of the cached files
-
-```python
-connection.cache(directory="./cache_directory",name="name")(
-    "select * from schema.table")
-```
-
-Finally, we might want to save a new cache every day while clearing out old
-files. This can be done using the `date_lower_bound` keyword argument. Files
-before this date will be deleted for **all** cached queries.
-
-```python
-from datetime import datetime, timedelta
-
-connection.cache(
-    date_lower_bound = datetime.now() - timedelta(days=1)
-)("select * from schema.table")
-```
-
-### Getting Basic Table Metadata
-
-To get information about the columns before running the query run the
-`describe_columns` method on the table using the required connection.
-
-```python
-connection.describe("table_name")
-```
-
-To get the schema of the table call the `schema` attribute on the LazyFrame
-
-```python
-df: pl.LazyFrame = connection("select * from some.table")
-df.schema
-```
-
-### Running Queries from a File
-
-To run a query directly from a file
-
-```python
-connection.from_file("path to file", *args, **kwargs)
-```
-
-where `*args`, `**kwargs` are the arguments for a regular `__call__`.
-
-#### Extracting queries and connections from a file
-
-We can include metadata to an sql file and call the `connectors.from_file`
-method to extract both a the connection and query. There are 3 ways we can
-include metadata.
-
-##### Basic Connection No Cache
-
-To create a simple connection we can add the following configuration string
-to the sql file.
-
-```sql
---! name/connector.{type}.{db}
-select * from some.table
-```
-
-Replace {} with connection information i.e. databricks.prod.
-
-The configuration string will be removed from the query.
-
-```python
-connection, query = connectors.from_file(filepath)
-df = connection(query)
-
-```
-
-##### Connection With Cache
-
-To create a connection with a path to a cache file add a string to the
-configuration specifying the path to the cache folder. The `name` provided will
-be used as the name of the cache i.e. `name.parquet`. If `name`=`_` then a
-unique identifier will be used as the name for the cache.
-
-```sql
---! name/"./temp"/connector.{type}.{db}
-select * from some.table
-```
-
-##### Connection With Cache and Date Lower Bound
-
-To add a date lower bound add a command which can be evaluated by python. Note, datetim and timedelta
-are imported during the eval process.
-
-```sql
---! name/"./temp"/datetime.now()-timedelta(days=7)/connector.{type}.{db}
-select * from some.table
-```
-
-### Parsing Files
-
-We might simply want to parse the files i.e. for automating tasks.
-
-```python
-from dbqq import utils
-
-data = utils.parse_file("<path to file>")
-```
-
-data for parsed sql can be found in connectors.data.parsed.sql
-
-### Jinja Templates
-
-We can parse jinja templates, let's say we have a template called `test_query.sql.j2`
-
-```jinja
-select
-{% for item in  columns %}
-{% if loop.last %}
-    {{ item }}
-{% else %}
-    {{ item }},
-{% endif %}
-{% endfor %}
-from
-  some.table
-```
-
-We can create a `RenderedTemplateLoader` from it using the following
-
-```python
-import dbqq.connectors as dbc
-
-conn = dbc.<source>.<conn>()
-
-rendered_template_loader = conn.render_template(
-    "test_query.sql.j2",
-    columns=[
-      "col1",
-      "col2",
-      "col3",
-      "col4"
-    ],
-)
-
-# will return a object that shows the renderedquery
-
-"""
-select
-  col1,
-  col2,
-  col3,
-  col4
-from
-  some.table
-"""
-
-table = rendered_template_loader.execute()
-
-```
-
-## Common Table Expressions
-
-We can construct a common table expression with the following method
-
-```python
-from dbqq import utils
-from triple_quote_clean import TripleQuoteCleaner
-
-tqc = TripleQuoteCleaner(skip_top_lines=1)
-
-cte = utils.CommonTableExpression()
-
-cte.add_query(
-    "query_1",
-    """--sql
-        select *
-        from table_1
-    """ >> tqc
-)
-
-cte.add_query(
-    "query_2",
-    """--sql
-        select
-            *
-        from
-            table_2 t2
-        inner join table_1 t1
-            on t1.col1 = t2.col2
-
-    """ >> tqc
-)
-
-print(cte("select * from table_2"))
-```
-
-output
-
-```sql
-with
-query_1 as (
-    select *
-    from table_1
-)
-,
-query_2 as (
-    select
-        *
-    from
-        table_2 t2
-    inner join table_1 t1
-        on t1.col1 = t2.col2
-)
-select * from table_2
-```
-
-### Rollback
-
-When in a jupyter notebook we can rollback queries during the development process
-
-```python
-cte.rollback_one() # or rollback(version_no)
-cte.add_query(
-    query_name,
-    query
-)
-```
-
-this allows us to modify the cte on the fly
-
-## Databricks Development
-
-sometimes we may want to develop databricks queries locally, and use spark when
-in databricks.
-
-```python
-connection = dbqq.connectors.databricks.prod()
-...
-```
-
-when in databricks the connection will be automatically converted into a
-
-```python
-dbqq.connectors.databricks.Cluster
-```
-
-object, which now will use the spark context to run queries.
-
-## CLI Tools
-
-### dbqq-clean-connections
-
-Clean up all the connections, useful for a fresh start
-
-```powershell
-usage: dbqq-clean-connections.exe [-h]
-
-Clean up all connection information
-
-optional arguments:
-  -h, --help  show this help message and exit
-```
-
-### dbqq-run-sql
-
-run the sql with the provided configurations
-
-```powershell
-usage: dbqq-run-sql.exe [-h] [-n ROWS] [-i {0,1}] file
-
-Run a query directly from an file
-
-positional arguments:
-  file                  *.sql file to be run
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -n ROWS, --rows ROWS  the total number of rows to show number, specify 'all' to show all
-  -i {0,1}, --show_index {0,1}
-                        show the index
-```
-
-Combine [parquet to csv](https://github.com/Chr1sC0de/ParquetToCSV) to view/convert the output
+Metadata-Version: 2.1
+Name: dbqq
+Version: 1.5.0
+Summary: 
+License: MIT
+Author: Chris.Mamon
+Author-email: chrisam1993@live.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: boto3 (>=1.28.2,<2.0.0)
+Requires-Dist: connectorx (>=0.3.1,<0.4.0)
+Requires-Dist: databricks-sql-connector (>=2.7.0,<3.0.0)
+Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: polars (>=0.18.7,<0.19.0)
+Requires-Dist: pyaml (>=23.7.0,<24.0.0)
+Requires-Dist: pyarrow (>=12.0.1,<13.0.0)
+Requires-Dist: rsa (>=4.9,<5.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
+Requires-Dist: triple-quote-clean (>=1.1.0,<2.0.0)
+Description-Content-Type: text/markdown
+
+# Database Quick Query
+
+- [Database Quick Query](#database-quick-query)
+  - [Environment Variables](#environment-variables)
+  - [Initialization](#initialization)
+  - [Connection Configuration](#connection-configuration)
+    - [Parameter Stores](#parameter-stores)
+  - [Encrypting Configs](#encrypting-configs)
+    - [Creating Private and Public Keys](#creating-private-and-public-keys)
+    - [Encrypting The Configuration File](#encrypting-the-configuration-file)
+  - [Connectors](#connectors)
+    - [Caching](#caching)
+    - [Getting Basic Table Metadata](#getting-basic-table-metadata)
+    - [Running Queries from a File](#running-queries-from-a-file)
+      - [Extracting queries and connections from a file](#extracting-queries-and-connections-from-a-file)
+        - [Basic Connection No Cache](#basic-connection-no-cache)
+        - [Connection With Cache](#connection-with-cache)
+        - [Connection With Cache and Date Lower Bound](#connection-with-cache-and-date-lower-bound)
+    - [Parsing Files](#parsing-files)
+    - [Jinja Templates](#jinja-templates)
+  - [Common Table Expressions](#common-table-expressions)
+    - [Rollback](#rollback)
+  - [Databricks Development](#databricks-development)
+  - [CLI Tools](#cli-tools)
+    - [dbqq-clean-connections](#dbqq-clean-connections)
+    - [dbqq-run-sql](#dbqq-run-sql)
+
+A wrapper over various database connector libraries for quickly performing
+queries for analysis. The package leverages [polars](https://www.pola.rs/) and
+[connectorx](https://github.com/sfu-db/connector-x) for their speed when handling Big data.
+
+## Environment Variables
+
+Example environment variable setup
+
+```powershell
+# path to private key
+$env:DBQQ_PRIVATE_KEY = ".\private_key.pem" or ".\private_key.der" or "none"
+# path to connections, supports encrypted or flat yaml files
+$env:DBQQ_CONNECTORS = ".\connections.dbqq" or ".\connections.yaml"
+# if we have aws parameter store configuration
+$env:DBQQ_SSM_NAME= "name of parameter"
+```
+
+## Initialization
+
+Connections are loaded dynamically, and are initially blank within the
+connection files
+
+```python
+# dbqq/connectors/databricks.py etc.
+
+#! begin inject regex
+
+#! end inject regex
+```
+
+To initialize connections, simply install the package and run the command
+
+```powershell
+dbqq-initialize-connectors
+```
+
+As an example, after importing the package the configured connections should now
+be visible within the connection files. The following will be the result of an
+initialization given the configs in the `Connection Configuration` section.
+
+```python
+# dbqq/connectors/databricks.py
+
+#! begin inject regex
+
+class preprod(_general_connector):
+    source: str = 'preprod'
+
+class prod(_general_connector):
+    source: str = 'prod'
+
+class test(_general_connector):
+    source: str = 'test'
+
+class dev(_general_connector):
+    source: str = 'dev'
+
+#! end inject regex
+```
+
+## Connection Configuration
+
+To configure login details for various databases fill out the following required
+details into a `.yaml` (optionally now encrypt the file and delete the yaml)
+and set the environment variable `DBQQ_PRIVATE_KEY` to the location of the file.
+
+```yaml
+databricks:
+  dev:
+    access_token: "*******"
+    http_path: "*******"
+    server_hostname: "*******"
+  test:
+    access_token: "*******"
+    http_path: "*******"
+    server_hostname: "*******"
+  preprod:
+    access_token: "*******"
+    http_path: "*******"
+    server_hostname: "*******"
+  prod:
+    access_token: "*******"
+    http_path: "*******"
+    server_hostname: "*******"
+mssql:
+  conn1:
+    authentication_type: "*******"
+    database: "*******"
+    driver: "*******"
+    hostname: "*******"
+    password: "*******"
+    port: "*******"
+    username: "*******"
+  conn2:
+    authentication_type: "*******"
+    database: "*******"
+    driver: "*******"
+    hostname: "*******"
+    password: "*******"
+    port: "*******"
+    username: "*******"
+oracle:
+  conn1:
+    authentication_type: "*******"
+    connection_type: "*******"
+    database: "*******"
+    hostname: "*******"
+    password: "*******"
+    port: "*******"
+    role: "*******"
+    username: "*******"
+  conn2:
+    authentication_type: "*******"
+    connection_type: "*******"
+    database: "*******"
+    hostname: "*******"
+    password: "*******"
+    port: "*******"
+    role: "*******"
+    username: "*******"
+```
+
+### Parameter Stores
+
+Parameters can be extracted from the AWS Parameter Store, which overrides local
+configs. To retrieve the parameters, set the `name` and the `region`. By default,
+the region is set to `ap-southeast-2``.
+
+
+
+```powershell
+$env:DBQQ_SSM_NAME="name"
+$env:DBQQ_SSM_REGION="region"
+```
+
+## Encrypting Configs
+
+It is probably not the best idea to store passwords as a flat file on your local
+computer. We have added the ability to encrypt configuration files via the
+`dbqq-encrypt-yaml.exe`.
+
+### Creating Private and Public Keys
+
+Before we can encrypt our configuration file we need to create both private and
+public keys. For our example let's say we have a working directory
+with the following configuration file
+
+```powershell
+C:\devops> ls
+
+Mode                 LastWriteTime         Length Name
+----                 -------------         ------ ----
+-a----                                            config.yaml
+
+```
+
+create a folder called keys
+
+```powershell
+C:\devops> mkdir keys
+```
+
+we can use the `dbqq-write-keys.exe` method to generate the private and public
+keys
+
+```powershell
+C:\devops> dbqq-write-keys -l './keys' -k 1024 # supports der or pem call -h for help
+C:\devops> ls keys
+Mode                 LastWriteTime         Length Name
+----                 -------------         ------ ----
+-a----                                            private_key.der
+-a----                                            public_key.der
+```
+
+### Encrypting The Configuration File
+
+Apply `dbqq-encrypt-yaml` on the config file with the generated private key
+
+```powershell
+
+C:\devops> dbqq-encrypt-yaml 'config.yaml' './keys/private_key.der'
+C:\devops> ls keys
+Mode                 LastWriteTime         Length Name
+----                 -------------         ------ ----
+-a----                                            config.dbqq
+
+```
+
+Finally secure the private key
+
+## Connectors
+
+The connectors module reads from the configuration files, categorizing the
+details into (currently) either an `oracle`, `mssql` or `databricks` connection.
+
+Given our example configuration file we can create an `oracle` to db `conn1` by
+calling:
+
+```python
+import polars as pl
+from dbqq import connectors
+
+connection = connectors.oracle.db1()
+
+```
+
+to run a query simply call the connection
+
+```python
+df: pl.LazyFrame = connection("select * from some.table")
+```
+
+connection calls always return a polars
+[LazyFrame](https://pola-rs.github.io/polars/py-polars/html/reference/lazyframe/index.html).
+This is because LazyFrames allow for whole-query optimisation in addition to
+parallelism, making them the preferred (and highest-performance) mode of
+operation for polars.
+
+Run `collect` to work with a DataFrame or `fetch` to partially collect
+
+```python
+df: pl.Dataframe = df.collect()
+```
+
+### Caching
+
+During the analysis, we may want to cache queries for iteration. This can be
+performed simply by calling the cache method:
+
+```python
+connection.cache()("select * from schema.table")
+```
+
+the data will be saved as a `.parquet` file with a corresponding `.yaml` file.
+The cached files will be stored in the `.temp` folder with a unique identifier
+unless specified.
+
+To set the location and name of the cached files
+
+```python
+connection.cache(directory="./cache_directory",name="name")(
+    "select * from schema.table")
+```
+
+Finally, we might want to save a new cache every day while clearing out old
+files. This can be done using the `date_lower_bound` keyword argument. Files
+before this date will be deleted for **all** cached queries.
+
+```python
+from datetime import datetime, timedelta
+
+connection.cache(
+    date_lower_bound = datetime.now() - timedelta(days=1)
+)("select * from schema.table")
+```
+
+### Getting Basic Table Metadata
+
+To get information about the columns before running the query run the
+`describe_columns` method on the table using the required connection.
+
+```python
+connection.describe("table_name")
+```
+
+To get the schema of the table call the `schema` attribute on the LazyFrame
+
+```python
+df: pl.LazyFrame = connection("select * from some.table")
+df.schema
+```
+
+### Running Queries from a File
+
+To run a query directly from a file
+
+```python
+connection.from_file("path to file", *args, **kwargs)
+```
+
+where `*args`, `**kwargs` are the arguments for a regular `__call__`.
+
+#### Extracting queries and connections from a file
+
+We can include metadata to an sql file and call the `connectors.from_file`
+method to extract both a the connection and query. There are 3 ways we can
+include metadata.
+
+##### Basic Connection No Cache
+
+To create a simple connection we can add the following configuration string
+to the sql file.
+
+```sql
+--! name/connector.{type}.{db}
+select * from some.table
+```
+
+Replace {} with connection information i.e. databricks.prod.
+
+The configuration string will be removed from the query.
+
+```python
+connection, query = connectors.from_file(filepath)
+df = connection(query)
+
+```
+
+##### Connection With Cache
+
+To create a connection with a path to a cache file add a string to the
+configuration specifying the path to the cache folder. The `name` provided will
+be used as the name of the cache i.e. `name.parquet`. If `name`=`_` then a
+unique identifier will be used as the name for the cache.
+
+```sql
+--! name/"./temp"/connector.{type}.{db}
+select * from some.table
+```
+
+##### Connection With Cache and Date Lower Bound
+
+To add a date lower bound add a command which can be evaluated by python. Note, datetim and timedelta
+are imported during the eval process.
+
+```sql
+--! name/"./temp"/datetime.now()-timedelta(days=7)/connector.{type}.{db}
+select * from some.table
+```
+
+### Parsing Files
+
+We might simply want to parse the files i.e. for automating tasks.
+
+```python
+from dbqq import utils
+
+data = utils.parse_file("<path to file>")
+```
+
+data for parsed sql can be found in connectors.data.parsed.sql
+
+### Jinja Templates
+
+We can parse jinja templates, let's say we have a template called `test_query.sql.j2`
+
+```jinja
+select
+{% for item in  columns %}
+{% if loop.last %}
+    {{ item }}
+{% else %}
+    {{ item }},
+{% endif %}
+{% endfor %}
+from
+  some.table
+```
+
+We can create a `RenderedTemplateLoader` from it using the following
+
+```python
+import dbqq.connectors as dbc
+
+conn = dbc.<source>.<conn>()
+
+rendered_template_loader = conn.render_template(
+    "test_query.sql.j2",
+    columns=[
+      "col1",
+      "col2",
+      "col3",
+      "col4"
+    ],
+)
+
+# will return a object that shows the renderedquery
+
+"""
+select
+  col1,
+  col2,
+  col3,
+  col4
+from
+  some.table
+"""
+
+table = rendered_template_loader.execute()
+
+```
+
+## Common Table Expressions
+
+We can construct a common table expression with the following method
+
+```python
+from dbqq import utils
+from triple_quote_clean import TripleQuoteCleaner
+
+tqc = TripleQuoteCleaner(skip_top_lines=1)
+
+cte = utils.CommonTableExpression()
+
+cte.add_query(
+    "query_1",
+    """--sql
+        select *
+        from table_1
+    """ >> tqc
+)
+
+cte.add_query(
+    "query_2",
+    """--sql
+        select
+            *
+        from
+            table_2 t2
+        inner join table_1 t1
+            on t1.col1 = t2.col2
+
+    """ >> tqc
+)
+
+print(cte("select * from table_2"))
+```
+
+output
+
+```sql
+with
+query_1 as (
+    select *
+    from table_1
+)
+,
+query_2 as (
+    select
+        *
+    from
+        table_2 t2
+    inner join table_1 t1
+        on t1.col1 = t2.col2
+)
+select * from table_2
+```
+
+### Rollback
+
+When in a jupyter notebook we can rollback queries during the development process
+
+```python
+cte.rollback_one() # or rollback(version_no)
+cte.add_query(
+    query_name,
+    query
+)
+```
+
+this allows us to modify the cte on the fly
+
+## Databricks Development
+
+sometimes we may want to develop databricks queries locally, and use spark when
+in databricks.
+
+```python
+connection = dbqq.connectors.databricks.prod()
+...
+```
+
+when in databricks the connection will be automatically converted into a
+
+```python
+dbqq.connectors.databricks.Cluster
+```
+
+object, which now will use the spark context to run queries.
+
+## CLI Tools
+
+### dbqq-clean-connections
+
+Clean up all the connections, useful for a fresh start
+
+```powershell
+usage: dbqq-clean-connections.exe [-h]
+
+Clean up all connection information
+
+optional arguments:
+  -h, --help  show this help message and exit
+```
+
+### dbqq-run-sql
+
+run the sql with the provided configurations
+
+```powershell
+usage: dbqq-run-sql.exe [-h] [-n ROWS] [-i {0,1}] file
+
+Run a query directly from an file
+
+positional arguments:
+  file                  *.sql file to be run
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -n ROWS, --rows ROWS  the total number of rows to show number, specify 'all' to show all
+  -i {0,1}, --show_index {0,1}
+                        show the index
+```
+
+Combine [parquet to csv](https://github.com/Chr1sC0de/ParquetToCSV) to view/convert the output
+
```

### Comparing `dbqq-1.4.0/license.md` & `dbqq-1.5.0/license.md`

 * *Files identical despite different names*

### Comparing `dbqq-1.4.0/src/dbqq/cli/clean_connections.py` & `dbqq-1.5.0/src/dbqq/cli/clean_connections.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.4.0/src/dbqq/cli/initialize_connections.py` & `dbqq-1.5.0/src/dbqq/cli/initialize_connections.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.4.0/src/dbqq/cli/run_query.py` & `dbqq-1.5.0/src/dbqq/cli/run_query.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.4.0/src/dbqq/connectors/__init__.py` & `dbqq-1.5.0/src/dbqq/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.4.0/src/dbqq/connectors/_base.py` & `dbqq-1.5.0/src/dbqq/connectors/_base.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.4.0/src/dbqq/connectors/_polar_connector.py` & `dbqq-1.5.0/src/dbqq/connectors/_polar_connector.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.4.0/src/dbqq/connectors/databricks.py` & `dbqq-1.5.0/src/dbqq/connectors/databricks.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.4.0/src/dbqq/connectors/mssql.py` & `dbqq-1.5.0/src/dbqq/connectors/mssql.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.4.0/src/dbqq/connectors/oracle.py` & `dbqq-1.5.0/src/dbqq/connectors/oracle.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.4.0/src/dbqq/data/parsed/sql.py` & `dbqq-1.5.0/src/dbqq/data/parsed/sql.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.4.0/src/dbqq/security/cli/decrypt_yaml.py` & `dbqq-1.5.0/src/dbqq/security/cli/decrypt_yaml.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.4.0/src/dbqq/security/cli/encrypt_yaml.py` & `dbqq-1.5.0/src/dbqq/security/cli/encrypt_yaml.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.4.0/src/dbqq/security/cli/write_keys.py` & `dbqq-1.5.0/src/dbqq/security/cli/write_keys.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.4.0/src/dbqq/security/functions/_functions.py` & `dbqq-1.5.0/src/dbqq/security/functions/_functions.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.4.0/src/dbqq/security/functions/_yaml.py` & `dbqq-1.5.0/src/dbqq/security/functions/_yaml.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.4.0/src/dbqq/security/helpers.py` & `dbqq-1.5.0/src/dbqq/security/helpers.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.4.0/src/dbqq/utils.py` & `dbqq-1.5.0/src/dbqq/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,19 +9,39 @@
 
 from .security.functions._functions import load_private_key
 from .security.functions._yaml import decrypt
 from .security.helpers import RSA
 from .data import parsed
 
 
+def get_ssm_connector_details(name: str, region: str = "ap-southeast-2"):
+    import boto3
+    import yaml
+
+    client = boto3.client("ssm", region_name=region)
+    parameter = client.get_parameter(Name=name, WithDecryption=True)[
+        "Parameter"
+    ]["Value"]
+    return yaml.safe_load(parameter)
+
+
 def get_connector_details(dev_path: pt.Path = None) -> Dict[str, str]:
+    ssm_name = os.getenv("DBQQ_SSM_NAME", None)
+    ssm_region = os.getenv("DBQQ_SSM_REGION", "ap-southeast-2")
+    connector_path = os.getenv("DBQQ_CONNECTORS", None)
     if dev_path is not None:
         connector_file = pt.Path(dev_path)
+    elif ssm_name is not None:
+        return get_ssm_connector_details(ssm_name, region=ssm_region)
     else:
-        connector_file = pt.Path(os.getenv("DBQQ_CONNECTORS"))
+        try:
+            connector_file = pt.Path(connector_path)
+        except TypeError as type_error:
+            print("DBQQ_CONNECTORS environment variable not set")
+            raise type_error
     assert connector_file.exists(), "%s does not exist" % connector_file
 
     if connector_file.suffix == ".yaml":
         with open(connector_file, "r") as f:
             connector_details = yaml.safe_load(f)
 
     elif connector_file.suffix == ".dbqq":
```

