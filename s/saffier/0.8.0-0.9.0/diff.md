# Comparing `tmp/saffier-0.8.0.tar.gz` & `tmp/saffier-0.9.0.tar.gz`

## Comparing `saffier-0.8.0.tar` & `saffier-0.9.0.tar`

### file list

```diff
@@ -1,78 +1,83 @@
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/__init__.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/exceptions.py
--rw-r--r--   0        0        0    11401 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/fields.py
--rw-r--r--   0        0        0    14214 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/metaclass.py
--rw-r--r--   0        0        0     9296 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/models.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/py.typed
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/testclient.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/types.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/conf/__init__.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/conf/enums.py
--rw-r--r--   0        0        0     6920 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/conf/functional.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/conf/global_settings.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/conf/module_import.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/core/__init__.py
--rw-r--r--   0        0        0     6740 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/core/base.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/core/datastructures.py
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/core/events.py
--rw-r--r--   0        0        0     6366 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/core/formats.py
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/core/registry.py
--rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/core/schemas.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/core/sync.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/core/unique.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/core/utils.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/core/terminal/__init__.py
--rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/core/terminal/base.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/core/terminal/print.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/core/terminal/terminal.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/db/__init__.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/db/connection.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/db/constants.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/db/datastructures.py
--rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/db/fields.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/db/manager.py
--rw-r--r--   0        0        0    26886 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/db/queryset.py
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/db/related.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/db/query/__init__.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/db/query/protocols.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/__init__.py
--rw-r--r--   0        0        0    11109 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/base.py
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/cli.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/constants.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/decorators.py
--rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/env.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/__init__.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/branches.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/check.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/current.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/downgrade.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/edit.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/heads.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/history.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/init.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/list_templates.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/makemigrations.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/merge.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/migrate.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/revision.py
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/show.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/stamp.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/shell/__init__.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/shell/base.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/shell/enums.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/shell/ipython.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/shell/ptpython.py
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/shell/utils.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/templates/default/README
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/templates/default/alembic.ini.mako
--rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/templates/default/env.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/templates/default/script.py.mako
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/sqlalchemy/fields.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/sqlalchemy/protocols.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/sqlalchemy/types.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 saffier-0.8.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 saffier-0.8.0/LICENSE
--rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 saffier-0.8.0/README.md
--rw-r--r--   0        0        0     4808 2020-02-02 00:00:00.000000 saffier-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    11190 2020-02-02 00:00:00.000000 saffier-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/__init__.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/exceptions.py
+-rw-r--r--   0        0        0    15826 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/fields.py
+-rw-r--r--   0        0        0    15553 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/metaclass.py
+-rw-r--r--   0        0        0     9587 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/models.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/py.typed
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/testclient.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/types.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/conf/__init__.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/conf/enums.py
+-rw-r--r--   0        0        0     6920 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/conf/functional.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/conf/global_settings.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/conf/module_import.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/core/__init__.py
+-rw-r--r--   0        0        0     6740 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/core/base.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/core/datastructures.py
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/core/events.py
+-rw-r--r--   0        0        0     6366 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/core/formats.py
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/core/registry.py
+-rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/core/schemas.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/core/sync.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/core/unique.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/core/utils.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/core/terminal/__init__.py
+-rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/core/terminal/base.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/core/terminal/print.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/core/terminal/terminal.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/db/__init__.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/db/connection.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/db/constants.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/db/datastructures.py
+-rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/db/fields.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/db/manager.py
+-rw-r--r--   0        0        0    27826 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/db/queryset.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/db/query/__init__.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/db/query/protocols.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/db/relationships/__init__.py
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/db/relationships/related.py
+-rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/db/relationships/relation.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/migrations/__init__.py
+-rw-r--r--   0        0        0    11109 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/migrations/base.py
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/migrations/cli.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/migrations/constants.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/migrations/decorators.py
+-rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/migrations/env.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/migrations/operations/__init__.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/migrations/operations/branches.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/migrations/operations/check.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/migrations/operations/current.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/migrations/operations/downgrade.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/migrations/operations/edit.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/migrations/operations/heads.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/migrations/operations/history.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/migrations/operations/init.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/migrations/operations/list_templates.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/migrations/operations/makemigrations.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/migrations/operations/merge.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/migrations/operations/migrate.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/migrations/operations/revision.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/migrations/operations/show.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/migrations/operations/stamp.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/migrations/operations/shell/__init__.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/migrations/operations/shell/base.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/migrations/operations/shell/enums.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/migrations/operations/shell/ipython.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/migrations/operations/shell/ptpython.py
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/migrations/operations/shell/utils.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/migrations/templates/default/README
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/migrations/templates/default/alembic.ini.mako
+-rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/migrations/templates/default/env.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/migrations/templates/default/script.py.mako
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/protocols/__init__.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/protocols/many_relationship.py
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/protocols/queryset.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/sqlalchemy/fields.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/sqlalchemy/protocols.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 saffier-0.9.0/saffier/sqlalchemy/types.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 saffier-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 saffier-0.9.0/LICENSE
+-rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 saffier-0.9.0/README.md
+-rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 saffier-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    11139 2020-02-02 00:00:00.000000 saffier-0.9.0/PKG-INFO
```

### Comparing `saffier-0.8.0/saffier/__init__.py` & `saffier-0.9.0/saffier/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 
 from saffier.conf import settings
 from saffier.conf.global_settings import SaffierSettings
 
 from .core.registry import Registry
 from .db.connection import Database
 from .db.constants import CASCADE, RESTRICT, SET_NULL
@@ -20,14 +20,15 @@
     DecimalField,
     EmailField,
     FloatField,
     ForeignKey,
     IntegerField,
     IPAddressField,
     JSONField,
+    ManyToManyField,
     OneToOneField,
     PasswordField,
     TextField,
     TimeField,
     URLField,
     UUIDField,
 )
@@ -48,14 +49,15 @@
     "EmailField",
     "FloatField",
     "ForeignKey",
     "Index",
     "IPAddressField",
     "IntegerField",
     "JSONField",
+    "ManyToManyField",
     "Manager",
     "Migrate",
     "Model",
     "MultipleObjectsReturned",
     "OneToOneField",
     "PasswordField",
     "QuerySet",
```

### Comparing `saffier-0.8.0/saffier/exceptions.py` & `saffier-0.9.0/saffier/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,9 +37,21 @@
     ...
 
 
 class ForeignKeyBadConfigured(SaffierException):
     ...
 
 
+class RelationshipIncompatible(SaffierException):
+    ...
+
+
+class DuplicateRecordError(SaffierException):
+    ...
+
+
+class RelationshipNotFound(SaffierException):
+    ...
+
+
 class CommandEnvironmentError(SaffierException):
     ...
```

### Comparing `saffier-0.8.0/saffier/fields.py` & `saffier-0.9.0/saffier/fields.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import typing
+import warnings
 from datetime import date, datetime
 
 import sqlalchemy
 
+import saffier
+from saffier.core.terminal import Terminal
 from saffier.db.constants import CASCADE, SET_NULL
 from saffier.db.fields import (
     URL,
     UUID,
     Any,
     Boolean,
     Date,
@@ -16,14 +19,19 @@
     Float,
     Integer,
 )
 from saffier.db.fields import IPAddress as CoreIPAddress
 from saffier.db.fields import Password, SaffierField, String, Time
 from saffier.sqlalchemy.fields import IPAddress
 
+if typing.TYPE_CHECKING:
+    from saffier import Model
+
+terminal = Terminal()
+
 
 class Field:
     """
     Base field for the model declaration fields.
     """
 
     def __init__(
@@ -235,19 +243,20 @@
 
     class ForeignKeyValidator(SaffierField):
         def check(self, value: typing.Any) -> typing.Any:
             return value.pk
 
     def __init__(
         self,
-        to: typing.Any,
+        to: typing.Type["Model"],
         null: bool = False,
         on_delete: typing.Optional[str] = None,
         on_update: typing.Optional[str] = None,
         related_name: typing.Optional[str] = None,
+        **kwargs: Any,
     ):
         assert on_delete is not None, "on_delete must not be null."
 
         if on_delete == SET_NULL and not null:
             raise AssertionError("When SET_NULL is enabled, null must be True.")
 
         if on_update and (on_update == SET_NULL and not null):
@@ -290,14 +299,136 @@
     def expand_relationship(self, value: typing.Any) -> typing.Any:
         target = self.target
         if isinstance(value, target):
             return value
         return target(pk=value)
 
 
+class ManyToManyField(Field):
+    """
+    Representation of a ManyToManyField based on a foreignkey.
+    """
+
+    def __init__(
+        self,
+        to: typing.Type["Model"],
+        through: typing.Optional[typing.Type["Model"]] = None,
+        **kwargs: typing.Any,
+    ):
+        if "null" in kwargs:
+            message = terminal.write_warning(
+                "Declaring `null` on a ManyToMany relationship has no effect."
+            )
+            warnings.warn(message, UserWarning, stacklevel=2)
+
+        super().__init__(null=True)
+        self.to = to
+        self.through = through
+        self.related_name = kwargs.pop("related_name", None)
+
+        if self.related_name:
+            assert isinstance(self.related_name, str), "related_name must be a string."
+
+        self.related_name = self.related_name.lower() if self.related_name else None
+
+    @property
+    def target(self) -> typing.Any:
+        if not hasattr(self, "_target"):
+            if isinstance(self.to, str):
+                self._target = self.registry.models[self.to]  # type: ignore
+            else:
+                self._target = self.to
+        return self._target
+
+    def get_column(self, name: str) -> sqlalchemy.Column:
+        target = self.target
+        to_field = target.fields[target.pkname]
+
+        column_type = to_field.get_column_type()
+        constraints = [
+            sqlalchemy.schema.ForeignKey(
+                f"{target._meta.tablename}.{target.pkname}",
+                ondelete=saffier.CASCADE,
+                onupdate=saffier.CASCADE,
+                name=f"fk_{self.owner._meta.tablename}_{target._meta.tablename}"
+                f"_{target.pkname}_{name}",
+            )
+        ]
+        return sqlalchemy.Column(name, column_type, *constraints, nullable=self.null)
+
+    def add_model_to_register(self, model: typing.Type["Model"]):
+        """
+        Adds the model to the registry to make sure it can be generated by the Migrations
+        """
+        self.registry.models[model.__name__] = model
+
+    def create_through_model(self) -> None:
+        """
+        Creates the default empty through model.
+
+        Generates a middle model based on the owner of the field and the field itself and adds
+        it to the main registry to make sure it generates the proper models and migrations.
+        """
+        if self.through:
+            if isinstance(self.through, str):
+                self.through = self.owner._meta.registry.models[self.through]
+
+            self.through._meta.is_multi = True
+            self.through._meta.multi_related = [self.to.__name__.lower()]
+            return self.through
+
+        owner_name = self.owner.__name__
+        to_name = self.to.__name__
+        class_name = f"{owner_name}{to_name}"
+        tablename = f"{owner_name.lower()}s_{to_name}s".lower()
+
+        new_meta_namespace = {
+            "tablename": tablename,
+            "registry": self.owner._meta.registry,
+            "is_multi": True,
+            "multi_related": [to_name.lower()],
+        }
+
+        new_meta = type("MetaInfo", (), new_meta_namespace)
+
+        # Define the related names
+        owner_related_name = (
+            f"{self.related_name}_{class_name.lower()}s_set"
+            if self.related_name
+            else f"{owner_name.lower()}_{class_name.lower()}s_set"
+        )
+
+        to_related_name = (
+            f"{self.related_name}"
+            if self.related_name
+            else f"{to_name.lower()}_{class_name.lower()}s_set"
+        )
+
+        through_model = type(
+            class_name,
+            (saffier.Model,),
+            {
+                "Meta": new_meta,
+                "id": saffier.IntegerField(primary_key=True),
+                f"{owner_name.lower()}": ForeignKey(
+                    self.owner,
+                    on_delete=saffier.CASCADE,
+                    null=True,
+                    related_name=owner_related_name,
+                ),
+                f"{to_name.lower()}": ForeignKey(
+                    self.to, on_delete=saffier.CASCADE, null=True, related_name=to_related_name
+                ),
+            },
+        )
+        self.through = typing.cast(typing.Type["Model"], through_model)
+
+        self.add_model_to_register(self.through)
+
+
 class OneToOneField(ForeignKey):
     """
     Representation of a one to one field.
     """
 
     def get_column(self, name: str) -> sqlalchemy.Column:
         target = self.target
```

### Comparing `saffier-0.8.0/saffier/metaclass.py` & `saffier-0.9.0/saffier/metaclass.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 import typing
 from typing import TYPE_CHECKING
 
 import sqlalchemy
 
 from saffier import fields as saffier_fields
 from saffier.core.registry import Registry
+from saffier.db.constants import MANY_TO_MANY_RELATION
 from saffier.db.datastructures import Index, UniqueConstraint
 from saffier.db.manager import Manager
-from saffier.db.related import RelatedField
+from saffier.db.relationships.related import RelatedField
+from saffier.db.relationships.relation import Relation
 from saffier.exceptions import ForeignKeyBadConfigured, ImproperlyConfigured
 from saffier.fields import BigIntegerField, Field
 from saffier.types import DictAny
 
 if TYPE_CHECKING:
     from saffier.models import Model, ReflectModel
 
@@ -27,38 +29,44 @@
         "tablename",
         "unique_together",
         "indexes",
         "foreign_key_fields",
         "parents",
         "pk",
         "one_to_one_fields",
+        "many_to_many_fields",
         "pk_attribute",
         "manager",
         "_model",
         "reflect",
         "_managers",
+        "is_multi",
+        "multi_related",
     )
 
     def __init__(self, meta: typing.Optional["Model.Meta"] = None) -> None:
         self.abstract: bool = getattr(meta, "abstract", False)
         self.fields: typing.Set = set()
         self.fields_mapping: typing.Dict[str, Field] = {}
         self.registry: typing.Optional[typing.Type[Registry]] = getattr(meta, "registry", None)
         self.tablename: typing.Optional[str] = getattr(meta, "tablename", None)
         self.parents: typing.Any = getattr(meta, "parents", None) or []
         self.pk: typing.Optional[Field] = None
         self.one_to_one_fields: typing.Set[str] = set()
+        self.many_to_many_fields: typing.Set[str] = set()
         self.foreign_key_fields: typing.Set[str] = set()
         self.pk_attribute: typing.Union[Field, str] = getattr(meta, "pk_attribute", "")
         self._model: typing.Optional[typing.Type["Model"]] = None
         self.manager: Manager = getattr(meta, "manager", Manager())
         self.unique_together: typing.Any = getattr(meta, "unique_together", None)
         self.indexes: typing.Any = getattr(meta, "indexes", None)
         self.reflect: bool = getattr(meta, "reflect", False)
         self._managers: bool = getattr(meta, "_managers", None)
+        self.is_multi: bool = getattr(meta, "is_multi", False)
+        self.multi_related: typing.List[str] = getattr(meta, "multi_related", [])
 
 
 def _check_model_inherited_registry(
     bases: typing.Tuple[typing.Type, ...]
 ) -> typing.Type[Registry]:
     """
     When a registry is missing from the Meta class, it should look up for the bases
@@ -131,23 +139,34 @@
             related_from=model_class,
         )
 
         # Set the related name
         setattr(foreign_key.target, default_related_name, related_field)
 
 
+def _set_many_to_many_relation(
+    m2m: saffier_fields.ManyToManyField,
+    model_class: typing.Union["Model", "ReflectModel"],
+    field: str,
+) -> None:
+    m2m.create_through_model()
+    relation = Relation(through=m2m.through, to=m2m.to, owner=m2m.owner)
+    setattr(model_class, MANY_TO_MANY_RELATION.format(key=field), relation)
+
+
 class BaseModelMeta(type):
     __slots__ = ()
 
     def __new__(
         cls, name: str, bases: typing.Tuple[typing.Type, ...], attrs: DictAny
     ) -> typing.Any:
         fields: typing.Dict[str, Field] = {}
         one_to_one_fields: typing.Any = set()
         foreign_key_fields: typing.Any = set()
+        many_to_many_fields: typing.Any = set()
         meta_class: "Model.Meta" = attrs.get("Meta", type("Meta", (), {}))
         pk_attribute: str = "id"
         registry: typing.Any = None
 
         # Searching for fields "Field" in the class hierarchy.
         def __search_for_fields(base: typing.Type, attrs: DictAny) -> None:
             """
@@ -214,24 +233,32 @@
                 if getattr(meta_class, "abstract", None):
                     value = copy.copy(value)
 
                 fields[key] = value
 
                 if isinstance(value, saffier_fields.OneToOneField):
                     one_to_one_fields.add(value)
-                elif isinstance(value, saffier_fields.ForeignKey):
+                    continue
+                elif isinstance(value, saffier_fields.ManyToManyField):
+                    many_to_many_fields.add(value)
+                    continue
+                elif isinstance(value, saffier_fields.ForeignKey) and not isinstance(
+                    value, saffier_fields.ManyToManyField
+                ):
                     foreign_key_fields.add(value)
+                    continue
 
         for slot in fields:
             attrs.pop(slot, None)
         attrs["_meta"] = meta = MetaInfo(meta_class)
 
         meta.fields_mapping = fields
         meta.foreign_key_fields = foreign_key_fields
         meta.one_to_one_fields = one_to_one_fields
+        meta.many_to_many_fields = many_to_many_fields
         meta.pk_attribute = pk_attribute
         meta.pk = fields.get(pk_attribute)
 
         if not fields:
             meta.abstract = True
 
         model_class = super().__new__
@@ -314,27 +341,31 @@
 
         new_class._db_model = True
         new_class.fields = meta.fields_mapping
 
         meta._model = new_class  # type: ignore
         meta.manager.model_class = new_class
 
+        # Set the owner of the field
+        for _, value in new_class.fields.items():
+            value.owner = new_class
+
         # Sets the foreign key fields
         if meta.foreign_key_fields:
             _set_related_name_for_foreign_keys(meta.foreign_key_fields, new_class)
 
+        for field, value in new_class.fields.items():
+            if isinstance(value, saffier_fields.ManyToManyField):
+                _set_many_to_many_relation(value, new_class, field)
+
         # Set the manager
         for _, value in attrs.items():
             if isinstance(value, Manager):
                 value.model_class = new_class
 
-        # Set the owner of the field
-        for _, value in new_class.fields.items():
-            value.owner = new_class
-
         return new_class
 
     @property
     def table(cls) -> typing.Any:
         """
         Making sure the tables on inheritance state, creates the new
         one properly.
```

### Comparing `saffier-0.8.0/saffier/models.py` & `saffier-0.9.0/saffier/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import asyncio
 import functools
 import typing
 
 import sqlalchemy
 from sqlalchemy.engine import Engine
 
+import saffier
 from saffier.core.schemas import Schema
 from saffier.core.utils import ModelUtil
+from saffier.db.constants import MANY_TO_MANY_RELATION
 from saffier.db.datastructures import Index, UniqueConstraint
 from saffier.db.manager import Manager
 from saffier.exceptions import ImproperlyConfigured
 from saffier.metaclass import MetaInfo, ModelMeta, ReflectMeta
 
 
 def async_adapter(wrapped_func):
@@ -165,15 +167,15 @@
         row = await self.database.fetch_one(expression)
 
         # Update the instance.
         for key, value in dict(row._mapping).items():
             setattr(self, key, value)
 
     @classmethod
-    def _from_row(cls, row: typing.Any, select_related: typing.Any = None) -> "Model":
+    def from_query_result(cls, row: typing.Any, select_related: typing.Any = None) -> "Model":
         """
         Instantiate a model instance, given a database row.
         """
         item = {}
 
         if not select_related:
             select_related = []
@@ -183,21 +185,21 @@
             if "__" in related:
                 first_part, remainder = related.split("__", 1)
                 try:
                     model_cls = cls.fields[first_part].target
                 except KeyError:
                     model_cls = getattr(cls, first_part).related_from
 
-                item[first_part] = model_cls._from_row(row, select_related=[remainder])
+                item[first_part] = model_cls.from_query_result(row, select_related=[remainder])
             else:
                 try:
                     model_cls = cls.fields[related].target
                 except KeyError:
                     model_cls = getattr(cls, related).related_from
-                item[related] = model_cls._from_row(row)
+                item[related] = model_cls.from_query_result(row)
 
         # Pull out the regular column values.
         for column in cls.table.columns:
             # Making sure when a table is reflected, maps the right fields of the ReflectModel
             if column.name not in cls.fields.keys():
                 continue
 
@@ -206,15 +208,21 @@
 
         return cls(**item)
 
     def __setattr__(self, key: typing.Any, value: typing.Any) -> typing.Any:
         if key in self.fields:
             # Setting a relationship to a raw pk value should set a
             # fully-fledged relationship instance, with just the pk loaded.
-            value = self.fields[key].expand_relationship(value)
+            field = self.fields[key]
+
+            if isinstance(field, saffier.ManyToManyField):
+                value = getattr(self, MANY_TO_MANY_RELATION.format(key=key))
+            else:
+                value = self.fields[key].expand_relationship(value)
+
         super().__setattr__(key, value)
 
     def __eq__(self, other: typing.Any) -> bool:
         if self.__class__ != other.__class__:
             return False
         for key in self.fields.keys():
             if getattr(self, key, None) != getattr(other, key, None):
```

### Comparing `saffier-0.8.0/saffier/conf/__init__.py` & `saffier-0.9.0/saffier/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/conf/functional.py` & `saffier-0.9.0/saffier/conf/functional.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/conf/global_settings.py` & `saffier-0.9.0/saffier/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/conf/module_import.py` & `saffier-0.9.0/saffier/conf/module_import.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/core/base.py` & `saffier-0.9.0/saffier/core/base.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/core/datastructures.py` & `saffier-0.9.0/saffier/core/datastructures.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/core/events.py` & `saffier-0.9.0/saffier/core/events.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/core/formats.py` & `saffier-0.9.0/saffier/core/formats.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/core/registry.py` & `saffier-0.9.0/saffier/core/registry.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/core/schemas.py` & `saffier-0.9.0/saffier/core/schemas.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/core/sync.py` & `saffier-0.9.0/saffier/core/sync.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/core/unique.py` & `saffier-0.9.0/saffier/core/unique.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/core/utils.py` & `saffier-0.9.0/saffier/core/utils.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/core/terminal/base.py` & `saffier-0.9.0/saffier/core/terminal/base.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/core/terminal/print.py` & `saffier-0.9.0/saffier/core/terminal/print.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/core/terminal/terminal.py` & `saffier-0.9.0/saffier/core/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/db/datastructures.py` & `saffier-0.9.0/saffier/db/datastructures.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/db/fields.py` & `saffier-0.9.0/saffier/db/fields.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/db/manager.py` & `saffier-0.9.0/saffier/db/manager.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/db/queryset.py` & `saffier-0.9.0/saffier/db/queryset.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,23 +6,24 @@
 import saffier
 from saffier.core.schemas import Schema
 from saffier.core.utils import ModelUtil
 from saffier.db.constants import DEFAULT_RELATED_LOOKUP_FIELD, FILTER_OPERATORS
 from saffier.db.query.protocols import AwaitableQuery
 from saffier.exceptions import DoesNotFound, MultipleObjectsReturned
 from saffier.fields import CharField, TextField
+from saffier.protocols.queryset import QuerySetProtocol
 
 if typing.TYPE_CHECKING:  # pragma: no cover
     from saffier.models import Model, ReflectModel
 
 
-SaffierModel = typing.TypeVar("SaffierModel", bound="Model")
+_SaffierModel = typing.TypeVar("_SaffierModel", bound="Model")
 ReflectSaffierModel = typing.TypeVar("ReflectSaffierModel", bound="ReflectModel")
 
-SaffierModels = typing.Union[SaffierModel, ReflectSaffierModel]
+SaffierModel = typing.Union[_SaffierModel, ReflectSaffierModel]
 
 
 class QuerySetProps:
     """
     Properties used by the Queryset are placed in isolation
     for clean access and maintainance.
     """
@@ -40,40 +41,57 @@
         fields = {key: field.validator for key, field in self.model_class.fields.items()}  # type: ignore
         return Schema(fields=fields)
 
     @property
     def pkname(self) -> typing.Any:
         return self.model_class.pkname  # type: ignore
 
+    @property
+    def is_m2m(self) -> bool:
+        return bool(self.model_class._meta.is_multi)
+
+    @property
+    def m2m_related(self) -> bool:
+        return self._m2m_related
+
+    @m2m_related.setter
+    def m2m_related(self, value: str) -> None:
+        self._m2m_related = value
 
-class BaseQuerySet(QuerySetProps, ModelUtil, AwaitableQuery[SaffierModels]):
+
+class BaseQuerySet(QuerySetProps, ModelUtil, AwaitableQuery[SaffierModel]):
     ESCAPE_CHARACTERS = ["%", "_"]
 
     def __init__(
         self,
         model_class: typing.Any = None,
         filter_clauses: typing.Any = None,
         select_related: typing.Any = None,
         limit_count: typing.Any = None,
         limit_offset: typing.Any = None,
         order_by: typing.Any = None,
         group_by: typing.Any = None,
         distinct_on: typing.Any = None,
+        m2m_related: typing.Any = None,
     ) -> None:
         super().__init__(model_class=model_class)
         self.model_class = model_class
         self.filter_clauses = [] if filter_clauses is None else filter_clauses
         self.limit_count = limit_count
         self._select_related = [] if select_related is None else select_related
         self._offset = limit_offset
         self._order_by = [] if order_by is None else order_by
         self._group_by = [] if group_by is None else group_by
         self.distinct_on = [] if distinct_on is None else distinct_on
         self._expression = None
         self._cache = None
+        self._m2m_related = m2m_related
+
+        if self.is_m2m and not self._m2m_related:
+            self._m2m_related = self.model_class._meta.multi_related[0]
 
     def _build_order_by_expression(
         self, order_by: typing.Any, expression: typing.Any
     ) -> typing.Any:
         """Builds the order by expression"""
         order_by = list(map(self._prepare_order_by, order_by))
         expression = expression.order_by(*order_by)
@@ -144,17 +162,19 @@
         Builds the tables relationships and joins.
         When a table contains more than one foreign key pointing to the same
         destination table, a lookup for the related field is made to understand
         from which foreign key the table is looked up from.
         """
         tables = [self.table]
         select_from = self.table
+
         has_many_fk_same_table = False
 
         for item in self._select_related:
+            # For m2m relationships
             model_class = self.model_class
             select_from = self.table
 
             for part in item.split("__"):
                 try:
                     model_class = model_class.fields[part].target
                 except KeyError:
@@ -305,14 +325,15 @@
         return self.__class__(
             model_class=self.model_class,
             filter_clauses=filter_clauses,
             select_related=select_related,
             limit_count=self.limit_count,
             limit_offset=self._offset,
             order_by=self._order_by,
+            m2m_related=self.m2m_related,
         )
 
     def _validate_kwargs(self, **kwargs: typing.Any) -> typing.Any:
         fields = self.model_class.fields
         validator = Schema(fields={key: value.validator for key, value in fields.items()})
         kwargs = validator.check(kwargs)
         for key, value in fields.items():
@@ -347,22 +368,23 @@
         queryset._select_related = copy.copy(self._select_related)
         queryset._offset = self._offset
         queryset._order_by = copy.copy(self._order_by)
         queryset._group_by = copy.copy(self._group_by)
         queryset.distinct_on = copy.copy(self.distinct_on)
         queryset._expression = self._expression
         queryset._cache = self._cache
+        queryset._m2m_related = self._m2m_related
         return queryset
 
     def _fetch_all(self) -> None:
         if self._cache is None:
             self._cache = self._make_query()
 
 
-class QuerySet(BaseQuerySet):
+class QuerySet(BaseQuerySet, QuerySetProtocol):
     """
     QuerySet object used for query retrieving.
     """
 
     def __get__(self, instance: typing.Any, owner: typing.Any) -> typing.Any:
         return self.__class__(model_class=owner)
 
@@ -370,15 +392,15 @@
     def sql(self) -> str:
         return str(self._expression)
 
     @sql.setter
     def sql(self, value: typing.Any) -> None:
         self._expression = value
 
-    async def __aiter__(self) -> typing.AsyncIterator[SaffierModels]:
+    async def __aiter__(self) -> typing.AsyncIterator[SaffierModel]:
         for value in await self:  # type: ignore
             yield value
 
     def _set_query_expression(self, expression: typing.Any) -> None:
         """
         Sets the value of the sql property to the expression used.
         """
@@ -403,31 +425,31 @@
         queryset.filter_clauses.append(clause)
         return queryset
 
     def filter(
         self,
         clause: typing.Optional[sqlalchemy.sql.expression.BinaryExpression] = None,
         **kwargs: typing.Any,
-    ) -> typing.Any:
+    ) -> "QuerySet":
         """
         Filters the QuerySet by the given kwargs and clause.
         """
         return self._filter_or_exclude(clause=clause, **kwargs)
 
     def exclude(
         self,
         clause: typing.Optional[sqlalchemy.sql.expression.BinaryExpression] = None,
         **kwargs: typing.Any,
-    ) -> typing.Any:
+    ) -> "QuerySet":
         """
         Exactly the same as the filter but for the exclude.
         """
         return self._filter_or_exclude(clause=clause, exclude=True, **kwargs)
 
-    def lookup(self, term: typing.Any) -> typing.Any:
+    def lookup(self, term: typing.Any) -> "QuerySet":
         """
         Broader way of searching for a given term
         """
         queryset = self._clone()
         if not term:
             return queryset
 
@@ -444,55 +466,55 @@
         if len(search_clauses) > 1:
             filter_clauses.append(sqlalchemy.sql.or_(*search_clauses))
         else:
             filter_clauses.extend(search_clauses)
 
         return queryset
 
-    def order_by(self, *order_by: str) -> typing.Any:
+    def order_by(self, *order_by: str) -> "QuerySet":
         """
         Returns a QuerySet ordered by the given fields.
         """
         queryset = self._clone()
         queryset._order_by = order_by
         return queryset
 
-    def limit(self, limit_count: int) -> typing.Any:
+    def limit(self, limit_count: int) -> "QuerySet":
         """
         Returns a QuerySet limited by.
         """
         queryset = self._clone()
         queryset.limit_count = limit_count
         return queryset
 
-    def offset(self, offset: int) -> typing.Any:
+    def offset(self, offset: int) -> "QuerySet":
         """
         Returns a Queryset limited by the offset.
         """
         queryset = self._clone()
         queryset._offset = offset
         return queryset
 
-    def group_by(self, *group_by: str) -> typing.Any:
+    def group_by(self, *group_by: str) -> "QuerySet":
         """
         Returns the values grouped by the given fields.
         """
         queryset = self._clone()
         queryset._group_by = group_by
         return queryset
 
-    def distinct(self, *distinct_on: str) -> typing.Any:
+    def distinct(self, *distinct_on: str) -> "QuerySet":
         """
         Returns a queryset with distinct results.
         """
         queryset = self._clone()
         queryset.distinct_on = distinct_on
         return queryset
 
-    def select_related(self, related: typing.Any) -> typing.Any:
+    def select_related(self, related: typing.Any) -> "QuerySet":
         """
         Returns a QuerySet that will “follow” foreign-key relationships, selecting additional
         related-object data when it executes its query.
 
         This is a performance booster which results in a single more complex query but means
 
         later use of foreign-key relationships won’t require database queries.
@@ -501,109 +523,119 @@
         if not isinstance(related, (list, tuple)):
             related = [related]
 
         related = list(self._select_related) + related
         queryset._select_related = related
         return queryset
 
-    async def exists(self) -> typing.Any:
+    async def exists(self) -> bool:
         """
         Returns a boolean indicating if a record exists or not.
         """
         expression = self._build_select()
         expression = sqlalchemy.exists(expression).select()
         self._set_query_expression(expression)
         return await self.database.fetch_val(expression)
 
-    async def count(self) -> typing.Any:
+    async def count(self) -> int:
         """
         Returns an indicating the total records.
         """
         expression = self._build_select().alias("subquery_for_count")
         expression = sqlalchemy.func.count().select().select_from(expression)
         self._set_query_expression(expression)
         return await self.database.fetch_val(expression)
 
-    async def get_or_none(self, **kwargs: typing.Any) -> typing.Any:
+    async def get_or_none(self, **kwargs: typing.Any) -> typing.Union[SaffierModel, None]:
         """
         Fetch one object matching the parameters or returns None.
         """
         queryset: "QuerySet" = self.filter(**kwargs)
         expression = queryset._build_select().limit(2)
         self._set_query_expression(expression)
         rows = await self.database.fetch_all(expression)
 
         if not rows:
             return None
         if len(rows) > 1:
             raise MultipleObjectsReturned()
-        return self.model_class._from_row(rows[0], select_related=self._select_related)
+        return self.model_class.from_query_result(rows[0], select_related=self._select_related)
 
-    async def all(self, **kwargs: typing.Any) -> typing.Any:
+    async def all(self, **kwargs: typing.Any) -> typing.List[SaffierModel]:
         """
         Returns the queryset records based on specific filters
         """
         queryset = self._clone()
+
+        if self.is_m2m:
+            queryset.distinct_on = [self.m2m_related]
+
         if kwargs:
             return await queryset.filter(**kwargs).all()
 
         expression = queryset._build_select()
         self._set_query_expression(expression)
 
         rows = await queryset.database.fetch_all(expression)
 
         # Attach the raw query to the object
         queryset.model_class.raw_query = self.sql
-        return [
-            queryset.model_class._from_row(row, select_related=self._select_related)
+
+        results = [
+            queryset.model_class.from_query_result(row, select_related=self._select_related)
             for row in rows
         ]
 
-    async def get(self, **kwargs: typing.Any) -> typing.Any:
+        if not self.is_m2m:
+            return results
+
+        return [getattr(result, self.m2m_related) for result in results]
+
+    async def get(self, **kwargs: typing.Any) -> SaffierModel:
         """
         Returns a single record based on the given kwargs.
         """
         if kwargs:
             return await self.filter(**kwargs).get()
 
         expression = self._build_select().limit(2)
         rows = await self.database.fetch_all(expression)
         self._set_query_expression(expression)
 
         if not rows:
             raise DoesNotFound()
         if len(rows) > 1:
             raise MultipleObjectsReturned()
-        return self.model_class._from_row(rows[0], select_related=self._select_related)
+        return self.model_class.from_query_result(rows[0], select_related=self._select_related)
 
-    async def first(self, **kwargs: typing.Any) -> typing.Any:
+    async def first(self, **kwargs: typing.Any) -> SaffierModel:
         """
         Returns the first record of a given queryset.
         """
         queryset = self._clone()
         if kwargs:
             return await queryset.filter(**kwargs).order_by("id").get()
 
         rows = await queryset.limit(1).order_by("id").all()
         if rows:
             return rows[0]
 
-    async def last(self, **kwargs: typing.Any) -> typing.Any:
+    async def last(self, **kwargs: typing.Any) -> SaffierModel:
         """
         Returns the last record of a given queryset.
         """
         queryset = self._clone()
         if kwargs:
             return await queryset.filter(**kwargs).order_by("-id").get()
 
         rows = await queryset.order_by("-id").all()
         if rows:
             return rows[0]
 
-    async def create(self, **kwargs: typing.Any) -> typing.Any:
+    async def create(self, **kwargs: typing.Any) -> SaffierModel:
         """
         Creates a record in a specific table.
         """
         kwargs = self._validate_kwargs(**kwargs)
         instance = self.model_class(**kwargs)
         expression = self.table.insert().values(**kwargs)
         self._set_query_expression(expression)
@@ -620,17 +652,15 @@
         """
         new_objs = [self._validate_kwargs(**obj) for obj in objs]
 
         expression = self.table.insert().values(new_objs)
         self._set_query_expression(expression)
         await self.database.execute(expression)
 
-    async def bulk_update(
-        self, objs: typing.List[SaffierModels], fields: typing.List[str]
-    ) -> None:
+    async def bulk_update(self, objs: typing.List[SaffierModel], fields: typing.List[str]) -> None:
         """
         Bulk updates records in a table.
 
         A similar solution was suggested here: https://github.com/encode/orm/pull/148
 
         It is thought to be a clean approach to a simple problem so it was added here and
         refactored to be compatible with Saffier.
@@ -672,15 +702,15 @@
         expression = self.table.delete()
         for filter_clause in self.filter_clauses:
             expression = expression.where(filter_clause)
 
         self._set_query_expression(expression)
         await self.database.execute(expression)
 
-    async def update(self, **kwargs: typing.Any) -> None:
+    async def update(self, **kwargs: typing.Any) -> int:
         """
         Updates a record in a specific table with the given kwargs.
         """
         fields = {
             key: field.validator for key, field in self.model_class.fields.items() if key in kwargs
         }
 
@@ -692,55 +722,55 @@
             expression = expression.where(filter_clause)
 
         self._set_query_expression(expression)
         await self.database.execute(expression)
 
     async def get_or_create(
         self, defaults: typing.Dict[str, typing.Any], **kwargs: typing.Any
-    ) -> typing.Tuple[typing.Any, bool]:
+    ) -> typing.Tuple[SaffierModel, bool]:
         """
         Creates a record in a specific table or updates if already exists.
         """
         try:
             instance = await self.get(**kwargs)
             return instance, False
         except DoesNotFound:
             kwargs.update(defaults)
             instance = await self.create(**kwargs)
             return instance, True
 
     async def update_or_create(
         self, defaults: typing.Dict[str, typing.Any], **kwargs: typing.Any
-    ) -> typing.Tuple[typing.Any, bool]:
+    ) -> typing.Tuple[SaffierModel, bool]:
         """
         Updates a record in a specific table or creates a new one.
         """
         try:
             instance = await self.get(**kwargs)
             await instance.update(**defaults)
             return instance, False
         except DoesNotFound:
             kwargs.update(defaults)
             instance = await self.create(**kwargs)
             return instance, True
 
-    async def contains(self, instance: SaffierModels) -> SaffierModels:
+    async def contains(self, instance: SaffierModel) -> bool:
         """Returns true if the QuerySet contains the provided object.
         False if otherwise.
         """
         if getattr(instance, "pk", None) is None:
             raise ValueError("'obj' must be a model or reflect model instance.")
         return await self.filter(pk=instance.pk).exists()
 
     async def _execute(self) -> typing.Any:
         return await self.all()
 
     def __await__(
         self,
-    ) -> typing.Generator[typing.Any, None, typing.List[SaffierModels]]:
+    ) -> typing.Generator[typing.Any, None, typing.List[SaffierModel]]:
         return self._execute().__await__()
 
     def __class_getitem__(cls, *args: typing.Any, **kwargs: typing.Any) -> typing.Any:
         return cls
 
     def __deepcopy__(self, memo: typing.Any) -> typing.Any:
         """Don't populate the QuerySet's cache."""
```

### Comparing `saffier-0.8.0/saffier/db/related.py` & `saffier-0.9.0/saffier/db/relationships/related.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,30 +21,53 @@
         instance: Optional[Union[Type["Model"], Type["ReflectModel"]]] = None,
     ) -> None:
         self.related_name = related_name
         self.related_to = related_to
         self.related_from = related_from
         self.instance = instance
 
+    @functools.cached_property
+    def manager(self):
+        """Returns the manager class"""
+        return self.related_from._meta.manager
+
+    @functools.cached_property
+    def queryset(self):
+        return self.manager.get_queryset()
+
+    def m2m_related(self):
+        """
+        Guarantees the the m2m filter is done by the owner of the call
+        and not by the children.
+        """
+        if not self.related_from._meta.is_multi:
+            return
+
+        related = [
+            key
+            for key, value in self.related_from.fields.items()
+            if key != self.related_to.__name__.lower() and isinstance(value, fields.ForeignKey)
+        ]
+        return related
+
     def __get__(self, instance: Any, owner: Any) -> Any:
         return self.__class__(
             related_name=self.related_name,
             related_to=self.related_to,
             instance=instance,
             related_from=self.related_from,
         )
 
     def __getattr__(self, item: Any) -> Any:
         """
         Gets the attribute from the queryset and if it does not
         exist, then lookup in the model.
         """
-        manager = self.related_from._meta.manager
         try:
-            attr = getattr(manager.get_queryset(), item)
+            attr = getattr(self.queryset, item)
         except AttributeError:
             attr = getattr(self.related_from, item)
 
         func = self.wrap_args(attr)
         return func
 
     def get_foreign_key_field_name(self) -> str:
@@ -67,14 +90,18 @@
         return field_name
 
     def wrap_args(self, func: Any) -> Any:
         @functools.wraps(func)
         def wrapped(*args: Any, **kwargs: Any) -> Any:
             field = self.get_foreign_key_field_name()
             kwargs[field] = self.instance.pk
+
+            related = self.m2m_related()
+            if related:
+                self.queryset.m2m_related = related[0]
             return func(*args, **kwargs)
 
         return wrapped
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__}: {self}>"
```

### Comparing `saffier-0.8.0/saffier/db/query/protocols.py` & `saffier-0.9.0/saffier/db/query/protocols.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/migrations/base.py` & `saffier-0.9.0/saffier/migrations/base.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/migrations/cli.py` & `saffier-0.9.0/saffier/migrations/cli.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/migrations/env.py` & `saffier-0.9.0/saffier/migrations/env.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/migrations/operations/__init__.py` & `saffier-0.9.0/saffier/migrations/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/migrations/operations/branches.py` & `saffier-0.9.0/saffier/migrations/operations/branches.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/migrations/operations/current.py` & `saffier-0.9.0/saffier/migrations/operations/current.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/migrations/operations/downgrade.py` & `saffier-0.9.0/saffier/migrations/operations/downgrade.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/migrations/operations/heads.py` & `saffier-0.9.0/saffier/migrations/operations/heads.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/migrations/operations/history.py` & `saffier-0.9.0/saffier/migrations/operations/history.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/migrations/operations/init.py` & `saffier-0.9.0/saffier/migrations/operations/init.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/migrations/operations/makemigrations.py` & `saffier-0.9.0/saffier/migrations/operations/makemigrations.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/migrations/operations/merge.py` & `saffier-0.9.0/saffier/migrations/operations/merge.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/migrations/operations/migrate.py` & `saffier-0.9.0/saffier/migrations/operations/migrate.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/migrations/operations/revision.py` & `saffier-0.9.0/saffier/migrations/operations/revision.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/migrations/operations/stamp.py` & `saffier-0.9.0/saffier/migrations/operations/stamp.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/migrations/operations/shell/base.py` & `saffier-0.9.0/saffier/migrations/operations/shell/base.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/migrations/operations/shell/ipython.py` & `saffier-0.9.0/saffier/migrations/operations/shell/ipython.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/migrations/operations/shell/ptpython.py` & `saffier-0.9.0/saffier/migrations/operations/shell/ptpython.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/migrations/operations/shell/utils.py` & `saffier-0.9.0/saffier/migrations/operations/shell/utils.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/migrations/templates/default/alembic.ini.mako` & `saffier-0.9.0/saffier/migrations/templates/default/alembic.ini.mako`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/migrations/templates/default/env.py` & `saffier-0.9.0/saffier/migrations/templates/default/env.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/sqlalchemy/fields.py` & `saffier-0.9.0/saffier/sqlalchemy/fields.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/saffier/sqlalchemy/protocols.py` & `saffier-0.9.0/saffier/sqlalchemy/protocols.py`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/LICENSE` & `saffier-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/README.md` & `saffier-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `saffier-0.8.0/pyproject.toml` & `saffier-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
 dependencies = [
     "alembic>=1.9.3,<2.0.0",
     "anyio>=3.6.2,<4",
     "click>=8.1.3,<9.0.0",
-    "loguru>=0.6.0,<0.7.0",
+    "loguru>=0.6.0,<0.10.0",
     "databasez>=0.2.2",
     "orjson >=3.8.5,<4.0.0",
     "pydantic>=1.10.5,<2.0.0",
     "rich>=13.3.1,<14.0.0",
 ]
 keywords = [
     "api",
@@ -76,42 +76,41 @@
 test = [
     "asyncpg>=0.27.0,<1",
     "asyncmy>=0.2.7,<0.3.0",
     "esmerald>=1.1.0",
     "pytest>=7.1.3,<8.0.0",
     "pytest-cov>=2.12.0,<5.0.0",
     "pytest-asyncio >=0.19.0",
-    "mypy==1.1.1",
+    "mypy==1.2.0",
     "flake8>=5.0.4",
     "black== 23.3.0",
     "isort>=5.0.6,<6.0.0",
     "freezegun>=1.2.2,<2.0.0",
-    "mock==5.0.1",
+    "mock==5.0.2",
     "pydantic>=1.10.5",
     "pymysql>=1.0.2,<2.0.0",
     "types-orjson==3.6.2",
     "ruff>=0.0.256,<1.0.0",
 ]
 
 dev = [
     "autoflake >=1.4.0",
     "flake8>=5.0.4",
     "uvicorn[standard] >=0.19.0",
     "pre-commit>=2.17.0,<4.0.0",
-    "loguru>=0.6.0,<0.7.0",
     "watchfiles>=0.16.1,<0.20.0",
 ]
 
 doc = [
     "mkautodoc>=0.2.0,<0.3.0",
     "mkdocs>=1.4.2,<2.0.0",
-    "mkdocs-material==9.1.5",
+    "mkdocs-material==9.1.8",
     "mdx-include>=1.4.1,<2.0.0",
     "mkdocs-markdownextradata-plugin>=0.1.7,<0.3.0",
-    "mkdocstrings>=0.19.0,<0.21.0",
+    "mkdocstrings>=0.19.0,<0.22.0",
     "pyyaml>=5.3.1,<7.0.0",
 ]
 
 testing = ["sqlalchemy_utils>=0.40.0"]
 postgres = ["databasez[postgresql]"]
 mysql = ["databasez[mysql]"]
 sqlite = ["databasez[sqlite]"]
```

### Comparing `saffier-0.8.0/PKG-INFO` & `saffier-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saffier
-Version: 0.8.0
+Version: 0.9.0
 Summary: The only python ORM you will ever need.
 Project-URL: Homepage, https://github.com/tarsil/saffier
 Project-URL: Documentation, https://saffier.tarsild.io/
 Project-URL: Changelog, https://saffier.tarsild.io/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/tarsil/saffier
 Author-email: Tiago Silva <tiago.arasilva@gmail.com>
@@ -36,38 +36,37 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: alembic<2.0.0,>=1.9.3
 Requires-Dist: anyio<4,>=3.6.2
 Requires-Dist: click<9.0.0,>=8.1.3
 Requires-Dist: databasez>=0.2.2
-Requires-Dist: loguru<0.7.0,>=0.6.0
+Requires-Dist: loguru<0.10.0,>=0.6.0
 Requires-Dist: orjson<4.0.0,>=3.8.5
 Requires-Dist: pydantic<2.0.0,>=1.10.5
 Requires-Dist: rich<14.0.0,>=13.3.1
 Provides-Extra: all
 Requires-Dist: databasez[mysql,postgresql,sqlite]; extra == 'all'
 Requires-Dist: ipython<9.0.0,>=8.10.0; extra == 'all'
 Requires-Dist: orjson<4.0.0,>=3.8.5; extra == 'all'
 Requires-Dist: ptpython<4.0.0,>=3.0.23; extra == 'all'
 Requires-Dist: pydantic<2.0.0,>=1.10.4; extra == 'all'
 Provides-Extra: dev
 Requires-Dist: autoflake>=1.4.0; extra == 'dev'
 Requires-Dist: flake8>=5.0.4; extra == 'dev'
-Requires-Dist: loguru<0.7.0,>=0.6.0; extra == 'dev'
 Requires-Dist: pre-commit<4.0.0,>=2.17.0; extra == 'dev'
 Requires-Dist: uvicorn[standard]>=0.19.0; extra == 'dev'
 Requires-Dist: watchfiles<0.20.0,>=0.16.1; extra == 'dev'
 Provides-Extra: doc
 Requires-Dist: mdx-include<2.0.0,>=1.4.1; extra == 'doc'
 Requires-Dist: mkautodoc<0.3.0,>=0.2.0; extra == 'doc'
 Requires-Dist: mkdocs-markdownextradata-plugin<0.3.0,>=0.1.7; extra == 'doc'
-Requires-Dist: mkdocs-material==9.1.5; extra == 'doc'
+Requires-Dist: mkdocs-material==9.1.8; extra == 'doc'
 Requires-Dist: mkdocs<2.0.0,>=1.4.2; extra == 'doc'
-Requires-Dist: mkdocstrings<0.21.0,>=0.19.0; extra == 'doc'
+Requires-Dist: mkdocstrings<0.22.0,>=0.19.0; extra == 'doc'
 Requires-Dist: pyyaml<7.0.0,>=5.3.1; extra == 'doc'
 Provides-Extra: ipython
 Requires-Dist: ipython<9.0.0,>=8.10.0; extra == 'ipython'
 Provides-Extra: mysql
 Requires-Dist: databasez[mysql]; extra == 'mysql'
 Provides-Extra: postgres
 Requires-Dist: databasez[postgresql]; extra == 'postgres'
@@ -79,16 +78,16 @@
 Requires-Dist: asyncmy<0.3.0,>=0.2.7; extra == 'test'
 Requires-Dist: asyncpg<1,>=0.27.0; extra == 'test'
 Requires-Dist: black==23.3.0; extra == 'test'
 Requires-Dist: esmerald>=1.1.0; extra == 'test'
 Requires-Dist: flake8>=5.0.4; extra == 'test'
 Requires-Dist: freezegun<2.0.0,>=1.2.2; extra == 'test'
 Requires-Dist: isort<6.0.0,>=5.0.6; extra == 'test'
-Requires-Dist: mock==5.0.1; extra == 'test'
-Requires-Dist: mypy==1.1.1; extra == 'test'
+Requires-Dist: mock==5.0.2; extra == 'test'
+Requires-Dist: mypy==1.2.0; extra == 'test'
 Requires-Dist: pydantic>=1.10.5; extra == 'test'
 Requires-Dist: pymysql<2.0.0,>=1.0.2; extra == 'test'
 Requires-Dist: pytest-asyncio>=0.19.0; extra == 'test'
 Requires-Dist: pytest-cov<5.0.0,>=2.12.0; extra == 'test'
 Requires-Dist: pytest<8.0.0,>=7.1.3; extra == 'test'
 Requires-Dist: ruff<1.0.0,>=0.0.256; extra == 'test'
 Requires-Dist: types-orjson==3.6.2; extra == 'test'
```

