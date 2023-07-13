# Comparing `tmp/seedwork_python-0.2.0.tar.gz` & `tmp/seedwork_python-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seedwork_python-0.2.0.tar", max compression
+gzip compressed data, was "seedwork_python-0.3.0.tar", max compression
```

## Comparing `seedwork_python-0.2.0.tar` & `seedwork_python-0.3.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1066 2023-07-08 14:25:12.259881 seedwork_python-0.2.0/LICENSE
--rw-r--r--   0        0        0      373 2021-07-16 00:27:15.175286 seedwork_python-0.2.0/README.md
--rw-r--r--   0        0        0     1667 2023-07-12 03:07:09.478712 seedwork_python-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-04 14:12:17.070490 seedwork_python-0.2.0/seedwork/__init__.py
--rw-r--r--   0        0        0       52 2023-07-07 11:49:36.263799 seedwork_python-0.2.0/seedwork/application/__init__.py
--rw-r--r--   0        0        0      115 2023-07-08 05:10:39.020400 seedwork_python-0.2.0/seedwork/application/command.py
--rw-r--r--   0        0        0      195 2023-07-04 00:24:30.486852 seedwork_python-0.2.0/seedwork/domain/__init__.py
--rw-r--r--   0        0        0      237 2023-07-08 12:38:37.709567 seedwork_python-0.2.0/seedwork/domain/aggregate_root.py
--rw-r--r--   0        0        0     1112 2023-07-08 12:40:08.210080 seedwork_python-0.2.0/seedwork/domain/entity.py
--rw-r--r--   0        0        0      496 2023-07-03 11:32:45.559964 seedwork_python-0.2.0/seedwork/domain/enumeration.py
--rw-r--r--   0        0        0      102 2023-07-03 11:32:45.560059 seedwork_python-0.2.0/seedwork/domain/event.py
--rw-r--r--   0        0        0        0 2023-07-08 11:20:04.255707 seedwork_python-0.2.0/seedwork/domain/repository/__init__.py
--rw-r--r--   0        0        0     1199 2023-07-12 02:56:35.068004 seedwork_python-0.2.0/seedwork/domain/repository/generic.py
--rw-r--r--   0        0        0      202 2023-07-08 11:13:57.483175 seedwork_python-0.2.0/seedwork/domain/repository/repository.py
--rw-r--r--   0        0        0      702 2023-07-05 11:09:01.743339 seedwork_python-0.2.0/seedwork/domain/unit_of_work.py
--rw-r--r--   0        0        0      114 2023-07-03 11:32:45.560142 seedwork_python-0.2.0/seedwork/domain/value_object.py
--rw-r--r--   0        0        0        0 2023-07-06 11:16:26.140518 seedwork_python-0.2.0/seedwork/infrastructure/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 13:03:28.615076 seedwork_python-0.2.0/seedwork/infrastructure/cache/__init__.py
--rw-r--r--   0        0        0      275 2023-07-12 00:46:02.079133 seedwork_python-0.2.0/seedwork/infrastructure/cache/cache.py
--rw-r--r--   0        0        0     6024 2023-07-12 00:46:01.737856 seedwork_python-0.2.0/seedwork/infrastructure/cache/r.py
--rw-r--r--   0        0        0     1226 2023-07-12 00:46:02.082123 seedwork_python-0.2.0/seedwork/infrastructure/cache/redis.py
--rw-r--r--   0        0        0       49 2023-07-07 12:26:02.202328 seedwork_python-0.2.0/seedwork/infrastructure/logging/__init__.py
--rw-r--r--   0        0        0      149 2023-07-07 12:46:45.930202 seedwork_python-0.2.0/seedwork/infrastructure/logging/logger.py
--rw-r--r--   0        0        0        0 2023-07-06 11:16:26.140575 seedwork_python-0.2.0/seedwork/infrastructure/persistence/__init__.py
--rw-r--r--   0        0        0      247 2023-07-12 03:06:40.868222 seedwork_python-0.2.0/seedwork/infrastructure/persistence/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      966 2023-07-12 02:56:35.063869 seedwork_python-0.2.0/seedwork/infrastructure/persistence/sqlalchemy/generic.py
--rw-r--r--   0        0        0      191 2023-07-06 11:16:26.140773 seedwork_python-0.2.0/seedwork/infrastructure/persistence/sqlalchemy/repository.py
--rw-r--r--   0        0        0      933 2023-07-06 11:16:26.140861 seedwork_python-0.2.0/seedwork/infrastructure/persistence/sqlalchemy/unit_of_work.py
--rw-r--r--   0        0        0        0 2023-07-09 00:50:53.962442 seedwork_python-0.2.0/seedwork/py.typed
--rw-r--r--   0        0        0      318 2023-07-08 12:13:02.552819 seedwork_python-0.2.0/seedwork/typings.py
--rw-r--r--   0        0        0     1280 1970-01-01 00:00:00.000000 seedwork_python-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-08 14:25:12.259881 seedwork_python-0.3.0/LICENSE
+-rw-r--r--   0        0        0      373 2021-07-16 00:27:15.175286 seedwork_python-0.3.0/README.md
+-rw-r--r--   0        0        0     1667 2023-07-13 00:17:21.456971 seedwork_python-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-04 14:12:17.070490 seedwork_python-0.3.0/seedwork/__init__.py
+-rw-r--r--   0        0        0       52 2023-07-07 11:49:36.263799 seedwork_python-0.3.0/seedwork/application/__init__.py
+-rw-r--r--   0        0        0      115 2023-07-08 05:10:39.020400 seedwork_python-0.3.0/seedwork/application/command.py
+-rw-r--r--   0        0        0      195 2023-07-04 00:24:30.486852 seedwork_python-0.3.0/seedwork/domain/__init__.py
+-rw-r--r--   0        0        0      237 2023-07-08 12:38:37.709567 seedwork_python-0.3.0/seedwork/domain/aggregate_root.py
+-rw-r--r--   0        0        0     1112 2023-07-08 12:40:08.210080 seedwork_python-0.3.0/seedwork/domain/entity.py
+-rw-r--r--   0        0        0      496 2023-07-03 11:32:45.559964 seedwork_python-0.3.0/seedwork/domain/enumeration.py
+-rw-r--r--   0        0        0      102 2023-07-03 11:32:45.560059 seedwork_python-0.3.0/seedwork/domain/event.py
+-rw-r--r--   0        0        0        0 2023-07-08 11:20:04.255707 seedwork_python-0.3.0/seedwork/domain/repository/__init__.py
+-rw-r--r--   0        0        0     1199 2023-07-12 02:56:35.068004 seedwork_python-0.3.0/seedwork/domain/repository/generic.py
+-rw-r--r--   0        0        0      202 2023-07-08 11:13:57.483175 seedwork_python-0.3.0/seedwork/domain/repository/repository.py
+-rw-r--r--   0        0        0      531 2023-07-12 12:58:06.029998 seedwork_python-0.3.0/seedwork/domain/unit_of_work.py
+-rw-r--r--   0        0        0      114 2023-07-03 11:32:45.560142 seedwork_python-0.3.0/seedwork/domain/value_object.py
+-rw-r--r--   0        0        0        0 2023-07-06 11:16:26.140518 seedwork_python-0.3.0/seedwork/infrastructure/__init__.py
+-rw-r--r--   0        0        0        2 2023-07-13 00:17:10.022932 seedwork_python-0.3.0/seedwork/infrastructure/cache/__init__.py
+-rw-r--r--   0        0        0      275 2023-07-12 00:46:02.079133 seedwork_python-0.3.0/seedwork/infrastructure/cache/cache.py
+-rw-r--r--   0        0        0     6024 2023-07-12 00:46:01.737856 seedwork_python-0.3.0/seedwork/infrastructure/cache/r.py
+-rw-r--r--   0        0        0     1226 2023-07-12 00:46:02.082123 seedwork_python-0.3.0/seedwork/infrastructure/cache/redis.py
+-rw-r--r--   0        0        0       49 2023-07-07 12:26:02.202328 seedwork_python-0.3.0/seedwork/infrastructure/logging/__init__.py
+-rw-r--r--   0        0        0      149 2023-07-07 12:46:45.930202 seedwork_python-0.3.0/seedwork/infrastructure/logging/logger.py
+-rw-r--r--   0        0        0        0 2023-07-06 11:16:26.140575 seedwork_python-0.3.0/seedwork/infrastructure/persistence/__init__.py
+-rw-r--r--   0        0        0      247 2023-07-12 03:06:40.868222 seedwork_python-0.3.0/seedwork/infrastructure/persistence/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      966 2023-07-12 02:56:35.063869 seedwork_python-0.3.0/seedwork/infrastructure/persistence/sqlalchemy/generic.py
+-rw-r--r--   0        0        0      191 2023-07-06 11:16:26.140773 seedwork_python-0.3.0/seedwork/infrastructure/persistence/sqlalchemy/repository.py
+-rw-r--r--   0        0        0      980 2023-07-12 12:58:53.466985 seedwork_python-0.3.0/seedwork/infrastructure/persistence/sqlalchemy/unit_of_work.py
+-rw-r--r--   0        0        0        0 2023-07-09 00:50:53.962442 seedwork_python-0.3.0/seedwork/py.typed
+-rw-r--r--   0        0        0      318 2023-07-08 12:13:02.552819 seedwork_python-0.3.0/seedwork/typings.py
+-rw-r--r--   0        0        0     1280 1970-01-01 00:00:00.000000 seedwork_python-0.3.0/PKG-INFO
```

### Comparing `seedwork_python-0.2.0/LICENSE` & `seedwork_python-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seedwork_python-0.2.0/pyproject.toml` & `seedwork_python-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seedwork-python"
-version = "0.2.0"
+version = "0.3.0"
 description = "Python seedwork library."
 license = "MIT"
 authors = ["Huang Kai <h1770360848@outlook.com>"]
 maintainers = ["Huang Kai <h1770360848@outlook.com>"]
 readme = "README.md"
 repository = "https://github.com/Huangkai1008/seedwork-python"
 classifiers = [
```

### Comparing `seedwork_python-0.2.0/seedwork/domain/entity.py` & `seedwork_python-0.3.0/seedwork/domain/entity.py`

 * *Files identical despite different names*

### Comparing `seedwork_python-0.2.0/seedwork/domain/repository/generic.py` & `seedwork_python-0.3.0/seedwork/domain/repository/generic.py`

 * *Files identical despite different names*

### Comparing `seedwork_python-0.2.0/seedwork/domain/unit_of_work.py` & `seedwork_python-0.3.0/seedwork/domain/unit_of_work.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,26 @@
-from abc import ABC, abstractmethod
 from traceback import TracebackException
-from typing import Optional
+from typing import Optional, Protocol, runtime_checkable
 
 from typing_extensions import Self
 
-__all__ = ['AbstractUnitOfWork']
+__all__ = ['IUnitOfWork']
 
 
-class AbstractUnitOfWork(ABC):
+@runtime_checkable
+class IUnitOfWork(Protocol):
     def commit(self) -> None:
-        self._commit()
-
-    def rollback(self) -> None:
-        self._rollback()
-
-    @abstractmethod
-    def _commit(self) -> None:
         ...
 
-    @abstractmethod
-    def _rollback(self) -> None:
+    def rollback(self) -> None:
         ...
 
     def __enter__(self) -> Self:
-        return self
+        ...
 
     def __exit__(
         self,
         exc_type: Optional[type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: TracebackException,
     ) -> None:
-        self.rollback()
+        ...
```

### Comparing `seedwork_python-0.2.0/seedwork/infrastructure/cache/r.py` & `seedwork_python-0.3.0/seedwork/infrastructure/cache/r.py`

 * *Files identical despite different names*

### Comparing `seedwork_python-0.2.0/seedwork/infrastructure/cache/redis.py` & `seedwork_python-0.3.0/seedwork/infrastructure/cache/redis.py`

 * *Files identical despite different names*

### Comparing `seedwork_python-0.2.0/seedwork/infrastructure/persistence/sqlalchemy/generic.py` & `seedwork_python-0.3.0/seedwork/infrastructure/persistence/sqlalchemy/generic.py`

 * *Files identical despite different names*

### Comparing `seedwork_python-0.2.0/seedwork/infrastructure/persistence/sqlalchemy/unit_of_work.py` & `seedwork_python-0.3.0/seedwork/infrastructure/persistence/sqlalchemy/unit_of_work.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 from traceback import TracebackException
 from typing import Optional
 
 from sqlalchemy.orm import Session, sessionmaker
 from typing_extensions import Self
 
-from seedwork.domain.unit_of_work import AbstractUnitOfWork
-
 __all__ = ['SQLAlchemyUnitOfWork']
 
 
-class SQLAlchemyUnitOfWork(AbstractUnitOfWork):
+class SQLAlchemyUnitOfWork:
+    """SQLAlchemy unit of work implementation."""
+
     def __init__(self, session_factory: sessionmaker) -> None:
         self.session_factory: sessionmaker = session_factory
 
-    def _commit(self) -> None:
-        self.session.commit()
+    def commit(self) -> None:
+        self._commit()
 
-    def _rollback(self) -> None:
-        self.session.rollback()
+    def rollback(self) -> None:
+        self._rollback()
 
     def __enter__(self) -> Self:
         self.session: Session = self.session_factory()
-        return super().__enter__()
+        return self
 
     def __exit__(
         self,
         exc_type: Optional[type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: TracebackException,
     ) -> None:
-        super().__exit__(exc_type, exc_val, exc_tb)
+        self.session.rollback()
         self.session.close()
+
+    def _commit(self) -> None:
+        self.session.commit()
+
+    def _rollback(self) -> None:
+        self.session.rollback()
```

### Comparing `seedwork_python-0.2.0/PKG-INFO` & `seedwork_python-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seedwork-python
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python seedwork library.
 Home-page: https://github.com/Huangkai1008/seedwork-python
 License: MIT
 Author: Huang Kai
 Author-email: h1770360848@outlook.com
 Maintainer: Huang Kai
 Maintainer-email: h1770360848@outlook.com
```

