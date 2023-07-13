# Comparing `tmp/fps_auth-0.1.9.tar.gz` & `tmp/fps_auth-0.2.0.tar.gz`

## Comparing `fps_auth-0.1.9.tar` & `fps_auth-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_auth-0.1.9/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_auth-0.1.9/fps_auth/__init__.py
--rw-r--r--   0        0        0    11596 2020-02-02 00:00:00.000000 fps_auth-0.1.9/fps_auth/backends.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 fps_auth-0.1.9/fps_auth/config.py
--rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 fps_auth-0.1.9/fps_auth/db.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 fps_auth-0.1.9/fps_auth/main.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fps_auth-0.1.9/fps_auth/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_auth-0.1.9/fps_auth/py.typed
--rw-r--r--   0        0        0     7820 2020-02-02 00:00:00.000000 fps_auth-0.1.9/fps_auth/routes.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_auth-0.1.9/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_auth-0.1.9/COPYING.md
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 fps_auth-0.1.9/README.md
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 fps_auth-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 fps_auth-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_auth-0.2.0/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_auth-0.2.0/fps_auth/__init__.py
+-rw-r--r--   0        0        0    11618 2020-02-02 00:00:00.000000 fps_auth-0.2.0/fps_auth/backends.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 fps_auth-0.2.0/fps_auth/config.py
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 fps_auth-0.2.0/fps_auth/db.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 fps_auth-0.2.0/fps_auth/main.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fps_auth-0.2.0/fps_auth/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_auth-0.2.0/fps_auth/py.typed
+-rw-r--r--   0        0        0     7820 2020-02-02 00:00:00.000000 fps_auth-0.2.0/fps_auth/routes.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_auth-0.2.0/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_auth-0.2.0/COPYING.md
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 fps_auth-0.2.0/README.md
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 fps_auth-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 fps_auth-0.2.0/PKG-INFO
```

### Comparing `fps_auth-0.1.9/fps_auth/backends.py` & `fps_auth-0.2.0/fps_auth/backends.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         get_strategy=get_jwt_strategy,
     )
 
     github_authentication = GitHubOAuth2(auth_config.client_id, auth_config.client_secret)
 
     class UserManager(UUIDIDMixin, BaseUserManager[User, uuid.UUID]):
         async def on_after_register(self, user: User, request: Optional[Request] = None):
-            for oauth_account in user.oauth_accounts:
+            for oauth_account in await user.awaitable_attrs.oauth_accounts:
                 if oauth_account.oauth_name == "github":
                     async with httpx.AsyncClient() as client:
                         r = (
                             await client.get(
                                 f"https://api.github.com/user/{oauth_account.account_id}"
                             )
                         ).json()
```

### Comparing `fps_auth-0.1.9/fps_auth/config.py` & `fps_auth-0.2.0/fps_auth/config.py`

 * *Files identical despite different names*

### Comparing `fps_auth-0.1.9/fps_auth/db.py` & `fps_auth-0.2.0/fps_auth/db.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,44 +6,44 @@
 
 from fastapi import Depends
 from fastapi_users.db import SQLAlchemyBaseOAuthAccountTableUUID
 from fastapi_users.db import (
     SQLAlchemyBaseUserTableUUID,
     SQLAlchemyUserDatabase,
 )
-from sqlalchemy import JSON, Boolean, Column, String, Text  # type: ignore
-from sqlalchemy.ext.asyncio import AsyncSession, create_async_engine  # type: ignore
-from sqlalchemy.ext.declarative import DeclarativeMeta, declarative_base  # type: ignore
-from sqlalchemy.orm import relationship, sessionmaker  # type: ignore
+from sqlalchemy import JSON, Boolean, Column, String, Text
+from sqlalchemy.ext.asyncio import AsyncAttrs, AsyncSession, async_sessionmaker, create_async_engine
+from sqlalchemy.orm import DeclarativeBase, Mapped, relationship
 
 from .config import _AuthConfig
 
 
 logger = logging.getLogger("auth")
 
-Base: DeclarativeMeta = declarative_base()
+
+class Base(AsyncAttrs, DeclarativeBase):
+    pass
 
 
 class OAuthAccount(SQLAlchemyBaseOAuthAccountTableUUID, Base):
     pass
 
 
 class User(SQLAlchemyBaseUserTableUUID, Base):
     anonymous = Column(Boolean, default=True, nullable=False)
-    email = Column(String(length=32), nullable=False, unique=True)
     username = Column(String(length=32), nullable=False, unique=True)
     name = Column(String(length=32), default="")
     display_name = Column(String(length=32), default="")
     initials = Column(String(length=8), nullable=True)
     color = Column(String(length=32), nullable=True)
     avatar_url = Column(String(length=32), nullable=True)
     workspace = Column(Text(), default="{}", nullable=False)
     settings = Column(Text(), default="{}", nullable=False)
     permissions = Column(JSON, default={}, nullable=False)
-    oauth_accounts: List[OAuthAccount] = relationship("OAuthAccount", lazy="joined")
+    oauth_accounts: Mapped[List[OAuthAccount]] = relationship("OAuthAccount", lazy="joined")
 
 
 @dataclass
 class Res:
     User: Any
     async_session_maker: Any
     create_db_and_tables: Any
@@ -78,15 +78,15 @@
         secret_path.write_text(secrets.token_hex(32))
 
     secret = secret_path.read_text()
 
     database_url = f"sqlite+aiosqlite:///{userdb_path}"
 
     engine = create_async_engine(database_url)
-    async_session_maker = sessionmaker(engine, class_=AsyncSession, expire_on_commit=False)
+    async_session_maker = async_sessionmaker(engine, expire_on_commit=False)
 
     async def create_db_and_tables():
         async with engine.begin() as conn:
             await conn.run_sync(Base.metadata.create_all)
 
     async def get_async_session() -> AsyncGenerator[AsyncSession, None]:
         async with async_session_maker() as session:
```

### Comparing `fps_auth-0.1.9/fps_auth/main.py` & `fps_auth-0.2.0/fps_auth/main.py`

 * *Files identical despite different names*

### Comparing `fps_auth-0.1.9/fps_auth/routes.py` & `fps_auth-0.2.0/fps_auth/routes.py`

 * *Files identical despite different names*

### Comparing `fps_auth-0.1.9/.gitignore` & `fps_auth-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_auth-0.1.9/COPYING.md` & `fps_auth-0.2.0/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_auth-0.1.9/pyproject.toml` & `fps_auth-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 name = "fps_auth"
 description = "An FPS plugin for the authentication API"
 keywords = ["jupyter", "server", "fastapi", "plugins"]
 dynamic = ["version"]
 requires-python = ">=3.8"
 dependencies = [
     "aiosqlite",
-    "fastapi-users[sqlalchemy,oauth] >=11,<12",
-    "sqlalchemy >=1,<2",
+    "fastapi-users[sqlalchemy,oauth] >=12,<13",
     "jupyverse-api >=0.1.2,<1",
 ]
 
 [[project.authors]]
 name = "Jupyter Development Team"
 email = "jupyter@googlegroups.com"
```

### Comparing `fps_auth-0.1.9/PKG-INFO` & `fps_auth-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: fps_auth
-Version: 0.1.9
+Version: 0.2.0
 Summary: An FPS plugin for the authentication API
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
 Requires-Dist: aiosqlite
-Requires-Dist: fastapi-users[oauth,sqlalchemy]<12,>=11
+Requires-Dist: fastapi-users[oauth,sqlalchemy]<13,>=12
 Requires-Dist: jupyverse-api<1,>=0.1.2
-Requires-Dist: sqlalchemy<2,>=1
 Description-Content-Type: text/markdown
 
 # fps-auth
 
 An FPS plugin for the authentication API.
```

