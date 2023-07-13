# Comparing `tmp/moonstreamdb-0.3.3.tar.gz` & `tmp/moonstreamdb-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moonstreamdb-0.3.3.tar", last modified: Wed Mar  8 17:15:08 2023, max compression
+gzip compressed data, was "moonstreamdb-0.3.4.tar", last modified: Thu Jul 13 09:23:41 2023, max compression
```

## Comparing `moonstreamdb-0.3.3.tar` & `moonstreamdb-0.3.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 17:15:08.078117 moonstreamdb-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (122)     2344 2023-03-08 17:15:08.078117 moonstreamdb-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-03-08 17:14:53.000000 moonstreamdb-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 17:15:08.078117 moonstreamdb-0.3.3/moonstreamdb/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-08 17:14:53.000000 moonstreamdb-0.3.3/moonstreamdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3680 2023-03-08 17:14:53.000000 moonstreamdb-0.3.3/moonstreamdb/blockchain.py
--rw-r--r--   0 runner    (1001) docker     (122)     3157 2023-03-08 17:14:53.000000 moonstreamdb-0.3.3/moonstreamdb/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     3110 2023-03-08 17:14:53.000000 moonstreamdb-0.3.3/moonstreamdb/db.py
--rw-r--r--   0 runner    (1001) docker     (122)    19631 2023-03-08 17:14:53.000000 moonstreamdb-0.3.3/moonstreamdb/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     1353 2023-03-08 17:14:53.000000 moonstreamdb-0.3.3/moonstreamdb/networks.py
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-03-08 17:14:53.000000 moonstreamdb-0.3.3/moonstreamdb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 17:15:08.078117 moonstreamdb-0.3.3/moonstreamdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2344 2023-03-08 17:15:08.000000 moonstreamdb-0.3.3/moonstreamdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      434 2023-03-08 17:15:08.000000 moonstreamdb-0.3.3/moonstreamdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-08 17:15:08.000000 moonstreamdb-0.3.3/moonstreamdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-03-08 17:15:08.000000 moonstreamdb-0.3.3/moonstreamdb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-08 17:15:07.000000 moonstreamdb-0.3.3/moonstreamdb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-03-08 17:15:08.000000 moonstreamdb-0.3.3/moonstreamdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-03-08 17:15:08.000000 moonstreamdb-0.3.3/moonstreamdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-08 17:15:08.078117 moonstreamdb-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1491 2023-03-08 17:14:53.000000 moonstreamdb-0.3.3/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-13 09:23:41.013266 moonstreamdb-0.3.4/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2027 2023-07-13 09:23:41.013266 moonstreamdb-0.3.4/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1210 2023-06-06 15:34:13.000000 moonstreamdb-0.3.4/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-13 09:23:41.009266 moonstreamdb-0.3.4/moonstreamdb/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 15:34:13.000000 moonstreamdb-0.3.4/moonstreamdb/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4575 2023-07-13 09:04:28.000000 moonstreamdb-0.3.4/moonstreamdb/blockchain.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3157 2023-06-06 15:34:13.000000 moonstreamdb-0.3.4/moonstreamdb/cli.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3110 2023-07-13 09:04:28.000000 moonstreamdb-0.3.4/moonstreamdb/db.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23595 2023-07-13 09:04:28.000000 moonstreamdb-0.3.4/moonstreamdb/models.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1695 2023-07-13 09:04:28.000000 moonstreamdb-0.3.4/moonstreamdb/networks.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       69 2023-07-13 09:04:28.000000 moonstreamdb-0.3.4/moonstreamdb/version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-13 09:23:41.013266 moonstreamdb-0.3.4/moonstreamdb.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2027 2023-07-13 09:23:40.000000 moonstreamdb-0.3.4/moonstreamdb.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      434 2023-07-13 09:23:40.000000 moonstreamdb-0.3.4/moonstreamdb.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-13 09:23:40.000000 moonstreamdb-0.3.4/moonstreamdb.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       55 2023-07-13 09:23:40.000000 moonstreamdb-0.3.4/moonstreamdb.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-10-19 09:13:57.000000 moonstreamdb-0.3.4/moonstreamdb.egg-info/not-zip-safe
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      103 2023-07-13 09:23:40.000000 moonstreamdb-0.3.4/moonstreamdb.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       13 2023-07-13 09:23:40.000000 moonstreamdb-0.3.4/moonstreamdb.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-13 09:23:41.013266 moonstreamdb-0.3.4/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1491 2023-06-06 15:34:13.000000 moonstreamdb-0.3.4/setup.py
```

### Comparing `moonstreamdb-0.3.3/PKG-INFO` & `moonstreamdb-0.3.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 Metadata-Version: 2.1
 Name: moonstreamdb
-Version: 0.3.3
+Version: 0.3.4
 Summary: Moonstream database
 Home-page: https://github.com/bugout-dev/moonstream
 Author: Bugout.dev
 Author-email: engineers@bugout.dev
 License: Apache License 2.0
-Description: # moonstream db
-        
-        ### Setting up moonstreamdb
-        
-        Copy `sample.env` to a new file and set the environment variables to appropriate values. This new file
-        should be sourced every time you want to access the database with the `moonstreamdb` application or any
-        dependents.
-        
-        To be able to run migrations, copy [`alembic.sample.ini`](./alembic.sample.ini) to a separate file
-        (e.g. `./secrets/alembic.dev.ini`) and modify the `sqlalchemy.url` setting in the new file to point
-        at your database.
-        
-        Make sure your database is at the latest alembic migration:
-        
-        ```bash
-        alembic -c ./secrets/alembic.dev.ini upgrade head
-        ```
-        
-        ### Adding a new table to database
-        
-        Add SQLAlchemy model in [`moonstreamdb/models.py`](./moonstreamdb/models.py)
-        
-        Import new model and add tablename to whitelist in [`alembic/env.py`](.alembic/env.py)
-        
-        Create a migration:
-        
-        ```bash
-        alembic -c <alembic config file> revision -m "<revision message>" --autogenerate
-        ```
-        
-        Always check the autogenerated file to make sure that it isn't performing any actions that you don't want it to.
-        A good policy is to delete any operations that don't touch the tables that you created.
-        
-        Then run the migration:
-        
-        ```bash
-        alembic -c <alembic config file> upgrade head
-        ```
-        
 Platform: all
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: distribute
+
+# moonstream db
+
+### Setting up moonstreamdb
+
+Copy `sample.env` to a new file and set the environment variables to appropriate values. This new file
+should be sourced every time you want to access the database with the `moonstreamdb` application or any
+dependents.
+
+To be able to run migrations, copy [`alembic.sample.ini`](./alembic.sample.ini) to a separate file
+(e.g. `./secrets/alembic.dev.ini`) and modify the `sqlalchemy.url` setting in the new file to point
+at your database.
+
+Make sure your database is at the latest alembic migration:
+
+```bash
+alembic -c ./secrets/alembic.dev.ini upgrade head
+```
+
+### Adding a new table to database
+
+Add SQLAlchemy model in [`moonstreamdb/models.py`](./moonstreamdb/models.py)
+
+Import new model and add tablename to whitelist in [`alembic/env.py`](.alembic/env.py)
+
+Create a migration:
+
+```bash
+alembic -c <alembic config file> revision -m "<revision message>" --autogenerate
+```
+
+Always check the autogenerated file to make sure that it isn't performing any actions that you don't want it to.
+A good policy is to delete any operations that don't touch the tables that you created.
+
+Then run the migration:
+
+```bash
+alembic -c <alembic config file> upgrade head
+```
```

### Comparing `moonstreamdb-0.3.3/README.md` & `moonstreamdb-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `moonstreamdb-0.3.3/moonstreamdb/blockchain.py` & `moonstreamdb-0.3.4/moonstreamdb/blockchain.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,85 +1,123 @@
-from .db import yield_db_session, yield_db_session_ctx
+from enum import Enum
+from typing import Type, Union
+
 from .models import (
     EthereumBlock,
     EthereumLabel,
     EthereumTransaction,
-    PolygonBlock,
-    PolygonLabel,
-    PolygonTransaction,
     MumbaiBlock,
     MumbaiLabel,
     MumbaiTransaction,
-    XDaiBlock,
-    XDaiLabel,
-    XDaiTransaction,
+    PolygonBlock,
+    PolygonLabel,
+    PolygonTransaction,
     WyrmBlock,
     WyrmLabel,
     WyrmTransaction,
+    XDaiBlock,
+    XDaiLabel,
+    XDaiTransaction,
+    ZkSyncEraTestnetBlock,
+    ZkSyncEraTestnetLabel,
+    ZkSyncEraTestnetTransaction,
 )
 
-from enum import Enum
-
-from typing import Type, Union
-
 
 class AvailableBlockchainType(Enum):
     ETHEREUM = "ethereum"
     POLYGON = "polygon"
     MUMBAI = "mumbai"
     XDAI = "xdai"
     WYRM = "wyrm"
+    ZKSYNC_ERA_TESTNET = "zksync_era_testnet"
 
 
 def get_block_model(
     blockchain_type: AvailableBlockchainType,
-) -> Type[Union[EthereumBlock, PolygonBlock, MumbaiBlock, XDaiBlock, WyrmBlock]]:
+) -> Type[
+    Union[
+        EthereumBlock,
+        PolygonBlock,
+        MumbaiBlock,
+        XDaiBlock,
+        WyrmBlock,
+        ZkSyncEraTestnetBlock,
+    ]
+]:
     """
     Depends on provided blockchain type: Ethereum, Polygon, Mumbai, XDai, Wyrm
     set proper blocks model.
     """
     block_model: Type[
-        Union[EthereumBlock, PolygonBlock, MumbaiBlock, XDaiBlock, WyrmBlock]
+        Union[
+            EthereumBlock,
+            PolygonBlock,
+            MumbaiBlock,
+            XDaiBlock,
+            WyrmBlock,
+            ZkSyncEraTestnetBlock,
+        ]
     ]
     if blockchain_type == AvailableBlockchainType.ETHEREUM:
         block_model = EthereumBlock
     elif blockchain_type == AvailableBlockchainType.POLYGON:
         block_model = PolygonBlock
     elif blockchain_type == AvailableBlockchainType.MUMBAI:
         block_model = MumbaiBlock
     elif blockchain_type == AvailableBlockchainType.XDAI:
         block_model = XDaiBlock
     elif blockchain_type == AvailableBlockchainType.WYRM:
         block_model = WyrmBlock
+    elif blockchain_type == AvailableBlockchainType.ZKSYNC_ERA_TESTNET:
+        block_model = ZkSyncEraTestnetBlock
     else:
         raise Exception("Unsupported blockchain type provided")
 
     return block_model
 
 
 def get_label_model(
     blockchain_type: AvailableBlockchainType,
-) -> Type[Union[EthereumLabel, PolygonLabel, MumbaiLabel, XDaiLabel, WyrmLabel]]:
+) -> Type[
+    Union[
+        EthereumLabel,
+        PolygonLabel,
+        MumbaiLabel,
+        XDaiLabel,
+        WyrmLabel,
+        ZkSyncEraTestnetLabel,
+    ]
+]:
     """
     Depends on provided blockchain type: Ethereum, Polygon, Mumbai, XDai, Wyrm
     set proper block label model.
     """
     label_model: Type[
-        Union[EthereumLabel, PolygonLabel, MumbaiLabel, XDaiLabel, WyrmLabel]
+        Union[
+            EthereumLabel,
+            PolygonLabel,
+            MumbaiLabel,
+            XDaiLabel,
+            WyrmLabel,
+            ZkSyncEraTestnetLabel,
+        ]
     ]
     if blockchain_type == AvailableBlockchainType.ETHEREUM:
         label_model = EthereumLabel
     elif blockchain_type == AvailableBlockchainType.POLYGON:
         label_model = PolygonLabel
     elif blockchain_type == AvailableBlockchainType.MUMBAI:
         label_model = MumbaiLabel
     elif blockchain_type == AvailableBlockchainType.XDAI:
         label_model = XDaiLabel
     elif blockchain_type == AvailableBlockchainType.WYRM:
         label_model = WyrmLabel
+    elif blockchain_type == AvailableBlockchainType.ZKSYNC_ERA_TESTNET:
+        label_model = ZkSyncEraTestnetLabel
     else:
         raise Exception("Unsupported blockchain type provided")
 
     return label_model
 
 
 def get_transaction_model(
@@ -87,36 +125,40 @@
 ) -> Type[
     Union[
         EthereumTransaction,
         PolygonTransaction,
         MumbaiTransaction,
         XDaiTransaction,
         WyrmTransaction,
+        ZkSyncEraTestnetTransaction,
     ]
 ]:
     """
     Depends on provided blockchain type: Ethereum, Polygon, Mumbai, XDai, Wyrm
     set proper block transactions model.
     """
     transaction_model: Type[
         Union[
             EthereumTransaction,
             PolygonTransaction,
             MumbaiTransaction,
             XDaiTransaction,
             WyrmTransaction,
+            ZkSyncEraTestnetTransaction,
         ]
     ]
     if blockchain_type == AvailableBlockchainType.ETHEREUM:
         transaction_model = EthereumTransaction
     elif blockchain_type == AvailableBlockchainType.POLYGON:
         transaction_model = PolygonTransaction
     elif blockchain_type == AvailableBlockchainType.MUMBAI:
         transaction_model = MumbaiTransaction
     elif blockchain_type == AvailableBlockchainType.XDAI:
         transaction_model = XDaiTransaction
     elif blockchain_type == AvailableBlockchainType.WYRM:
         transaction_model = WyrmTransaction
+    elif blockchain_type == AvailableBlockchainType.ZKSYNC_ERA_TESTNET:
+        transaction_model = ZkSyncEraTestnetTransaction
     else:
         raise Exception("Unsupported blockchain type provided")
 
     return transaction_model
```

### Comparing `moonstreamdb-0.3.3/moonstreamdb/cli.py` & `moonstreamdb-0.3.4/moonstreamdb/cli.py`

 * *Files identical despite different names*

### Comparing `moonstreamdb-0.3.3/moonstreamdb/db.py` & `moonstreamdb-0.3.4/moonstreamdb/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Moonstream database connection.
 """
-from contextlib import contextmanager
 import os
+from contextlib import contextmanager
 from typing import Generator
 
 from sqlalchemy import create_engine
-from sqlalchemy.orm import sessionmaker, Session
+from sqlalchemy.orm import Session, sessionmaker
 
 MOONSTREAM_DB_URI = os.environ.get("MOONSTREAM_DB_URI")
 if MOONSTREAM_DB_URI is None:
     raise ValueError("MOONSTREAM_DB_URI environment variable must be set")
 
 MOONSTREAM_DB_URI_READ_ONLY = os.environ.get("MOONSTREAM_DB_URI_READ_ONLY")
 if MOONSTREAM_DB_URI_READ_ONLY is None:
```

### Comparing `moonstreamdb-0.3.3/moonstreamdb/models.py` & `moonstreamdb-0.3.4/moonstreamdb/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import uuid
 
-from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy import (
+    VARCHAR,
     BigInteger,
     Column,
     DateTime,
+    ForeignKey,
     Index,
     Integer,
-    ForeignKey,
     MetaData,
     Numeric,
     Text,
-    VARCHAR,
 )
 from sqlalchemy.dialects.postgresql import JSONB, UUID
-from sqlalchemy.sql import expression
 from sqlalchemy.ext.compiler import compiles
+from sqlalchemy.ext.declarative import declarative_base
+from sqlalchemy.sql import expression
 
 """
 Naming conventions doc
 https://docs.sqlalchemy.org/en/13/core/constraints.html#configuring-constraint-naming-conventions
 """
 convention = {
     "ix": "ix_%(column_0_label)s",
@@ -580,14 +580,145 @@
             "address",
             "block_timestamp",
             unique=False,
         ),
     )
 
     id = Column(
+        UUID(as_uuid=True),
+        primary_key=True,
+        default=uuid.uuid4,
+        unique=True,
+        nullable=False,
+    )
+    label = Column(VARCHAR(256), nullable=False, index=True)
+    block_number = Column(
+        BigInteger,
+        nullable=True,
+        index=True,
+    )
+    address = Column(
+        VARCHAR(256),
+        nullable=True,
+        index=True,
+    )
+    transaction_hash = Column(
+        VARCHAR(256),
+        nullable=True,
+        index=True,
+    )
+    label_data = Column(JSONB, nullable=True)
+    block_timestamp = Column(BigInteger, index=True)
+    log_index = Column(Integer, nullable=True)
+    created_at = Column(
+        DateTime(timezone=True), server_default=utcnow(), nullable=False
+    )
+
+
+class ZkSyncEraTestnetBlock(Base):  # type: ignore
+    __tablename__ = "zksync_era_testnet_blocks"
+
+    block_number = Column(
+        BigInteger, primary_key=True, unique=True, nullable=False, index=True
+    )
+    difficulty = Column(BigInteger)
+    extra_data = Column(VARCHAR(128))
+    gas_limit = Column(BigInteger)
+    gas_used = Column(BigInteger)
+    base_fee_per_gas = Column(Numeric(precision=78, scale=0), nullable=True)
+    hash = Column(VARCHAR(256), index=True)
+    logs_bloom = Column(VARCHAR(1024))
+    miner = Column(VARCHAR(256))
+    nonce = Column(VARCHAR(256))
+    parent_hash = Column(VARCHAR(256))
+    receipt_root = Column(VARCHAR(256))
+    uncles = Column(VARCHAR(256))
+    size = Column(Integer)
+    state_root = Column(VARCHAR(256))
+    timestamp = Column(BigInteger, index=True)
+    total_difficulty = Column(VARCHAR(256))
+    transactions_root = Column(VARCHAR(256))
+
+    indexed_at = Column(
+        DateTime(timezone=True), server_default=utcnow(), nullable=False
+    )
+
+    mix_hash = Column(VARCHAR(256), nullable=True)
+    sha3_uncles = Column(VARCHAR(256), nullable=True)
+
+    l1_batch_number = Column(BigInteger, nullable=True)
+    l1_batch_timestamp = Column(BigInteger, nullable=True)
+
+
+class ZkSyncEraTestnetTransaction(Base):  # type: ignore
+    __tablename__ = "zksync_era_testnet_transactions"
+
+    hash = Column(
+        VARCHAR(256), primary_key=True, unique=True, nullable=False, index=True
+    )
+    block_number = Column(
+        BigInteger,
+        ForeignKey("zksync_era_testnet_blocks.block_number", ondelete="CASCADE"),
+        nullable=False,
+        index=True,
+    )
+    from_address = Column(VARCHAR(256), index=True)
+    to_address = Column(VARCHAR(256), index=True)
+    gas = Column(Numeric(precision=78, scale=0), index=True)
+    gas_price = Column(Numeric(precision=78, scale=0), index=True)
+    max_fee_per_gas = Column(Numeric(precision=78, scale=0), nullable=True)
+    max_priority_fee_per_gas = Column(Numeric(precision=78, scale=0), nullable=True)
+    input = Column(Text)
+    nonce = Column(VARCHAR(256))
+    transaction_index = Column(BigInteger)
+    transaction_type = Column(Integer, nullable=True)
+    value = Column(Numeric(precision=78, scale=0), index=True)
+
+    indexed_at = Column(
+        DateTime(timezone=True), server_default=utcnow(), nullable=False
+    )
+
+    l1_batch_number = Column(BigInteger, nullable=True)
+    l1_batch_tx_index = Column(BigInteger, nullable=True)
+
+
+class ZkSyncEraTestnetLabel(Base):  # type: ignore
+    """
+    Example of label_data:
+        {
+            "label": "ERC20",
+            "label_data": {
+                "name": "Uniswap",
+                "symbol": "UNI"
+            }
+        },
+        {
+            "label": "Exchange"
+            "label_data": {...}
+        }
+    """
+
+    __tablename__ = "zksync_era_testnet_labels"
+
+    __table_args__ = (
+        Index(
+            "ix_zksync_era_testnet_labels_address_block_number",
+            "address",
+            "block_number",
+            unique=False,
+        ),
+        Index(
+            "ix_zksync_era_testnet_labels_address_block_timestamp",
+            "address",
+            "block_timestamp",
+            unique=False,
+        ),
+    )
+
+    id = Column(
         UUID(as_uuid=True),
         primary_key=True,
         default=uuid.uuid4,
         unique=True,
         nullable=False,
     )
     label = Column(VARCHAR(256), nullable=False, index=True)
```

### Comparing `moonstreamdb-0.3.3/moonstreamdb/networks.py` & `moonstreamdb-0.3.4/moonstreamdb/networks.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,31 +14,36 @@
     PolygonTransaction,
     WyrmBlock,
     WyrmLabel,
     WyrmTransaction,
     XDaiBlock,
     XDaiLabel,
     XDaiTransaction,
+    ZkSyncEraTestnetBlock,
+    ZkSyncEraTestnetLabel,
+    ZkSyncEraTestnetTransaction,
 )
 
 
 class Network(Enum):
     ethereum = "ethereum"
     polygon = "polygon"
     mumbai = "mumbai"
     xdai = "xdai"
     wyrm = "wyrm"
+    zksync_era_testnet = "zksync_era_testnet"
 
 
 tx_raw_types = Union[
     EthereumTransaction,
     MumbaiTransaction,
     PolygonTransaction,
     WyrmTransaction,
     XDaiTransaction,
+    ZkSyncEraTestnetTransaction,
 ]
 
 MODELS: Dict[Network, Dict[str, Base]] = {
     Network.ethereum: {
         "blocks": EthereumBlock,
         "labels": EthereumLabel,
         "transactions": EthereumTransaction,
@@ -59,8 +64,13 @@
         "transactions": XDaiTransaction,
     },
     Network.wyrm: {
         "blocks": WyrmBlock,
         "labels": WyrmLabel,
         "transactions": WyrmTransaction,
     },
+    Network.zksync_era_testnet: {
+        "blocks": ZkSyncEraTestnetBlock,
+        "labels": ZkSyncEraTestnetLabel,
+        "transactions": ZkSyncEraTestnetTransaction,
+    },
 }
```

### Comparing `moonstreamdb-0.3.3/moonstreamdb.egg-info/PKG-INFO` & `moonstreamdb-0.3.4/moonstreamdb.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 Metadata-Version: 2.1
 Name: moonstreamdb
-Version: 0.3.3
+Version: 0.3.4
 Summary: Moonstream database
 Home-page: https://github.com/bugout-dev/moonstream
 Author: Bugout.dev
 Author-email: engineers@bugout.dev
 License: Apache License 2.0
-Description: # moonstream db
-        
-        ### Setting up moonstreamdb
-        
-        Copy `sample.env` to a new file and set the environment variables to appropriate values. This new file
-        should be sourced every time you want to access the database with the `moonstreamdb` application or any
-        dependents.
-        
-        To be able to run migrations, copy [`alembic.sample.ini`](./alembic.sample.ini) to a separate file
-        (e.g. `./secrets/alembic.dev.ini`) and modify the `sqlalchemy.url` setting in the new file to point
-        at your database.
-        
-        Make sure your database is at the latest alembic migration:
-        
-        ```bash
-        alembic -c ./secrets/alembic.dev.ini upgrade head
-        ```
-        
-        ### Adding a new table to database
-        
-        Add SQLAlchemy model in [`moonstreamdb/models.py`](./moonstreamdb/models.py)
-        
-        Import new model and add tablename to whitelist in [`alembic/env.py`](.alembic/env.py)
-        
-        Create a migration:
-        
-        ```bash
-        alembic -c <alembic config file> revision -m "<revision message>" --autogenerate
-        ```
-        
-        Always check the autogenerated file to make sure that it isn't performing any actions that you don't want it to.
-        A good policy is to delete any operations that don't touch the tables that you created.
-        
-        Then run the migration:
-        
-        ```bash
-        alembic -c <alembic config file> upgrade head
-        ```
-        
 Platform: all
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: distribute
+
+# moonstream db
+
+### Setting up moonstreamdb
+
+Copy `sample.env` to a new file and set the environment variables to appropriate values. This new file
+should be sourced every time you want to access the database with the `moonstreamdb` application or any
+dependents.
+
+To be able to run migrations, copy [`alembic.sample.ini`](./alembic.sample.ini) to a separate file
+(e.g. `./secrets/alembic.dev.ini`) and modify the `sqlalchemy.url` setting in the new file to point
+at your database.
+
+Make sure your database is at the latest alembic migration:
+
+```bash
+alembic -c ./secrets/alembic.dev.ini upgrade head
+```
+
+### Adding a new table to database
+
+Add SQLAlchemy model in [`moonstreamdb/models.py`](./moonstreamdb/models.py)
+
+Import new model and add tablename to whitelist in [`alembic/env.py`](.alembic/env.py)
+
+Create a migration:
+
+```bash
+alembic -c <alembic config file> revision -m "<revision message>" --autogenerate
+```
+
+Always check the autogenerated file to make sure that it isn't performing any actions that you don't want it to.
+A good policy is to delete any operations that don't touch the tables that you created.
+
+Then run the migration:
+
+```bash
+alembic -c <alembic config file> upgrade head
+```
```

### Comparing `moonstreamdb-0.3.3/setup.py` & `moonstreamdb-0.3.4/setup.py`

 * *Files identical despite different names*

