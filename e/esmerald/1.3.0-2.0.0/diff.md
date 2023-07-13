# Comparing `tmp/esmerald-1.3.0.tar.gz` & `tmp/esmerald-2.0.0.tar.gz`

## Comparing `esmerald-1.3.0.tar` & `esmerald-2.0.0.tar`

### file list

```diff
@@ -1,185 +1,186 @@
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/__init__.py
--rw-r--r--   0        0        0    32636 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/applications.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/backgound.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/concurrency.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/enums.py
--rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/exception_handlers.py
--rw-r--r--   0        0        0     3871 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/exceptions.py
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/injector.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/logging.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/param_functions.py
--rw-r--r--   0        0        0    14464 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/params.py
--rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/parsers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/py.typed
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/requests.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/staticfiles.py
--rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/testclient.py
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/types.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/typing.py
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/websockets.py
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/__init__.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/enums.py
--rw-r--r--   0        0        0    13292 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/global_settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/app_template/__init__.py-tpl
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/app_template/tests.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/app_template/directives/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/app_template/directives/operations/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/app_template/v1/__init__.py-tpl
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/app_template/v1/schemas.py-tpl
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/app_template/v1/urls.py-tpl
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/app_template/v1/views.py-tpl
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/project_template/.gitignore.e-tpl
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/project_template/Makefile.e-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/project_template/project_name/__init__.py-tpl
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/project_template/project_name/main.py-tpl
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/project_template/project_name/serve.py-tpl
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/project_template/project_name/urls.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/project_template/project_name/apps/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/project_template/project_name/configs/__init__.py-tpl
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/project_template/project_name/configs/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/project_template/project_name/configs/development/__init__.py-tpl
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/project_template/project_name/configs/development/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/project_template/project_name/configs/testing/__init__.py-tpl
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/project_template/project_name/configs/testing/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/project_template/project_name/tests/__init__.py-tpl
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/conf/project_template/project_name/tests/test_app.py-tpl
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/config/__init__.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/config/asyncexit.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/config/cors.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/config/csrf.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/config/jwt.py
--rw-r--r--   0        0        0     6585 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/config/openapi.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/config/session.py
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/config/static_files.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/config/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/contrib/__init__.py
--rw-r--r--   0        0        0     7517 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/contrib/encoding.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/contrib/auth/__init__.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/contrib/auth/constants.py
--rw-r--r--   0        0        0     8616 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/contrib/auth/hashers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/contrib/auth/common/__init__.py
--rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/contrib/auth/common/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/contrib/auth/saffier/__init__.py
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/contrib/auth/saffier/base_user.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/contrib/auth/saffier/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/directives/__init__.py
--rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/directives/base.py
--rw-r--r--   0        0        0     4004 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/directives/cli.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/directives/constants.py
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/directives/env.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/directives/exceptions.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/directives/parsers.py
--rw-r--r--   0        0        0     6561 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/directives/templates.py
--rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/directives/utils.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/directives/operations/__init__.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/directives/operations/_constants.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/directives/operations/createapp.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/directives/operations/createproject.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/directives/operations/list.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/directives/operations/run.py
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/directives/operations/runserver.py
--rw-r--r--   0        0        0     4046 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/directives/operations/show_urls.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/terminal/__init__.py
--rw-r--r--   0        0        0     8301 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/terminal/base.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/terminal/print.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/terminal/terminal.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/urls/__init__.py
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/core/urls/base.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/datastructures/__init__.py
--rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/datastructures/base.py
--rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/datastructures/encoders.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/datastructures/file.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/datastructures/json.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/datastructures/redirect.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/datastructures/stream.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/datastructures/template.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/datastructures/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/interceptors/__init__.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/interceptors/interceptor.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/interceptors/types.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/middleware/__init__.py
--rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/middleware/_exception_handlers.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/middleware/asyncexitstack.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/middleware/authentication.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/middleware/basic.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/middleware/cors.py
--rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/middleware/csrf.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/middleware/errors.py
--rw-r--r--   0        0        0     6161 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/middleware/exceptions.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/middleware/gzip.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/middleware/https.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/middleware/sessions.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/middleware/settings_middleware.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/middleware/trustedhost.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/middleware/wsgi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/openapi/__init__.py
--rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/openapi/apiview.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/openapi/datastructures.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/openapi/enums.py
--rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/openapi/parameters.py
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/openapi/path_item.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/openapi/request_body.py
--rw-r--r--   0        0        0     8944 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/openapi/responses.py
--rw-r--r--   0        0        0     8991 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/openapi/schema.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/openapi/types.py
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/openapi/utils.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/permissions/__init__.py
--rw-r--r--   0        0        0     6857 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/permissions/base.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/permissions/types.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/permissions/utils.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/pluggables/__init__.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/pluggables/base.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/protocols/__init__.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/protocols/asyncdao.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/protocols/dao.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/protocols/extension.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/protocols/interceptor.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/protocols/middleware.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/protocols/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/protocols/utils/__init__.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/protocols/utils/protocols.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/responses/__init__.py
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/responses/base.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/responses/encoders.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/responses/json.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/responses/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/routing/__init__.py
--rw-r--r--   0        0        0    22142 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/routing/base.py
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/routing/events.py
--rw-r--r--   0        0        0     7328 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/routing/gateways.py
--rw-r--r--   0        0        0    22845 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/routing/handlers.py
--rw-r--r--   0        0        0    41247 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/routing/router.py
--rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/routing/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/security/__init__.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/security/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/security/jwt/__init__.py
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/security/jwt/token.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/template/__init__.py
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/template/jinja.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/template/mako.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/transformers/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/transformers/constants.py
--rw-r--r--   0        0        0     3573 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/transformers/datastructures.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/transformers/helpers.py
--rw-r--r--   0        0        0    14560 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/transformers/model.py
--rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/transformers/signature.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/transformers/types.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/transformers/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/utils/__init__.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/utils/constants.py
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/utils/crypto.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/utils/dependency.py
--rw-r--r--   0        0        0     7143 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/utils/functional.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/utils/helpers.py
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/utils/model.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/utils/module_loading.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/utils/sync.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/utils/url.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/utils/pydantic/__init__.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 esmerald-1.3.0/esmerald/utils/pydantic/schema.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 esmerald-1.3.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 esmerald-1.3.0/LICENSE
--rw-r--r--   0        0        0    15142 2020-02-02 00:00:00.000000 esmerald-1.3.0/README.md
--rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 esmerald-1.3.0/pyproject.toml
--rw-r--r--   0        0        0    20195 2020-02-02 00:00:00.000000 esmerald-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/__init__.py
+-rw-r--r--   0        0        0    39505 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/applications.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/backgound.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/concurrency.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/enums.py
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/exception_handlers.py
+-rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/exceptions.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/injector.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/logging.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/param_functions.py
+-rw-r--r--   0        0        0    21321 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/params.py
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/parsers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/py.typed
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/requests.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/staticfiles.py
+-rw-r--r--   0        0        0     6030 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/testclient.py
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/types.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/typing.py
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/websockets.py
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/__init__.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/enums.py
+-rw-r--r--   0        0        0    14737 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/global_settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/app_template/__init__.py-tpl
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/app_template/tests.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/app_template/directives/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/app_template/directives/operations/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/app_template/v1/__init__.py-tpl
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/app_template/v1/schemas.py-tpl
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/app_template/v1/urls.py-tpl
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/app_template/v1/views.py-tpl
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/project_template/.gitignore.e-tpl
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/project_template/Makefile.e-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/project_template/project_name/__init__.py-tpl
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/project_template/project_name/main.py-tpl
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/project_template/project_name/serve.py-tpl
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/project_template/project_name/urls.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/project_template/project_name/apps/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/project_template/project_name/configs/__init__.py-tpl
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/project_template/project_name/configs/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/project_template/project_name/configs/development/__init__.py-tpl
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/project_template/project_name/configs/development/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/project_template/project_name/configs/testing/__init__.py-tpl
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/project_template/project_name/configs/testing/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/project_template/project_name/tests/__init__.py-tpl
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/conf/project_template/project_name/tests/test_app.py-tpl
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/config/__init__.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/config/asyncexit.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/config/cors.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/config/csrf.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/config/jwt.py
+-rw-r--r--   0        0        0     5344 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/config/openapi.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/config/session.py
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/config/static_files.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/config/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/contrib/__init__.py
+-rw-r--r--   0        0        0     7517 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/contrib/encoding.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/contrib/auth/__init__.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/contrib/auth/constants.py
+-rw-r--r--   0        0        0     8616 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/contrib/auth/hashers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/contrib/auth/common/__init__.py
+-rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/contrib/auth/common/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/contrib/auth/saffier/__init__.py
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/contrib/auth/saffier/base_user.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/contrib/auth/saffier/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/directives/__init__.py
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/directives/base.py
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/directives/cli.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/directives/constants.py
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/directives/env.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/directives/exceptions.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/directives/parsers.py
+-rw-r--r--   0        0        0     6522 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/directives/templates.py
+-rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/directives/utils.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/directives/operations/__init__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/directives/operations/_constants.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/directives/operations/createapp.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/directives/operations/createproject.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/directives/operations/list.py
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/directives/operations/run.py
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/directives/operations/runserver.py
+-rw-r--r--   0        0        0     4046 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/directives/operations/show_urls.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/terminal/__init__.py
+-rw-r--r--   0        0        0     8301 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/terminal/base.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/terminal/print.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/terminal/terminal.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/urls/__init__.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/core/urls/base.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/datastructures/__init__.py
+-rw-r--r--   0        0        0     3813 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/datastructures/base.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/datastructures/encoders.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/datastructures/file.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/datastructures/json.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/datastructures/redirect.py
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/datastructures/stream.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/datastructures/template.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/datastructures/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/interceptors/__init__.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/interceptors/interceptor.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/interceptors/types.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/middleware/__init__.py
+-rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/middleware/_exception_handlers.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/middleware/asyncexitstack.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/middleware/authentication.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/middleware/basic.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/middleware/cors.py
+-rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/middleware/csrf.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/middleware/errors.py
+-rw-r--r--   0        0        0     6161 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/middleware/exceptions.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/middleware/gzip.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/middleware/https.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/middleware/sessions.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/middleware/settings_middleware.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/middleware/trustedhost.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/middleware/wsgi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/openapi/__init__.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/openapi/_internal.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/openapi/constants.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/openapi/datastructures.py
+-rw-r--r--   0        0        0     6142 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/openapi/docs.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/openapi/enums.py
+-rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/openapi/models.py
+-rw-r--r--   0        0        0    17266 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/openapi/openapi.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/openapi/params.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/openapi/responses.py
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/openapi/utils.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/permissions/__init__.py
+-rw-r--r--   0        0        0     6857 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/permissions/base.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/permissions/types.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/permissions/utils.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/pluggables/__init__.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/pluggables/base.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/protocols/__init__.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/protocols/asyncdao.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/protocols/dao.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/protocols/extension.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/protocols/interceptor.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/protocols/middleware.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/protocols/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/protocols/utils/__init__.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/protocols/utils/protocols.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/responses/__init__.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/responses/base.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/responses/encoders.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/responses/json.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/responses/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/routing/__init__.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/routing/_internal.py
+-rw-r--r--   0        0        0    22141 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/routing/base.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/routing/events.py
+-rw-r--r--   0        0        0     7436 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/routing/gateways.py
+-rw-r--r--   0        0        0    22735 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/routing/handlers.py
+-rw-r--r--   0        0        0    42063 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/routing/router.py
+-rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/routing/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/security/__init__.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/security/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/security/jwt/__init__.py
+-rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/security/jwt/token.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/template/__init__.py
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/template/jinja.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/template/mako.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/transformers/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/transformers/constants.py
+-rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/transformers/datastructures.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/transformers/helpers.py
+-rw-r--r--   0        0        0    14628 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/transformers/model.py
+-rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/transformers/signature.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/transformers/types.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/transformers/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/utils/__init__.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/utils/constants.py
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/utils/crypto.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/utils/dependency.py
+-rw-r--r--   0        0        0     7143 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/utils/functional.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/utils/helpers.py
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/utils/model.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/utils/module_loading.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/utils/sync.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/utils/url.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/utils/pydantic/__init__.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 esmerald-2.0.0/esmerald/utils/pydantic/schema.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 esmerald-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 esmerald-2.0.0/LICENSE
+-rw-r--r--   0        0        0    15810 2020-02-02 00:00:00.000000 esmerald-2.0.0/README.md
+-rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 esmerald-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    21018 2020-02-02 00:00:00.000000 esmerald-2.0.0/PKG-INFO
```

### Comparing `esmerald-1.3.0/esmerald/__init__.py` & `esmerald-2.0.0/esmerald/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.3.0"
+__version__ = "2.0.0"
 
 
 from starlette import status
 
 from esmerald.conf import settings
 from esmerald.conf.global_settings import EsmeraldAPISettings
 from esmerald.injector import Inject
```

### Comparing `esmerald-1.3.0/esmerald/applications.py` & `esmerald-2.0.0/esmerald/applications.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Sequence,
     Type,
     TypeVar,
     Union,
     cast,
 )
 
-from openapi_schemas_pydantic.v3_1_0 import Contact, License, SecurityRequirement, Server, Tag
+from openapi_schemas_pydantic.v3_1_0 import Contact, License, SecurityScheme, Tag
 from openapi_schemas_pydantic.v3_1_0.open_api import OpenAPI
 from pydantic import AnyUrl
 from starlette.applications import Starlette
 from starlette.middleware import Middleware as StarletteMiddleware  # noqa
 from starlette.types import Lifespan, Receive, Scope, Send
 
 from esmerald.conf import settings as esmerald_settings
@@ -126,24 +126,25 @@
         title: Optional[str] = None,
         version: Optional[str] = None,
         summary: Optional[str] = None,
         description: Optional[str] = None,
         contact: Optional[Contact] = None,
         terms_of_service: Optional[AnyUrl] = None,
         license: Optional[License] = None,
-        security: Optional[List[SecurityRequirement]] = None,
-        servers: Optional[List[Server]] = None,
+        security: Optional[List[SecurityScheme]] = None,
+        servers: Optional[List[Dict[str, Union[str, Any]]]] = None,
         secret_key: Optional[str] = None,
         allowed_hosts: Optional[List[str]] = None,
         allow_origins: Optional[List[str]] = None,
         permissions: Optional[Sequence["Permission"]] = None,
         interceptors: Optional[Sequence["Interceptor"]] = None,
         dependencies: Optional["Dependencies"] = None,
         csrf_config: Optional["CSRFConfig"] = None,
         openapi_config: Optional["OpenAPIConfig"] = None,
+        openapi_version: Optional[str] = None,
         cors_config: Optional["CORSConfig"] = None,
         static_files_config: Optional["StaticFilesConfig"] = None,
         template_config: Optional["TemplateConfig"] = None,
         session_config: Optional["SessionConfig"] = None,
         response_class: Optional["ResponseType"] = None,
         response_cookies: Optional["ResponseCookies"] = None,
         response_headers: Optional["ResponseHeaders"] = None,
@@ -162,14 +163,26 @@
         tags: Optional[List[Tag]] = None,
         include_in_schema: Optional[bool] = None,
         deprecated: Optional[bool] = None,
         enable_openapi: Optional[bool] = None,
         redirect_slashes: Optional[bool] = None,
         pluggables: Optional[Dict[str, Pluggable]] = None,
         parent: Optional[Union["ParentType", "Esmerald", "ChildEsmerald"]] = None,
+        root_path_in_servers: bool = None,
+        openapi_url: Optional[str] = None,
+        docs_url: Optional[str] = None,
+        redoc_url: Optional[str] = None,
+        swagger_ui_oauth2_redirect_url: Optional[str] = None,
+        redoc_js_url: Optional[str] = None,
+        redoc_favicon_url: Optional[str] = None,
+        swagger_ui_init_oauth: Optional[Dict[str, Any]] = None,
+        swagger_ui_parameters: Optional[Dict[str, Any]] = None,
+        swagger_js_url: Optional[str] = None,
+        swagger_css_url: Optional[str] = None,
+        swagger_favicon_url: Optional[str] = None,
     ) -> None:
         self.settings_config = None
 
         if settings_config:
             if not isinstance(settings_config, EsmeraldAPISettings) and not is_class_and_subclass(
                 settings_config, EsmeraldAPISettings
             ):
@@ -192,26 +205,30 @@
 
         self._debug = (
             debug
             if debug is not None
             else self.get_settings_value(self.settings_config, esmerald_settings, "debug")
         )
         self.debug = self._debug
+
         self.title = title or self.get_settings_value(
             self.settings_config, esmerald_settings, "title"
         )
         self.app_name = app_name or self.get_settings_value(
             self.settings_config, esmerald_settings, "app_name"
         )
         self.description = description or self.get_settings_value(
             self.settings_config, esmerald_settings, "app_name"
         )
         self.version = version or self.get_settings_value(
             self.settings_config, esmerald_settings, "version"
         )
+        self.openapi_version = openapi_version or self.get_settings_value(
+            self.settings_config, esmerald_settings, "openapi_version"
+        )
         self.summary = summary or self.get_settings_value(
             self.settings_config, esmerald_settings, "summary"
         )
         self.contact = contact or self.get_settings_value(
             self.settings_config, esmerald_settings, "contact"
         )
         self.terms_of_service = terms_of_service or self.get_settings_value(
@@ -348,14 +365,103 @@
         )
         self.pluggables = (
             pluggables
             if pluggables
             else self.get_settings_value(self.settings_config, esmerald_settings, "pluggables")
         )
 
+        # OpenAPI Related
+        self.root_path_in_servers = (
+            root_path_in_servers
+            if root_path_in_servers is not None
+            else self.get_settings_value(
+                self.settings_config, esmerald_settings, "root_path_in_servers"
+            )
+        )
+        if not self.include_in_schema or not self.enable_openapi:
+            self.root_path_in_servers = False
+
+        self.openapi_url = (
+            openapi_url
+            if openapi_url
+            else self.get_settings_value(self.settings_config, esmerald_settings, "openapi_url")
+        )
+
+        self.docs_url = (
+            docs_url
+            if docs_url
+            else self.get_settings_value(self.settings_config, esmerald_settings, "docs_url")
+        )
+
+        self.redoc_url = (
+            redoc_url
+            if redoc_url
+            else self.get_settings_value(self.settings_config, esmerald_settings, "redoc_url")
+        )
+
+        self.swagger_ui_oauth2_redirect_url = (
+            swagger_ui_oauth2_redirect_url
+            if swagger_ui_oauth2_redirect_url
+            else self.get_settings_value(
+                self.settings_config, esmerald_settings, "swagger_ui_oauth2_redirect_url"
+            )
+        )
+
+        self.redoc_js_url = (
+            redoc_js_url
+            if redoc_js_url
+            else self.get_settings_value(self.settings_config, esmerald_settings, "redoc_js_url")
+        )
+
+        self.redoc_favicon_url = (
+            redoc_favicon_url
+            if redoc_favicon_url
+            else self.get_settings_value(
+                self.settings_config, esmerald_settings, "redoc_favicon_url"
+            )
+        )
+
+        self.swagger_ui_init_oauth = (
+            swagger_ui_init_oauth
+            if swagger_ui_init_oauth
+            else self.get_settings_value(
+                self.settings_config, esmerald_settings, "swagger_ui_init_oauth"
+            )
+        )
+
+        self.swagger_ui_parameters = (
+            swagger_ui_parameters
+            if swagger_ui_parameters
+            else self.get_settings_value(
+                self.settings_config, esmerald_settings, "swagger_ui_parameters"
+            )
+        )
+
+        self.swagger_js_url = (
+            swagger_js_url
+            if swagger_js_url
+            else self.get_settings_value(self.settings_config, esmerald_settings, "swagger_js_url")
+        )
+
+        self.swagger_css_url = (
+            swagger_css_url
+            if swagger_css_url
+            else self.get_settings_value(
+                self.settings_config, esmerald_settings, "swagger_css_url"
+            )
+        )
+
+        self.swagger_favicon_url = (
+            swagger_favicon_url
+            if swagger_favicon_url
+            else self.get_settings_value(
+                self.settings_config, esmerald_settings, "swagger_favicon_url"
+            )
+        )
+
         self.openapi_schema: Optional["OpenAPI"] = None
         self.state = State()
         self.async_exit_config = esmerald_settings.async_exit_config
 
         self.router: "Router" = Router(
             on_shutdown=self.on_shutdown,
             on_startup=self.on_startup,
@@ -419,29 +525,77 @@
         if local_settings:
             setting_value = getattr(local_settings, value, None)
         if not setting_value:
             return getattr(global_settings, value, None)
         return setting_value
 
     def activate_openapi(self) -> None:
-        if self.openapi_config and self.enable_openapi:
-            self.openapi_schema = self.openapi_config.create_openapi_schema_model(self)
-            gateway = gateways.Gateway(handler=self.openapi_config.openapi_apiview)  # type: ignore
-            self.add_apiview(value=gateway)
+        if self.enable_openapi:
+            if self.title or not self.openapi_config.title:
+                self.openapi_config.title = self.title
+            if self.version or not self.openapi_config.version:
+                self.openapi_config.version = self.version
+            if self.openapi_version or not self.openapi_config.openapi_version:
+                self.openapi_config.openapi_version = self.openapi_version
+            if self.summary or not self.openapi_config.summary:
+                self.openapi_config.summary = self.summary
+            if self.description or not self.openapi_config.description:
+                self.openapi_config.description = self.description
+            if self.tags or not self.openapi_config.tags:
+                self.openapi_config.tags = self.tags
+            if self.servers or not self.openapi_config.servers:
+                self.openapi_config.servers = self.servers
+            if self.terms_of_service or not self.openapi_config.terms_of_service:
+                self.openapi_config.terms_of_service = self.terms_of_service
+            if self.contact or not self.openapi_config.contact:
+                self.openapi_config.contact = self.contact
+            if self.license or not self.openapi_config.license:
+                self.openapi_config.license = self.license
+            if self.root_path_in_servers or not self.openapi_config.root_path_in_servers:
+                self.openapi_config.root_path_in_servers = self.root_path_in_servers
+            if self.docs_url or not self.openapi_config.docs_url:
+                self.openapi_config.docs_url = self.docs_url
+            if self.redoc_url or not self.openapi_config.redoc_url:
+                self.openapi_config.redoc_url = self.redoc_url
+            if (
+                self.swagger_ui_oauth2_redirect_url
+                or not self.openapi_config.swagger_ui_oauth2_redirect_url
+            ):
+                self.openapi_config.swagger_ui_oauth2_redirect_url = (
+                    self.swagger_ui_oauth2_redirect_url
+                )
+            if self.redoc_js_url or not self.openapi_config.redoc_js_url:
+                self.openapi_config.redoc_js_url = self.redoc_js_url
+            if self.redoc_favicon_url or not self.openapi_config.redoc_favicon_url:
+                self.openapi_config.redoc_favicon_url = self.redoc_favicon_url
+            if self.swagger_ui_init_oauth or not self.openapi_config.swagger_ui_init_oauth:
+                self.openapi_config.swagger_ui_init_oauth = self.swagger_ui_init_oauth
+            if self.swagger_ui_parameters or not self.openapi_config.swagger_ui_parameters:
+                self.openapi_config.swagger_ui_parameters = self.swagger_ui_parameters
+            if self.swagger_js_url or not self.openapi_config.swagger_js_url:
+                self.openapi_config.swagger_js_url = self.swagger_js_url
+            if self.swagger_css_url or not self.openapi_config.swagger_css_url:
+                self.openapi_config.swagger_css_url = self.swagger_css_url
+            if self.swagger_favicon_url or not self.openapi_config.swagger_favicon_url:
+                self.openapi_config.swagger_favicon_url = self.swagger_favicon_url
+            if self.openapi_url or not self.openapi_config.openapi_url:
+                self.openapi_config.openapi_url = self.openapi_url
+
+            self.openapi_config.enable(self)
 
     def get_template_engine(
         self, template_config: "TemplateConfig"
     ) -> Optional["TemplateEngineProtocol"]:
         """
         Returns the template engine for the application.
         """
         if not template_config:
             return None
 
-        engine = template_config.engine(template_config.directory)
+        engine: "TemplateEngineProtocol" = template_config.engine(template_config.directory)
         return engine
 
     def add_apiview(
         self,
         value: Union["gateways.Gateway", "gateways.WebSocketGateway"],
     ) -> None:
         """
@@ -457,14 +611,15 @@
         dependencies: Optional["Dependencies"] = None,
         exception_handlers: Optional["ExceptionHandlerMap"] = None,
         interceptors: Optional[List["Interceptor"]] = None,
         permissions: Optional[List["Permission"]] = None,
         middleware: Optional[List["Middleware"]] = None,
         name: Optional[str] = None,
         include_in_schema: bool = True,
+        activate_openapi: bool = True,
     ) -> None:
         """
         Adds a route into the router.
         """
         router = router or self.router
         router.add_route(
             path=path,
@@ -474,15 +629,16 @@
             interceptors=interceptors,
             permissions=permissions,
             middleware=middleware,
             name=name,
             include_in_schema=include_in_schema,
         )
 
-        self.activate_openapi()
+        if activate_openapi:
+            self.activate_openapi()
 
     def add_websocket_route(
         self,
         path: str,
         handler: "WebSocketHandler",
         router: Optional["Router"] = None,
         dependencies: Optional["Dependencies"] = None,
@@ -517,15 +673,15 @@
         middleware: Optional[Sequence["Middleware"]] = None,
         dependencies: Optional["Dependencies"] = None,
         exception_handlers: Optional["ExceptionHandlerMap"] = None,
         interceptors: Optional[List["Interceptor"]] = None,
         permissions: Optional[List["Permission"]] = None,
         include_in_schema: Optional[bool] = True,
         deprecated: Optional[bool] = None,
-        security: Optional[List["SecurityRequirement"]] = None,
+        security: Optional[List["SecurityScheme"]] = None,
     ) -> None:
         """
         Adds a child esmerald into the application routers.
         """
         if not isinstance(child, ChildEsmerald):
             raise ImproperlyConfigured("The child must be an instance of a ChildEsmerald.")
```

### Comparing `esmerald-1.3.0/esmerald/backgound.py` & `esmerald-2.0.0/esmerald/backgound.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/enums.py` & `esmerald-2.0.0/esmerald/enums.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 class MediaType(str, Enum):
     JSON = "application/json"
     HTML = "text/html"
     TEXT = "text/plain"
     TEXT_CHARSET = "text/plain; charset=utf-8"
     PNG = "image/png"
+    OCTET = "application/octet-stream"
 
 
 class OpenAPIMediaType(str, Enum):
     OPENAPI_YAML = "application/vnd.oai.openapi"
     OPENAPI_JSON = "application/vnd.oai.openapi+json"
```

### Comparing `esmerald-1.3.0/esmerald/exception_handlers.py` & `esmerald-2.0.0/esmerald/exception_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Union
 
-from pydantic.error_wrappers import ValidationError
+from pydantic import ValidationError
 from starlette import status
 from starlette.exceptions import HTTPException as StarletteHTTPException
 from starlette.requests import Request
 from starlette.responses import Response as StarletteResponse
 
 from esmerald.enums import MediaType
 from esmerald.exceptions import ExceptionErrorMap, HTTPException, ImproperlyConfigured
```

### Comparing `esmerald-1.3.0/esmerald/exceptions.py` & `esmerald-2.0.0/esmerald/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         super().__init__(*args, detail=f"Template {template_name} not found.")
 
 
 class MissingDependency(EsmeraldAPIException, ImportError):
     ...
 
 
-class OpenAPIError(ValueError):
+class OpenAPIException(ImproperlyConfigured):
     ...
 
 
 class WebSocketException(StarletteWebSocketException):
     ...
```

### Comparing `esmerald-1.3.0/esmerald/injector.py` & `esmerald-2.0.0/esmerald/injector.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from esmerald.parsers import ArbitraryHashableBaseModel
 from esmerald.transformers.datastructures import Signature
 from esmerald.typing import Void
 from esmerald.utils.helpers import is_async_callable
 
 if TYPE_CHECKING:
-    from pydantic.typing import AnyCallable
+    from esmerald.typing import AnyCallable
 
 
 class Inject(ArbitraryHashableBaseModel):
     def __init__(self, dependency: "AnyCallable", use_cache: bool = False, **kwargs: Any):
         super().__init__(**kwargs)
         self.dependency = dependency
         self.signature_model: Optional["Type[Signature]"] = None
```

### Comparing `esmerald-1.3.0/esmerald/logging.py` & `esmerald-2.0.0/esmerald/logging.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/parsers.py` & `esmerald-2.0.0/esmerald/parsers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from contextlib import suppress
 from json import JSONDecodeError, loads
 from typing import TYPE_CHECKING, Any, Dict
 
-from pydantic import BaseConfig, BaseModel
-from pydantic.fields import SHAPE_LIST, SHAPE_SINGLETON
+from pydantic import BaseModel, ConfigDict
+from pydantic.v1.fields import SHAPE_LIST, SHAPE_SINGLETON
 
 from esmerald.datastructures import UploadFile
 from esmerald.enums import EncodingType
 
 if TYPE_CHECKING:
-    from pydantic.fields import ModelField
-    from pydantic.typing import DictAny
+    from pydantic.fields import FieldInfo
     from starlette.datastructures import FormData
 
 
 class HashableBaseModel(BaseModel):
     """
     Pydantic BaseModel by default doesn't handle with hashable types the same way
     a python object would and therefore there are types that are mutable (list, set)
@@ -35,49 +34,49 @@
 
 
 class ArbitraryHashableBaseModel(HashableBaseModel):
     """
     Same as HashableBaseModel but allowing arbitrary values
     """
 
-    class Config:
-        extra = "allow"
-        arbitrary_types_allowed = True
+    model_config = ConfigDict(extra="allow", arbitrary_types_allowed=True)
 
 
 class BaseModelExtra(BaseModel):
     """
     BaseModel that allows extra to be passed.
     """
 
-    class Config:
-        extra = "allow"
+    model_config = ConfigDict(extra="allow")
 
 
 class ArbitraryBaseModel(BaseModel):
     """
     ArbitratyBaseModel that allows arbitrary_types_allowed to be passed.
     """
 
-    class Config(BaseConfig):
-        arbitrary_types_allowed = True
+    model_config = ConfigDict(arbitrary_types_allowed=True)
 
 
-def validate_media_type(field: "ModelField", values: Any) -> Any:
+class ArbitraryExtraBaseModel(BaseModel):
+    model_config = ConfigDict(extra="allow", arbitrary_types_allowed=True)
+
+
+def validate_media_type(field: "FieldInfo", values: Any) -> Any:
     """
     Validates the media type against the available types.
     """
     if field.shape == SHAPE_LIST:
         return list(values.values())
     if field.shape == SHAPE_SINGLETON and field.type_in[UploadFile] and values:
         return list(values.values())[0]
 
 
-def parse_form_data(media_type: "EncodingType", form_data: "FormData", field: "ModelField") -> Any:
-    values: "DictAny" = {}
+def parse_form_data(media_type: "EncodingType", form_data: "FormData", field: "FieldInfo") -> Any:
+    values: Any = {}
     for key, value in form_data.multi_items():
         if not isinstance(value, UploadFile):
             with suppress(JSONDecodeError):
                 value = loads(value)
         if isinstance(value, UploadFile):
             value = UploadFile(
                 file=value.file,
```

### Comparing `esmerald-1.3.0/esmerald/requests.py` & `esmerald-2.0.0/esmerald/requests.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/testclient.py` & `esmerald-2.0.0/esmerald/testclient.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,16 @@
     Optional,
     Union,
     cast,
 )
 
 import httpx  # noqa
 from httpx._client import CookieTypes
+from openapi_schemas_pydantic.v3_1_0 import Contact, License, SecurityScheme, Tag
+from pydantic import AnyUrl
 from starlette.testclient import TestClient  # noqa
 
 from esmerald.applications import Esmerald
 from esmerald.utils.crypto import get_random_secret_key
 
 if TYPE_CHECKING:
     from typing_extensions import Literal
@@ -72,14 +74,23 @@
 
 def create_client(
     routes: Union["APIGateHandler", List["APIGateHandler"]],
     *,
     settings_config: Optional["SettingsType"] = None,
     debug: Optional[bool] = None,
     app_name: Optional[str] = None,
+    title: Optional[str] = None,
+    version: Optional[str] = None,
+    summary: Optional[str] = None,
+    description: Optional[str] = None,
+    contact: Optional[Contact] = None,
+    terms_of_service: Optional[AnyUrl] = None,
+    license: Optional[License] = None,
+    security: Optional[List[SecurityScheme]] = None,
+    servers: Optional[List[Dict[str, Union[str, Any]]]] = None,
     secret_key: Optional[str] = get_random_secret_key(),
     allowed_hosts: Optional[List[str]] = None,
     allow_origins: Optional[List[str]] = None,
     base_url: str = "http://testserver",
     backend: "Literal['asyncio', 'trio']" = "asyncio",
     backend_options: Optional[Dict[str, Any]] = None,
     interceptors: Optional[List["Interceptor"]] = None,
@@ -93,26 +104,39 @@
     on_startup: Optional[List["LifeSpanHandler"]] = None,
     cors_config: Optional["CORSConfig"] = None,
     session_config: Optional["SessionConfig"] = None,
     scheduler_class: Optional["SchedulerType"] = None,
     scheduler_tasks: Optional[Dict[str, str]] = None,
     scheduler_configurations: Optional[Dict[str, Union[str, Dict[str, str]]]] = None,
     enable_scheduler: bool = None,
+    enable_openapi: bool = True,
+    include_in_schema: bool = True,
+    openapi_version: Optional[str] = "3.1.0",
     raise_server_exceptions: bool = True,
     root_path: str = "",
     static_files_config: Optional["StaticFilesConfig"] = None,
     template_config: Optional["TemplateConfig"] = None,
     lifespan: Optional[Callable[["Esmerald"], "AsyncContextManager"]] = None,
     cookies: Optional[CookieTypes] = None,
     redirect_slashes: Optional[bool] = None,
+    tags: Optional[List[Tag]] = None,
 ) -> EsmeraldTestClient:
     return EsmeraldTestClient(
         app=Esmerald(
             settings_config=settings_config,
             debug=debug,
+            title=title,
+            version=version,
+            summary=summary,
+            description=description,
+            contact=contact,
+            terms_of_service=terms_of_service,
+            license=license,
+            security=security,
+            servers=servers,
             routes=cast("Any", routes if isinstance(routes, list) else [routes]),
             app_name=app_name,
             secret_key=secret_key,
             allowed_hosts=allowed_hosts,
             allow_origins=allow_origins,
             interceptors=interceptors,
             permissions=permissions,
@@ -129,14 +153,18 @@
             scheduler_configurations=scheduler_configurations,
             enable_scheduler=enable_scheduler,
             static_files_config=static_files_config,
             template_config=template_config,
             session_config=session_config,
             lifespan=lifespan,
             redirect_slashes=redirect_slashes,
+            enable_openapi=enable_openapi,
+            openapi_version=openapi_version,
+            include_in_schema=include_in_schema,
+            tags=tags,
         ),
         base_url=base_url,
         backend=backend,
         backend_options=backend_options,
         root_path=root_path,
         raise_server_exceptions=raise_server_exceptions,
         cookies=cookies,
```

### Comparing `esmerald-1.3.0/esmerald/types.py` & `esmerald-2.0.0/esmerald/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     Gateway,
     WebSocketGateway,
 ]
 
 RouteParent = Union["Router", "Include", "ASGIApp", "Gateway", "WebSocketGateway"]
 
 BackgroundTaskType = Union[BackgroundTask, BackgroundTasks]
-SecurityRequirement = Dict[str, List[str]]
+SecurityScheme = Dict[str, List[str]]
 
 ConnectionType = Union["Request", "WebSocket"]
 DictStr = Dict[str, str]
 DictAny = Dict[str, Any]
 SettingsType = Type["EsmeraldAPISettings"]
 
 LifeSpanHandler = Union[
```

### Comparing `esmerald-1.3.0/esmerald/websockets.py` & `esmerald-2.0.0/esmerald/websockets.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/conf/__init__.py` & `esmerald-2.0.0/esmerald/conf/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         """
         settings_module: str = os.environ.get(
             ENVIRONMENT_VARIABLE, "esmerald.conf.global_settings.EsmeraldAPISettings"
         )
 
         settings: Any = import_string(settings_module)
 
-        for setting, _ in settings().dict().items():
+        for setting, _ in settings().model_dump().items():
             assert setting.islower(), "%s should be in lowercase." % setting
 
         self._wrapped = settings()
 
     def __repr__(self: "EsmeraldLazySettings") -> str:
         # Hardcode the class name as otherwise it yields 'Settings'.
         if self._wrapped is empty:
```

### Comparing `esmerald-1.3.0/esmerald/conf/project_template/.gitignore.e-tpl` & `esmerald-2.0.0/esmerald/conf/project_template/.gitignore.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/conf/project_template/Makefile.e-tpl` & `esmerald-2.0.0/esmerald/conf/project_template/Makefile.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/conf/project_template/project_name/main.py-tpl` & `esmerald-2.0.0/esmerald/conf/project_template/project_name/main.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/conf/project_template/project_name/serve.py-tpl` & `esmerald-2.0.0/esmerald/conf/project_template/project_name/serve.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/conf/project_template/project_name/urls.py-tpl` & `esmerald-2.0.0/esmerald/conf/project_template/project_name/urls.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/conf/project_template/project_name/configs/settings.py-tpl` & `esmerald-2.0.0/esmerald/conf/project_template/project_name/configs/settings.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/config/jwt.py` & `esmerald-2.0.0/esmerald/config/jwt.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/config/static_files.py` & `esmerald-2.0.0/esmerald/config/static_files.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,28 @@
-from typing import TYPE_CHECKING, Dict, List, Optional, Tuple, Union
+from pathlib import Path
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
-from pydantic import BaseModel, DirectoryPath, constr, validator
+from pydantic import BaseModel, DirectoryPath, constr, field_validator
 from starlette.staticfiles import StaticFiles
 
 from esmerald.utils.url import clean_path
 
 if TYPE_CHECKING:
     from starlette.types import ASGIApp
 
 
 class StaticFilesConfig(BaseModel):
     path: constr(min_length=1)  # type: ignore
-    directory: Optional[DirectoryPath] = None
+    directory: Optional[Union[DirectoryPath, str, Path, Any]] = None
     html: bool = False
     packages: Optional[List[Union[str, Tuple[str, str]]]] = None
     check_dir: bool = True
 
-    @validator("path")
-    def validate_path(cls, value: str) -> str:  # pylint: disable=no-self-argument
+    @field_validator("path")
+    def validate_path(cls, value: str) -> str:
         if "{" in value:
             raise ValueError("path parameters are not supported for static files")
         return clean_path(value)
 
     def _build_kwargs(
         self,
     ) -> Dict[str, Union[bool, int, DirectoryPath, List[Union[str, Tuple[str, str]]]]]:
```

### Comparing `esmerald-1.3.0/esmerald/contrib/encoding.py` & `esmerald-2.0.0/esmerald/contrib/encoding.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/contrib/auth/hashers.py` & `esmerald-2.0.0/esmerald/contrib/auth/hashers.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/contrib/auth/common/middleware.py` & `esmerald-2.0.0/esmerald/contrib/auth/common/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/contrib/auth/saffier/base_user.py` & `esmerald-2.0.0/esmerald/contrib/auth/saffier/base_user.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/contrib/auth/saffier/middleware.py` & `esmerald-2.0.0/esmerald/contrib/auth/saffier/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/core/directives/base.py` & `esmerald-2.0.0/esmerald/core/directives/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import argparse
 import os
 import sys
 from abc import ABC, abstractmethod
 from typing import Any, Type
 
-from pydantic import BaseConfig, BaseModel
-
 import esmerald
 from esmerald.core.directives.exceptions import DirectiveError
 from esmerald.core.directives.parsers import DirectiveParser
 from esmerald.core.terminal.print import Print
+from esmerald.parsers import ArbitraryExtraBaseModel
 from esmerald.utils.helpers import is_async_callable
 
 printer = Print()
 
 
-class BaseDirective(BaseModel, ABC):
+class BaseDirective(ArbitraryExtraBaseModel, ABC):
     """The base class from which all directrives derive"""
 
     help: str = ""
 
     def get_version(self) -> str:
         """
         Returns the current version of Esmerald.
@@ -70,11 +69,7 @@
             printer.write_info(output)
         return output
 
     @abstractmethod
     def handle(self, *args: Any, **options: Any) -> Any:
         """The logic of the directive. Subclasses must implement this method"""
         raise NotImplementedError("subclasses of BaseDirective must provide a handle() method.")
-
-    class Config(BaseConfig):
-        extra = "allow"  # type: ignore
-        arbitrary_types_allowed = True
```

### Comparing `esmerald-1.3.0/esmerald/core/directives/cli.py` & `esmerald-2.0.0/esmerald/core/directives/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             except OSError as e:
                 if not any(value in sys.argv for value in IGNORE_DIRECTIVES):
                     printer.write_error(str(e))
                     sys.exit(1)
         return super().invoke(ctx)
 
 
-@click.group(
+@click.group(  # type: ignore
     cls=DirectiveGroup,
 )
 @click.option(
     APP_PARAMETER,
     "path",
     help="Module path to the application to generate the migrations. In a module:path formatyping.",
 )
```

### Comparing `esmerald-1.3.0/esmerald/core/directives/env.py` & `esmerald-2.0.0/esmerald/core/directives/env.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/core/directives/templates.py` & `esmerald-2.0.0/esmerald/core/directives/templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,15 @@
 
 class TemplateDirective(BaseDirective):
     """
     Copy either an Esmerald application layout template or an Esmerald project
     layout.
     """
 
-    url_schemes = ["http", "https", "ftp"]
-
-    rewrite_template_suffixes = (
+    rewrite_template_suffixes: Any = (
         (".py-tpl", ".py"),
         (".e-tpl", ""),
     )
 
     def handle(self, app_or_project: str, name: str, **options: Any) -> Any:
         self.app_or_project = app_or_project
         self.name = name
```

### Comparing `esmerald-1.3.0/esmerald/core/directives/utils.py` & `esmerald-2.0.0/esmerald/core/directives/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/core/directives/operations/createapp.py` & `esmerald-2.0.0/esmerald/core/directives/operations/createapp.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from esmerald.core.directives.templates import TemplateDirective
 from esmerald.core.terminal import Print
 from esmerald.utils.crypto import get_random_secret_key
 
 printer = Print()
 
 
-@click.option("-v", "--verbosity", default=1, type=int, help="Displays the files generated")
+@click.option("-v", "--verbosity", default=1, type=int, help="Displays the files generated")  # type: ignore
 @click.argument("name", type=str)
 @click.command(name="createapp")
 def create_app(name: str, verbosity: int) -> None:
     """Creates the scaffold of an application
 
     How to run: `esmerald createapp <NAME>`
```

### Comparing `esmerald-1.3.0/esmerald/core/directives/operations/createproject.py` & `esmerald-2.0.0/esmerald/core/directives/operations/createproject.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from esmerald.core.directives.templates import TemplateDirective
 from esmerald.core.terminal import Print
 from esmerald.utils.crypto import get_random_secret_key
 
 printer = Print()
 
 
-@click.option("-v", "--verbosity", default=1, type=int, help="Displays the files generated")
+@click.option("-v", "--verbosity", default=1, type=int, help="Displays the files generated")  # type: ignore
 @click.argument("name", type=str)
 @click.command(name="createproject")
 def create_project(name: str, verbosity: int) -> None:
     """
     Creates the scaffold of a project.
 
     How to run: `esmerald createproject <NAME>`
```

### Comparing `esmerald-1.3.0/esmerald/core/directives/operations/list.py` & `esmerald-2.0.0/esmerald/core/directives/operations/list.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/core/directives/operations/run.py` & `esmerald-2.0.0/esmerald/core/directives/operations/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 
 class Position(int, Enum):
     DEFAULT = 5
     BACK = 3
 
 
-@click.option(
+@click.option(  # type: ignore
     "--directive",
     "directive",
     required=True,
     help=("The name of the file of the custom directive to run."),
 )
 @click.argument("directive_args", nargs=-1, type=click.UNPROCESSED)
 @click.command(
```

### Comparing `esmerald-1.3.0/esmerald/core/directives/operations/runserver.py` & `esmerald-2.0.0/esmerald/core/directives/operations/runserver.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 if TYPE_CHECKING:
     pass
 
 printer = Print()
 terminal = Terminal()
 
 
-@click.option(
+@click.option(  # type: ignore
     "-p",
     "--port",
     type=int,
     default=8000,
     help="Port to run the development server.",
     show_default=True,
 )
```

### Comparing `esmerald-1.3.0/esmerald/core/directives/operations/show_urls.py` & `esmerald-2.0.0/esmerald/core/directives/operations/show_urls.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/core/terminal/base.py` & `esmerald-2.0.0/esmerald/core/terminal/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/core/terminal/print.py` & `esmerald-2.0.0/esmerald/core/terminal/print.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/core/terminal/terminal.py` & `esmerald-2.0.0/esmerald/core/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/core/urls/base.py` & `esmerald-2.0.0/esmerald/core/urls/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/datastructures/__init__.py` & `esmerald-2.0.0/esmerald/datastructures/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/datastructures/base.py` & `esmerald-2.0.0/esmerald/datastructures/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from abc import ABC, abstractmethod
 from copy import copy
 from http.cookies import SimpleCookie
 from typing import TYPE_CHECKING, Any, Dict, Generic, List, Optional, Type, TypeVar, Union
 
-from pydantic import BaseConfig, BaseModel, validator  # noqa
-from pydantic.generics import GenericModel  # noqa
+from pydantic import BaseModel, ConfigDict, field_validator  # noqa
 from starlette.datastructures import URL as URL  # noqa: F401
 from starlette.datastructures import Address as Address  # noqa: F401
 from starlette.datastructures import FormData as FormData  # noqa: F401
 from starlette.datastructures import Headers as Headers  # noqa: F401
 from starlette.datastructures import MutableHeaders as MutableHeaders  # noqa
 from starlette.datastructures import QueryParams as QueryParams  # noqa: F401
 from starlette.datastructures import State as StarletteStateClass  # noqa: F401
@@ -79,25 +78,23 @@
     description: Optional[str] = None
 
     def to_header(self, **kwargs: Any) -> str:
         simple_cookie: SimpleCookie = SimpleCookie()
         simple_cookie[self.key] = self.value or ""
         if self.max_age:
             simple_cookie[self.key]["max-age"] = self.max_age
-        cookie_dict = self.dict()
+        cookie_dict = self.model_dump()
         for key in ["expires", "path", "domain", "secure", "httponly", "samesite"]:
             if cookie_dict[key] is not None:
                 simple_cookie[self.key][key] = cookie_dict[key]
         return simple_cookie.output(**kwargs).strip()
 
 
-class ResponseContainer(GenericModel, ABC, Generic[R]):
-    class Config(BaseConfig):
-        arbitrary_types_allowed = True
-
+class ResponseContainer(BaseModel, ABC, Generic[R]):
+    model_config = ConfigDict(arbitrary_types_allowed=True)
     background: Optional[Union[BackgroundTask, BackgroundTasks]] = None
     headers: Dict[str, Any] = {}
     cookies: List[Cookie] = []
 
     @abstractmethod
     def to_response(
         self,
@@ -106,15 +103,13 @@
         status_code: int,
         app: Type["Esmerald"],
     ) -> R:  # pragma: no cover
         raise NotImplementedError("not implemented")
 
 
 class ResponseHeader(BaseModel):
-    value: Any = None
+    value: Optional[Any] = None
 
-    @validator("value", always=True)
-    def validate_value(
-        cls, value: Any, values: Dict[str, Any]
-    ) -> Any:  # pylint: disable=no-self-argument
+    @field_validator("value")  # type: ignore
+    def validate_value(cls, value: Any, values: Dict[str, Any]) -> Any:
         if value is not None:
             return value
```

### Comparing `esmerald-1.3.0/esmerald/datastructures/encoders.py` & `esmerald-2.0.0/esmerald/datastructures/encoders.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 try:
     from esmerald.responses.encoders import UJSONResponse
 except ImportError:
     UJSONResponse = None  # type: ignore
 
 
 class OrJSON(ResponseContainer[ORJSONResponse]):
+    media_type: str = "application/json"
     content: Optional[Dict[str, Any]] = None
     status_code: Optional[int] = None
 
     def __init__(
         self,
         content: Optional[Dict[str, Any]] = None,
         status_code: Optional[int] = None,
@@ -49,14 +50,15 @@
             status_code=status,
             media_type=media_type,
             background=self.background,
         )
 
 
 class UJSON(ResponseContainer[UJSONResponse]):
+    media_type: str = "application/json"
     content: Optional[Dict[str, Any]] = None
     status_code: Optional[int] = None
 
     def __init__(
         self,
         content: Optional[Dict[str, Any]] = None,
         status_code: Optional[int] = None,
```

### Comparing `esmerald-1.3.0/esmerald/datastructures/file.py` & `esmerald-2.0.0/esmerald/datastructures/file.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import os
 from typing import TYPE_CHECKING, Any, Dict, Optional, Type, Union, cast
 
-from pydantic import FilePath, validator  # noqa
+from pydantic import FilePath, field_validator, model_validator  # noqa
 from starlette.responses import FileResponse  # noqa
 
 from esmerald.datastructures.base import ResponseContainer
 
 if TYPE_CHECKING:
     from esmerald.applications import Esmerald
     from esmerald.enums import MediaType
 
 
 class File(ResponseContainer[FileResponse]):
     path: FilePath
     filename: str
     stat_result: Optional[os.stat_result] = None
 
-    @validator("stat_result", always=True)
-    def validate_status_code(  # pylint: disable=no-self-argument
-        cls, value: Optional[os.stat_result], values: Dict[str, Any]
-    ) -> os.stat_result:
-        """Set the stat_result value for the given filepath."""
-        return value or os.stat(cast("str", values.get("path")))
+    @model_validator(mode="before")
+    def validate_fields(cls, values: Dict[str, Any]) -> Any:
+        stat_result = values.get("stat_result")
+        values["stat_result"] = stat_result or os.stat(cast("str", values.get("path")))
+        return values
 
     def to_response(
         self,
         headers: Dict[str, Any],
         media_type: Union["MediaType", str],
         status_code: int,
         app: Type["Esmerald"],
```

### Comparing `esmerald-1.3.0/esmerald/datastructures/json.py` & `esmerald-2.0.0/esmerald/datastructures/json.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,24 +11,26 @@
 class JSON(ResponseContainer[JSONResponse]):
     """
     Returns a wrapper of a JSONResponse.
     """
 
     content: Optional[Dict[str, Any]] = None
     status_code: Optional[int] = None
+    media_type: str = "application/json"
 
     def __init__(
         self,
         content: Optional[Dict[str, Any]] = None,
         status_code: Optional[int] = None,
         **kwargs: Any,
     ):
         super().__init__(**kwargs)
         self.content = content
         self.status_code = status_code
+        self._media_type = self.media_type
 
     def to_response(
         self,
         headers: Dict[str, Any],
         media_type: Union["MediaType", str],
         status_code: int,
         app: Type["Esmerald"],
```

### Comparing `esmerald-1.3.0/esmerald/datastructures/redirect.py` & `esmerald-2.0.0/esmerald/datastructures/redirect.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/datastructures/stream.py` & `esmerald-2.0.0/esmerald/datastructures/stream.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,19 +21,16 @@
     from esmerald.applications import Esmerald
     from esmerald.enums import MediaType
 
 
 class Stream(ResponseContainer[StreamingResponse]):
     iterator: Union[
         Iterator[Union[str, bytes]],
-        Generator[Union[str, bytes], Any, Any],
         AsyncIterator[Union[str, bytes]],
         AsyncGenerator[Union[str, bytes], Any],
-        Type[Iterator[Union[str, bytes]]],
-        Type[AsyncIterator[Union[str, bytes]]],
         Callable[[], AsyncGenerator[Union[str, bytes], Any]],
         Callable[[], Generator[Union[str, bytes], Any, Any]],
     ]
 
     def to_response(
         self,
         headers: Dict[str, Any],
```

### Comparing `esmerald-1.3.0/esmerald/datastructures/template.py` & `esmerald-2.0.0/esmerald/datastructures/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/interceptors/interceptor.py` & `esmerald-2.0.0/esmerald/interceptors/interceptor.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/middleware/__init__.py` & `esmerald-2.0.0/esmerald/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/middleware/_exception_handlers.py` & `esmerald-2.0.0/esmerald/middleware/_exception_handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/middleware/asyncexitstack.py` & `esmerald-2.0.0/esmerald/middleware/asyncexitstack.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/middleware/authentication.py` & `esmerald-2.0.0/esmerald/middleware/authentication.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, Any
 
-from pydantic import BaseConfig, BaseModel
 from starlette.requests import HTTPConnection
 
 from esmerald.enums import ScopeType
+from esmerald.parsers import ArbitraryBaseModel
 from esmerald.protocols.middleware import MiddlewareProtocol
 
 if TYPE_CHECKING:
     from starlette.types import ASGIApp, Receive, Scope, Send
 
 
-class AuthResult(BaseModel):
+class AuthResult(ArbitraryBaseModel):
     user: Any
 
-    class Config(BaseConfig):
-        arbitrary_types_allowed = True
-
 
 class BaseAuthMiddleware(ABC, MiddlewareProtocol):
     scopes = {ScopeType.HTTP, ScopeType.WEBSOCKET}
 
     def __init__(self, app: "ASGIApp"):
         super().__init__(app)
         self.app = app
```

### Comparing `esmerald-1.3.0/esmerald/middleware/basic.py` & `esmerald-2.0.0/esmerald/middleware/basic.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/middleware/csrf.py` & `esmerald-2.0.0/esmerald/middleware/csrf.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/middleware/errors.py` & `esmerald-2.0.0/esmerald/middleware/errors.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/middleware/exceptions.py` & `esmerald-2.0.0/esmerald/middleware/exceptions.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/middleware/settings_middleware.py` & `esmerald-2.0.0/esmerald/middleware/settings_middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/permissions/base.py` & `esmerald-2.0.0/esmerald/permissions/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/permissions/utils.py` & `esmerald-2.0.0/esmerald/permissions/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/pluggables/base.py` & `esmerald-2.0.0/esmerald/pluggables/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/protocols/asyncdao.py` & `esmerald-2.0.0/esmerald/protocols/asyncdao.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/protocols/dao.py` & `esmerald-2.0.0/esmerald/protocols/dao.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/protocols/interceptor.py` & `esmerald-2.0.0/esmerald/protocols/interceptor.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/protocols/template.py` & `esmerald-2.0.0/esmerald/protocols/template.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import Any, Dict, List, Optional, TypeVar, Union
 
-from pydantic import DirectoryPath, validate_arguments
+from pydantic import DirectoryPath, validate_call
 from typing_extensions import Protocol, runtime_checkable
 
 
 @runtime_checkable
 class TemplateProtocol(Protocol):  # pragma: no cover
     def render(self, **context: Optional[Dict[str, Any]]) -> str:
         ...
 
 
 TP = TypeVar("TP", bound=TemplateProtocol, covariant=True)
 
 
 @runtime_checkable
 class TemplateEngineProtocol(Protocol[TP]):  # pragma: no cover
-    @validate_arguments
+    @validate_call
     def __init__(self, directory: Union[DirectoryPath, List[DirectoryPath]]) -> None:
         ...
 
     def get_template(self, template_name: str) -> TP:
         ...
```

### Comparing `esmerald-1.3.0/esmerald/responses/base.py` & `esmerald-2.0.0/esmerald/responses/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             background=cast("BackgroundTask", background),
         )
         self.cookies = cookies or []
 
     @staticmethod
     def transform(value: Any) -> Dict[str, Any]:
         if isinstance(value, BaseModel):
-            return value.dict()
+            return value.model_dump()
         raise TypeError("unsupported type")  # pragma: no cover
 
     def render(self, content: Any) -> bytes:
         try:
             if (
                 content is None
                 or content is NoReturn
```

### Comparing `esmerald-1.3.0/esmerald/responses/encoders.py` & `esmerald-2.0.0/esmerald/responses/encoders.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/responses/json.py` & `esmerald-2.0.0/esmerald/responses/json.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,9 +13,9 @@
     @staticmethod
     def transform(value: Any) -> Dict[str, Any]:
         """
         Makes sure that every value is checked and if it's a pydantic model then parses into
         a dict().
         """
         if isinstance(value, BaseModel):
-            return value.dict()
+            return value.model_dump()
         raise TypeError("unsupported type")
```

### Comparing `esmerald-1.3.0/esmerald/responses/template.py` & `esmerald-2.0.0/esmerald/responses/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/routing/base.py` & `esmerald-2.0.0/esmerald/routing/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,30 +41,29 @@
 from esmerald.transformers.signature import SignatureFactory
 from esmerald.transformers.utils import get_signature
 from esmerald.typing import Void, VoidType
 from esmerald.utils.helpers import is_async_callable, is_class_and_subclass
 from esmerald.utils.sync import AsyncCallable
 
 if TYPE_CHECKING:
-    from pydantic.typing import AnyCallable
-
     from esmerald.applications import Esmerald
     from esmerald.interceptors.interceptor import EsmeraldInterceptor
     from esmerald.interceptors.types import Interceptor
     from esmerald.permissions import BasePermission
     from esmerald.permissions.types import Permission
     from esmerald.routing.router import HTTPHandler
     from esmerald.types import (
         APIGateHandler,
         AsyncAnyCallable,
         Dependencies,
         ExceptionHandlerMap,
         ResponseCookies,
         ResponseHeaders,
     )
+    from esmerald.typing import AnyCallable
 
 param_type_map = {
     "str": str,
     "int": int,
     "float": float,
     "uuid": UUID,
     "decimal": Decimal,
```

### Comparing `esmerald-1.3.0/esmerald/routing/events.py` & `esmerald-2.0.0/esmerald/routing/events.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/routing/gateways.py` & `esmerald-2.0.0/esmerald/routing/gateways.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             handler = handler(parent=self)  # type: ignore
 
         if not is_from_router:
             self.path = clean_path(path + handler.path)
         else:
             self.path = clean_path(path)
 
-        self.methods = getattr(handler, "methods", None)
+        self.methods = getattr(handler, "http_methods", None)
 
         if not name:
             if not isinstance(handler, APIView):
                 name = clean_string(handler.fn.__name__)
             else:
                 name = clean_string(handler.__class__.__name__)
 
@@ -78,15 +78,15 @@
         )
         """
         A "bridge" to a handler and router mapping functionality.
         Since the default Starlette Route endpoint does not understand the Esmerald handlers,
         the Gateway bridges both functionalities and adds an extra "flair" to be compliant with both class based views and decorated function views.
         """
         self._interceptors: Union[List["Interceptor"], "VoidType"] = Void
-
+        self.name = name
         self.handler = handler
         self.dependencies = dependencies or {}
         self.interceptors: Sequence["Interceptor"] = interceptors or []
         self.permissions: Sequence["Permission"] = permissions or []
         self.middleware = middleware or []
         self.exception_handlers = exception_handlers or {}
         self.response_class = None
@@ -99,14 +99,15 @@
             handler.path_format,
             handler.param_convertors,
         ) = compile_path(self.path)
 
         if not is_class_and_subclass(self.handler, APIView) and not isinstance(
             self.handler, APIView
         ):
+            self.handler.name = self.name
             self.handler.get_response_handler()
 
             if not handler.operation_id:
                 handler.operation_id = self.generate_operation_id()
 
     async def handle(self, scope: "Scope", receive: "Receive", send: "Send") -> None:
         """
@@ -120,14 +121,16 @@
     def generate_operation_id(self) -> str:
         """
         Generates an unique operation if for the handler
         """
         operation_id = self.name + self.handler.path_format
         operation_id = re.sub(r"\W", "_", operation_id)
         methods = list(self.handler.methods)
+
+        assert self.handler.methods
         operation_id = f"{operation_id}_{methods[0].lower()}"
         return operation_id
 
 
 class WebSocketGateway(StarletteWebSocketRoute, BaseInterceptorMixin):
     __slots__ = (
         "_interceptors",
```

### Comparing `esmerald-1.3.0/esmerald/routing/handlers.py` & `esmerald-2.0.0/esmerald/routing/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from typing import TYPE_CHECKING, Dict, List, Optional, Sequence, Type, Union
 
 from starlette import status
 
 from esmerald.enums import HttpMethod, MediaType
 from esmerald.exceptions import HTTPException, ImproperlyConfigured
-from esmerald.openapi.datastructures import ResponseSpecification
+from esmerald.openapi.datastructures import OpenAPIResponse
 from esmerald.permissions.types import Permission
 from esmerald.routing.router import HTTPHandler, WebSocketHandler
 from esmerald.types import (
     BackgroundTaskType,
     Dependencies,
     ExceptionHandlerMap,
     Middleware,
     ResponseCookies,
     ResponseHeaders,
     ResponseType,
 )
 from esmerald.utils.constants import AVAILABLE_METHODS
 
 if TYPE_CHECKING:
-    from openapi_schemas_pydantic.v3_1_0 import SecurityRequirement
+    from openapi_schemas_pydantic.v3_1_0 import SecurityScheme
 
 
 SUCCESSFUL_RESPONSE = "Successful response"
 
 
 class get(HTTPHandler):
     def __init__(
@@ -43,19 +43,19 @@
         middleware: Optional[List[Middleware]] = None,
         media_type: Union[MediaType, str] = MediaType.JSON,
         response_class: Optional[ResponseType] = None,
         response_cookies: Optional[ResponseCookies] = None,
         response_headers: Optional[ResponseHeaders] = None,
         tags: Optional[Sequence[str]] = None,
         deprecated: Optional[bool] = None,
-        security: Optional[List["SecurityRequirement"]] = None,
+        security: Optional[List["SecurityScheme"]] = None,
         operation_id: Optional[str] = None,
         raise_exceptions: Optional[List[Type["HTTPException"]]] = None,
         response_description: Optional[str] = SUCCESSFUL_RESPONSE,
-        responses: Optional[Dict[int, ResponseSpecification]] = None,
+        responses: Optional[Dict[int, OpenAPIResponse]] = None,
     ) -> None:
         super().__init__(
             path=path,
             methods=[HttpMethod.GET],
             summary=summary,
             description=description,
             status_code=status_code,
@@ -99,19 +99,19 @@
         middleware: Optional[List[Middleware]] = None,
         media_type: Union[MediaType, str] = MediaType.JSON,
         response_class: Optional[ResponseType] = None,
         response_cookies: Optional[ResponseCookies] = None,
         response_headers: Optional[ResponseHeaders] = None,
         tags: Optional[Sequence[str]] = None,
         deprecated: Optional[bool] = None,
-        security: Optional[List["SecurityRequirement"]] = None,
+        security: Optional[List["SecurityScheme"]] = None,
         operation_id: Optional[str] = None,
         raise_exceptions: Optional[List[Type["HTTPException"]]] = None,
         response_description: Optional[str] = SUCCESSFUL_RESPONSE,
-        responses: Optional[Dict[int, ResponseSpecification]] = None,
+        responses: Optional[Dict[int, OpenAPIResponse]] = None,
     ) -> None:
         super().__init__(
             path=path,
             methods=[HttpMethod.HEAD],
             summary=summary,
             description=description,
             status_code=status_code,
@@ -155,19 +155,19 @@
         middleware: Optional[List[Middleware]] = None,
         media_type: Union[MediaType, str] = MediaType.JSON,
         response_class: Optional[ResponseType] = None,
         response_cookies: Optional[ResponseCookies] = None,
         response_headers: Optional[ResponseHeaders] = None,
         tags: Optional[Sequence[str]] = None,
         deprecated: Optional[bool] = None,
-        security: Optional[List["SecurityRequirement"]] = None,
+        security: Optional[List["SecurityScheme"]] = None,
         operation_id: Optional[str] = None,
         raise_exceptions: Optional[List[Type["HTTPException"]]] = None,
         response_description: Optional[str] = SUCCESSFUL_RESPONSE,
-        responses: Optional[Dict[int, ResponseSpecification]] = None,
+        responses: Optional[Dict[int, OpenAPIResponse]] = None,
     ) -> None:
         super().__init__(
             path=path,
             methods=[HttpMethod.OPTIONS],
             summary=summary,
             description=description,
             status_code=status_code,
@@ -211,19 +211,19 @@
         middleware: Optional[List[Middleware]] = None,
         media_type: Union[MediaType, str] = MediaType.JSON,
         response_class: Optional[ResponseType] = None,
         response_cookies: Optional[ResponseCookies] = None,
         response_headers: Optional[ResponseHeaders] = None,
         tags: Optional[Sequence[str]] = None,
         deprecated: Optional[bool] = None,
-        security: Optional[List["SecurityRequirement"]] = None,
+        security: Optional[List["SecurityScheme"]] = None,
         operation_id: Optional[str] = None,
         raise_exceptions: Optional[List[Type["HTTPException"]]] = None,
         response_description: Optional[str] = SUCCESSFUL_RESPONSE,
-        responses: Optional[Dict[int, ResponseSpecification]] = None,
+        responses: Optional[Dict[int, OpenAPIResponse]] = None,
     ) -> None:
         super().__init__(
             path=path,
             methods=[HttpMethod.TRACE],
             summary=summary,
             description=description,
             status_code=status_code,
@@ -267,19 +267,19 @@
         middleware: Optional[List[Middleware]] = None,
         media_type: Union[MediaType, str] = MediaType.JSON,
         response_class: Optional[ResponseType] = None,
         response_cookies: Optional[ResponseCookies] = None,
         response_headers: Optional[ResponseHeaders] = None,
         tags: Optional[Sequence[str]] = None,
         deprecated: Optional[bool] = None,
-        security: Optional[List["SecurityRequirement"]] = None,
+        security: Optional[List["SecurityScheme"]] = None,
         operation_id: Optional[str] = None,
         raise_exceptions: Optional[List[Type["HTTPException"]]] = None,
         response_description: Optional[str] = SUCCESSFUL_RESPONSE,
-        responses: Optional[Dict[int, ResponseSpecification]] = None,
+        responses: Optional[Dict[int, OpenAPIResponse]] = None,
     ) -> None:
         super().__init__(
             path=path,
             status_code=status_code,
             content_encoding=content_encoding,
             content_media_type=content_media_type,
             summary=summary,
@@ -323,19 +323,19 @@
         middleware: Optional[List[Middleware]] = None,
         media_type: Union[MediaType, str] = MediaType.JSON,
         response_class: Optional[ResponseType] = None,
         response_cookies: Optional[ResponseCookies] = None,
         response_headers: Optional[ResponseHeaders] = None,
         tags: Optional[Sequence[str]] = None,
         deprecated: Optional[bool] = None,
-        security: Optional[List["SecurityRequirement"]] = None,
+        security: Optional[List["SecurityScheme"]] = None,
         operation_id: Optional[str] = None,
         raise_exceptions: Optional[List[Type["HTTPException"]]] = None,
         response_description: Optional[str] = SUCCESSFUL_RESPONSE,
-        responses: Optional[Dict[int, ResponseSpecification]] = None,
+        responses: Optional[Dict[int, OpenAPIResponse]] = None,
     ) -> None:
         super().__init__(
             path=path,
             methods=[HttpMethod.PUT],
             summary=summary,
             description=description,
             status_code=status_code,
@@ -379,19 +379,19 @@
         middleware: Optional[List[Middleware]] = None,
         media_type: Union[MediaType, str] = MediaType.JSON,
         response_class: Optional[ResponseType] = None,
         response_cookies: Optional[ResponseCookies] = None,
         response_headers: Optional[ResponseHeaders] = None,
         tags: Optional[Sequence[str]] = None,
         deprecated: Optional[bool] = None,
-        security: Optional[List["SecurityRequirement"]] = None,
+        security: Optional[List["SecurityScheme"]] = None,
         operation_id: Optional[str] = None,
         raise_exceptions: Optional[List[Type["HTTPException"]]] = None,
         response_description: Optional[str] = SUCCESSFUL_RESPONSE,
-        responses: Optional[Dict[int, ResponseSpecification]] = None,
+        responses: Optional[Dict[int, OpenAPIResponse]] = None,
     ) -> None:
         super().__init__(
             path=path,
             methods=[HttpMethod.PATCH],
             summary=summary,
             description=description,
             status_code=status_code,
@@ -435,19 +435,19 @@
         middleware: Optional[List[Middleware]] = None,
         media_type: Union[MediaType, str] = MediaType.JSON,
         response_class: Optional[ResponseType] = None,
         response_cookies: Optional[ResponseCookies] = None,
         response_headers: Optional[ResponseHeaders] = None,
         tags: Optional[Sequence[str]] = None,
         deprecated: Optional[bool] = None,
-        security: Optional[List["SecurityRequirement"]] = None,
+        security: Optional[List["SecurityScheme"]] = None,
         operation_id: Optional[str] = None,
         raise_exceptions: Optional[List[Type["HTTPException"]]] = None,
         response_description: Optional[str] = SUCCESSFUL_RESPONSE,
-        responses: Optional[Dict[int, ResponseSpecification]] = None,
+        responses: Optional[Dict[int, OpenAPIResponse]] = None,
     ) -> None:
         super().__init__(
             path=path,
             methods=[HttpMethod.DELETE],
             summary=summary,
             description=description,
             status_code=status_code,
@@ -492,19 +492,19 @@
         middleware: Optional[List[Middleware]] = None,
         media_type: Union[MediaType, str] = MediaType.JSON,
         response_class: Optional[ResponseType] = None,
         response_cookies: Optional[ResponseCookies] = None,
         response_headers: Optional[ResponseHeaders] = None,
         tags: Optional[Sequence[str]] = None,
         deprecated: Optional[bool] = None,
-        security: Optional[List["SecurityRequirement"]] = None,
+        security: Optional[List["SecurityScheme"]] = None,
         operation_id: Optional[str] = None,
         raise_exceptions: Optional[List[Type["HTTPException"]]] = None,
         response_description: Optional[str] = SUCCESSFUL_RESPONSE,
-        responses: Optional[Dict[int, ResponseSpecification]] = None,
+        responses: Optional[Dict[int, OpenAPIResponse]] = None,
     ) -> None:
         if not methods or not isinstance(methods, list):
             raise ImproperlyConfigured(
                 "http handler demands `methods` to be declared. "
                 "An example would be: @route(methods=['GET', 'PUT'])."
             )
```

### Comparing `esmerald-1.3.0/esmerald/routing/router.py` & `esmerald-2.0.0/esmerald/routing/router.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,36 +39,38 @@
 from esmerald.core.urls import include
 from esmerald.datastructures import File, Redirect
 from esmerald.enums import HttpMethod, MediaType
 from esmerald.exceptions import (
     ImproperlyConfigured,
     MethodNotAllowed,
     NotFound,
+    OpenAPIException,
     ValidationErrorException,
 )
 from esmerald.interceptors.types import Interceptor
-from esmerald.openapi.datastructures import ResponseSpecification
+from esmerald.openapi.datastructures import OpenAPIResponse
+from esmerald.openapi.utils import is_status_code_allowed
 from esmerald.requests import Request
 from esmerald.responses import Response
+from esmerald.routing._internal import FieldInfoMixin
 from esmerald.routing.base import BaseHandlerMixin
 from esmerald.routing.events import handle_lifespan_events
 from esmerald.routing.gateways import Gateway, WebSocketGateway
 from esmerald.routing.views import APIView
 from esmerald.transformers.datastructures import EsmeraldSignature as SignatureModel
 from esmerald.transformers.model import TransformerModel
 from esmerald.transformers.utils import get_signature
 from esmerald.typing import Void, VoidType
 from esmerald.utils.constants import DATA, REDIRECT_STATUS_CODES, REQUEST, SOCKET
 from esmerald.utils.helpers import is_async_callable, is_class_and_subclass
 from esmerald.utils.url import clean_path
 from esmerald.websockets import WebSocket, WebSocketClose
 
 if TYPE_CHECKING:
-    from openapi_schemas_pydantic.v3_1_0 import SecurityRequirement
-    from pydantic.typing import AnyCallable
+    from openapi_schemas_pydantic.v3_1_0.security_scheme import SecurityScheme
 
     from esmerald.applications import Esmerald
     from esmerald.exceptions import HTTPException
     from esmerald.permissions.types import Permission
     from esmerald.types import (
         APIGateHandler,
         AsyncAnyCallable,
@@ -79,14 +81,15 @@
         Middleware,
         ParentType,
         ResponseCookies,
         ResponseHeaders,
         ResponseType,
         RouteParent,
     )
+    from esmerald.typing import AnyCallable
 
 
 class Parent:
     def create_signature_models(self, route: "RouteParent") -> None:
         """
         Creates the signature models for the given routes.
 
@@ -202,15 +205,15 @@
         middleware: Optional[Sequence["Middleware"]] = None,
         response_class: Optional["ResponseType"] = None,
         response_cookies: Optional["ResponseCookies"] = None,
         response_headers: Optional["ResponseHeaders"] = None,
         lifespan: Optional[Lifespan[Any]] = None,
         tags: Optional[Sequence[str]] = None,
         deprecated: Optional[bool] = None,
-        security: Optional[Sequence["SecurityRequirement"]] = None,
+        security: Optional[Sequence["SecurityScheme"]] = None,
     ):
         self.app = app
         if not path:
             path = "/"
         else:
             assert path.startswith("/"), "A path prefix must start with '/'"
             assert not path.endswith(
@@ -429,15 +432,15 @@
         def decorator(func: Callable) -> Callable:
             self.add_event_handler(event_type, func)
             return func
 
         return decorator
 
 
-class HTTPHandler(BaseHandlerMixin, StarletteRoute):
+class HTTPHandler(BaseHandlerMixin, FieldInfoMixin, StarletteRoute):
     __slots__ = (
         "path",
         "_permissions",
         "_dependencies",
         "_response_handler",
         "methods",
         "status_code",
@@ -482,16 +485,16 @@
         media_type: Union[MediaType, str] = MediaType.JSON,
         response_class: Optional["ResponseType"] = None,
         response_cookies: Optional["ResponseCookies"] = None,
         response_headers: Optional["ResponseHeaders"] = None,
         tags: Optional[Sequence[str]] = None,
         deprecated: Optional[bool] = None,
         response_description: Optional[str] = "Successful Response",
-        responses: Optional[Dict[int, ResponseSpecification]] = None,
-        security: Optional[List["SecurityRequirement"]] = None,
+        responses: Optional[Dict[int, OpenAPIResponse]] = None,
+        security: Optional[List["SecurityScheme"]] = None,
         operation_id: Optional[str] = None,
         raise_exceptions: Optional[List[Type["HTTPException"]]] = None,
     ) -> None:
         if not path:
             path = "/"
         super().__init__(path=path, endpoint=endpoint, include_in_schema=include_in_schema)
         """
@@ -551,14 +554,30 @@
         self.raise_exceptions = raise_exceptions
 
         self.fn: Optional["AnyCallable"] = None
         self.app: Optional["ASGIApp"] = None
         self.route_map: Dict[str, Tuple["HTTPHandler", "TransformerModel"]] = {}
         self.path_regex, self.path_format, self.param_convertors = compile_path(path)
 
+        if self.responses:
+            self.validate_responses(responses=self.responses)
+
+    def validate_responses(self, responses: Dict[int, OpenAPIResponse]) -> None:
+        """
+        Checks if the responses are valid or raises an exception otherwise.
+        """
+        for status_code, response in responses.items():
+            if not isinstance(response, OpenAPIResponse):
+                raise OpenAPIException(
+                    detail="An additional response must be an instance of OpenAPIResponse."
+                )
+
+            if not is_status_code_allowed(status_code):
+                raise OpenAPIException(detail="The status is not a valid OpenAPI status response.")
+
     @property
     def http_methods(self) -> List[str]:
         """
         Converts the methods set into a list of methods.
         """
         return list(self.methods)
 
@@ -832,15 +851,15 @@
 
         fn = cast("AsyncAnyCallable", self.fn)
         if isinstance(self.parent, APIView):
             await fn(self.parent, **kwargs)
         else:
             await fn(**kwargs)
 
-    async def get_kwargs(self, websocket: WebSocket[Any, Any]) -> Dict[str, Any]:
+    async def get_kwargs(self, websocket: WebSocket[Any, Any]) -> Any:
         """Resolves the required kwargs from the request data.
 
         Args:
             websocket: WebSocket instance
 
         Returns:
             Dictionary of parsed kwargs
@@ -897,15 +916,15 @@
         dependencies: Optional["Dependencies"] = None,
         exception_handlers: Optional["ExceptionHandlerMap"] = None,
         interceptors: Optional[Sequence["Interceptor"]] = None,
         permissions: Optional[Sequence["Permission"]] = None,
         middleware: Optional[List["Middleware"]] = None,
         include_in_schema: Optional[bool] = True,
         deprecated: Optional[bool] = None,
-        security: Optional[Sequence["SecurityRequirement"]] = None,
+        security: Optional[Sequence["SecurityScheme"]] = None,
     ) -> None:
         self.path = path
         if not path:
             self.path = "/"
 
         if namespace and routes:
             raise ImproperlyConfigured("It can only be namespace or routes, not both.")
```

### Comparing `esmerald-1.3.0/esmerald/routing/views.py` & `esmerald-2.0.0/esmerald/routing/views.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/security/jwt/token.py` & `esmerald-2.0.0/esmerald/security/jwt/token.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,55 @@
 from datetime import datetime, timezone
 from typing import Any, Dict, List, Optional, Union
 
 from jose import JWSError, JWTError, jwt
 from jose.exceptions import JWSAlgorithmError, JWSSignatureError
-from pydantic import BaseModel, Field, constr, validator
+from pydantic import BaseModel, Field, conint, constr, field_validator
 
 from esmerald.exceptions import ImproperlyConfigured
 from esmerald.security.utils import convert_time
 
 
 class Token(BaseModel):
     """
     Classic representation of a token via pydantic model.
     """
 
     exp: datetime
     iat: datetime = Field(default_factory=lambda: convert_time(datetime.now(timezone.utc)))
-    sub: constr(min_length=1)  # type: ignore
+    sub: Optional[Union[constr(min_length=1), conint(ge=1)]] = None  # type: ignore
     iss: Optional[str] = None
     aud: Optional[str] = None
     jti: Optional[str] = None
 
-    @validator("exp", always=True)
+    @field_validator("exp")
     def validate_expiration(cls, date: datetime) -> datetime:
         """
         When a token is issued, needs to be date in the future.
         """
         date = convert_time(date)
         if date.timestamp() >= convert_time(datetime.now(timezone.utc)).timestamp():
             return date
         raise ValueError("The exp must be a date in the future.")
 
-    @validator("iat", always=True)
-    def validate_iat(cls, date: datetime) -> datetime:  # pylint: disable=no-self-argument
+    @field_validator("iat")
+    def validate_iat(cls, date: datetime) -> datetime:
         """Ensures that the `Issued At` it's nt bigger than the current time."""
         date = convert_time(date)
         if date.timestamp() <= convert_time(datetime.now(timezone.utc)).timestamp():
             return date
         raise ValueError("iat must be a current or past time")
 
+    @field_validator("sub")
+    def validate_sub(cls, subject: Union[str, int]) -> str:
+        try:
+            return str(subject)
+        except (TypeError, ValueError) as e:
+            raise ValueError(f"{subject} is not a valid string.") from e
+
     def encode(self, key: str, algorithm: str) -> Union[str, Any]:
         """
         Encodes the token into a proper str formatted and allows passing kwargs.
         """
         try:
             return jwt.encode(
                 claims=self.dict(exclude_none=True),
```

### Comparing `esmerald-1.3.0/esmerald/template/jinja.py` & `esmerald-2.0.0/esmerald/template/jinja.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/template/mako.py` & `esmerald-2.0.0/esmerald/template/mako.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/transformers/datastructures.py` & `esmerald-2.0.0/esmerald/transformers/datastructures.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,34 @@
-"""
-Signature is widely used by Pydantic and comes from the inpect library.
-A lot of great work was done using the Signature and Esmerald is no exception.
-"""
-
 from inspect import Parameter as InspectParameter
 from inspect import Signature
-from typing import TYPE_CHECKING, Any, ClassVar, Optional, Set, Union
+from typing import Any, ClassVar, Optional, Set, Union
 
-from pydantic import BaseModel, ValidationError
+from pydantic import ValidationError
 
 from esmerald.exceptions import ImproperlyConfigured, InternalServerError, ValidationErrorException
+from esmerald.parsers import ArbitraryBaseModel
 from esmerald.requests import Request
 from esmerald.transformers.constants import UNDEFINED
 from esmerald.transformers.utils import get_connection_info
 from esmerald.utils.helpers import is_optional_union
 from esmerald.websockets import WebSocket
 
-if TYPE_CHECKING:
-    from pydantic.error_wrappers import ErrorDict
-    from pydantic.typing import DictAny
-
 
-class EsmeraldSignature(BaseModel):
+class EsmeraldSignature(ArbitraryBaseModel):
     dependency_names: ClassVar[Set[str]]
     return_annotation: ClassVar[Any]
 
-    class Config:
-        arbitrary_types_allowed = True
-
     @classmethod
     def parse_values_for_connection(
-        cls, connection: Union[Request, WebSocket], **kwargs: "DictAny"
-    ) -> "DictAny":
+        cls, connection: Union[Request, WebSocket], **kwargs: Any
+    ) -> Any:
         try:
             signature = cls(**kwargs)
             values = {}
-            for key in cls.__fields__:
+            for key in cls.model_fields:
                 values[key] = signature.field_value(key)
             return values
         except ValidationError as e:
             raise cls.build_exception(connection, e) from e
 
     @classmethod
     def build_exception(
@@ -58,38 +47,35 @@
         error_message = f"Validation failed for {url} with method {method}."
 
         if client_errors:
             return ValidationErrorException(detail=error_message, extra=client_errors)
         return InternalServerError(detail=error_message, extra=server_errors)
 
     @classmethod
-    def is_server_error(cls, error: "ErrorDict") -> bool:
+    def is_server_error(cls, error: Any) -> bool:
         """
         Classic approach functionality used widely to check if is a server error or not.
         """
         return error["loc"][-1] in cls.dependency_names
 
     def field_value(self, key: str) -> Any:
         return self.__getattribute__(key)
 
 
-class Parameter(BaseModel):
-    annotation: Optional[Any]
-    default: Optional[Any]
-    name: Optional[str]
-    optional: Optional[bool]
-    fn_name: Optional[str]
-    param_name: Optional[str]
-    parameter: Optional[InspectParameter]
-
-    class Config:
-        arbitrary_types_allowed = True
+class Parameter(ArbitraryBaseModel):
+    annotation: Optional[Any] = None
+    default: Optional[Any] = None
+    name: Optional[str] = None
+    optional: Optional[bool] = None
+    fn_name: Optional[str] = None
+    param_name: Optional[str] = None
+    parameter: Optional[InspectParameter] = None
 
     def __init__(
-        self, fn_name: str, param_name: str, parameter: InspectParameter, **kwargs: "DictAny"
+        self, fn_name: str, param_name: str, parameter: InspectParameter, **kwargs: Any
     ) -> None:
         super().__init__(**kwargs)
         if parameter.annotation is Signature.empty:
             raise ImproperlyConfigured(
                 f"The parameter name {param_name} from {fn_name} does not have a type annotation. "
                 "If it should receive any value, use 'Any' as type."
             )
```

### Comparing `esmerald-1.3.0/esmerald/transformers/helpers.py` & `esmerald-2.0.0/esmerald/transformers/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import inspect
 from typing import Any
 
-from pydantic import (
+from pydantic.v1 import (
     ConstrainedBytes,
     ConstrainedDate,
     ConstrainedDecimal,
     ConstrainedFloat,
     ConstrainedFrozenSet,
     ConstrainedInt,
     ConstrainedList,
```

### Comparing `esmerald-1.3.0/esmerald/transformers/model.py` & `esmerald-2.0.0/esmerald/transformers/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,54 +1,42 @@
 from typing import TYPE_CHECKING, Any, Dict, Mapping, Optional, Set, Tuple, Type, Union, cast
 
-from pydantic.fields import (
-    SHAPE_DEQUE,
-    SHAPE_FROZENSET,
-    SHAPE_LIST,
-    SHAPE_SEQUENCE,
-    SHAPE_SET,
-    SHAPE_TUPLE,
-    SHAPE_TUPLE_ELLIPSIS,
-    ModelField,
-)
+from pydantic.fields import FieldInfo
 
 from esmerald.enums import EncodingType, ParamType
 from esmerald.exceptions import ImproperlyConfigured
-from esmerald.parsers import BaseModelExtra, parse_form_data
+from esmerald.parsers import ArbitraryExtraBaseModel, parse_form_data
 from esmerald.requests import Request
 from esmerald.transformers.datastructures import EsmeraldSignature as SignatureModel
 from esmerald.transformers.utils import (
     Dependency,
     ParamSetting,
     create_parameter_setting,
     get_request_params,
     get_signature,
     merge_sets,
 )
-from esmerald.utils.constants import RESERVED_KWARGS
+from esmerald.utils.constants import DATA, RESERVED_KWARGS
 from esmerald.utils.pydantic.schema import is_field_optional
 
 if TYPE_CHECKING:
     from esmerald.types import Dependencies
     from esmerald.websockets import WebSocket
 
 
 MEDIA_TYPES = [EncodingType.MULTI_PART, EncodingType.URL_ENCODED]
 MappingUnion = Mapping[Union[int, str], Any]
 
 
-class TransformerModel(BaseModelExtra):
-    class Config(BaseModelExtra.Config):
-        arbitrary_types_allowed = True
-
+class TransformerModel(ArbitraryExtraBaseModel):
     def __init__(
         self,
         cookies: Set[ParamSetting],
         dependencies: Set[Dependency],
-        form_data: Optional[Tuple[EncodingType, ModelField]],
+        form_data: Optional[Tuple[EncodingType, FieldInfo]],
         headers: Set[ParamSetting],
         path_params: Set[ParamSetting],
         query_params: Set[ParamSetting],
         reserved_kwargs: Set[str],
         query_param_names: Set[ParamSetting],
         is_optional: bool,
         **kwargs: Any,
@@ -69,74 +57,83 @@
             or headers
             or path_params
             or query_params
             or reserved_kwargs
         )
         self.is_optional = is_optional
 
+    def get_cookie_params(self) -> Set[ParamSetting]:
+        return self.cookies
+
+    def get_path_params(self) -> Set[ParamSetting]:
+        return self.path_params
+
+    def get_query_params(self) -> Set[ParamSetting]:
+        return self.query_params
+
+    def get_header_params(self) -> Set[ParamSetting]:
+        return self.headers
+
+    def is_kwargs(
+        self,
+    ) -> Union[Set[ParamSetting], Set[str], Tuple[EncodingType, FieldInfo], Set[Dependency]]:
+        return self.has_kwargs
+
     @classmethod
     def dependency_tree(cls, key: str, dependencies: "Dependencies") -> Dependency:
         inject = dependencies[key]
-        dependency_keys = [key for key in get_signature(inject).__fields__ if key in dependencies]
+        dependency_keys = [
+            key for key in get_signature(inject).model_fields if key in dependencies
+        ]
         return Dependency(
             key=key,
             inject=inject,
             dependencies=[
                 cls.dependency_tree(key=key, dependencies=dependencies) for key in dependency_keys
             ],
         )
 
     @classmethod
     def get_parameter_settings(
         cls,
         path_parameters: Set[str],
         dependencies: "Dependencies",
-        signature_fields: Dict[str, ModelField],
+        signature_fields: Dict[str, FieldInfo],
     ) -> Tuple[Set[ParamSetting], set]:
-        shapes = {
-            SHAPE_LIST,
-            SHAPE_SET,
-            SHAPE_SEQUENCE,
-            SHAPE_TUPLE,
-            SHAPE_TUPLE_ELLIPSIS,
-            SHAPE_DEQUE,
-            SHAPE_FROZENSET,
-        }
-
         _dependencies = set()
 
         for key in dependencies:
             if key in signature_fields:
                 _dependencies.add(cls.dependency_tree(key=key, dependencies=dependencies))
 
         ignored_keys = {*RESERVED_KWARGS, *(dependency.key for dependency in _dependencies)}
 
         parameter_definitions = set()
         for field_name, model_field in signature_fields.items():
             if field_name not in ignored_keys:
+                allow_none = getattr(model_field, "allow_none", True)
                 parameter_definitions.add(
                     create_parameter_setting(
-                        allow_none=model_field.allow_none,
+                        allow_none=allow_none,
                         field_name=field_name,
-                        field_info=model_field.field_info,
+                        field_info=model_field,
                         path_parameters=path_parameters,
-                        is_sequence=model_field.shape in shapes,
                     )
                 )
 
         filtered = [item for item in signature_fields.items() if item[0] not in ignored_keys]
         for field_name, model_field in filtered:
-            signature_field = model_field.field_info
+            signature_field = model_field
+            allow_none = getattr(signature_field, "allow_none", True)
             parameter_definitions.add(
                 create_parameter_setting(
-                    allow_none=model_field.allow_none,
+                    allow_none=allow_none,
                     field_name=field_name,
                     field_info=signature_field,
                     path_parameters=path_parameters,
-                    is_sequence=model_field.shape in shapes,
                 )
             )
 
         return parameter_definitions, _dependencies
 
     @classmethod
     def create_signature(
@@ -144,27 +141,27 @@
         signature_model: Type[SignatureModel],
         dependencies: "Dependencies",
         path_parameters: Set[str],
     ) -> "TransformerModel":
         cls.validate_kwargs(
             path_parameters=path_parameters,
             dependencies=dependencies,
-            model_fields=signature_model.__fields__,
+            model_fields=signature_model.model_fields,
         )
 
         reserved_kwargs = set()
 
-        for field_name in signature_model.__fields__:
+        for field_name in signature_model.model_fields:
             if field_name in RESERVED_KWARGS:
                 reserved_kwargs.add(field_name)
 
         param_settings, _dependencies = cls.get_parameter_settings(
             path_parameters=path_parameters,
             dependencies=dependencies,
-            signature_fields=signature_model.__fields__,
+            signature_fields=signature_model.model_fields,
         )
 
         path_params = set()
         for param in param_settings:
             if param.param_type == ParamType.PATH:
                 path_params.add(param)
 
@@ -179,25 +176,23 @@
                 cookies.add(param)
 
         query_params = set()
         for param in param_settings:
             if param.param_type == ParamType.QUERY:
                 query_params.add(param)
 
-        query_params_names = set()
-        for param in param_settings:
-            if param.param_type == ParamType.QUERY and param.is_sequence:
-                query_params_names.add(param)
+        query_params_names: Set[ParamSetting] = set()
 
         form_data = None
 
         # For the reserved keyword data
-        data_field = signature_model.__fields__.get("data")
+        data_field = signature_model.model_fields.get("data")
         if data_field:
-            media_type = data_field.field_info.extra.get("media_type")
+            extra = getattr(data_field, "json_schema_extra", None) or {}
+            media_type = extra.get("media_type")
             if media_type in MEDIA_TYPES:
                 form_data = (media_type, data_field)
 
         path_params, query_params, cookies, headers, reserved_kwargs = cls.update_parameters(
             global_dependencies=dependencies,
             local_dependencies=_dependencies,
             path_params=path_params,
@@ -206,16 +201,16 @@
             headers=headers,
             reserved_kwargs=reserved_kwargs,
             path_parameters=path_parameters,
             form_data=form_data,
         )
 
         is_optional = False
-        if "data" in reserved_kwargs:
-            is_optional = is_field_optional(signature_model.__fields__["data"])
+        if DATA in reserved_kwargs:
+            is_optional = is_field_optional(signature_model.model_fields["data"])
 
         return TransformerModel(
             form_data=form_data,
             dependencies=_dependencies,
             path_params=path_params,
             query_params=query_params,
             cookies=cookies,
@@ -321,15 +316,15 @@
             reserved_kwargs["state"] = connection.app.state.copy()
 
         return {**reserved_kwargs, **path_params, **query_params, **headers, **cookies}
 
     @classmethod
     def validate_data(
         cls,
-        form_data: Optional[Tuple[EncodingType, ModelField]],
+        form_data: Optional[Tuple[EncodingType, FieldInfo]],
         dependency_model: "TransformerModel",
     ) -> None:
         if form_data and dependency_model.form_data:
             media_type, _ = form_data
             dependency_media_type, _ = dependency_model.form_data
             if media_type != dependency_media_type:
                 raise ImproperlyConfigured(
@@ -347,26 +342,27 @@
             )
 
     @classmethod
     def validate_kwargs(
         cls,
         path_parameters: Set[str],
         dependencies: "Dependencies",
-        model_fields: Dict[str, ModelField],
+        model_fields: Dict[str, FieldInfo],
     ) -> None:
         keys = set(dependencies.keys())
         names = set()
 
         for key, value in model_fields.items():
-            if (
-                value.field_info.extra.get(ParamType.QUERY)
-                or value.field_info.extra.get(ParamType.HEADER)
-                or value.field_info.extra.get(ParamType.COOKIE)
-            ):
-                names.add(key)
+            if value.json_schema_extra is not None:
+                if (
+                    value.json_schema_extra.get(ParamType.QUERY)
+                    or value.json_schema_extra.get(ParamType.HEADER)
+                    or value.json_schema_extra.get(ParamType.COOKIE)
+                ):
+                    names.add(key)
 
         for intersect in [
             path_parameters.intersection(keys)
             or path_parameters.intersection(names)
             or keys.intersection(names)
         ]:
             if intersect:
```

### Comparing `esmerald-1.3.0/esmerald/transformers/signature.py` & `esmerald-2.0.0/esmerald/transformers/signature.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from inspect import Signature as InspectSignature
 from typing import TYPE_CHECKING, Any, Dict, Generator, Optional, Set, Type
 
 from pydantic import create_model
-from pydantic.fields import Undefined
 
 from esmerald.exceptions import ImproperlyConfigured
-from esmerald.parsers import BaseModelExtra
+from esmerald.parsers import ArbitraryExtraBaseModel
 from esmerald.transformers.constants import CLASS_SPECIAL_WORDS, VALIDATION_NAMES
 from esmerald.transformers.datastructures import EsmeraldSignature, Parameter
 from esmerald.transformers.helpers import is_pydantic_constrained_field
 from esmerald.transformers.utils import get_field_definition_from_param
+from esmerald.typing import Undefined
 from esmerald.utils.dependency import is_dependency_field, should_skip_dependency_validation
 
 if TYPE_CHECKING:
-    from pydantic.typing import AnyCallable
+    from esmerald.typing import AnyCallable
 
 
-class SignatureFactory(BaseModelExtra):
-    class Config(BaseModelExtra.Config):
-        arbitrary_types_allowed = True
+object_setattr = object.__setattr__
 
+
+class SignatureFactory(ArbitraryExtraBaseModel):
     def __init__(
         self, fn: Optional["AnyCallable"], dependency_names: Set[str], **kwargs: Any
     ) -> None:
         super().__init__(**kwargs)
         if not fn:
             raise ImproperlyConfigured("Parameter 'fn' to SignatureFactory cannot be `None`.")
         self.fn = fn
```

### Comparing `esmerald-1.3.0/esmerald/transformers/types.py` & `esmerald-2.0.0/esmerald/transformers/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Type, Union
 
-from pydantic import (
+from pydantic.v1 import (
     ConstrainedBytes,
     ConstrainedDate,
     ConstrainedDecimal,
     ConstrainedFloat,
     ConstrainedFrozenSet,
     ConstrainedInt,
     ConstrainedList,
```

### Comparing `esmerald-1.3.0/esmerald/transformers/utils.py` & `esmerald-2.0.0/esmerald/transformers/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,44 @@
-from typing import TYPE_CHECKING, Any, List, NamedTuple, Set, Tuple, Type, cast
+from typing import TYPE_CHECKING, Any, List, NamedTuple, Set, Tuple, Type, Union, cast
 
-from pydantic.fields import FieldInfo, Undefined
+from pydantic.fields import FieldInfo
 from starlette.datastructures import URL
 
 from esmerald.enums import ParamType, ScopeType
 from esmerald.exceptions import ImproperlyConfigured, ValidationErrorException
-from esmerald.parsers import BaseModelExtra, HashableBaseModel
+from esmerald.params import Cookie, Header, Path, Query
+from esmerald.parsers import ArbitraryExtraBaseModel, HashableBaseModel
 from esmerald.requests import Request
+from esmerald.typing import Undefined
 from esmerald.utils.constants import REQUIRED
 
 if TYPE_CHECKING:
-    from pydantic.typing import MappingIntStrAny
-
     from esmerald.injector import Inject
     from esmerald.transformers.datastructures import EsmeraldSignature, Parameter
     from esmerald.types import ConnectionType
 
 
 class ParamSetting(NamedTuple):
     default_value: Any
     field_alias: str
     field_name: str
     is_required: bool
-    is_sequence: bool
     param_type: ParamType
     field_info: FieldInfo
 
 
-class Dependency(HashableBaseModel, BaseModelExtra):
+class Dependency(HashableBaseModel, ArbitraryExtraBaseModel):
     def __init__(
         self, key: str, inject: "Inject", dependencies: List["Dependency"], **kwargs: Any
     ) -> None:
         super().__init__(**kwargs)
         self.key = key
         self.inject = inject
         self.dependencies = dependencies
 
-    class Config(BaseModelExtra.Config):
-        arbitrary_types_allowed = True
-
 
 def merge_sets(first_set: Set[ParamSetting], second_set: Set[ParamSetting]) -> Set[ParamSetting]:
     merged_result = first_set.intersection(second_set)
     difference = first_set.symmetric_difference(second_set)
     for parameter in difference:
         if parameter.is_required or not any(
             param.field_alias == parameter.field_alias and param.is_required
@@ -53,49 +49,60 @@
 
 
 def create_parameter_setting(
     allow_none: bool,
     field_info: FieldInfo,
     field_name: str,
     path_parameters: Set[str],
-    is_sequence: bool,
 ) -> ParamSetting:
     """
     Creates a setting definition for a parameter.
     """
-    extra = field_info.extra
+    extra = field_info.json_schema_extra or {}
     is_required = extra.get(REQUIRED, True)
     default_value = field_info.default if field_info.default is not Undefined else None
 
     field_alias = extra.get(ParamType.QUERY) or field_name
     param_type = getattr(field_info, "in_", ParamType.QUERY)
+    param: Union[Path, Header, Cookie, Query]
 
     if field_name in path_parameters:
         field_alias = field_name
         param_type = param_type.PATH
+        param = Path()
     elif extra.get(ParamType.HEADER):
         field_alias = extra[ParamType.HEADER]
         param_type = ParamType.HEADER
+        param = Header()
+
     elif extra.get(ParamType.COOKIE):
         field_alias = extra[ParamType.COOKIE]
         param_type = ParamType.COOKIE
+        param = Cookie()
+    else:
+        param = Query()
+
+    if not field_info.alias:
+        field_info.alias = field_name
+
+    for key, _ in param._attributes_set.items():
+        setattr(param, key, getattr(field_info, key, None))
 
     param_settings = ParamSetting(
         param_type=param_type,
         field_alias=field_alias,
         default_value=default_value,
         field_name=field_name,
-        field_info=field_info,
-        is_sequence=is_sequence,
+        field_info=param,
         is_required=is_required and (default_value is None and not allow_none),
     )
     return param_settings
 
 
-def get_request_params(params: "MappingIntStrAny", expected: Set[ParamSetting], url: URL) -> Any:
+def get_request_params(params: Any, expected: Set[ParamSetting], url: URL) -> Any:
     """
     Gather the parameters from the request.
     """
     _params = []
     for param in expected:
         if param.is_required and param.field_alias not in params:
             _params.append(param.field_alias)
```

### Comparing `esmerald-1.3.0/esmerald/utils/constants.py` & `esmerald-2.0.0/esmerald/utils/constants.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/utils/crypto.py` & `esmerald-2.0.0/esmerald/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/utils/functional.py` & `esmerald-2.0.0/esmerald/utils/functional.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/utils/helpers.py` & `esmerald-2.0.0/esmerald/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/utils/model.py` & `esmerald-2.0.0/esmerald/utils/model.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,42 @@
+from dataclasses import Field as DataclassField
+from dataclasses import fields as get_dataclass_fields
 from inspect import isclass
-from typing import TYPE_CHECKING, Any, Dict, Type, cast
+from typing import TYPE_CHECKING, Any, Dict, Tuple, Type, cast
 
-from pydantic import BaseConfig, BaseModel, create_model
-from pyfactories.utils import create_model_from_dataclass
+from pydantic import BaseModel, ConfigDict, create_model
 
 if TYPE_CHECKING:
-    from pydantic.fields import ModelField
+    from pydantic.fields import FieldInfo
 
 
-class Config(BaseConfig):
-    arbitrary_types_allowed = True
+config = ConfigDict(arbitrary_types_allowed=True)
 
 
-def create_parsed_model_field(value: Type[Any]) -> "ModelField":
+def create_model_from_dataclass(dataclass: Any) -> Type[BaseModel]:
+    """Creates a subclass of BaseModel from a given dataclass.
+
+    We are limited here because Pydantic does not perform proper field
+    parsing when going this route - which requires we set the fields as
+    required and not required independently. We currently do not handle
+    deeply nested Any and Optional.
+    """
+    dataclass_fields: Tuple[DataclassField, ...] = get_dataclass_fields(dataclass)
+    model = create_model(dataclass.__name__, **{field.name: (field.type, ...) for field in dataclass_fields})  # type: ignore
+    for field_name, model_field in model.model_fields.items():
+        [field for field in dataclass_fields if field.name == field_name][0]
+        setattr(model, field_name, model_field)
+    return cast("Type[BaseModel]", model)
+
+
+def create_parsed_model_field(value: Type[Any]) -> "FieldInfo":
     """Create a pydantic model with the passed in value as its sole field, and
     return the parsed field."""
-    model = create_model("temp", __config__=Config, **{"value": (value, ... if not repr(value).startswith("typing.Optional") else None)})  # type: ignore
-    return cast("BaseModel", model).__fields__["value"]
+    model = create_model("temp", __config__=config, **{"value": (value, ... if not repr(value).startswith("typing.Optional") else None)})  # type: ignore
+    return cast("BaseModel", model).model_fields["value"]
 
 
 _dataclass_model_map: Dict[Any, Type[BaseModel]] = {}
 
 
 def convert_dataclass_to_model(dataclass: Any) -> Type[BaseModel]:
     """Converts a dataclass to a pydantic model and memoizes the result."""
```

### Comparing `esmerald-1.3.0/esmerald/utils/module_loading.py` & `esmerald-2.0.0/esmerald/utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/utils/sync.py` & `esmerald-2.0.0/esmerald/utils/sync.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/esmerald/utils/pydantic/schema.py` & `esmerald-2.0.0/esmerald/utils/pydantic/schema.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from decimal import Decimal
 from typing import TYPE_CHECKING, Any, TypeVar, cast
 
 T = TypeVar("T", int, float, Decimal)
 
 if TYPE_CHECKING:
-    from pydantic.fields import ModelField
+    from pydantic.fields import FieldInfo
 
 
-def is_field_optional(field: "ModelField") -> bool:
+def is_field_optional(field: "FieldInfo") -> bool:
     """
     Returns bool True or False for the optional model field.
     """
-    return not field.required and not is_any_type(field=field) and field.allow_none
+    allow_none = getattr(field, "allow_none", True)
+    return not field.is_required() and not is_any_type(field=field) and allow_none
 
 
-def is_any_type(field: "ModelField") -> bool:
+def is_any_type(field: "FieldInfo") -> bool:
     """
     Checks if the field is of type Any.
     """
-    name = cast("Any", getattr(field.outer_type_, "_name", None))
-    return (name is not None and "Any" in name) or field.type_ is Any
+    name = cast("Any", getattr(field.annotation, "_name", None))
+    return (name is not None and "Any" in name) or field.annotation is Any
```

### Comparing `esmerald-1.3.0/LICENSE` & `esmerald-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esmerald-1.3.0/README.md` & `esmerald-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -342,15 +342,15 @@
     @get(path='/{url}')
     async def home(request: Request, url: str) -> Response:
         return Response(f"URL: {url}")
 
     @post(path='/{url}', status_code=status.HTTP_201_CREATED)
     async def mars(request: Request, url: str) -> JSONResponse:
         ...
-    
+
     @websocket(path="/{path_param:str}")
     async def pluto(self, socket: Websocket) -> None:
         await socket.accept()
         msg = await socket.receive_json()
         assert msg
         assert socket
         await socket.close()
@@ -490,14 +490,30 @@
 INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
 INFO:     Started reloader process [28720]
 INFO:     Started server process [28722]
 INFO:     Waiting for application startup.
 INFO:     Application startup complete.
 ```
 
+## OpenAPI documentation
+
+Esmerald also comes with OpenAPI docs integrated. For those used to that, this is roughly the same and to make it
+happen, there were inspirations that helped Esmerald getting there fast.
+
+Esmerald starts automatically the OpenAPI documentation by injecting the OpenAPIConfig default from
+the settings and makes Swagger and ReDoc available to you out of the box.
+
+To access the OpenAPI, simply start your local development and access:
+
+* **Swagger** - `/docs/swagger`.
+* **Redoc** - `/docs/redoc`.
+
+There are more details about [how to configure the OpenAPIConfig](https://esmerald.dev/configurations/openapi/config.md)
+within the documentation.
+
 ## Notes
 
 This is just a very high-level demonstration of how to start quickly and what Esmerald can do.
 There are plenty more things you can do with Esmerald. Enjoy! 😊
 
 ## Sponsors
```

#### html2text {}

```diff
@@ -173,13 +173,22 @@
 127.0.0.1:8000 (Press CTRL+C to quit) INFO: Started reloader process [28720]
 INFO: Started server process [28722] INFO: Waiting for application startup.
 INFO: Application startup complete. ``` ## Run the application with custom
 settings **Using uvicorn**: ```shell ESMERALD_SETTINGS_MODULE=myapp.AppSettings
 uvicorn src:app --reload INFO: Uvicorn running on http://127.0.0.1:8000 (Press
 CTRL+C to quit) INFO: Started reloader process [28720] INFO: Started server
 process [28722] INFO: Waiting for application startup. INFO: Application
-startup complete. ``` ## Notes This is just a very high-level demonstration of
-how to start quickly and what Esmerald can do. There are plenty more things you
-can do with Esmerald. Enjoy! ð ## Sponsors Currently there are no sponsors
-of Esmerald but you can financially help and support the author though [GitHub
+startup complete. ``` ## OpenAPI documentation Esmerald also comes with OpenAPI
+docs integrated. For those used to that, this is roughly the same and to make
+it happen, there were inspirations that helped Esmerald getting there fast.
+Esmerald starts automatically the OpenAPI documentation by injecting the
+OpenAPIConfig default from the settings and makes Swagger and ReDoc available
+to you out of the box. To access the OpenAPI, simply start your local
+development and access: * **Swagger** - `/docs/swagger`. * **Redoc** - `/docs/
+redoc`. There are more details about [how to configure the OpenAPIConfig]
+(https://esmerald.dev/configurations/openapi/config.md) within the
+documentation. ## Notes This is just a very high-level demonstration of how to
+start quickly and what Esmerald can do. There are plenty more things you can do
+with Esmerald. Enjoy! ð ## Sponsors Currently there are no sponsors of
+Esmerald but you can financially help and support the author though [GitHub
 sponsors](https://github.com/sponsors/tarsil) and become a **Special one** or a
 **Legend**.
```

### Comparing `esmerald-1.3.0/pyproject.toml` & `esmerald-2.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -38,25 +38,27 @@
     "Topic :: Internet :: WWW/HTTP",
 ]
 dependencies = [
     "a2wsgi>=1.7.0,<2",
     "aiofiles>=0.8.0,<24",
     "anyio>=3.6.2,<4.0.0",
     "awesome-slugify>=1.6.5,<2",
+    "click>=8.1.4,<9.0.0",
     "httpx>=0.24.0,<0.30.0",
     "itsdangerous>=2.1.2,<3.0.0",
     "jinja2>=3.1.2,<4.0.0",
     "jsonschema_rs>=0.16.2,<0.20.0",
-    "loguru>=0.6.0,<0.7.0",
-    "pydantic>=1.10.9,<2.0.0",
-    "pyfactories>=1.0.0",
+    "loguru>=0.7.0,<0.8.0",
+    "pydantic>=2.0.1,<3.0.0",
+    "pydantic-extra-types>=2.0.0,<3.0.0",
+    "pydantic-settings>=2.0.0,<3.0.0",
     "python-multipart>=0.0.5,<0.0.7",
-    "openapi-schemas-pydantic>=1.1.0",
+    "openapi-schemas-pydantic>=2.0.0",
     "rich>=13.3.1,<14.0.0",
-    "starlette>=0.28.0,<1.0",
+    "starlette>=0.29.0,<1.0",
 ]
 keywords = [
     "api",
     "rest",
     "http",
     "asgi",
     "pydantic",
@@ -95,32 +97,33 @@
     "pytest-asyncio>=0.19.0",
     "mypy>=1.4.1",
     "flake8>=5.0.4",
     "black== 23.3.0",
     "isort>=5.0.6,<6.0.0",
     "aiofiles>=0.8.0,<24",
     "a2wsgi>=1.7.0,<2",
-    "asyncz>=0.3.1",
+    "asyncz>=0.4.0",
     "anyio[trio]>=3.6.2,<4.0.0",
     "asyncio[trio]>=3.4.3,<4.0.0",
     "brotli>=1.0.9,<2.0.0",
     "jinja2>=3.1.2,<4.0.0",
     "flask>=1.1.2,<3.0.0",
     "freezegun>=1.2.2,<2.0.0",
     "mock==5.0.1",
     "passlib==1.7.4",
+    "polyfactory>=2.5.0,<3.0.0",
     "python-jose>=3.3.0,<4",
     "orjson>=3.8.5,<4.0.0",
-    "saffier[postgres]>=0.13.0",
+    "saffier[postgres]>=0.14.0",
     "requests>=2.28.2,<3.0.0",
     "ruff>=0.0.256,<1.0.0",
     "ujson>=5.7.0,<6",
 
     # types
-    "types-ujson==5.7.0.5",
+    "types-ujson==5.8.0.0",
     "types-orjson==3.6.2",
 ]
 
 dev = [
     "autoflake>=1.4.0",
     "flake8>=3.8.3,<6.0.0",
     "uvicorn[standard]>=0.19.0",
@@ -140,15 +143,15 @@
 
 templates = ["mako==1.2.4"]
 
 jwt = ["passlib==1.7.4", "python-jose>=3.3.0,<4"]
 
 encoders = ["orjson>=3.8.5,<4.0.0", "ujson>=5.7.0,<6"]
 
-schedulers = ["asyncz>=0.2.0"]
+schedulers = ["asyncz>=0.4.0"]
 
 [tool.hatch.version]
 path = "esmerald/__init__.py"
 
 [project.scripts]
 esmerald = "esmerald.core.directives.cli:esmerald_cli"
```

### Comparing `esmerald-1.3.0/PKG-INFO` & `esmerald-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esmerald
-Version: 1.3.0
+Version: 2.0.0
 Summary: Highly scalable, performant, easy to learn, easy to code and for every application.
 Project-URL: Homepage, https://github.com/dymmond/esmerald
 Project-URL: Documentation, https://esmerald.dymmond.com/
 Project-URL: Changelog, https://esmerald.dymmond.com/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/dymmond/esmerald
 Author-email: Tiago Silva <tiago.silva@dymmond.com>
@@ -36,25 +36,27 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: a2wsgi<2,>=1.7.0
 Requires-Dist: aiofiles<24,>=0.8.0
 Requires-Dist: anyio<4.0.0,>=3.6.2
 Requires-Dist: awesome-slugify<2,>=1.6.5
+Requires-Dist: click<9.0.0,>=8.1.4
 Requires-Dist: httpx<0.30.0,>=0.24.0
 Requires-Dist: itsdangerous<3.0.0,>=2.1.2
 Requires-Dist: jinja2<4.0.0,>=3.1.2
 Requires-Dist: jsonschema-rs<0.20.0,>=0.16.2
-Requires-Dist: loguru<0.7.0,>=0.6.0
-Requires-Dist: openapi-schemas-pydantic>=1.1.0
-Requires-Dist: pydantic<2.0.0,>=1.10.9
-Requires-Dist: pyfactories>=1.0.0
+Requires-Dist: loguru<0.8.0,>=0.7.0
+Requires-Dist: openapi-schemas-pydantic>=2.0.0
+Requires-Dist: pydantic-extra-types<3.0.0,>=2.0.0
+Requires-Dist: pydantic-settings<3.0.0,>=2.0.0
+Requires-Dist: pydantic<3.0.0,>=2.0.1
 Requires-Dist: python-multipart<0.0.7,>=0.0.5
 Requires-Dist: rich<14.0.0,>=13.3.1
-Requires-Dist: starlette<1.0,>=0.28.0
+Requires-Dist: starlette<1.0,>=0.29.0
 Provides-Extra: dev
 Requires-Dist: autoflake>=1.4.0; extra == 'dev'
 Requires-Dist: flake8<6.0.0,>=3.8.3; extra == 'dev'
 Requires-Dist: pre-commit<4.0.0,>=3.0.4; extra == 'dev'
 Requires-Dist: uvicorn[standard]>=0.19.0; extra == 'dev'
 Requires-Dist: watchfiles<0.20.0,>=0.16.1; extra == 'dev'
 Provides-Extra: doc
@@ -68,43 +70,44 @@
 Provides-Extra: encoders
 Requires-Dist: orjson<4.0.0,>=3.8.5; extra == 'encoders'
 Requires-Dist: ujson<6,>=5.7.0; extra == 'encoders'
 Provides-Extra: jwt
 Requires-Dist: passlib==1.7.4; extra == 'jwt'
 Requires-Dist: python-jose<4,>=3.3.0; extra == 'jwt'
 Provides-Extra: schedulers
-Requires-Dist: asyncz>=0.2.0; extra == 'schedulers'
+Requires-Dist: asyncz>=0.4.0; extra == 'schedulers'
 Provides-Extra: templates
 Requires-Dist: mako==1.2.4; extra == 'templates'
 Provides-Extra: test
 Requires-Dist: a2wsgi<2,>=1.7.0; extra == 'test'
 Requires-Dist: aiofiles<24,>=0.8.0; extra == 'test'
 Requires-Dist: anyio[trio]<4.0.0,>=3.6.2; extra == 'test'
 Requires-Dist: asyncio[trio]<4.0.0,>=3.4.3; extra == 'test'
-Requires-Dist: asyncz>=0.3.1; extra == 'test'
+Requires-Dist: asyncz>=0.4.0; extra == 'test'
 Requires-Dist: black==23.3.0; extra == 'test'
 Requires-Dist: brotli<2.0.0,>=1.0.9; extra == 'test'
 Requires-Dist: flake8>=5.0.4; extra == 'test'
 Requires-Dist: flask<3.0.0,>=1.1.2; extra == 'test'
 Requires-Dist: freezegun<2.0.0,>=1.2.2; extra == 'test'
 Requires-Dist: isort<6.0.0,>=5.0.6; extra == 'test'
 Requires-Dist: jinja2<4.0.0,>=3.1.2; extra == 'test'
 Requires-Dist: mock==5.0.1; extra == 'test'
 Requires-Dist: mypy>=1.4.1; extra == 'test'
 Requires-Dist: orjson<4.0.0,>=3.8.5; extra == 'test'
 Requires-Dist: passlib==1.7.4; extra == 'test'
+Requires-Dist: polyfactory<3.0.0,>=2.5.0; extra == 'test'
 Requires-Dist: pytest-asyncio>=0.19.0; extra == 'test'
 Requires-Dist: pytest-cov<5.0.0,>=2.12.0; extra == 'test'
 Requires-Dist: pytest<8.0.0,>=7.3.1; extra == 'test'
 Requires-Dist: python-jose<4,>=3.3.0; extra == 'test'
 Requires-Dist: requests<3.0.0,>=2.28.2; extra == 'test'
 Requires-Dist: ruff<1.0.0,>=0.0.256; extra == 'test'
-Requires-Dist: saffier[postgres]>=0.13.0; extra == 'test'
+Requires-Dist: saffier[postgres]>=0.14.0; extra == 'test'
 Requires-Dist: types-orjson==3.6.2; extra == 'test'
-Requires-Dist: types-ujson==5.7.0.5; extra == 'test'
+Requires-Dist: types-ujson==5.8.0.0; extra == 'test'
 Requires-Dist: ujson<6,>=5.7.0; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Esmerald
 
 <p align="center">
   <a href="https://esmerald.dymmond.com"><img src="https://res.cloudinary.com/dymmond/image/upload/v1673619342/esmerald/img/logo-gr_z1ot8o.png" alt='Esmerald'></a>
@@ -448,15 +451,15 @@
     @get(path='/{url}')
     async def home(request: Request, url: str) -> Response:
         return Response(f"URL: {url}")
 
     @post(path='/{url}', status_code=status.HTTP_201_CREATED)
     async def mars(request: Request, url: str) -> JSONResponse:
         ...
-    
+
     @websocket(path="/{path_param:str}")
     async def pluto(self, socket: Websocket) -> None:
         await socket.accept()
         msg = await socket.receive_json()
         assert msg
         assert socket
         await socket.close()
@@ -596,14 +599,30 @@
 INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
 INFO:     Started reloader process [28720]
 INFO:     Started server process [28722]
 INFO:     Waiting for application startup.
 INFO:     Application startup complete.
 ```
 
+## OpenAPI documentation
+
+Esmerald also comes with OpenAPI docs integrated. For those used to that, this is roughly the same and to make it
+happen, there were inspirations that helped Esmerald getting there fast.
+
+Esmerald starts automatically the OpenAPI documentation by injecting the OpenAPIConfig default from
+the settings and makes Swagger and ReDoc available to you out of the box.
+
+To access the OpenAPI, simply start your local development and access:
+
+* **Swagger** - `/docs/swagger`.
+* **Redoc** - `/docs/redoc`.
+
+There are more details about [how to configure the OpenAPIConfig](https://esmerald.dev/configurations/openapi/config.md)
+within the documentation.
+
 ## Notes
 
 This is just a very high-level demonstration of how to start quickly and what Esmerald can do.
 There are plenty more things you can do with Esmerald. Enjoy! 😊
 
 ## Sponsors
```

