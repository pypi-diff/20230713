# Comparing `tmp/jupyverse-0.1.9.tar.gz` & `tmp/jupyverse-0.2.0.tar.gz`

## Comparing `jupyverse-0.1.9.tar` & `jupyverse-0.2.0.tar`

### file list

```diff
@@ -1,218 +1,218 @@
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 jupyverse-0.1.9/.pre-commit-config.yaml
--rw-r--r--   0        0        0    64563 2020-02-02 00:00:00.000000 jupyverse-0.1.9/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 jupyverse-0.1.9/CONTRIBUTING.md
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.1.9/MANIFEST.in
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 jupyverse-0.1.9/config.yaml
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 jupyverse-0.1.9/mkdocs.yml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 jupyverse-0.1.9/pytest.ini
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 jupyverse-0.1.9/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyverse-0.1.9/.devcontainer/requirements.txt
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 jupyverse-0.1.9/.github/workflows/check-release.yml
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 jupyverse-0.1.9/.github/workflows/main.yml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 jupyverse-0.1.9/binder/environment.yml
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 jupyverse-0.1.9/binder/jupyter_notebook_config.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyverse-0.1.9/binder/postBuild
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 jupyverse-0.1.9/binder/start
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 jupyverse-0.1.9/docs/index.md
--rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 jupyverse-0.1.9/docs/install.md
--rw-r--r--   0        0        0    11002 2020-02-02 00:00:00.000000 jupyverse-0.1.9/docs/jupyter.svg
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 jupyverse-0.1.9/docs/plugins/auth.md
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jupyverse-0.1.9/docs/plugins/contents.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 jupyverse-0.1.9/docs/plugins/frontend.md
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyverse-0.1.9/docs/plugins/jupyterlab.md
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyverse-0.1.9/docs/plugins/kernels.md
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 jupyverse-0.1.9/docs/plugins/lab.md
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyverse-0.1.9/docs/plugins/login.md
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyverse-0.1.9/docs/plugins/nbconvert.md
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 jupyverse-0.1.9/docs/plugins/resource_usage.md
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jupyverse-0.1.9/docs/plugins/retrolab.md
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 jupyverse-0.1.9/docs/plugins/terminals.md
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyverse-0.1.9/docs/plugins/yjs.md
--rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 jupyverse-0.1.9/docs/usage/microservices.md
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 jupyverse-0.1.9/docs/usage/multi_user.md
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 jupyverse-0.1.9/docs/usage/single_user.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse/py.typed
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/COPYING.md
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/README.md
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/pyproject.toml
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/__init__.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/cli.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/py.typed
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/app/__init__.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/auth/__init__.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/auth/models.py
--rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/contents/__init__.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/contents/models.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/frontend/__init__.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/jupyterlab/__init__.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/kernels/__init__.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/kernels/models.py
--rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/lab/__init__.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/login/__init__.py
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/main/__init__.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/nbconvert/__init__.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/resource_usage/__init__.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/retrolab/__init__.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/terminals/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/terminals/models.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/yjs/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/yjs/models.py
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 jupyverse-0.1.9/notebooks/admin_users.ipynb
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 jupyverse-0.1.9/notebooks/admin_users.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth/MANIFEST.in
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth/README.md
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth/fps_auth/__init__.py
--rw-r--r--   0        0        0    11596 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth/fps_auth/backends.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth/fps_auth/config.py
--rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth/fps_auth/db.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth/fps_auth/main.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth/fps_auth/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth/fps_auth/py.typed
--rw-r--r--   0        0        0     7820 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth/fps_auth/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth_fief/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth_fief/MANIFEST.in
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth_fief/README.md
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth_fief/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth_fief/fps_auth_fief/__init__.py
--rw-r--r--   0        0        0     3850 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth_fief/fps_auth_fief/backend.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth_fief/fps_auth_fief/config.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth_fief/fps_auth_fief/main.py
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth_fief/fps_auth_fief/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/contents/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/contents/MANIFEST.in
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/contents/README.md
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/contents/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/contents/fps_contents/__init__.py
--rw-r--r--   0        0        0     8561 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/contents/fps_contents/fileid.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/contents/fps_contents/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/contents/fps_contents/py.typed
--rw-r--r--   0        0        0     9809 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/contents/fps_contents/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/frontend/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/frontend/MANIFEST.in
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/frontend/README.md
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/frontend/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/frontend/fps_frontend/__init__.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/frontend/fps_frontend/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/frontend/fps_frontend/py.typed
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/jupyterlab/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/jupyterlab/MANIFEST.in
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/jupyterlab/README.md
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/jupyterlab/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/jupyterlab/fps_jupyterlab/__init__.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/jupyterlab/fps_jupyterlab/index.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/jupyterlab/fps_jupyterlab/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/jupyterlab/fps_jupyterlab/py.typed
--rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/jupyterlab/fps_jupyterlab/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/kernels/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/kernels/MANIFEST.in
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/kernels/README.md
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/kernels/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/kernels/fps_kernels/__init__.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/kernels/fps_kernels/main.py
--rw-r--r--   0        0        0    13257 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/kernels/fps_kernels/routes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/kernels/fps_kernels/kernel_driver/__init__.py
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/kernels/fps_kernels/kernel_driver/connect.py
--rw-r--r--   0        0        0     8632 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/kernels/fps_kernels/kernel_driver/driver.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py
--rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/kernels/fps_kernels/kernel_driver/message.py
--rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/kernels/fps_kernels/kernel_driver/paths.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/kernels/fps_kernels/kernel_server/__init__.py
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/kernels/fps_kernels/kernel_server/message.py
--rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/kernels/fps_kernels/kernel_server/server.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/lab/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/lab/MANIFEST.in
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/lab/README.md
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/lab/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/lab/fps_lab/__init__.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/lab/fps_lab/main.py
--rw-r--r--   0        0        0     7307 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/lab/fps_lab/routes.py
--rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/lab/fps_lab/static/favicon.ico
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/login/COPYING.md
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/login/MANIFEST.in
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/login/README.md
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/login/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/login/fps_login/__init__.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/login/fps_login/main.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/login/fps_login/routes.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/login/fps_login/static/index.html
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/login/fps_login/static/favicons/favicon-busy-1.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/login/fps_login/static/favicons/favicon-busy-2.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/login/fps_login/static/favicons/favicon-busy-3.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/login/fps_login/static/favicons/favicon-file.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/login/fps_login/static/favicons/favicon-notebook.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/login/fps_login/static/favicons/favicon-terminal.ico
--rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/login/fps_login/static/favicons/favicon.ico
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/login/fps_login/static/logo/github.svg
--rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/login/fps_login/static/logo/logo.png
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/login/fps_login/static/style/index.css
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/nbconvert/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/nbconvert/MANIFEST.in
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/nbconvert/README.md
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/nbconvert/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/nbconvert/fps_nbconvert/__init__.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/nbconvert/fps_nbconvert/main.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/nbconvert/fps_nbconvert/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/noauth/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/noauth/MANIFEST.in
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/noauth/README.md
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/noauth/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/noauth/fps_noauth/__init__.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/noauth/fps_noauth/backends.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/noauth/fps_noauth/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/noauth/fps_noauth/py.typed
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/resource_usage/COPYING.md
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/resource_usage/README.md
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/resource_usage/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/resource_usage/fps_resource_usage/__init__.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/resource_usage/fps_resource_usage/main.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/resource_usage/fps_resource_usage/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/retrolab/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/retrolab/MANIFEST.in
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/retrolab/README.md
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/retrolab/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/retrolab/fps_retrolab/__init__.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/retrolab/fps_retrolab/main.py
--rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/retrolab/fps_retrolab/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/terminals/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/terminals/MANIFEST.in
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/terminals/README.md
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/terminals/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/terminals/fps_terminals/__init__.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/terminals/fps_terminals/main.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/terminals/fps_terminals/routes.py
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/terminals/fps_terminals/server.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/terminals/fps_terminals/win_server.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/webdav/COPYING.md
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/webdav/README.md
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/webdav/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/webdav/fps_webdav/__init__.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/webdav/fps_webdav/config.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/webdav/fps_webdav/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/webdav/fps_webdav/py.typed
--rw-r--r--   0        0        0     3596 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/webdav/fps_webdav/routes.py
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/webdav/tests/test_webdav.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/yjs/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/yjs/MANIFEST.in
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/yjs/README.md
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/yjs/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/yjs/fps_yjs/__init__.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/yjs/fps_yjs/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/yjs/fps_yjs/py.typed
--rw-r--r--   0        0        0    14864 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/yjs/fps_yjs/routes.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 jupyverse-0.1.9/tests/conftest.py
--rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 jupyverse-0.1.9/tests/test_auth.py
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupyverse-0.1.9/tests/test_contents.py
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 jupyverse-0.1.9/tests/test_kernels.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 jupyverse-0.1.9/tests/test_server.py
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 jupyverse-0.1.9/tests/test_settings.py
--rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 jupyverse-0.1.9/tests/utils.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 jupyverse-0.1.9/tests/data/notebook0.ipynb
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 jupyverse-0.1.9/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.9/COPYING.md
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 jupyverse-0.1.9/README.md
--rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 jupyverse-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 jupyverse-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 jupyverse-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    66836 2020-02-02 00:00:00.000000 jupyverse-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 jupyverse-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.2.0/MANIFEST.in
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 jupyverse-0.2.0/config.yaml
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 jupyverse-0.2.0/mkdocs.yml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 jupyverse-0.2.0/pytest.ini
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 jupyverse-0.2.0/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyverse-0.2.0/.devcontainer/requirements.txt
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 jupyverse-0.2.0/.github/workflows/check-release.yml
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 jupyverse-0.2.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 jupyverse-0.2.0/binder/environment.yml
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 jupyverse-0.2.0/binder/jupyter_notebook_config.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyverse-0.2.0/binder/postBuild
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 jupyverse-0.2.0/binder/start
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 jupyverse-0.2.0/docs/index.md
+-rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 jupyverse-0.2.0/docs/install.md
+-rw-r--r--   0        0        0    11002 2020-02-02 00:00:00.000000 jupyverse-0.2.0/docs/jupyter.svg
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 jupyverse-0.2.0/docs/plugins/auth.md
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jupyverse-0.2.0/docs/plugins/contents.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 jupyverse-0.2.0/docs/plugins/frontend.md
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyverse-0.2.0/docs/plugins/jupyterlab.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyverse-0.2.0/docs/plugins/kernels.md
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 jupyverse-0.2.0/docs/plugins/lab.md
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyverse-0.2.0/docs/plugins/login.md
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyverse-0.2.0/docs/plugins/nbconvert.md
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 jupyverse-0.2.0/docs/plugins/resource_usage.md
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jupyverse-0.2.0/docs/plugins/retrolab.md
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 jupyverse-0.2.0/docs/plugins/terminals.md
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyverse-0.2.0/docs/plugins/yjs.md
+-rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 jupyverse-0.2.0/docs/usage/microservices.md
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 jupyverse-0.2.0/docs/usage/multi_user.md
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 jupyverse-0.2.0/docs/usage/single_user.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse/py.typed
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/COPYING.md
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/README.md
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/pyproject.toml
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/__init__.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/cli.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/py.typed
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/app/__init__.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/auth/__init__.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/auth/models.py
+-rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/contents/__init__.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/contents/models.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/frontend/__init__.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/jupyterlab/__init__.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/kernels/__init__.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/kernels/models.py
+-rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/lab/__init__.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/login/__init__.py
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/main/__init__.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/nbconvert/__init__.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/resource_usage/__init__.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/retrolab/__init__.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/terminals/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/terminals/models.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/yjs/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/yjs/models.py
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 jupyverse-0.2.0/notebooks/admin_users.ipynb
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 jupyverse-0.2.0/notebooks/admin_users.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth/MANIFEST.in
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth/README.md
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth/fps_auth/__init__.py
+-rw-r--r--   0        0        0    11618 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth/fps_auth/backends.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth/fps_auth/config.py
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth/fps_auth/db.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth/fps_auth/main.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth/fps_auth/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth/fps_auth/py.typed
+-rw-r--r--   0        0        0     7820 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth/fps_auth/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth_fief/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth_fief/MANIFEST.in
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth_fief/README.md
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth_fief/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth_fief/fps_auth_fief/__init__.py
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth_fief/fps_auth_fief/backend.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth_fief/fps_auth_fief/config.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth_fief/fps_auth_fief/main.py
+-rw-r--r--   0        0        0     7029 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth_fief/fps_auth_fief/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/contents/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/contents/MANIFEST.in
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/contents/README.md
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/contents/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/contents/fps_contents/__init__.py
+-rw-r--r--   0        0        0     8561 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/contents/fps_contents/fileid.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/contents/fps_contents/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/contents/fps_contents/py.typed
+-rw-r--r--   0        0        0     9815 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/contents/fps_contents/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/frontend/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/frontend/MANIFEST.in
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/frontend/README.md
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/frontend/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/frontend/fps_frontend/__init__.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/frontend/fps_frontend/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/frontend/fps_frontend/py.typed
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/jupyterlab/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/jupyterlab/MANIFEST.in
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/jupyterlab/README.md
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/jupyterlab/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/jupyterlab/fps_jupyterlab/__init__.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/jupyterlab/fps_jupyterlab/index.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/jupyterlab/fps_jupyterlab/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/jupyterlab/fps_jupyterlab/py.typed
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/jupyterlab/fps_jupyterlab/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/kernels/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/kernels/MANIFEST.in
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/kernels/README.md
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/kernels/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/kernels/fps_kernels/__init__.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/kernels/fps_kernels/main.py
+-rw-r--r--   0        0        0    13257 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/kernels/fps_kernels/routes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/kernels/fps_kernels/kernel_driver/__init__.py
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/kernels/fps_kernels/kernel_driver/connect.py
+-rw-r--r--   0        0        0     8632 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/kernels/fps_kernels/kernel_driver/driver.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py
+-rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/kernels/fps_kernels/kernel_driver/message.py
+-rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/kernels/fps_kernels/kernel_driver/paths.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/kernels/fps_kernels/kernel_server/__init__.py
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/kernels/fps_kernels/kernel_server/message.py
+-rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/kernels/fps_kernels/kernel_server/server.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/lab/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/lab/MANIFEST.in
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/lab/README.md
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/lab/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/lab/fps_lab/__init__.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/lab/fps_lab/main.py
+-rw-r--r--   0        0        0     7307 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/lab/fps_lab/routes.py
+-rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/lab/fps_lab/static/favicon.ico
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/login/COPYING.md
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/login/MANIFEST.in
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/login/README.md
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/login/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/login/fps_login/__init__.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/login/fps_login/main.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/login/fps_login/routes.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/login/fps_login/static/index.html
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/login/fps_login/static/favicons/favicon-busy-1.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/login/fps_login/static/favicons/favicon-busy-2.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/login/fps_login/static/favicons/favicon-busy-3.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/login/fps_login/static/favicons/favicon-file.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/login/fps_login/static/favicons/favicon-notebook.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/login/fps_login/static/favicons/favicon-terminal.ico
+-rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/login/fps_login/static/favicons/favicon.ico
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/login/fps_login/static/logo/github.svg
+-rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/login/fps_login/static/logo/logo.png
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/login/fps_login/static/style/index.css
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/nbconvert/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/nbconvert/MANIFEST.in
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/nbconvert/README.md
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/nbconvert/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/nbconvert/fps_nbconvert/__init__.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/nbconvert/fps_nbconvert/main.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/nbconvert/fps_nbconvert/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/noauth/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/noauth/MANIFEST.in
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/noauth/README.md
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/noauth/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/noauth/fps_noauth/__init__.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/noauth/fps_noauth/backends.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/noauth/fps_noauth/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/noauth/fps_noauth/py.typed
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/resource_usage/COPYING.md
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/resource_usage/README.md
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/resource_usage/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/resource_usage/fps_resource_usage/__init__.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/resource_usage/fps_resource_usage/main.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/resource_usage/fps_resource_usage/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/retrolab/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/retrolab/MANIFEST.in
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/retrolab/README.md
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/retrolab/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/retrolab/fps_retrolab/__init__.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/retrolab/fps_retrolab/main.py
+-rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/retrolab/fps_retrolab/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/terminals/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/terminals/MANIFEST.in
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/terminals/README.md
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/terminals/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/terminals/fps_terminals/__init__.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/terminals/fps_terminals/main.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/terminals/fps_terminals/routes.py
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/terminals/fps_terminals/server.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/terminals/fps_terminals/win_server.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/webdav/COPYING.md
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/webdav/README.md
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/webdav/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/webdav/fps_webdav/__init__.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/webdav/fps_webdav/config.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/webdav/fps_webdav/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/webdav/fps_webdav/py.typed
+-rw-r--r--   0        0        0     3596 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/webdav/fps_webdav/routes.py
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/webdav/tests/test_webdav.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/yjs/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/yjs/MANIFEST.in
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/yjs/README.md
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/yjs/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/yjs/fps_yjs/__init__.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/yjs/fps_yjs/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/yjs/fps_yjs/py.typed
+-rw-r--r--   0        0        0    15108 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/yjs/fps_yjs/routes.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 jupyverse-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 jupyverse-0.2.0/tests/test_auth.py
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupyverse-0.2.0/tests/test_contents.py
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 jupyverse-0.2.0/tests/test_kernels.py
+-rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 jupyverse-0.2.0/tests/test_server.py
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 jupyverse-0.2.0/tests/test_settings.py
+-rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 jupyverse-0.2.0/tests/utils.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 jupyverse-0.2.0/tests/data/notebook0.ipynb
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 jupyverse-0.2.0/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.0/COPYING.md
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 jupyverse-0.2.0/README.md
+-rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 jupyverse-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 jupyverse-0.2.0/PKG-INFO
```

### Comparing `jupyverse-0.1.9/.pre-commit-config.yaml` & `jupyverse-0.2.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -16,12 +16,12 @@
       - id: trailing-whitespace
 
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
 
-  - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.270
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.0.277
     hooks:
       - id: ruff
         args: ["--fix"]
```

### Comparing `jupyverse-0.1.9/CHANGELOG.md` & `jupyverse-0.2.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,45 @@
 # Changes in Jupyverse {#changelog}
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.2.0
+
+([Full Changelog](https://github.com/jupyter-server/jupyverse/compare/v0.1.10...ebf0e6d40a593eccccaf3ae2753e6ad272135e3b))
+
+### Merged PRs
+
+- Rerun flaky tests [#331](https://github.com/jupyter-server/jupyverse/pull/331) ([@davidbrochart](https://github.com/davidbrochart))
+- Use pydantic v2 [#330](https://github.com/jupyter-server/jupyverse/pull/330) ([@davidbrochart](https://github.com/davidbrochart))
+- Update fastapi-users v12 [#329](https://github.com/jupyter-server/jupyverse/pull/329) ([@davidbrochart](https://github.com/davidbrochart))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter-server/jupyverse/graphs/contributors?from=2023-07-05&to=2023-07-13&type=c))
+
+[@davidbrochart](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Adavidbrochart+updated%3A2023-07-05..2023-07-13&type=Issues) | [@frankie567](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Afrankie567+updated%3A2023-07-05..2023-07-13&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Apre-commit-ci+updated%3A2023-07-05..2023-07-13&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
+## 0.1.10
+
+([Full Changelog](https://github.com/jupyter-server/jupyverse/compare/v0.1.9...e15a7e4091cfa94dff41b05cf273ed92438ad299))
+
+### Merged PRs
+
+- Pin ypy-websocket \<0.11 [#325](https://github.com/jupyter-server/jupyverse/pull/325) ([@davidbrochart](https://github.com/davidbrochart))
+- Add GitHub authentication with fps-auth-fief [#324](https://github.com/jupyter-server/jupyverse/pull/324) ([@davidbrochart](https://github.com/davidbrochart))
+- Support ypy-websocket v0.12 [#320](https://github.com/jupyter-server/jupyverse/pull/320) ([@davidbrochart](https://github.com/davidbrochart))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter-server/jupyverse/graphs/contributors?from=2023-06-06&to=2023-07-05&type=c))
+
+[@davidbrochart](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Adavidbrochart+updated%3A2023-06-06..2023-07-05&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Apre-commit-ci+updated%3A2023-06-06..2023-07-05&type=Issues)
+
 ## 0.1.9
 
 ([Full Changelog](https://github.com/jupyter-server/jupyverse/compare/v0.1.8...ab09a2ea41fcdab226ec55541a26329c3d5b7583))
 
 ### Merged PRs
 
 - Fix fps-webdav logging config [#317](https://github.com/jupyter-server/jupyverse/pull/317) ([@davidbrochart](https://github.com/davidbrochart))
@@ -14,16 +48,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter-server/jupyverse/graphs/contributors?from=2023-05-31&to=2023-06-06&type=c))
 
 [@davidbrochart](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Adavidbrochart+updated%3A2023-05-31..2023-06-06&type=Issues) | [@trungleduc](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Atrungleduc+updated%3A2023-05-31..2023-06-06&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.1.8
 
 No merged PRs
 
 ## 0.1.7
 
 ([Full Changelog](https://github.com/jupyter-server/jupyverse/compare/v0.1.6...d1d54a22429136b87fd45b7540d43937b2e6b695))
```

### Comparing `jupyverse-0.1.9/CONTRIBUTING.md` & `jupyverse-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/config.yaml` & `jupyverse-0.2.0/config.yaml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/mkdocs.yml` & `jupyverse-0.2.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/.devcontainer/devcontainer.json` & `jupyverse-0.2.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/.github/workflows/check-release.yml` & `jupyverse-0.2.0/.github/workflows/check-release.yml`

 * *Files 0% similar despite different names*

```diff
@@ -55,10 +55,10 @@
           pip install -e plugins/yjs
           pip install -e plugins/auth
           pip install -e plugins/noauth
           pip install -e plugins/auth_fief
           pip install -e plugins/login
       - name: Check Release
         if: ${{ matrix.group == 'check_release' }}
-        uses: jupyter-server/jupyter_releaser/.github/actions/check-release@v1
+        uses: jupyter-server/jupyter_releaser/.github/actions/check-release@v2
         with:
           token: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `jupyverse-0.1.9/.github/workflows/main.yml` & `jupyverse-0.2.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/binder/jupyter_notebook_config.py` & `jupyverse-0.2.0/binder/jupyter_notebook_config.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/docs/index.md` & `jupyverse-0.2.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/docs/install.md` & `jupyverse-0.2.0/docs/install.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/docs/jupyter.svg` & `jupyverse-0.2.0/docs/jupyter.svg`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/docs/plugins/auth.md` & `jupyverse-0.2.0/docs/plugins/auth.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/docs/usage/microservices.md` & `jupyverse-0.2.0/docs/usage/microservices.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/docs/usage/multi_user.md` & `jupyverse-0.2.0/docs/usage/multi_user.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/docs/usage/single_user.md` & `jupyverse-0.2.0/docs/usage/single_user.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/jupyverse_api/COPYING.md` & `jupyverse-0.2.0/jupyverse_api/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/jupyverse_api/pyproject.toml` & `jupyverse-0.2.0/jupyverse_api/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-  "pydantic >=1.10.6,<2",
+  "pydantic >=2,<3",
   "fastapi >=0.95.0,<1",
   "rich-click >=1.6.1,<2",
   "asphalt >=4.11.0,<5",
   "asphalt-web[fastapi] >=1.1.0,<2",
 ]
 dynamic = ["version"]
```

### Comparing `jupyverse-0.1.9/jupyverse_api/jupyverse_api/__init__.py` & `jupyverse-0.2.0/jupyverse_api/jupyverse_api/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 from typing import Dict
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
 
 from .app import App
 
 
-__version__ = "0.1.9"
+__version__ = "0.2.0"
 
 
 class Singleton(type):
     _instances: Dict = {}
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
             cls._instances[cls] = super(Singleton, cls).__call__(*args, **kwargs)
         return cls._instances[cls]
 
 
 class Config(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = {"extra": "forbid"}
 
 
 class Router:
     _app: App
 
     def __init__(
         self,
```

### Comparing `jupyverse-0.1.9/jupyverse_api/jupyverse_api/cli.py` & `jupyverse-0.2.0/jupyverse_api/jupyverse_api/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pkg_resources
 from typing import List
 
 import rich_click as click
 from asphalt.core.cli import run
 
 
-@click.command()
+@click.command()  # type: ignore
 @click.option(
     "--open-browser",
     is_flag=True,
     show_default=True,
     default=False,
     help="Open a browser window.",
 )
```

### Comparing `jupyverse-0.1.9/jupyverse_api/jupyverse_api/app/__init__.py` & `jupyverse-0.2.0/jupyverse_api/jupyverse_api/app/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/jupyverse_api/jupyverse_api/auth/__init__.py` & `jupyverse-0.2.0/jupyverse_api/jupyverse_api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/jupyverse_api/jupyverse_api/contents/__init__.py` & `jupyverse-0.2.0/jupyverse_api/jupyverse_api/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/jupyverse_api/jupyverse_api/contents/models.py` & `jupyverse-0.2.0/jupyverse_api/jupyverse_api/contents/models.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/jupyverse_api/jupyverse_api/jupyterlab/__init__.py` & `jupyverse-0.2.0/jupyverse_api/jupyverse_api/jupyterlab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/jupyverse_api/jupyverse_api/kernels/__init__.py` & `jupyverse-0.2.0/jupyverse_api/jupyverse_api/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/jupyverse_api/jupyverse_api/kernels/models.py` & `jupyverse-0.2.0/jupyverse_api/jupyverse_api/kernels/models.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/jupyverse_api/jupyverse_api/lab/__init__.py` & `jupyverse-0.2.0/jupyverse_api/jupyverse_api/lab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/jupyverse_api/jupyverse_api/main/__init__.py` & `jupyverse-0.2.0/jupyverse_api/jupyverse_api/main/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/jupyverse_api/jupyverse_api/nbconvert/__init__.py` & `jupyverse-0.2.0/jupyverse_api/jupyverse_api/nbconvert/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/jupyverse_api/jupyverse_api/resource_usage/__init__.py` & `jupyverse-0.2.0/jupyverse_api/jupyverse_api/resource_usage/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/jupyverse_api/jupyverse_api/retrolab/__init__.py` & `jupyverse-0.2.0/jupyverse_api/jupyverse_api/retrolab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/jupyverse_api/jupyverse_api/terminals/__init__.py` & `jupyverse-0.2.0/jupyverse_api/jupyverse_api/terminals/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/jupyverse_api/jupyverse_api/yjs/__init__.py` & `jupyverse-0.2.0/jupyverse_api/jupyverse_api/yjs/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/notebooks/admin_users.ipynb` & `jupyverse-0.2.0/notebooks/admin_users.ipynb`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/notebooks/admin_users.py` & `jupyverse-0.2.0/notebooks/admin_users.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/auth/COPYING.md` & `jupyverse-0.2.0/plugins/auth/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/auth/pyproject.toml` & `jupyverse-0.2.0/plugins/auth/pyproject.toml`

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

### Comparing `jupyverse-0.1.9/plugins/auth/fps_auth/backends.py` & `jupyverse-0.2.0/plugins/auth/fps_auth/backends.py`

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

### Comparing `jupyverse-0.1.9/plugins/auth/fps_auth/config.py` & `jupyverse-0.2.0/plugins/auth/fps_auth/config.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/auth/fps_auth/db.py` & `jupyverse-0.2.0/plugins/auth/fps_auth/db.py`

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

### Comparing `jupyverse-0.1.9/plugins/auth/fps_auth/main.py` & `jupyverse-0.2.0/plugins/auth/fps_auth/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/auth/fps_auth/routes.py` & `jupyverse-0.2.0/plugins/auth/fps_auth/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/auth_fief/COPYING.md` & `jupyverse-0.2.0/plugins/auth_fief/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/auth_fief/pyproject.toml` & `jupyverse-0.2.0/plugins/auth_fief/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/auth_fief/fps_auth_fief/backend.py` & `jupyverse-0.2.0/plugins/auth_fief/fps_auth_fief/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,37 +6,39 @@
 from fief_client import FiefAccessTokenInfo, FiefAsync, FiefUserInfo
 from fief_client.integrations.fastapi import FiefAuth
 from jupyverse_api.auth import User
 
 from .config import _AuthFiefConfig
 
 
-class CustomFiefAuth(FiefAuth):
-    client: FiefAsync
-
-    async def get_unauthorized_response(self, request: Request, response: Response):
-        redirect_uri = str(request.url_for("auth_callback"))
-        auth_url = await self.client.auth_url(redirect_uri, scope=["openid"])
-        raise HTTPException(
-            status_code=status.HTTP_307_TEMPORARY_REDIRECT,
-            headers={"Location": auth_url},
-        )
-
-
 @dataclass
 class Res:
     fief: FiefAsync
     session_cookie_name: str
-    auth: CustomFiefAuth
+    auth: FiefAuth
     current_user: Any
     update_user: Any
     websocket_auth: Any
 
 
 def get_backend(auth_fief_config: _AuthFiefConfig) -> Res:
+    class CustomFiefAuth(FiefAuth):
+        client: FiefAsync
+
+        async def get_unauthorized_response(self, request: Request, response: Response):
+            if auth_fief_config.callback_url:
+                redirect_uri = auth_fief_config.callback_url
+            else:
+                redirect_uri = str(request.url_for("auth_callback"))
+            auth_url = await self.client.auth_url(redirect_uri, scope=["openid", "offline_access"])
+            raise HTTPException(
+                status_code=status.HTTP_307_TEMPORARY_REDIRECT,
+                headers={"Location": auth_url},
+            )
+
     fief = FiefAsync(
         auth_fief_config.base_url,
         auth_fief_config.client_id,
         auth_fief_config.client_secret,
     )
 
     session_cookie_name = "fps_auth_fief_user_session"
```

### Comparing `jupyverse-0.1.9/plugins/auth_fief/fps_auth_fief/main.py` & `jupyverse-0.2.0/plugins/auth_fief/fps_auth_fief/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/auth_fief/fps_auth_fief/routes.py` & `jupyverse-0.2.0/tests/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,88 +1,120 @@
-import json
-from typing import Any, Callable, Dict, List, Optional, Tuple
-
-from fastapi import APIRouter, Depends, Query, Request, Response
-from fastapi.responses import RedirectResponse
-from fief_client import FiefAccessTokenInfo
-from jupyverse_api import Router
-from jupyverse_api.app import App
-from jupyverse_api.auth import Auth, User
-
-from .backend import get_backend
-from .config import _AuthFiefConfig
-
-
-def auth_factory(
-    app: App,
-    auth_fief_config: _AuthFiefConfig,
-):
-    backend = get_backend(auth_fief_config)
-
-    class _AuthFief(Auth, Router):
-        def __init__(self) -> None:
-            super().__init__(app)
-
-            router = APIRouter()
-
-            @router.get("/auth-callback", name="auth_callback")
-            async def auth_callback(request: Request, response: Response, code: str = Query(...)):
-                redirect_uri = str(request.url_for("auth_callback"))
-                tokens, _ = await backend.fief.auth_callback(code, redirect_uri)
-
-                response = RedirectResponse(request.url_for("root"))
-                response.set_cookie(
-                    backend.session_cookie_name,
-                    tokens["access_token"],
-                    max_age=tokens["expires_in"],
-                    httponly=True,
-                    secure=False,
-                )
-
-                return response
-
-            @router.get("/api/me")
-            async def get_api_me(
-                request: Request,
-                user: User = Depends(self.current_user()),
-                access_token_info: FiefAccessTokenInfo = Depends(backend.auth.authenticated()),
-            ):
-                checked_permissions: Dict[str, List[str]] = {}
-                permissions = json.loads(
-                    dict(request.query_params).get("permissions", "{}").replace("'", '"')
-                )
-                if permissions:
-                    user_permissions: Dict[str, List[str]] = {}
-                    for permission in access_token_info["permissions"]:
-                        resource, action = permission.split(":")
-                        if resource not in user_permissions:
-                            user_permissions[resource] = []
-                        user_permissions[resource].append(action)
-                    for resource, actions in permissions.items():
-                        user_resource_permissions = user_permissions.get(resource, [])
-                        allowed = checked_permissions[resource] = []
-                        for action in actions:
-                            if action in user_resource_permissions:
-                                allowed.append(action)
-
-                keys = ["username", "name", "display_name", "initials", "avatar_url", "color"]
-                identity = {k: getattr(user, k) for k in keys}
-                return {
-                    "identity": identity,
-                    "permissions": checked_permissions,
-                }
-
-            self.include_router(router)
-
-        def current_user(self, permissions: Optional[Dict[str, List[str]]] = None) -> Callable:
-            return backend.current_user(permissions)
-
-        async def update_user(self, update_user=Depends(backend.update_user)) -> Callable:
-            return update_user
-
-        def websocket_auth(
-            self,
-            permissions: Optional[Dict[str, List[str]]] = None,
-        ) -> Callable[[], Tuple[Any, Dict[str, List[str]]]]:
-            return backend.websocket_auth(permissions)
-
-    return _AuthFief()
+from copy import deepcopy
+from uuid import uuid4
+from typing import Dict, List, Optional
+
+
+async def authenticate_client(http, port, permissions={}):
+    # create a new user
+    username = uuid4().hex
+    # if logged in, log out
+    first_time = True
+    while True:
+        response = await http.get(f"http://127.0.0.1:{port}/api/me")
+        if response.status_code == 403:
+            break
+        assert first_time
+        response = await http.post(f"http://127.0.0.1:{port}/auth/logout")
+        assert response.status_code == 200
+        first_time = False
+
+    # register user
+    register_body = {
+        "email": f"{username}@example.com",
+        "password": username,
+        "username": username,
+        "permissions": permissions,
+    }
+    response = await http.post(f"http://127.0.0.1:{port}/auth/register", json=register_body)
+    # check that we cannot register if not logged in
+    assert response.status_code == 403
+    # log in as admin
+    login_body = {"username": "admin@jupyter.com", "password": "jupyverse"}
+    response = await http.post(f"http://127.0.0.1:{port}/auth/login", data=login_body)
+    assert response.status_code == 204
+    # register user
+    response = await http.post(f"http://127.0.0.1:{port}/auth/register", json=register_body)
+    assert response.status_code == 201
+
+    # log out
+    response = await http.post(f"http://127.0.0.1:{port}/auth/logout")
+    assert response.status_code == 204
+    # check that we can't get our identity, since we're not logged in
+    response = await http.get(f"http://127.0.0.1:{port}/api/me")
+    assert response.status_code == 403
+
+    # log in with registered user
+    login_body = {"username": f"{username}@example.com", "password": username}
+    response = await http.post(f"http://127.0.0.1:{port}/auth/login", data=login_body)
+    assert response.status_code == 204
+    # we should now have a cookie
+    assert "fastapiusersauth" in http.cookies
+    # check our identity, since we're logged in
+    response = await http.get(
+        f"http://127.0.0.1:{port}/api/me", params={"permissions": permissions}
+    )
+    assert response.status_code == 200
+    me = response.json()
+    assert me["identity"]["username"] == username
+    # check our permissions
+    assert me["permissions"] == permissions
+
+
+def configure(components, config):
+    # TODO: generalize to arbitrary nested dictionaries, not just one level
+    _components = deepcopy(components)
+    for k1, v1 in config.items():
+        for k2, v2 in v1.items():
+            _components[k1][k2] = v2
+    return _components
+
+
+def create_content(
+    content: Optional[List],
+    type: str,
+    size: Optional[int],
+    mimetype: Optional[str],
+    name: str,
+    path: str,
+    format: Optional[str],
+) -> Dict:
+    return {
+        "content": content,
+        "created": None,
+        "format": format,
+        "last_modified": None,
+        "mimetype": mimetype,
+        "name": name,
+        "path": path,
+        "size": size,
+        "type": type,
+        "writable": True,
+    }
+
+
+def clear_content_values(content: Dict, keys: List[str] = []):
+    for k in content:
+        if k in keys:
+            content[k] = None
+        if k == "content" and isinstance(content[k], list):
+            for c in content[k]:
+                clear_content_values(c, keys)
+    return content
+
+
+def sort_content_by_name(content: Dict):
+    for k in content:
+        if k == "content" and isinstance(content[k], list):
+            # FIXME: this sorting algorithm is terrible!
+            names = [c["name"] for c in content[k]]
+            names.sort()
+            new_content = []
+            for name in names:
+                for i, c in enumerate(content[k]):
+                    if c["name"] == name:
+                        break
+                content[k].pop(i)
+                new_content.append(c)
+            content[k] = new_content
+            for c in content[k]:
+                sort_content_by_name(c)
+    return content
```

### Comparing `jupyverse-0.1.9/plugins/contents/COPYING.md` & `jupyverse-0.2.0/plugins/contents/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/contents/pyproject.toml` & `jupyverse-0.2.0/plugins/contents/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/contents/fps_contents/fileid.py` & `jupyverse-0.2.0/plugins/contents/fps_contents/fileid.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/contents/fps_contents/routes.py` & `jupyverse-0.2.0/plugins/contents/fps_contents/routes.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
     ) -> Content:
         if isinstance(path, str):
             path = Path(path)
         content: Optional[Union[str, Dict, List[Dict]]] = None
         if get_content:
             if path.is_dir():
                 content = [
-                    (await self.read_content(subpath, get_content=False)).dict()
+                    (await self.read_content(subpath, get_content=False)).model_dump()
                     for subpath in path.iterdir()
                     if not subpath.name.startswith(".")
                 ]
             elif path.is_file() or path.is_symlink():
                 try:
                     async with await open_file(path, mode="rb") as f:
                         content_bytes = await f.read()
```

### Comparing `jupyverse-0.1.9/plugins/frontend/COPYING.md` & `jupyverse-0.2.0/plugins/frontend/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/frontend/pyproject.toml` & `jupyverse-0.2.0/plugins/frontend/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/jupyterlab/COPYING.md` & `jupyverse-0.2.0/plugins/jupyterlab/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/jupyterlab/pyproject.toml` & `jupyverse-0.2.0/plugins/jupyterlab/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/jupyterlab/fps_jupyterlab/index.py` & `jupyverse-0.2.0/plugins/jupyterlab/fps_jupyterlab/index.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/jupyterlab/fps_jupyterlab/main.py` & `jupyverse-0.2.0/plugins/jupyterlab/fps_jupyterlab/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/jupyterlab/fps_jupyterlab/routes.py` & `jupyverse-0.2.0/plugins/jupyterlab/fps_jupyterlab/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/kernels/COPYING.md` & `jupyverse-0.2.0/plugins/kernels/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/kernels/pyproject.toml` & `jupyverse-0.2.0/plugins/kernels/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/kernels/fps_kernels/main.py` & `jupyverse-0.2.0/plugins/kernels/fps_kernels/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/kernels/fps_kernels/routes.py` & `jupyverse-0.2.0/plugins/kernels/fps_kernels/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/kernels/fps_kernels/kernel_driver/connect.py` & `jupyverse-0.2.0/plugins/kernels/fps_kernels/kernel_driver/connect.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/kernels/fps_kernels/kernel_driver/driver.py` & `jupyverse-0.2.0/plugins/kernels/fps_kernels/kernel_driver/driver.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py` & `jupyverse-0.2.0/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/kernels/fps_kernels/kernel_driver/message.py` & `jupyverse-0.2.0/plugins/kernels/fps_kernels/kernel_driver/message.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/kernels/fps_kernels/kernel_driver/paths.py` & `jupyverse-0.2.0/plugins/kernels/fps_kernels/kernel_driver/paths.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/kernels/fps_kernels/kernel_server/message.py` & `jupyverse-0.2.0/plugins/kernels/fps_kernels/kernel_server/message.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/kernels/fps_kernels/kernel_server/server.py` & `jupyverse-0.2.0/plugins/kernels/fps_kernels/kernel_server/server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/lab/COPYING.md` & `jupyverse-0.2.0/plugins/lab/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/lab/pyproject.toml` & `jupyverse-0.2.0/plugins/lab/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/lab/fps_lab/main.py` & `jupyverse-0.2.0/plugins/lab/fps_lab/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/lab/fps_lab/routes.py` & `jupyverse-0.2.0/plugins/lab/fps_lab/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/lab/fps_lab/static/favicon.ico` & `jupyverse-0.2.0/plugins/lab/fps_lab/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/login/COPYING.md` & `jupyverse-0.2.0/plugins/login/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/login/pyproject.toml` & `jupyverse-0.2.0/plugins/login/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/login/fps_login/routes.py` & `jupyverse-0.2.0/plugins/login/fps_login/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/login/fps_login/static/index.html` & `jupyverse-0.2.0/plugins/login/fps_login/static/index.html`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/login/fps_login/static/favicons/favicon-busy-1.ico` & `jupyverse-0.2.0/plugins/login/fps_login/static/favicons/favicon-busy-1.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/login/fps_login/static/favicons/favicon-busy-2.ico` & `jupyverse-0.2.0/plugins/login/fps_login/static/favicons/favicon-busy-2.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/login/fps_login/static/favicons/favicon-busy-3.ico` & `jupyverse-0.2.0/plugins/login/fps_login/static/favicons/favicon-busy-3.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/login/fps_login/static/favicons/favicon-file.ico` & `jupyverse-0.2.0/plugins/login/fps_login/static/favicons/favicon-file.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/login/fps_login/static/favicons/favicon-notebook.ico` & `jupyverse-0.2.0/plugins/login/fps_login/static/favicons/favicon-notebook.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/login/fps_login/static/favicons/favicon-terminal.ico` & `jupyverse-0.2.0/plugins/login/fps_login/static/favicons/favicon-terminal.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/login/fps_login/static/favicons/favicon.ico` & `jupyverse-0.2.0/plugins/login/fps_login/static/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/login/fps_login/static/logo/github.svg` & `jupyverse-0.2.0/plugins/login/fps_login/static/logo/github.svg`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/login/fps_login/static/logo/logo.png` & `jupyverse-0.2.0/plugins/login/fps_login/static/logo/logo.png`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/login/fps_login/static/style/index.css` & `jupyverse-0.2.0/plugins/login/fps_login/static/style/index.css`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/nbconvert/COPYING.md` & `jupyverse-0.2.0/plugins/nbconvert/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/nbconvert/pyproject.toml` & `jupyverse-0.2.0/plugins/nbconvert/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/nbconvert/fps_nbconvert/routes.py` & `jupyverse-0.2.0/plugins/nbconvert/fps_nbconvert/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/noauth/COPYING.md` & `jupyverse-0.2.0/plugins/noauth/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/noauth/pyproject.toml` & `jupyverse-0.2.0/plugins/noauth/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/noauth/fps_noauth/backends.py` & `jupyverse-0.2.0/plugins/noauth/fps_noauth/backends.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/resource_usage/COPYING.md` & `jupyverse-0.2.0/plugins/resource_usage/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/resource_usage/pyproject.toml` & `jupyverse-0.2.0/plugins/resource_usage/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/resource_usage/fps_resource_usage/main.py` & `jupyverse-0.2.0/plugins/resource_usage/fps_resource_usage/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/resource_usage/fps_resource_usage/routes.py` & `jupyverse-0.2.0/plugins/resource_usage/fps_resource_usage/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/retrolab/COPYING.md` & `jupyverse-0.2.0/plugins/retrolab/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/retrolab/pyproject.toml` & `jupyverse-0.2.0/plugins/retrolab/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/retrolab/fps_retrolab/main.py` & `jupyverse-0.2.0/plugins/retrolab/fps_retrolab/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/retrolab/fps_retrolab/routes.py` & `jupyverse-0.2.0/plugins/retrolab/fps_retrolab/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/terminals/COPYING.md` & `jupyverse-0.2.0/plugins/terminals/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/terminals/pyproject.toml` & `jupyverse-0.2.0/plugins/terminals/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/terminals/fps_terminals/main.py` & `jupyverse-0.2.0/plugins/terminals/fps_terminals/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/terminals/fps_terminals/routes.py` & `jupyverse-0.2.0/plugins/terminals/fps_terminals/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/terminals/fps_terminals/server.py` & `jupyverse-0.2.0/plugins/terminals/fps_terminals/server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/terminals/fps_terminals/win_server.py` & `jupyverse-0.2.0/plugins/terminals/fps_terminals/win_server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/webdav/COPYING.md` & `jupyverse-0.2.0/plugins/webdav/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/webdav/pyproject.toml` & `jupyverse-0.2.0/plugins/webdav/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/webdav/fps_webdav/routes.py` & `jupyverse-0.2.0/plugins/webdav/fps_webdav/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/webdav/tests/test_webdav.py` & `jupyverse-0.2.0/plugins/webdav/tests/test_webdav.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/yjs/COPYING.md` & `jupyverse-0.2.0/plugins/yjs/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/yjs/pyproject.toml` & `jupyverse-0.2.0/plugins/yjs/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "fps_yjs"
 description = "An FPS plugin for the Yjs API"
 keywords = [ "jupyter", "server", "fastapi", "plugins" ]
 requires-python = ">=3.8"
 dependencies = [
     "jupyter_ydoc >=1,<2",
-    "ypy-websocket >=0.8.2,<1",
+    "ypy-websocket >=0.12.1,<0.13.0",
     "y-py >=0.6.0,<0.7.0",
     "jupyverse-api >=0.1.2,<1",
 ]
 dynamic = [ "version",]
 [[project.authors]]
 name = "Jupyter Development Team"
 email = "jupyter@googlegroups.com"
```

### Comparing `jupyverse-0.1.9/plugins/yjs/fps_yjs/main.py` & `jupyverse-0.2.0/plugins/yjs/fps_yjs/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/plugins/yjs/fps_yjs/routes.py` & `jupyverse-0.2.0/plugins/yjs/fps_yjs/routes.py`

 * *Files 3% similar despite different names*

```diff
@@ -144,26 +144,28 @@
         self.contents = contents
         self.documents = {}  # a dictionary of room_name:document
         self.watchers = {}  # a dictionary of file_id:task
         self.savers = {}  # a dictionary of file_id:task
         self.cleaners = {}  # a dictionary of room:task
         self.last_modified = {}  # a dictionary of file_id:last_modification_date
         self.websocket_server = JupyterWebsocketServer(rooms_ready=False, auto_clean_rooms=False)
+        self.websocket_server_task = asyncio.create_task(self.websocket_server.start())
         self.lock = asyncio.Lock()
 
     def stop(self):
         for watcher in self.watchers.values():
             watcher.cancel()
         for saver in self.savers.values():
             saver.cancel()
         for cleaner in self.cleaners.values():
             cleaner.cancel()
+        self.websocket_server.stop()
 
     async def serve(self, websocket: YpyWebsocket, permissions) -> None:
-        room = self.websocket_server.get_room(websocket.path)
+        room = await self.websocket_server.get_room(websocket.path)
         can_write = permissions is None or "write" in permissions.get("yjs", [])
         room.on_message = partial(self.filter_message, can_write)
         is_stored_document = websocket.path.count(":") >= 2
         if is_stored_document:
             assert room.ystore is not None
             file_format, file_type, file_id = websocket.path.split(":", 2)
             if room in self.cleaners:
@@ -205,14 +207,15 @@
                     )
                     # update the document when file changes
                     if file_id not in self.watchers:
                         self.watchers[file_id] = asyncio.create_task(
                             self.watch_file(file_format, file_id, document)
                         )
 
+        await self.websocket_server.started.wait()
         await self.websocket_server.serve(websocket)
 
         if is_stored_document and not room.clients:
             # no client in this room after we disconnect
             self.cleaners[room] = asyncio.create_task(self.maybe_clean_room(room, websocket.path))
 
     async def filter_message(self, can_write: bool, message: bytes) -> bool:
@@ -350,19 +353,21 @@
         room_name = self.websocket_server.get_room_name(room)
         self.websocket_server.delete_room(room=room)
         file_path = await self.get_file_path(file_id, document)
         logger.info(f"Closing collaboration room: {room_name} ({file_path})")
 
 
 class JupyterWebsocketServer(WebsocketServer):
-    def get_room(self, ws_path: str) -> YRoom:
+    async def get_room(self, ws_path: str) -> YRoom:
         if ws_path not in self.rooms:
             if ws_path.count(":") >= 2:
                 # it is a stored document (e.g. a notebook)
                 file_format, file_type, file_id = ws_path.split(":", 2)
                 updates_file_path = f".{file_type}:{file_id}.y"
                 ystore = JupyterSQLiteYStore(path=updates_file_path)  # FIXME: pass in config
                 self.rooms[ws_path] = YRoom(ready=False, ystore=ystore)
             else:
                 # it is a transient document (e.g. awareness)
                 self.rooms[ws_path] = YRoom()
-        return self.rooms[ws_path]
+        room = self.rooms[ws_path]
+        await self.start_room(room)
+        return room
```

### Comparing `jupyverse-0.1.9/tests/conftest.py` & `jupyverse-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/tests/test_auth.py` & `jupyverse-0.2.0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/tests/test_contents.py` & `jupyverse-0.2.0/tests/test_contents.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/tests/test_kernels.py` & `jupyverse-0.2.0/tests/test_kernels.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/tests/test_server.py` & `jupyverse-0.2.0/tests/test_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,18 +75,19 @@
                 "format": "json",
                 "type": "notebook",
             }
         ),
     )
     file_id = response.json()["fileId"]
     document_id = f"json:notebook:{file_id}"
-    async with connect(f"{ws_url}/api/collaboration/room/{document_id}") as websocket:
+    ydoc = Y.YDoc()
+    async with connect(
+        f"{ws_url}/api/collaboration/room/{document_id}"
+    ) as websocket, WebsocketProvider(ydoc, websocket):
         # connect to the shared notebook document
-        ydoc = Y.YDoc()
-        WebsocketProvider(ydoc, websocket)
         # wait for file to be loaded and Y model to be created in server and client
         await asyncio.sleep(0.5)
         # execute notebook
         for cell_idx in range(3):
             response = requests.post(
                 f"{url}/api/kernels/{kernel_id}/execute",
                 data=json.dumps(
```

### Comparing `jupyverse-0.1.9/tests/test_settings.py` & `jupyverse-0.2.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/tests/data/notebook0.ipynb` & `jupyverse-0.2.0/tests/data/notebook0.ipynb`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/.gitignore` & `jupyverse-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/COPYING.md` & `jupyverse-0.2.0/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/README.md` & `jupyverse-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.9/pyproject.toml` & `jupyverse-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,16 @@
 auth-fief = ["fps-auth-fief >=0.1.2,<1"]
 noauth = ["fps-noauth >=0.1.2,<1"]
 test = [
     "mypy",
     "types-setuptools",
     "pytest",
     "pytest-asyncio",
+    "pytest-rerunfailures",
+    "pytest-timeout",
     "pytest-env",
     "httpx",
     "httpx-ws",
     "requests",
     "websockets",
     "ipykernel",
 ]
@@ -94,15 +96,15 @@
 ]
 
 [[tool.hatch.envs.dev.matrix]]
 frontend = ["jupyterlab", "retrolab"]
 auth = ["noauth", "auth", "auth_fief"]
 
 [tool.hatch.envs.dev.scripts]
-test = "pytest ./tests plugins/webdav/tests -v"
+test = "pytest ./tests plugins/webdav/tests -v --reruns 5 --timeout=60"
 lint = [
   "black --line-length 100 jupyverse ./plugins",
   "isort --profile=black jupyverse ./plugins",
 ]
 typecheck0 = """mypy --no-incremental \
 ./jupyverse_api \
 ./plugins/contents \
```

### Comparing `jupyverse-0.1.9/PKG-INFO` & `jupyverse-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyverse
-Version: 0.1.9
+Version: 0.2.0
 Summary: A set of FPS plugins implementing a Jupyter server
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
@@ -34,14 +34,16 @@
 Requires-Dist: httpx; extra == 'test'
 Requires-Dist: httpx-ws; extra == 'test'
 Requires-Dist: ipykernel; extra == 'test'
 Requires-Dist: mypy; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-asyncio; extra == 'test'
 Requires-Dist: pytest-env; extra == 'test'
+Requires-Dist: pytest-rerunfailures; extra == 'test'
+Requires-Dist: pytest-timeout; extra == 'test'
 Requires-Dist: requests; extra == 'test'
 Requires-Dist: types-setuptools; extra == 'test'
 Requires-Dist: websockets; extra == 'test'
 Description-Content-Type: text/markdown
 
 [![Build Status](https://github.com/jupyter-server/jupyverse/workflows/CI/badge.svg)](https://github.com/jupyter-server/jupyverse/actions)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

